# Comparing `tmp/robotcode_robot-0.33.0.tar.gz` & `tmp/robotcode_robot-0.34.1.tar.gz`

## Comparing `robotcode_robot-0.33.0.tar` & `robotcode_robot-0.34.1.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.33.0/src/robotcode/robot/__version__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.33.0/src/robotcode/robot/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.33.0/src/robotcode/robot/config/__init__.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 robotcode_robot-0.33.0/src/robotcode/robot/config/loader.py
--rw-r--r--   0        0        0    77296 2020-02-02 00:00:00.000000 robotcode_robot-0.33.0/src/robotcode/robot/config/model.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 robotcode_robot-0.33.0/src/robotcode/robot/config/utils.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.33.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.33.0/LICENSE.txt
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.33.0/README.md
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 robotcode_robot-0.33.0/pyproject.toml
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 robotcode_robot-0.33.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.34.1/src/robotcode/robot/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.34.1/src/robotcode/robot/__version__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.34.1/src/robotcode/robot/py.typed
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.34.1/src/robotcode/robot/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.34.1/src/robotcode/robot/config/__init__.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 robotcode_robot-0.34.1/src/robotcode/robot/config/loader.py
+-rw-r--r--   0        0        0    77317 2020-02-02 00:00:00.000000 robotcode_robot-0.34.1/src/robotcode/robot/config/model.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 robotcode_robot-0.34.1/src/robotcode/robot/config/utils.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.34.1/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.34.1/LICENSE.txt
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.34.1/README.md
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 robotcode_robot-0.34.1/pyproject.toml
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 robotcode_robot-0.34.1/PKG-INFO
```

### Comparing `robotcode_robot-0.33.0/src/robotcode/robot/config/loader.py` & `robotcode_robot-0.34.1/src/robotcode/robot/config/loader.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.33.0/src/robotcode/robot/config/model.py` & `robotcode_robot-0.34.1/src/robotcode/robot/config/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# ruff: noqa: RUF009
+
 import dataclasses
 import datetime
 import fnmatch
 import os
 import platform
 import re
 from dataclasses import dataclass
@@ -2157,15 +2159,15 @@
 
             names = (*(default_profile or ()),)
 
         for name in names:
             profile_names = [p for p in profiles.keys() if fnmatch.fnmatchcase(p, name)]
 
             if not profile_names:
-                raise ValueError(f"Can't find any profiles matching the pattern '{name}''.")
+                raise ValueError(f"Can't find any profiles matching the pattern '{name}'.")
 
             for v in profile_names:
                 result.update({v: profiles[v]})
 
         return result
 
     def combine_profiles(self, *names: str, verbose_callback: Callable[..., None] = None) -> RobotBaseProfile:
```

### Comparing `robotcode_robot-0.33.0/src/robotcode/robot/config/utils.py` & `robotcode_robot-0.34.1/src/robotcode/robot/config/utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.33.0/.gitignore` & `robotcode_robot-0.34.1/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.33.0/LICENSE.txt` & `robotcode_robot-0.34.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.33.0/README.md` & `robotcode_robot-0.34.1/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.33.0/pyproject.toml` & `robotcode_robot-0.34.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
   "tomli>=1.1.0; python_version < '3.11'",
-  "robotcode-core",
+  "robotcode-core==0.34.1",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
```

### Comparing `robotcode_robot-0.33.0/PKG-INFO` & `robotcode_robot-0.34.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-robot
-Version: 0.33.0
+Version: 0.34.1
 Summary: Support classes for RobotCode for handling Robot Framework projects.
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-core
+Requires-Dist: robotcode-core==0.34.1
 Requires-Dist: robotframework>=4.1.0
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # robotcode-robot
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-robot.svg)](https://pypi.org/project/robotcode-robot)
```

