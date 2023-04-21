# Comparing `tmp/monplugin-0.5.1.tar.gz` & `tmp/monplugin-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monplugin-0.5.1.tar", last modified: Wed Apr  5 12:53:47 2023, max compression
+gzip compressed data, was "monplugin-0.6.0.tar", last modified: Fri Apr 21 12:19:40 2023, max compression
```

## Comparing `monplugin-0.5.1.tar` & `monplugin-0.6.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      188 2023-04-05 12:16:51.767308 monplugin-0.5.1/README.md
--rw-r--r--   0        0        0     8435 2023-04-05 12:50:49.146236 monplugin-0.5.1/monplugin/__init__.py
--rw-r--r--   0        0        0      515 2023-04-05 12:52:19.832594 monplugin-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 monplugin-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      188 2023-04-05 12:16:51.767308 monplugin-0.6.0/README.md
+-rw-r--r--   0        0        0     8542 2023-04-21 12:10:43.505809 monplugin-0.6.0/monplugin/__init__.py
+-rw-r--r--   0        0        0      542 2023-04-21 12:18:36.449379 monplugin-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 monplugin-0.6.0/PKG-INFO
```

### Comparing `monplugin-0.5.1/monplugin/__init__.py` & `monplugin-0.6.0/monplugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,28 @@
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 
 import enum
 import io
 import re
 import time
+import warnings
 
 class Status(enum.Enum):
     OK       = 0
     WARNING  = 1
     CRITICAL = 2
     UNKNOWN  = 3
 
 class MonIllegalInstruction(Exception):
     pass
 
+class MonShortnameDeprecated(UserWarning):
+    pass
+
 class Range:
     def __init__(self, range_spec=None):
         """
         Handle Range specs like :10, ~:10, 10:20 or @1.0:1.5 and the like. See:
         https://www.monitoring-plugins.org/doc/guidelines.html#THRESHOLDFORMAT
         """
         self.range_spec = range_spec
@@ -142,16 +146,17 @@
         return "'{label}'={value}{uom};{warning};{critical};{min};{max}".format( **d )
 
     def __repr__(self):
         return f'PerformanceLabel({str(self)})'
 
 
 class Check:
-    def __init__(self, shortname='unknown', threshold=None):
-        self.shortname = shortname
+    def __init__(self, *, shortname=None, threshold=None):
+        if shortname is not None:
+            warnings.warn("Check.__init__(shortname=) is deprecated", MonShortnameDeprecated, stacklevel=2)
         self.set_threshold(threshold)
         self._perfdata = []
         self._perfmultidata = {}
         self._messages = {
             Status.OK: [],
             Status.WARNING: [],
             Status.CRITICAL: [],
@@ -182,15 +187,15 @@
         self._perfdata.append( PerformanceLabel(**kwargs) )
 
     def add_perfmultidata(self, entity, check, **kwargs):
         if self._perfdata:
             raise MonIllegalInstruction("you already used add_perfdata")
 
         if not check:
-            check = self.shortname.lower() or "unknown"
+            check = "unknown"
 
         self._perfmultidata.setdefault((entity, check), [])
         self._perfmultidata[(entity,check)].append( PerformanceLabel(**kwargs) )
 
 
     def check_messages(self, separator=' ', separator_all=None, allok=None):
         """
@@ -233,16 +238,15 @@
     def check_threshold(self, *args):
         return self.threshold.get_status(*args)
 
     def exit(self, code=Status.OK, message="OK"):
         if isinstance(code, str):
             code = Status[code]
 
-        print("{name} {code} - {text}".format(
-            name=self.shortname,
+        print("{code}: {text}".format(
             code=code.name,
             text=message
         ))
 
         print(self.get_perfdata())
         raise SystemExit(code.value)
```

### Comparing `monplugin-0.5.1/pyproject.toml` & `monplugin-0.6.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "monplugin"
 readme = "README.md"
 description = "Partial python port of perls Monitoring::Plugin"
-version = "0.5.1"
+version = "0.6.0"
+requires-python = ">= 3.6"
 authors = [
     { name = "Danijel Tasov", email = "danijel.tasov@consol.de" }
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: System :: Monitoring",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `monplugin-0.5.1/PKG-INFO` & `monplugin-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: monplugin
-Version: 0.5.1
+Version: 0.6.0
 Summary: Partial python port of perls Monitoring::Plugin
 Author-email: Danijel Tasov <danijel.tasov@consol.de>
+Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 partial port of perls Monitoring::Plugins
```

