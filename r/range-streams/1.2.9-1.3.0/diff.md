# Comparing `tmp/range_streams-1.2.9.tar.gz` & `tmp/range_streams-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/range_streams-1.2.9.tar", last modified: Fri Aug 13 20:22:44 2021, max compression
+gzip compressed data, was "range_streams-1.3.0.tar", last modified: Fri Apr 21 21:11:40 2023, max compression
```

## Comparing `range_streams-1.2.9.tar` & `range_streams-1.3.0.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.111518 range_streams-1.2.9/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.103519 range_streams-1.2.9/.github/
--rw-rw-r--   0 louis     (1000) louis     (1000)     3142 2021-07-05 23:46:16.000000 range_streams-1.2.9/.github/CONTRIBUTING.md
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.107519 range_streams-1.2.9/.github/workflows/
--rw-rw-r--   0 louis     (1000) louis     (1000)     3516 2021-07-26 21:48:49.000000 range_streams-1.2.9/.github/workflows/master.yml
--rw-rw-r--   0 louis     (1000) louis     (1000)      174 2021-07-13 20:38:14.000000 range_streams-1.2.9/.gitignore
--rw-rw-r--   0 louis     (1000) louis     (1000)      592 2021-08-02 14:38:54.000000 range_streams-1.2.9/.pre-commit-config.yaml
--rw-rw-r--   0 louis     (1000) louis     (1000)      326 2021-07-15 08:47:04.000000 range_streams-1.2.9/.readthedocs.yml
--rw-rw-r--   0 louis     (1000) louis     (1000)     1069 2021-07-10 13:40:21.000000 range_streams-1.2.9/LICENSE
--rw-rw-r--   0 louis     (1000) louis     (1000)     2351 2021-08-13 20:22:44.111518 range_streams-1.2.9/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)      996 2021-07-14 12:24:48.000000 range_streams-1.2.9/README.md
--rw-rw-r--   0 louis     (1000) louis     (1000)      175 2021-07-08 22:31:55.000000 range_streams-1.2.9/codecov.yml
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.107519 range_streams-1.2.9/data/
--rw-rw-r--   0 louis     (1000) louis     (1000)      340 2021-07-24 16:56:47.000000 range_streams-1.2.9/data/README.md
--rw-rw-r--   0 louis     (1000) louis     (1000)     8192 2021-07-29 09:22:23.000000 range_streams-1.2.9/data/data.tar
--rw-rw-r--   0 louis     (1000) louis     (1000)     5787 2021-07-29 09:22:36.000000 range_streams-1.2.9/data/data.tar.bz2
--rw-rw-r--   0 louis     (1000) louis     (1000)     5397 2021-07-29 09:22:45.000000 range_streams-1.2.9/data/data.tar.gz
--rw-rw-r--   0 louis     (1000) louis     (1000)       11 2021-07-24 16:05:50.000000 range_streams-1.2.9/data/example_text_file.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)      187 2021-07-24 16:12:38.000000 range_streams-1.2.9/data/example_text_file.txt.zip
--rw-rw-r--   0 louis     (1000) louis     (1000)     1310 2021-07-26 22:31:17.000000 range_streams-1.2.9/data/one_red_pixel.png
--rw-rw-r--   0 louis     (1000) louis     (1000)     1329 2021-07-26 22:47:39.000000 range_streams-1.2.9/data/one_semitransparent_pixel.png
--rw-rw-r--   0 louis     (1000) louis     (1000)     1318 2021-07-26 22:32:04.000000 range_streams-1.2.9/data/one_transparent_pixel.png
--rw-rw-r--   0 louis     (1000) louis     (1000)      276 2021-07-24 16:17:16.000000 range_streams-1.2.9/data/red_square.png
--rw-rw-r--   0 louis     (1000) louis     (1000)     5124 2021-07-26 23:02:23.000000 range_streams-1.2.9/data/red_square_rgba_semitransparent.png
--rw-rw-r--   0 louis     (1000) louis     (1000)    83498 2021-06-24 17:02:19.000000 range_streams-1.2.9/data/tqdm-4.61.1-pyhd3eb1b0_1.conda
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.107519 range_streams-1.2.9/docs/
--rw-rw-r--   0 louis     (1000) louis     (1000)      634 2021-07-14 19:39:18.000000 range_streams-1.2.9/docs/Makefile
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.103519 range_streams-1.2.9/docs/_static/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.107519 range_streams-1.2.9/docs/_static/css/
--rw-rw-r--   0 louis     (1000) louis     (1000)       70 2021-07-15 12:38:09.000000 range_streams-1.2.9/docs/_static/css/style.css
--rw-rw-r--   0 louis     (1000) louis     (1000)     2525 2021-08-11 17:55:11.000000 range_streams-1.2.9/docs/api.rst
--rw-rw-r--   0 louis     (1000) louis     (1000)     3785 2021-07-17 21:00:55.000000 range_streams-1.2.9/docs/conf.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     8800 2021-07-13 23:35:46.000000 range_streams-1.2.9/docs/design.rst
--rw-rw-r--   0 louis     (1000) louis     (1000)      566 2021-07-14 16:08:35.000000 range_streams-1.2.9/docs/index.rst
--rw-rw-r--   0 louis     (1000) louis     (1000)      795 2021-07-13 20:11:42.000000 range_streams-1.2.9/docs/make.bat
--rw-rw-r--   0 louis     (1000) louis     (1000)     4906 2021-07-13 23:35:34.000000 range_streams-1.2.9/docs/motivation.rst
--rw-rw-r--   0 louis     (1000) louis     (1000)     2700 2021-08-12 20:18:12.000000 range_streams-1.2.9/docs/overview.rst
--rw-rw-r--   0 louis     (1000) louis     (1000)      354 2021-07-07 17:18:42.000000 range_streams-1.2.9/mypy.ini
--rw-r--r--   0 louis     (1000) louis     (1000)      361 2021-07-08 22:30:19.000000 range_streams-1.2.9/pyproject.toml
--rw-rw-r--   0 louis     (1000) louis     (1000)       42 2021-08-11 14:07:25.000000 range_streams-1.2.9/requirements.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       38 2021-08-13 20:22:44.111518 range_streams-1.2.9/setup.cfg
--rw-rw-r--   0 louis     (1000) louis     (1000)     3248 2021-07-28 19:11:23.000000 range_streams-1.2.9/setup.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.103519 range_streams-1.2.9/src/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.107519 range_streams-1.2.9/src/range_streams/
--rw-rw-r--   0 louis     (1000) louis     (1000)     8541 2021-08-12 20:18:59.000000 range_streams-1.2.9/src/range_streams/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     9039 2021-08-13 20:20:42.000000 range_streams-1.2.9/src/range_streams/async_utils.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.107519 range_streams-1.2.9/src/range_streams/codecs/
--rw-rw-r--   0 louis     (1000) louis     (1000)      562 2021-07-29 11:04:48.000000 range_streams-1.2.9/src/range_streams/codecs/__init__.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.107519 range_streams-1.2.9/src/range_streams/codecs/conda/
--rw-rw-r--   0 louis     (1000) louis     (1000)       59 2021-07-29 13:24:10.000000 range_streams-1.2.9/src/range_streams/codecs/conda/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     4602 2021-08-13 15:36:15.000000 range_streams-1.2.9/src/range_streams/codecs/conda/stream.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.107519 range_streams-1.2.9/src/range_streams/codecs/png/
--rw-rw-r--   0 louis     (1000) louis     (1000)       55 2021-07-26 12:04:00.000000 range_streams-1.2.9/src/range_streams/codecs/png/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     4491 2021-07-28 18:35:47.000000 range_streams-1.2.9/src/range_streams/codecs/png/data.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     2831 2021-07-27 13:48:41.000000 range_streams-1.2.9/src/range_streams/codecs/png/reconstruct.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    17666 2021-08-13 15:36:58.000000 range_streams-1.2.9/src/range_streams/codecs/png/stream.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.111518 range_streams-1.2.9/src/range_streams/codecs/share/
--rw-rw-r--   0 louis     (1000) louis     (1000)       59 2021-07-29 09:44:51.000000 range_streams-1.2.9/src/range_streams/codecs/share/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      271 2021-07-29 09:45:04.000000 range_streams-1.2.9/src/range_streams/codecs/share/data.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.111518 range_streams-1.2.9/src/range_streams/codecs/tar/
--rw-rw-r--   0 louis     (1000) louis     (1000)       55 2021-07-29 09:48:24.000000 range_streams-1.2.9/src/range_streams/codecs/tar/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     1831 2021-07-29 12:16:00.000000 range_streams-1.2.9/src/range_streams/codecs/tar/data.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    10997 2021-08-13 15:37:21.000000 range_streams-1.2.9/src/range_streams/codecs/tar/stream.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.111518 range_streams-1.2.9/src/range_streams/codecs/zip/
--rw-rw-r--   0 louis     (1000) louis     (1000)       55 2021-07-24 19:54:53.000000 range_streams-1.2.9/src/range_streams/codecs/zip/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     2709 2021-07-29 09:45:43.000000 range_streams-1.2.9/src/range_streams/codecs/zip/data.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    20428 2021-08-13 15:37:43.000000 range_streams-1.2.9/src/range_streams/codecs/zip/stream.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.111518 range_streams-1.2.9/src/range_streams/codecs/zstd/
--rw-rw-r--   0 louis     (1000) louis     (1000)       72 2021-07-26 11:48:34.000000 range_streams-1.2.9/src/range_streams/codecs/zstd/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     1109 2021-07-27 13:26:38.000000 range_streams-1.2.9/src/range_streams/codecs/zstd/tar.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     3612 2021-08-03 21:58:41.000000 range_streams-1.2.9/src/range_streams/http_utils.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      582 2021-08-11 13:03:42.000000 range_streams-1.2.9/src/range_streams/log_utils.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     2215 2021-08-12 19:46:07.000000 range_streams-1.2.9/src/range_streams/overlaps.py
--rw-rw-r--   0 louis     (1000) louis     (1000)        0 2021-07-05 19:24:20.000000 range_streams-1.2.9/src/range_streams/py.typed
--rw-rw-r--   0 louis     (1000) louis     (1000)     6333 2021-08-04 13:58:30.000000 range_streams-1.2.9/src/range_streams/range_utils.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    12954 2021-08-12 20:29:08.000000 range_streams-1.2.9/src/range_streams/request.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    21406 2021-08-13 11:59:06.000000 range_streams-1.2.9/src/range_streams/response.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    42183 2021-08-13 14:18:23.000000 range_streams-1.2.9/src/range_streams/stream.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      198 2021-08-12 08:43:40.000000 range_streams-1.2.9/src/range_streams/types.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.107519 range_streams-1.2.9/src/range_streams.egg-info/
--rw-rw-r--   0 louis     (1000) louis     (1000)     2351 2021-08-13 20:22:44.000000 range_streams-1.2.9/src/range_streams.egg-info/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)     2370 2021-08-13 20:22:44.000000 range_streams-1.2.9/src/range_streams.egg-info/SOURCES.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2021-08-13 20:22:44.000000 range_streams-1.2.9/src/range_streams.egg-info/dependency_links.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2021-07-13 16:17:39.000000 range_streams-1.2.9/src/range_streams.egg-info/not-zip-safe
--rw-rw-r--   0 louis     (1000) louis     (1000)      235 2021-08-13 20:22:44.000000 range_streams-1.2.9/src/range_streams.egg-info/requires.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       14 2021-08-13 20:22:44.000000 range_streams-1.2.9/src/range_streams.egg-info/top_level.txt
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.111518 range_streams-1.2.9/tests/
--rw-rw-r--   0 louis     (1000) louis     (1000)        0 2021-07-07 15:46:39.000000 range_streams-1.2.9/tests/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     5503 2021-08-12 22:46:18.000000 range_streams-1.2.9/tests/async_test.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.111518 range_streams-1.2.9/tests/codecs/
--rw-rw-r--   0 louis     (1000) louis     (1000)        0 2021-07-24 17:11:48.000000 range_streams-1.2.9/tests/codecs/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     5874 2021-07-26 20:26:29.000000 range_streams-1.2.9/tests/codecs/conda_test.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      747 2021-07-31 21:15:39.000000 range_streams-1.2.9/tests/codecs/data.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     3004 2021-08-02 21:53:44.000000 range_streams-1.2.9/tests/codecs/png_test.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     1605 2021-07-29 12:46:14.000000 range_streams-1.2.9/tests/codecs/tar_test.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     2259 2021-07-27 13:52:53.000000 range_streams-1.2.9/tests/codecs/zip_test.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      244 2021-08-12 20:29:07.000000 range_streams-1.2.9/tests/data.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      756 2021-08-03 21:31:58.000000 range_streams-1.2.9/tests/http_utils_test.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    11163 2021-08-04 15:27:56.000000 range_streams-1.2.9/tests/overlaps_test.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     6726 2021-08-12 20:19:24.000000 range_streams-1.2.9/tests/range_stream_core_test.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    13014 2021-08-02 14:04:07.000000 range_streams-1.2.9/tests/range_stream_edge_case_test.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     7546 2021-08-04 15:52:25.000000 range_streams-1.2.9/tests/range_stream_mono_test.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     4148 2021-07-26 21:03:48.000000 range_streams-1.2.9/tests/range_utils_test.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     1641 2021-08-03 21:58:41.000000 range_streams-1.2.9/tests/request_test.py
--rw-rw-r--   0 louis     (1000) louis     (1000)     3680 2021-08-12 20:28:14.000000 range_streams-1.2.9/tests/response_test.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      222 2021-08-02 14:37:53.000000 range_streams-1.2.9/tests/share.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.103519 range_streams-1.2.9/tools/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2021-08-13 20:22:44.111518 range_streams-1.2.9/tools/github/
--rw-rw-r--   0 louis     (1000) louis     (1000)      353 2021-07-07 14:16:47.000000 range_streams-1.2.9/tools/github/install_miniconda.sh
--rw-rw-r--   0 louis     (1000) louis     (1000)     1150 2021-07-26 21:39:19.000000 range_streams-1.2.9/tox.ini
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.475777 range_streams-1.3.0/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.467777 range_streams-1.3.0/.github/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3142 2021-07-05 23:46:16.000000 range_streams-1.3.0/.github/CONTRIBUTING.md
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.467777 range_streams-1.3.0/.github/workflows/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3516 2021-07-26 21:48:49.000000 range_streams-1.3.0/.github/workflows/master.yml
+-rw-rw-r--   0 louis     (1000) louis     (1000)      174 2021-07-13 20:38:14.000000 range_streams-1.3.0/.gitignore
+-rw-rw-r--   0 louis     (1000) louis     (1000)      592 2023-04-21 21:05:59.000000 range_streams-1.3.0/.pre-commit-config.yaml
+-rw-rw-r--   0 louis     (1000) louis     (1000)      326 2021-07-15 08:47:04.000000 range_streams-1.3.0/.readthedocs.yml
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1069 2021-07-10 13:40:21.000000 range_streams-1.3.0/LICENSE
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2150 2023-04-21 21:11:40.475777 range_streams-1.3.0/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)      996 2021-07-14 12:24:48.000000 range_streams-1.3.0/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)      175 2021-07-08 22:31:55.000000 range_streams-1.3.0/codecov.yml
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.467777 range_streams-1.3.0/data/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      340 2021-07-24 16:56:47.000000 range_streams-1.3.0/data/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)     8192 2021-07-29 09:22:23.000000 range_streams-1.3.0/data/data.tar
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5787 2021-07-29 09:22:36.000000 range_streams-1.3.0/data/data.tar.bz2
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5397 2021-07-29 09:22:45.000000 range_streams-1.3.0/data/data.tar.gz
+-rw-rw-r--   0 louis     (1000) louis     (1000)       11 2021-07-24 16:05:50.000000 range_streams-1.3.0/data/example_text_file.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)      187 2021-07-24 16:12:38.000000 range_streams-1.3.0/data/example_text_file.txt.zip
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1310 2021-07-26 22:31:17.000000 range_streams-1.3.0/data/one_red_pixel.png
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1329 2021-07-26 22:47:39.000000 range_streams-1.3.0/data/one_semitransparent_pixel.png
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1318 2021-07-26 22:32:04.000000 range_streams-1.3.0/data/one_transparent_pixel.png
+-rw-rw-r--   0 louis     (1000) louis     (1000)      276 2021-07-24 16:17:16.000000 range_streams-1.3.0/data/red_square.png
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5124 2021-07-26 23:02:23.000000 range_streams-1.3.0/data/red_square_rgba_semitransparent.png
+-rw-rw-r--   0 louis     (1000) louis     (1000)    83498 2021-06-24 17:02:19.000000 range_streams-1.3.0/data/tqdm-4.61.1-pyhd3eb1b0_1.conda
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.467777 range_streams-1.3.0/docs/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      634 2021-07-14 19:39:18.000000 range_streams-1.3.0/docs/Makefile
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.463777 range_streams-1.3.0/docs/_static/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.467777 range_streams-1.3.0/docs/_static/css/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       70 2021-07-15 12:38:09.000000 range_streams-1.3.0/docs/_static/css/style.css
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2525 2021-08-11 17:55:11.000000 range_streams-1.3.0/docs/api.rst
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3785 2021-07-17 21:00:55.000000 range_streams-1.3.0/docs/conf.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     8800 2021-07-13 23:35:46.000000 range_streams-1.3.0/docs/design.rst
+-rw-rw-r--   0 louis     (1000) louis     (1000)      566 2021-07-14 16:08:35.000000 range_streams-1.3.0/docs/index.rst
+-rw-rw-r--   0 louis     (1000) louis     (1000)      795 2021-07-13 20:11:42.000000 range_streams-1.3.0/docs/make.bat
+-rw-rw-r--   0 louis     (1000) louis     (1000)     4906 2021-07-13 23:35:34.000000 range_streams-1.3.0/docs/motivation.rst
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2700 2021-08-12 20:18:12.000000 range_streams-1.3.0/docs/overview.rst
+-rw-rw-r--   0 louis     (1000) louis     (1000)      354 2021-07-07 17:18:42.000000 range_streams-1.3.0/mypy.ini
+-rw-r--r--   0 louis     (1000) louis     (1000)      361 2021-07-08 22:30:19.000000 range_streams-1.3.0/pyproject.toml
+-rw-rw-r--   0 louis     (1000) louis     (1000)       42 2023-04-21 21:08:10.000000 range_streams-1.3.0/requirements.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       38 2023-04-21 21:11:40.475777 range_streams-1.3.0/setup.cfg
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3248 2021-07-28 19:11:23.000000 range_streams-1.3.0/setup.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.463777 range_streams-1.3.0/src/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.471777 range_streams-1.3.0/src/range_streams/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     8541 2021-08-12 20:18:59.000000 range_streams-1.3.0/src/range_streams/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    11173 2023-04-21 21:08:10.000000 range_streams-1.3.0/src/range_streams/async_utils.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.471777 range_streams-1.3.0/src/range_streams/codecs/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      562 2021-07-29 11:04:48.000000 range_streams-1.3.0/src/range_streams/codecs/__init__.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.471777 range_streams-1.3.0/src/range_streams/codecs/conda/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       59 2021-07-29 13:24:10.000000 range_streams-1.3.0/src/range_streams/codecs/conda/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     4602 2021-08-13 15:36:15.000000 range_streams-1.3.0/src/range_streams/codecs/conda/stream.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.471777 range_streams-1.3.0/src/range_streams/codecs/png/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       55 2021-07-26 12:04:00.000000 range_streams-1.3.0/src/range_streams/codecs/png/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     4491 2021-07-28 18:35:47.000000 range_streams-1.3.0/src/range_streams/codecs/png/data.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2831 2021-07-27 13:48:41.000000 range_streams-1.3.0/src/range_streams/codecs/png/reconstruct.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    17666 2021-08-13 15:36:58.000000 range_streams-1.3.0/src/range_streams/codecs/png/stream.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.471777 range_streams-1.3.0/src/range_streams/codecs/share/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       59 2021-07-29 09:44:51.000000 range_streams-1.3.0/src/range_streams/codecs/share/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      271 2021-07-29 09:45:04.000000 range_streams-1.3.0/src/range_streams/codecs/share/data.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.471777 range_streams-1.3.0/src/range_streams/codecs/tar/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       55 2021-07-29 09:48:24.000000 range_streams-1.3.0/src/range_streams/codecs/tar/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1831 2021-07-29 12:16:00.000000 range_streams-1.3.0/src/range_streams/codecs/tar/data.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    11127 2023-04-21 20:55:08.000000 range_streams-1.3.0/src/range_streams/codecs/tar/stream.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.471777 range_streams-1.3.0/src/range_streams/codecs/zip/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       55 2021-07-24 19:54:53.000000 range_streams-1.3.0/src/range_streams/codecs/zip/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2709 2021-07-29 09:45:43.000000 range_streams-1.3.0/src/range_streams/codecs/zip/data.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    20428 2021-08-13 15:37:43.000000 range_streams-1.3.0/src/range_streams/codecs/zip/stream.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.471777 range_streams-1.3.0/src/range_streams/codecs/zstd/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       72 2021-07-26 11:48:34.000000 range_streams-1.3.0/src/range_streams/codecs/zstd/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1109 2021-07-27 13:26:38.000000 range_streams-1.3.0/src/range_streams/codecs/zstd/tar.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3612 2021-08-03 21:58:41.000000 range_streams-1.3.0/src/range_streams/http_utils.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      582 2021-08-11 13:03:42.000000 range_streams-1.3.0/src/range_streams/log_utils.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2215 2023-04-21 21:08:10.000000 range_streams-1.3.0/src/range_streams/overlaps.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)        0 2021-07-05 19:24:20.000000 range_streams-1.3.0/src/range_streams/py.typed
+-rw-rw-r--   0 louis     (1000) louis     (1000)     6333 2021-08-04 13:58:30.000000 range_streams-1.3.0/src/range_streams/range_utils.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    12954 2021-08-12 20:29:08.000000 range_streams-1.3.0/src/range_streams/request.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    21406 2021-08-13 11:59:06.000000 range_streams-1.3.0/src/range_streams/response.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    42258 2021-08-13 22:20:16.000000 range_streams-1.3.0/src/range_streams/stream.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      198 2021-08-12 08:43:40.000000 range_streams-1.3.0/src/range_streams/types.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.471777 range_streams-1.3.0/src/range_streams.egg-info/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2150 2023-04-21 21:11:40.000000 range_streams-1.3.0/src/range_streams.egg-info/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2370 2023-04-21 21:11:40.000000 range_streams-1.3.0/src/range_streams.egg-info/SOURCES.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-04-21 21:11:40.000000 range_streams-1.3.0/src/range_streams.egg-info/dependency_links.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-04-21 21:11:40.000000 range_streams-1.3.0/src/range_streams.egg-info/not-zip-safe
+-rw-rw-r--   0 louis     (1000) louis     (1000)      235 2023-04-21 21:11:40.000000 range_streams-1.3.0/src/range_streams.egg-info/requires.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       14 2023-04-21 21:11:40.000000 range_streams-1.3.0/src/range_streams.egg-info/top_level.txt
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.475777 range_streams-1.3.0/tests/
+-rw-rw-r--   0 louis     (1000) louis     (1000)        0 2021-07-07 15:46:39.000000 range_streams-1.3.0/tests/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5503 2021-08-12 22:46:18.000000 range_streams-1.3.0/tests/async_test.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.475777 range_streams-1.3.0/tests/codecs/
+-rw-rw-r--   0 louis     (1000) louis     (1000)        0 2021-07-24 17:11:48.000000 range_streams-1.3.0/tests/codecs/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     5874 2021-07-26 20:26:29.000000 range_streams-1.3.0/tests/codecs/conda_test.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      747 2021-07-31 21:15:39.000000 range_streams-1.3.0/tests/codecs/data.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3004 2021-08-02 21:53:44.000000 range_streams-1.3.0/tests/codecs/png_test.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1605 2021-07-29 12:46:14.000000 range_streams-1.3.0/tests/codecs/tar_test.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2259 2021-07-27 13:52:53.000000 range_streams-1.3.0/tests/codecs/zip_test.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      244 2021-08-12 20:29:07.000000 range_streams-1.3.0/tests/data.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      756 2021-08-03 21:31:58.000000 range_streams-1.3.0/tests/http_utils_test.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    11163 2021-08-04 15:27:56.000000 range_streams-1.3.0/tests/overlaps_test.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     6726 2021-08-12 20:19:24.000000 range_streams-1.3.0/tests/range_stream_core_test.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    13014 2021-08-02 14:04:07.000000 range_streams-1.3.0/tests/range_stream_edge_case_test.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     7546 2021-08-04 15:52:25.000000 range_streams-1.3.0/tests/range_stream_mono_test.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     4148 2021-07-26 21:03:48.000000 range_streams-1.3.0/tests/range_utils_test.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1641 2021-08-03 21:58:41.000000 range_streams-1.3.0/tests/request_test.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3680 2021-08-12 20:28:14.000000 range_streams-1.3.0/tests/response_test.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      222 2021-08-02 14:37:53.000000 range_streams-1.3.0/tests/share.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.463777 range_streams-1.3.0/tools/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 21:11:40.475777 range_streams-1.3.0/tools/github/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      353 2021-07-07 14:16:47.000000 range_streams-1.3.0/tools/github/install_miniconda.sh
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1150 2021-07-26 21:39:19.000000 range_streams-1.3.0/tox.ini
```

### Comparing `range_streams-1.2.9/.github/CONTRIBUTING.md` & `range_streams-1.3.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/.github/workflows/master.yml` & `range_streams-1.3.0/.github/workflows/master.yml`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/.pre-commit-config.yaml` & `range_streams-1.3.0/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 repos:
   - repo: https://github.com/psf/black
-    rev: 21.6b0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3.8
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.9.2
     hooks:
```

### Comparing `range_streams-1.2.9/LICENSE` & `range_streams-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/PKG-INFO` & `range_streams-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,20 @@
 Metadata-Version: 2.1
 Name: range_streams
-Version: 1.2.9
+Version: 1.3.0
 Summary: Streaming via range requests.
 Home-page: https://github.com/lmmx/range-streams
 Author: Louis Maddox
 Author-email: louismmx@gmail.com
 Maintainer: Louis Maddox
 Maintainer-email: louismmx@gmail.com
 License: MIT
 Project-URL: Documentation, https://range-streams.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/lmmx/range-streams/issues
 Project-URL: Source Code, https://github.com/lmmx/range-streams
-Description: # range-streams
-        
-        [![Documentation](https://readthedocs.org/projects/range-streams/badge/?version=latest)](https://range-streams.readthedocs.io/en/latest/)
-        [![CI Status](https://github.com/lmmx/range-streams/actions/workflows/master.yml/badge.svg)](https://github.com/lmmx/range-streams/actions/workflows/master.yml)
-        [![Coverage](https://codecov.io/gh/lmmx/range-streams/branch/master/graph/badge.svg)](https://codecov.io/github/lmmx/range-streams)
-        [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        Streaming via range requests in Python
-        
-        [Read The Docs](https://range-streams.readthedocs.io/en/latest/)
-        
-        ## Requires
-        
-        - Python 3.8+
-        
-        ## Installation
-        
-        ```sh
-        pip install range-streams
-        ```
-        
-        > _range-streams_ is available from [PyPI](https://pypi.org/project/range-streams), and
-        > the code is on [GitHub](https://github.com/lmmx/range-streams)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -49,7 +23,33 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: dev
+License-File: LICENSE
+
+# range-streams
+
+[![Documentation](https://readthedocs.org/projects/range-streams/badge/?version=latest)](https://range-streams.readthedocs.io/en/latest/)
+[![CI Status](https://github.com/lmmx/range-streams/actions/workflows/master.yml/badge.svg)](https://github.com/lmmx/range-streams/actions/workflows/master.yml)
+[![Coverage](https://codecov.io/gh/lmmx/range-streams/branch/master/graph/badge.svg)](https://codecov.io/github/lmmx/range-streams)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+Streaming via range requests in Python
+
+[Read The Docs](https://range-streams.readthedocs.io/en/latest/)
+
+## Requires
+
+- Python 3.8+
+
+## Installation
+
+```sh
+pip install range-streams
+```
+
+> _range-streams_ is available from [PyPI](https://pypi.org/project/range-streams), and
+> the code is on [GitHub](https://github.com/lmmx/range-streams)
```

### Comparing `range_streams-1.2.9/README.md` & `range_streams-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/data/data.tar` & `range_streams-1.3.0/data/data.tar`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/data/data.tar.bz2` & `range_streams-1.3.0/data/data.tar.bz2`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/data/data.tar.gz` & `range_streams-1.3.0/data/data.tar.gz`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/data/one_red_pixel.png` & `range_streams-1.3.0/data/one_red_pixel.png`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/data/one_semitransparent_pixel.png` & `range_streams-1.3.0/data/one_semitransparent_pixel.png`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/data/one_transparent_pixel.png` & `range_streams-1.3.0/data/one_transparent_pixel.png`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/data/red_square_rgba_semitransparent.png` & `range_streams-1.3.0/data/red_square_rgba_semitransparent.png`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/data/tqdm-4.61.1-pyhd3eb1b0_1.conda` & `range_streams-1.3.0/data/tqdm-4.61.1-pyhd3eb1b0_1.conda`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/docs/Makefile` & `range_streams-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/docs/api.rst` & `range_streams-1.3.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/docs/conf.py` & `range_streams-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/docs/design.rst` & `range_streams-1.3.0/docs/design.rst`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/docs/index.rst` & `range_streams-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/docs/make.bat` & `range_streams-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/docs/motivation.rst` & `range_streams-1.3.0/docs/motivation.rst`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/docs/overview.rst` & `range_streams-1.3.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/setup.py` & `range_streams-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/__init__.py` & `range_streams-1.3.0/src/range_streams/__init__.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/async_utils.py` & `range_streams-1.3.0/src/range_streams/async_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from asyncio.events import AbstractEventLoop
 from functools import partial
 from signal import SIGINT, SIGTERM, Signals
 from sys import stderr
 from typing import TYPE_CHECKING, Callable, Coroutine, Iterator, Type
 
 from aiostream import stream
+from aiostream.core import StreamEmpty
 from ranges import Range, RangeSet
 
 MYPY = False  # when using mypy will be overrided as True
 if MYPY or not TYPE_CHECKING:  # pragma: no cover
     import httpx  # avoid importing to Sphinx type checker
 
 import tqdm
@@ -30,23 +31,40 @@
         stream_cls: Type[RangeStreamOrSubclass],
         urls: list[str],
         callback: Callable | None = None,
         verbose: bool = False,
         show_progress_bar: bool = True,
         timeout_s: float = 5.0,
         client=None,
+        close_client: bool = False,
         **kwargs,
     ):
         """
         Any kwargs are passed through to the stream class constructor.
 
         Args:
-          callback : A function to be passed 3 values: the AsyncFetcher which is calling
-                     it, the awaited RangeStream, and its source URL (a ``httpx.URL``,
-                     which can be coerced to a string).
+          stream_cls        : The :class:`~range_streams.stream.RangeStream` class or a
+                              subclass (i.e. one of its codecs or a custom subclass)
+                              to instantiate for each of the URLs. Note: these classes
+                              also have a helper method
+                              :meth:`~range_streams.stream.RangeStream.make_async_fetcher`
+          urls              : The list of URLs to fetch until completion
+          callback          : A function to be passed 3 values: the AsyncFetcher which
+                              is calling it, the awaited RangeStream, and its source URL
+                              (a ``httpx.URL``, which can be coerced to a string).
+          verbose           : Whether to log to console
+          show_progress_bar : Whether to show a tqdm progress bar (async-compatible)
+          timeout_s         : The timeout to set on the client (converted into
+                              ``httpx.Timeout`` configuration on instantiation)
+          client            : The client to pass, if any, or one will be instantiated
+                              and closed on each usage (note: not each instantiation!)
+          close_client      : Whether to close the client upon completion (only if
+                              provided: if no client is provided, one will be created
+                              and closed by the standard `async with httpx.AsyncClient`
+                              contextmanager block).
         """
         if urls == []:
             raise ValueError("The list of URLs to fetch cannot be empty")
         self.stream_cls = stream_cls
         self.stream_cls_kwargs = kwargs
         self.url_list = urls
         self.callback = callback
@@ -55,34 +73,43 @@
         if n_urls != n_unique_urls:
             msg = f"List of URLs is not unique (only {n_unique_urls} of {n_urls})"
             raise ValueError(msg)
         self.n = n_urls
         self.verbose = verbose
         self.show_progress_bar = show_progress_bar and not self.verbose
         self.client = client
+        self.close_client_on_completion = close_client
         self.timeout = httpx.Timeout(timeout=timeout_s)
         self.completed = RangeSet()
         set_up_logging(quiet=not verbose)
 
     def make_calls(self):
         """
         The method called to run the event loop to fetch URLs, after initialisation
         and/or repeatedly upon exitting the loop (i.e. it can recover from errors).
         """
         urlset = (u for u in self.filtered_url_list)  # single use URL generator
         if self.show_progress_bar:
             self.set_up_progress_bar()
-        self.fetch_things(urls=urlset)
+        try:
+            self.fetch_things(urls=urlset)
+        except StreamEmpty as exc:
+            # Treat this like a StopIteration (was called despite completed URLs)
+            if self.close_client_on_completion:
+                asyncio.run(self.client.aclose())
+            else:
+                raise
+            # Note: to avoid throwing exception, check `total_complete` before calling
         if self.show_progress_bar:
             self.pbar.close()
 
     async def process_stream(self, range_stream: RangeStreamOrSubclass):
         """
         Process an awaited RangeStream within an async fetch loop, calling the callback
-        set on the `~range_streams.async_utils.AsyncFetcher.callback` attribute.
+        set on the :attr:`~range_streams.async_utils.AsyncFetcher.callback` attribute.
 
         Args:
           range_stream : The awaited RangeStream (or one of its subclasses)
         """
         monostream_response = range_stream._ranges[range_stream.total_range]
         resp = monostream_response.request.response  # httpx.Response
         source_url = resp.history[0].url if resp.history else resp.url
@@ -90,16 +117,20 @@
         i = next(i for (i, u) in enumerate(self.url_list) if source_url == u)
         if self.callback is not None:
             await self.callback(self, range_stream, source_url)
         if self.verbose:
             log.debug(f"Processed URL in async callback: {source_url}")
         if self.show_progress_bar:
             self.pbar.update()
-        self.complete_row(row_index=i)
+        if i not in self.completed:
+            # Don't bother putting in if already been marked as complete in the callback
+            self.complete_row(row_index=i)
         await resp.aclose()
+        if self.total_complete == self.n and self.close_client_on_completion:
+            await self.client.aclose()
 
     @property
     def total_complete(self) -> int:
         return sum([r.length() for r in self.completed.ranges()])
 
     def mark_url_complete(self, url: str) -> None:
         """
@@ -170,14 +201,17 @@
         urls: Iterator[str],
     ) -> Coroutine:
         """
         If the :attr:`~range_streams.async_utils.AsyncFetcher.client` is ``None``, create one
         in a contextmanager block (i.e. close it immediately after use), otherwise use
         the one provided, not in a contextmanager block (i.e. leave it up to the user to
         close the client).
+
+        Args:
+          urls         : The URLs to fetch, as an exhaustible iterator (not a Sequence)
         """
         await self.set_async_signal_handlers()
         if self.client is None:
             async with httpx.AsyncClient() as client:
                 processed = await self.fetch_and_process(urls=urls, client=client)
         else:
             if self.client.is_closed:
```

### Comparing `range_streams-1.2.9/src/range_streams/codecs/__init__.py` & `range_streams-1.3.0/src/range_streams/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/codecs/conda/stream.py` & `range_streams-1.3.0/src/range_streams/codecs/conda/stream.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/codecs/png/data.py` & `range_streams-1.3.0/src/range_streams/codecs/png/data.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/codecs/png/reconstruct.py` & `range_streams-1.3.0/src/range_streams/codecs/png/reconstruct.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/codecs/png/stream.py` & `range_streams-1.3.0/src/range_streams/codecs/png/stream.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/codecs/tar/data.py` & `range_streams-1.3.0/src/range_streams/codecs/tar/data.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/codecs/tar/stream.py` & `range_streams-1.3.0/src/range_streams/codecs/tar/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,18 @@
         file_size_rng_end = file_size_rng_start + self.data.HEADER._H_FILE_SIZE_SIZE
         file_size_rng = Range(file_size_rng_start, file_size_rng_end)
         if self.client_is_async:
             self.add_async(file_size_rng)
         else:
             self.add(file_size_rng)
         file_size_b = self.active_range_response.read()
-        file_size = int(file_size_b, 8)  # convert octal number from bitstring
+        try:
+            file_size = int(file_size_b, 8)  # convert octal number from bitstring
+        except ValueError:
+            file_size = int(file_size_b.rstrip(b"\x00"), 8)  # may be null-terminated
         return file_size
 
     def add_file_ranges(self):
         for tf_info in self.tarred_files:
             assert tf_info.filename is not None
             if self.client_is_async:
                 self.add_async(tf_info.file_range, name=tf_info.filename)
```

### Comparing `range_streams-1.2.9/src/range_streams/codecs/zip/data.py` & `range_streams-1.3.0/src/range_streams/codecs/zip/data.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/codecs/zip/stream.py` & `range_streams-1.3.0/src/range_streams/codecs/zip/stream.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/codecs/zstd/tar.py` & `range_streams-1.3.0/src/range_streams/codecs/zstd/tar.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/http_utils.py` & `range_streams-1.3.0/src/range_streams/http_utils.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/log_utils.py` & `range_streams-1.3.0/src/range_streams/log_utils.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/overlaps.py` & `range_streams-1.3.0/src/range_streams/overlaps.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/range_utils.py` & `range_streams-1.3.0/src/range_streams/range_utils.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/request.py` & `range_streams-1.3.0/src/range_streams/request.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/response.py` & `range_streams-1.3.0/src/range_streams/response.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/src/range_streams/stream.py` & `range_streams-1.3.0/src/range_streams/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -894,19 +894,21 @@
         cls,
         urls: list[str],
         callback: Callable | None = None,
         verbose: bool = False,
         show_progress_bar: bool = True,
         timeout_s: float = 5.0,
         client=None,
+        close_client: bool = False,
         **kwargs,
     ):
         return AsyncFetcher(
             stream_cls=cls,
             urls=urls,
             callback=callback,
             verbose=verbose,
             show_progress_bar=show_progress_bar,
             timeout_s=timeout_s,
             client=client,
+            close_client=close_client,
             **kwargs,  # Any other kwargs can be passed through to RangeStream subclass
         )
```

### Comparing `range_streams-1.2.9/src/range_streams.egg-info/PKG-INFO` & `range_streams-1.3.0/src/range_streams.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,20 @@
 Metadata-Version: 2.1
 Name: range-streams
-Version: 1.2.9
+Version: 1.3.0
 Summary: Streaming via range requests.
 Home-page: https://github.com/lmmx/range-streams
 Author: Louis Maddox
 Author-email: louismmx@gmail.com
 Maintainer: Louis Maddox
 Maintainer-email: louismmx@gmail.com
 License: MIT
 Project-URL: Documentation, https://range-streams.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/lmmx/range-streams/issues
 Project-URL: Source Code, https://github.com/lmmx/range-streams
-Description: # range-streams
-        
-        [![Documentation](https://readthedocs.org/projects/range-streams/badge/?version=latest)](https://range-streams.readthedocs.io/en/latest/)
-        [![CI Status](https://github.com/lmmx/range-streams/actions/workflows/master.yml/badge.svg)](https://github.com/lmmx/range-streams/actions/workflows/master.yml)
-        [![Coverage](https://codecov.io/gh/lmmx/range-streams/branch/master/graph/badge.svg)](https://codecov.io/github/lmmx/range-streams)
-        [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        Streaming via range requests in Python
-        
-        [Read The Docs](https://range-streams.readthedocs.io/en/latest/)
-        
-        ## Requires
-        
-        - Python 3.8+
-        
-        ## Installation
-        
-        ```sh
-        pip install range-streams
-        ```
-        
-        > _range-streams_ is available from [PyPI](https://pypi.org/project/range-streams), and
-        > the code is on [GitHub](https://github.com/lmmx/range-streams)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -49,7 +23,33 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: dev
+License-File: LICENSE
+
+# range-streams
+
+[![Documentation](https://readthedocs.org/projects/range-streams/badge/?version=latest)](https://range-streams.readthedocs.io/en/latest/)
+[![CI Status](https://github.com/lmmx/range-streams/actions/workflows/master.yml/badge.svg)](https://github.com/lmmx/range-streams/actions/workflows/master.yml)
+[![Coverage](https://codecov.io/gh/lmmx/range-streams/branch/master/graph/badge.svg)](https://codecov.io/github/lmmx/range-streams)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+Streaming via range requests in Python
+
+[Read The Docs](https://range-streams.readthedocs.io/en/latest/)
+
+## Requires
+
+- Python 3.8+
+
+## Installation
+
+```sh
+pip install range-streams
+```
+
+> _range-streams_ is available from [PyPI](https://pypi.org/project/range-streams), and
+> the code is on [GitHub](https://github.com/lmmx/range-streams)
```

### Comparing `range_streams-1.2.9/src/range_streams.egg-info/SOURCES.txt` & `range_streams-1.3.0/src/range_streams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tests/async_test.py` & `range_streams-1.3.0/tests/async_test.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tests/codecs/conda_test.py` & `range_streams-1.3.0/tests/codecs/conda_test.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tests/codecs/data.py` & `range_streams-1.3.0/tests/codecs/data.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tests/codecs/png_test.py` & `range_streams-1.3.0/tests/codecs/png_test.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tests/codecs/tar_test.py` & `range_streams-1.3.0/tests/codecs/tar_test.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tests/codecs/zip_test.py` & `range_streams-1.3.0/tests/codecs/zip_test.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tests/http_utils_test.py` & `range_streams-1.3.0/tests/http_utils_test.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tests/overlaps_test.py` & `range_streams-1.3.0/tests/overlaps_test.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tests/range_stream_core_test.py` & `range_streams-1.3.0/tests/range_stream_core_test.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tests/range_stream_edge_case_test.py` & `range_streams-1.3.0/tests/range_stream_edge_case_test.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tests/range_stream_mono_test.py` & `range_streams-1.3.0/tests/range_stream_mono_test.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tests/range_utils_test.py` & `range_streams-1.3.0/tests/range_utils_test.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tests/request_test.py` & `range_streams-1.3.0/tests/request_test.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tests/response_test.py` & `range_streams-1.3.0/tests/response_test.py`

 * *Files identical despite different names*

### Comparing `range_streams-1.2.9/tox.ini` & `range_streams-1.3.0/tox.ini`

 * *Files identical despite different names*

