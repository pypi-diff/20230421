# Comparing `tmp/pydvma-0.9.2.tar.gz` & `tmp/pydvma-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydvma-0.9.2.tar", last modified: Fri Apr 21 09:49:17 2023, max compression
+gzip compressed data, was "pydvma-0.9.3.tar", last modified: Fri Apr 21 09:58:11 2023, max compression
```

## Comparing `pydvma-0.9.2.tar` & `pydvma-0.9.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 09:49:17.928030 pydvma-0.9.2/
--rw-rw-rw-   0        0        0     1634 2022-04-26 11:34:19.000000 pydvma-0.9.2/LICENSE
--rw-rw-rw-   0        0        0     3150 2023-04-21 09:49:17.928030 pydvma-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     2940 2023-04-19 10:31:43.000000 pydvma-0.9.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 09:49:17.920026 pydvma-0.9.2/pydvma/
--rw-rw-rw-   0        0        0     1165 2023-04-20 11:25:15.000000 pydvma-0.9.2/pydvma/__init__.py
--rw-rw-rw-   0        0        0    10825 2023-04-20 11:25:15.000000 pydvma-0.9.2/pydvma/acquisition.py
--rw-rw-rw-   0        0        0    16393 2023-04-20 11:25:15.000000 pydvma-0.9.2/pydvma/analysis.py
--rw-rw-rw-   0        0        0    30676 2023-04-21 09:32:53.000000 pydvma-0.9.2/pydvma/datastructure.py
--rw-rw-rw-   0        0        0    16695 2023-04-19 14:11:21.000000 pydvma-0.9.2/pydvma/file.py
--rw-rw-rw-   0        0        0   126497 2023-04-21 09:47:49.000000 pydvma-0.9.2/pydvma/gui.py
--rw-rw-rw-   0        0        0     2815 2023-04-19 10:31:43.000000 pydvma-0.9.2/pydvma/gui_tk.py
--rw-rw-rw-   0        0        0   144611 2023-04-19 10:31:43.000000 pydvma-0.9.2/pydvma/icon.png
--rw-rw-rw-   0        0        0    10628 2023-04-20 11:25:15.000000 pydvma-0.9.2/pydvma/modal.py
--rw-rw-rw-   0        0        0     8111 2023-04-21 09:24:50.000000 pydvma-0.9.2/pydvma/options.py
--rw-rw-rw-   0        0        0    14944 2023-04-20 11:25:15.000000 pydvma-0.9.2/pydvma/oscilloscope.py
--rw-rw-rw-   0        0        0    27763 2023-04-20 11:25:15.000000 pydvma-0.9.2/pydvma/plotting.py
--rw-rw-rw-   0        0        0    26182 2023-04-20 11:25:15.000000 pydvma-0.9.2/pydvma/streams.py
--rw-rw-rw-   0        0        0     2871 2023-04-20 11:25:15.000000 pydvma-0.9.2/pydvma/testdata.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:49:17.927026 pydvma-0.9.2/pydvma.egg-info/
--rw-rw-rw-   0        0        0     3150 2023-04-21 09:49:16.000000 pydvma-0.9.2/pydvma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-04-21 09:49:17.000000 pydvma-0.9.2/pydvma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 09:49:16.000000 pydvma-0.9.2/pydvma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-04-21 09:49:16.000000 pydvma-0.9.2/pydvma.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 09:49:16.000000 pydvma-0.9.2/pydvma.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 09:49:17.928030 pydvma-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-04-21 09:32:56.000000 pydvma-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:58:11.313694 pydvma-0.9.3/
+-rw-rw-rw-   0        0        0     1634 2022-04-26 11:34:19.000000 pydvma-0.9.3/LICENSE
+-rw-rw-rw-   0        0        0     3150 2023-04-21 09:58:11.313694 pydvma-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2940 2023-04-19 10:31:43.000000 pydvma-0.9.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 09:58:11.307489 pydvma-0.9.3/pydvma/
+-rw-rw-rw-   0        0        0     1165 2023-04-20 11:25:15.000000 pydvma-0.9.3/pydvma/__init__.py
+-rw-rw-rw-   0        0        0    10825 2023-04-20 11:25:15.000000 pydvma-0.9.3/pydvma/acquisition.py
+-rw-rw-rw-   0        0        0    16393 2023-04-20 11:25:15.000000 pydvma-0.9.3/pydvma/analysis.py
+-rw-rw-rw-   0        0        0    30676 2023-04-21 09:57:55.000000 pydvma-0.9.3/pydvma/datastructure.py
+-rw-rw-rw-   0        0        0    16695 2023-04-19 14:11:21.000000 pydvma-0.9.3/pydvma/file.py
+-rw-rw-rw-   0        0        0   126497 2023-04-21 09:47:49.000000 pydvma-0.9.3/pydvma/gui.py
+-rw-rw-rw-   0        0        0     2815 2023-04-19 10:31:43.000000 pydvma-0.9.3/pydvma/gui_tk.py
+-rw-rw-rw-   0        0        0   144611 2023-04-19 10:31:43.000000 pydvma-0.9.3/pydvma/icon.png
+-rw-rw-rw-   0        0        0    10628 2023-04-20 11:25:15.000000 pydvma-0.9.3/pydvma/modal.py
+-rw-rw-rw-   0        0        0     8111 2023-04-21 09:24:50.000000 pydvma-0.9.3/pydvma/options.py
+-rw-rw-rw-   0        0        0    14944 2023-04-20 11:25:15.000000 pydvma-0.9.3/pydvma/oscilloscope.py
+-rw-rw-rw-   0        0        0    27763 2023-04-20 11:25:15.000000 pydvma-0.9.3/pydvma/plotting.py
+-rw-rw-rw-   0        0        0    26195 2023-04-21 09:57:37.000000 pydvma-0.9.3/pydvma/streams.py
+-rw-rw-rw-   0        0        0     2871 2023-04-20 11:25:15.000000 pydvma-0.9.3/pydvma/testdata.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:58:11.312683 pydvma-0.9.3/pydvma.egg-info/
+-rw-rw-rw-   0        0        0     3150 2023-04-21 09:58:11.000000 pydvma-0.9.3/pydvma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-04-21 09:58:11.000000 pydvma-0.9.3/pydvma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:58:11.000000 pydvma-0.9.3/pydvma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-21 09:58:11.000000 pydvma-0.9.3/pydvma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 09:58:11.000000 pydvma-0.9.3/pydvma.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 09:58:11.313694 pydvma-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-04-21 09:57:50.000000 pydvma-0.9.3/setup.py
```

### Comparing `pydvma-0.9.2/LICENSE` & `pydvma-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.2/PKG-INFO` & `pydvma-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydvma
-Version: 0.9.2
+Version: 0.9.3
 Home-page: https://github.com/torebutlin/pydvma
 Author: Tore Butlin
 Author-email: tb267@cam.ac.uk
 License: BSD 3-Clause License
 License-File: LICENSE
 
 # pydvma
```

### Comparing `pydvma-0.9.2/README.md` & `pydvma-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.2/pydvma/__init__.py` & `pydvma-0.9.3/pydvma/__init__.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.2/pydvma/acquisition.py` & `pydvma-0.9.3/pydvma/acquisition.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.2/pydvma/analysis.py` & `pydvma-0.9.3/pydvma/analysis.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.2/pydvma/datastructure.py` & `pydvma-0.9.3/pydvma/datastructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import numpy as np
 import datetime
 import uuid
 import copy
 
 #%% version
-VERSION = '0.9.2' # keep in sync with setup.py
+VERSION = '0.9.3' # keep in sync with setup.py
 
 def update_dataset(dataset):
     dataset_new = DataSet()
     dataset_new.add_to_dataset(dataset.time_data_list)
     dataset_new.add_to_dataset(dataset.freq_data_list)
     dataset_new.add_to_dataset(dataset.tf_data_list)
     dataset_new.add_to_dataset(dataset.cross_spec_data_list)
```

### Comparing `pydvma-0.9.2/pydvma/file.py` & `pydvma-0.9.3/pydvma/file.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.2/pydvma/gui.py` & `pydvma-0.9.3/pydvma/gui.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.2/pydvma/gui_tk.py` & `pydvma-0.9.3/pydvma/gui_tk.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.2/pydvma/icon.png` & `pydvma-0.9.3/pydvma/icon.png`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.2/pydvma/modal.py` & `pydvma-0.9.3/pydvma/modal.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.2/pydvma/options.py` & `pydvma-0.9.3/pydvma/options.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.2/pydvma/oscilloscope.py` & `pydvma-0.9.3/pydvma/oscilloscope.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.2/pydvma/plotting.py` & `pydvma-0.9.3/pydvma/plotting.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.2/pydvma/streams.py` & `pydvma-0.9.3/pydvma/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,15 +477,15 @@
     
         try:
             self.audio_stream.end_stream()
         except:
             pass
         
         # Make AutoRegN be one of set of possible numbers that works with nidaqmx
-        AutoRegN = int([10,100,1000])
+        AutoRegN = [int(n) for n in [10,100,1000]]
         check = np.where(AutoRegN <= settings.chunk_size)
         AutoRegN = AutoRegN[check[0][-1]]
         
         if settings.NI_mode == 'DAQmx_Val_RSE':
             pdaq_mode = pdaq.DAQmx_Val_RSE
         elif settings.NI_mode == 'DAQmx_Val_PseudoDiff':
             pdaq_mode = pdaq.DAQmx_Val_PseudoDiff
```

### Comparing `pydvma-0.9.2/pydvma/testdata.py` & `pydvma-0.9.3/pydvma/testdata.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.2/pydvma.egg-info/PKG-INFO` & `pydvma-0.9.3/pydvma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydvma
-Version: 0.9.2
+Version: 0.9.3
 Home-page: https://github.com/torebutlin/pydvma
 Author: Tore Butlin
 Author-email: tb267@cam.ac.uk
 License: BSD 3-Clause License
 License-File: LICENSE
 
 # pydvma
```

### Comparing `pydvma-0.9.2/setup.py` & `pydvma-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from setuptools import setup, find_packages
 
 requires = ['peakutils', 'numpy', 'scipy', 'pyqtgraph', 'matplotlib', 'seaborn', 'sounddevice']
 
 setup(
     name='pydvma',
-    version='0.9.2', # keep in sync with datastructure.py
+    version='0.9.3', # keep in sync with datastructure.py
     install_requires=requires,
     packages=['pydvma'],
     package_data={'': ['icon.png']},
     license='BSD 3-Clause License',
     long_description=open('README.md').read(),
     author='Tore Butlin',
     author_email='tb267@cam.ac.uk',
```

