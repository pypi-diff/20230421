# Comparing `tmp/lovehim-0.53.tar.gz` & `tmp/lovehim-0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lovehim-0.53.tar", last modified: Fri Apr 21 08:06:06 2023, max compression
+gzip compressed data, was "lovehim-0.54.tar", last modified: Fri Apr 21 08:06:57 2023, max compression
```

## Comparing `lovehim-0.53.tar` & `lovehim-0.54.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:06:06.117058 lovehim-0.53/
--rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:06:06.116876 lovehim-0.53/PKG-INFO
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:06:06.115891 lovehim-0.53/lovehim/
--rw-r--r--   0 gera       (501) staff       (20)       59 2023-04-21 06:29:58.000000 lovehim-0.53/lovehim/__init__.py
--rw-r--r--   0 gera       (501) staff       (20)      580 2023-04-21 08:05:53.000000 lovehim-0.53/lovehim/__main__.py
--rwxr-xr-x   0 gera       (501) staff       (20)      899 2023-04-21 08:05:02.000000 lovehim-0.53/lovehim/get_verse.py
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:06:06.116665 lovehim-0.53/lovehim.egg-info/
--rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:06:06.000000 lovehim-0.53/lovehim.egg-info/PKG-INFO
--rw-r--r--   0 gera       (501) staff       (20)      257 2023-04-21 08:06:06.000000 lovehim-0.53/lovehim.egg-info/SOURCES.txt
--rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 08:06:06.000000 lovehim-0.53/lovehim.egg-info/dependency_links.txt
--rw-r--r--   0 gera       (501) staff       (20)       51 2023-04-21 08:06:06.000000 lovehim-0.53/lovehim.egg-info/entry_points.txt
--rw-r--r--   0 gera       (501) staff       (20)       16 2023-04-21 08:06:06.000000 lovehim-0.53/lovehim.egg-info/requires.txt
--rw-r--r--   0 gera       (501) staff       (20)        8 2023-04-21 08:06:06.000000 lovehim-0.53/lovehim.egg-info/top_level.txt
--rw-r--r--   0 gera       (501) staff       (20)       38 2023-04-21 08:06:06.117107 lovehim-0.53/setup.cfg
--rw-r--r--   0 gera       (501) staff       (20)      306 2023-04-21 08:05:43.000000 lovehim-0.53/setup.py
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:06:57.518827 lovehim-0.54/
+-rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:06:57.518715 lovehim-0.54/PKG-INFO
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:06:57.517892 lovehim-0.54/lovehim/
+-rw-r--r--   0 gera       (501) staff       (20)       59 2023-04-21 06:29:58.000000 lovehim-0.54/lovehim/__init__.py
+-rw-r--r--   0 gera       (501) staff       (20)      580 2023-04-21 08:05:53.000000 lovehim-0.54/lovehim/__main__.py
+-rwxr-xr-x   0 gera       (501) staff       (20)      899 2023-04-21 08:06:46.000000 lovehim-0.54/lovehim/get_verse.py
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 08:06:57.518553 lovehim-0.54/lovehim.egg-info/
+-rw-r--r--   0 gera       (501) staff       (20)       50 2023-04-21 08:06:57.000000 lovehim-0.54/lovehim.egg-info/PKG-INFO
+-rw-r--r--   0 gera       (501) staff       (20)      257 2023-04-21 08:06:57.000000 lovehim-0.54/lovehim.egg-info/SOURCES.txt
+-rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 08:06:57.000000 lovehim-0.54/lovehim.egg-info/dependency_links.txt
+-rw-r--r--   0 gera       (501) staff       (20)       51 2023-04-21 08:06:57.000000 lovehim-0.54/lovehim.egg-info/entry_points.txt
+-rw-r--r--   0 gera       (501) staff       (20)       16 2023-04-21 08:06:57.000000 lovehim-0.54/lovehim.egg-info/requires.txt
+-rw-r--r--   0 gera       (501) staff       (20)        8 2023-04-21 08:06:57.000000 lovehim-0.54/lovehim.egg-info/top_level.txt
+-rw-r--r--   0 gera       (501) staff       (20)       38 2023-04-21 08:06:57.518862 lovehim-0.54/setup.cfg
+-rw-r--r--   0 gera       (501) staff       (20)      306 2023-04-21 08:06:51.000000 lovehim-0.54/setup.py
```

### Comparing `lovehim-0.53/lovehim/__main__.py` & `lovehim-0.54/lovehim/__main__.py`

 * *Files identical despite different names*

### Comparing `lovehim-0.53/lovehim/get_verse.py` & `lovehim-0.54/lovehim/get_verse.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         max_tokens=50,
         n=1,
         stop=None,
         temperature=0.5,
         presence_penalty=0.5,
     )
     verse = response.choices[0].text.strip()
-    return verse
+    print(verse)
 
 def main():
     parser = argparse.ArgumentParser(description='Get a Bible verse based on a topic')
     parser.add_argument('topic', nargs='+', help='the topic you want the verse to be about')
     args = parser.parse_args()
     topic = ' '.join(args.topic)
     verse = generate_verse(topic)
```

