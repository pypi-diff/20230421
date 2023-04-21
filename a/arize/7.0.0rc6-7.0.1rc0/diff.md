# Comparing `tmp/arize-7.0.0rc6.tar.gz` & `tmp/arize-7.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arize-7.0.0rc6.tar", last modified: Thu Apr 13 01:46:58 2023, max compression
+gzip compressed data, was "arize-7.0.1rc0.tar", last modified: Fri Apr 21 19:39:04 2023, max compression
```

## Comparing `arize-7.0.0rc6.tar` & `arize-7.0.1rc0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.220308 arize-7.0.0rc6/
--rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-03-30 21:17:25.000000 arize-7.0.0rc6/LICENSE.md
--rw-r--r--   0 kiko       (501) staff       (20)       65 2023-03-30 21:17:25.000000 arize-7.0.0rc6/MANIFEST.in
--rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-04-13 01:46:58.220851 arize-7.0.0rc6/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-03-30 21:17:25.000000 arize-7.0.0rc6/README.md
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.148036 arize-7.0.0rc6/arize/
--rw-r--r--   0 kiko       (501) staff       (20)       25 2023-04-13 01:46:45.000000 arize-7.0.0rc6/arize/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    26240 2023-04-13 01:39:58.000000 arize-7.0.0rc6/arize/api.py
--rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/bounded_executor.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.169092 arize-7.0.0rc6/arize/examples/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/examples/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/examples/bulk_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/examples/bulk_client_shap.py
--rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/examples/client_shap_values.py
--rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/examples/log_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-04-10 03:28:13.000000 arize-7.0.0rc6/arize/examples/log_pandas_dataframe.py
--rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/examples/preproduction_client.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.170804 arize-7.0.0rc6/arize/pandas/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/pandas/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.182041 arize-7.0.0rc6/arize/pandas/embeddings/
--rw-r--r--   0 kiko       (501) staff       (20)      124 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/pandas/embeddings/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-04-11 17:42:22.000000 arize-7.0.0rc6/arize/pandas/embeddings/auto_generator.py
--rw-r--r--   0 kiko       (501) staff       (20)     6583 2023-04-10 21:49:18.000000 arize-7.0.0rc6/arize/pandas/embeddings/base_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      213 2023-04-10 22:55:57.000000 arize-7.0.0rc6/arize/pandas/embeddings/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     1962 2023-04-10 03:28:13.000000 arize-7.0.0rc6/arize/pandas/embeddings/cv_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      571 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/pandas/embeddings/models.py
--rw-r--r--   0 kiko       (501) staff       (20)     3576 2023-04-13 01:39:58.000000 arize-7.0.0rc6/arize/pandas/embeddings/nlp_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)     5809 2023-04-10 03:28:13.000000 arize-7.0.0rc6/arize/pandas/embeddings/tabular_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      412 2023-04-10 22:55:57.000000 arize-7.0.0rc6/arize/pandas/embeddings/usecases.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.182921 arize-7.0.0rc6/arize/pandas/generative/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-10 22:55:57.000000 arize-7.0.0rc6/arize/pandas/generative/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.200864 arize-7.0.0rc6/arize/pandas/generative/llm_evaluation/
--rw-r--r--   0 kiko       (501) staff       (20)      160 2023-04-10 22:55:57.000000 arize-7.0.0rc6/arize/pandas/generative/llm_evaluation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      183 2023-04-10 22:55:57.000000 arize-7.0.0rc6/arize/pandas/generative/llm_evaluation/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)    12188 2023-04-11 17:42:22.000000 arize-7.0.0rc6/arize/pandas/generative/llm_evaluation/hf_metrics.py
--rw-r--r--   0 kiko       (501) staff       (20)    22747 2023-04-13 01:39:58.000000 arize-7.0.0rc6/arize/pandas/logger.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.202383 arize-7.0.0rc6/arize/pandas/surrogate_explainer/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/pandas/surrogate_explainer/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     4910 2023-04-10 03:28:13.000000 arize-7.0.0rc6/arize/pandas/surrogate_explainer/mimic.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.204990 arize-7.0.0rc6/arize/pandas/validation/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/pandas/validation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    23189 2023-04-13 01:39:58.000000 arize-7.0.0rc6/arize/pandas/validation/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)    60237 2023-04-13 01:39:58.000000 arize-7.0.0rc6/arize/pandas/validation/validator.py
--rw-r--r--   0 kiko       (501) staff       (20)   167683 2023-04-13 01:39:58.000000 arize-7.0.0rc6/arize/public_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.210885 arize-7.0.0rc6/arize/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/utils/logging.py
--rw-r--r--   0 kiko       (501) staff       (20)     4177 2023-04-10 23:06:12.000000 arize-7.0.0rc6/arize/utils/model_mapping.json
--rw-r--r--   0 kiko       (501) staff       (20)    22046 2023-04-11 17:42:22.000000 arize-7.0.0rc6/arize/utils/types.py
--rw-r--r--   0 kiko       (501) staff       (20)     7229 2023-04-11 17:42:22.000000 arize-7.0.0rc6/arize/utils/utils.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.161838 arize-7.0.0rc6/arize.egg-info/
--rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-04-13 01:46:58.000000 arize-7.0.0rc6/arize.egg-info/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)     1463 2023-04-13 01:46:58.000000 arize-7.0.0rc6/arize.egg-info/SOURCES.txt
--rw-r--r--   0 kiko       (501) staff       (20)        1 2023-04-13 01:46:58.000000 arize-7.0.0rc6/arize.egg-info/dependency_links.txt
--rw-r--r--   0 kiko       (501) staff       (20)      434 2023-04-13 01:46:58.000000 arize-7.0.0rc6/arize.egg-info/requires.txt
--rw-r--r--   0 kiko       (501) staff       (20)        6 2023-04-13 01:46:58.000000 arize-7.0.0rc6/arize.egg-info/top_level.txt
--rw-r--r--   0 kiko       (501) staff       (20)      167 2023-03-30 21:17:25.000000 arize-7.0.0rc6/pyproject.toml
--rw-r--r--   0 kiko       (501) staff       (20)     1522 2023-04-13 01:46:58.224384 arize-7.0.0rc6/setup.cfg
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.213599 arize-7.0.0rc6/tests/
--rw-r--r--   0 kiko       (501) staff       (20)    44544 2023-04-13 01:39:58.000000 arize-7.0.0rc6/tests/test_api.py
--rw-r--r--   0 kiko       (501) staff       (20)      952 2023-03-30 21:17:25.000000 arize-7.0.0rc6/tests/test_utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:04.051568 arize-7.0.1rc0/
+-rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-03-30 21:17:25.000000 arize-7.0.1rc0/LICENSE.md
+-rw-r--r--   0 kiko       (501) staff       (20)       65 2023-03-30 21:17:25.000000 arize-7.0.1rc0/MANIFEST.in
+-rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-04-21 19:39:04.052714 arize-7.0.1rc0/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-03-30 21:17:25.000000 arize-7.0.1rc0/README.md
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:03.940431 arize-7.0.1rc0/arize/
+-rw-r--r--   0 kiko       (501) staff       (20)       25 2023-04-21 19:37:33.000000 arize-7.0.1rc0/arize/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    26430 2023-04-21 06:56:16.000000 arize-7.0.1rc0/arize/api.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/bounded_executor.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:03.978476 arize-7.0.1rc0/arize/examples/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/examples/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/examples/bulk_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/examples/bulk_client_shap.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/examples/client_shap_values.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/examples/log_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-04-10 03:28:13.000000 arize-7.0.1rc0/arize/examples/log_pandas_dataframe.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/examples/preproduction_client.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:03.980297 arize-7.0.1rc0/arize/pandas/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/pandas/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:03.999123 arize-7.0.1rc0/arize/pandas/embeddings/
+-rw-r--r--   0 kiko       (501) staff       (20)      124 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/pandas/embeddings/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-04-18 19:34:15.000000 arize-7.0.1rc0/arize/pandas/embeddings/auto_generator.py
+-rw-r--r--   0 kiko       (501) staff       (20)     6583 2023-04-18 21:41:36.000000 arize-7.0.1rc0/arize/pandas/embeddings/base_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      213 2023-04-13 06:03:38.000000 arize-7.0.1rc0/arize/pandas/embeddings/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1962 2023-04-10 03:28:13.000000 arize-7.0.1rc0/arize/pandas/embeddings/cv_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      571 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/pandas/embeddings/models.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3576 2023-04-13 06:03:38.000000 arize-7.0.1rc0/arize/pandas/embeddings/nlp_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5809 2023-04-10 03:28:13.000000 arize-7.0.1rc0/arize/pandas/embeddings/tabular_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      412 2023-04-13 06:03:38.000000 arize-7.0.1rc0/arize/pandas/embeddings/usecases.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:04.000800 arize-7.0.1rc0/arize/pandas/generative/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-13 06:03:38.000000 arize-7.0.1rc0/arize/pandas/generative/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:04.031073 arize-7.0.1rc0/arize/pandas/generative/llm_evaluation/
+-rw-r--r--   0 kiko       (501) staff       (20)      160 2023-04-13 06:03:38.000000 arize-7.0.1rc0/arize/pandas/generative/llm_evaluation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      183 2023-04-13 06:03:38.000000 arize-7.0.1rc0/arize/pandas/generative/llm_evaluation/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)    12188 2023-04-21 06:56:16.000000 arize-7.0.1rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py
+-rw-r--r--   0 kiko       (501) staff       (20)    22774 2023-04-21 19:38:35.000000 arize-7.0.1rc0/arize/pandas/logger.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:04.034056 arize-7.0.1rc0/arize/pandas/surrogate_explainer/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/pandas/surrogate_explainer/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4910 2023-04-21 06:56:16.000000 arize-7.0.1rc0/arize/pandas/surrogate_explainer/mimic.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:04.038118 arize-7.0.1rc0/arize/pandas/validation/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/pandas/validation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    22928 2023-04-21 06:56:16.000000 arize-7.0.1rc0/arize/pandas/validation/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)    59550 2023-04-21 06:56:16.000000 arize-7.0.1rc0/arize/pandas/validation/validator.py
+-rw-r--r--   0 kiko       (501) staff       (20)   169752 2023-04-19 18:46:11.000000 arize-7.0.1rc0/arize/public_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:04.045198 arize-7.0.1rc0/arize/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/utils/logging.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4995 2023-04-19 18:46:11.000000 arize-7.0.1rc0/arize/utils/model_mapping.json
+-rw-r--r--   0 kiko       (501) staff       (20)    22046 2023-04-21 06:56:16.000000 arize-7.0.1rc0/arize/utils/types.py
+-rw-r--r--   0 kiko       (501) staff       (20)     7229 2023-04-21 06:56:16.000000 arize-7.0.1rc0/arize/utils/utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:03.949528 arize-7.0.1rc0/arize.egg-info/
+-rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-04-21 19:39:03.000000 arize-7.0.1rc0/arize.egg-info/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)     1463 2023-04-21 19:39:03.000000 arize-7.0.1rc0/arize.egg-info/SOURCES.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        1 2023-04-21 19:39:03.000000 arize-7.0.1rc0/arize.egg-info/dependency_links.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      434 2023-04-21 19:39:03.000000 arize-7.0.1rc0/arize.egg-info/requires.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        6 2023-04-21 19:39:03.000000 arize-7.0.1rc0/arize.egg-info/top_level.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      167 2023-03-30 21:17:25.000000 arize-7.0.1rc0/pyproject.toml
+-rw-r--r--   0 kiko       (501) staff       (20)     1522 2023-04-21 19:39:04.055934 arize-7.0.1rc0/setup.cfg
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:04.050238 arize-7.0.1rc0/tests/
+-rw-r--r--   0 kiko       (501) staff       (20)    44544 2023-04-21 06:56:16.000000 arize-7.0.1rc0/tests/test_api.py
+-rw-r--r--   0 kiko       (501) staff       (20)      952 2023-03-30 21:17:25.000000 arize-7.0.1rc0/tests/test_utils.py
```

### Comparing `arize-7.0.0rc6/LICENSE.md` & `arize-7.0.1rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/PKG-INFO` & `arize-7.0.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.0rc6
+Version: 7.0.1rc0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.0rc6/README.md` & `arize-7.0.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/api.py` & `arize-7.0.1rc0/arize/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,23 +404,25 @@
 def _validate_categorical_label(
     model_type: ModelTypes,
     label: Union[str, bool, int, float, Tuple[Union[str, bool], float]],
 ):
     is_valid = (
         isinstance(label, str)
         or isinstance(label, bool)
+        or isinstance(label, int)
+        or isinstance(label, float)
         or (
             isinstance(label, tuple)
             and isinstance(label[0], (str, bool))
             and isinstance(label[1], float)
         )
     )
     if not is_valid:
         raise TypeError(
-            f"label {label} has type {type(label)}, but must be str, bool, or Tuple[str, "
+            f"label {label} has type {type(label)}, but must be str, bool, int, float or Tuple[str, "
             f"float] for ModelTypes.{model_type}"
         )
     if isinstance(label, tuple) and label[1] is np.nan:
         raise ValueError(
             f"Prediction confidence score for ModelTypes.{model_type} cannot be null value"
         )
 
@@ -507,14 +509,16 @@
     value: Union[bool, str, Tuple[str, float]],
 ) -> Union[pb2.PredictionLabel, pb2.ActualLabel]:
     sc = pb2.ScoreCategorical()
     if isinstance(value, bool):
         sc.category.category = str(value)
     elif isinstance(value, str):
         sc.category.category = value
+    elif isinstance(value, int) or isinstance(value, float):
+        sc.score_value.value = value
     elif isinstance(value, tuple):
         # Expect Tuple[str,float]
         if value[1] is None:
             raise TypeError(
                 f"Received {prediction_or_actual}_label = {value}, of type "
                 f"{type(value)}[{type(value[0])}, None]. "
                 f"{[mt.prediction_or_actual for mt in CATEGORICAL_MODEL_TYPES]} models accept "
@@ -532,15 +536,15 @@
         else:
             sc.score_category.category = value[0]
         sc.score_category.score = value[1]
     else:
         raise TypeError(
             f"Received {prediction_or_actual}_label = {value}, of type {type(value)}. "
             + f"{[mt.prediction_or_actual for mt in CATEGORICAL_MODEL_TYPES]} models accept values "
-            f"of type str, bool, or Tuple[str, float]"
+            f"of type str, bool, int, float or Tuple[str, float]"
         )
     if prediction_or_actual == "prediction":
         return pb2.PredictionLabel(score_categorical=sc)
     elif prediction_or_actual == "actual":
         return pb2.ActualLabel(score_categorical=sc)
```

### Comparing `arize-7.0.0rc6/arize/bounded_executor.py` & `arize-7.0.1rc0/arize/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/examples/bulk_client.py` & `arize-7.0.1rc0/arize/examples/bulk_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/examples/bulk_client_shap.py` & `arize-7.0.1rc0/arize/examples/bulk_client_shap.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/examples/client_shap_values.py` & `arize-7.0.1rc0/arize/examples/client_shap_values.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/examples/log_client.py` & `arize-7.0.1rc0/arize/examples/log_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/examples/log_pandas_dataframe.py` & `arize-7.0.1rc0/arize/examples/log_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/examples/preproduction_client.py` & `arize-7.0.1rc0/arize/examples/preproduction_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/pandas/embeddings/auto_generator.py` & `arize-7.0.1rc0/arize/pandas/embeddings/auto_generator.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/pandas/embeddings/base_generators.py` & `arize-7.0.1rc0/arize/pandas/embeddings/base_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/pandas/embeddings/cv_generators.py` & `arize-7.0.1rc0/arize/pandas/embeddings/cv_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/pandas/embeddings/models.py` & `arize-7.0.1rc0/arize/pandas/embeddings/models.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/pandas/embeddings/nlp_generators.py` & `arize-7.0.1rc0/arize/pandas/embeddings/nlp_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/pandas/embeddings/tabular_generators.py` & `arize-7.0.1rc0/arize/pandas/embeddings/tabular_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/pandas/generative/llm_evaluation/hf_metrics.py` & `arize-7.0.1rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/pandas/logger.py` & `arize-7.0.1rc0/arize/pandas/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         :class:`Response` object from the Requests HTTP library to ensure successful delivery of
         records.
 
         :param dataframe (pd.DataFrame): The dataframe containing model data.
         :param schema (Schema): A Schema instance that specifies the column names for corresponding
         data in the dataframe.
         :param environment (Environments): The environment the data corresponds to (Production,
-        Training, or Validation).
+        Training, Validation).
         :param model_id (str): A unique name to identify your model in the Arize platform.
         :param model_type (ModelTypes): Declare your model type. Can check the supported model types
         running `ModelTypes.list_types()`.
         :param metrics_validation (List[Metrics], optional): A list of desired metric types;
         defaults to None. When populated, and if validate=True, the presence of schema columns are
         validated against the desired metrics.
         :param model_version (str, optional): Used to group a subset of predictions and actuals for
@@ -260,15 +260,17 @@
                 schema = schema.replace(embedding_feature_column_names=prompt_response_map)
             else:
                 schema.embedding_feature_column_names.update(prompt_response_map)
         if validate:
             if verbose:
                 logger.info("Performing values validation.")
             errors = Validator.validate_values(
-                dataframe=dataframe, schema=schema, model_type=model_type
+                dataframe=dataframe,
+                schema=schema,
+                model_type=model_type,
             )
             if errors:
                 for e in errors:
                     logger.error(e)
                 raise err.ValidationFailure(errors)
 
         if verbose:
@@ -294,15 +296,15 @@
         elif model_type in CATEGORICAL_MODEL_TYPES:
             s.constants.model_type = pb2.Schema.ModelType.SCORE_CATEGORICAL
         elif model_type == ModelTypes.RANKING:
             s.constants.model_type = pb2.Schema.ModelType.RANKING
         elif model_type == ModelTypes.OBJECT_DETECTION:
             s.constants.model_type = pb2.Schema.ModelType.OBJECT_DETECTION
         elif model_type == ModelTypes.GENERATIVE_LLM:
-            s.constants.model_type = pb2.Schema.ModelType.SCORE_CATEGORICAL
+            s.constants.model_type = pb2.Schema.ModelType.GENERATIVE_LLM
 
         if batch_id is not None:
             s.constants.batch_id = batch_id
 
         if schema.prediction_id_column_name is not None:
             s.arrow_schema.prediction_id_column_name = schema.prediction_id_column_name
```

### Comparing `arize-7.0.0rc6/arize/pandas/surrogate_explainer/mimic.py` & `arize-7.0.1rc0/arize/pandas/surrogate_explainer/mimic.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/pandas/validation/errors.py` & `arize-7.0.1rc0/arize/pandas/validation/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,34 +225,23 @@
     def error_message(self) -> str:
         return (
             "The schema must specify prompt_column_names and response_column_names for "
             "ModelTypes.GENERATIVE_LLM models"
         )
 
 
-class MissingPredActShapNumeric(ValidationError):
+class MissingPredActShapNumericAndCategorical(ValidationError):
     def __repr__(self) -> str:
-        return "Missing_Pred_or_Act_or_SHAP_Numeric"
+        return "Missing_Pred_or_Act_or_SHAP_Numeric_and_Categorical"
 
     def error_message(self) -> str:
         return (
-            "For a numeric model, the schema must specify at least one of the following: "
-            "prediction label, prediction score, actual label, actual score, or SHAP value column "
-            "names"
-        )
-
-
-class MissingPredLabelScoreCategorical(ValidationError):
-    def __repr__(self) -> str:
-        return "Missing_Pred_Label_Score_Categorical"
-
-    def error_message(self) -> str:
-        return (
-            "When sending a prediction confidence score and an actual label, the schema must also include "
-            "a prediction label."
+            "For a numeric model or a categorical model, the schema must specify at least one "
+            "of the following: prediction label, prediction score, actual label, actual score, "
+            "or SHAP value column names"
         )
 
 
 class MissingPreprodPredAct(ValidationError):
     def __repr__(self) -> str:
         return "Missing_Preproduction_Pred_and_Act"
 
@@ -265,22 +254,22 @@
     def __repr__(self) -> str:
         return "Missing_Preproduction_Act"
 
     def error_message(self) -> str:
         return "For logging pre-production data, the schema must specify actual label column."
 
 
-class MissingPreprodPredActNumeric(ValidationError):
+class MissingPreprodPredActNumericAndCategorical(ValidationError):
     def __repr__(self) -> str:
-        return "Missing_Preproduction_Pred_and_Act_Numeric"
+        return "Missing_Preproduction_Pred_and_Act_Numeric_and_Categorical"
 
     def error_message(self) -> str:
         return (
-            "For logging pre-production data for a numeric model, "
-            "the schema must specify both prediction and actual label or confidence score columns."
+            "For logging pre-production data for a numeric or a categorical model, "
+            "the schema must specify both prediction and actual label or score columns."
         )
 
 
 class MissingRequiredColumnsForRankingModel(ValidationError):
     def __repr__(self) -> str:
         return "Missing_Required_Columns_For_Ranking_Model"
```

### Comparing `arize-7.0.0rc6/arize/pandas/validation/validator.py` & `arize-7.0.1rc0/arize/pandas/validation/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,17 +68,16 @@
                 Validator._check_existence_pred_act_shap_score_or_label(schema),
                 Validator._check_existence_preprod_pred_act_score_or_label(schema, environment),
                 Validator._check_missing_object_detection_columns(schema, model_type),
             )
             return list(chain(general_checks, num_checks))
         elif model_type in CATEGORICAL_MODEL_TYPES:
             sc_checks = chain(
-                Validator._check_existence_pred_act_shap(schema),
-                Validator._check_existence_preprod_pred_act(schema, environment),
-                Validator._check_existence_pred_label(schema),
+                Validator._check_existence_pred_act_shap_score_or_label(schema),
+                Validator._check_existence_preprod_pred_act_score_or_label(schema, environment),
                 Validator._check_missing_object_detection_columns(schema, model_type),
             )
             return list(chain(general_checks, sc_checks))
         elif model_type == ModelTypes.GENERATIVE_LLM:
             gllm_checks = chain(
                 Validator._check_existence_prompt_response_generative_llm(schema),
                 Validator._check_existence_preprod_act(schema, environment),
@@ -142,27 +141,28 @@
             )
             return list(chain(general_checks, od_checks))
 
         return list(general_checks)
 
     @staticmethod
     def validate_values(
-        dataframe: pd.DataFrame, schema: Schema, model_type: ModelTypes
+        dataframe: pd.DataFrame,
+        schema: Schema,
+        model_type: ModelTypes,
     ) -> List[err.ValidationError]:
         # ASSUMPTION: at this point the param and type checks should have passed.
         # This function may crash if that is not true, e.g. if columns are missing
         # or are of the wrong types.
 
         general_checks = chain(
             Validator._check_value_timestamp(dataframe, schema),
-            Validator._check_value_missing(dataframe, schema),
+            Validator._check_value_missing(dataframe, schema, model_type),
             Validator._check_value_prediction_id(dataframe, schema),
             Validator._check_embedding_features_dimensionality(dataframe, schema),
         )
-
         if model_type == ModelTypes.RANKING:
             r_checks = chain(
                 Validator._check_value_rank(dataframe, schema),
                 Validator._check_value_prediction_group_id(dataframe, schema),
                 Validator._check_value_ranking_category(dataframe, schema),
             )
             return list(chain(general_checks, r_checks))
@@ -463,76 +463,52 @@
         environment: Environments,
     ) -> List[err.InvalidEnvironment]:
         if environment in (env for env in Environments):
             return []
         return [err.InvalidEnvironment()]
 
     @staticmethod
-    def _check_existence_pred_act_shap(
-        schema: Schema,
-    ) -> List[err.MissingPredActShap]:
-        if (
-            schema.prediction_label_column_name is not None
-            or schema.actual_label_column_name is not None
-            or schema.shap_values_column_names is not None
-        ):
-            return []
-        return [err.MissingPredActShap()]
-
-    @staticmethod
     def _check_existence_prompt_response_generative_llm(
         schema: Schema,
     ) -> List[err.MissingPromptResponseGenerativeLLM]:
         if schema.prompt_column_names is None or schema.response_column_names is None:
             return [err.MissingPromptResponseGenerativeLLM()]
         return []
 
     @staticmethod
     def _check_existence_pred_act_shap_score_or_label(
         schema: Schema,
-    ) -> List[err.MissingPredActShapNumeric]:
+    ) -> List[err.MissingPredActShapNumericAndCategorical]:
         if (
             (
                 schema.prediction_label_column_name is not None
                 or schema.prediction_score_column_name is not None
             )
             or (
                 schema.actual_label_column_name is not None
                 or schema.actual_score_column_name is not None
             )
             or schema.shap_values_column_names is not None
         ):
             return []
-        return [err.MissingPredActShapNumeric()]
-
-    @staticmethod
-    def _check_existence_pred_label(
-        schema: Schema,
-    ) -> List[err.MissingPredLabelScoreCategorical]:
-        if (
-            schema.prediction_score_column_name is not None
-            and schema.actual_label_column_name is not None
-            and schema.prediction_label_column_name is None
-        ):
-            return [err.MissingPredLabelScoreCategorical()]
-        return []
+        return [err.MissingPredActShapNumericAndCategorical()]
 
     @staticmethod
     def _check_existence_preprod_pred_act_score_or_label(
         schema: Schema,
         environment: Environments,
-    ) -> List[err.MissingPreprodPredActNumeric]:
+    ) -> List[err.MissingPreprodPredActNumericAndCategorical]:
         if environment in (Environments.VALIDATION, Environments.TRAINING) and (
             (
                 schema.prediction_label_column_name is None
                 and schema.prediction_score_column_name is None
             )
             or (schema.actual_label_column_name is None and schema.actual_score_column_name is None)
         ):
-            return [err.MissingPreprodPredActNumeric()]
+            return [err.MissingPreprodPredActNumericAndCategorical()]
         return []
 
     @staticmethod
     def _check_existence_pred_act_od_column_names(
         schema: Schema, environment: Environments
     ) -> List[err.MissingObjectDetectionPredAct]:
         # Checks that the required prediction/actual columns are given in the schema depending on
@@ -586,25 +562,14 @@
             if col is not None:
                 wrong_cols.append(col)
         if wrong_cols:
             return [err.InvalidPredActColumnNamesForObjectDetectionModelType(wrong_cols)]
         return []
 
     @staticmethod
-    def _check_existence_preprod_pred_act(
-        schema: Schema,
-        environment: Environments,
-    ) -> List[err.MissingPreprodPredAct]:
-        if environment in (Environments.VALIDATION, Environments.TRAINING) and (
-            schema.prediction_label_column_name is None or schema.actual_label_column_name is None
-        ):
-            return [err.MissingPreprodPredAct()]
-        return []
-
-    @staticmethod
     def _check_existence_preprod_act(
         schema: Schema,
         environment: Environments,
     ) -> List[err.MissingPreprodAct]:
         if environment in (Environments.VALIDATION, Environments.TRAINING) and (
             schema.actual_label_column_name is None
         ):
@@ -833,32 +798,41 @@
                 pa.int64(),
                 pa.bool_(),
                 pa.float64(),
                 pa.int32(),
                 pa.float32(),
                 pa.int16(),
                 pa.int8(),
+                pa.null(),
             )
             for name, col in columns:
-                if col in column_types and column_types[col] not in allowed_datatypes:
+                if (
+                    col is not None
+                    and col in column_types
+                    and column_types[col] not in allowed_datatypes
+                ):
                     errors.append(
                         err.InvalidType(name, expected_types=["float", "int", "bool", "str"])
                     )
         elif model_type in NUMERIC_MODEL_TYPES:
             # should mirror server side
             allowed_datatypes = (
                 pa.float64(),
                 pa.int64(),
                 pa.float32(),
                 pa.int32(),
                 pa.int16(),
                 pa.int8(),
             )
             for name, col in columns:
-                if col in column_types and column_types[col] not in allowed_datatypes:
+                if (
+                    col is not None
+                    and col in column_types
+                    and column_types[col] not in allowed_datatypes
+                ):
                     errors.append(err.InvalidType(name, expected_types=["float", "int"]))
         return errors
 
     @staticmethod
     def _check_type_pred_act_scores(
         model_type: ModelTypes, schema: Schema, column_types: Dict[str, Any]
     ) -> List[err.InvalidType]:
@@ -877,14 +851,15 @@
             allowed_datatypes = (
                 pa.float64(),
                 pa.int64(),
                 pa.float32(),
                 pa.int32(),
                 pa.int16(),
                 pa.int8(),
+                pa.null(),
             )
             for name, col in columns:
                 if (
                     col is not None
                     and col in column_types
                     and column_types[col] not in allowed_datatypes
                 ):
@@ -1238,27 +1213,31 @@
                     err.InvalidValueTimestamp("Prediction timestamp", acceptable_range="one year")
                 ]
 
         return []
 
     @staticmethod
     def _check_value_missing(
-        dataframe: pd.DataFrame, schema: Schema
+        dataframe: pd.DataFrame, schema: Schema, model_type: ModelTypes
     ) -> List[err.InvalidValueMissingValue]:
         errors = []
-        columns = (
-            ("Prediction IDs", schema.prediction_id_column_name),
-            ("Prediction labels", schema.prediction_label_column_name),
-            ("Actual labels", schema.actual_label_column_name),
-            ("Prediction Group IDs", schema.prediction_group_id_column_name),
-            ("Ranks", schema.rank_column_name),
-            ("Attributions", schema.attributions_column_name),
-            ("Relevance Score", schema.relevance_score_column_name),
-            ("Relevance Labels", schema.relevance_labels_column_name),
-        )
+        columns = ()
+        if model_type == ModelTypes.SCORE_CATEGORICAL:
+            columns = (("Prediction IDs", schema.prediction_id_column_name),)
+        else:
+            columns = (
+                ("Prediction IDs", schema.prediction_id_column_name),
+                ("Prediction labels", schema.prediction_label_column_name),
+                ("Actual labels", schema.actual_label_column_name),
+                ("Prediction Group IDs", schema.prediction_group_id_column_name),
+                ("Ranks", schema.rank_column_name),
+                ("Attributions", schema.attributions_column_name),
+                ("Relevance Score", schema.relevance_score_column_name),
+                ("Relevance Labels", schema.relevance_labels_column_name),
+            )
         for name, col in columns:
             if col is not None and col in dataframe.columns:
                 if dataframe[col].isnull().any():
                     errors.append(err.InvalidValueMissingValue(name, wrong_values="missing"))
                 elif (
                     dataframe[col].dtype in (np.dtype("float64"), np.dtype("float32"))
                     and np.isinf(dataframe[col]).any()
```

### Comparing `arize-7.0.0rc6/arize/public_pb2.py` & `arize-7.0.1rc0/arize/public_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: public.proto
-
+"""Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
@@ -53,16 +53,16 @@
       name='PRODUCTION', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3999,
-  serialized_end=4071,
+  serialized_start=4088,
+  serialized_end=4160,
 )
 _sym_db.RegisterEnumDescriptor(_FILEHEADER_ENVIRONMENT)
 
 _SCHEMA_ENVIRONMENT = _descriptor.EnumDescriptor(
   name='Environment',
   full_name='public.Schema.Environment',
   filename=None,
@@ -88,16 +88,16 @@
       name='PRODUCTION', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=8902,
-  serialized_end=8986,
+  serialized_start=8991,
+  serialized_end=9075,
 )
 _sym_db.RegisterEnumDescriptor(_SCHEMA_ENVIRONMENT)
 
 _SCHEMA_MODELTYPE = _descriptor.EnumDescriptor(
   name='ModelType',
   full_name='public.Schema.ModelType',
   filename=None,
@@ -566,16 +566,47 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1403,
-  serialized_end=1431,
+  serialized_start=1463,
+  serialized_end=1491,
+)
+
+_SCORECATEGORICAL_SCOREVALUE = _descriptor.Descriptor(
+  name='ScoreValue',
+  full_name='public.ScoreCategorical.ScoreValue',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='value', full_name='public.ScoreCategorical.ScoreValue.value', index=0,
+      number=1, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1493,
+  serialized_end=1520,
 )
 
 _SCORECATEGORICAL_SCORECATEGORY = _descriptor.Descriptor(
   name='ScoreCategory',
   full_name='public.ScoreCategorical.ScoreCategory',
   filename=None,
   file=DESCRIPTOR,
@@ -611,16 +642,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1433,
-  serialized_end=1511,
+  serialized_start=1522,
+  serialized_end=1600,
 )
 
 _SCORECATEGORICAL = _descriptor.Descriptor(
   name='ScoreCategorical',
   full_name='public.ScoreCategorical',
   filename=None,
   file=DESCRIPTOR,
@@ -651,33 +682,40 @@
     _descriptor.FieldDescriptor(
       name='score_category', full_name='public.ScoreCategorical.score_category', index=3,
       number=4, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='score_value', full_name='public.ScoreCategorical.score_value', index=4,
+      number=5, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_SCORECATEGORICAL_CATEGORY, _SCORECATEGORICAL_SCORECATEGORY, ],
+  nested_types=[_SCORECATEGORICAL_CATEGORY, _SCORECATEGORICAL_SCOREVALUE, _SCORECATEGORICAL_SCORECATEGORY, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='type', full_name='public.ScoreCategorical.type',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
   serialized_start=1218,
-  serialized_end=1519,
+  serialized_end=1608,
 )
 
 
 _OBJECTDETECTION_BOUNDINGBOX = _descriptor.Descriptor(
   name='BoundingBox',
   full_name='public.ObjectDetection.BoundingBox',
   filename=None,
@@ -714,16 +752,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1602,
-  serialized_end=1699,
+  serialized_start=1691,
+  serialized_end=1788,
 )
 
 _OBJECTDETECTION = _descriptor.Descriptor(
   name='ObjectDetection',
   full_name='public.ObjectDetection',
   filename=None,
   file=DESCRIPTOR,
@@ -745,16 +783,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1522,
-  serialized_end=1699,
+  serialized_start=1611,
+  serialized_end=1788,
 )
 
 
 _RANKINGPREDICTION = _descriptor.Descriptor(
   name='RankingPrediction',
   full_name='public.RankingPrediction',
   filename=None,
@@ -798,16 +836,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1702,
-  serialized_end=1835,
+  serialized_start=1791,
+  serialized_end=1924,
 )
 
 
 _RANKINGACTUAL = _descriptor.Descriptor(
   name='RankingActual',
   full_name='public.RankingActual',
   filename=None,
@@ -837,16 +875,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1837,
-  serialized_end=1945,
+  serialized_start=1926,
+  serialized_end=2034,
 )
 
 
 _LABEL = _descriptor.Descriptor(
   name='Label',
   full_name='public.Label',
   filename=None,
@@ -895,16 +933,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='data', full_name='public.Label.data',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=1948,
-  serialized_end=2078,
+  serialized_start=2037,
+  serialized_end=2167,
 )
 
 
 _PREDICTIONLABEL = _descriptor.Descriptor(
   name='PredictionLabel',
   full_name='public.PredictionLabel',
   filename=None,
@@ -967,16 +1005,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='data', full_name='public.PredictionLabel.data',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=2081,
-  serialized_end=2320,
+  serialized_start=2170,
+  serialized_end=2409,
 )
 
 
 _ACTUALLABEL = _descriptor.Descriptor(
   name='ActualLabel',
   full_name='public.ActualLabel',
   filename=None,
@@ -1039,16 +1077,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='data', full_name='public.ActualLabel.data',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=2323,
-  serialized_end=2554,
+  serialized_start=2412,
+  serialized_end=2643,
 )
 
 
 _PREDICTION_FEATURESENTRY = _descriptor.Descriptor(
   name='FeaturesEntry',
   full_name='public.Prediction.FeaturesEntry',
   filename=None,
@@ -1078,16 +1116,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2822,
-  serialized_end=2884,
+  serialized_start=2911,
+  serialized_end=2973,
 )
 
 _PREDICTION_TAGSENTRY = _descriptor.Descriptor(
   name='TagsEntry',
   full_name='public.Prediction.TagsEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -1116,16 +1154,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2886,
-  serialized_end=2944,
+  serialized_start=2975,
+  serialized_end=3033,
 )
 
 _PREDICTION = _descriptor.Descriptor(
   name='Prediction',
   full_name='public.Prediction',
   filename=None,
   file=DESCRIPTOR,
@@ -1182,16 +1220,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2557,
-  serialized_end=2944,
+  serialized_start=2646,
+  serialized_end=3033,
 )
 
 
 _VALUE = _descriptor.Descriptor(
   name='Value',
   full_name='public.Value',
   filename=None,
@@ -1247,16 +1285,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='data', full_name='public.Value.data',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=2947,
-  serialized_end=3096,
+  serialized_start=3036,
+  serialized_end=3185,
 )
 
 
 _MULTIVALUE = _descriptor.Descriptor(
   name='MultiValue',
   full_name='public.MultiValue',
   filename=None,
@@ -1279,16 +1317,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3098,
-  serialized_end=3126,
+  serialized_start=3187,
+  serialized_end=3215,
 )
 
 
 _EMBEDDING_RAWDATA = _descriptor.Descriptor(
   name='RawData',
   full_name='public.Embedding.RawData',
   filename=None,
@@ -1316,16 +1354,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='type', full_name='public.Embedding.RawData.type',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=3255,
-  serialized_end=3330,
+  serialized_start=3344,
+  serialized_end=3419,
 )
 
 _EMBEDDING_TOKENARRAY = _descriptor.Descriptor(
   name='TokenArray',
   full_name='public.Embedding.TokenArray',
   filename=None,
   file=DESCRIPTOR,
@@ -1347,16 +1385,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3332,
-  serialized_end=3360,
+  serialized_start=3421,
+  serialized_end=3449,
 )
 
 _EMBEDDING = _descriptor.Descriptor(
   name='Embedding',
   full_name='public.Embedding',
   filename=None,
   file=DESCRIPTOR,
@@ -1392,16 +1430,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3129,
-  serialized_end=3366,
+  serialized_start=3218,
+  serialized_end=3455,
 )
 
 
 _ACTUAL_TAGSENTRY = _descriptor.Descriptor(
   name='TagsEntry',
   full_name='public.Actual.TagsEntry',
   filename=None,
@@ -1431,16 +1469,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2886,
-  serialized_end=2944,
+  serialized_start=2975,
+  serialized_end=3033,
 )
 
 _ACTUAL = _descriptor.Descriptor(
   name='Actual',
   full_name='public.Actual',
   filename=None,
   file=DESCRIPTOR,
@@ -1483,16 +1521,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3369,
-  serialized_end=3601,
+  serialized_start=3458,
+  serialized_end=3690,
 )
 
 
 _FEATUREIMPORTANCES_FEATUREIMPORTANCESENTRY = _descriptor.Descriptor(
   name='FeatureImportancesEntry',
   full_name='public.FeatureImportances.FeatureImportancesEntry',
   filename=None,
@@ -1522,16 +1560,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3777,
-  serialized_end=3834,
+  serialized_start=3866,
+  serialized_end=3923,
 )
 
 _FEATUREIMPORTANCES = _descriptor.Descriptor(
   name='FeatureImportances',
   full_name='public.FeatureImportances',
   filename=None,
   file=DESCRIPTOR,
@@ -1567,16 +1605,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3604,
-  serialized_end=3834,
+  serialized_start=3693,
+  serialized_end=3923,
 )
 
 
 _PREDICTIONANDACTUAL = _descriptor.Descriptor(
   name='PredictionAndActual',
   full_name='public.PredictionAndActual',
   filename=None,
@@ -1606,16 +1644,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3836,
-  serialized_end=3929,
+  serialized_start=3925,
+  serialized_end=4018,
 )
 
 
 _FILEHEADER = _descriptor.Descriptor(
   name='FileHeader',
   full_name='public.FileHeader',
   filename=None,
@@ -1639,16 +1677,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3932,
-  serialized_end=4071,
+  serialized_start=4021,
+  serialized_end=4160,
 )
 
 
 _SCHEMA_CONSTANTS = _descriptor.Descriptor(
   name='Constants',
   full_name='public.Schema.Constants',
   filename=None,
@@ -1699,16 +1737,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4520,
-  serialized_end=4685,
+  serialized_start=4609,
+  serialized_end=4774,
 )
 
 _SCHEMA_ARIZECONCLUSIONS = _descriptor.Descriptor(
   name='ArizeConclusions',
   full_name='public.Schema.ArizeConclusions',
   filename=None,
   file=DESCRIPTOR,
@@ -1723,16 +1761,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4687,
-  serialized_end=4705,
+  serialized_start=4776,
+  serialized_end=4794,
 )
 
 _SCHEMA_ARIZEEXPLANATIONS = _descriptor.Descriptor(
   name='ArizeExplanations',
   full_name='public.Schema.ArizeExplanations',
   filename=None,
   file=DESCRIPTOR,
@@ -1747,16 +1785,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4707,
-  serialized_end=4726,
+  serialized_start=4796,
+  serialized_end=4815,
 )
 
 _SCHEMA_ARIZECONCLUSIONPOINTERS = _descriptor.Descriptor(
   name='ArizeConclusionPointers',
   full_name='public.Schema.ArizeConclusionPointers',
   filename=None,
   file=DESCRIPTOR,
@@ -1771,16 +1809,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4728,
-  serialized_end=4753,
+  serialized_start=4817,
+  serialized_end=4842,
 )
 
 _SCHEMA_ARIZEEXPLANATIONPOINTERS = _descriptor.Descriptor(
   name='ArizeExplanationPointers',
   full_name='public.Schema.ArizeExplanationPointers',
   filename=None,
   file=DESCRIPTOR,
@@ -1795,16 +1833,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4755,
-  serialized_end=4781,
+  serialized_start=4844,
+  serialized_end=4870,
 )
 
 _SCHEMA_ARROWSCHEMA_SHAPVALUESCOLUMNNAMESENTRY = _descriptor.Descriptor(
   name='ShapValuesColumnNamesEntry',
   full_name='public.Schema.ArrowSchema.ShapValuesColumnNamesEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -1833,16 +1871,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5767,
-  serialized_end=5827,
+  serialized_start=5856,
+  serialized_end=5916,
 )
 
 _SCHEMA_ARROWSCHEMA_EMBEDDINGFEATURECOLUMNNAMESMAPENTRY = _descriptor.Descriptor(
   name='EmbeddingFeatureColumnNamesMapEntry',
   full_name='public.Schema.ArrowSchema.EmbeddingFeatureColumnNamesMapEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -1871,16 +1909,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5829,
-  serialized_end=5935,
+  serialized_start=5918,
+  serialized_end=6024,
 )
 
 _SCHEMA_ARROWSCHEMA = _descriptor.Descriptor(
   name='ArrowSchema',
   full_name='public.Schema.ArrowSchema',
   filename=None,
   file=DESCRIPTOR,
@@ -2028,16 +2066,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4784,
-  serialized_end=5935,
+  serialized_start=4873,
+  serialized_end=6024,
 )
 
 _SCHEMA_OBJECTDETECTIONLABELCOLUMNNAMES = _descriptor.Descriptor(
   name='ObjectDetectionLabelColumnNames',
   full_name='public.Schema.ObjectDetectionLabelColumnNames',
   filename=None,
   file=DESCRIPTOR,
@@ -2073,16 +2111,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5938,
-  serialized_end=6085,
+  serialized_start=6027,
+  serialized_end=6174,
 )
 
 _SCHEMA_EMBEDDINGCOLUMNNAMES = _descriptor.Descriptor(
   name='EmbeddingColumnNames',
   full_name='public.Schema.EmbeddingColumnNames',
   filename=None,
   file=DESCRIPTOR,
@@ -2118,16 +2156,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6087,
-  serialized_end=6197,
+  serialized_start=6176,
+  serialized_end=6286,
 )
 
 _SCHEMA_GENERICSCHEMA_FIELDDESCRIPTOR = _descriptor.Descriptor(
   name='FieldDescriptor',
   full_name='public.Schema.GenericSchema.FieldDescriptor',
   filename=None,
   file=DESCRIPTOR,
@@ -2149,16 +2187,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7827,
-  serialized_end=7864,
+  serialized_start=7916,
+  serialized_end=7953,
 )
 
 _SCHEMA_GENERICSCHEMA_GROUPFIELDDESCRIPTOR = _descriptor.Descriptor(
   name='GroupFieldDescriptor',
   full_name='public.Schema.GenericSchema.GroupFieldDescriptor',
   filename=None,
   file=DESCRIPTOR,
@@ -2187,16 +2225,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7866,
-  serialized_end=7931,
+  serialized_start=7955,
+  serialized_end=8020,
 )
 
 _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP_PROPERTIESMAPENTRY = _descriptor.Descriptor(
   name='PropertiesMapEntry',
   full_name='public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap.PropertiesMapEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -2225,16 +2263,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8197,
-  serialized_end=8249,
+  serialized_start=8286,
+  serialized_end=8338,
 )
 
 _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP = _descriptor.Descriptor(
   name='EmbeddingPropertyMap',
   full_name='public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap',
   filename=None,
   file=DESCRIPTOR,
@@ -2256,16 +2294,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8054,
-  serialized_end=8249,
+  serialized_start=8143,
+  serialized_end=8338,
 )
 
 _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_PROPERTIESENTRY = _descriptor.Descriptor(
   name='PropertiesEntry',
   full_name='public.Schema.GenericSchema.EmbeddingFieldDescriptor.PropertiesEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -2294,16 +2332,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8251,
-  serialized_end=8376,
+  serialized_start=8340,
+  serialized_end=8465,
 )
 
 _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR = _descriptor.Descriptor(
   name='EmbeddingFieldDescriptor',
   full_name='public.Schema.GenericSchema.EmbeddingFieldDescriptor',
   filename=None,
   file=DESCRIPTOR,
@@ -2325,16 +2363,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7934,
-  serialized_end=8376,
+  serialized_start=8023,
+  serialized_end=8465,
 )
 
 _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP_PROPERTIESMAPENTRY = _descriptor.Descriptor(
   name='PropertiesMapEntry',
   full_name='public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap.PropertiesMapEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -2363,16 +2401,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8197,
-  serialized_end=8249,
+  serialized_start=8286,
+  serialized_end=8338,
 )
 
 _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP = _descriptor.Descriptor(
   name='ObjectDetectionLabelPropertyMap',
   full_name='public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap',
   filename=None,
   file=DESCRIPTOR,
@@ -2394,16 +2432,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8521,
-  serialized_end=8750,
+  serialized_start=8610,
+  serialized_end=8839,
 )
 
 _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_PROPERTIESENTRY = _descriptor.Descriptor(
   name='PropertiesEntry',
   full_name='public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.PropertiesEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -2432,16 +2470,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8753,
-  serialized_end=8900,
+  serialized_start=8842,
+  serialized_end=8989,
 )
 
 _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR = _descriptor.Descriptor(
   name='ObjectDetectionLabelFieldDescriptor',
   full_name='public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor',
   filename=None,
   file=DESCRIPTOR,
@@ -2463,16 +2501,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8379,
-  serialized_end=8900,
+  serialized_start=8468,
+  serialized_end=8989,
 )
 
 _SCHEMA_GENERICSCHEMA = _descriptor.Descriptor(
   name='GenericSchema',
   full_name='public.Schema.GenericSchema',
   filename=None,
   file=DESCRIPTOR,
@@ -2641,16 +2679,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6200,
-  serialized_end=8900,
+  serialized_start=6289,
+  serialized_end=8989,
 )
 
 _SCHEMA = _descriptor.Descriptor(
   name='Schema',
   full_name='public.Schema',
   filename=None,
   file=DESCRIPTOR,
@@ -2838,23 +2876,28 @@
 _PREPRODUCTIONRECORD.oneofs_by_name['record_type'].fields.append(
   _PREPRODUCTIONRECORD.fields_by_name['training_record'])
 _PREPRODUCTIONRECORD.fields_by_name['training_record'].containing_oneof = _PREPRODUCTIONRECORD.oneofs_by_name['record_type']
 _PREPRODUCTIONRECORD.oneofs_by_name['record_type'].fields.append(
   _PREPRODUCTIONRECORD.fields_by_name['validation_record'])
 _PREPRODUCTIONRECORD.fields_by_name['validation_record'].containing_oneof = _PREPRODUCTIONRECORD.oneofs_by_name['record_type']
 _SCORECATEGORICAL_CATEGORY.containing_type = _SCORECATEGORICAL
+_SCORECATEGORICAL_SCOREVALUE.containing_type = _SCORECATEGORICAL
 _SCORECATEGORICAL_SCORECATEGORY.containing_type = _SCORECATEGORICAL
 _SCORECATEGORICAL.fields_by_name['category'].message_type = _SCORECATEGORICAL_CATEGORY
 _SCORECATEGORICAL.fields_by_name['score_category'].message_type = _SCORECATEGORICAL_SCORECATEGORY
+_SCORECATEGORICAL.fields_by_name['score_value'].message_type = _SCORECATEGORICAL_SCOREVALUE
 _SCORECATEGORICAL.oneofs_by_name['type'].fields.append(
   _SCORECATEGORICAL.fields_by_name['category'])
 _SCORECATEGORICAL.fields_by_name['category'].containing_oneof = _SCORECATEGORICAL.oneofs_by_name['type']
 _SCORECATEGORICAL.oneofs_by_name['type'].fields.append(
   _SCORECATEGORICAL.fields_by_name['score_category'])
 _SCORECATEGORICAL.fields_by_name['score_category'].containing_oneof = _SCORECATEGORICAL.oneofs_by_name['type']
+_SCORECATEGORICAL.oneofs_by_name['type'].fields.append(
+  _SCORECATEGORICAL.fields_by_name['score_value'])
+_SCORECATEGORICAL.fields_by_name['score_value'].containing_oneof = _SCORECATEGORICAL.oneofs_by_name['type']
 _OBJECTDETECTION_BOUNDINGBOX.fields_by_name['score'].message_type = google_dot_protobuf_dot_wrappers__pb2._DOUBLEVALUE
 _OBJECTDETECTION_BOUNDINGBOX.containing_type = _OBJECTDETECTION
 _OBJECTDETECTION.fields_by_name['bounding_boxes'].message_type = _OBJECTDETECTION_BOUNDINGBOX
 _RANKINGPREDICTION.fields_by_name['prediction_score'].message_type = google_dot_protobuf_dot_wrappers__pb2._DOUBLEVALUE
 _RANKINGACTUAL.fields_by_name['category'].message_type = _MULTIVALUE
 _RANKINGACTUAL.fields_by_name['relevance_score'].message_type = google_dot_protobuf_dot_wrappers__pb2._DOUBLEVALUE
 _LABEL.fields_by_name['score_categorical'].message_type = _SCORECATEGORICAL
@@ -3140,26 +3183,34 @@
   'Category' : _reflection.GeneratedProtocolMessageType('Category', (_message.Message,), {
     'DESCRIPTOR' : _SCORECATEGORICAL_CATEGORY,
     '__module__' : 'public_pb2'
     # @@protoc_insertion_point(class_scope:public.ScoreCategorical.Category)
     })
   ,
 
+  'ScoreValue' : _reflection.GeneratedProtocolMessageType('ScoreValue', (_message.Message,), {
+    'DESCRIPTOR' : _SCORECATEGORICAL_SCOREVALUE,
+    '__module__' : 'public_pb2'
+    # @@protoc_insertion_point(class_scope:public.ScoreCategorical.ScoreValue)
+    })
+  ,
+
   'ScoreCategory' : _reflection.GeneratedProtocolMessageType('ScoreCategory', (_message.Message,), {
     'DESCRIPTOR' : _SCORECATEGORICAL_SCORECATEGORY,
     '__module__' : 'public_pb2'
     # @@protoc_insertion_point(class_scope:public.ScoreCategorical.ScoreCategory)
     })
   ,
   'DESCRIPTOR' : _SCORECATEGORICAL,
   '__module__' : 'public_pb2'
   # @@protoc_insertion_point(class_scope:public.ScoreCategorical)
   })
 _sym_db.RegisterMessage(ScoreCategorical)
 _sym_db.RegisterMessage(ScoreCategorical.Category)
+_sym_db.RegisterMessage(ScoreCategorical.ScoreValue)
 _sym_db.RegisterMessage(ScoreCategorical.ScoreCategory)
 
 ObjectDetection = _reflection.GeneratedProtocolMessageType('ObjectDetection', (_message.Message,), {
 
   'BoundingBox' : _reflection.GeneratedProtocolMessageType('BoundingBox', (_message.Message,), {
     'DESCRIPTOR' : _OBJECTDETECTION_BOUNDINGBOX,
     '__module__' : 'public_pb2'
```

### Comparing `arize-7.0.0rc6/arize/utils/logging.py` & `arize-7.0.1rc0/arize/utils/logging.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/utils/model_mapping.json` & `arize-7.0.1rc0/arize/utils/model_mapping.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950810185185185%*

 * *Differences: {"'required_columns_map'": "{0: {'mappings': {2: {'metrics': {delete: [3, 0]}}, insert: [(3, "*

 * *                           "OrderedDict([('metrics', [['auc_log_loss']]), ('required_columns', "*

 * *                           "OrderedDict([('arrow', OrderedDict([('required', "*

 * *                           "[['prediction_score_column_name']]), ('latent', "*

 * *                           "[['actual_label_column_name']])])), ('generic', "*

 * *                           "OrderedDict([('required', [['prediction_score']]), ('late […]*

```diff
@@ -80,52 +80,114 @@
                             ]
                         }
                     }
                 },
                 {
                     "metrics": [
                         [
-                            "auc_log_loss"
-                        ],
-                        [
                             "auc_log_loss",
                             "classification"
                         ],
                         [
                             "regression",
                             "classification"
-                        ],
+                        ]
+                    ],
+                    "required_columns": {
+                        "arrow": {
+                            "latent": [
+                                [
+                                    "actual_label_column_name"
+                                ]
+                            ],
+                            "required": [
+                                [
+                                    "prediction_label_column_name",
+                                    "prediction_score_column_name"
+                                ]
+                            ]
+                        },
+                        "generic": {
+                            "latent": [
+                                [
+                                    "actual_label"
+                                ]
+                            ],
+                            "required": [
+                                [
+                                    "prediction_label",
+                                    "prediction_score"
+                                ]
+                            ]
+                        }
+                    }
+                },
+                {
+                    "metrics": [
+                        [
+                            "auc_log_loss"
+                        ]
+                    ],
+                    "required_columns": {
+                        "arrow": {
+                            "latent": [
+                                [
+                                    "actual_label_column_name"
+                                ]
+                            ],
+                            "required": [
+                                [
+                                    "prediction_score_column_name"
+                                ]
+                            ]
+                        },
+                        "generic": {
+                            "latent": [
+                                [
+                                    "actual_label"
+                                ]
+                            ],
+                            "required": [
+                                [
+                                    "prediction_score"
+                                ]
+                            ]
+                        }
+                    }
+                },
+                {
+                    "metrics": [
                         [
                             "regression",
                             "auc_log_loss"
                         ]
                     ],
                     "required_columns": {
                         "arrow": {
                             "latent": [
                                 [
+                                    "actual_score_column_name",
                                     "actual_label_column_name"
                                 ]
                             ],
                             "required": [
                                 [
-                                    "prediction_label_column_name",
                                     "prediction_score_column_name"
                                 ]
                             ]
                         },
                         "generic": {
                             "latent": [
                                 [
+                                    "actual_score",
                                     "actual_label"
                                 ]
                             ],
                             "required": [
                                 [
-                                    "prediction_label",
                                     "prediction_score"
                                 ]
                             ]
                         }
                     }
                 },
                 {
```

### Comparing `arize-7.0.0rc6/arize/utils/types.py` & `arize-7.0.1rc0/arize/utils/types.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize/utils/utils.py` & `arize-7.0.1rc0/arize/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/arize.egg-info/PKG-INFO` & `arize-7.0.1rc0/arize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.0rc6
+Version: 7.0.1rc0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.0rc6/arize.egg-info/SOURCES.txt` & `arize-7.0.1rc0/arize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/setup.cfg` & `arize-7.0.1rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/tests/test_api.py` & `arize-7.0.1rc0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc6/tests/test_utils.py` & `arize-7.0.1rc0/tests/test_utils.py`

 * *Files identical despite different names*

