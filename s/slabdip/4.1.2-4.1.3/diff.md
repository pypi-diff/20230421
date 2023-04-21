# Comparing `tmp/slabdip-4.1.2.tar.gz` & `tmp/slabdip-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slabdip-4.1.2.tar", last modified: Tue Apr 18 11:52:18 2023, max compression
+gzip compressed data, was "slabdip-4.1.3.tar", last modified: Fri Apr 21 00:49:51 2023, max compression
```

## Comparing `slabdip-4.1.2.tar` & `slabdip-4.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:52:18.888452 slabdip-4.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-18 11:52:04.000000 slabdip-4.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-18 11:52:18.888452 slabdip-4.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-18 11:52:04.000000 slabdip-4.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 11:52:18.888452 slabdip-4.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-18 11:52:04.000000 slabdip-4.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:52:18.884452 slabdip-4.1.2/slabdip/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 11:52:04.000000 slabdip-4.1.2/slabdip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:52:18.884452 slabdip-4.1.2/slabdip/data/
--rw-r--r--   0 runner    (1001) docker     (123)   547866 2023-04-18 11:52:04.000000 slabdip-4.1.2/slabdip/data/subduction_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-04-18 11:52:04.000000 slabdip-4.1.2/slabdip/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:52:18.884452 slabdip-4.1.2/slabdip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-18 11:52:18.000000 slabdip-4.1.2/slabdip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-18 11:52:18.000000 slabdip-4.1.2/slabdip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:52:18.000000 slabdip-4.1.2/slabdip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-18 11:52:18.000000 slabdip-4.1.2/slabdip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 11:52:18.000000 slabdip-4.1.2/slabdip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.642512 slabdip-4.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-21 00:49:40.000000 slabdip-4.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-04-21 00:49:51.642512 slabdip-4.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-21 00:49:40.000000 slabdip-4.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 00:49:51.642512 slabdip-4.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-21 00:49:40.000000 slabdip-4.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.638512 slabdip-4.1.3/slabdip/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 00:49:40.000000 slabdip-4.1.3/slabdip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.642512 slabdip-4.1.3/slabdip/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   547866 2023-04-21 00:49:40.000000 slabdip-4.1.3/slabdip/data/subduction_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-04-21 00:49:40.000000 slabdip-4.1.3/slabdip/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.642512 slabdip-4.1.3/slabdip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-04-21 00:49:51.000000 slabdip-4.1.3/slabdip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-21 00:49:51.000000 slabdip-4.1.3/slabdip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:49:51.000000 slabdip-4.1.3/slabdip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 00:49:51.000000 slabdip-4.1.3/slabdip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 00:49:51.000000 slabdip-4.1.3/slabdip.egg-info/top_level.txt
```

### Comparing `slabdip-4.1.2/LICENSE` & `slabdip-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slabdip-4.1.2/PKG-INFO` & `slabdip-4.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slabdip
-Version: 4.1.2
+Version: 4.1.3
 Summary: Method to calculate slab dip using simple plate kinematic parameters
 Home-page: https://github.com/brmather/Slab-Dip
 Author: Ben Mather
 Author-email: ben.mather@sydney.edu.au
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
@@ -34,14 +34,15 @@
 ## Dependencies
 
 To run the Jupyter notebooks some dependencies are required:
 
 - [pygplates](https://www.gplates.org/download/)
 - [gplately](https://github.com/GPlates/gplately)
 - [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools/tree/master/ptt)
+- [Scikit-Learn](https://scikit-learn.org)
 - [cartopy](https://scitools.org.uk/cartopy/docs/latest/installing.html) (for mapping)
 - [netCDF4](https://pypi.org/project/netCDF4/) (to extract age grids of the seafloor)
 
 Instructions to install these dependencies can be found within each package above.
 Some conda instructions for setting up a Python environment are [here](https://www.benmather.info/post/2022-07-07-python-for-mac-m1/). While these have been written with the Mac M1 architecture in mind, the same instructions should apply equally to other distributions.
 
 ## Installation
```

### Comparing `slabdip-4.1.2/README.md` & `slabdip-4.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ## Dependencies
 
 To run the Jupyter notebooks some dependencies are required:
 
 - [pygplates](https://www.gplates.org/download/)
 - [gplately](https://github.com/GPlates/gplately)
 - [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools/tree/master/ptt)
+- [Scikit-Learn](https://scikit-learn.org)
 - [cartopy](https://scitools.org.uk/cartopy/docs/latest/installing.html) (for mapping)
 - [netCDF4](https://pypi.org/project/netCDF4/) (to extract age grids of the seafloor)
 
 Instructions to install these dependencies can be found within each package above.
 Some conda instructions for setting up a Python environment are [here](https://www.benmather.info/post/2022-07-07-python-for-mac-m1/). While these have been written with the Mac M1 architecture in mind, the same instructions should apply equally to other distributions.
 
 ## Installation
```

### Comparing `slabdip-4.1.2/setup.py` & `slabdip-4.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 this_directory = path.abspath(path.dirname(__file__))
 with io.open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 if __name__ == "__main__":
     setup(
         name='slabdip',
-        version='4.1.2',
+        version='4.1.3',
         description='Method to calculate slab dip using simple plate kinematic parameters',
         long_description=long_description,
         long_description_content_type='text/markdown',
         author='Ben Mather',
         author_email='ben.mather@sydney.edu.au',
         url='https://github.com/brmather/Slab-Dip',
         install_requires=[
             'pandas',
             'numpy',
-            'gplately >= 0.4'
+            'scikit-learn',
+            'gplately >= 1.0'
         ],
         extras_require={'plotting': ['matplotlib', 'jupyter', 'cartopy']},
         packages=['slabdip'],
         package_data={'slabdip': ['data/subduction_data.csv']},
         include_package_data = True,
         classifiers     = ['Programming Language :: Python :: 2',
                            'Programming Language :: Python :: 2.6',
```

### Comparing `slabdip-4.1.2/slabdip/data/subduction_data.csv` & `slabdip-4.1.3/slabdip/data/subduction_data.csv`

 * *Files identical despite different names*

### Comparing `slabdip-4.1.2/slabdip/predictor.py` & `slabdip-4.1.3/slabdip/predictor.py`

 * *Files identical despite different names*

### Comparing `slabdip-4.1.2/slabdip.egg-info/PKG-INFO` & `slabdip-4.1.3/slabdip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slabdip
-Version: 4.1.2
+Version: 4.1.3
 Summary: Method to calculate slab dip using simple plate kinematic parameters
 Home-page: https://github.com/brmather/Slab-Dip
 Author: Ben Mather
 Author-email: ben.mather@sydney.edu.au
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
@@ -34,14 +34,15 @@
 ## Dependencies
 
 To run the Jupyter notebooks some dependencies are required:
 
 - [pygplates](https://www.gplates.org/download/)
 - [gplately](https://github.com/GPlates/gplately)
 - [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools/tree/master/ptt)
+- [Scikit-Learn](https://scikit-learn.org)
 - [cartopy](https://scitools.org.uk/cartopy/docs/latest/installing.html) (for mapping)
 - [netCDF4](https://pypi.org/project/netCDF4/) (to extract age grids of the seafloor)
 
 Instructions to install these dependencies can be found within each package above.
 Some conda instructions for setting up a Python environment are [here](https://www.benmather.info/post/2022-07-07-python-for-mac-m1/). While these have been written with the Mac M1 architecture in mind, the same instructions should apply equally to other distributions.
 
 ## Installation
```

