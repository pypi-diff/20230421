# Comparing `tmp/unstructured-0.6.0.tar.gz` & `tmp/unstructured-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.6.0.tar", last modified: Fri Apr 21 17:13:54 2023, max compression
+gzip compressed data, was "unstructured-0.6.1.tar", last modified: Fri Apr 21 18:50:55 2023, max compression
```

## Comparing `unstructured-0.6.0.tar` & `unstructured-0.6.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:54.009134 unstructured-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-21 17:13:43.000000 unstructured-0.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-04-21 17:13:54.009134 unstructured-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-04-21 17:13:43.000000 unstructured-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-21 17:13:54.009134 unstructured-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-21 17:13:43.000000 unstructured-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.993133 unstructured-0.6.0/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.993133 unstructured-0.6.0/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-21 17:13:43.000000 unstructured-0.6.0/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-21 17:13:43.000000 unstructured-0.6.0/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-21 17:13:43.000000 unstructured-0.6.0/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-21 17:13:43.000000 unstructured-0.6.0/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.993133 unstructured-0.6.0/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.997133 unstructured-0.6.0/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.997133 unstructured-0.6.0/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.997133 unstructured-0.6.0/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.997133 unstructured-0.6.0/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.997133 unstructured-0.6.0/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:54.001134 unstructured-0.6.0/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27999 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:54.001134 unstructured-0.6.0/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:54.005134 unstructured-0.6.0/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:54.005134 unstructured-0.6.0/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/text_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:54.009134 unstructured-0.6.0/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.997133 unstructured-0.6.0/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-04-21 17:13:53.000000 unstructured-0.6.0/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-21 17:13:53.000000 unstructured-0.6.0/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 17:13:53.000000 unstructured-0.6.0/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 17:13:53.000000 unstructured-0.6.0/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-21 17:13:53.000000 unstructured-0.6.0/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 17:13:53.000000 unstructured-0.6.0/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.106627 unstructured-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-21 18:50:46.000000 unstructured-0.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-04-21 18:50:55.106627 unstructured-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-04-21 18:50:46.000000 unstructured-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-21 18:50:55.106627 unstructured-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-21 18:50:47.000000 unstructured-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-21 18:50:47.000000 unstructured-0.6.1/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-21 18:50:47.000000 unstructured-0.6.1/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-21 18:50:47.000000 unstructured-0.6.1/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-21 18:50:47.000000 unstructured-0.6.1/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.098627 unstructured-0.6.1/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.098627 unstructured-0.6.1/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27999 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.098627 unstructured-0.6.1/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.102627 unstructured-0.6.1/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.102627 unstructured-0.6.1/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/text_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.106627 unstructured-0.6.1/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-04-21 18:50:54.000000 unstructured-0.6.1/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-21 18:50:55.000000 unstructured-0.6.1/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:50:54.000000 unstructured-0.6.1/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 18:50:54.000000 unstructured-0.6.1/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-21 18:50:54.000000 unstructured-0.6.1/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 18:50:54.000000 unstructured-0.6.1/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.6.0/LICENSE.md` & `unstructured-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/PKG-INFO` & `unstructured-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.0 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.1 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.6.0/README.md` & `unstructured-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/setup.py` & `unstructured-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.6.1/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.6.1/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/test_unstructured/test_utils.py` & `unstructured-0.6.1/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/cleaners/core.py` & `unstructured-0.6.1/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/cleaners/extract.py` & `unstructured-0.6.1/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/cleaners/translate.py` & `unstructured-0.6.1/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/documents/base.py` & `unstructured-0.6.1/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/documents/elements.py` & `unstructured-0.6.1/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/documents/email_elements.py` & `unstructured-0.6.1/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/documents/html.py` & `unstructured-0.6.1/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/documents/xml.py` & `unstructured-0.6.1/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/file_utils/exploration.py` & `unstructured-0.6.1/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/file_utils/file_conversion.py` & `unstructured-0.6.1/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/file_utils/filetype.py` & `unstructured-0.6.1/unstructured/file_utils/filetype.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/file_utils/metadata.py` & `unstructured-0.6.1/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/connector/azure.py` & `unstructured-0.6.1/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/connector/biomed.py` & `unstructured-0.6.1/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/connector/fsspec.py` & `unstructured-0.6.1/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/connector/git.py` & `unstructured-0.6.1/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/connector/github.py` & `unstructured-0.6.1/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/connector/gitlab.py` & `unstructured-0.6.1/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/connector/google_drive.py` & `unstructured-0.6.1/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/connector/local.py` & `unstructured-0.6.1/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/connector/reddit.py` & `unstructured-0.6.1/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/connector/s3.py` & `unstructured-0.6.1/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/connector/slack.py` & `unstructured-0.6.1/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.6.1/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.6.1/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/interfaces.py` & `unstructured-0.6.1/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/ingest/main.py` & `unstructured-0.6.1/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/nlp/english-words.txt` & `unstructured-0.6.1/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/nlp/english_words.py` & `unstructured-0.6.1/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/nlp/patterns.py` & `unstructured-0.6.1/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/nlp/tokenize.py` & `unstructured-0.6.1/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/__init__.py` & `unstructured-0.6.1/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/auto.py` & `unstructured-0.6.1/unstructured/partition/auto.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     include_page_breaks: bool = False,
     strategy: str = "hi_res",
     encoding: str = "utf-8",
     paragraph_grouper: Optional[Callable[[str], str]] = None,
     headers: Dict[str, str] = {},
     ssl_verify: bool = True,
     ocr_languages: str = "eng",
-    pdf_extract_tables: bool = False,
+    pdf_infer_table_structure: bool = False,
 ):
     """Partitions a document into its constituent elements. Will use libmagic to determine
     the file's type and route it to the appropriate partitioning function. Applies the default
     parameters for each partitioning function. Use the document-type specific partitioning
     functions if you need access to additional kwarg options.
 
     Parameters
@@ -67,17 +67,19 @@
         The headers to be used in conjunction with the HTTP request if URL is set.
     ssl_verify
         If the URL parameter is set, determines whether or not partition uses SSL verification
         in the HTTP request.
     ocr_languages
         The languages to use for the Tesseract agent. To use a language, you'll first need
         to isntall the appropriate Tesseract language pack.
-    pdf_extract_tables
-        If True, in the case that the file to be processed is detected to be a PDF, any tables that
-        are detected will be extracted.
+    pdf_infer_table_structure
+        If True and strategy=hi_res, any Table Elements extracted from a PDF will include an
+        additional metadata field, "text_as_html," where the value (string) is a just a
+        transformation of the data into an HTML <table>.
+        The "text" field for a partitioned Table Element is always present, whether True or False.
     """
     exactly_one(file=file, filename=filename, url=url)
 
     if url is not None:
         file, filetype = file_and_type_from_url(
             url=url,
             content_type=content_type,
@@ -130,15 +132,15 @@
     elif filetype == FileType.PDF:
         elements = partition_pdf(
             filename=filename,  # type: ignore
             file=file,  # type: ignore
             url=None,
             include_page_breaks=include_page_breaks,
             encoding=encoding,
-            extract_tables=pdf_extract_tables,
+            infer_table_structure=pdf_infer_table_structure,
             strategy=strategy,
             ocr_languages=ocr_languages,
         )
     elif (filetype == FileType.PNG) or (filetype == FileType.JPG):
         elements = partition_image(
             filename=filename,  # type: ignore
             file=file,  # type: ignore
```

### Comparing `unstructured-0.6.0/unstructured/partition/common.py` & `unstructured-0.6.1/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/doc.py` & `unstructured-0.6.1/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/docx.py` & `unstructured-0.6.1/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/email.py` & `unstructured-0.6.1/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/epub.py` & `unstructured-0.6.1/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/html.py` & `unstructured-0.6.1/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/image.py` & `unstructured-0.6.1/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/json.py` & `unstructured-0.6.1/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/md.py` & `unstructured-0.6.1/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/msg.py` & `unstructured-0.6.1/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/pdf.py` & `unstructured-0.6.1/unstructured/partition/pdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     filename: str = "",
     file: Optional[bytes] = None,
     url: Optional[str] = None,
     template: str = "layout/pdf",
     token: Optional[str] = None,
     include_page_breaks: bool = False,
     strategy: str = "hi_res",
-    extract_tables: bool = False,
+    infer_table_structure: bool = False,
     encoding: str = "utf-8",
     ocr_languages: str = "eng",
 ) -> List[Element]:
     """Parses a pdf document into a list of interpreted elements.
     Parameters
     ----------
     filename
@@ -41,20 +41,21 @@
         be used.
     token
         A string defining the authentication token for a self-host url, if applicable.
     strategy
         The strategy to use for partitioning the PDF. Uses a layout detection model if set
         to 'hi_res', otherwise partition_pdf simply extracts the text from the document
         and processes it.
-    extract_tables
-        If True, extracts any tables that are detected when using 'hi_res' strategy. Whether this
-        is True or False, the partitioning process will attempt to identify any tables in the
-        document. This parameter indicates that the partitioning process will attempt to extract the
-        structure of any identified tables. The table structure and cell contents will be stored as
-        HTML in the metadata in the text_as_html property, e.g. element.metadata.text_as_html
+    infer_table_structure
+        Only applicable if `strategy=hi_res`.
+        If True, any Table elements that are extracted will also have a metadata field
+        named "text_as_html" where the table's text content is rendered into an html string.
+        I.e., rows and cells are preserved.
+        Whether True or False, the "text" field is always present in any Table element
+        and is the text content of the table (no structure).
     encoding
         The encoding method used to decode the text input. If None, utf-8 will be used.
     ocr_languages
         The languages to use for the Tesseract agent. To use a language, you'll first need
         to isntall the appropriate Tesseract language pack.
     """
     exactly_one(filename=filename, file=file)
@@ -62,30 +63,30 @@
         filename=filename,
         file=file,
         url=url,
         template=template,
         token=token,
         include_page_breaks=include_page_breaks,
         strategy=strategy,
-        extract_tables=extract_tables,
+        infer_table_structure=infer_table_structure,
         encoding=encoding,
         ocr_languages=ocr_languages,
     )
 
 
 def partition_pdf_or_image(
     filename: str = "",
     file: Optional[bytes] = None,
     url: Optional[str] = "https://ml.unstructured.io/",
     template: str = "layout/pdf",
     token: Optional[str] = None,
     is_image: bool = False,
     include_page_breaks: bool = False,
     strategy: str = "hi_res",
-    extract_tables: bool = False,
+    infer_table_structure: bool = False,
     encoding: str = "utf-8",
     ocr_languages: str = "eng",
 ) -> List[Element]:
     """Parses a pdf or image document into a list of interpreted elements."""
     if url is None:
         # TODO(alan): Extract information about the filetype to be processed from the template
         # route. Decoding the routing should probably be handled by a single function designed for
@@ -113,26 +114,26 @@
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 layout_elements = _partition_pdf_or_image_local(
                     filename=filename,
                     file=file,
                     template=out_template,
                     is_image=is_image,
-                    extract_tables=extract_tables,
+                    infer_table_structure=infer_table_structure,
                     include_page_breaks=True,
                     ocr_languages=ocr_languages,
                 )
 
         elif strategy == "fast" or fallback_to_fast:
             if strategy == "hi_res":
                 logger.warning(
                     "detectron2 is not installed. Cannot use the hi_res partitioning "
                     "strategy. Falling back to partitioning with the fast strategy.",
                 )
-            if extract_tables:
+            if infer_table_structure:
                 logger.warning(
                     "Table extraction was selected, but is being ignored while using the fast "
                     "strategy.",
                 )
 
             return _partition_pdf_with_pdfminer(
                 filename=filename,
@@ -169,15 +170,15 @@
 
 
 def _partition_pdf_or_image_local(
     filename: str = "",
     file: Optional[bytes] = None,
     template: Optional[str] = None,
     is_image: bool = False,
-    extract_tables: bool = False,
+    infer_table_structure: bool = False,
     include_page_breaks: bool = False,
     ocr_languages: str = "eng",
 ) -> List[Element]:
     """Partition using package installed locally."""
     try:
         from unstructured_inference.inference.layout import (
             process_data_with_model,
@@ -200,23 +201,23 @@
 
     if file is None:
         layout = process_file_with_model(
             filename,
             template,
             is_image=is_image,
             ocr_languages=ocr_languages,
-            extract_tables=extract_tables,
+            extract_tables=infer_table_structure,
         )
     else:
         layout = process_data_with_model(
             file,
             template,
             is_image=is_image,
             ocr_languages=ocr_languages,
-            extract_tables=extract_tables,
+            extract_tables=infer_table_structure,
         )
 
     return document_to_element_list(layout, include_page_breaks=include_page_breaks)
 
 
 @requires_dependencies("pdfminer", "local-inference")
 def _partition_pdf_with_pdfminer(
```

### Comparing `unstructured-0.6.0/unstructured/partition/ppt.py` & `unstructured-0.6.1/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/pptx.py` & `unstructured-0.6.1/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/rtf.py` & `unstructured-0.6.1/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/text.py` & `unstructured-0.6.1/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/partition/text_type.py` & `unstructured-0.6.1/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/staging/argilla.py` & `unstructured-0.6.1/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/staging/base.py` & `unstructured-0.6.1/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/staging/datasaur.py` & `unstructured-0.6.1/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/staging/huggingface.py` & `unstructured-0.6.1/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/staging/label_box.py` & `unstructured-0.6.1/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/staging/label_studio.py` & `unstructured-0.6.1/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/staging/prodigy.py` & `unstructured-0.6.1/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured/utils.py` & `unstructured-0.6.1/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.0/unstructured.egg-info/PKG-INFO` & `unstructured-0.6.1/unstructured.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.0 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.1 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.6.0/unstructured.egg-info/SOURCES.txt` & `unstructured-0.6.1/unstructured.egg-info/SOURCES.txt`

 * *Files identical despite different names*

