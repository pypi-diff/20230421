# Comparing `tmp/llm4gpt-2023.4.21.14.0.12.tar.gz` & `tmp/llm4gpt-2023.4.21.14.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4gpt-2023.4.21.14.0.12.tar", last modified: Fri Apr 21 06:00:12 2023, max compression
+gzip compressed data, was "llm4gpt-2023.4.21.14.1.34.tar", last modified: Fri Apr 21 06:01:34 2023, max compression
```

## Comparing `llm4gpt-2023.4.21.14.0.12.tar` & `llm4gpt-2023.4.21.14.1.34.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:00:12.537486 llm4gpt-2023.4.21.14.0.12/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4gpt-2023.4.21.14.0.12/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 06:00:12.537577 llm4gpt-2023.4.21.14.0.12/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4gpt-2023.4.21.14.0.12/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:00:12.527157 llm4gpt-2023.4.21.14.0.12/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:00:12.529554 llm4gpt-2023.4.21.14.0.12/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4gpt-2023.4.21.14.0.12/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4gpt-2023.4.21.14.0.12/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.0.12/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.0.12/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.0.12/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.0.12/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:00:12.533765 llm4gpt-2023.4.21.14.0.12/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4gpt-2023.4.21.14.0.12/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4gpt-2023.4.21.14.0.12/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4gpt-2023.4.21.14.0.12/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:00:12.534248 llm4gpt-2023.4.21.14.0.12/llm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/llm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:00:12.534503 llm4gpt-2023.4.21.14.0.12/llm/ann/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 llm4gpt-2023.4.21.14.0.12/llm/ann/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 llm4gpt-2023.4.21.14.0.12/llm/ann/lite.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:00:12.535010 llm4gpt-2023.4.21.14.0.12/llm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 llm4gpt-2023.4.21.14.0.12/llm/applications/ChatPDF.py
--rw-r--r--   0 betterme   (501) staff       (20)     2563 2023-04-21 06:00:10.000000 llm4gpt-2023.4.21.14.0.12/llm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-21 05:07:18.000000 llm4gpt-2023.4.21.14.0.12/llm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 llm4gpt-2023.4.21.14.0.12/llm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.14.0.12/llm/chatllm.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:00:12.535403 llm4gpt-2023.4.21.14.0.12/llm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/llm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/llm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/llm/clis/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:00:12.535770 llm4gpt-2023.4.21.14.0.12/llm/docutils/
--rw-r--r--   0 betterme   (501) staff       (20)      295 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.14.0.12/llm/docutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-04-21 05:15:17.000000 llm4gpt-2023.4.21.14.0.12/llm/docutils/doc_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.14.0.12/llm/docutils/doc_parse.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:00:12.536155 llm4gpt-2023.4.21.14.0.12/llm/kb/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 llm4gpt-2023.4.21.14.0.12/llm/kb/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4gpt-2023.4.21.14.0.12/llm/kb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 llm4gpt-2023.4.21.14.0.12/llm/kb/kbqa.py
--rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.14.0.12/llm/qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:00:12.536272 llm4gpt-2023.4.21.14.0.12/llm/uis/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.21.14.0.12/llm/uis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2710 2023-04-21 05:19:03.000000 llm4gpt-2023.4.21.14.0.12/llm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:00:12.537102 llm4gpt-2023.4.21.14.0.12/llm4gpt.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 06:00:12.000000 llm4gpt-2023.4.21.14.0.12/llm4gpt.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1242 2023-04-21 06:00:12.000000 llm4gpt-2023.4.21.14.0.12/llm4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 06:00:12.000000 llm4gpt-2023.4.21.14.0.12/llm4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-21 06:00:12.000000 llm4gpt-2023.4.21.14.0.12/llm4gpt.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 06:00:12.000000 llm4gpt-2023.4.21.14.0.12/llm4gpt.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-21 06:00:12.000000 llm4gpt-2023.4.21.14.0.12/llm4gpt.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-21 06:00:12.000000 llm4gpt-2023.4.21.14.0.12/llm4gpt.egg-info/top_level.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 llm4gpt-2023.4.21.14.0.12/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-21 06:00:12.537894 llm4gpt-2023.4.21.14.0.12/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.21.14.0.12/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:00:12.537369 llm4gpt-2023.4.21.14.0.12/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.0.12/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:01:34.319884 llm4gpt-2023.4.21.14.1.34/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4gpt-2023.4.21.14.1.34/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 06:01:34.319979 llm4gpt-2023.4.21.14.1.34/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4gpt-2023.4.21.14.1.34/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:01:34.309800 llm4gpt-2023.4.21.14.1.34/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:01:34.312100 llm4gpt-2023.4.21.14.1.34/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4gpt-2023.4.21.14.1.34/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4gpt-2023.4.21.14.1.34/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.1.34/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.1.34/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.1.34/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.1.34/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:01:34.316328 llm4gpt-2023.4.21.14.1.34/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4gpt-2023.4.21.14.1.34/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4gpt-2023.4.21.14.1.34/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4gpt-2023.4.21.14.1.34/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:01:34.316803 llm4gpt-2023.4.21.14.1.34/llm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/llm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:01:34.317043 llm4gpt-2023.4.21.14.1.34/llm/ann/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 llm4gpt-2023.4.21.14.1.34/llm/ann/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 llm4gpt-2023.4.21.14.1.34/llm/ann/lite.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:01:34.317515 llm4gpt-2023.4.21.14.1.34/llm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 llm4gpt-2023.4.21.14.1.34/llm/applications/ChatPDF.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2575 2023-04-21 06:01:29.000000 llm4gpt-2023.4.21.14.1.34/llm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-21 05:07:18.000000 llm4gpt-2023.4.21.14.1.34/llm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 llm4gpt-2023.4.21.14.1.34/llm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.14.1.34/llm/chatllm.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:01:34.317869 llm4gpt-2023.4.21.14.1.34/llm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/llm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/llm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/llm/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:01:34.318238 llm4gpt-2023.4.21.14.1.34/llm/docutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      295 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.14.1.34/llm/docutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-04-21 05:15:17.000000 llm4gpt-2023.4.21.14.1.34/llm/docutils/doc_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.14.1.34/llm/docutils/doc_parse.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:01:34.318599 llm4gpt-2023.4.21.14.1.34/llm/kb/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 llm4gpt-2023.4.21.14.1.34/llm/kb/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4gpt-2023.4.21.14.1.34/llm/kb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 llm4gpt-2023.4.21.14.1.34/llm/kb/kbqa.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.14.1.34/llm/qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:01:34.318714 llm4gpt-2023.4.21.14.1.34/llm/uis/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.21.14.1.34/llm/uis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2710 2023-04-21 05:19:03.000000 llm4gpt-2023.4.21.14.1.34/llm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:01:34.319521 llm4gpt-2023.4.21.14.1.34/llm4gpt.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 06:01:34.000000 llm4gpt-2023.4.21.14.1.34/llm4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1242 2023-04-21 06:01:34.000000 llm4gpt-2023.4.21.14.1.34/llm4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 06:01:34.000000 llm4gpt-2023.4.21.14.1.34/llm4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-21 06:01:34.000000 llm4gpt-2023.4.21.14.1.34/llm4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 06:01:34.000000 llm4gpt-2023.4.21.14.1.34/llm4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-21 06:01:34.000000 llm4gpt-2023.4.21.14.1.34/llm4gpt.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-21 06:01:34.000000 llm4gpt-2023.4.21.14.1.34/llm4gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 llm4gpt-2023.4.21.14.1.34/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-21 06:01:34.320290 llm4gpt-2023.4.21.14.1.34/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.21.14.1.34/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:01:34.319772 llm4gpt-2023.4.21.14.1.34/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.1.34/tox.ini
```

### Comparing `llm4gpt-2023.4.21.14.0.12/.gitignore` & `llm4gpt-2023.4.21.14.1.34/.gitignore`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/.travis.yml` & `llm4gpt-2023.4.21.14.1.34/.travis.yml`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/CONTRIBUTING.rst` & `llm4gpt-2023.4.21.14.1.34/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/LICENSE` & `llm4gpt-2023.4.21.14.1.34/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/Makefile` & `llm4gpt-2023.4.21.14.1.34/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/PKG-INFO` & `llm4gpt-2023.4.21.14.1.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.21.14.0.12
+Version: 2023.4.21.14.1.34
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.21.14.0.12/README.md` & `llm4gpt-2023.4.21.14.1.34/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/README.rst` & `llm4gpt-2023.4.21.14.1.34/README.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/data/医/500种中药现代研究.txt` & `llm4gpt-2023.4.21.14.1.34/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/data/医/古今医统大全.txt` & `llm4gpt-2023.4.21.14.1.34/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/data/姚明.txt` & `llm4gpt-2023.4.21.14.1.34/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/data/王治郅.txt` & `llm4gpt-2023.4.21.14.1.34/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/data/科比.txt` & `llm4gpt-2023.4.21.14.1.34/data/科比.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/docs/Makefile` & `llm4gpt-2023.4.21.14.1.34/docs/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/docs/README.md` & `llm4gpt-2023.4.21.14.1.34/docs/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/docs/conf.py` & `llm4gpt-2023.4.21.14.1.34/docs/conf.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/docs/img.png` & `llm4gpt-2023.4.21.14.1.34/docs/img.png`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/docs/installation.rst` & `llm4gpt-2023.4.21.14.1.34/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/docs/make.bat` & `llm4gpt-2023.4.21.14.1.34/docs/make.bat`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/llm/applications/Question2Answer.py` & `llm4gpt-2023.4.21.14.1.34/llm/applications/Question2Answer.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                    url="https://top.baidu.com/board?tab=realtime",
                    xpath='//*[@id="sanRoot"]/main/div[2]/div/div[2]/div[*]/div[2]/a/div[1]//text()'
                    ):
         knowledge_base = Crawler(url).xpath(xpath)
 
         return self.qa(query, knowledge_base)
 
-    def ann4qa(self, query, max_turns=1, topk=3, query_embedd, da: DocumentArray):
+    def ann4qa(self, query, query_embedd=None, da: DocumentArray = None, max_turns=1, topk=3):
 
         # ann召回知识
         v = query_embedd(query)
         knowledge_base = da.find(v, topk=topk)[0].texts  # [:, ('text', 'scores__cosine__value')]
 
         return self.qa(query, knowledge_base, max_turns=max_turns)
```

### Comparing `llm4gpt-2023.4.21.14.0.12/llm/chatllm.py` & `llm4gpt-2023.4.21.14.1.34/llm/chatllm.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/llm/clis/cli.py` & `llm4gpt-2023.4.21.14.1.34/llm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/llm/docutils/doc_embedding.py` & `llm4gpt-2023.4.21.14.1.34/llm/docutils/doc_embedding.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/llm/kb/FaissANN.py` & `llm4gpt-2023.4.21.14.1.34/llm/kb/FaissANN.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/llm/qa.py` & `llm4gpt-2023.4.21.14.1.34/llm/qa.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/llm/utils.py` & `llm4gpt-2023.4.21.14.1.34/llm/utils.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/llm4gpt.egg-info/PKG-INFO` & `llm4gpt-2023.4.21.14.1.34/llm4gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.21.14.0.12
+Version: 2023.4.21.14.1.34
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.21.14.0.12/llm4gpt.egg-info/SOURCES.txt` & `llm4gpt-2023.4.21.14.1.34/llm4gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/setup.py` & `llm4gpt-2023.4.21.14.1.34/setup.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.0.12/tests/test_llm4gpt.py` & `llm4gpt-2023.4.21.14.1.34/tests/test_llm4gpt.py`

 * *Files identical despite different names*

