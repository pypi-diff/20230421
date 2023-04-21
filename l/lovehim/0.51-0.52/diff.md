# Comparing `tmp/lovehim-0.51.tar.gz` & `tmp/lovehim-0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lovehim-0.51.tar", last modified: Fri Apr 21 08:00:46 2023, max compression
+gzip compressed data, was "lovehim-0.52.tar", last modified: Fri Apr 21 08:03:03 2023, max compression
```

## Comparing `lovehim-0.51.tar` & `lovehim-0.52.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:00:46.630122 lovehim-0.51/
--rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:00:46.630013 lovehim-0.51/PKG-INFO
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:00:46.629102 lovehim-0.51/lovehim/
--rw-r--r--   0 gera       (501) staff       (20)       59 2023-04-21 06:29:58.000000 lovehim-0.51/lovehim/__init__.py
--rw-r--r--   0 gera       (501) staff       (20)      555 2023-04-21 07:48:23.000000 lovehim-0.51/lovehim/__main__.py
--rwxr-xr-x   0 gera       (501) staff       (20)      882 2023-04-21 08:00:18.000000 lovehim-0.51/lovehim/get_verse.py
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:00:46.629843 lovehim-0.51/lovehim.egg-info/
--rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:00:46.000000 lovehim-0.51/lovehim.egg-info/PKG-INFO
--rw-r--r--   0 gera       (501) staff       (20)      257 2023-04-21 08:00:46.000000 lovehim-0.51/lovehim.egg-info/SOURCES.txt
--rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 08:00:46.000000 lovehim-0.51/lovehim.egg-info/dependency_links.txt
--rw-r--r--   0 gera       (501) staff       (20)       51 2023-04-21 08:00:46.000000 lovehim-0.51/lovehim.egg-info/entry_points.txt
--rw-r--r--   0 gera       (501) staff       (20)       16 2023-04-21 08:00:46.000000 lovehim-0.51/lovehim.egg-info/requires.txt
--rw-r--r--   0 gera       (501) staff       (20)        8 2023-04-21 08:00:46.000000 lovehim-0.51/lovehim.egg-info/top_level.txt
--rw-r--r--   0 gera       (501) staff       (20)       38 2023-04-21 08:00:46.630164 lovehim-0.51/setup.cfg
--rw-r--r--   0 gera       (501) staff       (20)      306 2023-04-21 08:00:25.000000 lovehim-0.51/setup.py
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:03:03.801310 lovehim-0.52/
+-rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:03:03.801199 lovehim-0.52/PKG-INFO
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:03:03.800279 lovehim-0.52/lovehim/
+-rw-r--r--   0 gera       (501) staff       (20)       59 2023-04-21 06:29:58.000000 lovehim-0.52/lovehim/__init__.py
+-rw-r--r--   0 gera       (501) staff       (20)      580 2023-04-21 08:02:48.000000 lovehim-0.52/lovehim/__main__.py
+-rwxr-xr-x   0 gera       (501) staff       (20)      882 2023-04-21 08:00:18.000000 lovehim-0.52/lovehim/get_verse.py
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:03:03.801044 lovehim-0.52/lovehim.egg-info/
+-rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:03:03.000000 lovehim-0.52/lovehim.egg-info/PKG-INFO
+-rw-r--r--   0 gera       (501) staff       (20)      257 2023-04-21 08:03:03.000000 lovehim-0.52/lovehim.egg-info/SOURCES.txt
+-rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 08:03:03.000000 lovehim-0.52/lovehim.egg-info/dependency_links.txt
+-rw-r--r--   0 gera       (501) staff       (20)       51 2023-04-21 08:03:03.000000 lovehim-0.52/lovehim.egg-info/entry_points.txt
+-rw-r--r--   0 gera       (501) staff       (20)       16 2023-04-21 08:03:03.000000 lovehim-0.52/lovehim.egg-info/requires.txt
+-rw-r--r--   0 gera       (501) staff       (20)        8 2023-04-21 08:03:03.000000 lovehim-0.52/lovehim.egg-info/top_level.txt
+-rw-r--r--   0 gera       (501) staff       (20)       38 2023-04-21 08:03:03.801344 lovehim-0.52/setup.cfg
+-rw-r--r--   0 gera       (501) staff       (20)      306 2023-04-21 08:02:54.000000 lovehim-0.52/setup.py
```

### Comparing `lovehim-0.51/lovehim/__main__.py` & `lovehim-0.52/lovehim/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from .get_verse import generate_verse
 
 # Set up the OpenAI API key
 openai.api_key = "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"
 
 # Parse the command-line arguments
 parser = argparse.ArgumentParser(description='Get a Bible verse based on a topic')
-parser.add_argument('topic', type=str, help='the topic you want the verse to be about')
+parser.add_argument('topic', nargs='+', help='the topic you want the verse to be about')
 args = parser.parse_args()
 
 # Call the generate_verse function with the user-specified topic
-verse = generate_verse(args.topic)
+topic = ' '.join(args.topic)
+verse = generate_verse(topic)
 
 # Print out the resulting Bible verse
 print(verse)
```

### Comparing `lovehim-0.51/lovehim/get_verse.py` & `lovehim-0.52/lovehim/get_verse.py`

 * *Files identical despite different names*

