# Comparing `tmp/coco_types-0.0.6.tar.gz` & `tmp/coco_types-0.0.7.tar.gz`

## Comparing `coco_types-0.0.6.tar` & `coco_types-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 coco_types-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 coco_types-0.0.6/pytest.ini
--rwxr-xr-x   0        0        0     1301 2020-02-02 00:00:00.000000 coco_types-0.0.6/setup.cfg
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 coco_types-0.0.6/requirements/README.md
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 coco_types-0.0.6/requirements/requirements-build.txt
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 coco_types-0.0.6/requirements/requirements-dev.txt
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 coco_types-0.0.6/requirements/requirements-test.txt
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 coco_types-0.0.6/requirements/requirements.txt
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 coco_types-0.0.6/src/coco_types/__init__.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 coco_types-0.0.6/src/coco_types/coco_keypoints.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 coco_types-0.0.6/src/coco_types/coco_object_detection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coco_types-0.0.6/src/coco_types/py.typed
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 coco_types-0.0.6/src/coco_types/dicts/__init__.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 coco_types-0.0.6/src/coco_types/dicts/coco_keypoints.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 coco_types-0.0.6/src/coco_types/dicts/coco_object_detection.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 coco_types-0.0.6/tests/test_load_pydantic.py
--rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 coco_types-0.0.6/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 coco_types-0.0.6/LICENSE.md
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 coco_types-0.0.6/README.md
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 coco_types-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 coco_types-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 coco_types-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 coco_types-0.0.7/pytest.ini
+-rwxr-xr-x   0        0        0     1301 2020-02-02 00:00:00.000000 coco_types-0.0.7/setup.cfg
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 coco_types-0.0.7/requirements/README.md
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 coco_types-0.0.7/requirements/requirements-build.txt
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 coco_types-0.0.7/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 coco_types-0.0.7/requirements/requirements-test.txt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 coco_types-0.0.7/requirements/requirements.txt
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 coco_types-0.0.7/src/coco_types/__init__.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 coco_types-0.0.7/src/coco_types/coco_keypoints.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 coco_types-0.0.7/src/coco_types/coco_object_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coco_types-0.0.7/src/coco_types/py.typed
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 coco_types-0.0.7/src/coco_types/dicts/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 coco_types-0.0.7/src/coco_types/dicts/coco_keypoints.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 coco_types-0.0.7/src/coco_types/dicts/coco_object_detection.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 coco_types-0.0.7/tests/test_load_pydantic.py
+-rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 coco_types-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 coco_types-0.0.7/LICENSE.md
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 coco_types-0.0.7/README.md
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 coco_types-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 coco_types-0.0.7/PKG-INFO
```

### Comparing `coco_types-0.0.6/.pre-commit-config.yaml` & `coco_types-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.6/setup.cfg` & `coco_types-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.6/requirements/README.md` & `coco_types-0.0.7/requirements/README.md`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.6/requirements/requirements-build.txt` & `coco_types-0.0.7/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.6/requirements/requirements-dev.txt` & `coco_types-0.0.7/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.6/requirements/requirements-test.txt` & `coco_types-0.0.7/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.6/src/coco_types/coco_keypoints.py` & `coco_types-0.0.7/src/coco_types/coco_keypoints.py`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.6/src/coco_types/coco_object_detection.py` & `coco_types-0.0.7/src/coco_types/coco_object_detection.py`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.6/src/coco_types/dicts/coco_object_detection.py` & `coco_types-0.0.7/src/coco_types/dicts/coco_object_detection.py`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.6/LICENSE.md` & `coco_types-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.6/README.md` & `coco_types-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.6/pyproject.toml` & `coco_types-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.6/PKG-INFO` & `coco_types-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coco_types
-Version: 0.0.6
+Version: 0.0.7
 Summary: Package for handling COCO datasets types.
 Project-URL: Homepage, https://github.com/hoel-bagard/coco_types
 Project-URL: Bug Tracker, https://github.com/hoel-bagard/coco_types/issues
 Author: Bagard Hoel
 License: MIT
 License-File: LICENSE.md
 Keywords: COCO,COCO dataset
```

