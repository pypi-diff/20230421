# Comparing `tmp/minolz-1.1.tar.gz` & `tmp/minolz-2.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minolz-1.1.tar", last modified: Fri Apr 21 17:15:13 2023, max compression
+gzip compressed data, was "minolz-2.3b1.tar", last modified: Sun Apr 16 12:15:38 2023, max compression
```

## Comparing `minolz-1.1.tar` & `minolz-2.3b1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 17:15:13.585087 minolz-1.1/
--rw-rw-rw-   0        0        0     1195 2023-04-21 17:15:13.585087 minolz-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-04-21 17:13:17.000000 minolz-1.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 17:15:13.584087 minolz-1.1/minolz.egg-info/
--rw-rw-rw-   0        0        0     1195 2023-04-21 17:15:13.000000 minolz-1.1/minolz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-04-21 17:15:13.000000 minolz-1.1/minolz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 17:15:13.000000 minolz-1.1/minolz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 17:15:13.000000 minolz-1.1/minolz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13348 2023-04-21 17:13:28.000000 minolz-1.1/minolz.py
--rw-rw-rw-   0        0        0       42 2023-04-21 17:15:13.585087 minolz-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-04-21 17:13:02.000000 minolz-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:15:38.132706 minolz-2.3b1/
+-rw-rw-rw-   0        0        0     1205 2023-04-16 12:15:38.132706 minolz-2.3b1/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-04-16 12:05:39.000000 minolz-2.3b1/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 12:15:38.131695 minolz-2.3b1/minolz.egg-info/
+-rw-rw-rw-   0        0        0     1205 2023-04-16 12:15:38.000000 minolz-2.3b1/minolz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-04-16 12:15:38.000000 minolz-2.3b1/minolz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 12:15:38.000000 minolz-2.3b1/minolz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 12:15:38.000000 minolz-2.3b1/minolz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13354 2023-04-16 12:12:02.000000 minolz-2.3b1/minolz.py
+-rw-rw-rw-   0        0        0       42 2023-04-16 12:15:38.133716 minolz-2.3b1/setup.cfg
+-rw-rw-rw-   0        0        0     1168 2023-04-16 12:11:10.000000 minolz-2.3b1/setup.py
```

### Comparing `minolz-1.1/PKG-INFO` & `minolz-2.3b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: minolz
-Version: 1.1
+Version: 2.3b1
 Summary: A python library that can download any files in a few lines
-Home-page: http://liztochekcodesoon.epizy.com/
+Home-page: http://bitbucket.org/techtonik/python-wget/
 Author: liztochekcode <liztochekcode@gmail.com>
 License: Public Domain
 Classifier: Environment :: Console
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -35,10 +35,10 @@
 Alternative progress bar:
 
   >>> minolz.download(url, bar=bar_thermometer)
 
 
 ChangeLog
 
-0.5 (2023-04-21)
+0.1 (2023-04-16)
  * release
```

### Comparing `minolz-1.1/minolz.egg-info/PKG-INFO` & `minolz-2.3b1/minolz.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: minolz
-Version: 1.1
+Version: 2.3b1
 Summary: A python library that can download any files in a few lines
-Home-page: http://liztochekcodesoon.epizy.com/
+Home-page: http://bitbucket.org/techtonik/python-wget/
 Author: liztochekcode <liztochekcode@gmail.com>
 License: Public Domain
 Classifier: Environment :: Console
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -35,10 +35,10 @@
 Alternative progress bar:
 
   >>> minolz.download(url, bar=bar_thermometer)
 
 
 ChangeLog
 
-0.5 (2023-04-21)
+0.1 (2023-04-16)
  * release
```

### Comparing `minolz-1.1/minolz.py` & `minolz-2.3b1/minolz.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   import urllib.request as urllib
   import urllib.parse as urlparse
 else:
   import urllib
   import urlparse
 
 
-__version__ = "1.1"
+__version__ = "2.3-beta1"
 
 
 def filename_from_url(url):
     """:return: detected filename or None"""
     fname = os.path.basename(urlparse.urlparse(url).path)
     if len(fname.strip(" \n\t.")) == 0:
         return None
```

### Comparing `minolz-1.1/setup.py` & `minolz-2.3b1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             elif "'" in line:
                 return line.split("'")[1]
 
 setup(
     name='minolz',
     version=get_version('minolz.py'),
     author='liztochekcode <liztochekcode@gmail.com>',
-    url='http://liztochekcodesoon.epizy.com/',
+    url='http://bitbucket.org/techtonik/python-wget/',
 
     description="A python library that can download any files in a few lines",
     license="Public Domain",
     classifiers=[
         'Environment :: Console',
         'License :: Public Domain',
         'Operating System :: OS Independent',
```

