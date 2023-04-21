# Comparing `tmp/synthdid-0.9.4.tar.gz` & `tmp/synthdid-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\synthdid-0.9.4.tar", last modified: Fri Apr 21 18:46:39 2023, max compression
+gzip compressed data, was "dist\synthdid-0.9.5.tar", last modified: Fri Apr 21 18:48:46 2023, max compression
```

## Comparing `synthdid-0.9.4.tar` & `synthdid-0.9.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 18:46:39.599051 synthdid-0.9.4/
--rw-rw-rw-   0        0        0     9195 2023-04-21 18:46:39.598048 synthdid-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-21 18:46:39.599051 synthdid-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0     1857 2023-04-21 18:46:18.000000 synthdid-0.9.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:46:39.584050 synthdid-0.9.4/synthdid/
--rw-rw-rw-   0        0        0        0 2023-04-17 22:50:30.000000 synthdid-0.9.4/synthdid/__init__.py
--rw-rw-rw-   0        0        0     1701 2023-04-17 22:50:30.000000 synthdid-0.9.4/synthdid/get_data.py
--rw-rw-rw-   0        0        0     3520 2023-04-17 22:50:30.000000 synthdid-0.9.4/synthdid/placebo_simulations.py
--rw-rw-rw-   0        0        0     6127 2023-04-18 02:08:10.000000 synthdid-0.9.4/synthdid/plots.py
--rw-rw-rw-   0        0        0     9303 2023-04-17 22:50:30.000000 synthdid-0.9.4/synthdid/sdid.py
--rw-rw-rw-   0        0        0     5439 2023-04-17 22:50:30.000000 synthdid-0.9.4/synthdid/solver.py
--rw-rw-rw-   0        0        0      410 2023-04-18 01:36:21.000000 synthdid-0.9.4/synthdid/summary.py
--rw-rw-rw-   0        0        0      792 2023-04-18 01:32:26.000000 synthdid-0.9.4/synthdid/synthdid.py
--rw-rw-rw-   0        0        0     3610 2023-04-17 22:50:30.000000 synthdid-0.9.4/synthdid/utils.py
--rw-rw-rw-   0        0        0     5043 2023-04-17 22:50:30.000000 synthdid-0.9.4/synthdid/vcov.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:46:39.597049 synthdid-0.9.4/synthdid.egg-info/
--rw-rw-rw-   0        0        0     9195 2023-04-21 18:46:39.000000 synthdid-0.9.4/synthdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-04-21 18:46:39.000000 synthdid-0.9.4/synthdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 18:46:39.000000 synthdid-0.9.4/synthdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      623 2023-04-21 18:46:39.000000 synthdid-0.9.4/synthdid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 18:46:39.000000 synthdid-0.9.4/synthdid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 18:48:46.096260 synthdid-0.9.5/
+-rw-rw-rw-   0        0        0      544 2023-04-21 18:48:46.096260 synthdid-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-21 18:48:46.096260 synthdid-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     1863 2023-04-21 18:48:43.000000 synthdid-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:48:46.087260 synthdid-0.9.5/synthdid/
+-rw-rw-rw-   0        0        0        0 2023-04-17 22:50:30.000000 synthdid-0.9.5/synthdid/__init__.py
+-rw-rw-rw-   0        0        0     1701 2023-04-17 22:50:30.000000 synthdid-0.9.5/synthdid/get_data.py
+-rw-rw-rw-   0        0        0     3520 2023-04-17 22:50:30.000000 synthdid-0.9.5/synthdid/placebo_simulations.py
+-rw-rw-rw-   0        0        0     6127 2023-04-18 02:08:10.000000 synthdid-0.9.5/synthdid/plots.py
+-rw-rw-rw-   0        0        0     9303 2023-04-17 22:50:30.000000 synthdid-0.9.5/synthdid/sdid.py
+-rw-rw-rw-   0        0        0     5439 2023-04-17 22:50:30.000000 synthdid-0.9.5/synthdid/solver.py
+-rw-rw-rw-   0        0        0      410 2023-04-18 01:36:21.000000 synthdid-0.9.5/synthdid/summary.py
+-rw-rw-rw-   0        0        0      792 2023-04-18 01:32:26.000000 synthdid-0.9.5/synthdid/synthdid.py
+-rw-rw-rw-   0        0        0     3610 2023-04-17 22:50:30.000000 synthdid-0.9.5/synthdid/utils.py
+-rw-rw-rw-   0        0        0     5043 2023-04-17 22:50:30.000000 synthdid-0.9.5/synthdid/vcov.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:48:46.095260 synthdid-0.9.5/synthdid.egg-info/
+-rw-rw-rw-   0        0        0      544 2023-04-21 18:48:46.000000 synthdid-0.9.5/synthdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-04-21 18:48:46.000000 synthdid-0.9.5/synthdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 18:48:46.000000 synthdid-0.9.5/synthdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      623 2023-04-21 18:48:46.000000 synthdid-0.9.5/synthdid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 18:48:46.000000 synthdid-0.9.5/synthdid.egg-info/top_level.txt
```

### Comparing `synthdid-0.9.4/setup.py` & `synthdid-0.9.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
-with open("./Readme.md", "r", encoding="utf-8") as f:
-    long_description = f.read()
+# with open("./Readme.md", "r", encoding="utf-8") as f:
+#     long_description = f.read()
 
 setup(
     dependency_links=[],
     install_requires=[
         "appdirs==1.4.3",
         "attrs==19.1.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
         "black==19.3b0; python_version >= '3.6'",
@@ -30,17 +30,17 @@
         "six==1.16.0",
         "statsmodels==0.13.5",
         "toml==0.10.0",
         "zipp==3.15.0",
     ],
     name="synthdid",
     author="D2CML Team, Alexander Quispe, Rodrigo  Grijalba, Jhon Flores, Franco Caceres",
-    version="0.9.4",
+    version="0.9.5",
     packages=find_packages(),
-    long_description=long_description,
+    # long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="causal-inference",
     url="https://github.com/d2cml-ai/synthdid.py",
     license="MIT",
     description="Synthdid",
     classifiers=[
         "Intended Audience :: Developers",
```

### Comparing `synthdid-0.9.4/synthdid/get_data.py` & `synthdid-0.9.5/synthdid/get_data.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.4/synthdid/placebo_simulations.py` & `synthdid-0.9.5/synthdid/placebo_simulations.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.4/synthdid/plots.py` & `synthdid-0.9.5/synthdid/plots.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.4/synthdid/sdid.py` & `synthdid-0.9.5/synthdid/sdid.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.4/synthdid/solver.py` & `synthdid-0.9.5/synthdid/solver.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.4/synthdid/synthdid.py` & `synthdid-0.9.5/synthdid/synthdid.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.4/synthdid/utils.py` & `synthdid-0.9.5/synthdid/utils.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.4/synthdid/vcov.py` & `synthdid-0.9.5/synthdid/vcov.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.4/synthdid.egg-info/requires.txt` & `synthdid-0.9.5/synthdid.egg-info/requires.txt`

 * *Files identical despite different names*

