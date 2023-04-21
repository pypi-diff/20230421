# Comparing `tmp/maxilearn-0.1.9.tar.gz` & `tmp/maxilearn-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxilearn-0.1.9.tar", last modified: Fri Apr 21 15:54:18 2023, max compression
+gzip compressed data, was "maxilearn-0.3.9.tar", last modified: Fri Apr 21 16:08:21 2023, max compression
```

## Comparing `maxilearn-0.1.9.tar` & `maxilearn-0.3.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 15:54:18.824537 maxilearn-0.1.9/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-0.1.9/LICENSE
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      198 2023-04-21 15:54:18.824339 maxilearn-0.1.9/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-0.1.9/README.md
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 15:54:18.824094 maxilearn-0.1.9/maxilearn.egg-info/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      198 2023-04-21 15:54:18.000000 maxilearn-0.1.9/maxilearn.egg-info/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      190 2023-04-21 15:54:18.000000 maxilearn-0.1.9/maxilearn.egg-info/SOURCES.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 15:54:18.000000 maxilearn-0.1.9/maxilearn.egg-info/dependency_links.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       23 2023-04-21 15:54:18.000000 maxilearn-0.1.9/maxilearn.egg-info/requires.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 15:54:18.000000 maxilearn-0.1.9/maxilearn.egg-info/top_level.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       38 2023-04-21 15:54:18.824596 maxilearn-0.1.9/setup.cfg
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      384 2023-04-21 15:54:07.000000 maxilearn-0.1.9/setup.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 16:08:21.766154 maxilearn-0.3.9/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 maxilearn-0.3.9/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      243 2023-04-21 16:08:21.765918 maxilearn-0.3.9/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      268 2023-04-21 15:13:38.000000 maxilearn-0.3.9/README.md
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-21 16:08:21.765600 maxilearn-0.3.9/maxilearn.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      243 2023-04-21 16:08:21.000000 maxilearn-0.3.9/maxilearn.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      190 2023-04-21 16:08:21.000000 maxilearn-0.3.9/maxilearn.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 16:08:21.000000 maxilearn-0.3.9/maxilearn.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       55 2023-04-21 16:08:21.000000 maxilearn-0.3.9/maxilearn.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-21 16:08:21.000000 maxilearn-0.3.9/maxilearn.egg-info/top_level.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       38 2023-04-21 16:08:21.766221 maxilearn-0.3.9/setup.cfg
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      447 2023-04-21 16:04:52.000000 maxilearn-0.3.9/setup.py
```

### Comparing `maxilearn-0.1.9/LICENSE` & `maxilearn-0.3.9/LICENSE`

 * *Files identical despite different names*

