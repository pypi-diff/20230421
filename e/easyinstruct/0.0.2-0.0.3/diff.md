# Comparing `tmp/easyinstruct-0.0.2.tar.gz` & `tmp/easyinstruct-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyinstruct-0.0.2.tar", last modified: Sat Mar 25 09:40:12 2023, max compression
+gzip compressed data, was "easyinstruct-0.0.3.tar", last modified: Fri Apr 21 04:50:22 2023, max compression
```

## Comparing `easyinstruct-0.0.2.tar` & `easyinstruct-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 oeheart   (1000) oeheart   (1000)        0 2023-03-25 09:40:12.674060 easyinstruct-0.0.2/
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)     1063 2023-03-25 09:38:39.000000 easyinstruct-0.0.2/LICENSE
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)     1623 2023-03-25 09:40:12.673059 easyinstruct-0.0.2/PKG-INFO
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)      961 2023-03-25 09:38:39.000000 easyinstruct-0.0.2/README.md
-drwxr-xr-x   0 oeheart   (1000) oeheart   (1000)        0 2023-03-25 09:40:12.635976 easyinstruct-0.0.2/easyinstruct/
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)       23 2023-03-25 09:38:39.000000 easyinstruct-0.0.2/easyinstruct/__init__.py
-drwxr-xr-x   0 oeheart   (1000) oeheart   (1000)        0 2023-03-25 09:40:12.668056 easyinstruct-0.0.2/easyinstruct/prompts/
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)      199 2023-03-25 09:38:39.000000 easyinstruct-0.0.2/easyinstruct/prompts/__init__.py
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)     2568 2023-03-25 09:38:39.000000 easyinstruct-0.0.2/easyinstruct/prompts/base_prompt.py
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)      493 2023-03-25 09:38:39.000000 easyinstruct-0.0.2/easyinstruct/prompts/cot_prompt.py
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)      701 2023-03-25 09:38:39.000000 easyinstruct-0.0.2/easyinstruct/prompts/icl_prompt.py
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)    18953 2023-03-25 09:38:39.000000 easyinstruct-0.0.2/easyinstruct/prompts/ie_prompt.py
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)     3592 2023-03-25 09:38:39.000000 easyinstruct-0.0.2/easyinstruct/prompts/index_prompt.py
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)      433 2023-03-25 09:38:39.000000 easyinstruct-0.0.2/easyinstruct/utils.py
-drwxr-xr-x   0 oeheart   (1000) oeheart   (1000)        0 2023-03-25 09:40:12.650335 easyinstruct-0.0.2/easyinstruct.egg-info/
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)     1623 2023-03-25 09:40:12.000000 easyinstruct-0.0.2/easyinstruct.egg-info/PKG-INFO
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)      475 2023-03-25 09:40:12.000000 easyinstruct-0.0.2/easyinstruct.egg-info/SOURCES.txt
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)        1 2023-03-25 09:40:12.000000 easyinstruct-0.0.2/easyinstruct.egg-info/dependency_links.txt
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)       59 2023-03-25 09:40:12.000000 easyinstruct-0.0.2/easyinstruct.egg-info/requires.txt
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)       13 2023-03-25 09:40:12.000000 easyinstruct-0.0.2/easyinstruct.egg-info/top_level.txt
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)       38 2023-03-25 09:40:12.675056 easyinstruct-0.0.2/setup.cfg
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)     1395 2023-03-25 09:38:39.000000 easyinstruct-0.0.2/setup.py
-drwxr-xr-x   0 oeheart   (1000) oeheart   (1000)        0 2023-03-25 09:40:12.670054 easyinstruct-0.0.2/test/
--rw-r--r--   0 oeheart   (1000) oeheart   (1000)      288 2023-03-25 09:38:39.000000 easyinstruct-0.0.2/test/test.py
+drwxrwxr-x   0 oeheart   (1020) oeheart   (1020)        0 2023-04-21 04:50:22.793072 easyinstruct-0.0.3/
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     1063 2023-04-21 04:37:37.000000 easyinstruct-0.0.3/LICENSE
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)    13204 2023-04-21 04:50:22.793072 easyinstruct-0.0.3/PKG-INFO
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)    12543 2023-04-21 04:50:03.000000 easyinstruct-0.0.3/README.md
+drwxrwxr-x   0 oeheart   (1020) oeheart   (1020)        0 2023-04-21 04:50:22.793072 easyinstruct-0.0.3/easyinstruct/
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)       23 2023-04-21 04:37:37.000000 easyinstruct-0.0.3/easyinstruct/__init__.py
+drwxrwxr-x   0 oeheart   (1020) oeheart   (1020)        0 2023-04-21 04:50:22.793072 easyinstruct-0.0.3/easyinstruct/prompts/
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)      269 2023-04-21 04:37:37.000000 easyinstruct-0.0.3/easyinstruct/prompts/__init__.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     4424 2023-04-21 04:37:37.000000 easyinstruct-0.0.3/easyinstruct/prompts/base_prompt.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     2721 2023-04-21 04:37:37.000000 easyinstruct-0.0.3/easyinstruct/prompts/batch_prompt.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)      493 2023-04-21 04:37:37.000000 easyinstruct-0.0.3/easyinstruct/prompts/cot_prompt.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     1007 2023-04-21 04:37:37.000000 easyinstruct-0.0.3/easyinstruct/prompts/icl_prompt.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)    18141 2023-04-21 04:37:37.000000 easyinstruct-0.0.3/easyinstruct/prompts/ie_prompt.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     3592 2023-04-21 04:37:37.000000 easyinstruct-0.0.3/easyinstruct/prompts/index_prompt.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     4815 2023-04-21 04:37:37.000000 easyinstruct-0.0.3/easyinstruct/prompts/mm_prompt.py
+drwxrwxr-x   0 oeheart   (1020) oeheart   (1020)        0 2023-04-21 04:50:22.793072 easyinstruct-0.0.3/easyinstruct.egg-info/
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)    13204 2023-04-21 04:50:22.000000 easyinstruct-0.0.3/easyinstruct.egg-info/PKG-INFO
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)      511 2023-04-21 04:50:22.000000 easyinstruct-0.0.3/easyinstruct.egg-info/SOURCES.txt
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)        1 2023-04-21 04:50:22.000000 easyinstruct-0.0.3/easyinstruct.egg-info/dependency_links.txt
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)       76 2023-04-21 04:50:22.000000 easyinstruct-0.0.3/easyinstruct.egg-info/requires.txt
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)       13 2023-04-21 04:50:22.000000 easyinstruct-0.0.3/easyinstruct.egg-info/top_level.txt
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)       38 2023-04-21 04:50:22.793072 easyinstruct-0.0.3/setup.cfg
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     1440 2023-04-21 04:42:03.000000 easyinstruct-0.0.3/setup.py
```

### Comparing `easyinstruct-0.0.2/LICENSE` & `easyinstruct-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easyinstruct-0.0.2/easyinstruct/prompts/index_prompt.py` & `easyinstruct-0.0.3/easyinstruct/prompts/index_prompt.py`

 * *Files identical despite different names*

### Comparing `easyinstruct-0.0.2/setup.py` & `easyinstruct-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 
 REQUIRES = """
 openai==0.27.0
+anthropic==0.2.7
 llama-index==0.4.29
 langchain
 tiktoken
 nltk
 """
 
 def get_install_requires():
@@ -18,26 +19,27 @@
 with open("README.md") as f:
     readme = f.read()
 
 
 def do_setup():
     setup(
         name="easyinstruct",
-        version = '0.0.2',
+        version = '0.0.3',
         description = "A easy-to-use framework to instruct large language models.",
         url="https://github.com/zjunlp/EasyInstruct",
         author = 'Yixin Ou',
         long_description=readme,
         long_description_content_type="text/markdown",
         install_requires=get_install_requires(),
         python_requires=">=3.7.0",
         packages=find_packages(
             exclude=[
                 "test*",
                 "examples*",
+                "gitbook*",
             ]
         ),
         keywords=["AI", "NLP", "instruction", "language model"],
         classifiers=[
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
```

