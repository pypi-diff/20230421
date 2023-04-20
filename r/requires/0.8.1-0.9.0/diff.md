# Comparing `tmp/requires-0.8.1.tar.gz` & `tmp/requires-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requires-0.8.1.tar", max compression
+gzip compressed data, was "requires-0.9.0.tar", max compression
```

## Comparing `requires-0.8.1.tar` & `requires-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1056 2020-09-04 20:39:06.089407 requires-0.8.1/LICENSE
--rw-r--r--   0        0        0     1782 2021-02-18 01:04:43.137746 requires-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      419 2021-02-18 01:00:43.958895 requires-0.8.1/requires/__init__.py
--rw-r--r--   0        0        0      188 2021-02-18 01:04:56.409823 requires-0.8.1/requires/_meta.py
--rw-r--r--   0        0        0    11034 2021-02-18 01:32:42.128318 requires-0.8.1/requires/core.py
--rw-r--r--   0        0        0        0 2020-09-04 20:39:06.148406 requires-0.8.1/requires/py.typed
--rw-r--r--   0        0        0     2335 2021-02-18 01:00:13.011310 requires-0.8.1/requires/shed.py
--rw-r--r--   0        0        0      725 2021-02-18 01:36:35.900881 requires-0.8.1/setup.py
--rw-r--r--   0        0        0      994 2021-02-18 01:36:35.900881 requires-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2020-09-04 20:39:06.089407 requires-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1113 2021-02-26 18:35:42.597041 requires-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      483 2021-02-26 19:21:14.964552 requires-0.9.0/requires/__init__.py
+-rw-r--r--   0        0        0      188 2021-02-26 18:35:49.098291 requires-0.9.0/requires/_meta.py
+-rw-r--r--   0        0        0    11317 2021-02-26 19:33:31.896464 requires-0.9.0/requires/core.py
+-rw-r--r--   0        0        0        0 2020-09-04 20:39:06.148406 requires-0.9.0/requires/py.typed
+-rw-r--r--   0        0        0     2335 2021-02-18 01:00:13.011310 requires-0.9.0/requires/shed.py
+-rw-r--r--   0        0        0      725 2021-02-26 19:51:43.812084 requires-0.9.0/setup.py
+-rw-r--r--   0        0        0      994 2021-02-26 19:51:43.812084 requires-0.9.0/PKG-INFO
```

### Comparing `requires-0.8.1/LICENSE` & `requires-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `requires-0.8.1/pyproject.toml` & `requires-0.9.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "requires"
-version = "0.8.1"
+version = "0.9.0"
 description = "Require and import dependencies at runtime"
 license = "MIT"
 authors = ["jesse <jesse@dgi.com>"]
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 packages = [
     { include = "requires", from = "." },
 ]
@@ -29,30 +29,10 @@
 python = "==3.*,>=3.6.1"
 funkify = "^0.3.0"
 dataclasses = {version = "*", python = "~3.6.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "==5.*,>=5.3.0"
 
-[tool.dephell.main]
-from = {format = "poetry", path = "pyproject.toml"}
-to = {format = "setuppy", path = "setup.py"}
-# explicitly specify your versioning scheme to let your users know what they can expect
-versioning = "semver"
-# git tag template for releases
-tag = "v"
-
-[tool.dephell.vendorized]
-from = {format = "poetry", path = "pyproject.toml"}
-to = {format = "wheel", path = "dist-vendored/"}
-envs = ["main"]
-
-# Make vendorized version of the project:
-# dephell vendor download --env=vendorized
-# dephell vendor import --env=vendorized
-[tool.dephell.vendorized.vendor]
-path = "dephell_vendor"
-exclude = ["jinja2", "tests", "setuptools", "pip"]
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `requires-0.8.1/requires/core.py` & `requires-0.9.0/requires/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,26 @@
 
 def _fn_globals(f: Any) -> Any:
     if hasattr(f, "__wrapped__"):
         return _fn_globals(f.__wrapped__)
     return f.__globals__
 
 
-class RequirementError(Exception):
+class RequirementError(ModuleNotFoundError):
     """Exception for requries"""
 
     pass
 
 
+class RequirementAttributeError(AttributeError):
+    """Requirement attribute error"""
+
+    pass
+
+
 @dataclass
 class Requirement:
     _import: str
     _from: Optional[str] = None
     _as: Optional[str] = None
     pip: Optional[Union[str, bool]] = None
     conda: Optional[Union[str, bool]] = None
@@ -119,18 +125,19 @@
 
     def import_requirement(self) -> Any:
         """Import and return the requirement"""
         try:
             if self._from is None:
                 return import_module(self._import)
             req = import_module(self._from)
+            # Import ok BUT the attr/thing imported from the module does not exist
             try:
                 return getattr(req, self._import)
             except AttributeError as ae:
-                raise RequirementError(
+                raise RequirementAttributeError(
                     "\n".join(
                         [
                             f"Module/Package(s) import AttributeError: `{self.import_string}`",
                             f"    AttributeError: {str(ae)}",
                         ]
                     )
                 )
@@ -293,14 +300,15 @@
     *requirements: Union[str, Dict[str, str], Requirement],
     _import: Optional[str] = None,
     _as: Optional[str] = None,
     _from: Optional[str] = None,
     pip: Optional[Union[str, bool]] = None,
     conda: Optional[Union[str, bool]] = None,
     conda_forge: Optional[Union[str, bool]] = None,
+    details: Optional[str] = None,
 ) -> Callable[[Callable[..., T]], Callable[..., T]]:
     """Decorator to specify the packages a function or class requires
 
     The decorator will not do anything unless a NameError is thrown. If a
     NameError is thrown then the required package is likely not installed and
     a `RequirementError` will be thrown with instructions on how to install
     the required packages.
@@ -321,17 +329,19 @@
             Requirement(
                 _import=str(_import),
                 _from=_from,
                 _as=_as,
                 pip=pip,
                 conda=conda,
                 conda_forge=conda_forge,
+                details=details,
             )
         ]
-    _requirements = make_requirements(list(requirements))
+    else:
+        _requirements = make_requirements(list(requirements))
 
     def _requires_dec(f: Callable[..., T]) -> Callable[..., T]:
         _wrapped_fn = f
         for el in _requirements:
             _wrapped_fn = el(_wrapped_fn)
         wraps(f)(_wrapped_fn)
         return _wrapped_fn
```

### Comparing `requires-0.8.1/requires/shed.py` & `requires-0.9.0/requires/shed.py`

 * *Files identical despite different names*

### Comparing `requires-0.8.1/setup.py` & `requires-0.9.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['funkify>=0.3.0,<0.4.0']
 
 setup_kwargs = {
     'name': 'requires',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': 'Require and import dependencies at runtime',
     'long_description': None,
     'author': 'jesse',
     'author_email': 'jesse@dgi.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/dynamic-graphics-inc/dgpy-libs',
```

### Comparing `requires-0.8.1/PKG-INFO` & `requires-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requires
-Version: 0.8.1
+Version: 0.9.0
 Summary: Require and import dependencies at runtime
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs
 License: MIT
 Keywords: requires,dgpy,python,modules,funkified,import,dependencies,lazy
 Author: jesse
 Author-email: jesse@dgi.com
 Requires-Python: >=3.6.1,<4.0.0
```

