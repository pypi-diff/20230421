# Comparing `tmp/lovehim-0.4.tar.gz` & `tmp/lovehim-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lovehim-0.4.tar", last modified: Fri Apr 21 07:46:31 2023, max compression
+gzip compressed data, was "lovehim-0.5.tar", last modified: Fri Apr 21 07:49:25 2023, max compression
```

## Comparing `lovehim-0.4.tar` & `lovehim-0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 07:46:31.676030 lovehim-0.4/
--rw-r--r--   0 gera       (501) staff       (20)       49 2023-04-21 07:46:31.675858 lovehim-0.4/PKG-INFO
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 07:46:31.674890 lovehim-0.4/lovehim/
--rw-r--r--   0 gera       (501) staff       (20)       59 2023-04-21 06:29:58.000000 lovehim-0.4/lovehim/__init__.py
--rwxr-xr-x   0 gera       (501) staff       (20)      870 2023-04-21 07:45:13.000000 lovehim-0.4/lovehim/get_verse.py
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 07:46:31.675661 lovehim-0.4/lovehim.egg-info/
--rw-r--r--   0 gera       (501) staff       (20)       49 2023-04-21 07:46:31.000000 lovehim-0.4/lovehim.egg-info/PKG-INFO
--rw-r--r--   0 gera       (501) staff       (20)      237 2023-04-21 07:46:31.000000 lovehim-0.4/lovehim.egg-info/SOURCES.txt
--rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 07:46:31.000000 lovehim-0.4/lovehim.egg-info/dependency_links.txt
--rw-r--r--   0 gera       (501) staff       (20)       51 2023-04-21 07:46:31.000000 lovehim-0.4/lovehim.egg-info/entry_points.txt
--rw-r--r--   0 gera       (501) staff       (20)       16 2023-04-21 07:46:31.000000 lovehim-0.4/lovehim.egg-info/requires.txt
--rw-r--r--   0 gera       (501) staff       (20)        8 2023-04-21 07:46:31.000000 lovehim-0.4/lovehim.egg-info/top_level.txt
--rw-r--r--   0 gera       (501) staff       (20)       38 2023-04-21 07:46:31.676080 lovehim-0.4/setup.cfg
--rw-r--r--   0 gera       (501) staff       (20)      305 2023-04-21 07:46:23.000000 lovehim-0.4/setup.py
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 07:49:25.262726 lovehim-0.5/
+-rw-r--r--   0 gera       (501) staff       (20)       49 2023-04-21 07:49:25.262617 lovehim-0.5/PKG-INFO
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 07:49:25.261680 lovehim-0.5/lovehim/
+-rw-r--r--   0 gera       (501) staff       (20)       59 2023-04-21 06:29:58.000000 lovehim-0.5/lovehim/__init__.py
+-rw-r--r--   0 gera       (501) staff       (20)      555 2023-04-21 07:48:23.000000 lovehim-0.5/lovehim/__main__.py
+-rwxr-xr-x   0 gera       (501) staff       (20)      870 2023-04-21 07:48:43.000000 lovehim-0.5/lovehim/get_verse.py
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 07:49:25.262458 lovehim-0.5/lovehim.egg-info/
+-rw-r--r--   0 gera       (501) staff       (20)       49 2023-04-21 07:49:25.000000 lovehim-0.5/lovehim.egg-info/PKG-INFO
+-rw-r--r--   0 gera       (501) staff       (20)      257 2023-04-21 07:49:25.000000 lovehim-0.5/lovehim.egg-info/SOURCES.txt
+-rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 07:49:25.000000 lovehim-0.5/lovehim.egg-info/dependency_links.txt
+-rw-r--r--   0 gera       (501) staff       (20)       51 2023-04-21 07:49:25.000000 lovehim-0.5/lovehim.egg-info/entry_points.txt
+-rw-r--r--   0 gera       (501) staff       (20)       16 2023-04-21 07:49:25.000000 lovehim-0.5/lovehim.egg-info/requires.txt
+-rw-r--r--   0 gera       (501) staff       (20)        8 2023-04-21 07:49:25.000000 lovehim-0.5/lovehim.egg-info/top_level.txt
+-rw-r--r--   0 gera       (501) staff       (20)       38 2023-04-21 07:49:25.262760 lovehim-0.5/setup.cfg
+-rw-r--r--   0 gera       (501) staff       (20)      305 2023-04-21 07:49:18.000000 lovehim-0.5/setup.py
```

### Comparing `lovehim-0.4/lovehim/get_verse.py` & `lovehim-0.5/lovehim/get_verse.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,11 +20,11 @@
     return verse
 
 def main():
     parser = argparse.ArgumentParser(description='Get a Bible verse based on a topic')
     parser.add_argument('topic', type=str, help='the topic you want the verse to be about')
     args = parser.parse_args()
     verse = generate_verse(args.topic)
-    print(verse)
+    return verse
 
 if __name__ == '__main__':
     main()
```

