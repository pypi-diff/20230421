# Comparing `tmp/solox-2.5.9.tar.gz` & `tmp/solox-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-f6gwnpz6/solox-2.5.9.tar", last modified: Wed Apr 19 09:34:31 2023, max compression
+gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-oece9rip/solox-2.6.0.tar", last modified: Fri Apr 21 09:41:59 2023, max compression
```

## Comparing `solox-2.5.9.tar` & `solox-2.6.0.tar`

### file list

```diff
@@ -1,109 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-19 09:34:19.000000 solox-2.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-19 09:34:19.000000 solox-2.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-19 09:34:31.000000 solox-2.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-19 09:34:19.000000 solox-2.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-19 09:34:31.000000 solox-2.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-19 09:34:19.000000 solox-2.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-19 09:34:19.000000 solox-2.5.9/solox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-19 09:34:19.000000 solox-2.5.9/solox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-19 09:34:19.000000 solox-2.5.9/solox/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/public/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/_iosPerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/public/adb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/public/adb/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/adb/linux/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/public/adb/linux_arm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/adb/linux_arm/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/public/adb/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/adb/mac/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/public/adb/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/adb/windows/AdbWinApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/adb/windows/AdbWinUsbApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/adb/windows/adb.exe
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/apm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/apm_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23736 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/fps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/public/iosperf/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30644 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    41041 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_hexdump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_imagemounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9935 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)    39139 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_ipautil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_safe_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/_wdaproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/bplist.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/plistlib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/requests_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-19 09:34:19.000000 solox-2.5.9/solox/public/iosperf/struct2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/css/highlight.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/css/select2-bootstrap-5-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/css/sweetalert2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/css/tabler.demo.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/css/tabler.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/static/image/
--rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/image/404.png
--rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/image/500.png
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/image/avatar.png
--rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/image/coffee.png
--rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/image/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/static/image/readme/
--rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/image/readme/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/image/readme/pk.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/apexcharts.js
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/gray.js
--rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/highstock.js
--rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/html2canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/socket.io.js
--rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/sweetalert2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/tabler.demo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/js/tabler.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-04-19 09:34:19.000000 solox-2.5.9/solox/static/logo/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)    47094 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/analysis_pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    35648 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    91984 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-04-19 09:34:19.000000 solox-2.5.9/solox/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox/view/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 09:34:19.000000 solox-2.5.9/solox/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24225 2023-04-19 09:34:19.000000 solox-2.5.9/solox/view/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-04-19 09:34:19.000000 solox-2.5.9/solox/view/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-19 09:34:19.000000 solox-2.5.9/solox/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:34:31.000000 solox-2.5.9/solox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-19 09:34:31.000000 solox-2.5.9/solox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-19 09:34:31.000000 solox-2.5.9/solox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 09:34:31.000000 solox-2.5.9/solox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-19 09:34:31.000000 solox-2.5.9/solox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 09:34:31.000000 solox-2.5.9/solox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-21 09:41:51.000000 solox-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-21 09:41:51.000000 solox-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-21 09:41:59.000000 solox-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-21 09:41:51.000000 solox-2.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-21 09:41:59.000000 solox-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-21 09:41:51.000000 solox-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 09:41:51.000000 solox-2.6.0/solox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-21 09:41:51.000000 solox-2.6.0/solox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-21 09:41:51.000000 solox-2.6.0/solox/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/_iosPerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/adb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/adb/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/adb/linux/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/adb/linux_arm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/adb/linux_arm/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/adb/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/adb/mac/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/adb/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/adb/windows/AdbWinApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/adb/windows/AdbWinUsbApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/adb/windows/adb.exe
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/apm_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27081 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/fps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/iosperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30644 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41041 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_imagemounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9935 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39139 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_ipautil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_safe_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_wdaproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/bplist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/plistlib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/requests_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/struct2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/report_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    29240 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/report_template/android.html
+-rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/report_template/ios.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/css/highlight.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/css/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/css/sweetalert2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/css/tabler.demo.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/css/tabler.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/static/image/
+-rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/image/404.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/image/500.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/image/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/image/coffee.png
+-rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/image/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/static/image/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/image/readme/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/image/readme/pk.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/apexcharts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/gray.js
+-rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/highstock.js
+-rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/html2canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/socket.io.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/sweetalert2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/tabler.demo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/tabler.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/logo/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)    53512 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/analysis_pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35648 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    92057 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 09:41:51.000000 solox-2.6.0/solox/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-04-21 09:41:51.000000 solox-2.6.0/solox/view/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-04-21 09:41:51.000000 solox-2.6.0/solox/view/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-21 09:41:51.000000 solox-2.6.0/solox/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-21 09:41:59.000000 solox-2.6.0/solox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-21 09:41:59.000000 solox-2.6.0/solox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:41:59.000000 solox-2.6.0/solox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 09:41:59.000000 solox-2.6.0/solox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 09:41:59.000000 solox-2.6.0/solox.egg-info/top_level.txt
```

### Comparing `solox-2.5.9/LICENSE` & `solox-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/PKG-INFO` & `solox-2.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.5.9
+Version: 2.6.0
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -27,25 +27,25 @@
 </p>
 <p align="center">
 <a href="https://pypi.org/project/solox/" target="__blank"><img src="https://img.shields.io/pypi/v/solox" alt="solox preview"></a>
 <a href="https://pypistats.org/packages/solox" target="__blank"><img src="https://img.shields.io/pypi/dm/solox"></a>
 <br>
 </p>
 
-## 🔎Preview
+## 🔎Preview	
 
 SoloX - Real-time collection tool for Android/iOS performance data.
 
 We are committed to solving inefficient, cumbersome test execution, and our goal is Simple Test In SoloX!
 
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%" >
 
 ## 📦Requirements
 
-- Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
+Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
 
 💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4.
 
 💡 If Windows users need to test ios, install and start Itunes.
 
 ## 📥Installation
 
@@ -76,23 +76,25 @@
 ```shell
 python -m solox --host={ip} --port={port}
 ```
 
 ## 🏴󠁣󠁩󠁣󠁭󠁿Collect in python
 
 ```python
+
 from solox.public.apm import APM
 from solox.public.common import Devices
 
 # solox version >= 2.1.2
 
 d = Devices()
 pids = d.getPid(deviceId='ca6bd5a5', pkgName='com.bilibili.app.in')
 
-apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True, noLog=True, pid=None)
+apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', 
+          surfaceview=True, noLog=True, pid=None)
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS') only supports one device
 # surfaceview： False = gfxinfo (Developer - GPU rendering mode - adb shell dumpsys gfxinfo)
 # noLog : False (Save test data to log file)
 
 cpu = apm.collectCpu() # %
 memory = apm.collectMemory() # MB
 flow = apm.collectFlow(wifi=True) # KB
@@ -121,19 +123,19 @@
 target in ['cpu','memory','network','fps','battery','gpu']
 ```
 
 ## 🔥Features
 
 * **No ROOT/Jailbreak:** No need of Root for Android devices, Jailbreak for iOS devices. Efficiently solving the test and analysis challenges in Android & iOS performance.
 * **Data Integrality:** We provide the data about Screenshot, CPU, GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get.
-* **Beautiful report board:** A beautiful and detailed report analysis, where to store, visualize, edit, manage, and download all the test cases collected with SoloX no matter where you are or when is it.
-* **Useful monitoring settings:** Support setting alarm values, collecting duration, and accessing mobile devices on other PC machines during the monitoring process.
-* **PK model:** Supports simultaneous comparative testing of two mobile devices.
-  🌱2-devices: test the same app on two different phones.
-  🌱2-apps: test two different apps on two phones with the same configuration.
+* **Beautiful Report:** A beautiful and detailed report analysis, where to store, visualize, edit, manage, and download all the test cases collected with SoloX no matter where you are or when is it.
+* **Useful Monitoring Settings:** Support setting alarm values, collecting duration, and accessing mobile devices on other PC machines during the monitoring process.
+* **PK Model:** Supports simultaneous comparative testing of two mobile devices.
+  - 🌱2-devices: test the same app on two different phones.
+  - 🌱2-apps: test two different apps on two phones with the same configuration.
 
 ## Browser
 
 <img src="https://cdn.nlark.com/yuque/0/2023/png/153412/1677553244198-96ce5709-f33f-4038-888f-f330d1f74450.png" alt="Chrome" width="50px" height="50px" />
 
 ## Terminal
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: solox Version: 2.5.9 Summary: SoloX - Real-time
+Metadata-Version: 2.1 Name: solox Version: 2.6.0 Summary: SoloX - Real-time
 collection tool for Android/iOS performance data. Home-page: https://
 github.com/smart-test-ti/SoloX Author: Rafa Chen Author-email:
 rafacheninc@gamil.com License: MIT Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE
                                English | ä¸­æ
                                    [SoloX]
 
             [solox_preview] [https://img.shields.io/pypi/dm/solox]
 ## ðPreview SoloX - Real-time collection tool for Android/iOS performance
 data. We are committed to solving inefficient, cumbersome test execution, and
 our goal is Simple Test In SoloX! [https://cdn.nlark.com/yuque/0/2022/png/
 153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-
-process=image%2Fresize%2Cw_1500%2Climit_0] ## ð¦Requirements - Install Python
+process=image%2Fresize%2Cw_1500%2Climit_0] ## ð¦Requirements Install Python
 3.10 + [**Download**](https://www.python.org/downloads/) ð¡ Python 3.6 ~ 3.9
 , please download a version of solox lower than 2.5.4. ð¡ If Windows users
 need to test ios, install and start Itunes. ## ð¥Installation ### default
 ```shell pip install -U solox ``` ### mirrors ```shell pip install -i https://
 mirrors.ustc.edu.cn/pypi/web/simple -U solox ``` ð¡ If your network is unable
 to download through [pip install -U solox], please try using mirrors to
 download, but the download of SoloX may not be the latest version. ##
@@ -42,17 +42,17 @@
 iOS: http://{ip}:{port}/apm/
 collect?platform=iOS&pkgname=com.bilibili.app.in&target=cpu target in
 ['cpu','memory','network','fps','battery','gpu'] ``` ## ð¥Features * **No
 ROOT/Jailbreak:** No need of Root for Android devices, Jailbreak for iOS
 devices. Efficiently solving the test and analysis challenges in Android & iOS
 performance. * **Data Integrality:** We provide the data about Screenshot, CPU,
 GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get. *
-**Beautiful report board:** A beautiful and detailed report analysis, where to
-store, visualize, edit, manage, and download all the test cases collected with
-SoloX no matter where you are or when is it. * **Useful monitoring settings:**
+**Beautiful Report:** A beautiful and detailed report analysis, where to store,
+visualize, edit, manage, and download all the test cases collected with SoloX
+no matter where you are or when is it. * **Useful Monitoring Settings:**
 Support setting alarm values, collecting duration, and accessing mobile devices
-on other PC machines during the monitoring process. * **PK model:** Supports
-simultaneous comparative testing of two mobile devices. ð±2-devices: test the
-same app on two different phones. ð±2-apps: test two different apps on two
-phones with the same configuration. ## Browser [Chrome] ## Terminal - windows:
-PowerShell - macOSï¼iTerm2 (https://iterm2.com/) ## ðThanks - https://
-github.com/alibaba/taobao-iphone-device
+on other PC machines during the monitoring process. * **PK Model:** Supports
+simultaneous comparative testing of two mobile devices. - ð±2-devices: test
+the same app on two different phones. - ð±2-apps: test two different apps on
+two phones with the same configuration. ## Browser [Chrome] ## Terminal -
+windows: PowerShell - macOSï¼iTerm2 (https://iterm2.com/) ## ðThanks -
+https://github.com/alibaba/taobao-iphone-device
```

### Comparing `solox-2.5.9/README.md` & `solox-2.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 </p>
 <p align="center">
 <a href="https://pypi.org/project/solox/" target="__blank"><img src="https://img.shields.io/pypi/v/solox" alt="solox preview"></a>
 <a href="https://pypistats.org/packages/solox" target="__blank"><img src="https://img.shields.io/pypi/dm/solox"></a>
 <br>
 </p>
 
-## 🔎Preview
+## 🔎Preview	
 
 SoloX - Real-time collection tool for Android/iOS performance data.
 
 We are committed to solving inefficient, cumbersome test execution, and our goal is Simple Test In SoloX!
 
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%" >
 
 ## 📦Requirements
 
-- Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
+Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
 
 💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4.
 
 💡 If Windows users need to test ios, install and start Itunes.
 
 ## 📥Installation
 
@@ -61,23 +61,25 @@
 ```shell
 python -m solox --host={ip} --port={port}
 ```
 
 ## 🏴󠁣󠁩󠁣󠁭󠁿Collect in python
 
 ```python
+
 from solox.public.apm import APM
 from solox.public.common import Devices
 
 # solox version >= 2.1.2
 
 d = Devices()
 pids = d.getPid(deviceId='ca6bd5a5', pkgName='com.bilibili.app.in')
 
-apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True, noLog=True, pid=None)
+apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', 
+          surfaceview=True, noLog=True, pid=None)
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS') only supports one device
 # surfaceview： False = gfxinfo (Developer - GPU rendering mode - adb shell dumpsys gfxinfo)
 # noLog : False (Save test data to log file)
 
 cpu = apm.collectCpu() # %
 memory = apm.collectMemory() # MB
 flow = apm.collectFlow(wifi=True) # KB
@@ -106,19 +108,19 @@
 target in ['cpu','memory','network','fps','battery','gpu']
 ```
 
 ## 🔥Features
 
 * **No ROOT/Jailbreak:** No need of Root for Android devices, Jailbreak for iOS devices. Efficiently solving the test and analysis challenges in Android & iOS performance.
 * **Data Integrality:** We provide the data about Screenshot, CPU, GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get.
-* **Beautiful report board:** A beautiful and detailed report analysis, where to store, visualize, edit, manage, and download all the test cases collected with SoloX no matter where you are or when is it.
-* **Useful monitoring settings:** Support setting alarm values, collecting duration, and accessing mobile devices on other PC machines during the monitoring process.
-* **PK model:** Supports simultaneous comparative testing of two mobile devices.
-  🌱2-devices: test the same app on two different phones.
-  🌱2-apps: test two different apps on two phones with the same configuration.
+* **Beautiful Report:** A beautiful and detailed report analysis, where to store, visualize, edit, manage, and download all the test cases collected with SoloX no matter where you are or when is it.
+* **Useful Monitoring Settings:** Support setting alarm values, collecting duration, and accessing mobile devices on other PC machines during the monitoring process.
+* **PK Model:** Supports simultaneous comparative testing of two mobile devices.
+  - 🌱2-devices: test the same app on two different phones.
+  - 🌱2-apps: test two different apps on two phones with the same configuration.
 
 ## Browser
 
 <img src="https://cdn.nlark.com/yuque/0/2023/png/153412/1677553244198-96ce5709-f33f-4038-888f-f330d1f74450.png" alt="Chrome" width="50px" height="50px" />
 
 ## Terminal
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
                                    [SoloX]
 
             [solox_preview] [https://img.shields.io/pypi/dm/solox]
 ## ðPreview SoloX - Real-time collection tool for Android/iOS performance
 data. We are committed to solving inefficient, cumbersome test execution, and
 our goal is Simple Test In SoloX! [https://cdn.nlark.com/yuque/0/2022/png/
 153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-
-process=image%2Fresize%2Cw_1500%2Climit_0] ## ð¦Requirements - Install Python
+process=image%2Fresize%2Cw_1500%2Climit_0] ## ð¦Requirements Install Python
 3.10 + [**Download**](https://www.python.org/downloads/) ð¡ Python 3.6 ~ 3.9
 , please download a version of solox lower than 2.5.4. ð¡ If Windows users
 need to test ios, install and start Itunes. ## ð¥Installation ### default
 ```shell pip install -U solox ``` ### mirrors ```shell pip install -i https://
 mirrors.ustc.edu.cn/pypi/web/simple -U solox ``` ð¡ If your network is unable
 to download through [pip install -U solox], please try using mirrors to
 download, but the download of SoloX may not be the latest version. ##
@@ -35,17 +35,17 @@
 iOS: http://{ip}:{port}/apm/
 collect?platform=iOS&pkgname=com.bilibili.app.in&target=cpu target in
 ['cpu','memory','network','fps','battery','gpu'] ``` ## ð¥Features * **No
 ROOT/Jailbreak:** No need of Root for Android devices, Jailbreak for iOS
 devices. Efficiently solving the test and analysis challenges in Android & iOS
 performance. * **Data Integrality:** We provide the data about Screenshot, CPU,
 GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get. *
-**Beautiful report board:** A beautiful and detailed report analysis, where to
-store, visualize, edit, manage, and download all the test cases collected with
-SoloX no matter where you are or when is it. * **Useful monitoring settings:**
+**Beautiful Report:** A beautiful and detailed report analysis, where to store,
+visualize, edit, manage, and download all the test cases collected with SoloX
+no matter where you are or when is it. * **Useful Monitoring Settings:**
 Support setting alarm values, collecting duration, and accessing mobile devices
-on other PC machines during the monitoring process. * **PK model:** Supports
-simultaneous comparative testing of two mobile devices. ð±2-devices: test the
-same app on two different phones. ð±2-apps: test two different apps on two
-phones with the same configuration. ## Browser [Chrome] ## Terminal - windows:
-PowerShell - macOSï¼iTerm2 (https://iterm2.com/) ## ðThanks - https://
-github.com/alibaba/taobao-iphone-device
+on other PC machines during the monitoring process. * **PK Model:** Supports
+simultaneous comparative testing of two mobile devices. - ð±2-devices: test
+the same app on two different phones. - ð±2-apps: test two different apps on
+two phones with the same configuration. ## Browser [Chrome] ## Terminal -
+windows: PowerShell - macOSï¼iTerm2 (https://iterm2.com/) ## ðThanks -
+https://github.com/alibaba/taobao-iphone-device
```

### Comparing `solox-2.5.9/setup.py` & `solox-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/debug.py` & `solox-2.6.0/solox/debug.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/_iosPerf.py` & `solox-2.6.0/solox/public/_iosPerf.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/adb/mac/adb` & `solox-2.6.0/solox/public/adb/mac/adb`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/adb.py` & `solox-2.6.0/solox/public/adb.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/apm.py` & `solox-2.6.0/solox/public/apm.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import time
 import os
 from logzero import logger
 import tidevice
 import solox.public._iosPerf as iosP
 from solox.public.iosperf._perf import DataType, Performance
 from solox.public.adb import adb
-from solox.public.common import Devices, file, Method, Platform
+from solox.public.common import Devices, File, Method, Platform
 from solox.public.fps import FPSMonitor, TimeUtils
 
 d = Devices()
-f = file()
+f = File()
 m = Method()
 
 class Target:
     CPU = 'cpu'
     Memory = 'memory'
     Battery = 'battery'
     Network = 'network'
@@ -102,15 +102,14 @@
         return appCpuRate, sysCpuRate
 
     def getCpuRate(self, noLog=False):
         """Get the cpu rate of a process, unit:%"""
         appCpuRate, systemCpuRate = self.getAndroidCpuRate(noLog) if self.platform == Platform.Android else self.getiOSCpuRate(noLog)
         return appCpuRate, systemCpuRate
 
-
 class MEM(object):
     def __init__(self, pkgName, deviceId, platform=Platform.Android, pid=None):
         self.pkgName = pkgName
         self.deviceId = deviceId
         self.platform = platform
         self.pid = pid
         if self.pid is None and self.platform == Platform.Android:
@@ -144,15 +143,14 @@
             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
             f.add_log(os.path.join(f.report_dir,'mem_total.log'), apm_time, totalPass)
             if self.platform == Platform.Android:
                 f.add_log(os.path.join(f.report_dir,'mem_native.log'), apm_time, nativePass)
                 f.add_log(os.path.join(f.report_dir,'mem_dalvik.log'), apm_time, dalvikPass)
         return totalPass, nativePass, dalvikPass
 
-
 class Battery(object):
     def __init__(self, deviceId, platform=Platform.Android):
         self.deviceId = deviceId
         self.platform = platform
     
     def getBattery(self, noLog=False):
         if self.platform == Platform.Android:
@@ -197,15 +195,14 @@
         return tem, current, voltage, power
 
     def recoverBattery(self):
         """Reset phone charging status"""
         cmd = 'dumpsys battery reset'
         adb.shell(cmd=cmd, deviceId=self.deviceId)
 
-
 class Flow(object):
 
     def __init__(self, pkgName, deviceId, platform=Platform.Android, pid=None):
         self.pkgName = pkgName
         self.deviceId = deviceId
         self.platform = platform
         self.pid = pid
@@ -252,15 +249,14 @@
         sendNum, recNum = self.getAndroidNet(wifi) if self.platform == Platform.Android else self.getiOSNet()
         if noLog is False:
             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
             f.add_log(os.path.join(f.report_dir,'upflow.log'), apm_time, sendNum)
             f.add_log(os.path.join(f.report_dir,'downflow.log'), apm_time, recNum)
         return sendNum, recNum
 
-
 class FPS(object):
 
     def __init__(self, pkgName, deviceId, platform=Platform.Android, surfaceview=True):
         self.pkgName = pkgName
         self.deviceId = deviceId
         self.platform = platform
         self.surfaceview = surfaceview
@@ -336,15 +332,14 @@
             perf.stop()
             perf_value = self.downflow, self.upflow
         else:
             perf = iosP.Performance(self.deviceId, [perfTpe])
             perf_value = perf.start(self.pkgName, callback=self.callback)
         return perf_value
 
-
 class APM(object):
     """for python api"""
 
     def __init__(self, pkgName, deviceId=None, platform=Platform.Android, surfaceview=True, noLog=True, pid=None):
         self.pkgName = pkgName
         self.deviceId = deviceId
         self.platform = platform
```

### Comparing `solox-2.5.9/solox/public/apm_pk.py` & `solox-2.6.0/solox/public/apm_pk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 import re
 import time
 from solox.public.adb import adb
-from solox.public.common import Devices, file
+from solox.public.common import Devices, File
 from solox.public.fps import FPSMonitor, TimeUtils
 
 d = Devices()
-f = file()
+f = File()
 
 
 class CPU_PK:
 
     def __init__(self, pkgNameList: list, deviceId1, deviceId2):
         self.pkgNameList = pkgNameList
         self.deviceId1 = deviceId1
```

### Comparing `solox-2.5.9/solox/public/common.py` & `solox-2.6.0/solox/public/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from logzero import logger
 from solox.public.adb import adb
 from tqdm import tqdm
 import traceback
 from urllib.request import urlopen
 import ssl
 import xlwt
-
+from jinja2 import Environment, FileSystemLoader
+ 
 class Platform:
     Android = 'Android'
     iOS = 'iOS'
     Mac = 'MacOS'
     Windows = 'Windows'
 
 class Devices:
@@ -51,19 +52,16 @@
     def getDevicesName(self, deviceId):
         """Get the device name of the Android corresponding device ID"""
         devices_name = os.popen(f'{self.adb} -s {deviceId} shell getprop ro.product.model').readlines()
         return devices_name[0].strip()
 
     def getDevices(self):
         """Get all Android devices"""
-        Devices = []
         DeviceIds = self.getDeviceIds()
-        for id in DeviceIds:
-            devices_name = self.getDevicesName(id)
-            Devices.append(f'{id}({devices_name})')
+        Devices = [f'{id}({self.getDevicesName(id)})' for id in DeviceIds]
         return Devices
 
     def getIdbyDevice(self, deviceinfo, platform):
         """Obtain the corresponding device id according to the Android device information"""
         if platform == Platform.Android:
             deviceId = re.sub(u"\\(.*?\\)|\\{.*?}|\\[.*?]", "", deviceinfo)
             if deviceId not in self.getDeviceIds():
@@ -72,20 +70,20 @@
             deviceId = deviceinfo.split(':')[1]
         return deviceId
 
     def getPid(self, deviceId, pkgName):
         """Get the pid corresponding to the Android package name"""
         result = os.popen(f"{self.adb} -s {deviceId} shell ps -ef | {self.filterType()} {pkgName}").readlines()
         try:
-            processList = []
-            for process in result:
-                processInfo = '{}:{}'.format(process.split()[1],process.split()[7])
-                processList.append(processInfo)
+            processList = ['{}:{}'.format(process.split()[1],process.split()[7]) for process in result]
+            processList.reverse()
+            if len(processList) == 0:
+               logger.warning('no pid found')     
         except Exception:
-            logger.error('no pid found')
+            traceback.print_exc()
         return processList
 
     def checkPkgname(self, pkgname):
         flag = True
         replace_list = ['com.google']
         for i in replace_list:
             if i in pkgname:
@@ -111,17 +109,15 @@
             deviceUdid = deviceResult[i]['udid']
             deviceInfo.append(f'{deviceName}:{deviceUdid}')
         return deviceInfo
 
     def getPkgnameByiOS(self, udid):
         """Get all package names of the corresponding iOS device"""
         pkgResult = self.execCmd(f'tidevice --udid {udid} applist').split('\n')
-        pkgNames = []
-        for i in range(len(pkgResult)):
-            pkgNames.append(pkgResult[i].split(' ')[0])
+        pkgNames = [pkgResult[i].split(' ')[0] for i in range(len(pkgResult))]
         return pkgNames
 
     def devicesCheck(self, platform, deviceid=None, pkgname=None):
         """Check the device environment"""
         match(platform):
             case Platform.Android:
                 if len(self.getDeviceIds()) == 0:
@@ -151,22 +147,22 @@
                 result['version'] = iosInfo['ProductVersion']
                 result['serialno'] = iosInfo['SerialNumber']
                 result['wifiadr'] = iosInfo['WiFiAddress']
             case _:
                 raise Exception('{} is undefined'.format(platform)) 
         return result       
 
-class file:
+class File:
 
     def __init__(self, fileroot='.'):
         self.fileroot = fileroot
         self.report_dir = self.get_repordir()
     
     def export_excel(self, platform, scene):
-        
+        logger.info('Exporting excel ...')
         android_log_file_list = ['cpu_app','cpu_sys','mem_total','mem_native','mem_dalvik',
                                  'battery_level', 'battery_tem','upflow','downflow','fps']
         ios_log_file_list = ['cpu_app','cpu_sys', 'mem_total', 'battery_tem', 'battery_current', 
                              'battery_voltage', 'battery_power','upflow','downflow','fps','gpu']
         log_file_list = android_log_file_list if platform == 'Android' else ios_log_file_list
         wb = xlwt.Workbook(encoding = 'utf-8')
        
@@ -183,15 +179,61 @@
                     target = lines.split('=')
                     k += 1
                     for i in range(len(target)):
                         ws1.write(row, col ,target[i])
                         col += 1
                     row += 1
                     col = 0
-        wb.save(f'{scene}.xls')   
+        xls_path = os.path.join(self.report_dir, scene, f'{scene}.xls')            
+        wb.save(xls_path)
+        logger.info('Exporting excel success : {}'.format(xls_path))
+        return xls_path   
+    
+    def make_android_html(self, scene, summary : dict):
+        logger.info('Generating HTML ...')
+        STATICPATH = os.path.dirname(os.path.realpath(__file__))
+        file_loader = FileSystemLoader(os.path.join(STATICPATH, 'report_template'))
+        env = Environment(loader=file_loader)
+        template = env.get_template('android.html')
+        with open(os.path.join(self.report_dir, scene, 'report.html'),'w+') as fout:
+            html_content = template.render(cpu_app=summary['cpu_app'],cpu_sys=summary['cpu_sys'],
+                                           mem_total=summary['mem_total'],mem_native=summary['mem_native'],
+                                           mem_dalvik=summary['mem_dalvik'],fps=summary['fps'],
+                                           jank=summary['jank'],level=summary['level'],
+                                           tem=summary['tem'],net_send=summary['net_send'],
+                                           net_recv=summary['net_recv'],cpu_charts=summary['cpu_charts'],
+                                           mem_charts=summary['mem_charts'],net_charts=summary['net_charts'],
+                                           battery_charts=summary['battery_charts'],fps_charts=summary['fps_charts'],
+                                           jank_charts=summary['jank_charts'])
+            
+            fout.write(html_content)
+        html_path = os.path.join(self.report_dir, scene, 'report.html')    
+        logger.info('Generating HTML success : {}'.format(html_path))  
+        return html_path
+    
+    def make_ios_html(self, scene, summary : dict):
+        logger.info('Generating HTML ...')
+        STATICPATH = os.path.dirname(os.path.realpath(__file__))
+        file_loader = FileSystemLoader(os.path.join(STATICPATH, 'report_template'))
+        env = Environment(loader=file_loader)
+        template = env.get_template('ios.html')
+        with open(os.path.join(self.report_dir, scene, 'report.html'),'w+') as fout:
+            html_content = template.render(cpu_app=summary['cpu_app'],cpu_sys=summary['cpu_sys'],gpu=summary['gpu'],
+                                           mem_total=summary['mem_total'],fps=summary['fps'],
+                                           tem=summary['tem'],current=summary['current'],
+                                           voltage=summary['voltage'],power=summary['power'],
+                                           net_send=summary['net_send'],net_recv=summary['net_recv'],
+                                           cpu_charts=summary['cpu_charts'],mem_charts=summary['mem_charts'],
+                                           net_charts=summary['net_charts'],battery_charts=summary['battery_charts'],
+                                           fps_charts=summary['fps_charts'],gpu_charts=summary['gpu_charts'])            
+            fout.write(html_content)
+        html_path = os.path.join(self.report_dir, scene, 'report.html')    
+        logger.info('Generating HTML success : {}'.format(html_path))  
+        return html_path
+  
 
     def get_repordir(self):
         report_dir = os.path.join(os.getcwd(), 'report')
         if not os.path.exists(report_dir):
             os.mkdir(report_dir)
         return report_dir
 
@@ -219,14 +261,15 @@
                 net_dict['recv'] = recv
                 content = json.dumps(net_dict)
                 self.create_file(filename='end_net.json', content=content)
             case _:
                 logger.error('record network data failed')
     
     def make_report(self, app, devices, platform='Android', model='normal'):
+        logger.info('Generating test results ...')
         current_time = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
         result_dict = {
             "app": app,
             "icon": "",
             "platform": platform,
             "model": model,
             "devices": devices,
@@ -238,14 +281,15 @@
         if not os.path.exists(report_new_dir):
             os.mkdir(report_new_dir)
 
         for f in os.listdir(self.report_dir):
             filename = os.path.join(self.report_dir, f)
             if f.split(".")[-1] in ['log', 'json']:
                 shutil.move(filename, report_new_dir)
+        logger.info('Generating test results success: {}'.format(report_new_dir))        
 
     def instance_type(self, data):
         if isinstance(data, float):
             return 'float'
         elif isinstance(data, int):
             return 'int'
         else:
```

### Comparing `solox-2.5.9/solox/public/fps.py` & `solox-2.6.0/solox/public/fps.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/__main__.py` & `solox-2.6.0/solox/public/iosperf/__main__.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_crash.py` & `solox-2.6.0/solox/public/iosperf/_crash.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_device.py` & `solox-2.6.0/solox/public/iosperf/_device.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_hexdump.py` & `solox-2.6.0/solox/public/iosperf/_hexdump.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_imagemounter.py` & `solox-2.6.0/solox/public/iosperf/_imagemounter.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_installation.py` & `solox-2.6.0/solox/public/iosperf/_installation.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_instruments.py` & `solox-2.6.0/solox/public/iosperf/_instruments.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_ipautil.py` & `solox-2.6.0/solox/public/iosperf/_ipautil.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_perf.py` & `solox-2.6.0/solox/public/iosperf/_perf.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_proto.py` & `solox-2.6.0/solox/public/iosperf/_proto.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_relay.py` & `solox-2.6.0/solox/public/iosperf/_relay.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_safe_socket.py` & `solox-2.6.0/solox/public/iosperf/_safe_socket.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_ssl.py` & `solox-2.6.0/solox/public/iosperf/_ssl.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_sync.py` & `solox-2.6.0/solox/public/iosperf/_sync.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_types.py` & `solox-2.6.0/solox/public/iosperf/_types.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_usbmux.py` & `solox-2.6.0/solox/public/iosperf/_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_utils.py` & `solox-2.6.0/solox/public/iosperf/_utils.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/_wdaproxy.py` & `solox-2.6.0/solox/public/iosperf/_wdaproxy.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/bplist.py` & `solox-2.6.0/solox/public/iosperf/bplist.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/exceptions.py` & `solox-2.6.0/solox/public/iosperf/exceptions.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/plistlib2.py` & `solox-2.6.0/solox/public/iosperf/plistlib2.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/requests_usbmux.py` & `solox-2.6.0/solox/public/iosperf/requests_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/public/iosperf/struct2.py` & `solox-2.6.0/solox/public/iosperf/struct2.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/css/highlight.min.css` & `solox-2.6.0/solox/static/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/css/select2-bootstrap-5-theme.min.css` & `solox-2.6.0/solox/static/css/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/css/select2-bootstrap-5-theme.rtl.min.css` & `solox-2.6.0/solox/static/css/select2-bootstrap-5-theme.rtl.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/css/select2.min.css` & `solox-2.6.0/solox/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/css/sweetalert2.min.css` & `solox-2.6.0/solox/static/css/sweetalert2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/css/tabler.demo.min.css` & `solox-2.6.0/solox/static/css/tabler.demo.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/css/tabler.min.css` & `solox-2.6.0/solox/static/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/image/404.png` & `solox-2.6.0/solox/static/image/404.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/image/500.png` & `solox-2.6.0/solox/static/image/500.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/image/avatar.png` & `solox-2.6.0/solox/static/image/avatar.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/image/coffee.png` & `solox-2.6.0/solox/static/image/coffee.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/image/empty.png` & `solox-2.6.0/solox/static/image/empty.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/image/readme/home.png` & `solox-2.6.0/solox/static/image/readme/home.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/image/readme/pk.png` & `solox-2.6.0/solox/static/image/readme/pk.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/js/apexcharts.js` & `solox-2.6.0/solox/static/js/apexcharts.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/js/gray.js` & `solox-2.6.0/solox/static/js/gray.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/js/highlight.min.js` & `solox-2.6.0/solox/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/js/highstock.js` & `solox-2.6.0/solox/static/js/highstock.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/js/html2canvas.min.js` & `solox-2.6.0/solox/static/js/html2canvas.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/js/jquery.min.js` & `solox-2.6.0/solox/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/js/select2.min.js` & `solox-2.6.0/solox/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/js/socket.io.js` & `solox-2.6.0/solox/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/js/sweetalert2.min.js` & `solox-2.6.0/solox/static/js/sweetalert2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/js/tabler.demo.min.js` & `solox-2.6.0/solox/static/js/tabler.demo.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/js/tabler.min.js` & `solox-2.6.0/solox/static/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/static/logo/logo.png` & `solox-2.6.0/solox/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/templates/404.html` & `solox-2.6.0/solox/templates/404.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/templates/500.html` & `solox-2.6.0/solox/templates/500.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/templates/analysis.html` & `solox-2.6.0/solox/templates/analysis_pk.html`

 * *Files 12% similar despite different names*

```diff
@@ -33,38 +33,39 @@
     </a>
   </li>
   <li class="nav-item active" id="report_tab" style="margin-left: 20px;font-weight: bolder;">
     <a class="nav-link" href="/report?lan={{ lan }}" >
       <span class="nav-link-icon d-md-none d-lg-inline-block">
         <svg t="1643364122000" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="29349" width="300" height="300"><path d="M777 806.7c0 38.7-31.1 70.3-69.7 70.3H225.9c-38.7 0-69.9-31.6-69.9-70.3V174.4c0-38.7 31.2-70.4 69.9-70.4h481.4c38.7 0 69.7 31.7 69.7 70.4v632.3z" fill="#FFFFFF" p-id="29350"></path><path d="M707.3 886H225.9c-43.5 0-78.9-35.8-78.9-79.3V174.4c0-43.5 35.4-79.4 78.9-79.4h481.4c43.5 0 79.7 35.9 79.7 79.4v632.3c0 43.5-36.2 79.3-79.7 79.3zM225.9 113c-33.7 0-59.9 27.7-59.9 61.4v632.3c0 33.7 26.2 61.3 59.9 61.3h481.4c33.7 0 60.7-27.6 60.7-61.3V174.4c0-33.7-27-61.4-60.7-61.4H225.9z" fill="#282828" p-id="29351"></path><path d="M732 763.1c0 33.3-26.1 60.9-59.4 60.9H251.7c-33.3 0-59.7-27.6-59.7-60.9V226.9c0-33.3 26.4-60.9 59.7-60.9h420.9c33.3 0 59.4 27.5 59.4 60.9v536.2z" fill="#50BCFF" p-id="29352"></path><path d="M361.8 251.9H208.6c-4.9 0-8.9-4-8.9-8.9s4-8.9 8.9-8.9h153.1c4.9 0 8.9 4 8.9 8.9s-3.9 8.9-8.8 8.9zM549.2 313H208.6c-4.9 0-8.9-4-8.9-8.9s4-8.9 8.9-8.9h340.5c4.9 0 8.9 4 8.9 8.9s-3.9 8.9-8.8 8.9zM652 448.4H208.6c-4.9 0-8.9-4-8.9-8.9s4-8.9 8.9-8.9H652c4.9 0 8.9 4 8.9 8.9s-4 8.9-8.9 8.9zM588.4 515.8H208.6c-4.9 0-8.9-4-8.9-8.9s4-8.9 8.9-8.9h379.7c4.9 0 8.9 4 8.9 8.9 0.1 4.9-3.9 8.9-8.8 8.9z" fill="#282828" p-id="29353"></path><path d="M673.3 113.3c0 19.6-15.9 35.5-35.5 35.5h-346c-19.6 0-35.5-15.9-35.5-35.5v-6.7c0-19.6 15.9-35.5 35.5-35.5h346c19.6 0 35.5 15.9 35.5 35.5v6.7z" fill="#1A6DFF" p-id="29354"></path><path d="M637.8 157.6h-346c-24.5 0-44.4-19.9-44.4-44.4v-6.7c0-24.5 19.9-44.4 44.4-44.4h346c24.5 0 44.4 19.9 44.4 44.4v6.7c0 24.5-19.9 44.4-44.4 44.4zM291.9 80c-14.7 0-26.6 11.9-26.6 26.6v6.7c0 14.7 11.9 26.6 26.6 26.6h346c14.7 0 26.6-11.9 26.6-26.6v-6.7c0-14.7-11.9-26.6-26.6-26.6h-346z" fill="#282828" p-id="29355"></path><path d="M849.7 758.4c0 106.3-86.2 192.4-192.4 192.4-106.3 0-192.4-86.2-192.4-192.4C464.8 652.1 551 566 657.3 566c106.2 0 192.4 86.1 192.4 192.4z" fill="#FFFFFF" p-id="29356"></path><path d="M657.3 959.7c-111 0-201.3-90.3-201.3-201.3s90.3-201.3 201.3-201.3 201.3 90.3 201.3 201.3-90.3 201.3-201.3 201.3z m0-384.8c-101.2 0-183.5 82.3-183.5 183.5S556.1 942 657.3 942s183.6-82.3 183.6-183.6c-0.1-101.2-82.4-183.5-183.6-183.5z" fill="#282828" p-id="29357"></path><path d="M657.3 553.6v204.9h203.6c-0.2-112.7-91.2-204-203.6-204.9z" fill="#1A6DFF" p-id="29358"></path><path d="M860.9 767.3H657.3c-4.9 0-8.9-4-8.9-8.9V553.6c0-2.4 0.9-4.6 2.6-6.3 1.7-1.7 3.6-2.4 6.3-2.6 116.9 0.9 212.2 96.8 212.4 213.7 0 2.4-0.9 4.6-2.6 6.3-1.6 1.7-3.9 2.6-6.2 2.6z m-194.8-17.8h185.6C847 649.3 766.2 568 666.1 562.7v186.8z" fill="#282828" p-id="29359"></path><path d="M794.1 903.7c-2.3 0-4.6-0.9-6.3-2.6L652.1 764.7c-3.5-3.5-3.4-9.1 0-12.6 3.5-3.5 9.1-3.4 12.6 0l135.7 136.5c3.5 3.5 3.4 9.1 0 12.6-1.8 1.7-4 2.5-6.3 2.5z" fill="#282828" p-id="29360"></path></svg>
       </span>
-      <span class="nav-link-title strong-text">{% if lan == 'cn' %} 报告管理 {% else %} Report {% endif %}</span>
+      <span class="nav-link-title strong-text">Report{% if lan == 'cn' %} 比对模式 {% else %} PK Model {% endif %}</span>
     </a>
   </li>
 </ul>
 {% endblock %}
 
 {% block page_body %}
 <div class="col-12 mb-3">
     <div class="row row-cards">
+        {% if model == '2-devices' %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
                             <span class="bg-dark text-white avatar">
                                 CPU
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                APP
+                                Device1
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.cpuAppRate }}
+                                Avg：{{ apm_data.cpuAppRate1 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         <div class="col-sm-6 col-lg-2">
@@ -74,18 +75,18 @@
                         <div class="col-auto">
                             <span class="bg-dark text-white avatar">
                                 CPU
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                System
+                                Device2
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.cpuSystemRate }}
+                                Avg：{{ apm_data.cpuAppRate2 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         <div class="col-sm-6 col-lg-2">
@@ -95,256 +96,250 @@
                         <div class="col-auto">
                             <span class="bg-yellow text-white avatar">
                                 MEM
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Total
+                                Device1
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.totalPassAvg }}
+                                Avg：{{ apm_data.totalPassAvg1 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
-        {% if platform == 'Android' %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
                             <span class="bg-yellow text-white avatar">
                                 MEM
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Native
+                                Device2
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.nativePassAvg }}
+                                Avg：{{ apm_data.totalPassAvg2 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-yellow text-white avatar">
-                                MEM
+                            <span class="bg-pink text-white avatar">
+                                FPS
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Dalvik
+                                Device1
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.dalvikPassAvg }}
+                                Avg：{{ apm_data.fpsAvg1 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
-        {% endif %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
                             <span class="bg-pink text-white avatar">
                                 FPS
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                FPS
+                                Device2
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.fps }}
+                                Avg：{{ apm_data.fpsAvg2 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
-        {% if platform == 'Android' %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-pink text-white avatar">
-                                Jank
+                            <span class="bg-blue text-white avatar">
+                                NET
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Jank
+                                Device1
                             </div>
                             <div class="text-muted">
-                                All：{{ apm_data.jank }}
+                                All：{{ apm_data.network1 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
-        {% if platform == 'Android' %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-green text-white avatar">
-                                A.C
+                            <span class="bg-blue text-white avatar">
+                                NET
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Level
+                                Device2
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.batteryLevel }}
+                                All：{{ apm_data.network2 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
+        {% else %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-green text-white avatar">
-                                A.C
+                            <span class="bg-dark text-white avatar">
+                                CPU
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Temperature
+                                APP1
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.batteryTeml }}
+                                Avg：{{ apm_data.cpuAppRate1 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
-        {% else %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-green text-white avatar">
-                                A.C
+                            <span class="bg-dark text-white avatar">
+                                CPU
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Temperature
+                                APP2
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.batteryTeml }}
+                                Avg：{{ apm_data.cpuAppRate2 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-green text-white avatar">
-                                A.C
+                            <span class="bg-yellow text-white avatar">
+                                MEM
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Current
+                                APP1
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.batteryCurrent }}
+                                Avg：{{ apm_data.totalPassAvg1 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-green text-white avatar">
-                                A.C
+                            <span class="bg-yellow text-white avatar">
+                                MEM
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Voltage
+                                APP2
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.batteryVoltage }}
+                                Avg：{{ apm_data.totalPassAvg2 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-green text-white avatar">
-                                A.C
+                            <span class="bg-pink text-white avatar">
+                                FPS
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Power
+                                APP1
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.batteryPower }}
+                                Avg：{{ apm_data.fpsAvg1 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
-        {% endif %}
-        {% endif %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-blue text-white avatar">
-                                NET
+                            <span class="bg-pink text-white avatar">
+                                FPS
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Send
+                                APP2
                             </div>
                             <div class="text-muted">
-                                All：{{ apm_data.flow_send }}
+                                Avg：{{ apm_data.fpsAvg2 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         <div class="col-sm-6 col-lg-2">
@@ -354,40 +349,39 @@
                         <div class="col-auto">
                             <span class="bg-blue text-white avatar">
                                 NET
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Recv
+                                APP1
                             </div>
                             <div class="text-muted">
-                                All：{{ apm_data.flow_recv }}
+                                All：{{ apm_data.network1 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
-        {% if platform == 'iOS' %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-purple text-white avatar">
-                                GPU
+                            <span class="bg-blue text-white avatar">
+                                NET
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                GPU
+                                APP2
                             </div>
                             <div class="text-muted">
-                                Avg: {{ apm_data.gpu }}
+                                All：{{ apm_data.network2 }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         {% endif %}
@@ -438,48 +432,14 @@
                 </a>
             </div>
         </div>
         <div class="card-body">
             <div id="chart-fps"></div>
         </div>
     </div>
-    {% if platform == 'Android' %}
-    <div class="card jank-card mt-3">
-        <div class="card-header">
-            <div class='card-title'>JANK</div>
-            <div class="card-actions btn-actions">
-                <a class="btn-action cursor-pointer" id="jank_loading">
-                    <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
-                </a>
-                <a class="btn-action cursor-pointer" id="jank_png" onclick="screenshot('jank-card','jank.png')">
-                    <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
-                </a>
-            </div>
-        </div>
-        <div class="card-body">
-            <div id="chart-jank"></div>
-        </div>
-    </div>
-    <div class="card battery-card mt-3">
-        <div class="card-header">
-            <div class='card-title'>A.C（%）</div>
-            <div class="card-actions btn-actions">
-                <a class="btn-action cursor-pointer" id="battery_loading">
-                    <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
-                </a>
-                <a class="btn-action cursor-pointer" id="battery_png" onclick="screenshot('battery-card','battery.png')">
-                    <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
-                </a>
-            </div>
-        </div>
-        <div class="card-body">
-            <div id="chart-battery"></div>
-        </div>
-    </div>
-    {% endif %}
     <div class="card networkdata-card mt-3">
         <div class="card-header">
             <div class='card-title'>Network Data（KB）</div>
             <div class="card-actions btn-actions">
                 <a class="btn-action cursor-pointer" id="networkdata_loading">
                     <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
                 </a>
@@ -488,50 +448,27 @@
                 </a>
             </div>
         </div>
         <div class="card-body">
             <div id="chart-networkdata"></div>
         </div>
     </div>
-    {% if platform == 'iOS' %}
-    <div class="card gpu-card mt-3">
-        <div class="card-header">
-            <div class='card-title'>GPU（%）</div>
-            <div class="card-actions btn-actions">
-                <a class="btn-action cursor-pointer" id="gpu_loading">
-                    <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
-                </a>
-                <a class="btn-action cursor-pointer" id="gpu_png" onclick="screenshot('gpu-card','gpu.png')">
-                    <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
-                </a>
-            </div>
-        </div>
-        <div class="card-body">
-            <div id="chart-gpu"></div>
-        </div>
-    </div>
-    {% endif %}
 
 </div>
 {% endblock %}
 
 {% block js %}
 <script>
 
+    const model = '{{ model }}';
+
     $(document).ready(function() {
         $('#cpu_loading').click();
         $('#mem_loading').click();
         $('#fps_loading').click();
-        if(platform == 'Android'){
-            $('#jank_loading').click();
-        }
-        if(platform == 'iOS'){
-            $('#gpu_loading').click();
-        }
-        $('#battery_loading').click();
         $('#networkdata_loading').click();
     });
 
     function options(type,dataLabels=false) {
         let options = {
             chart: {
                 type: type,
@@ -545,15 +482,15 @@
                     enabled: false
                 },
             },
             dataLabels: {
                 enabled: dataLabels
             },
             fill: {
-                opacity: 1
+                opacity: 1,
             },
             stroke: {
                 width: 2,
                 lineCap: "round",
                 curve: "smooth",
             },
             series: [],
@@ -568,242 +505,169 @@
         return options
     }
 
     var cpu_chart = new ApexCharts(document.querySelector("#chart-cpu"), options('line'));
     cpu_chart.render();
     $('#cpu_loading').click(function () {
         $.ajax({
-            url: '/apm/log',
+            url: '/apm/log/pk',
             type: "GET",
             async: true,
             cache: false,
             data:{
                 scene:'{{ scene }}',
-                target:'cpu',
-                platform:platform
+                target1:'cpu_app1',
+                target2:'cpu_app2'
             },
             beforeSend: function () {
                 SwalLoading('Loading','')
             },
             complete: function () {
                 swal.close();
             },
             success: function (data) {
-                cpu_chart.updateSeries([{
-                    name: 'app Usage',
-                    data: data['cpuAppData']
-                },{
-                    name: 'sys Usage',
-                    data: data['cpuSysData']
-                }])
-            }
-        });
-    });
-    
-    var battery_chart = new ApexCharts(document.querySelector("#chart-battery"), options('line'));
-        battery_chart.render();
-        $('#battery_loading').click(function () {
-            $.ajax({
-                url: '/apm/log',
-                type: "GET",
-                async: true,
-                cache: false,
-                data:{
-                    scene:'{{ scene }}',
-                    target:'battery',
-                    platform:platform
-                },
-                beforeSend: function () {
-                    SwalLoading('Loading','')
-                },
-                complete: function () {
-                    swal.close();
-                },
-                success: function (data) {
-                    if(platform == 'Android'){
-                        battery_chart.updateSeries([{
-                            name: 'level',
-                            data: data['batteryLevel']
-                        },{
-                            name: 'temperature',
-                            data: data['batteryTem']
-                        }])
-                    }else {
-                        battery_chart.updateSeries([{
-                            name: 'temperature',
-                            data: data['batteryTem']
-                        },{
-                            name: 'Current',
-                            data: data['batteryCurrent']
-                        },{
-                            name: 'Voltage',
-                            data: data['batteryVoltage']
-                        },{
-                            name: 'Power',
-                            data: data['batteryPower']
-                        }])
-                    }
-                }
-            });
-        });
-
-    if(platform == 'Android'){
-        var jank_chart = new ApexCharts(document.querySelector("#chart-jank"), options('line'));
-        jank_chart.render();
-        $('#jank_loading').click(function () {
-            $.ajax({
-                url: '/apm/log',
-                type: "GET",
-                async: true,
-                cache: false,
-                data:{
-                    scene:'{{ scene }}',
-                    target:'fps',
-                    platform:platform
-                },
-                beforeSend: function () {
-                    SwalLoading('Loading','')
-                },
-                complete: function () {
-                    swal.close();
-                },
-                success: function (data) {
-                    jank_chart.updateSeries([{
-                        name: 'jank',
-                        data: data['jank']
+                if(model == '2-devices'){
+                    cpu_chart.updateSeries([{
+                        name: 'Device1',
+                        data: data['first']
+                    },{
+                        name: 'Device2',
+                        data: data['second']
                     }])
-                }
-            });
-        });
-    }
-
-    if(platform == 'iOS'){
-        var gpu_chart = new ApexCharts(document.querySelector("#chart-gpu"), options('line'));
-        gpu_chart.render();
-        $('#gpu_loading').click(function () {
-            $.ajax({
-                url: '/apm/log',
-                type: "GET",
-                async: true,
-                cache: false,
-                data:{
-                    scene:'{{ scene }}',
-                    target:'gpu',
-                    platform:platform
-                },
-                beforeSend: function () {
-                    SwalLoading('Loading','')
-                },
-                complete: function () {
-                    swal.close();
-                },
-                success: function (data) {
-                    gpu_chart.updateSeries([{
-                        name: 'gpu',
-                        data: data['gpu']
+                }else{
+                    cpu_chart.updateSeries([{
+                        name: 'APP1',
+                        data: data['first']
+                    },{
+                        name: 'APP2',
+                        data: data['second']
                     }])
                 }
-            });
+
+            }
         });
-    }
+    });
 
     var fps_chart = new ApexCharts(document.querySelector("#chart-fps"), options('line'));
     fps_chart.render();
     $('#fps_loading').click(function () {
         $.ajax({
-            url: '/apm/log',
+            url: '/apm/log/pk',
             type: "GET",
             async: true,
             cache: false,
             data:{
                 scene:'{{ scene }}',
-                target:'fps',
-                platform:platform
+                target1:'fps1',
+                target2:'fps2'
             },
             beforeSend: function () {
                 SwalLoading('Loading','')
             },
             complete: function () {
                 swal.close();
             },
             success: function (data) {
-                fps_chart.updateSeries([{
-                    name: 'fps',
-                    data: data['fps']
-                }])
+                if(model == '2-devices'){
+                    fps_chart.updateSeries([{
+                        name: 'Device1',
+                        data: data['first']
+                    },{
+                        name: 'Device2',
+                        data: data['second']
+                    }])
+                }else{
+                    fps_chart.updateSeries([{
+                        name: 'APP1',
+                        data: data['first']
+                    },{
+                        name: 'APP2',
+                        data: data['second']
+                    }])
+                }
             }
         });
     });
 
     var mem_chart = new ApexCharts(document.querySelector("#chart-mem"), options('line'));
     mem_chart.render();
     $('#mem_loading').click(function () {
         $.ajax({
-            url: '/apm/log',
+            url: '/apm/log/pk',
             type: "GET",
             async: true,
             cache: false,
             data:{
                 scene:'{{ scene }}',
-                target:'mem',
-                platform:platform
+                target1:'mem1',
+                target2:'mem2'
             },
             beforeSend: function () {
                 SwalLoading('Loading','')
             },
             complete: function () {
                 swal.close();
             },
             success: function (data) {
-                if(platform == 'Android'){
+                if(model == '2-devices'){
                     mem_chart.updateSeries([{
-                        name: 'total',
-                        data: data['memTotalData']
-                    },{
-                        name: 'native',
-                        data: data['memNativeData']
+                        name: 'Device1',
+                        data: data['first']
                     },{
-                        name: 'dalvik',
-                        data: data['memDalvikData']
+                        name: 'Device2',
+                        data: data['second']
                     }])
                 }else{
                     mem_chart.updateSeries([{
-                        name: 'total',
-                        data: data['memTotalData']
+                        name: 'APP1',
+                        data: data['first']
+                    },{
+                        name: 'APP2',
+                        data: data['second']
                     }])
                 }
             }
         });
     });
 
     var network_chart = new ApexCharts(document.querySelector("#chart-networkdata"), options('line',false));
     network_chart.render();
     $('#networkdata_loading').click(function () {
         $.ajax({
-            url: '/apm/log',
+            url: '/apm/log/pk',
             type: "GET",
             async: true,
             cache: false,
             data:{
                 scene:'{{ scene }}',
-                target:'flow',
-                platform:platform
+                target1:'network1',
+                target2:'network2'
             },
             beforeSend: function () {
                 SwalLoading('Loading','')
             },
             complete: function () {
                 swal.close();
             },
             success: function (data) {
-                network_chart.updateSeries([{
-                    name: 'send',
-                    data: data['upFlow']
-                },{
-                    name: 'recv',
-                    data: data['downFlow']
-                }])
+                if(model == '2-devices'){
+                    network_chart.updateSeries([{
+                        name: 'Device1',
+                        data: data['first']
+                    },{
+                        name: 'Device2',
+                        data: data['second']
+                    }])
+                }else{
+                    network_chart.updateSeries([{
+                        name: 'APP1',
+                        data: data['first']
+                    },{
+                        name: 'APP2',
+                        data: data['second']
+                    }])
+                }
             }
         });
     });
 </script>
 {% endblock %}
```

### Comparing `solox-2.5.9/solox/templates/analysis_pk.html` & `solox-2.6.0/solox/templates/analysis.html`

 * *Files 25% similar despite different names*

```diff
@@ -10,17 +10,21 @@
 <svg t="1635085520789" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="165732" width="200" height="200"><path d="M360.704 280.746667l45.226667-45.226667 246.570666 246.528a42.666667 42.666667 0 0 1 0 60.330667l-246.528 246.570666-45.22666601-45.269333 231.42400001-231.466667-231.466667-231.424z" p-id="165733"></path></svg>
 {{ scene }}
 {% endblock %}
 
 {% block ms_auto %}
 <div class="col-auto ms-auto d-print-none">
     <div class="btn-list">
+        <a onclick="saveHtml('{{ platform }}','{{ scene }}')" class="btn">
+            <svg t="1681980190479" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="13623" width="50" height="50"><path d="M192 384h640a42.666667 42.666667 0 0 1 42.666667 42.666667v362.666666a42.666667 42.666667 0 0 1-42.666667 42.666667H192v106.666667a21.333333 21.333333 0 0 0 21.333333 21.333333h725.333334a21.333333 21.333333 0 0 0 21.333333-21.333333V308.821333L949.909333 298.666667h-126.528A98.048 98.048 0 0 1 725.333333 200.618667V72.661333L716.714667 64H213.333333a21.333333 21.333333 0 0 0-21.333333 21.333333v298.666667zM128 832H42.666667a42.666667 42.666667 0 0 1-42.666667-42.666667V426.666667a42.666667 42.666667 0 0 1 42.666667-42.666667h85.333333V85.333333a85.333333 85.333333 0 0 1 85.333333-85.333333h530.026667L1024 282.453333V938.666667a85.333333 85.333333 0 0 1-85.333333 85.333333H213.333333a85.333333 85.333333 0 0 1-85.333333-85.333333v-106.666667zM64 472.490667V746.666667h37.226667v-121.344h93.866666V746.666667h37.248V472.490667H195.093333v114.432h-93.866666v-114.432H64z m195.370667 0v38.4h52.544V746.666667h37.248V510.890667h52.522666v-38.4h-142.293333z m169.386666 0V746.666667h37.226667v-188.928h1.28L534.058667 746.666667h32.128l66.837333-188.928h1.28V746.666667h37.226667V472.490667h-43.605334l-77.013333 215.04h-1.28l-77.312-215.04h-43.605333z m287.36 0V746.666667H832v-38.4h-78.976V472.490667h-36.906667z" fill="#6CB600" p-id="13624"></path></svg>
+            {% if lan == 'cn' %} 保存Html {% else %} Save Html {% endif %}
+        </a>
         <a download="report.png" onclick="screenshot('sceen-body','report.png')" class="btn">
-            <svg t="1645944931399" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="4026" width="200" height="200"><path d="M523.73504 319.29344h-204.8c-16.896 0-30.72-13.824-30.72-30.72s13.824-30.72 30.72-30.72h204.8c16.896 0 30.72 13.824 30.72 30.72s-13.824 30.72-30.72 30.72zM605.65504 452.41344h-286.72c-16.896 0-30.72-13.824-30.72-30.72s13.824-30.72 30.72-30.72h286.72c16.896 0 30.72 13.824 30.72 30.72s-13.824 30.72-30.72 30.72z" fill="#FFFFFF" p-id="4027"></path><path d="M658.176 146.57536H267.8784c-40.07936 0-72.58112 32.13312-72.58112 71.7824v587.29472c0 39.63904 32.49152 71.7824 72.58112 71.7824h488.2432c40.07936 0 72.58112-32.13312 72.58112-71.7824V303.18592L658.176 146.57536z" fill="#3889FF" p-id="4028"></path><path d="M317.10208 195.29728h341.06368v146.176H317.10208zM268.38016 633.8048h487.23968v243.61984H268.38016z" fill="#FFFFFF" p-id="4029"></path><path d="M598.71232 317.10208a25.6 25.6 0 0 1-25.6-25.6v-46.24384a25.6 25.6 0 1 1 51.2 0v46.24384a25.6 25.6 0 0 1-25.6 25.6zM640 736.2048h-256a25.6 25.6 0 1 1 0-51.2h256a25.6 25.6 0 1 1 0 51.2zM643.0208 829.17376h-256a25.6 25.6 0 1 1 0-51.2h256a25.6 25.6 0 0 1 0 51.2z" fill="#3889FF" p-id="4030"></path></svg>
-            {% if lan == 'cn' %} 保存图片 {% else %} Save image {% endif %}
+            <svg t="1681980127752" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="11730" width="50" height="50"><path d="M957.31 368.25L903.1 732.12c-6 40.19-33.93 71.32-69.35 82.48a96.61 96.61 0 0 1-44.19 3.26L213.21 727c-39.51-6.23-70-35.53-80.55-72.54l90.55-64.06L363.29 702l193.4-234.78L847.8 681.67V394c0-56.57-44.59-102.43-99.6-102.43H177.34l6.73-45.17c8.33-55.92 59.16-94.3 113.53-85.73l576.35 90.83c54.37 8.56 91.69 60.83 83.36 116.75z" fill="#C5E3FF" p-id="11731"></path><path d="M804.86 831.57a110.71 110.71 0 0 1-17.24-1.36l-576.35-90.83c-42.89-6.76-78.46-38.74-90.62-81.47a12.5 12.5 0 0 1 4.8-13.62L216 580.22a12.5 12.5 0 0 1 15 0.43l130.45 103.9L547 459.27a12.5 12.5 0 0 1 17.06-2.12L835.3 656.93V394c0-49.59-39.07-89.93-87.1-89.93H177.34A12.5 12.5 0 0 1 165 289.71l6.73-45.17a114.5 114.5 0 0 1 45.56-76.09 109.35 109.35 0 0 1 82.29-20.14l576.35 90.83c61 9.62 103.11 68.37 93.78 131L915.46 734A115.87 115.87 0 0 1 889 792.38a112.1 112.1 0 0 1-51.45 34.14 108.3 108.3 0 0 1-32.69 5.05zM147.47 659.32c11.42 29.21 37.19 50.55 67.69 55.36l576.35 90.83a83.72 83.72 0 0 0 38.49-2.84c31.84-10 55.68-38.44 60.74-72.4l54.21-363.87c7.31-49.07-25.41-95.08-72.95-102.58L295.65 173a84.54 84.54 0 0 0-63.6 15.6 89.67 89.67 0 0 0-35.62 59.63l-4.59 30.82h556.37c61.81 0 112.1 51.56 112.1 114.93v287.69a12.5 12.5 0 0 1-19.91 10.06L558.81 484.3 372.93 709.93a12.5 12.5 0 0 1-17.44 1.83L222.77 606z" fill="#3D9FF9" p-id="11732"></path><path d="M748.21 877H165.12C103.31 877 53 825.48 53 762.11V394c0-63.37 50.29-114.93 112.1-114.93h583.11c61.81 0 112.1 51.56 112.1 114.93v368.11C860.3 825.48 810 877 748.21 877zM165.13 304c-48 0-87.1 40.34-87.1 89.93v368.18C78 811.7 117.1 852 165.12 852h583.09c48 0 87.1-40.34 87.1-89.93V394c0-49.59-39.07-89.93-87.1-89.93z" fill="#3D9FF9" p-id="11733"></path><path d="M748.21 877H165.12C103.31 877 53 825.48 53 762.11V702a12.5 12.5 0 0 1 5.28-10.2L216 580.22a12.5 12.5 0 0 1 15 0.43l130.45 103.9L547 459.27a12.5 12.5 0 0 1 17.06-2.12L855.22 671.6a12.5 12.5 0 0 1 5.09 10.06v80.44a117 117 0 0 1-15.75 58.77 114.17 114.17 0 0 1-40.07 40.64A109.94 109.94 0 0 1 748.21 877zM78 708.46v53.65C78 811.7 117.1 852 165.12 852h583.09c30.88 0 58.82-16.35 74.74-43.73a92 92 0 0 0 12.36-46.21V688l-276.5-203.7-185.88 225.63a12.5 12.5 0 0 1-17.44 1.83L222.77 606z" fill="#3D9FF9" p-id="11734"></path><path d="M847.8 681.67v80.44a104.16 104.16 0 0 1-14.05 52.49c-17.39 29.91-49.19 49.94-85.54 49.94H165.12c-55 0-99.6-45.86-99.6-102.43V702l67.14-47.5 90.55-64.06L363.29 702l193.4-234.78z" fill="#C5E3FF" p-id="11735"></path><path d="M748.21 877H165.12C103.31 877 53 825.48 53 762.11V702a12.5 12.5 0 0 1 5.28-10.2L216 580.22a12.5 12.5 0 0 1 15 0.43l130.45 103.9L547 459.27a12.5 12.5 0 0 1 17.06-2.12L855.22 671.6a12.5 12.5 0 0 1 5.09 10.06v80.44a117 117 0 0 1-15.75 58.77 114.17 114.17 0 0 1-40.07 40.64A109.94 109.94 0 0 1 748.21 877zM78 708.46v53.65C78 811.7 117.1 852 165.12 852h583.09c30.88 0 58.82-16.35 74.74-43.73a92 92 0 0 0 12.36-46.21V688l-276.5-203.7-185.88 225.63a12.5 12.5 0 0 1-17.44 1.83L222.77 606z" fill="#3D9FF9" p-id="11736"></path><path d="M226.91 418.1m-69.43 0a69.43 69.43 0 1 0 138.86 0 69.43 69.43 0 1 0-138.86 0Z" fill="#C5E3FF" p-id="11737"></path><path d="M226.91 500a81.93 81.93 0 1 1 81.93-81.93A82 82 0 0 1 226.91 500z m0-138.86a56.93 56.93 0 1 0 56.93 56.93 57 57 0 0 0-56.93-56.9z" fill="#3D9FF9" p-id="11738"></path></svg>
+            {% if lan == 'cn' %} 保存图片 {% else %} Save Image {% endif %}
         </a>
     </div>
 </div>
 {% endblock %}
 
 {% block navbar_nav %}
 <ul class="navbar-nav">
@@ -33,39 +37,38 @@
     </a>
   </li>
   <li class="nav-item active" id="report_tab" style="margin-left: 20px;font-weight: bolder;">
     <a class="nav-link" href="/report?lan={{ lan }}" >
       <span class="nav-link-icon d-md-none d-lg-inline-block">
         <svg t="1643364122000" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="29349" width="300" height="300"><path d="M777 806.7c0 38.7-31.1 70.3-69.7 70.3H225.9c-38.7 0-69.9-31.6-69.9-70.3V174.4c0-38.7 31.2-70.4 69.9-70.4h481.4c38.7 0 69.7 31.7 69.7 70.4v632.3z" fill="#FFFFFF" p-id="29350"></path><path d="M707.3 886H225.9c-43.5 0-78.9-35.8-78.9-79.3V174.4c0-43.5 35.4-79.4 78.9-79.4h481.4c43.5 0 79.7 35.9 79.7 79.4v632.3c0 43.5-36.2 79.3-79.7 79.3zM225.9 113c-33.7 0-59.9 27.7-59.9 61.4v632.3c0 33.7 26.2 61.3 59.9 61.3h481.4c33.7 0 60.7-27.6 60.7-61.3V174.4c0-33.7-27-61.4-60.7-61.4H225.9z" fill="#282828" p-id="29351"></path><path d="M732 763.1c0 33.3-26.1 60.9-59.4 60.9H251.7c-33.3 0-59.7-27.6-59.7-60.9V226.9c0-33.3 26.4-60.9 59.7-60.9h420.9c33.3 0 59.4 27.5 59.4 60.9v536.2z" fill="#50BCFF" p-id="29352"></path><path d="M361.8 251.9H208.6c-4.9 0-8.9-4-8.9-8.9s4-8.9 8.9-8.9h153.1c4.9 0 8.9 4 8.9 8.9s-3.9 8.9-8.8 8.9zM549.2 313H208.6c-4.9 0-8.9-4-8.9-8.9s4-8.9 8.9-8.9h340.5c4.9 0 8.9 4 8.9 8.9s-3.9 8.9-8.8 8.9zM652 448.4H208.6c-4.9 0-8.9-4-8.9-8.9s4-8.9 8.9-8.9H652c4.9 0 8.9 4 8.9 8.9s-4 8.9-8.9 8.9zM588.4 515.8H208.6c-4.9 0-8.9-4-8.9-8.9s4-8.9 8.9-8.9h379.7c4.9 0 8.9 4 8.9 8.9 0.1 4.9-3.9 8.9-8.8 8.9z" fill="#282828" p-id="29353"></path><path d="M673.3 113.3c0 19.6-15.9 35.5-35.5 35.5h-346c-19.6 0-35.5-15.9-35.5-35.5v-6.7c0-19.6 15.9-35.5 35.5-35.5h346c19.6 0 35.5 15.9 35.5 35.5v6.7z" fill="#1A6DFF" p-id="29354"></path><path d="M637.8 157.6h-346c-24.5 0-44.4-19.9-44.4-44.4v-6.7c0-24.5 19.9-44.4 44.4-44.4h346c24.5 0 44.4 19.9 44.4 44.4v6.7c0 24.5-19.9 44.4-44.4 44.4zM291.9 80c-14.7 0-26.6 11.9-26.6 26.6v6.7c0 14.7 11.9 26.6 26.6 26.6h346c14.7 0 26.6-11.9 26.6-26.6v-6.7c0-14.7-11.9-26.6-26.6-26.6h-346z" fill="#282828" p-id="29355"></path><path d="M849.7 758.4c0 106.3-86.2 192.4-192.4 192.4-106.3 0-192.4-86.2-192.4-192.4C464.8 652.1 551 566 657.3 566c106.2 0 192.4 86.1 192.4 192.4z" fill="#FFFFFF" p-id="29356"></path><path d="M657.3 959.7c-111 0-201.3-90.3-201.3-201.3s90.3-201.3 201.3-201.3 201.3 90.3 201.3 201.3-90.3 201.3-201.3 201.3z m0-384.8c-101.2 0-183.5 82.3-183.5 183.5S556.1 942 657.3 942s183.6-82.3 183.6-183.6c-0.1-101.2-82.4-183.5-183.6-183.5z" fill="#282828" p-id="29357"></path><path d="M657.3 553.6v204.9h203.6c-0.2-112.7-91.2-204-203.6-204.9z" fill="#1A6DFF" p-id="29358"></path><path d="M860.9 767.3H657.3c-4.9 0-8.9-4-8.9-8.9V553.6c0-2.4 0.9-4.6 2.6-6.3 1.7-1.7 3.6-2.4 6.3-2.6 116.9 0.9 212.2 96.8 212.4 213.7 0 2.4-0.9 4.6-2.6 6.3-1.6 1.7-3.9 2.6-6.2 2.6z m-194.8-17.8h185.6C847 649.3 766.2 568 666.1 562.7v186.8z" fill="#282828" p-id="29359"></path><path d="M794.1 903.7c-2.3 0-4.6-0.9-6.3-2.6L652.1 764.7c-3.5-3.5-3.4-9.1 0-12.6 3.5-3.5 9.1-3.4 12.6 0l135.7 136.5c3.5 3.5 3.4 9.1 0 12.6-1.8 1.7-4 2.5-6.3 2.5z" fill="#282828" p-id="29360"></path></svg>
       </span>
-      <span class="nav-link-title strong-text">Report{% if lan == 'cn' %} 比对模式 {% else %} PK Model {% endif %}</span>
+      <span class="nav-link-title strong-text">{% if lan == 'cn' %} 报告管理 {% else %} Report {% endif %}</span>
     </a>
   </li>
 </ul>
 {% endblock %}
 
 {% block page_body %}
 <div class="col-12 mb-3">
     <div class="row row-cards">
-        {% if model == '2-devices' %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
                             <span class="bg-dark text-white avatar">
                                 CPU
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Device1
+                                APP
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.cpuAppRate1 }}
+                                Avg：{{ apm_data.cpuAppRate }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         <div class="col-sm-6 col-lg-2">
@@ -75,18 +78,18 @@
                         <div class="col-auto">
                             <span class="bg-dark text-white avatar">
                                 CPU
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Device2
+                                System
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.cpuAppRate2 }}
+                                Avg：{{ apm_data.cpuSystemRate }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         <div class="col-sm-6 col-lg-2">
@@ -96,250 +99,256 @@
                         <div class="col-auto">
                             <span class="bg-yellow text-white avatar">
                                 MEM
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Device1
+                                Total
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.totalPassAvg1 }}
+                                Avg：{{ apm_data.totalPassAvg }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
+        {% if platform == 'Android' %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
                             <span class="bg-yellow text-white avatar">
                                 MEM
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Device2
+                                Native
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.totalPassAvg2 }}
+                                Avg：{{ apm_data.nativePassAvg }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-pink text-white avatar">
-                                FPS
+                            <span class="bg-yellow text-white avatar">
+                                MEM
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Device1
+                                Dalvik
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.fpsAvg1 }}
+                                Avg：{{ apm_data.dalvikPassAvg }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
+        {% endif %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
                             <span class="bg-pink text-white avatar">
                                 FPS
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Device2
+                                FPS
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.fpsAvg2 }}
+                                Avg：{{ apm_data.fps }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
+        {% if platform == 'Android' %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-blue text-white avatar">
-                                NET
+                            <span class="bg-pink text-white avatar">
+                                Jank
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Device1
+                                Jank
                             </div>
                             <div class="text-muted">
-                                All：{{ apm_data.network1 }}
+                                All：{{ apm_data.jank }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
+        {% if platform == 'Android' %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-blue text-white avatar">
-                                NET
+                            <span class="bg-green text-white avatar">
+                                A.C
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                Device2
+                                Level
                             </div>
                             <div class="text-muted">
-                                All：{{ apm_data.network2 }}
+                                Avg：{{ apm_data.batteryLevel }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
-        {% else %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-dark text-white avatar">
-                                CPU
+                            <span class="bg-green text-white avatar">
+                                A.C
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                APP1
+                                Temperature
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.cpuAppRate1 }}
+                                Avg：{{ apm_data.batteryTeml }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
+        {% else %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-dark text-white avatar">
-                                CPU
+                            <span class="bg-green text-white avatar">
+                                A.C
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                APP2
+                                Temperature
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.cpuAppRate2 }}
+                                Avg：{{ apm_data.batteryTeml }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-yellow text-white avatar">
-                                MEM
+                            <span class="bg-green text-white avatar">
+                                A.C
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                APP1
+                                Current
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.totalPassAvg1 }}
+                                Avg：{{ apm_data.batteryCurrent }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-yellow text-white avatar">
-                                MEM
+                            <span class="bg-green text-white avatar">
+                                A.C
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                APP2
+                                Voltage
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.totalPassAvg2 }}
+                                Avg：{{ apm_data.batteryVoltage }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-pink text-white avatar">
-                                FPS
+                            <span class="bg-green text-white avatar">
+                                A.C
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                APP1
+                                Power
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.fpsAvg1 }}
+                                Avg：{{ apm_data.batteryPower }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
+        {% endif %}
+        {% endif %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-pink text-white avatar">
-                                FPS
+                            <span class="bg-blue text-white avatar">
+                                NET
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                APP2
+                                Send
                             </div>
                             <div class="text-muted">
-                                Avg：{{ apm_data.fpsAvg2 }}
+                                All：{{ apm_data.flow_send }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         <div class="col-sm-6 col-lg-2">
@@ -349,39 +358,40 @@
                         <div class="col-auto">
                             <span class="bg-blue text-white avatar">
                                 NET
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                APP1
+                                Recv
                             </div>
                             <div class="text-muted">
-                                All：{{ apm_data.network1 }}
+                                All：{{ apm_data.flow_recv }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
+        {% if platform == 'iOS' %}
         <div class="col-sm-6 col-lg-2">
             <div class="card card-sm">
                 <div class="card-body">
                     <div class="row align-items-center">
                         <div class="col-auto">
-                            <span class="bg-blue text-white avatar">
-                                NET
+                            <span class="bg-purple text-white avatar">
+                                GPU
                             </span>
                         </div>
                         <div class="col">
                             <div class="font-weight-medium">
-                                APP2
+                                GPU
                             </div>
                             <div class="text-muted">
-                                All：{{ apm_data.network2 }}
+                                Avg: {{ apm_data.gpu }}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         {% endif %}
@@ -432,14 +442,48 @@
                 </a>
             </div>
         </div>
         <div class="card-body">
             <div id="chart-fps"></div>
         </div>
     </div>
+    {% if platform == 'Android' %}
+    <div class="card jank-card mt-3">
+        <div class="card-header">
+            <div class='card-title'>JANK</div>
+            <div class="card-actions btn-actions">
+                <a class="btn-action cursor-pointer" id="jank_loading">
+                    <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
+                </a>
+                <a class="btn-action cursor-pointer" id="jank_png" onclick="screenshot('jank-card','jank.png')">
+                    <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
+                </a>
+            </div>
+        </div>
+        <div class="card-body">
+            <div id="chart-jank"></div>
+        </div>
+    </div>
+    <div class="card battery-card mt-3">
+        <div class="card-header">
+            <div class='card-title'>A.C（%）</div>
+            <div class="card-actions btn-actions">
+                <a class="btn-action cursor-pointer" id="battery_loading">
+                    <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
+                </a>
+                <a class="btn-action cursor-pointer" id="battery_png" onclick="screenshot('battery-card','battery.png')">
+                    <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
+                </a>
+            </div>
+        </div>
+        <div class="card-body">
+            <div id="chart-battery"></div>
+        </div>
+    </div>
+    {% endif %}
     <div class="card networkdata-card mt-3">
         <div class="card-header">
             <div class='card-title'>Network Data（KB）</div>
             <div class="card-actions btn-actions">
                 <a class="btn-action cursor-pointer" id="networkdata_loading">
                     <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
                 </a>
@@ -448,30 +492,127 @@
                 </a>
             </div>
         </div>
         <div class="card-body">
             <div id="chart-networkdata"></div>
         </div>
     </div>
+    {% if platform == 'iOS' %}
+    <div class="card gpu-card mt-3">
+        <div class="card-header">
+            <div class='card-title'>GPU（%）</div>
+            <div class="card-actions btn-actions">
+                <a class="btn-action cursor-pointer" id="gpu_loading">
+                    <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
+                </a>
+                <a class="btn-action cursor-pointer" id="gpu_png" onclick="screenshot('gpu-card','gpu.png')">
+                    <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
+                </a>
+            </div>
+        </div>
+        <div class="card-body">
+            <div id="chart-gpu"></div>
+        </div>
+    </div>
+    {% endif %}
 
 </div>
 {% endblock %}
 
 {% block js %}
 <script>
 
-    const model = '{{ model }}';
-
     $(document).ready(function() {
         $('#cpu_loading').click();
         $('#mem_loading').click();
         $('#fps_loading').click();
+        if(platform == 'Android'){
+            $('#jank_loading').click();
+        }
+        if(platform == 'iOS'){
+            $('#gpu_loading').click();
+        }
+        $('#battery_loading').click();
         $('#networkdata_loading').click();
     });
 
+    function saveHtml(platform, scene){
+        if(platform=='Android'){
+            saveAndroidHtml(scene)
+        }else{
+            saveiOSHtml(scene)
+        }
+    }
+
+    function saveAndroidHtml(scene){
+        $.ajax({
+            url: "/apm/export/html/android",
+            type: "GET",
+            async: true,
+            cache: false,
+            data:{
+                scene: scene,
+                cpu_app:'{{ apm_data.cpuAppRate }}',
+                cpu_sys:'{{ apm_data.cpuSystemRate }}',
+                mem_total:'{{ apm_data.totalPassAvg }}',
+                mem_native:'{{ apm_data.nativePassAvg }}',
+                mem_dalvik:'{{ apm_data.dalvikPassAvg }}',
+                fps:'{{ apm_data.fps }}',
+                jank:'{{ apm_data.jank }}',
+                level:'{{ apm_data.batteryLevel }}',
+                temperature:'{{ apm_data.batteryTeml }}',
+                net_send:'{{ apm_data.flow_send }}',
+                net_recv:'{{ apm_data.flow_recv }}'
+            },
+            beforeSend: function () {
+                SwalLoading('Save Html','Saving html.')
+            },
+            success: function (data) {
+                if(data['status']  == 1 ){
+                    SwalFire('success', 'Save successuly !', data['path'], 5000);
+                }else{
+                    SwalFire('error', 'Save failed !', data['msg'], 2000);
+                }
+            }
+        });
+    }
+
+    function saveiOSHtml(scene){
+        $.ajax({
+            url: "/apm/export/html/ios",
+            type: "GET",
+            async: true,
+            cache: false,
+            data:{
+                scene: scene,
+                cpu_app:'{{ apm_data.cpuAppRate }}',
+                cpu_sys:'{{ apm_data.cpuSystemRate }}',
+                gpu:'{{ apm_data.gpu }}',
+                mem_total:'{{ apm_data.totalPassAvg }}',
+                fps:'{{ apm_data.fps }}',
+                temperature:'{{ apm_data.batteryTeml }}',
+                current:'{{ apm_data.batteryCurrent }}',
+                voltage:'{{ apm_data.batteryVoltage }}',
+                power:'{{ apm_data.batteryPower }}',
+                net_send:'{{ apm_data.flow_send }}',
+                net_recv:'{{ apm_data.flow_recv }}'
+            },
+            beforeSend: function () {
+                SwalLoading('Save Html','Saving html.')
+            },
+            success: function (data) {
+                if(data['status']  == 1 ){
+                    SwalFire('success', 'Save successuly !', data['path'], 5000);
+                }else{
+                    SwalFire('error', 'Save failed !', data['msg'], 2000);
+                }
+            }
+        });
+    }
+
     function options(type,dataLabels=false) {
         let options = {
             chart: {
                 type: type,
                 fontFamily: 'inherit',
                 height: 240,
                 parentHeightOffset: 0,
@@ -482,15 +623,15 @@
                     enabled: false
                 },
             },
             dataLabels: {
                 enabled: dataLabels
             },
             fill: {
-                opacity: 1,
+                opacity: 1
             },
             stroke: {
                 width: 2,
                 lineCap: "round",
                 curve: "smooth",
             },
             series: [],
@@ -505,169 +646,242 @@
         return options
     }
 
     var cpu_chart = new ApexCharts(document.querySelector("#chart-cpu"), options('line'));
     cpu_chart.render();
     $('#cpu_loading').click(function () {
         $.ajax({
-            url: '/apm/log/pk',
+            url: '/apm/log',
             type: "GET",
             async: true,
             cache: false,
             data:{
                 scene:'{{ scene }}',
-                target1:'cpu_app1',
-                target2:'cpu_app2'
+                target:'cpu',
+                platform:platform
             },
             beforeSend: function () {
                 SwalLoading('Loading','')
             },
             complete: function () {
                 swal.close();
             },
             success: function (data) {
-                if(model == '2-devices'){
-                    cpu_chart.updateSeries([{
-                        name: 'Device1',
-                        data: data['first']
-                    },{
-                        name: 'Device2',
-                        data: data['second']
-                    }])
-                }else{
-                    cpu_chart.updateSeries([{
-                        name: 'APP1',
-                        data: data['first']
-                    },{
-                        name: 'APP2',
-                        data: data['second']
+                cpu_chart.updateSeries([{
+                    name: 'app',
+                    data: data['cpuAppData']
+                },{
+                    name: 'sys',
+                    data: data['cpuSysData']
+                }])
+            }
+        });
+    });
+    
+    var battery_chart = new ApexCharts(document.querySelector("#chart-battery"), options('line'));
+        battery_chart.render();
+        $('#battery_loading').click(function () {
+            $.ajax({
+                url: '/apm/log',
+                type: "GET",
+                async: true,
+                cache: false,
+                data:{
+                    scene:'{{ scene }}',
+                    target:'battery',
+                    platform:platform
+                },
+                beforeSend: function () {
+                    SwalLoading('Loading','')
+                },
+                complete: function () {
+                    swal.close();
+                },
+                success: function (data) {
+                    if(platform == 'Android'){
+                        battery_chart.updateSeries([{
+                            name: 'level',
+                            data: data['batteryLevel']
+                        },{
+                            name: 'temperature',
+                            data: data['batteryTem']
+                        }])
+                    }else {
+                        battery_chart.updateSeries([{
+                            name: 'temperature',
+                            data: data['batteryTem']
+                        },{
+                            name: 'Current',
+                            data: data['batteryCurrent']
+                        },{
+                            name: 'Voltage',
+                            data: data['batteryVoltage']
+                        },{
+                            name: 'Power',
+                            data: data['batteryPower']
+                        }])
+                    }
+                }
+            });
+        });
+
+    if(platform == 'Android'){
+        var jank_chart = new ApexCharts(document.querySelector("#chart-jank"), options('line'));
+        jank_chart.render();
+        $('#jank_loading').click(function () {
+            $.ajax({
+                url: '/apm/log',
+                type: "GET",
+                async: true,
+                cache: false,
+                data:{
+                    scene:'{{ scene }}',
+                    target:'fps',
+                    platform:platform
+                },
+                beforeSend: function () {
+                    SwalLoading('Loading','')
+                },
+                complete: function () {
+                    swal.close();
+                },
+                success: function (data) {
+                    jank_chart.updateSeries([{
+                        name: 'jank',
+                        data: data['jank']
                     }])
                 }
+            });
+        });
+    }
 
-            }
+    if(platform == 'iOS'){
+        var gpu_chart = new ApexCharts(document.querySelector("#chart-gpu"), options('line'));
+        gpu_chart.render();
+        $('#gpu_loading').click(function () {
+            $.ajax({
+                url: '/apm/log',
+                type: "GET",
+                async: true,
+                cache: false,
+                data:{
+                    scene:'{{ scene }}',
+                    target:'gpu',
+                    platform:platform
+                },
+                beforeSend: function () {
+                    SwalLoading('Loading','')
+                },
+                complete: function () {
+                    swal.close();
+                },
+                success: function (data) {
+                    gpu_chart.updateSeries([{
+                        name: 'gpu',
+                        data: data['gpu']
+                    }])
+                }
+            });
         });
-    });
+    }
 
     var fps_chart = new ApexCharts(document.querySelector("#chart-fps"), options('line'));
     fps_chart.render();
     $('#fps_loading').click(function () {
         $.ajax({
-            url: '/apm/log/pk',
+            url: '/apm/log',
             type: "GET",
             async: true,
             cache: false,
             data:{
                 scene:'{{ scene }}',
-                target1:'fps1',
-                target2:'fps2'
+                target:'fps',
+                platform:platform
             },
             beforeSend: function () {
                 SwalLoading('Loading','')
             },
             complete: function () {
                 swal.close();
             },
             success: function (data) {
-                if(model == '2-devices'){
-                    fps_chart.updateSeries([{
-                        name: 'Device1',
-                        data: data['first']
-                    },{
-                        name: 'Device2',
-                        data: data['second']
-                    }])
-                }else{
-                    fps_chart.updateSeries([{
-                        name: 'APP1',
-                        data: data['first']
-                    },{
-                        name: 'APP2',
-                        data: data['second']
-                    }])
-                }
+                fps_chart.updateSeries([{
+                    name: 'fps',
+                    data: data['fps']
+                }])
             }
         });
     });
 
     var mem_chart = new ApexCharts(document.querySelector("#chart-mem"), options('line'));
     mem_chart.render();
     $('#mem_loading').click(function () {
         $.ajax({
-            url: '/apm/log/pk',
+            url: '/apm/log',
             type: "GET",
             async: true,
             cache: false,
             data:{
                 scene:'{{ scene }}',
-                target1:'mem1',
-                target2:'mem2'
+                target:'mem',
+                platform:platform
             },
             beforeSend: function () {
                 SwalLoading('Loading','')
             },
             complete: function () {
                 swal.close();
             },
             success: function (data) {
-                if(model == '2-devices'){
+                if(platform == 'Android'){
                     mem_chart.updateSeries([{
-                        name: 'Device1',
-                        data: data['first']
+                        name: 'total',
+                        data: data['memTotalData']
                     },{
-                        name: 'Device2',
-                        data: data['second']
+                        name: 'native',
+                        data: data['memNativeData']
+                    },{
+                        name: 'dalvik',
+                        data: data['memDalvikData']
                     }])
                 }else{
                     mem_chart.updateSeries([{
-                        name: 'APP1',
-                        data: data['first']
-                    },{
-                        name: 'APP2',
-                        data: data['second']
+                        name: 'total',
+                        data: data['memTotalData']
                     }])
                 }
             }
         });
     });
 
     var network_chart = new ApexCharts(document.querySelector("#chart-networkdata"), options('line',false));
     network_chart.render();
     $('#networkdata_loading').click(function () {
         $.ajax({
-            url: '/apm/log/pk',
+            url: '/apm/log',
             type: "GET",
             async: true,
             cache: false,
             data:{
                 scene:'{{ scene }}',
-                target1:'network1',
-                target2:'network2'
+                target:'flow',
+                platform:platform
             },
             beforeSend: function () {
                 SwalLoading('Loading','')
             },
             complete: function () {
                 swal.close();
             },
             success: function (data) {
-                if(model == '2-devices'){
-                    network_chart.updateSeries([{
-                        name: 'Device1',
-                        data: data['first']
-                    },{
-                        name: 'Device2',
-                        data: data['second']
-                    }])
-                }else{
-                    network_chart.updateSeries([{
-                        name: 'APP1',
-                        data: data['first']
-                    },{
-                        name: 'APP2',
-                        data: data['second']
-                    }])
-                }
+                network_chart.updateSeries([{
+                    name: 'send',
+                    data: data['upFlow']
+                },{
+                    name: 'recv',
+                    data: data['downFlow']
+                }])
             }
         });
     });
 </script>
 {% endblock %}
```

### Comparing `solox-2.5.9/solox/templates/base.html` & `solox-2.6.0/solox/templates/base.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/templates/index.html` & `solox-2.6.0/solox/templates/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
                 
             },
             success: function (data) {
                 if(data['status'] != 1 ) {
                     if(lan == 'cn' ){
                         SwalFire('error', '连接失败','请检查当前移动设备的是否连接了PC端', 2000);
                     }else{
-                        SwalFire('error', 'Connet failed !', 'No devices found', 2000);
+                        SwalFire('error', 'Connection failed !', 'No devices found', 2000);
                     } 
                 }else{
                     for(var i=0;i<data['pkgnames'].length;i++){
                         $('.select-app').append('<option>'+data['pkgnames'][i]+'</option>')
                     }
                     swal.close();
                 }
@@ -332,30 +332,31 @@
             data:{
                 platform:platform,
                 device:$('.select-device').val(),
                 pkgname:this.value
             },
             beforeSend: function () {
                 $('.select-pid').empty();
-                $('.select-pid').append('<option></option>');
+                // $('.select-pid').append('<option></option>');
                 if(lan == 'cn' ){
                     SwalLoading('初始化','正在获取该APP上的所有进程, 请您稍等！');
                 }else{
                     SwalLoading('Process initialization!','Initializing Process, please wait a mmoment.');
                 }
                 
             },
             success: function (data) {
                 if(data['status'] != 1 ) {
                     if(lan == 'cn' ){
                         SwalFire('error', '连接失败','请检查当前移动设备的是否连接了PC端', 2000);
                     }else{
-                        SwalFire('error', 'Connet failed !', 'No pid found', 2000);
+                        SwalFire('error', 'Connection failed !', 'No pid found', 2000);
                     } 
                 }else{
+                    // $('.select-pid').val(data['pids'][0]);
                     for(var i=0;i<data['pids'].length;i++){
                         $('.select-pid').append('<option>'+data['pids'][i]+'</option>')
                     }
                     swal.close();
                 }
             }
         });
```

### Comparing `solox-2.5.9/solox/templates/pk.html` & `solox-2.6.0/solox/templates/pk.html`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox/templates/report.html` & `solox-2.6.0/solox/templates/report.html`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,15 @@
             beforeSend: function () {
                 SwalLoading('Exporting',scene)
             },
             success: function (data) {
                 if(data['status'] != 1 ){
                     SwalFire('error', 'Export failed !', data['msg'], 2000);
                 }else{
-                    SwalFire('success', scene+'.xls in current directory', '', 5000);
+                    SwalFire('success', 'Export success', data['path'], 5000);
                 }
             }
         });
     }
 
     function removeCheckedData(){
         $('#cancel_remove_selected_confirm').click();
```

### Comparing `solox-2.5.9/solox/view/apis.py` & `solox-2.6.0/solox/view/apis.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import time
 from flask import request, make_response
 from logzero import logger
 from flask import Blueprint
 import traceback
 from solox.public.apm import CPU, MEM, Flow, FPS, Battery, GPU, Target
 from solox.public.apm_pk import CPU_PK, MEM_PK, Flow_PK, FPS_PK
-from solox.public.common import Devices, file, Method, Install, Platform
+from solox.public.common import Devices, File, Method, Install, Platform
 
 d = Devices()
-f = file()
+f = File()
 api = Blueprint("api", __name__)
 method = Method()
 
 @api.route('/apm/cookie', methods=['post', 'get'])
 def setCookie():
     """set apm data to cookie"""
     cpuWarning = request.args.get('cpuWarning')
@@ -360,15 +360,15 @@
             wifi = False if wifi_switch == 'false' else True
             deviceId = d.getIdbyDevice(devices, platform)
             pid = process.split(':')[0] if platform == Platform.Android else None
             flow = Flow(pkgName=app, deviceId=deviceId, platform=platform, pid=pid)
             data = flow.setAndroidNet(wifi=wifi)
             f.record_net('end', data[0], data[1])
             app = process
-        file(fileroot=f'apm_{current_time}').make_report(app=app, devices=devices, platform=platform, model=model)
+        File(fileroot=f'apm_{current_time}').make_report(app=app, devices=devices, platform=platform, model=model)
         result = {'status': 1}
     except Exception as e:
         traceback.print_exc()
         result = {'status': 0, 'msg': str(e)}
     return result
 
 
@@ -392,16 +392,96 @@
     return result
 
 @api.route('/apm/export/report', methods=['post', 'get'])
 def exportReport():
     platform = method._request(request, 'platform')
     scene = method._request(request, 'scene')
     try:
-        file().export_excel(platform=platform, scene=scene)
-        result = {'status': 1, 'msg':'success'}
+        path = f.export_excel(platform=platform, scene=scene)
+        result = {'status': 1, 'msg':'success', 'path': path}
+    except Exception as e:
+        traceback.print_exc()
+        result = {'status': 0, 'msg':str(e)}    
+    return result
+
+@api.route('/apm/export/html/android', methods=['post', 'get'])
+def exportAndroidHtml():
+    scene = method._request(request, 'scene')
+    cpu_app = method._request(request, 'cpu_app')
+    cpu_sys = method._request(request, 'cpu_sys')
+    mem_total = method._request(request, 'mem_total')
+    mem_native = method._request(request, 'mem_native')
+    mem_dalvik = method._request(request, 'mem_dalvik')
+    fps = method._request(request, 'fps')
+    jank = method._request(request, 'jank')
+    level = method._request(request, 'level')
+    temperature = method._request(request, 'temperature')
+    net_send = method._request(request, 'net_send')
+    net_recv = method._request(request, 'net_recv')
+    try:
+        summary_dict = {}
+        summary_dict['cpu_app'] = cpu_app
+        summary_dict['cpu_sys'] = cpu_sys
+        summary_dict['mem_total'] = mem_total
+        summary_dict['mem_native'] = mem_native
+        summary_dict['mem_dalvik'] = mem_dalvik
+        summary_dict['fps'] = fps
+        summary_dict['jank'] = jank
+        summary_dict['level'] = level
+        summary_dict['tem'] = temperature
+        summary_dict['net_send'] = net_send
+        summary_dict['net_recv'] = net_recv
+        summary_dict['cpu_charts'] = f.getCpuLog(Platform.Android, scene)
+        summary_dict['mem_charts'] = f.getMemLog(Platform.Android, scene)
+        summary_dict['net_charts'] = f.getFlowLog(Platform.Android, scene)
+        summary_dict['battery_charts'] = f.getBatteryLog(Platform.Android, scene)
+        summary_dict['fps_charts'] = f.getFpsLog(Platform.Android, scene)['fps']
+        summary_dict['jank_charts'] = f.getFpsLog(Platform.Android, scene)['jank']
+        path = f.make_android_html(scene, summary_dict)
+        result = {'status': 1, 'msg':'success', 'path':path}
+    except Exception as e:
+        traceback.print_exc()
+        result = {'status': 0, 'msg':str(e)}    
+    return result
+
+@api.route('/apm/export/html/ios', methods=['post', 'get'])
+def exportiOSHtml():
+    scene = method._request(request, 'scene')
+    cpu_app = method._request(request, 'cpu_app')
+    cpu_sys = method._request(request, 'cpu_sys')
+    mem_total = method._request(request, 'mem_total')
+    gpu = method._request(request, 'gpu')
+    fps = method._request(request, 'fps')
+    temperature = method._request(request, 'temperature')
+    current = method._request(request, 'current')
+    voltage = method._request(request, 'voltage')
+    power = method._request(request, 'power')
+    net_send = method._request(request, 'net_send')
+    net_recv = method._request(request, 'net_recv')
+    try:
+        summary_dict = {}
+        summary_dict['cpu_app'] = cpu_app
+        summary_dict['cpu_sys'] = cpu_sys
+        summary_dict['mem_total'] = mem_total
+        summary_dict['gpu'] = gpu
+        summary_dict['fps'] = fps
+        summary_dict['tem'] = temperature
+        summary_dict['current'] = current
+        summary_dict['voltage'] = voltage
+        summary_dict['power'] = power
+        summary_dict['net_send'] = net_send
+        summary_dict['net_recv'] = net_recv
+        summary_dict['cpu_charts'] = f.getCpuLog(Platform.iOS, scene)
+        summary_dict['mem_charts'] = f.getMemLog(Platform.iOS, scene)
+        summary_dict['net_charts'] = f.getFlowLog(Platform.iOS, scene)
+        summary_dict['battery_charts'] = f.getBatteryLog(Platform.iOS, scene)
+        summary_dict['fps_charts'] = f.getFpsLog(Platform.iOS, scene)
+        summary_dict['gpu_charts'] = f.getGpuLog(Platform.iOS, scene)
+        path = f.make_ios_html(scene, summary_dict)
+        result = {'status': 1, 'msg':'success', 'path':path}
     except Exception as e:
         traceback.print_exc()
         result = {'status': 0, 'msg':str(e)}    
     return result    
 
 @api.route('/apm/log', methods=['post', 'get'])
 def getLogData():
@@ -426,16 +506,16 @@
 @api.route('/apm/log/pk', methods=['post', 'get'])
 def getpkLogData():
     """Get apm detailed data"""
     scene = method._request(request, 'scene')
     target1 = method._request(request, 'target1')
     target2 = method._request(request, 'target2')
     try:
-        first = file().readLog(scene=scene, filename=f'{target1}.log')[0]
-        second = file().readLog(scene=scene, filename=f'{target2}.log')[0]
+        first = f.readLog(scene=scene, filename=f'{target1}.log')[0]
+        second = f.readLog(scene=scene, filename=f'{target2}.log')[0]
         result = {'status': 1, 'first': first, 'second': second}
     except Exception as e:
         result = {'status': 0, 'msg': str(e)}
     return result
 
 
 @api.route('/apm/remove/report', methods=['post', 'get'])
```

### Comparing `solox-2.5.9/solox/web.py` & `solox-2.6.0/solox/web.py`

 * *Files identical despite different names*

### Comparing `solox-2.5.9/solox.egg-info/PKG-INFO` & `solox-2.6.0/solox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.5.9
+Version: 2.6.0
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -27,25 +27,25 @@
 </p>
 <p align="center">
 <a href="https://pypi.org/project/solox/" target="__blank"><img src="https://img.shields.io/pypi/v/solox" alt="solox preview"></a>
 <a href="https://pypistats.org/packages/solox" target="__blank"><img src="https://img.shields.io/pypi/dm/solox"></a>
 <br>
 </p>
 
-## 🔎Preview
+## 🔎Preview	
 
 SoloX - Real-time collection tool for Android/iOS performance data.
 
 We are committed to solving inefficient, cumbersome test execution, and our goal is Simple Test In SoloX!
 
 <img src="https://cdn.nlark.com/yuque/0/2022/png/153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-process=image%2Fresize%2Cw_1500%2Climit_0"  width="100%" >
 
 ## 📦Requirements
 
-- Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
+Install Python 3.10 + [**Download**](https://www.python.org/downloads/)
 
 💡 Python 3.6 ~ 3.9 , please download a version of solox lower than 2.5.4.
 
 💡 If Windows users need to test ios, install and start Itunes.
 
 ## 📥Installation
 
@@ -76,23 +76,25 @@
 ```shell
 python -m solox --host={ip} --port={port}
 ```
 
 ## 🏴󠁣󠁩󠁣󠁭󠁿Collect in python
 
 ```python
+
 from solox.public.apm import APM
 from solox.public.common import Devices
 
 # solox version >= 2.1.2
 
 d = Devices()
 pids = d.getPid(deviceId='ca6bd5a5', pkgName='com.bilibili.app.in')
 
-apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', surfaceview=True, noLog=True, pid=None)
+apm = APM(pkgName='com.bilibili.app.in',deviceId='ca6bd5a5',platform='Android', 
+          surfaceview=True, noLog=True, pid=None)
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS') only supports one device
 # surfaceview： False = gfxinfo (Developer - GPU rendering mode - adb shell dumpsys gfxinfo)
 # noLog : False (Save test data to log file)
 
 cpu = apm.collectCpu() # %
 memory = apm.collectMemory() # MB
 flow = apm.collectFlow(wifi=True) # KB
@@ -121,19 +123,19 @@
 target in ['cpu','memory','network','fps','battery','gpu']
 ```
 
 ## 🔥Features
 
 * **No ROOT/Jailbreak:** No need of Root for Android devices, Jailbreak for iOS devices. Efficiently solving the test and analysis challenges in Android & iOS performance.
 * **Data Integrality:** We provide the data about Screenshot, CPU, GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get.
-* **Beautiful report board:** A beautiful and detailed report analysis, where to store, visualize, edit, manage, and download all the test cases collected with SoloX no matter where you are or when is it.
-* **Useful monitoring settings:** Support setting alarm values, collecting duration, and accessing mobile devices on other PC machines during the monitoring process.
-* **PK model:** Supports simultaneous comparative testing of two mobile devices.
-  🌱2-devices: test the same app on two different phones.
-  🌱2-apps: test two different apps on two phones with the same configuration.
+* **Beautiful Report:** A beautiful and detailed report analysis, where to store, visualize, edit, manage, and download all the test cases collected with SoloX no matter where you are or when is it.
+* **Useful Monitoring Settings:** Support setting alarm values, collecting duration, and accessing mobile devices on other PC machines during the monitoring process.
+* **PK Model:** Supports simultaneous comparative testing of two mobile devices.
+  - 🌱2-devices: test the same app on two different phones.
+  - 🌱2-apps: test two different apps on two phones with the same configuration.
 
 ## Browser
 
 <img src="https://cdn.nlark.com/yuque/0/2023/png/153412/1677553244198-96ce5709-f33f-4038-888f-f330d1f74450.png" alt="Chrome" width="50px" height="50px" />
 
 ## Terminal
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: solox Version: 2.5.9 Summary: SoloX - Real-time
+Metadata-Version: 2.1 Name: solox Version: 2.6.0 Summary: SoloX - Real-time
 collection tool for Android/iOS performance data. Home-page: https://
 github.com/smart-test-ti/SoloX Author: Rafa Chen Author-email:
 rafacheninc@gamil.com License: MIT Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE
                                English | ä¸­æ
                                    [SoloX]
 
             [solox_preview] [https://img.shields.io/pypi/dm/solox]
 ## ðPreview SoloX - Real-time collection tool for Android/iOS performance
 data. We are committed to solving inefficient, cumbersome test execution, and
 our goal is Simple Test In SoloX! [https://cdn.nlark.com/yuque/0/2022/png/
 153412/1662348054846-b0164165-e83a-443e-9a05-8c1f9ddb355f.png?x-oss-
-process=image%2Fresize%2Cw_1500%2Climit_0] ## ð¦Requirements - Install Python
+process=image%2Fresize%2Cw_1500%2Climit_0] ## ð¦Requirements Install Python
 3.10 + [**Download**](https://www.python.org/downloads/) ð¡ Python 3.6 ~ 3.9
 , please download a version of solox lower than 2.5.4. ð¡ If Windows users
 need to test ios, install and start Itunes. ## ð¥Installation ### default
 ```shell pip install -U solox ``` ### mirrors ```shell pip install -i https://
 mirrors.ustc.edu.cn/pypi/web/simple -U solox ``` ð¡ If your network is unable
 to download through [pip install -U solox], please try using mirrors to
 download, but the download of SoloX may not be the latest version. ##
@@ -42,17 +42,17 @@
 iOS: http://{ip}:{port}/apm/
 collect?platform=iOS&pkgname=com.bilibili.app.in&target=cpu target in
 ['cpu','memory','network','fps','battery','gpu'] ``` ## ð¥Features * **No
 ROOT/Jailbreak:** No need of Root for Android devices, Jailbreak for iOS
 devices. Efficiently solving the test and analysis challenges in Android & iOS
 performance. * **Data Integrality:** We provide the data about Screenshot, CPU,
 GPU, Memory, Battery, Network,FPS, Jank, etc., which you may easy to get. *
-**Beautiful report board:** A beautiful and detailed report analysis, where to
-store, visualize, edit, manage, and download all the test cases collected with
-SoloX no matter where you are or when is it. * **Useful monitoring settings:**
+**Beautiful Report:** A beautiful and detailed report analysis, where to store,
+visualize, edit, manage, and download all the test cases collected with SoloX
+no matter where you are or when is it. * **Useful Monitoring Settings:**
 Support setting alarm values, collecting duration, and accessing mobile devices
-on other PC machines during the monitoring process. * **PK model:** Supports
-simultaneous comparative testing of two mobile devices. ð±2-devices: test the
-same app on two different phones. ð±2-apps: test two different apps on two
-phones with the same configuration. ## Browser [Chrome] ## Terminal - windows:
-PowerShell - macOSï¼iTerm2 (https://iterm2.com/) ## ðThanks - https://
-github.com/alibaba/taobao-iphone-device
+on other PC machines during the monitoring process. * **PK Model:** Supports
+simultaneous comparative testing of two mobile devices. - ð±2-devices: test
+the same app on two different phones. - ð±2-apps: test two different apps on
+two phones with the same configuration. ## Browser [Chrome] ## Terminal -
+windows: PowerShell - macOSï¼iTerm2 (https://iterm2.com/) ## ðThanks -
+https://github.com/alibaba/taobao-iphone-device
```

### Comparing `solox-2.5.9/solox.egg-info/SOURCES.txt` & `solox-2.6.0/solox.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 solox/public/iosperf/_version.py
 solox/public/iosperf/_wdaproxy.py
 solox/public/iosperf/bplist.py
 solox/public/iosperf/exceptions.py
 solox/public/iosperf/plistlib2.py
 solox/public/iosperf/requests_usbmux.py
 solox/public/iosperf/struct2.py
+solox/public/report_template/android.html
+solox/public/report_template/ios.html
 solox/static/css/highlight.min.css
 solox/static/css/select2-bootstrap-5-theme.min.css
 solox/static/css/select2-bootstrap-5-theme.rtl.min.css
 solox/static/css/select2.min.css
 solox/static/css/sweetalert2.min.css
 solox/static/css/tabler.demo.min.css
 solox/static/css/tabler.min.css
```

