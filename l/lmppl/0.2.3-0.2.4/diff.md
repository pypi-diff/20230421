# Comparing `tmp/lmppl-0.2.3.tar.gz` & `tmp/lmppl-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmppl-0.2.3.tar", last modified: Wed Apr  5 16:38:39 2023, max compression
+gzip compressed data, was "lmppl-0.2.4.tar", last modified: Fri Apr 21 10:45:41 2023, max compression
```

## Comparing `lmppl-0.2.3.tar` & `lmppl-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-05 16:38:39.739261 lmppl-0.2.3/
--rw-r--r--   0 asahi      (501) staff       (20)     1064 2023-02-07 11:28:13.000000 lmppl-0.2.3/LICENSE.txt
--rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-04-05 16:38:39.739468 lmppl-0.2.3/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)     4437 2023-02-09 18:23:49.000000 lmppl-0.2.3/README.md
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-05 16:38:39.734375 lmppl-0.2.3/lmppl/
--rw-r--r--   0 asahi      (501) staff       (20)      150 2023-04-05 16:38:19.000000 lmppl-0.2.3/lmppl/__init__.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-05 16:38:39.737099 lmppl-0.2.3/lmppl/lmppl_cl/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2023-02-07 11:25:50.000000 lmppl-0.2.3/lmppl/lmppl_cl/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     1999 2023-04-05 16:36:36.000000 lmppl-0.2.3/lmppl/openai_models.py
--rw-r--r--   0 asahi      (501) staff       (20)     8597 2023-04-01 16:15:20.000000 lmppl-0.2.3/lmppl/ppl_encoder_decoder_lm.py
--rw-r--r--   0 asahi      (501) staff       (20)     6883 2023-03-10 20:47:02.000000 lmppl-0.2.3/lmppl/ppl_mlm.py
--rw-r--r--   0 asahi      (501) staff       (20)     5709 2023-04-02 14:48:07.000000 lmppl-0.2.3/lmppl/ppl_recurrent_lm.py
--rw-r--r--   0 asahi      (501) staff       (20)      227 2023-02-07 13:19:37.000000 lmppl-0.2.3/lmppl/util.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-05 16:38:39.736674 lmppl-0.2.3/lmppl.egg-info/
--rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-04-05 16:38:39.000000 lmppl-0.2.3/lmppl.egg-info/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)      399 2023-04-05 16:38:39.000000 lmppl-0.2.3/lmppl.egg-info/SOURCES.txt
--rw-r--r--   0 asahi      (501) staff       (20)        1 2023-04-05 16:38:39.000000 lmppl-0.2.3/lmppl.egg-info/dependency_links.txt
--rw-r--r--   0 asahi      (501) staff       (20)       79 2023-04-05 16:38:39.000000 lmppl-0.2.3/lmppl.egg-info/requires.txt
--rw-r--r--   0 asahi      (501) staff       (20)        6 2023-04-05 16:38:39.000000 lmppl-0.2.3/lmppl.egg-info/top_level.txt
--rw-r--r--   0 asahi      (501) staff       (20)       38 2023-04-05 16:38:39.739973 lmppl-0.2.3/setup.cfg
--rw-r--r--   0 asahi      (501) staff       (20)     1760 2023-04-05 16:37:50.000000 lmppl-0.2.3/setup.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-05 16:38:39.738373 lmppl-0.2.3/test/
--rw-r--r--   0 asahi      (501) staff       (20)     1249 2023-02-09 19:14:51.000000 lmppl-0.2.3/test/test_analogy.py
--rw-r--r--   0 asahi      (501) staff       (20)     2261 2023-02-12 13:50:45.000000 lmppl-0.2.3/test/test_model_with_simple_input.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-21 10:45:41.279328 lmppl-0.2.4/
+-rw-r--r--   0 asahi      (501) staff       (20)     1064 2023-02-07 11:28:13.000000 lmppl-0.2.4/LICENSE.txt
+-rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-04-21 10:45:41.279514 lmppl-0.2.4/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)     4437 2023-02-09 18:23:49.000000 lmppl-0.2.4/README.md
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-21 10:45:41.274244 lmppl-0.2.4/lmppl/
+-rw-r--r--   0 asahi      (501) staff       (20)      150 2023-04-05 16:38:19.000000 lmppl-0.2.4/lmppl/__init__.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-21 10:45:41.276872 lmppl-0.2.4/lmppl/lmppl_cl/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2023-02-07 11:25:50.000000 lmppl-0.2.4/lmppl/lmppl_cl/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2642 2023-04-21 10:44:59.000000 lmppl-0.2.4/lmppl/openai_models.py
+-rw-r--r--   0 asahi      (501) staff       (20)     8597 2023-04-01 16:15:20.000000 lmppl-0.2.4/lmppl/ppl_encoder_decoder_lm.py
+-rw-r--r--   0 asahi      (501) staff       (20)     6883 2023-03-10 20:47:02.000000 lmppl-0.2.4/lmppl/ppl_mlm.py
+-rw-r--r--   0 asahi      (501) staff       (20)     5709 2023-04-02 14:48:07.000000 lmppl-0.2.4/lmppl/ppl_recurrent_lm.py
+-rw-r--r--   0 asahi      (501) staff       (20)      227 2023-02-07 13:19:37.000000 lmppl-0.2.4/lmppl/util.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-21 10:45:41.276505 lmppl-0.2.4/lmppl.egg-info/
+-rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-04-21 10:45:41.000000 lmppl-0.2.4/lmppl.egg-info/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)      399 2023-04-21 10:45:41.000000 lmppl-0.2.4/lmppl.egg-info/SOURCES.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        1 2023-04-21 10:45:41.000000 lmppl-0.2.4/lmppl.egg-info/dependency_links.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       79 2023-04-21 10:45:41.000000 lmppl-0.2.4/lmppl.egg-info/requires.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        6 2023-04-21 10:45:41.000000 lmppl-0.2.4/lmppl.egg-info/top_level.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       38 2023-04-21 10:45:41.280008 lmppl-0.2.4/setup.cfg
+-rw-r--r--   0 asahi      (501) staff       (20)     1760 2023-04-21 10:45:28.000000 lmppl-0.2.4/setup.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-21 10:45:41.278450 lmppl-0.2.4/test/
+-rw-r--r--   0 asahi      (501) staff       (20)     1249 2023-02-09 19:14:51.000000 lmppl-0.2.4/test/test_analogy.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2261 2023-02-12 13:50:45.000000 lmppl-0.2.4/test/test_model_with_simple_input.py
```

### Comparing `lmppl-0.2.3/LICENSE.txt` & `lmppl-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.3/PKG-INFO` & `lmppl-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lmppl
-Version: 0.2.3
+Version: 0.2.4
 Summary: Calculate perplexity on the text with pre-trained language models.
 Home-page: https://github.com/asahi417/lmppl
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT License
-Download-URL: https://github.com/asahi417/lmppl/archive/v0.2.3.tar.gz
+Download-URL: https://github.com/asahi417/lmppl/archive/v0.2.4.tar.gz
 Keywords: language model,t5,gpt3,bert,perplexity,nlp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lmppl-0.2.3/README.md` & `lmppl-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.3/lmppl/ppl_encoder_decoder_lm.py` & `lmppl-0.2.4/lmppl/ppl_encoder_decoder_lm.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.3/lmppl/ppl_mlm.py` & `lmppl-0.2.4/lmppl/ppl_mlm.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.3/lmppl/ppl_recurrent_lm.py` & `lmppl-0.2.4/lmppl/ppl_recurrent_lm.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.3/lmppl.egg-info/PKG-INFO` & `lmppl-0.2.4/lmppl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lmppl
-Version: 0.2.3
+Version: 0.2.4
 Summary: Calculate perplexity on the text with pre-trained language models.
 Home-page: https://github.com/asahi417/lmppl
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT License
-Download-URL: https://github.com/asahi417/lmppl/archive/v0.2.3.tar.gz
+Download-URL: https://github.com/asahi417/lmppl/archive/v0.2.4.tar.gz
 Keywords: language model,t5,gpt3,bert,perplexity,nlp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lmppl-0.2.3/setup.py` & `lmppl-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
-VERSION = '0.2.3'
+VERSION = '0.2.4'
 NAME = 'lmppl'
 LICENSE = 'MIT License'
 setup(
     name=NAME,
     packages=find_packages(exclude=['tests', 'misc', 'asset']),
     version=VERSION,
     license=LICENSE,
```

### Comparing `lmppl-0.2.3/test/test_analogy.py` & `lmppl-0.2.4/test/test_analogy.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.3/test/test_model_with_simple_input.py` & `lmppl-0.2.4/test/test_model_with_simple_input.py`

 * *Files identical despite different names*

