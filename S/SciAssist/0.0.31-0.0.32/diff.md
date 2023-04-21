# Comparing `tmp/SciAssist-0.0.31.tar.gz` & `tmp/SciAssist-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciAssist-0.0.31.tar", last modified: Thu Apr 20 12:01:42 2023, max compression
+gzip compressed data, was "SciAssist-0.0.32.tar", last modified: Fri Apr 21 07:22:37 2023, max compression
```

## Comparing `SciAssist-0.0.31.tar` & `SciAssist-0.0.32.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.448026 SciAssist-0.0.31/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    21150 2022-09-28 02:29:12.000000 SciAssist-0.0.31/LICENSE
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       38 2022-09-28 02:29:12.000000 SciAssist-0.0.31/MANIFEST.in
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-20 12:01:42.448026 SciAssist-0.0.31/PKG-INFO
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6208 2022-11-05 13:55:02.000000 SciAssist-0.0.31/README.md
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1451 2023-04-20 12:01:26.000000 SciAssist-0.0.31/pyproject.toml
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      635 2023-04-20 12:01:42.448026 SciAssist-0.0.31/setup.cfg
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       96 2022-09-28 02:29:12.000000 SciAssist-0.0.31/setup.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/SciAssist/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      818 2023-04-14 07:10:04.000000 SciAssist-0.0.31/src/SciAssist/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/SciAssist/bin/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      668 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.440025 SciAssist-0.0.31/src/SciAssist/bin/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      916 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.440025 SciAssist-0.0.31/src/SciAssist/bin/doc2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    11558 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/LICENSE
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.440025 SciAssist-0.0.31/src/SciAssist/bin/doc2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      158 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.440025 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.440025 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      167 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      227 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/__pycache__/config.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    15546 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       59 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/config.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.440025 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.440025 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      179 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2874 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    15434 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.440025 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4449 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.440025 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      186 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6183 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5972 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6614 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1019 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2736 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     9058 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        8 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/pdf_to_tei.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3622 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    27209 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    16382 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/s2orc.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.440025 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.440025 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      173 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2743 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8839 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3531 2023-03-15 13:25:23.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3144 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    11737 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6935 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4235 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      585 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.440025 SciAssist-0.0.31/src/SciAssist/bin/doc2json/scripts/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       73 2022-10-04 11:07:26.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      751 2022-10-04 11:09:22.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      275 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/bin/doc2json/setup.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.444026 SciAssist-0.0.31/src/SciAssist/datamodules/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/datamodules/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4113 2023-03-26 03:08:44.000000 SciAssist-0.0.31/src/SciAssist/datamodules/acl_datamodule.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.444026 SciAssist-0.0.31/src/SciAssist/datamodules/components/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/datamodules/components/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      370 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/datamodules/components/cora_label.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3112 2022-11-05 13:55:02.000000 SciAssist-0.0.31/src/SciAssist/datamodules/cora_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3357 2023-04-14 07:10:04.000000 SciAssist-0.0.31/src/SciAssist/datamodules/dataset_extraction_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3198 2022-11-10 14:45:14.000000 SciAssist-0.0.31/src/SciAssist/datamodules/fid_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2948 2022-11-27 14:04:32.000000 SciAssist-0.0.31/src/SciAssist/datamodules/general_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4331 2022-12-14 08:45:15.000000 SciAssist-0.0.31/src/SciAssist/datamodules/longsumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3179 2023-04-02 03:32:15.000000 SciAssist-0.0.31/src/SciAssist/datamodules/mup_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     7753 2023-03-18 16:34:11.000000 SciAssist-0.0.31/src/SciAssist/datamodules/mup_mup_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6978 2023-04-20 07:49:03.000000 SciAssist-0.0.31/src/SciAssist/datamodules/mup_scisumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5865 2023-04-14 07:09:42.000000 SciAssist-0.0.31/src/SciAssist/datamodules/scisumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4850 2023-02-23 16:55:34.000000 SciAssist-0.0.31/src/SciAssist/datamodules/test_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4211 2022-12-18 15:08:30.000000 SciAssist-0.0.31/src/SciAssist/datamodules/xsum_datamodule.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.444026 SciAssist-0.0.31/src/SciAssist/models/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/models/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.444026 SciAssist-0.0.31/src/SciAssist/models/components/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/models/components/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1554 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/models/components/bart_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2845 2023-04-14 07:10:04.000000 SciAssist-0.0.31/src/SciAssist/models/components/bert_dataset_extraction.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1547 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/models/components/bert_token_classifier.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    10090 2022-12-05 04:05:34.000000 SciAssist-0.0.31/src/SciAssist/models/components/fid_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1728 2023-04-17 15:52:16.000000 SciAssist-0.0.31/src/SciAssist/models/components/flant5_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1565 2022-11-21 03:52:20.000000 SciAssist-0.0.31/src/SciAssist/models/components/frost_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1590 2022-11-08 07:42:28.000000 SciAssist-0.0.31/src/SciAssist/models/components/longt5_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6869 2022-11-19 15:12:24.000000 SciAssist-0.0.31/src/SciAssist/models/cora_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8632 2023-04-14 07:10:04.000000 SciAssist-0.0.31/src/SciAssist/models/dataset_extraction_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13319 2023-04-02 03:32:15.000000 SciAssist-0.0.31/src/SciAssist/models/mup_bart_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     7880 2022-11-15 05:02:37.000000 SciAssist-0.0.31/src/SciAssist/models/mup_fid_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8141 2023-04-14 07:09:36.000000 SciAssist-0.0.31/src/SciAssist/models/mup_frost_module.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.444026 SciAssist-0.0.31/src/SciAssist/pipelines/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4287 2023-04-17 02:07:27.000000 SciAssist-0.0.31/src/SciAssist/pipelines/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    12872 2023-04-14 07:10:04.000000 SciAssist-0.0.31/src/SciAssist/pipelines/dataset_extraction.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2056 2022-11-05 13:55:02.000000 SciAssist-0.0.31/src/SciAssist/pipelines/pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13826 2022-11-05 13:55:02.000000 SciAssist-0.0.31/src/SciAssist/pipelines/reference_string_parsing.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    14701 2023-04-20 11:53:19.000000 SciAssist-0.0.31/src/SciAssist/pipelines/summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    12861 2023-04-14 07:08:00.000000 SciAssist-0.0.31/src/SciAssist/pipelines/summarization_origin.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1950 2023-02-20 05:27:12.000000 SciAssist-0.0.31/src/SciAssist/pipelines/testing_pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4003 2022-11-05 13:55:02.000000 SciAssist-0.0.31/src/SciAssist/pipelines/training_pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      786 2022-09-28 02:29:12.000000 SciAssist-0.0.31/src/SciAssist/test.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2022-10-02 15:49:40.000000 SciAssist-0.0.31/src/SciAssist/train.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2852 2022-11-27 16:49:31.000000 SciAssist-0.0.31/src/SciAssist/training_args.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.444026 SciAssist-0.0.31/src/SciAssist/utils/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4733 2023-02-03 14:21:07.000000 SciAssist-0.0.31/src/SciAssist/utils/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2714 2023-03-25 10:51:15.000000 SciAssist-0.0.31/src/SciAssist/utils/acl.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.444026 SciAssist-0.0.31/src/SciAssist/utils/collators/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2323 2022-11-10 14:30:40.000000 SciAssist-0.0.31/src/SciAssist/utils/collators/CollatorForFid.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-11-06 14:22:00.000000 SciAssist-0.0.31/src/SciAssist/utils/collators/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1232 2023-01-11 16:34:32.000000 SciAssist-0.0.31/src/SciAssist/utils/data_reader.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    75574 2023-04-20 07:47:38.000000 SciAssist-0.0.31/src/SciAssist/utils/data_utils.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    60999 2023-04-14 06:53:22.000000 SciAssist-0.0.31/src/SciAssist/utils/data_utils2.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1751 2023-03-01 06:47:44.000000 SciAssist-0.0.31/src/SciAssist/utils/evaluate_sr.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      661 2023-03-25 10:26:12.000000 SciAssist-0.0.31/src/SciAssist/utils/extract_acl.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5324 2023-03-30 02:58:27.000000 SciAssist-0.0.31/src/SciAssist/utils/extract_keysents.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3124 2023-04-20 07:43:17.000000 SciAssist-0.0.31/src/SciAssist/utils/extract_keywords.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2837 2023-04-19 13:38:32.000000 SciAssist-0.0.31/src/SciAssist/utils/extract_keywords_flant5.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1573 2023-03-19 09:05:48.000000 SciAssist-0.0.31/src/SciAssist/utils/extract_keywords_tfidf.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1703 2023-04-05 08:45:37.000000 SciAssist-0.0.31/src/SciAssist/utils/extract_keywords_yake.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5041 2023-03-25 10:36:56.000000 SciAssist-0.0.31/src/SciAssist/utils/pdf2text.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1502 2023-03-07 08:47:10.000000 SciAssist-0.0.31/src/SciAssist/utils/testset.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2261 2023-03-27 00:48:06.000000 SciAssist-0.0.31/src/SciAssist/utils/windows_pdf2text.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1499 2023-03-22 11:40:06.000000 SciAssist-0.0.31/src/SciAssist/utils/xml2txt.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/SciAssist.egg-info/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-20 12:01:42.000000 SciAssist-0.0.31/src/SciAssist.egg-info/PKG-INFO
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5886 2023-04-20 12:01:42.000000 SciAssist-0.0.31/src/SciAssist.egg-info/SOURCES.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        1 2023-04-20 12:01:42.000000 SciAssist-0.0.31/src/SciAssist.egg-info/dependency_links.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       98 2023-04-20 12:01:42.000000 SciAssist-0.0.31/src/SciAssist.egg-info/entry_points.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      396 2023-04-20 12:01:42.000000 SciAssist-0.0.31/src/SciAssist.egg-info/requires.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       70 2023-04-20 12:01:42.000000 SciAssist-0.0.31/src/SciAssist.egg-info/top_level.txt
--rwxrwxr-x   0 yixi      (1025) yixi      (1027)     1321 2023-03-05 16:03:26.000000 SciAssist-0.0.31/src/chatsonic.py
--rwxrwxr-x   0 yixi      (1025) yixi      (1027)     7944 2022-12-04 10:40:25.000000 SciAssist-0.0.31/src/convert_pegasus.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/latest-run/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/latest-run/files/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/latest-run/files/code/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.444026 SciAssist-0.0.31/src/logs/wandb/latest-run/files/code/SciAssist/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2023-04-20 07:50:06.000000 SciAssist-0.0.31/src/logs/wandb/latest-run/files/code/SciAssist/train.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230417_155336-2z994gwy/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230417_155336-2z994gwy/files/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230417_155336-2z994gwy/files/code/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.444026 SciAssist-0.0.31/src/logs/wandb/run-20230417_155336-2z994gwy/files/code/SciAssist/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2023-04-17 15:53:37.000000 SciAssist-0.0.31/src/logs/wandb/run-20230417_155336-2z994gwy/files/code/SciAssist/train.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230417_155949-31z04vyy/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230417_155949-31z04vyy/files/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230417_155949-31z04vyy/files/code/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.444026 SciAssist-0.0.31/src/logs/wandb/run-20230417_155949-31z04vyy/files/code/SciAssist/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2023-04-17 15:59:50.000000 SciAssist-0.0.31/src/logs/wandb/run-20230417_155949-31z04vyy/files/code/SciAssist/train.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230417_160829-2urucygj/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230417_160829-2urucygj/files/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230417_160829-2urucygj/files/code/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.444026 SciAssist-0.0.31/src/logs/wandb/run-20230417_160829-2urucygj/files/code/SciAssist/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2023-04-17 16:08:30.000000 SciAssist-0.0.31/src/logs/wandb/run-20230417_160829-2urucygj/files/code/SciAssist/train.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230417_160931-2nx959kb/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230417_160931-2nx959kb/files/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230417_160931-2nx959kb/files/code/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.448026 SciAssist-0.0.31/src/logs/wandb/run-20230417_160931-2nx959kb/files/code/SciAssist/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2023-04-17 16:09:32.000000 SciAssist-0.0.31/src/logs/wandb/run-20230417_160931-2nx959kb/files/code/SciAssist/train.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230420_075005-2k1zl74s/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230420_075005-2k1zl74s/files/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.436025 SciAssist-0.0.31/src/logs/wandb/run-20230420_075005-2k1zl74s/files/code/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.448026 SciAssist-0.0.31/src/logs/wandb/run-20230420_075005-2k1zl74s/files/code/SciAssist/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2023-04-20 07:50:06.000000 SciAssist-0.0.31/src/logs/wandb/run-20230420_075005-2k1zl74s/files/code/SciAssist/train.py
--rwxrwxr-x   0 yixi      (1025) yixi      (1027)      690 2022-12-10 17:44:58.000000 SciAssist-0.0.31/src/process.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-20 12:01:42.448026 SciAssist-0.0.31/tests/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1095 2022-12-11 12:29:46.000000 SciAssist-0.0.31/tests/test_rsp.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1129 2022-12-11 12:29:46.000000 SciAssist-0.0.31/tests/test_summ.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.284450 SciAssist-0.0.32/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    21150 2022-09-28 02:29:12.000000 SciAssist-0.0.32/LICENSE
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       38 2022-09-28 02:29:12.000000 SciAssist-0.0.32/MANIFEST.in
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-21 07:22:37.284450 SciAssist-0.0.32/PKG-INFO
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6208 2022-11-05 13:55:02.000000 SciAssist-0.0.32/README.md
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1451 2023-04-21 07:21:37.000000 SciAssist-0.0.32/pyproject.toml
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      635 2023-04-21 07:22:37.284450 SciAssist-0.0.32/setup.cfg
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       96 2022-09-28 02:29:12.000000 SciAssist-0.0.32/setup.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/SciAssist/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      818 2023-04-14 07:10:04.000000 SciAssist-0.0.32/src/SciAssist/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.276450 SciAssist-0.0.32/src/SciAssist/bin/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      668 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.276450 SciAssist-0.0.32/src/SciAssist/bin/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      916 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.276450 SciAssist-0.0.32/src/SciAssist/bin/doc2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    11558 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/LICENSE
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.276450 SciAssist-0.0.32/src/SciAssist/bin/doc2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      158 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.276450 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.276450 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      167 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      227 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/__pycache__/config.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    15546 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       59 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/config.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.276450 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.276450 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      179 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2874 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    15434 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.276450 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4449 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.276450 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      186 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6183 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5972 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6614 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1019 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2736 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     9058 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        8 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/pdf_to_tei.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3622 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    27209 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    16382 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/s2orc.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.276450 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.276450 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      173 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2743 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8839 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3531 2023-03-15 13:25:23.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3144 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    11737 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6935 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4235 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      585 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.276450 SciAssist-0.0.32/src/SciAssist/bin/doc2json/scripts/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       73 2022-10-04 11:07:26.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      751 2022-10-04 11:09:22.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      275 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/bin/doc2json/setup.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.280450 SciAssist-0.0.32/src/SciAssist/datamodules/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/datamodules/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4113 2023-03-26 03:08:44.000000 SciAssist-0.0.32/src/SciAssist/datamodules/acl_datamodule.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.280450 SciAssist-0.0.32/src/SciAssist/datamodules/components/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/datamodules/components/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      370 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/datamodules/components/cora_label.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3112 2022-11-05 13:55:02.000000 SciAssist-0.0.32/src/SciAssist/datamodules/cora_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3357 2023-04-14 07:10:04.000000 SciAssist-0.0.32/src/SciAssist/datamodules/dataset_extraction_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3198 2022-11-10 14:45:14.000000 SciAssist-0.0.32/src/SciAssist/datamodules/fid_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2948 2022-11-27 14:04:32.000000 SciAssist-0.0.32/src/SciAssist/datamodules/general_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4331 2022-12-14 08:45:15.000000 SciAssist-0.0.32/src/SciAssist/datamodules/longsumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3179 2023-04-02 03:32:15.000000 SciAssist-0.0.32/src/SciAssist/datamodules/mup_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     7753 2023-03-18 16:34:11.000000 SciAssist-0.0.32/src/SciAssist/datamodules/mup_mup_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6978 2023-04-20 07:49:03.000000 SciAssist-0.0.32/src/SciAssist/datamodules/mup_scisumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5865 2023-04-14 07:09:42.000000 SciAssist-0.0.32/src/SciAssist/datamodules/scisumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4850 2023-02-23 16:55:34.000000 SciAssist-0.0.32/src/SciAssist/datamodules/test_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4211 2022-12-18 15:08:30.000000 SciAssist-0.0.32/src/SciAssist/datamodules/xsum_datamodule.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.280450 SciAssist-0.0.32/src/SciAssist/models/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/models/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.280450 SciAssist-0.0.32/src/SciAssist/models/components/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/models/components/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1554 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/models/components/bart_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2845 2023-04-14 07:10:04.000000 SciAssist-0.0.32/src/SciAssist/models/components/bert_dataset_extraction.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1547 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/models/components/bert_token_classifier.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    10090 2022-12-05 04:05:34.000000 SciAssist-0.0.32/src/SciAssist/models/components/fid_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1728 2023-04-17 15:52:16.000000 SciAssist-0.0.32/src/SciAssist/models/components/flant5_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1565 2022-11-21 03:52:20.000000 SciAssist-0.0.32/src/SciAssist/models/components/frost_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1590 2022-11-08 07:42:28.000000 SciAssist-0.0.32/src/SciAssist/models/components/longt5_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6869 2022-11-19 15:12:24.000000 SciAssist-0.0.32/src/SciAssist/models/cora_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8632 2023-04-14 07:10:04.000000 SciAssist-0.0.32/src/SciAssist/models/dataset_extraction_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    13319 2023-04-02 03:32:15.000000 SciAssist-0.0.32/src/SciAssist/models/mup_bart_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     7880 2022-11-15 05:02:37.000000 SciAssist-0.0.32/src/SciAssist/models/mup_fid_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8141 2023-04-14 07:09:36.000000 SciAssist-0.0.32/src/SciAssist/models/mup_frost_module.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.280450 SciAssist-0.0.32/src/SciAssist/pipelines/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4266 2023-04-21 07:18:08.000000 SciAssist-0.0.32/src/SciAssist/pipelines/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    12872 2023-04-14 07:10:04.000000 SciAssist-0.0.32/src/SciAssist/pipelines/dataset_extraction.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2056 2022-11-05 13:55:02.000000 SciAssist-0.0.32/src/SciAssist/pipelines/pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    13826 2022-11-05 13:55:02.000000 SciAssist-0.0.32/src/SciAssist/pipelines/reference_string_parsing.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    14701 2023-04-20 11:53:19.000000 SciAssist-0.0.32/src/SciAssist/pipelines/summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    12861 2023-04-14 07:08:00.000000 SciAssist-0.0.32/src/SciAssist/pipelines/summarization_origin.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1950 2023-02-20 05:27:12.000000 SciAssist-0.0.32/src/SciAssist/pipelines/testing_pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4003 2022-11-05 13:55:02.000000 SciAssist-0.0.32/src/SciAssist/pipelines/training_pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      786 2022-09-28 02:29:12.000000 SciAssist-0.0.32/src/SciAssist/test.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2022-10-02 15:49:40.000000 SciAssist-0.0.32/src/SciAssist/train.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2852 2022-11-27 16:49:31.000000 SciAssist-0.0.32/src/SciAssist/training_args.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.284450 SciAssist-0.0.32/src/SciAssist/utils/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4733 2023-02-03 14:21:07.000000 SciAssist-0.0.32/src/SciAssist/utils/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2714 2023-03-25 10:51:15.000000 SciAssist-0.0.32/src/SciAssist/utils/acl.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.284450 SciAssist-0.0.32/src/SciAssist/utils/collators/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2323 2022-11-10 14:30:40.000000 SciAssist-0.0.32/src/SciAssist/utils/collators/CollatorForFid.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-11-06 14:22:00.000000 SciAssist-0.0.32/src/SciAssist/utils/collators/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1232 2023-01-11 16:34:32.000000 SciAssist-0.0.32/src/SciAssist/utils/data_reader.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    75574 2023-04-20 07:47:38.000000 SciAssist-0.0.32/src/SciAssist/utils/data_utils.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    60999 2023-04-14 06:53:22.000000 SciAssist-0.0.32/src/SciAssist/utils/data_utils2.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1751 2023-03-01 06:47:44.000000 SciAssist-0.0.32/src/SciAssist/utils/evaluate_sr.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      661 2023-03-25 10:26:12.000000 SciAssist-0.0.32/src/SciAssist/utils/extract_acl.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5324 2023-03-30 02:58:27.000000 SciAssist-0.0.32/src/SciAssist/utils/extract_keysents.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3124 2023-04-20 07:43:17.000000 SciAssist-0.0.32/src/SciAssist/utils/extract_keywords.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2837 2023-04-19 13:38:32.000000 SciAssist-0.0.32/src/SciAssist/utils/extract_keywords_flant5.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1573 2023-03-19 09:05:48.000000 SciAssist-0.0.32/src/SciAssist/utils/extract_keywords_tfidf.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1703 2023-04-05 08:45:37.000000 SciAssist-0.0.32/src/SciAssist/utils/extract_keywords_yake.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5041 2023-03-25 10:36:56.000000 SciAssist-0.0.32/src/SciAssist/utils/pdf2text.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1502 2023-03-07 08:47:10.000000 SciAssist-0.0.32/src/SciAssist/utils/testset.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2261 2023-03-27 00:48:06.000000 SciAssist-0.0.32/src/SciAssist/utils/windows_pdf2text.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1499 2023-03-22 11:40:06.000000 SciAssist-0.0.32/src/SciAssist/utils/xml2txt.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/SciAssist.egg-info/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-21 07:22:37.000000 SciAssist-0.0.32/src/SciAssist.egg-info/PKG-INFO
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5886 2023-04-21 07:22:37.000000 SciAssist-0.0.32/src/SciAssist.egg-info/SOURCES.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        1 2023-04-21 07:22:37.000000 SciAssist-0.0.32/src/SciAssist.egg-info/dependency_links.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       98 2023-04-21 07:22:37.000000 SciAssist-0.0.32/src/SciAssist.egg-info/entry_points.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      396 2023-04-21 07:22:37.000000 SciAssist-0.0.32/src/SciAssist.egg-info/requires.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       70 2023-04-21 07:22:37.000000 SciAssist-0.0.32/src/SciAssist.egg-info/top_level.txt
+-rwxrwxr-x   0 yixi      (1025) yixi      (1027)     1321 2023-03-05 16:03:26.000000 SciAssist-0.0.32/src/chatsonic.py
+-rwxrwxr-x   0 yixi      (1025) yixi      (1027)     7944 2022-12-04 10:40:25.000000 SciAssist-0.0.32/src/convert_pegasus.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/latest-run/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/latest-run/files/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/latest-run/files/code/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.284450 SciAssist-0.0.32/src/logs/wandb/latest-run/files/code/SciAssist/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2023-04-20 07:50:06.000000 SciAssist-0.0.32/src/logs/wandb/latest-run/files/code/SciAssist/train.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230417_155336-2z994gwy/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230417_155336-2z994gwy/files/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230417_155336-2z994gwy/files/code/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.284450 SciAssist-0.0.32/src/logs/wandb/run-20230417_155336-2z994gwy/files/code/SciAssist/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2023-04-17 15:53:37.000000 SciAssist-0.0.32/src/logs/wandb/run-20230417_155336-2z994gwy/files/code/SciAssist/train.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230417_155949-31z04vyy/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230417_155949-31z04vyy/files/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230417_155949-31z04vyy/files/code/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.284450 SciAssist-0.0.32/src/logs/wandb/run-20230417_155949-31z04vyy/files/code/SciAssist/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2023-04-17 15:59:50.000000 SciAssist-0.0.32/src/logs/wandb/run-20230417_155949-31z04vyy/files/code/SciAssist/train.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230417_160829-2urucygj/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230417_160829-2urucygj/files/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230417_160829-2urucygj/files/code/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.284450 SciAssist-0.0.32/src/logs/wandb/run-20230417_160829-2urucygj/files/code/SciAssist/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2023-04-17 16:08:30.000000 SciAssist-0.0.32/src/logs/wandb/run-20230417_160829-2urucygj/files/code/SciAssist/train.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230417_160931-2nx959kb/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230417_160931-2nx959kb/files/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230417_160931-2nx959kb/files/code/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.284450 SciAssist-0.0.32/src/logs/wandb/run-20230417_160931-2nx959kb/files/code/SciAssist/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2023-04-17 16:09:32.000000 SciAssist-0.0.32/src/logs/wandb/run-20230417_160931-2nx959kb/files/code/SciAssist/train.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230420_075005-2k1zl74s/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230420_075005-2k1zl74s/files/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.272450 SciAssist-0.0.32/src/logs/wandb/run-20230420_075005-2k1zl74s/files/code/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.284450 SciAssist-0.0.32/src/logs/wandb/run-20230420_075005-2k1zl74s/files/code/SciAssist/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2023-04-20 07:50:06.000000 SciAssist-0.0.32/src/logs/wandb/run-20230420_075005-2k1zl74s/files/code/SciAssist/train.py
+-rwxrwxr-x   0 yixi      (1025) yixi      (1027)      690 2022-12-10 17:44:58.000000 SciAssist-0.0.32/src/process.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-21 07:22:37.284450 SciAssist-0.0.32/tests/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1095 2022-12-11 12:29:46.000000 SciAssist-0.0.32/tests/test_rsp.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1129 2022-12-11 12:29:46.000000 SciAssist-0.0.32/tests/test_summ.py
```

### Comparing `SciAssist-0.0.31/LICENSE` & `SciAssist-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/PKG-INFO` & `SciAssist-0.0.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciAssist
-Version: 0.0.31
+Version: 0.0.32
 Summary: A toolkit for Scientific Document Processing
 Author-email: WING-NUS <dingyixi@hotmail.com>
 Maintainer-email: Yixi Ding <dingyixi@hotmail.com>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `SciAssist-0.0.31/README.md` & `SciAssist-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/pyproject.toml` & `SciAssist-0.0.32/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SciAssist"
-version = "0.0.31"
+version = "0.0.32"
 authors = [
   { name="WING-NUS", email="dingyixi@hotmail.com" },
 ]
 maintainers = [
   { name="Yixi Ding", email="dingyixi@hotmail.com" },
 ]
 description = "A toolkit for Scientific Document Processing"
```

### Comparing `SciAssist-0.0.31/setup.cfg` & `SciAssist-0.0.32/setup.cfg`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/__init__.py` & `SciAssist-0.0.32/src/SciAssist/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/__init__.py` & `SciAssist-0.0.32/src/SciAssist/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc` & `SciAssist-0.0.32/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/LICENSE` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/LICENSE`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/s2orc.py` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/s2orc.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh` & `SciAssist-0.0.32/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/datamodules/acl_datamodule.py` & `SciAssist-0.0.32/src/SciAssist/datamodules/acl_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/datamodules/cora_datamodule.py` & `SciAssist-0.0.32/src/SciAssist/datamodules/cora_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/datamodules/dataset_extraction_datamodule.py` & `SciAssist-0.0.32/src/SciAssist/datamodules/dataset_extraction_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/datamodules/fid_datamodule.py` & `SciAssist-0.0.32/src/SciAssist/datamodules/fid_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/datamodules/general_datamodule.py` & `SciAssist-0.0.32/src/SciAssist/datamodules/general_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/datamodules/longsumm_datamodule.py` & `SciAssist-0.0.32/src/SciAssist/datamodules/longsumm_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/datamodules/mup_datamodule.py` & `SciAssist-0.0.32/src/SciAssist/datamodules/mup_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/datamodules/mup_mup_datamodule.py` & `SciAssist-0.0.32/src/SciAssist/datamodules/mup_mup_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/datamodules/mup_scisumm_datamodule.py` & `SciAssist-0.0.32/src/SciAssist/datamodules/mup_scisumm_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/datamodules/scisumm_datamodule.py` & `SciAssist-0.0.32/src/SciAssist/datamodules/scisumm_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/datamodules/test_datamodule.py` & `SciAssist-0.0.32/src/SciAssist/datamodules/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/datamodules/xsum_datamodule.py` & `SciAssist-0.0.32/src/SciAssist/datamodules/xsum_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/models/components/bart_summarization.py` & `SciAssist-0.0.32/src/SciAssist/models/components/bart_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/models/components/bert_dataset_extraction.py` & `SciAssist-0.0.32/src/SciAssist/models/components/bert_dataset_extraction.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/models/components/bert_token_classifier.py` & `SciAssist-0.0.32/src/SciAssist/models/components/bert_token_classifier.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/models/components/fid_summarization.py` & `SciAssist-0.0.32/src/SciAssist/models/components/fid_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/models/components/flant5_summarization.py` & `SciAssist-0.0.32/src/SciAssist/models/components/flant5_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/models/components/frost_summarization.py` & `SciAssist-0.0.32/src/SciAssist/models/components/frost_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/models/components/longt5_summarization.py` & `SciAssist-0.0.32/src/SciAssist/models/components/longt5_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/models/cora_module.py` & `SciAssist-0.0.32/src/SciAssist/models/cora_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/models/dataset_extraction_module.py` & `SciAssist-0.0.32/src/SciAssist/models/dataset_extraction_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/models/mup_bart_module.py` & `SciAssist-0.0.32/src/SciAssist/models/mup_bart_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/models/mup_fid_module.py` & `SciAssist-0.0.32/src/SciAssist/models/mup_fid_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/models/mup_frost_module.py` & `SciAssist-0.0.32/src/SciAssist/models/mup_frost_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/pipelines/__init__.py` & `SciAssist-0.0.32/src/SciAssist/pipelines/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # main developer: Yixi Ding <dingyixi@hotmail.com>
 
 from typing import Dict
 
 import torch
 
 from SciAssist import BASE_CACHE_DIR
+from SciAssist.models.components.bert_dataset_extraction import BertForDatasetExtraction
 from SciAssist.models.components.bert_token_classifier import BertForTokenClassifier
 from SciAssist.models.components.flant5_summarization import FlanT5ForSummarization
-from SciAssist.models.components.bert_dataset_extraction import BertForDatasetExtraction
 from SciAssist.utils.data_utils import (
     DataUtilsForTokenClassification,
-    DataUtilsForSeq2Seq, DataUtilsForFlanT5, DataUtilsForT5,
+    DataUtilsForFlanT5, DataUtilsForT5,
     DataUtilsForSeq2Seq,
     DataUtilsForDatasetExtraction
 )
 
 # Provided models for each task
 TASKS = {
     "reference-string-parsing": {
@@ -60,15 +60,15 @@
             # "model_dict_url": None,
             "data_utils": DataUtilsForFlanT5,
         }
     },
     "dataset-extraction": {
         "default": {
             "model": BertForDatasetExtraction,
-            "model_dict_url": "https://huggingface.co/spaces/wing-nus/SciAssist/resolve/main/dataset-extraction.pt",
+            "model_dict_url": "https://huggingface.co/spaces/kirinzhu/SciAssist/resolve/main/dataset_extraction.pt",
             "data_utils": DataUtilsForDatasetExtraction,
         },
     },
 
     # "controlled-summarization": {
     #     "default": {
     #         "model": FrostForSummarization,
```

### Comparing `SciAssist-0.0.31/src/SciAssist/pipelines/dataset_extraction.py` & `SciAssist-0.0.32/src/SciAssist/pipelines/dataset_extraction.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/pipelines/pipeline.py` & `SciAssist-0.0.32/src/SciAssist/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/pipelines/reference_string_parsing.py` & `SciAssist-0.0.32/src/SciAssist/pipelines/reference_string_parsing.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/pipelines/summarization.py` & `SciAssist-0.0.32/src/SciAssist/pipelines/summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/pipelines/summarization_origin.py` & `SciAssist-0.0.32/src/SciAssist/pipelines/summarization_origin.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/pipelines/testing_pipeline.py` & `SciAssist-0.0.32/src/SciAssist/pipelines/testing_pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/pipelines/training_pipeline.py` & `SciAssist-0.0.32/src/SciAssist/pipelines/training_pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/test.py` & `SciAssist-0.0.32/src/SciAssist/test.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/train.py` & `SciAssist-0.0.32/src/SciAssist/train.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/training_args.py` & `SciAssist-0.0.32/src/SciAssist/training_args.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/__init__.py` & `SciAssist-0.0.32/src/SciAssist/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/acl.py` & `SciAssist-0.0.32/src/SciAssist/utils/acl.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/collators/CollatorForFid.py` & `SciAssist-0.0.32/src/SciAssist/utils/collators/CollatorForFid.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/data_reader.py` & `SciAssist-0.0.32/src/SciAssist/utils/data_reader.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/data_utils.py` & `SciAssist-0.0.32/src/SciAssist/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/data_utils2.py` & `SciAssist-0.0.32/src/SciAssist/utils/data_utils2.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/evaluate_sr.py` & `SciAssist-0.0.32/src/SciAssist/utils/evaluate_sr.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/extract_acl.py` & `SciAssist-0.0.32/src/SciAssist/utils/extract_acl.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/extract_keysents.py` & `SciAssist-0.0.32/src/SciAssist/utils/extract_keysents.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/extract_keywords.py` & `SciAssist-0.0.32/src/SciAssist/utils/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/extract_keywords_flant5.py` & `SciAssist-0.0.32/src/SciAssist/utils/extract_keywords_flant5.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/extract_keywords_tfidf.py` & `SciAssist-0.0.32/src/SciAssist/utils/extract_keywords_tfidf.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/extract_keywords_yake.py` & `SciAssist-0.0.32/src/SciAssist/utils/extract_keywords_yake.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/pdf2text.py` & `SciAssist-0.0.32/src/SciAssist/utils/pdf2text.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/testset.py` & `SciAssist-0.0.32/src/SciAssist/utils/testset.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/windows_pdf2text.py` & `SciAssist-0.0.32/src/SciAssist/utils/windows_pdf2text.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist/utils/xml2txt.py` & `SciAssist-0.0.32/src/SciAssist/utils/xml2txt.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/SciAssist.egg-info/PKG-INFO` & `SciAssist-0.0.32/src/SciAssist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciAssist
-Version: 0.0.31
+Version: 0.0.32
 Summary: A toolkit for Scientific Document Processing
 Author-email: WING-NUS <dingyixi@hotmail.com>
 Maintainer-email: Yixi Ding <dingyixi@hotmail.com>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `SciAssist-0.0.31/src/SciAssist.egg-info/SOURCES.txt` & `SciAssist-0.0.32/src/SciAssist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/chatsonic.py` & `SciAssist-0.0.32/src/chatsonic.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/convert_pegasus.py` & `SciAssist-0.0.32/src/convert_pegasus.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/logs/wandb/latest-run/files/code/SciAssist/train.py` & `SciAssist-0.0.32/src/logs/wandb/latest-run/files/code/SciAssist/train.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/logs/wandb/run-20230417_155336-2z994gwy/files/code/SciAssist/train.py` & `SciAssist-0.0.32/src/logs/wandb/run-20230417_155336-2z994gwy/files/code/SciAssist/train.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/logs/wandb/run-20230417_155949-31z04vyy/files/code/SciAssist/train.py` & `SciAssist-0.0.32/src/logs/wandb/run-20230417_155949-31z04vyy/files/code/SciAssist/train.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/logs/wandb/run-20230417_160829-2urucygj/files/code/SciAssist/train.py` & `SciAssist-0.0.32/src/logs/wandb/run-20230417_160829-2urucygj/files/code/SciAssist/train.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/logs/wandb/run-20230417_160931-2nx959kb/files/code/SciAssist/train.py` & `SciAssist-0.0.32/src/logs/wandb/run-20230417_160931-2nx959kb/files/code/SciAssist/train.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/logs/wandb/run-20230420_075005-2k1zl74s/files/code/SciAssist/train.py` & `SciAssist-0.0.32/src/logs/wandb/run-20230420_075005-2k1zl74s/files/code/SciAssist/train.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/src/process.py` & `SciAssist-0.0.32/src/process.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/tests/test_rsp.py` & `SciAssist-0.0.32/tests/test_rsp.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.31/tests/test_summ.py` & `SciAssist-0.0.32/tests/test_summ.py`

 * *Files identical despite different names*

