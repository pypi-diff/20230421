# Comparing `tmp/egauge-python-0.7.2.tar.gz` & `tmp/egauge-python-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egauge-python-0.7.2.tar", last modified: Mon Apr 10 19:10:39 2023, max compression
+gzip compressed data, was "egauge-python-0.7.3.tar", last modified: Fri Apr 21 02:04:10 2023, max compression
```

## Comparing `egauge-python-0.7.2.tar` & `egauge-python-0.7.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.893046 egauge-python-0.7.2/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1090 2023-02-23 18:58:55.000000 egauge-python-0.7.2/LICENSE
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     2956 2023-04-10 19:10:39.893046 egauge-python-0.7.2/PKG-INFO
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     2301 2023-04-10 19:09:39.000000 egauge-python-0.7.2/README.md
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.717049 egauge-python-0.7.2/egauge/
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.753048 egauge-python-0.7.2/egauge/ctid/
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       71 2022-05-10 19:26:55.000000 egauge-python-0.7.2/egauge/ctid/__init__.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     2234 2022-04-22 23:39:14.000000 egauge-python-0.7.2/egauge/ctid/bit_stuffer.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    29354 2022-05-14 04:25:32.000000 egauge-python-0.7.2/egauge/ctid/ctid.py
--rwxrwxr-x   0 davidm    (1000) davidm    (1000)    12370 2022-05-14 04:25:14.000000 egauge-python-0.7.2/egauge/ctid/encoder.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     8791 2022-05-10 19:45:02.000000 egauge-python-0.7.2/egauge/ctid/waveform.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.765048 egauge-python-0.7.2/egauge/pyside2/
--rw-r--r--   0 davidm    (1000) davidm    (1000)        0 2020-03-06 20:43:49.000000 egauge-python-0.7.2/egauge/pyside2/__init__.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     3643 2022-04-22 23:39:14.000000 egauge-python-0.7.2/egauge/pyside2/ansi2html.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    10640 2022-04-22 23:39:14.000000 egauge-python-0.7.2/egauge/pyside2/terminal.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.781048 egauge-python-0.7.2/egauge/webapi/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1346 2020-07-16 19:02:13.000000 egauge-python-0.7.2/egauge/webapi/__init__.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     8335 2022-05-04 18:07:16.000000 egauge-python-0.7.2/egauge/webapi/auth.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.793048 egauge-python-0.7.2/egauge/webapi/cloud/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1293 2020-03-12 14:56:16.000000 egauge-python-0.7.2/egauge/webapi/cloud/__init__.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     4069 2022-05-04 18:28:54.000000 egauge-python-0.7.2/egauge/webapi/cloud/credentials.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.797047 egauge-python-0.7.2/egauge/webapi/cloud/gui/
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     3950 2022-04-22 23:52:29.000000 egauge-python-0.7.2/egauge/webapi/cloud/gui/credentials_dialog.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     7561 2022-05-05 19:36:33.000000 egauge-python-0.7.2/egauge/webapi/cloud/serial_number.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.841047 egauge-python-0.7.2/egauge/webapi/device/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1502 2022-09-19 21:16:17.000000 egauge-python-0.7.2/egauge/webapi/device/__init__.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    13955 2023-03-01 22:13:47.000000 egauge-python-0.7.2/egauge/webapi/device/capture.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    16279 2023-03-18 20:49:18.000000 egauge-python-0.7.2/egauge/webapi/device/ctid_info.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     7379 2023-02-23 18:36:07.000000 egauge-python-0.7.2/egauge/webapi/device/device.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     6603 2023-03-01 22:14:28.000000 egauge-python-0.7.2/egauge/webapi/device/local.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    12412 2022-09-20 20:05:39.000000 egauge-python-0.7.2/egauge/webapi/device/physical_quantity.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    14201 2022-09-20 18:48:03.000000 egauge-python-0.7.2/egauge/webapi/device/physical_units.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     9065 2022-09-19 15:49:48.000000 egauge-python-0.7.2/egauge/webapi/device/register.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     5356 2023-03-02 00:28:30.000000 egauge-python-0.7.2/egauge/webapi/device/register_row.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)    30705 2023-02-23 21:18:54.000000 egauge-python-0.7.2/egauge/webapi/device/register_type.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     9308 2023-03-01 22:33:44.000000 egauge-python-0.7.2/egauge/webapi/device/virtual_register.py
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1405 2022-04-22 23:39:14.000000 egauge-python-0.7.2/egauge/webapi/error.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     9209 2023-04-10 18:59:44.000000 egauge-python-0.7.2/egauge/webapi/json_api.py
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.869046 egauge-python-0.7.2/egauge_python.egg-info/
--rw-r--r--   0 davidm    (1000) davidm    (1000)     2956 2023-04-10 19:10:39.000000 egauge-python-0.7.2/egauge_python.egg-info/PKG-INFO
--rw-r--r--   0 davidm    (1000) davidm    (1000)     1222 2023-04-10 19:10:39.000000 egauge-python-0.7.2/egauge_python.egg-info/SOURCES.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)        1 2023-04-10 19:10:39.000000 egauge-python-0.7.2/egauge_python.egg-info/dependency_links.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       59 2023-04-10 19:10:39.000000 egauge-python-0.7.2/egauge_python.egg-info/entry_points.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       94 2023-04-10 19:10:39.000000 egauge-python-0.7.2/egauge_python.egg-info/requires.txt
--rw-r--r--   0 davidm    (1000) davidm    (1000)       21 2023-04-10 19:10:39.000000 egauge-python-0.7.2/egauge_python.egg-info/top_level.txt
-drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-10 19:10:39.889046 egauge-python-0.7.2/examples/
--rwxrwxr-x   0 davidm    (1000) davidm    (1000)     2224 2023-03-10 21:32:59.000000 egauge-python-0.7.2/examples/test_capture.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)      716 2023-03-02 01:05:11.000000 egauge-python-0.7.2/examples/test_common.py
--rwxrwxr-x   0 davidm    (1000) davidm    (1000)     2236 2023-03-10 21:33:26.000000 egauge-python-0.7.2/examples/test_ctid.py
--rwxrwxr-x   0 davidm    (1000) davidm    (1000)     4775 2023-03-10 20:47:54.000000 egauge-python-0.7.2/examples/test_local.py
--rwxrwxr-x   0 davidm    (1000) davidm    (1000)     3214 2023-03-10 22:06:39.000000 egauge-python-0.7.2/examples/test_register.py
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       55 2022-05-11 01:22:07.000000 egauge-python-0.7.2/pyproject.toml
--rw-rw-r--   0 davidm    (1000) davidm    (1000)       38 2023-04-10 19:10:39.893046 egauge-python-0.7.2/setup.cfg
--rw-rw-r--   0 davidm    (1000) davidm    (1000)     1440 2023-04-10 19:10:03.000000 egauge-python-0.7.2/setup.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.242138 egauge-python-0.7.3/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1090 2023-02-23 18:58:55.000000 egauge-python-0.7.3/LICENSE
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     2956 2023-04-21 02:04:10.242138 egauge-python-0.7.3/PKG-INFO
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     2301 2023-04-20 23:53:17.000000 egauge-python-0.7.3/README.md
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge/
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge/ctid/
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       71 2022-05-10 19:26:55.000000 egauge-python-0.7.3/egauge/ctid/__init__.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     2234 2022-04-22 23:39:14.000000 egauge-python-0.7.3/egauge/ctid/bit_stuffer.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    29354 2022-05-14 04:25:32.000000 egauge-python-0.7.3/egauge/ctid/ctid.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)    12370 2022-05-14 04:25:14.000000 egauge-python-0.7.3/egauge/ctid/encoder.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     8791 2022-05-10 19:45:02.000000 egauge-python-0.7.3/egauge/ctid/waveform.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge/pyside2/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)        0 2020-03-06 20:43:49.000000 egauge-python-0.7.3/egauge/pyside2/__init__.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     3643 2022-04-22 23:39:14.000000 egauge-python-0.7.3/egauge/pyside2/ansi2html.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    10640 2022-04-22 23:39:14.000000 egauge-python-0.7.3/egauge/pyside2/terminal.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge/webapi/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1346 2020-07-16 19:02:13.000000 egauge-python-0.7.3/egauge/webapi/__init__.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     8335 2022-05-04 18:07:16.000000 egauge-python-0.7.3/egauge/webapi/auth.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge/webapi/cloud/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1293 2020-03-12 14:56:16.000000 egauge-python-0.7.3/egauge/webapi/cloud/__init__.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     4069 2022-05-04 18:28:54.000000 egauge-python-0.7.3/egauge/webapi/cloud/credentials.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge/webapi/cloud/gui/
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     3950 2022-04-22 23:52:29.000000 egauge-python-0.7.3/egauge/webapi/cloud/gui/credentials_dialog.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     7561 2022-05-05 19:36:33.000000 egauge-python-0.7.3/egauge/webapi/cloud/serial_number.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge/webapi/device/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1502 2022-09-19 21:16:17.000000 egauge-python-0.7.3/egauge/webapi/device/__init__.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    13955 2023-03-01 22:13:47.000000 egauge-python-0.7.3/egauge/webapi/device/capture.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    16279 2022-04-22 23:39:14.000000 egauge-python-0.7.3/egauge/webapi/device/ctid_info.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     7548 2023-04-21 02:01:09.000000 egauge-python-0.7.3/egauge/webapi/device/device.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     6603 2023-03-01 22:14:28.000000 egauge-python-0.7.3/egauge/webapi/device/local.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    12412 2022-09-20 20:05:39.000000 egauge-python-0.7.3/egauge/webapi/device/physical_quantity.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    14201 2022-09-20 18:48:03.000000 egauge-python-0.7.3/egauge/webapi/device/physical_units.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     9065 2022-09-19 15:49:48.000000 egauge-python-0.7.3/egauge/webapi/device/register.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     5356 2023-03-02 00:28:30.000000 egauge-python-0.7.3/egauge/webapi/device/register_row.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)    30705 2023-02-23 21:18:54.000000 egauge-python-0.7.3/egauge/webapi/device/register_type.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     9308 2023-03-01 22:33:44.000000 egauge-python-0.7.3/egauge/webapi/device/virtual_register.py
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1405 2022-04-22 23:39:14.000000 egauge-python-0.7.3/egauge/webapi/error.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     9209 2023-04-20 23:53:17.000000 egauge-python-0.7.3/egauge/webapi/json_api.py
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/egauge_python.egg-info/
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     2956 2023-04-21 02:04:10.000000 egauge-python-0.7.3/egauge_python.egg-info/PKG-INFO
+-rw-r--r--   0 davidm    (1000) davidm    (1000)     1222 2023-04-21 02:04:10.000000 egauge-python-0.7.3/egauge_python.egg-info/SOURCES.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)        1 2023-04-21 02:04:10.000000 egauge-python-0.7.3/egauge_python.egg-info/dependency_links.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       59 2023-04-21 02:04:10.000000 egauge-python-0.7.3/egauge_python.egg-info/entry_points.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       94 2023-04-21 02:04:10.000000 egauge-python-0.7.3/egauge_python.egg-info/requires.txt
+-rw-r--r--   0 davidm    (1000) davidm    (1000)       21 2023-04-21 02:04:10.000000 egauge-python-0.7.3/egauge_python.egg-info/top_level.txt
+drwxrwxr-x   0 davidm    (1000) davidm    (1000)        0 2023-04-21 02:04:10.238138 egauge-python-0.7.3/examples/
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)     2224 2023-03-10 21:32:59.000000 egauge-python-0.7.3/examples/test_capture.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)      716 2023-03-02 01:05:11.000000 egauge-python-0.7.3/examples/test_common.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)     2236 2023-03-10 21:33:26.000000 egauge-python-0.7.3/examples/test_ctid.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)     4775 2023-03-10 20:47:54.000000 egauge-python-0.7.3/examples/test_local.py
+-rwxrwxr-x   0 davidm    (1000) davidm    (1000)     3214 2023-03-10 22:06:39.000000 egauge-python-0.7.3/examples/test_register.py
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       55 2022-05-11 01:22:07.000000 egauge-python-0.7.3/pyproject.toml
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)       38 2023-04-21 02:04:10.242138 egauge-python-0.7.3/setup.cfg
+-rw-rw-r--   0 davidm    (1000) davidm    (1000)     1440 2023-04-21 02:02:35.000000 egauge-python-0.7.3/setup.py
```

### Comparing `egauge-python-0.7.2/LICENSE` & `egauge-python-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/PKG-INFO` & `egauge-python-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egauge-python
-Version: 0.7.2
+Version: 0.7.3
 Summary: .
 Home-page: https://bitbucket.org/egauge/python/
 Author: David Mosberger-Tang
 Author-email: davidm@egauge.net
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `egauge-python-0.7.2/README.md` & `egauge-python-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/ctid/bit_stuffer.py` & `egauge-python-0.7.3/egauge/ctid/bit_stuffer.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/ctid/ctid.py` & `egauge-python-0.7.3/egauge/ctid/ctid.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/ctid/encoder.py` & `egauge-python-0.7.3/egauge/ctid/encoder.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/ctid/waveform.py` & `egauge-python-0.7.3/egauge/ctid/waveform.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/pyside2/ansi2html.py` & `egauge-python-0.7.3/egauge/pyside2/ansi2html.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/pyside2/terminal.py` & `egauge-python-0.7.3/egauge/pyside2/terminal.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/__init__.py` & `egauge-python-0.7.3/egauge/webapi/__init__.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/auth.py` & `egauge-python-0.7.3/egauge/webapi/auth.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/cloud/__init__.py` & `egauge-python-0.7.3/egauge/webapi/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/cloud/credentials.py` & `egauge-python-0.7.3/egauge/webapi/cloud/credentials.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/cloud/gui/credentials_dialog.py` & `egauge-python-0.7.3/egauge/webapi/cloud/gui/credentials_dialog.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/cloud/serial_number.py` & `egauge-python-0.7.3/egauge/webapi/cloud/serial_number.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/device/__init__.py` & `egauge-python-0.7.3/egauge/webapi/device/__init__.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/device/capture.py` & `egauge-python-0.7.3/egauge/webapi/device/capture.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/device/ctid_info.py` & `egauge-python-0.7.3/egauge/webapi/device/ctid_info.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/device/device.py` & `egauge-python-0.7.3/egauge/webapi/device/device.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,18 +51,20 @@
 class Device:
     """This class provides access to an eGauge device's JSON WebAPI.
     See "Web API Design" document for details."""
 
     def __init__(self, dev_uri, auth=None, verify=True):
         """Return a device object that can be used to access the device a
         address DEV_URI.  An example DEV_URI would be
-        "http://proto1.egaug.es".  AUTH should be an authentication object
-        that provides the credentials to access the device.  Typically,
-        this should be a JWTAuth object.  VERIFY can be set to False
-        to turn off certificate verification.
+        "http://eGaugeHQ.egauge.io".  AUTH should be an authentication
+        object that provides the credentials to access the device.
+        Typically, this should be a JWTAuth object.  VERIFY can be set
+        to False to turn off certificate verification.  It may also be
+        set to the path of a file that holds the certificate the
+        server should be validated against.
 
         """
         self.api_uri = dev_uri + "/api"
         self.auth = auth
         self._reg_info = None  # cached register info
         self._chan_info = None  # cached channel info
         self._verify = verify
@@ -70,63 +72,55 @@
     def get(self, resource, **kwargs):
         """Issue GET request for /api resource RESOURCE and return the parsed
         JSON data or None if the request failed or returned invalid
         JSON data.  Additional keyword arguments are passed on to
         requests.get().
 
         """
-        return json_api.get(
-            self.api_uri + resource,
-            auth=self.auth,
-            verify=self._verify,
-            **kwargs
-        )
+        if "verify" not in kwargs:
+            kwargs["verify"] = self._verify
+        return json_api.get(self.api_uri + resource, auth=self.auth, **kwargs)
 
     def put(self, resource, json_data, **kwargs):
         """Issue PUT request with JSON_DATA as body to /api resource RESOURCE
         and return parsed JSON reply or None if the request failed or
         returned invalid JSON data.  Additional keyword arguments are
         passed on to requests.put().
 
         """
+        if "verify" not in kwargs:
+            kwargs["verify"] = self._verify
         return json_api.put(
-            self.api_uri + resource,
-            json_data,
-            auth=self.auth,
-            verify=self._verify,
-            **kwargs
+            self.api_uri + resource, json_data, auth=self.auth, **kwargs
         )
 
     def post(self, resource, json_data, **kwargs):
         """Issue POST request with JSON_DATA as body to /api resource RESOURCE
         and return parsed JSON reply or None if the request failed or
         returned invalid JSON data.  Additional keyword arguments are
         passed on to requests.post().
 
         """
+        if "verify" not in kwargs:
+            kwargs["verify"] = self._verify
         return json_api.post(
-            self.api_uri + resource,
-            json_data,
-            auth=self.auth,
-            verify=self._verify,
-            **kwargs
+            self.api_uri + resource, json_data, auth=self.auth, **kwargs
         )
 
     def delete(self, resource, **kwargs):
         """Issue DELETE request for /api resource RESOURCE and return parsed
         JSON reply or None if the request failed or returned invalid
         JSON data.  Additional keyword arguments are passed on to
         requests.post().
 
         """
+        if "verify" not in kwargs:
+            kwargs["verify"] = self._verify
         return json_api.delete(
-            self.api_uri + resource,
-            auth=self.auth,
-            verify=self._verify,
-            **kwargs
+            self.api_uri + resource, auth=self.auth, **kwargs
         )
 
     def _fetch_reg_info(self):
         """Fetch register info, including type and virtual register
         formulas."""
         reply = self.get("/register", params={"virtual": "formula"})
         if reply is None or "registers" not in reply:
```

### Comparing `egauge-python-0.7.2/egauge/webapi/device/local.py` & `egauge-python-0.7.3/egauge/webapi/device/local.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/device/physical_quantity.py` & `egauge-python-0.7.3/egauge/webapi/device/physical_quantity.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/device/physical_units.py` & `egauge-python-0.7.3/egauge/webapi/device/physical_units.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/device/register.py` & `egauge-python-0.7.3/egauge/webapi/device/register.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/device/register_row.py` & `egauge-python-0.7.3/egauge/webapi/device/register_row.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/device/register_type.py` & `egauge-python-0.7.3/egauge/webapi/device/register_type.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/device/virtual_register.py` & `egauge-python-0.7.3/egauge/webapi/device/virtual_register.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/error.py` & `egauge-python-0.7.3/egauge/webapi/error.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge/webapi/json_api.py` & `egauge-python-0.7.3/egauge/webapi/json_api.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/egauge_python.egg-info/PKG-INFO` & `egauge-python-0.7.3/egauge_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egauge-python
-Version: 0.7.2
+Version: 0.7.3
 Summary: .
 Home-page: https://bitbucket.org/egauge/python/
 Author: David Mosberger-Tang
 Author-email: davidm@egauge.net
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `egauge-python-0.7.2/egauge_python.egg-info/SOURCES.txt` & `egauge-python-0.7.3/egauge_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/examples/test_capture.py` & `egauge-python-0.7.3/examples/test_capture.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/examples/test_common.py` & `egauge-python-0.7.3/examples/test_common.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/examples/test_ctid.py` & `egauge-python-0.7.3/examples/test_ctid.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/examples/test_local.py` & `egauge-python-0.7.3/examples/test_local.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/examples/test_register.py` & `egauge-python-0.7.3/examples/test_register.py`

 * *Files identical despite different names*

### Comparing `egauge-python-0.7.2/setup.py` & `egauge-python-0.7.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name="egauge-python",
-    version="0.7.2",
+    version="0.7.3",
     packages=setuptools.find_namespace_packages(include="egauge.*"),
     install_requires=[
         "crcmod",
         "deprecated",
         "intelhex",
         "wheel",
         "pexpect",
```

