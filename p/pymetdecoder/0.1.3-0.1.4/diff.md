# Comparing `tmp/pymetdecoder-0.1.3.tar.gz` & `tmp/pymetdecoder-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetdecoder-0.1.3.tar", last modified: Mon Apr 17 09:03:06 2023, max compression
+gzip compressed data, was "pymetdecoder-0.1.4.tar", last modified: Fri Apr 21 09:17:09 2023, max compression
```

## Comparing `pymetdecoder-0.1.3.tar` & `pymetdecoder-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-04-17 09:03:06.464609 pymetdecoder-0.1.3/
--rw-rw-r--   0 tdba      (1001) tdba      (1001)      356 2022-08-30 11:15:11.000000 pymetdecoder-0.1.3/LICENSE.md
--rw-rw-r--   0 tdba      (1001) tdba      (1001)     7154 2023-04-17 09:03:06.464609 pymetdecoder-0.1.3/PKG-INFO
--rw-rw-r--   0 tdba      (1001) tdba      (1001)     6625 2023-01-26 09:28:17.000000 pymetdecoder-0.1.3/README.md
-drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-04-17 09:03:06.464609 pymetdecoder-0.1.3/pymetdecoder/
--rw-rw-r--   0 tdba      (1001) tdba      (1001)    14250 2023-04-17 08:57:16.000000 pymetdecoder-0.1.3/pymetdecoder/__init__.py
--rw-rw-r--   0 tdba      (1001) tdba      (1001)    39868 2023-01-26 09:28:17.000000 pymetdecoder-0.1.3/pymetdecoder/code_tables.py
--rw-rw-r--   0 tdba      (1001) tdba      (1001)     5429 2022-08-30 11:15:11.000000 pymetdecoder-0.1.3/pymetdecoder/conversion.py
-drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-04-17 09:03:06.464609 pymetdecoder-0.1.3/pymetdecoder/synop/
--rw-rw-r--   0 tdba      (1001) tdba      (1001)    59831 2023-01-26 09:28:17.000000 pymetdecoder-0.1.3/pymetdecoder/synop/__init__.py
--rw-rw-r--   0 tdba      (1001) tdba      (1001)    57239 2023-01-26 09:28:17.000000 pymetdecoder-0.1.3/pymetdecoder/synop/observations.py
-drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-04-17 09:03:06.464609 pymetdecoder-0.1.3/pymetdecoder.egg-info/
--rw-rw-r--   0 tdba      (1001) tdba      (1001)     7154 2023-04-17 09:03:06.000000 pymetdecoder-0.1.3/pymetdecoder.egg-info/PKG-INFO
--rw-rw-r--   0 tdba      (1001) tdba      (1001)      319 2023-04-17 09:03:06.000000 pymetdecoder-0.1.3/pymetdecoder.egg-info/SOURCES.txt
--rw-rw-r--   0 tdba      (1001) tdba      (1001)        1 2023-04-17 09:03:06.000000 pymetdecoder-0.1.3/pymetdecoder.egg-info/dependency_links.txt
--rw-rw-r--   0 tdba      (1001) tdba      (1001)       13 2023-04-17 09:03:06.000000 pymetdecoder-0.1.3/pymetdecoder.egg-info/top_level.txt
--rw-rw-r--   0 tdba      (1001) tdba      (1001)       38 2023-04-17 09:03:06.464609 pymetdecoder-0.1.3/setup.cfg
--rw-rw-r--   0 tdba      (1001) tdba      (1001)      865 2023-04-17 08:57:16.000000 pymetdecoder-0.1.3/setup.py
+drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-04-21 09:17:09.318445 pymetdecoder-0.1.4/
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)      356 2022-08-30 11:15:11.000000 pymetdecoder-0.1.4/LICENSE.md
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)     7154 2023-04-21 09:17:09.318445 pymetdecoder-0.1.4/PKG-INFO
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)     6625 2023-04-21 08:48:47.000000 pymetdecoder-0.1.4/README.md
+drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-04-21 09:17:09.318445 pymetdecoder-0.1.4/pymetdecoder/
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)    14375 2023-04-21 09:13:04.000000 pymetdecoder-0.1.4/pymetdecoder/__init__.py
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)    39868 2023-01-26 09:28:17.000000 pymetdecoder-0.1.4/pymetdecoder/code_tables.py
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)     5429 2022-08-30 11:15:11.000000 pymetdecoder-0.1.4/pymetdecoder/conversion.py
+drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-04-21 09:17:09.318445 pymetdecoder-0.1.4/pymetdecoder/synop/
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)    59830 2023-04-21 08:54:00.000000 pymetdecoder-0.1.4/pymetdecoder/synop/__init__.py
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)    57420 2023-04-21 09:13:04.000000 pymetdecoder-0.1.4/pymetdecoder/synop/observations.py
+drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-04-21 09:17:09.318445 pymetdecoder-0.1.4/pymetdecoder.egg-info/
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)     7154 2023-04-21 09:17:09.000000 pymetdecoder-0.1.4/pymetdecoder.egg-info/PKG-INFO
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)      319 2023-04-21 09:17:09.000000 pymetdecoder-0.1.4/pymetdecoder.egg-info/SOURCES.txt
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)        1 2023-04-21 09:17:09.000000 pymetdecoder-0.1.4/pymetdecoder.egg-info/dependency_links.txt
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)       13 2023-04-21 09:17:09.000000 pymetdecoder-0.1.4/pymetdecoder.egg-info/top_level.txt
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)       38 2023-04-21 09:17:09.318445 pymetdecoder-0.1.4/setup.cfg
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)      865 2023-04-21 09:15:47.000000 pymetdecoder-0.1.4/setup.py
```

### Comparing `pymetdecoder-0.1.3/PKG-INFO` & `pymetdecoder-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetdecoder
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python module to decode/encode met reports e.g. SYNOPs
 Home-page: https://github.com/antarctica/pymetdecoder
 Author: Tim Barnes
 Author-email: tdba@bas.ac.uk
 License: Open Government License v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -245,15 +245,15 @@
 
 ## Changelog
 
 See `CHANGELOG.md` for the list of changes
 
 ## Known issues
 
-This version is 0.1.2. There may be some uncaught bugs/issues or other problems that have not been found yet. The following is a list of known issues which are still to be addressed:
+This version is 0.1.4. There may be some uncaught bugs/issues or other problems that have not been found yet. The following is a list of known issues which are still to be addressed:
 
 * Not all countries are auto-detected. As more region-specific handling is added, more countries will be added to the list
 * Section 5 of the SYNOP messages are not handled yet. Any codes in these sections are stored in the output dict under the `section5` attribute
 * Most of the group 9 codes of section 3 are handled. Any codes not handled are added to a list in the output dict under the `_not_implemented` attribute
 * Some aspects of encoding have not been fully tested
 
 Feel free to raise any additional issues/bugs in the issue tracker
```

### Comparing `pymetdecoder-0.1.3/README.md` & `pymetdecoder-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
 
 ## Changelog
 
 See `CHANGELOG.md` for the list of changes
 
 ## Known issues
 
-This version is 0.1.2. There may be some uncaught bugs/issues or other problems that have not been found yet. The following is a list of known issues which are still to be addressed:
+This version is 0.1.4. There may be some uncaught bugs/issues or other problems that have not been found yet. The following is a list of known issues which are still to be addressed:
 
 * Not all countries are auto-detected. As more region-specific handling is added, more countries will be added to the list
 * Section 5 of the SYNOP messages are not handled yet. Any codes in these sections are stored in the output dict under the `section5` attribute
 * Most of the group 9 codes of section 3 are handled. Any codes not handled are added to a list in the output dict under the `_not_implemented` attribute
 * Some aspects of encoding have not been fully tested
 
 Feel free to raise any additional issues/bugs in the issue tracker
```

### Comparing `pymetdecoder-0.1.3/pymetdecoder/__init__.py` & `pymetdecoder-0.1.4/pymetdecoder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 #
 # Main __init__ script for pymetdecoder
 #
 # TDBA 2019-01-16:
 #   * First version
 # TDBA 2023-04-14:
 #   * Removed logging configuration (#8)
+# TDBA 2023-04-21:
+#   * Rainfall group in section 3 now decodes properly if cloud group (or other
+#     group) follows (#9)
 ################################################################################
 # IMPORTS
 ################################################################################
 import sys, json, logging, re
 from . import conversion
 ################################################################################
 # EXCEPTION CLASSES
```

### Comparing `pymetdecoder-0.1.3/pymetdecoder/code_tables.py` & `pymetdecoder-0.1.4/pymetdecoder/code_tables.py`

 * *Files identical despite different names*

### Comparing `pymetdecoder-0.1.3/pymetdecoder/conversion.py` & `pymetdecoder-0.1.4/pymetdecoder/conversion.py`

 * *Files identical despite different names*

### Comparing `pymetdecoder-0.1.3/pymetdecoder/synop/__init__.py` & `pymetdecoder-0.1.4/pymetdecoder/synop/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,15 +482,15 @@
                             radiation_type = RADIATION_TYPES[int(m[0])]
                         if "radiation" not in data:
                             data["radiation"] = {}
                         if radiation_type not in data["radiation"]:
                             data["radiation"][radiation_type] = []
                         data["radiation"][radiation_type].append(radiation)
                 if len(msg_5) > 0 and msg_5[-1].startswith("6") and data["precipitation_indicator"]["in_group_3"]:
-                    data["precipitation_s3"] = obs.Precipitation().decode(next_group, tenths=False)
+                    data["precipitation_s3"] = obs.Precipitation().decode(msg_5[-1], tenths=False)
                     if "short_wave" in data["radiation"]:
                         if len(data["radiation"]["short_wave"]) == 1:
                             del(data["radiation"]["short_wave"])
                         else:
                             del(data["radiation"]["short_wave"][-1])
                     # if len(data["radiation"]["short_wave"]):
                     #     del(data["radiation"]["short_wave"][-1])
```

### Comparing `pymetdecoder-0.1.3/pymetdecoder/synop/observations.py` & `pymetdecoder-0.1.4/pymetdecoder/synop/observations.py`

 * *Files identical despite different names*

```diff
@@ -3,14 +3,16 @@
 #
 # Observation classes from SYNOP
 #
 # TDBA 2019-01-21:
 #   * First version
 # TDBA 2020-11-12:
 #   * Merged from individual section scripts
+# TDBA 2023-04-21:
+#   * Fixed erroneous error message for temperatures (#10)
 ################################################################################
 # CONFIGURATION
 ################################################################################
 import re
 from pymetdecoder import Observation, logging, DecodeError, EncodeError, InvalidCode
 from pymetdecoder import code_tables as ct
 ################################################################################
@@ -1442,16 +1444,18 @@
     """
     _CODE_LEN = 4
     def _decode(self, group):
         # Get the sign (sn) and temperature (TTT):
         sn  = group[1:2]
         TTT = group[2:5]
 
-        # The last character can sometimes be a "/" instead of a 0, so fix
-        TTT = re.sub("\/$", "0", TTT)
+        # The last character can sometimes be a "/" instead of a 0, so fix.
+        # But, only do this if the whole thing isn't /// (see issue #10)
+        if TTT != "///":
+            TTT = re.sub("\/$", "0", TTT)
 
         # If sign is not 0 or 1, return None with log message
         if sn not in ["0", "1", "/"]:
             logging.warning("{} is an invalid temperature group".format(group))
             return None
 
         # Return value
```

### Comparing `pymetdecoder-0.1.3/pymetdecoder.egg-info/PKG-INFO` & `pymetdecoder-0.1.4/pymetdecoder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetdecoder
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python module to decode/encode met reports e.g. SYNOPs
 Home-page: https://github.com/antarctica/pymetdecoder
 Author: Tim Barnes
 Author-email: tdba@bas.ac.uk
 License: Open Government License v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -245,15 +245,15 @@
 
 ## Changelog
 
 See `CHANGELOG.md` for the list of changes
 
 ## Known issues
 
-This version is 0.1.2. There may be some uncaught bugs/issues or other problems that have not been found yet. The following is a list of known issues which are still to be addressed:
+This version is 0.1.4. There may be some uncaught bugs/issues or other problems that have not been found yet. The following is a list of known issues which are still to be addressed:
 
 * Not all countries are auto-detected. As more region-specific handling is added, more countries will be added to the list
 * Section 5 of the SYNOP messages are not handled yet. Any codes in these sections are stored in the output dict under the `section5` attribute
 * Most of the group 9 codes of section 3 are handled. Any codes not handled are added to a list in the output dict under the `_not_implemented` attribute
 * Some aspects of encoding have not been fully tested
 
 Feel free to raise any additional issues/bugs in the issue tracker
```

### Comparing `pymetdecoder-0.1.3/setup.py` & `pymetdecoder-0.1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name             = "pymetdecoder",
-    version          = "0.1.3",
+    version          = "0.1.4",
     author           = "Tim Barnes",
     author_email     = "tdba@bas.ac.uk",
     description      = "Python module to decode/encode met reports e.g. SYNOPs",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url              = "https://github.com/antarctica/pymetdecoder",
     license          = "Open Government License v3.0",
```

