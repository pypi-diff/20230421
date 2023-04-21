# Comparing `tmp/conventional_pre_commit-2.1.1.tar.gz` & `tmp/conventional_pre_commit-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conventional_pre_commit-2.1.1.tar", last modified: Thu Sep 22 21:59:44 2022, max compression
+gzip compressed data, was "conventional_pre_commit-2.2.0.tar", last modified: Fri Apr 21 21:47:21 2023, max compression
```

## Comparing `conventional_pre_commit-2.1.1.tar` & `conventional_pre_commit-2.2.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:59:44.334337 conventional_pre_commit-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-22 21:59:34.000000 conventional_pre_commit-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4391 2022-09-22 21:59:44.334337 conventional_pre_commit-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3899 2022-09-22 21:59:34.000000 conventional_pre_commit-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:59:44.334337 conventional_pre_commit-2.1.1/conventional_pre_commit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 21:59:34.000000 conventional_pre_commit-2.1.1/conventional_pre_commit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-09-22 21:59:34.000000 conventional_pre_commit-2.1.1/conventional_pre_commit/format.py
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-09-22 21:59:34.000000 conventional_pre_commit-2.1.1/conventional_pre_commit/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 21:59:44.334337 conventional_pre_commit-2.1.1/conventional_pre_commit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4391 2022-09-22 21:59:44.000000 conventional_pre_commit-2.1.1/conventional_pre_commit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-09-22 21:59:44.000000 conventional_pre_commit-2.1.1/conventional_pre_commit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 21:59:44.000000 conventional_pre_commit-2.1.1/conventional_pre_commit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-22 21:59:44.000000 conventional_pre_commit-2.1.1/conventional_pre_commit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-09-22 21:59:44.000000 conventional_pre_commit-2.1.1/conventional_pre_commit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-09-22 21:59:34.000000 conventional_pre_commit-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-09-22 21:59:44.334337 conventional_pre_commit-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-22 21:59:34.000000 conventional_pre_commit-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:47:21.734058 conventional_pre_commit-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-04-21 21:47:21.734058 conventional_pre_commit-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:47:21.734058 conventional_pre_commit-2.2.0/conventional_pre_commit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/conventional_pre_commit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/conventional_pre_commit/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/conventional_pre_commit/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:47:21.734058 conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-04-21 21:47:21.000000 conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-21 21:47:21.000000 conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 21:47:21.000000 conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-21 21:47:21.000000 conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-21 21:47:21.000000 conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 21:47:21.000000 conventional_pre_commit-2.2.0/conventional_pre_commit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 21:47:21.734058 conventional_pre_commit-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:47:21.734058 conventional_pre_commit-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-21 21:47:04.000000 conventional_pre_commit-2.2.0/tests/test_hook.py
```

### Comparing `conventional_pre_commit-2.1.1/LICENSE` & `conventional_pre_commit-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conventional_pre_commit-2.1.1/PKG-INFO` & `conventional_pre_commit-2.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: conventional_pre_commit
-Version: 2.1.1
-Summary: A pre-commit hook that checks commit messages for Conventional Commits formatting.
-Home-page: https://github.com/compilerla/conventional-pre-commit
-Author: Compiler LLC
-Author-email: dev@compiler.la
-License: Apache 2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # conventional-pre-commit
 
 A [`pre-commit`](https://pre-commit.com) hook to check commit messages for
 [Conventional Commits](https://conventionalcommits.org) formatting.
 
 ## Usage
 
@@ -27,16 +13,15 @@
 touch .pre-commit-config.yaml
 ```
 
 Add a new repo entry to your configuration file:
 
 ```yaml
 repos:
-
-# - repo: ...
+  # - repo: ...
 
   - repo: https://github.com/compilerla/conventional-pre-commit
     rev: <git sha or tag>
     hooks:
       - id: conventional-pre-commit
         stages: [commit-msg]
         args: [] # optional: list of Conventional Commits types to allow e.g. [feat, fix, ci, chore, test]
@@ -103,17 +88,17 @@
 
 Then run the command line script:
 
 ```shell
 conventional-pre-commit [types] input
 ```
 
-Where `[types]` is an optional list of Conventional Commit types to allow (e.g. `feat fix chore`)
+- `[types]` is an optional list of Conventional Commit types to allow (e.g. `feat fix chore`)
 
-And `input` is a file containing the commit message to check:
+- `input` is a file containing the commit message to check:
 
 ```shell
 conventional-pre-commit feat fix chore ci test .git/COMMIT_MSG
 ```
 
 Or from a Python program:
 
@@ -126,18 +111,14 @@
 # prints False
 print(is_conventional("nope: this is not a conventional commit"))
 
 # prints True
 print(is_conventional("custom: this is a conventional commit", types=["custom"]))
 ```
 
-## Versioning
-
-Versioning generally follows [Semantic Versioning](https://semver.org/).
-
 ## Development
 
 `conventional-pre-commit` comes with a [VS Code devcontainer](https://code.visualstudio.com/learn/develop-cloud/containers)
 configuration to provide a consistent development environment.
 
 With the `Remote - Containers` extension enabled, open the folder containing this repository inside Visual Studio Code.
 
@@ -147,12 +128,35 @@
 If you do not receive a prompt, or when you feel like starting from a fresh environment:
 
 1. `Ctrl/Cmd+Shift+P` to bring up the command palette in Visual Studio Code
 1. Type `Remote-Containers` to filter the commands
 1. Select `Rebuild and Reopen in Container` to completely rebuild the devcontainer
 1. Select `Reopen in Container` to reopen the most recent devcontainer build
 
+## Versioning
+
+Versioning generally follows [Semantic Versioning](https://semver.org/).
+
+## Making a release
+
+Releases to PyPI are triggered by [publishing a release on GitHub](https://github.com/compilerla/conventional-pre-commit/releases/new).
+
+1. Create a branch `chore/release`
+1. Bump the version in `pyproject.toml`
+1. PR, merge `chore/release` into `main`
+1. Tag `main` with the new version (prefixed by `v`):
+
+   ```bash
+   git fetch
+   git reset --hard origin/main
+   git tag vX.Y.Z
+   git push origin vX.Y.Z
+   ```
+
+1. Publish a pre-release to push the new package to TestPyPI
+1. Publish a regular Release to push the new package to PyPI
+
 ## License
 
 [Apache 2.0](LICENSE)
 
 Inspired by matthorgan's [`pre-commit-conventional-commits`](https://github.com/matthorgan/pre-commit-conventional-commits).
```

### Comparing `conventional_pre_commit-2.1.1/conventional_pre_commit/format.py` & `conventional_pre_commit-2.2.0/conventional_pre_commit/format.py`

 * *Files identical despite different names*

### Comparing `conventional_pre_commit-2.1.1/conventional_pre_commit/hook.py` & `conventional_pre_commit-2.2.0/conventional_pre_commit/hook.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,16 +25,28 @@
         argv = sys.argv[1:]
 
     try:
         args = parser.parse_args(argv)
     except SystemExit:
         return RESULT_FAIL
 
-    with open(args.input) as f:
-        message = f.read()
+    try:
+        with open(args.input, encoding="utf-8") as f:
+            message = f.read()
+    except UnicodeDecodeError:
+        print(
+            f"""
+{Colors.LRED}[Bad Commit message encoding] {Colors.RESTORE}
+
+{Colors.YELLOW}conventional-pre-commit couldn't decode your commit message.{Colors.RESTORE}
+{Colors.YELLOW}UTF-8{Colors.RESTORE} encoding is assumed, please configure git to write commit messages in UTF-8.
+See {Colors.LBLUE}https://git-scm.com/docs/git-commit/#_discussion{Colors.RESTORE} for more.
+        """
+        )
+        return RESULT_FAIL
 
     if format.is_conventional(message, args.types):
         return RESULT_SUCCESS
     else:
         print(
             f"""
         {Colors.LRED}[Bad Commit message] >>{Colors.RESTORE} {message}
```

