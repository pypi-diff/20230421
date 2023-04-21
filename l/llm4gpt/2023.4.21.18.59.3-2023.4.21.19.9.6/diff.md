# Comparing `tmp/llm4gpt-2023.4.21.18.59.3.tar.gz` & `tmp/llm4gpt-2023.4.21.19.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4gpt-2023.4.21.18.59.3.tar", last modified: Fri Apr 21 10:59:03 2023, max compression
+gzip compressed data, was "llm4gpt-2023.4.21.19.9.6.tar", last modified: Fri Apr 21 11:09:06 2023, max compression
```

## Comparing `llm4gpt-2023.4.21.18.59.3.tar` & `llm4gpt-2023.4.21.19.9.6.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:59:03.602306 llm4gpt-2023.4.21.18.59.3/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4gpt-2023.4.21.18.59.3/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 10:59:03.602409 llm4gpt-2023.4.21.18.59.3/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4gpt-2023.4.21.18.59.3/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:59:03.582986 llm4gpt-2023.4.21.18.59.3/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:59:03.585571 llm4gpt-2023.4.21.18.59.3/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4gpt-2023.4.21.18.59.3/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4gpt-2023.4.21.18.59.3/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.18.59.3/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.18.59.3/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.18.59.3/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.18.59.3/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:59:03.598386 llm4gpt-2023.4.21.18.59.3/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4gpt-2023.4.21.18.59.3/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4gpt-2023.4.21.18.59.3/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4gpt-2023.4.21.18.59.3/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:59:03.598922 llm4gpt-2023.4.21.18.59.3/llm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/llm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:59:03.599434 llm4gpt-2023.4.21.18.59.3/llm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 llm4gpt-2023.4.21.18.59.3/llm/applications/ChatPDF.py
--rw-r--r--   0 betterme   (501) staff       (20)     3293 2023-04-21 10:46:58.000000 llm4gpt-2023.4.21.18.59.3/llm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-21 05:07:18.000000 llm4gpt-2023.4.21.18.59.3/llm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 llm4gpt-2023.4.21.18.59.3/llm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1798 2023-04-21 10:59:01.000000 llm4gpt-2023.4.21.18.59.3/llm/chatllm.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:59:03.599818 llm4gpt-2023.4.21.18.59.3/llm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/llm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/llm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/llm/clis/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:59:03.600201 llm4gpt-2023.4.21.18.59.3/llm/docutils/
--rw-r--r--   0 betterme   (501) staff       (20)      295 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.18.59.3/llm/docutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 07:32:03.000000 llm4gpt-2023.4.21.18.59.3/llm/docutils/doc_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.18.59.3/llm/docutils/doc_parse.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:59:03.600590 llm4gpt-2023.4.21.18.59.3/llm/kb/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 llm4gpt-2023.4.21.18.59.3/llm/kb/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4gpt-2023.4.21.18.59.3/llm/kb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 llm4gpt-2023.4.21.18.59.3/llm/kb/kbqa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:59:03.600869 llm4gpt-2023.4.21.18.59.3/llm/knowledge_base/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 llm4gpt-2023.4.21.18.59.3/llm/knowledge_base/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 llm4gpt-2023.4.21.18.59.3/llm/knowledge_base/lite.py
--rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.18.59.3/llm/qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:59:03.601004 llm4gpt-2023.4.21.18.59.3/llm/uis/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.21.18.59.3/llm/uis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2684 2023-04-21 07:32:03.000000 llm4gpt-2023.4.21.18.59.3/llm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:59:03.601884 llm4gpt-2023.4.21.18.59.3/llm4gpt.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 10:59:03.000000 llm4gpt-2023.4.21.18.59.3/llm4gpt.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1264 2023-04-21 10:59:03.000000 llm4gpt-2023.4.21.18.59.3/llm4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 10:59:03.000000 llm4gpt-2023.4.21.18.59.3/llm4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-21 10:59:03.000000 llm4gpt-2023.4.21.18.59.3/llm4gpt.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 10:59:03.000000 llm4gpt-2023.4.21.18.59.3/llm4gpt.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-21 10:59:03.000000 llm4gpt-2023.4.21.18.59.3/llm4gpt.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-21 10:59:03.000000 llm4gpt-2023.4.21.18.59.3/llm4gpt.egg-info/top_level.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 llm4gpt-2023.4.21.18.59.3/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-21 10:59:03.602720 llm4gpt-2023.4.21.18.59.3/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.21.18.59.3/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:59:03.602165 llm4gpt-2023.4.21.18.59.3/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.59.3/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 11:09:06.848066 llm4gpt-2023.4.21.19.9.6/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4gpt-2023.4.21.19.9.6/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     2119 2023-04-21 11:09:06.848169 llm4gpt-2023.4.21.19.9.6/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4gpt-2023.4.21.19.9.6/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 11:09:06.822398 llm4gpt-2023.4.21.19.9.6/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 11:09:06.826209 llm4gpt-2023.4.21.19.9.6/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4gpt-2023.4.21.19.9.6/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4gpt-2023.4.21.19.9.6/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.19.9.6/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.19.9.6/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.19.9.6/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.19.9.6/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 11:09:06.841085 llm4gpt-2023.4.21.19.9.6/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4gpt-2023.4.21.19.9.6/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4gpt-2023.4.21.19.9.6/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4gpt-2023.4.21.19.9.6/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 11:09:06.842035 llm4gpt-2023.4.21.19.9.6/llm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/llm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 11:09:06.843377 llm4gpt-2023.4.21.19.9.6/llm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 llm4gpt-2023.4.21.19.9.6/llm/applications/ChatPDF.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3293 2023-04-21 10:46:58.000000 llm4gpt-2023.4.21.19.9.6/llm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-21 05:07:18.000000 llm4gpt-2023.4.21.19.9.6/llm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 llm4gpt-2023.4.21.19.9.6/llm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1798 2023-04-21 10:59:01.000000 llm4gpt-2023.4.21.19.9.6/llm/chatllm.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 11:09:06.843976 llm4gpt-2023.4.21.19.9.6/llm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/llm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/llm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/llm/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 11:09:06.844677 llm4gpt-2023.4.21.19.9.6/llm/docutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      295 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.19.9.6/llm/docutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 07:32:03.000000 llm4gpt-2023.4.21.19.9.6/llm/docutils/doc_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.19.9.6/llm/docutils/doc_parse.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 11:09:06.845686 llm4gpt-2023.4.21.19.9.6/llm/kb/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 llm4gpt-2023.4.21.19.9.6/llm/kb/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4gpt-2023.4.21.19.9.6/llm/kb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 llm4gpt-2023.4.21.19.9.6/llm/kb/kbqa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 11:09:06.846269 llm4gpt-2023.4.21.19.9.6/llm/knowledge_base/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 llm4gpt-2023.4.21.19.9.6/llm/knowledge_base/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 llm4gpt-2023.4.21.19.9.6/llm/knowledge_base/lite.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.19.9.6/llm/qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 11:09:06.846528 llm4gpt-2023.4.21.19.9.6/llm/uis/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.21.19.9.6/llm/uis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2684 2023-04-21 07:32:03.000000 llm4gpt-2023.4.21.19.9.6/llm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 11:09:06.847627 llm4gpt-2023.4.21.19.9.6/llm4gpt.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     2119 2023-04-21 11:09:06.000000 llm4gpt-2023.4.21.19.9.6/llm4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1264 2023-04-21 11:09:06.000000 llm4gpt-2023.4.21.19.9.6/llm4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 11:09:06.000000 llm4gpt-2023.4.21.19.9.6/llm4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-21 11:09:06.000000 llm4gpt-2023.4.21.19.9.6/llm4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 11:09:06.000000 llm4gpt-2023.4.21.19.9.6/llm4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-21 11:09:06.000000 llm4gpt-2023.4.21.19.9.6/llm4gpt.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-21 11:09:06.000000 llm4gpt-2023.4.21.19.9.6/llm4gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 llm4gpt-2023.4.21.19.9.6/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-21 11:09:06.848480 llm4gpt-2023.4.21.19.9.6/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.21.19.9.6/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 11:09:06.847921 llm4gpt-2023.4.21.19.9.6/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.19.9.6/tox.ini
```

### Comparing `llm4gpt-2023.4.21.18.59.3/.gitignore` & `llm4gpt-2023.4.21.19.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/.travis.yml` & `llm4gpt-2023.4.21.19.9.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/CONTRIBUTING.rst` & `llm4gpt-2023.4.21.19.9.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/LICENSE` & `llm4gpt-2023.4.21.19.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/Makefile` & `llm4gpt-2023.4.21.19.9.6/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/PKG-INFO` & `llm4gpt-2023.4.21.19.9.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.21.18.59.3
+Version: 2023.4.21.19.9.6
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.21.18.59.3/README.md` & `llm4gpt-2023.4.21.19.9.6/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/README.rst` & `llm4gpt-2023.4.21.19.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/data/医/500种中药现代研究.txt` & `llm4gpt-2023.4.21.19.9.6/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/data/医/古今医统大全.txt` & `llm4gpt-2023.4.21.19.9.6/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/data/姚明.txt` & `llm4gpt-2023.4.21.19.9.6/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/data/王治郅.txt` & `llm4gpt-2023.4.21.19.9.6/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/data/科比.txt` & `llm4gpt-2023.4.21.19.9.6/data/科比.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/docs/Makefile` & `llm4gpt-2023.4.21.19.9.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/docs/README.md` & `llm4gpt-2023.4.21.19.9.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/docs/conf.py` & `llm4gpt-2023.4.21.19.9.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/docs/img.png` & `llm4gpt-2023.4.21.19.9.6/docs/img.png`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/docs/installation.rst` & `llm4gpt-2023.4.21.19.9.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/docs/make.bat` & `llm4gpt-2023.4.21.19.9.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/llm/applications/Question2Answer.py` & `llm4gpt-2023.4.21.19.9.6/llm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/llm/chatllm.py` & `llm4gpt-2023.4.21.19.9.6/llm/chatllm.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/llm/clis/cli.py` & `llm4gpt-2023.4.21.19.9.6/llm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/llm/docutils/doc_embedding.py` & `llm4gpt-2023.4.21.19.9.6/llm/docutils/doc_embedding.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/llm/kb/FaissANN.py` & `llm4gpt-2023.4.21.19.9.6/llm/kb/FaissANN.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/llm/qa.py` & `llm4gpt-2023.4.21.19.9.6/llm/qa.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/llm/utils.py` & `llm4gpt-2023.4.21.19.9.6/llm/utils.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/llm4gpt.egg-info/PKG-INFO` & `llm4gpt-2023.4.21.19.9.6/llm4gpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.21.18.59.3
+Version: 2023.4.21.19.9.6
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.21.18.59.3/llm4gpt.egg-info/SOURCES.txt` & `llm4gpt-2023.4.21.19.9.6/llm4gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/setup.py` & `llm4gpt-2023.4.21.19.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.18.59.3/tests/test_llm4gpt.py` & `llm4gpt-2023.4.21.19.9.6/tests/test_llm4gpt.py`

 * *Files identical despite different names*

