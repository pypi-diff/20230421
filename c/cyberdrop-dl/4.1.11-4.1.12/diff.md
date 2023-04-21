# Comparing `tmp/cyberdrop-dl-4.1.11.tar.gz` & `tmp/cyberdrop-dl-4.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.1.11.tar", last modified: Fri Apr 14 16:01:16 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.1.12.tar", last modified: Fri Apr 21 04:46:29 2023, max compression
```

## Comparing `cyberdrop-dl-4.1.11.tar` & `cyberdrop-dl-4.1.12.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.967603 cyberdrop-dl-4.1.11/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-04-14 16:01:16.967603 cyberdrop-dl-4.1.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.959603 cyberdrop-dl-4.1.11/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.963603 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.963603 cyberdrop-dl-4.1.11/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/client/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.967603 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    19384 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.967603 cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18269 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.967603 cyberdrop-dl-4.1.11/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:01:16.959603 cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-04-14 16:01:16.000000 cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-14 16:01:16.000000 cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:01:16.000000 cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 16:01:16.000000 cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-14 16:01:16.000000 cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 16:01:16.000000 cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-14 16:01:16.967603 cyberdrop-dl-4.1.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:01:06.000000 cyberdrop-dl-4.1.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.071224 cyberdrop-dl-4.1.12/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-04-21 04:46:29.071224 cyberdrop-dl-4.1.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.059224 cyberdrop-dl-4.1.12/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.063224 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.063224 cyberdrop-dl-4.1.12/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/client/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.067224 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19384 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.071224 cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.071224 cyberdrop-dl-4.1.12/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.059224 cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-04-21 04:46:29.000000 cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-21 04:46:29.000000 cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 04:46:29.000000 cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-21 04:46:29.000000 cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-21 04:46:29.000000 cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 04:46:29.000000 cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-21 04:46:29.071224 cyberdrop-dl-4.1.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/setup.py
```

### Comparing `cyberdrop-dl-4.1.11/LICENSE` & `cyberdrop-dl-4.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/PKG-INFO` & `cyberdrop-dl-4.1.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.11
+Version: 4.1.12
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.11 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.12 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.11/README.md` & `cyberdrop-dl-4.1.12/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/config_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,21 +57,22 @@
         },
         "Runtime": {
             "allow_insecure_connections": False,
             "attempts": 10,
             "block_sub_folders": False,
             "disable_attempt_limit": False,
             "include_id": False,
-            "skip_download_mark_completed": False,
             "output_errored_urls": False,
             "output_unsupported_urls": False,
             "proxy": "",
             "remove_bunkr_identifier": False,
             "required_free_space": 5,
             "simultaneous_downloads_per_domain": 4,
+            "skip_download_mark_completed": False,
+            "user_agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/112.0",
         },
         "Sorting": {
             "sort_downloads": False,
             "sort_directory": "Sorted Downloads",
             "sorted_audio": "{sort_dir}/{base_dir}/Audio",
             "sorted_images": "{sort_dir}/{base_dir}/Images",
             "sorted_others": "{sort_dir}/{base_dir}/Other",
```

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/client/rate_limiting.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/client/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     async def get_token(self, session: ScrapeSession, api_token=None):
         """Creates an anon gofile account to use."""
         if self.token:
             return
 
         if api_token:
             self.token = api_token
+            await self.set_cookie(session)
             return
 
         try:
             json_obj = await session.get_json(self.api_address / "createAccount")
             if json_obj["status"] == "ok":
                 self.token = json_obj["data"]["token"]
                 await self.set_cookie(session)
@@ -70,15 +71,15 @@
         """Gets links from the given url, creates media_items"""
         results = []
         params = {
             "token": self.token,
             "contentId": content_id,
             "websiteToken": "12345",
         }
-        content = await session.get_json_with_params(self.api_address / "getContent", params)
+        content = await session.get_json(self.api_address / "getContent", params)
         if content["status"] != "ok":
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             return results
 
         content = content['data']
         if title:
```

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,12 +71,11 @@
         images = images.findAll("img")
         for link in images:
             link = link.get('src').replace("thumbs", "images").replace("_b", "_o")
             output.append(URL(link))
 
         return title, output
 
-    async def singular(self, session: ScrapeSession, url: URL):
+    async def singular(self, session: ScrapeSession, url: URL) -> URL:
         """Gets individual links"""
         soup = await session.get_BS4(url)
-        link = URL(soup.select_one("img[id=img]").get('src'))
-        return link
+        return URL(soup.select_one("img[id=img]").get('src'))
```

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
 
     async def get_listings(self, session: ScrapeSession, identifier: str, url: URL):
         """Handles album scraping"""
         media_items = []
         try:
-            content = await session.get_json((self.api / "list" / identifier))
+            content = await session.get_json(self.api / "list" / identifier)
             for file in content['files']:
                 link = await self.create_download_link(file['id'])
                 try:
                     filename, ext = await get_filename_and_ext(file['name'])
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(link))
                     continue
@@ -54,17 +54,15 @@
             return media_items
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
-    async def get_file_name(self, session: ScrapeSession, identifier: str):
+    async def get_file_name(self, session: ScrapeSession, identifier: str) -> str:
         """Gets filename for the given file identifier"""
-        content = await session.get_json((self.api / 'file' / identifier / 'info'))
-        filename = content['name']
-        return filename
+        content = await session.get_json(self.api / 'file' / identifier / 'info')
+        return content['name']
 
-    async def create_download_link(self, file: str):
+    async def create_download_link(self, file: str) -> URL:
         """Gets download links for the file given"""
-        final_url = (self.api / 'file' / file).with_query('download')
-        return final_url
+        return (self.api / 'file' / file).with_query('download')
```

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,17 +60,16 @@
                     continue
                 complete = await self.SQL_Helper.check_complete_singular("postimg", img)
                 media_item = MediaItem(img, referer, complete, filename, ext, filename)
 
                 content.append(media_item)
         return content
 
-    async def get_singular(self, session: ScrapeSession, url: URL):
+    async def get_singular(self, session: ScrapeSession, url: URL) -> MediaItem:
         """Handles singular folder scraping"""
         soup = await session.get_BS4(url)
         link = URL(soup.select_one("a[id=download]").get('href').replace("?dl=1", ""))
 
         filename, ext = await get_filename_and_ext(link.name)
         complete = await self.SQL_Helper.check_complete_singular("postimg", link)
-        media_item = MediaItem(link, url, complete, filename, ext, filename)
 
-        return media_item
+        return MediaItem(link, url, complete, filename, ext, filename)
```

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,18 +44,17 @@
         else:
             await self.parse_profile(session, url, domain_obj)
 
         await self.SQL_Helper.insert_domain("sharex", url, domain_obj)
         await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return domain_obj
 
-    async def jpg_fish_from_church(self, url: URL):
+    async def jpg_fish_from_church(self, url: URL) -> URL:
         pattern = r"simp([1-5])\.jpg\.church/"
-        url = URL(re.sub(pattern, r'simp\1.jpg.fish/', str(url)))
-        return url
+        return URL(re.sub(pattern, r'simp\1.jpg.fish/', str(url)))
 
     async def get_albums(self, session: ScrapeSession, url: URL, domain_obj: DomainItem):
         """Handles scraping for Albums"""
         try:
             soup = await session.get_BS4(url)
             albums = soup.select("a[class='image-container --media']")
             for album in albums:
```

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/main.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
     forum_opts = parser.add_argument_group("Forum options")
     forum_opts.add_argument("--output-last-forum-post", help="outputs the last post of a forum scrape to use as a starting point for future runs", action="store_true")
     forum_opts.add_argument("--separate-posts", help="separates forum scraping into folders by post number", action="store_true")
 
     # Authentication details
     config_group = config_data["Authentication"]
     auth_opts = parser.add_argument_group("Authentication options")
+    auth_opts.add_argument("--gofile-api-key", help="api key for premium gofile", default=config_group["gofile_api_key"])
     auth_opts.add_argument("--pixeldrain-api-key", help="api key for premium pixeldrain", default=config_group["pixeldrain_api_key"])
     auth_opts.add_argument("--simpcity-username", help="username to login to simpcity", default=config_group["simpcity_username"])
     auth_opts.add_argument("--simpcity-password", help="password to login to simpcity", default=config_group['simpcity_password'])
     auth_opts.add_argument("--socialmediagirls-username", help="username to login to socialmediagirls", default=config_group["socialmediagirls_username"])
     auth_opts.add_argument("--socialmediagirls-password", help="password to login to socialmediagirls", default=config_group["socialmediagirls_password"])
     auth_opts.add_argument("--xbunker-username", help="username to login to xbunker", default=config_group["xbunker_username"])
     auth_opts.add_argument("--xbunker-password", help="password to login to xbunker", default=config_group["xbunker_password"])
@@ -225,15 +226,16 @@
 
     if not await check_free_space(args['Runtime']['required_free_space'], args['Files']['output_folder']):
         await log("Not enough free space to continue. You can change the required space required using --required-free-space.", style="red")
         exit(1)
 
     links = await consolidate_links(args, links)
     client = Client(args['Ratelimiting']['ratelimit'], args['Ratelimiting']['throttle'],
-                    args['Runtime']['allow_insecure_connections'], args["Ratelimiting"]["connection_timeout"])
+                    args['Runtime']['allow_insecure_connections'], args["Ratelimiting"]["connection_timeout"],
+                    args['Runtime']['user_agent'])
     SQL_Helper = SQLHelper(args['Ignore']['ignore_history'], args['Ignore']['ignore_cache'], args['Files']['db_file'])
     Scraper = ScrapeMapper(args, client, SQL_Helper, False)
 
     await SQL_Helper.sql_initialize()
 
     if links:
         Cascade, Forums = await scrape_links(Scraper, links)
```

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.1.12/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.11
+Version: 4.1.12
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.11 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.12 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.11/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.11/setup.cfg` & `cyberdrop-dl-4.1.12/setup.cfg`

 * *Files identical despite different names*

