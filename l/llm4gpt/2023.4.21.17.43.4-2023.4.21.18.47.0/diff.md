# Comparing `tmp/llm4gpt-2023.4.21.17.43.4.tar.gz` & `tmp/llm4gpt-2023.4.21.18.47.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4gpt-2023.4.21.17.43.4.tar", last modified: Fri Apr 21 09:43:05 2023, max compression
+gzip compressed data, was "llm4gpt-2023.4.21.18.47.0.tar", last modified: Fri Apr 21 10:47:00 2023, max compression
```

## Comparing `llm4gpt-2023.4.21.17.43.4.tar` & `llm4gpt-2023.4.21.18.47.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 09:43:05.100213 llm4gpt-2023.4.21.17.43.4/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4gpt-2023.4.21.17.43.4/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 09:43:05.100313 llm4gpt-2023.4.21.17.43.4/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4gpt-2023.4.21.17.43.4/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 09:43:05.077048 llm4gpt-2023.4.21.17.43.4/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 09:43:05.080818 llm4gpt-2023.4.21.17.43.4/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4gpt-2023.4.21.17.43.4/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4gpt-2023.4.21.17.43.4/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.17.43.4/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.17.43.4/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.17.43.4/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.17.43.4/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 09:43:05.092922 llm4gpt-2023.4.21.17.43.4/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4gpt-2023.4.21.17.43.4/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4gpt-2023.4.21.17.43.4/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4gpt-2023.4.21.17.43.4/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 09:43:05.094382 llm4gpt-2023.4.21.17.43.4/llm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/llm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 09:43:05.095578 llm4gpt-2023.4.21.17.43.4/llm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 llm4gpt-2023.4.21.17.43.4/llm/applications/ChatPDF.py
--rw-r--r--   0 betterme   (501) staff       (20)     2780 2023-04-21 07:34:46.000000 llm4gpt-2023.4.21.17.43.4/llm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-21 05:07:18.000000 llm4gpt-2023.4.21.17.43.4/llm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 llm4gpt-2023.4.21.17.43.4/llm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.17.43.4/llm/chatllm.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 09:43:05.096125 llm4gpt-2023.4.21.17.43.4/llm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/llm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/llm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/llm/clis/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 09:43:05.096829 llm4gpt-2023.4.21.17.43.4/llm/docutils/
--rw-r--r--   0 betterme   (501) staff       (20)      295 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.17.43.4/llm/docutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 07:32:03.000000 llm4gpt-2023.4.21.17.43.4/llm/docutils/doc_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.17.43.4/llm/docutils/doc_parse.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 09:43:05.097757 llm4gpt-2023.4.21.17.43.4/llm/kb/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 llm4gpt-2023.4.21.17.43.4/llm/kb/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4gpt-2023.4.21.17.43.4/llm/kb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 llm4gpt-2023.4.21.17.43.4/llm/kb/kbqa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 09:43:05.098264 llm4gpt-2023.4.21.17.43.4/llm/knowledge_base/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 llm4gpt-2023.4.21.17.43.4/llm/knowledge_base/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 llm4gpt-2023.4.21.17.43.4/llm/knowledge_base/lite.py
--rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.17.43.4/llm/qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 09:43:05.098515 llm4gpt-2023.4.21.17.43.4/llm/uis/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.21.17.43.4/llm/uis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2684 2023-04-21 07:32:03.000000 llm4gpt-2023.4.21.17.43.4/llm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 09:43:05.099714 llm4gpt-2023.4.21.17.43.4/llm4gpt.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 09:43:04.000000 llm4gpt-2023.4.21.17.43.4/llm4gpt.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1264 2023-04-21 09:43:05.000000 llm4gpt-2023.4.21.17.43.4/llm4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 09:43:04.000000 llm4gpt-2023.4.21.17.43.4/llm4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-21 09:43:04.000000 llm4gpt-2023.4.21.17.43.4/llm4gpt.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 09:43:04.000000 llm4gpt-2023.4.21.17.43.4/llm4gpt.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-21 09:43:04.000000 llm4gpt-2023.4.21.17.43.4/llm4gpt.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-21 09:43:04.000000 llm4gpt-2023.4.21.17.43.4/llm4gpt.egg-info/top_level.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 llm4gpt-2023.4.21.17.43.4/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-21 09:43:05.100618 llm4gpt-2023.4.21.17.43.4/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.21.17.43.4/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 09:43:05.100038 llm4gpt-2023.4.21.17.43.4/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.17.43.4/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:47:00.406680 llm4gpt-2023.4.21.18.47.0/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4gpt-2023.4.21.18.47.0/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 10:47:00.406787 llm4gpt-2023.4.21.18.47.0/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4gpt-2023.4.21.18.47.0/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:47:00.380241 llm4gpt-2023.4.21.18.47.0/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:47:00.383942 llm4gpt-2023.4.21.18.47.0/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4gpt-2023.4.21.18.47.0/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4gpt-2023.4.21.18.47.0/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.18.47.0/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.18.47.0/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.18.47.0/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.18.47.0/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:47:00.398265 llm4gpt-2023.4.21.18.47.0/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4gpt-2023.4.21.18.47.0/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4gpt-2023.4.21.18.47.0/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4gpt-2023.4.21.18.47.0/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:47:00.399916 llm4gpt-2023.4.21.18.47.0/llm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/llm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:47:00.400893 llm4gpt-2023.4.21.18.47.0/llm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 llm4gpt-2023.4.21.18.47.0/llm/applications/ChatPDF.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3293 2023-04-21 10:46:58.000000 llm4gpt-2023.4.21.18.47.0/llm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-21 05:07:18.000000 llm4gpt-2023.4.21.18.47.0/llm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 llm4gpt-2023.4.21.18.47.0/llm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.18.47.0/llm/chatllm.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:47:00.401577 llm4gpt-2023.4.21.18.47.0/llm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/llm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/llm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/llm/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:47:00.403599 llm4gpt-2023.4.21.18.47.0/llm/docutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      295 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.18.47.0/llm/docutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 07:32:03.000000 llm4gpt-2023.4.21.18.47.0/llm/docutils/doc_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.18.47.0/llm/docutils/doc_parse.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:47:00.404556 llm4gpt-2023.4.21.18.47.0/llm/kb/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 llm4gpt-2023.4.21.18.47.0/llm/kb/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4gpt-2023.4.21.18.47.0/llm/kb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 llm4gpt-2023.4.21.18.47.0/llm/kb/kbqa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:47:00.405030 llm4gpt-2023.4.21.18.47.0/llm/knowledge_base/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 llm4gpt-2023.4.21.18.47.0/llm/knowledge_base/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 llm4gpt-2023.4.21.18.47.0/llm/knowledge_base/lite.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.18.47.0/llm/qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:47:00.405281 llm4gpt-2023.4.21.18.47.0/llm/uis/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.21.18.47.0/llm/uis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2684 2023-04-21 07:32:03.000000 llm4gpt-2023.4.21.18.47.0/llm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:47:00.406221 llm4gpt-2023.4.21.18.47.0/llm4gpt.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 10:47:00.000000 llm4gpt-2023.4.21.18.47.0/llm4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1264 2023-04-21 10:47:00.000000 llm4gpt-2023.4.21.18.47.0/llm4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 10:47:00.000000 llm4gpt-2023.4.21.18.47.0/llm4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-21 10:47:00.000000 llm4gpt-2023.4.21.18.47.0/llm4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 10:47:00.000000 llm4gpt-2023.4.21.18.47.0/llm4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-21 10:47:00.000000 llm4gpt-2023.4.21.18.47.0/llm4gpt.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-21 10:47:00.000000 llm4gpt-2023.4.21.18.47.0/llm4gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 llm4gpt-2023.4.21.18.47.0/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-21 10:47:00.407080 llm4gpt-2023.4.21.18.47.0/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.21.18.47.0/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 10:47:00.406527 llm4gpt-2023.4.21.18.47.0/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.18.47.0/tox.ini
```

### Comparing `llm4gpt-2023.4.21.17.43.4/.gitignore` & `llm4gpt-2023.4.21.18.47.0/.gitignore`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/.travis.yml` & `llm4gpt-2023.4.21.18.47.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/CONTRIBUTING.rst` & `llm4gpt-2023.4.21.18.47.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/LICENSE` & `llm4gpt-2023.4.21.18.47.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/Makefile` & `llm4gpt-2023.4.21.18.47.0/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/PKG-INFO` & `llm4gpt-2023.4.21.18.47.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.21.17.43.4
+Version: 2023.4.21.18.47.0
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.21.17.43.4/README.md` & `llm4gpt-2023.4.21.18.47.0/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/README.rst` & `llm4gpt-2023.4.21.18.47.0/README.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/data/医/500种中药现代研究.txt` & `llm4gpt-2023.4.21.18.47.0/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/data/医/古今医统大全.txt` & `llm4gpt-2023.4.21.18.47.0/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/data/姚明.txt` & `llm4gpt-2023.4.21.18.47.0/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/data/王治郅.txt` & `llm4gpt-2023.4.21.18.47.0/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/data/科比.txt` & `llm4gpt-2023.4.21.18.47.0/data/科比.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/docs/Makefile` & `llm4gpt-2023.4.21.18.47.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/docs/README.md` & `llm4gpt-2023.4.21.18.47.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/docs/conf.py` & `llm4gpt-2023.4.21.18.47.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/docs/img.png` & `llm4gpt-2023.4.21.18.47.0/docs/img.png`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/docs/installation.rst` & `llm4gpt-2023.4.21.18.47.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/docs/make.bat` & `llm4gpt-2023.4.21.18.47.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/llm/applications/Question2Answer.py` & `llm4gpt-2023.4.21.18.47.0/llm/applications/Question2Answer.py`

 * *Files 17% similar despite different names*

```diff
@@ -54,29 +54,49 @@
         if knowledge_base:
             query = self.prompt_template.format(context=knowledge_base, question=query)
 
             if print_knowledge_base:
                 pprint({'knowledge_base': knowledge_base})
 
         result = self.chat_func(query=query, history=self.history[-max_turns:])
-        response = history = None
+
         if isinstance(result, types.GeneratorType):
-            for response, history in tqdm(result, desc='Stream'):
-                yield response, history
+            return self._stream(result)
         else:
             response, history = result
+            self.history = history  # 历史所有
 
-        self.history = history  # 历史所有
         return response
 
+    def _stream(self, result):  # yield > return
+        history = None
+        for response, history in tqdm(result, desc='Stream'):
+            yield response, history
+        self.history = history
+
     @property
     def default_document_prompt(self):
         prompt_template = """
             基于以下已知信息，简洁和专业的来回答用户的问题。
             如果无法从中得到答案，请说 "根据已知信息无法回答该问题" 或 "没有提供足够的相关信息"，不允许在答案中添加编造成分，答案请使用中文。
             已知内容:
             {context}
             问题:
             {question}
             """.strip()
 
         return prompt_template
+
+
+if __name__ == '__main__':
+    from llm.utils import llm_load
+
+    model, tokenizer = llm_load("/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm")
+    qa = Question2Answer(
+        # chat_func=partial(model.stream_chat, tokenizer=tokenizer),
+        chat_func=partial(model.chat, tokenizer=tokenizer),
+
+    )
+
+    # for i, _ in qa._qa('1+1'):
+    #     print(i, flush=True)
+    print(qa._qa('1+1'))
```

### Comparing `llm4gpt-2023.4.21.17.43.4/llm/chatllm.py` & `llm4gpt-2023.4.21.18.47.0/llm/chatllm.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/llm/clis/cli.py` & `llm4gpt-2023.4.21.18.47.0/llm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/llm/docutils/doc_embedding.py` & `llm4gpt-2023.4.21.18.47.0/llm/docutils/doc_embedding.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/llm/kb/FaissANN.py` & `llm4gpt-2023.4.21.18.47.0/llm/kb/FaissANN.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/llm/qa.py` & `llm4gpt-2023.4.21.18.47.0/llm/qa.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/llm/utils.py` & `llm4gpt-2023.4.21.18.47.0/llm/utils.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/llm4gpt.egg-info/PKG-INFO` & `llm4gpt-2023.4.21.18.47.0/llm4gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.21.17.43.4
+Version: 2023.4.21.18.47.0
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.21.17.43.4/llm4gpt.egg-info/SOURCES.txt` & `llm4gpt-2023.4.21.18.47.0/llm4gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/setup.py` & `llm4gpt-2023.4.21.18.47.0/setup.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.17.43.4/tests/test_llm4gpt.py` & `llm4gpt-2023.4.21.18.47.0/tests/test_llm4gpt.py`

 * *Files identical despite different names*

