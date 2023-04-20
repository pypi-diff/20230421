# Comparing `tmp/cmake_pre_commit_hooks-1.8.0.tar.gz` & `tmp/cmake_pre_commit_hooks-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmake_pre_commit_hooks-1.8.0.tar", last modified: Thu Feb 16 11:07:01 2023, max compression
+gzip compressed data, was "cmake_pre_commit_hooks-1.8.1.tar", last modified: Thu Apr 20 21:59:21 2023, max compression
```

## Comparing `cmake_pre_commit_hooks-1.8.0.tar` & `cmake_pre_commit_hooks-1.8.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 11:07:01.710217 cmake_pre_commit_hooks-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/.codespell.allow
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 11:07:01.706217 cmake_pre_commit_hooks-1.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 11:07:01.706217 cmake_pre_commit_hooks-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/.github/workflows/draft_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/.github/workflows/publish_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-02-16 11:07:01.710217 cmake_pre_commit_hooks-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 11:07:01.710217 cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18580 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/clang_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/clang_tidy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/cppcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/cpplint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/include_what_you_use.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1951 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/lizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 11:07:01.710217 cmake_pre_commit_hooks-1.8.0/cmake_pre_commit_hooks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-02-16 11:07:01.000000 cmake_pre_commit_hooks-1.8.0/cmake_pre_commit_hooks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-02-16 11:07:01.000000 cmake_pre_commit_hooks-1.8.0/cmake_pre_commit_hooks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 11:07:01.000000 cmake_pre_commit_hooks-1.8.0/cmake_pre_commit_hooks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-16 11:07:01.000000 cmake_pre_commit_hooks-1.8.0/cmake_pre_commit_hooks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-16 11:07:01.000000 cmake_pre_commit_hooks-1.8.0/cmake_pre_commit_hooks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-16 11:07:01.000000 cmake_pre_commit_hooks-1.8.0/cmake_pre_commit_hooks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 11:07:01.710217 cmake_pre_commit_hooks-1.8.0/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/misc/license_header.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-02-16 11:07:01.710217 cmake_pre_commit_hooks-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 11:07:01.710217 cmake_pre_commit_hooks-1.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 11:07:01.710217 cmake_pre_commit_hooks-1.8.0/tests/cmake_bad/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/tests/cmake_bad/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/tests/cmake_bad/.pre-commit-win.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/tests/cmake_bad/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/tests/cmake_bad/bad.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 11:07:01.710217 cmake_pre_commit_hooks-1.8.0/tests/cmake_good/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/tests/cmake_good/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/tests/cmake_good/.pre-commit-win.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/tests/cmake_good/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/tests/cmake_good/good.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/tests/run_tests.ps1
--rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-02-16 11:06:50.000000 cmake_pre_commit_hooks-1.8.0/tests/run_tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.codespell.allow
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.417322 cmake_pre_commit_hooks-1.8.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.github/workflows/draft_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.github/workflows/publish_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19785 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/clang_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/clang_tidy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/cppcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/cpplint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/include_what_you_use.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1951 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/lizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-04-20 21:59:21.000000 cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-20 21:59:21.000000 cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:59:21.000000 cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-20 21:59:21.000000 cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-20 21:59:21.000000 cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 21:59:21.000000 cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/misc/license_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/tests/cmake_bad/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_bad/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_bad/.pre-commit-win.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_bad/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_bad/bad.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:21.421322 cmake_pre_commit_hooks-1.8.1/tests/cmake_good/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_good/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_good/.pre-commit-win.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_good/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/cmake_good/good.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/run_tests.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-04-20 21:59:12.000000 cmake_pre_commit_hooks-1.8.1/tests/run_tests.sh
```

### Comparing `cmake_pre_commit_hooks-1.8.0/.github/workflows/ci.yml` & `cmake_pre_commit_hooks-1.8.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/.github/workflows/codeql-analysis.yml` & `cmake_pre_commit_hooks-1.8.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/.github/workflows/draft_release.yml` & `cmake_pre_commit_hooks-1.8.1/.github/workflows/draft_release.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/.github/workflows/format.yml` & `cmake_pre_commit_hooks-1.8.1/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/.github/workflows/publish_release.yml` & `cmake_pre_commit_hooks-1.8.1/.github/workflows/publish_release.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/.gitignore` & `cmake_pre_commit_hooks-1.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/.pre-commit-config.yaml` & `cmake_pre_commit_hooks-1.8.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -16,52 +16,52 @@
       - id: check-toml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
 
   - repo: https://github.com/Lucas-C/pre-commit-hooks
-    rev: v1.4.2
+    rev: v1.5.1
     hooks:
       - id: remove-tabs
 
   - repo: https://github.com/PyCQA/doc8/
     rev: v1.1.1
     hooks:
       - id: doc8
         require_serial: false
         additional_dependencies: [tomli]
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
         files: .*\.(py|txt|cmake|md|rst|sh|ps1|hpp|tpp|cpp|cc)$
         args: [-I, .codespell.allow]
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
     rev: v0.9.0.2
     hooks:
       - id: shellcheck
         require_serial: false
         args: [-x, --severity=info]
 
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.29.0
+    rev: v1.30.0
     hooks:
       - id: yamllint
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
         name: isort (python)
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
 
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.13.0
     hooks:
@@ -72,15 +72,15 @@
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.3.1
     hooks:
       - id: pyupgrade
         args: [--py38-plus, --keep-mock]
 
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args: [-c, pyproject.toml]
         additional_dependencies: ["bandit[toml]"]
 
   - repo: https://github.com/PyCQA/flake8
     rev: 5.0.4
@@ -90,9 +90,9 @@
                                   flake8-docstrings, flake8-eradicate,
                                   flake8-mutable]
 
   - repo: https://github.com/pre-commit/mirrors-pylint
     rev: 'v3.0.0a5'
     hooks:
       - id: pylint
-        additional_dependencies: [CLinters, fasteners, pylint-secure-coding-standard]
+        additional_dependencies: [CLinters, fasteners, filelock, pylint-secure-coding-standard]
         args: [--load-plugins=pylint_secure_coding_standard]
```

### Comparing `cmake_pre_commit_hooks-1.8.0/.pre-commit-hooks.yaml` & `cmake_pre_commit_hooks-1.8.1/.pre-commit-hooks.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -3,51 +3,51 @@
 # which hooks are provided by this repo
 # for use by other git repos.
 
 - id: clang-format
   name: clang-format
   entry: cmake-pc-clang-format-hook
   description: Formats C/CPP code
-  files: \.(c|cc|cu|cxx|cpp|h|hpp|hxx|m)$
+  files: \.(c|c\+\+m|cc|ccm|cpp|cppm|cu|cxx|cxxm|h|hpp|hxx|ixx|m|mxx)$
   language: python
 - id: clang-tidy
   name: clang-tidy
   entry: cmake-pc-clang-tidy-hook
   description: Find warnings/errors in C/CPP code
-  files: \.(c|cc|cu|cxx|cpp|h|hpp|hxx|m)$
+  files: \.(c|c\+\+m|cc|ccm|cpp|cppm|cu|cxx|cxxm|h|hpp|hxx|ixx|m|mxx)$
   language: python
 - id: cppcheck
   name: cppcheck (system)
   entry: cmake-pc-cppcheck-hook
   description: Find warnings/errors in C/CPP code
-  files: \.(c|cc|cu|cxx|cpp|h|hpp|hxx|m)$
+  files: \.(c|c\+\+m|cc|ccm|cpp|cppm|cu|cxx|cxxm|h|hpp|hxx|ixx|m|mxx)$
   language: python
 - id: cppcheck-conda
   name: cppcheck (conda)
   entry: cmake-pc-cppcheck-hook
   description: Find warnings/errors in C/CPP code
-  files: \.(c|cc|cu|cxx|cpp|h|hpp|hxx|m)$
+  files: \.(c|c\+\+m|cc|ccm|cpp|cppm|cu|cxx|cxxm|h|hpp|hxx|ixx|m|mxx)$
   language: conda
 - id: cpplint
   name: cpplint
   entry: cmake-pc-cpplint-hook
   description: Find warnings/errors in C/CPP code
-  files: \.(c|cc|cpp|cu|cuh|cxx|h|hh|hpp|hxx)$
+  files: \.(c|c\+\+m|cc|ccm|cpp|cppm|cu|cuh|cxx|cxxm|h|hh|hpp|hxx|ixx|mxx)$
   language: python
 - id: include-what-you-use
   name: include-what-you-use (system)
   entry: cmake-pc-include-what-you-use-hook
   description: Find unused include directives in C/CPP code
-  files: \.(c|cc|cu|cxx|cpp|h|hpp|hxx|m)$
+  files: \.(c|c\+\+m|cc|ccm|cpp|cppm|cu|cxx|cxxm|h|hpp|hxx|ixx|m|mxx)$
   language: python
 - id: include-what-you-use-conda
   name: include-what-you-use (conda)
   entry: cmake-pc-include-what-you-use-hook
   description: Find unused include directives in C/CPP code
-  files: \.(c|cc|cu|cxx|cpp|h|hpp|hxx|m)$
+  files: \.(c|c\+\+m|cc|ccm|cpp|cppm|cu|cxx|cxxm|h|hpp|hxx|ixx|m|mxx)$
   language: conda
 - id: lizard
   name: lizard
   entry: cmake-pc-lizard-hook
   description: Code complexity analyzer for C/CPP/ObjC/...
-  files: \.(c|cc|cpp|cu|cuh|cxx|h|hh|hpp|hxx|py|f|f90|f95|f03|F|F90|F95|F03)$
+  files: \.(F|F03|F90|F95|c|c\+\+m|cc|ccm|cpp|cppm|cu|cuh|cxx|cxxm|f|f03|f90|f95|h|hh|hpp|hxx|ixx|mxx|py)$
   language: python
```

### Comparing `cmake_pre_commit_hooks-1.8.0/CHANGELOG.md` & `cmake_pre_commit_hooks-1.8.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,37 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v1.8.1] - 2023-04-20
+
+### Added
+
+-   Added support for C++ module files by default
+
+### Fixed
+
+-   Fixed some typos in the README file (thanks to @onuralpszr)
+
+### Changed
+
+-   Require users to explicitly set `-B`\|`--build-dir` if they pass `--preset` to CMake (see issue [#63](https://github.com/Takishima/cmake-pre-commit-hooks/issues/63))
+
+### Repository
+
+-   Update `Lucas-C/pre-commit-hooks` hook to v1.5.1
+-   Update `codespell` to v2.2.4
+-   Update `yamllint` hook to v1.30.0
+-   Update `black` hook to v23.3.0
+-   Update `bandit` hook to v1.7.5
+-   Update `isort` hook to v5.12.0
+
 ## [v1.8.0] - 2023-02-16
 
 ### Added
 
 -   Added support for the CMake `--preset` command line argument
 
 ## [v1.7.0] - 2023-02-09
@@ -207,14 +230,15 @@
 -   Support for specifying more than one build directory
     If one of those exists and contains a configured CMake directory, that one will be chosen. If none already exist,
     the first specified alternative will be chosen.
 
 ### Fixed
 
 -   Issues with arguments parsing for arguments that are specified more than once
+-   Fix issue with CMake configure step when running hooks in parallel
 
 ### Repository
 
 -   Update pre-commit configuration
 
 ## [1.0.1] - 2021-06-20
 
@@ -236,15 +260,17 @@
 
 Initial release with support for:
 
 -   clang-format
 -   clang-tidy
 -   cppcheck
 
-[Unreleased]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.8.0...HEAD
+[Unreleased]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.8.1...HEAD
+
+[v1.8.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.8.0...v1.8.1
 
 [v1.8.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.7.0...v1.8.0
 
 [v1.7.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.6.0...v1.7.0
 
 [v1.6.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.5.3...v1.6.0
```

### Comparing `cmake_pre_commit_hooks-1.8.0/LICENSE` & `cmake_pre_commit_hooks-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/PKG-INFO` & `cmake_pre_commit_hooks-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake_pre_commit_hooks
-Version: 1.8.0
+Version: 1.8.1
 Summary: pre-commit hooks for CMake based projects
 Home-page: https://github.com/Takishima/cmake-pre-commit-hooks
 Author: Damien Nguyen
 Author-email: ngn.damien@gmail.com
 License: Apache2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -57,15 +57,15 @@
 
 with the following file contents:
 
 __.pre-commit-config.yaml__
 
     repos:
       - repo: https://github.com/Takishima/cmake-pre-commit-hooks
-        rev: 1.0.0
+        rev: v1.8.0
         hooks:
           - id: clang-format
           - id: clang-tidy
             args: [--checks=readability-magic-numbers,--warnings-as-errors=*]
           - id: cppcheck
           - id: include-what-you-use
 
@@ -167,14 +167,15 @@
 | `-S <path-to-source>`        | Explicitly specify a source directory.           |
 | `-B <path-to-build>`         | Explicitly specify a build directory.            |
 | `-D <var>[:<type>]=<value>`  | Create or update a cmake cache entry.            |
 | `-U <globbing_expr>`         | Remove matching entries from CMake cache.        |
 | `-G <generator-name>`        | Specify a build system generator.                |
 | `-T <toolset-name>`          | Specify toolset name if supported by generator.  |
 | `-A <platform-name>`         | Specify platform name if supported by generator. |
+| `--preset <preset>`          | Specify a configure preset.                      |
 | `-Wdev`                      | Enable developer warnings.                       |
 | `-Wno-dev`                   | Suppress developer warnings.                     |
 | `-Werror=dev`                | Make developer warnings errors.                  |
 | `-Wno-error=dev`             | Make developer warnings not errors.              |
 
 One important thing to note (particularly for those that intend to use this on CIs), you may specify the build directory
 argument (`-B`) multiple times. The hooks will then simply cycle through all of the values provided and choose the first
@@ -206,15 +207,15 @@
 
 
 Usage example:
 
 ```yaml
 repos:
 - repo: https://github.com/Takishima/cmake-pre-commit-hooks
-  rev: 1.0.0
+  rev: v1.8.0
   hooks:
     - id: cppcheck
       args: [-DBUILD_TESTING=ON,
              --unix="-DCMAKE_CXX_COMPILER=g++-10",
              --win="-DCMAKE_CXX_COMPILER=cl.exe"
              -Bpath/to/build_dir,
              -Bpath/to/other_build_dir,
```

### Comparing `cmake_pre_commit_hooks-1.8.0/README.md` & `cmake_pre_commit_hooks-1.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 with the following file contents:
 
 __.pre-commit-config.yaml__
 
     repos:
       - repo: https://github.com/Takishima/cmake-pre-commit-hooks
-        rev: 1.0.0
+        rev: v1.8.0
         hooks:
           - id: clang-format
           - id: clang-tidy
             args: [--checks=readability-magic-numbers,--warnings-as-errors=*]
           - id: cppcheck
           - id: include-what-you-use
 
@@ -146,14 +146,15 @@
 | `-S <path-to-source>`        | Explicitly specify a source directory.           |
 | `-B <path-to-build>`         | Explicitly specify a build directory.            |
 | `-D <var>[:<type>]=<value>`  | Create or update a cmake cache entry.            |
 | `-U <globbing_expr>`         | Remove matching entries from CMake cache.        |
 | `-G <generator-name>`        | Specify a build system generator.                |
 | `-T <toolset-name>`          | Specify toolset name if supported by generator.  |
 | `-A <platform-name>`         | Specify platform name if supported by generator. |
+| `--preset <preset>`          | Specify a configure preset.                      |
 | `-Wdev`                      | Enable developer warnings.                       |
 | `-Wno-dev`                   | Suppress developer warnings.                     |
 | `-Werror=dev`                | Make developer warnings errors.                  |
 | `-Wno-error=dev`             | Make developer warnings not errors.              |
 
 One important thing to note (particularly for those that intend to use this on CIs), you may specify the build directory
 argument (`-B`) multiple times. The hooks will then simply cycle through all of the values provided and choose the first
@@ -185,15 +186,15 @@
 
 
 Usage example:
 
 ```yaml
 repos:
 - repo: https://github.com/Takishima/cmake-pre-commit-hooks
-  rev: 1.0.0
+  rev: v1.8.0
   hooks:
     - id: cppcheck
       args: [-DBUILD_TESTING=ON,
              --unix="-DCMAKE_CXX_COMPILER=g++-10",
              --win="-DCMAKE_CXX_COMPILER=cl.exe"
              -Bpath/to/build_dir,
              -Bpath/to/other_build_dir,
```

### Comparing `cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/__init__.py` & `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/_utils.py` & `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,18 +21,20 @@
 import platform
 import shutil
 import subprocess as sp
 import sys
 from pathlib import Path
 
 import fasteners
+import filelock
 import hooks.utils
 
 _LOGLEVEL = os.environ.get('LOGLEVEL', 'WARNING').upper()  # pylint: disable=no-member
 logging.basicConfig(level=_LOGLEVEL)
+logging.getLogger('filelock').setLevel(logging.WARNING)
 
 
 def get_cmake_command(cmake_names=None):
     """
     Get the path to a CMake executable on the PATH or in the virtual environment.
 
     Args:
@@ -241,14 +243,16 @@
         self.cmake = known_args.cmake
         self.all_at_once = known_args.all_at_once
         self.read_json_db = known_args.read_json_db
         self.clean_build = known_args.clean
         self.source_dir = Path(known_args.source_dir).resolve()
 
         if not known_args.build_dir:
+            if known_args.preset:
+                raise RuntimeError('You *must* specify -B|--build-dir if you pass --preset as a CMake argument!')
             known_args.build_dir = [self.build_dir]  # default value
 
         # Try all the passed build directories if one already exists, use that one, otherwise take the first one
         for build_dir in [Path(path) for path in known_args.build_dir]:
             if build_dir.exists() and Path(build_dir, 'CMakeCache.txt').exists():
                 self.build_dir = build_dir.resolve()
                 break
@@ -295,78 +299,46 @@
         self.history.append(self._call_process([self.command] + filenames + self.args + self.ddash_args))
 
         # Compatibility with CLinters
         self.stdout = self.history[-1].stdout.encode()
         self.stderr = self.history[-1].stderr.encode()
         self.returncode = self.history[-1].returncode
 
-    def run_cmake_configure(self):  # pylint: disable=too-many-branches
-        """Run a CMake configure step."""
-        configuring = Path(self.build_dir, '_configuring')
+    def run_cmake_configure(self):
+        """Run the CMake configure step.
+
+        This member function is essentially here to handle the case where multiple processes are attempting to call
+        CMake configure within the same build directory. This can happen if the pre-commit hooks are not configured with
+        `serial: True` inside the configuration file.
+        """
+        cmake_configure_lock_file = Path(self.build_dir, '_cmake_configure_lock')
+        cmake_configure_try_lock_file = Path(self.build_dir, '_cmake_configure_try_lock')
 
         self.build_dir.mkdir(exist_ok=True)
 
-        rw_lock = fasteners.InterProcessReaderWriterLock(configuring)
-        if not configuring.exists():
-            with rw_lock.write_lock():
-                if self.clean_build:
-                    for path in self.build_dir.iterdir():
-                        if path.is_dir():
-                            shutil.rmtree(path)
-                        elif path != configuring:
-                            path.unlink()
-
-                result = self._call_process(self.cmake + [str(self.source_dir)] + self.cmake_args, cwd=self.build_dir)
-                result.stdout = '\n'.join(
-                    [
-                        f'Running CMake with: {self.cmake + [str(self.source_dir)] + self.cmake_args}',
-                        f'  from within {self.build_dir}',
-                        result.stdout,
-                        '',
-                    ]
-                )
-
-                if result.returncode == 0:
-                    compiledb = Path(self.build_dir, 'compile_commands.json')
-                    if not compiledb.exists():
-                        result.returncode = 1
-                        result.stderr += f'\nUnable to locate {compiledb}\n\n'
-                        copy_std_output_to_sys(result)
-                    else:
-                        compiledb_srcdir = Path(self.source_dir, 'compile_commands.json')
-                        if compiledb_srcdir.is_symlink() and compiledb_srcdir.resolve() == compiledb:
-                            # If it's a symbolic link and points to the compilation database in the build directory,
-                            # we're all good.
-                            pass
-                        else:
-                            # In all other cases, we copy the compilation database into the source directory
-                            if compiledb_srcdir.is_symlink():
-                                logging.debug('Removing symbolic link at: %s', compiledb_srcdir)
-                                compiledb_srcdir.unlink()
-                                logging.debug(
-                                    'copying compilation database from %s to %s', self.build_dir, self.source_dir
-                                )
-                            shutil.copy(compiledb, self.source_dir)
-                else:
-                    copy_std_output_to_sys(result)
+        # NB: disable weird error on pre-commit CI
+        # pylint: disable=no-member
 
-                self.history.append(result)
-                returncode = result.returncode
-            configuring.unlink()
-        else:
-            returncode = 0
-            with rw_lock.read_lock():
-                pass
+        cmake_configure_try_lock = filelock.FileLock(cmake_configure_try_lock_file)
+        cmake_configure_lock = fasteners.InterProcessReaderWriterLock(cmake_configure_lock_file)
+        try:
+            with cmake_configure_try_lock.acquire(blocking=False):
+                with cmake_configure_lock.write_lock():
+                    logging.debug('Command %s with id %s is running CMake configure', self.command, os.getpid())
+                    returncode = self._run_cmake_configure((cmake_configure_lock_file, cmake_configure_try_lock_file))
+                    logging.debug('Command %s with id %s is done running CMake configure', self.command, os.getpid())
+        except filelock.Timeout:
+            logging.debug('Command %s with id %s is not running CMake configure and waiting', self.command, os.getpid())
+            with cmake_configure_lock.read_lock():
+                logging.debug('Command %s with id %s is done waiting', self.command, os.getpid())
+                returncode = 0
 
         if returncode != 0:
             sys.exit(returncode)
 
-    def _parse_output(self, result):  # pylint: disable=unused-argument
-        return NotImplemented
-
     def _call_process(self, args, **kwargs):
         try:
             sp_child = sp.run(args, check=True, stdout=sp.PIPE, stderr=sp.PIPE, **kwargs)
         except sp.CalledProcessError as e:
             ret = _History(e.stdout.decode(), e.stderr.decode(), e.returncode)
         else:
             ret = _History(sp_child.stdout.decode(), sp_child.stderr.decode(), sp_child.returncode)
@@ -374,14 +346,63 @@
             logging.debug('command `%s` exited with %d', ' '.join(args), ret.returncode)
             for line in ret.stdout.split('\n'):
                 logging.debug('(stdout) %s', line)
             for line in ret.stderr.split('\n'):
                 logging.debug('(stderr) %s', line)
         return ret
 
+    def _parse_output(self, result):  # pylint: disable=unused-argument
+        return NotImplemented
+
+    def _run_cmake_configure(self, lock_files):  # pylint: disable=too-many-branches
+        """Run a CMake configure step."""
+        self.build_dir.mkdir(exist_ok=True)
+
+        if self.clean_build:
+            for path in self.build_dir.iterdir():
+                if path.is_dir():
+                    shutil.rmtree(path)
+                elif path not in lock_files:
+                    path.unlink()
+
+        result = self._call_process(self.cmake + [str(self.source_dir)] + self.cmake_args, cwd=self.build_dir)
+        result.stdout = '\n'.join(
+            [
+                f'Running CMake with: {self.cmake + [str(self.source_dir)] + self.cmake_args}',
+                f'  from within {self.build_dir}',
+                result.stdout,
+                '',
+            ]
+        )
+
+        if result.returncode == 0:
+            compiledb = Path(self.build_dir, 'compile_commands.json')
+            if not compiledb.exists():
+                result.returncode = 1
+                result.stderr += f'\nUnable to locate {compiledb}\n\n'
+                copy_std_output_to_sys(result)
+            else:
+                compiledb_srcdir = Path(self.source_dir, 'compile_commands.json')
+                if compiledb_srcdir.is_symlink() and compiledb_srcdir.resolve() == compiledb:
+                    # If it's a symbolic link and points to the compilation database in the build directory,
+                    # we're all good.
+                    pass
+                else:
+                    # In all other cases, we copy the compilation database into the source directory
+                    if compiledb_srcdir.is_symlink():
+                        logging.debug('Removing symbolic link at: %s', compiledb_srcdir)
+                        compiledb_srcdir.unlink()
+                        logging.debug('copying compilation database from %s to %s', self.build_dir, self.source_dir)
+                    shutil.copy(compiledb, self.source_dir)
+        else:
+            copy_std_output_to_sys(result)
+
+        self.history.append(result)
+        return result.returncode
+
     def _setup_cmake_args(self, args):  # pylint: disable=too-many-branches
         self.cmake = args.cmake if isinstance(args.cmake, list) else [args.cmake]
         if not self.cmake:
             raise RuntimeError('Unable to locate CMake command')
 
         for define in args.defines:
             self.cmake_args.append(f'-D{define}')
```

### Comparing `cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/clang_format.py` & `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/clang_format.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/clang_tidy.py` & `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/clang_tidy.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/cppcheck.py` & `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/cppcheck.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/cpplint.py` & `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/cpplint.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/include_what_you_use.py` & `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/include_what_you_use.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/cmake_pc_hooks/lizard.py` & `cmake_pre_commit_hooks-1.8.1/cmake_pc_hooks/lizard.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/cmake_pre_commit_hooks.egg-info/PKG-INFO` & `cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake-pre-commit-hooks
-Version: 1.8.0
+Version: 1.8.1
 Summary: pre-commit hooks for CMake based projects
 Home-page: https://github.com/Takishima/cmake-pre-commit-hooks
 Author: Damien Nguyen
 Author-email: ngn.damien@gmail.com
 License: Apache2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -57,15 +57,15 @@
 
 with the following file contents:
 
 __.pre-commit-config.yaml__
 
     repos:
       - repo: https://github.com/Takishima/cmake-pre-commit-hooks
-        rev: 1.0.0
+        rev: v1.8.0
         hooks:
           - id: clang-format
           - id: clang-tidy
             args: [--checks=readability-magic-numbers,--warnings-as-errors=*]
           - id: cppcheck
           - id: include-what-you-use
 
@@ -167,14 +167,15 @@
 | `-S <path-to-source>`        | Explicitly specify a source directory.           |
 | `-B <path-to-build>`         | Explicitly specify a build directory.            |
 | `-D <var>[:<type>]=<value>`  | Create or update a cmake cache entry.            |
 | `-U <globbing_expr>`         | Remove matching entries from CMake cache.        |
 | `-G <generator-name>`        | Specify a build system generator.                |
 | `-T <toolset-name>`          | Specify toolset name if supported by generator.  |
 | `-A <platform-name>`         | Specify platform name if supported by generator. |
+| `--preset <preset>`          | Specify a configure preset.                      |
 | `-Wdev`                      | Enable developer warnings.                       |
 | `-Wno-dev`                   | Suppress developer warnings.                     |
 | `-Werror=dev`                | Make developer warnings errors.                  |
 | `-Wno-error=dev`             | Make developer warnings not errors.              |
 
 One important thing to note (particularly for those that intend to use this on CIs), you may specify the build directory
 argument (`-B`) multiple times. The hooks will then simply cycle through all of the values provided and choose the first
@@ -206,15 +207,15 @@
 
 
 Usage example:
 
 ```yaml
 repos:
 - repo: https://github.com/Takishima/cmake-pre-commit-hooks
-  rev: 1.0.0
+  rev: v1.8.0
   hooks:
     - id: cppcheck
       args: [-DBUILD_TESTING=ON,
              --unix="-DCMAKE_CXX_COMPILER=g++-10",
              --win="-DCMAKE_CXX_COMPILER=cl.exe"
              -Bpath/to/build_dir,
              -Bpath/to/other_build_dir,
```

### Comparing `cmake_pre_commit_hooks-1.8.0/cmake_pre_commit_hooks.egg-info/SOURCES.txt` & `cmake_pre_commit_hooks-1.8.1/cmake_pre_commit_hooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/misc/license_header.txt` & `cmake_pre_commit_hooks-1.8.1/misc/license_header.txt`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/pyproject.toml` & `cmake_pre_commit_hooks-1.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/setup.cfg` & `cmake_pre_commit_hooks-1.8.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 [options]
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	CLinters >= 1.3.0
 	fasteners
+	filelock
 
 [options.entry_points]
 console_scripts = 
 	cmake-pc-clang-format-hook = cmake_pc_hooks.clang_format:main
 	cmake-pc-clang-tidy-hook = cmake_pc_hooks.clang_tidy:main
 	cmake-pc-cppcheck-hook = cmake_pc_hooks.cppcheck:main
 	cmake-pc-cpplint-hook = cmake_pc_hooks.cpplint:main
```

### Comparing `cmake_pre_commit_hooks-1.8.0/setup.py` & `cmake_pre_commit_hooks-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/tests/cmake_bad/.pre-commit-config.yaml` & `cmake_pre_commit_hooks-1.8.1/tests/cmake_bad/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/tests/cmake_good/.pre-commit-config.yaml` & `cmake_pre_commit_hooks-1.8.1/tests/cmake_good/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/tests/run_tests.ps1` & `cmake_pre_commit_hooks-1.8.1/tests/run_tests.ps1`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.8.0/tests/run_tests.sh` & `cmake_pre_commit_hooks-1.8.1/tests/run_tests.sh`

 * *Files identical despite different names*

