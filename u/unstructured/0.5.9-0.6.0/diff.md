# Comparing `tmp/unstructured-0.5.9.tar.gz` & `tmp/unstructured-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.5.9.tar", last modified: Mon Apr  3 18:19:40 2023, max compression
+gzip compressed data, was "unstructured-0.6.0.tar", last modified: Fri Apr 21 17:13:54 2023, max compression
```

## Comparing `unstructured-0.5.9.tar` & `unstructured-0.6.0.tar`

### file list

```diff
@@ -1,102 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.363400 unstructured-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-03 18:19:33.000000 unstructured-0.5.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-04-03 18:19:40.363400 unstructured-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-04-03 18:19:33.000000 unstructured-0.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-03 18:19:40.363400 unstructured-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-03 18:19:33.000000 unstructured-0.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.351400 unstructured-0.5.9/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.351400 unstructured-0.5.9/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-03 18:19:33.000000 unstructured-0.5.9/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-03 18:19:33.000000 unstructured-0.5.9/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-03 18:19:33.000000 unstructured-0.5.9/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-03 18:19:33.000000 unstructured-0.5.9/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23278 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.359400 unstructured-0.5.9/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.363400 unstructured-0.5.9/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/text_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.363400 unstructured-0.5.9/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-04-03 18:19:40.000000 unstructured-0.5.9/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-03 18:19:40.000000 unstructured-0.5.9/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 18:19:40.000000 unstructured-0.5.9/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-03 18:19:40.000000 unstructured-0.5.9/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-03 18:19:40.000000 unstructured-0.5.9/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-03 18:19:40.000000 unstructured-0.5.9/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:54.009134 unstructured-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-21 17:13:43.000000 unstructured-0.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-04-21 17:13:54.009134 unstructured-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-04-21 17:13:43.000000 unstructured-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-21 17:13:54.009134 unstructured-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-21 17:13:43.000000 unstructured-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.993133 unstructured-0.6.0/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.993133 unstructured-0.6.0/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-21 17:13:43.000000 unstructured-0.6.0/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-21 17:13:43.000000 unstructured-0.6.0/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-21 17:13:43.000000 unstructured-0.6.0/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-21 17:13:43.000000 unstructured-0.6.0/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.993133 unstructured-0.6.0/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.997133 unstructured-0.6.0/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.997133 unstructured-0.6.0/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.997133 unstructured-0.6.0/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.997133 unstructured-0.6.0/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.997133 unstructured-0.6.0/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:54.001134 unstructured-0.6.0/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27999 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:54.001134 unstructured-0.6.0/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:54.005134 unstructured-0.6.0/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:54.005134 unstructured-0.6.0/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/partition/text_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:54.009134 unstructured-0.6.0/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-21 17:13:43.000000 unstructured-0.6.0/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:13:53.997133 unstructured-0.6.0/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-04-21 17:13:53.000000 unstructured-0.6.0/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-21 17:13:53.000000 unstructured-0.6.0/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 17:13:53.000000 unstructured-0.6.0/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 17:13:53.000000 unstructured-0.6.0/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-21 17:13:53.000000 unstructured-0.6.0/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 17:13:53.000000 unstructured-0.6.0/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.5.9/LICENSE.md` & `unstructured-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/PKG-INFO` & `unstructured-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.5.9
+Version: 0.6.0
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -30,14 +30,26 @@
           href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
             <img src="https://img.shields.io/badge/JOIN US ON SLACK-4A154B?style=for-the-badge&logo=slack&logoColor=white" />
           </a>
           <a href="https://www.linkedin.com/company/unstructuredio/">
             <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
           </a>
         </div>
+        <h2 align="center">
+          <p>Announcement!!!</p>
+        </h2>
+        <div align="center">
+          <p>We're excited to announce the public release of the unstructured.io hosted API! Now you can leverage Unstructured with a simple API call to render clean text in JSON format out of your images, documents, powerpoints, and more.</p>
+        
+        <p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. You’ll also find instructions there about how to host your own version of the API. Unstructured data just got easier! 
+        We'd love to hear your feedback, let us know how it goes in our <a
+          href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
+           community slack</a>. And stay tuned for improvements to both quality and performance over the coming months!
+        <p><img src="easy.gif"></p></p>
+        </div>
         
         <h3 align="center">
           <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
         </h3>
         
         The `unstructured` library provides open-source components for pre-processing text documents
         such as **PDFs**, **HTML** and **Word** Documents. These components are packaged as *bricks* 🧱, which provide
@@ -65,15 +77,15 @@
           Depending on what document types you're parsing, you may not need all of these.
             - `libmagic-dev` (filetype detection)
             - `poppler-utils` (images and PDFs)
             - `tesseract-ocr` (images and PDFs)
             - `libreoffice` (MS Office docs)
         - If you are parsing PDFs, run the following to install the `detectron2` model, which
           `unstructured` uses for layout detection:
-            - `pip install "detectron2@git+https://github.com/facebookresearch/detectron2.git@v0.6#egg=detectron2"`
+            - `pip install "detectron2@git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"`
         
         At this point, you should be able to run the following code:
         
         ```python
         from unstructured.partition.auto import partition
         
         elements = partition(filename="example-docs/fake-email.eml")
@@ -171,15 +183,15 @@
         you can also uninstall the hooks with `pre-commit uninstall`.
         
         ## :clap: Quick Tour
         
         You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
         
         The following examples show how to get started with the `unstructured` library.
-        You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **EPUB**, **DOC**, **DOCX**, **PPT**, **PPTX**, **JPG**,
+        You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**, **PPT**, **PPTX**, **JPG**,
         and **PNG** documents with one line of code!
         <br></br>
         See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
         of the features in the library.
         
         ### Document Parsing
         
@@ -393,9 +405,10 @@
 Provides-Extra: huggingface
 Provides-Extra: local-inference
 Provides-Extra: s3
 Provides-Extra: azure
 Provides-Extra: github
 Provides-Extra: gitlab
 Provides-Extra: reddit
+Provides-Extra: slack
 Provides-Extra: wikipedia
 Provides-Extra: google-drive
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.5.9 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.0 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -12,14 +12,24 @@
     /img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg) ![https://
  GitHub.com/unstructured-io/unstructured.js/releases](https://img.shields.io/
   github/release/unstructured-io/unstructured) ![https://github.com/Naereen/
 badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)
      [https://img.shields.io/badge/JOIN_US_ON_SLACK-4A154B?style=for-the-
    badge&logo=slack&logoColor=white] [https://img.shields.io/badge/LinkedIn-
            0077B5?style=for-the-badge&logo=linkedin&logoColor=white]
+                          ***** Announcement!!! *****
+We're excited to announce the public release of the unstructured.io hosted API!
+ Now you can leverage Unstructured with a simple API call to render clean text
+     in JSON format out of your images, documents, powerpoints, and more.
+ Checkout the readme here to get started making API calls. Youâll also find
+instructions there about how to host your own version of the API. Unstructured
+data just got easier! We'd love to hear your feedback, let us know how it goes
+  in our community_slack. And stay tuned for improvements to both quality and
+                      performance over the coming months!
+                                  [easy.gif]
        **** Open-Source Pre-Processing Tools for Unstructured Data ****
 The `unstructured` library provides open-source components for pre-processing
 text documents such as **PDFs**, **HTML** and **Word** Documents. These
 components are packaged as *bricks* ð§±, which provide users the building
 blocks they need to build pipelines targeted at the documents they care about.
 Bricks in the library fall into three categories: - :jigsaw: ***Partitioning
 bricks*** that break raw documents down into standard, structured elements. - :
@@ -34,19 +44,19 @@
 Install the following system dependencies if they are not already available on
 your system. Depending on what document types you're parsing, you may not need
 all of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
 - If you are parsing PDFs, run the following to install the `detectron2` model,
 which `unstructured` uses for layout detection: - `pip install
 "detectron2@git+https://github.com/facebookresearch/
-detectron2.git@v0.6#egg=detectron2"` At this point, you should be able to run
-the following code: ```python from unstructured.partition.auto import partition
-elements = partition(filename="example-docs/fake-email.eml") print("\n\n".join(
-[str(el) for el in elements])) ``` And if you installed with `local-inference`,
-you should be able to run this as well: ```python from
+detectron2.git@e2ce8dc#egg=detectron2"` At this point, you should be able to
+run the following code: ```python from unstructured.partition.auto import
+partition elements = partition(filename="example-docs/fake-email.eml") print
+("\n\n".join([str(el) for el in elements])) ``` And if you installed with
+`local-inference`, you should be able to run this as well: ```python from
 unstructured.partition.auto import partition elements = partition("example-
 docs/layout-parser-paper.pdf") print("\n\n".join([str(el) for el in elements]))
 ``` ## :dizzy: Instructions for using the docker image The following
 instructions are intended to help you get up and running using Docker to
 interact with `unstructured`. See [here](https://docs.docker.com/get-docker/
 ) if you don't already have docker installed on your machine. NOTE: we build
 multi-platform images to support both x86_64 and Apple silicon hardware.
@@ -98,16 +108,16 @@
 `pre-commit`, you'll just need to install the hooks with `pre-commit install`
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
 show how to get started with the `unstructured` library. You can parse **TXT**,
-**HTML**, **PDF**, **EML**, **MSG**, **EPUB**, **DOC**, **DOCX**, **PPT**,
-**PPTX**, **JPG**, and **PNG** documents with one line of code!
+**HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
+**PPT**, **PPTX**, **JPG**, and **PNG** documents with one line of code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
@@ -208,9 +218,9 @@
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.7.0 Description-Content-Type:
 text/markdown Provides-Extra: huggingface Provides-Extra: local-inference
 Provides-Extra: s3 Provides-Extra: azure Provides-Extra: github Provides-Extra:
-gitlab Provides-Extra: reddit Provides-Extra: wikipedia Provides-Extra: google-
-drive
+gitlab Provides-Extra: reddit Provides-Extra: slack Provides-Extra: wikipedia
+Provides-Extra: google-drive
```

### Comparing `unstructured-0.5.9/README.md` & `unstructured-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,26 @@
   href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
     <img src="https://img.shields.io/badge/JOIN US ON SLACK-4A154B?style=for-the-badge&logo=slack&logoColor=white" />
   </a>
   <a href="https://www.linkedin.com/company/unstructuredio/">
     <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
   </a>
 </div>
+<h2 align="center">
+  <p>Announcement!!!</p>
+</h2>
+<div align="center">
+  <p>We're excited to announce the public release of the unstructured.io hosted API! Now you can leverage Unstructured with a simple API call to render clean text in JSON format out of your images, documents, powerpoints, and more.</p>
+
+<p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. You’ll also find instructions there about how to host your own version of the API. Unstructured data just got easier! 
+We'd love to hear your feedback, let us know how it goes in our <a
+  href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
+   community slack</a>. And stay tuned for improvements to both quality and performance over the coming months!
+<p><img src="easy.gif"></p></p>
+</div>
 
 <h3 align="center">
   <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
 </h3>
 
 The `unstructured` library provides open-source components for pre-processing text documents
 such as **PDFs**, **HTML** and **Word** Documents. These components are packaged as *bricks* 🧱, which provide
@@ -57,15 +69,15 @@
   Depending on what document types you're parsing, you may not need all of these.
     - `libmagic-dev` (filetype detection)
     - `poppler-utils` (images and PDFs)
     - `tesseract-ocr` (images and PDFs)
     - `libreoffice` (MS Office docs)
 - If you are parsing PDFs, run the following to install the `detectron2` model, which
   `unstructured` uses for layout detection:
-    - `pip install "detectron2@git+https://github.com/facebookresearch/detectron2.git@v0.6#egg=detectron2"`
+    - `pip install "detectron2@git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"`
 
 At this point, you should be able to run the following code:
 
 ```python
 from unstructured.partition.auto import partition
 
 elements = partition(filename="example-docs/fake-email.eml")
@@ -163,15 +175,15 @@
 you can also uninstall the hooks with `pre-commit uninstall`.
 
 ## :clap: Quick Tour
 
 You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
 
 The following examples show how to get started with the `unstructured` library.
-You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **EPUB**, **DOC**, **DOCX**, **PPT**, **PPTX**, **JPG**,
+You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**, **PPT**, **PPTX**, **JPG**,
 and **PNG** documents with one line of code!
 <br></br>
 See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
 of the features in the library.
 
 ### Document Parsing
```

#### html2text {}

```diff
@@ -8,14 +8,24 @@
     /img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg) ![https://
  GitHub.com/unstructured-io/unstructured.js/releases](https://img.shields.io/
   github/release/unstructured-io/unstructured) ![https://github.com/Naereen/
 badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)
      [https://img.shields.io/badge/JOIN_US_ON_SLACK-4A154B?style=for-the-
    badge&logo=slack&logoColor=white] [https://img.shields.io/badge/LinkedIn-
            0077B5?style=for-the-badge&logo=linkedin&logoColor=white]
+                          ***** Announcement!!! *****
+We're excited to announce the public release of the unstructured.io hosted API!
+ Now you can leverage Unstructured with a simple API call to render clean text
+     in JSON format out of your images, documents, powerpoints, and more.
+ Checkout the readme here to get started making API calls. Youâll also find
+instructions there about how to host your own version of the API. Unstructured
+data just got easier! We'd love to hear your feedback, let us know how it goes
+  in our community_slack. And stay tuned for improvements to both quality and
+                      performance over the coming months!
+                                  [easy.gif]
        **** Open-Source Pre-Processing Tools for Unstructured Data ****
 The `unstructured` library provides open-source components for pre-processing
 text documents such as **PDFs**, **HTML** and **Word** Documents. These
 components are packaged as *bricks* ð§±, which provide users the building
 blocks they need to build pipelines targeted at the documents they care about.
 Bricks in the library fall into three categories: - :jigsaw: ***Partitioning
 bricks*** that break raw documents down into standard, structured elements. - :
@@ -30,19 +40,19 @@
 Install the following system dependencies if they are not already available on
 your system. Depending on what document types you're parsing, you may not need
 all of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
 - If you are parsing PDFs, run the following to install the `detectron2` model,
 which `unstructured` uses for layout detection: - `pip install
 "detectron2@git+https://github.com/facebookresearch/
-detectron2.git@v0.6#egg=detectron2"` At this point, you should be able to run
-the following code: ```python from unstructured.partition.auto import partition
-elements = partition(filename="example-docs/fake-email.eml") print("\n\n".join(
-[str(el) for el in elements])) ``` And if you installed with `local-inference`,
-you should be able to run this as well: ```python from
+detectron2.git@e2ce8dc#egg=detectron2"` At this point, you should be able to
+run the following code: ```python from unstructured.partition.auto import
+partition elements = partition(filename="example-docs/fake-email.eml") print
+("\n\n".join([str(el) for el in elements])) ``` And if you installed with
+`local-inference`, you should be able to run this as well: ```python from
 unstructured.partition.auto import partition elements = partition("example-
 docs/layout-parser-paper.pdf") print("\n\n".join([str(el) for el in elements]))
 ``` ## :dizzy: Instructions for using the docker image The following
 instructions are intended to help you get up and running using Docker to
 interact with `unstructured`. See [here](https://docs.docker.com/get-docker/
 ) if you don't already have docker installed on your machine. NOTE: we build
 multi-platform images to support both x86_64 and Apple silicon hardware.
@@ -94,16 +104,16 @@
 `pre-commit`, you'll just need to install the hooks with `pre-commit install`
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
 show how to get started with the `unstructured` library. You can parse **TXT**,
-**HTML**, **PDF**, **EML**, **MSG**, **EPUB**, **DOC**, **DOCX**, **PPT**,
-**PPTX**, **JPG**, and **PNG** documents with one line of code!
+**HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
+**PPT**, **PPTX**, **JPG**, and **PNG** documents with one line of code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
```

### Comparing `unstructured-0.5.9/setup.py` & `unstructured-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,25 +72,29 @@
             "langdetect",
             "sacremoses",
             "sentencepiece",
             "torch",
             "transformers",
         ],
         "local-inference": [
-            # NOTE(robinson) - Upper bound is temporary due to a multithreading issue
-            "unstructured-inference~=0.2.4",
+            "unstructured-inference>=0.4.2",
         ],
         "s3": ["s3fs", "fsspec"],
         "azure": ["adlfs", "fsspec"],
         "github": [
             # NOTE - pygithub==1.58.0 fails due to https://github.com/PyGithub/PyGithub/issues/2436
             # In the future, we can update this to pygithub>1.58.0
             "pygithub==1.57.0",
         ],
         "gitlab": ["python-gitlab"],
         "reddit": ["praw"],
+        "slack": ["slack_sdk"],
         "wikipedia": ["wikipedia"],
-        "google-drive": ["google-api-python-client"],
+        "google-drive": [
+            "google-api-python-client",
+            # consistency with local-inference-pin
+            "protobuf<3.21",
+        ],
     },
     package_dir={"unstructured": "unstructured"},
     package_data={"unstructured": ["nlp/*.txt"]},
 )
```

### Comparing `unstructured-0.5.9/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.6.0/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.6.0/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/test_unstructured/test_utils.py` & `unstructured-0.6.0/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/cleaners/core.py` & `unstructured-0.6.0/unstructured/cleaners/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import quopri
 import re
 import sys
 import unicodedata
 
-from unstructured.nlp.patterns import UNICODE_BULLETS_RE
+from unstructured.nlp.patterns import (
+    DOUBLE_PARAGRAPH_PATTERN_RE,
+    PARAGRAPH_PATTERN,
+    PARAGRAPH_PATTERN_RE,
+    UNICODE_BULLETS_RE,
+)
 
 
 def clean_non_ascii_chars(text) -> str:
     """Cleans non-ascii characters from unicode string.
 
     Example
     -------
@@ -53,14 +58,57 @@
 
     if len(bullet[0]) > 2:
         return text
 
     return text_cl
 
 
+def group_broken_paragraphs(
+    text: str,
+    line_split: re.Pattern = PARAGRAPH_PATTERN_RE,
+    paragraph_split: re.Pattern = DOUBLE_PARAGRAPH_PATTERN_RE,
+) -> str:
+    """Groups paragraphs that have line breaks for visual/formatting purposes.
+    For example:
+
+    '''The big red fox
+    is walking down the lane.
+
+    At the end of the lane
+    the fox met a bear.'''
+
+    Gets converted to
+
+    '''The big red fox is walking down the lane.
+    At the end of the land the fox met a bear.'''
+    """
+    paragraphs = paragraph_split.split(text)
+    clean_paragraphs = []
+    for paragraph in paragraphs:
+        if not paragraph.strip():
+            continue
+
+        # NOTE(robinson) - This block is to account for lines like the following that shouldn't be
+        # grouped together, but aren't separated by a double line break.
+        #     Apache License
+        #     Version 2.0, January 2004
+        #     http://www.apache.org/licenses/
+        para_split = line_split.split(paragraph)
+        all_lines_short = all(len(line.strip().split(" ")) < 5 for line in para_split)
+
+        if UNICODE_BULLETS_RE.match(paragraph.strip()):
+            clean_paragraphs.extend(re.split(PARAGRAPH_PATTERN, paragraph))
+        elif all_lines_short:
+            clean_paragraphs.extend([line for line in para_split if line.strip()])
+        else:
+            clean_paragraphs.append(re.sub(PARAGRAPH_PATTERN, " ", paragraph))
+
+    return "\n\n".join(clean_paragraphs)
+
+
 # TODO(robinson) - There's likely a cleaner was to accomplish this and get all of the
 # unicode characters instead of just the quotes. Doing this for now since quotes are
 # an issue that are popping up in the SEC filings tests
 def replace_unicode_quotes(text) -> str:
     """Replaces unicode bullets in text with the expected character
 
     Example
@@ -135,22 +183,22 @@
     Example
     -------
     ITEM 1.     BUSINESS. -> ITEM 1.     BUSINESS
     """
     return text.strip().rstrip(".,:;")
 
 
-def replace_mime_encodings(text: str) -> str:
-    """Replaces MIME encodings with their UTF-8 equivalent characters.
+def replace_mime_encodings(text: str, encoding: str = "utf-8") -> str:
+    """Replaces MIME encodings with their equivalent characters in the specified encoding.
 
     Example
     -------
     5 w=E2=80-99s -> 5 w’s
     """
-    return quopri.decodestring(text.encode()).decode("utf-8")
+    return quopri.decodestring(text.encode()).decode(encoding)
 
 
 def clean_prefix(text: str, pattern: str, ignore_case: bool = False, strip: bool = True) -> str:
     """Removes prefixes from a string according to the specified pattern. Strips leading
     whitespace if the strip parameter is set to True.
 
     Input
@@ -206,7 +254,14 @@
     cleaned_text = (
         clean_trailing_punctuation(cleaned_text) if trailing_punctuation else cleaned_text
     )
     cleaned_text = clean_dashes(cleaned_text) if dashes else cleaned_text
     cleaned_text = clean_extra_whitespace(cleaned_text) if extra_whitespace else cleaned_text
     cleaned_text = clean_bullets(cleaned_text) if bullets else cleaned_text
     return cleaned_text.strip()
+
+
+def bytes_string_to_string(text: str, encoding: str = "utf-8"):
+    """Converts a string representation of a byte string to a regular string using the
+    specified encoding."""
+    text_bytes = bytes([ord(char) for char in text])
+    return text_bytes.decode(encoding)
```

### Comparing `unstructured-0.5.9/unstructured/cleaners/extract.py` & `unstructured-0.6.0/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/cleaners/translate.py` & `unstructured-0.6.0/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/documents/base.py` & `unstructured-0.6.0/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/documents/elements.py` & `unstructured-0.6.0/unstructured/documents/elements.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 import hashlib
 import pathlib
 from abc import ABC
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 
 class NoID(ABC):
     """Class to indicate that an element do not have an ID."""
 
     pass
 
 
 @dataclass
 class ElementMetadata:
     filename: Optional[str] = None
+    date: Optional[str] = None
+
+    # Page numbers currenlty supported for PDF, HTML and PPT documents
     page_number: Optional[int] = None
+
+    # Webpage specific metadata fields
     url: Optional[str] = None
 
+    # E-mail specific metadata fields
+    sent_from: Optional[List[str]] = None
+    sent_to: Optional[List[str]] = None
+    subject: Optional[str] = None
+
+    # Text format metadata fields
+    text_as_html: Optional[str] = None
+
     def __post_init__(self):
         if isinstance(self.filename, pathlib.Path):
             self.filename = str(self.filename)
 
     def to_dict(self):
         return {key: value for key, value in self.__dict__.items() if value is not None}
 
@@ -31,19 +44,19 @@
 
 class Element(ABC):
     """An element is a section of a page in the document."""
 
     def __init__(
         self,
         element_id: Union[str, NoID] = NoID(),
-        coordinates: Optional[List[float]] = None,
+        coordinates: Optional[Tuple[Tuple[float, float], ...]] = None,
         metadata: ElementMetadata = ElementMetadata(),
     ):
         self.id: Union[str, NoID] = element_id
-        self.coordinates: Optional[List[float]] = coordinates
+        self.coordinates: Optional[Tuple[Tuple[float, float], ...]] = coordinates
         self.metadata = metadata
 
     def to_dict(self) -> dict:
         return {
             "type": None,
             "coordinates": self.coordinates,
             "element_id": self.id,
@@ -54,20 +67,20 @@
 class CheckBox(Element):
     """A checkbox with an attribute indicating whether its checked or not. Primarily used
     in documents that are forms"""
 
     def __init__(
         self,
         element_id: Union[str, NoID] = NoID(),
-        coordinates: Optional[List[float]] = None,
+        coordinates: Optional[Tuple[Tuple[float, float], ...]] = None,
         checked: bool = False,
         metadata: ElementMetadata = ElementMetadata(),
     ):
         self.id: Union[str, NoID] = element_id
-        self.coordinates: Optional[List[float]] = coordinates
+        self.coordinates: Optional[Tuple[Tuple[float, float], ...]] = coordinates
         self.checked: bool = checked
         self.metadata = metadata
 
     def __eq__(self, other):
         return (self.checked == other.checked) and (self.coordinates) == (other.coordinates)
 
     def to_dict(self) -> dict:
@@ -85,15 +98,15 @@
 
     category = "UncategorizedText"
 
     def __init__(
         self,
         text: str,
         element_id: Union[str, NoID] = NoID(),
-        coordinates: Optional[List[float]] = None,
+        coordinates: Optional[Tuple[Tuple[float, float], ...]] = None,
         metadata: ElementMetadata = ElementMetadata(),
     ):
         self.text: str = text
 
         if isinstance(element_id, NoID):
             # NOTE(robinson) - Cut the SHA256 hex in half to get the first 128 bits
             element_id = hashlib.sha256(text.encode()).hexdigest()[:32]
@@ -194,20 +207,29 @@
         element_id: Union[str, NoID] = NoID(),
         coordinates: Optional[List[float]] = None,
         metadata: ElementMetadata = ElementMetadata(),
     ):
         super().__init__(text="<PAGE BREAK>")
 
 
+class Table(Text):
+    """An element for capturing tables."""
+
+    category = "Table"
+
+    pass
+
+
 TYPE_TO_TEXT_ELEMENT_MAP: Dict[str, Any] = {
     "UncategorizedText": Text,
     "FigureCaption": FigureCaption,
     "Figure": FigureCaption,
     "Text": NarrativeText,
     "NarrativeText": NarrativeText,
     "ListItem": ListItem,
     "BulletedText": ListItem,
     "Title": Title,
     "Address": Address,
     "Image": Image,
     "PageBreak": PageBreak,
+    "Table": Table,
 }
```

### Comparing `unstructured-0.5.9/unstructured/documents/email_elements.py` & `unstructured-0.6.0/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/documents/html.py` & `unstructured-0.6.0/unstructured/documents/html.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
     return True
 
 
 def _has_adjacent_bulleted_spans(tag_elem: etree.Element, children: List[etree.Element]) -> bool:
     """Checks to see if a div contains two or more adjacent spans beginning with a bullet. If
     this is the case, it is treated as a single bulleted text element."""
     if tag_elem.tag == "div":
-        all_spans = all([child.tag == "span" for child in children])
+        all_spans = all(child.tag == "span" for child in children)
         _is_bulleted = children[0].text is not None and is_bulleted_text(children[0].text)
         if all_spans and _is_bulleted:
             return True
     return False
 
 
 def has_table_ancestor(element: TagsMixin) -> bool:
```

### Comparing `unstructured-0.5.9/unstructured/documents/xml.py` & `unstructured-0.6.0/unstructured/documents/xml.py`

 * *Files 15% similar despite different names*

```diff
@@ -50,16 +50,32 @@
         """Gets all elements from pages in sequential order."""
         if self._pages is None:
             self._pages = self._read()
         return super().pages
 
     def _read_xml(self, content):
         """Reads in an XML file and converts it to an lxml element tree object."""
+        # NOTE(robinson) - without the carriage return at the beginning, you get
+        # output that looks like the following when you run partition_pdf
+        #   'h   3       a   l   i   g   n   =   "   c   e   n   t   e   r   "   >'
+        # The correct output is returned once you add the initial return.
+        is_html_parser = isinstance(self.parser, etree.HTMLParser)
+        if content and not content.startswith("\n") and is_html_parser:
+            content = "\n" + content
         if self.document_tree is None:
-            document_tree = etree.fromstring(content.encode(), self.parser)
+            try:
+                document_tree = etree.fromstring(content, self.parser)
+                if document_tree is None:
+                    raise ValueError("document_tree is None")
+            # NOTE(robinson) - The following ValueError occurs with unicode strings. In that
+            # case, we call back to encoding the string and passing in bytes.
+            #     ValueError: Unicode strings with encoding declaration are not supported.
+            #     Please use  bytes input or XML fragments without declaration.
+            except ValueError:
+                document_tree = etree.fromstring(content.encode(), self.parser)
 
             if self.stylesheet:
                 if isinstance(self.parser, etree.HTMLParser):
                     logger.warning(
                         "You are using the HTML parser with an XSLT stylesheet. "
                         "Stylesheets are more commonly parsed with the "
                         "XMLParser. If your HTML does not display properly, try "
```

### Comparing `unstructured-0.5.9/unstructured/file_utils/exploration.py` & `unstructured-0.6.0/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/file_utils/file_conversion.py` & `unstructured-0.6.0/unstructured/file_utils/file_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,32 +18,33 @@
             f"{err}"
         )
         raise FileNotFoundError(msg)
 
     return text
 
 
-def convert_epub_to_html(
+def convert_file_to_html_text(
+    source_format: str,
     filename: Optional[str] = None,
     file: Optional[IO] = None,
 ) -> str:
-    """Converts an EPUB document to HTML raw text. Enables an EPUB doucment to be
+    """Converts a document to HTML raw text. Enables the doucment to be
     processed using the partition_html function."""
     exactly_one(filename=filename, file=file)
 
     if file is not None:
         tmp = tempfile.NamedTemporaryFile(delete=False)
         tmp.write(file.read())
         tmp.close()
         html_text = convert_file_to_text(
             filename=tmp.name,
-            source_format="epub",
+            source_format=source_format,
             target_format="html",
         )
     elif filename is not None:
         html_text = convert_file_to_text(
             filename=filename,
-            source_format="epub",
+            source_format=source_format,
             target_format="html",
         )
 
     return html_text
```

### Comparing `unstructured-0.5.9/unstructured/file_utils/filetype.py` & `unstructured-0.6.0/unstructured/file_utils/filetype.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     def __lt__(self, other):
         return self.name < other.name
 
 
 STR_TO_FILETYPE = {
     "application/pdf": FileType.PDF,
     "application/msword": FileType.DOC,
+    "application/vnd.openxmlformats-officedocument.wordprocessingml.document": FileType.DOCX,
     "image/jpeg": FileType.JPG,
     "image/png": FileType.PNG,
     "text/markdown": FileType.MD,
     "text/x-markdown": FileType.MD,
     "application/epub": FileType.EPUB,
     "application/epub+zip": FileType.EPUB,
     "text/html": FileType.HTML,
@@ -173,20 +174,25 @@
 
     if content_type:
         filetype = STR_TO_FILETYPE.get(content_type)
         if filetype:
             return filetype
 
     if filename or file_filename:
-        _, extension = os.path.splitext(filename or file_filename or "")
+        _filename = filename or file_filename or ""
+        _, extension = os.path.splitext(_filename)
         extension = extension.lower()
-        if LIBMAGIC_AVAILABLE:
+        if os.path.isfile(_filename) and LIBMAGIC_AVAILABLE:
             mime_type = magic.from_file(filename or file_filename, mime=True)  # type: ignore
+            # NOTE(crag): for older versions of the OS libmagic package, such as is currently
+            # installed on the Unstructured docker image, .json files resolve to "text/plain"
+            # rather than "application/json". this corrects for that case.
+            if mime_type == "text/plain" and extension == ".json":
+                return FileType.JSON
         else:
-            # might not need this
             return EXT_TO_FILETYPE.get(extension.lower(), FileType.UNK)
     elif file is not None:
         extension = None
         # NOTE(robinson) - the python-magic docs recommend reading at least the first 2048 bytes
         # Increased to 4096 because otherwise .xlsx files get detected as a zip file
         # ref: https://github.com/ahupp/python-magic#usage
         if LIBMAGIC_AVAILABLE:
@@ -224,19 +230,27 @@
     elif mime_type in MD_MIME_TYPES:
         # NOTE - I am not sure whether libmagic ever returns these mimetypes.
         return FileType.MD
 
     elif mime_type in EPUB_MIME_TYPES:
         return FileType.EPUB
 
+    # NOTE(robinson) - examples are application/rtf or text/rtf.
+    # magic often returns text/plain for RTF files
+    elif mime_type.endswith("rtf"):
+        return FileType.RTF
+
     elif mime_type in TXT_MIME_TYPES:
         if extension and extension == ".eml":
             return FileType.EML
-        if extension and extension == ".md":
+        elif extension and extension == ".md":
             return FileType.MD
+        elif extension and extension == ".rtf":
+            return FileType.RTF
+
         if file and not extension and _check_eml_from_buffer(file=file) is True:
             return FileType.EML
         return FileType.TXT
 
     elif mime_type.endswith("xml"):
         if extension and extension == ".html":
             return FileType.HTML
@@ -292,19 +306,19 @@
     """Detects the filetype, given a file with an application/octet-stream MIME type."""
     file.seek(0)
     if zipfile.is_zipfile(file):
         file.seek(0)
         archive = zipfile.ZipFile(file)
 
         archive_filenames = [f.filename for f in archive.filelist]
-        if all([f in archive_filenames for f in EXPECTED_DOCX_FILES]):
+        if all(f in archive_filenames for f in EXPECTED_DOCX_FILES):
             return FileType.DOCX
-        elif all([f in archive_filenames for f in EXPECTED_XLSX_FILES]):
+        elif all(f in archive_filenames for f in EXPECTED_XLSX_FILES):
             return FileType.XLSX
-        elif all([f in archive_filenames for f in EXPECTED_PPTX_FILES]):
+        elif all(f in archive_filenames for f in EXPECTED_PPTX_FILES):
             return FileType.PPTX
 
     logger.warning("Could not detect the filetype from application/octet-stream MIME type.")
     return FileType.UNK
 
 
 def _check_eml_from_buffer(file: IO) -> bool:
```

### Comparing `unstructured-0.5.9/unstructured/file_utils/metadata.py` & `unstructured-0.6.0/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/ingest/connector/azure.py` & `unstructured-0.6.0/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/ingest/connector/biomed.py` & `unstructured-0.6.0/unstructured/ingest/connector/biomed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import json
 import os
 import urllib.request
 from dataclasses import dataclass
-from datetime import datetime
 from ftplib import FTP, error_perm
 from pathlib import Path
 from typing import List, Optional, Union
 
 import requests
 from bs4 import BeautifulSoup
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
 )
 from unstructured.ingest.logger import logger
+from unstructured.utils import (
+    validate_date_args,
+)
 
 DOMAIN = "ftp.ncbi.nlm.nih.gov"
 FTP_DOMAIN = f"ftp://{DOMAIN}"
 PMC_DIR = "pub/pmc"
 PDF_DIR = "oa_pdf"
 
 
@@ -43,50 +45,31 @@
     until: str
 
     # Standard Connector options
     download_dir: str
     # where to write structured data, with the directory structure matching FTP path
     output_dir: str
     re_download: bool = False
+    download_only: bool = False
     preserve_downloads: bool = False
     metadata_include: Optional[str] = None
     metadata_exclude: Optional[str] = None
+    partition_by_api: bool = False
+    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
     fields_include: str = "element_id,text,type,metadata"
     flatten_metadata: bool = False
 
-    def _validate_date_args(self, date):
-        date_formats = ["%Y-%m-%d", "%Y-%m-%d+%H:%M:%S"]
-
-        valid = False
-        if date:
-            date = date.replace(" ", "+").replace("%20", "+")
-            for format in date_formats:
-                try:
-                    datetime.strptime(date, format)
-                    valid = True
-                    break
-                except ValueError:
-                    pass
-
-            if not valid:
-                raise ValueError(
-                    f"The from argument {date} does not satisfy the format: "
-                    "YYYY-MM-DD or YYYY-MM-DD HH:MM:SS",
-                )
-
-        return valid
-
     def validate_api_inputs(self):
         valid = False
 
         if self.from_:
-            valid = self._validate_date_args(self.from_)
+            valid = validate_date_args(self.from_)
 
         if self.until:
-            valid = self._validate_date_args(self.until)
+            valid = validate_date_args(self.until)
 
         return valid
 
     def __post_init__(self):
         self.is_file = False
         self.is_dir = False
         self.is_api = False
@@ -138,15 +121,19 @@
     def filename(self):
         return Path(self.file_meta.download_filepath).resolve()  # type: ignore
 
     def _output_filename(self):
         return Path(f"{self.file_meta.output_filepath}.json").resolve()
 
     def cleanup_file(self):
-        if not self.config.preserve_downloads and self.filename.is_file():
+        if (
+            not self.config.preserve_downloads
+            and self.filename.is_file()
+            and not self.config.download_only
+        ):
             logger.debug(f"Cleaning up {self}")
             Path.unlink(self.filename)
 
     def has_output(self):
         """Determine if structured output for this doc already exists."""
         output_filename = self._output_filename()
         return output_filename.is_file() and output_filename.stat()
@@ -166,27 +153,29 @@
             self.file_meta.download_filepath,
         )
 
         logger.debug(f"File downloaded: {self.file_meta.download_filepath}")
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
+        if self.config.download_only:
+            return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w") as output_f:
             output_f.write(json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2))
         logger.info(f"Wrote {output_filename}")
 
 
 class BiomedConnector(BaseConnector):
     """Objects of this class support fetching documents from Biomedical literature FTP directory"""
 
     def __init__(self, config):
         self.config = config
-        self.cleanup_files = not self.config.preserve_downloads
+        self.cleanup_files = not self.config.preserve_downloads and not self.config.download_only
 
     def _list_objects_api(self):
         def urls_to_metadata(urls):
             files = []
             for url in urls:
                 parts = url.split(PDF_DIR)
                 if len(parts) > 1:
```

### Comparing `unstructured-0.5.9/unstructured/ingest/connector/fsspec.py` & `unstructured-0.6.0/unstructured/ingest/connector/fsspec.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,19 @@
     path: str
 
     # base connector options
     download_dir: str
     output_dir: str
     preserve_downloads: bool = False
     re_download: bool = False
+    download_only: bool = False
     metadata_include: Optional[str] = None
     metadata_exclude: Optional[str] = None
+    partition_by_api: bool = False
+    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
     fields_include: str = "element_id,text,type,metadata"
     flatten_metadata: bool = False
 
     # fsspec specific options
     access_kwargs: dict = field(default_factory=dict)
 
     protocol: str = field(init=False)
@@ -117,28 +120,30 @@
         )
 
         logger.debug(f"Fetching {self} - PID: {os.getpid()}")
         fs.get(rpath=self.remote_file_path, lpath=self._tmp_download_file().as_posix())
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
+        if self.config.download_only:
+            return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w") as output_f:
             output_f.write(json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2))
         logger.info(f"Wrote {output_filename}")
 
     @property
     def filename(self):
         """The filename of the file after downloading from s3"""
         return self._tmp_download_file()
 
     def cleanup_file(self):
-        """Removes the local copy the file after successful processing."""
-        if not self.config.preserve_downloads:
+        """Removes the local copy of the file after successful processing."""
+        if not self.config.preserve_downloads and not self.config.download_only:
             logger.debug(f"Cleaning up {self}")
             os.unlink(self._tmp_download_file())
 
 
 class FsspecConnector(BaseConnector):
     """Objects of this class support fetching document(s) from"""
 
@@ -150,15 +155,15 @@
     ):
         from fsspec import AbstractFileSystem, get_filesystem_class
 
         self.config = config
         self.fs: AbstractFileSystem = get_filesystem_class(self.config.protocol)(
             **self.config.access_kwargs,
         )
-        self.cleanup_files = not config.preserve_downloads
+        self.cleanup_files = not config.preserve_downloads and not config.download_only
 
     def cleanup(self, cur_dir=None):
         """cleanup linginering empty sub-dirs from s3 paths, but leave remaining files
         (and their paths) in tact as that indicates they were not processed"""
         if not self.cleanup_files:
             return
```

### Comparing `unstructured-0.5.9/unstructured/ingest/connector/git.py` & `unstructured-0.6.0/unstructured/ingest/connector/git.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,19 @@
 
     # Standard Connector options
     download_dir: str
     # where to write structured data, with the directory structure matching the github repository
     output_dir: str
     preserve_downloads: bool = False
     re_download: bool = False
+    download_only: bool = False
     metadata_include: Optional[str] = None
     metadata_exclude: Optional[str] = None
+    partition_by_api: bool = False
+    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
     fields_include: str = "element_id,text,type,metadata"
     flatten_metadata: bool = False
 
     repo_path: str = field(init=False, repr=False)
 
 
 @dataclass
@@ -47,16 +50,16 @@
         return Path(self.config.output_dir) / f"{self.path}.json"
 
     def _create_full_tmp_dir_path(self):
         """includes directories in in the gitlab repository"""
         self.filename.parent.mkdir(parents=True, exist_ok=True)
 
     def cleanup_file(self):
-        """Removes the local copy the file (or anything else) after successful processing."""
-        if not self.config.preserve_downloads:
+        """Removes the local copy of the file (or anything else) after successful processing."""
+        if not self.config.preserve_downloads and not self.config.download_only:
             logger.debug(f"Cleaning up {self}")
             os.unlink(self.filename)
 
     def get_file(self):
         """Fetches the "remote" doc and stores it locally on the filesystem."""
         self._create_full_tmp_dir_path()
         if not self.config.re_download and self.filename.is_file() and self.filename.stat():
@@ -72,27 +75,29 @@
     def has_output(self):
         """Determine if structured output for this doc already exists."""
         output_filename = self._output_filename()
         return output_filename.is_file() and output_filename.stat()
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
+        if self.config.download_only:
+            return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w", encoding="utf8") as output_f:
             json.dump(self.isd_elems_no_filename, output_f, ensure_ascii=False, indent=2)
         logger.info(f"Wrote {output_filename}")
 
 
 @dataclass
 class GitConnector(BaseConnector):
     config: SimpleGitConfig
 
     def __post_init__(self) -> None:
-        self.cleanup_files = not self.config.preserve_downloads
+        self.cleanup_files = not self.config.preserve_downloads and not self.config.download_only
 
     def cleanup(self, cur_dir=None):
         if not self.cleanup_files:
             return
 
         if cur_dir is None:
             cur_dir = self.config.download_dir
```

### Comparing `unstructured-0.5.9/unstructured/ingest/connector/github.py` & `unstructured-0.6.0/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/ingest/connector/gitlab.py` & `unstructured-0.6.0/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/ingest/connector/google_drive.py` & `unstructured-0.6.0/unstructured/ingest/connector/google_drive.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,17 +72,20 @@
     extension: str
 
     # Standard Connector options
     download_dir: str
     # where to write structured data, with the directory structure matching drive path
     output_dir: str
     re_download: bool = False
+    download_only: bool = False
     preserve_downloads: bool = False
     metadata_include: Optional[str] = None
     metadata_exclude: Optional[str] = None
+    partition_by_api: bool = False
+    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
     fields_include: str = "element_id,text,type,metadata"
     flatten_metadata: bool = False
 
     recursive: bool = False
 
     def __post_init__(self):
         if self.extension and self.extension not in EXT_TO_FILETYPE.keys():
@@ -102,15 +105,19 @@
     def filename(self):
         return Path(self.file_meta.get("download_filepath")).resolve()  # type: ignore
 
     def _output_filename(self):
         return Path(f"{self.file_meta.get('output_filepath')}.json").resolve()
 
     def cleanup_file(self):
-        if not self.config.preserve_downloads and self.filename.is_file():
+        if (
+            not self.config.preserve_downloads
+            and self.filename.is_file()
+            and not self.config.download_only
+        ):
             logger.debug(f"Cleaning up {self}")
             Path.unlink(self.filename)
 
     def has_output(self):
         """Determine if structured output for this doc already exists."""
         output_filename = self._output_filename()
         return output_filename.is_file() and output_filename.stat()
@@ -170,27 +177,29 @@
                     logger.debug(f"File downloaded: {self.filename}.")
 
         if not saved:
             logger.error(f"Error while downloading and saving file: {self.filename}.")
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
+        if self.config.download_only:
+            return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w") as output_f:
             output_f.write(json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2))
         logger.info(f"Wrote {output_filename}")
 
 
 class GoogleDriveConnector(BaseConnector):
     """Objects of this class support fetching documents from Google Drive"""
 
     def __init__(self, config):
         self.config = config
-        self.cleanup_files = not self.config.preserve_downloads
+        self.cleanup_files = not self.config.preserve_downloads and not self.config.download_only
 
     def _list_objects(self, drive_id, recursive=False):
         files = []
 
         def traverse(drive_id, download_dir, output_dir, recursive=False):
             page_token = None
             while True:
```

### Comparing `unstructured-0.5.9/unstructured/ingest/connector/local.py` & `unstructured-0.6.0/unstructured/ingest/connector/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,21 @@
 
     # Local specific options
     input_path: str
     recursive: bool = False
     file_glob: Optional[str] = None
 
     # base connector options
+    download_only: bool = False
     metadata_include: Optional[str] = None
     metadata_exclude: Optional[str] = None
+    partition_by_api: bool = False
+    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
     fields_include: str = "element_id,text,type,metadata"
+    flatten_metadata: bool = False
 
     def __post_init__(self):
         if os.path.isfile(self.input_path):
             self.input_path_is_file = True
         else:
             self.input_path_is_file = False
 
@@ -65,14 +69,16 @@
 
     def has_output(self):
         """Determine if structured output for this doc already exists."""
         return self._output_filename().is_file() and os.path.getsize(self._output_filename())
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
+        if self.config.download_only:
+            return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w") as output_f:
             output_f.write(json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2))
         logger.info(f"Wrote {output_filename}")
```

### Comparing `unstructured-0.5.9/unstructured/ingest/connector/reddit.py` & `unstructured-0.6.0/unstructured/ingest/connector/reddit.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,19 @@
 
     # Standard Connector options
     download_dir: str
     # where to write structured data
     output_dir: str
     preserve_downloads: bool = False
     re_download: bool = False
+    download_only: bool = False
     metadata_include: Optional[str] = None
     metadata_exclude: Optional[str] = None
+    partition_by_api: bool = False
+    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
     fields_include: str = "element_id,text,type,metadata"
     flatten_metadata: bool = False
 
     def __post_init__(self):
         if self.num_posts <= 0:
             raise ValueError("The number of Reddit posts to fetch must be positive.")
 
@@ -53,16 +56,16 @@
     def _output_filename(self):
         return Path(self.config.output_dir) / f"{self.post.id}.json"
 
     def _create_full_tmp_dir_path(self):
         self.filename.parent.mkdir(parents=True, exist_ok=True)
 
     def cleanup_file(self):
-        """Removes the local copy the file (or anything else) after successful processing."""
-        if not self.config.preserve_downloads:
+        """Removes the local copy of the file (or anything else) after successful processing."""
+        if not self.config.preserve_downloads and not self.config.download_only:
             logger.debug(f"Cleaning up {self}")
             os.unlink(self.filename)
 
     def get_file(self):
         """Fetches the "remote" doc and stores it locally on the filesystem."""
         self._create_full_tmp_dir_path()
         if not self.config.re_download and self.filename.is_file() and self.filename.stat():
@@ -78,14 +81,16 @@
     def has_output(self):
         """Determine if structured output for this doc already exists."""
         output_filename = self._output_filename()
         return output_filename.is_file() and output_filename.stat()
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
+        if self.config.download_only:
+            return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w", encoding="utf8") as output_f:
             json.dump(self.isd_elems_no_filename, output_f, ensure_ascii=False, indent=2)
         logger.info(f"Wrote {output_filename}")
 
 
@@ -96,15 +101,15 @@
 
         self.config = config
         self.reddit = Reddit(
             client_id=config.client_id,
             client_secret=config.client_secret,
             user_agent=config.user_agent,
         )
-        self.cleanup_files = not config.preserve_downloads
+        self.cleanup_files = not config.preserve_downloads and not config.download_only
 
     def cleanup(self, cur_dir=None):
         if not self.cleanup_files:
             return
 
         if cur_dir is None:
             cur_dir = self.config.download_dir
```

### Comparing `unstructured-0.5.9/unstructured/ingest/connector/s3.py` & `unstructured-0.6.0/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.6.0/unstructured/ingest/connector/wikipedia.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,19 @@
 
     # Standard Connector options
     download_dir: str
     # where to write structured data
     output_dir: str
     preserve_downloads: bool = False
     re_download: bool = False
+    download_only: bool = False
     metadata_include: Optional[str] = None
     metadata_exclude: Optional[str] = None
+    partition_by_api: bool = False
+    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
     fields_include: str = "element_id,text,type,metadata"
     flatten_metadata: bool = False
 
 
 @dataclass
 class WikipediaIngestDoc(BaseIngestDoc):
     config: SimpleWikipediaConfig = field(repr=False)
@@ -48,16 +51,16 @@
     def _output_filename(self):
         raise NotImplementedError()
 
     def _create_full_tmp_dir_path(self):
         self.filename.parent.mkdir(parents=True, exist_ok=True)
 
     def cleanup_file(self):
-        """Removes the local copy the file (or anything else) after successful processing."""
-        if not self.config.preserve_downloads:
+        """Removes the local copy of the file (or anything else) after successful processing."""
+        if not self.config.preserve_downloads and not self.config.download_only:
             logger.debug(f"Cleaning up {self}")
             os.unlink(self.filename)
 
     def get_file(self):
         """Fetches the "remote" doc and stores it locally on the filesystem."""
         self._create_full_tmp_dir_path()
         if not self.config.re_download and self.filename.is_file() and self.filename.stat():
@@ -71,14 +74,16 @@
     def has_output(self):
         """Determine if structured output for this doc already exists."""
         output_filename = self._output_filename()
         return output_filename.is_file() and output_filename.stat()
 
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
+        if self.config.download_only:
+            return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w", encoding="utf8") as output_f:
             json.dump(self.isd_elems_no_filename, output_f, ensure_ascii=False, indent=2)
         logger.info(f"Wrote {output_filename}")
 
 
@@ -129,15 +134,15 @@
             Path(self.config.output_dir) / f"{self.page.title}-{self.page.revision_id}-summary.json"
         )
 
 
 class WikipediaConnector(BaseConnector):
     def __init__(self, config: SimpleWikipediaConfig):
         self.config = config
-        self.cleanup_files = not config.preserve_downloads
+        self.cleanup_files = not config.preserve_downloads and not config.download_only
 
     def cleanup(self, cur_dir=None):
         if not self.cleanup_files:
             return
 
         if cur_dir is None:
             cur_dir = self.config.download_dir
```

### Comparing `unstructured-0.5.9/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.6.0/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/ingest/interfaces.py` & `unstructured-0.6.0/unstructured/ingest/interfaces.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Defines Abstract Base Classes (ABC's) core to batch processing documents
 through Unstructured."""
 
 from abc import ABC, abstractmethod
 from typing import Optional
 
+import requests
+
 from unstructured.ingest.logger import logger
 from unstructured.partition.auto import partition
 from unstructured.staging.base import convert_to_dict
 
 
 class BaseConnector(ABC):
     """Abstract Base Class for a connector to a remote source, e.g. S3 or Google Drive."""
@@ -44,16 +46,19 @@
 
     # where raw documents are stored for processing, and then removed if not preserve_downloads
     download_dir: str
     preserve_downloads: bool = False
     # where to write structured data outputs
     output_dir: str
     re_download: bool = False
+    download_only: bool = False
     metadata_include: Optional[str] = None
     metadata_exclude: Optional[str] = None
+    partition_by_api: bool = False
+    partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
     fields_include: str = "element_id,text,type,metadata"
     flatten_metadata: bool = False
 
 
 class BaseIngestDoc(ABC):
     """An "ingest document" is specific to a connector, and provides
     methods to fetch a single raw document, store it locally for processing, any cleanup
@@ -88,19 +93,42 @@
         pass
 
     @abstractmethod
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
         pass
 
+    def partition_file(self):
+        if not self.config.partition_by_api:
+            logger.debug("Using local partition")
+            elements = partition(filename=str(self.filename))
+            return convert_to_dict(elements)
+
+        else:
+            endpoint = self.config.partition_endpoint
+
+            logger.debug(f"Using remote partition ({endpoint})")
+
+            with open(self.filename, "rb") as f:
+                response = requests.post(
+                    f"{endpoint}",
+                    files={"files": (str(self.filename), f)},
+                )
+
+            if response.status_code != 200:
+                raise RuntimeError(f"Caught {response.status_code} from API: {response.text}")
+
+            return response.json()
+
     def process_file(self):
+        if self.config.download_only:
+            return
         logger.info(f"Processing {self.filename}")
 
-        elements = partition(filename=str(self.filename))
-        isd_elems = convert_to_dict(elements)
+        isd_elems = self.partition_file()
 
         self.isd_elems_no_filename = []
         for elem in isd_elems:
             # type: ignore
             if (
                 self.config.metadata_exclude is not None
                 and self.config.metadata_include is not None
@@ -111,15 +139,15 @@
                 )
             elif self.config.metadata_exclude is not None:
                 ex_list = self.config.metadata_exclude.split(",")
                 for ex in ex_list:
                     elem["metadata"].pop(ex, None)  # type: ignore[attr-defined]
             elif self.config.metadata_include is not None:
                 in_list = self.config.metadata_include.split(",")
-                for k in elem["metadata"]:
+                for k in list(elem["metadata"].keys()):  # type: ignore[attr-defined]
                     if k not in in_list:
                         elem["metadata"].pop(k, None)  # type: ignore[attr-defined]
 
             in_list = self.config.fields_include.split(",")
             elem = {k: v for k, v in elem.items() if k in in_list}
 
             if self.config.flatten_metadata:
```

### Comparing `unstructured-0.5.9/unstructured/ingest/main.py` & `unstructured-0.6.0/unstructured/ingest/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,14 @@
 import warnings
 from contextlib import suppress
 from pathlib import Path
 from urllib.parse import urlparse
 
 import click
 
-from unstructured.ingest.connector.azure import (
-    AzureBlobStorageConnector,
-    SimpleAzureBlobStorageConfig,
-)
-from unstructured.ingest.connector.biomed import BiomedConnector, SimpleBiomedConfig
-from unstructured.ingest.connector.fsspec import FsspecConnector, SimpleFsspecConfig
-from unstructured.ingest.connector.github import GitHubConnector, SimpleGitHubConfig
-from unstructured.ingest.connector.gitlab import GitLabConnector, SimpleGitLabConfig
-from unstructured.ingest.connector.google_drive import (
-    GoogleDriveConnector,
-    SimpleGoogleDriveConfig,
-)
-from unstructured.ingest.connector.local import LocalConnector, SimpleLocalConfig
-from unstructured.ingest.connector.reddit import RedditConnector, SimpleRedditConfig
-from unstructured.ingest.connector.s3 import S3Connector, SimpleS3Config
 from unstructured.ingest.connector.wikipedia import (
     SimpleWikipediaConfig,
     WikipediaConnector,
 )
 from unstructured.ingest.doc_processor.generalized import initialize, process_document
 from unstructured.ingest.logger import ingest_log_streaming_init, logger
 
@@ -141,14 +126,27 @@
     "--metadata-exclude",
     default=None,
     help="If set, drop the specified metadata fields if they exist. "
     "Usage: provide a single string with comma separated values. "
     "Example: --metadata-exclude filename,page_number ",
 )
 @click.option(
+    "--partition-by-api",
+    is_flag=True,
+    default=False,
+    help="Use a remote API to partition the files."
+    " Otherwise, use the function from partition.auto",
+)
+@click.option(
+    "--partition-endpoint",
+    default="https://api.unstructured.io/general/v0/general",
+    help="If partitioning via api, use the following host. "
+    "Default: https://api.unstructured.io/general/v0/general",
+)
+@click.option(
     "--local-input-path",
     default=None,
     help="Path to the location in the local file system that will be processed.",
 )
 @click.option(
     "--local-recursive",
     is_flag=True,
@@ -312,14 +310,45 @@
 @click.option("--reddit-num-posts", default=10, help="The number of posts to fetch.")
 @click.option(
     "--re-download/--no-re-download",
     default=False,
     help="Re-download files even if they are already present in --download-dir.",
 )
 @click.option(
+    "--download-only",
+    is_flag=True,
+    default=False,
+    help="Download any files that are not already present in either --download-dir or "
+    "the default download ~/.cache/... location in case --download-dir is not specified and "
+    "skip processing them through unstructured.",
+)
+@click.option(
+    "--slack-channels",
+    default=None,
+    help="Comma separated list of Slack channel IDs to pull messages from, "
+    "can be a public or private channel",
+)
+@click.option(
+    "--slack-token",
+    default=None,
+    help="Bot token used to access Slack API, must have channels:history " "scope for the bot user",
+)
+@click.option(
+    "--start-date",
+    default=None,
+    help="Start date/time in formats YYYY-MM-DD or YYYY-MM-DDTHH:MM:SS or "
+    "YYYY-MM-DD+HH:MM:SS or YYYY-MM-DDTHH:MM:SStz",
+)
+@click.option(
+    "--end-date",
+    default=None,
+    help="End date/time in formats YYYY-MM-DD or YYYY-MM-DDTHH:MM:SS or "
+    "YYYY-MM-DD+HH:MM:SS or YYYY-MM-DDTHH:MM:SStz",
+)
+@click.option(
     "--download-dir",
     help="Where files are downloaded to, defaults to `$HOME/.cache/unstructured/ingest/<SHA256>`.",
 )
 @click.option(
     "--preserve-downloads",
     is_flag=True,
     default=False,
@@ -370,28 +399,35 @@
     subreddit_name,
     reddit_client_id,
     reddit_client_secret,
     reddit_user_agent,
     reddit_search_query,
     reddit_num_posts,
     re_download,
+    slack_channels,
+    slack_token,
+    start_date,
+    end_date,
     download_dir,
     preserve_downloads,
     structured_output_dir,
     reprocess,
     num_processes,
     verbose,
     metadata_include,
     metadata_exclude,
     fields_include,
     flatten_metadata,
     max_docs,
+    partition_by_api,
+    partition_endpoint,
     local_input_path,
     local_recursive,
     local_file_glob,
+    download_only,
 ):
     if flatten_metadata and "metadata" not in fields_include:
         logger.warning(
             "`--flatten-metadata` is specified, but there is no metadata to flatten, "
             "since `metadata` is not specified in `--fields-include`.",
         )
     if "metadata" not in fields_include and (metadata_include or metadata_exclude):
@@ -401,18 +437,31 @@
         )
     if metadata_exclude is not None and metadata_include is not None:
         logger.error(
             "Arguments `--metadata-include` and `--metadata-exclude` are "
             "mutually exclusive with each other.",
         )
         sys.exit(1)
-    if not preserve_downloads and download_dir:
+    if (
+        not partition_by_api
+        and partition_endpoint != "https://api.unstructured.io/general/v0/general"
+    ):
+        logger.warning(
+            "Ignoring --partition-endpoint because --partition-by-api was not set",
+        )
+    if (not preserve_downloads and not download_only) and download_dir:
         logger.warning(
             "Not preserving downloaded files but --download_dir is specified",
         )
+    if local_input_path is not None and download_dir:
+        logger.warning(
+            "Files should already be in local file system: there is nothing to download, "
+            "but --download-dir is specified.",
+        )
+        sys.exit(1)
     if local_input_path is None and not download_dir:
         cache_path = Path.home() / ".cache" / "unstructured" / "ingest"
         if not cache_path.exists():
             cache_path.mkdir(parents=True, exist_ok=True)
         if s3_url:
             warnings.warn(
                 "The `--s3-url` option will be deprecated in favor of `--remote-url`"
@@ -461,29 +510,39 @@
             logger.warning(
                 f"Preserving downloaded files but --download-dir is not specified,"
                 f" using {download_dir}",
             )
     if remote_url:
         protocol = urlparse(remote_url).scheme
         if protocol in ("s3", "s3a"):
+            from unstructured.ingest.connector.s3 import S3Connector, SimpleS3Config
+
             doc_connector = S3Connector(  # type: ignore
                 config=SimpleS3Config(
                     path=s3_url,
                     access_kwargs={"anon": s3_anonymous},
                     download_dir=download_dir,
                     output_dir=structured_output_dir,
                     re_download=re_download,
                     preserve_downloads=preserve_downloads,
                     metadata_include=metadata_include,
                     metadata_exclude=metadata_exclude,
+                    partition_by_api=partition_by_api,
+                    partition_endpoint=partition_endpoint,
                     fields_include=fields_include,
                     flatten_metadata=flatten_metadata,
+                    download_only=download_only,
                 ),
             )
         elif protocol in ("abfs", "az"):
+            from unstructured.ingest.connector.azure import (
+                AzureBlobStorageConnector,
+                SimpleAzureBlobStorageConfig,
+            )
+
             if azure_account_name:
                 access_kwargs = {
                     "account_name": azure_account_name,
                     "account_key": azure_account_key,
                 }
             elif azure_connection_string:
                 access_kwargs = {"connection_string": azure_connection_string}
@@ -495,75 +554,108 @@
                     access_kwargs=access_kwargs,
                     download_dir=download_dir,
                     output_dir=structured_output_dir,
                     re_download=re_download,
                     preserve_downloads=preserve_downloads,
                     metadata_include=metadata_include,
                     metadata_exclude=metadata_exclude,
+                    partition_by_api=partition_by_api,
+                    partition_endpoint=partition_endpoint,
                     fields_include=fields_include,
                     flatten_metadata=flatten_metadata,
+                    download_only=download_only,
                 ),
             )
         else:
             warnings.warn(
                 f"`fsspec` protocol {protocol} is not directly supported by `unstructured`,"
                 " so use it at your own risk. Supported protocols are `s3`, `s3a`, `abfs`,"
                 " and `az`.",
                 UserWarning,
             )
+
+            from unstructured.ingest.connector.fsspec import (
+                FsspecConnector,
+                SimpleFsspecConfig,
+            )
+
             doc_connector = FsspecConnector(  # type: ignore
                 config=SimpleFsspecConfig(
                     path=remote_url,
                     download_dir=download_dir,
                     output_dir=structured_output_dir,
                     re_download=re_download,
                     preserve_downloads=preserve_downloads,
                     metadata_include=metadata_include,
                     metadata_exclude=metadata_exclude,
+                    partition_by_api=partition_by_api,
+                    partition_endpoint=partition_endpoint,
                     fields_include=fields_include,
                     flatten_metadata=flatten_metadata,
+                    download_only=download_only,
                 ),
             )
     elif github_url:
+        from unstructured.ingest.connector.github import (
+            GitHubConnector,
+            SimpleGitHubConfig,
+        )
+
         doc_connector = GitHubConnector(  # type: ignore
             config=SimpleGitHubConfig(
                 url=github_url,
                 access_token=git_access_token,
                 branch=git_branch,
                 file_glob=git_file_glob,
                 # defaults params:
                 download_dir=download_dir,
                 preserve_downloads=preserve_downloads,
                 output_dir=structured_output_dir,
                 re_download=re_download,
                 metadata_include=metadata_include,
                 metadata_exclude=metadata_exclude,
+                partition_by_api=partition_by_api,
+                partition_endpoint=partition_endpoint,
                 fields_include=fields_include,
                 flatten_metadata=flatten_metadata,
+                download_only=download_only,
             ),
         )
     elif gitlab_url:
+        from unstructured.ingest.connector.gitlab import (
+            GitLabConnector,
+            SimpleGitLabConfig,
+        )
+
         doc_connector = GitLabConnector(  # type: ignore
             config=SimpleGitLabConfig(
                 url=gitlab_url,
                 access_token=git_access_token,
                 branch=git_branch,
                 file_glob=git_file_glob,
                 # defaults params:
                 download_dir=download_dir,
                 preserve_downloads=preserve_downloads,
                 output_dir=structured_output_dir,
                 re_download=re_download,
                 metadata_include=metadata_include,
                 metadata_exclude=metadata_exclude,
+                partition_by_api=partition_by_api,
+                partition_endpoint=partition_endpoint,
                 fields_include=fields_include,
                 flatten_metadata=flatten_metadata,
+                download_only=download_only,
             ),
         )
     elif subreddit_name:
+        from unstructured.ingest.connector.reddit import (
+            RedditConnector,
+            SimpleRedditConfig,
+        )
+
         doc_connector = RedditConnector(  # type: ignore
             config=SimpleRedditConfig(
                 subreddit_name=subreddit_name,
                 client_id=reddit_client_id,
                 client_secret=reddit_client_secret,
                 user_agent=reddit_user_agent,
                 search_query=reddit_search_query,
@@ -571,81 +663,131 @@
                 # defaults params:
                 download_dir=download_dir,
                 preserve_downloads=preserve_downloads,
                 output_dir=structured_output_dir,
                 re_download=re_download,
                 metadata_include=metadata_include,
                 metadata_exclude=metadata_exclude,
+                partition_by_api=partition_by_api,
+                partition_endpoint=partition_endpoint,
                 fields_include=fields_include,
                 flatten_metadata=flatten_metadata,
+                download_only=download_only,
+            ),
+        )
+    elif slack_channels:
+        from unstructured.ingest.connector.slack import (
+            SimpleSlackConfig,
+            SlackConnector,
+        )
+
+        doc_connector = SlackConnector(  # type: ignore
+            config=SimpleSlackConfig(
+                channels=SimpleSlackConfig.parse_channels(slack_channels),
+                token=slack_token,
+                oldest=start_date,
+                latest=end_date,
+                # defaults params:
+                download_dir=download_dir,
+                preserve_downloads=preserve_downloads,
+                output_dir=structured_output_dir,
+                re_download=re_download,
+                verbose=verbose,
             ),
         )
     elif wikipedia_page_title:
         doc_connector = WikipediaConnector(  # type: ignore
             config=SimpleWikipediaConfig(
                 title=wikipedia_page_title,
                 auto_suggest=wikipedia_auto_suggest,
                 # defaults params:
                 download_dir=download_dir,
                 preserve_downloads=preserve_downloads,
                 output_dir=structured_output_dir,
                 re_download=re_download,
                 metadata_include=metadata_include,
                 metadata_exclude=metadata_exclude,
+                partition_by_api=partition_by_api,
+                partition_endpoint=partition_endpoint,
                 fields_include=fields_include,
                 flatten_metadata=flatten_metadata,
+                download_only=download_only,
             ),
         )
     elif drive_id:
+        from unstructured.ingest.connector.google_drive import (
+            GoogleDriveConnector,
+            SimpleGoogleDriveConfig,
+        )
+
         doc_connector = GoogleDriveConnector(  # type: ignore
             config=SimpleGoogleDriveConfig(
                 drive_id=drive_id,
                 service_account_key=drive_service_account_key,
                 recursive=drive_recursive,
                 extension=drive_extension,
                 # defaults params:
                 download_dir=download_dir,
                 preserve_downloads=preserve_downloads,
                 output_dir=structured_output_dir,
                 re_download=re_download,
                 metadata_include=metadata_include,
                 metadata_exclude=metadata_exclude,
+                partition_by_api=partition_by_api,
+                partition_endpoint=partition_endpoint,
                 fields_include=fields_include,
                 flatten_metadata=flatten_metadata,
+                download_only=download_only,
             ),
         )
     elif biomed_path or biomed_api_id or biomed_api_from or biomed_api_until:
+        from unstructured.ingest.connector.biomed import (
+            BiomedConnector,
+            SimpleBiomedConfig,
+        )
+
         doc_connector = BiomedConnector(  # type: ignore
             config=SimpleBiomedConfig(
                 path=biomed_path,
                 id_=biomed_api_id,
                 from_=biomed_api_from,
                 until=biomed_api_until,
                 # defaults params:
                 download_dir=download_dir,
                 preserve_downloads=preserve_downloads,
                 output_dir=structured_output_dir,
                 re_download=re_download,
                 metadata_include=metadata_include,
                 metadata_exclude=metadata_exclude,
+                partition_by_api=partition_by_api,
+                partition_endpoint=partition_endpoint,
                 fields_include=fields_include,
                 flatten_metadata=flatten_metadata,
+                download_only=download_only,
             ),
         )
     elif local_input_path:
+        from unstructured.ingest.connector.local import (
+            LocalConnector,
+            SimpleLocalConfig,
+        )
+
         doc_connector = LocalConnector(  # type: ignore
             config=SimpleLocalConfig(
                 input_path=local_input_path,
                 recursive=local_recursive,
                 file_glob=local_file_glob,
                 # defaults params:
                 output_dir=structured_output_dir,
                 metadata_include=metadata_include,
                 metadata_exclude=metadata_exclude,
+                partition_by_api=partition_by_api,
+                partition_endpoint=partition_endpoint,
                 fields_include=fields_include,
+                flatten_metadata=flatten_metadata,
             ),
         )
     # Check for other connector-specific options here and define the doc_connector object
     # e.g. "elif azure_container:  ..."
 
     else:
         logger.error("No connector-specific option was specified!")
```

### Comparing `unstructured-0.5.9/unstructured/nlp/english-words.txt` & `unstructured-0.6.0/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/nlp/english_words.py` & `unstructured-0.6.0/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/nlp/patterns.py` & `unstructured-0.6.0/unstructured/nlp/patterns.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,17 @@
 )
 EMAIL_HEAD_RE = re.compile(EMAIL_HEAD_PATTERN)
 
 # Helps split text by paragraphs. There must be one newline, with potential whitespace
 # (incluing \r and \n chars) on either side
 PARAGRAPH_PATTERN = r"\s*\n\s*"  # noqa: W605 NOTE(harrell)
 
+PARAGRAPH_PATTERN_RE = re.compile(f"((?:{'|'.join(UNICODE_BULLETS)})|{PARAGRAPH_PATTERN})")
+DOUBLE_PARAGRAPH_PATTERN_RE = re.compile("(" + PARAGRAPH_PATTERN + "){2}")
+
 # IP Address examples: ba23::58b5:2236:45g2:88h2 or 10.0.2.01
 IP_ADDRESS_PATTERN = (
     "[0-9]{1,2}\.[0-9]{1,2}\.[0-9]{1,2}\.[0-9]{1,2}",  # noqa: W605 NOTE(harrell)
     # - skipping qa because we need the escape for the regex
     "[a-z0-9]{4}::[a-z0-9]{4}:[a-z0-9]{4}:[a-z0-9]{4}:[a-z0-9]{4}%?[0-9]*",
 )
 IP_ADDRESS_PATTERN_RE = re.compile(f"({'|'.join(IP_ADDRESS_PATTERN)})")
```

### Comparing `unstructured-0.5.9/unstructured/nlp/tokenize.py` & `unstructured-0.6.0/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/partition/__init__.py` & `unstructured-0.6.0/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/partition/common.py` & `unstructured-0.6.0/unstructured/partition/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import subprocess
-from typing import List, Optional, Union
+from typing import List, Optional, Tuple, Union
 
 from unstructured.documents.elements import (
     TYPE_TO_TEXT_ELEMENT_MAP,
     CheckBox,
     Element,
     ElementMetadata,
     ListItem,
@@ -38,15 +38,18 @@
         return CheckBox(checked=True, coordinates=coordinates)
     elif element_type == "Unchecked":
         return CheckBox(checked=False, coordinates=coordinates)
     else:
         return Text(text=text, coordinates=coordinates)
 
 
-def layout_list_to_list_items(text: str, coordinates: List[float]) -> List[Element]:
+def layout_list_to_list_items(
+    text: str,
+    coordinates: Tuple[Tuple[float, float], ...],
+) -> List[Element]:
     """Converts a list LayoutElement to a list of ListItem elements."""
     split_items = ENUMERATED_BULLETS_RE.split(text)
     # NOTE(robinson) - this means there wasn't a match for the enumerated bullets
     if len(split_items) == 1:
         split_items = UNICODE_BULLETS_RE.split(text)
 
     list_items: List[Element] = []
@@ -83,15 +86,24 @@
 ) -> List[Element]:
     """Adds document metadata to the document element. Document metadata includes information
     like the filename, source url, and page number."""
     elements: List[Element] = []
     page_number: int = 1
     for layout_element in layout_elements:
         element = normalize_layout_element(layout_element)
-        metadata = ElementMetadata(filename=filename, url=url, page_number=page_number)
+        if hasattr(layout_element, "text_as_html"):
+            text_as_html: Optional[str] = layout_element.text_as_html
+        else:
+            text_as_html = None
+        metadata = ElementMetadata(
+            filename=filename,
+            url=url,
+            page_number=page_number,
+            text_as_html=text_as_html,
+        )
         if isinstance(element, list):
             for _element in element:
                 _element.metadata = metadata
             elements.extend(element)
         elif isinstance(element, PageBreak):
             page_number += 1
             if include_page_breaks is True:
```

### Comparing `unstructured-0.5.9/unstructured/partition/doc.py` & `unstructured-0.6.0/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/partition/docx.py` & `unstructured-0.6.0/unstructured/partition/docx.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 
 def _paragraph_to_element(paragraph: docx.text.paragraph.Paragraph) -> Optional[Text]:
     """Converts a docx Paragraph object into the appropriate unstructured document element.
     If the paragraph style is "Normal" or unknown, we try to predict the element type from the
     raw text."""
     text = paragraph.text
-    style_name = paragraph.style.name
+    style_name = paragraph.style and paragraph.style.name  # .style can be None
 
     if len(text.strip()) == 0:
         return None
 
     element_class = STYLE_TO_ELEMENT_MAPPING.get(style_name)
 
     # NOTE(robinson) - The "Normal" style name will return None since it's in the mapping.
```

### Comparing `unstructured-0.5.9/unstructured/partition/email.py` & `unstructured-0.6.0/unstructured/partition/email.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import datetime
 import email
 import re
 import sys
 from email.message import Message
+from functools import partial
 from typing import IO, Dict, List, Optional, Tuple, Union
 
 from unstructured.partition.common import exactly_one
 
 if sys.version_info < (3, 8):
     from typing_extensions import Final
 else:
@@ -83,26 +85,57 @@
             elements += _parse_received_data(item[1])
         else:
             elements.append(MetaData(name=item[0], text=item[1]))
 
     return elements
 
 
+def build_email_metadata(msg: Message) -> ElementMetadata:
+    """Creates an ElementMetadata object from the header information in the email."""
+    header_dict = dict(msg.raw_items())
+    email_date = header_dict.get("Date")
+    if email_date is not None:
+        email_date = convert_to_iso_8601(email_date)
+
+    sent_from = header_dict.get("To")
+    if sent_from is not None:
+        sent_from = [sender.strip() for sender in sent_from.split(",")]
+
+    sent_to = header_dict.get("To")
+    if sent_to is not None:
+        sent_to = [recipient.strip() for recipient in sent_to.split(",")]
+
+    return ElementMetadata(
+        sent_to=sent_to,
+        sent_from=sent_from,
+        subject=header_dict.get("Subject"),
+        date=email_date,
+    )
+
+
+def convert_to_iso_8601(time: str) -> str:
+    """Converts the datetime from the email output to ISO-8601 format."""
+    datetime_object = datetime.datetime.strptime(time, "%a, %d %b %Y %H:%M:%S %z")
+    return datetime_object.isoformat()
+
+
 def extract_attachment_info(
     message: Message,
     output_dir: Optional[str] = None,
 ) -> List[Dict[str, str]]:
     list_attachments = []
-    attachment_info = {}
+
     for part in message.walk():
         if "content-disposition" in part:
             cdisp = part["content-disposition"].split(";")
             cdisp = [clean_extra_whitespace(item) for item in cdisp]
 
             for item in cdisp:
+                attachment_info = {}
+
                 if item.lower() == "attachment":
                     continue
                 key, value = item.split("=")
                 key = clean_extra_whitespace(key.replace('"', ""))
                 value = clean_extra_whitespace(value.replace('"', ""))
                 attachment_info[clean_extra_whitespace(key)] = clean_extra_whitespace(value)
             attachment_info["payload"] = part.get_payload(decode=True)
@@ -213,15 +246,16 @@
         #    <li>Item 2<li>=
         # </ul>
         list_content = content.split("=\n")
         content = "".join(list_content)
         elements = partition_html(text=content, include_metadata=False)
         for element in elements:
             if isinstance(element, Text):
-                element.apply(replace_mime_encodings)
+                _replace_mime_encodings = partial(replace_mime_encodings, encoding=encoding)
+                element.apply(_replace_mime_encodings)
     elif content_source == "text/plain":
         list_content = split_by_paragraph(content)
         elements = partition_text(text=content)
 
     for idx, element in enumerate(elements):
         indices = has_embedded_image(element)
         if (isinstance(element, (NarrativeText, Title))) and indices:
@@ -230,10 +264,12 @@
             elements.insert(idx + 1, image_info)
 
     header: List[Element] = []
     if include_headers:
         header = partition_email_header(msg)
     all_elements = header + elements
 
+    metadata = build_email_metadata(msg)
+    metadata.filename = filename
     for element in all_elements:
-        element.metadata = ElementMetadata(filename=filename)
+        element.metadata = metadata
     return all_elements
```

### Comparing `unstructured-0.5.9/unstructured/partition/epub.py` & `unstructured-0.6.0/unstructured/partition/md.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,57 @@
-from typing import IO, List, Optional
+from typing import IO, List, Optional, Union
+
+import markdown
+import requests
 
 from unstructured.documents.elements import Element
-from unstructured.file_utils.file_conversion import convert_epub_to_html
+from unstructured.documents.xml import VALID_PARSERS
+from unstructured.partition.common import exactly_one
 from unstructured.partition.html import partition_html
 
 
-def partition_epub(
+def optional_decode(contents: Union[str, bytes]) -> str:
+    if isinstance(contents, bytes):
+        return contents.decode("utf-8")
+    return contents
+
+
+def partition_md(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
+    text: Optional[str] = None,
+    url: Optional[str] = None,
     include_page_breaks: bool = False,
+    include_metadata: bool = True,
+    parser: VALID_PARSERS = None,
 ) -> List[Element]:
-    """Partitions an EPUB document. The document is first converted to HTML and then
-    partitoned using partiton_html.
+    # Verify that only one of the arguments was provided
+    if text is None:
+        text = ""
+    exactly_one(filename=filename, file=file, text=text, url=url)
+
+    if filename is not None:
+        with open(filename, encoding="utf8") as f:
+            text = optional_decode(f.read())
+
+    elif file is not None:
+        text = optional_decode(file.read())
+
+    elif url is not None:
+        response = requests.get(url)
+        if not response.ok:
+            raise ValueError(f"URL return an error: {response.status_code}")
+
+        content_type = response.headers.get("Content-Type", "")
+        if not content_type.startswith("text/markdown"):
+            raise ValueError(f"Expected content type text/markdown. Got {content_type}.")
+
+        text = response.text
+
+    html = markdown.markdown(text)
 
-    Parameters
-    ----------
-     filename
-        A string defining the target filename path.
-    file
-        A file-like object using "rb" mode --> open(filename, "rb").
-    include_page_breaks
-        If True, the output will include page breaks if the filetype supports it
-    """
-    html_text = convert_epub_to_html(filename=filename, file=file)
-    # NOTE(robinson) - pypandoc returns a text string with unicode encoding
-    # ref: https://github.com/JessicaTegner/pypandoc#usage
     return partition_html(
-        text=html_text,
+        text=html,
         include_page_breaks=include_page_breaks,
-        encoding="unicode",
+        include_metadata=include_metadata,
+        parser=parser,
     )
```

### Comparing `unstructured-0.5.9/unstructured/partition/html.py` & `unstructured-0.6.0/unstructured/partition/html.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import IO, Dict, List, Optional
 
 import requests
 
 from unstructured.documents.elements import Element
 from unstructured.documents.html import HTMLDocument
 from unstructured.documents.xml import VALID_PARSERS
+from unstructured.file_utils.file_conversion import convert_file_to_html_text
 from unstructured.partition.common import (
     add_element_metadata,
     document_to_element_list,
     exactly_one,
 )
 
 
@@ -17,14 +18,15 @@
     file: Optional[IO] = None,
     text: Optional[str] = None,
     url: Optional[str] = None,
     encoding: Optional[str] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     headers: Dict[str, str] = {},
+    ssl_verify: bool = True,
     parser: VALID_PARSERS = None,
 ) -> List[Element]:
     """Partitions an HTML document into its constituent elements.
 
     Parameters
     ----------
      filename
@@ -38,14 +40,19 @@
     encoding
         The encoding method used to decode the text input. If None, utf-8 will be used.
     include_page_breaks
         If True, includes page breaks at the end of each page in the document.
     include_metadata
         Optionally allows for excluding metadata from the output. Primarily intended
         for when partition_html is called in other partition bricks (like partition_email)
+    headers
+        The headers to be used in conjunction with the HTTP request if URL is set.
+    ssl_verify
+        If the URL parameter is set, determines whether or not partition uses SSL verification
+        in the HTTP request.
     parser
         The parser to use for parsing the HTML document. If None, default parser will be used.
     """
     if text is not None and text.strip() == "" and not file and not filename and not url:
         return []
 
     # Verify that only one of the arguments was provided
@@ -67,15 +74,15 @@
         document = HTMLDocument.from_string(file_text, parser=parser)
 
     elif text is not None:
         _text: str = str(text)
         document = HTMLDocument.from_string(_text, parser=parser)
 
     elif url is not None:
-        response = requests.get(url, headers=headers)
+        response = requests.get(url, headers=headers, verify=ssl_verify)
         if not response.ok:
             raise ValueError(f"URL return an error: {response.status_code}")
 
         content_type = response.headers.get("Content-Type", "")
         if not content_type.startswith("text/html"):
             raise ValueError(f"Expected content type text/html. Got {content_type}.")
 
@@ -87,7 +94,38 @@
             layout_elements,
             include_page_breaks=include_page_breaks,
             filename=filename,
             url=url,
         )
     else:
         return layout_elements
+
+
+def convert_and_partition_html(
+    source_format: str,
+    filename: Optional[str] = None,
+    file: Optional[IO] = None,
+    include_page_breaks: bool = False,
+) -> List[Element]:
+    """Converts a document to HTML and then partitions it using partition_html. Works with
+    any file format support by pandoc.
+
+    Parameters
+    ----------
+    source_format
+        The format of the source document, i.e. rst
+    filename
+        A string defining the target filename path.
+    file
+        A file-like object using "rb" mode --> open(filename, "rb").
+
+    include_page_breaks
+        If True, the output will include page breaks if the filetype supports it
+    """
+    html_text = convert_file_to_html_text(source_format=source_format, filename=filename, file=file)
+    # NOTE(robinson) - pypandoc returns a text string with unicode encoding
+    # ref: https://github.com/JessicaTegner/pypandoc#usage
+    return partition_html(
+        text=html_text,
+        include_page_breaks=include_page_breaks,
+        encoding="unicode",
+    )
```

### Comparing `unstructured-0.5.9/unstructured/partition/image.py` & `unstructured-0.6.0/unstructured/partition/image.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 def partition_image(
     filename: str = "",
     file: Optional[bytes] = None,
     url: Optional[str] = None,
     template: Optional[str] = None,
     token: Optional[str] = None,
     include_page_breaks: bool = False,
+    ocr_languages: str = "eng",
 ) -> List[Element]:
     """Parses an image into a list of interpreted elements.
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
@@ -23,18 +24,22 @@
         A string defining the model to be used. Default None uses default model ("layout/image" url
         if using the API).
     url
         A string endpoint to self-host an inference API, if desired. If None, local inference will
         be used.
     token
         A string defining the authentication token for a self-host url, if applicable.
+    ocr_languages
+        The languages to use for the Tesseract agent. To use a language, you'll first need
+        to isntall the appropriate Tesseract language pack.
     """
     if template is None:
         template = "layout/image"
     return partition_pdf_or_image(
         filename=filename,
         file=file,
         url=url,
         template=template,
         token=token,
         include_page_breaks=include_page_breaks,
+        ocr_languages=ocr_languages,
     )
```

### Comparing `unstructured-0.5.9/unstructured/partition/json.py` & `unstructured-0.6.0/unstructured/partition/json.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     file: Optional[IO] = None,
     text: Optional[str] = None,
 ) -> List[Element]:
     """Partitions an .json document into its constituent elements."""
     if text is not None and text.strip() == "" and not file and not filename:
         return []
 
-    exactly_one(filenmae=filename, file=file, text=text)
+    exactly_one(filename=filename, file=file, text=text)
 
     if filename is not None:
         with open(filename, encoding="utf8") as f:
             file_text = f.read()
     elif file is not None:
         file_text = file.read()
     elif text is not None:
```

### Comparing `unstructured-0.5.9/unstructured/partition/md.py` & `unstructured-0.6.0/unstructured/partition/ppt.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,50 @@
-from typing import IO, List, Optional, Union
-
-import markdown
-import requests
+import os
+import tempfile
+from typing import IO, List, Optional
 
 from unstructured.documents.elements import Element
-from unstructured.documents.xml import VALID_PARSERS
-from unstructured.partition.common import exactly_one
-from unstructured.partition.html import partition_html
-
-
-def optional_decode(contents: Union[str, bytes]) -> str:
-    if isinstance(contents, bytes):
-        return contents.decode("utf-8")
-    return contents
+from unstructured.partition.common import convert_office_doc, exactly_one
+from unstructured.partition.pptx import partition_pptx
 
 
-def partition_md(
+def partition_ppt(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
-    text: Optional[str] = None,
-    url: Optional[str] = None,
     include_page_breaks: bool = False,
-    include_metadata: bool = True,
-    parser: VALID_PARSERS = None,
 ) -> List[Element]:
-    # Verify that only one of the arguments was provided
-    if text is None:
-        text = ""
-    exactly_one(filename=filename, file=file, text=text, url=url)
-
-    if filename is not None:
-        with open(filename, encoding="utf8") as f:
-            text = optional_decode(f.read())
+    """Partitions Microsoft PowerPoint Documents in .ppt format into their document elements.
 
+    Parameters
+    ----------
+    filename
+        A string defining the target filename path.
+    file
+        A file-like object using "rb" mode --> open(filename, "rb").
+    include_page_breaks
+        If True, includes a PageBreak element between slides
+    """
+    # Verify that only one of the arguments was provided
+    if filename is None:
+        filename = ""
+    exactly_one(filename=filename, file=file)
+
+    if len(filename) > 0:
+        _, filename_no_path = os.path.split(os.path.abspath(filename))
+        base_filename, _ = os.path.splitext(filename_no_path)
+        if not os.path.exists(filename):
+            raise ValueError(f"The file {filename} does not exist.")
     elif file is not None:
-        text = optional_decode(file.read())
+        tmp = tempfile.NamedTemporaryFile(delete=False)
+        tmp.write(file.read())
+        tmp.close()
+        filename = tmp.name
+        _, filename_no_path = os.path.split(os.path.abspath(tmp.name))
+
+    base_filename, _ = os.path.splitext(filename_no_path)
+
+    with tempfile.TemporaryDirectory() as tmpdir:
+        convert_office_doc(filename, tmpdir, target_format="pptx")
+        pptx_filename = os.path.join(tmpdir, f"{base_filename}.pptx")
+        elements = partition_pptx(filename=pptx_filename, metadata_filename=filename)
 
-    elif url is not None:
-        response = requests.get(url)
-        if not response.ok:
-            raise ValueError(f"URL return an error: {response.status_code}")
-
-        content_type = response.headers.get("Content-Type", "")
-        if not content_type.startswith("text/markdown"):
-            raise ValueError(f"Expected content type text/markdown. Got {content_type}.")
-
-        text = response.text
-
-    html = markdown.markdown(text)
-
-    return partition_html(
-        text=html,
-        include_page_breaks=include_page_breaks,
-        include_metadata=include_metadata,
-        parser=parser,
-    )
+    return elements
```

### Comparing `unstructured-0.5.9/unstructured/partition/pdf.py` & `unstructured-0.6.0/unstructured/partition/pdf.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,15 +18,17 @@
     filename: str = "",
     file: Optional[bytes] = None,
     url: Optional[str] = None,
     template: str = "layout/pdf",
     token: Optional[str] = None,
     include_page_breaks: bool = False,
     strategy: str = "hi_res",
+    extract_tables: bool = False,
     encoding: str = "utf-8",
+    ocr_languages: str = "eng",
 ) -> List[Element]:
     """Parses a pdf document into a list of interpreted elements.
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
@@ -39,79 +41,103 @@
         be used.
     token
         A string defining the authentication token for a self-host url, if applicable.
     strategy
         The strategy to use for partitioning the PDF. Uses a layout detection model if set
         to 'hi_res', otherwise partition_pdf simply extracts the text from the document
         and processes it.
+    extract_tables
+        If True, extracts any tables that are detected when using 'hi_res' strategy. Whether this
+        is True or False, the partitioning process will attempt to identify any tables in the
+        document. This parameter indicates that the partitioning process will attempt to extract the
+        structure of any identified tables. The table structure and cell contents will be stored as
+        HTML in the metadata in the text_as_html property, e.g. element.metadata.text_as_html
     encoding
         The encoding method used to decode the text input. If None, utf-8 will be used.
+    ocr_languages
+        The languages to use for the Tesseract agent. To use a language, you'll first need
+        to isntall the appropriate Tesseract language pack.
     """
     exactly_one(filename=filename, file=file)
     return partition_pdf_or_image(
         filename=filename,
         file=file,
         url=url,
         template=template,
         token=token,
         include_page_breaks=include_page_breaks,
         strategy=strategy,
+        extract_tables=extract_tables,
         encoding=encoding,
+        ocr_languages=ocr_languages,
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
+    extract_tables: bool = False,
     encoding: str = "utf-8",
+    ocr_languages: str = "eng",
 ) -> List[Element]:
     """Parses a pdf or image document into a list of interpreted elements."""
     if url is None:
         # TODO(alan): Extract information about the filetype to be processed from the template
         # route. Decoding the routing should probably be handled by a single function designed for
         # that task so as routing design changes, those changes are implemented in a single
         # function.
         route_args = template.strip("/").split("/")
         is_image = route_args[-1] == "image"
         out_template: Optional[str] = template
         if route_args[0] == "layout":
             out_template = None
 
         fallback_to_fast = False
-        if not dependency_exists("detectron2"):
+        detectron2_installed = dependency_exists("detectron2")
+
+        if not detectron2_installed:
             if is_image:
                 raise ValueError(
-                    "detectron2 is not installed. detectron2 is required for " "partioning images.",
+                    "detectron2 is not installed. detectron2 is required for partioning images.",
                 )
             else:
                 fallback_to_fast = True
-                logger.warn(
-                    "detectron2 is not installed. Cannot use the hi_res partitioning "
-                    "strategy. Falling back to partitioning with the fast strategy.",
-                )
 
         if strategy == "hi_res" and not fallback_to_fast:
             # NOTE(robinson): Catches a UserWarning that occurs when detectron is called
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 layout_elements = _partition_pdf_or_image_local(
                     filename=filename,
                     file=file,
                     template=out_template,
                     is_image=is_image,
+                    extract_tables=extract_tables,
                     include_page_breaks=True,
+                    ocr_languages=ocr_languages,
                 )
 
         elif strategy == "fast" or fallback_to_fast:
+            if strategy == "hi_res":
+                logger.warning(
+                    "detectron2 is not installed. Cannot use the hi_res partitioning "
+                    "strategy. Falling back to partitioning with the fast strategy.",
+                )
+            if extract_tables:
+                logger.warning(
+                    "Table extraction was selected, but is being ignored while using the fast "
+                    "strategy.",
+                )
+
             return _partition_pdf_with_pdfminer(
                 filename=filename,
                 file=file,
                 include_page_breaks=include_page_breaks,
                 encoding=encoding,
             )
 
@@ -143,15 +169,17 @@
 
 
 def _partition_pdf_or_image_local(
     filename: str = "",
     file: Optional[bytes] = None,
     template: Optional[str] = None,
     is_image: bool = False,
+    extract_tables: bool = False,
     include_page_breaks: bool = False,
+    ocr_languages: str = "eng",
 ) -> List[Element]:
     """Partition using package installed locally."""
     try:
         from unstructured_inference.inference.layout import (
             process_data_with_model,
             process_file_with_model,
         )
@@ -166,19 +194,30 @@
         raise Exception(
             "There was a problem importing unstructured_inference module - it may not be installed "
             "correctly... try running pip install unstructured[local-inference] if you installed "
             "the unstructured library as a package. If you cloned the unstructured repository, try "
             "running make install-local-inference from the root directory of the repository.",
         ) from e
 
-    layout = (
-        process_file_with_model(filename, template, is_image=is_image)
-        if file is None
-        else process_data_with_model(file, template, is_image=is_image)
-    )
+    if file is None:
+        layout = process_file_with_model(
+            filename,
+            template,
+            is_image=is_image,
+            ocr_languages=ocr_languages,
+            extract_tables=extract_tables,
+        )
+    else:
+        layout = process_data_with_model(
+            file,
+            template,
+            is_image=is_image,
+            ocr_languages=ocr_languages,
+            extract_tables=extract_tables,
+        )
 
     return document_to_element_list(layout, include_page_breaks=include_page_breaks)
 
 
 @requires_dependencies("pdfminer", "local-inference")
 def _partition_pdf_with_pdfminer(
     filename: str = "",
```

### Comparing `unstructured-0.5.9/unstructured/partition/pptx.py` & `unstructured-0.6.0/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/partition/text.py` & `unstructured-0.6.0/unstructured/partition/text.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
-from typing import IO, List, Optional
+from typing import IO, Callable, List, Optional
 
-from unstructured.cleaners.core import clean_bullets
+from unstructured.cleaners.core import clean_bullets, group_broken_paragraphs
 from unstructured.documents.elements import (
     Address,
     Element,
     ElementMetadata,
     ListItem,
     NarrativeText,
     Text,
@@ -26,26 +26,30 @@
 
 
 def partition_text(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     text: Optional[str] = None,
     encoding: Optional[str] = "utf-8",
+    paragraph_grouper: Optional[Callable[[str], str]] = None,
 ) -> List[Element]:
     """Partitions an .txt documents into its constituent elements.
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "r" mode --> open(filename, "r").
     text
         The string representation of the .txt document.
     encoding
         The encoding method used to decode the text input. If None, utf-8 will be used.
+    paragrapher_grouper
+        A str -> str function for fixing paragraphs that are interrupted by line breaks
+        for formatting purposes.
     """
     if text is not None and text.strip() == "" and not file and not filename:
         return []
 
     # Verify that only one of the arguments was provided
     exactly_one(filename=filename, file=file, text=text)
 
@@ -60,14 +64,19 @@
         file_text = file.read()
         if isinstance(file_text, bytes):
             file_text = file_text.decode(encoding)
 
     elif text is not None:
         file_text = str(text)
 
+    if paragraph_grouper is not None:
+        file_text = paragraph_grouper(file_text)
+    else:
+        file_text = group_broken_paragraphs(file_text)
+
     file_content = split_by_paragraph(file_text)
 
     elements: List[Element] = []
     metadata = ElementMetadata(filename=filename)
     for ctext in file_content:
         ctext = ctext.strip()
```

### Comparing `unstructured-0.5.9/unstructured/partition/text_type.py` & `unstructured-0.6.0/unstructured/partition/text_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -261,23 +261,32 @@
     threshold
         If the percentage of words beginning with a capital letter exceeds this threshold,
         the function returns True
     """
     # NOTE(robinson) - Currently limiting this to only sections of text with one sentence.
     # The assumption is that sections with multiple sentences are not titles.
     if sentence_count(text, 3) > 1:
-        logger.debug(f"Text does not contain multiple sentences:\n\n{text}")
         return False
 
     if text.isupper():
         return False
 
-    tokens = word_tokenize(text)
+    # NOTE(jay-ylee) - The word_tokenize function also recognizes and separates special characters
+    # into one word, causing problems with ratio measurement.
+    # Therefore, only words consisting of alphabets are used to measure the ratio.
+    # ex. world_tokenize("ITEM 1. Financial Statements (Unaudited)")
+    #     = ['ITEM', '1', '.', 'Financial', 'Statements', '(', 'Unaudited', ')'],
+    # however, "ITEM 1. Financial Statements (Unaudited)" is Title, not NarrativeText
+    tokens = [tk for tk in word_tokenize(text) if tk.isalpha()]
+
+    # NOTE(jay-ylee) - If word_tokenize(text) is empty, return must be True to
+    # avoid being misclassified as Narrative Text.
     if len(tokens) == 0:
-        return False
+        return True
+
     capitalized = sum([word.istitle() or word.isupper() for word in tokens])
     ratio = capitalized / len(tokens)
     return ratio > threshold
 
 
 def is_us_city_state_zip(text) -> bool:
     """Checks if the given text is in the format of US city/state/zip code.
```

### Comparing `unstructured-0.5.9/unstructured/staging/argilla.py` & `unstructured-0.6.0/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/staging/base.py` & `unstructured-0.6.0/unstructured/staging/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import csv
 import io
 import json
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Tuple
 
 import pandas as pd
 
 from unstructured.documents.elements import (
     TYPE_TO_TEXT_ELEMENT_MAP,
     CheckBox,
     Element,
@@ -59,15 +59,18 @@
 
 def isd_to_elements(isd: List[Dict[str, Any]]) -> List[Element]:
     """Converts an Initial Structured Data (ISD) dictionary to a list of elements."""
     elements: List[Element] = []
 
     for item in isd:
         element_id: str = item.get("element_id", NoID())
-        coordinates: Optional[List[float]] = item.get("coordinates")
+        coord_value: Optional[List[List[float]]] = item.get("coordinates")
+        coordinates: Optional[Tuple[Tuple[float, float], ...]] = None
+        if coord_value is not None:
+            coordinates = tuple((x, y) for x, y in coord_value)
 
         metadata = ElementMetadata()
         _metadata_dict = item.get("metadata")
         if _metadata_dict is not None:
             metadata = ElementMetadata.from_dict(_metadata_dict)
 
         if item["type"] in TYPE_TO_TEXT_ELEMENT_MAP:
```

### Comparing `unstructured-0.5.9/unstructured/staging/datasaur.py` & `unstructured-0.6.0/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/staging/huggingface.py` & `unstructured-0.6.0/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/staging/label_box.py` & `unstructured-0.6.0/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/staging/label_studio.py` & `unstructured-0.6.0/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured/staging/prodigy.py` & `unstructured-0.6.0/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.9/unstructured.egg-info/PKG-INFO` & `unstructured-0.6.0/unstructured.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.5.9
+Version: 0.6.0
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -30,14 +30,26 @@
           href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
             <img src="https://img.shields.io/badge/JOIN US ON SLACK-4A154B?style=for-the-badge&logo=slack&logoColor=white" />
           </a>
           <a href="https://www.linkedin.com/company/unstructuredio/">
             <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
           </a>
         </div>
+        <h2 align="center">
+          <p>Announcement!!!</p>
+        </h2>
+        <div align="center">
+          <p>We're excited to announce the public release of the unstructured.io hosted API! Now you can leverage Unstructured with a simple API call to render clean text in JSON format out of your images, documents, powerpoints, and more.</p>
+        
+        <p>Checkout the <a href="https://github.com/Unstructured-IO/unstructured-api#--">readme</a> here to get started making API calls. You’ll also find instructions there about how to host your own version of the API. Unstructured data just got easier! 
+        We'd love to hear your feedback, let us know how it goes in our <a
+          href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
+           community slack</a>. And stay tuned for improvements to both quality and performance over the coming months!
+        <p><img src="easy.gif"></p></p>
+        </div>
         
         <h3 align="center">
           <p>Open-Source Pre-Processing Tools for Unstructured Data</p>
         </h3>
         
         The `unstructured` library provides open-source components for pre-processing text documents
         such as **PDFs**, **HTML** and **Word** Documents. These components are packaged as *bricks* 🧱, which provide
@@ -65,15 +77,15 @@
           Depending on what document types you're parsing, you may not need all of these.
             - `libmagic-dev` (filetype detection)
             - `poppler-utils` (images and PDFs)
             - `tesseract-ocr` (images and PDFs)
             - `libreoffice` (MS Office docs)
         - If you are parsing PDFs, run the following to install the `detectron2` model, which
           `unstructured` uses for layout detection:
-            - `pip install "detectron2@git+https://github.com/facebookresearch/detectron2.git@v0.6#egg=detectron2"`
+            - `pip install "detectron2@git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"`
         
         At this point, you should be able to run the following code:
         
         ```python
         from unstructured.partition.auto import partition
         
         elements = partition(filename="example-docs/fake-email.eml")
@@ -171,15 +183,15 @@
         you can also uninstall the hooks with `pre-commit uninstall`.
         
         ## :clap: Quick Tour
         
         You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
         
         The following examples show how to get started with the `unstructured` library.
-        You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **EPUB**, **DOC**, **DOCX**, **PPT**, **PPTX**, **JPG**,
+        You can parse **TXT**, **HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**, **PPT**, **PPTX**, **JPG**,
         and **PNG** documents with one line of code!
         <br></br>
         See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
         of the features in the library.
         
         ### Document Parsing
         
@@ -393,9 +405,10 @@
 Provides-Extra: huggingface
 Provides-Extra: local-inference
 Provides-Extra: s3
 Provides-Extra: azure
 Provides-Extra: github
 Provides-Extra: gitlab
 Provides-Extra: reddit
+Provides-Extra: slack
 Provides-Extra: wikipedia
 Provides-Extra: google-drive
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.5.9 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.0 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -12,14 +12,24 @@
     /img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg) ![https://
  GitHub.com/unstructured-io/unstructured.js/releases](https://img.shields.io/
   github/release/unstructured-io/unstructured) ![https://github.com/Naereen/
 badges/](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)
      [https://img.shields.io/badge/JOIN_US_ON_SLACK-4A154B?style=for-the-
    badge&logo=slack&logoColor=white] [https://img.shields.io/badge/LinkedIn-
            0077B5?style=for-the-badge&logo=linkedin&logoColor=white]
+                          ***** Announcement!!! *****
+We're excited to announce the public release of the unstructured.io hosted API!
+ Now you can leverage Unstructured with a simple API call to render clean text
+     in JSON format out of your images, documents, powerpoints, and more.
+ Checkout the readme here to get started making API calls. Youâll also find
+instructions there about how to host your own version of the API. Unstructured
+data just got easier! We'd love to hear your feedback, let us know how it goes
+  in our community_slack. And stay tuned for improvements to both quality and
+                      performance over the coming months!
+                                  [easy.gif]
        **** Open-Source Pre-Processing Tools for Unstructured Data ****
 The `unstructured` library provides open-source components for pre-processing
 text documents such as **PDFs**, **HTML** and **Word** Documents. These
 components are packaged as *bricks* ð§±, which provide users the building
 blocks they need to build pipelines targeted at the documents they care about.
 Bricks in the library fall into three categories: - :jigsaw: ***Partitioning
 bricks*** that break raw documents down into standard, structured elements. - :
@@ -34,19 +44,19 @@
 Install the following system dependencies if they are not already available on
 your system. Depending on what document types you're parsing, you may not need
 all of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
 - If you are parsing PDFs, run the following to install the `detectron2` model,
 which `unstructured` uses for layout detection: - `pip install
 "detectron2@git+https://github.com/facebookresearch/
-detectron2.git@v0.6#egg=detectron2"` At this point, you should be able to run
-the following code: ```python from unstructured.partition.auto import partition
-elements = partition(filename="example-docs/fake-email.eml") print("\n\n".join(
-[str(el) for el in elements])) ``` And if you installed with `local-inference`,
-you should be able to run this as well: ```python from
+detectron2.git@e2ce8dc#egg=detectron2"` At this point, you should be able to
+run the following code: ```python from unstructured.partition.auto import
+partition elements = partition(filename="example-docs/fake-email.eml") print
+("\n\n".join([str(el) for el in elements])) ``` And if you installed with
+`local-inference`, you should be able to run this as well: ```python from
 unstructured.partition.auto import partition elements = partition("example-
 docs/layout-parser-paper.pdf") print("\n\n".join([str(el) for el in elements]))
 ``` ## :dizzy: Instructions for using the docker image The following
 instructions are intended to help you get up and running using Docker to
 interact with `unstructured`. See [here](https://docs.docker.com/get-docker/
 ) if you don't already have docker installed on your machine. NOTE: we build
 multi-platform images to support both x86_64 and Apple silicon hardware.
@@ -98,16 +108,16 @@
 `pre-commit`, you'll just need to install the hooks with `pre-commit install`
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
 show how to get started with the `unstructured` library. You can parse **TXT**,
-**HTML**, **PDF**, **EML**, **MSG**, **EPUB**, **DOC**, **DOCX**, **PPT**,
-**PPTX**, **JPG**, and **PNG** documents with one line of code!
+**HTML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
+**PPT**, **PPTX**, **JPG**, and **PNG** documents with one line of code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
@@ -208,9 +218,9 @@
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.7.0 Description-Content-Type:
 text/markdown Provides-Extra: huggingface Provides-Extra: local-inference
 Provides-Extra: s3 Provides-Extra: azure Provides-Extra: github Provides-Extra:
-gitlab Provides-Extra: reddit Provides-Extra: wikipedia Provides-Extra: google-
-drive
+gitlab Provides-Extra: reddit Provides-Extra: slack Provides-Extra: wikipedia
+Provides-Extra: google-drive
```

### Comparing `unstructured-0.5.9/unstructured.egg-info/SOURCES.txt` & `unstructured-0.6.0/unstructured.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 unstructured/ingest/connector/git.py
 unstructured/ingest/connector/github.py
 unstructured/ingest/connector/gitlab.py
 unstructured/ingest/connector/google_drive.py
 unstructured/ingest/connector/local.py
 unstructured/ingest/connector/reddit.py
 unstructured/ingest/connector/s3.py
+unstructured/ingest/connector/slack.py
 unstructured/ingest/connector/wikipedia.py
 unstructured/ingest/doc_processor/__init__.py
 unstructured/ingest/doc_processor/generalized.py
 unstructured/models/__init__.py
 unstructured/nlp/__init__.py
 unstructured/nlp/english-words.txt
 unstructured/nlp/english_words.py
@@ -70,14 +71,15 @@
 unstructured/partition/image.py
 unstructured/partition/json.py
 unstructured/partition/md.py
 unstructured/partition/msg.py
 unstructured/partition/pdf.py
 unstructured/partition/ppt.py
 unstructured/partition/pptx.py
+unstructured/partition/rtf.py
 unstructured/partition/text.py
 unstructured/partition/text_type.py
 unstructured/staging/__init__.py
 unstructured/staging/argilla.py
 unstructured/staging/base.py
 unstructured/staging/datasaur.py
 unstructured/staging/huggingface.py
```

