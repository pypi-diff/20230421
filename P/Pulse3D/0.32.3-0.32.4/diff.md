# Comparing `tmp/Pulse3D-0.32.3.tar.gz` & `tmp/Pulse3D-0.32.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pulse3D-0.32.3.tar", last modified: Tue Apr  4 19:00:35 2023, max compression
+gzip compressed data, was "Pulse3D-0.32.4.tar", last modified: Fri Apr 21 20:31:18 2023, max compression
```

## Comparing `Pulse3D-0.32.3.tar` & `Pulse3D-0.32.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:00:35.250918 Pulse3D-0.32.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-04 19:00:35.250918 Pulse3D-0.32.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:00:35.246918 Pulse3D-0.32.3/mantarray-magnet-finding/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-04 18:59:27.000000 Pulse3D-0.32.3/mantarray-magnet-finding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:00:35.246918 Pulse3D-0.32.3/mantarray-magnet-finding/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:00:35.246918 Pulse3D-0.32.3/mantarray-magnet-finding/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-04 18:59:27.000000 Pulse3D-0.32.3/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-04 18:59:27.000000 Pulse3D-0.32.3/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-04 18:59:27.000000 Pulse3D-0.32.3/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-04 18:59:27.000000 Pulse3D-0.32.3/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-04 19:00:35.254918 Pulse3D-0.32.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:00:35.246918 Pulse3D-0.32.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:00:35.250918 Pulse3D-0.32.3/src/Pulse3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-04 19:00:35.000000 Pulse3D-0.32.3/src/Pulse3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-04 19:00:35.000000 Pulse3D-0.32.3/src/Pulse3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:00:19.000000 Pulse3D-0.32.3/src/Pulse3D.egg-info/not-zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:00:35.250918 Pulse3D-0.32.3/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-04 18:59:58.000000 Pulse3D-0.32.3/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-04 18:59:58.000000 Pulse3D-0.32.3/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-04 18:59:58.000000 Pulse3D-0.32.3/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-04 18:59:58.000000 Pulse3D-0.32.3/src/mantarray_magnet_finding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:00:35.250918 Pulse3D-0.32.3/src/pulse3D/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/src/pulse3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/src/pulse3D/compression_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/src/pulse3D/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    45242 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/src/pulse3D/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/src/pulse3D/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/src/pulse3D/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34501 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/src/pulse3D/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19450 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/src/pulse3D/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/src/pulse3D/plate_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/src/pulse3D/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/src/pulse3D/stimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/src/pulse3D/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-04 18:59:24.000000 Pulse3D-0.32.3/src/pulse3D/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/mantarray-magnet-finding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-21 20:30:15.000000 Pulse3D-0.32.4/mantarray-magnet-finding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/mantarray-magnet-finding/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/mantarray-magnet-finding/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-21 20:30:15.000000 Pulse3D-0.32.4/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-21 20:30:15.000000 Pulse3D-0.32.4/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-21 20:30:15.000000 Pulse3D-0.32.4/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-21 20:30:15.000000 Pulse3D-0.32.4/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/src/Pulse3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-21 20:31:18.000000 Pulse3D-0.32.4/src/Pulse3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-21 20:31:18.000000 Pulse3D-0.32.4/src/Pulse3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:31:03.000000 Pulse3D-0.32.4/src/Pulse3D.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-21 20:30:44.000000 Pulse3D-0.32.4/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-21 20:30:44.000000 Pulse3D-0.32.4/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-21 20:30:44.000000 Pulse3D-0.32.4/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-21 20:30:44.000000 Pulse3D-0.32.4/src/mantarray_magnet_finding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:31:18.127540 Pulse3D-0.32.4/src/pulse3D/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/compression_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45242 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34501 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19450 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/plate_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-21 20:30:11.000000 Pulse3D-0.32.4/src/pulse3D/utils.py
```

### Comparing `Pulse3D-0.32.3/LICENSE` & `Pulse3D-0.32.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/PKG-INFO` & `Pulse3D-0.32.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.32.3
+Version: 0.32.4
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.32.3/mantarray-magnet-finding/setup.py` & `Pulse3D-0.32.4/mantarray-magnet-finding/setup.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.32.4/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.32.4/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/setup.py` & `Pulse3D-0.32.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 extensions = [Extension("pulse3D.compression_cy", [os.path.join("src", "pulse3D", "compression_cy") + ext])]
 if USE_CYTHON:
     # cythonizing compression_cy.pyx with kwarg annotate=True will help when optimizing the code by enabling generation of the html annotation file
     extensions = cythonize(extensions, annotate=False)
 
 setup(
     name="Pulse3D",
-    version="0.32.3",
+    version="0.32.4",
     description="Pulse3D Analysis Platform",
     url="https://github.com/CuriBio/Pulse3D",
     project_urls={"Documentation": "https://pulse3D.readthedocs.io/en/latest/"},
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `Pulse3D-0.32.3/src/Pulse3D.egg-info/PKG-INFO` & `Pulse3D-0.32.4/src/Pulse3D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.32.3
+Version: 0.32.4
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.32.3/src/Pulse3D.egg-info/SOURCES.txt` & `Pulse3D-0.32.4/src/Pulse3D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.32.4/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.32.4/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/src/pulse3D/compression_cy.pyx` & `Pulse3D-0.32.4/src/pulse3D/compression_cy.pyx`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/src/pulse3D/constants.py` & `Pulse3D-0.32.4/src/pulse3D/constants.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/src/pulse3D/excel_writer.py` & `Pulse3D-0.32.4/src/pulse3D/excel_writer.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/src/pulse3D/exceptions.py` & `Pulse3D-0.32.4/src/pulse3D/exceptions.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/src/pulse3D/magnet_finding.py` & `Pulse3D-0.32.4/src/pulse3D/magnet_finding.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     initial_magnet_finding_params: Dict[str, Union[int, float]],
     filter_inputs: bool = True,
     filter_outputs: bool = False,
 ) -> Dict[str, NDArray[(1, Any), float]]:
     if filter_inputs:
         fields = filter_raw_signal(fields)
 
-    output_dict = get_positions((fields.T - baseline).T)
+    output_dict = get_positions((fields.T - baseline).T, **initial_magnet_finding_params)  # type: ignore # mypy complaining about **
 
     if filter_outputs:
         for param, output_arr in output_dict.items():
             output_dict[param] = filter_magnet_positions(output_arr)
 
     return output_dict
```

### Comparing `Pulse3D-0.32.3/src/pulse3D/metrics.py` & `Pulse3D-0.32.4/src/pulse3D/metrics.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/src/pulse3D/peak_detection.py` & `Pulse3D-0.32.4/src/pulse3D/peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/src/pulse3D/plate_recording.py` & `Pulse3D-0.32.4/src/pulse3D/plate_recording.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/src/pulse3D/plotting.py` & `Pulse3D-0.32.4/src/pulse3D/plotting.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/src/pulse3D/stimulation.py` & `Pulse3D-0.32.4/src/pulse3D/stimulation.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/src/pulse3D/transforms.py` & `Pulse3D-0.32.4/src/pulse3D/transforms.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.3/src/pulse3D/utils.py` & `Pulse3D-0.32.4/src/pulse3D/utils.py`

 * *Files identical despite different names*

