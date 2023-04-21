# Comparing `tmp/easytorch-3.7.0.tar.gz` & `tmp/easytorch-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytorch-3.7.0.tar", last modified: Thu Apr  6 01:04:48 2023, max compression
+gzip compressed data, was "easytorch-3.7.1.tar", last modified: Fri Apr 21 00:03:49 2023, max compression
```

## Comparing `easytorch-3.7.0.tar` & `easytorch-3.7.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:04:48.016923 easytorch-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-06 01:04:34.000000 easytorch-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-06 01:04:48.016923 easytorch-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-06 01:04:34.000000 easytorch-3.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:04:48.012923 easytorch-3.7.0/easytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:04:48.012923 easytorch-3.7.0/easytorch/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/config/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:04:48.012923 easytorch-3.7.0/easytorch/data/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/data/datautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/data/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/easytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:04:48.016923 easytorch-3.7.0/easytorch/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:04:48.016923 easytorch-3.7.0/easytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/utils/ddp_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/utils/tensorutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:04:48.016923 easytorch-3.7.0/easytorch/vision/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/vision/imageutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/vision/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-06 01:04:34.000000 easytorch-3.7.0/easytorch/vision/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:04:48.012923 easytorch-3.7.0/easytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-06 01:04:47.000000 easytorch-3.7.0/easytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-06 01:04:47.000000 easytorch-3.7.0/easytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 01:04:47.000000 easytorch-3.7.0/easytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-06 01:04:47.000000 easytorch-3.7.0/easytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 01:04:47.000000 easytorch-3.7.0/easytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 01:04:48.016923 easytorch-3.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-06 01:04:34.000000 easytorch-3.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:49.920190 easytorch-3.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 00:03:37.000000 easytorch-3.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-21 00:03:49.920190 easytorch-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-21 00:03:37.000000 easytorch-3.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:49.916190 easytorch-3.7.1/easytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:49.916190 easytorch-3.7.1/easytorch/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/config/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:49.920190 easytorch-3.7.1/easytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/data/datautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/data/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/easytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:49.920190 easytorch-3.7.1/easytorch/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:49.920190 easytorch-3.7.1/easytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/utils/ddp_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/utils/tensorutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:49.920190 easytorch-3.7.1/easytorch/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/vision/imageutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/vision/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-21 00:03:37.000000 easytorch-3.7.1/easytorch/vision/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:49.916190 easytorch-3.7.1/easytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-21 00:03:49.000000 easytorch-3.7.1/easytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-21 00:03:49.000000 easytorch-3.7.1/easytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:03:49.000000 easytorch-3.7.1/easytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-21 00:03:49.000000 easytorch-3.7.1/easytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 00:03:49.000000 easytorch-3.7.1/easytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 00:03:49.920190 easytorch-3.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-21 00:03:37.000000 easytorch-3.7.1/setup.py
```

### Comparing `easytorch-3.7.0/LICENSE` & `easytorch-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/PKG-INFO` & `easytorch-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.7.0
+Version: 3.7.1
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `easytorch-3.7.0/README.md` & `easytorch-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch/config/__init__.py` & `easytorch-3.7.1/easytorch/config/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch/config/state.py` & `easytorch-3.7.1/easytorch/config/state.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch/data/data.py` & `easytorch-3.7.1/easytorch/data/data.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch/data/datautils.py` & `easytorch-3.7.1/easytorch/data/datautils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch/data/multiproc.py` & `easytorch-3.7.1/easytorch/data/multiproc.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch/easytorch.py` & `easytorch-3.7.1/easytorch/easytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,17 @@
         self._make_reproducible()
         self.conf.update(is_master=self.conf.get('is_master', True), world_rank=0)
         self.conf['RUN-ID'] = _dtime.now().strftime("ET-%Y%m%d-%H%M%S-") + _uuid.uuid4().hex[:4].upper()
 
         self.conf['save_dir'] = self.conf['output_base_dir'] + _sep + self.conf['phase'].upper() + _sep + self.conf[
             "name"]
 
+        """ No multi Loading in other than train mode """
+        self.conf['multi_load'] = self.conf['multi_load'] and self.conf['phase'] == Phase.TRAIN
+
     def _device_check(self):
         self.conf['gpus'] = self.conf['gpus'] if self.conf.get('gpus') else []
         if self.conf['verbose'] and len(self.conf['gpus']) > NUM_GPUS:
             warn(f"{len(self.conf['gpus'])} GPU(s) requested "
                  f"but {NUM_GPUS if CUDA_AVAILABLE else 'GPU(s) not'} detected. "
                  f"Using {str(NUM_GPUS) + ' GPU(s)' if CUDA_AVAILABLE else 'CPU(Much slower)'}.")
             self.conf['gpus'] = list(range(NUM_GPUS))
```

### Comparing `easytorch-3.7.0/easytorch/metrics/loss.py` & `easytorch-3.7.1/easytorch/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch/metrics/metrics.py` & `easytorch-3.7.1/easytorch/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch/runner.py` & `easytorch-3.7.1/easytorch/runner.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch/utils/__init__.py` & `easytorch-3.7.1/easytorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch/utils/ddp_check.py` & `easytorch-3.7.1/easytorch/utils/ddp_check.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch/utils/tensorutils.py` & `easytorch-3.7.1/easytorch/utils/tensorutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch/vision/imageutils.py` & `easytorch-3.7.1/easytorch/vision/imageutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch/vision/plotter.py` & `easytorch-3.7.1/easytorch/vision/plotter.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch/vision/transforms.py` & `easytorch-3.7.1/easytorch/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/easytorch.egg-info/PKG-INFO` & `easytorch-3.7.1/easytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.7.0
+Version: 3.7.1
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `easytorch-3.7.0/easytorch.egg-info/SOURCES.txt` & `easytorch-3.7.1/easytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.0/setup.py` & `easytorch-3.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     import cv2
 except:
     _requires.append('opencv-contrib-python-headless')
 
 # This call to setup() does all the work
 setup(
     name="easytorch",
-    version="3.7.0",
+    version="3.7.1",
     description="Easy Neural Network Experiments with pytorch",
     long_description=_README,
     long_description_content_type="text/markdown",
     url="https://github.com/sraashis/easytorch",
     author="Aashis Khana1",
     author_email="sraashis@gmail.com",
     license="MIT",
```

