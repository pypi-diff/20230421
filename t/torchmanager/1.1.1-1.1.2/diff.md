# Comparing `tmp/torchmanager-1.1.1.tar.gz` & `tmp/torchmanager-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager-1.1.1.tar", last modified: Tue Apr  4 16:15:41 2023, max compression
+gzip compressed data, was "torchmanager-1.1.2.tar", last modified: Fri Apr 21 18:44:52 2023, max compression
```

## Comparing `torchmanager-1.1.1.tar` & `torchmanager-1.1.2.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-04 16:15:41.118913 torchmanager-1.1.1/
--rw-r--r--   0 kisonho    (501) staff       (20)     1318 2023-03-16 14:38:14.000000 torchmanager-1.1.1/LICENSE
--rw-r--r--   0 kisonho    (501) staff       (20)     2102 2023-04-04 16:15:41.118635 torchmanager-1.1.1/PKG-INFO
--rw-r--r--   0 kisonho    (501) staff       (20)     1806 2023-04-04 16:06:45.000000 torchmanager-1.1.1/README.md
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-04 16:15:41.102122 torchmanager-1.1.1/core/
--rw-r--r--   0 kisonho    (501) staff       (20)      434 2023-04-04 16:06:33.000000 torchmanager-1.1.1/core/__init__.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-04 16:15:41.103143 torchmanager-1.1.1/core/devices/
--rw-r--r--   0 kisonho    (501) staff       (20)      114 2023-04-04 16:06:33.000000 torchmanager-1.1.1/core/devices/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     5590 2023-04-04 16:06:33.000000 torchmanager-1.1.1/core/devices/device.py
--rw-r--r--   0 kisonho    (501) staff       (20)      264 2023-03-16 14:38:14.000000 torchmanager-1.1.1/core/devices/protocols.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-04 16:15:41.104039 torchmanager-1.1.1/core/errors/
--rw-r--r--   0 kisonho    (501) staff       (20)      153 2023-03-19 20:02:58.000000 torchmanager-1.1.1/core/errors/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)      350 2023-03-19 20:02:58.000000 torchmanager-1.1.1/core/errors/runtime.py
--rw-r--r--   0 kisonho    (501) staff       (20)      669 2023-03-19 20:02:58.000000 torchmanager-1.1.1/core/errors/train.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2728 2023-03-19 20:02:58.000000 torchmanager-1.1.1/core/protocols.py
--rw-r--r--   0 kisonho    (501) staff       (20)      204 2023-03-19 20:02:58.000000 torchmanager-1.1.1/core/typing.py
--rw-r--r--   0 kisonho    (501) staff       (20)     1298 2023-04-04 16:06:45.000000 torchmanager-1.1.1/core/version.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-04 16:15:41.104736 torchmanager-1.1.1/core/view/
--rw-r--r--   0 kisonho    (501) staff       (20)      126 2023-04-04 16:06:33.000000 torchmanager-1.1.1/core/view/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)      313 2023-03-16 14:38:14.000000 torchmanager-1.1.1/core/view/protocols.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-04 16:15:41.106497 torchmanager-1.1.1/lib/
--rw-r--r--   0 kisonho    (501) staff       (20)      281 2023-04-04 16:06:33.000000 torchmanager-1.1.1/lib/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)    11039 2023-04-04 16:06:45.000000 torchmanager-1.1.1/lib/basic.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-04 16:15:41.109755 torchmanager-1.1.1/lib/callbacks/
--rw-r--r--   0 kisonho    (501) staff       (20)      476 2023-03-19 20:02:58.000000 torchmanager-1.1.1/lib/callbacks/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4255 2023-03-19 20:02:58.000000 torchmanager-1.1.1/lib/callbacks/callback.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4542 2023-03-19 20:02:58.000000 torchmanager-1.1.1/lib/callbacks/ckpt.py
--rw-r--r--   0 kisonho    (501) staff       (20)     3523 2023-03-19 20:02:58.000000 torchmanager-1.1.1/lib/callbacks/dynamic.py
--rw-r--r--   0 kisonho    (501) staff       (20)     1608 2023-03-19 20:02:58.000000 torchmanager-1.1.1/lib/callbacks/early_stop.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4897 2023-04-04 16:06:45.000000 torchmanager-1.1.1/lib/callbacks/experiment.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2224 2023-03-19 20:02:58.000000 torchmanager-1.1.1/lib/callbacks/lr.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2440 2023-03-19 20:02:58.000000 torchmanager-1.1.1/lib/callbacks/tensorboard.py
--rw-r--r--   0 kisonho    (501) staff       (20)      847 2023-04-04 16:06:45.000000 torchmanager-1.1.1/lib/compatibility.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-04 16:15:41.110550 torchmanager-1.1.1/lib/data/
--rw-r--r--   0 kisonho    (501) staff       (20)       69 2023-04-04 16:06:45.000000 torchmanager-1.1.1/lib/data/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     6866 2023-03-31 14:32:51.000000 torchmanager-1.1.1/lib/data/dataset.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-04 16:15:41.111340 torchmanager-1.1.1/lib/data/utils/
--rw-r--r--   0 kisonho    (501) staff       (20)       35 2023-04-04 16:06:45.000000 torchmanager-1.1.1/lib/data/utils/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2483 2023-04-04 16:06:45.000000 torchmanager-1.1.1/lib/data/utils/sliding.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-04 16:15:41.113083 torchmanager-1.1.1/lib/losses/
--rw-r--r--   0 kisonho    (501) staff       (20)      171 2023-04-04 16:06:33.000000 torchmanager-1.1.1/lib/losses/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     5386 2023-03-19 20:02:58.000000 torchmanager-1.1.1/lib/losses/cross_entropy.py
--rw-r--r--   0 kisonho    (501) staff       (20)     1044 2023-03-19 20:02:58.000000 torchmanager-1.1.1/lib/losses/dice.py
--rw-r--r--   0 kisonho    (501) staff       (20)     7061 2023-04-04 16:06:33.000000 torchmanager-1.1.1/lib/losses/loss.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2381 2023-04-04 16:06:33.000000 torchmanager-1.1.1/lib/losses/mse.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-04 16:15:41.114780 torchmanager-1.1.1/lib/metrics/
--rw-r--r--   0 kisonho    (501) staff       (20)      223 2023-04-04 16:06:33.000000 torchmanager-1.1.1/lib/metrics/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     3272 2023-04-04 16:06:33.000000 torchmanager-1.1.1/lib/metrics/accuracy.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2126 2023-03-19 20:02:58.000000 torchmanager-1.1.1/lib/metrics/conf_met.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2561 2023-04-04 16:06:33.000000 torchmanager-1.1.1/lib/metrics/iou.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4000 2023-03-19 20:02:58.000000 torchmanager-1.1.1/lib/metrics/metric.py
--rw-r--r--   0 kisonho    (501) staff       (20)     9401 2023-04-04 16:06:45.000000 torchmanager-1.1.1/lib/testing.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-04 16:15:41.115944 torchmanager-1.1.1/lib/train/
--rw-r--r--   0 kisonho    (501) staff       (20)      191 2023-04-04 16:06:33.000000 torchmanager-1.1.1/lib/train/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4964 2023-03-19 20:02:58.000000 torchmanager-1.1.1/lib/train/checkpoint.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2037 2023-04-04 16:06:33.000000 torchmanager-1.1.1/lib/train/learning_rate.py
--rw-r--r--   0 kisonho    (501) staff       (20)    14893 2023-04-04 16:06:45.000000 torchmanager-1.1.1/lib/training.py
--rw-r--r--   0 kisonho    (501) staff       (20)       38 2023-04-04 16:15:41.119005 torchmanager-1.1.1/setup.cfg
--rw-r--r--   0 kisonho    (501) staff       (20)     1465 2023-04-04 16:06:45.000000 torchmanager-1.1.1/setup.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-04 16:15:41.118128 torchmanager-1.1.1/torchmanager.egg-info/
--rw-r--r--   0 kisonho    (501) staff       (20)     2102 2023-04-04 16:15:41.000000 torchmanager-1.1.1/torchmanager.egg-info/PKG-INFO
--rw-r--r--   0 kisonho    (501) staff       (20)     1130 2023-04-04 16:15:41.000000 torchmanager-1.1.1/torchmanager.egg-info/SOURCES.txt
--rw-r--r--   0 kisonho    (501) staff       (20)        1 2023-04-04 16:15:41.000000 torchmanager-1.1.1/torchmanager.egg-info/dependency_links.txt
--rw-r--r--   0 kisonho    (501) staff       (20)       11 2023-04-04 16:15:41.000000 torchmanager-1.1.1/torchmanager.egg-info/requires.txt
--rw-r--r--   0 kisonho    (501) staff       (20)       31 2023-04-04 16:15:41.000000 torchmanager-1.1.1/torchmanager.egg-info/top_level.txt
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.733735 torchmanager-1.1.2/
+-rw-r--r--   0 kisonho    (501) staff       (20)     1318 2023-04-07 18:23:00.000000 torchmanager-1.1.2/LICENSE
+-rw-r--r--   0 kisonho    (501) staff       (20)     2102 2023-04-21 18:44:52.733328 torchmanager-1.1.2/PKG-INFO
+-rw-r--r--   0 kisonho    (501) staff       (20)     1806 2023-04-07 18:23:00.000000 torchmanager-1.1.2/README.md
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.709401 torchmanager-1.1.2/core/
+-rw-r--r--   0 kisonho    (501) staff       (20)      443 2023-04-21 18:38:20.000000 torchmanager-1.1.2/core/__init__.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.711064 torchmanager-1.1.2/core/devices/
+-rw-r--r--   0 kisonho    (501) staff       (20)      114 2023-04-21 18:38:20.000000 torchmanager-1.1.2/core/devices/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     5587 2023-04-21 18:38:20.000000 torchmanager-1.1.2/core/devices/device.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      264 2023-03-16 14:38:14.000000 torchmanager-1.1.2/core/devices/protocols.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.712803 torchmanager-1.1.2/core/errors/
+-rw-r--r--   0 kisonho    (501) staff       (20)      153 2023-04-07 18:23:00.000000 torchmanager-1.1.2/core/errors/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      350 2023-04-07 18:23:00.000000 torchmanager-1.1.2/core/errors/runtime.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      669 2023-04-07 18:23:00.000000 torchmanager-1.1.2/core/errors/train.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2728 2023-04-21 18:38:20.000000 torchmanager-1.1.2/core/protocols.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      204 2023-04-07 18:23:00.000000 torchmanager-1.1.2/core/typing.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     5288 2023-04-21 18:38:20.000000 torchmanager-1.1.2/core/version.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.713919 torchmanager-1.1.2/core/view/
+-rw-r--r--   0 kisonho    (501) staff       (20)      126 2023-04-21 18:38:20.000000 torchmanager-1.1.2/core/view/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      313 2023-03-16 14:38:14.000000 torchmanager-1.1.2/core/view/protocols.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.716500 torchmanager-1.1.2/lib/
+-rw-r--r--   0 kisonho    (501) staff       (20)      281 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)    11052 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/basic.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.720931 torchmanager-1.1.2/lib/callbacks/
+-rw-r--r--   0 kisonho    (501) staff       (20)      658 2023-04-21 18:31:47.000000 torchmanager-1.1.2/lib/callbacks/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4255 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/callbacks/callback.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4542 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/callbacks/ckpt.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     3523 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/callbacks/dynamic.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     1608 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/callbacks/early_stop.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4846 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/callbacks/experiment.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2224 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/callbacks/lr.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2440 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/callbacks/tensorboard.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      963 2023-04-21 18:34:55.000000 torchmanager-1.1.2/lib/compatibility.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.722427 torchmanager-1.1.2/lib/data/
+-rw-r--r--   0 kisonho    (501) staff       (20)       85 2023-04-21 18:31:47.000000 torchmanager-1.1.2/lib/data/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     6866 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/data/dataset.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2236 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/data/sliding.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.724764 torchmanager-1.1.2/lib/losses/
+-rw-r--r--   0 kisonho    (501) staff       (20)      171 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/losses/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     5386 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/losses/cross_entropy.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     1044 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/losses/dice.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     7061 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/losses/loss.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2381 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/losses/mse.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.727102 torchmanager-1.1.2/lib/metrics/
+-rw-r--r--   0 kisonho    (501) staff       (20)      234 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/metrics/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     3272 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/metrics/accuracy.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2546 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/metrics/conf_met.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2440 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/metrics/iou.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4000 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/metrics/metric.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     9401 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/testing.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.728550 torchmanager-1.1.2/lib/train/
+-rw-r--r--   0 kisonho    (501) staff       (20)      191 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/train/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4964 2023-04-07 18:23:00.000000 torchmanager-1.1.2/lib/train/checkpoint.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2037 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/train/learning_rate.py
+-rw-r--r--   0 kisonho    (501) staff       (20)    14893 2023-04-21 18:38:20.000000 torchmanager-1.1.2/lib/training.py
+-rw-r--r--   0 kisonho    (501) staff       (20)       38 2023-04-21 18:44:52.733904 torchmanager-1.1.2/setup.cfg
+-rw-r--r--   0 kisonho    (501) staff       (20)     1377 2023-04-21 18:38:20.000000 torchmanager-1.1.2/setup.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.730162 torchmanager-1.1.2/tests/
+-rw-r--r--   0 kisonho    (501) staff       (20)     1203 2023-04-17 18:56:25.000000 torchmanager-1.1.2/tests/test_0101.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      934 2023-04-17 15:45:19.000000 torchmanager-1.1.2/tests/test_0102.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      263 2023-04-17 15:33:18.000000 torchmanager-1.1.2/tests/test_base.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 18:44:52.732740 torchmanager-1.1.2/torchmanager.egg-info/
+-rw-r--r--   0 kisonho    (501) staff       (20)     2102 2023-04-21 18:44:52.000000 torchmanager-1.1.2/torchmanager.egg-info/PKG-INFO
+-rw-r--r--   0 kisonho    (501) staff       (20)     1154 2023-04-21 18:44:52.000000 torchmanager-1.1.2/torchmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 kisonho    (501) staff       (20)        1 2023-04-21 18:44:52.000000 torchmanager-1.1.2/torchmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 kisonho    (501) staff       (20)       11 2023-04-21 18:44:52.000000 torchmanager-1.1.2/torchmanager.egg-info/requires.txt
+-rw-r--r--   0 kisonho    (501) staff       (20)       31 2023-04-21 18:44:52.000000 torchmanager-1.1.2/torchmanager.egg-info/top_level.txt
```

### Comparing `torchmanager-1.1.1/LICENSE` & `torchmanager-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/PKG-INFO` & `torchmanager-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torchmanager
-Version: 1.1.1
-Summary: PyTorch Training Manager v1.1.1
+Version: 1.1.2
+Summary: PyTorch Training Manager v1.1.2
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Kison Ho
 Author-email: unfit-gothic.0q@icloud.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `torchmanager-1.1.1/README.md` & `torchmanager-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/core/devices/device.py` & `torchmanager-1.1.2/core/devices/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,16 +88,16 @@
         specified = [specified]
     elif len(specified) > 0:
         # set default device
         device = torch.device(specified[0].type)
 
         # check for each device
         for d in specified:
-            if d.type != GPU.type: raise SystemError("All devices in the specified list must have the same device type with GPU type")
-            if d.index is None: raise SystemError("All devices in the specified list must have a device index")
+            if d.type != specified[0].type: raise SystemError("All devices in the specified list must have the same device type.")
+            if d.index is None: raise SystemError("All devices in the specified list must have a device index.")
     else: raise SystemError("Specified device list must not be empty")
     return CPU, device, specified
 
 def move_to_device(target: Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]], device: torch.device, recursive: bool = False) -> Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]]:
     """
     Recurrently move a target variable to device if elements perform to `DeviceMovable` protocol
```

### Comparing `torchmanager-1.1.1/core/errors/train.py` & `torchmanager-1.1.2/core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/core/protocols.py` & `torchmanager-1.1.2/core/protocols.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/basic.py` & `torchmanager-1.1.2/lib/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from torchmanager_core import torch, _raise, API_VERSION, VERSION as CURRENT_VERSION
+from torchmanager_core import torch, Version, _raise, API_VERSION, VERSION as CURRENT_VERSION
 from torchmanager_core.typing import Any, Collection, Dict, Generic, Module, Optional, OrderedDict, Self, Tuple, Union
 
 from .compatibility import convert
 from .losses import Loss, MultiLosses, MultiOutputsLosses, ParallelLoss
 from .metrics import Metric
 from .train import Checkpoint
 
@@ -43,15 +43,15 @@
         - raw_model: A non-paralleled target `torch.nn.Module` model
     """
     # properties
     loss_fn: Optional[Union[Loss, ParallelLoss]]
     metric_fns: Dict[str, Metric]
     model: Module
     optimizer: Optional[torch.optim.Optimizer]
-    version: str
+    version: Version
 
     @property
     def compiled(self) -> bool:
         return True if self.loss_fn is not None and self.optimizer is not None else False
 
     @property
     def raw_loss_fn(self) -> Optional[Loss]:
```

### Comparing `torchmanager-1.1.1/lib/callbacks/callback.py` & `torchmanager-1.1.2/lib/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/callbacks/ckpt.py` & `torchmanager-1.1.2/lib/callbacks/ckpt.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/callbacks/dynamic.py` & `torchmanager-1.1.2/lib/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/callbacks/early_stop.py` & `torchmanager-1.1.2/lib/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/callbacks/experiment.py` & `torchmanager-1.1.2/lib/callbacks/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
             best_ckpt_path = os.path.join(ckpt_path, f"best_{m}.model")
             best_ckpt = BestCheckpoint(m, model, best_ckpt_path, monitor_type=mode)
             self.best_ckpts.append(best_ckpt)
 
         # initialize logging
         log_file = os.path.basename(experiment.replace(".exp", ".log"))
         log_path = os.path.join(experiment_dir, log_file)
-        os.makedirs(experiment_dir, exist_ok=True)
         logger = logging.getLogger("torchmanager")
         logger.handlers.clear()
         logger.setLevel(logging.INFO)
         file_handler = logging.FileHandler(log_path)
         formatter = logging.Formatter("%(message)s")
         file_handler.setFormatter(formatter)
         logger.addHandler(file_handler)
```

### Comparing `torchmanager-1.1.1/lib/callbacks/lr.py` & `torchmanager-1.1.2/lib/callbacks/lr.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/callbacks/tensorboard.py` & `torchmanager-1.1.2/lib/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/compatibility.py` & `torchmanager-1.1.2/lib/compatibility.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+from torchmanager_core import Version
 from torchmanager_core.typing import Any, Optional, TypeVar
 
 from .losses import KLDiv
 from .metrics import Accuracy, MAE, Reduction
 
 T = TypeVar("T")
 
 
-def convert(obj: T, from_version: Optional[str] = None) -> T:
+def convert(obj: T, from_version: Optional[Any] = None) -> T:
     """
     Convert an object from old version of torchmanager to the latest one.
     """
+    # format version
+    v = Version(from_version) if from_version is not None else Version("v1.0")
+
     # Return if None
     if obj is None:
         return obj
 
-    if from_version is None: # convert from 1.0 (from_version = None)
+    if v < Version("v1.1"): # convert from 1.0
         # convert KLDiv
         if isinstance(obj, KLDiv) and not hasattr(obj, "replace_nan"):
             obj.replace_nan = False
         elif isinstance(obj, KLDiv) and not hasattr(obj, "_t"):
             obj._t = None
 
         # convert Accuracy and MAE
```

### Comparing `torchmanager-1.1.1/lib/data/dataset.py` & `torchmanager-1.1.2/lib/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/data/utils/sliding.py` & `torchmanager-1.1.2/lib/data/sliding.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 from itertools import product
 from torchmanager_core import torch, _raise
 from torchmanager_core.typing import List, Tuple
 
+
 def sliding_window(image: torch.Tensor, window_size: Tuple[int, ...], stride: Tuple[int, ...]) -> torch.Tensor:
     """
-    Extract sliding windows from a multi-dimensional PyTorch tensor.
+    Extract sliding windows from a multi-dimensional `torch.Tensor`.
 
     - Parameters:
         - image: The input image `torch.Tensor`. Can have any number of dimensions.
         - window_size: A `tuple` of the size of the sliding window in `int` to extract from the image, must have the same number of dimensions as the input image tensor.
         - stride: A `tuple` of the stride of the sliding window in `int`, must have the same number of dimensions as the input image tensor.
-
-    Returns: A list of PyTorch tensors, where each tensor corresponds to a
-            sliding window extracted from the input image tensor.
-
-    Raises: ValueError: If the window size or stride are not valid for the input image tensor.
+    Returns: A `list` of `torch.Tensor`, where each tensor corresponds to a sliding window extracted from the input image tensor.
+    Raises: `ValueError` if the window size or stride are not valid for the input image tensor.
 
     Example:
     ```
     >>> image = torch.randn(3, 224, 224)
     >>> window_size = (64, 64)
     >>> stride = (32, 32)
     >>> windows = sliding_window(image, window_size, stride)
     >>> windows.shape[0]
-    49
+    36
     ```
     """
-    # check inputs
-    assert len(window_size) == len(image.shape) == len(image.shape), _raise(ValueError(f"Window size dimension ({len(window_size)}) and stride dimension ({stride}) must be the same of image ({len(image.shape)})."))
+    # initialize
+    assert len(window_size) == len(stride), _raise(ValueError(f"Window size dimension ({len(window_size)}) and stride dimension ({stride}) must be the same."))
+    stride_dims: List[int] = []
+    windows: List[torch.Tensor] = []
+    window_dims: List[int] = []
 
     # Calculate number of windows in each dimension
-    window_dims: List[int] = []
-    stride_dims: List[int] = []
-    for dim_size, window_dim, stride_dim in zip(image.shape, window_size, stride):
+    for dim_size, window_dim, stride_dim in zip(image.shape[1:], window_size, stride):
         num_windows = (dim_size - window_dim) // stride_dim + 1
         window_dims.append(num_windows)
         stride_dims.append(stride_dim)
-    
-    # Create a list to hold the windows
-    windows: List[torch.Tensor] = []
-    
+
     # Iterate over each window
     window_starts = product(*[range(num_windows) for num_windows in window_dims])
-    for starts in window_starts:
+    for indices in window_starts:
         # Calculate the starting coordinates of the window
-        starts = torch.tensor(starts)
-        window_starts = starts * torch.tensor(stride_dims)
-        window_ends = window_starts + torch.tensor(window_size)
-        
+        indices = (slice(None),) + tuple(slice(i, i+ws) for i, ws in zip(indices, window_size))
+
         # Extract the window from the image
-        window = image[tuple(slice(s, e) for s, e in zip(window_starts, window_ends))]
-        
+        window = image[indices]
+
         # Add the window to the list
         windows.append(window.unsqueeze(0))
-    return torch.cat(windows)
+    return torch.cat(windows)
```

### Comparing `torchmanager-1.1.1/lib/losses/cross_entropy.py` & `torchmanager-1.1.2/lib/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/losses/dice.py` & `torchmanager-1.1.2/lib/losses/dice.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/losses/loss.py` & `torchmanager-1.1.2/lib/losses/loss.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/losses/mse.py` & `torchmanager-1.1.2/lib/losses/mse.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/metrics/accuracy.py` & `torchmanager-1.1.2/lib/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/metrics/iou.py` & `torchmanager-1.1.2/lib/metrics/iou.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,19 +14,15 @@
     """
 
     def __init__(self, num_classes: int, target: Optional[str] = None) -> None:
         super().__init__(num_classes, target=target)
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         # argmax for input
-        input = input.argmax(1).to(target.dtype)
-
-        # calculate mean IoU
-        hist = super().forward(input, target)
-        iou = torch.diag(hist) / (hist.sum(1) + hist.sum(0) - torch.diag(hist))
+        iou = torch.diag(input) / (input.sum(1) + input.sum(0) - torch.diag(input))
         return iou.nanmean()
 
 
 class MeanIoU(Metric):
     """
     The mIoU metric for segmentation
```

### Comparing `torchmanager-1.1.1/lib/metrics/metric.py` & `torchmanager-1.1.2/lib/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/testing.py` & `torchmanager-1.1.2/lib/testing.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/train/checkpoint.py` & `torchmanager-1.1.2/lib/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/train/learning_rate.py` & `torchmanager-1.1.2/lib/train/learning_rate.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/lib/training.py` & `torchmanager-1.1.2/lib/training.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.1/setup.py` & `torchmanager-1.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 from distutils.core import setup
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='torchmanager',
-    version="1.1.1",
-    description="PyTorch Training Manager v1.1.1",
+    version="1.1.2",
+    description="PyTorch Training Manager v1.1.2",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Kison Ho',
     author_email='unfit-gothic.0q@icloud.com',
     packages=[
         'torchmanager',
         'torchmanager.callbacks',
         'torchmanager.data',
-        'torchmanager.data.utils',
         'torchmanager.losses',
         'torchmanager.metrics',
         'torchmanager.train',
         'torchmanager_core',
         'torchmanager_core.devices',
         'torchmanager_core.errors',
         'torchmanager_core.view',
     ],
     package_dir={
         'torchmanager': 'lib',
         'torchmanager.callbacks': 'lib/callbacks',
         'torchmanager.data': 'lib/data',
-        'torchmanager.data.utils': 'lib/data/utils',
         'torchmanager.losses': 'lib/losses',
         'torchmanager.metrics': 'lib/metrics',
         'torchmanager.train': 'lib/train',
         'torchmanager_core': 'core',
         'torchmanager_core.devices': 'core/devices',
         'torchmanager_core.errors': 'core/errors',
         'torchmanager_core.view': 'core/view',
```

### Comparing `torchmanager-1.1.1/torchmanager.egg-info/PKG-INFO` & `torchmanager-1.1.2/torchmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torchmanager
-Version: 1.1.1
-Summary: PyTorch Training Manager v1.1.1
+Version: 1.1.2
+Summary: PyTorch Training Manager v1.1.2
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Kison Ho
 Author-email: unfit-gothic.0q@icloud.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `torchmanager-1.1.1/torchmanager.egg-info/SOURCES.txt` & `torchmanager-1.1.2/torchmanager.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,27 +24,29 @@
 lib/callbacks/dynamic.py
 lib/callbacks/early_stop.py
 lib/callbacks/experiment.py
 lib/callbacks/lr.py
 lib/callbacks/tensorboard.py
 lib/data/__init__.py
 lib/data/dataset.py
-lib/data/utils/__init__.py
-lib/data/utils/sliding.py
+lib/data/sliding.py
 lib/losses/__init__.py
 lib/losses/cross_entropy.py
 lib/losses/dice.py
 lib/losses/loss.py
 lib/losses/mse.py
 lib/metrics/__init__.py
 lib/metrics/accuracy.py
 lib/metrics/conf_met.py
 lib/metrics/iou.py
 lib/metrics/metric.py
 lib/train/__init__.py
 lib/train/checkpoint.py
 lib/train/learning_rate.py
+tests/test_0101.py
+tests/test_0102.py
+tests/test_base.py
 torchmanager.egg-info/PKG-INFO
 torchmanager.egg-info/SOURCES.txt
 torchmanager.egg-info/dependency_links.txt
 torchmanager.egg-info/requires.txt
 torchmanager.egg-info/top_level.txt
```

