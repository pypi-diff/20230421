# Comparing `tmp/lovehim-0.3.tar.gz` & `tmp/lovehim-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lovehim-0.3.tar", last modified: Fri Apr 21 07:37:45 2023, max compression
+gzip compressed data, was "lovehim-0.4.tar", last modified: Fri Apr 21 07:46:31 2023, max compression
```

## Comparing `lovehim-0.3.tar` & `lovehim-0.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 07:37:45.752530 lovehim-0.3/
--rw-r--r--   0 gera       (501) staff       (20)       49 2023-04-21 07:37:45.752392 lovehim-0.3/PKG-INFO
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 07:37:45.751422 lovehim-0.3/lovehim/
--rw-r--r--   0 gera       (501) staff       (20)       59 2023-04-21 06:29:58.000000 lovehim-0.3/lovehim/__init__.py
--rw-r--r--   0 gera       (501) staff       (20)      555 2023-04-21 07:32:35.000000 lovehim-0.3/lovehim/__main__.py
--rwxr-xr-x   0 gera       (501) staff       (20)      889 2023-04-21 07:35:07.000000 lovehim-0.3/lovehim/get_verse.py
-drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 07:37:45.752223 lovehim-0.3/lovehim.egg-info/
--rw-r--r--   0 gera       (501) staff       (20)       49 2023-04-21 07:37:45.000000 lovehim-0.3/lovehim.egg-info/PKG-INFO
--rw-r--r--   0 gera       (501) staff       (20)      257 2023-04-21 07:37:45.000000 lovehim-0.3/lovehim.egg-info/SOURCES.txt
--rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 07:37:45.000000 lovehim-0.3/lovehim.egg-info/dependency_links.txt
--rw-r--r--   0 gera       (501) staff       (20)       51 2023-04-21 07:37:45.000000 lovehim-0.3/lovehim.egg-info/entry_points.txt
--rw-r--r--   0 gera       (501) staff       (20)       16 2023-04-21 07:37:45.000000 lovehim-0.3/lovehim.egg-info/requires.txt
--rw-r--r--   0 gera       (501) staff       (20)        8 2023-04-21 07:37:45.000000 lovehim-0.3/lovehim.egg-info/top_level.txt
--rw-r--r--   0 gera       (501) staff       (20)       38 2023-04-21 07:37:45.752572 lovehim-0.3/setup.cfg
--rw-r--r--   0 gera       (501) staff       (20)      305 2023-04-21 07:36:10.000000 lovehim-0.3/setup.py
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 07:46:31.676030 lovehim-0.4/
+-rw-r--r--   0 gera       (501) staff       (20)       49 2023-04-21 07:46:31.675858 lovehim-0.4/PKG-INFO
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 07:46:31.674890 lovehim-0.4/lovehim/
+-rw-r--r--   0 gera       (501) staff       (20)       59 2023-04-21 06:29:58.000000 lovehim-0.4/lovehim/__init__.py
+-rwxr-xr-x   0 gera       (501) staff       (20)      870 2023-04-21 07:45:13.000000 lovehim-0.4/lovehim/get_verse.py
+drwxr-xr-x   0 gera       (501) staff       (20)        0 2023-04-21 07:46:31.675661 lovehim-0.4/lovehim.egg-info/
+-rw-r--r--   0 gera       (501) staff       (20)       49 2023-04-21 07:46:31.000000 lovehim-0.4/lovehim.egg-info/PKG-INFO
+-rw-r--r--   0 gera       (501) staff       (20)      237 2023-04-21 07:46:31.000000 lovehim-0.4/lovehim.egg-info/SOURCES.txt
+-rw-r--r--   0 gera       (501) staff       (20)        1 2023-04-21 07:46:31.000000 lovehim-0.4/lovehim.egg-info/dependency_links.txt
+-rw-r--r--   0 gera       (501) staff       (20)       51 2023-04-21 07:46:31.000000 lovehim-0.4/lovehim.egg-info/entry_points.txt
+-rw-r--r--   0 gera       (501) staff       (20)       16 2023-04-21 07:46:31.000000 lovehim-0.4/lovehim.egg-info/requires.txt
+-rw-r--r--   0 gera       (501) staff       (20)        8 2023-04-21 07:46:31.000000 lovehim-0.4/lovehim.egg-info/top_level.txt
+-rw-r--r--   0 gera       (501) staff       (20)       38 2023-04-21 07:46:31.676080 lovehim-0.4/setup.cfg
+-rw-r--r--   0 gera       (501) staff       (20)      305 2023-04-21 07:46:23.000000 lovehim-0.4/setup.py
```

### Comparing `lovehim-0.3/lovehim/get_verse.py` & `lovehim-0.4/lovehim/get_verse.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,16 @@
         stop=None,
         temperature=0.5,
         presence_penalty=0.5,
     )
     verse = response.choices[0].text.strip()
     return verse
 
-# Parse the command-line arguments
-parser = argparse.ArgumentParser(description='Get a Bible verse based on a topic')
-parser.add_argument('topic', type=str, help='the topic you want the verse to be about')
+def main():
+    parser = argparse.ArgumentParser(description='Get a Bible verse based on a topic')
+    parser.add_argument('topic', type=str, help='the topic you want the verse to be about')
+    args = parser.parse_args()
+    verse = generate_verse(args.topic)
+    print(verse)
 
-args = parser.parse_args()
-
-# Call the generate_verse function with the user-specified topic
-verse = generate_verse(args.topic)
+if __name__ == '__main__':
+    main()
```

