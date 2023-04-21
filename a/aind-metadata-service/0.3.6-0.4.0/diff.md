# Comparing `tmp/aind_metadata_service-0.3.6.tar.gz` & `tmp/aind_metadata_service-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_service-0.3.6.tar", last modified: Thu Mar 30 20:08:16 2023, max compression
+gzip compressed data, was "aind_metadata_service-0.4.0.tar", last modified: Fri Apr 21 16:41:02 2023, max compression
```

## Comparing `aind_metadata_service-0.3.6.tar` & `aind_metadata_service-0.4.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:16.017681 aind_metadata_service-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:15.989682 aind_metadata_service-0.3.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:15.997681 aind_metadata_service-0.3.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:15.997681 aind_metadata_service-0.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-03-30 20:08:16.017681 aind_metadata_service-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:16.001681 aind_metadata_service-0.3.6/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:16.001681 aind_metadata_service-0.3.6/doc_template/source/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/doc_template/source/aind_metadata_service.labtracks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/doc_template/source/aind_metadata_service.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/doc_template/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 20:08:16.017681 aind_metadata_service-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:15.993682 aind_metadata_service-0.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:16.001681 aind_metadata_service-0.3.6/src/aind_metadata_service/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/src/aind_metadata_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/src/aind_metadata_service/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:16.005681 aind_metadata_service-0.3.6/src/aind_metadata_service/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/src/aind_metadata_service/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/src/aind_metadata_service/labtracks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/src/aind_metadata_service/labtracks/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/src/aind_metadata_service/response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/src/aind_metadata_service/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:16.009682 aind_metadata_service-0.3.6/src/aind_metadata_service/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/src/aind_metadata_service/sharepoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   102957 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/src/aind_metadata_service/sharepoint/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/src/aind_metadata_service/sharepoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:16.005681 aind_metadata_service-0.3.6/src/aind_metadata_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-03-30 20:08:15.000000 aind_metadata_service-0.3.6/src/aind_metadata_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-03-30 20:08:15.000000 aind_metadata_service-0.3.6/src/aind_metadata_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:08:15.000000 aind_metadata_service-0.3.6/src/aind_metadata_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-30 20:08:15.000000 aind_metadata_service-0.3.6/src/aind_metadata_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-30 20:08:15.000000 aind_metadata_service-0.3.6/src/aind_metadata_service.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:16.009682 aind_metadata_service-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:16.009682 aind_metadata_service-0.3.6/tests/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/labtracks/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/labtracks/test_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/labtracks/test_response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:16.009682 aind_metadata_service-0.3.6/tests/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:08:16.017681 aind_metadata_service-0.3.6/tests/sharepoint/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item7.json
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item9.json
--rw-r--r--   0 runner    (1001) docker     (123)    39684 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/sharepoint/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-30 20:07:58.000000 aind_metadata_service-0.3.6/tests/test_response_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.860521 aind_metadata_service-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.852521 aind_metadata_service-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.852521 aind_metadata_service-0.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.852521 aind_metadata_service-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-21 16:41:02.860521 aind_metadata_service-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.852521 aind_metadata_service-0.4.0/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/doc_template/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/doc_template/source/aind_metadata_service.labtracks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/doc_template/source/aind_metadata_service.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/doc_template/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 16:41:02.860521 aind_metadata_service-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.852521 aind_metadata_service-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/src/aind_metadata_service/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/src/aind_metadata_service/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/labtracks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/labtracks/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/src/aind_metadata_service/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/sharepoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102957 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/sharepoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/sharepoint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-21 16:41:02.000000 aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-21 16:41:02.000000 aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:41:02.000000 aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-21 16:41:02.000000 aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 16:41:02.000000 aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/tests/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/labtracks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/labtracks/test_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/labtracks/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/tests/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.860521 aind_metadata_service-0.4.0/tests/sharepoint/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item7.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item9.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39684 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/test_response_handle.py
```

### Comparing `aind_metadata_service-0.3.6/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_service-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_service-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_service-0.4.0/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/.github/workflows/ci.yml` & `aind_metadata_service-0.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/.github/workflows/publish.yml` & `aind_metadata_service-0.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/.gitignore` & `aind_metadata_service-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/Dockerfile` & `aind_metadata_service-0.4.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/LICENSE` & `aind_metadata_service-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/PKG-INFO` & `aind_metadata_service-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_metadata_service
-Version: 0.3.6
+Version: 0.4.0
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.3.6/README.md` & `aind_metadata_service-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/doc_template/Makefile` & `aind_metadata_service-0.4.0/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/doc_template/make.bat` & `aind_metadata_service-0.4.0/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/doc_template/source/aind_metadata_service.labtracks.rst` & `aind_metadata_service-0.4.0/doc_template/source/aind_metadata_service.labtracks.rst`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/doc_template/source/conf.py` & `aind_metadata_service-0.4.0/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/pyproject.toml` & `aind_metadata_service-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/src/aind_metadata_service/client.py` & `aind_metadata_service-0.4.0/src/aind_metadata_service/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/src/aind_metadata_service/labtracks/client.py` & `aind_metadata_service-0.4.0/src/aind_metadata_service/labtracks/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/src/aind_metadata_service/labtracks/query_builder.py` & `aind_metadata_service-0.4.0/src/aind_metadata_service/labtracks/query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/src/aind_metadata_service/response_handler.py` & `aind_metadata_service-0.4.0/src/aind_metadata_service/response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/src/aind_metadata_service/server.py` & `aind_metadata_service-0.4.0/src/aind_metadata_service/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 """Starts and runs a Flask Service"""
 
 import os
 
 from fastapi import FastAPI
+from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import RedirectResponse
 
 from aind_metadata_service.labtracks.client import LabTracksClient
 from aind_metadata_service.sharepoint.client import SharePointClient
 
 app = FastAPI()
 
+app.add_middleware(
+    CORSMiddleware,
+    allow_origins=["*"],
+    allow_methods=["GET"],
+    allow_headers=["*"],
+)
+
 # TODO: Handle configs better?
 favicon_path = os.getenv("FAVICON_PATH")
 
 labtracks_driver = os.getenv("ODBC_DRIVER")
 labtracks_server = os.getenv("LABTRACKS_SERVER")
 labtracks_port = os.getenv("LABTRACKS_PORT")
 labtracks_db = os.getenv("LABTRACKS_DATABASE")
```

### Comparing `aind_metadata_service-0.3.6/src/aind_metadata_service/sharepoint/client.py` & `aind_metadata_service-0.4.0/src/aind_metadata_service/sharepoint/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/src/aind_metadata_service/sharepoint/utils.py` & `aind_metadata_service-0.4.0/src/aind_metadata_service/sharepoint/utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/src/aind_metadata_service.egg-info/PKG-INFO` & `aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-service
-Version: 0.3.6
+Version: 0.4.0
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.3.6/src/aind_metadata_service.egg-info/SOURCES.txt` & `aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/labtracks/test_client.py` & `aind_metadata_service-0.4.0/tests/labtracks/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/labtracks/test_query_builder.py` & `aind_metadata_service-0.4.0/tests/labtracks/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/labtracks/test_response_handler.py` & `aind_metadata_service-0.4.0/tests/labtracks/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item1.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item10.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item11.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item12.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item12.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item13.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item13.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item14.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item14.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item15.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item15.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item16.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item16.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item17.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item17.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item2.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item3.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item4.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item5.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item6.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item7.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item8.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/resources/list_item9.json` & `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/sharepoint/test_client.py` & `aind_metadata_service-0.4.0/tests/sharepoint/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/test_client.py` & `aind_metadata_service-0.4.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.3.6/tests/test_response_handle.py` & `aind_metadata_service-0.4.0/tests/test_response_handle.py`

 * *Files identical despite different names*

