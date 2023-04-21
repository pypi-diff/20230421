# Comparing `tmp/llm4gpt-2023.4.20.20.13.57.tar.gz` & `tmp/llm4gpt-2023.4.21.13.7.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4gpt-2023.4.20.20.13.57.tar", last modified: Thu Apr 20 12:13:57 2023, max compression
+gzip compressed data, was "llm4gpt-2023.4.21.13.7.20.tar", last modified: Fri Apr 21 05:07:20 2023, max compression
```

## Comparing `llm4gpt-2023.4.20.20.13.57.tar` & `llm4gpt-2023.4.21.13.7.20.tar`

### file list

```diff
@@ -1,67 +1,84 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.720235 llm4gpt-2023.4.20.20.13.57/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4gpt-2023.4.20.20.13.57/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     2121 2023-04-20 12:13:57.720331 llm4gpt-2023.4.20.20.13.57/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4gpt-2023.4.20.20.13.57/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.711121 llm4gpt-2023.4.20.20.13.57/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.713259 llm4gpt-2023.4.20.20.13.57/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4gpt-2023.4.20.20.13.57/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4gpt-2023.4.20.20.13.57/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.20.13.57/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.20.13.57/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.20.13.57/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4gpt-2023.4.20.20.13.57/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.717766 llm4gpt-2023.4.20.20.13.57/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4gpt-2023.4.20.20.13.57/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4gpt-2023.4.20.20.13.57/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4gpt-2023.4.20.20.13.57/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.718258 llm4gpt-2023.4.20.20.13.57/llm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/llm/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-04-20 12:07:40.000000 llm4gpt-2023.4.20.20.13.57/llm/chatllm.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.718644 llm4gpt-2023.4.20.20.13.57/llm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/llm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/llm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/llm/clis/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.718882 llm4gpt-2023.4.20.20.13.57/llm/kb/
--rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-04-20 10:20:30.000000 llm4gpt-2023.4.20.20.13.57/llm/kb/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4gpt-2023.4.20.20.13.57/llm/kb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4gpt-2023.4.20.20.13.57/llm/qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.719002 llm4gpt-2023.4.20.20.13.57/llm/uis/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.20.20.13.57/llm/uis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2923 2023-04-20 09:28:23.000000 llm4gpt-2023.4.20.20.13.57/llm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.719809 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     2121 2023-04-20 12:13:57.000000 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      988 2023-04-20 12:13:57.000000 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 12:13:57.000000 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-20 12:13:57.000000 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-20 12:13:57.000000 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       18 2023-04-20 12:13:57.000000 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-20 12:13:57.000000 llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/top_level.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-20 11:28:30.000000 llm4gpt-2023.4.20.20.13.57/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-20 12:13:57.720635 llm4gpt-2023.4.20.20.13.57/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.20.20.13.57/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-20 12:13:57.720096 llm4gpt-2023.4.20.20.13.57/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.20.20.13.57/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.939354 llm4gpt-2023.4.21.13.7.20/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4gpt-2023.4.21.13.7.20/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 05:07:20.939455 llm4gpt-2023.4.21.13.7.20/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4gpt-2023.4.21.13.7.20/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.917606 llm4gpt-2023.4.21.13.7.20/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.921035 llm4gpt-2023.4.21.13.7.20/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4gpt-2023.4.21.13.7.20/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4gpt-2023.4.21.13.7.20/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.13.7.20/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.13.7.20/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.13.7.20/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4gpt-2023.4.21.13.7.20/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.932857 llm4gpt-2023.4.21.13.7.20/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4gpt-2023.4.21.13.7.20/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4gpt-2023.4.21.13.7.20/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4gpt-2023.4.21.13.7.20/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.934956 llm4gpt-2023.4.21.13.7.20/llm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/llm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.935318 llm4gpt-2023.4.21.13.7.20/llm/ann/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 llm4gpt-2023.4.21.13.7.20/llm/ann/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 llm4gpt-2023.4.21.13.7.20/llm/ann/lite.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.935836 llm4gpt-2023.4.21.13.7.20/llm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 llm4gpt-2023.4.21.13.7.20/llm/applications/ChatPDF.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2164 2023-04-21 05:06:48.000000 llm4gpt-2023.4.21.13.7.20/llm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-21 05:07:18.000000 llm4gpt-2023.4.21.13.7.20/llm/applications/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.913234 llm4gpt-2023.4.21.13.7.20/llm/cachedir/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.936080 llm4gpt-2023.4.21.13.7.20/llm/cachedir/0fad8225447b1d2ff0229997036dfa9c/
+-rw-r--r--   0 betterme   (501) staff       (20)     6330 2023-04-21 04:16:31.000000 llm4gpt-2023.4.21.13.7.20/llm/cachedir/0fad8225447b1d2ff0229997036dfa9c/__output.pkl
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.936278 llm4gpt-2023.4.21.13.7.20/llm/cachedir/aa8377f2a91b640aa9e08004766e81bb/
+-rw-r--r--   0 betterme   (501) staff       (20)     6330 2023-04-21 04:17:11.000000 llm4gpt-2023.4.21.13.7.20/llm/cachedir/aa8377f2a91b640aa9e08004766e81bb/__output.pkl
+-rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.13.7.20/llm/chatllm.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.936768 llm4gpt-2023.4.21.13.7.20/llm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/llm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/llm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/llm/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.937170 llm4gpt-2023.4.21.13.7.20/llm/docutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      295 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.13.7.20/llm/docutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1390 2023-04-21 04:32:17.000000 llm4gpt-2023.4.21.13.7.20/llm/docutils/doc_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 llm4gpt-2023.4.21.13.7.20/llm/docutils/doc_parse.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.937758 llm4gpt-2023.4.21.13.7.20/llm/kb/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 llm4gpt-2023.4.21.13.7.20/llm/kb/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4gpt-2023.4.21.13.7.20/llm/kb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 llm4gpt-2023.4.21.13.7.20/llm/kb/kbqa.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4gpt-2023.4.21.13.7.20/llm/qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.937989 llm4gpt-2023.4.21.13.7.20/llm/uis/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4gpt-2023.4.21.13.7.20/llm/uis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3138 2023-04-21 04:55:31.000000 llm4gpt-2023.4.21.13.7.20/llm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.938937 llm4gpt-2023.4.21.13.7.20/llm4gpt.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     2120 2023-04-21 05:07:20.000000 llm4gpt-2023.4.21.13.7.20/llm4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1331 2023-04-21 05:07:20.000000 llm4gpt-2023.4.21.13.7.20/llm4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 05:07:20.000000 llm4gpt-2023.4.21.13.7.20/llm4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-21 05:07:20.000000 llm4gpt-2023.4.21.13.7.20/llm4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-21 05:07:20.000000 llm4gpt-2023.4.21.13.7.20/llm4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-21 05:07:20.000000 llm4gpt-2023.4.21.13.7.20/llm4gpt.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-21 05:07:20.000000 llm4gpt-2023.4.21.13.7.20/llm4gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 llm4gpt-2023.4.21.13.7.20/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-21 05:07:20.939783 llm4gpt-2023.4.21.13.7.20/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.21.13.7.20/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-21 05:07:20.939214 llm4gpt-2023.4.21.13.7.20/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.21.13.7.20/tox.ini
```

### Comparing `llm4gpt-2023.4.20.20.13.57/.gitignore` & `llm4gpt-2023.4.21.13.7.20/.gitignore`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/.travis.yml` & `llm4gpt-2023.4.21.13.7.20/.travis.yml`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/CONTRIBUTING.rst` & `llm4gpt-2023.4.21.13.7.20/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/LICENSE` & `llm4gpt-2023.4.21.13.7.20/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/Makefile` & `llm4gpt-2023.4.21.13.7.20/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/PKG-INFO` & `llm4gpt-2023.4.21.13.7.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.20.20.13.57
+Version: 2023.4.21.13.7.20
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.20.20.13.57/README.md` & `llm4gpt-2023.4.21.13.7.20/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/README.rst` & `llm4gpt-2023.4.21.13.7.20/README.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/data/医/500种中药现代研究.txt` & `llm4gpt-2023.4.21.13.7.20/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/data/医/古今医统大全.txt` & `llm4gpt-2023.4.21.13.7.20/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/data/姚明.txt` & `llm4gpt-2023.4.21.13.7.20/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/data/王治郅.txt` & `llm4gpt-2023.4.21.13.7.20/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/data/科比.txt` & `llm4gpt-2023.4.21.13.7.20/data/科比.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/docs/Makefile` & `llm4gpt-2023.4.21.13.7.20/docs/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/docs/README.md` & `llm4gpt-2023.4.21.13.7.20/docs/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/docs/conf.py` & `llm4gpt-2023.4.21.13.7.20/docs/conf.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/docs/img.png` & `llm4gpt-2023.4.21.13.7.20/docs/img.png`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/docs/installation.rst` & `llm4gpt-2023.4.21.13.7.20/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/docs/make.bat` & `llm4gpt-2023.4.21.13.7.20/docs/make.bat`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/llm/chatllm.py` & `llm4gpt-2023.4.21.13.7.20/llm/chatllm.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/llm/clis/cli.py` & `llm4gpt-2023.4.21.13.7.20/llm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/llm/kb/FaissANN.py` & `llm4gpt-2023.4.21.13.7.20/llm/kb/FaissANN.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def __init__(self, folder_path: str = None,
                  index_name: str = "index",
                  model_name_or_path="shibing624/text2vec-base-chinese"):
         self.embeddings = HuggingFaceEmbeddings(model_name=model_name_or_path)
         self.folder_path = folder_path
         self.faiss_ann = self.load_local(folder_path, index_name)  # 加载已存在的索引
 
-    def add_texts(self, texts, metadatas: Optional[List[dict]] = None):
+    def add_texts(self, texts, metadatas: Optional[List[dict]] = None):  # todo: 增加进度条
         self.faiss_ann = FAISS.from_texts(texts, self.embeddings, metadatas)  # metadatas = [{'source': 'xx'}]
 
     def update(self, target: FAISS, index_name=None):
         self.faiss_ann.merge_from(target)  # Add the target FAISS to the current one.
         if index_name:
             logger.info('保存新的索引文件')
             self.faiss_ann.save_local(self.folder_path, index_name)
```

### Comparing `llm4gpt-2023.4.20.20.13.57/llm/qa.py` & `llm4gpt-2023.4.21.13.7.20/llm/qa.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/llm/utils.py` & `llm4gpt-2023.4.21.13.7.20/llm/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 def cuda_empty_cache(device=None):  # todo: 减少清空次数
     if torch.cuda.is_available():
         with torch.cuda.device(device):
             torch.cuda.empty_cache()
             torch.cuda.ipc_collect()
 
 
+@decorator()
+def clear_cuda_cache(device=None, *args, **kwargs):
+    if torch.cuda.is_available():
+        with torch.cuda.device(device):
+            torch.cuda.empty_cache()
+            torch.cuda.ipc_collect()
+
+
 def auto_configure_device_map(num_gpus: int) -> Dict[str, int]:
     # transformer.word_embeddings 占用1层
     # transformer.final_layernorm 和 lm_head 占用1层
     # transformer.layers 占用 28 层
     # 总共30层分配到num_gpus张卡上
     num_trans_layers = 28
     per_gpu_layers = 30 / num_gpus
```

### Comparing `llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/PKG-INFO` & `llm4gpt-2023.4.21.13.7.20/llm4gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.20.20.13.57
+Version: 2023.4.21.13.7.20
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.20.20.13.57/llm4gpt.egg-info/SOURCES.txt` & `llm4gpt-2023.4.21.13.7.20/llm4gpt.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -35,19 +35,30 @@
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 llm/__init__.py
 llm/chatllm.py
 llm/qa.py
 llm/utils.py
+llm/ann/__init__.py
+llm/ann/lite.py
+llm/applications/ChatPDF.py
+llm/applications/Question2Answer.py
+llm/applications/__init__.py
+llm/cachedir/0fad8225447b1d2ff0229997036dfa9c/__output.pkl
+llm/cachedir/aa8377f2a91b640aa9e08004766e81bb/__output.pkl
 llm/clis/README.md
 llm/clis/__init__.py
 llm/clis/cli.py
+llm/docutils/__init__.py
+llm/docutils/doc_embedding.py
+llm/docutils/doc_parse.py
 llm/kb/FaissANN.py
 llm/kb/__init__.py
+llm/kb/kbqa.py
 llm/uis/__init__.py
 llm4gpt.egg-info/PKG-INFO
 llm4gpt.egg-info/SOURCES.txt
 llm4gpt.egg-info/dependency_links.txt
 llm4gpt.egg-info/entry_points.txt
 llm4gpt.egg-info/not-zip-safe
 llm4gpt.egg-info/requires.txt
```

### Comparing `llm4gpt-2023.4.20.20.13.57/setup.py` & `llm4gpt-2023.4.21.13.7.20/setup.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.20.20.13.57/tests/test_llm4gpt.py` & `llm4gpt-2023.4.21.13.7.20/tests/test_llm4gpt.py`

 * *Files identical despite different names*

