# Comparing `tmp/ga4gh.vrsatile.pydantic-0.1.dev5.tar.gz` & `tmp/ga4gh.vrsatile.pydantic-0.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ga4gh.vrsatile.pydantic-0.1.dev5.tar", last modified: Thu Dec  8 20:39:49 2022, max compression
+gzip compressed data, was "ga4gh.vrsatile.pydantic-0.1.dev6.tar", last modified: Tue Dec 13 16:59:38 2022, max compression
```

## Comparing `ga4gh.vrsatile.pydantic-0.1.dev5.tar` & `ga4gh.vrsatile.pydantic-0.1.dev6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:39:49.367201 ga4gh.vrsatile.pydantic-0.1.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2022-12-08 20:39:41.000000 ga4gh.vrsatile.pydantic-0.1.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2022-12-08 20:39:49.367201 ga4gh.vrsatile.pydantic-0.1.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2022-12-08 20:39:41.000000 ga4gh.vrsatile.pydantic-0.1.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2022-12-08 20:39:49.367201 ga4gh.vrsatile.pydantic-0.1.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-08 20:39:41.000000 ga4gh.vrsatile.pydantic-0.1.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:39:49.367201 ga4gh.vrsatile.pydantic-0.1.dev5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:39:49.367201 ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:39:49.367201 ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh/vrsatile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:39:49.367201 ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh/vrsatile/pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2022-12-08 20:39:41.000000 ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh/vrsatile/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2022-12-08 20:39:41.000000 ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh/vrsatile/pydantic/core_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2022-12-08 20:39:41.000000 ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh/vrsatile/pydantic/vrs_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2022-12-08 20:39:41.000000 ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh/vrsatile/pydantic/vrsatile_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:39:49.367201 ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh.vrsatile.pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2022-12-08 20:39:49.000000 ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh.vrsatile.pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2022-12-08 20:39:49.000000 ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh.vrsatile.pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 20:39:49.000000 ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh.vrsatile.pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 20:39:49.000000 ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh.vrsatile.pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-08 20:39:49.000000 ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh.vrsatile.pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-08 20:39:49.000000 ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh.vrsatile.pydantic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:59:38.513420 ga4gh.vrsatile.pydantic-0.1.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2022-12-13 16:59:30.000000 ga4gh.vrsatile.pydantic-0.1.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2022-12-13 16:59:38.513420 ga4gh.vrsatile.pydantic-0.1.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2022-12-13 16:59:30.000000 ga4gh.vrsatile.pydantic-0.1.dev6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2022-12-13 16:59:38.513420 ga4gh.vrsatile.pydantic-0.1.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-13 16:59:30.000000 ga4gh.vrsatile.pydantic-0.1.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:59:38.509420 ga4gh.vrsatile.pydantic-0.1.dev6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:59:38.509420 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:59:38.509420 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:59:38.513420 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2022-12-13 16:59:30.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2022-12-13 16:59:30.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/pydantic/core_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13988 2022-12-13 16:59:30.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/pydantic/vrs_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2022-12-13 16:59:30.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/pydantic/vrsatile_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:59:38.513420 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2022-12-13 16:59:38.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2022-12-13 16:59:38.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 16:59:38.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 16:59:38.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-13 16:59:38.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-13 16:59:38.000000 ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/top_level.txt
```

### Comparing `ga4gh.vrsatile.pydantic-0.1.dev5/LICENSE` & `ga4gh.vrsatile.pydantic-0.1.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `ga4gh.vrsatile.pydantic-0.1.dev5/PKG-INFO` & `ga4gh.vrsatile.pydantic-0.1.dev6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga4gh.vrsatile.pydantic
-Version: 0.1.dev5
+Version: 0.1.dev6
 Summary: "Translation of the GA4GH VRS and VRSATILE Schemas to a Pydantic data model"
 Home-page: https://github.com/ga4gh/vrs-pydantic
 Author: Alex H. Wagner
 Author-email: alex.wagner@nationwidechildrens.org
 Keywords: bioinformatics,ga4gh,genomics,hgvs,spdi,variation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ga4gh.vrsatile.pydantic-0.1.dev5/README.md` & `ga4gh.vrsatile.pydantic-0.1.dev6/README.md`

 * *Files identical despite different names*

### Comparing `ga4gh.vrsatile.pydantic-0.1.dev5/setup.cfg` & `ga4gh.vrsatile.pydantic-0.1.dev6/setup.cfg`

 * *Files identical despite different names*

### Comparing `ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh/vrsatile/pydantic/__init__.py` & `ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh/vrsatile/pydantic/core_models.py` & `ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/pydantic/core_models.py`

 * *Files identical despite different names*

### Comparing `ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh/vrsatile/pydantic/vrs_models.py` & `ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/pydantic/vrs_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
 
 class RelativeCopyClass(str, Enum):
     """The relative copy class"""
 
     COPY_NUMBER_GAIN = "EFO:0030070"
     HIGH_LEVEL_COPY_NUMBER_GAIN = "EFO:0030072"
-    FOCAL_GENOME_AMPLIFICATION = "EFO:0030073"
     LOW_LEVEL_COPY_NUMBER_GAIN = "EFO:0030071"
     COPY_NUMBER_LOSS = "EFO:0030067"
     COMPLETE_GENOMIC_DELETION = "EFO:0030069"
     LOW_LEVEL_COPY_NUMBER_LOSS = "EFO:0030068"
 
 
 # =============================================================================
```

### Comparing `ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh/vrsatile/pydantic/vrsatile_models.py` & `ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh/vrsatile/pydantic/vrsatile_models.py`

 * *Files identical despite different names*

### Comparing `ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh.vrsatile.pydantic.egg-info/PKG-INFO` & `ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga4gh.vrsatile.pydantic
-Version: 0.1.dev5
+Version: 0.1.dev6
 Summary: "Translation of the GA4GH VRS and VRSATILE Schemas to a Pydantic data model"
 Home-page: https://github.com/ga4gh/vrs-pydantic
 Author: Alex H. Wagner
 Author-email: alex.wagner@nationwidechildrens.org
 Keywords: bioinformatics,ga4gh,genomics,hgvs,spdi,variation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ga4gh.vrsatile.pydantic-0.1.dev5/src/ga4gh.vrsatile.pydantic.egg-info/SOURCES.txt` & `ga4gh.vrsatile.pydantic-0.1.dev6/src/ga4gh.vrsatile.pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

