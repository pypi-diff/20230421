# Comparing `tmp/asaman-0.2.0.tar.gz` & `tmp/asaman-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asaman-0.2.0.tar", last modified: Sun Apr 16 07:26:03 2023, max compression
+gzip compressed data, was "asaman-0.2.1.tar", last modified: Fri Apr 21 17:23:16 2023, max compression
```

## Comparing `asaman-0.2.0.tar` & `asaman-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      863 2023-03-09 09:29:11.152792 asaman-0.2.0/.github/workflows/github-actions.yml
--rw-r--r--   0        0        0      266 2021-10-05 09:02:57.760675 asaman-0.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1066 2021-10-03 15:53:23.164770 asaman-0.2.0/LICENSE
--rw-r--r--   0        0        0     6961 2023-04-16 07:24:08.410438 asaman-0.2.0/README.md
--rw-r--r--   0        0        0    12131 2023-04-16 07:24:08.410438 asaman-0.2.0/asaman/__init__.py
--rw-r--r--   0        0        0     1380 2023-04-16 07:24:08.411438 asaman-0.2.0/dev-ci.txt
--rw-r--r--   0        0        0      174 2023-04-16 07:24:08.411438 asaman-0.2.0/dev-requirements.in
--rw-r--r--   0        0        0     1390 2023-04-16 07:24:08.411438 asaman-0.2.0/dev-requirements.txt
--rw-r--r--   0        0        0      638 2021-10-05 05:06:13.614201 asaman-0.2.0/docs/Makefile
--rw-r--r--   0        0        0      799 2021-10-05 05:06:13.616201 asaman-0.2.0/docs/make.bat
--rw-r--r--   0        0        0       20 2021-10-05 09:04:05.395133 asaman-0.2.0/docs/requirements.txt
--rw-r--r--   0        0        0     1885 2023-04-16 07:24:08.411438 asaman-0.2.0/docs/source/conf.py
--rw-r--r--   0        0        0      654 2021-10-12 07:09:53.897433 asaman-0.2.0/docs/source/hacking.rst
--rw-r--r--   0        0        0      568 2021-10-13 09:30:04.118485 asaman-0.2.0/docs/source/index.rst
--rw-r--r--   0        0        0      196 2021-10-05 05:15:36.281858 asaman-0.2.0/docs/source/install.rst
--rw-r--r--   0        0        0     4071 2023-03-09 08:59:08.269150 asaman-0.2.0/docs/source/usage.rst
--rw-r--r--   0        0        0      746 2021-10-05 03:18:05.770095 asaman-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      151 2023-04-16 07:24:08.411438 asaman-0.2.0/requirements.in
--rw-r--r--   0        0        0     2467 2023-04-16 07:24:08.411438 asaman-0.2.0/requirements.txt
--rw-r--r--   0        0        0        3 2023-03-09 09:29:11.152792 asaman-0.2.0/test.in
--rw-r--r--   0        0        0      759 2023-03-09 09:29:11.152792 asaman-0.2.0/test.txt
--rw-r--r--   0        0        0       62 2021-10-06 04:36:45.710606 asaman-0.2.0/tests/test_requirements.py
--rw-r--r--   0        0        0     7462 1970-01-01 00:00:00.000000 asaman-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      863 2023-03-09 09:29:11.152792 asaman-0.2.1/.github/workflows/github-actions.yml
+-rw-r--r--   0        0        0      266 2021-10-05 09:02:57.760675 asaman-0.2.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1066 2021-10-03 15:53:23.164770 asaman-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6961 2023-04-16 07:24:08.410438 asaman-0.2.1/README.md
+-rw-r--r--   0        0        0    12131 2023-04-21 17:22:53.348102 asaman-0.2.1/asaman/__init__.py
+-rw-r--r--   0        0        0     1380 2023-04-16 07:24:08.411438 asaman-0.2.1/dev-ci.txt
+-rw-r--r--   0        0        0      174 2023-04-16 07:24:08.411438 asaman-0.2.1/dev-requirements.in
+-rw-r--r--   0        0        0     1390 2023-04-16 07:24:08.411438 asaman-0.2.1/dev-requirements.txt
+-rw-r--r--   0        0        0      638 2021-10-05 05:06:13.614201 asaman-0.2.1/docs/Makefile
+-rw-r--r--   0        0        0      799 2021-10-05 05:06:13.616201 asaman-0.2.1/docs/make.bat
+-rw-r--r--   0        0        0       20 2021-10-05 09:04:05.395133 asaman-0.2.1/docs/requirements.txt
+-rw-r--r--   0        0        0     1885 2023-04-21 17:22:53.349102 asaman-0.2.1/docs/source/conf.py
+-rw-r--r--   0        0        0      654 2021-10-12 07:09:53.897433 asaman-0.2.1/docs/source/hacking.rst
+-rw-r--r--   0        0        0      568 2021-10-13 09:30:04.118485 asaman-0.2.1/docs/source/index.rst
+-rw-r--r--   0        0        0      196 2021-10-05 05:15:36.281858 asaman-0.2.1/docs/source/install.rst
+-rw-r--r--   0        0        0     5550 2023-04-21 17:22:53.350102 asaman-0.2.1/docs/source/usage.rst
+-rw-r--r--   0        0        0      777 2023-04-21 17:22:53.350102 asaman-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-04-16 07:24:08.411438 asaman-0.2.1/requirements.in
+-rw-r--r--   0        0        0     2467 2023-04-16 07:24:08.411438 asaman-0.2.1/requirements.txt
+-rw-r--r--   0        0        0        3 2023-03-09 09:29:11.152792 asaman-0.2.1/test.in
+-rw-r--r--   0        0        0      759 2023-03-09 09:29:11.152792 asaman-0.2.1/test.txt
+-rw-r--r--   0        0        0       62 2021-10-06 04:36:45.710606 asaman-0.2.1/tests/test_requirements.py
+-rw-r--r--   0        0        0     7501 1970-01-01 00:00:00.000000 asaman-0.2.1/PKG-INFO
```

### Comparing `asaman-0.2.0/.github/workflows/github-actions.yml` & `asaman-0.2.1/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `asaman-0.2.0/LICENSE` & `asaman-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asaman-0.2.0/README.md` & `asaman-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `asaman-0.2.0/asaman/__init__.py` & `asaman-0.2.1/asaman/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 "A tool to create reproducible wheels"
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 import glob
 import os
 import shutil
 import subprocess
 import sys
 import tempfile
```

### Comparing `asaman-0.2.0/dev-ci.txt` & `asaman-0.2.1/dev-ci.txt`

 * *Files identical despite different names*

### Comparing `asaman-0.2.0/dev-requirements.txt` & `asaman-0.2.1/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `asaman-0.2.0/docs/Makefile` & `asaman-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `asaman-0.2.0/docs/make.bat` & `asaman-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `asaman-0.2.0/docs/source/conf.py` & `asaman-0.2.1/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "asaman"
 copyright = "2021-2023, Kushal Das"
 author = "Kushal Das"
 
 # The full version, including alpha/beta/rc tags
-release = "0.2.0"
+release = "0.2.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `asaman-0.2.0/docs/source/hacking.rst` & `asaman-0.2.1/docs/source/hacking.rst`

 * *Files identical despite different names*

### Comparing `asaman-0.2.0/docs/source/index.rst` & `asaman-0.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `asaman-0.2.0/docs/source/usage.rst` & `asaman-0.2.1/docs/source/usage.rst`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,48 @@
 ======
 
 `asaman` can be used in various ways, the simplest form would be to create a
 reproducible wheel for your own project, via a source tarball.
 
 To achive this, the project uses a `SOURCE_DATE_EPOCH` value as `1309379017`,
 this time has been chosen to remember `Aaron Swartz <https://en.wikipedia.org/wiki/Aaron_Swartz>`_,
-his first commit to the SecureDrop project.
+his first commit to the SecureDrop project. You can pass a different value as an argument to `--sde`.
 
 We also use `/tmp/pip-wheel-build/` directory to build the wheels.
 
+Command line options
+---------------------
+
+::
+
+    Usage: asaman [OPTIONS]
+
+      Tool to build reproducible wheels.
+
+    Options:
+      -s, --source FILE          A single source tarball or zip file.
+      -d, --directory DIRECTORY  A directory containing all source tarballs and
+                                 zips.
+      -o, --output DIRECTORY     The output directory to store all wheel files.
+                                 Default: ./wheels
+      -r, --requirement FILE     Path to the requirement.txt file which contains
+                                 all packages to build along with hashes.
+      --sde TEXT                 Custom SOURCE_DATE_EPOCH value.
+      --no-hash                  DO NOT USE UNLESS VERY SURE: In case we skip hash
+                                 checking for download.
+      --keep-sources             Copy over the sources to output directory
+      --with-index TEXT          In case you want to install build time
+                                 dependencies from an index, pass the URL.
+      --trusted-host TEXT        Pass --trusted-host VALUE to pip, helps in local
+                                 indexes over HTTP. Pass the correct hostname.
+      --skip-build-deps          While downloading the sources, skip downloading
+                                 the build dependencies as source  [default: True]
+      --help                     Show this message and exit.
+
+
 Creating wheel from a source tarball
 -------------------------------------
 
 ::
 
     asaman -s path/to/source.tar.gz
```

### Comparing `asaman-0.2.0/pyproject.toml` & `asaman-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 dynamic = ["version", "description"]
 dependencies = [
     "wheel",
     "build>=0.7.0",
     "click",
     "pep517",
     "setuptools",
+    "pip-requirements-parser",
 ]
 
 [project.urls]
 Documentation = "https://asaman.readthedocs.io/en/latest/"
 Source = "https://github.com/kushaldas/asaman"
 
 [project.scripts]
```

### Comparing `asaman-0.2.0/requirements.txt` & `asaman-0.2.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `asaman-0.2.0/test.txt` & `asaman-0.2.1/test.txt`

 * *Files identical despite different names*

### Comparing `asaman-0.2.0/PKG-INFO` & `asaman-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: asaman
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool to create reproducible wheels
 Author-email: Kushal Das <mail@kushaldas.in>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: wheel
 Requires-Dist: build>=0.7.0
 Requires-Dist: click
 Requires-Dist: pep517
 Requires-Dist: setuptools
+Requires-Dist: pip-requirements-parser
 Project-URL: Documentation, https://asaman.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/kushaldas/asaman
 
 # asaman: Amra Saman (আমরা সমান)
 
 This is a tool to build reproducible wheels for your Python project or for all of your dependencies. What this means is if you use the same Operating System version and similar system level dependencies, you will always get the same wheel generated. This enables us to have a bit more protection from side-channel attacks. Any user of the wheels can verify that they are using the correct build from the exact source via verifying the builds themselves.
```

