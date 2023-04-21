# Comparing `tmp/Trial2Vec-0.0.4.tar.gz` & `tmp/Trial2Vec-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Trial2Vec-0.0.4.tar", last modified: Thu Dec  8 16:34:24 2022, max compression
+gzip compressed data, was "dist/Trial2Vec-0.1.0.tar", last modified: Fri Apr 21 15:33:51 2023, max compression
```

## Comparing `Trial2Vec-0.0.4.tar` & `Trial2Vec-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-12-08 16:34:24.000000 Trial2Vec-0.0.4/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1063 2022-10-09 01:32:45.000000 Trial2Vec-0.0.4/LICENSE
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3677 2022-12-08 16:34:24.000000 Trial2Vec-0.0.4/PKG-INFO
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2989 2022-12-08 16:31:43.000000 Trial2Vec-0.0.4/README.md
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-12-08 16:34:24.000000 Trial2Vec-0.0.4/Trial2Vec.egg-info/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3677 2022-12-08 16:34:24.000000 Trial2Vec-0.0.4/Trial2Vec.egg-info/PKG-INFO
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      393 2022-12-08 16:34:24.000000 Trial2Vec-0.0.4/Trial2Vec.egg-info/SOURCES.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        1 2022-12-08 16:34:24.000000 Trial2Vec-0.0.4/Trial2Vec.egg-info/dependency_links.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       78 2022-12-08 16:34:24.000000 Trial2Vec-0.0.4/Trial2Vec.egg-info/requires.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       10 2022-12-08 16:34:24.000000 Trial2Vec-0.0.4/Trial2Vec.egg-info/top_level.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       38 2022-12-08 16:34:24.000000 Trial2Vec-0.0.4/setup.cfg
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1219 2022-12-08 16:31:11.000000 Trial2Vec-0.0.4/setup.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-12-08 16:34:24.000000 Trial2Vec-0.0.4/trial2vec/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      143 2022-12-08 16:30:46.000000 Trial2Vec-0.0.4/trial2vec/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6576 2022-10-09 01:35:40.000000 Trial2Vec-0.0.4/trial2vec/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3088 2022-10-09 01:35:31.000000 Trial2Vec-0.0.4/trial2vec/check.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1567 2022-10-09 01:40:32.000000 Trial2Vec-0.0.4/trial2vec/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1311 2022-10-09 18:50:12.000000 Trial2Vec-0.0.4/trial2vec/demo_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1223 2022-10-09 01:38:42.000000 Trial2Vec-0.0.4/trial2vec/losses.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      551 2022-10-09 01:40:49.000000 Trial2Vec-0.0.4/trial2vec/metrics.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    43822 2022-12-08 16:30:00.000000 Trial2Vec-0.0.4/trial2vec/model.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10434 2022-10-09 01:36:58.000000 Trial2Vec-0.0.4/trial2vec/parallel.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    17955 2022-10-09 01:38:45.000000 Trial2Vec-0.0.4/trial2vec/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 15:33:51.000000 Trial2Vec-0.1.0/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1063 2022-10-09 01:32:45.000000 Trial2Vec-0.1.0/LICENSE
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3677 2023-04-21 15:33:51.000000 Trial2Vec-0.1.0/PKG-INFO
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2989 2022-12-08 16:31:43.000000 Trial2Vec-0.1.0/README.md
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 15:33:51.000000 Trial2Vec-0.1.0/Trial2Vec.egg-info/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3677 2023-04-21 15:33:51.000000 Trial2Vec-0.1.0/Trial2Vec.egg-info/PKG-INFO
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      393 2023-04-21 15:33:51.000000 Trial2Vec-0.1.0/Trial2Vec.egg-info/SOURCES.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        1 2023-04-21 15:33:51.000000 Trial2Vec-0.1.0/Trial2Vec.egg-info/dependency_links.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       78 2023-04-21 15:33:51.000000 Trial2Vec-0.1.0/Trial2Vec.egg-info/requires.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       10 2023-04-21 15:33:51.000000 Trial2Vec-0.1.0/Trial2Vec.egg-info/top_level.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       38 2023-04-21 15:33:51.000000 Trial2Vec-0.1.0/setup.cfg
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1219 2023-04-21 15:33:10.000000 Trial2Vec-0.1.0/setup.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 15:33:51.000000 Trial2Vec-0.1.0/trial2vec/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      143 2023-04-21 15:33:25.000000 Trial2Vec-0.1.0/trial2vec/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6576 2022-10-09 01:35:40.000000 Trial2Vec-0.1.0/trial2vec/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3088 2022-10-09 01:35:31.000000 Trial2Vec-0.1.0/trial2vec/check.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1567 2022-10-09 01:40:32.000000 Trial2Vec-0.1.0/trial2vec/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1311 2022-10-09 18:50:12.000000 Trial2Vec-0.1.0/trial2vec/demo_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1223 2022-10-09 01:38:42.000000 Trial2Vec-0.1.0/trial2vec/losses.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      551 2022-10-09 01:40:49.000000 Trial2Vec-0.1.0/trial2vec/metrics.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    43856 2023-04-21 15:24:04.000000 Trial2Vec-0.1.0/trial2vec/model.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10434 2022-10-09 01:36:58.000000 Trial2Vec-0.1.0/trial2vec/parallel.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    17955 2022-10-09 01:38:45.000000 Trial2Vec-0.1.0/trial2vec/trainer.py
```

### Comparing `Trial2Vec-0.0.4/LICENSE` & `Trial2Vec-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Trial2Vec-0.0.4/PKG-INFO` & `Trial2Vec-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Trial2Vec
-Version: 0.0.4
+Version: 0.1.0
 Summary: Pretrained BERT models for encoding clinical trial documents to compact embeddings.
 Home-page: https://github.com/RyanWangZf/Trial2Vec
 Author: Zifeng Wang
 Author-email: zifengw2@illinois.edu
 Keywords: clinical trial,machine learning,data mining,information retrieval
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Trial2Vec-0.0.4/README.md` & `Trial2Vec-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `Trial2Vec-0.0.4/Trial2Vec.egg-info/PKG-INFO` & `Trial2Vec-0.1.0/Trial2Vec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Trial2Vec
-Version: 0.0.4
+Version: 0.1.0
 Summary: Pretrained BERT models for encoding clinical trial documents to compact embeddings.
 Home-page: https://github.com/RyanWangZf/Trial2Vec
 Author: Zifeng Wang
 Author-email: zifengw2@illinois.edu
 Keywords: clinical trial,machine learning,data mining,information retrieval
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Trial2Vec-0.0.4/setup.py` & `Trial2Vec-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # read the contents of requirements.txt
 with open(os.path.join(this_directory, 'requirements.txt'),
           encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name = 'Trial2Vec',
-    version = '0.0.4',
+    version = '0.1.0',
     author = 'Zifeng Wang',
     author_email = 'zifengw2@illinois.edu',
     description = 'Pretrained BERT models for encoding clinical trial documents to compact embeddings.',
     url = 'https://github.com/RyanWangZf/Trial2Vec',
     keywords=['clinical trial', 'machine learning', 'data mining', 'information retrieval'],
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `Trial2Vec-0.0.4/trial2vec/base.py` & `Trial2Vec-0.1.0/trial2vec/base.py`

 * *Files identical despite different names*

### Comparing `Trial2Vec-0.0.4/trial2vec/check.py` & `Trial2Vec-0.1.0/trial2vec/check.py`

 * *Files identical despite different names*

### Comparing `Trial2Vec-0.0.4/trial2vec/data.py` & `Trial2Vec-0.1.0/trial2vec/data.py`

 * *Files identical despite different names*

### Comparing `Trial2Vec-0.0.4/trial2vec/demo_data.py` & `Trial2Vec-0.1.0/trial2vec/demo_data.py`

 * *Files identical despite different names*

### Comparing `Trial2Vec-0.0.4/trial2vec/losses.py` & `Trial2Vec-0.1.0/trial2vec/losses.py`

 * *Files identical despite different names*

### Comparing `Trial2Vec-0.0.4/trial2vec/metrics.py` & `Trial2Vec-0.1.0/trial2vec/metrics.py`

 * *Files identical despite different names*

### Comparing `Trial2Vec-0.0.4/trial2vec/model.py` & `Trial2Vec-0.1.0/trial2vec/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -829,15 +829,15 @@
         checkpoint: str
             The input dir that stores the pretrained model.
             If a directory, the only checkpoint file `*.pth.tar` will be loaded.
             If a filepath, will load from this file.
         '''
         checkpoint_filename = check_checkpoint_file(checkpoint)
         config_filename = check_model_config_file(checkpoint)
-        state_dict = torch.load(checkpoint_filename)
+        state_dict = torch.load(checkpoint_filename, map_location=torch.device('cpu'))
         if config_filename is not None:
             config = self._load_model_config(config_filename)
             self.config.update(config)
             self.model.config.update({'fields':config['fields'], 'ctx_fields':config['ctx_fields']})
         self.model.load_state_dict(state_dict['model'])
         self.trial_embs = state_dict['emb']
```

### Comparing `Trial2Vec-0.0.4/trial2vec/parallel.py` & `Trial2Vec-0.1.0/trial2vec/parallel.py`

 * *Files identical despite different names*

### Comparing `Trial2Vec-0.0.4/trial2vec/trainer.py` & `Trial2Vec-0.1.0/trial2vec/trainer.py`

 * *Files identical despite different names*

