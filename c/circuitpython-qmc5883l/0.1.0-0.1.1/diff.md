# Comparing `tmp/circuitpython-qmc5883l-0.1.0.tar.gz` & `tmp/circuitpython-qmc5883l-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-qmc5883l-0.1.0.tar", last modified: Sat Mar 25 18:08:08 2023, max compression
+gzip compressed data, was "circuitpython-qmc5883l-0.1.1.tar", last modified: Thu Apr 20 21:33:12 2023, max compression
```

## Comparing `circuitpython-qmc5883l-0.1.0.tar` & `circuitpython-qmc5883l-0.1.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 18:08:08.849207 circuitpython-qmc5883l-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 18:08:08.845207 circuitpython-qmc5883l-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 18:08:08.845207 circuitpython-qmc5883l-0.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 18:08:08.845207 circuitpython-qmc5883l-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 18:08:08.845207 circuitpython-qmc5883l-0.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-03-25 18:08:08.849207 circuitpython-qmc5883l-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 18:08:08.849207 circuitpython-qmc5883l-0.1.0/circuitpython_qmc5883l.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-03-25 18:08:08.000000 circuitpython-qmc5883l-0.1.0/circuitpython_qmc5883l.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-25 18:08:08.000000 circuitpython-qmc5883l-0.1.0/circuitpython_qmc5883l.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 18:08:08.000000 circuitpython-qmc5883l-0.1.0/circuitpython_qmc5883l.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-25 18:08:08.000000 circuitpython-qmc5883l-0.1.0/circuitpython_qmc5883l.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 18:08:08.000000 circuitpython-qmc5883l-0.1.0/circuitpython_qmc5883l.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 18:08:08.849207 circuitpython-qmc5883l-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 18:08:08.849207 circuitpython-qmc5883l-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 18:08:08.849207 circuitpython-qmc5883l-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-25 18:08:01.000000 circuitpython-qmc5883l-0.1.0/examples/qmc5883l_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-25 18:08:01.000000 circuitpython-qmc5883l-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-03-25 18:08:01.000000 circuitpython-qmc5883l-0.1.0/qmc5883l.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-25 18:07:52.000000 circuitpython-qmc5883l-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 18:08:08.849207 circuitpython-qmc5883l-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:33:12.554372 circuitpython-qmc5883l-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:33:12.546372 circuitpython-qmc5883l-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:33:12.550372 circuitpython-qmc5883l-0.1.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:33:12.550372 circuitpython-qmc5883l-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:33:12.550372 circuitpython-qmc5883l-0.1.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-20 21:33:12.554372 circuitpython-qmc5883l-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:33:12.550372 circuitpython-qmc5883l-0.1.1/circuitpython_qmc5883l.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-20 21:33:12.000000 circuitpython-qmc5883l-0.1.1/circuitpython_qmc5883l.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-20 21:33:12.000000 circuitpython-qmc5883l-0.1.1/circuitpython_qmc5883l.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:33:12.000000 circuitpython-qmc5883l-0.1.1/circuitpython_qmc5883l.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-20 21:33:12.000000 circuitpython-qmc5883l-0.1.1/circuitpython_qmc5883l.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 21:33:12.000000 circuitpython-qmc5883l-0.1.1/circuitpython_qmc5883l.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:33:12.554372 circuitpython-qmc5883l-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:33:12.554372 circuitpython-qmc5883l-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:33:12.554372 circuitpython-qmc5883l-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-20 21:33:03.000000 circuitpython-qmc5883l-0.1.1/examples/qmc5883l_advanced_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-20 21:33:03.000000 circuitpython-qmc5883l-0.1.1/examples/qmc5883l_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-20 21:33:03.000000 circuitpython-qmc5883l-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-20 21:33:03.000000 circuitpython-qmc5883l-0.1.1/qmc5883l.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 21:32:51.000000 circuitpython-qmc5883l-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 21:33:12.554372 circuitpython-qmc5883l-0.1.1/setup.cfg
```

### Comparing `circuitpython-qmc5883l-0.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-qmc5883l-0.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.0/.gitignore` & `circuitpython-qmc5883l-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.0/.pre-commit-config.yaml` & `circuitpython-qmc5883l-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.0/.pylintrc` & `circuitpython-qmc5883l-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.0/CODE_OF_CONDUCT.md` & `circuitpython-qmc5883l-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.0/LICENSE` & `circuitpython-qmc5883l-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-qmc5883l-0.1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.0/LICENSES/MIT.txt` & `circuitpython-qmc5883l-0.1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.0/LICENSES/Unlicense.txt` & `circuitpython-qmc5883l-0.1.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.0/PKG-INFO` & `circuitpython-qmc5883l-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-qmc5883l
-Version: 0.1.0
+Version: 0.1.1
 Summary: CircuitPython driver for the qmc5883l magnetometer
 Author-email: "Jose D. Montoya" <qmc@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_qmc5883l
 Keywords: adafruit,blinka,circuitpython,micropython,qmc5883l,magnetometer,driver,sensor,qmc5883l
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-qmc5883l-0.1.0/README.rst` & `circuitpython-qmc5883l-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.0/circuitpython_qmc5883l.egg-info/PKG-INFO` & `circuitpython-qmc5883l-0.1.1/circuitpython_qmc5883l.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-qmc5883l
-Version: 0.1.0
+Version: 0.1.1
 Summary: CircuitPython driver for the qmc5883l magnetometer
 Author-email: "Jose D. Montoya" <qmc@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_qmc5883l
 Keywords: adafruit,blinka,circuitpython,micropython,qmc5883l,magnetometer,driver,sensor,qmc5883l
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-qmc5883l-0.1.0/circuitpython_qmc5883l.egg-info/SOURCES.txt` & `circuitpython-qmc5883l-0.1.1/circuitpython_qmc5883l.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/qmc5883l_advanced_settings.py
 examples/qmc5883l_simpletest.py
```

### Comparing `circuitpython-qmc5883l-0.1.0/docs/_static/favicon.ico` & `circuitpython-qmc5883l-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.0/docs/conf.py` & `circuitpython-qmc5883l-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.0/docs/index.rst` & `circuitpython-qmc5883l-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-qmc5883l-0.1.0/examples/qmc5883l_simpletest.py` & `circuitpython-qmc5883l-0.1.1/examples/qmc5883l_advanced_settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 # pylint: disable=protected-access
-import time
 import board
-import circuitpython_qmc5883l as qmc5883
+import qmc5883l
 
 
 i2c = board.I2C()
-qmc = qmc5883.QMC5883L(i2c)
+qmc = qmc5883l.QMC5883L(i2c)
 
 print("Initial Configuration register", bin(qmc._conf_reg))
 print("Setting Oversample to 64(0b11)")
-qmc.oversample = qmc5883.OVERSAMPLE_64
+qmc.oversample = qmc5883l.OVERSAMPLE_64
 print("Configuration register", bin(qmc._conf_reg))
 print("Setting Oversample to 128(0b10)")
-qmc.oversample = qmc5883.OVERSAMPLE_128
+qmc.oversample = qmc5883l.OVERSAMPLE_128
 print("Configuration register", bin(qmc._conf_reg))
 print("Setting Oversample to 2G (0b00)")
-qmc.field_range = qmc5883.FIELDRANGE_2G
+qmc.field_range = qmc5883l.FIELDRANGE_2G
 print("Configuration register", bin(qmc._conf_reg))
 print("Setting Range to 8G (0b01)")
-qmc.field_range = qmc5883.FIELDRANGE_8G
+qmc.field_range = qmc5883l.FIELDRANGE_8G
 print("Configuration register", bin(qmc._conf_reg))
 print("setting ouput Data Rate 100HZ (0b10)")
-qmc.output_data_rate = qmc5883.OUTPUT_DATA_RATE_100
+qmc.output_data_rate = qmc5883l.OUTPUT_DATA_RATE_100
 print("Configuration register", bin(qmc._conf_reg))
 print("setting ouput Data Rate 200HZ (0b11)")
-qmc.output_data_rate = qmc5883.OUTPUT_DATA_RATE_200
+qmc.output_data_rate = qmc5883l.OUTPUT_DATA_RATE_200
 print("Configuration register", bin(qmc._conf_reg))
 print("setting Mode to Continuous (0b01)")
-qmc.mode_control = qmc5883.MODE_CONTINUOUS
+qmc.mode_control = qmc5883l.MODE_CONTINUOUS
 print("Configuration register", bin(qmc._conf_reg))
-
-for i in range(50):
-    mag_x, mag_y, mag_z = qmc.magnetic
-    print(mag_x, mag_y, mag_z)
-    time.sleep(0.3)
```

### Comparing `circuitpython-qmc5883l-0.1.0/pyproject.toml` & `circuitpython-qmc5883l-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-qmc5883l"
 description = "CircuitPython driver for the qmc5883l magnetometer"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "qmc@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_qmc5883l"}
 keywords = [
     "adafruit",
```

### Comparing `circuitpython-qmc5883l-0.1.0/qmc5883l.py` & `circuitpython-qmc5883l-0.1.1/qmc5883l.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya for Trinity
 #
 # SPDX-License-Identifier: MIT
 """
 `qmc5883l`
 ================================================================================
 
@@ -16,26 +15,26 @@
 
 
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 * Adafruit's Register library: https://github.com/adafruit/Adafruit_CircuitPython_Register
 
 """
 
+import time
 from micropython import const
 from adafruit_bus_device import i2c_device
-from adafruit_register.i2c_struct import ROUnaryStruct, UnaryStruct
+from adafruit_register.i2c_struct import ROUnaryStruct, UnaryStruct, Struct
 from adafruit_register.i2c_bits import RWBits, ROBits
 
 try:
     from busio import I2C
-    from typing_extensions import NoReturn
 except ImportError:
     pass
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/CircuitPython_qmc5883l.git"
 
 _I2C_ADDR = const(0xD)
 _REG_WHOAMI = const(0x0D)
 _REG_SET_RESET = const(0x0B)
 _REG_OPERATION_MODE = const(0x09)
 _REG_STATUS = const(0x06)
@@ -71,15 +70,15 @@
 
     Here is an example of using the :class:`QMC5883L` class.
     First you will need to import the libraries to use the sensor
 
         .. code-block:: python
 
             import board
-            import circuitpython_qmc5883l.qmc5883l as qmc5883l
+            import qmc5883l
 
     Once this is done you can define your `board.I2C` object and define your sensor object
 
         .. code-block:: python
 
             i2c = board.I2C()  # uses board.SCL and board.SDA
             qmc = qmc5883l.QMC5883L(i2c)
@@ -97,20 +96,15 @@
     _reset = UnaryStruct(_REG_SET_RESET, "H")
     _conf_reg = ROUnaryStruct(_REG_OPERATION_MODE, "H")
     _oversample = RWBits(2, _REG_OPERATION_MODE, 6)
     _field_range = RWBits(2, _REG_OPERATION_MODE, 4)
     _output_data_rate = RWBits(2, _REG_OPERATION_MODE, 2)
     _mode_control = RWBits(2, _REG_OPERATION_MODE, 0)
     _data_ready_register = ROBits(1, _REG_STATUS, 2)
-    _x_LSB = ROUnaryStruct(0x00, "H")
-    _x_MSB = ROUnaryStruct(0x01, "H")
-    _y_LSB = ROUnaryStruct(0x02, "H")
-    _y_MSB = ROUnaryStruct(0x03, "H")
-    _z_LSB = ROUnaryStruct(0x04, "H")
-    _z_MSB = ROUnaryStruct(0x05, "H")
+    _measures = Struct(0x00, "<hhhBh")
 
     def __init__(self, i2c_bus: I2C, address: int = _I2C_ADDR) -> None:
         self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
         self.resolution = 12000
 
         if self._device_id != 0xFF:
             raise RuntimeError("Failed to find QMC5883L")
@@ -151,15 +145,15 @@
             qmc.oversample = qmc5883.OVERSAMPLE_64
 
         """
 
         return self._oversample
 
     @oversample.setter
-    def oversample(self, rate: int) -> NoReturn:
+    def oversample(self, rate: int) -> None:
 
         self._oversample = rate
 
     @property
     def field_range(self) -> int:
         """Field ranges of the magnetic sensor can be selected through the register RNG.
         The full scale field range is determined by the application environments.
@@ -192,17 +186,17 @@
             qmc.field_range = qmc5883.FIELDRANGE_2G
 
         """
 
         return self._field_range
 
     @field_range.setter
-    def field_range(self, field_range: int) -> NoReturn:
+    def field_range(self, field_range: int) -> None:
 
-        if range == 1:
+        if field_range == 1:
             self.resolution = 3000
         else:
             self.resolution = 12000
 
         self._field_range = field_range
 
     @property
@@ -242,15 +236,15 @@
             qmc.output_data_rate = qmc5883.OUTPUT_DATA_RATE_200
 
         """
 
         return self._output_data_rate
 
     @output_data_rate.setter
-    def output_data_rate(self, rate: int) -> NoReturn:
+    def output_data_rate(self, rate: int) -> None:
 
         self._output_data_rate = rate
 
     @property
     def mode_control(self) -> int:
         """Two bits of MODE registers can transfer mode of operations in the device,
         the two modes are Standby, and Continuous measurements. The default mode
@@ -281,31 +275,19 @@
             qmc.output_data_rate = qmc5883.MODE_STANDBY
 
         """
 
         return self._mode_control
 
     @mode_control.setter
-    def mode_control(self, mode: int) -> NoReturn:
+    def mode_control(self, mode: int) -> None:
 
         self._mode_control = mode
 
     @property
     def magnetic(self):
         """Magnetic property"""
-        if self._data_ready_register == 1:
+        while self._data_ready_register != 1:
+            time.sleep(0.001)
+        x, y, z, _, _ = self._measures
 
-            values = (
-                self._x_LSB,
-                self._x_MSB,
-                self._y_LSB,
-                self._y_MSB,
-                self._z_LSB,
-                self._z_MSB,
-            )
-
-            return (
-                values[0] / self.resolution,
-                values[2] / self.resolution,
-                values[4] / self.resolution,
-            )
-        return None
+        return x / self.resolution, y / self.resolution, z / self.resolution
```

