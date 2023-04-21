# Comparing `tmp/syngen-0.0.92.tar.gz` & `tmp/syngen-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.0.92.tar", last modified: Wed Apr 19 14:56:42 2023, max compression
+gzip compressed data, was "syngen-0.0.93.tar", last modified: Thu Apr 20 12:37:53 2023, max compression
```

## Comparing `syngen-0.0.92.tar` & `syngen-0.0.93.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.128434 syngen-0.0.92/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-19 14:55:18.000000 syngen-0.0.92/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-19 14:55:18.000000 syngen-0.0.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-19 14:55:18.000000 syngen-0.0.92/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-19 14:56:42.128434 syngen-0.0.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14148 2023-04-19 14:55:18.000000 syngen-0.0.92/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-19 14:55:18.000000 syngen-0.0.92/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-04-19 14:56:42.128434 syngen-0.0.92/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.116433 syngen-0.0.92/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.120433 syngen-0.0.92/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.120433 syngen-0.0.92/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.120433 syngen-0.0.92/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10105 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.124433 syngen-0.0.92/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.124433 syngen-0.0.92/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7294 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.124433 syngen-0.0.92/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.124433 syngen-0.0.92/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.120433 syngen-0.0.92/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.124433 syngen-0.0.92/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.124433 syngen-0.0.92/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43499 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.124433 syngen-0.0.92/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.128434 syngen-0.0.92/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6256 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.128434 syngen-0.0.92/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.128434 syngen-0.0.92/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15923 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.128434 syngen-0.0.92/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.128434 syngen-0.0.92/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.128434 syngen-0.0.92/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    28464 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10390 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.128434 syngen-0.0.92/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11009 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.128434 syngen-0.0.92/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.128434 syngen-0.0.92/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12935 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-04-19 14:55:18.000000 syngen-0.0.92/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:56:42.120433 syngen-0.0.92/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-19 14:56:42.000000 syngen-0.0.92/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-19 14:56:42.000000 syngen-0.0.92/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 14:56:42.000000 syngen-0.0.92/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-19 14:56:42.000000 syngen-0.0.92/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-19 14:56:42.000000 syngen-0.0.92/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-19 14:56:42.000000 syngen-0.0.92/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.783266 syngen-0.0.93/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-20 12:36:14.000000 syngen-0.0.93/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-20 12:36:14.000000 syngen-0.0.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-20 12:36:14.000000 syngen-0.0.93/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-20 12:37:53.787267 syngen-0.0.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14148 2023-04-20 12:36:14.000000 syngen-0.0.93/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-20 12:36:14.000000 syngen-0.0.93/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-04-20 12:37:53.787267 syngen-0.0.93/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.771266 syngen-0.0.93/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.775266 syngen-0.0.93/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.775266 syngen-0.0.93/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.775266 syngen-0.0.93/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10094 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.775266 syngen-0.0.93/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.775266 syngen-0.0.93/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7294 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.775266 syngen-0.0.93/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.779266 syngen-0.0.93/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.771266 syngen-0.0.93/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.779266 syngen-0.0.93/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.779266 syngen-0.0.93/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43499 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.779266 syngen-0.0.93/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.779266 syngen-0.0.93/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6256 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.783266 syngen-0.0.93/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.783266 syngen-0.0.93/src/syngen/ml/train_chain/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/train_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15923 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/train_chain/train_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.783266 syngen-0.0.93/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.783266 syngen-0.0.93/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.783266 syngen-0.0.93/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28464 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10390 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.783266 syngen-0.0.93/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11009 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.783266 syngen-0.0.93/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.783266 syngen-0.0.93/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12935 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-04-20 12:36:14.000000 syngen-0.0.93/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 12:37:53.775266 syngen-0.0.93/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-20 12:37:53.000000 syngen-0.0.93/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-20 12:37:53.000000 syngen-0.0.93/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 12:37:53.000000 syngen-0.0.93/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-20 12:37:53.000000 syngen-0.0.93/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-20 12:37:53.000000 syngen-0.0.93/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-20 12:37:53.000000 syngen-0.0.93/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.0.92/LICENSE` & `syngen-0.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/PKG-INFO` & `syngen-0.0.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.0.92
+Version: 0.0.93
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.0.92 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.0.93 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.0.92/README.md` & `syngen-0.0.93/README.md`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/setup.cfg` & `syngen-0.0.93/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/infer.py` & `syngen-0.0.93/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/config/configurations.py` & `syngen-0.0.93/src/syngen/ml/config/configurations.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,14 +238,14 @@
         return {
             "original_data_path": f"model_artifacts/tmp_store/{dynamic_name}/input_data_{dynamic_name}.pkl",
             "synthetic_data_path": f"model_artifacts/tmp_store/{dynamic_name}/merged_infer_{dynamic_name}.csv",
             "draws_path": f"model_artifacts/tmp_store/{dynamic_name}/draws",
             "input_data_path": f"model_artifacts/tmp_store/{dynamic_name}/input_data_{dynamic_name}.pkl",
             "path_to_merged_infer": f"model_artifacts/tmp_store/{dynamic_name}/merged_infer_{dynamic_name}.csv",
             "state_path": f"model_artifacts/resources/{dynamic_name}/vae/checkpoints",
-            "train_config_pickle_path": f"model_artifacts/resources/{self.slugify_table_name}/vae/checkpoints/train_config.pkl",
+            "train_config_pickle_path": f"model_artifacts/resources/{dynamic_name}/vae/checkpoints/train_config.pkl",
             "tmp_store_path": f"model_artifacts/tmp_store/{dynamic_name}",
             "vae_resources_path": f"model_artifacts/resources/{dynamic_name}/vae/checkpoints/",
             "dataset_pickle_path": f"model_artifacts/resources/{dynamic_name}/vae/checkpoints/model_dataset.pkl",
             "fk_kde_path": f"model_artifacts/resources/{dynamic_name}/vae/checkpoints/",
             "path_to_no_ml": f"model_artifacts/resources/{dynamic_name}/no_ml/checkpoints/kde_params.pkl",
         }
```

### Comparing `syngen-0.0.92/src/syngen/ml/convertor/convertor.py` & `syngen-0.0.93/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.0.93/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/metrics/__init__.py` & `syngen-0.0.93/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.0.93/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.0.93/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.0.93/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.0.93/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.0.93/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.0.93/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/metrics/utils.py` & `syngen-0.0.93/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/reporters/reporters.py` & `syngen-0.0.93/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/strategies/strategies.py` & `syngen-0.0.93/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/train_chain/train_chain.py` & `syngen-0.0.93/src/syngen/ml/train_chain/train_chain.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/utils/utils.py` & `syngen-0.0.93/src/syngen/ml/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.0.93/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/vae/models/dataset.py` & `syngen-0.0.93/src/syngen/ml/vae/models/dataset.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/vae/models/features.py` & `syngen-0.0.93/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/vae/models/model.py` & `syngen-0.0.93/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.0.93/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.0.93/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/ml/worker/worker.py` & `syngen-0.0.93/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen/train.py` & `syngen-0.0.93/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.92/src/syngen.egg-info/PKG-INFO` & `syngen-0.0.93/src/syngen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.0.92
+Version: 0.0.93
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.0.92 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.0.93 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.0.92/src/syngen.egg-info/SOURCES.txt` & `syngen-0.0.93/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

