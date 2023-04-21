# Comparing `tmp/trx-python-0.1.tar.gz` & `tmp/trx-python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trx-python-0.1.tar", last modified: Thu Jan 12 19:09:21 2023, max compression
+gzip compressed data, was "trx-python-0.1.2.tar", last modified: Fri Apr 21 13:33:04 2023, max compression
```

## Comparing `trx-python-0.1.tar` & `trx-python-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-12 19:09:21.235841 trx-python-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-12 19:09:21.219841 trx-python-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-12 19:09:21.227841 trx-python-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1012 2023-01-12 19:09:14.000000 trx-python-0.1/.github/workflows/docbuild.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1120 2023-01-12 19:09:14.000000 trx-python-0.1/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1031 2023-01-12 19:09:14.000000 trx-python-0.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1833 2023-01-12 19:09:14.000000 trx-python-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1314 2023-01-12 19:09:14.000000 trx-python-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1803 2023-01-12 19:09:21.235841 trx-python-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1134 2023-01-12 19:09:14.000000 trx-python-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-12 19:09:21.227841 trx-python-0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (116)      639 2023-01-12 19:09:14.000000 trx-python-0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-12 19:09:21.227841 trx-python-0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)    38942 2023-01-12 19:09:14.000000 trx-python-0.1/docs/_static/trx_logo.png
--rw-r--r--   0 runner    (1001) docker     (116)      804 2023-01-12 19:09:14.000000 trx-python-0.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-12 19:09:21.231841 trx-python-0.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (116)     2789 2023-01-12 19:09:14.000000 trx-python-0.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)     2353 2023-01-12 19:09:14.000000 trx-python-0.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      405 2023-01-12 19:09:14.000000 trx-python-0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-12 19:09:21.231841 trx-python-0.1/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-12 19:09:21.231841 trx-python-0.1/scripts/tests/
--rw-r--r--   0 runner    (1001) docker     (116)    10377 2023-01-12 19:09:14.000000 trx-python-0.1/scripts/tests/test_workflows.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2609 2023-01-12 19:09:14.000000 trx-python-0.1/scripts/tff_concatenate_tractograms.py
--rw-r--r--   0 runner    (1001) docker     (116)     2323 2023-01-12 19:09:14.000000 trx-python-0.1/scripts/tff_convert_dsi_studio.py
--rw-r--r--   0 runner    (1001) docker     (116)     2145 2023-01-12 19:09:14.000000 trx-python-0.1/scripts/tff_convert_tractogram.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6544 2023-01-12 19:09:14.000000 trx-python-0.1/scripts/tff_generate_trx_from_scratch.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1127 2023-01-12 19:09:14.000000 trx-python-0.1/scripts/tff_simple_compare.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2359 2023-01-12 19:09:14.000000 trx-python-0.1/scripts/tff_validate_trx.py
--rw-r--r--   0 runner    (1001) docker     (116)      756 2023-01-12 19:09:14.000000 trx-python-0.1/scripts/tff_verify_header_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (116)     1165 2023-01-12 19:09:14.000000 trx-python-0.1/scripts/tff_visualize_overlap.py
--rw-r--r--   0 runner    (1001) docker     (116)      894 2023-01-12 19:09:21.239841 trx-python-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      841 2023-01-12 19:09:14.000000 trx-python-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-12 19:09:21.235841 trx-python-0.1/trx/
--rwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-12 19:09:14.000000 trx-python-0.1/trx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       83 2023-01-12 19:09:21.000000 trx-python-0.1/trx/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     3007 2023-01-12 19:09:14.000000 trx-python-0.1/trx/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (116)     2943 2023-01-12 19:09:14.000000 trx-python-0.1/trx/io.py
--rw-r--r--   0 runner    (1001) docker     (116)     4420 2023-01-12 19:09:14.000000 trx-python-0.1/trx/streamlines_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-12 19:09:21.235841 trx-python-0.1/trx/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     2214 2023-01-12 19:09:14.000000 trx-python-0.1/trx/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (116)    10608 2023-01-12 19:09:14.000000 trx-python-0.1/trx/tests/test_memmap.py
--rw-r--r--   0 runner    (1001) docker     (116)     3307 2023-01-12 19:09:14.000000 trx-python-0.1/trx/tests/test_streamlines_ops.py
--rw-r--r--   0 runner    (1001) docker     (116)    61850 2023-01-12 19:09:14.000000 trx-python-0.1/trx/trx_file_memmap.py
--rw-r--r--   0 runner    (1001) docker     (116)    13332 2023-01-12 19:09:14.000000 trx-python-0.1/trx/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      155 2023-01-12 19:09:21.000000 trx-python-0.1/trx/version.py
--rw-r--r--   0 runner    (1001) docker     (116)     3691 2023-01-12 19:09:14.000000 trx-python-0.1/trx/viz.py
--rw-r--r--   0 runner    (1001) docker     (116)    16742 2023-01-12 19:09:14.000000 trx-python-0.1/trx/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-12 19:09:21.235841 trx-python-0.1/trx_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1803 2023-01-12 19:09:21.000000 trx-python-0.1/trx_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      991 2023-01-12 19:09:21.000000 trx-python-0.1/trx_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-12 19:09:21.000000 trx-python-0.1/trx_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      261 2023-01-12 19:09:21.000000 trx-python-0.1/trx_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        4 2023-01-12 19:09:21.000000 trx-python-0.1/trx_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:33:04.806664 trx-python-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:33:04.798663 trx-python-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:33:04.802664 trx-python-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-21 13:32:51.000000 trx-python-0.1.2/.github/workflows/docbuild.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-21 13:32:51.000000 trx-python-0.1.2/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-21 13:32:51.000000 trx-python-0.1.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-21 13:32:51.000000 trx-python-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-21 13:32:51.000000 trx-python-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-21 13:33:04.806664 trx-python-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-21 13:32:51.000000 trx-python-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:33:04.802664 trx-python-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-21 13:32:51.000000 trx-python-0.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:33:04.802664 trx-python-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    38942 2023-04-21 13:32:51.000000 trx-python-0.1.2/docs/_static/trx_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-21 13:32:51.000000 trx-python-0.1.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:33:04.802664 trx-python-0.1.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-21 13:32:51.000000 trx-python-0.1.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-21 13:32:51.000000 trx-python-0.1.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-21 13:32:51.000000 trx-python-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:33:04.802664 trx-python-0.1.2/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:33:04.802664 trx-python-0.1.2/scripts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-21 13:32:51.000000 trx-python-0.1.2/scripts/tests/test_workflows.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2609 2023-04-21 13:32:51.000000 trx-python-0.1.2/scripts/tff_concatenate_tractograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-21 13:32:51.000000 trx-python-0.1.2/scripts/tff_convert_dsi_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-21 13:32:51.000000 trx-python-0.1.2/scripts/tff_convert_tractogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6544 2023-04-21 13:32:51.000000 trx-python-0.1.2/scripts/tff_generate_trx_from_scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-21 13:32:51.000000 trx-python-0.1.2/scripts/tff_manipulate_datatype.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1127 2023-04-21 13:32:51.000000 trx-python-0.1.2/scripts/tff_simple_compare.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2359 2023-04-21 13:32:51.000000 trx-python-0.1.2/scripts/tff_validate_trx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-21 13:32:51.000000 trx-python-0.1.2/scripts/tff_verify_header_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-21 13:32:51.000000 trx-python-0.1.2/scripts/tff_visualize_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-21 13:33:04.806664 trx-python-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-21 13:32:51.000000 trx-python-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:33:04.806664 trx-python-0.1.2/trx/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:32:51.000000 trx-python-0.1.2/trx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-21 13:33:04.000000 trx-python-0.1.2/trx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-21 13:32:51.000000 trx-python-0.1.2/trx/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-21 13:32:51.000000 trx-python-0.1.2/trx/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-21 13:32:51.000000 trx-python-0.1.2/trx/streamlines_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:33:04.806664 trx-python-0.1.2/trx/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-21 13:32:51.000000 trx-python-0.1.2/trx/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-04-21 13:32:51.000000 trx-python-0.1.2/trx/tests/test_memmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-21 13:32:51.000000 trx-python-0.1.2/trx/tests/test_streamlines_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65889 2023-04-21 13:32:51.000000 trx-python-0.1.2/trx/trx_file_memmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-04-21 13:32:51.000000 trx-python-0.1.2/trx/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 13:33:04.000000 trx-python-0.1.2/trx/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-21 13:32:51.000000 trx-python-0.1.2/trx/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20224 2023-04-21 13:32:51.000000 trx-python-0.1.2/trx/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:33:04.806664 trx-python-0.1.2/trx_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-21 13:33:04.000000 trx-python-0.1.2/trx_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-21 13:33:04.000000 trx-python-0.1.2/trx_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:33:04.000000 trx-python-0.1.2/trx_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-21 13:33:04.000000 trx-python-0.1.2/trx_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-21 13:33:04.000000 trx-python-0.1.2/trx_python.egg-info/top_level.txt
```

### Comparing `trx-python-0.1/.github/workflows/docbuild.yml` & `trx-python-0.1.2/.github/workflows/docbuild.yml`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/.github/workflows/publish-to-test-pypi.yml` & `trx-python-0.1.2/.github/workflows/publish-to-test-pypi.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 name: Publish Python 🐍 distributions 📦 to PyPI and TestPyPI
 
 on: push
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to PyPI and TestPyPI
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@master
     - name: Set up Python 3.9
       uses: actions/setup-python@v1
       with:
         python-version: 3.9
-    - name: Install pep517
+    - name: Install pypa/build
       run: >-
         python -m
         pip install
-        pep517
+        build
         --user
     - name: Build a binary wheel and a source tarball
       run: >-
         python -m
-        pep517.build
-        --source
-        --binary
-        --out-dir dist/
+        build
+        --sdist
+        --wheel
+        --outdir dist/
         .
     - name: Publish distribution 📦 to Test PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.test_pypi_password }}
         repository_url: https://test.pypi.org/legacy/
```

### Comparing `trx-python-0.1/.gitignore` & `trx-python-0.1.2/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+trx/version.py
 .DS_Store
 *_version.py
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
@@ -47,15 +47,15 @@
 .nox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 *.cover
-*.py,cover
+*.py, cover
 .hypothesis/
 .pytest_cache/
 
 # Translations
 *.mo
 *.pot
 
@@ -89,15 +89,15 @@
 .python-version
 
 # pipenv
 #   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
 #   However, in case of collaboration, if having platform-specific dependencies or dependencies
 #   having no cross-platform support, pipenv may install dependencies that don't work, or not
 #   install all needed dependencies.
-#Pipfile.lock
+# Pipfile.lock
 
 # PEP 582; used by e.g. github.com/David-OConnor/pyflow
 __pypackages__/
 
 # Celery stuff
 celerybeat-schedule
 celerybeat.pid
```

### Comparing `trx-python-0.1/LICENSE` & `trx-python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/PKG-INFO` & `trx-python-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trx-python
-Version: 0.1
+Version: 0.1.2
 Summary: Experiments with new file format for tractography
 Home-page: https://github.com/tee-ar-ex/trx-python
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
@@ -31,14 +31,20 @@
 
 Or, to install from source:
 
     git clone https://github.com/tee-ar-ex/trx-python.git
     cd trx-python
     pip install .
 
+### Install Dipy for integration
+If you wish to use all the scripts and run the test you will need to install Dipy
+
+    pip install cython packaging
+    pip install dipy@git+https://git@github.com/frheault/dipy@ba3ce0c59#egg=dipy
+
 ### Temporary Directory
 The TRX file format uses memmaps to limit RAM usage. When dealing with large files this means several gigabytes could be required on disk (instead of RAM). 
 
 By default, the temporary directory on Linux and MacOS is `/tmp` and on Windows it should be `C:\WINDOWS\Temp`.
 
 If you wish to change the directory add the following variable to your script or to your .bashrc or .bash_profile:
 `export TRX_TMPDIR=/WHERE/I/WANT/MY/TMP/DATA` (a)
```

### Comparing `trx-python-0.1/README.md` & `trx-python-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 
 Or, to install from source:
 
     git clone https://github.com/tee-ar-ex/trx-python.git
     cd trx-python
     pip install .
 
+### Install Dipy for integration
+If you wish to use all the scripts and run the test you will need to install Dipy
+
+    pip install cython packaging
+    pip install dipy@git+https://git@github.com/frheault/dipy@ba3ce0c59#egg=dipy
+
 ### Temporary Directory
 The TRX file format uses memmaps to limit RAM usage. When dealing with large files this means several gigabytes could be required on disk (instead of RAM). 
 
 By default, the temporary directory on Linux and MacOS is `/tmp` and on Windows it should be `C:\WINDOWS\Temp`.
 
 If you wish to change the directory add the following variable to your script or to your .bashrc or .bash_profile:
 `export TRX_TMPDIR=/WHERE/I/WANT/MY/TMP/DATA` (a)
```

### Comparing `trx-python-0.1/docs/Makefile` & `trx-python-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/docs/_static/trx_logo.png` & `trx-python-0.1.2/docs/_static/trx_logo.png`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/docs/make.bat` & `trx-python-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/docs/source/conf.py` & `trx-python-0.1.2/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,17 +59,14 @@
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_logo = "../_static/trx_logo.png"
 
 
 html_theme_options = {
-    "logo": {
-        "text": "TRX Python",
-    },
     "icon_links": [
         {
             # Label for this link
             "name": "GitHub",
             # URL where the link will redirect
             "url": "https://github.com/tee-ar-ex",  # required
             # Icon class (if "type": "fontawesome"), or path to local image (if "type": "local")
```

### Comparing `trx-python-0.1/docs/source/index.rst` & `trx-python-0.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/scripts/tests/test_workflows.py` & `trx-python-0.1.2/scripts/tests/test_workflows.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+from deepdiff import DeepDiff
 import os
 
 import pytest
 import numpy as np
 from numpy.testing import assert_equal, assert_array_equal, assert_allclose
 try:
     from dipy.io.streamline import load_tractogram
@@ -14,48 +15,42 @@
 
 from trx.fetcher import (get_testing_files_dict,
                          fetch_data, get_home)
 from trx.io import get_trx_tmpdir
 import trx.trx_file_memmap as tmm
 from trx.workflows import (convert_dsi_studio,
                            convert_tractogram,
+                           manipulate_trx_datatype,
                            generate_trx_from_scratch,
-                           validate_tractogram)
+                           validate_tractogram,)
 
 
 # If they already exist, this only takes 5 seconds (check md5sum)
 fetch_data(get_testing_files_dict(), keys=['DSI.zip', 'trx_from_scratch.zip'])
 tmp_dir = get_trx_tmpdir()
 
 
 def test_help_option_convert_dsi(script_runner):
-    if not dipy_available:
-        pytest.skip('Dipy library is missing, cannot test scripts involving '
-                    'tck/trk/vtk.')
     ret = script_runner.run('tff_convert_dsi_studio.py', '--help')
     assert ret.success
 
 
 def test_help_option_convert(script_runner):
-    if not dipy_available:
-        pytest.skip('Dipy library is missing, cannot test scripts involving '
-                    'tck/trk/vtk.')
     ret = script_runner.run('tff_convert_tractogram.py', '--help')
     assert ret.success
 
 
 def test_help_option_generate_trx_from_scratch(script_runner):
     ret = script_runner.run('tff_generate_trx_from_scratch.py', '--help')
     assert ret.success
 
 
+@pytest.mark.skipif(not dipy_available,
+                    reason='Dipy is not installed.')
 def test_execution_convert_dsi():
-    if not dipy_available:
-        pytest.skip('Dipy library is missing, cannot test scripts involving '
-                    'tck/trk/vtk.')
     os.chdir(os.path.expanduser(tmp_dir.name))
     in_trk = os.path.join(get_home(), 'DSI',
                           'CC.trk.gz')
     in_nii = os.path.join(get_home(), 'DSI',
                           'CC.nii.gz')
     exp_data = os.path.join(get_home(), 'DSI',
                             'CC_fix_data.npy')
@@ -69,18 +64,17 @@
     offsets_fix = np.load(exp_offsets)
 
     sft = load_tractogram('fixed.trk', 'same')
     assert_equal(sft.streamlines._data, data_fix)
     assert_equal(sft.streamlines._offsets, offsets_fix)
 
 
+@pytest.mark.skipif(not dipy_available,
+                    reason='Dipy is not installed.')
 def test_execution_convert_to_trx():
-    if not dipy_available:
-        pytest.skip('Dipy library is missing, cannot test scripts involving '
-                    'tck/trk/vtk.')
     os.chdir(os.path.expanduser(tmp_dir.name))
     in_trk = os.path.join(get_home(), 'DSI',
                           'CC_fix.trk')
     exp_data = os.path.join(get_home(), 'DSI',
                             'CC_fix_data.npy')
     exp_offsets = os.path.join(get_home(), 'DSI',
                                'CC_fix_offsets.npy')
@@ -92,18 +86,17 @@
     trx = tmm.load('CC_fix.trx')
     assert_equal(trx.streamlines._data.dtype, np.float32)
     assert_equal(trx.streamlines._offsets.dtype, np.uint32)
     assert_array_equal(trx.streamlines._data, data_fix)
     assert_array_equal(trx.streamlines._offsets, offsets_fix)
 
 
+@pytest.mark.skipif(not dipy_available,
+                    reason='Dipy is not installed.')
 def test_execution_convert_from_trx():
-    if not dipy_available:
-        pytest.skip('Dipy library is missing, cannot test scripts involving '
-                    'tck/trk/vtk.')
     os.chdir(os.path.expanduser(tmp_dir.name))
     in_trk = os.path.join(get_home(), 'DSI',
                           'CC_fix.trk')
     in_nii = os.path.join(get_home(), 'DSI',
                           'CC.nii.gz')
     exp_data = os.path.join(get_home(), 'DSI',
                             'CC_fix_data.npy')
@@ -123,33 +116,31 @@
     assert_equal(sft.streamlines._offsets, offsets_fix)
 
     sft = load_tractogram('CC_converted.tck', in_nii)
     assert_equal(sft.streamlines._data, data_fix)
     assert_equal(sft.streamlines._offsets, offsets_fix)
 
 
+@pytest.mark.skipif(not dipy_available,
+                    reason='Dipy is not installed.')
 def test_execution_convert_dtype_p16_o64():
-    if not dipy_available:
-        pytest.skip('Dipy library is missing, cannot test scripts involving '
-                    'tck/trk/vtk.')
     os.chdir(os.path.expanduser(tmp_dir.name))
     in_trk = os.path.join(get_home(), 'DSI',
                           'CC_fix.trk')
     convert_tractogram(in_trk, 'CC_fix_p16_o64.trx', None,
                        pos_dtype='float16', offsets_dtype='uint64')
 
     trx = tmm.load('CC_fix_p16_o64.trx')
     assert_equal(trx.streamlines._data.dtype, np.float16)
     assert_equal(trx.streamlines._offsets.dtype, np.uint64)
 
 
+@pytest.mark.skipif(not dipy_available,
+                    reason='Dipy is not installed.')
 def test_execution_convert_dtype_p64_o32():
-    if not dipy_available:
-        pytest.skip('Dipy library is missing, cannot test scripts involving '
-                    'tck/trk/vtk.')
     os.chdir(os.path.expanduser(tmp_dir.name))
     in_trk = os.path.join(get_home(), 'DSI',
                           'CC_fix.trk')
     convert_tractogram(in_trk, 'CC_fix_p64_o32.trx', None,
                        pos_dtype='float64', offsets_dtype='uint32')
 
     trx = tmm.load('CC_fix_p64_o32.trx')
@@ -182,20 +173,22 @@
                               positions=os.path.join(raw_arr_dir,
                                                      'positions.npy'),
                               offsets=os.path.join(raw_arr_dir,
                                                    'offsets.npy'),
                               positions_dtype='float16',
                               offsets_dtype='uint64',
                               space_str='rasmm', origin_str='nifti',
-                              verify_invalid=True, dpv=dpv, dps=dps,
+                              verify_invalid=False, dpv=dpv, dps=dps,
                               groups=groups, dpg=dpg)
 
     exp_trx = tmm.load(expected_trx)
     gen_trx = tmm.load('generated.trx')
 
+    assert DeepDiff(exp_trx.get_dtype_dict(), gen_trx.get_dtype_dict()) == {}
+
     assert_allclose(exp_trx.streamlines._data, gen_trx.streamlines._data,
                     atol=0.1, rtol=0.1)
     assert_equal(exp_trx.streamlines._offsets, gen_trx.streamlines._offsets)
 
     for key in exp_trx.data_per_vertex.keys():
         assert_equal(exp_trx.data_per_vertex[key]._data,
                      gen_trx.data_per_vertex[key]._data)
@@ -210,22 +203,23 @@
     for group in exp_trx.groups.keys():
         if group in exp_trx.data_per_group:
             for key in exp_trx.data_per_group[group].keys():
                 assert_equal(exp_trx.data_per_group[group][key],
                              gen_trx.data_per_group[group][key])
 
 
+@pytest.mark.skipif(not dipy_available,
+                    reason='Dipy is not installed.')
 def test_execution_concatenate_validate_trx():
     os.chdir(os.path.expanduser(tmp_dir.name))
     trx1 = tmm.load(os.path.join(get_home(), 'gold_standard',
                                  'gs.trx'))
     trx2 = tmm.load(os.path.join(get_home(), 'gold_standard',
                                  'gs.trx'))
-    trx2.streamlines._data += + 0.001
-
+    # trx2.streamlines._data += 0.001
     trx = tmm.concatenate([trx1, trx2], preallocation=False)
 
     # Right size
     assert_equal(len(trx.streamlines), 2*len(trx1.streamlines))
 
     # Right data
     end_idx = trx1.header['NB_VERTICES']
@@ -247,11 +241,58 @@
                      trx2.data_per_streamline[key])
 
     # Validate
     tmm.save(trx, 'concat.trx')
     validate_tractogram('concat.trx', None, 'valid.trx',
                         remove_identical_streamlines=True,
                         precision=0)
-    trx = tmm.load('valid.trx')
+    trx_val = tmm.load('valid.trx')
+
+    # Right dtype
+    assert DeepDiff(trx.get_dtype_dict(), trx_val.get_dtype_dict()) == {}
 
     # Right size
-    assert_equal(len(trx.streamlines), len(trx1.streamlines))
+    assert_equal(len(trx1.streamlines), len(trx_val.streamlines))
+
+
+@pytest.mark.skipif(not dipy_available,
+                    reason='Dipy is not installed.')
+def test_execution_manipulate_trx_datatype():
+    os.chdir(os.path.expanduser(tmp_dir.name))
+    expected_trx = os.path.join(get_home(), 'trx_from_scratch',
+                                'expected.trx')
+    trx = tmm.load(expected_trx)
+
+    expected_dtype = {'positions': np.dtype('float16'),
+                      'offsets': np.dtype('uint64'),
+                      'dpv': {'dpv_cx': np.dtype('uint8'),
+                              'dpv_cy': np.dtype('uint8'),
+                              'dpv_cz': np.dtype('uint8')},
+                      'dps': {'dps_algo': np.dtype('uint8'),
+                              'dps_cw': np.dtype('float64')},
+                      'dpg': {'g_AF_L':
+                              {'dpg_AF_L_mean_fa': np.dtype('float32'),
+                               'dpg_AF_L_volume': np.dtype('float32')},
+                              'g_AF_R':
+                              {'dpg_AF_R_mean_fa': np.dtype('float32')}},
+                      'groups': {'g_AF_L': np.dtype('int32'),
+                                 'g_AF_R': np.dtype('int32')}}
+    assert DeepDiff(trx.get_dtype_dict(), expected_dtype) == {}
+
+    generated_dtype = {'positions': np.dtype('float32'),
+                       'offsets': np.dtype('uint32'),
+                       'dpv': {'dpv_cx': np.dtype('uint16'),
+                               'dpv_cy': np.dtype('uint16'),
+                               'dpv_cz': np.dtype('uint16')},
+                       'dps': {'dps_algo': np.dtype('uint8'),
+                               'dps_cw': np.dtype('float32')},
+                       'dpg': {'g_AF_L':
+                               {'dpg_AF_L_mean_fa': np.dtype('float64'),
+                                'dpg_AF_L_volume': np.dtype('float32')},
+                               'g_AF_R':
+                               {'dpg_AF_R_mean_fa': np.dtype('float64')}},
+                       'groups': {'g_AF_L': np.dtype('uint16'),
+                                  'g_AF_R': np.dtype('uint16')}}
+
+    manipulate_trx_datatype(expected_trx, 'generated.trx', generated_dtype)
+    trx = tmm.load('generated.trx')
+    assert DeepDiff(trx.get_dtype_dict(), generated_dtype) == {}
```

### Comparing `trx-python-0.1/scripts/tff_concatenate_tractograms.py` & `trx-python-0.1.2/scripts/tff_concatenate_tractograms.py`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/scripts/tff_convert_dsi_studio.py` & `trx-python-0.1.2/scripts/tff_convert_dsi_studio.py`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/scripts/tff_convert_tractogram.py` & `trx-python-0.1.2/scripts/tff_convert_tractogram.py`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/scripts/tff_generate_trx_from_scratch.py` & `trx-python-0.1.2/scripts/tff_generate_trx_from_scratch.py`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/scripts/tff_simple_compare.py` & `trx-python-0.1.2/scripts/tff_simple_compare.py`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/scripts/tff_validate_trx.py` & `trx-python-0.1.2/scripts/tff_validate_trx.py`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/scripts/tff_verify_header_compatibility.py` & `trx-python-0.1.2/scripts/tff_verify_header_compatibility.py`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/scripts/tff_visualize_overlap.py` & `trx-python-0.1.2/scripts/tff_visualize_overlap.py`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/setup.cfg` & `trx-python-0.1.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -7,36 +7,39 @@
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Topic :: Scientific/Engineering
 license = BSD License
 description = Experiments with new file format for tractography
-long_description = file:README.md
+long_description = file: README.md
 long_description_content_type = text/markdown
 platforms = OS Independent
 packages = find:
 include_package_data = True
 
 [options]
 python_requires = >=3.7
-setup_requires = packaging >=19.0
-install_requires = nibabel >= 3.*
+setup_requires = 
+	packaging >= 19.0
+	cython >= 0.29
+install_requires = 
+	setuptools_scm
+	deepdiff
+	nibabel >= 3
 
 [options.extras_require]
-doc = sphinx<=6.*
+doc = sphinx <= 6
 	pydata-sphinx-theme
 	sphinx-autoapi
 	numpydoc
 test = 
 	flake8
-	pytest>=7.*
-	pytest-console-scripts>=0.*
-	fury
-	dipy
+	pytest >= 7
+	pytest-console-scripts >= 0
 all = 
 	%(doc)s
 	%(test)s
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trx-python-0.1/setup.py` & `trx-python-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
             else:
                 gh_in_int.append(str(string.ascii_letters.find(char)))
         return "".join(gh_in_int)
     else:
         return ""
 
 
-opts = dict(use_scm_version={"root": ".", "relative_to": __file__,
-                     "write_to": op.join("trx", "version.py"),
-                     "local_scheme": local_version},
-            scripts=glob.glob("scripts/*.py"))
+opts = dict(use_scm_version={
+    "root": ".", "relative_to": __file__,
+    "write_to": op.join("trx", "version.py"),
+    "local_scheme": local_version},
+    scripts=glob.glob("scripts/*.py"))
 
 
 if __name__ == '__main__':
     setup(**opts)
```

### Comparing `trx-python-0.1/trx/fetcher.py` & `trx-python-0.1.2/trx/fetcher.py`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/trx/io.py` & `trx-python-0.1.2/trx/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import os
 import logging
 import tempfile
 
 try:
-    from dipy.io.stateful_tractogram import StatefulTractogram
-    from dipy.io.streamline import load_tractogram, save_tractogram
+    import dipy
     dipy_available = True
 except ImportError:
     dipy_available = False
 
 from trx.utils import split_name_with_gz
 
 
@@ -29,14 +28,16 @@
 
 def load_sft_with_reference(filepath, reference=None,
                             bbox_check=True):
     if not dipy_available:
         logging.error('Dipy library is missing, cannot use functions related '
                       'to the StatefulTractogram.')
         return None
+    from dipy.io.streamline import load_tractogram
+
     # Force the usage of --reference for all file formats without an header
     _, ext = os.path.splitext(filepath)
     if ext == '.trk':
         if reference is not None and reference != 'same':
             logging.warning('Reference is discarded for this file format '
                             '{}.'.format(filepath))
         sft = load_tractogram(filepath, 'same',
@@ -64,20 +65,27 @@
                                                  bbox_check=False)
     else:
         tractogram_obj = tmm.load(tractogram_filename)
 
     return tractogram_obj
 
 
-def save(tractogram_obj, tractogram_filename):
+def save(tractogram_obj, tractogram_filename, bbox_valid_check=False):
+    if not dipy_available:
+        logging.error('Dipy library is missing, cannot use functions related '
+                    'to the StatefulTractogram.')
+        return None
+    from dipy.io.stateful_tractogram import StatefulTractogram
+    from dipy.io.streamline import save_tractogram
     import trx.trx_file_memmap as tmm
+
     out_ext = split_name_with_gz(tractogram_filename)[1]
 
     if out_ext != '.trx':
         if not isinstance(tractogram_obj, StatefulTractogram):
             tractogram_obj = tractogram_obj.to_sft()
         save_tractogram(tractogram_obj, tractogram_filename,
-                        bbox_valid_check=False)
+                        bbox_valid_check=bbox_valid_check)
     else:
         if not isinstance(tractogram_obj, tmm.TrxFile):
             tractogram_obj = tmm.TrxFile.from_sft(tractogram_obj)
         tmm.save(tractogram_obj, tractogram_filename)
```

### Comparing `trx-python-0.1/trx/streamlines_ops.py` & `trx-python-0.1.2/trx/streamlines_ops.py`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/trx/tests/test_io.py` & `trx-python-0.1.2/trx/tests/test_io.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,26 +2,34 @@
 # -*- coding: utf-8 -*-
 
 import os
 
 import pytest
 import numpy as np
 from numpy.testing import assert_allclose
+
+try:
+    import dipy
+    dipy_available = True
+except ImportError:
+    dipy_available = False
+
 from trx.trx_file_memmap import TrxFile
 from trx.io import load, save, get_trx_tmpdir
 from trx.fetcher import (get_testing_files_dict,
                          fetch_data, get_home)
 
 
 fetch_data(get_testing_files_dict(), keys=['gold_standard.zip'])
 tmp_dir = get_trx_tmpdir()
 
 
 @pytest.mark.parametrize("path", [("gs.trx"), ("gs.trk"), ("gs.tck"),
                                   ("gs.vtk")])
+@pytest.mark.skipif(not dipy_available, reason='Dipy is not installed.')
 def test_load_vox(path):
     dir = os.path.join(get_home(), 'gold_standard')
     path = os.path.join(dir, path)
     coord = np.loadtxt(os.path.join(get_home(), 'gold_standard',
                                     'gs_vox_space.txt'))
     obj = load(path, os.path.join(dir, 'gs.nii'))
 
@@ -29,28 +37,30 @@
     sft.to_vox()
 
     assert_allclose(sft.streamlines._data, coord, rtol=1e-04, atol=1e-06)
 
 
 @pytest.mark.parametrize("path", [("gs.trx"), ("gs.trk"), ("gs.tck"),
                                   ("gs.vtk")])
+@pytest.mark.skipif(not dipy_available, reason='Dipy is not installed.')
 def test_load_voxmm(path):
     dir = os.path.join(get_home(), 'gold_standard')
     path = os.path.join(dir, path)
     coord = np.loadtxt(os.path.join(get_home(), 'gold_standard',
                                     'gs_voxmm_space.txt'))
     obj = load(path, os.path.join(dir, 'gs.nii'))
 
     sft = obj.to_sft() if isinstance(obj, TrxFile) else obj
     sft.to_voxmm()
 
     assert_allclose(sft.streamlines._data, coord, rtol=1e-04, atol=1e-06)
 
 
-@pytest.mark.parametrize("path", [("gs.trk"), ("gs.trx"), ("gs_fldr.trx"), ])
+@pytest.mark.parametrize("path", [("gs.trk"), ("gs.trx"), ("gs_fldr.trx")])
+@pytest.mark.skipif(not dipy_available, reason='Dipy is not installed.')
 def test_multi_load_save_rasmm(path):
     dir = os.path.join(get_home(), 'gold_standard')
     basename, ext = os.path.splitext(path)
     out_path = os.path.join(tmp_dir.name, '{}_tmp{}'.format(basename, ext))
     path = os.path.join(dir, path)
     coord = np.loadtxt(os.path.join(get_home(), 'gold_standard',
                                     'gs_rasmm_space.txt'))
```

### Comparing `trx-python-0.1/trx/tests/test_memmap.py` & `trx-python-0.1.2/trx/tests/test_memmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 import os
 
 from nibabel.streamlines.tests.test_tractogram import make_dummy_streamline
 from nibabel.streamlines import LazyTractogram
 import numpy as np
 import pytest
 
+try:
+    import dipy
+    dipy_available = True
+except ImportError:
+    dipy_available = False
+
 from trx.io import get_trx_tmpdir
 import trx.trx_file_memmap as tmm
 from trx.fetcher import (get_testing_files_dict,
                          fetch_data, get_home)
 
 
 fetch_data(get_testing_files_dict(), keys=['memmap_test_data.zip'])
@@ -213,14 +219,15 @@
     concat.append(trx1, extra_buffer=buffer)
     if buffer > 0:
         concat.resize()
     assert len(concat) == len(trx1)
 
 
 @pytest.mark.parametrize("path, buffer", [("small.trx", 10000)])
+@pytest.mark.skipif(not dipy_available, reason="Dipy is not installed")
 def test_append_StatefulTractogram(path, buffer):
     path = os.path.join(get_home(), 'memmap_test_data', path)
     trx = tmm.load(path)
     obj = trx.to_sft()
     concat = tmm.TrxFile(nb_vertices=1, nb_streamlines=1, init_as=trx)
 
     concat.append(obj, extra_buffer=buffer)
@@ -245,15 +252,15 @@
 @pytest.mark.parametrize("path, size, buffer", [("small.trx", 50, 10000),
                                                 ("small.trx", 0, 10000),
                                                 ("small.trx", 25000, 10000),
                                                 ("small.trx", 50, 0),
                                                 ("small.trx", 0, 0),
                                                 ("small.trx", 25000, 10000)])
 def test_from_lazy_tractogram(path, size, buffer):
-    rng = np.random.RandomState(1776)
+    _ = np.random.RandomState(1776)
     streamlines = []
     fa = []
     commit_weights = []
     clusters_QB = []
     gen_range = [1, 2, 5, 2, 1] * (size // 5)
     for i in gen_range:
         data = make_dummy_streamline(i)
@@ -261,34 +268,35 @@
         streamlines.append(streamline)
         fa.append(data_per_point['fa'].astype(np.float16))
         commit_weights.append(
             data_for_streamline['mean_curvature'].astype(np.float32))
         clusters_QB.append(
             data_for_streamline['mean_torsion'].astype(np.uint16))
 
-    data_per_point = {'fa': [e for e in fa]}
-    data_per_streamline = {
-        'commit_weights': [e for e in commit_weights],
-        'clusters_QB': [e for e in clusters_QB]}
-
     def streamlines_func(): return (e for e in streamlines)
     data_per_point_func = {'fa': lambda: (e for e in fa)}
     data_per_streamline_func = {
         'commit_weights': lambda: (e for e in commit_weights),
         'clusters_QB': lambda: (e for e in clusters_QB)}
 
     obj = LazyTractogram(streamlines_func,
                          data_per_streamline_func,
                          data_per_point_func,
                          affine_to_rasmm=np.eye(4))
 
+    dtype_dict = {'positions': np.float32, 'offsets': np.uint32,
+                  'dpv': {'fa': np.float16},
+                  'dps': {'commit_weights': np.float32,
+                          'clusters_QB': np.uint16}}
     path = os.path.join(get_home(), 'memmap_test_data', path)
     trx = tmm.TrxFile.from_lazy_tractogram(obj, reference=path,
                                            extra_buffer=buffer,
-                                           chunk_size=1000)
+                                           chunk_size=1000,
+                                           dtype_dict=dtype_dict)
+
     assert len(trx) == len(gen_range)
 
 
 def test_zip_from_folder():
     pass
```

### Comparing `trx-python-0.1/trx/tests/test_streamlines_ops.py` & `trx-python-0.1.2/trx/tests/test_streamlines_ops.py`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/trx/trx_file_memmap.py` & `trx-python-0.1.2/trx/trx_file_memmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,46 +13,46 @@
 from nibabel.affines import voxel_sizes
 from nibabel.nifti1 import Nifti1Header, Nifti1Image
 from nibabel.orientations import aff2axcodes
 from nibabel.streamlines.array_sequence import ArraySequence
 from nibabel.streamlines.trk import TrkFile
 from nibabel.streamlines.tractogram import Tractogram, LazyTractogram
 import numpy as np
-from numpy.typing import ArrayLike, NDArray
 
 from trx.io import get_trx_tmpdir
 from trx.utils import (get_reference_info_wrapper,
                        convert_data_dict_to_tractogram,
                        append_generator_to_dict)
 
 try:
-    from dipy.io.stateful_tractogram import StatefulTractogram
+    import dipy
+    dipy_available = True
 except:
-    StatefulTractogram = None
+    dipy_available = False
 
 
-def _append_last_offsets(nib_offsets: NDArray, nb_vertices: int) -> NDArray:
+def _append_last_offsets(nib_offsets: np.ndarray, nb_vertices: int) -> np.ndarray:
     """Appends the last element of offsets from header information
 
     Keyword arguments:
-        nib_offsets -- NDArray
+        nib_offsets -- np.ndarray
             Array of offsets with the last element being the start of the last
             streamline (nibabel convention)
         nb_vertices -- int
             Total number of vertices in the streamlines
     Returns:
-        Offsets -- NDArray (VTK convention)
+        Offsets -- np.ndarray (VTK convention)
     """
     def is_sorted(a): return np.all(a[:-1] <= a[1:])
     if not is_sorted(nib_offsets):
         raise ValueError('Offsets must be sorted values.')
     return np.append(nib_offsets, nb_vertices).astype(nib_offsets.dtype)
 
 
-def _generate_filename_from_data(arr: ArrayLike, filename: str) -> str:
+def _generate_filename_from_data(arr: np.ndarray, filename: str) -> str:
     """Determines the data type from array data and generates the appropriate
     filename
 
     Keyword arguments:
         arr -- a NumPy array (1-2D, otherwise ValueError raised)
         filename -- the original filename
 
@@ -100,22 +100,22 @@
     dim = 1 if len(split) == 2 else split[1]
 
     _is_dtype_valid(ext)
 
     return basename, int(dim), ext
 
 
-def _compute_lengths(offsets: NDArray) -> NDArray:
+def _compute_lengths(offsets: np.ndarray) -> np.ndarray:
     """Compute lengths from offsets
 
     Keyword arguments:
-        offsets -- An NDArray of offsets
+        offsets -- An np.ndarray of offsets
 
     Returns:
-        lengths -- An NDArray of lengths
+        lengths -- An np.ndarray of lengths
     """
     if len(offsets) > 0:
         last_elem_pos = _dichotomic_search(offsets)
         lengths = np.ediff1d(offsets)
         if len(lengths) > last_elem_pos:
             lengths[last_elem_pos] = 0
     else:
@@ -139,20 +139,20 @@
         isinstance(np.dtype(ext.replace(".", "")), np.dtype)
         return True
     except TypeError:
         return False
 
 
 def _dichotomic_search(
-    x: NDArray, l_bound: Optional[int] = None, r_bound: Optional[int] = None
+    x: np.ndarray, l_bound: Optional[int] = None, r_bound: Optional[int] = None
 ) -> int:
     """Find where data of a contiguous array is actually ending
 
     Keyword arguments:
-        x -- NDArray of values
+        x -- np.ndarray of values
         l_bound -- lower bound index for search
         r_bound -- upper bound index for search
     Returns:
         index at which array value is 0 (if possible), otherwise returns -1"""
     if l_bound is None and r_bound is None:
         l_bound = 0
         r_bound = len(x) - 1
@@ -172,35 +172,36 @@
 def _create_memmap(
     filename: str,
     mode: str = "r",
     shape: Tuple = (1,),
     dtype: np.dtype = np.float32,
     offset: int = 0,
     order: str = "C",
-) -> NDArray:
+) -> np.ndarray:
     """Wrapper to support empty array as memmaps
 
     Keyword arguments:
         filename -- filename where the empty memmap should be created
         mode -- file open mode (see: np.memmap for options)
-        shape -- shape of memmapped NDArray
-        dtype -- datatype of memmapped NDArray
+        shape -- shape of memmapped np.ndarray
+        dtype -- datatype of memmapped np.ndarray
         offset -- offset of the data within the file
         order -- data representation on disk (C or Fortran)
 
     Returns:
-        mmapped NDArray or a zero-filled Numpy array if array has a shape of 0
+        mmapped np.ndarray or a zero-filled Numpy array if array has a shape of 0
             in the first dimension
     """
     if np.dtype(dtype) == bool:
         filename = filename.replace(".bool", ".bit")
 
     if shape[0]:
         return np.memmap(
-            filename, mode=mode, offset=offset, shape=shape, dtype=dtype, order=order
+            filename, mode=mode, offset=offset, shape=shape, dtype=dtype,
+            order=order
         )
     else:
         if not os.path.isfile(filename):
             f = open(filename, "wb")
             f.close()
         return np.zeros(shape, dtype=dtype)
 
@@ -211,15 +212,15 @@
     Keyword arguments:
     input_obj -- A directory name or filepath to the trx data
     check_dpg -- Boolean denoting if group metadata should be checked
 
     Returns:
         TrxFile object representing the read data
     """
-    # TODO Check if 0 streamlines, if yes then 0 vertices is expected (vice-versa)
+    # TODO Check if 0 streamlines, then 0 vertices is expected (vice-versa)
     # TODO 4x4 affine matrices should contains values (no all-zeros)
     # TODO 3x1 dimensions array should contains values at each position (int)
     if os.path.isfile(input_obj):
         was_compressed = False
         with zipfile.ZipFile(input_obj, "r") as zf:
             for info in zf.infolist():
                 if info.compress_type != 0:
@@ -228,15 +229,16 @@
         if was_compressed:
             with zipfile.ZipFile(input_obj, "r") as zf:
                 tmpdir = get_trx_tmpdir()
                 zf.extractall(tmpdir.name)
                 trx = load_from_directory(tmpdir.name)
                 trx._uncompressed_folder_handle = tmpdir
                 logging.info(
-                    "File was compressed, call the close() " "function before exiting."
+                    "File was compressed, call the close() " "function before"
+                    "exiting."
                 )
         else:
             trx = load_from_zip(input_obj)
     elif os.path.isdir(input_obj):
         trx = load_from_directory(input_obj)
     else:
         raise ValueError("File/Folder does not exist")
@@ -250,15 +252,16 @@
                         dpg)
                 )
 
     return trx
 
 
 def load_from_zip(filename: str) -> Type["TrxFile"]:
-    """Load a TrxFile from a single zipfile. Note: does not work with compressed zipfiles
+    """Load a TrxFile from a single zipfile. Note: does not work with
+    compressed zipfiles
 
     Keyword arguments:
     filename -- path of the zipped TrxFile
 
     Returns:
         TrxFile representing the read data
     """
@@ -312,17 +315,16 @@
     Returns:
         TrxFile representing the read data
     """
 
     directory = os.path.abspath(directory)
     with open(os.path.join(directory, "header.json")) as header:
         header = json.load(header)
-        header["VOXEL_TO_RASMM"] = np.reshape(header["VOXEL_TO_RASMM"], (4, 4)).astype(
-            np.float32
-        )
+        header["VOXEL_TO_RASMM"] = np.reshape(header["VOXEL_TO_RASMM"],
+                                              (4, 4)).astype(np.float32)
         header["DIMENSIONS"] = np.array(header["DIMENSIONS"], dtype=np.uint16)
     files_pointer_size = {}
     for root, dirs, files in os.walk(directory):
         for name in files:
             elem_filename = os.path.join(root, name)
             _, ext = os.path.splitext(elem_filename)
             if ext == ".json":
@@ -342,15 +344,16 @@
             if size.is_integer():
                 files_pointer_size[elem_filename] = 0, int(size)
             elif os.path.getsize(elem_filename) == 1:
                 files_pointer_size[elem_filename] = 0, 0
             else:
                 raise ValueError("Wrong size or datatype")
 
-    return TrxFile._create_trx_from_pointer(header, files_pointer_size, root=directory)
+    return TrxFile._create_trx_from_pointer(header, files_pointer_size,
+                                            root=directory)
 
 
 def concatenate(
     trx_list: List["TrxFile"],
     delete_dpv: bool = False,
     delete_dps: bool = False,
     delete_groups: bool = False,
@@ -417,16 +420,14 @@
                     )
                     raise ValueError(
                         "TrxFile must be sharing identical dpv " "keys.")
             elif (
                 ref_trx.data_per_vertex[key]._data.dtype
                 != curr_trx.data_per_vertex[key]._data.dtype
             ):
-                print(key, ref_trx.data_per_vertex[key]._data.dtype,
-                      curr_trx.data_per_vertex[key]._data.dtype)
                 logging.debug(
                     "{} dpv key is not declared with the same dtype "
                     "in all TrxFile.".format(key)
                 )
                 raise ValueError("Shared dpv key, has different dtype.")
 
     for curr_trx in trx_list:
@@ -476,15 +477,16 @@
         nb_streamlines = 0
         for curr_trx in to_concat_list:
             curr_strs_len, curr_pts_len = curr_trx._get_real_len()
             nb_streamlines += curr_strs_len
             nb_vertices += curr_pts_len
 
         new_trx = TrxFile(
-            nb_vertices=nb_vertices, nb_streamlines=nb_streamlines, init_as=ref_trx
+            nb_vertices=nb_vertices, nb_streamlines=nb_streamlines,
+            init_as=ref_trx
         )
         if delete_dps:
             new_trx.data_per_streamline = {}
         if delete_dpv:
             new_trx.data_per_vertex = {}
         if delete_groups:
             new_trx.groups = {}
@@ -506,16 +508,16 @@
             )
             if delete_groups:
                 continue
             pos = 0
             count = 0
             for curr_trx in trx_list:
                 curr_len = len(curr_trx.groups[group_key])
-                new_trx.groups[group_key][pos: pos +
-                                          curr_len] = curr_trx.groups[group_key] + count
+                new_trx.groups[group_key][pos: pos + curr_len] = \
+                    curr_trx.groups[group_key] + count
                 pos += curr_len
                 count += curr_trx.header["NB_STREAMLINES"]
 
         strs_end, pts_end = 0, 0
     else:
         new_trx = ref_trx
         strs_end, pts_end = new_trx._get_real_len()
@@ -850,18 +852,20 @@
     ) -> Tuple[int, int]:
         """Fill a TrxFile using another and start indexes (preallocation)
 
         Keyword arguments:
             trx -- TrxFile to copy data from
             strs_start -- The start index of the streamline
             pts_start -- The start index of the point
-            nb_strs_to_copy -- The number of streamlines to copy. If not set will copy all
+            nb_strs_to_copy -- The number of streamlines to copy. If not set
+                                will copy all
 
         Returns
-            A tuple representing the end of the copied streamlines and end of copied points
+            A tuple representing the end of the copied streamlines and end of
+                copied points
         """
         if nb_strs_to_copy is None:
             curr_strs_len, curr_pts_len = trx._get_real_len()
         else:
             curr_strs_len = int(nb_strs_to_copy)
             curr_pts_len = np.sum(trx.streamlines._lengths[0:curr_strs_len])
             curr_pts_len = int(curr_pts_len)
@@ -869,23 +873,20 @@
         strs_end = strs_start + curr_strs_len
         pts_end = pts_start + curr_pts_len
 
         if curr_pts_len == 0:
             return strs_start, pts_start
 
         # Mandatory arrays
-        self.streamlines._data[pts_start:pts_end] = trx.streamlines._data[
-            0:curr_pts_len
-        ]
-        self.streamlines._offsets[strs_start:strs_end] = (
-            trx.streamlines._offsets[0:curr_strs_len] + pts_start
-        )
-        self.streamlines._lengths[strs_start:strs_end] = trx.streamlines._lengths[
-            0:curr_strs_len
-        ]
+        self.streamlines._data[pts_start:pts_end] = \
+            trx.streamlines._data[0:curr_pts_len]
+        self.streamlines._offsets[strs_start:strs_end] = \
+            (trx.streamlines._offsets[0:curr_strs_len] + pts_start)
+        self.streamlines._lengths[strs_start:strs_end] = \
+            trx.streamlines._lengths[0:curr_strs_len]
 
         # Optional fixed-sized arrays
         for dpv_key in self.data_per_vertex.keys():
             self.data_per_vertex[dpv_key]._data[
                 pts_start:pts_end
             ] = trx.data_per_vertex[dpv_key]._data[0:curr_pts_len]
             self.data_per_vertex[dpv_key]._offsets = self.streamlines._offsets
@@ -896,16 +897,16 @@
                 strs_start:strs_end
             ] = trx.data_per_streamline[dps_key][0:curr_strs_len]
 
         return strs_end, pts_end
 
     @staticmethod
     def _initialize_empty_trx(
-        nb_streamlines: int, nb_vertices: int, init_as: Optional[Type["TrxFile"]] = None
-    ) -> Type["TrxFile"]:
+            nb_streamlines: int, nb_vertices: int,
+            init_as: Optional[Type["TrxFile"]] = None) -> Type["TrxFile"]:
         """Create on-disk memmaps of a certain size (preallocation)
 
         Keyword arguments:
             nb_streamlines -- The number of streamlines that the empty TrxFile
                 will be initialized with
             nb_vertices -- The number of vertices that the empty TrxFile will
                 be initialized with
@@ -942,22 +943,24 @@
             "Initializing lengths with dtype: {}".format(lengths_dtype.name))
 
         # A TrxFile without init_as only contain the essential arrays
         positions_filename = os.path.join(
             tmp_dir.name, "positions.3.{}".format(positions_dtype.name)
         )
         trx.streamlines._data = _create_memmap(
-            positions_filename, mode="w+", shape=(nb_vertices, 3), dtype=positions_dtype
+            positions_filename, mode="w+", shape=(nb_vertices, 3),
+            dtype=positions_dtype
         )
 
         offsets_filename = os.path.join(
             tmp_dir.name, "offsets.{}".format(offsets_dtype.name)
         )
         trx.streamlines._offsets = _create_memmap(
-            offsets_filename, mode="w+", shape=(nb_streamlines,), dtype=offsets_dtype
+            offsets_filename, mode="w+", shape=(nb_streamlines,),
+            dtype=offsets_dtype
         )
         trx.streamlines._lengths = np.zeros(
             shape=(nb_streamlines,), dtype=lengths_dtype
         )
 
         # Only the structure of fixed-size arrays is copied
         if init_as is not None:
@@ -1091,49 +1094,53 @@
                 nb_scalar = size / trx.header["NB_STREAMLINES"]
                 if not nb_scalar.is_integer() or nb_scalar != dim:
                     raise ValueError("Wrong dps size/dimensionality.")
                 else:
                     shape = (trx.header["NB_STREAMLINES"], int(nb_scalar))
 
                 trx.data_per_streamline[base] = _create_memmap(
-                    filename, mode="r+", offset=mem_adress, shape=shape, dtype=ext[1:]
+                    filename, mode="r+", offset=mem_adress, shape=shape,
+                    dtype=ext[1:]
                 )
             elif folder == "dpv":
                 nb_scalar = size / trx.header["NB_VERTICES"]
                 if not nb_scalar.is_integer() or nb_scalar != dim:
                     raise ValueError("Wrong dpv size/dimensionality.")
                 else:
                     shape = (trx.header["NB_VERTICES"], int(nb_scalar))
 
                 trx.data_per_vertex[base] = _create_memmap(
-                    filename, mode="r+", offset=mem_adress, shape=shape, dtype=ext[1:]
+                    filename, mode="r+", offset=mem_adress, shape=shape,
+                    dtype=ext[1:]
                 )
             elif folder.startswith("dpg"):
                 if int(size) != dim:
                     raise ValueError("Wrong dpg size/dimensionality.")
                 else:
                     shape = (1, int(size))
 
                 # Handle the two-layers architecture
                 data_name = os.path.basename(base)
                 sub_folder = os.path.basename(folder)
                 if sub_folder not in trx.data_per_group:
                     trx.data_per_group[sub_folder] = {}
                 trx.data_per_group[sub_folder][data_name] = _create_memmap(
-                    filename, mode="r+", offset=mem_adress, shape=shape, dtype=ext[1:]
+                    filename, mode="r+", offset=mem_adress, shape=shape,
+                    dtype=ext[1:]
                 )
             elif folder == "groups":
                 # Groups are simply indices, nothing else
                 # TODO Crash if not uint?
                 if dim != 1:
                     raise ValueError("Wrong group dimensionality.")
                 else:
                     shape = (int(size),)
                 trx.groups[base] = _create_memmap(
-                    filename, mode="r+", offset=mem_adress, shape=shape, dtype=ext[1:]
+                    filename, mode="r+", offset=mem_adress, shape=shape,
+                    dtype=ext[1:]
                 )
             else:
                 logging.error(
                     "{} is not part of a valid structure.".format(
                         elem_filename)
                 )
 
@@ -1262,33 +1269,60 @@
                 shape = self.data_per_group[group_key][dpg_key].shape
                 if dpg_key not in trx.data_per_group[group_key]:
                     trx.data_per_group[group_key][dpg_key] = {}
                 trx.data_per_group[group_key][dpg_key] = _create_memmap(
                     dpg_filename, mode="w+", shape=shape, dtype=dpg_dtype
                 )
 
-                trx.data_per_group[group_key][dpg_key][:] = self.data_per_group[
-                    group_key
-                ][dpg_key]
+                trx.data_per_group[group_key][dpg_key][:] = \
+                    self.data_per_group[group_key][dpg_key]
 
         self.close()
         self.__dict__ = trx.__dict__
 
-    def append(self, obj: Union["StatefulTractogram", "TrxFile",
-                                "Tractogram", "LazyTractogram"],
-               extra_buffer: int = 0) -> None:
-
-        if not isinstance(obj, (StatefulTractogram, TrxFile,
-                                Tractogram)):
-            raise TypeError("{} is not a supported object type for appending.")
+    def get_dtype_dict(self):
+        """Get the dtype dictionary for the TrxFile
+
+        Returns
+            A dictionary containing the dtype for each data element
+        """
+        dtype_dict = {"positions": self.streamlines._data.dtype,
+                      "offsets": self.streamlines._offsets.dtype,
+                      "dpv": {}, "dps": {}, "dpg": {}, "groups": {}}
+
+        for key in self.data_per_vertex.keys():
+            dtype_dict['dpv'][key] = self.data_per_vertex[key]._data.dtype
+        for key in self.data_per_streamline.keys():
+            dtype_dict['dps'][key] = self.data_per_streamline[key].dtype
+
+        for group_key in self.data_per_group.keys():
+            dtype_dict['groups'][group_key] = self.groups[group_key].dtype
+
+        for group_key in self.data_per_group.keys():
+            dtype_dict['dpg'][group_key] = {}
+            for dpg_key in self.data_per_group[group_key].keys():
+                dtype_dict['dpg'][group_key][dpg_key] = \
+                    self.data_per_group[group_key][dpg_key].dtype
+
+        return dtype_dict
+
+    def append(self, obj, extra_buffer: int = 0) -> None:
+        curr_dtype_dict = self.get_dtype_dict()
+        if dipy_available:
+            from dipy.io.stateful_tractogram import StatefulTractogram
+
+        if not isinstance(obj, (TrxFile, Tractogram)) \
+                and (dipy_available and not isinstance(obj, StatefulTractogram)):
+            raise TypeError(
+                "{} is not a supported object type for appending.".format(type(obj)))
         elif isinstance(obj, Tractogram):
             obj = self.from_tractogram(obj, reference=self.header,
-                                       cast_position=np.float32)
-        elif isinstance(obj, StatefulTractogram):
-            obj = self.from_sft(obj, cast_position=np.float32)
+                                       dtype_dict=curr_dtype_dict)
+        elif dipy_available and isinstance(obj, StatefulTractogram):
+            obj = self.from_sft(obj, dtype_dict=curr_dtype_dict)
 
         self._append_trx(obj, extra_buffer=extra_buffer)
 
     def _append_trx(self, trx: Type["TrxFile"],
                     extra_buffer: int = 0) -> None:
         """Append a TrxFile to another (support buffer)
 
@@ -1323,15 +1357,15 @@
 
         Returns
             A TrxFile exclusively containing data from said group
         """
         return self.select(self.groups[key], keep_group=keep_group, copy_safe=copy_safe)
 
     def select(
-        self, indices: ArrayLike, keep_group: bool = True, copy_safe: bool = False
+        self, indices: np.ndarray, keep_group: bool = True, copy_safe: bool = False
     ) -> Type["TrxFile"]:
         """Get a subset of items, always vertices to the same memmaps
 
         Keyword arguments:
             indices -- The list of indices of elements to return
             keep_group -- Ensure group is returned in output TrxFile
             copy_safe -- Perform a deep-copy
@@ -1412,26 +1446,30 @@
         new_trx.header["NB_VERTICES"] = len(new_trx.streamlines._data)
         new_trx.header["NB_STREAMLINES"] = len(new_trx.streamlines._lengths)
         return new_trx.deepcopy() if copy_safe else new_trx
 
     @staticmethod
     def from_lazy_tractogram(obj: ["LazyTractogram"], reference,
                              extra_buffer: int = 0,
-                             chunk_size: int = 10000) -> None:
+                             chunk_size: int = 10000,
+                             dtype_dict: dict = {'positions': np.float32,
+                                                 'offsets': np.uint32,
+                                                 'dpv': {}, 'dps': {}}) \
+            -> Type["TrxFile"]:
         """Append a TrxFile to another (support buffer)
 
         Keyword arguments:
             trx -- The TrxFile to append to the current TrxFile
             extra_buffer -- The buffer space between reallocation.
                             This number should be a number of streamlines.
                             Use 0 for no buffer.
             chunk_size -- The number of streamlines to save at a time.
         """
 
-        data = {'strs': [], 'dpp': {}, 'dps': {}}
+        data = {'strs': [], 'dpv': {}, 'dps': {}}
         concat = None
         count = 0
         iterator = iter(obj)
         while True:
             if count < chunk_size:
                 try:
                     i = next(iterator)
@@ -1439,44 +1477,64 @@
                 except StopIteration:
                     obj = convert_data_dict_to_tractogram(data)
                     if concat is None:
                         if len(obj.streamlines) == 0:
                             concat = TrxFile()
                         else:
                             concat = TrxFile.from_tractogram(obj,
-                                                             reference=reference)
+                                                             reference=reference,
+                                                             dtype_dict=dtype_dict)
                     elif len(obj.streamlines) > 0:
                         curr_obj = TrxFile.from_tractogram(obj,
-                                                           reference=reference)
+                                                           reference=reference,
+                                                           dtype_dict=dtype_dict)
                         concat.append(curr_obj)
                     break
                 append_generator_to_dict(i, data)
             else:
                 obj = convert_data_dict_to_tractogram(data)
                 if concat is None:
-                    concat = TrxFile.from_tractogram(obj, reference=reference)
+                    concat = TrxFile.from_tractogram(obj,
+                                                     reference=reference,
+                                                     dtype_dict=dtype_dict)
                 else:
                     curr_obj = TrxFile.from_tractogram(obj,
-                                                       reference=reference)
+                                                       reference=reference,
+                                                       dtype_dict=dtype_dict)
                     concat.append(curr_obj, extra_buffer=extra_buffer)
-                data = {'strs': [], 'dpp': {}, 'dps': {}}
+                data = {'strs': [], 'dpv': {}, 'dps': {}}
                 count = 0
 
         concat.resize()
         return concat
 
     @staticmethod
-    def from_sft(sft, cast_position=np.float32):
+    def from_sft(sft, dtype_dict={}):
         """Generate a valid TrxFile from a StatefulTractogram"""
 
-        if not np.issubdtype(cast_position, np.floating):
+        if len(sft.dtype_dict) > 0:
+            dtype_dict = sft.dtype_dict
+        if 'dpp' in dtype_dict:
+            dtype_dict['dpv'] = dtype_dict.pop('dpp')
+        elif len(dtype_dict) == 0:
+            dtype_dict = {'positions': np.float32, 'offsets': np.uint32,
+                          'dpv': {}, 'dps': {}}
+
+        positions_dtype = dtype_dict['positions']
+        offsets_dtype = dtype_dict['offsets']
+
+        if not np.issubdtype(positions_dtype, np.floating):
             logging.warning(
-                "Casting as {}, considering using a floating point "
-                "dtype.".format(cast_position)
-            )
+                "Casting positions as {}, considering using a floating point "
+                "dtype.".format(positions_dtype))
+
+        if not np.issubdtype(offsets_dtype, np.integer):
+            logging.warning(
+                "Casting offsets as {}, considering using a integer "
+                "dtype.".format(offsets_dtype))
 
         trx = TrxFile(nb_vertices=len(sft.streamlines._data),
                       nb_streamlines=len(sft.streamlines))
         trx.header = {
             "DIMENSIONS": sft.dimensions.tolist(),
             "VOXEL_TO_RASMM": sft.affine.tolist(),
             "NB_VERTICES": len(sft.streamlines._data),
@@ -1485,79 +1543,112 @@
 
         old_space = deepcopy(sft.space)
         old_origin = deepcopy(sft.origin)
 
         # TrxFile are written on disk in RASMM/center convention
         sft.to_rasmm()
         sft.to_center()
-        if cast_position != np.float32:
-            tmp_streamlines = deepcopy(sft.streamlines)
-        else:
-            tmp_streamlines = sft.streamlines
-        sft.to_space(old_space)
-        sft.to_origin(old_origin)
+
+        tmp_streamlines = deepcopy(sft.streamlines)
 
         # Cast the int64 of Nibabel to uint32
-        tmp_streamlines._offsets = tmp_streamlines._offsets.astype(np.uint32)
-        if cast_position != np.float32:
-            tmp_streamlines._data = tmp_streamlines._data.astype(cast_position)
+        tmp_streamlines._offsets = tmp_streamlines._offsets.astype(
+            offsets_dtype)
+        tmp_streamlines._data = tmp_streamlines._data.astype(positions_dtype)
 
         trx.streamlines = tmp_streamlines
-        trx.data_per_streamline = sft.data_per_streamline
-        trx.data_per_vertex = sft.data_per_point
+        for key in sft.data_per_point:
+            dtype_to_use = dtype_dict['dpv'][key] if key in dtype_dict['dpv'] \
+                else np.float32
+            trx.data_per_vertex[key] = \
+                sft.data_per_point[key]
+            trx.data_per_vertex[key]._data = \
+                sft.data_per_point[key]._data.astype(dtype_to_use)
+
+        for key in sft.data_per_streamline:
+            dtype_to_use = dtype_dict['dps'][key] if key in dtype_dict['dps'] \
+                else np.float32
+            trx.data_per_streamline[key] = sft.data_per_streamline[key].astype(
+                dtype_to_use)
 
         # For safety and for RAM, convert the whole object to memmaps
         tmpdir = get_trx_tmpdir()
         save(trx, tmpdir.name)
         trx = load_from_directory(tmpdir.name)
         trx._uncompressed_folder_handle = tmpdir
 
+        sft.to_space(old_space)
+        sft.to_origin(old_origin)
+        del tmp_streamlines
+
         return trx
 
     @staticmethod
-    def from_tractogram(tractogram, reference, cast_position=np.float32):
+    def from_tractogram(tractogram, reference,
+                        dtype_dict={'positions': np.float32,
+                                    'offsets': np.uint32,
+                                    'dpv': {}, 'dps': {}}):
         """Generate a valid TrxFile from a Nibabel Tractogram"""
-        if not np.issubdtype(cast_position, np.floating):
+
+        positions_dtype = dtype_dict['positions'] if 'positions' in dtype_dict \
+            else np.float32
+        offsets_dtype = dtype_dict['offsets'] if 'offsets' in dtype_dict \
+            else np.uint32
+
+        if not np.issubdtype(positions_dtype, np.floating):
             logging.warning(
-                "Casting as {}, considering using a floating point "
-                "dtype.".format(cast_position)
-            )
+                "Casting positions as {}, considering using a floating point "
+                "dtype.".format(positions_dtype))
+
+        if not np.issubdtype(offsets_dtype, np.integer):
+            logging.warning(
+                "Casting offsets as {}, considering using a integer "
+                "dtype.".format(offsets_dtype))
 
         trx = TrxFile(
             nb_vertices=len(tractogram.streamlines._data),
             nb_streamlines=len(tractogram.streamlines),
         )
 
         affine, dimensions, _, _ = get_reference_info_wrapper(reference)
         trx.header = {
             "DIMENSIONS": dimensions,
             "VOXEL_TO_RASMM": affine,
             "NB_VERTICES": len(tractogram.streamlines._data),
             "NB_STREAMLINES": len(tractogram.streamlines),
         }
 
-        if cast_position != np.float32:
-            tmp_streamlines = deepcopy(tractogram.streamlines)
-        else:
-            tmp_streamlines = tractogram.streamlines
+        tmp_streamlines = deepcopy(tractogram.streamlines)
 
         # Cast the int64 of Nibabel to uint32
-        tmp_streamlines._offsets = tmp_streamlines._offsets.astype(np.uint32)
-        if cast_position != np.float32:
-            tmp_streamlines._data = tmp_streamlines._data.astype(cast_position)
+        tmp_streamlines._offsets = tmp_streamlines._offsets.astype(
+            offsets_dtype)
+        tmp_streamlines._data = tmp_streamlines._data.astype(positions_dtype)
 
         trx.streamlines = tmp_streamlines
-        trx.data_per_streamline = tractogram.data_per_streamline
-        trx.data_per_vertex = tractogram.data_per_point
+        for key in tractogram.data_per_point:
+            dtype_to_use = dtype_dict['dpv'][key] if key in dtype_dict['dpv'] \
+                else np.float32
+            trx.data_per_vertex[key] = \
+                tractogram.data_per_point[key]
+            trx.data_per_vertex[key]._data = \
+                tractogram.data_per_point[key]._data.astype(dtype_to_use)
+
+        for key in tractogram.data_per_streamline:
+            dtype_to_use = dtype_dict['dps'][key] if key in dtype_dict['dps'] \
+                else np.float32
+            trx.data_per_streamline[key] = \
+                tractogram.data_per_streamline[key].astype(dtype_to_use)
 
         # For safety and for RAM, convert the whole object to memmaps
         tmpdir = get_trx_tmpdir()
         save(trx, tmpdir.name)
         trx = load_from_directory(tmpdir.name)
         trx._uncompressed_folder_handle = tmpdir
+        del tmp_streamlines
 
         return trx
 
     def to_tractogram(self, resize=False):
         """Convert a TrxFile to a nibabel Tractogram (in RAM)"""
         if resize:
             self.resize()
@@ -1621,14 +1712,18 @@
         sft = StatefulTractogram(
             self.streamlines,
             space_attributes,
             Space.RASMM,
             data_per_point=self.data_per_vertex,
             data_per_streamline=self.data_per_streamline,
         )
+        tmp_dict = self.get_dtype_dict()
+        if 'dpv' in tmp_dict:
+            tmp_dict['dpp'] = tmp_dict.pop('dpv')
+        sft.dtype_dict = self.get_dtype_dict()
 
         return sft
 
     def close(self) -> None:
         """Cleanup on-disk temporary folder and initialize an empty TrxFile"""
         if self._uncompressed_folder_handle is not None:
             self._uncompressed_folder_handle.cleanup()
```

### Comparing `trx-python-0.1/trx/utils.py` & `trx-python-0.1.2/trx/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 import logging
 
 import nibabel as nib
 import numpy as np
 
 try:
     import dipy
-    from dipy.io.stateful_tractogram import StatefulTractogram, Space, Origin
-    from dipy.io.streamline import load_tractogram
-    from dipy.io.utils import is_reference_info_valid
     dipy_available = True
 except ImportError:
     dipy_available = False
 
 
 def split_name_with_gz(filename):
     """
@@ -128,14 +125,15 @@
     else:
         raise TypeError('Input reference is not one of the supported format')
 
     if isinstance(voxel_order, np.bytes_):
         voxel_order = voxel_order.decode('utf-8')
 
     if dipy_available:
+        from dipy.io.utils import is_reference_info_valid
         is_reference_info_valid(affine, dimensions, voxel_sizes, voxel_order)
 
     return affine, dimensions, voxel_sizes, voxel_order
 
 
 def is_header_compatible(reference_1, reference_2):
     """ Will compare the spatial attribute of 2 references.
@@ -175,58 +173,14 @@
     if voxel_order_1 != voxel_order_2:
         logging.error('Voxel_order not equal')
         identical_header = False
 
     return identical_header
 
 
-def load_tractogram_with_reference(filepath, reference=None,
-                                   bbox_check=True):
-    """ Load a tractogram with a reference (if required).
-
-    Parameters
-    ----------
-    filepath : str
-        Path to the tractogram file.
-    reference : Nifti or Trk filename, Nifti1Image or TrkFile,
-        Nifti1Header or trk.header (dict)
-        Reference that provides the spatial attribute.
-    bbox_check : bool
-        Check if the tractogram is inside the bounding box of the reference.
-    Returns
-    -------
-    output : dipy.io.stateful_tractogram.StatefulTractogram
-        Tractogram object.
-    """
-    if not dipy_available:
-        logging.error('Dipy library is missing, cannot use functions related '
-                      'to the StatefulTractogram.')
-        return None
-    # Force the usage of --reference for all file formats without an header
-    _, ext = os.path.splitext(filepath)
-    if ext == '.trk':
-        if reference is not None and reference != 'same':
-            logging.warning('Reference is discarded for this file format '
-                            '{}.'.format(filepath))
-        sft = load_tractogram(filepath, 'same',
-                              bbox_valid_check=bbox_check)
-    elif ext in ['.tck', '.fib', '.vtk', '.dpy']:
-        if reference is None or reference == 'same':
-            raise IOError('--reference is required for this file format '
-                          '{}.'.format(filepath))
-        else:
-            sft = load_tractogram(filepath, reference,
-                                  bbox_valid_check=bbox_check)
-
-    else:
-        raise IOError('{} is an unsupported file format'.format(filepath))
-
-    return sft
-
-
 def get_axis_shift_vector(flip_axes):
     """
     Parameters
     ----------
     flip_axes : list of str
         String containing the axis to flip.
         Possible values are 'x', 'y', 'z'
@@ -319,14 +273,15 @@
     flipped_streamlines = []
     for streamline in sft.streamlines:
         mod_streamline = streamline + shift_vector
         mod_streamline *= flip_vector
         mod_streamline -= shift_vector
         flipped_streamlines.append(mod_streamline)
 
+    from dipy.io.stateful_tractogram import StatefulTractogram
     new_sft = StatefulTractogram.from_sft(flipped_streamlines, sft,
                                           data_per_point=sft.data_per_point,
                                           data_per_streamline=sft.data_per_streamline)
     return new_sft
 
 
 def load_matrix_in_any_format(filepath):
@@ -365,14 +320,16 @@
     -------
     output : str
         Space and Origin as Enums.
     """
     if not dipy_available:
         logging.error('Dipy library is missing, cannot use functions related '
                       'to the StatefulTractogram.')
+        return None
+    from dipy.io.stateful_tractogram import Space, Origin
     origin = Origin.NIFTI if origin_str.lower() == 'nifti' else Origin.TRACKVIS
     if space_str.lower() == 'rasmm':
         space = Space.RASMM
     elif space_str.lower() == 'voxmm':
         space = Space.VOXMM
     else:
         space = Space.VOX
@@ -389,39 +346,96 @@
     Returns:
         A Tractogram object
     """
     streamlines = ArraySequence(data['strs'])
     streamlines._data = streamlines._data
 
     for key in data['dps']:
-        data['dps'][key] = np.array(data['dps'][key])
+        shape = (len(streamlines), len(data['dps'][key]) // len(streamlines))
+        data['dps'][key] = np.array(data['dps'][key]).reshape(shape)
 
-    data['data_per_point'] = {}
-    for key in data['dpp']:
-        if key not in data['data_per_point']:
-            tmp_arr = ArraySequence()
-            tmp_arr._data = data['dpp'][key]
-            tmp_arr._offsets = streamlines._offsets
-            tmp_arr._lengths = streamlines._lengths
-            data['data_per_point'][key] = tmp_arr
+    for key in data['dpv']:
+        shape = (len(streamlines._data), len(
+            data['dpv'][key]) // len(streamlines._data))
+        data['dpv'][key] = np.array(data['dpv'][key]).reshape(shape)
+
+        tmp_arr = ArraySequence()
+        tmp_arr._data = data['dpv'][key]
+        tmp_arr._offsets = streamlines._offsets
+        tmp_arr._lengths = streamlines._lengths
+        data['dpv'][key] = tmp_arr
 
-    obj = Tractogram(streamlines, data_per_point=data['data_per_point'],
+    obj = Tractogram(streamlines, data_per_point=data['dpv'],
                      data_per_streamline=data['dps'])
 
     return obj
 
 
 def append_generator_to_dict(gen, data):
     if isinstance(gen, TractogramItem):
         data['strs'].append(gen.streamline.tolist())
         for key in gen.data_for_points:
-            if key not in data['dpp']:
-                data['dpp'][key] = np.array([])
-            data['dpp'][key] = np.append(
-                data['dpp'][key], gen.data_for_points[key])
+            if key not in data['dpv']:
+                data['dpv'][key] = np.array([])
+            data['dpv'][key] = np.append(
+                data['dpv'][key], gen.data_for_points[key])
         for key in gen.data_for_streamline:
             if key not in data['dps']:
                 data['dps'][key] = np.array([])
             data['dps'][key] = np.append(
                 data['dps'][key], gen.data_for_streamline[key])
     else:
         data['strs'].append(gen.tolist())
+
+
+def verify_trx_dtype(trx, dict_dtype):
+    """ Verify if the dtype of the data in the trx is the same as the one in
+    the dict.
+
+    Parameters
+    ----------
+    trx : Tractogram
+        Tractogram to verify.
+    dict_dtype : dict
+        Dictionary containing the dtype to verify.
+    Returns
+    -------
+    output : bool
+        True if the dtype is the same, False otherwise.
+    """
+    identical = True
+    for key in dict_dtype:
+        if key == 'positions':
+            if trx.streamlines._data.dtype != dict_dtype[key]:
+                logging.warning('Positions dtype is different')
+                identical = False
+        elif key == 'offsets':
+            if trx.streamlines._offsets.dtype != dict_dtype[key]:
+                logging.warning('Offsets dtype is different')
+                identical = False
+        elif key == 'dpv':
+            for key_dpv in dict_dtype[key]:
+                if trx.data_per_vertex[key_dpv]._data.dtype != dict_dtype[key][key_dpv]:
+                    logging.warning(
+                        'Data per vertex ({}) dtype is different'.format(key_dpv))
+                    identical = False
+        elif key == 'dps':
+            for key_dps in dict_dtype[key]:
+                if trx.data_per_streamline[key_dps].dtype != dict_dtype[key][key_dps]:
+                    logging.warning(
+                        'Data per streamline ({}) dtype is different'.format(key_dps))
+                    identical = False
+        elif key == 'dpg':
+            for key_group in dict_dtype[key]:
+                for key_dpg in dict_dtype[key][key_group]:
+                    if trx.data_per_point[key_group][key_dpg].dtype != dict_dtype[key][key_group][key_dpg]:
+                        logging.warning(
+                            'Data per group ({}) dtype is different'.format(key_dpg))
+                        identical = False
+        elif key == 'groups':
+            for key_group in dict_dtype[key]:
+                if trx.data_per_point[key_group]._data.dtype != dict_dtype[key][key_group]:
+                    logging.warning(
+                        'Data per group ({}) dtype is different'.format(key_group))
+                    identical = False
+
+    return identical
```

### Comparing `trx-python-0.1/trx/viz.py` & `trx-python-0.1.2/trx/viz.py`

 * *Files identical despite different names*

### Comparing `trx-python-0.1/trx/workflows.py` & `trx-python-0.1.2/trx/workflows.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 
 from copy import deepcopy
 import csv
 import gzip
 import json
 import logging
 import os
+import tempfile
 
 import nibabel as nib
 from nibabel.streamlines.array_sequence import ArraySequence
 import numpy as np
 try:
-    from dipy.io.stateful_tractogram import StatefulTractogram, Space
-    from dipy.io.streamline import save_tractogram, load_tractogram
-    from dipy.tracking.streamline import set_number_of_points
-    from dipy.tracking.utils import density_map
+    import dipy
     dipy_available = True
 except ImportError:
     dipy_available = False
 
 from trx.io import get_trx_tmpdir, load, load_sft_with_reference, save
 from trx.streamlines_ops import perform_streamlines_operation, intersection
 import trx.trx_file_memmap as tmm
@@ -33,14 +31,17 @@
 
 
 def convert_dsi_studio(in_dsi_tractogram, in_dsi_fa, out_tractogram,
                        remove_invalid=True, keep_invalid=False):
     if not dipy_available:
         logging.error('Dipy library is missing, scripts are not available.')
         return None
+    from dipy.io.stateful_tractogram import StatefulTractogram, Space
+    from dipy.io.streamline import save_tractogram, load_tractogram
+
     in_ext = split_name_with_gz(in_dsi_tractogram)[1]
     out_ext = split_name_with_gz(out_tractogram)[1]
 
     if in_ext == '.trk.gz':
         with gzip.open(in_dsi_tractogram, 'rb') as f_in:
             with open('tmp.trk', 'wb') as f_out:
                 f_out.writelines(f_in)
@@ -77,14 +78,16 @@
 
 
 def convert_tractogram(in_tractogram, out_tractogram, reference,
                        pos_dtype='float32', offsets_dtype='uint32'):
     if not dipy_available:
         logging.error('Dipy library is missing, scripts are not available.')
         return None
+    from dipy.io.streamline import save_tractogram
+
     in_ext = split_name_with_gz(in_tractogram)[1]
     out_ext = split_name_with_gz(out_tractogram)[1]
 
     if in_ext == out_ext:
         raise IOError('Input and output cannot be of the same file format.')
 
     if in_ext != '.trx':
@@ -114,14 +117,16 @@
         tmm.save(trx, out_tractogram)
 
 
 def tractogram_simple_compare(in_tractograms, reference):
     if not dipy_available:
         logging.error('Dipy library is missing, scripts are not available.')
         return
+    from dipy.io.stateful_tractogram import StatefulTractogram
+
     tractogram_obj = load(in_tractograms[0], reference)
     if not isinstance(tractogram_obj, StatefulTractogram):
         sft_1 = tractogram_obj.to_sft()
     else:
         sft_1 = tractogram_obj
 
     tractogram_obj = load(in_tractograms[1], reference)
@@ -156,14 +161,15 @@
             sft_1.streamlines._data - sft_2.streamlines._data, axis=0)))
 
 
 def verify_header_compatibility(in_files):
     if not dipy_available:
         logging.error('Dipy library is missing, scripts are not available.')
         return
+
     all_valid = True
     for filepath in in_files:
         if not os.path.isfile(filepath):
             print('{} does not exist'.format(filepath))
         _, in_extension = split_name_with_gz(filepath)
         if in_extension not in ['.trk', '.nii', '.nii.gz', '.trx']:
             raise IOError('{} does not have a supported extension'.format(
@@ -176,14 +182,17 @@
         print('All input files have compatible headers.')
 
 
 def tractogram_visualize_overlap(in_tractogram, reference, remove_invalid=True):
     if not dipy_available:
         logging.error('Dipy library is missing, scripts are not available.')
         return None
+    from dipy.io.stateful_tractogram import StatefulTractogram
+    from dipy.tracking.streamline import set_number_of_points
+    from dipy.tracking.utils import density_map
 
     tractogram_obj = load(in_tractogram, reference)
     if not isinstance(tractogram_obj, StatefulTractogram):
         sft = tractogram_obj.to_sft()
     else:
         sft = tractogram_obj
     sft.streamlines._data = sft.streamlines._data.astype(float)
@@ -218,22 +227,31 @@
 
     display(img.get_fdata(), volume_affine=affine,
             streamlines=sft.streamlines,  title='VOXMM')
 
 
 def validate_tractogram(in_tractogram, reference, out_tractogram,
                         remove_identical_streamlines=True, precision=1):
+
+    if not dipy_available:
+        logging.error('Dipy library is missing, scripts are not available.')
+        return None
+    from dipy.io.stateful_tractogram import StatefulTractogram
+
     tractogram_obj = load(in_tractogram, reference)
+
     if not isinstance(tractogram_obj, StatefulTractogram):
         sft = tractogram_obj.to_sft()
     else:
         sft = tractogram_obj
-    # print(sft)
+
+    ori_dtype = sft.dtype_dict
     ori_len = len(sft)
     tot_remove = 0
+
     invalid_coord_ind, _ = sft.remove_invalid_streamlines()
     tot_remove += len(invalid_coord_ind)
     logging.warning('Removed {} streamlines with invalid coordinates.'.format(
         len(invalid_coord_ind)))
 
     indices = [i for i in range(len(sft)) if len(sft.streamlines[i]) <= 1]
     tot_remove = + len(indices)
@@ -264,23 +282,24 @@
         indices_final = np.intersect1d(indices_val, indices_uniq)
     else:
         indices_final = indices_val
 
     if out_tractogram:
         streamlines = sft.streamlines[indices_final].copy()
         dpp = {}
-        for key in dpp.keys():
-            dpp[key] = sft.data_per_point[key][indices_final]
+        for key in sft.data_per_point.keys():
+            dpp[key] = sft.data_per_point[key][indices_final].copy()
 
         dps = {}
-        for key in dps.keys():
+        for key in sft.data_per_streamline.keys():
             dps[key] = sft.data_per_streamline[key][indices_final]
         new_sft = StatefulTractogram.from_sft(streamlines, sft,
                                               data_per_point=dpp,
                                               data_per_streamline=dps)
+        new_sft.dtype_dict = ori_dtype
         save(new_sft, out_tractogram)
 
 
 def generate_trx_from_scratch(reference, out_tractogram, positions_csv=False,
                               positions=False, offsets=False,
                               positions_dtype='float32', offsets_dtype='uint64',
                               space_str='rasmm', origin_str='nifti',
@@ -306,14 +325,15 @@
         if space_str.lower() != 'rasmm' or origin_str.lower() != 'nifti' or \
                 verify_invalid:
             if not dipy_available:
                 logging.error('Dipy library is missing, advanced options '
                               'related to spatial transforms and invalid '
                               'streamlines are not available.')
                 return
+            from dipy.io.stateful_tractogram import StatefulTractogram
 
             space, origin = get_reverse_enum(space_str, origin_str)
             sft = StatefulTractogram(streamlines, reference, space, origin)
             if verify_invalid:
                 rem, _ = sft.remove_invalid_streamlines()
                 print('{} streamlines were removed becaused they were '
                       'invalid.'.format(len(rem)))
@@ -406,7 +426,64 @@
                     curr_arr.shape[-1])
                 curr_filename = os.path.join(tmpdirname, 'dpg', arg[0], '{}.{}{}'.format(
                     os.path.basename(os.path.splitext(arg[1])[0]), dim, arg[2]))
                 curr_arr.tofile(curr_filename)
 
         trx = tmm.load(tmpdirname)
         tmm.save(trx, out_tractogram)
+
+
+def manipulate_trx_datatype(in_filename, out_filename, dict_dtype):
+    trx = tmm.load(in_filename)
+
+    # For each key in dict_dtype, we create a new memmap with the new dtype
+    # and we copy the data from the old memmap to the new one.
+    for key in dict_dtype:
+        if key == 'positions':
+            tmp_mm = np.memmap(tempfile.NamedTemporaryFile(),
+                               dtype=dict_dtype[key],
+                               mode='w+',
+                               shape=trx.streamlines._data.shape)
+            tmp_mm[:] = trx.streamlines._data[:]
+            trx.streamlines._data = tmp_mm
+        elif key == 'offsets':
+            tmp_mm = np.memmap(tempfile.NamedTemporaryFile(),
+                               dtype=dict_dtype[key],
+                               mode='w+',
+                               shape=trx.streamlines._offsets.shape)
+            tmp_mm[:] = trx.streamlines._offsets[:]
+            trx.streamlines._offsets = tmp_mm
+        elif key == 'dpv':
+            for key_dpv in dict_dtype[key]:
+                tmp_mm = np.memmap(tempfile.NamedTemporaryFile(),
+                                   dtype=dict_dtype[key][key_dpv],
+                                   mode='w+',
+                                   shape=trx.data_per_vertex[key_dpv]._data.shape)
+                tmp_mm[:] = trx.data_per_vertex[key_dpv]._data[:]
+                trx.data_per_vertex[key_dpv]._data = tmp_mm
+        elif key == 'dps':
+            for key_dps in dict_dtype[key]:
+                tmp_mm = np.memmap(tempfile.NamedTemporaryFile(),
+                                   dtype=dict_dtype[key][key_dps],
+                                   mode='w+',
+                                   shape=trx.data_per_streamline[key_dps].shape)
+                tmp_mm[:] = trx.data_per_streamline[key_dps][:]
+                trx.data_per_streamline[key_dps] = tmp_mm
+        elif key == 'dpg':
+            for key_group in dict_dtype[key]:
+                for key_dpg in dict_dtype[key][key_group]:
+                    tmp_mm = np.memmap(tempfile.NamedTemporaryFile(),
+                                       dtype=dict_dtype[key][key_group][key_dpg],
+                                       mode='w+',
+                                       shape=trx.data_per_group[key_group][key_dpg].shape)
+                    tmp_mm[:] = trx.data_per_group[key_group][key_dpg][:]
+                    trx.data_per_group[key_group][key_dpg] = tmp_mm
+        elif key == 'groups':
+            for key_group in dict_dtype[key]:
+                tmp_mm = np.memmap(tempfile.NamedTemporaryFile(),
+                                   dtype=dict_dtype[key][key_group],
+                                   mode='w+',
+                                   shape=trx.groups[key_group].shape)
+                tmp_mm[:] = trx.groups[key_group][:]
+                trx.groups[key_group] = tmp_mm
+
+    tmm.save(trx, out_filename)
```

### Comparing `trx-python-0.1/trx_python.egg-info/PKG-INFO` & `trx-python-0.1.2/trx_python.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trx-python
-Version: 0.1
+Version: 0.1.2
 Summary: Experiments with new file format for tractography
 Home-page: https://github.com/tee-ar-ex/trx-python
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
@@ -31,14 +31,20 @@
 
 Or, to install from source:
 
     git clone https://github.com/tee-ar-ex/trx-python.git
     cd trx-python
     pip install .
 
+### Install Dipy for integration
+If you wish to use all the scripts and run the test you will need to install Dipy
+
+    pip install cython packaging
+    pip install dipy@git+https://git@github.com/frheault/dipy@ba3ce0c59#egg=dipy
+
 ### Temporary Directory
 The TRX file format uses memmaps to limit RAM usage. When dealing with large files this means several gigabytes could be required on disk (instead of RAM). 
 
 By default, the temporary directory on Linux and MacOS is `/tmp` and on Windows it should be `C:\WINDOWS\Temp`.
 
 If you wish to change the directory add the following variable to your script or to your .bashrc or .bash_profile:
 `export TRX_TMPDIR=/WHERE/I/WANT/MY/TMP/DATA` (a)
```

### Comparing `trx-python-0.1/trx_python.egg-info/SOURCES.txt` & `trx-python-0.1.2/trx_python.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 docs/_static/trx_logo.png
 docs/source/conf.py
 docs/source/index.rst
 scripts/tff_concatenate_tractograms.py
 scripts/tff_convert_dsi_studio.py
 scripts/tff_convert_tractogram.py
 scripts/tff_generate_trx_from_scratch.py
+scripts/tff_manipulate_datatype.py
 scripts/tff_simple_compare.py
 scripts/tff_validate_trx.py
 scripts/tff_verify_header_compatibility.py
 scripts/tff_visualize_overlap.py
 scripts/tests/test_workflows.py
 trx/__init__.py
 trx/_version.py
```

