# Comparing `tmp/bxa-4.0.7.tar.gz` & `tmp/bxa-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bxa-4.0.7.tar", last modified: Thu Nov 10 08:09:12 2022, max compression
+gzip compressed data, was "bxa-4.1.0.tar", last modified: Thu Apr 20 14:30:53 2023, max compression
```

## Comparing `bxa-4.0.7.tar` & `bxa-4.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2022-11-10 08:09:12.939381 bxa-4.0.7/
--rw-r--r--   0 user      (1000) jbuchner  (1000)    35149 2021-05-10 10:26:12.000000 bxa-4.0.7/LICENSE
--rw-r--r--   0 user      (1000) jbuchner  (1000)       72 2021-05-10 10:26:12.000000 bxa-4.0.7/MANIFEST.in
--rw-r--r--   0 user      (1000) jbuchner  (1000)     7746 2022-11-10 08:09:12.939381 bxa-4.0.7/PKG-INFO
--rw-r--r--   0 user      (1000) jbuchner  (1000)     6892 2021-05-10 10:26:12.000000 bxa-4.0.7/README.rst
--rw-r--r--   0 user      (1000) jbuchner  (1000)     5426 2021-05-10 10:26:46.000000 bxa-4.0.7/addspec.py
-drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2022-11-10 08:09:12.883385 bxa-4.0.7/bxa/
--rw-r--r--   0 user      (1000) jbuchner  (1000)      269 2022-11-10 08:09:07.000000 bxa-4.0.7/bxa/__init__.py
-drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2022-11-10 08:09:12.887385 bxa-4.0.7/bxa/sherpa/
--rw-r--r--   0 user      (1000) jbuchner  (1000)      921 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/__init__.py
-drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2022-11-10 08:09:12.939381 bxa-4.0.7/bxa/sherpa/background/
--rw-r--r--   0 user      (1000) jbuchner  (1000)        0 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/__init__.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)   431614 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/chandra_1024.json
--rw-r--r--   0 user      (1000) jbuchner  (1000)   267761 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/erosita_1024.json
--rw-r--r--   0 user      (1000) jbuchner  (1000)    16677 2021-08-31 11:06:48.000000 bxa-4.0.7/bxa/sherpa/background/fitters.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)     1788 2021-08-31 11:22:07.000000 bxa-4.0.7/bxa/sherpa/background/kde.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)    16911 2021-08-31 11:06:48.000000 bxa-4.0.7/bxa/sherpa/background/models.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)  1253996 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/nustar_4096.json
--rw-r--r--   0 user      (1000) jbuchner  (1000)    13251 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/pca.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)  1161850 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/suzaku_4096.json
--rw-r--r--   0 user      (1000) jbuchner  (1000)   318648 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/swift_xrt_1024.json
--rw-r--r--   0 user      (1000) jbuchner  (1000)    20063 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/xmm.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)  2882995 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/xmm_2400.json
--rw-r--r--   0 user      (1000) jbuchner  (1000)  3558683 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/xmm_4096.json
--rw-r--r--   0 user      (1000) jbuchner  (1000)   927873 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/xmm_epn_1024.json
--rw-r--r--   0 user      (1000) jbuchner  (1000)  1658222 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/xmm_epn_4096.json
--rw-r--r--   0 user      (1000) jbuchner  (1000)    78814 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/xrte_hexa_256.json
--rw-r--r--   0 user      (1000) jbuchner  (1000)    78972 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/xrte_hexb_256.json
--rw-r--r--   0 user      (1000) jbuchner  (1000)    62879 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/background/xrte_pca_128.json
--rw-r--r--   0 user      (1000) jbuchner  (1000)     2202 2021-08-31 11:06:48.000000 bxa-4.0.7/bxa/sherpa/cachedmodel.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)      944 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/galabs.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)    19866 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/invgauss.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)     4086 2021-09-15 15:07:36.000000 bxa-4.0.7/bxa/sherpa/priors.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)     2820 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/qq.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)     5416 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/sherpa/rebinnedmodel.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)     7586 2022-11-09 21:53:07.000000 bxa-4.0.7/bxa/sherpa/solver.py
-drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2022-11-10 08:09:12.939381 bxa-4.0.7/bxa/xspec/
--rw-r--r--   0 user      (1000) jbuchner  (1000)      802 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/xspec/__init__.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)     7854 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/xspec/gof.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)     3141 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/xspec/priors.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)     4993 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/xspec/qq.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)     3878 2021-05-10 10:26:12.000000 bxa-4.0.7/bxa/xspec/sinning.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)    17795 2022-11-09 21:53:07.000000 bxa-4.0.7/bxa/xspec/solver.py
-drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2022-11-10 08:09:12.887385 bxa-4.0.7/bxa.egg-info/
--rw-r--r--   0 user      (1000) jbuchner  (1000)     7746 2022-11-10 08:09:12.000000 bxa-4.0.7/bxa.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) jbuchner  (1000)     1178 2022-11-10 08:09:12.000000 bxa-4.0.7/bxa.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) jbuchner  (1000)        1 2022-11-10 08:09:12.000000 bxa-4.0.7/bxa.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) jbuchner  (1000)       52 2022-11-10 08:09:12.000000 bxa-4.0.7/bxa.egg-info/requires.txt
--rw-r--r--   0 user      (1000) jbuchner  (1000)        4 2022-11-10 08:09:12.000000 bxa-4.0.7/bxa.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) jbuchner  (1000)     2632 2021-05-10 10:26:12.000000 bxa-4.0.7/fixkeywords.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)     1808 2021-05-10 10:26:12.000000 bxa-4.0.7/gal.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)       38 2022-11-10 08:09:12.939381 bxa-4.0.7/setup.cfg
--rw-r--r--   0 user      (1000) jbuchner  (1000)     1893 2022-11-10 08:09:07.000000 bxa-4.0.7/setup.py
+drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2023-04-20 14:30:53.735134 bxa-4.1.0/
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    35149 2021-05-10 10:26:12.000000 bxa-4.1.0/LICENSE
+-rw-r--r--   0 user      (1000) jbuchner  (1000)       72 2021-05-10 10:26:12.000000 bxa-4.1.0/MANIFEST.in
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     7746 2023-04-20 14:30:53.735134 bxa-4.1.0/PKG-INFO
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     6892 2021-05-10 10:26:12.000000 bxa-4.1.0/README.rst
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     5426 2021-05-10 10:26:46.000000 bxa-4.1.0/addspec.py
+drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2023-04-20 14:30:53.687134 bxa-4.1.0/bxa/
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      269 2023-04-20 13:24:37.000000 bxa-4.1.0/bxa/__init__.py
+drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2023-04-20 14:30:53.687134 bxa-4.1.0/bxa/sherpa/
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      921 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/__init__.py
+drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2023-04-20 14:30:53.735134 bxa-4.1.0/bxa/sherpa/background/
+-rw-r--r--   0 user      (1000) jbuchner  (1000)        0 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/__init__.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)   431614 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/chandra_1024.json
+-rw-r--r--   0 user      (1000) jbuchner  (1000)   267761 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/erosita_1024.json
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    16677 2021-08-31 11:06:48.000000 bxa-4.1.0/bxa/sherpa/background/fitters.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     1788 2021-08-31 11:22:07.000000 bxa-4.1.0/bxa/sherpa/background/kde.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    16911 2021-08-31 11:06:48.000000 bxa-4.1.0/bxa/sherpa/background/models.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)  1253996 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/nustar_4096.json
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    13251 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/pca.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)  1161850 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/suzaku_4096.json
+-rw-r--r--   0 user      (1000) jbuchner  (1000)   318648 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/swift_xrt_1024.json
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    20063 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/xmm.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)  2882995 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/xmm_2400.json
+-rw-r--r--   0 user      (1000) jbuchner  (1000)  3558683 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/xmm_4096.json
+-rw-r--r--   0 user      (1000) jbuchner  (1000)   927873 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/xmm_epn_1024.json
+-rw-r--r--   0 user      (1000) jbuchner  (1000)  1658222 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/xmm_epn_4096.json
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    78814 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/xrte_hexa_256.json
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    78972 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/xrte_hexb_256.json
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    62879 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/background/xrte_pca_128.json
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     2202 2021-08-31 11:06:48.000000 bxa-4.1.0/bxa/sherpa/cachedmodel.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      944 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/galabs.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    19866 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/invgauss.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     4086 2021-09-15 15:07:36.000000 bxa-4.1.0/bxa/sherpa/priors.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     2820 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/qq.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     5416 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/sherpa/rebinnedmodel.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     7586 2022-11-09 21:53:07.000000 bxa-4.1.0/bxa/sherpa/solver.py
+drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2023-04-20 14:30:53.735134 bxa-4.1.0/bxa/xspec/
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      802 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/xspec/__init__.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     7854 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/xspec/gof.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     3141 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/xspec/priors.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     4993 2021-05-10 10:26:12.000000 bxa-4.1.0/bxa/xspec/qq.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     4450 2023-04-20 12:58:11.000000 bxa-4.1.0/bxa/xspec/sinning.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    17839 2023-04-20 12:09:47.000000 bxa-4.1.0/bxa/xspec/solver.py
+drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2023-04-20 14:30:53.687134 bxa-4.1.0/bxa.egg-info/
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     7746 2023-04-20 14:30:53.000000 bxa-4.1.0/bxa.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     1178 2023-04-20 14:30:53.000000 bxa-4.1.0/bxa.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) jbuchner  (1000)        1 2023-04-20 14:30:53.000000 bxa-4.1.0/bxa.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) jbuchner  (1000)       52 2023-04-20 14:30:53.000000 bxa-4.1.0/bxa.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) jbuchner  (1000)        4 2023-04-20 14:30:53.000000 bxa-4.1.0/bxa.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     2632 2021-05-10 10:26:12.000000 bxa-4.1.0/fixkeywords.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     1808 2021-05-10 10:26:12.000000 bxa-4.1.0/gal.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)       38 2023-04-20 14:30:53.735134 bxa-4.1.0/setup.cfg
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     1893 2023-04-20 13:24:37.000000 bxa-4.1.0/setup.py
```

### Comparing `bxa-4.0.7/LICENSE` & `bxa-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/PKG-INFO` & `bxa-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bxa
-Version: 4.0.7
+Version: 4.1.0
 Summary: Bayesian X-ray spectral analysis
 Home-page: https://github.com/JohannesBuchner/BXA/
 Author: Johannes Buchner
 Author-email: johannes.buchner.acad@gmx.com
 License: GNU General Public License v3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bxa-4.0.7/README.rst` & `bxa-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/addspec.py` & `bxa-4.1.0/addspec.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/__init__.py` & `bxa-4.1.0/bxa/sherpa/__init__.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/chandra_1024.json` & `bxa-4.1.0/bxa/sherpa/background/chandra_1024.json`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/erosita_1024.json` & `bxa-4.1.0/bxa/sherpa/background/erosita_1024.json`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/fitters.py` & `bxa-4.1.0/bxa/sherpa/background/fitters.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/kde.py` & `bxa-4.1.0/bxa/sherpa/background/kde.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/models.py` & `bxa-4.1.0/bxa/sherpa/background/models.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/nustar_4096.json` & `bxa-4.1.0/bxa/sherpa/background/nustar_4096.json`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/pca.py` & `bxa-4.1.0/bxa/sherpa/background/pca.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/suzaku_4096.json` & `bxa-4.1.0/bxa/sherpa/background/suzaku_4096.json`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/swift_xrt_1024.json` & `bxa-4.1.0/bxa/sherpa/background/swift_xrt_1024.json`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/xmm.py` & `bxa-4.1.0/bxa/sherpa/background/xmm.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/xmm_2400.json` & `bxa-4.1.0/bxa/sherpa/background/xmm_2400.json`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/xmm_4096.json` & `bxa-4.1.0/bxa/sherpa/background/xmm_4096.json`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/xmm_epn_1024.json` & `bxa-4.1.0/bxa/sherpa/background/xmm_epn_1024.json`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/xmm_epn_4096.json` & `bxa-4.1.0/bxa/sherpa/background/xmm_epn_4096.json`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/xrte_hexa_256.json` & `bxa-4.1.0/bxa/sherpa/background/xrte_hexa_256.json`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/xrte_hexb_256.json` & `bxa-4.1.0/bxa/sherpa/background/xrte_hexb_256.json`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/background/xrte_pca_128.json` & `bxa-4.1.0/bxa/sherpa/background/xrte_pca_128.json`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/cachedmodel.py` & `bxa-4.1.0/bxa/sherpa/cachedmodel.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/galabs.py` & `bxa-4.1.0/bxa/sherpa/galabs.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/invgauss.py` & `bxa-4.1.0/bxa/sherpa/invgauss.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/priors.py` & `bxa-4.1.0/bxa/sherpa/priors.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/qq.py` & `bxa-4.1.0/bxa/sherpa/qq.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/rebinnedmodel.py` & `bxa-4.1.0/bxa/sherpa/rebinnedmodel.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/sherpa/solver.py` & `bxa-4.1.0/bxa/sherpa/solver.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/xspec/__init__.py` & `bxa-4.1.0/bxa/xspec/__init__.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/xspec/gof.py` & `bxa-4.1.0/bxa/xspec/gof.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/xspec/priors.py` & `bxa-4.1.0/bxa/xspec/priors.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/xspec/qq.py` & `bxa-4.1.0/bxa/xspec/qq.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/bxa/xspec/sinning.py` & `bxa-4.1.0/bxa/xspec/sinning.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,76 +10,92 @@
 import scipy.special, scipy.stats
 from . import gof
 import tqdm
 
 
 def group_adapt(xdata, ydata, xlo, xhi, nmin = 20):
 	"""
-	Adaptive grouping into nmin count bins
+	Adaptive grouping into nmin count bins.
+	
+	Args:
+		:param xdata: bin center
+		:param ydata: count values
+		:param xlo: bin lower edge
+		:param xhi: bin upper edge
+		:param nmin: desired minimum number of counts in each bin
+	
+	Returns:
+		sequence of (lower edge, upper edge, number of counts) tuples
 	"""
 	i = 0
 	while i < len(xlo):
 		for j in range(i, len(xlo)):
 			# [i:j] (with j)
 			xmask = numpy.logical_and(xdata >= xlo[i], xdata < xhi[j])
 			
 			if ydata[xmask].sum() >= nmin or j + 1 >= len(xlo):
 				yield (xlo[i], xhi[j], ydata[xmask].sum())
 				#print '  groups', i,j
 				break
 		i = j + 1
 
 
-def binning(outputfiles_basename, bins, widths, data, models):
-	"""
-	Bins the data for plotting.
+def binning(outputfiles_basename, bins, widths, data, models, nmin=20):
+	"""Bins the data for plotting and checks the model.
+
 	Using the gof module, computes a Poisson goodness-of-fit range,
 	i.e. ranges where the model must lie. This is done for multiple
 	binning sizes simultaneously.
+
+	:param outputfiles_basename: not used.
+	:param bins: bin location from Plot.x()
+	:param widths: bin width from Plot.xErr()
+	:param data: counts per bin width from Plot.y() with Plot.background = True and Plot('counts')
+	:param model: counts per bin width predicted by the model, from Plot.model()
+	:param nmin: number of counts per bin to use for rebinning.
 	
-	Returns:
+	Returns
+	--------
 	
-	* marked_binned: data points binned to contain 10 counts
+	* marked_binned: data points binned to contain `nmin` counts
 	  a sequence ready to be passed to matplotlib.pyplot.errorbar
 	* modelrange: range allowed by the data
 	  ready to be passed to matplotlib.pyplot.fill_between
 	* and statistics (GoF measure)
 	
-	outputfiles_basename is not used.
 	"""
 	
 	xdata = bins
 	xlo = bins - widths
 	xhi = bins + widths
 	# convert from densities to counts
 	ydata = numpy.rint(data * widths * 2)
 	models = models * widths * 2
 	
 	best_gof = None
 	best_gof_stats = None
 	data = None
 	
-	grouped_data = list(group_adapt(xdata, ydata, xlo, xhi))
+	grouped_data = list(group_adapt(xdata, ydata, xlo, xhi, nmin=nmin))
 	data = numpy.array([ydata[numpy.logical_and(xdata >= i, xdata < j)].sum() for i, j in zip(xlo, xhi)])
 	
-	for icomponent in range(models.shape[1]):
-		component = models[:,icomponent,:]
-		for i, counts_predicted in enumerate(tqdm.tqdm(component)):
-			modelrange_low, modelrange_high = gof.calc_models_range(data)
+	component = models[:,0,:]
+	for i, counts_predicted in enumerate(tqdm.tqdm(component)):
+		modelrange_low, modelrange_high = gof.calc_models_range(data)
+	
+		stats = gof.calc_multigof(data, counts_predicted)
+		curgof = -numpy.log10(
+			numpy.min([stats[stats[:,0] == n][:,2].min() * (stats[:,0] == n).sum() 
+				for n in sorted(set(stats[:,0]))]) + 1e-300)
 		
-			stats = gof.calc_multigof(data, counts_predicted)
-			curgof = -numpy.log10(
-				numpy.min([stats[stats[:,0] == n][:,2].min() * (stats[:,0] == n).sum() 
-					for n in sorted(set(stats[:,0]))]) + 1e-300)
-			
-			if best_gof is None or curgof < best_gof:
-				best_gof = curgof
-				best_gof_stats = stats
-			if i > 100:
-				break
+		if best_gof is None or curgof < best_gof:
+			best_gof = curgof
+			best_gof_stats = stats
+		if i > 100:
+			break
 
 	# check if we can reproduce the data
 	curgof = best_gof
 	stats = best_gof_stats
 	
 	data_gofp = [numpy.nan] * len(grouped_data)
 	for n in numpy.unique(stats[:,0].astype(int)):
```

### Comparing `bxa-4.0.7/bxa/xspec/solver.py` & `bxa-4.1.0/bxa/xspec/solver.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from . import qq
 from .sinning import binning
 
 from xspec import Xset, AllModels, Fit, Plot
 import xspec
 import matplotlib.pyplot as plt
 from tqdm import tqdm  # if this fails --> pip install tqdm
-from .priors import *
+#from .priors import *
 
 
 class XSilence(object):
 	"""Context for temporarily making xspec quiet."""
 
 	def __enter__(self):
 		self.oldchatter = Xset.chatter, Xset.logChatter
@@ -225,15 +225,15 @@
 					region_filter=False)
 
 			self.sampler.run(**run_kwargs)
 			self.sampler.print_results()
 			self.results = self.sampler.results
 			try:
 				self.sampler.plot()
-			except Exception as e:
+			except Exception:
 				import traceback
 				traceback.print_exc()
 				warnings.warn("plotting failed.")
 
 			logls = [self.results['weighted_samples']['logl'][
 				numpy.where(self.results['weighted_samples']['points'] == sample)[0][0]]
 				for sample in self.results['samples']]
@@ -255,14 +255,18 @@
 
 		The so-created chain can be combined with redshift information to propagate
 		the uncertainty. This is especially important if redshift is a variable
 		parameter in the fit (with some prior).
 
 		Returns erg/cm^2 energy flux (first column) and photon flux (second column)
 		for each posterior sample.
+		
+		:param spectrum: spectrum to use for spectrum.flux
+		:param erange: argument to AllModels.calcFlux, energy range
+		:param nsamples: number of samples to consider (the default, None, means all)
 		"""
 		# prefix = analyzer.outputfiles_basename
 		# modelnames = set([t['model'].name for t in transformations])
 
 		with XSilence():
 			# plot models
 			flux = []
@@ -288,57 +292,48 @@
 		"""
 		# get data, binned to 10 counts
 		# overplot models
 		# can we do this component-wise?
 		data = [None]  # bin, bin width, data and data error
 		models = []    #
 		if component_names is None:
-			component_names = [''] * 100
+			component_names = ['convolved model'] + ['component%d' for i in range(100-1)]
 		if plot_args is None:
 			plot_args = [{}] * 100
+			for i, c in enumerate(plt.rcParams['axes.prop_cycle'].by_key()['color']):
+				plot_args[i] = dict(color=c)
+				del i, c
 		bands = []
 		Plot.background = True
+		Plot.add = True
 
-		def plot_convolved_components(content):
+		for content in self.posterior_predictions_plot(plottype='counts', nsamples=nsamples):
 			xmid = content[:, 0]
 			ndata_columns = 6 if Plot.background else 4
 			ncomponents = content.shape[1] - ndata_columns
 			if data[0] is None:
 				data[0] = content[:, 0:ndata_columns]
 			model_contributions = []
 			for component in range(ncomponents):
 				y = content[:, ndata_columns + component]
-				kwargs = dict(drawstyle='steps', alpha=0.1, color='k')
-				kwargs.update(plot_args[component])
-
-				label = component_names[component]
-				# we only label the first time we enter here
-				# otherwise we get lots of entries in the legend
-				component_names[component] = ''
 				if component >= len(bands):
-					bands.append(PredictionBand(
-						xmid,
-						shadeargs=dict(color=kwargs['color']),
-						lineargs=dict(color=kwargs['color'])))
-				if label != 'ignore':
-					# plt.plot(xmid, y, label=label, **kwargs)
-					bands[component].add(y)
+					bands.append(PredictionBand(xmid))
+				bands[component].add(y)
 
 				model_contributions.append(y)
 			models.append(model_contributions)
 
-		self.posterior_predictions_plot(
-			plottype='counts',
-			callback=plot_convolved_components,
-			nsamples=nsamples)
-
-		for band, label in zip(bands, component_names):
-			band.shade(alpha=0.5, label=label)
-			band.shade(q=0.495, alpha=0.1)
-			band.line()
+		for band, label, component_plot_args in zip(bands, component_names, plot_args):
+			if label == 'ignore': continue
+			lineargs = dict(drawstyle='steps', color='k')
+			lineargs.update(component_plot_args)
+			shadeargs = dict(color=lineargs['color'])
+			band.shade(alpha=0.5, **shadeargs)
+			band.shade(q=0.495, alpha=0.1, **shadeargs)
+			band.line(label=label, **lineargs)
 
 		if Plot.background:
 			results = dict(list(zip('bins,width,data,error,background,backgrounderr'.split(','), data[0].transpose())))
 		else:
 			results = dict(list(zip('bins,width,data,error'.split(','), data[0].transpose())))
 		results['models'] = numpy.array(models)
 		return results
@@ -347,99 +342,90 @@
 		self, component_names=None, plot_args=None, nsamples=400,
 		plottype='model',
 	):
 		"""
 		Plot unconvolved model posterior predictions.
 
 		:param component_names: labels to use. Set to 'ignore' to skip plotting a component
-		:param plot_args: matplotlib.pyplot.plot arguments for each component
+		:param plot_args: list of matplotlib.pyplot.plot arguments for each component, e.g. [dict(color='r'), dict(color='g'), dict(color='b')]
 		:param nsamples: number of posterior samples to use (lower is faster)
+		:param plottype: type of plot string, passed to `xspec.Plot()`
 		"""
 		if component_names is None:
-			component_names = [''] * 100
+			component_names = ['model'] + ['component%d' for i in range(100-1)]
 		if plot_args is None:
 			plot_args = [{}] * 100
+			for i, c in enumerate(plt.rcParams['axes.prop_cycle'].by_key()['color']):
+				plot_args[i] = dict(color=c)
+				del i, c
+		Plot.add = True
 		bands = []
 
-		def plot_unconvolved_components(content):
+		for content in self.posterior_predictions_plot(plottype=plottype, nsamples=nsamples):
 			xmid = content[:, 0]
 			ncomponents = content.shape[1] - 2
 			for component in range(ncomponents):
 				y = content[:, 2 + component]
-				kwargs = dict(drawstyle='steps', alpha=0.1, color='k')
-				kwargs.update(plot_args[component])
 
-				label = component_names[component]
-				# we only label the first time we enter here
-				# otherwise we get lots of entries in the legend
-				component_names[component] = ''
 				if component >= len(bands):
-					bands.append(PredictionBand(
-						xmid,
-						shadeargs=dict(color=kwargs['color']),
-						lineargs=dict(color=kwargs['color'])))
-				if label != 'ignore':
-					# plt.plot(xmid, y, label=label, **kwargs)
-					bands[component].add(y)
-
-		self.posterior_predictions_plot(
-			plottype=plottype,
-			callback=plot_unconvolved_components,
-			nsamples=nsamples)
-		for band, label in zip(bands, component_names):
-			band.shade(alpha=0.5, label=label)
-			band.shade(q=0.495, alpha=0.1)
-			band.line()
+					bands.append(PredictionBand(xmid))
+				bands[component].add(y)
+
+		for band, label, component_plot_args in zip(bands, component_names, plot_args):
+			if label == 'ignore': continue
+			lineargs = dict(drawstyle='steps', color='k')
+			lineargs.update(component_plot_args)
+			shadeargs = dict(color=lineargs['color'])
+			band.shade(alpha=0.5, **shadeargs)
+			band.shade(q=0.495, alpha=0.1, **shadeargs)
+			band.line(label=label, **lineargs)
 
-	def posterior_predictions_plot(self, plottype, callback, nsamples=None):
+	def posterior_predictions_plot(self, plottype, nsamples=None):
 		"""
 		Internal Routine used by posterior_predictions_unconvolved, posterior_predictions_convolved
 		"""
-		posterior = self.posterior
 		# for plotting, we don't need so many points, and especially the
 		# points that barely made it into the analysis are not that interesting.
 		# so pick a random subset of at least nsamples points
-		if nsamples is not None and len(posterior) > nsamples:
-			if hasattr(numpy.random, 'choice'):
-				chosen = numpy.random.choice(
-					numpy.arange(len(posterior)),
-					replace=False, size=nsamples)
-			else:
-				chosen = list(set(numpy.random.randint(
-					0, len(posterior), size=10 * nsamples)))[:nsamples]
-			posterior = posterior[chosen, :]
-			assert len(posterior) == nsamples
-		prefix = self.outputfiles_basename
-		tmpfilename = os.path.join(os.path.dirname(prefix), os.path.basename(prefix).replace('.', '_') + '-wdatatmp.qdp')
-		if os.path.exists(tmpfilename):
-			os.remove(tmpfilename)
+		posterior = self.posterior[:nsamples]
 
 		with XSilence():
 			olddevice = Plot.device
 			Plot.device = '/null'
-			# modelnames = set([t['model'].name for t in transformations])
-
-			while len(Plot.commands) > 0:
-				Plot.delCommand(1)
-			Plot.addCommand('wdata "%s"' % tmpfilename.replace('.qdp', ''))
 
 			# plot models
+			maxncomp = 100 if Plot.add else 0
 			for k, row in enumerate(tqdm(posterior, disable=None)):
 				set_parameters(values=row, transformations=self.transformations)
-				if os.path.exists(tmpfilename):
-					os.remove(tmpfilename)
-				xspec.Plot(plottype)
-				content = numpy.genfromtxt(tmpfilename, skip_header=3)
-				os.remove(tmpfilename)
-				callback(content)
-			xspec.Plot.device = olddevice
-			while len(Plot.commands) > 0:
-				Plot.delCommand(1)
-			if os.path.exists(tmpfilename):
-				os.remove(tmpfilename)
+				Plot(plottype)
+				# get plot data
+				if plottype == 'model':
+					base_content = numpy.transpose([
+						Plot.x(), Plot.xErr(), Plot.model()])
+				elif Plot.background:
+					base_content = numpy.transpose([
+						Plot.x(), Plot.xErr(), Plot.y(), Plot.yErr(),
+						Plot.backgroundVals(), numpy.zeros_like(Plot.backgroundVals()),
+						Plot.model()])
+				else:
+					base_content = numpy.transpose([
+						Plot.x(), Plot.xErr(), Plot.y(), Plot.yErr(),
+						Plot.model()])
+				# get additive components, if there are any
+				comp = []
+				for i in range(1, maxncomp):
+					try:
+						comp.append(Plot.addComp(i))
+					except Exception:
+						print('The error "***XSPEC Error: Requested array does not exist for this plot." can be ignored.')
+						maxncomp = i
+						break	
+				content = numpy.hstack((base_content, numpy.transpose(comp).reshape((len(base_content), -1))))
+				yield content
+			Plot.device = olddevice
 
 
 def standard_analysis(
 	transformations, outputfiles_basename,
 	skipsteps=[], **kwargs
 ):
 	"""
@@ -457,14 +443,15 @@
 	* prints out model evidence
 
 	Look at the source of this function to figure out how to do
 	the individual parts.
 	Copy them to your scripts and adapt them to your needs.
 	"""
 	#   run nested sampling
+	warnings.warn("standard_analysis() is deprecated and will be removed in future BXA releases.")
 	print('running analysis ...')
 	solver = BXASolver(
 		transformations=transformations,
 		outputfiles_basename=outputfiles_basename)
 	solver.run(**kwargs)
 	print('running analysis ... done')
```

### Comparing `bxa-4.0.7/bxa.egg-info/PKG-INFO` & `bxa-4.1.0/bxa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bxa
-Version: 4.0.7
+Version: 4.1.0
 Summary: Bayesian X-ray spectral analysis
 Home-page: https://github.com/JohannesBuchner/BXA/
 Author: Johannes Buchner
 Author-email: johannes.buchner.acad@gmx.com
 License: GNU General Public License v3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bxa-4.0.7/bxa.egg-info/SOURCES.txt` & `bxa-4.1.0/bxa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/fixkeywords.py` & `bxa-4.1.0/fixkeywords.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/gal.py` & `bxa-4.1.0/gal.py`

 * *Files identical despite different names*

### Comparing `bxa-4.0.7/setup.py` & `bxa-4.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 except ImportError:
     sherpa_available = False
 
 if not sherpa_available and not xspec_available:
     warnings.warn("BXA is a plugin for xspec/sherpa, but neither xspec nor sherpa are installed in the current environment!")
 
 setup(name='bxa',
-    version='4.0.7',
+    version='4.1.0',
     author='Johannes Buchner',
     url='https://github.com/JohannesBuchner/BXA/',
     author_email='johannes.buchner.acad@gmx.com',
     description='Bayesian X-ray spectral analysis',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
```

