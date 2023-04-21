# Comparing `tmp/mybox-0.7.7.tar.gz` & `tmp/mybox-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mybox-0.7.7.tar", max compression
+gzip compressed data, was "mybox-0.7.8.tar", max compression
```

## Comparing `mybox-0.7.7.tar` & `mybox-0.7.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    34916 2023-04-01 03:33:16.181371 mybox-0.7.7/LICENSE.md
--rw-r--r--   0        0        0     1449 2023-04-01 03:33:16.181371 mybox-0.7.7/README.md
--rw-r--r--   0        0        0        0 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/__init__.py
--rw-r--r--   0        0        0     2558 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/compute.py
--rw-r--r--   0        0        0      932 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/configparser.py
--rw-r--r--   0        0        0     9803 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/driver.py
--rw-r--r--   0        0        0     2406 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/filters.py
--rw-r--r--   0        0        0     1281 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/main.py
--rw-r--r--   0        0        0     3198 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/manager.py
--rw-r--r--   0        0        0     1135 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/__init__.py
--rw-r--r--   0        0        0     6797 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/archive.py
--rw-r--r--   0        0        0     2047 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/base.py
--rw-r--r--   0        0        0     2032 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/clone.py
--rw-r--r--   0        0        0      339 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/destination.py
--rw-r--r--   0        0        0     3330 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/github.py
--rw-r--r--   0        0        0     8997 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/installer.py
--rw-r--r--   0        0        0     1985 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/links.py
--rw-r--r--   0        0        0     4788 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/manual.py
--rw-r--r--   0        0        0      792 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/manual_version.py
--rw-r--r--   0        0        0     1567 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/npm.py
--rw-r--r--   0        0        0      907 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/pip.py
--rw-r--r--   0        0        0     1577 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/pip_base.py
--rw-r--r--   0        0        0      931 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/pipx.py
--rw-r--r--   0        0        0      500 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/root.py
--rw-r--r--   0        0        0     1794 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/shell.py
--rw-r--r--   0        0        0     2347 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/system.py
--rw-r--r--   0        0        0     1402 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/tracked.py
--rw-r--r--   0        0        0      621 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/url.py
--rw-r--r--   0        0        0     1634 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/package/yum_repo.py
--rw-r--r--   0        0        0     2602 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/parallel.py
--rw-r--r--   0        0        0      141 2023-04-01 03:33:16.181371 mybox-0.7.7/mybox/state/__init__.py
--rw-r--r--   0        0        0     4142 2023-04-01 03:33:16.185371 mybox-0.7.7/mybox/state/base.py
--rw-r--r--   0        0        0      315 2023-04-01 03:33:16.185371 mybox-0.7.7/mybox/state/installed.py
--rw-r--r--   0        0        0      160 2023-04-01 03:33:16.185371 mybox-0.7.7/mybox/state/version.py
--rw-r--r--   0        0        0     3626 2023-04-01 03:33:16.185371 mybox-0.7.7/mybox/utils.py
--rw-r--r--   0        0        0     2120 2023-04-01 03:33:31.605562 mybox-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 mybox-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-04-21 00:05:38.974069 mybox-0.7.8/LICENSE.md
+-rw-r--r--   0        0        0     1463 2023-04-21 00:05:38.974069 mybox-0.7.8/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/__init__.py
+-rw-r--r--   0        0        0     2558 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/compute.py
+-rw-r--r--   0        0        0      932 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/configparser.py
+-rw-r--r--   0        0        0     9803 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/driver.py
+-rw-r--r--   0        0        0     2406 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/filters.py
+-rw-r--r--   0        0        0     1281 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/main.py
+-rw-r--r--   0        0        0     3198 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/manager.py
+-rw-r--r--   0        0        0     1135 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/package/__init__.py
+-rw-r--r--   0        0        0     6797 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/package/archive.py
+-rw-r--r--   0        0        0     2047 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/package/base.py
+-rw-r--r--   0        0        0     2018 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/package/clone.py
+-rw-r--r--   0        0        0      339 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/package/destination.py
+-rw-r--r--   0        0        0     3330 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/package/github.py
+-rw-r--r--   0        0        0     8997 2023-04-21 00:05:38.974069 mybox-0.7.8/mybox/package/installer.py
+-rw-r--r--   0        0        0     1985 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/links.py
+-rw-r--r--   0        0        0     4788 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/manual.py
+-rw-r--r--   0        0        0      792 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/manual_version.py
+-rw-r--r--   0        0        0     1567 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/npm.py
+-rw-r--r--   0        0        0      907 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/pip.py
+-rw-r--r--   0        0        0     1577 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/pip_base.py
+-rw-r--r--   0        0        0      931 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/pipx.py
+-rw-r--r--   0        0        0      500 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/root.py
+-rw-r--r--   0        0        0     1794 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/shell.py
+-rw-r--r--   0        0        0     2347 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/system.py
+-rw-r--r--   0        0        0     1402 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/tracked.py
+-rw-r--r--   0        0        0      621 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/url.py
+-rw-r--r--   0        0        0     1634 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/package/yum_repo.py
+-rw-r--r--   0        0        0     2602 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/parallel.py
+-rw-r--r--   0        0        0      141 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/state/__init__.py
+-rw-r--r--   0        0        0     4142 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/state/base.py
+-rw-r--r--   0        0        0      315 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/state/installed.py
+-rw-r--r--   0        0        0      160 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/state/version.py
+-rw-r--r--   0        0        0     3626 2023-04-21 00:05:38.978069 mybox-0.7.8/mybox/utils.py
+-rw-r--r--   0        0        0     2120 2023-04-21 00:06:00.114082 mybox-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0     2495 1970-01-01 00:00:00.000000 mybox-0.7.8/PKG-INFO
```

### Comparing `mybox-0.7.7/LICENSE.md` & `mybox-0.7.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/README.md` & `mybox-0.7.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 * [Poetry](https://python-poetry.org/)
 * [ShellCheck](https://www.shellcheck.net/)
 
 Run [`./lint`](lint) to check style & types, `./lint --format` to apply
 formatting automatically.
 
-Run [`./test`](test) to execute the project's tests.
+Run [`./test-script`](test-script) to execute the project's tests.
 
 ### Running locally
 
 * Run `poetry install`.
 * Run `poetry shell`.
 * In the launched shell, go to the directory with package definitions.
 * Run `mybox` with the desired arguments.
```

### Comparing `mybox-0.7.7/mybox/compute.py` & `mybox-0.7.8/mybox/compute.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/configparser.py` & `mybox-0.7.8/mybox/configparser.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/driver.py` & `mybox-0.7.8/mybox/driver.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/filters.py` & `mybox-0.7.8/mybox/filters.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/main.py` & `mybox-0.7.8/mybox/main.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/manager.py` & `mybox-0.7.8/mybox/manager.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/__init__.py` & `mybox-0.7.8/mybox/package/__init__.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/archive.py` & `mybox-0.7.8/mybox/package/archive.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/base.py` & `mybox-0.7.8/mybox/package/base.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/clone.py` & `mybox-0.7.8/mybox/package/clone.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     repo: str = Field(..., alias="clone")
 
     @property
     def name(self) -> str:
         return self.repo
 
     async def directory_exists(self) -> bool:
-        return await self.driver.run_ok("test", "-d", await self.destination())
+        return await self.driver.is_dir(await self.destination())
 
     @async_cached
     async def git_args(self) -> list[RunArg]:
         return ["git", "-C", await self.destination()]
 
     async def run_git(self, *args: RunArg) -> None:
         await self.driver.run(*await self.git_args(), *args)
```

### Comparing `mybox-0.7.7/mybox/package/github.py` & `mybox-0.7.8/mybox/package/github.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/installer.py` & `mybox-0.7.8/mybox/package/installer.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         return all packages' versions.
         """
         args = [
             "dnf",
             "--quiet",
             "repoquery",
             "--queryformat",
-            "%{NAME} %{VERSION}",
+            "%{name} %{version}",
             "--latest-limit",
             "1",
             "--arch",
             "x86_64,noarch",
         ]
 
         if package:
```

### Comparing `mybox-0.7.7/mybox/package/links.py` & `mybox-0.7.8/mybox/package/links.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/manual.py` & `mybox-0.7.8/mybox/package/manual.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/manual_version.py` & `mybox-0.7.8/mybox/package/manual_version.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/npm.py` & `mybox-0.7.8/mybox/package/npm.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/pip.py` & `mybox-0.7.8/mybox/package/pip.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/pip_base.py` & `mybox-0.7.8/mybox/package/pip_base.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/pipx.py` & `mybox-0.7.8/mybox/package/pipx.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/shell.py` & `mybox-0.7.8/mybox/package/shell.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/system.py` & `mybox-0.7.8/mybox/package/system.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/tracked.py` & `mybox-0.7.8/mybox/package/tracked.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/url.py` & `mybox-0.7.8/mybox/package/url.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/package/yum_repo.py` & `mybox-0.7.8/mybox/package/yum_repo.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/parallel.py` & `mybox-0.7.8/mybox/parallel.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/state/base.py` & `mybox-0.7.8/mybox/state/base.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/mybox/utils.py` & `mybox-0.7.8/mybox/utils.py`

 * *Files identical despite different names*

### Comparing `mybox-0.7.7/pyproject.toml` & `mybox-0.7.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mybox"
-version = "v0.7.7"
+version = "v0.7.8"
 description = "Manage the configuration and tools on your workstation without bothering the OS too much"
 readme = "README.md"
 repository = "https://github.com/koterpillar/mybox"
 authors = ["Alexey Kotlyarov <a@koterpillar.com>"]
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
```

### Comparing `mybox-0.7.7/PKG-INFO` & `mybox-0.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mybox
-Version: 0.7.7
+Version: 0.7.8
 Summary: Manage the configuration and tools on your workstation without bothering the OS too much
 Home-page: https://github.com/koterpillar/mybox
 License: GPL-3.0-or-later
 Author: Alexey Kotlyarov
 Author-email: a@koterpillar.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -59,15 +59,15 @@
 
 * [Poetry](https://python-poetry.org/)
 * [ShellCheck](https://www.shellcheck.net/)
 
 Run [`./lint`](lint) to check style & types, `./lint --format` to apply
 formatting automatically.
 
-Run [`./test`](test) to execute the project's tests.
+Run [`./test-script`](test-script) to execute the project's tests.
 
 ### Running locally
 
 * Run `poetry install`.
 * Run `poetry shell`.
 * In the launched shell, go to the directory with package definitions.
 * Run `mybox` with the desired arguments.
```

