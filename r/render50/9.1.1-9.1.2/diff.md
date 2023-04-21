# Comparing `tmp/render50-9.1.1.tar.gz` & `tmp/render50-9.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render50-9.1.1.tar", last modified: Fri Apr  7 21:32:34 2023, max compression
+gzip compressed data, was "render50-9.1.2.tar", last modified: Fri Apr 21 14:08:58 2023, max compression
```

## Comparing `render50-9.1.1.tar` & `render50-9.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:32:34.235087 render50-9.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-07 21:32:13.000000 render50-9.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-07 21:32:34.235087 render50-9.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-07 21:32:13.000000 render50-9.1.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    20439 2023-04-07 21:32:13.000000 render50-9.1.1/render50
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:32:34.235087 render50-9.1.1/render50.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-07 21:32:34.000000 render50-9.1.1/render50.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-07 21:32:34.000000 render50-9.1.1/render50.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:32:34.000000 render50-9.1.1/render50.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-07 21:32:34.000000 render50-9.1.1/render50.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:32:34.000000 render50-9.1.1/render50.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 21:32:34.235087 render50-9.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-07 21:32:13.000000 render50-9.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:08:58.058109 render50-9.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 14:08:37.000000 render50-9.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-21 14:08:58.058109 render50-9.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-21 14:08:37.000000 render50-9.1.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20439 2023-04-21 14:08:37.000000 render50-9.1.2/render50
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:08:58.058109 render50-9.1.2/render50.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-21 14:08:58.000000 render50-9.1.2/render50.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-21 14:08:58.000000 render50-9.1.2/render50.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:08:58.000000 render50-9.1.2/render50.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-21 14:08:58.000000 render50-9.1.2/render50.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:08:58.000000 render50-9.1.2/render50.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:08:58.058109 render50-9.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-21 14:08:37.000000 render50-9.1.2/setup.py
```

### Comparing `render50-9.1.1/LICENSE` & `render50-9.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `render50-9.1.1/render50` & `render50-9.1.2/render50`

 * *Files identical despite different names*

### Comparing `render50-9.1.1/setup.py` & `render50-9.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     classifiers=[
         "Intended Audience :: Education",
         "Programming Language :: Python :: 3",
         "Topic :: Education",
         "Topic :: Utilities"
     ],
     description="This is render50, with which you can render source code as PDFs.",
-    install_requires=["backports.shutil_get_terminal_size", "backports.shutil_which", "braceexpand", "beautifulsoup4", "natsort", "Pygments>=2.7.1", "PyPDF2", "requests", "six>=1.10.0", "termcolor", "WeasyPrint"],
+    install_requires=["backports.shutil_get_terminal_size", "backports.shutil_which", "braceexpand", "beautifulsoup4", "natsort", "Pygments>=2.7.1", "PyPDF2==2.12.1", "requests", "six>=1.10.0", "termcolor", "WeasyPrint"],
     keywords=["render", "render50"],
     license="GPLv3",
     long_description_content_type="text/markdown",
     name="render50",
     python_requires=">=3.6",
     scripts=["render50"],
     url="https://github.com/cs50/render50",
-    version="9.1.1"
+    version="9.1.2"
 )
```

