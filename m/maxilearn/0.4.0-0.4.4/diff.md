# Comparing `tmp/maxilearn-0.4.0.tar.gz` & `tmp/maxilearn-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxilearn-0.4.0.tar", last modified: Fri Apr 21 16:14:33 2023, max compression
+gzip compressed data, was "maxilearn-0.4.4.tar", last modified: Fri Apr 21 16:19:51 2023, max compression
```

## Comparing `maxilearn-0.4.0.tar` & `maxilearn-0.4.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 16:14:33.387043 maxilearn-0.4.0/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-0.4.0/LICENSE
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      243 2023-04-21 16:14:33.386851 maxilearn-0.4.0/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-0.4.0/README.md
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 16:14:33.386598 maxilearn-0.4.0/maxilearn.egg-info/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      243 2023-04-21 16:14:33.000000 maxilearn-0.4.0/maxilearn.egg-info/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      190 2023-04-21 16:14:33.000000 maxilearn-0.4.0/maxilearn.egg-info/SOURCES.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 16:14:33.000000 maxilearn-0.4.0/maxilearn.egg-info/dependency_links.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       50 2023-04-21 16:14:33.000000 maxilearn-0.4.0/maxilearn.egg-info/requires.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 16:14:33.000000 maxilearn-0.4.0/maxilearn.egg-info/top_level.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       38 2023-04-21 16:14:33.387102 maxilearn-0.4.0/setup.cfg
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      442 2023-04-21 16:14:15.000000 maxilearn-0.4.0/setup.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 16:19:51.755892 maxilearn-0.4.4/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-0.4.4/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      243 2023-04-21 16:19:51.755723 maxilearn-0.4.4/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-0.4.4/README.md
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 16:19:51.755501 maxilearn-0.4.4/maxilearn.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      243 2023-04-21 16:19:51.000000 maxilearn-0.4.4/maxilearn.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      190 2023-04-21 16:19:51.000000 maxilearn-0.4.4/maxilearn.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 16:19:51.000000 maxilearn-0.4.4/maxilearn.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       42 2023-04-21 16:19:51.000000 maxilearn-0.4.4/maxilearn.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 16:19:51.000000 maxilearn-0.4.4/maxilearn.egg-info/top_level.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       38 2023-04-21 16:19:51.755952 maxilearn-0.4.4/setup.cfg
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      423 2023-04-21 16:19:17.000000 maxilearn-0.4.4/setup.py
```

### Comparing `maxilearn-0.4.0/LICENSE` & `maxilearn-0.4.4/LICENSE`

 * *Files identical despite different names*

