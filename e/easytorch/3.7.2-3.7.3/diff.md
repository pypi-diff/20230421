# Comparing `tmp/easytorch-3.7.2.tar.gz` & `tmp/easytorch-3.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytorch-3.7.2.tar", last modified: Fri Apr 21 00:39:38 2023, max compression
+gzip compressed data, was "easytorch-3.7.3.tar", last modified: Fri Apr 21 12:11:56 2023, max compression
```

## Comparing `easytorch-3.7.2.tar` & `easytorch-3.7.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:39:38.652628 easytorch-3.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 00:39:27.000000 easytorch-3.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-21 00:39:38.652628 easytorch-3.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-21 00:39:27.000000 easytorch-3.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:39:38.652628 easytorch-3.7.2/easytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:39:38.652628 easytorch-3.7.2/easytorch/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/config/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:39:38.652628 easytorch-3.7.2/easytorch/data/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12980 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/data/datautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/data/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/easytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:39:38.652628 easytorch-3.7.2/easytorch/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:39:38.652628 easytorch-3.7.2/easytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/utils/ddp_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/utils/tensorutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:39:38.652628 easytorch-3.7.2/easytorch/vision/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/vision/imageutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/vision/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-21 00:39:27.000000 easytorch-3.7.2/easytorch/vision/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:39:38.652628 easytorch-3.7.2/easytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-21 00:39:38.000000 easytorch-3.7.2/easytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-21 00:39:38.000000 easytorch-3.7.2/easytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:39:38.000000 easytorch-3.7.2/easytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-21 00:39:38.000000 easytorch-3.7.2/easytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 00:39:38.000000 easytorch-3.7.2/easytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 00:39:38.652628 easytorch-3.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-21 00:39:27.000000 easytorch-3.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:11:56.023514 easytorch-3.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 12:11:42.000000 easytorch-3.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-21 12:11:56.023514 easytorch-3.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-21 12:11:42.000000 easytorch-3.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:11:56.023514 easytorch-3.7.3/easytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:11:56.023514 easytorch-3.7.3/easytorch/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/config/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:11:56.023514 easytorch-3.7.3/easytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12983 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/data/datautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/data/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/easytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:11:56.023514 easytorch-3.7.3/easytorch/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:11:56.023514 easytorch-3.7.3/easytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/utils/ddp_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/utils/tensorutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:11:56.023514 easytorch-3.7.3/easytorch/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/vision/imageutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/vision/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-21 12:11:42.000000 easytorch-3.7.3/easytorch/vision/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:11:56.023514 easytorch-3.7.3/easytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-21 12:11:55.000000 easytorch-3.7.3/easytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-21 12:11:55.000000 easytorch-3.7.3/easytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:11:55.000000 easytorch-3.7.3/easytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-21 12:11:55.000000 easytorch-3.7.3/easytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 12:11:55.000000 easytorch-3.7.3/easytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:11:56.023514 easytorch-3.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-21 12:11:42.000000 easytorch-3.7.3/setup.py
```

### Comparing `easytorch-3.7.2/LICENSE` & `easytorch-3.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/PKG-INFO` & `easytorch-3.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.7.2
+Version: 3.7.3
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `easytorch-3.7.2/README.md` & `easytorch-3.7.3/README.md`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch/config/__init__.py` & `easytorch-3.7.3/easytorch/config/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch/config/state.py` & `easytorch-3.7.3/easytorch/config/state.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch/data/data.py` & `easytorch-3.7.3/easytorch/data/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
                 self.conf,
                 self.__class__,
                 diskcache=self.diskcache
             )
             self.gather(dataset_objs)
         else:
             for i, file in enumerate(_files, 1):
-                info(f"Loading... {i}/{_files_len}", i % _multi.LOG_FREQ == 0, self.conf['verbose'])
+                info(f"Loading... {i}/{_files_len}", i % _multi.LOG_FREQ == 0 and self.conf['verbose'])
                 self.load_index(file)
         success(f'{self.mode}, {len(self)} indices Loaded.', verbose)
 
     def gather(self, dataset_objs):
         for d in dataset_objs:
             attributes = vars(d)
             for k, v in attributes.items():
```

### Comparing `easytorch-3.7.2/easytorch/data/datautils.py` & `easytorch-3.7.3/easytorch/data/datautils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch/data/multiproc.py` & `easytorch-3.7.3/easytorch/data/multiproc.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch/easytorch.py` & `easytorch-3.7.3/easytorch/easytorch.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch/metrics/loss.py` & `easytorch-3.7.3/easytorch/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch/metrics/metrics.py` & `easytorch-3.7.3/easytorch/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch/runner.py` & `easytorch-3.7.3/easytorch/runner.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch/utils/__init__.py` & `easytorch-3.7.3/easytorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch/utils/ddp_check.py` & `easytorch-3.7.3/easytorch/utils/ddp_check.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch/utils/tensorutils.py` & `easytorch-3.7.3/easytorch/utils/tensorutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch/vision/imageutils.py` & `easytorch-3.7.3/easytorch/vision/imageutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch/vision/plotter.py` & `easytorch-3.7.3/easytorch/vision/plotter.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch/vision/transforms.py` & `easytorch-3.7.3/easytorch/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/easytorch.egg-info/PKG-INFO` & `easytorch-3.7.3/easytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.7.2
+Version: 3.7.3
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `easytorch-3.7.2/easytorch.egg-info/SOURCES.txt` & `easytorch-3.7.3/easytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.2/setup.py` & `easytorch-3.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     import cv2
 except:
     _requires.append('opencv-contrib-python-headless')
 
 # This call to setup() does all the work
 setup(
     name="easytorch",
-    version="3.7.2",
+    version="3.7.3",
     description="Easy Neural Network Experiments with pytorch",
     long_description=_README,
     long_description_content_type="text/markdown",
     url="https://github.com/sraashis/easytorch",
     author="Aashis Khana1",
     author_email="sraashis@gmail.com",
     license="MIT",
```

