# Comparing `tmp/lovehim-0.55.tar.gz` & `tmp/lovehim-0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lovehim-0.55.tar", last modified: Fri Apr 21 08:09:58 2023, max compression
+gzip compressed data, was "lovehim-0.56.tar", last modified: Fri Apr 21 08:12:34 2023, max compression
```

## Comparing `lovehim-0.55.tar` & `lovehim-0.56.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:09:58.335348 lovehim-0.55/
--rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:09:58.335229 lovehim-0.55/PKG-INFO
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:09:58.334282 lovehim-0.55/lovehim/
--rw-r--r--   0 gera       (501) staff       (20)       59 2023-04-21 06:29:58.000000 lovehim-0.55/lovehim/__init__.py
--rw-r--r--   0 gera       (501) staff       (20)      741 2023-04-21 08:09:40.000000 lovehim-0.55/lovehim/__main__.py
--rwxr-xr-x   0 gera       (501) staff       (20)      899 2023-04-21 08:08:39.000000 lovehim-0.55/lovehim/get_verse.py
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:09:58.335057 lovehim-0.55/lovehim.egg-info/
--rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:09:58.000000 lovehim-0.55/lovehim.egg-info/PKG-INFO
--rw-r--r--   0 gera       (501) staff       (20)      257 2023-04-21 08:09:58.000000 lovehim-0.55/lovehim.egg-info/SOURCES.txt
--rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 08:09:58.000000 lovehim-0.55/lovehim.egg-info/dependency_links.txt
--rw-r--r--   0 gera       (501) staff       (20)       51 2023-04-21 08:09:58.000000 lovehim-0.55/lovehim.egg-info/entry_points.txt
--rw-r--r--   0 gera       (501) staff       (20)       16 2023-04-21 08:09:58.000000 lovehim-0.55/lovehim.egg-info/requires.txt
--rw-r--r--   0 gera       (501) staff       (20)        8 2023-04-21 08:09:58.000000 lovehim-0.55/lovehim.egg-info/top_level.txt
--rw-r--r--   0 gera       (501) staff       (20)       38 2023-04-21 08:09:58.335383 lovehim-0.55/setup.cfg
--rw-r--r--   0 gera       (501) staff       (20)      306 2023-04-21 08:09:51.000000 lovehim-0.55/setup.py
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:12:34.829381 lovehim-0.56/
+-rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:12:34.829217 lovehim-0.56/PKG-INFO
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:12:34.828220 lovehim-0.56/lovehim/
+-rw-r--r--   0 gera       (501) staff       (20)       59 2023-04-21 06:29:58.000000 lovehim-0.56/lovehim/__init__.py
+-rw-r--r--   0 gera       (501) staff       (20)      741 2023-04-21 08:12:24.000000 lovehim-0.56/lovehim/__main__.py
+-rwxr-xr-x   0 gera       (501) staff       (20)      899 2023-04-21 08:11:21.000000 lovehim-0.56/lovehim/get_verse.py
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:12:34.829021 lovehim-0.56/lovehim.egg-info/
+-rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:12:34.000000 lovehim-0.56/lovehim.egg-info/PKG-INFO
+-rw-r--r--   0 gera       (501) staff       (20)      257 2023-04-21 08:12:34.000000 lovehim-0.56/lovehim.egg-info/SOURCES.txt
+-rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 08:12:34.000000 lovehim-0.56/lovehim.egg-info/dependency_links.txt
+-rw-r--r--   0 gera       (501) staff       (20)       51 2023-04-21 08:12:34.000000 lovehim-0.56/lovehim.egg-info/entry_points.txt
+-rw-r--r--   0 gera       (501) staff       (20)       16 2023-04-21 08:12:34.000000 lovehim-0.56/lovehim.egg-info/requires.txt
+-rw-r--r--   0 gera       (501) staff       (20)        8 2023-04-21 08:12:34.000000 lovehim-0.56/lovehim.egg-info/top_level.txt
+-rw-r--r--   0 gera       (501) staff       (20)       38 2023-04-21 08:12:34.829423 lovehim-0.56/setup.cfg
+-rw-r--r--   0 gera       (501) staff       (20)      306 2023-04-21 08:12:28.000000 lovehim-0.56/setup.py
```

### Comparing `lovehim-0.55/lovehim/__main__.py` & `lovehim-0.56/lovehim/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 
 import argparse
 import openai
 from .get_verse import generate_verse
 
 # Set up the OpenAI API key
-openai.api_key = "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"
+openai.api_key = "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"
 
 # Parse the command-line arguments
 parser = argparse.ArgumentParser(description='Get a Bible verse based on a topic')
 parser.add_argument('topic', nargs='+', help='the topic you want the verse to be about')
 args = parser.parse_args()
 
 # Call the generate_verse function with the user-specified topic
```

### Comparing `lovehim-0.55/lovehim/get_verse.py` & `lovehim-0.56/lovehim/get_verse.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import openai
 import argparse
 
 # Set up the OpenAI API key
-openai.api_key = "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"
+openai.api_key = "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"
 
 # Define the function to generate a Bible verse based on a topic
 def generate_verse(topic):
     prompt = f"Generate a Bible verse about {topic}"
     response = openai.Completion.create(
         engine="text-davinci-003",
         prompt=prompt,
```

