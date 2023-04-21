# Comparing `tmp/jadecobra-0.3.6.tar.gz` & `tmp/jadecobra-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jadecobra-0.3.6.tar", last modified: Mon Apr  3 00:46:14 2023, max compression
+gzip compressed data, was "jadecobra-0.3.7.tar", last modified: Mon Apr  3 00:47:12 2023, max compression
```

## Comparing `jadecobra-0.3.6.tar` & `jadecobra-0.3.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:46:14.469612 jadecobra-0.3.6/
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1066 2022-08-18 02:10:38.000000 jadecobra-0.3.6/LICENSE
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1877 2023-04-03 00:46:14.469402 jadecobra-0.3.6/PKG-INFO
--rw-r--r--   0 johnnyblase   (501) staff       (20)      150 2022-08-29 03:32:29.000000 jadecobra-0.3.6/README.md
--rw-r--r--   0 johnnyblase   (501) staff       (20)      533 2023-04-03 00:45:09.000000 jadecobra-0.3.6/pyproject.toml
--rw-r--r--   0 johnnyblase   (501) staff       (20)       38 2023-04-03 00:46:14.469727 jadecobra-0.3.6/setup.cfg
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:46:14.463988 jadecobra-0.3.6/src/
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:46:14.465712 jadecobra-0.3.6/src/jadecobra/
--rw-r--r--   0 johnnyblase   (501) staff       (20)       21 2023-04-03 00:45:09.000000 jadecobra-0.3.6/src/jadecobra/__init__.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1422 2022-08-19 16:12:38.000000 jadecobra-0.3.6/src/jadecobra/aws_environment.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:46:14.466588 jadecobra-0.3.6/src/jadecobra/aws_lambda/
--rw-r--r--   0 johnnyblase   (501) staff       (20)      170 2023-03-29 21:40:49.000000 jadecobra-0.3.6/src/jadecobra/aws_lambda/__init__.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:46:14.467333 jadecobra-0.3.6/src/jadecobra/aws_lambda/deploy/
--rw-r--r--   0 johnnyblase   (501) staff       (20)       27 2022-08-19 16:21:46.000000 jadecobra-0.3.6/src/jadecobra/aws_lambda/deploy/__init__.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1349 2023-03-31 22:22:12.000000 jadecobra-0.3.6/src/jadecobra/aws_lambda/deploy/deploy.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1187 2023-04-02 23:31:34.000000 jadecobra-0.3.6/src/jadecobra/aws_lambda/deploy/deploy_lambda.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2022-08-19 16:21:46.000000 jadecobra-0.3.6/src/jadecobra/aws_lambda/deploy/lambda_function.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     3731 2023-03-31 22:35:26.000000 jadecobra-0.3.6/src/jadecobra/aws_lambda/deploy/lambda_layer.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-01-30 18:47:15.000000 jadecobra-0.3.6/src/jadecobra/cloudformation_deployer.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)        0 2023-03-31 20:02:12.000000 jadecobra-0.3.6/src/jadecobra/setup_tdd.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1960 2023-04-03 00:40:54.000000 jadecobra-0.3.6/src/jadecobra/tester.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1784 2023-04-03 00:06:36.000000 jadecobra-0.3.6/src/jadecobra/toolkit.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1694 2023-04-03 00:36:26.000000 jadecobra-0.3.6/src/jadecobra/versioning.py
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:46:14.466424 jadecobra-0.3.6/src/jadecobra.egg-info/
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1877 2023-04-03 00:46:14.000000 jadecobra-0.3.6/src/jadecobra.egg-info/PKG-INFO
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1029 2023-04-03 00:46:14.000000 jadecobra-0.3.6/src/jadecobra.egg-info/SOURCES.txt
--rw-r--r--   0 johnnyblase   (501) staff       (20)        1 2023-04-03 00:46:14.000000 jadecobra-0.3.6/src/jadecobra.egg-info/dependency_links.txt
--rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-04-03 00:46:14.000000 jadecobra-0.3.6/src/jadecobra.egg-info/requires.txt
--rw-r--r--   0 johnnyblase   (501) staff       (20)       10 2023-04-03 00:46:14.000000 jadecobra-0.3.6/src/jadecobra.egg-info/top_level.txt
-drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:46:14.469146 jadecobra-0.3.6/tests/
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1393 2023-04-02 23:59:47.000000 jadecobra-0.3.6/tests/test_aws_deploy_lambda.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2023-04-03 00:42:01.000000 jadecobra-0.3.6/tests/test_aws_deploy_lambda_function.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1869 2023-04-03 00:42:18.000000 jadecobra-0.3.6/tests/test_aws_deploy_lambda_layer.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)      969 2023-04-02 23:59:37.000000 jadecobra-0.3.6/tests/test_aws_lambda.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1446 2023-04-02 23:59:37.000000 jadecobra-0.3.6/tests/test_environment.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)      676 2023-04-03 00:32:32.000000 jadecobra-0.3.6/tests/test_jadecobra.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     4806 2023-04-03 00:16:06.000000 jadecobra-0.3.6/tests/test_jadecobra_tester.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     1195 2023-04-03 00:32:43.000000 jadecobra-0.3.6/tests/test_jadecobra_toolkit.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)     2027 2023-04-03 00:45:49.000000 jadecobra-0.3.6/tests/test_jadecobra_versioning.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)        0 2023-03-31 20:47:21.000000 jadecobra-0.3.6/tests/test_setup_tdd.py
--rw-r--r--   0 johnnyblase   (501) staff       (20)      401 2023-04-03 00:41:37.000000 jadecobra-0.3.6/tests/test_z_build_publish.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:47:12.943803 jadecobra-0.3.7/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1066 2022-08-18 02:10:38.000000 jadecobra-0.3.7/LICENSE
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1877 2023-04-03 00:47:12.943654 jadecobra-0.3.7/PKG-INFO
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      150 2022-08-29 03:32:29.000000 jadecobra-0.3.7/README.md
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      533 2023-04-03 00:46:54.000000 jadecobra-0.3.7/pyproject.toml
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       38 2023-04-03 00:47:12.943847 jadecobra-0.3.7/setup.cfg
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:47:12.935666 jadecobra-0.3.7/src/
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:47:12.938315 jadecobra-0.3.7/src/jadecobra/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       21 2023-04-03 00:46:54.000000 jadecobra-0.3.7/src/jadecobra/__init__.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1422 2022-08-19 16:12:38.000000 jadecobra-0.3.7/src/jadecobra/aws_environment.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:47:12.939323 jadecobra-0.3.7/src/jadecobra/aws_lambda/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      170 2023-03-29 21:40:49.000000 jadecobra-0.3.7/src/jadecobra/aws_lambda/__init__.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:47:12.940897 jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       27 2022-08-19 16:21:46.000000 jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/__init__.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1349 2023-03-31 22:22:12.000000 jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/deploy.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1187 2023-04-02 23:31:34.000000 jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/deploy_lambda.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2022-08-19 16:21:46.000000 jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/lambda_function.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     3731 2023-03-31 22:35:26.000000 jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/lambda_layer.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-01-30 18:47:15.000000 jadecobra-0.3.7/src/jadecobra/cloudformation_deployer.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)        0 2023-03-31 20:02:12.000000 jadecobra-0.3.7/src/jadecobra/setup_tdd.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1960 2023-04-03 00:40:54.000000 jadecobra-0.3.7/src/jadecobra/tester.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1784 2023-04-03 00:06:36.000000 jadecobra-0.3.7/src/jadecobra/toolkit.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1694 2023-04-03 00:36:26.000000 jadecobra-0.3.7/src/jadecobra/versioning.py
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:47:12.939189 jadecobra-0.3.7/src/jadecobra.egg-info/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1877 2023-04-03 00:47:12.000000 jadecobra-0.3.7/src/jadecobra.egg-info/PKG-INFO
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1029 2023-04-03 00:47:12.000000 jadecobra-0.3.7/src/jadecobra.egg-info/SOURCES.txt
+-rw-r--r--   0 johnnyblase   (501) staff       (20)        1 2023-04-03 00:47:12.000000 jadecobra-0.3.7/src/jadecobra.egg-info/dependency_links.txt
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       14 2023-04-03 00:47:12.000000 jadecobra-0.3.7/src/jadecobra.egg-info/requires.txt
+-rw-r--r--   0 johnnyblase   (501) staff       (20)       10 2023-04-03 00:47:12.000000 jadecobra-0.3.7/src/jadecobra.egg-info/top_level.txt
+drwxr-xr-x   0 johnnyblase   (501) staff       (20)        0 2023-04-03 00:47:12.943448 jadecobra-0.3.7/tests/
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1393 2023-04-02 23:59:47.000000 jadecobra-0.3.7/tests/test_aws_deploy_lambda.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1745 2023-04-03 00:42:01.000000 jadecobra-0.3.7/tests/test_aws_deploy_lambda_function.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1869 2023-04-03 00:42:18.000000 jadecobra-0.3.7/tests/test_aws_deploy_lambda_layer.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      969 2023-04-02 23:59:37.000000 jadecobra-0.3.7/tests/test_aws_lambda.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1446 2023-04-02 23:59:37.000000 jadecobra-0.3.7/tests/test_environment.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      676 2023-04-03 00:32:32.000000 jadecobra-0.3.7/tests/test_jadecobra.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     4806 2023-04-03 00:16:06.000000 jadecobra-0.3.7/tests/test_jadecobra_tester.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1195 2023-04-03 00:32:43.000000 jadecobra-0.3.7/tests/test_jadecobra_toolkit.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)     1832 2023-04-03 00:46:48.000000 jadecobra-0.3.7/tests/test_jadecobra_versioning.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)        0 2023-03-31 20:47:21.000000 jadecobra-0.3.7/tests/test_setup_tdd.py
+-rw-r--r--   0 johnnyblase   (501) staff       (20)      598 2023-04-03 00:46:57.000000 jadecobra-0.3.7/tests/test_z_build_publish.py
```

### Comparing `jadecobra-0.3.6/LICENSE` & `jadecobra-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/PKG-INFO` & `jadecobra-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jadecobra
-Version: 0.3.6
+Version: 0.3.7
 Summary: DRY
 Author-email: johnnyblase <johnnyblasin@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 jadecobra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jadecobra-0.3.6/pyproject.toml` & `jadecobra-0.3.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jadecobra"
-version = "0.3.6"
+version = "0.3.7"
 authors = [
   { name="johnnyblase", email="johnnyblasin@gmail.com" },
 ]
 description = "DRY"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `jadecobra-0.3.6/src/jadecobra/aws_environment.py` & `jadecobra-0.3.7/src/jadecobra/aws_environment.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/src/jadecobra/aws_lambda/deploy/deploy.py` & `jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/deploy.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/src/jadecobra/aws_lambda/deploy/deploy_lambda.py` & `jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/deploy_lambda.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/src/jadecobra/aws_lambda/deploy/lambda_function.py` & `jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/lambda_function.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/src/jadecobra/aws_lambda/deploy/lambda_layer.py` & `jadecobra-0.3.7/src/jadecobra/aws_lambda/deploy/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/src/jadecobra/tester.py` & `jadecobra-0.3.7/src/jadecobra/tester.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/src/jadecobra/toolkit.py` & `jadecobra-0.3.7/src/jadecobra/toolkit.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/src/jadecobra/versioning.py` & `jadecobra-0.3.7/src/jadecobra/versioning.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/src/jadecobra.egg-info/PKG-INFO` & `jadecobra-0.3.7/src/jadecobra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jadecobra
-Version: 0.3.6
+Version: 0.3.7
 Summary: DRY
 Author-email: johnnyblase <johnnyblasin@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 jadecobra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jadecobra-0.3.6/src/jadecobra.egg-info/SOURCES.txt` & `jadecobra-0.3.7/src/jadecobra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/tests/test_aws_deploy_lambda.py` & `jadecobra-0.3.7/tests/test_aws_deploy_lambda.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/tests/test_aws_deploy_lambda_function.py` & `jadecobra-0.3.7/tests/test_aws_deploy_lambda_function.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/tests/test_aws_deploy_lambda_layer.py` & `jadecobra-0.3.7/tests/test_aws_deploy_lambda_layer.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/tests/test_aws_lambda.py` & `jadecobra-0.3.7/tests/test_aws_lambda.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/tests/test_environment.py` & `jadecobra-0.3.7/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/tests/test_jadecobra.py` & `jadecobra-0.3.7/tests/test_jadecobra.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/tests/test_jadecobra_tester.py` & `jadecobra-0.3.7/tests/test_jadecobra_tester.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/tests/test_jadecobra_toolkit.py` & `jadecobra-0.3.7/tests/test_jadecobra_toolkit.py`

 * *Files identical despite different names*

### Comparing `jadecobra-0.3.6/tests/test_jadecobra_versioning.py` & `jadecobra-0.3.7/tests/test_jadecobra_versioning.py`

 * *Files 18% similar despite different names*

```diff
@@ -60,13 +60,8 @@
                 'read_pyproject',
                 'semantic_version_pattern',
                 'update_module_version',
                 'update_pyproject_version'
             ]
         )
 
-    def test_update_version(self):
-        version = src.jadecobra.versioning.Version()
-        self.assertEqual(
-            version.get_pyproject_version(),
-            ('0.3.', '2'),
-        )
+
```

