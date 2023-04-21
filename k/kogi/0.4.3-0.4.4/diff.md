# Comparing `tmp/kogi-0.4.3.tar.gz` & `tmp/kogi-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kogi-0.4.3.tar", last modified: Mon Apr 17 03:42:33 2023, max compression
+gzip compressed data, was "kogi-0.4.4.tar", last modified: Fri Apr 21 12:24:08 2023, max compression
```

## Comparing `kogi-0.4.3.tar` & `kogi-0.4.4.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.676872 kogi-0.4.3/
--rw-r--r--   0 kimio      (501) staff       (20)      602 2023-04-17 03:42:33.676576 kogi-0.4.3/PKG-INFO
--rw-r--r--   0 kimio      (501) staff       (20)       27 2023-04-17 03:41:54.000000 kogi-0.4.3/README.md
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.636895 kogi-0.4.3/kogi/
--rw-r--r--   0 kimio      (501) staff       (20)      235 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/__init__.py
--rw-r--r--   0 kimio      (501) staff       (20)       86 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ai.py
--rw-r--r--   0 kimio      (501) staff       (20)       40 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/canvas.py
--rw-r--r--   0 kimio      (501) staff       (20)    10338 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/chat.py
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.640963 kogi-0.4.3/kogi/data/
--rw-r--r--   0 kimio      (501) staff       (20)      622 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/data/common_loader.py
--rw-r--r--   0 kimio      (501) staff       (20)      301 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/data/diagnosis_ja.py
--rw-r--r--   0 kimio      (501) staff       (20)    31773 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/data/diagnosis_ja.txt
--rw-r--r--   0 kimio      (501) staff       (20)    11255 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/data/error.txt
--rw-r--r--   0 kimio      (501) staff       (20)      670 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/data/error_desc.py
--rw-r--r--   0 kimio      (501) staff       (20)     3073 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/hook.py
--rw-r--r--   0 kimio      (501) staff       (20)      119 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/jwu2.py
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.644195 kogi-0.4.3/kogi/liberr/
--rw-r--r--   0 kimio      (501) staff       (20)      210 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/liberr/__init__.py
--rw-r--r--   0 kimio      (501) staff       (20)     5733 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/liberr/_extract_emsg.py
--rw-r--r--   0 kimio      (501) staff       (20)     7332 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/liberr/_traceback2.py
--rw-r--r--   0 kimio      (501) staff       (20)    28678 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/liberr/emsg_rules.tsv
--rw-r--r--   0 kimio      (501) staff       (20)     1490 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/liberr/extract_vars.py
--rw-r--r--   0 kimio      (501) staff       (20)     5170 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/liberr/rulebase.py
--rw-r--r--   0 kimio      (501) staff       (20)     5824 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/pan.py
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.647331 kogi-0.4.3/kogi/problem/
--rw-r--r--   0 kimio      (501) staff       (20)      847 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/problem/__init__.py
--rw-r--r--   0 kimio      (501) staff       (20)     1874 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/problem/atcoder.py
--rw-r--r--   0 kimio      (501) staff       (20)     2846 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/problem/drill.py
--rw-r--r--   0 kimio      (501) staff       (20)     2777 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/problem/judge.py
--rw-r--r--   0 kimio      (501) staff       (20)      346 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/problem/testdata.py
--rw-r--r--   0 kimio      (501) staff       (20)      681 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/problem/timeout.py
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.651896 kogi-0.4.3/kogi/service/
--rw-r--r--   0 kimio      (501) staff       (20)      792 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/__init__.py
--rw-r--r--   0 kimio      (501) staff       (20)     1535 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/chatgpt.py
--rw-r--r--   0 kimio      (501) staff       (20)     2892 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/flaskapi.py
--rw-r--r--   0 kimio      (501) staff       (20)     5901 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/flaskserv.py
--rw-r--r--   0 kimio      (501) staff       (20)      464 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/globals.py
--rw-r--r--   0 kimio      (501) staff       (20)     5027 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/huggingface.py
--rw-r--r--   0 kimio      (501) staff       (20)     2630 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/s3logging.py
--rw-r--r--   0 kimio      (501) staff       (20)      711 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/slack.py
--rw-r--r--   0 kimio      (501) staff       (20)     2027 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/textra.py
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.655371 kogi-0.4.3/kogi/task/
--rw-r--r--   0 kimio      (501) staff       (20)        0 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/task/__init__.py
--rw-r--r--   0 kimio      (501) staff       (20)       82 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/task/all.py
--rw-r--r--   0 kimio      (501) staff       (20)     2197 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/task/code.py
--rw-r--r--   0 kimio      (501) staff       (20)      264 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/task/common.py
--rw-r--r--   0 kimio      (501) staff       (20)     6997 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/task/diagnosis.py
--rw-r--r--   0 kimio      (501) staff       (20)      933 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/task/multi.py
--rw-r--r--   0 kimio      (501) staff       (20)     1936 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/task/runner.py
--rw-r--r--   0 kimio      (501) staff       (20)     5946 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/transform.py
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.675983 kogi-0.4.3/kogi/ui/
--rw-r--r--   0 kimio      (501) staff       (20)      373 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/__init__.py
--rw-r--r--   0 kimio      (501) staff       (20)    12317 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/_canvas.py
--rw-r--r--   0 kimio      (501) staff       (20)      110 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/_google.py
--rw-r--r--   0 kimio      (501) staff       (20)    40724 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/chatgpt-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)      931 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/content.py
--rw-r--r--   0 kimio      (501) staff       (20)     3973 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/dialog.css
--rw-r--r--   0 kimio      (501) staff       (20)     1697 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/dialog.html
--rw-r--r--   0 kimio      (501) staff       (20)      907 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/dialog.js
--rw-r--r--   0 kimio      (501) staff       (20)     2062 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/dialog_colab.py
--rw-r--r--   0 kimio      (501) staff       (20)     1371 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/dialog_ipywidgets.py
--rw-r--r--   0 kimio      (501) staff       (20)    42938 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/error-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)     7378 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/girl-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)    30227 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/girl_think-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)     5937 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/keylogin.py
--rw-r--r--   0 kimio      (501) staff       (20)     6629 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/kogi-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)    40724 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/kogi_doya-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)    42938 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/kogi_error-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)    48169 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/kogi_gaan-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)     8228 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/kogi_vow-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)      233 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/main.css
--rw-r--r--   0 kimio      (501) staff       (20)     4812 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/message.py
--rw-r--r--   0 kimio      (501) staff       (20)     6473 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/openai-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)     8080 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/render.py
--rw-r--r--   0 kimio      (501) staff       (20)     4397 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/rmt.py
--rw-r--r--   0 kimio      (501) staff       (20)     5914 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/robot-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)      652 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/slides.py
--rw-r--r--   0 kimio      (501) staff       (20)     4551 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/ta-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)      683 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/typewriter.py
--rw-r--r--   0 kimio      (501) staff       (20)     2073 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/wait_and_ready.py
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.638498 kogi-0.4.3/kogi.egg-info/
--rw-r--r--   0 kimio      (501) staff       (20)      602 2023-04-17 03:42:33.000000 kogi-0.4.3/kogi.egg-info/PKG-INFO
--rw-r--r--   0 kimio      (501) staff       (20)     1681 2023-04-17 03:42:33.000000 kogi-0.4.3/kogi.egg-info/SOURCES.txt
--rw-r--r--   0 kimio      (501) staff       (20)        1 2023-04-17 03:42:33.000000 kogi-0.4.3/kogi.egg-info/dependency_links.txt
--rw-r--r--   0 kimio      (501) staff       (20)       51 2023-04-17 03:42:33.000000 kogi-0.4.3/kogi.egg-info/requires.txt
--rw-r--r--   0 kimio      (501) staff       (20)        5 2023-04-17 03:42:33.000000 kogi-0.4.3/kogi.egg-info/top_level.txt
--rw-r--r--   0 kimio      (501) staff       (20)       38 2023-04-17 03:42:33.676962 kogi-0.4.3/setup.cfg
--rw-r--r--   0 kimio      (501) staff       (20)     1168 2023-04-17 03:41:54.000000 kogi-0.4.3/setup.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-21 12:24:08.541223 kogi-0.4.4/
+-rw-r--r--   0 kimio      (501) staff       (20)     1072 2023-04-21 11:17:52.000000 kogi-0.4.4/LICENSE
+-rw-r--r--   0 kimio      (501) staff       (20)      591 2023-04-21 12:24:08.541075 kogi-0.4.4/PKG-INFO
+-rw-r--r--   0 kimio      (501) staff       (20)       27 2023-04-21 11:17:52.000000 kogi-0.4.4/README.md
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-21 12:24:08.529099 kogi-0.4.4/kogi/
+-rw-r--r--   0 kimio      (501) staff       (20)      235 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/__init__.py
+-rw-r--r--   0 kimio      (501) staff       (20)       86 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ai.py
+-rw-r--r--   0 kimio      (501) staff       (20)       40 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/canvas.py
+-rw-r--r--   0 kimio      (501) staff       (20)    10150 2023-04-21 12:14:02.000000 kogi-0.4.4/kogi/chat.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-21 12:24:08.530625 kogi-0.4.4/kogi/data/
+-rw-r--r--   0 kimio      (501) staff       (20)      622 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/data/common_loader.py
+-rw-r--r--   0 kimio      (501) staff       (20)      301 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/data/diagnosis_ja.py
+-rw-r--r--   0 kimio      (501) staff       (20)    31773 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/data/diagnosis_ja.txt
+-rw-r--r--   0 kimio      (501) staff       (20)    11255 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/data/error.txt
+-rw-r--r--   0 kimio      (501) staff       (20)      670 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/data/error_desc.py
+-rw-r--r--   0 kimio      (501) staff       (20)     3073 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/hook.py
+-rw-r--r--   0 kimio      (501) staff       (20)       64 2023-04-21 11:23:05.000000 kogi-0.4.4/kogi/jwu.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-21 12:24:08.531624 kogi-0.4.4/kogi/liberr/
+-rw-r--r--   0 kimio      (501) staff       (20)      210 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/liberr/__init__.py
+-rw-r--r--   0 kimio      (501) staff       (20)     5733 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/liberr/_extract_emsg.py
+-rw-r--r--   0 kimio      (501) staff       (20)     7332 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/liberr/_traceback2.py
+-rw-r--r--   0 kimio      (501) staff       (20)    28678 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/liberr/emsg_rules.tsv
+-rw-r--r--   0 kimio      (501) staff       (20)     1490 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/liberr/extract_vars.py
+-rw-r--r--   0 kimio      (501) staff       (20)     5170 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/liberr/rulebase.py
+-rw-r--r--   0 kimio      (501) staff       (20)     5824 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/pan.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-21 12:24:08.532536 kogi-0.4.4/kogi/problem/
+-rw-r--r--   0 kimio      (501) staff       (20)      847 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/problem/__init__.py
+-rw-r--r--   0 kimio      (501) staff       (20)     1874 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/problem/atcoder.py
+-rw-r--r--   0 kimio      (501) staff       (20)     2846 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/problem/drill.py
+-rw-r--r--   0 kimio      (501) staff       (20)     2777 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/problem/judge.py
+-rw-r--r--   0 kimio      (501) staff       (20)      346 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/problem/testdata.py
+-rw-r--r--   0 kimio      (501) staff       (20)      681 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/problem/timeout.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-21 12:24:08.534044 kogi-0.4.4/kogi/service/
+-rw-r--r--   0 kimio      (501) staff       (20)      792 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/service/__init__.py
+-rw-r--r--   0 kimio      (501) staff       (20)     1548 2023-04-21 12:19:35.000000 kogi-0.4.4/kogi/service/chatgpt.py
+-rw-r--r--   0 kimio      (501) staff       (20)     2892 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/service/flaskapi.py
+-rw-r--r--   0 kimio      (501) staff       (20)     5901 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/service/flaskserv.py
+-rw-r--r--   0 kimio      (501) staff       (20)      464 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/service/globals.py
+-rw-r--r--   0 kimio      (501) staff       (20)     5027 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/service/huggingface.py
+-rw-r--r--   0 kimio      (501) staff       (20)     2630 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/service/s3logging.py
+-rw-r--r--   0 kimio      (501) staff       (20)      711 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/service/slack.py
+-rw-r--r--   0 kimio      (501) staff       (20)     2027 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/service/textra.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-21 12:24:08.535386 kogi-0.4.4/kogi/task/
+-rw-r--r--   0 kimio      (501) staff       (20)        0 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/task/__init__.py
+-rw-r--r--   0 kimio      (501) staff       (20)       82 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/task/all.py
+-rw-r--r--   0 kimio      (501) staff       (20)     2197 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/task/code.py
+-rw-r--r--   0 kimio      (501) staff       (20)      264 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/task/common.py
+-rw-r--r--   0 kimio      (501) staff       (20)     6997 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/task/diagnosis.py
+-rw-r--r--   0 kimio      (501) staff       (20)      933 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/task/multi.py
+-rw-r--r--   0 kimio      (501) staff       (20)     1936 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/task/runner.py
+-rw-r--r--   0 kimio      (501) staff       (20)     5946 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/transform.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-21 12:24:08.540823 kogi-0.4.4/kogi/ui/
+-rw-r--r--   0 kimio      (501) staff       (20)      373 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/__init__.py
+-rw-r--r--   0 kimio      (501) staff       (20)    12317 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/_canvas.py
+-rw-r--r--   0 kimio      (501) staff       (20)      110 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/_google.py
+-rw-r--r--   0 kimio      (501) staff       (20)    40724 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/chatgpt-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)      931 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/content.py
+-rw-r--r--   0 kimio      (501) staff       (20)     3973 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/dialog.css
+-rw-r--r--   0 kimio      (501) staff       (20)     1697 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/dialog.html
+-rw-r--r--   0 kimio      (501) staff       (20)      907 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/dialog.js
+-rw-r--r--   0 kimio      (501) staff       (20)     2062 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/dialog_colab.py
+-rw-r--r--   0 kimio      (501) staff       (20)     1371 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/dialog_ipywidgets.py
+-rw-r--r--   0 kimio      (501) staff       (20)    42938 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/error-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)     7378 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/girl-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)    30227 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/girl_think-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)     5937 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/keylogin.py
+-rw-r--r--   0 kimio      (501) staff       (20)     6629 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/kogi-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)    40724 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/kogi_doya-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)    42938 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/kogi_error-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)    48169 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/kogi_gaan-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)     8228 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/kogi_vow-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)      233 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/main.css
+-rw-r--r--   0 kimio      (501) staff       (20)     4812 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/message.py
+-rw-r--r--   0 kimio      (501) staff       (20)     6473 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/openai-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)     8080 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/render.py
+-rw-r--r--   0 kimio      (501) staff       (20)     4397 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/rmt.py
+-rw-r--r--   0 kimio      (501) staff       (20)     5914 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/robot-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)      652 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/slides.py
+-rw-r--r--   0 kimio      (501) staff       (20)     4551 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/ta-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)      683 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/typewriter.py
+-rw-r--r--   0 kimio      (501) staff       (20)     2073 2023-04-21 11:17:52.000000 kogi-0.4.4/kogi/ui/wait_and_ready.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-21 12:24:08.529784 kogi-0.4.4/kogi.egg-info/
+-rw-r--r--   0 kimio      (501) staff       (20)      591 2023-04-21 12:24:08.000000 kogi-0.4.4/kogi.egg-info/PKG-INFO
+-rw-r--r--   0 kimio      (501) staff       (20)     1688 2023-04-21 12:24:08.000000 kogi-0.4.4/kogi.egg-info/SOURCES.txt
+-rw-r--r--   0 kimio      (501) staff       (20)        1 2023-04-21 12:24:08.000000 kogi-0.4.4/kogi.egg-info/dependency_links.txt
+-rw-r--r--   0 kimio      (501) staff       (20)       51 2023-04-21 12:24:08.000000 kogi-0.4.4/kogi.egg-info/requires.txt
+-rw-r--r--   0 kimio      (501) staff       (20)        5 2023-04-21 12:24:08.000000 kogi-0.4.4/kogi.egg-info/top_level.txt
+-rw-r--r--   0 kimio      (501) staff       (20)       38 2023-04-21 12:24:08.541265 kogi-0.4.4/setup.cfg
+-rw-r--r--   0 kimio      (501) staff       (20)     1168 2023-04-21 11:58:37.000000 kogi-0.4.4/setup.py
```

### Comparing `kogi-0.4.3/PKG-INFO` & `kogi-0.4.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: kogi
-Version: 0.4.3
+Version: 0.4.4
 Summary: Kogi Programming Assistant AI
 Home-page: https://github.com/kkuramitsu/kogi
 Author: Kimio Kuramitsu
-Author-email: UNKNOWN
 License: MIT
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: IPython
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Education
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `kogi-0.4.3/kogi/chat.py` & `kogi-0.4.4/kogi/chat.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,24 @@
 from IPython import get_ipython
 
 from .service import (
     translate, model_prompt, kogi_get,
     record_log, debug_print
 )
 
+def remove_comment(code):
+    ss = []
+    for line in code.splitlines():
+        if '"' in line or "'" in line:
+            ss.append(line)
+        else:
+            line, _, _ = line.partition('#')
+            ss.append(line)
+    return '\n'.join(ss)
+
 
 class ChatAI(object):
     slots: dict
     chats: dict
 
     def __init__(self, slots=None):
         self.slots = slots or {}
@@ -24,15 +34,14 @@
         self.face_icon = '@kogi_plus'
         self.prev_time = time.time()
 
     def get(self, key, value):
         return self.slots.get(key, value)
 
     def update(self, context: dict):
-        self.chats = {}
         if context:
             self.slots = dict(context)
         else:
             self.slots = {}
         self.slots['rec_id'] = None
 
     def difftime(self):
@@ -52,115 +61,107 @@
             record_log(type='likeit', rec_id=rec_id, score=score,
                        context=context, prompt=prompt, response=response, data=data)
         self.slots['rec_id'] = None
 
     def face(self, text):
         return f'{self.face_icon}:{text}'
 
-    def prompt(self, prompt):
+    def prompt(self, input_text, **kwargs):
         if self.slots['rec_id'] is not None:
             self.likeit(self.slots['rec_id'], 0)
             self.face_icon = '@kogi_minus'
         else:
             self.face_icon = '@kogi_plus'
         # 将来は分類モデルに置き換える
-        if 'どうしたら' in prompt or 'どしたら' in prompt:
-            return self.error_hint(prompt)
-        if '直して' in prompt or 'たすけて' in prompt or '助けて' in prompt:
-            return self.fix_code(prompt)
-        if prompt.startswith('+') or prompt.startswith('＋'):
-            prompt = prompt[1:]
-            if 'again' in self.slots:
-                return self.dialog_again(prompt)
-        return self.dialog_request(prompt)
+        if '直して' in input_text:
+            kwargs['include_code'] = True
+        if 'エラー' in input_text or 'どうしたら' in input_text:
+            kwargs['include_eline'] = True
+        if len(input_text) < 7: #コードを直して
+            kwargs['detailed'] = True
+        # if 'どうしたら' in prompt or 'どしたら' in prompt:
+        #     return self.error_hint(prompt)
+        # if '直して' in prompt or 'たすけて' in prompt or '助けて' in prompt:
+        #     return self.fix_code(prompt)
+        # if prompt.startswith('+') or prompt.startswith('＋'):
+        #     prompt = prompt[1:]
+        #     if 'again' in self.slots:
+        #         return self.dialog_again(prompt)
+        return self.dialog_with_context(input_text, **kwargs)
 
     def no_response(self):
         return 'AIが反応しない..'
 
-    def dialog_request(self, input_text):
-        prompt = input_text
-        response, tokens = model_prompt(prompt)
-        if response == '':
-            return self.no_response()
-        rec_id = record_log(type='prompt', prompt_type='request', difftime=self.difftime(),
-                            context='', prompt=prompt, response=response, tokens=tokens)
-        self.chats[rec_id] = ('', prompt, response,
-                              ('dialog_request', input_text))
-        self.slots['rec_id'] = rec_id
-        return self.face(response), rec_id
-
-    def dialog_again(self, input_text):
-        if 'again' in self.slots:
-            context, prompt, response = self.slots['again']
-        prompt = f'{prompt}\n{input_text}'
-        response, tokens = model_prompt(prompt, context=context)
-        if response == '':
-            return self.no_response()
-        rec_id = record_log(type='prompt', prompt_type='again', difftime=self.difftime(),
-                            context=context, prompt=prompt, response=response, tokens=tokens)
-        self.chats[rec_id] = (context, prompt, response,
-                              ('dialog_again', input_text))
-        self.slots['rec_id'] = rec_id
-        return self.face(response), rec_id
-
-    def get_context(self, include_eline=False, include_code=False):
+    def get_context(self, **kwargs):
         ss = []
+        if kwargs.get('include_code', False) and 'code' in self.slots:
+            ss.append('コード:')
+            ss.append('```')
+            ss.append(remove_comment(self.slots['code']))
+            ss.append('```')
         if 'emsg' in self.slots:
             emsg = self.slots['emsg']
-            ss.append(f'エラーの発生: {emsg}')
-        if include_eline and 'eline' in self.slots:
+            ss.append(f'発生したエラー: {emsg}')
+        if kwargs.get('include_eline', False) and 'eline' in self.slots:
             eline = self.slots['eline']
             ss.append(f'エラーの発生した行: {eline}')
-        if include_code and 'code' in self.slots:
-            ss.append('コード:')
-            ss.append('```')
-            for line in self.slots['code'].splitlines():
-                if '"' in line or "'" in line:
-                    ss.append(line)
-                else:
-                    line, _, _ = line.partition('#')
-                    ss.append(line)
-            ss.append('```')
+        if 'prev_input_text' in self.slots and kwargs.get('detailed', False):
+            ss.append(self.slots['prev_input_text'])
         return '\n'.join(ss)
 
-    def error_hint(self, prompt):
-        emsg = self.slots['emsg']
-        eline = self.slots['eline']
-        context = self.get_context(include_eline=True)
-        prompt = '原因と解決のヒントを簡潔に教えてください。'
+    def dialog_with_context(self, input_text, **kwargs):
+        prompt = input_text
+        context = self.get_context(**kwargs)
         response, tokens = model_prompt(prompt, context=context)
         if response == '':
             return self.no_response()
-        rec_id = record_log(type='prompt', prompt_type='error', difftime=self.difftime(),
+        self.slots['prev_input_text'] = input_text
+        rec_id = record_log(type='prompt', prompt_type='auto', difftime=self.difftime(),
+                            input_text=input_text,
                             context=context, prompt=prompt, response=response, tokens=tokens)
-        record_log(type='error_hint',
-                   response=response, tokens=tokens, emsg=emsg, eline=eline)
         self.chats[rec_id] = (context, prompt, response,
-                              ('error_hint', emsg, eline))
+                              ('dialog_request', input_text, kwargs))
         self.slots['rec_id'] = rec_id
         return self.face(response), rec_id
 
-    def fix_code(self, prompt):
-        emsg = self.slots['emsg']
-        code = self.slots['code']
-        if len(code) > 512:
-            return '@kogi:コードがちょっと長すぎるね', 0
-        context = self.get_context(include_code=True)
-        prompt = f'上記のコードを修正してください。'
-        response, tokens = model_prompt(prompt, context=context)
-        if response == '':
-            return self.no_response()
-        rec_id = record_log(type='prompt', prompt_type='code', difftime=self.difftime(),
-                            context=context, prompt=prompt, response=response, tokens=tokens)
-        record_log(type='fix_code',
-                   response=response, tokens=tokens, emsg=emsg, code=code)
-        self.chats[rec_id] = (context, prompt, response,
-                              ('fix_code', emsg, code))
-        self.slots['rec_id'] = rec_id
-        return self.face(response), rec_id
+    # def error_hint(self, prompt):
+    #     emsg = self.slots['emsg']
+    #     eline = self.slots['eline']
+    #     context = self.get_context(include_eline=True)
+    #     prompt = '解決のヒントを簡潔に教えてください。'
+    #     response, tokens = model_prompt(prompt, context=context)
+    #     if response == '':
+    #         return self.no_response()
+    #     rec_id = record_log(type='prompt', prompt_type='error', difftime=self.difftime(),
+    #                         context=context, prompt=prompt, response=response, tokens=tokens)
+    #     record_log(type='error_hint',
+    #                response=response, tokens=tokens, emsg=emsg, eline=eline)
+    #     self.chats[rec_id] = (context, prompt, response,
+    #                           ('error_hint', emsg, eline))
+    #     self.slots['rec_id'] = rec_id
+    #     return self.face(response), rec_id
+
+    # def fix_code(self, prompt):
+    #     emsg = self.slots['emsg']
+    #     code = self.slots['code']
+    #     if len(code) > 512:
+    #         return '@kogi:コードがちょっと長すぎるね', 0
+    #     context = self.get_context(include_code=True)
+    #     prompt = f'上記のコードを修正してください。'
+    #     response, tokens = model_prompt(prompt, context=context)
+    #     if response == '':
+    #         return self.no_response()
+    #     rec_id = record_log(type='prompt', prompt_type='code', difftime=self.difftime(),
+    #                         context=context, prompt=prompt, response=response, tokens=tokens)
+    #     record_log(type='fix_code',
+    #                response=response, tokens=tokens, emsg=emsg, code=code)
+    #     self.chats[rec_id] = (context, prompt, response,
+    #                           ('fix_code', emsg, code))
+    #     self.slots['rec_id'] = rec_id
+    #     return self.face(response), rec_id
 
 
 _DefaultChatbot = ChatAI()
 
 
 def set_chatbot(chatbot):
     global _DefaultChatbot
@@ -221,31 +222,20 @@
         google_colab.register_callback('notebook.ask', ask)
         google_colab.register_callback('notebook.like', like)
         # if start != '':
         #     ask(start)
     return target
 
 
-def remove_comment(code):
-    ss = []
-    for line in code.splitlines():
-        if '#kogi' in line:
-            line, _, _ = line.rpartition('#kogi')
-        if len(line) > 0:
-            ss.append(line)
-    return '\n'.join(ss)
-
-
 def call_and_start_kogi(actions, code: str = None, context: dict = None):
     for user_text in actions:
         _DefaultChatbot.update(context)
+        _DefaultChatbot.slots['code']=code
         code = remove_comment(code)
-        if len(code) > 0:
-            user_text = f'コーディング中:\n```\n{code}\n```\n{user_text}\n'
-        doc, rec_id = _DefaultChatbot.prompt(user_text)
+        doc, rec_id = _DefaultChatbot.prompt(user_text, include_code=len(code) > 0)
         doc = Doc.md(doc)
         doc.add_likeit(rec_id)
         start_dialog(_DefaultChatbot, doc)
         return
 
 
 def error_message(record):
```

### Comparing `kogi-0.4.3/kogi/data/common_loader.py` & `kogi-0.4.4/kogi/data/common_loader.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/data/diagnosis_ja.txt` & `kogi-0.4.4/kogi/data/diagnosis_ja.txt`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/data/error.txt` & `kogi-0.4.4/kogi/data/error.txt`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/data/error_desc.py` & `kogi-0.4.4/kogi/data/error_desc.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/hook.py` & `kogi-0.4.4/kogi/hook.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/liberr/_extract_emsg.py` & `kogi-0.4.4/kogi/liberr/_extract_emsg.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/liberr/_traceback2.py` & `kogi-0.4.4/kogi/liberr/_traceback2.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/liberr/emsg_rules.tsv` & `kogi-0.4.4/kogi/liberr/emsg_rules.tsv`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/liberr/extract_vars.py` & `kogi-0.4.4/kogi/liberr/extract_vars.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/liberr/rulebase.py` & `kogi-0.4.4/kogi/liberr/rulebase.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/pan.py` & `kogi-0.4.4/kogi/pan.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/problem/__init__.py` & `kogi-0.4.4/kogi/problem/__init__.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/problem/atcoder.py` & `kogi-0.4.4/kogi/problem/atcoder.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/problem/drill.py` & `kogi-0.4.4/kogi/problem/drill.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/problem/judge.py` & `kogi-0.4.4/kogi/problem/judge.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/problem/timeout.py` & `kogi-0.4.4/kogi/problem/timeout.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/service/__init__.py` & `kogi-0.4.4/kogi/service/__init__.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/service/chatgpt.py` & `kogi-0.4.4/kogi/service/chatgpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     global model_cache
     input_text = f'{context}{prompt}{post_prompt}'
     if input_text in model_cache:
         return model_cache[input_text], 0
 
     role = kwargs.get('role', '優秀なPythonの先生')
     if 'disable_example' in kwargs:
-        req = '1文で短く教えてください。例えや例は不要です。'
+        req = '100字以内で簡潔に教えてください。例えや例は不要です。'
     else:
-        req = '1文で短く教えてください。'
+        req = '100字以内で教えてください。'
     premise = f"あなたは{role}です。{req}\n{context}"
     try:
         response = openai.ChatCompletion.create(
             model="gpt-3.5-turbo",
             messages=[
                 {"role": "system", "content": premise},
                 {"role": "user", f"content": f"{prompt}\n{post_prompt}"},
```

### Comparing `kogi-0.4.3/kogi/service/flaskapi.py` & `kogi-0.4.4/kogi/service/flaskapi.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/service/flaskserv.py` & `kogi-0.4.4/kogi/service/flaskserv.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/service/huggingface.py` & `kogi-0.4.4/kogi/service/huggingface.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/service/s3logging.py` & `kogi-0.4.4/kogi/service/s3logging.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/service/slack.py` & `kogi-0.4.4/kogi/service/slack.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/service/textra.py` & `kogi-0.4.4/kogi/service/textra.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/task/code.py` & `kogi-0.4.4/kogi/task/code.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/task/diagnosis.py` & `kogi-0.4.4/kogi/task/diagnosis.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/task/multi.py` & `kogi-0.4.4/kogi/task/multi.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/task/runner.py` & `kogi-0.4.4/kogi/task/runner.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/transform.py` & `kogi-0.4.4/kogi/transform.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/_canvas.py` & `kogi-0.4.4/kogi/ui/_canvas.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/chatgpt-fs8.png` & `kogi-0.4.4/kogi/ui/chatgpt-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/content.py` & `kogi-0.4.4/kogi/ui/content.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/dialog.css` & `kogi-0.4.4/kogi/ui/dialog.css`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/dialog.html` & `kogi-0.4.4/kogi/ui/dialog.html`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/dialog.js` & `kogi-0.4.4/kogi/ui/dialog.js`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/dialog_colab.py` & `kogi-0.4.4/kogi/ui/dialog_colab.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/dialog_ipywidgets.py` & `kogi-0.4.4/kogi/ui/dialog_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/error-fs8.png` & `kogi-0.4.4/kogi/ui/error-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/girl-fs8.png` & `kogi-0.4.4/kogi/ui/girl-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/girl_think-fs8.png` & `kogi-0.4.4/kogi/ui/girl_think-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/keylogin.py` & `kogi-0.4.4/kogi/ui/keylogin.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/kogi-fs8.png` & `kogi-0.4.4/kogi/ui/kogi-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/kogi_doya-fs8.png` & `kogi-0.4.4/kogi/ui/kogi_doya-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/kogi_error-fs8.png` & `kogi-0.4.4/kogi/ui/kogi_error-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/kogi_gaan-fs8.png` & `kogi-0.4.4/kogi/ui/kogi_gaan-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/kogi_vow-fs8.png` & `kogi-0.4.4/kogi/ui/kogi_vow-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/message.py` & `kogi-0.4.4/kogi/ui/message.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/openai-fs8.png` & `kogi-0.4.4/kogi/ui/openai-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/render.py` & `kogi-0.4.4/kogi/ui/render.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/rmt.py` & `kogi-0.4.4/kogi/ui/rmt.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/robot-fs8.png` & `kogi-0.4.4/kogi/ui/robot-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/slides.py` & `kogi-0.4.4/kogi/ui/slides.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/ta-fs8.png` & `kogi-0.4.4/kogi/ui/ta-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/typewriter.py` & `kogi-0.4.4/kogi/ui/typewriter.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi/ui/wait_and_ready.py` & `kogi-0.4.4/kogi/ui/wait_and_ready.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.3/kogi.egg-info/PKG-INFO` & `kogi-0.4.4/kogi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: kogi
-Version: 0.4.3
+Version: 0.4.4
 Summary: Kogi Programming Assistant AI
 Home-page: https://github.com/kkuramitsu/kogi
 Author: Kimio Kuramitsu
-Author-email: UNKNOWN
 License: MIT
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: IPython
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Education
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `kogi-0.4.3/kogi.egg-info/SOURCES.txt` & `kogi-0.4.4/kogi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+LICENSE
 README.md
 setup.py
 kogi/__init__.py
 kogi/ai.py
 kogi/canvas.py
 kogi/chat.py
 kogi/hook.py
-kogi/jwu2.py
+kogi/jwu.py
 kogi/pan.py
 kogi/transform.py
 kogi.egg-info/PKG-INFO
 kogi.egg-info/SOURCES.txt
 kogi.egg-info/dependency_links.txt
 kogi.egg-info/requires.txt
 kogi.egg-info/top_level.txt
```

### Comparing `kogi-0.4.3/setup.py` & `kogi-0.4.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(name="kogi",
-      version="0.4.3",
+      version="0.4.4",
       license='MIT',
       author='Kimio Kuramitsu',
       description="Kogi Programming Assistant AI",
       url="https://github.com/kkuramitsu/kogi",
       packages=['kogi', 'kogi.liberr', 'kogi.task', 'kogi.data',
                 'kogi.service', 'kogi.problem', 'kogi.ui'],
       # package_dir={"": "src"},
```

