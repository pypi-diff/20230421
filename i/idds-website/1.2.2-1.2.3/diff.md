# Comparing `tmp/idds-website-1.2.2.tar.gz` & `tmp/idds-website-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-website-1.2.2.tar", last modified: Wed Apr 19 10:36:01 2023, max compression
+gzip compressed data, was "idds-website-1.2.3.tar", last modified: Fri Apr 21 12:33:21 2023, max compression
```

## Comparing `idds-website-1.2.2.tar` & `idds-website-1.2.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.214243 idds-website-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-19 10:35:37.000000 idds-website-1.2.2/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-19 10:36:01.214243 idds-website-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 10:35:37.000000 idds-website-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.206243 idds-website-1.2.2/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.206243 idds-website-1.2.2/data/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.206243 idds-website-1.2.2/data/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)    29063 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/assets/css/font-awesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    79155 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/assets/css/main.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.206243 idds-website-1.2.2/data/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   124988 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/assets/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/assets/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   391622 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/assets/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   152796 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/assets/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    90412 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/assets/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    71896 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/assets/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.206243 idds-website-1.2.2/data/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)    95957 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/assets/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/assets/js/jquery.scrollex.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/assets/js/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/assets/js/skel.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/assets/js/util.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.214243 idds-website-1.2.2/data/images/
--rw-r--r--   0 runner    (1001) docker     (123)   474892 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/bg.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19506 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/idds.png
--rw-r--r--   0 runner    (1001) docker     (123)   185271 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/idds_architecture.png
--rw-r--r--   0 runner    (1001) docker     (123)   207445 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/idds_components.png
--rw-r--r--   0 runner    (1001) docker     (123)   291395 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/idds_delivery.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   351386 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/idds_full.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   216628 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/idds_intelligent.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   245328 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/idds_main.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   102173 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/idds_orchestration.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   191197 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/idds_transform.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/images.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62680 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/pic01.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    73227 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/pic02.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    51569 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/pic03.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    55020 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/pic04.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   575353 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/slide01.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   343913 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/slide02.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   547740 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/slide03.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   351032 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/slide04.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   505742 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/images/slide05.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-04-19 10:35:37.000000 idds-website-1.2.2/data/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.206243 idds-website-1.2.2/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.214243 idds-website-1.2.2/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 10:35:37.000000 idds-website-1.2.2/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.214243 idds-website-1.2.2/lib/idds/website/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 10:35:37.000000 idds-website-1.2.2/lib/idds/website/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-19 10:35:53.000000 idds-website-1.2.2/lib/idds/website/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:01.214243 idds-website-1.2.2/lib/idds_website.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-19 10:36:01.000000 idds-website-1.2.2/lib/idds_website.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-19 10:36:01.000000 idds-website-1.2.2/lib/idds_website.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:36:01.000000 idds-website-1.2.2/lib/idds_website.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 10:36:01.000000 idds-website-1.2.2/lib/idds_website.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 10:36:01.214243 idds-website-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-19 10:35:37.000000 idds-website-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.942738 idds-website-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-21 12:33:07.000000 idds-website-1.2.3/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-21 12:33:21.942738 idds-website-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-21 12:33:07.000000 idds-website-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.930738 idds-website-1.2.3/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.930738 idds-website-1.2.3/data/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.930738 idds-website-1.2.3/data/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    29063 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/assets/css/font-awesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    79155 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/assets/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.934738 idds-website-1.2.3/data/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   124988 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/assets/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/assets/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   391622 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/assets/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   152796 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/assets/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    90412 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/assets/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    71896 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/assets/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.934738 idds-website-1.2.3/data/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    95957 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/assets/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/assets/js/jquery.scrollex.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/assets/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/assets/js/skel.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/assets/js/util.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.938738 idds-website-1.2.3/data/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   474892 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/bg.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19506 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/idds.png
+-rw-r--r--   0 runner    (1001) docker     (123)   185271 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/idds_architecture.png
+-rw-r--r--   0 runner    (1001) docker     (123)   207445 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/idds_components.png
+-rw-r--r--   0 runner    (1001) docker     (123)   291395 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/idds_delivery.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   351386 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/idds_full.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   216628 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/idds_intelligent.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   245328 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/idds_main.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   102173 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/idds_orchestration.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   191197 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/idds_transform.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/images.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62680 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/pic01.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    73227 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/pic02.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    51569 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/pic03.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    55020 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/pic04.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   575353 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/slide01.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   343913 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/slide02.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   547740 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/slide03.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   351032 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/slide04.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   505742 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/images/slide05.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-04-21 12:33:07.000000 idds-website-1.2.3/data/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.930738 idds-website-1.2.3/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.938738 idds-website-1.2.3/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 12:33:07.000000 idds-website-1.2.3/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.938738 idds-website-1.2.3/lib/idds/website/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 12:33:07.000000 idds-website-1.2.3/lib/idds/website/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-21 12:33:15.000000 idds-website-1.2.3/lib/idds/website/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.942738 idds-website-1.2.3/lib/idds_website.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-21 12:33:21.000000 idds-website-1.2.3/lib/idds_website.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-21 12:33:21.000000 idds-website-1.2.3/lib/idds_website.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:33:21.000000 idds-website-1.2.3/lib/idds_website.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 12:33:21.000000 idds-website-1.2.3/lib/idds_website.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-21 12:33:21.942738 idds-website-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-21 12:33:07.000000 idds-website-1.2.3/setup.py
```

### Comparing `idds-website-1.2.2/LICENSE.rst` & `idds-website-1.2.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/PKG-INFO` & `idds-website-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-website
-Version: 1.2.2
+Version: 1.2.3
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-website-1.2.2/data/assets/css/font-awesome.min.css` & `idds-website-1.2.3/data/assets/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/assets/css/main.css` & `idds-website-1.2.3/data/assets/css/main.css`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/assets/fonts/FontAwesome.otf` & `idds-website-1.2.3/data/assets/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/assets/fonts/fontawesome-webfont.eot` & `idds-website-1.2.3/data/assets/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/assets/fonts/fontawesome-webfont.svg` & `idds-website-1.2.3/data/assets/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/assets/fonts/fontawesome-webfont.ttf` & `idds-website-1.2.3/data/assets/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/assets/fonts/fontawesome-webfont.woff` & `idds-website-1.2.3/data/assets/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/assets/fonts/fontawesome-webfont.woff2` & `idds-website-1.2.3/data/assets/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/assets/js/jquery.min.js` & `idds-website-1.2.3/data/assets/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/assets/js/jquery.scrollex.min.js` & `idds-website-1.2.3/data/assets/js/jquery.scrollex.min.js`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/assets/js/main.js` & `idds-website-1.2.3/data/assets/js/main.js`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/assets/js/skel.min.js` & `idds-website-1.2.3/data/assets/js/skel.min.js`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/assets/js/util.js` & `idds-website-1.2.3/data/assets/js/util.js`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/bg.jpg` & `idds-website-1.2.3/data/images/bg.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/idds.png` & `idds-website-1.2.3/data/images/idds.png`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/idds_architecture.png` & `idds-website-1.2.3/data/images/idds_architecture.png`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/idds_components.png` & `idds-website-1.2.3/data/images/idds_components.png`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/idds_delivery.jpg` & `idds-website-1.2.3/data/images/idds_delivery.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/idds_full.jpg` & `idds-website-1.2.3/data/images/idds_full.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/idds_intelligent.jpg` & `idds-website-1.2.3/data/images/idds_intelligent.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/idds_main.jpg` & `idds-website-1.2.3/data/images/idds_main.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/idds_orchestration.jpg` & `idds-website-1.2.3/data/images/idds_orchestration.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/idds_transform.jpg` & `idds-website-1.2.3/data/images/idds_transform.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/images.jpg` & `idds-website-1.2.3/data/images/images.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/pic01.jpg` & `idds-website-1.2.3/data/images/pic01.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/pic02.jpg` & `idds-website-1.2.3/data/images/pic02.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/pic03.jpg` & `idds-website-1.2.3/data/images/pic03.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/pic04.jpg` & `idds-website-1.2.3/data/images/pic04.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/slide01.jpg` & `idds-website-1.2.3/data/images/slide01.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/slide02.jpg` & `idds-website-1.2.3/data/images/slide02.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/slide03.jpg` & `idds-website-1.2.3/data/images/slide03.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/slide04.jpg` & `idds-website-1.2.3/data/images/slide04.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/images/slide05.jpg` & `idds-website-1.2.3/data/images/slide05.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/data/index.html` & `idds-website-1.2.3/data/index.html`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/lib/idds_website.egg-info/PKG-INFO` & `idds-website-1.2.3/lib/idds_website.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-website
-Version: 1.2.2
+Version: 1.2.3
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-website-1.2.2/lib/idds_website.egg-info/SOURCES.txt` & `idds-website-1.2.3/lib/idds_website.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-website-1.2.2/setup.py` & `idds-website-1.2.3/setup.py`

 * *Files identical despite different names*

