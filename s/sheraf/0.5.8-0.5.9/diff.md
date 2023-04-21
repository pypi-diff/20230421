# Comparing `tmp/sheraf-0.5.8.tar.gz` & `tmp/sheraf-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheraf-0.5.8.tar", max compression
+gzip compressed data, was "sheraf-0.5.9.tar", max compression
```

## Comparing `sheraf-0.5.8.tar` & `sheraf-0.5.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1051 2020-02-14 10:22:37.639183 sheraf-0.5.8/LICENSE.md
--rw-r--r--   0        0        0     1500 2021-02-18 09:16:42.723796 sheraf-0.5.8/README.md
--rw-r--r--   0        0        0     3215 2021-07-26 10:05:35.484413 sheraf-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     2206 2021-07-06 07:30:17.706341 sheraf-0.5.8/sheraf/__init__.py
--rw-r--r--   0        0        0    14510 2021-07-26 09:41:50.960911 sheraf-0.5.8/sheraf/attributes/__init__.py
--rw-r--r--   0        0        0     3583 2021-07-06 07:33:51.185733 sheraf-0.5.8/sheraf/attributes/blobs.py
--rw-r--r--   0        0        0    19002 2021-07-26 09:41:50.960911 sheraf-0.5.8/sheraf/attributes/collections.py
--rw-r--r--   0        0        0     4202 2021-07-26 09:41:50.960911 sheraf-0.5.8/sheraf/attributes/counter.py
--rw-r--r--   0        0        0     3039 2021-07-02 12:24:03.489217 sheraf-0.5.8/sheraf/attributes/enum.py
--rw-r--r--   0        0        0     6132 2021-07-06 07:35:00.192203 sheraf-0.5.8/sheraf/attributes/files.py
--rw-r--r--   0        0        0    12013 2021-07-26 09:41:50.960911 sheraf-0.5.8/sheraf/attributes/index.py
--rw-r--r--   0        0        0    16759 2021-07-26 09:41:50.960911 sheraf-0.5.8/sheraf/attributes/models.py
--rw-r--r--   0        0        0     1799 2021-05-04 08:33:17.397607 sheraf-0.5.8/sheraf/attributes/password.py
--rw-r--r--   0        0        0     3983 2021-07-26 09:41:50.960911 sheraf-0.5.8/sheraf/attributes/simples.py
--rw-r--r--   0        0        0      780 2021-07-02 12:19:29.959878 sheraf-0.5.8/sheraf/cli.py
--rw-r--r--   0        0        0      915 2020-02-24 11:44:32.404074 sheraf-0.5.8/sheraf/conftest.py
--rw-r--r--   0        0        0       17 2020-02-24 11:44:32.427408 sheraf-0.5.8/sheraf/constants.py
--rw-r--r--   0        0        0    13191 2021-07-26 09:41:50.960911 sheraf-0.5.8/sheraf/databases.py
--rw-r--r--   0        0        0     7989 2021-07-26 09:48:09.497137 sheraf-0.5.8/sheraf/exceptions.py
--rw-r--r--   0        0        0    10319 2021-07-02 12:19:29.959878 sheraf-0.5.8/sheraf/health/__init__.py
--rw-r--r--   0        0        0     3606 2021-07-26 09:41:50.960911 sheraf-0.5.8/sheraf/health/checks.py
--rw-r--r--   0        0        0       62 2021-02-05 13:36:20.196497 sheraf-0.5.8/sheraf/health/fixes.py
--rw-r--r--   0        0        0     2044 2021-07-05 12:48:15.463175 sheraf-0.5.8/sheraf/health/utils.py
--rw-r--r--   0        0        0     2828 2021-04-06 07:50:46.962034 sheraf-0.5.8/sheraf/models/__init__.py
--rw-r--r--   0        0        0     2656 2021-02-26 10:01:15.253989 sheraf-0.5.8/sheraf/models/attributes.py
--rw-r--r--   0        0        0    12344 2021-07-06 07:34:37.902266 sheraf-0.5.8/sheraf/models/base.py
--rw-r--r--   0        0        0    28245 2021-07-26 09:41:50.960911 sheraf-0.5.8/sheraf/models/indexation.py
--rw-r--r--   0        0        0     9399 2021-07-26 09:41:50.960911 sheraf-0.5.8/sheraf/models/indexmanager.py
--rw-r--r--   0        0        0     2828 2021-02-23 09:49:23.250208 sheraf-0.5.8/sheraf/models/inline.py
--rw-r--r--   0        0        0    22927 2021-07-26 09:41:50.960911 sheraf-0.5.8/sheraf/queryset.py
--rw-r--r--   0        0        0        0 2020-02-24 11:44:32.430741 sheraf-0.5.8/sheraf/tools/__init__.py
--rw-r--r--   0        0        0     1501 2021-01-19 13:34:26.162172 sheraf-0.5.8/sheraf/tools/dicttools.py
--rw-r--r--   0        0        0      727 2020-07-29 08:02:56.155340 sheraf-0.5.8/sheraf/tools/more_itertools.py
--rw-r--r--   0        0        0     5584 2021-07-26 09:46:08.223924 sheraf-0.5.8/sheraf/transactions.py
--rw-r--r--   0        0        0     1012 2020-10-14 08:13:19.747314 sheraf-0.5.8/sheraf/types/__init__.py
--rw-r--r--   0        0        0     4456 2020-02-25 11:12:53.820653 sheraf-0.5.8/sheraf/types/counter.py
--rw-r--r--   0        0        0     1883 2020-07-29 08:02:56.155340 sheraf-0.5.8/sheraf/types/largedict.py
--rw-r--r--   0        0        0     4349 2021-05-04 08:33:17.397607 sheraf-0.5.8/sheraf/types/largelist.py
--rw-r--r--   0        0        0       80 2021-07-26 10:05:48.191054 sheraf-0.5.8/sheraf/version.py
--rw-r--r--   0        0        0     2738 2021-07-26 10:09:19.059632 sheraf-0.5.8/setup.py
--rw-r--r--   0        0        0     3177 2021-07-26 10:09:19.059945 sheraf-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1051 2020-02-23 14:36:34.668830 sheraf-0.5.9/LICENSE.md
+-rw-r--r--   0        0        0     1500 2021-02-17 22:46:37.675507 sheraf-0.5.9/README.md
+-rw-r--r--   0        0        0     3215 2021-07-28 09:16:13.844557 sheraf-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     2206 2021-07-16 07:12:23.736667 sheraf-0.5.9/sheraf/__init__.py
+-rw-r--r--   0        0        0    15026 2021-07-28 09:14:22.738341 sheraf-0.5.9/sheraf/attributes/__init__.py
+-rw-r--r--   0        0        0     3583 2021-07-16 07:12:23.736667 sheraf-0.5.9/sheraf/attributes/blobs.py
+-rw-r--r--   0        0        0    19002 2021-07-16 07:58:32.898892 sheraf-0.5.9/sheraf/attributes/collections.py
+-rw-r--r--   0        0        0     4202 2021-07-16 07:58:32.902225 sheraf-0.5.9/sheraf/attributes/counter.py
+-rw-r--r--   0        0        0     3039 2021-07-16 07:12:23.736667 sheraf-0.5.9/sheraf/attributes/enum.py
+-rw-r--r--   0        0        0     6132 2021-07-16 07:12:23.736667 sheraf-0.5.9/sheraf/attributes/files.py
+-rw-r--r--   0        0        0    12013 2021-07-16 07:58:32.902225 sheraf-0.5.9/sheraf/attributes/index.py
+-rw-r--r--   0        0        0    16759 2021-07-16 07:58:32.902225 sheraf-0.5.9/sheraf/attributes/models.py
+-rw-r--r--   0        0        0     1799 2021-07-16 07:12:23.736667 sheraf-0.5.9/sheraf/attributes/password.py
+-rw-r--r--   0        0        0     3983 2021-07-16 07:58:32.902225 sheraf-0.5.9/sheraf/attributes/simples.py
+-rw-r--r--   0        0        0      780 2021-07-04 10:33:56.216832 sheraf-0.5.9/sheraf/cli.py
+-rw-r--r--   0        0        0      915 2021-02-14 21:19:52.734794 sheraf-0.5.9/sheraf/conftest.py
+-rw-r--r--   0        0        0       17 2021-02-14 21:19:52.724794 sheraf-0.5.9/sheraf/constants.py
+-rw-r--r--   0        0        0    13191 2021-07-16 07:58:32.902225 sheraf-0.5.9/sheraf/databases.py
+-rw-r--r--   0        0        0     7989 2021-07-28 09:14:22.738341 sheraf-0.5.9/sheraf/exceptions.py
+-rw-r--r--   0        0        0    10319 2021-05-04 18:28:15.172546 sheraf-0.5.9/sheraf/health/__init__.py
+-rw-r--r--   0        0        0     3606 2021-07-16 07:58:32.902225 sheraf-0.5.9/sheraf/health/checks.py
+-rw-r--r--   0        0        0       62 2021-02-14 21:19:52.728128 sheraf-0.5.9/sheraf/health/fixes.py
+-rw-r--r--   0        0        0     2044 2021-07-04 10:33:56.216832 sheraf-0.5.9/sheraf/health/utils.py
+-rw-r--r--   0        0        0     2828 2021-07-16 07:12:23.736667 sheraf-0.5.9/sheraf/models/__init__.py
+-rw-r--r--   0        0        0     2656 2021-07-16 07:12:23.736667 sheraf-0.5.9/sheraf/models/attributes.py
+-rw-r--r--   0        0        0    12344 2021-07-16 07:12:23.736667 sheraf-0.5.9/sheraf/models/base.py
+-rw-r--r--   0        0        0    28245 2021-07-16 07:58:32.902225 sheraf-0.5.9/sheraf/models/indexation.py
+-rw-r--r--   0        0        0     9399 2021-07-16 07:58:32.902225 sheraf-0.5.9/sheraf/models/indexmanager.py
+-rw-r--r--   0        0        0     2828 2021-02-19 20:26:53.237443 sheraf-0.5.9/sheraf/models/inline.py
+-rw-r--r--   0        0        0    22927 2021-07-16 07:58:32.902225 sheraf-0.5.9/sheraf/queryset.py
+-rw-r--r--   0        0        0        0 2021-02-14 21:19:52.734794 sheraf-0.5.9/sheraf/tools/__init__.py
+-rw-r--r--   0        0        0     1501 2021-02-14 21:19:52.734794 sheraf-0.5.9/sheraf/tools/dicttools.py
+-rw-r--r--   0        0        0      727 2021-02-14 21:19:52.734794 sheraf-0.5.9/sheraf/tools/more_itertools.py
+-rw-r--r--   0        0        0     5584 2021-07-28 09:14:22.738341 sheraf-0.5.9/sheraf/transactions.py
+-rw-r--r--   0        0        0     1012 2021-07-16 07:12:23.740001 sheraf-0.5.9/sheraf/types/__init__.py
+-rw-r--r--   0        0        0     4456 2021-07-16 07:12:23.740001 sheraf-0.5.9/sheraf/types/counter.py
+-rw-r--r--   0        0        0     1883 2021-07-16 07:12:23.740001 sheraf-0.5.9/sheraf/types/largedict.py
+-rw-r--r--   0        0        0     4349 2021-07-16 07:12:23.740001 sheraf-0.5.9/sheraf/types/largelist.py
+-rw-r--r--   0        0        0       80 2021-07-28 09:16:18.154540 sheraf-0.5.9/sheraf/version.py
+-rw-r--r--   0        0        0     2738 2021-07-28 09:16:29.995288 sheraf-0.5.9/setup.py
+-rw-r--r--   0        0        0     3177 2021-07-28 09:16:29.995563 sheraf-0.5.9/PKG-INFO
```

### Comparing `sheraf-0.5.8/LICENSE.md` & `sheraf-0.5.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/README.md` & `sheraf-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/pyproject.toml` & `sheraf-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry>=1.0.0"]
 build-backend = "poetry.masonry.api"
 
 [tool]
 [tool.poetry]
 name = "sheraf"
-version = "0.5.8"
+version = "0.5.9"
 description = "Versatile ZODB abstraction layer"
 license = "MIT"
 keywords = ["zodb", "orm"]
 classifiers = [
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
```

### Comparing `sheraf-0.5.8/sheraf/__init__.py` & `sheraf-0.5.9/sheraf/__init__.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/attributes/__init__.py` & `sheraf-0.5.9/sheraf/attributes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,14 +378,30 @@
 
         def wrapper(func):
             self.cb_deletion.append(func)
             return func
 
         return wrapper if not args else wrapper(args[0])
 
+    def on_change(self, *args, **kwargs):
+        """
+        Shortcut for :meth:`~sheraf.attributes.Attribute.on_creation`,
+        :meth:`~sheraf.attributes.Attribute.on_edition`
+        and :meth:`~sheraf.attributes.Attribute.on_deletion` at the
+        same time.
+        """
+
+        def wrapper(func):
+            self.cb_creation.append(func)
+            self.cb_edition.append(func)
+            self.cb_deletion.append(func)
+            return func
+
+        return wrapper if not args else wrapper(args[0])
+
     def default(self, func):
         """
         Decorator for a callback to call to generate a default value for
         the attribute.
 
         >>> class Cowboy(sheraf.Model):
         ...     table = "default_cowboys"
```

### Comparing `sheraf-0.5.8/sheraf/attributes/blobs.py` & `sheraf-0.5.9/sheraf/attributes/blobs.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/attributes/collections.py` & `sheraf-0.5.9/sheraf/attributes/collections.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/attributes/counter.py` & `sheraf-0.5.9/sheraf/attributes/counter.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/attributes/enum.py` & `sheraf-0.5.9/sheraf/attributes/enum.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/attributes/files.py` & `sheraf-0.5.9/sheraf/attributes/files.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/attributes/index.py` & `sheraf-0.5.9/sheraf/attributes/index.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/attributes/models.py` & `sheraf-0.5.9/sheraf/attributes/models.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/attributes/password.py` & `sheraf-0.5.9/sheraf/attributes/password.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/attributes/simples.py` & `sheraf-0.5.9/sheraf/attributes/simples.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/cli.py` & `sheraf-0.5.9/sheraf/cli.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/conftest.py` & `sheraf-0.5.9/sheraf/conftest.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/databases.py` & `sheraf-0.5.9/sheraf/databases.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/exceptions.py` & `sheraf-0.5.9/sheraf/exceptions.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/health/__init__.py` & `sheraf-0.5.9/sheraf/health/__init__.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/health/checks.py` & `sheraf-0.5.9/sheraf/health/checks.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/health/utils.py` & `sheraf-0.5.9/sheraf/health/utils.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/models/__init__.py` & `sheraf-0.5.9/sheraf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/models/attributes.py` & `sheraf-0.5.9/sheraf/models/attributes.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/models/base.py` & `sheraf-0.5.9/sheraf/models/base.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/models/indexation.py` & `sheraf-0.5.9/sheraf/models/indexation.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/models/indexmanager.py` & `sheraf-0.5.9/sheraf/models/indexmanager.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/models/inline.py` & `sheraf-0.5.9/sheraf/models/inline.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/queryset.py` & `sheraf-0.5.9/sheraf/queryset.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/tools/dicttools.py` & `sheraf-0.5.9/sheraf/tools/dicttools.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/tools/more_itertools.py` & `sheraf-0.5.9/sheraf/tools/more_itertools.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/transactions.py` & `sheraf-0.5.9/sheraf/transactions.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/types/__init__.py` & `sheraf-0.5.9/sheraf/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/types/counter.py` & `sheraf-0.5.9/sheraf/types/counter.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/types/largedict.py` & `sheraf-0.5.9/sheraf/types/largedict.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/sheraf/types/largelist.py` & `sheraf-0.5.9/sheraf/types/largelist.py`

 * *Files identical despite different names*

### Comparing `sheraf-0.5.8/setup.py` & `sheraf-0.5.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'zeo': ['zeo']}
 
 entry_points = \
 {'console_scripts': ['sheraf = sheraf.cli:cli']}
 
 setup_kwargs = {
     'name': 'sheraf',
-    'version': '0.5.8',
+    'version': '0.5.9',
     'description': 'Versatile ZODB abstraction layer',
     'long_description': '# A versatile ZODB abstraction layer\n\nsheraf is a wrapper library around [ZODB](https://www.zodb.org) that provides models management and indexation. It aims to make the use of `ZODB` simple by providing ready-to-use tools and explicit tools. sheraf is currently compatible with `ZODB 5` and `python 3.6+`.\n\nYou can expect sheraf to:\n\n- Do few things, but do them right;\n- Be simple enough so beginners can do a lot with a few lines;\n- Be powerful enough and tunable for python experts;\n- Have a simple and expressive code, that allows you to hack it if needed.\n\n## Installation\n\nsheraf is compatible with Python 3.6+\n\n    poetry add sheraf\n    # or\n    pip install sheraf\n\nIf you need pytest fixtures for your project check out [pytest-sheraf](https://gitlab.com/yaal/pytest-sheraf). There are also [sheraf fixtures for unittest](https://gitlab.com/yaal/unittest-sheraf).\n\n    pip install pytest-sheraf\n\n## Contributing\n\nBug reports and pull requests are highly encouraged!\n\n - Test some code : `poetry run pytest` and `poetry run tox`\n - Format code :\xa0`black`\n - Generate documentation : `poetry run tox -e doc`\n\n## Documentation\n\nYou can build it with the following commands, or read it on [readthedocs](https://sheraf.readthedocs.io/en/latest/).\n\n    poetry run tox -e doc\n    open build/sphinx/html/index.html\n\n## Development installation\n\nsheraf use poetry as its main build tool. Do not hesitate to check [the documentation](https://python-poetry.org/docs/).\n\n    poetry install --extras all\n',
     'author': 'Yaal team',
     'author_email': 'contact@yaal.fr',
     'maintainer': 'Éloi Rivard',
     'maintainer_email': 'eloi@yaal.fr',
     'url': 'https://sheraf.readthedocs.io/en/latest/',
```

### Comparing `sheraf-0.5.8/PKG-INFO` & `sheraf-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheraf
-Version: 0.5.8
+Version: 0.5.9
 Summary: Versatile ZODB abstraction layer
 Home-page: https://sheraf.readthedocs.io/en/latest/
 License: MIT
 Keywords: zodb,orm
 Author: Yaal team
 Author-email: contact@yaal.fr
 Maintainer: Éloi Rivard
```

