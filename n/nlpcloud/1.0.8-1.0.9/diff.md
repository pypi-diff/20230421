# Comparing `tmp/nlpcloud-1.0.8.tar.gz` & `tmp/nlpcloud-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nlpcloud-1.0.8.tar", last modified: Mon Apr 26 17:51:36 2021, max compression
+gzip compressed data, was "nlpcloud-1.0.9.tar", last modified: Tue Apr 27 14:32:13 2021, max compression
```

## Comparing `nlpcloud-1.0.8.tar` & `nlpcloud-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 juliensalinas  (1000) juliensalinas  (1000)        0 2021-04-26 17:51:36.196126 nlpcloud-1.0.8/
--rw-rw-r--   0 juliensalinas  (1000) juliensalinas  (1000)      792 2021-04-26 17:51:36.196126 nlpcloud-1.0.8/PKG-INFO
--rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)     4325 2021-04-26 17:44:23.000000 nlpcloud-1.0.8/README.md
-drwxrwxr-x   0 juliensalinas  (1000) juliensalinas  (1000)        0 2021-04-26 17:51:36.196126 nlpcloud-1.0.8/nlpcloud/
--rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)     2490 2021-03-04 20:17:13.000000 nlpcloud-1.0.8/nlpcloud/__init__.py
-drwxrwxr-x   0 juliensalinas  (1000) juliensalinas  (1000)        0 2021-04-26 17:51:36.196126 nlpcloud-1.0.8/nlpcloud.egg-info/
--rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)      792 2021-04-26 17:51:36.000000 nlpcloud-1.0.8/nlpcloud.egg-info/PKG-INFO
--rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)      167 2021-04-26 17:51:36.000000 nlpcloud-1.0.8/nlpcloud.egg-info/SOURCES.txt
--rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)        1 2021-04-26 17:51:36.000000 nlpcloud-1.0.8/nlpcloud.egg-info/dependency_links.txt
--rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)        9 2021-04-26 17:51:36.000000 nlpcloud-1.0.8/nlpcloud.egg-info/top_level.txt
--rw-rw-r--   0 juliensalinas  (1000) juliensalinas  (1000)       38 2021-04-26 17:51:36.196126 nlpcloud-1.0.8/setup.cfg
--rw-rw-r--   0 juliensalinas  (1000) juliensalinas  (1000)      855 2021-04-26 17:51:25.000000 nlpcloud-1.0.8/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-04-27 14:32:13.368677 nlpcloud-1.0.9/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      792 2021-04-27 14:32:13.368677 nlpcloud-1.0.9/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4529 2021-04-27 14:32:00.000000 nlpcloud-1.0.9/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-04-27 14:32:13.368677 nlpcloud-1.0.9/nlpcloud/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2756 2021-04-27 14:31:18.000000 nlpcloud-1.0.9/nlpcloud/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-04-27 14:32:13.368677 nlpcloud-1.0.9/nlpcloud.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      792 2021-04-27 14:32:12.000000 nlpcloud-1.0.9/nlpcloud.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      167 2021-04-27 14:32:12.000000 nlpcloud-1.0.9/nlpcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2021-04-27 14:32:12.000000 nlpcloud-1.0.9/nlpcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2021-04-27 14:32:12.000000 nlpcloud-1.0.9/nlpcloud.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2021-04-27 14:32:13.368677 nlpcloud-1.0.9/setup.cfg
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      855 2021-04-27 14:30:53.000000 nlpcloud-1.0.9/setup.py
```

### Comparing `nlpcloud-1.0.8/PKG-INFO` & `nlpcloud-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: nlpcloud
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python client for the NLP Cloud API
 Home-page: https://github.com/nlpcloud/nlpcloud-python
 Author: Julien Salinas
 Author-email: all@juliensalinas.com
 License: MIT
 Description: NLP Cloud serves high performance pre-trained or custom models for NER, sentiment-analysis, classification, summarization, question answering, and POS tagging, ready for production, served through a REST API.
```

### Comparing `nlpcloud-1.0.8/README.md` & `nlpcloud-1.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -132,14 +132,24 @@
 
 ```python
 client.summarization("<Your text to summarize>")
 ```
 
 The above command returns a JSON object.
 
+### Translation Endpoint
+
+Call the `translation()` method and pass the text you want to translate.
+
+```python
+client.translation("<Your text to translate>")
+```
+
+The above command returns a JSON object.
+
 ### Dependencies Endpoint
 
 Call the `dependencies()` method and pass the text you want to perform part of speech tagging (POS) + arcs on.
 
 ```python
 client.dependencies("<Your block of text>")
 ```
```

### Comparing `nlpcloud-1.0.8/nlpcloud/__init__.py` & `nlpcloud-1.0.9/nlpcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,26 @@
         r = requests.post(
             "{}/{}".format(self.root_url, "summarization"), json=payload, headers=self.headers)
 
         r.raise_for_status()
 
         return r.json()
 
+    def translation(self, text):
+        payload = {
+            "text": text
+        }
+
+        r = requests.post(
+            "{}/{}".format(self.root_url, "translation"), json=payload, headers=self.headers)
+
+        r.raise_for_status()
+
+        return r.json()
+
     def dependencies(self, text):
         payload = {
             "text": text
         }
 
         r = requests.post(
             "{}/{}".format(self.root_url, "dependencies"), json=payload, headers=self.headers)
```

### Comparing `nlpcloud-1.0.8/nlpcloud.egg-info/PKG-INFO` & `nlpcloud-1.0.9/nlpcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: nlpcloud
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python client for the NLP Cloud API
 Home-page: https://github.com/nlpcloud/nlpcloud-python
 Author: Julien Salinas
 Author-email: all@juliensalinas.com
 License: MIT
 Description: NLP Cloud serves high performance pre-trained or custom models for NER, sentiment-analysis, classification, summarization, question answering, and POS tagging, ready for production, served through a REST API.
```

### Comparing `nlpcloud-1.0.8/setup.py` & `nlpcloud-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='nlpcloud',
-    version='1.0.8',
+    version='1.0.9',
     description='Python client for the NLP Cloud API',
     long_description="NLP Cloud serves high performance pre-trained or custom models for NER, sentiment-analysis, classification, summarization, question answering, and POS tagging, ready for production, served through a REST API.\n\nThis is the Python client for the API.\n\nMore details here: https://nlpcloud.io\n\nDocumentation: https://docs.nlpcloud.io\n\nGithub: https://github.com/nlpcloud/nlpcloud-python",
     packages=['nlpcloud'],
     author='Julien Salinas',
     author_email='all@juliensalinas.com',
     license='MIT',
     keywords=['api', 'NLP', 'spacy', 'Hugging Face', 'deep learning', 'machine learning',
```

