# Comparing `tmp/pyannote.database-5.0.0.tar.gz` & `tmp/pyannote.database-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyannote.database-5.0.0.tar", last modified: Mon Mar 27 14:41:38 2023, max compression
+gzip compressed data, was "pyannote.database-5.0.1.tar", last modified: Fri Apr 21 13:51:44 2023, max compression
```

## Comparing `pyannote.database-5.0.0.tar` & `pyannote.database-5.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:41:38.041359 pyannote.database-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-27 14:41:38.041359 pyannote.database-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    29993 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:41:38.037359 pyannote.database-5.0.0/pyannote/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:41:38.041359 pyannote.database-5.0.0/pyannote/database/
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-27 14:41:38.041359 pyannote.database-5.0.0/pyannote/database/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/file_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:41:38.041359 pyannote.database-5.0.0/pyannote/database/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/protocol/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/protocol/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/protocol/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/protocol/speaker_diarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/protocol/speaker_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/protocol/speaker_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/protocol/speaker_spotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/protocol/speaker_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)    17482 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/pyannote/database/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:41:38.037359 pyannote.database-5.0.0/pyannote.database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-27 14:41:38.000000 pyannote.database-5.0.0/pyannote.database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-27 14:41:38.000000 pyannote.database-5.0.0/pyannote.database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:41:38.000000 pyannote.database-5.0.0/pyannote.database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-27 14:41:38.000000 pyannote.database-5.0.0/pyannote.database.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-27 14:41:38.000000 pyannote.database-5.0.0/pyannote.database.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-27 14:41:38.000000 pyannote.database-5.0.0/pyannote.database.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-27 14:41:38.000000 pyannote.database-5.0.0/pyannote.database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-27 14:41:38.041359 pyannote.database-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    62474 2023-03-27 14:41:27.000000 pyannote.database-5.0.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:51:44.705033 pyannote.database-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-21 13:51:44.705033 pyannote.database-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    29993 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:51:44.701033 pyannote.database-5.0.1/pyannote/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:51:44.705033 pyannote.database-5.0.1/pyannote/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-21 13:51:44.705033 pyannote.database-5.0.1/pyannote/database/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15751 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:51:44.705033 pyannote.database-5.0.1/pyannote/database/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/protocol/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/protocol/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/protocol/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/protocol/speaker_diarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/protocol/speaker_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/protocol/speaker_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/protocol/speaker_spotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/protocol/speaker_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17482 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/pyannote/database/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:51:44.701033 pyannote.database-5.0.1/pyannote.database.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-21 13:51:44.000000 pyannote.database-5.0.1/pyannote.database.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-21 13:51:44.000000 pyannote.database-5.0.1/pyannote.database.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:51:44.000000 pyannote.database-5.0.1/pyannote.database.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-21 13:51:44.000000 pyannote.database-5.0.1/pyannote.database.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 13:51:44.000000 pyannote.database-5.0.1/pyannote.database.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-21 13:51:44.000000 pyannote.database-5.0.1/pyannote.database.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 13:51:44.000000 pyannote.database-5.0.1/pyannote.database.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-21 13:51:44.705033 pyannote.database-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62474 2023-04-21 13:51:31.000000 pyannote.database-5.0.1/versioneer.py
```

### Comparing `pyannote.database-5.0.0/LICENSE` & `pyannote.database-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/PKG-INFO` & `pyannote.database-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyannote.database
-Version: 5.0.0
+Version: 5.0.1
 Summary: Interface to multimedia databases and experimental protocols
 Home-page: http://pyannote.github.io/
 Author: Hervé Bredin
 Author-email: bredin@limsi.fr
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyannote.database-5.0.0/README.md` & `pyannote.database-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/__init__.py` & `pyannote.database-5.0.1/pyannote/__init__.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/__init__.py` & `pyannote.database-5.0.1/pyannote/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/cli.py` & `pyannote.database-5.0.1/pyannote/database/cli.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/custom.py` & `pyannote.database-5.0.1/pyannote/database/custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 
 from . import protocol as protocol_module
 
 from pyannote.database.protocol.protocol import ProtocolFile
 import yaml
 import warnings
+from numbers import Number
 from typing import Text, Dict, Callable, Any, Union
 import functools
 
 from .protocol.protocol import Subset, Scope
 from .protocol.segmentation import SegmentationProtocol
 from .protocol.speaker_diarization import SpeakerDiarizationProtocol
 
@@ -111,14 +112,20 @@
 
         loader = Loader(path)
         return loader(current_file)
 
     return load
 
 
+def NumericValue(value):
+    def load(current_file: ProtocolFile):
+        return value
+    return load
+
+
 def resolve_path(path: Path, database_yml: Path) -> Path:
     """Resolve path
 
     Parameters
     ----------
     path : `Path`
         Path. Can be either absolute, relative to current working directory, 
@@ -207,14 +214,18 @@
     lazy_loader = dict()
 
     for key, value in entries.items():
 
         if key == "uri" or key == "trial":
             continue
 
+        if isinstance(value, Number):
+            lazy_loader[key] = NumericValue(value)
+            continue
+
         # check whether value (path) contains placeholders such as {uri} or {subset}
         _, placeholders, _, _ = zip(*string.Formatter().parse(value))
         is_template = len(set(placeholders) - set([None])) > 0
 
         if is_template:
 
             # make sure old database.yml specifications still work but warn the user
@@ -438,24 +449,26 @@
     metadata = dict()
 
     if issubclass(base_class, SegmentationProtocol):
         if "classes" in protocol_entries:
             metadata["classes"] = protocol_entries.pop("classes")
 
     if issubclass(base_class, SpeakerDiarizationProtocol):
-        if "scope" in protocol_entries:
-            scope = protocol_entries.pop("scope")
-        else:
-            scope = "file"
+        scope = protocol_entries.pop("scope", None)
+
+        if scope is None and database != "X":
             msg = (
                 f"'{database}.{task}.{protocol}' found in {database_yml} does not define "
                 f"the 'scope' of speaker labels (file, database, or global). Setting it to 'file'."
             )   
             print(msg)
-        metadata["scope"] = scope
+            metadata["scope"] = "file"
+
+        else:
+            metadata["scope"] = scope
 
     methods = dict()
     for subset, subset_entries in protocol_entries.items():
 
         if subset not in [
             "files",
             "train",
```

### Comparing `pyannote.database-5.0.0/pyannote/database/database.py` & `pyannote.database-5.0.1/pyannote/database/database.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/file_finder.py` & `pyannote.database-5.0.1/pyannote/database/file_finder.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/loader.py` & `pyannote.database-5.0.1/pyannote/database/loader.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/protocol/__init__.py` & `pyannote.database-5.0.1/pyannote/database/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/protocol/collection.py` & `pyannote.database-5.0.1/pyannote/database/protocol/collection.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/protocol/protocol.py` & `pyannote.database-5.0.1/pyannote/database/protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/protocol/segmentation.py` & `pyannote.database-5.0.1/pyannote/database/protocol/segmentation.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/protocol/speaker_diarization.py` & `pyannote.database-5.0.1/pyannote/database/protocol/speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/protocol/speaker_identification.py` & `pyannote.database-5.0.1/pyannote/database/protocol/speaker_identification.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/protocol/speaker_recognition.py` & `pyannote.database-5.0.1/pyannote/database/protocol/speaker_recognition.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/protocol/speaker_spotting.py` & `pyannote.database-5.0.1/pyannote/database/protocol/speaker_spotting.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/protocol/speaker_verification.py` & `pyannote.database-5.0.1/pyannote/database/protocol/speaker_verification.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/registry.py` & `pyannote.database-5.0.1/pyannote/database/registry.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote/database/util.py` & `pyannote.database-5.0.1/pyannote/database/util.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/pyannote.database.egg-info/PKG-INFO` & `pyannote.database-5.0.1/pyannote.database.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyannote.database
-Version: 5.0.0
+Version: 5.0.1
 Summary: Interface to multimedia databases and experimental protocols
 Home-page: http://pyannote.github.io/
 Author: Hervé Bredin
 Author-email: bredin@limsi.fr
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyannote.database-5.0.0/pyannote.database.egg-info/SOURCES.txt` & `pyannote.database-5.0.1/pyannote.database.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/setup.py` & `pyannote.database-5.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyannote.database-5.0.0/versioneer.py` & `pyannote.database-5.0.1/versioneer.py`

 * *Files identical despite different names*

