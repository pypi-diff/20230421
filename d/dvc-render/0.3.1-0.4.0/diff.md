# Comparing `tmp/dvc-render-0.3.1.tar.gz` & `tmp/dvc-render-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-render-0.3.1.tar", last modified: Thu Mar 16 19:29:55 2023, max compression
+gzip compressed data, was "dvc-render-0.4.0.tar", last modified: Fri Apr 21 19:43:43 2023, max compression
```

## Comparing `dvc-render-0.3.1.tar` & `dvc-render-0.4.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:29:55.174292 dvc-render-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-16 19:29:32.000000 dvc-render-0.3.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-16 19:29:32.000000 dvc-render-0.3.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:29:55.162292 dvc-render-0.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-16 19:29:32.000000 dvc-render-0.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:29:55.162292 dvc-render-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-16 19:29:32.000000 dvc-render-0.3.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-16 19:29:32.000000 dvc-render-0.3.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-03-16 19:29:32.000000 dvc-render-0.3.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-16 19:29:32.000000 dvc-render-0.3.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-03-16 19:29:32.000000 dvc-render-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-03-16 19:29:32.000000 dvc-render-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-03-16 19:29:32.000000 dvc-render-0.3.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-03-16 19:29:32.000000 dvc-render-0.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-03-16 19:29:32.000000 dvc-render-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-16 19:29:55.174292 dvc-render-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-16 19:29:32.000000 dvc-render-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:29:55.166292 dvc-render-0.3.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:29:55.166292 dvc-render-0.3.1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-16 19:29:32.000000 dvc-render-0.3.1/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-16 19:29:32.000000 dvc-render-0.3.1/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-16 19:29:32.000000 dvc-render-0.3.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-16 19:29:32.000000 dvc-render-0.3.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-16 19:29:32.000000 dvc-render-0.3.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-16 19:29:32.000000 dvc-render-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-16 19:29:55.174292 dvc-render-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:29:55.158292 dvc-render-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:29:55.170292 dvc-render-0.3.1/src/dvc_render/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-16 19:29:32.000000 dvc-render-0.3.1/src/dvc_render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-16 19:29:32.000000 dvc-render-0.3.1/src/dvc_render/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-16 19:29:32.000000 dvc-render-0.3.1/src/dvc_render/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-03-16 19:29:32.000000 dvc-render-0.3.1/src/dvc_render/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-03-16 19:29:32.000000 dvc-render-0.3.1/src/dvc_render/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-16 19:29:32.000000 dvc-render-0.3.1/src/dvc_render/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-03-16 19:29:32.000000 dvc-render-0.3.1/src/dvc_render/plotly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-16 19:29:32.000000 dvc-render-0.3.1/src/dvc_render/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-16 19:29:32.000000 dvc-render-0.3.1/src/dvc_render/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-03-16 19:29:32.000000 dvc-render-0.3.1/src/dvc_render/vega.py
--rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-03-16 19:29:32.000000 dvc-render-0.3.1/src/dvc_render/vega_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:29:55.170292 dvc-render-0.3.1/src/dvc_render.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-16 19:29:55.000000 dvc-render-0.3.1/src/dvc_render.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-16 19:29:55.000000 dvc-render-0.3.1/src/dvc_render.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 19:29:55.000000 dvc-render-0.3.1/src/dvc_render.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 19:29:54.000000 dvc-render-0.3.1/src/dvc_render.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-16 19:29:55.000000 dvc-render-0.3.1/src/dvc_render.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-16 19:29:55.000000 dvc-render-0.3.1/src/dvc_render.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:29:55.174292 dvc-render-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 19:29:32.000000 dvc-render-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-03-16 19:29:32.000000 dvc-render-0.3.1/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-03-16 19:29:32.000000 dvc-render-0.3.1/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-16 19:29:32.000000 dvc-render-0.3.1/tests/test_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-03-16 19:29:32.000000 dvc-render-0.3.1/tests/test_parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-16 19:29:32.000000 dvc-render-0.3.1/tests/test_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-16 19:29:32.000000 dvc-render-0.3.1/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-03-16 19:29:32.000000 dvc-render-0.3.1/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-03-16 19:29:32.000000 dvc-render-0.3.1/tests/test_vega.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.249693 dvc-render-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.241693 dvc-render-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.241693 dvc-render-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-21 19:43:15.000000 dvc-render-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-21 19:43:15.000000 dvc-render-0.4.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-21 19:43:15.000000 dvc-render-0.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-21 19:43:15.000000 dvc-render-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-21 19:43:43.249693 dvc-render-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-21 19:43:15.000000 dvc-render-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.241693 dvc-render-0.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.241693 dvc-render-0.4.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-21 19:43:15.000000 dvc-render-0.4.0/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-21 19:43:15.000000 dvc-render-0.4.0/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 19:43:15.000000 dvc-render-0.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-21 19:43:15.000000 dvc-render-0.4.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-21 19:43:15.000000 dvc-render-0.4.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-21 19:43:15.000000 dvc-render-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-21 19:43:43.249693 dvc-render-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.237693 dvc-render-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.245693 dvc-render-0.4.0/src/dvc_render/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/plotly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/vega.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-04-21 19:43:15.000000 dvc-render-0.4.0/src/dvc_render/vega_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.245693 dvc-render-0.4.0/src/dvc_render.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-21 19:43:43.000000 dvc-render-0.4.0/src/dvc_render.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-21 19:43:43.000000 dvc-render-0.4.0/src/dvc_render.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:43:43.000000 dvc-render-0.4.0/src/dvc_render.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:43:42.000000 dvc-render-0.4.0/src/dvc_render.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-21 19:43:43.000000 dvc-render-0.4.0/src/dvc_render.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 19:43:43.000000 dvc-render-0.4.0/src/dvc_render.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:43.249693 dvc-render-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-21 19:43:15.000000 dvc-render-0.4.0/tests/test_vega.py
```

### Comparing `dvc-render-0.3.1/.cruft.json` & `dvc-render-0.4.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/.github/dependabot.yml` & `dvc-render-0.4.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/.github/workflows/docs.yml` & `dvc-render-0.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/.github/workflows/release.yml` & `dvc-render-0.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/.github/workflows/tests.yml` & `dvc-render-0.4.0/.github/workflows/tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
   cancel-in-progress: true
 
 jobs:
   tests:
-    timeout-minutes: 10
+    timeout-minutes: 20
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-20.04, windows-latest, macos-latest]
         pyv: ['3.8', '3.9', '3.10', '3.11']
         include:
```

### Comparing `dvc-render-0.3.1/.gitignore` & `dvc-render-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/.pre-commit-config.yaml` & `dvc-render-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/CODE_OF_CONDUCT.rst` & `dvc-render-0.4.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/CONTRIBUTING.rst` & `dvc-render-0.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/LICENSE` & `dvc-render-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/docs/assets/logo.svg` & `dvc-render-0.4.0/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/docs/gen_ref_pages.py` & `dvc-render-0.4.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/mkdocs.yml` & `dvc-render-0.4.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/noxfile.py` & `dvc-render-0.4.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/pyproject.toml` & `dvc-render-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/setup.cfg` & `dvc-render-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/src/dvc_render/base.py` & `dvc-render-0.4.0/src/dvc_render/base.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/src/dvc_render/html.py` & `dvc-render-0.4.0/src/dvc_render/html.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/src/dvc_render/image.py` & `dvc-render-0.4.0/src/dvc_render/image.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/src/dvc_render/markdown.py` & `dvc-render-0.4.0/src/dvc_render/markdown.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/src/dvc_render/plotly.py` & `dvc-render-0.4.0/src/dvc_render/plotly.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/src/dvc_render/table.py` & `dvc-render-0.4.0/src/dvc_render/table.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/src/dvc_render/vega.py` & `dvc-render-0.4.0/src/dvc_render/vega.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/src/dvc_render/vega_templates.py` & `dvc-render-0.4.0/src/dvc_render/vega_templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,14 +263,15 @@
                         }
                     },
                     "mark": "rect",
                     "encoding": {
                         "tooltip": [
                             {"field": Template.anchor("x"), "type": "nominal"},
                             {"field": Template.anchor("y"), "type": "nominal"},
+                            {"field": "xy_count", "type": "quantitative"},
                         ],
                         "opacity": {
                             "condition": {"selection": "label", "value": 1},
                             "value": 0,
                         },
                     },
                 },
@@ -279,15 +280,14 @@
                     "layer": [
                         {"mark": {"type": "rect", "color": "lightpink"}},
                     ],
                 },
                 {
                     "mark": "text",
                     "encoding": {
-                        "text": {"field": "xy_count", "type": "quantitative"},
                         "color": {
                             "condition": {
                                 "test": "datum.percent_of_max > 0.5",
                                 "value": "white",
                             },
                             "value": "black",
                         },
@@ -373,14 +373,19 @@
                         }
                     },
                     "mark": "rect",
                     "encoding": {
                         "tooltip": [
                             {"field": Template.anchor("x"), "type": "nominal"},
                             {"field": Template.anchor("y"), "type": "nominal"},
+                            {
+                                "field": "percent_of_y",
+                                "type": "quantitative",
+                                "format": ".2f",
+                            },
                         ],
                         "opacity": {
                             "condition": {"selection": "label", "value": 1},
                             "value": 0,
                         },
                     },
                 },
@@ -389,19 +394,14 @@
                     "layer": [
                         {"mark": {"type": "rect", "color": "lightpink"}},
                     ],
                 },
                 {
                     "mark": "text",
                     "encoding": {
-                        "text": {
-                            "field": "percent_of_y",
-                            "type": "quantitative",
-                            "format": ".2f",
-                        },
                         "color": {
                             "condition": {
                                 "test": "datum.percent_of_y > 0.5",
                                 "value": "white",
                             },
                             "value": "black",
                         },
```

### Comparing `dvc-render-0.3.1/src/dvc_render.egg-info/SOURCES.txt` & `dvc-render-0.4.0/src/dvc_render.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/src/dvc_render.egg-info/requires.txt` & `dvc-render-0.4.0/src/dvc_render.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/tests/test_html.py` & `dvc-render-0.4.0/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/tests/test_image.py` & `dvc-render-0.4.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/tests/test_markdown.py` & `dvc-render-0.4.0/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/tests/test_parallel_coordinates.py` & `dvc-render-0.4.0/tests/test_parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/tests/test_table.py` & `dvc-render-0.4.0/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/tests/test_templates.py` & `dvc-render-0.4.0/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.3.1/tests/test_vega.py` & `dvc-render-0.4.0/tests/test_vega.py`

 * *Files identical despite different names*

