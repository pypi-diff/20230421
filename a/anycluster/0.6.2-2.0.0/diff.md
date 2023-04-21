# Comparing `tmp/anycluster-0.6.2.tar.gz` & `tmp/anycluster-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anycluster-0.6.2.tar", last modified: Mon Dec 30 14:04:32 2019, max compression
+gzip compressed data, was "anycluster-2.0.0.tar", last modified: Fri Apr 21 13:23:56 2023, max compression
```

## Comparing `anycluster-0.6.2.tar` & `anycluster-2.0.0.tar`

### file list

```diff
@@ -1,45 +1,70 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-30 14:04:32.000000 anycluster-0.6.2/
--rw-r--r--   0 tom       (1000) tom       (1000)      113 2019-09-04 07:49:56.000000 anycluster-0.6.2/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)     3427 2019-12-30 14:04:32.000000 anycluster-0.6.2/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2326 2019-09-09 13:09:42.000000 anycluster-0.6.2/README.md
--rw-r--r--   0 tom       (1000) tom       (1000)     1078 2019-09-04 09:08:55.000000 anycluster-0.6.2/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2019-12-30 14:04:32.000000 anycluster-0.6.2/setup.cfg
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-30 14:04:32.000000 anycluster-0.6.2/anycluster/
--rw-r--r--   0 tom       (1000) tom       (1000)     2953 2019-09-16 14:44:43.000000 anycluster-0.6.2/anycluster/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)      383 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/tests.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16529 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/globalmaptiles.py
--rw-r--r--   0 tom       (1000) tom       (1000)      586 2019-09-06 09:25:26.000000 anycluster-0.6.2/anycluster/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-30 14:04:32.000000 anycluster-0.6.2/anycluster/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-30 14:04:32.000000 anycluster-0.6.2/anycluster/static/anycluster/
--rw-r--r--   0 tom       (1000) tom       (1000)    22914 2019-09-16 14:43:40.000000 anycluster-0.6.2/anycluster/static/anycluster/anycluster.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3262 2019-09-13 12:04:21.000000 anycluster-0.6.2/anycluster/static/anycluster/anycluster_marker.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1265 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/static/anycluster/django_ajax_csrf.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-30 14:04:32.000000 anycluster-0.6.2/anycluster/static/anycluster/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     1023 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/static/anycluster/images/50_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1409 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/static/anycluster/images/10000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/static/anycluster/images/10.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2093 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/static/anycluster/images/1000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1974 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/static/anycluster/images/50.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1034 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/static/anycluster/images/100_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      784 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/static/anycluster/images/10_empty.png
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/static/anycluster/images/pin_unknown.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2811 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/static/anycluster/images/10000.png
--rw-r--r--   0 tom       (1000) tom       (1000)      749 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/static/anycluster/images/5_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1912 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/static/anycluster/images/100.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1262 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/static/anycluster/images/1000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1253 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/static/anycluster/images/5.png
--rw-r--r--   0 tom       (1000) tom       (1000)      540 2019-09-09 13:44:25.000000 anycluster-0.6.2/anycluster/static/anycluster/anycluster.css
--rw-r--r--   0 tom       (1000) tom       (1000)    32869 2019-10-09 14:56:12.000000 anycluster-0.6.2/anycluster/MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10626 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/MapTools.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-30 14:04:32.000000 anycluster-0.6.2/anycluster/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-30 14:04:32.000000 anycluster-0.6.2/anycluster/templates/anycluster/
--rw-r--r--   0 tom       (1000) tom       (1000)       74 2019-09-04 07:49:56.000000 anycluster-0.6.2/anycluster/templates/anycluster/clusterPopup.html
--rw-rw-r--   0 tom       (1000) tom       (1000)     1142 2019-09-13 13:58:22.000000 anycluster-0.6.2/anycluster/clusters.py
--rw-r--r--   0 tom       (1000) tom       (1000)      945 2019-12-30 14:02:42.000000 anycluster-0.6.2/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2019-12-30 14:04:32.000000 anycluster-0.6.2/anycluster.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     3427 2019-12-30 14:04:32.000000 anycluster-0.6.2/anycluster.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2019-12-30 14:04:32.000000 anycluster-0.6.2/anycluster.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)     1241 2019-12-30 14:04:32.000000 anycluster-0.6.2/anycluster.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       11 2019-12-30 14:04:32.000000 anycluster-0.6.2/anycluster.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        9 2019-12-30 14:04:32.000000 anycluster-0.6.2/anycluster.egg-info/requires.txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.135873 anycluster-2.0.0/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.0.0/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-21 13:23:32.000000 anycluster-2.0.0/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)     2915 2023-04-21 13:23:56.135873 anycluster-2.0.0/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2326 2023-01-20 06:49:37.000000 anycluster-2.0.0/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.131873 anycluster-2.0.0/anycluster/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.0.0/anycluster/ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2680 2023-04-20 07:53:43.000000 anycluster-2.0.0/anycluster/FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    31624 2023-04-19 10:53:31.000000 anycluster-2.0.0/anycluster/MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.0.0/anycluster/MapTools.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.0.0/anycluster/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.131873 anycluster-2.0.0/anycluster/api/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.131873 anycluster-2.0.0/anycluster/api/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.0.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.0.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2592 2023-04-21 13:09:53.000000 anycluster-2.0.0/anycluster/api/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)      940 2023-03-17 13:31:29.000000 anycluster-2.0.0/anycluster/api/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     5797 2023-04-19 10:41:51.000000 anycluster-2.0.0/anycluster/api/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.0.0/anycluster/api/json_schemas.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2572 2023-04-21 13:09:52.000000 anycluster-2.0.0/anycluster/api/serializers.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.131873 anycluster-2.0.0/anycluster/api/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.135873 anycluster-2.0.0/anycluster/api/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.0.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1120 2023-03-17 13:45:55.000000 anycluster-2.0.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     6965 2023-04-19 19:03:37.000000 anycluster-2.0.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)      826 2023-03-02 13:13:55.000000 anycluster-2.0.0/anycluster/api/tests/test_serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9420 2023-04-19 19:03:34.000000 anycluster-2.0.0/anycluster/api/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      882 2023-03-17 13:31:28.000000 anycluster-2.0.0/anycluster/api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7179 2023-04-19 10:29:29.000000 anycluster-2.0.0/anycluster/api/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.0.0/anycluster/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/clusters.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.0.0/anycluster/definitions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/globalmaptiles.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.131873 anycluster-2.0.0/anycluster/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.131873 anycluster-2.0.0/anycluster/static/anycluster/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.135873 anycluster-2.0.0/anycluster/static/anycluster/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/10.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/100.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/1000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/10000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/10000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/1000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/100_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/10_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/5.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/50.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/50_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/5_empty.png
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/pin_unknown.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.135873 anycluster-2.0.0/anycluster/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.135873 anycluster-2.0.0/anycluster/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.0.0/anycluster/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2533 2023-04-19 10:53:00.000000 anycluster-2.0.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.0.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2790 2023-04-21 13:19:15.000000 anycluster-2.0.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.0.0/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    10728 2023-04-19 10:54:13.000000 anycluster-2.0.0/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.0.0/anycluster/tests/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2096 2023-04-19 10:47:07.000000 anycluster-2.0.0/anycluster/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.0.0/anycluster/tests/test_ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3995 2023-04-21 13:19:10.000000 anycluster-2.0.0/anycluster/tests/test_FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16495 2023-04-19 10:54:09.000000 anycluster-2.0.0/anycluster/tests/test_MapClusterer.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.131873 anycluster-2.0.0/anycluster.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2915 2023-04-21 13:23:56.000000 anycluster-2.0.0/anycluster.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2191 2023-04-21 13:23:56.000000 anycluster-2.0.0/anycluster.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-04-21 13:23:56.000000 anycluster-2.0.0/anycluster.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-04-21 13:23:56.000000 anycluster-2.0.0/anycluster.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-04-21 13:23:56.000000 anycluster-2.0.0/anycluster.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-04-21 13:23:56.135873 anycluster-2.0.0/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-04-21 13:20:38.000000 anycluster-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `anycluster-0.6.2/README.md` & `anycluster-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/LICENSE` & `anycluster-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/globalmaptiles.py` & `anycluster-2.0.0/anycluster/globalmaptiles.py`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/static/anycluster/images/50_empty.png` & `anycluster-2.0.0/anycluster/static/anycluster/images/50_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/static/anycluster/images/10000_empty.png` & `anycluster-2.0.0/anycluster/static/anycluster/images/10000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/static/anycluster/images/10.png` & `anycluster-2.0.0/anycluster/static/anycluster/images/10.png`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/static/anycluster/images/1000.png` & `anycluster-2.0.0/anycluster/static/anycluster/images/1000.png`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/static/anycluster/images/50.png` & `anycluster-2.0.0/anycluster/static/anycluster/images/50.png`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/static/anycluster/images/100_empty.png` & `anycluster-2.0.0/anycluster/static/anycluster/images/100_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/static/anycluster/images/10_empty.png` & `anycluster-2.0.0/anycluster/static/anycluster/images/10_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/static/anycluster/images/pin_unknown.png` & `anycluster-2.0.0/anycluster/static/anycluster/images/pin_unknown.png`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/static/anycluster/images/10000.png` & `anycluster-2.0.0/anycluster/static/anycluster/images/10000.png`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/static/anycluster/images/5_empty.png` & `anycluster-2.0.0/anycluster/static/anycluster/images/5_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/static/anycluster/images/100.png` & `anycluster-2.0.0/anycluster/static/anycluster/images/100.png`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/static/anycluster/images/1000_empty.png` & `anycluster-2.0.0/anycluster/static/anycluster/images/1000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/static/anycluster/images/5.png` & `anycluster-2.0.0/anycluster/static/anycluster/images/5.png`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/anycluster/MapClusterer.py` & `anycluster-2.0.0/anycluster/MapClusterer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,43 @@
-'''---------------------------------------------------------------------------------------
-
-DJANGO MAP CLUSTERING
-
+'''-------------------------------------------------------------------------------------------------------------------------
+SERVER SIDE MAP CLUSTERING
 - kmeans
 - grid
+-------------------------------------------------------------------------------------------------------------------------'''
 
-VERSION: 0.1
-AUTHOR: biodiv
-LICENSE: GPL
-
----------------------------------------------------------------------------------------'''
-
-'''--------------------------------------------------------------------------------------
+'''-------------------------------------------------------------------------------------------------------------------------
 
     WORKFLOW
 
     1. anycluster receives viewport coordinates from ajax query
     2. anycluster calculates map grid in pixels (coordinates -> mercator -> pixels)
     3a. (grid cluster) counts markers in each cell
     3b. (kmeans cluster) calculates k centroids for each cell
-    4a. (gridcluster) returns the cells as polygons (output srid = input srid) alongside the count
+    4a. (grid_cluster) returns the cells as polygons (output srid = input srid) alongside the count
     4b. (kmeans cluster) returns kmeans centroids (output srid = input srid)
 
---------------------------------------------------------------------------------------'''
+-------------------------------------------------------------------------------------------------------------------------'''
 
-'''--------------------------------------------------------------------------------------
+'''-------------------------------------------------------------------------------------------------------------------------
     A VIEWPORT is defined by topright bottomleft coordinates and the SRID of those coordinates
 
     4-------------a
     |             |
     |             |
     |             |
     b-------------2
 
     Polygon GEOS String:
     a -> 2 -> b -> 4 -> a
     
     GEOSGeometry('POLYGON((a.long a.lat, a.long b.lat, b.long b.lat, b.long a.lat, a.long a.lat))')
 
---------------------------------------------------------------------------------------'''
+-------------------------------------------------------------------------------------------------------------------------'''
 
-'''--------------------------------------------------------------------------------------
+'''-------------------------------------------------------------------------------------------------------------------------
     TILE BOUNDARY RESTRICTIONS
 
     WGS84 datum (longitude/latitude):
     -180 -85.05112877980659
     180 85.0511287798066
 
     Spherical Mercator (meters):
@@ -58,29 +51,30 @@
     Pixels at zoom 0 (default, depends on gridsize):
     0 0 256 256
 
     "World" is a system google uses internally
     World max: 40075016
     World min: 40075016
 
----------------------------------------------------------------------------------------'''
-
-import json, math, numbers, decimal
-from anycluster.MapTools import MapTools
-from django.contrib.gis.geos import Point, GEOSGeometry
-from django.contrib.gis.gdal import SpatialReference, CoordTransform
-from django.contrib.gis.db.models.fields import BaseSpatialField
-from django.db import connections
+-------------------------------------------------------------------------------------------------------------------------'''
 
-from django.conf import settings
-from django.db.models import Q, Min, ForeignKey
-from django.apps import apps
 
 from .clusters import PointCluster
+from django.apps import apps
+from django.db.models import ForeignKey
+from django.conf import settings
+from django.db import connections
+from django.contrib.gis.db.models.fields import BaseSpatialField
+from django.contrib.gis.gdal import SpatialReference, CoordTransform
+from django.contrib.gis.geos import Point, GEOSGeometry
+from anycluster import MapTools, ClusterCache, FilterComposer
+from anycluster.definitions import (CLUSTER_TYPE_KMEANS, CLUSTER_TYPE_GRID, GEOMETRY_TYPE_VIEWPORT, GEOMETRY_TYPE_AREA,
+                                    MAX_BOUNDS)
 
+import json, math
 BASE_K = getattr(settings, 'ANYCLUSTER_BASE_K', 6)
 K_CAP = getattr(settings, 'ANYCLUSTER_K_CAP', 30)
 
 # get the model as defined in settings
 geoapp, geomodel = settings.ANYCLUSTER_GEODJANGO_MODEL.split('.')
 geo_column_str = settings.ANYCLUSTER_COORDINATES_COLUMN
 
@@ -105,474 +99,413 @@
 Gis = app_config.get_model(geomodel)
 
 geo_table = Gis._meta.db_table
 
 
 class MapClusterer():
 
-    def __init__(self, request, zoom=1, gridSize=256, input_srid=4326, mapTileSize=256, schema_name='public'):
+    def __init__(self, cluster_cache, grid_size=256, maptile_size=256, output_srid=4326, schema_name='public'):
 
-        self.schema_name = schema_name
-        
-        # the srid of the coordinates coming from javascript. input_srid = output_srid
-        self.input_srid = int(input_srid)
-        # the srid of the database, falls back to 4326
-        self.db_srid = self.getDatabaseSRID()
+        self.cluster_cache = cluster_cache
 
         # the size of the grid in pixels. each grid cell gets its own kmeans clustering
-        self.gridSize = int(gridSize)
+        self.grid_size = int(grid_size)
 
-        self.zoom = int(zoom)
-        self.maptools = MapTools(int(mapTileSize))
+        self.output_srid = output_srid
+
+        self.schema_name = schema_name
+
+        # the srid of the database, falls back to 4326
+        self.db_srid = self.get_database_srid()
+
+        self.maptools = MapTools(int(maptile_size))
 
         # filter operators
         self.valid_operators = ['=', '<', '>', '<=', '>=', 'list', '!list']
 
-        self.request = request
-        self.params = self.loadJson(request)
-        self.cache = request.session.get("clustercache", {})
+    # read the srid of the database.
 
-    # read the srid of the database. 
-    def getDatabaseSRID(self):
+    def get_database_srid(self):
 
         db_srid = None
 
         srid_qry = 'SELECT id, ST_SRID({geo_column}) FROM {schema_name}.{geo_table} LIMIT 1;'.format(
             geo_column=geo_column_str, schema_name=self.schema_name, geo_table=geo_table)
 
         with connections['default'].cursor() as cursor:
             cursor.execute(srid_qry)
-        
+
             row = cursor.fetchone()
 
             if row and len(row) == 2:
                 db_srid = row[1]
-                
 
         if not db_srid:
             try:
                 db_srid = settings.ANYCLUSTER_COORDINATES_COLUMN_SRID
             except:
                 db_srid = 4326
-        
-        return db_srid
-
-    
-    '''---------------------------------------------------------------------------------------------------------------------------
-        LOADING THE AJAX INPUT
-
-        - The variables and filters coming from the ajax request are transformed into python-usables like lists and dictionaries
-        - anycluster receives a json object containing geojson and filters
-    ---------------------------------------------------------------------------------------------------------------------------'''   
-    def loadJson(self, request):
-        json_str = request.body.decode(encoding='UTF-8')
-        params = json.loads(json_str)
-
-        if "geojson" in params:
-            request.session['geojson'] = params['geojson']
-        
-        return params    
 
+        return db_srid
 
-    '''---------------------------------------------------------------------------------------------------------------------------------
+    '''---------------------------------------------------------------------------------------------------------------------
         CONVERTING QUADKEY CELLS TO POSTGIS USABLE POLYGONS
 
         - ST_Collect(geom)
         - create a geometry collection to reduce the database queries to 1
         - this is not yet working
-    ---------------------------------------------------------------------------------------------------------------------------------'''
-    def convertCellsToGEOS(self,cells):
+    ---------------------------------------------------------------------------------------------------------------------'''
+    '''
+    def convert_cells_to_geos(self, cells):
 
-        #ST_Collect(ST_GeomFromText('POINT(1 2)'),ST_GeomFromText('POINT(-2 3)') )
+        # ST_Collect(ST_GeomFromText('POINT(1 2)'),ST_GeomFromText('POINT(-2 3)') )
 
-        query_collection = "ST_Collect(ARRAY["
+        query_collection = 'ST_Collect(ARRAY['
 
         for counter, cell in enumerate(cells):
-            
-            poly = self.clusterCellToBounds(cell)
-                
+
+            poly = self.cluster_cell_to_bounds(cell)
+
             if counter > 0:
-                query_collection += ","
+                query_collection += ','
 
             # ST_GeomFromText('POLYGON((0 0, 10000 0, 10000 10000, 0 10000, 0 0))',3857)
-            query_collection += "ST_GeomFromText('{poly}', {srid})".format(poly=poly, srid=self.db_srid)
+            query_collection += "ST_GeomFromText('{poly}', {srid})".format(
+                poly=poly, srid=self.db_srid)
 
-        query_collection += "])"
+        query_collection += '])'
 
         return query_collection
-                
-
+    '''
 
-    '''---------------------------------------------------------------------------------------------------------------------------------
+    '''---------------------------------------------------------------------------------------------------------------------
         CONVERTING GEOJSON TO GEOS
 
         multipolygon and collections are not supported by ST_Within so they need to be split into several geometries
-    ---------------------------------------------------------------------------------------------------------------------------------'''
+    ---------------------------------------------------------------------------------------------------------------------'''
+    def get_srid_from_geojson_feature(self, geojson_feature):
 
-    # returns a list of polygons in GEOS format and db_srid
-    def convertGeojsonFeatureToGEOS(self, feature):
+        srid = 4326
+
+        if 'crs' in geojson_feature['geometry']:
+            srid_str = geojson_feature['geometry']['crs']['properties']['name']
+            srid = int(srid_str.split(':')[-1])
+
+        return srid
+
+    def convert_geojson_feature_to_geos(self, geojson_feature):
 
         geos_geometries = []
 
-        if "properties" in feature and "srid" in feature["properties"]:
-            srid = feature["properties"]["srid"]
-        else:
-            srid = 4326
+        input_srid = self.get_srid_from_geojson_feature(geojson_feature)
 
-        if feature["geometry"]["type"] == "MultiPolygon":
+        if geojson_feature['geometry']['type'] == 'MultiPolygon':
 
-            for polygon in feature["geometry"]["coordinates"]:
+            for polygon in geojson_feature['geometry']['coordinates']:
 
-                geom = { "type": "Polygon", "coordinates": [polygon[0]] }
+                geom = {
+                    'type': 'Polygon',
+                    'coordinates': [polygon]
+                }
 
-                geos = GEOSGeometry(json.dumps(geom), srid=srid)
-                
-                if geos.srid != self.db_srid: 
-                    ct = CoordTransform(SpatialReference(geos.srid), SpatialReference(self.db_srid))
+                geos = GEOSGeometry(json.dumps(geom), srid=input_srid)
+
+                if geos.srid != self.db_srid:
+                    ct = CoordTransform(SpatialReference(
+                        geos.srid), SpatialReference(self.db_srid))
                     geos.transform(ct)
 
                 geos_geometries.append(geos)
-                
 
         else:
-            
+
             try:
-                geos = GEOSGeometry(json.dumps(feature["geometry"]), srid=srid)
+                geos = GEOSGeometry(json.dumps(
+                    geojson_feature['geometry']), srid=input_srid)
             except:
-                raise TypeError("Invalid GEOJSON geometry for cluster area. Use Polygon or Multipolygon")
+                raise TypeError(
+                    'Invalid GEOJSON geometry for cluster area. Use Polygon or Multipolygon')
 
             if geos:
 
                 if geos.srid != self.db_srid:
-                    ct = CoordTransform(SpatialReference(geos.srid), SpatialReference(self.db_srid))
+                    ct = CoordTransform(SpatialReference(
+                        geos.srid), SpatialReference(self.db_srid))
                     geos.transform(ct)
-                
+
                 geos_geometries.append(geos)
-                
 
         return geos_geometries
 
-    '''--------------------------------------------------------------------------------------------------------------
-        GET CLUSTER GEOMETRIES AND CACHING MECHANISM
 
-        The input is always a geojson Polygon or MultiPolygon.
-        1. The envelope of this MP is calculated
-        2. The envelope ist snapped to the grid and split into cells
-        3. if the MP was not a rectangle, each cell is merged with the polygon
-        4. the resulting set of polygons is the clusterGeometry AS GEOS
-
-        compare with cache:
-        - always cluster all cells if zoom has changed
-        - always cluster all cells if filters have changed
-        - only cluster uncached cells if neither zoom nor filter changed
-
-        cache format:
-        dict: {'filters':{}, 'geometries':[geojson,geojson,geojsn], 'zoom':1, 'clustertype': 'grid' or 'kmeans'}
-    --------------------------------------------------------------------------------------------------------------'''
-    def getClusterGeometries(self, clustertype):
+    # returns a list of polygons in GEOS format and db_srid
+    def convert_geojson_to_geos(self, geojson):
+
+        geos_geometries = []
+
+        if geojson['type'] == 'FeatureCollection':
+
+            geos_geometries = []
+
+            for feature in geojson['features']:
+
+                geos_geometries += self.convert_geojson_feature_to_geos(
+                    feature)
+
+        elif geojson['type'] == 'Feature':
+
+            geos_geometries = self.convert_geojson_feature_to_geos(geojson)
+
+        return geos_geometries
+
+
+    '''
+    expected geometry:
+    var coordinates = [ [
+        [ viewport["left"], viewport["top"] ], 
+        [ viewport["right"], viewport["top"] ],
+        [ viewport["right"], viewport["bottom"] ],
+        [ viewport["left"], viewport["bottom"] ],
+        [ viewport["left"], viewport["top"] ]
+    ]];
+    '''
+    def sanitize_geojson_viewport(self, geojson):
+
+        coordinates = geojson['geometry']['coordinates']
+
+        # check if the viewport spans the edges of coordinate system
+        left = coordinates[0][0][0]
+        top = coordinates[0][0][1]
+        right = coordinates[0][1][0]
+        bottom = coordinates[0][2][1]
+
+        srid =  geojson['geometry']['crs']['properties']['name'].split(':')[-1]
+
+        if left > right:
+
+            sanitized_geojson = {
+                'type': 'Feature',
+                'geometry': {
+                    'crs': geojson['geometry']['crs'],
+                    'type': 'MultiPolygon',
+                    'coordinates': [
+                        [
+                            [left, top],
+                            [MAX_BOUNDS[srid]['max_x'], top],
+                            [MAX_BOUNDS[srid]['max_x'], bottom],
+                            [left, bottom],
+                            [left, top]
+                        ],
+                        [
+                            [MAX_BOUNDS[srid]['min_x'], top],
+                            [right, top],
+                            [right, bottom],
+                            [MAX_BOUNDS[srid]['min_x'], bottom],
+                            [MAX_BOUNDS[srid]['min_x'], top]
+                        ]
+                    ]
+                }
+            }
+        else:
+            sanitized_geojson = geojson
 
-        geojson_feature = self.params['geojson']
+        return sanitized_geojson
+
+
+    def get_cluster_geometries(self, geojson, geometry_type, zoom):
+
+        if geometry_type == GEOMETRY_TYPE_VIEWPORT:
+            geojson = self.sanitize_geojson_viewport(geojson)
 
         # list of polygons
-        geos_geometries = self.convertGeojsonFeatureToGEOS(geojson_feature)
+        geos_geometries = self.convert_geojson_to_geos(geojson)
 
-        clusterGeometries = []
-        remove_cached_geometries = True
-        new_cache = {
-            "geometries":[],
-            "clustertype":clustertype,
-            "zoom":self.zoom,
-            "filters":json.dumps(self.params["filters"])
-        }
-        
-        if self.zoom != self.cache.get("zoom",-1):
-            remove_cached_geometries = False
-        elif bool(self.params.get("deliver_cache",False)) == True:
-            remove_cached_geometries = False
-        elif self.params.get("filters", {}) != json.loads(self.cache.get("filters","{}")):
-            remove_cached_geometries = False
-        elif clustertype != self.cache.get("clustertype", None):
-            remove_cached_geometries = False
-        elif self.params.get("cache","") == "load":
-            remove_cached_geometries = False
+        cluster_geometries = []
+
+        # eg when panning, only new cluster areas which appeared on the viewport are returned
+        cluster_cache = self.cluster_cache
 
+        # elif bool(self.params.get('deliver_cache', False)) == True:
+        #    remove_cached_geometries = False
+        # elif self.params.get('cache', '') == 'load':
+        #    remove_cached_geometries = False
 
         for geos in geos_geometries:
-            envelope = geos.envelope
-            
-            cells = self.rectangleToClusterCells(envelope)
 
-            for cell in cells:
+            if geometry_type == GEOMETRY_TYPE_AREA:
 
-                # check if geos is rectangular, better check needed
-                if geos.equals(envelope) == True:
+                if geos.geojson not in cluster_cache.geometries:
+                    cluster_geometries.append(geos)
+                    cluster_cache.add_geometry(geos.geojson)
 
-                    cell_wk = {"geos":cell, "k":BASE_K}
+            elif geometry_type == GEOMETRY_TYPE_VIEWPORT:
+                envelope = geos.envelope
 
-                    if remove_cached_geometries == True:
-                        if cell.geojson not in self.cache["geometries"]:
-                            clusterGeometries.append(cell_wk)
-                    else:
-                        clusterGeometries.append(cell_wk)
+                cells = self.rectangle_to_clustercells(envelope, zoom)
 
-                    new_cache["geometries"].append(cell.geojson)
-                else:
-                    if cell.intersects(geos):
-                        intersection = cell.intersection(geos)
+                for cell in cells:
 
-                        intersection_wk = {"geos":intersection, "k":BASE_K}
-                        if remove_cached_geometries == True:
-                            if intersection.geojson not in self.cache["geometries"]:
-                                clusterGeometries.append(intersection_wk)
-                        else:
-                            clusterGeometries.append(intersection_wk)
+                    # check if geos is rectangular, better check needed
+                    if geos.equals(envelope) == True:
+                        cluster_geometry = cell
 
-                        new_cache["geometries"].append(intersection.geojson)
+                    elif cell.intersects(geos):
+                        cluster_geometry = cell.intersection(geos)
 
-        self.request.session["clustercache"] = new_cache
-        
-        return clusterGeometries
 
+                    if cluster_geometry.geojson not in cluster_cache.geometries:
+                        cluster_geometries.append(cluster_geometry)
+                        cluster_cache.add_geometry(cluster_geometry.geojson)
+
+            else:
+                raise TypeError('Invalid geometry_type')
+
+        self.cluster_cache = cluster_cache
+
+        return cluster_geometries
 
-    '''---------------------------------------------------------------------------------------------------------------------------------
+    '''---------------------------------------------------------------------------------------------------------------------
         CALCULATE CELL-IDs ACCORDING TO VIEWPORT
 
         - given the viewport, expand to the nearest grid and get all cell ids of this grid
         - returns QuadKey IDS of a viewport according to MapClusterer.gridSize
 
         To calculate those cells, the coordinates are transformed as shown below:
         
 
-    LatLng --------> Meters (Mercator) ---------> Shifted origin ---------> pixel coords ---------> GRID, depending on tilesize
+    LatLng ---------> Meters (Mercator) -----> Shifted origin -------> pixel coords ---------> GRID, depending on tilesize
 
-     -----------           -----------                -----------              -----------           -----------
-    |           |         |           |              |           |            |           |         |00|10|20|30|
-    |           |         |           |              |           |            |           |         |01|11|21|31|
-    |     O     |         |     O     |              |           |            |           |          -----------
-    |           |         |           |              |           |            |           |         |02|12|22|32|
-    |           |         |           |              |           |            |           |         |03|13|23|33|
-     -----------           -----------               O-----------             O-----------           -----------
-       LATLNG                 METERS                     METERS                   PIXELS                 GRID
-                                                 (shifted coordinates)                          (CELL-IDs according to QuadKey, depends on zoom level)
+     -----------       -----------             -----------              -----------           -----------
+    |           |     |           |           |           |            |           |         |00|10|20|30|
+    |           |     |           |           |           |            |           |         |01|11|21|31|
+    |     O     |     |     O     |           |           |            |           |          -----------
+    |           |     |           |           |           |            |           |         |02|12|22|32|
+    |           |     |           |           |           |            |           |         |03|13|23|33|
+     -----------       -----------            O-----------             O-----------           -----------
+       LATLNG            METERS                  METERS                   PIXELS                 GRID
+                                          (shifted coordinates)                          (CELL-IDs according to QuadKey,
+                                                                                          depends on zoom level)
 
     O = origin
 
     The coordinate system with shifted origin has only coordinates with positive values (essential).
     Now, get the CELL-ID (=QuadKey ID) the top-right (and bottom-left) viewport coordinate sits in.
     Finally calculate all CELL-IDs that are spanned by the top-right and bottom-left cell.
         
-    ---------------------------------------------------------------------------------------------------------------------------------'''
-
-
+    ---------------------------------------------------------------------------------------------------------------------'''
 
     '''
         Expands an envelope (=rectangle) to the fixed world grid
         Splits the grid into cells of defined size
     '''
-    def rectangleToClusterCells(self, geos_envelope):
-        linearRing = geos_envelope[0]
-                
-        left = linearRing[0][0]
-        bottom = linearRing[0][1]
-        right = linearRing[1][0]
-        top = linearRing[2][1]
+
+    def rectangle_to_clustercells(self, geos_envelope, zoom):
+        linear_ring = geos_envelope[0]
+
+        left = linear_ring[0][0]
+        bottom = linear_ring[0][1]
+        right = linear_ring[1][0]
+        top = linear_ring[2][1]
 
         topright = Point(right, top, srid=self.db_srid)
         bottomleft = Point(left, bottom, srid=self.db_srid)
 
         # project points to mercator 3875, plane coordinates
         self.maptools.point_ToMercator(topright)
         self.maptools.point_ToMercator(bottomleft)
 
         # shift origin
         self.maptools.point_MercatorToWorld(topright)
         self.maptools.point_MercatorToWorld(bottomleft)
 
         # calculate pixelcoords from world coords depending on zoom
-        self.maptools.point_WorldToPixels(topright, self.zoom)
-        self.maptools.point_WorldToPixels(bottomleft, self.zoom)
+        self.maptools.point_WorldToPixels(topright, zoom)
+        self.maptools.point_WorldToPixels(bottomleft, zoom)
 
         # get topright and bottom left cellID, e.g. (03,01)
-        toprightCell = self.maptools.point_PixelToCellID(topright, self.gridSize)
-        bottomleftCell = self.maptools.point_PixelToCellID(bottomleft, self.gridSize)
+        topright_cell = self.maptools.point_PixelToCellID(
+            topright, self.grid_size)
+        bottomleft_cell = self.maptools.point_PixelToCellID(
+            bottomleft, self.grid_size)
 
         # get all Cells that need to be clustered, as quadKey
-        clusterCells = self.maptools.getClusterCellsAsPolyList(toprightCell, bottomleftCell, self.zoom,
-                                                               self.gridSize, self.db_srid)
-
-        return clusterCells
-        
-
-    '''---------------------------------------------------------------------------------------------------------------------------------
-        SQL FOR FILTERING
-
-        Converts the filter dictionary into a raw querystring that is added to the raw sql later
-
-        Used by both kmeans and grid cluster
-    ---------------------------------------------------------------------------------------------------------------------------------'''
-    def parseFilterValue(self, operator, value):
-
-        if type(value) == str:
-            if operator == "startswith":
-                return "'^{value}.*' ".format(value=value)
-
-            elif operator == "contains":
-                return "'{value}.*'".format(value=value)
-            
-            else:
-                return "'{value}'".format(value=value)
-
-        elif type(value) == bool:
+        cluster_cells = self.maptools.getClusterCellsAsPolyList(topright_cell, bottomleft_cell, zoom, self.grid_size,
+                                                                self.db_srid)
 
-            if value == False:
-                return "FALSE"
+        return cluster_cells
 
-            else:
-                return "TRUE"
-
-        elif isinstance(value, numbers.Number) or isinstance(value, decimal.Decimal):
-            return value
-
-        else:
-            return value
-
-
-    def constructFilterstring(self, filters):
-
-        operator_mapping = {
-            "=" : "=",
-            "!=" : "!=",
-            ">=" : ">=",
-            "<=" : "<=",
-            "startswith" : "~",
-            "contains" : "~"
-        }
-
-        filterstring = ''
-
-        for filter in filters:
-
-            column = list(filter.keys())[0]
-
-            filterparams = filter[column]
-
-            filterstring += ' AND ('
-            
-            operator_pre = filterparams.get("operator", "=")
-
-            values = filterparams["values"]
-
-            if "either" in operator_pre:
-
-                parts = operator_pre.split('_')
-
-                operator = operator_mapping[parts[-1]]
-
-                for counter, value in enumerate(values):
-                    if counter >0:
-                        filterstring += " OR "
-
-                    sql_value = self.parseFilterValue(parts[-1], value)
-
-                    filterstring += "{column} {operator} {sql_value}".format(column=column, operator=operator,
-                                                                             sql_value=sql_value)
-                
-
-            else:
-                
-                if type(values) == str or type(values) == bool:
-                    operator = operator_mapping[operator_pre]
-                    sql_value = self.parseFilterValue(operator_pre, values)
-                    
-
-                elif type(values) == list:
-                    if operator_pre == "!=":
-                        operator = "NOT IN"
-                    else:
-                        operator = "IN"
-
-                    sql_value = str(tuple(values))
-
-                filterstring += "{column} {operator} {sql_value}".format(column=column, operator=operator,
-                                                                         sql_value=sql_value)
-                    
-
-            filterstring += ')'
-
-        return filterstring
-
-
-
-    '''---------------------------------------------------------------------------------------------------------------------------------
+    '''---------------------------------------------------------------------------------------------------------------------
         MERGING MARKERS BY DISTANCE
         - retrieves cluster_rows
         - returns a list of PointCluster instances
         
-        - if the geometric centroids are too close to each other after the kmeans algorithm (e.g. overlap), they are merged to one cluster
-        - used by kmeansCluster as phase 2
+        - if the geometric centroids are too close to each other after the kmeans algorithm (e.g. overlap),
+          they are merged to one cluster
+        - used by kmeans_cluster as phase 2
         - uses pixels for calculation as this is constant on every zoom level
         - transforms cluster.id into a list
-    ---------------------------------------------------------------------------------------------------------------------------------'''
+    ---------------------------------------------------------------------------------------------------------------------'''
 
-    def distanceCluster(self, cluster_rows, c_distance=30):
+    def distance_cluster(self, cluster_rows, zoom, c_distance=30):
 
         clusters_processed = []
 
         for cluster_row in cluster_rows:
 
-            point_cluster = PointCluster(cluster_row, geo_column_str, self.db_srid)
-            
+            point_cluster = PointCluster(
+                cluster_row, geo_column_str, self.db_srid)
+
             clustercoords = getattr(point_cluster, geo_column_str)
 
             added = False
 
             for processed_cluster in clusters_processed:
                 processed_coords = getattr(processed_cluster, geo_column_str)
-                pixel_distance = self.maptools.points_calcPixelDistance(clustercoords, processed_coords, self.zoom)
-                
+                pixel_distance = self.maptools.points_calcPixelDistance(
+                    clustercoords, processed_coords, zoom)
+
                 if pixel_distance <= c_distance:
                     if not type(processed_cluster.id) == list:
                         processed_cluster.id = [processed_cluster.id]
 
                     processed_cluster.id.append(point_cluster.id)
                     processed_cluster.count += point_cluster.count
                     added = True
                     break
 
             if not added:
                 if not type(point_cluster.id) == list:
                     point_cluster.id = [point_cluster.id]
                 clusters_processed.append(point_cluster)
 
-        
         return clusters_processed
 
-    
-    '''---------------------------------------------------------------------------------------------------------------------------------
+    '''---------------------------------------------------------------------------------------------------------------------
         KMEANS CLUSTERING
         - cluster only if 1. the geometry contains a new area or 2. the filters changed
-        - perform a raw query on the database, pass the result to phase 2 (distanceCluster) and return the result
-    ---------------------------------------------------------------------------------------------------------------------------------'''        
+        - perform a raw query on the database, pass the result to phase 2 (distance_cluster) and return the result
+    ---------------------------------------------------------------------------------------------------------------------'''
 
-    def kmeansCluster(self, custom_filterstring=""):
-        
-        clusterGeometries = self.getClusterGeometries("kmeans")
+    def kmeans_cluster(self, geojson, geometry_type, zoom, filters):
+
+        cluster_geometries = self.get_cluster_geometries(geojson, geometry_type, zoom)
 
         markers = []
 
-        if clusterGeometries:
+        if cluster_geometries:
 
-            filterstring = self.constructFilterstring(self.params["filters"])
+            filter_composer = FilterComposer(filters)
+            filterstring = filter_composer.as_sql()
 
-            filterstring += custom_filterstring
+            for geos_geometry in cluster_geometries:
 
-            for geometry_dic in clusterGeometries:
+                k = BASE_K
 
-                geos_geometry = geometry_dic["geos"]
-                k = geometry_dic["k"]
+                if geometry_type == GEOMETRY_TYPE_AREA:
+                    k = self.calculate_k(geos_geometry, zoom)
 
                 sql = '''
                     SELECT kmeans AS id, count(*), ST_AsText(ST_Centroid(ST_Collect({geo_column})))
                     AS {geo_column} {pin_qry_0} {additional_column_qry_0}
                     FROM ( 
                       SELECT {pin_qry_1} {additional_column_qry_1} kmeans(ARRAY[ST_X({geo_column}), ST_Y({geo_column})], {k}) OVER ()
                       AS kmeans, {geo_column}
@@ -582,281 +515,315 @@
                     ) AS ksub
 
                     GROUP BY id
                     ORDER BY kmeans;
                     
                 '''.format(geo_column=geo_column_str, pin_qry_0=pin_qry[0], pin_qry_1=pin_qry[1], k=k,
                            schema_name=self.schema_name, geo_table=geo_table, geos_geometry=geos_geometry.ewkt,
-                           filterstring=filterstring,additional_column_qry_0=additional_column_qry[0],
+                           filterstring=filterstring, additional_column_qry_0=additional_column_qry[
+                               0],
                            additional_column_qry_1=additional_column_qry[1])
 
-
                 with connections['default'].cursor() as cursor:
                     cursor.execute(sql)
-                
+
                     cluster_rows = cursor.fetchall()
 
-                
-                kclusters = self.distanceCluster(cluster_rows)
-                
+                kclusters = self.distance_cluster(cluster_rows, zoom)
 
                 for point_cluster in kclusters:
                     point = getattr(point_cluster, geo_column_str)
 
-                    if point.srid != self.input_srid:
-                        self.maptools.point_AnyToAny(point, point.srid, self.input_srid)
+                    if point.srid != self.output_srid:
+                        self.maptools.point_AnyToAny(
+                            point, point.srid, self.output_srid)
 
                     marker = {
-                        'ids': point_cluster.id,
+                        'ids': point_cluster.id, # distance cluster clusters ids
                         'count': point_cluster.count,
                         'center': {
-                                'x': point.x,
-                                'y': point.y
+                            'x': point.x,
+                            'y': point.y
                         },
                         'pinimg': point_cluster.pinimg,
                     }
 
                     if ADDITIONAL_COLUMN:
-                        marker[ADDITIONAL_COLUMN] = getattr(point_cluster, ADDITIONAL_COLUMN)
+                        marker[ADDITIONAL_COLUMN] = getattr(
+                            point_cluster, ADDITIONAL_COLUMN)
 
                     markers.append(marker)
 
-
         return markers
 
-
-
-    '''---------------------------------------------------------------------------------------------------------------------------------
+    '''---------------------------------------------------------------------------------------------------------------------
         GRID CLUSTERING 
-    ---------------------------------------------------------------------------------------------------------------------------------'''
-    
-    
-    def gridCluster(self):
+        - only for GEOMETRY_TYPE_VIEWPORT, not for GEOMETRY_TYPE_AREA
+    ---------------------------------------------------------------------------------------------------------------------'''
+    def grid_cluster(self, geojson, zoom, filters):
 
-        clusterGeometries = self.getClusterGeometries("grid")
+        cluster_geometries = self.get_cluster_geometries(geojson, GEOMETRY_TYPE_VIEWPORT, zoom)
 
         gridCells = []
 
-        if clusterGeometries:
+        if cluster_geometries:
 
-            filterstring = self.constructFilterstring(self.params["filters"])
+            filter_composer = FilterComposer(filters)
+            filterstring = filter_composer.as_sql()
 
             cursor = connections['default'].cursor()
 
-            cursor.execute('''CREATE TEMPORARY TABLE temp_clusterareas (
-                  id serial,
-                  polygon geometry
-               )''')
+            sql_create_temporary_table = '''CREATE TEMPORARY TABLE temp_clusterareas (
+                id serial,
+                polygon geometry(Geometry,3857)
+            )'''
+
+            cursor.execute(sql_create_temporary_table)
 
-            for clusterGeometry in clusterGeometries:
-                cursor.execute('''
+            for clusterGeometry in cluster_geometries:
+
+                sql_insert_clustergeom = '''
                     INSERT INTO temp_clusterareas (polygon)
                     ( SELECT (
                         ST_Dump(
                             ST_GeometryFromText('{geometry}')
                     )).geom )
-                '''.format(geometry=clusterGeometry["geos"].ewkt))
+                '''.format(geometry=clusterGeometry.ewkt)
+
+                cursor.execute(sql_insert_clustergeom)
 
             # indexing did not increase performance
             # cursor.execute('''CREATE INDEX temp_gix ON temp_clusterareas USING GIST (polygon);''')
 
-            gridcluster_queryset = '''SELECT count(*) AS count, polygon {pin_qry_0}
-                FROM {schema_name}.{geo_table}, temp_clusterareas
+            grid_cluster_queryset = '''SELECT count(*) AS count, polygon {pin_qry_0}, ST_Union(coordinates), MAX(geotable.id)
+                FROM {schema_name}.{geo_table} geotable, temp_clusterareas
                 WHERE coordinates IS NOT NULL AND ST_Intersects(coordinates, polygon) {filterstring}
                 GROUP BY polygon
             '''.format(schema_name=self.schema_name, geo_table=geo_table, filterstring=filterstring,
                        pin_qry_0=pin_qry[0])
 
-            cursor.execute(gridcluster_queryset)            
+            cursor.execute(grid_cluster_queryset)
 
             gridCells_pre = cursor.fetchall()
 
             for cell in gridCells_pre:
 
                 count = cell[0]
                 pinimg = None
+                id = None
+
+                geos = GEOSGeometry(cell[1], srid=3857)
+                geos.transform(self.output_srid)
 
                 if count == 1 and PINCOLUMN:
                     pinimg = cell[2]
+                    point_geos = GEOSGeometry(cell[3], srid=3857)
+                    point_geos.transform(self.output_srid)
+                    x = point_geos.x
+                    y = point_geos.y
+                    id = cell[4]
 
-                geos = GEOSGeometry(cell[1])
-                geos.transform(self.input_srid)
-                centroid = geos.centroid
-                
-                cellobj = {"count":count, "geojson": geos.geojson, "center":{"x":centroid.x, "y": centroid.y},
-                           "pinimg" : pinimg}
+                else:
+                    centroid = geos.centroid
+                    x = centroid.x
+                    y = centroid.y            
+
+                cellobj = {
+                    'count': count,
+                    'geojson': json.loads(geos.geojson),
+                    'center': {
+                        'x': x,
+                        'y': y
+                    },
+                    'pinimg': pinimg,
+                    'id': id
+                }
 
                 gridCells.append(cellobj)
-                
-                
-        return gridCells
 
+            sql_drop_temporary_table = 'DROP TABLE temp_clusterareas'
+            cursor.execute(sql_drop_temporary_table)
 
-    
-    '''---------------------------------------------------------------------------------------------------------------------------------
+        return gridCells
+
+    '''---------------------------------------------------------------------------------------------------------------------
         NON-CLUSTERING METHODS
-    ---------------------------------------------------------------------------------------------------------------------------------'''
+    ---------------------------------------------------------------------------------------------------------------------'''
+
     def get_gis_field_names(self):
 
         gis_fields = Gis._meta.concrete_fields
 
         gis_field_names = []
 
         # Relational Fields are not supported
         for field in gis_fields:
             if isinstance(field, ForeignKey):
-                #name = field.get_attname_column()[0]
+                # name = field.get_attname_column()[0]
                 continue
             if isinstance(field, BaseSpatialField):
                 name = '{name}::bytea'.format(name=field.name)
             else:
                 name = field.name
 
             gis_field_names.append(name)
 
         return gis_field_names
-        
-        
+
+
     def get_gis_fields_str(self):
 
         gis_field_names = self.get_gis_field_names()
 
         gis_fields_str = ','.join(gis_field_names)
 
         gis_fields_str.rstrip(',')
 
         return gis_fields_str
 
-    # return all IDs of the pins contained by a cluster
-    def getClusterContent(self, custom_filterstring=""):
 
-        x = self.params["x"]
-        y = self.params["y"]
+    # return all IDs of the pins contained by a kmeans cluster
+    def get_kmeans_cluster_content(self, geometry_type, ids, x, y, filters, zoom, input_srid=4326):
 
-        cluster = Point(x, y, srid=self.input_srid)
+        cluster = Point(x, y, srid=input_srid)
 
         # request lnglat point
-        cell_geos = self.maptools.getCellForPointAsGeos(cluster, self.zoom, self.gridSize, self.db_srid)
-        
+        cell_geos = self.maptools.getCellForPointAsGeos(cluster, zoom, self.grid_size, self.db_srid)
+
         cluster.transform(self.db_srid)
 
         query_geometry = None
-        
-        for geometry in self.cache["geometries"]:
+        k = BASE_K
+
+        for geometry in self.cluster_cache.geometries:
+
             geos = GEOSGeometry(geometry)
-            
+            # cached geometries are always srid==self.db_srid
+            # bug: geos.srid is set to 4326 here, which is wrong
+            # it is impossible to instnatiate with GEOSGeometry(geometry, srid=3857), which throws an error
+
+            #if geos.srid != self.db_srid:
+            #    ct = CoordTransform(SpatialReference(geos.srid), SpatialReference(self.db_srid))
+            #    geos.transform(ct)
+
+
             if cluster.within(geos):
-                query_geometry = geos.intersection(cell_geos)
+
+                if geometry_type == GEOMETRY_TYPE_VIEWPORT:
+                    query_geometry = geos.intersection(cell_geos)
+                elif geometry_type == GEOMETRY_TYPE_AREA:
+                    k = self.calculate_k(geos, zoom)
+                    query_geometry = geos
+                    
                 break
 
+        if not query_geometry:
+            raise ValueError('cluster not found in cache')
 
-        filterstring = self.constructFilterstring(json.loads(self.cache["filters"]))
-        filterstring += custom_filterstring
+        filter_composer = FilterComposer(filters)
+        filterstring = filter_composer.as_sql()
 
-        kmeans_list = self.params["ids"]
-        kmeans_string = (",").join(str(k) for k in kmeans_list)
+        kmeans_list = ids
+        kmeans_string = (',').join(str(k) for k in kmeans_list)
 
         gis_fields_str = self.get_gis_fields_str()
 
-        sql= '''
+        sql = '''
             SELECT {fields} FROM ( 
-              SELECT kmeans(ARRAY[ST_X({geo_column}), ST_Y({geo_column})], {base_k}) OVER ()
+              SELECT kmeans(ARRAY[ST_X({geo_column}), ST_Y({geo_column})], {k}) OVER ()
               AS kmeans, "{geo_table}".*
               FROM {schema_name}.{geo_table} WHERE {geo_column} IS NOT NULL
               AND ST_Intersects({geo_column}, ST_GeometryFromText('{geometry}', {srid}) ) {filterstring}
             ) AS ksub
             WHERE kmeans IN ({kmeans_string})
-            '''.format(geo_column=geo_column_str, base_k=BASE_K, geo_table=geo_table, schema_name=self.schema_name,
+            '''.format(geo_column=geo_column_str, k=k, geo_table=geo_table, schema_name=self.schema_name,
                        geometry=query_geometry.ewkt, srid=self.db_srid, filterstring=filterstring,
                        kmeans_string=kmeans_string, fields=gis_fields_str)
 
-        
         entries_queryset = Gis.objects.raw(sql)
-                                               
-        return entries_queryset
+
+        return list(entries_queryset)
 
 
-    def getAreaContent(self, custom_filterstring=""):
+    def get_area_content(self, geojson, filters):
 
-        geomfilterstring = self.getGeomFilterstring(self.params["geojson"])
-        filterstring = self.constructFilterstring(json.loads(self.cache["filters"]))
+        geomfilterstring = self.get_geom_filterstring(geojson)
+
+        filter_composer = FilterComposer(filters)
+        filterstring = filter_composer.as_sql()
 
         gis_fields_str = self.get_gis_fields_str()
-        
+
         entries_queryset = Gis.objects.raw(
             '''SELECT {fields} FROM {schema_name}.{geo_table} WHERE {geomfilterstring} {filterstring};'''.format(
                 schema_name=self.schema_name, geo_table=geo_table, geomfilterstring=geomfilterstring,
                 filterstring=filterstring, fields=gis_fields_str)
-            )
+        )
 
         return entries_queryset
 
 
-    '''---------------------------------------------------------------------------------------------------------------------------------
+    def get_dataset_content(self, id):
+
+        gis_fields_str = self.get_gis_fields_str()
+
+        queryset = Gis.objects.raw(
+            '''SELECT {fields} FROM {schema_name}.{geo_table} WHERE id={id};'''.format(
+                schema_name=self.schema_name, geo_table=geo_table, fields=gis_fields_str, id=str(id))
+        )
+
+        return queryset
+
+    '''---------------------------------------------------------------------------------------------------------------------
         COSTRUCT A FILTERSTRING FOR GEOMETRIES
 
         multipolygon and collections are not supported by ST_Within so they need to be split into several geometries
         this function converts geometries into a string usable as a raw sql query
         if no request is given, it will take the geometry from the cache
 
         first, the geojson is converted to a list of GEOS
         second, the list is converted to a string
-    ---------------------------------------------------------------------------------------------------------------------------------'''
+    ---------------------------------------------------------------------------------------------------------------------'''
 
-    def getGeomFilterstring(self, geojson):
+    def get_geom_filterstring(self, geojson):
 
-        geomfilterstring = ""
-            
-        if geojson["type"] == "FeatureCollection":
+        geos_geometries = self.convert_geojson_to_geos(geojson)
 
-            geos_geometries = []
-            
-            for feature in geojson["features"]:
-
-                geos_geometries += self.convertGeojsonFeatureToGEOS(feature)
-                
-                
-
-        elif geojson["type"] == "Feature":
+        geomfilterstring = ''
 
-                geos_geometries = self.convertGeojsonFeatureToGEOS(geojson)
+        geomfilterstring += '('
 
-
-        geomfilterstring += "("
-        
         for counter, geos in enumerate(geos_geometries):
             if counter > 0:
-                geomfilterstring += " OR "
+                geomfilterstring += ' OR '
             geomfilterstring += " ST_Intersects({geo_column}, ST_GeometryFromText('{geometry}', {srid}) ) ".format(
                 geo_column=geo_column_str, geometry=geos.wkt, srid=self.db_srid)
 
-        geomfilterstring += ")"
-            
+        geomfilterstring += ')'
 
         return geomfilterstring
-        
 
-            
-    '''---------------------------------------------------------------------------------------------------------------------------------
+    '''---------------------------------------------------------------------------------------------------------------------
         K Calculation
 
         this is only used for strict geometries, such as drawn polygons or drawn circles
         based on the BASE_K in the settings (defaults to 6) it increases the k if one draws a big shape
-    ---------------------------------------------------------------------------------------------------------------------------------'''
+    ---------------------------------------------------------------------------------------------------------------------'''
     # k calculation has to be done on square-pixel areas
-    def calculateK(self, geos_geometry):
 
-        geom_copy = geos_geometry.transform(3857, clone=True)
-        
-        cellarea_pixels = self.gridSize * self.gridSize
+    def calculate_k(self, geos_geometry, zoom):
+
+        geom_copy = geos_geometry.clone() #transform(3857, clone=True)
+
+        cellarea_pixels = self.grid_size * self.grid_size
 
         # 1m = ? pixels
         init_resolution = self.maptools.mapTileSize / (2 * math.pi * 6378137)
-        
-        resolution = init_resolution * (2**self.zoom)
+
+        resolution = init_resolution * (2**zoom)
 
         area_factor = resolution**2
 
         geom_copy_area_pixels = geom_copy.area * area_factor
 
         new_k = (BASE_K / cellarea_pixels) * geom_copy_area_pixels
```

### Comparing `anycluster-0.6.2/anycluster/MapTools.py` & `anycluster-2.0.0/anycluster/MapTools.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,16 +214,14 @@
                                                        "topright": toprightEdgeCellID, "bottomleft": bottomleftCellID}])
 
         return clusterCells
 
 
     def clusterCellToBounds(self, cell, zoom, gridSize, srid):
 
-        bounds = []
-
         pixelbounds = self.cellIDToTileBounds(cell, gridSize)
         mercatorbounds = self.bounds_PixelToMercator(pixelbounds, zoom)
 
         # convert mercatorbounds to latlngbounds
         cell_topright = Point(mercatorbounds['right'], mercatorbounds['top'], srid=3857)
         cell_bottomleft = Point(mercatorbounds['left'], mercatorbounds['bottom'], srid=3857)
```

### Comparing `anycluster-0.6.2/anycluster/clusters.py` & `anycluster-2.0.0/anycluster/clusters.py`

 * *Files identical despite different names*

### Comparing `anycluster-0.6.2/setup.py` & `anycluster-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 install_requires = [
     'psycopg2',
+    'djangorestframework',
+    'jsonschema',
 ]
 
 setup(
     name="anycluster",
-    version='0.6.2',
+    version='2.0.0',
     description='anycluster provides Server-Side clustering of map markers for Geodjango',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
-    keywords='django, cluster, k-means, grid, server-side clustering',
+    keywords='django, cluster, kmeans, grid, server-side clustering',
     author='Thomas Uher',
     author_email='thomas.uher@sisol-systems.com',
     url='https://github.com/biodiv/anycluster',
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

