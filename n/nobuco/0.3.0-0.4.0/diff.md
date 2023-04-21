# Comparing `tmp/nobuco-0.3.0.tar.gz` & `tmp/nobuco-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.3.0.tar", last modified: Thu Apr 20 12:10:50 2023, max compression
+gzip compressed data, was "nobuco-0.4.0.tar", last modified: Fri Apr 21 21:39:49 2023, max compression
```

## Comparing `nobuco-0.3.0.tar` & `nobuco-0.4.0.tar`

### file list

```diff
@@ -1,94 +1,67 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.847216 nobuco-0.3.0/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.3.0/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)       14 2023-04-15 10:44:29.000000 nobuco-0.3.0/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)    21658 2023-04-20 12:10:50.847216 nobuco-0.3.0/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    19824 2023-04-20 12:08:50.000000 nobuco-0.3.0/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.843216 nobuco-0.3.0/docs/
--rw-rw-r--   0 alex      (1000) alex      (1000)    64876 2023-03-25 20:16:55.000000 nobuco-0.3.0/docs/channel_ordering.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    63145 2023-03-25 20:46:53.000000 nobuco-0.3.0/docs/channel_ordering_forced.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    67966 2023-04-18 11:28:12.000000 nobuco-0.3.0/docs/control_if.png
--rw-rw-r--   0 alex      (1000) alex      (1000)     2110 2023-04-05 14:55:45.000000 nobuco-0.3.0/docs/converter_inside_converter1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    26497 2023-04-05 19:25:33.000000 nobuco-0.3.0/docs/converter_inside_converter1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2319 2023-04-05 14:56:10.000000 nobuco-0.3.0/docs/converter_inside_converter2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    30325 2023-04-05 19:25:54.000000 nobuco-0.3.0/docs/converter_inside_converter2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1061 2023-04-20 11:04:43.000000 nobuco-0.3.0/docs/dynamic_shape1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    29177 2023-04-20 10:58:19.000000 nobuco-0.3.0/docs/dynamic_shape1.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    13716 2023-04-20 10:56:49.000000 nobuco-0.3.0/docs/dynamic_shape1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2299 2023-04-20 11:06:54.000000 nobuco-0.3.0/docs/dynamic_shape2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    65071 2023-04-20 11:08:28.000000 nobuco-0.3.0/docs/dynamic_shape2.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    31893 2023-04-20 11:07:03.000000 nobuco-0.3.0/docs/dynamic_shape2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     3070 2023-04-06 09:06:34.000000 nobuco-0.3.0/docs/essentials1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    35615 2023-04-06 09:06:58.000000 nobuco-0.3.0/docs/essentials1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2811 2023-04-05 14:47:00.000000 nobuco-0.3.0/docs/essentials2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    32971 2023-04-05 19:22:33.000000 nobuco-0.3.0/docs/essentials2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2281 2023-04-05 14:48:33.000000 nobuco-0.3.0/docs/essentials3.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    28090 2023-04-05 19:22:46.000000 nobuco-0.3.0/docs/essentials3.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1559 2023-04-05 14:51:28.000000 nobuco-0.3.0/docs/inplace1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    18606 2023-04-05 19:23:57.000000 nobuco-0.3.0/docs/inplace1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1050 2023-04-05 14:52:17.000000 nobuco-0.3.0/docs/inplace2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    11981 2023-04-05 19:24:22.000000 nobuco-0.3.0/docs/inplace2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-04-05 14:52:18.000000 nobuco-0.3.0/docs/inplace3.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    14409 2023-04-05 19:25:18.000000 nobuco-0.3.0/docs/inplace3.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     6859 2023-03-24 11:40:17.000000 nobuco-0.3.0/docs/inplace_empty.png
--rw-rw-r--   0 alex      (1000) alex      (1000)   863504 2023-04-19 06:48:26.000000 nobuco-0.3.0/docs/nobuco.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    82036 2023-03-03 12:08:40.000000 nobuco-0.3.0/docs/tutorial.png
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.843216 nobuco-0.3.0/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      526 2023-04-20 09:21:24.000000 nobuco-0.3.0/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      818 2023-04-19 23:06:10.000000 nobuco-0.3.0/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13153 2023-04-19 22:56:45.000000 nobuco-0.3.0/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.843216 nobuco-0.3.0/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.3.0/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-18 11:13:00.000000 nobuco-0.3.0/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-19 23:06:10.000000 nobuco-0.3.0/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-18 18:43:24.000000 nobuco-0.3.0/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.3.0/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3497 2023-03-07 10:32:51.000000 nobuco-0.3.0/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.843216 nobuco-0.3.0/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.3.0/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-20 11:44:40.000000 nobuco-0.3.0/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13309 2023-04-18 18:06:08.000000 nobuco-0.3.0/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-20 10:41:07.000000 nobuco-0.3.0/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.843216 nobuco-0.3.0/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.3.0/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.3.0/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4886 2023-04-18 10:06:25.000000 nobuco-0.3.0/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.3.0/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-18 10:06:25.000000 nobuco-0.3.0/nobuco/layers/weight.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1202 2023-04-20 09:37:25.000000 nobuco-0.3.0/nobuco/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.847216 nobuco-0.3.0/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-18 09:00:20.000000 nobuco-0.3.0/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4398 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4675 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9840 2023-04-18 17:59:47.000000 nobuco-0.3.0/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6816 2023-04-19 23:20:41.000000 nobuco-0.3.0/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3071 2023-04-19 08:28:44.000000 nobuco-0.3.0/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2568 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10232 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/tensor_manipulation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.847216 nobuco-0.3.0/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.3.0/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.3.0/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9670 2023-04-18 11:49:04.000000 nobuco-0.3.0/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-18 18:22:15.000000 nobuco-0.3.0/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.847216 nobuco-0.3.0/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.3.0/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1943 2023-04-18 10:12:57.000000 nobuco-0.3.0/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3167 2023-04-18 10:12:58.000000 nobuco-0.3.0/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.843216 nobuco-0.3.0/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    21658 2023-04-20 12:10:50.000000 nobuco-0.3.0/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     2218 2023-04-20 12:10:50.000000 nobuco-0.3.0/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-20 12:10:50.000000 nobuco-0.3.0/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-20 12:10:50.000000 nobuco-0.3.0/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-20 12:10:50.000000 nobuco-0.3.0/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-20 11:19:12.000000 nobuco-0.3.0/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-20 12:10:50.847216 nobuco-0.3.0/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.926740 nobuco-0.4.0/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.4.0/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21659 2023-04-21 21:39:49.926740 nobuco-0.4.0/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    19825 2023-04-21 21:38:56.000000 nobuco-0.4.0/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.918740 nobuco-0.4.0/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-21 10:22:54.000000 nobuco-0.4.0/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-21 21:36:43.000000 nobuco-0.4.0/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13497 2023-04-21 21:36:43.000000 nobuco-0.4.0/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.922740 nobuco-0.4.0/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.4.0/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-18 11:13:00.000000 nobuco-0.4.0/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-19 23:06:10.000000 nobuco-0.4.0/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-18 18:43:24.000000 nobuco-0.4.0/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.4.0/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3874 2023-04-21 21:15:19.000000 nobuco-0.4.0/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.922740 nobuco-0.4.0/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.4.0/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-20 11:44:40.000000 nobuco-0.4.0/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14889 2023-04-21 21:37:11.000000 nobuco-0.4.0/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-20 10:41:07.000000 nobuco-0.4.0/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.922740 nobuco-0.4.0/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.4.0/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.4.0/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-21 13:07:22.000000 nobuco-0.4.0/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.4.0/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-18 10:06:25.000000 nobuco-0.4.0/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.922740 nobuco-0.4.0/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-21 10:21:12.000000 nobuco-0.4.0/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-21 13:21:40.000000 nobuco-0.4.0/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-21 10:22:11.000000 nobuco-0.4.0/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.926740 nobuco-0.4.0/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-18 09:00:20.000000 nobuco-0.4.0/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4398 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4675 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9840 2023-04-21 11:09:43.000000 nobuco-0.4.0/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6824 2023-04-21 11:14:16.000000 nobuco-0.4.0/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3071 2023-04-19 08:28:44.000000 nobuco-0.4.0/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2568 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10232 2023-04-18 11:44:33.000000 nobuco-0.4.0/nobuco/node_converters/tensor_manipulation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.926740 nobuco-0.4.0/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.4.0/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.4.0/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9421 2023-04-21 09:46:48.000000 nobuco-0.4.0/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-18 18:22:15.000000 nobuco-0.4.0/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.926740 nobuco-0.4.0/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.4.0/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-21 13:07:22.000000 nobuco-0.4.0/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-21 13:07:21.000000 nobuco-0.4.0/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-21 21:39:49.918740 nobuco-0.4.0/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21659 2023-04-21 21:39:49.000000 nobuco-0.4.0/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1589 2023-04-21 21:39:49.000000 nobuco-0.4.0/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-21 21:39:49.000000 nobuco-0.4.0/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-21 21:39:49.000000 nobuco-0.4.0/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-21 21:39:49.000000 nobuco-0.4.0/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-21 11:10:10.000000 nobuco-0.4.0/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-21 21:39:49.926740 nobuco-0.4.0/setup.cfg
```

### Comparing `nobuco-0.3.0/LICENSE` & `nobuco-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/PKG-INFO` & `nobuco-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.3.0
+Version: 0.4.0
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -324,15 +324,15 @@
         return x
 ```
 
 Of course, it's possible to translate the dynamic module into a tensorflow layer
 (don't forget to decorate it with `@tf.function` for autograph to kick in).
 But what if it contains inner modules, do you replicate them in tensorflow all by hand?
 Not unless you want to! 
-Just convert them separately and use the resulting graph inside the parent layer.
+Just convert them separately and use the resulting graphs inside the parent layer.
 
 ```python
 class ControlIfKeras(tf.keras.layers.Layer):
     def __init__(self, conv_pre, conv_true, conv_false, conv_shared, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.conv_pre = conv_pre
         self.conv_true = conv_true
@@ -383,15 +383,15 @@
 <img src="docs/control_if.png" width="25%">
 </p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
 ### Dynamic shapes
 
-What if we wanted out module to accept images of arbitrary height and width?
+What if we wanted our module to accept images of arbitrary height and width?
 Can we have that? Let's try:
 
 ```python
 class DynamicShape(nn.Module):
     def __init__(self):
         super().__init__()
         self.conv = nn.Conv2d(3, 16, kernel_size=(1, 1))
```

### Comparing `nobuco-0.3.0/README.md` & `nobuco-0.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
         return x
 ```
 
 Of course, it's possible to translate the dynamic module into a tensorflow layer
 (don't forget to decorate it with `@tf.function` for autograph to kick in).
 But what if it contains inner modules, do you replicate them in tensorflow all by hand?
 Not unless you want to! 
-Just convert them separately and use the resulting graph inside the parent layer.
+Just convert them separately and use the resulting graphs inside the parent layer.
 
 ```python
 class ControlIfKeras(tf.keras.layers.Layer):
     def __init__(self, conv_pre, conv_true, conv_false, conv_shared, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.conv_pre = conv_pre
         self.conv_true = conv_true
@@ -347,15 +347,15 @@
 <img src="docs/control_if.png" width="25%">
 </p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
 ### Dynamic shapes
 
-What if we wanted out module to accept images of arbitrary height and width?
+What if we wanted our module to accept images of arbitrary height and width?
 Can we have that? Let's try:
 
 ```python
 class DynamicShape(nn.Module):
     def __init__(self):
         super().__init__()
         self.conv = nn.Conv2d(3, 16, kernel_size=(1, 1))
```

### Comparing `nobuco-0.3.0/nobuco/__init__.py` & `nobuco-0.4.0/nobuco/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from nobuco.funcs import force_tensorflow_order, force_pytorch_order, shape
-from nobuco.locate import locate_converter
+from nobuco.locate.locate import locate_converter
 from nobuco.trace.trace import traceable
 
 from nobuco.converters.node_converter import converter
 from nobuco.convert import pytorch_to_keras
 from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
```

### Comparing `nobuco-0.3.0/nobuco/convert.py` & `nobuco-0.4.0/nobuco/convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import torch
 from nobuco.converters.tensor import permute_pytorch2keras
 from torch import nn
 import tensorflow as tf
 from tensorflow import keras
 
-from nobuco.commons import ChannelOrder, ChannelOrderingStrategy, TF_TENSOR_CLASSES
+from nobuco.commons import ChannelOrder, ChannelOrderingStrategy, TF_TENSOR_CLASSES, TraceLevel
 from nobuco.converters.channel_ordering import t_pytorch2keras, set_channel_order, t_keras2pytorch
 from nobuco.converters.validation import validate, ValidationResult, ConversionResult
 from nobuco.layers.channel_order import ChangeOrderingLayer
 from nobuco.layers.container import TransientContainer
 from nobuco.layers.stub import UnimplementedOpStub
 from nobuco.util import get_torch_tensor_identifier, collect_recursively, replace_recursively_func, \
     clone_torch_tensors_recursively
@@ -30,14 +30,18 @@
 Tracer.decorate_all()
 
 
 def has_converter(node: PytorchNode, converter_dict: Dict[object, Pytorch2KerasNodeConverter]) -> bool:
     return node.get_type() in converter_dict.keys()
 
 
+def find_converter(node: PytorchNode, converter_dict: Dict[object, Pytorch2KerasNodeConverter]) -> Optional[Pytorch2KerasNodeConverter]:
+    return converter_dict.get(node.get_type(), None)
+
+
 def find_unimplemented(hierarchy: PytorchNodeHierarchy, converter_dict: Dict[object, Pytorch2KerasNodeConverter]) -> Optional[PytorchNodeHierarchy]:
     # Test if the node itself has a converter
     if has_converter(hierarchy.node, converter_dict):
         return None
     elif len(hierarchy.children) == 0:
         return PytorchNodeHierarchy(hierarchy.node, hierarchy.children)
     else:
@@ -110,45 +114,48 @@
 
 def convert_hierarchy(
         node_hierarchy: PytorchNodeHierarchy,
         converter_dict: Dict[object, Pytorch2KerasNodeConverter],
         reuse_layers: bool = True,
         full_validation: bool = True,
         tolerance=1e-4,
-        constants_to_variables: bool = True) -> KerasConvertedNode:
+        constants_to_variables: bool = True,
+) -> KerasConvertedNode:
 
     def convert(hierarchy: PytorchNodeHierarchy, converted_op_dict:Dict, reuse_layers: bool, full_validation: bool, depth):
         node = hierarchy.node
         children = hierarchy.children
 
         input_names = node.input_names
         output_names = node.output_names
 
+        converter = find_converter(node, converter_dict)
+
         keras_op, children_converted_nodes = converted_op_dict.get(node.get_op(), (None, []))
         node_is_reusable = False
         if reuse_layers and keras_op is not None:
-            conversion_result = ConversionResult(converted_manually=False, is_duplicate=True)
+            conversion_result = ConversionResult(converted_manually=False, is_duplicate=True, converter=converter)
         elif has_converter(node, converter_dict):
             children_converted_nodes = []
             node_converter: Pytorch2KerasNodeConverter = converter_dict.get(node.get_type(), None)
             node_is_reusable = node_converter.reusable
             keras_op = convert_node(node, node_converter)
-            conversion_result = ConversionResult(converted_manually=True)
+            conversion_result = ConversionResult(converted_manually=True, converter=converter)
         elif len(children) > 0:
             children_converted_nodes = [convert(child, converted_op_dict, reuse_layers, full_validation, depth + 1) for child in children]
             keras_op = convert_container(node, children, children_converted_nodes, input_names, output_names, node.output_tensors, constants_to_variables=constants_to_variables)
 
             connectivity_status = keras_op.get_connectivity_status()
             if not connectivity_status.is_connected():
                 warnings.warn(f'[{node.get_type()} : {keras_op}] is disconnected!', category=RuntimeWarning)
-            conversion_result = ConversionResult(converted_manually=False, connectivity_status=connectivity_status)
+            conversion_result = ConversionResult(converted_manually=False, connectivity_status=connectivity_status, converter=converter)
         else:
             children_converted_nodes = []
             keras_op = UnimplementedOpStub(node.get_op())
-            conversion_result = ConversionResult(converted_manually=False, is_implemented=False)
+            conversion_result = ConversionResult(converted_manually=False, is_implemented=False, converter=converter)
 
         if full_validation or depth == 0:
             diff, status = validate(node, node.wrapped_op.op, keras_op, node.input_args, node.input_kwargs, node.output_tensors, node.get_type(), tolerance=tolerance)
             validation_result = ValidationResult(diff, status)
         else:
             validation_result = None
 
@@ -235,38 +242,45 @@
         inputs_channel_order: Union[ChannelOrder, Dict[torch.Tensor, ChannelOrder]] = ChannelOrder.TENSORFLOW,
         outputs_channel_order: Union[ChannelOrder, Dict[int, ChannelOrder]] = None,
         converter_dict=CONVERTER_DICT,
         constants_to_variables: bool = True,
         full_validation: bool = True,
         validation_tolerance=1e-4,
         save_trace_html=False,
-        return_outputs_pt=False
+        return_outputs_pt=False,
+        debug_traces: TraceLevel = TraceLevel.DEFAULT,
 ) -> Union[keras.Model, Tuple[keras.Model, object]]:
     start = time.time()
     node_hierarchy = Tracer.trace(module, args, kwargs)
 
     keras_converted_node = convert_hierarchy(node_hierarchy, converter_dict,
                                              reuse_layers=True, full_validation=full_validation, constants_to_variables=constants_to_variables,
                                              tolerance=validation_tolerance,
                                              )
 
     validation_result_dict = collect_validation_results(keras_converted_node)
     conversion_result_dict = collect_conversion_results(keras_converted_node)
 
-    print(node_hierarchy.__str__(validation_result_dict=validation_result_dict, conversion_result_dict=conversion_result_dict, with_legend=True))
+    vis_params = {
+        'validation_result_dict': validation_result_dict,
+        'conversion_result_dict': conversion_result_dict,
+        'debug_traces': debug_traces,
+    }
+
+    print(node_hierarchy.__str__(with_legend=True, **vis_params))
 
     if save_trace_html:
-        html = node_hierarchy.__str__(validation_result_dict=validation_result_dict, conversion_result_dict=conversion_result_dict, with_legend=True, stylizer=HtmlStylizer())
+        html = node_hierarchy.__str__(with_legend=True, stylizer=HtmlStylizer(), **vis_params)
         with open('trace.html', 'w') as f:
             f.write(html)
 
     unimplemented_hierarchy = find_unimplemented(node_hierarchy, converter_dict)
     if unimplemented_hierarchy is not None:
         print('Unimplemented nodes:')
-        print(unimplemented_hierarchy.__str__(validation_result_dict=validation_result_dict, conversion_result_dict=conversion_result_dict))
+        print(unimplemented_hierarchy.__str__(**vis_params))
         raise Exception('Unimplemented nodes')
 
     keras_op = keras_converted_node.keras_op
 
     args_tf, kwargs_tf = prepare_inputs_tf((args, kwargs), inputs_channel_order, input_shapes)
     outputs_tf = keras_op(*args_tf, **kwargs_tf)
     outputs_tf = postprocess_outputs_tf(outputs_tf, outputs_channel_order)
```

### Comparing `nobuco-0.3.0/nobuco/converters/channel_ordering.py` & `nobuco-0.4.0/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/converters/node_converter.py` & `nobuco-0.4.0/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/converters/tensor.py` & `nobuco-0.4.0/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/converters/type_cast.py` & `nobuco-0.4.0/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/converters/validation.py` & `nobuco-0.4.0/nobuco/converters/validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from enum import Enum
 import math
 
 import torch
 
 from nobuco.commons import ChannelOrder, TF_TENSOR_CLASSES
 from nobuco.converters.channel_ordering import t_keras2pytorch, pytorch2keras_recursively
+from nobuco.locate.link import get_link_to_obj
 from nobuco.util import str_parents, collect_recursively
 
 
 class ValidationStatus(Enum):
     SUCCESS = 1
     FAIL = 2
     INACCURATE = 3
@@ -18,32 +19,42 @@
 class ValidationResult:
     def __init__(self, diff, status):
         self.diff = diff
         self.status = status
 
 
 class ConversionResult:
-    def __init__(self, converted_manually, is_implemented=True, is_duplicate=False, connectivity_status=None):
+    def __init__(self, converted_manually, is_implemented=True, is_duplicate=False, connectivity_status=None, converter=None):
         self.converted_manually = converted_manually
         self.is_implemented = is_implemented
         self.is_duplicate = is_duplicate
         self.connectivity_status = connectivity_status
+        self.converter = converter
+
+    def get_converter_link(self):
+        if self.converter is None:
+            return None
+        else:
+            convert_func = self.converter.convert_func
+            location_link = get_link_to_obj(convert_func)
+            return location_link
 
 
 def validate(node, pytorch_op, keras_op, input_args, input_kwargs, output_tensors, op_type, tolerance=1e-4):
     try:
         diffs = validate_diff_default(keras_op, pytorch_op, input_args, input_kwargs, output_tensors)
 
         if len(diffs):
             for i, diff in enumerate(diffs):
                 if diff > tolerance or math.isnan(diff):
                     warnings.warn(
                         f'[{op_type}|{str_parents(node)}] conversion procedure might be incorrect: max. discrepancy for output #{i} is {diff:5f}',
                         category=RuntimeWarning
                     )
+                    pass
             diff = max(diffs)
         else:
             diff = 0
 
         if diff > tolerance or math.isnan(diff):
             return diff, ValidationStatus.INACCURATE
         else:
```

### Comparing `nobuco-0.3.0/nobuco/entity/keras.py` & `nobuco-0.4.0/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/entity/pytorch.py` & `nobuco-0.4.0/nobuco/entity/pytorch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import inspect
 import time
 from typing import Collection, List
 
 import torch
+from nobuco.locate.link import get_link_to_obj
 from torch import nn
 
+from nobuco.commons import TraceLevel
 from nobuco.converters.validation import ValidationStatus
 
 from nobuco.converters.channel_ordering import make_template_recursively
 from nobuco.util import collect_recursively, get_torch_tensor_identifier
 from nobuco.vis.console_stylizer import ConsoleStylizer
 
 
@@ -52,23 +55,24 @@
         self.style = style
         self.is_last = is_last
         self.is_disconnected = is_disconnected
         self.has_parent_outputs = has_parent_outputs
 
 
 class PytorchNode:
-    def __init__(self, wrapped_op: WrappedOp, module_name, parent_list, instance, input_args, input_kwargs, outputs, is_inplace):
+    def __init__(self, wrapped_op: WrappedOp, module_name, parent_list, instance, input_args, input_kwargs, outputs, is_inplace, traceback_summary):
         self.wrapped_op = wrapped_op
         self.module_name = module_name
         self.parent_list = parent_list
         self.instance = instance
         self.input_args = input_args
         self.input_kwargs = input_kwargs
         self.outputs = outputs
         self.is_inplace = is_inplace
+        self.traceback_summary = traceback_summary
 
     def make_inputs_template(self):
         args_template, kwargs_template = make_template_recursively((self.input_args, self.input_kwargs))
         return args_template, kwargs_template
 
     def make_outputs_template(self):
         outputs_template = make_template_recursively(self.outputs)
@@ -110,15 +114,16 @@
         self.children = children
 
     def __str__(self, tier=0,
                 tier_statuses=None,
                 validation_result_dict=None, conversion_result_dict=None,
                 with_legend=False, parent_connectivity_status=None,
                 tensor_name_assigner: TensorNameAssigner = None,
-                stylizer=None
+                stylizer=None,
+                debug_traces: TraceLevel = TraceLevel.NEVER,
                 ) -> str:
 
         if tier_statuses is None:
             tier_statuses = []
 
         if validation_result_dict is None:
             validation_result_dict = {}
@@ -260,14 +265,35 @@
                 result += stylizer.stylize(f' (!) Max diff {validation_result.diff:.6f} ', stylizer.styles_join(style, stylizer.style_inverse)) + ' '
             if is_disconnected:
                 result += stylizer.stylize(f' (!) Subgraph disconnected ', stylizer.style_inverse) + ' '
             if is_inplace:
                 result += stylizer.stylize(f' (!) Inplace ', stylizer.style_inplace) + ' '
             result += '\n'
 
+        are_problems = status == ValidationStatus.FAIL or status == ValidationStatus.INACCURATE or is_disconnected
+
+        if debug_traces == TraceLevel.ALWAYS or (debug_traces == TraceLevel.DEFAULT and are_problems):
+            result += get_tier_str(tier_statuses, is_additional=True)
+            summary = self.node.traceback_summary
+            result += stylizer.stylize(f' I ', stylizer.style_grey) + stylizer.stylize(f' File "{summary.filename}", line {summary.lineno}', stylizer.style_grey) + ' '
+            result += '\n'
+
+            link = get_link_to_obj(self.node.get_op().__class__)
+            if link is not None:
+                result += get_tier_str(tier_statuses, is_additional=True)
+                result += stylizer.stylize(f' D ', stylizer.style_grey) + stylizer.stylize(f' {link} ', stylizer.style_grey) + ' '
+                result += '\n'
+
+            if conversion_result is not None:
+                converter_link = conversion_result.get_converter_link()
+                if converter_link is not None:
+                    result += get_tier_str(tier_statuses, is_additional=True)
+                    result += stylizer.stylize(f' C ', style) + stylizer.stylize(f' {converter_link} ', stylizer.style_grey) + ' '
+                    result += '\n'
+
         result += get_tier_str(tier_statuses)
         result += \
             stylizer.stylize(
                 f'{"*" if is_duplicate else ""}' + f'{self.node.get_type().__name__}' + f'[{self.node.module_name}]',
                 style
             ) + \
             f'{to_str(FunctionArgs(self.node.input_args, self.node.input_kwargs), connectivity_status, parent_connectivity_status, is_input=True)}' + \
@@ -287,12 +313,13 @@
             for i, child in enumerate(self.children):
                 is_last = i == len(self.children) - 1
                 result += child.__str__(tier + 1,
                                         tier_statuses + [TierStatus(style=style, is_last=is_last, is_disconnected=is_disconnected, has_parent_outputs=has_parent_outputs_list[i])],
                                         validation_result_dict, conversion_result_dict,
                                         with_legend=False, parent_connectivity_status=connectivity_status,
                                         tensor_name_assigner=tensor_name_assigner,
-                                        stylizer=stylizer
+                                        stylizer=stylizer,
+                                        debug_traces=debug_traces,
                                         )
         if tier == 0:
             result = stylizer.postprocess(result)
         return result
```

### Comparing `nobuco-0.3.0/nobuco/funcs.py` & `nobuco-0.4.0/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/layers/channel_order.py` & `nobuco-0.4.0/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/layers/container.py` & `nobuco-0.4.0/nobuco/layers/container.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,13 @@
-from nobuco.commons import TF_TENSOR_CLASSES
+from nobuco.commons import TF_TENSOR_CLASSES, ConnectivityStatus
 from nobuco.layers.weight import WeightLayer
 from nobuco.converters.channel_ordering import TensorPlaceholder, template_insert_recursively
 from nobuco.util import collect_recursively
 
 
-class ConnectivityStatus:
-    def __init__(self, unused_inputs, unreached_outputs, unused_nodes, unprovided_inputs):
-        self.unused_inputs = unused_inputs
-        self.unreached_outputs = unreached_outputs
-        self.unused_nodes = unused_nodes
-        self.unprovided_inputs = unprovided_inputs
-
-    def is_connected(self):
-        return len(self.unreached_outputs) == 0
-
-
 class TransientContainer:
     def __init__(self, op_descr_list, input_names, output_names, outputs_template, constants_dict=None, disconnected_tensors_descr_list=None):
         self.op_descr_list = op_descr_list
         self.input_names = input_names
         self.output_names = output_names
         self.outputs_template = outputs_template
         self.constants_dict = {} if constants_dict is None else constants_dict
```

### Comparing `nobuco-0.3.0/nobuco/layers/weight.py` & `nobuco-0.4.0/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/locate.py` & `nobuco-0.4.0/nobuco/locate/link.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 import inspect
-from nobuco.trace.trace import Tracer
-from nobuco.converters.node_converter import CONVERTER_DICT
 
 
+# https://stackoverflow.com/a/64945941/4850610
+
 def get_link(file=None, line=None):
     """ Print a link in PyCharm to a line in file.
         Defaults to line where this function was called. """
     if file is None:
         file = inspect.stack()[1].filename
     if line is None:
         line = inspect.stack()[1].lineno
     string = f'File "{file}", line {max(line, 1)}'.replace("\\", "/")
     return string
 
 
 def get_link_to_obj(obj):
     """ Print a link in PyCharm to a module, function, class, method or property. """
-    if isinstance(obj, property):
-        obj = obj.fget
-    file = inspect.getfile(obj)
-    line = inspect.getsourcelines(obj)[1]
-    return get_link(file=file, line=line)
-
-
-def locate_converter(pytorch_node):
-    pytorch_node = Tracer.op_unwrap(pytorch_node)
-    node_converter = CONVERTER_DICT.get(pytorch_node, None)
-    if node_converter is not None:
-        convert_func = node_converter.convert_func
-        location_link = get_link_to_obj(convert_func)
-        source_code = inspect.getsource(convert_func)
-    else:
-        location_link, source_code = None, None
-    return location_link, source_code
+    try:
+        if isinstance(obj, property):
+            obj = obj.fget
+        file = inspect.getfile(obj)
+        line = inspect.getsourcelines(obj)[1]
+        return get_link(file=file, line=line)
+    except Exception:
+        return None
```

### Comparing `nobuco-0.3.0/nobuco/node_converters/activation.py` & `nobuco-0.4.0/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/boolean.py` & `nobuco-0.4.0/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/boolean_mask.py` & `nobuco-0.4.0/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/comparison.py` & `nobuco-0.4.0/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/convolution.py` & `nobuco-0.4.0/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/dropout.py` & `nobuco-0.4.0/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/interpolation.py` & `nobuco-0.4.0/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/linear.py` & `nobuco-0.4.0/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/math.py` & `nobuco-0.4.0/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/misc.py` & `nobuco-0.4.0/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/normalization.py` & `nobuco-0.4.0/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/padding.py` & `nobuco-0.4.0/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/pooling.py` & `nobuco-0.4.0/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/recurrent.py` & `nobuco-0.4.0/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/slice.py` & `nobuco-0.4.0/nobuco/node_converters/slice.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
     slices = _flatten(slices)
 
     if isinstance(slices[0], torch.Tensor):
         if slices[0].dtype == torch.bool:
             return converter_masked_select(self, slices[0])
         elif slices[0].dtype == torch.int64:
-            return getitem_indexed(self, slices)
+            return getitem_indexed.convert(self, slices)
 
     def is_light(slices):
         return all(isinstance(slc, slice) for slc in slices)
 
     if is_light(slices):
         def func(self, *slices):
             x = self
```

### Comparing `nobuco-0.3.0/nobuco/node_converters/tensor_cast.py` & `nobuco-0.4.0/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/tensor_creation.py` & `nobuco-0.4.0/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.4.0/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/trace/tensor_storage.py` & `nobuco-0.4.0/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/trace/trace.py` & `nobuco-0.4.0/nobuco/trace/trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,22 @@
 import inspect
+import traceback
 import types
 from copy import deepcopy
 from typing import List, Collection, Callable, Union
 
 import torch
 import torchvision
 from torch import nn
 
 from nobuco.entity.pytorch import PytorchNode, WrappedOp, PytorchNodeHierarchy
 from nobuco.trace.tensor_storage import clone_torch_tensors_recursively_with_cache, TensorStorage
 from nobuco.util import collect_recursively
 
 
-# def traceable():
-#     def inner(func_to_trace: Callable) -> Callable:
-#         if Tracer.is_decorated(func_to_trace):
-#             return func_to_trace
-#         else:
-#             module_suffix = func_to_trace.__qualname__
-#             module_suffix = '.'.join(module_suffix.split('.')[:-1])
-#             return Tracer.op_tracing_decorator(func_to_trace, inspect.getmodule(func_to_trace), module_suffix=module_suffix)
-#     return inner
-
-
 def traceable(func_to_trace: Callable):
     if Tracer.is_decorated(func_to_trace):
         return func_to_trace
     else:
         module_suffix = func_to_trace.__qualname__
         module_suffix = '.'.join(module_suffix.split('.')[:-1])
         return Tracer.op_tracing_decorator(func_to_trace, inspect.getmodule(func_to_trace), module_suffix=module_suffix)
@@ -96,15 +86,16 @@
                 Tracer._tracing_enabled = False
                 Tracer._parent_list = Tracer._parent_list[:-1]
 
                 # Protection from external modification
                 outputs_clone = clone_torch_tensors_recursively_with_cache(outputs, Tracer._tensor_storage)
                 is_inplace = not Tracer.are_equal((args, kwargs), (args_clone, kwargs_clone))
 
-                node = PytorchNode(wrapped_op, self.__module__, Tracer._parent_list.copy(), self, args_clone, kwargs_clone, outputs_clone, is_inplace)
+                summary: traceback.FrameSummary = traceback.extract_stack()[-3]
+                node = PytorchNode(wrapped_op, self.__module__, Tracer._parent_list.copy(), self, args_clone, kwargs_clone, outputs_clone, is_inplace, summary)
                 Tracer._node_list.append(node)
 
                 Tracer._tracing_enabled = True
                 return outputs
             else:
                 outputs = forward_func(*args, **kwargs)
             return outputs
@@ -146,15 +137,16 @@
                     if '__setitem__' in str(orig_method):
                         outputs = args[0]
 
                     # Protection from external modification
                     outputs_clone = clone_torch_tensors_recursively_with_cache(outputs, Tracer._tensor_storage)
                     is_inplace = not Tracer.are_equal((args, kwargs), (args_clone, kwargs_clone))
 
-                    node = PytorchNode(wrapped_op, module_name, Tracer._parent_list.copy(), None, args_clone, kwargs_clone, outputs_clone, is_inplace)
+                    summary: traceback.FrameSummary = traceback.extract_stack()[-2]
+                    node = PytorchNode(wrapped_op, module_name, Tracer._parent_list.copy(), None, args_clone, kwargs_clone, outputs_clone, is_inplace, summary)
                     Tracer._node_list.append(node)
 
                 Tracer._tracing_enabled = True
             else:
                 outputs = orig_method(*args, **kwargs)
             return outputs
```

### Comparing `nobuco-0.3.0/nobuco/util.py` & `nobuco-0.4.0/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.3.0/nobuco/vis/console_stylizer.py` & `nobuco-0.4.0/nobuco/vis/console_stylizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sty import ef, fg, rs
 
 from nobuco.converters.validation import ValidationStatus
-from nobuco.layers.container import ConnectivityStatus
+from nobuco.commons import ConnectivityStatus
 from nobuco.util import get_torch_tensor_identifier
 
 
 class ConsoleStylizer:
 
     def postprocess(self, text):
         return text
```

### Comparing `nobuco-0.3.0/nobuco/vis/html_stylizer.py` & `nobuco-0.4.0/nobuco/vis/html_stylizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict
 
 from nobuco.converters.validation import ValidationStatus
-from nobuco.layers.container import ConnectivityStatus
+from nobuco.commons import ConnectivityStatus
 from nobuco.util import get_torch_tensor_identifier
 
 
 class HtmlStylizer:
 
     def postprocess(self, text):
         text = text.replace('\n', '<br>\n')
```

### Comparing `nobuco-0.3.0/nobuco.egg-info/PKG-INFO` & `nobuco-0.4.0/nobuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.3.0
+Version: 0.4.0
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -324,15 +324,15 @@
         return x
 ```
 
 Of course, it's possible to translate the dynamic module into a tensorflow layer
 (don't forget to decorate it with `@tf.function` for autograph to kick in).
 But what if it contains inner modules, do you replicate them in tensorflow all by hand?
 Not unless you want to! 
-Just convert them separately and use the resulting graph inside the parent layer.
+Just convert them separately and use the resulting graphs inside the parent layer.
 
 ```python
 class ControlIfKeras(tf.keras.layers.Layer):
     def __init__(self, conv_pre, conv_true, conv_false, conv_shared, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.conv_pre = conv_pre
         self.conv_true = conv_true
@@ -383,15 +383,15 @@
 <img src="docs/control_if.png" width="25%">
 </p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
 ### Dynamic shapes
 
-What if we wanted out module to accept images of arbitrary height and width?
+What if we wanted our module to accept images of arbitrary height and width?
 Can we have that? Let's try:
 
 ```python
 class DynamicShape(nn.Module):
     def __init__(self):
         super().__init__()
         self.conv = nn.Conv2d(3, 16, kernel_size=(1, 1))
```

### Comparing `nobuco-0.3.0/pyproject.toml` & `nobuco-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.3.0"
+version = "0.4.0"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

