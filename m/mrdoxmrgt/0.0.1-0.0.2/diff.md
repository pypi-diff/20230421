# Comparing `tmp/mrdoxmrgt-0.0.1.tar.gz` & `tmp/mrdoxmrgt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrdoxmrgt-0.0.1.tar", last modified: Fri Apr 21 18:38:42 2023, max compression
+gzip compressed data, was "mrdoxmrgt-0.0.2.tar", last modified: Fri Apr 21 18:41:43 2023, max compression
```

## Comparing `mrdoxmrgt-0.0.1.tar` & `mrdoxmrgt-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 18:38:42.000000 mrdoxmrgt-0.0.1/
--rw-rw-rw-   0        0        0     1083 2023-04-20 14:15:02.000000 mrdoxmrgt-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      810 2023-04-21 18:38:42.000000 mrdoxmrgt-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-04-20 14:15:34.000000 mrdoxmrgt-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 18:38:42.000000 mrdoxmrgt-0.0.1/mrdoxmrgt/
--rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.1/mrdoxmrgt/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-04-21 18:03:58.000000 mrdoxmrgt-0.0.1/mrdoxmrgt/_main_.py
--rw-rw-rw-   0        0        0     3069 2023-04-21 18:06:14.000000 mrdoxmrgt-0.0.1/mrdoxmrgt/install.py
--rw-rw-rw-   0        0        0     1346 2023-04-21 18:03:38.000000 mrdoxmrgt-0.0.1/mrdoxmrgt/run.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:38:42.000000 mrdoxmrgt-0.0.1/mrdoxmrgt.egg-info/
--rw-rw-rw-   0        0        0      810 2023-04-21 18:38:42.000000 mrdoxmrgt-0.0.1/mrdoxmrgt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-21 18:38:42.000000 mrdoxmrgt-0.0.1/mrdoxmrgt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 18:38:42.000000 mrdoxmrgt-0.0.1/mrdoxmrgt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-04-21 18:38:42.000000 mrdoxmrgt-0.0.1/mrdoxmrgt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 18:38:42.000000 mrdoxmrgt-0.0.1/mrdoxmrgt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 18:38:42.000000 mrdoxmrgt-0.0.1/mrdoxmrgt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 18:38:42.000000 mrdoxmrgt-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1245 2023-04-21 17:54:44.000000 mrdoxmrgt-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-04-20 14:15:02.000000 mrdoxmrgt-0.0.2/LICENCE
+-rw-rw-rw-   0        0        0      810 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-20 14:15:34.000000 mrdoxmrgt-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt/
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:55:06.000000 mrdoxmrgt-0.0.2/mrdoxmrgt/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-04-21 18:03:58.000000 mrdoxmrgt-0.0.2/mrdoxmrgt/_main_.py
+-rw-rw-rw-   0        0        0     3069 2023-04-21 18:06:14.000000 mrdoxmrgt-0.0.2/mrdoxmrgt/install.py
+-rw-rw-rw-   0        0        0     1346 2023-04-21 18:03:38.000000 mrdoxmrgt-0.0.2/mrdoxmrgt/run.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/
+-rw-rw-rw-   0        0        0      810 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 18:41:44.000000 mrdoxmrgt-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2023-04-21 18:41:22.000000 mrdoxmrgt-0.0.2/setup.py
```

### Comparing `mrdoxmrgt-0.0.1/LICENCE` & `mrdoxmrgt-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.1/PKG-INFO` & `mrdoxmrgt-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/SMS_Forwarder
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.0.1/mrdoxmrgt/_main_.py` & `mrdoxmrgt-0.0.2/mrdoxmrgt/_main_.py`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.1/mrdoxmrgt/install.py` & `mrdoxmrgt-0.0.2/mrdoxmrgt/install.py`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.1/mrdoxmrgt/run.py` & `mrdoxmrgt-0.0.2/mrdoxmrgt/run.py`

 * *Files identical despite different names*

### Comparing `mrdoxmrgt-0.0.1/mrdoxmrgt.egg-info/PKG-INFO` & `mrdoxmrgt-0.0.2/mrdoxmrgt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrdoxmrgt
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/GreyTechno/SMS_Forwarder
 Download-URL: https://github.com/GreyTechno/gtf/archive/pypi.zip
 Author: MR_GT
 Author-email: friendyt89@gmail.com
 License: GPL
 Keywords: a1,a2,a3,a3,a4,a5,a6,a7,a8,a9
```

### Comparing `mrdoxmrgt-0.0.1/setup.py` & `mrdoxmrgt-0.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mrdoxmrgt',
     packages=find_packages(),
     include_package_data=True,
-    version="0.0.1",
+    version="0.0.2",
     description='A small example package',
     long_description="A small example package HI",
     long_description_content_type="text/markdown",
     author='MR_GT',
     author_email='friendyt89@gmail.com',
     url='https://github.com/GreyTechno/SMS_Forwarder',
     download_url="https://github.com/GreyTechno/gtf/archive/pypi.zip",
@@ -23,12 +23,12 @@
             'Operating System :: OS Independent',
             'Environment :: Console',
     ],
     install_requires=["requests"],
     license='GPL',
     entry_points={
             'console_scripts': [
-                'mrdoxmrgt = mrdoxmrgt.commands:main',
+                'mrdoxmrgt = mrdoxmrgt._main_:main',
             ],
     },
     python_requires='>=3.5'
 )
```

