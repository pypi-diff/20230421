# Comparing `tmp/llm4gpt-2023.4.21.14.7.31.tar.gz` & `tmp/llm4gpt-2023.4.21.14.8.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4gpt-2023.4.21.14.7.31.tar", last modified: Fri Apr 21 06:07:31 2023, max compression
+gzip compressed data, was "llm4gpt-2023.4.21.14.8.20.tar", last modified: Fri Apr 21 06:08:20 2023, max compression
```

## Comparing `llm4gpt-2023.4.21.14.7.31.tar` & `llm4gpt-2023.4.21.14.8.20.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:07:31.955435 llm4gpt-2023.4.21.14.7.31/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4gpt-2023.4.21.14.7.31/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 06:07:31.955535 llm4gpt-2023.4.21.14.7.31/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4gpt-2023.4.21.14.7.31/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:07:31.944057 llm4gpt-2023.4.21.14.7.31/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:07:31.946604 llm4gpt-2023.4.21.14.7.31/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4gpt-2023.4.21.14.7.31/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4gpt-2023.4.21.14.7.31/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.7.31/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.7.31/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.7.31/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.7.31/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:07:31.951462 llm4gpt-2023.4.21.14.7.31/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4gpt-2023.4.21.14.7.31/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4gpt-2023.4.21.14.7.31/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4gpt-2023.4.21.14.7.31/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:07:31.951983 llm4gpt-2023.4.21.14.7.31/llm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/llm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:07:31.952237 llm4gpt-2023.4.21.14.7.31/llm/ann/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 llm4gpt-2023.4.21.14.7.31/llm/ann/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 llm4gpt-2023.4.21.14.7.31/llm/ann/lite.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:07:31.952736 llm4gpt-2023.4.21.14.7.31/llm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 llm4gpt-2023.4.21.14.7.31/llm/applications/ChatPDF.py
--rw-r--r--   0 betterme   (501) staff       (20)     2678 2023-04-21 06:07:31.000000 llm4gpt-2023.4.21.14.7.31/llm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-21 05:07:18.000000 llm4gpt-2023.4.21.14.7.31/llm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 llm4gpt-2023.4.21.14.7.31/llm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.14.7.31/llm/chatllm.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:07:31.953110 llm4gpt-2023.4.21.14.7.31/llm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/llm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/llm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/llm/clis/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:07:31.953524 llm4gpt-2023.4.21.14.7.31/llm/docutils/
--rw-r--r--   0 betterme   (501) staff       (20)      295 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.14.7.31/llm/docutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-04-21 05:15:17.000000 llm4gpt-2023.4.21.14.7.31/llm/docutils/doc_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.14.7.31/llm/docutils/doc_parse.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:07:31.953972 llm4gpt-2023.4.21.14.7.31/llm/kb/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 llm4gpt-2023.4.21.14.7.31/llm/kb/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4gpt-2023.4.21.14.7.31/llm/kb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 llm4gpt-2023.4.21.14.7.31/llm/kb/kbqa.py
--rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.14.7.31/llm/qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:07:31.954121 llm4gpt-2023.4.21.14.7.31/llm/uis/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.21.14.7.31/llm/uis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2710 2023-04-21 05:19:03.000000 llm4gpt-2023.4.21.14.7.31/llm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:07:31.955032 llm4gpt-2023.4.21.14.7.31/llm4gpt.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 06:07:31.000000 llm4gpt-2023.4.21.14.7.31/llm4gpt.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1242 2023-04-21 06:07:31.000000 llm4gpt-2023.4.21.14.7.31/llm4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 06:07:31.000000 llm4gpt-2023.4.21.14.7.31/llm4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-21 06:07:31.000000 llm4gpt-2023.4.21.14.7.31/llm4gpt.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 06:07:31.000000 llm4gpt-2023.4.21.14.7.31/llm4gpt.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-21 06:07:31.000000 llm4gpt-2023.4.21.14.7.31/llm4gpt.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-21 06:07:31.000000 llm4gpt-2023.4.21.14.7.31/llm4gpt.egg-info/top_level.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 llm4gpt-2023.4.21.14.7.31/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-21 06:07:31.955864 llm4gpt-2023.4.21.14.7.31/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.21.14.7.31/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:07:31.955311 llm4gpt-2023.4.21.14.7.31/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.7.31/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:08:20.495220 llm4gpt-2023.4.21.14.8.20/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4gpt-2023.4.21.14.8.20/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 06:08:20.495320 llm4gpt-2023.4.21.14.8.20/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4gpt-2023.4.21.14.8.20/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:08:20.484586 llm4gpt-2023.4.21.14.8.20/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:08:20.486894 llm4gpt-2023.4.21.14.8.20/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4gpt-2023.4.21.14.8.20/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4gpt-2023.4.21.14.8.20/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.8.20/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.8.20/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.8.20/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.14.8.20/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:08:20.491102 llm4gpt-2023.4.21.14.8.20/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4gpt-2023.4.21.14.8.20/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4gpt-2023.4.21.14.8.20/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4gpt-2023.4.21.14.8.20/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:08:20.491602 llm4gpt-2023.4.21.14.8.20/llm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/llm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:08:20.491844 llm4gpt-2023.4.21.14.8.20/llm/ann/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 llm4gpt-2023.4.21.14.8.20/llm/ann/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 llm4gpt-2023.4.21.14.8.20/llm/ann/lite.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:08:20.492348 llm4gpt-2023.4.21.14.8.20/llm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 llm4gpt-2023.4.21.14.8.20/llm/applications/ChatPDF.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2664 2023-04-21 06:08:19.000000 llm4gpt-2023.4.21.14.8.20/llm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-21 05:07:18.000000 llm4gpt-2023.4.21.14.8.20/llm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 llm4gpt-2023.4.21.14.8.20/llm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.14.8.20/llm/chatllm.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:08:20.492748 llm4gpt-2023.4.21.14.8.20/llm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/llm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/llm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/llm/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:08:20.493142 llm4gpt-2023.4.21.14.8.20/llm/docutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      295 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.14.8.20/llm/docutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-04-21 05:15:17.000000 llm4gpt-2023.4.21.14.8.20/llm/docutils/doc_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.14.8.20/llm/docutils/doc_parse.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:08:20.493561 llm4gpt-2023.4.21.14.8.20/llm/kb/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 llm4gpt-2023.4.21.14.8.20/llm/kb/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4gpt-2023.4.21.14.8.20/llm/kb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 llm4gpt-2023.4.21.14.8.20/llm/kb/kbqa.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.14.8.20/llm/qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:08:20.493759 llm4gpt-2023.4.21.14.8.20/llm/uis/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.21.14.8.20/llm/uis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2710 2023-04-21 05:19:03.000000 llm4gpt-2023.4.21.14.8.20/llm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:08:20.494835 llm4gpt-2023.4.21.14.8.20/llm4gpt.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 06:08:20.000000 llm4gpt-2023.4.21.14.8.20/llm4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1242 2023-04-21 06:08:20.000000 llm4gpt-2023.4.21.14.8.20/llm4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 06:08:20.000000 llm4gpt-2023.4.21.14.8.20/llm4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-21 06:08:20.000000 llm4gpt-2023.4.21.14.8.20/llm4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 06:08:20.000000 llm4gpt-2023.4.21.14.8.20/llm4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-21 06:08:20.000000 llm4gpt-2023.4.21.14.8.20/llm4gpt.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-21 06:08:20.000000 llm4gpt-2023.4.21.14.8.20/llm4gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 llm4gpt-2023.4.21.14.8.20/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-21 06:08:20.495627 llm4gpt-2023.4.21.14.8.20/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.21.14.8.20/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 06:08:20.495092 llm4gpt-2023.4.21.14.8.20/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.14.8.20/tox.ini
```

### Comparing `llm4gpt-2023.4.21.14.7.31/.gitignore` & `llm4gpt-2023.4.21.14.8.20/.gitignore`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/.travis.yml` & `llm4gpt-2023.4.21.14.8.20/.travis.yml`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/CONTRIBUTING.rst` & `llm4gpt-2023.4.21.14.8.20/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/LICENSE` & `llm4gpt-2023.4.21.14.8.20/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/Makefile` & `llm4gpt-2023.4.21.14.8.20/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/PKG-INFO` & `llm4gpt-2023.4.21.14.8.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.21.14.7.31
+Version: 2023.4.21.14.8.20
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.21.14.7.31/README.md` & `llm4gpt-2023.4.21.14.8.20/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/README.rst` & `llm4gpt-2023.4.21.14.8.20/README.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/data/医/500种中药现代研究.txt` & `llm4gpt-2023.4.21.14.8.20/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/data/医/古今医统大全.txt` & `llm4gpt-2023.4.21.14.8.20/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/data/姚明.txt` & `llm4gpt-2023.4.21.14.8.20/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/data/王治郅.txt` & `llm4gpt-2023.4.21.14.8.20/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/data/科比.txt` & `llm4gpt-2023.4.21.14.8.20/data/科比.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/docs/Makefile` & `llm4gpt-2023.4.21.14.8.20/docs/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/docs/README.md` & `llm4gpt-2023.4.21.14.8.20/docs/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/docs/conf.py` & `llm4gpt-2023.4.21.14.8.20/docs/conf.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/docs/img.png` & `llm4gpt-2023.4.21.14.8.20/docs/img.png`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/docs/installation.rst` & `llm4gpt-2023.4.21.14.8.20/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/docs/make.bat` & `llm4gpt-2023.4.21.14.8.20/docs/make.bat`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/llm/applications/Question2Answer.py` & `llm4gpt-2023.4.21.14.8.20/llm/applications/Question2Answer.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,21 +30,21 @@
     def crawler4qa(self, query,
                    url="https://top.baidu.com/board?tab=realtime",
                    xpath='//*[@id="sanRoot"]/main/div[2]/div/div[2]/div[*]/div[2]/a/div[1]//text()', **kwargs):
         knowledge_base = Crawler(url).xpath(xpath)
 
         return self.qa(query, knowledge_base, **kwargs)
 
-    def ann4qa(self, query, query_embedd=None, da: DocumentArray = None, max_turns=1, topk=3):
+    def ann4qa(self, query, query_embedd=None, da: DocumentArray = None, topk=3, **kwargs):
 
         # ann召回知识
         v = query_embedd(query)
         knowledge_base = da.find(v, topk=topk)[0].texts  # [:, ('text', 'scores__cosine__value')]
 
-        return self.qa(query, knowledge_base, max_turns=max_turns)
+        return self.qa(query, knowledge_base, **kwargs)
 
     @clear_cuda_cache
     def qa(self, query, knowledge_base='', max_turns=1, print_knowledge_base=True):
         if knowledge_base:
             query = self.prompt_template.format(context=knowledge_base, question=query)
 
             if print_knowledge_base:
```

### Comparing `llm4gpt-2023.4.21.14.7.31/llm/chatllm.py` & `llm4gpt-2023.4.21.14.8.20/llm/chatllm.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/llm/clis/cli.py` & `llm4gpt-2023.4.21.14.8.20/llm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/llm/docutils/doc_embedding.py` & `llm4gpt-2023.4.21.14.8.20/llm/docutils/doc_embedding.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/llm/kb/FaissANN.py` & `llm4gpt-2023.4.21.14.8.20/llm/kb/FaissANN.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/llm/qa.py` & `llm4gpt-2023.4.21.14.8.20/llm/qa.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/llm/utils.py` & `llm4gpt-2023.4.21.14.8.20/llm/utils.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/llm4gpt.egg-info/PKG-INFO` & `llm4gpt-2023.4.21.14.8.20/llm4gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.21.14.7.31
+Version: 2023.4.21.14.8.20
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.21.14.7.31/llm4gpt.egg-info/SOURCES.txt` & `llm4gpt-2023.4.21.14.8.20/llm4gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/setup.py` & `llm4gpt-2023.4.21.14.8.20/setup.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.21.14.7.31/tests/test_llm4gpt.py` & `llm4gpt-2023.4.21.14.8.20/tests/test_llm4gpt.py`

 * *Files identical despite different names*

