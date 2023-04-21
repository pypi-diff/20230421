# Comparing `tmp/maxilearn-0.4.5.tar.gz` & `tmp/maxilearn-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxilearn-0.4.5.tar", last modified: Fri Apr 21 16:29:51 2023, max compression
+gzip compressed data, was "maxilearn-0.4.6.tar", last modified: Fri Apr 21 16:33:24 2023, max compression
```

## Comparing `maxilearn-0.4.5.tar` & `maxilearn-0.4.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 16:29:51.617810 maxilearn-0.4.5/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-0.4.5/LICENSE
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      243 2023-04-21 16:29:51.617632 maxilearn-0.4.5/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-0.4.5/README.md
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 16:29:51.617383 maxilearn-0.4.5/maxilearn.egg-info/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      243 2023-04-21 16:29:51.000000 maxilearn-0.4.5/maxilearn.egg-info/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      190 2023-04-21 16:29:51.000000 maxilearn-0.4.5/maxilearn.egg-info/SOURCES.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 16:29:51.000000 maxilearn-0.4.5/maxilearn.egg-info/dependency_links.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       36 2023-04-21 16:29:51.000000 maxilearn-0.4.5/maxilearn.egg-info/requires.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 16:29:51.000000 maxilearn-0.4.5/maxilearn.egg-info/top_level.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       38 2023-04-21 16:29:51.617869 maxilearn-0.4.5/setup.cfg
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      406 2023-04-21 16:29:37.000000 maxilearn-0.4.5/setup.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 16:33:24.606834 maxilearn-0.4.6/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-0.4.6/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      243 2023-04-21 16:33:24.606665 maxilearn-0.4.6/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-0.4.6/README.md
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 16:33:24.606417 maxilearn-0.4.6/maxilearn.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      243 2023-04-21 16:33:24.000000 maxilearn-0.4.6/maxilearn.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      190 2023-04-21 16:33:24.000000 maxilearn-0.4.6/maxilearn.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 16:33:24.000000 maxilearn-0.4.6/maxilearn.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       36 2023-04-21 16:33:24.000000 maxilearn-0.4.6/maxilearn.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 16:33:24.000000 maxilearn-0.4.6/maxilearn.egg-info/top_level.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       38 2023-04-21 16:33:24.609081 maxilearn-0.4.6/setup.cfg
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      406 2023-04-21 16:33:15.000000 maxilearn-0.4.6/setup.py
```

### Comparing `maxilearn-0.4.5/LICENSE` & `maxilearn-0.4.6/LICENSE`

 * *Files identical despite different names*

