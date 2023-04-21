# Comparing `tmp/lesiwka-2.0.20230118.0.tar.gz` & `tmp/lesiwka-2.1.20230423.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lesiwka-2.0.20230118.0.tar", last modified: Tue Jan 17 23:42:17 2023, max compression
+gzip compressed data, was "lesiwka-2.1.20230423.0.tar", last modified: Fri Apr 21 13:34:38 2023, max compression
```

## Comparing `lesiwka-2.0.20230118.0.tar` & `lesiwka-2.1.20230423.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 23:42:17.805336 lesiwka-2.0.20230118.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-01-17 23:42:17.805336 lesiwka-2.0.20230118.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 23:42:17.801336 lesiwka-2.0.20230118.0/lesiwka/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 23:42:17.805336 lesiwka-2.0.20230118.0/lesiwka/_decode/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_decode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_decode/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_decode/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_decode/rule_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_decode/rule_1_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_decode/rule_1_3.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_decode/rule_1_4.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_decode/rule_1_5.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_decode/rule_1_6.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_decode/rule_1_7.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_decode/rule_2_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_decode/rule_3_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_decode/rule_3_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_decode/rule_3_4.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/diacritics.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/punctuation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/lesiwka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 23:42:17.805336 lesiwka-2.0.20230118.0/lesiwka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-01-17 23:42:17.000000 lesiwka-2.0.20230118.0/lesiwka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-01-17 23:42:17.000000 lesiwka-2.0.20230118.0/lesiwka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 23:42:17.000000 lesiwka-2.0.20230118.0/lesiwka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-17 23:42:17.000000 lesiwka-2.0.20230118.0/lesiwka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-17 23:42:17.000000 lesiwka-2.0.20230118.0/lesiwka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-01-17 23:42:17.805336 lesiwka-2.0.20230118.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 23:42:10.000000 lesiwka-2.0.20230118.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:34:38.555656 lesiwka-2.1.20230423.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-21 13:34:38.555656 lesiwka-2.1.20230423.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:34:38.551656 lesiwka-2.1.20230423.0/lesiwka/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:34:38.555656 lesiwka-2.1.20230423.0/lesiwka/_decode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_1_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_1_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_1_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_1_6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_1_7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_2_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_3_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_3_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_3_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/diacritics.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/punctuation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:34:38.551656 lesiwka-2.1.20230423.0/lesiwka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-21 13:34:38.000000 lesiwka-2.1.20230423.0/lesiwka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-21 13:34:38.000000 lesiwka-2.1.20230423.0/lesiwka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:34:38.000000 lesiwka-2.1.20230423.0/lesiwka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 13:34:38.000000 lesiwka-2.1.20230423.0/lesiwka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 13:34:38.000000 lesiwka-2.1.20230423.0/lesiwka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-21 13:34:38.555656 lesiwka-2.1.20230423.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/setup.py
```

### Comparing `lesiwka-2.0.20230118.0/LICENSE` & `lesiwka-2.1.20230423.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lesiwka-2.0.20230118.0/PKG-INFO` & `lesiwka-2.1.20230423.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: lesiwka
-Version: 2.0.20230118.0
+Version: 2.1.20230423.0
 Summary: Python library to convert to/from Lesivka
 Author: Oleksandr Tishyn
 Author-email: 1079805+Mystic-Mirage@users.noreply.github.com
 License: CC0 1.0 Universal
 Project-URL: Source Code, https://github.com/lesiwka/python-lesiwka
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # python-lesiwka
 Python library to convert to/from Lesiwka
```

### Comparing `lesiwka-2.0.20230118.0/lesiwka/__main__.py` & `lesiwka-2.1.20230423.0/lesiwka/__main__.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.0.20230118.0/lesiwka/_decode/__init__.py` & `lesiwka-2.1.20230423.0/lesiwka/_decode/__init__.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.0.20230118.0/lesiwka/_decode/postprocess.py` & `lesiwka-2.1.20230423.0/lesiwka/_decode/postprocess.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.0.20230118.0/lesiwka/_decode/preprocess.py` & `lesiwka-2.1.20230423.0/lesiwka/_decode/preprocess.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.0.20230118.0/lesiwka/_decode/rule_2_2.py` & `lesiwka-2.1.20230423.0/lesiwka/_decode/rule_2_2.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.0.20230118.0/lesiwka/_encode.py` & `lesiwka-2.1.20230423.0/lesiwka/_encode.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,22 @@
     }
 )
 table[sqcq_lower_cyr] = sqcq_lower_lat
 table[sqcq_upper_cyr] = sqcq_upper_lat
 table = str.maketrans(table)
 
 
+def pre_validate(text):
+    return re.search("[ґєіїҐЄІЇ]", text) or not re.search("[ёўъыэЁЎЪЫЭ]", text)
+
+
 def encode(text, no_diacritics=False):
+    if not pre_validate(text):
+        return text
+
     result = text
 
     for pattern, repl in patterns:
         result = re.sub(pattern, repl, result)
 
     result = result.translate(table)
```

### Comparing `lesiwka-2.0.20230118.0/lesiwka/ascii.py` & `lesiwka-2.1.20230423.0/lesiwka/ascii.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.0.20230118.0/lesiwka/utils.py` & `lesiwka-2.1.20230423.0/lesiwka/utils.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.0.20230118.0/lesiwka.egg-info/PKG-INFO` & `lesiwka-2.1.20230423.0/lesiwka.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: lesiwka
-Version: 2.0.20230118.0
+Version: 2.1.20230423.0
 Summary: Python library to convert to/from Lesivka
 Author: Oleksandr Tishyn
 Author-email: 1079805+Mystic-Mirage@users.noreply.github.com
 License: CC0 1.0 Universal
 Project-URL: Source Code, https://github.com/lesiwka/python-lesiwka
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # python-lesiwka
 Python library to convert to/from Lesiwka
```

### Comparing `lesiwka-2.0.20230118.0/lesiwka.egg-info/SOURCES.txt` & `lesiwka-2.1.20230423.0/lesiwka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lesiwka-2.0.20230118.0/setup.cfg` & `lesiwka-2.1.20230423.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 project_urls = 
 	Source Code = https://github.com/lesiwka/python-lesiwka
 
 [options]
 packages = find:
 
 [options.extras_require]
```

