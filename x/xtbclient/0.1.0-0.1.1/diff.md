# Comparing `tmp/XTBClient-0.1.0.tar.gz` & `tmp/xtbclient-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XTBClient-0.1.0.tar", max compression
+gzip compressed data, was "xtbclient-0.1.1.tar", max compression
```

## Comparing `XTBClient-0.1.0.tar` & `xtbclient-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35823 2022-05-09 06:20:42.572457 XTBClient-0.1.0/LICENSE
--rw-r--r--   0        0        0      462 2022-05-10 15:42:44.333996 XTBClient-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-05-09 06:24:25.020117 XTBClient-0.1.0/XTBClient/__init__.py
--rw-r--r--   0        0        0        0 2022-05-10 15:40:00.546084 XTBClient-0.1.0/XTBClient/client/__init__.py
--rw-r--r--   0        0        0     6316 2022-05-11 17:59:45.472831 XTBClient-0.1.0/XTBClient/client/axtb.py
--rw-r--r--   0        0        0     6657 2022-05-11 17:59:45.504859 XTBClient-0.1.0/XTBClient/client/xtb.py
--rw-r--r--   0        0        0       91 2022-05-09 09:44:12.424501 XTBClient-0.1.0/XTBClient/errors.py
--rw-r--r--   0        0        0        0 2022-05-09 06:24:31.478719 XTBClient-0.1.0/XTBClient/models/__init__.py
--rw-r--r--   0        0        0    13565 2022-05-10 18:41:01.043717 XTBClient-0.1.0/XTBClient/models/models.py
--rw-r--r--   0        0        0     2118 2022-05-11 17:59:45.498856 XTBClient-0.1.0/XTBClient/models/requests.py
--rw-r--r--   0        0        0     3860 2022-05-11 17:59:45.510857 XTBClient-0.1.0/XTBClient/xtb_base.py
--rw-r--r--   0        0        0      795 2022-05-11 18:13:23.846379 XTBClient-0.1.0/setup.py
--rw-r--r--   0        0        0      558 2022-05-11 18:13:23.846379 XTBClient-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-05-09 06:20:42.572457 xtbclient-0.1.1/LICENSE
+-rw-r--r--   0        0        0      484 2023-04-21 19:19:46.367347 xtbclient-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6925 2023-03-06 10:11:12.031632 xtbclient-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-06 10:11:12.031632 xtbclient-0.1.1/XTBClient/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 10:11:12.032633 xtbclient-0.1.1/XTBClient/client/__init__.py
+-rw-r--r--   0        0        0     6316 2023-03-06 10:11:12.032633 xtbclient-0.1.1/XTBClient/client/axtb.py
+-rw-r--r--   0        0        0     6657 2023-03-06 10:11:12.032633 xtbclient-0.1.1/XTBClient/client/xtb.py
+-rw-r--r--   0        0        0       91 2023-03-06 10:11:12.033634 xtbclient-0.1.1/XTBClient/errors.py
+-rw-r--r--   0        0        0        0 2023-03-06 10:11:12.033634 xtbclient-0.1.1/XTBClient/models/__init__.py
+-rw-r--r--   0        0        0    13565 2023-03-06 10:11:12.033634 xtbclient-0.1.1/XTBClient/models/models.py
+-rw-r--r--   0        0        0     2118 2023-03-06 10:11:12.033634 xtbclient-0.1.1/XTBClient/models/requests.py
+-rw-r--r--   0        0        0     3860 2023-03-06 10:11:12.034632 xtbclient-0.1.1/XTBClient/xtb_base.py
+-rw-r--r--   0        0        0     7487 1970-01-01 00:00:00.000000 xtbclient-0.1.1/PKG-INFO
```

### Comparing `XTBClient-0.1.0/LICENSE` & `xtbclient-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `XTBClient-0.1.0/XTBClient/client/axtb.py` & `xtbclient-0.1.1/XTBClient/client/axtb.py`

 * *Files identical despite different names*

### Comparing `XTBClient-0.1.0/XTBClient/client/xtb.py` & `xtbclient-0.1.1/XTBClient/client/xtb.py`

 * *Files identical despite different names*

### Comparing `XTBClient-0.1.0/XTBClient/models/models.py` & `xtbclient-0.1.1/XTBClient/models/models.py`

 * *Files identical despite different names*

### Comparing `XTBClient-0.1.0/XTBClient/models/requests.py` & `xtbclient-0.1.1/XTBClient/models/requests.py`

 * *Files identical despite different names*

### Comparing `XTBClient-0.1.0/XTBClient/xtb_base.py` & `xtbclient-0.1.1/XTBClient/xtb_base.py`

 * *Files identical despite different names*

