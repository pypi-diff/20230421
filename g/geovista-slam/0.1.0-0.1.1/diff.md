# Comparing `tmp/geovista-slam-0.1.0.tar.gz` & `tmp/geovista-slam-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovista-slam-0.1.0.tar", last modified: Mon Apr 17 12:29:42 2023, max compression
+gzip compressed data, was "geovista-slam-0.1.1.tar", last modified: Thu Apr 20 21:37:57 2023, max compression
```

## Comparing `geovista-slam-0.1.0.tar` & `geovista-slam-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 itwl      (6006) avd       (1091)        0 2023-04-17 12:29:42.447953 geovista-slam-0.1.0/
-drwxr-xr-x   0 itwl      (6006) avd       (1091)        0 2023-04-17 12:29:42.372939 geovista-slam-0.1.0/.github/
-drwxr-xr-x   0 itwl      (6006) avd       (1091)        0 2023-04-17 12:29:42.397927 geovista-slam-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 itwl      (6006) avd       (1091)      944 2023-04-14 08:06:09.000000 geovista-slam-0.1.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 itwl      (6006) avd       (1091)      395 2023-04-14 08:06:09.000000 geovista-slam-0.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 itwl      (6006) avd       (1091)      288 2023-04-14 08:07:06.000000 geovista-slam-0.1.0/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 itwl      (6006) avd       (1091)      622 2023-04-14 08:07:06.000000 geovista-slam-0.1.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 itwl      (6006) avd       (1091)      259 2023-04-14 08:07:06.000000 geovista-slam-0.1.0/.github/ISSUE_TEMPLATE/issue.md
--rw-r--r--   0 itwl      (6006) avd       (1091)      409 2023-04-13 10:55:31.000000 geovista-slam-0.1.0/.github/dependabot.yml
--rw-r--r--   0 itwl      (6006) avd       (1091)      181 2023-04-14 22:44:34.000000 geovista-slam-0.1.0/.github/pull_request_template.md
-drwxr-xr-x   0 itwl      (6006) avd       (1091)        0 2023-04-17 12:29:42.410958 geovista-slam-0.1.0/.github/workflows/
--rw-r--r--   0 itwl      (6006) avd       (1091)     4026 2023-04-17 12:28:26.000000 geovista-slam-0.1.0/.github/workflows/ci-locks.yml
--rw-r--r--   0 itwl      (6006) avd       (1091)      651 2023-04-14 13:59:04.000000 geovista-slam-0.1.0/.github/workflows/ci-manifest.yml
--rw-r--r--   0 itwl      (6006) avd       (1091)     4068 2023-04-15 00:44:00.000000 geovista-slam-0.1.0/.github/workflows/ci-wheels.yml
--rw-r--r--   0 itwl      (6006) avd       (1091)     5488 2023-04-13 11:20:05.000000 geovista-slam-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 itwl      (6006) avd       (1091)     1519 2023-04-13 08:18:18.000000 geovista-slam-0.1.0/LICENSE
--rw-r--r--   0 itwl      (6006) avd       (1091)      173 2023-04-13 11:20:31.000000 geovista-slam-0.1.0/MANIFEST.in
--rw-r--r--   0 itwl      (6006) avd       (1091)     4256 2023-04-17 12:29:42.446953 geovista-slam-0.1.0/PKG-INFO
--rw-r--r--   0 itwl      (6006) avd       (1091)     3213 2023-04-13 14:49:47.000000 geovista-slam-0.1.0/README.md
--rw-r--r--   0 itwl      (6006) avd       (1091)     2521 2023-04-14 10:31:14.000000 geovista-slam-0.1.0/pyproject.toml
--rw-r--r--   0 itwl      (6006) avd       (1091)       38 2023-04-17 12:29:42.448934 geovista-slam-0.1.0/setup.cfg
--rw-r--r--   0 itwl      (6006) avd       (1091)       96 2023-04-13 08:18:18.000000 geovista-slam-0.1.0/setup.py
-drwxr-xr-x   0 itwl      (6006) avd       (1091)        0 2023-04-17 12:29:42.344949 geovista-slam-0.1.0/src/
-drwxr-xr-x   0 itwl      (6006) avd       (1091)        0 2023-04-17 12:29:42.435940 geovista-slam-0.1.0/src/geovista_slam.egg-info/
--rw-r--r--   0 itwl      (6006) avd       (1091)     4256 2023-04-17 12:29:42.000000 geovista-slam-0.1.0/src/geovista_slam.egg-info/PKG-INFO
--rw-r--r--   0 itwl      (6006) avd       (1091)      696 2023-04-17 12:29:42.000000 geovista-slam-0.1.0/src/geovista_slam.egg-info/SOURCES.txt
--rw-r--r--   0 itwl      (6006) avd       (1091)        1 2023-04-17 12:29:42.000000 geovista-slam-0.1.0/src/geovista_slam.egg-info/dependency_links.txt
--rw-r--r--   0 itwl      (6006) avd       (1091)        1 2023-04-14 07:48:57.000000 geovista-slam-0.1.0/src/geovista_slam.egg-info/not-zip-safe
--rw-r--r--   0 itwl      (6006) avd       (1091)       88 2023-04-17 12:29:42.000000 geovista-slam-0.1.0/src/geovista_slam.egg-info/requires.txt
--rw-r--r--   0 itwl      (6006) avd       (1091)        5 2023-04-17 12:29:42.000000 geovista-slam-0.1.0/src/geovista_slam.egg-info/top_level.txt
-drwxr-xr-x   0 itwl      (6006) avd       (1091)        0 2023-04-17 12:29:42.443912 geovista-slam-0.1.0/src/slam/
--rw-r--r--   0 itwl      (6006) avd       (1091)    21732 2023-04-13 13:47:39.000000 geovista-slam-0.1.0/src/slam/__init__.py
--rw-r--r--   0 itwl      (6006) avd       (1091)      160 2023-04-17 12:29:42.000000 geovista-slam-0.1.0/src/slam/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:57.098721 geovista-slam-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:57.094721 geovista-slam-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:57.094721 geovista-slam-0.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/.github/ISSUE_TEMPLATE/issue.md
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:57.094721 geovista-slam-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/.github/workflows/ci-citation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/.github/workflows/ci-locks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/.github/workflows/ci-manifest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/.github/workflows/ci-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-20 21:37:57.098721 geovista-slam-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 21:37:57.098721 geovista-slam-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:57.090721 geovista-slam-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:57.094721 geovista-slam-0.1.1/src/geovista_slam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-20 21:37:57.000000 geovista-slam-0.1.1/src/geovista_slam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-20 21:37:57.000000 geovista-slam-0.1.1/src/geovista_slam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:37:57.000000 geovista-slam-0.1.1/src/geovista_slam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:37:56.000000 geovista-slam-0.1.1/src/geovista_slam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-20 21:37:57.000000 geovista-slam-0.1.1/src/geovista_slam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 21:37:57.000000 geovista-slam-0.1.1/src/geovista_slam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:37:57.094721 geovista-slam-0.1.1/src/slam/
+-rw-r--r--   0 runner    (1001) docker     (123)    21735 2023-04-20 21:37:42.000000 geovista-slam-0.1.1/src/slam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 21:37:56.000000 geovista-slam-0.1.1/src/slam/_version.py
```

### Comparing `geovista-slam-0.1.0/.github/ISSUE_TEMPLATE/bug-report.md` & `geovista-slam-0.1.1/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `geovista-slam-0.1.0/.github/ISSUE_TEMPLATE/feature-request.md` & `geovista-slam-0.1.1/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `geovista-slam-0.1.0/.github/workflows/ci-locks.yml` & `geovista-slam-0.1.1/.github/workflows/ci-locks.yml`

 * *Files identical despite different names*

### Comparing `geovista-slam-0.1.0/.github/workflows/ci-manifest.yml` & `geovista-slam-0.1.1/.github/workflows/ci-manifest.yml`

 * *Files identical despite different names*

### Comparing `geovista-slam-0.1.0/.github/workflows/ci-wheels.yml` & `geovista-slam-0.1.1/.github/workflows/ci-wheels.yml`

 * *Files 2% similar despite different names*

```diff
@@ -139,24 +139,24 @@
         user: __token__
         password: ${{ secrets.TEST_PYPI_API_TOKEN }}
         repository_url: https://test.pypi.org/legacy/
         skip_existing: true
         print_hash: true
 
 
-#  publish-artifacts-pypi:
-#    needs: [test-artifacts]
-#    name: "Publish to PyPI"
-#    runs-on: ubuntu-latest
-#    # upload to PyPI for every tag starting with 'v'
-#    if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags/v')
-#    steps:
-#    - uses: actions/download-artifact@v3
-#      with:
-#        name: pypi-artifacts
-#        path: ${{ github.workspace }}/dist
-#
-#    - uses: pypa/gh-action-pypi-publish@release/v1
-#      with:
-#        user: __token__
-#        password: ${{ secrets.PYPI_API_TOKEN }}
-#        print_hash: true
+  publish-artifacts-pypi:
+    needs: [test-artifacts]
+    name: "Publish to PyPI"
+    runs-on: ubuntu-latest
+    # upload to PyPI for every tag starting with 'v'
+    if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags/v')
+    steps:
+    - uses: actions/download-artifact@v3
+      with:
+        name: pypi-artifacts
+        path: ${{ github.workspace }}/dist
+
+    - uses: pypa/gh-action-pypi-publish@release/v1
+      with:
+        user: __token__
+        password: ${{ secrets.PYPI_API_TOKEN }}
+        print_hash: true
```

### Comparing `geovista-slam-0.1.0/CODE_OF_CONDUCT.md` & `geovista-slam-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geovista-slam-0.1.0/LICENSE` & `geovista-slam-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geovista-slam-0.1.0/pyproject.toml` & `geovista-slam-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geovista-slam-0.1.0/src/geovista_slam.egg-info/SOURCES.txt` & `geovista-slam-0.1.1/src/geovista_slam.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+CITATION.cff
 CODE_OF_CONDUCT.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 .github/dependabot.yml
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug-report.md
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/documentation.md
 .github/ISSUE_TEMPLATE/feature-request.md
 .github/ISSUE_TEMPLATE/issue.md
+.github/workflows/ci-citation.yml
 .github/workflows/ci-locks.yml
 .github/workflows/ci-manifest.yml
 .github/workflows/ci-wheels.yml
 src/geovista_slam.egg-info/PKG-INFO
 src/geovista_slam.egg-info/SOURCES.txt
 src/geovista_slam.egg-info/dependency_links.txt
 src/geovista_slam.egg-info/not-zip-safe
```

### Comparing `geovista-slam-0.1.0/src/slam/__init__.py` & `geovista-slam-0.1.1/src/slam/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,22 +25,22 @@
     __version__ = "unknown"
 
 __all__ = ("Transform",)
 
 # type aliases
 CoordLike = Union[AuxCoord, DimCoord]
 PathLike = Union[str, Path]
-ShapeLike = Union[list[int], Tuple[int]]
+ShapeLike = Union[list[int], Tuple[int, ...]]
 
 CELL_IDS: str = "slamIdsGlobal"
 CELL_IDS_LOCAL: str = "slamIdsLocal"
 DEFAULT_FAST_SOLVE: bool = False
 DEFAULT_ROUNDING: bool = True
 DEFAULT_SHARE_SPATIAL: bool = False
-DEFAULT_CF_COORDINATE_SYSTEM: list[dict[str, Any], dict[str, Any]] = [
+DEFAULT_CF_COORDINATE_SYSTEM: list[dict[str, Any]] = [
     {
         "standard_name": "longitude",
         "long_name": "longitude coordinate",
         "units": "degrees",
     },
     {
         "standard_name": "latitude",
@@ -51,14 +51,15 @@
 MDI: int = -1
 
 
 # TODO:
 #   - trap for non-quad mesh
 #   - add developer diagnostics (warnings)
 #   - doc-strings
+#   - add tox
 #   - test coverage
 #   - restructure:
 #       - factories
 #       - anything spanning mesh dimension
 #   - discover crs from mesh
 #   - load/save
 #   - enable ci services
```

