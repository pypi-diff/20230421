# Comparing `tmp/napari-cilia-beating-frequency-0.1.tar.gz` & `tmp/napari-cilia-beating-frequency-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-cilia-beating-frequency-0.1.tar", last modified: Wed Jul 13 08:37:42 2022, max compression
+gzip compressed data, was "napari-cilia-beating-frequency-0.2.tar", last modified: Fri Apr 21 13:19:05 2023, max compression
```

## Comparing `napari-cilia-beating-frequency-0.1.tar` & `napari-cilia-beating-frequency-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 em         (501) staff       (20)        0 2022-07-13 08:37:42.841282 napari-cilia-beating-frequency-0.1/
--rw-r--r--   0 em         (501) staff       (20)      147 2022-05-23 15:00:43.000000 napari-cilia-beating-frequency-0.1/.editorconfig
--rw-r--r--   0 em         (501) staff       (20)       32 2022-07-13 08:36:02.000000 napari-cilia-beating-frequency-0.1/.gitignore
--rw-r--r--   0 em         (501) staff       (20)      475 2022-07-13 08:37:42.840958 napari-cilia-beating-frequency-0.1/PKG-INFO
--rw-r--r--   0 em         (501) staff       (20)       64 2022-05-23 15:30:02.000000 napari-cilia-beating-frequency-0.1/README.md
--rw-r--r--   0 em         (501) staff       (20)      927 2022-07-13 08:25:52.000000 napari-cilia-beating-frequency-0.1/pyproject.toml
--rw-r--r--   0 em         (501) staff       (20)       38 2022-07-13 08:37:42.841365 napari-cilia-beating-frequency-0.1/setup.cfg
--rw-r--r--   0 em         (501) staff       (20)       38 2022-05-23 15:01:40.000000 napari-cilia-beating-frequency-0.1/setup.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2022-07-13 08:37:42.837149 napari-cilia-beating-frequency-0.1/src/
-drwxr-xr-x   0 em         (501) staff       (20)        0 2022-07-13 08:37:42.838885 napari-cilia-beating-frequency-0.1/src/napari_cilia_beating_frequency/
--rw-r--r--   0 em         (501) staff       (20)     3279 2022-07-13 08:29:48.000000 napari-cilia-beating-frequency-0.1/src/napari_cilia_beating_frequency/__init__.py
--rw-r--r--   0 em         (501) staff       (20)      382 2022-05-24 09:32:18.000000 napari-cilia-beating-frequency-0.1/src/napari_cilia_beating_frequency/napari.toml
-drwxr-xr-x   0 em         (501) staff       (20)        0 2022-07-13 08:37:42.840557 napari-cilia-beating-frequency-0.1/src/napari_cilia_beating_frequency.egg-info/
--rw-r--r--   0 em         (501) staff       (20)      475 2022-07-13 08:37:42.000000 napari-cilia-beating-frequency-0.1/src/napari_cilia_beating_frequency.egg-info/PKG-INFO
--rw-r--r--   0 em         (501) staff       (20)      502 2022-07-13 08:37:42.000000 napari-cilia-beating-frequency-0.1/src/napari_cilia_beating_frequency.egg-info/SOURCES.txt
--rw-r--r--   0 em         (501) staff       (20)        1 2022-07-13 08:37:42.000000 napari-cilia-beating-frequency-0.1/src/napari_cilia_beating_frequency.egg-info/dependency_links.txt
--rw-r--r--   0 em         (501) staff       (20)       94 2022-07-13 08:37:42.000000 napari-cilia-beating-frequency-0.1/src/napari_cilia_beating_frequency.egg-info/entry_points.txt
--rw-r--r--   0 em         (501) staff       (20)       44 2022-07-13 08:37:42.000000 napari-cilia-beating-frequency-0.1/src/napari_cilia_beating_frequency.egg-info/requires.txt
--rw-r--r--   0 em         (501) staff       (20)       31 2022-07-13 08:37:42.000000 napari-cilia-beating-frequency-0.1/src/napari_cilia_beating_frequency.egg-info/top_level.txt
+drwxr-xr-x   0 em         (501) staff       (20)        0 2023-04-21 13:19:05.588112 napari-cilia-beating-frequency-0.2/
+-rw-r--r--   0 em         (501) staff       (20)      147 2022-05-23 15:00:43.000000 napari-cilia-beating-frequency-0.2/.editorconfig
+-rw-r--r--   0 em         (501) staff       (20)       32 2022-07-13 08:36:02.000000 napari-cilia-beating-frequency-0.2/.gitignore
+-rw-r--r--   0 em         (501) staff       (20)      443 2023-04-21 13:19:05.587673 napari-cilia-beating-frequency-0.2/PKG-INFO
+-rw-r--r--   0 em         (501) staff       (20)       64 2022-05-23 15:30:02.000000 napari-cilia-beating-frequency-0.2/README.md
+-rw-r--r--   0 em         (501) staff       (20)      904 2023-04-21 13:13:10.000000 napari-cilia-beating-frequency-0.2/pyproject.toml
+-rw-r--r--   0 em         (501) staff       (20)       38 2023-04-21 13:19:05.588206 napari-cilia-beating-frequency-0.2/setup.cfg
+-rw-r--r--   0 em         (501) staff       (20)       38 2022-05-23 15:01:40.000000 napari-cilia-beating-frequency-0.2/setup.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2023-04-21 13:19:05.581013 napari-cilia-beating-frequency-0.2/src/
+drwxr-xr-x   0 em         (501) staff       (20)        0 2023-04-21 13:19:05.584536 napari-cilia-beating-frequency-0.2/src/napari_cilia_beating_frequency/
+-rw-r--r--   0 em         (501) staff       (20)     3279 2022-07-13 08:29:48.000000 napari-cilia-beating-frequency-0.2/src/napari_cilia_beating_frequency/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)      382 2022-05-24 09:32:18.000000 napari-cilia-beating-frequency-0.2/src/napari_cilia_beating_frequency/napari.toml
+drwxr-xr-x   0 em         (501) staff       (20)        0 2023-04-21 13:19:05.587163 napari-cilia-beating-frequency-0.2/src/napari_cilia_beating_frequency.egg-info/
+-rw-r--r--   0 em         (501) staff       (20)      443 2023-04-21 13:19:05.000000 napari-cilia-beating-frequency-0.2/src/napari_cilia_beating_frequency.egg-info/PKG-INFO
+-rw-r--r--   0 em         (501) staff       (20)      502 2023-04-21 13:19:05.000000 napari-cilia-beating-frequency-0.2/src/napari_cilia_beating_frequency.egg-info/SOURCES.txt
+-rw-r--r--   0 em         (501) staff       (20)        1 2023-04-21 13:19:05.000000 napari-cilia-beating-frequency-0.2/src/napari_cilia_beating_frequency.egg-info/dependency_links.txt
+-rw-r--r--   0 em         (501) staff       (20)       94 2023-04-21 13:19:05.000000 napari-cilia-beating-frequency-0.2/src/napari_cilia_beating_frequency.egg-info/entry_points.txt
+-rw-r--r--   0 em         (501) staff       (20)       44 2023-04-21 13:19:05.000000 napari-cilia-beating-frequency-0.2/src/napari_cilia_beating_frequency.egg-info/requires.txt
+-rw-r--r--   0 em         (501) staff       (20)       31 2023-04-21 13:19:05.000000 napari-cilia-beating-frequency-0.2/src/napari_cilia_beating_frequency.egg-info/top_level.txt
```

### Comparing `napari-cilia-beating-frequency-0.1/pyproject.toml` & `napari-cilia-beating-frequency-0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = "Cilia beating frequency detection"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
     {name = "Emil Melnikov", email = "emilmelnikov@gmail.com"},
 ]
-classifiers = ["Development Status :: 2 - Pre-Alpha", "Framework :: napari"]
+classifiers = ["Development Status :: 2 - Pre-Alpha"]
 dependencies = [
     "magicgui",
     "napari[all]",
     "numpy>=1.20",
     "qtpy",
     "scipy",
 ]
```

### Comparing `napari-cilia-beating-frequency-0.1/src/napari_cilia_beating_frequency/__init__.py` & `napari-cilia-beating-frequency-0.2/src/napari_cilia_beating_frequency/__init__.py`

 * *Files identical despite different names*

