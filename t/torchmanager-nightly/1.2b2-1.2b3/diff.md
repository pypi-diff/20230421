# Comparing `tmp/torchmanager-nightly-1.2b2.tar.gz` & `tmp/torchmanager-nightly-1.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager-nightly-1.2b2.tar", last modified: Fri Apr  7 17:36:34 2023, max compression
+gzip compressed data, was "torchmanager-nightly-1.2b3.tar", last modified: Fri Apr 21 19:23:59 2023, max compression
```

## Comparing `torchmanager-nightly-1.2b2.tar` & `torchmanager-nightly-1.2b3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.429159 torchmanager-nightly-1.2b2/
--rw-r--r--   0 kisonho    (501) staff       (20)     1318 2023-03-16 14:38:14.000000 torchmanager-nightly-1.2b2/LICENSE
--rw-r--r--   0 kisonho    (501) staff       (20)     2117 2023-04-07 17:36:34.428718 torchmanager-nightly-1.2b2/PKG-INFO
--rw-r--r--   0 kisonho    (501) staff       (20)     1806 2023-04-04 16:25:31.000000 torchmanager-nightly-1.2b2/README.md
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.392858 torchmanager-nightly-1.2b2/core/
--rw-r--r--   0 kisonho    (501) staff       (20)      457 2023-04-07 17:35:31.000000 torchmanager-nightly-1.2b2/core/__init__.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.395006 torchmanager-nightly-1.2b2/core/devices/
--rw-r--r--   0 kisonho    (501) staff       (20)      109 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/core/devices/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4870 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/core/devices/device.py
--rw-r--r--   0 kisonho    (501) staff       (20)      264 2023-03-16 14:38:14.000000 torchmanager-nightly-1.2b2/core/devices/protocols.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.397213 torchmanager-nightly-1.2b2/core/errors/
--rw-r--r--   0 kisonho    (501) staff       (20)      153 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/core/errors/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)      350 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/core/errors/runtime.py
--rw-r--r--   0 kisonho    (501) staff       (20)      669 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/core/errors/train.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2728 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/core/protocols.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.398715 torchmanager-nightly-1.2b2/core/random/
--rw-r--r--   0 kisonho    (501) staff       (20)       44 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/core/random/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)      876 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/core/random/seed.py
--rw-r--r--   0 kisonho    (501) staff       (20)      204 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/core/typing.py
--rw-r--r--   0 kisonho    (501) staff       (20)     1305 2023-04-07 17:35:31.000000 torchmanager-nightly-1.2b2/core/version.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.399854 torchmanager-nightly-1.2b2/core/view/
--rw-r--r--   0 kisonho    (501) staff       (20)      439 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/core/view/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)      313 2023-03-16 14:38:14.000000 torchmanager-nightly-1.2b2/core/view/protocols.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.403638 torchmanager-nightly-1.2b2/lib/
--rw-r--r--   0 kisonho    (501) staff       (20)      290 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/lib/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)    10805 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/lib/basic.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.410461 torchmanager-nightly-1.2b2/lib/callbacks/
--rw-r--r--   0 kisonho    (501) staff       (20)      476 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/lib/callbacks/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4255 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/lib/callbacks/callback.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4542 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/lib/callbacks/ckpt.py
--rw-r--r--   0 kisonho    (501) staff       (20)     3523 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/lib/callbacks/dynamic.py
--rw-r--r--   0 kisonho    (501) staff       (20)     1608 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/lib/callbacks/early_stop.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4611 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/lib/callbacks/experiment.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2224 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/lib/callbacks/lr.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2440 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/lib/callbacks/tensorboard.py
--rw-r--r--   0 kisonho    (501) staff       (20)      810 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/lib/compatibility.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.411966 torchmanager-nightly-1.2b2/lib/configs/
--rw-r--r--   0 kisonho    (501) staff       (20)       26 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/lib/configs/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2836 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/lib/configs/basic.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.413568 torchmanager-nightly-1.2b2/lib/data/
--rw-r--r--   0 kisonho    (501) staff       (20)       69 2023-04-04 16:25:31.000000 torchmanager-nightly-1.2b2/lib/data/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     6866 2023-04-04 16:23:16.000000 torchmanager-nightly-1.2b2/lib/data/dataset.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.415266 torchmanager-nightly-1.2b2/lib/data/utils/
--rw-r--r--   0 kisonho    (501) staff       (20)       35 2023-04-04 16:25:31.000000 torchmanager-nightly-1.2b2/lib/data/utils/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2483 2023-04-04 16:25:31.000000 torchmanager-nightly-1.2b2/lib/data/utils/sliding.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.418532 torchmanager-nightly-1.2b2/lib/losses/
--rw-r--r--   0 kisonho    (501) staff       (20)      156 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/lib/losses/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     5386 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/lib/losses/cross_entropy.py
--rw-r--r--   0 kisonho    (501) staff       (20)     1044 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/lib/losses/dice.py
--rw-r--r--   0 kisonho    (501) staff       (20)     5757 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/lib/losses/loss.py
--rw-r--r--   0 kisonho    (501) staff       (20)     3108 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/lib/losses/mse.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.422337 torchmanager-nightly-1.2b2/lib/metrics/
--rw-r--r--   0 kisonho    (501) staff       (20)      238 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/lib/metrics/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     3056 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/lib/metrics/accuracy.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2126 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/lib/metrics/conf_met.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4539 2023-04-07 17:35:31.000000 torchmanager-nightly-1.2b2/lib/metrics/fid.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2182 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/lib/metrics/iou.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4000 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/lib/metrics/metric.py
--rw-r--r--   0 kisonho    (501) staff       (20)     9401 2023-04-04 16:43:13.000000 torchmanager-nightly-1.2b2/lib/testing.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.424806 torchmanager-nightly-1.2b2/lib/train/
--rw-r--r--   0 kisonho    (501) staff       (20)      164 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/lib/train/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4964 2023-03-19 20:02:58.000000 torchmanager-nightly-1.2b2/lib/train/checkpoint.py
--rw-r--r--   0 kisonho    (501) staff       (20)      694 2023-04-04 16:43:23.000000 torchmanager-nightly-1.2b2/lib/train/learning_rate.py
--rw-r--r--   0 kisonho    (501) staff       (20)    14893 2023-04-04 16:43:13.000000 torchmanager-nightly-1.2b2/lib/training.py
--rw-r--r--   0 kisonho    (501) staff       (20)       38 2023-04-07 17:36:34.429296 torchmanager-nightly-1.2b2/setup.cfg
--rw-r--r--   0 kisonho    (501) staff       (20)     1646 2023-04-07 17:36:26.000000 torchmanager-nightly-1.2b2/setup.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.425520 torchmanager-nightly-1.2b2/tests/
--rw-r--r--   0 kisonho    (501) staff       (20)      646 2023-04-07 16:18:37.000000 torchmanager-nightly-1.2b2/tests/test_0102.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-07 17:36:34.428100 torchmanager-nightly-1.2b2/torchmanager_nightly.egg-info/
--rw-r--r--   0 kisonho    (501) staff       (20)     2117 2023-04-07 17:36:34.000000 torchmanager-nightly-1.2b2/torchmanager_nightly.egg-info/PKG-INFO
--rw-r--r--   0 kisonho    (501) staff       (20)     1297 2023-04-07 17:36:34.000000 torchmanager-nightly-1.2b2/torchmanager_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 kisonho    (501) staff       (20)        1 2023-04-07 17:36:34.000000 torchmanager-nightly-1.2b2/torchmanager_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 kisonho    (501) staff       (20)       11 2023-04-07 17:36:34.000000 torchmanager-nightly-1.2b2/torchmanager_nightly.egg-info/requires.txt
--rw-r--r--   0 kisonho    (501) staff       (20)       31 2023-04-07 17:36:34.000000 torchmanager-nightly-1.2b2/torchmanager_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.935850 torchmanager-nightly-1.2b3/
+-rw-r--r--   0 kisonho    (501) staff       (20)     1318 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/LICENSE
+-rw-r--r--   0 kisonho    (501) staff       (20)     2117 2023-04-21 19:23:59.935405 torchmanager-nightly-1.2b3/PKG-INFO
+-rw-r--r--   0 kisonho    (501) staff       (20)     1806 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/README.md
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.908933 torchmanager-nightly-1.2b3/core/
+-rw-r--r--   0 kisonho    (501) staff       (20)      466 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/core/__init__.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.910516 torchmanager-nightly-1.2b3/core/devices/
+-rw-r--r--   0 kisonho    (501) staff       (20)      109 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/core/devices/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4879 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/core/devices/device.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      264 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/core/devices/protocols.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.911953 torchmanager-nightly-1.2b3/core/errors/
+-rw-r--r--   0 kisonho    (501) staff       (20)      153 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/core/errors/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      350 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/core/errors/runtime.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      669 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/core/errors/train.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2731 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/core/protocols.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.912869 torchmanager-nightly-1.2b3/core/random/
+-rw-r--r--   0 kisonho    (501) staff       (20)       44 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/core/random/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      879 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/core/random/seed.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      204 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/core/typing.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     5137 2023-04-21 19:20:06.000000 torchmanager-nightly-1.2b3/core/version.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.913781 torchmanager-nightly-1.2b3/core/view/
+-rw-r--r--   0 kisonho    (501) staff       (20)      439 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/core/view/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      313 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/core/view/protocols.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.916104 torchmanager-nightly-1.2b3/lib/
+-rw-r--r--   0 kisonho    (501) staff       (20)      290 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)    10862 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/basic.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.920290 torchmanager-nightly-1.2b3/lib/callbacks/
+-rw-r--r--   0 kisonho    (501) staff       (20)      658 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/callbacks/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4255 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/callbacks/callback.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4542 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/callbacks/ckpt.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     3523 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/callbacks/dynamic.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     1608 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/callbacks/early_stop.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4611 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/callbacks/experiment.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2224 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/callbacks/lr.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2440 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/callbacks/tensorboard.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      963 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/compatibility.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.921335 torchmanager-nightly-1.2b3/lib/configs/
+-rw-r--r--   0 kisonho    (501) staff       (20)       26 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/configs/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2938 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/configs/basic.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.922882 torchmanager-nightly-1.2b3/lib/data/
+-rw-r--r--   0 kisonho    (501) staff       (20)       85 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/data/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     6872 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/data/dataset.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2238 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/data/sliding.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.925418 torchmanager-nightly-1.2b3/lib/losses/
+-rw-r--r--   0 kisonho    (501) staff       (20)      156 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/losses/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     5386 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/losses/cross_entropy.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     1047 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/losses/dice.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     5763 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/losses/loss.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     3117 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/losses/mse.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.928664 torchmanager-nightly-1.2b3/lib/metrics/
+-rw-r--r--   0 kisonho    (501) staff       (20)      332 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/metrics/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4033 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/metrics/accuracy.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     3678 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/metrics/conf_met.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     5145 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/metrics/extractor.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2070 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/metrics/iou.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4003 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/metrics/metric.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     9661 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/testing.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.930436 torchmanager-nightly-1.2b3/lib/train/
+-rw-r--r--   0 kisonho    (501) staff       (20)       96 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/train/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4964 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/train/checkpoint.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      694 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/train/learning_rate.py
+-rw-r--r--   0 kisonho    (501) staff       (20)    14613 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/lib/training.py
+-rw-r--r--   0 kisonho    (501) staff       (20)       38 2023-04-21 19:23:59.935987 torchmanager-nightly-1.2b3/setup.cfg
+-rw-r--r--   0 kisonho    (501) staff       (20)     1558 2023-04-21 19:19:57.000000 torchmanager-nightly-1.2b3/setup.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.932147 torchmanager-nightly-1.2b3/tests/
+-rw-r--r--   0 kisonho    (501) staff       (20)     1203 2023-04-17 18:56:25.000000 torchmanager-nightly-1.2b3/tests/test_0101.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      934 2023-04-17 15:45:19.000000 torchmanager-nightly-1.2b3/tests/test_0102.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      263 2023-04-17 15:33:18.000000 torchmanager-nightly-1.2b3/tests/test_base.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-04-21 19:23:59.934652 torchmanager-nightly-1.2b3/torchmanager_nightly.egg-info/
+-rw-r--r--   0 kisonho    (501) staff       (20)     2117 2023-04-21 19:23:59.000000 torchmanager-nightly-1.2b3/torchmanager_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 kisonho    (501) staff       (20)     1308 2023-04-21 19:23:59.000000 torchmanager-nightly-1.2b3/torchmanager_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 kisonho    (501) staff       (20)        1 2023-04-21 19:23:59.000000 torchmanager-nightly-1.2b3/torchmanager_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 kisonho    (501) staff       (20)       11 2023-04-21 19:23:59.000000 torchmanager-nightly-1.2b3/torchmanager_nightly.egg-info/requires.txt
+-rw-r--r--   0 kisonho    (501) staff       (20)       31 2023-04-21 19:23:59.000000 torchmanager-nightly-1.2b3/torchmanager_nightly.egg-info/top_level.txt
```

### Comparing `torchmanager-nightly-1.2b2/LICENSE` & `torchmanager-nightly-1.2b3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager-nightly-1.2b2/PKG-INFO` & `torchmanager-nightly-1.2b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torchmanager-nightly
-Version: 1.2b2
-Summary: PyTorch Training Manager v1.2 (Beta 2)
+Version: 1.2b3
+Summary: PyTorch Training Manager v1.2 (Beta 3)
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Kison Ho
 Author-email: unfit-gothic.0q@icloud.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `torchmanager-nightly-1.2b2/README.md` & `torchmanager-nightly-1.2b3/README.md`

 * *Files identical despite different names*

### Comparing `torchmanager-nightly-1.2b2/core/devices/device.py` & `torchmanager-nightly-1.2b3/core/devices/device.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 except:
     DEFAULT = CPU
     GPU = NotImplemented
     GPUS = []
 
 Module = TypeVar('Module', bound=torch.nn.Module)
 
-def data_parallel(raw_model: Module, devices: List[torch.device] = GPUS, output_device: Optional[torch.device] = None, parallel_type: Type = torch.nn.parallel.DataParallel) -> Tuple[Union[Module, torch.nn.parallel.DataParallel], bool]:
+def data_parallel(raw_model: Module, /, devices: List[torch.device] = GPUS, *, output_device: Optional[torch.device] = None, parallel_type: Type = torch.nn.parallel.DataParallel) -> Tuple[Union[Module, torch.nn.parallel.DataParallel], bool]:
     """
     Make a `torch.nn.Module` data parallel
 
     - Parameters:
         - raw_model: A target `torch.nn.Module`
         - devices: A `list` of target `torch.device`
         - output_device: An optional `torch.device` of the target output device for the paralleled model
@@ -71,20 +71,20 @@
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
 
-def move_to_device(target: Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]], device: torch.device, recursive: bool = False) -> Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]]:
+def move_to_device(target: Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]], /, device: torch.device, *, recursive: bool = False) -> Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]]:
     """
     Recurrently move a target variable to device if elements perform to `DeviceMovable` protocol
     
     - Parameters:
         - target: Either a target in `DeviceMovable`, a `dict` of targets in `DeviceMovable`, or a `list` of targets in `DeviceMovable`, targets in a `list` or `dict` that does not perform to `DeviceMovable` protocol will be returned without changing
         - device: A `torch.device` of target device
         - recursive: A `bool` flag of if move to device recursively
```

### Comparing `torchmanager-nightly-1.2b2/core/errors/train.py` & `torchmanager-nightly-1.2b3/core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager-nightly-1.2b2/core/protocols.py` & `torchmanager-nightly-1.2b3/core/protocols.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     model: torch.nn.Module
 
 
 class StateDictLoadable(Protocol):
     """An object that can load state dict"""
 
     @abc.abstractmethod
-    def load_state_dict(self, state_dict: OrderedDict[str, Any], strict: bool = True) -> Any:
+    def load_state_dict(self, *, state_dict: OrderedDict[str, Any], strict: bool = True) -> Any:
         return NotImplemented
 
     @abc.abstractmethod
     def state_dict(self, *, prefix: str = "", keep_vars: bool = False) -> Dict[str, Any]:
         return NotImplemented
```

### Comparing `torchmanager-nightly-1.2b2/core/random/seed.py` & `torchmanager-nightly-1.2b3/core/random/seed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np, random, torch
 
 from .. import devices
 
-def freeze_seed(seed: int) -> None:
+def freeze_seed(seed: int, /) -> None:
     """
     Freeze random with given seed
 
     - Parameters:
         - seed: An `int` for the random seed
     """
     random.seed(seed)
```

### Comparing `torchmanager-nightly-1.2b2/lib/basic.py` & `torchmanager-nightly-1.2b3/lib/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from torchmanager_core import torch, _raise, API_VERSION, VERSION as CURRENT_VERSION
+from torchmanager_core import torch, Version, deprecated, _raise, API_VERSION, VERSION as CURRENT_VERSION
 from torchmanager_core.typing import Any, Collection, Dict, Generic, Module, Optional, OrderedDict, Self, Tuple, Union
 
 from .compatibility import convert
 from .losses import Loss, MultiLosses, ParallelLoss
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
@@ -106,14 +106,15 @@
         # initialize metrics
         for name, fn in metrics.items():
             self.metric_fns[name] = fn
 
         # initialize optimizer
         self.optimizer = optimizer
 
+    @deprecated('v1.3', 'v1.4')
     def compile(self, optimizer: torch.optim.Optimizer, loss_fn: Union[Loss, Dict[str, Loss]], metrics: Dict[str, Metric] = {}) -> None:
         """
         Recompiles the manager with optimizer loss function and metrics
 
         - Parameters:
             - loss_fn: A `Loss` object to calculate the loss for single loss or a `dict` of losses in `Loss` with their names in `str` to calculate multiple losses
             - metrics: A `dict` of metrics with a name in `str` and a `Metric` object to calculate the metric
```

### Comparing `torchmanager-nightly-1.2b2/lib/callbacks/callback.py` & `torchmanager-nightly-1.2b3/lib/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `torchmanager-nightly-1.2b2/lib/callbacks/ckpt.py` & `torchmanager-nightly-1.2b3/lib/callbacks/ckpt.py`

 * *Files identical despite different names*

### Comparing `torchmanager-nightly-1.2b2/lib/callbacks/dynamic.py` & `torchmanager-nightly-1.2b3/lib/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager-nightly-1.2b2/lib/callbacks/early_stop.py` & `torchmanager-nightly-1.2b3/lib/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `torchmanager-nightly-1.2b2/lib/callbacks/experiment.py` & `torchmanager-nightly-1.2b3/lib/callbacks/experiment.py`

 * *Files identical despite different names*

### Comparing `torchmanager-nightly-1.2b2/lib/callbacks/lr.py` & `torchmanager-nightly-1.2b3/lib/callbacks/lr.py`

 * *Files identical despite different names*

### Comparing `torchmanager-nightly-1.2b2/lib/callbacks/tensorboard.py` & `torchmanager-nightly-1.2b3/lib/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchmanager-nightly-1.2b2/lib/compatibility.py` & `torchmanager-nightly-1.2b3/lib/compatibility.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,28 @@
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
-    # convert from 1.0 (from_version = None)
-    if from_version is None and obj is not None:
+    # format version
+    v = Version(from_version) if from_version is not None else Version("v1.0")
+
+    # Return if None
+    if obj is None:
+        return obj
+
+    if v < Version("v1.1"): # convert from 1.0
         # convert KLDiv
         if isinstance(obj, KLDiv) and not hasattr(obj, "replace_nan"):
             obj.replace_nan = False
         elif isinstance(obj, KLDiv) and not hasattr(obj, "_t"):
             obj._t = None
 
         # convert Accuracy and MAE
```

### Comparing `torchmanager-nightly-1.2b2/lib/configs/basic.py` & `torchmanager-nightly-1.2b3/lib/configs/basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from torchmanager_core import argparse, abc, os, shutil, torch, view
 from torchmanager_core.typing import Any, Union
 from torchmanager_core import VERSION
 
 
-class Configs(argparse.Namespace):
+class Configs(argparse.Namespace, abc.ABC):
     """
     Basic Configurations
     
     * extends: `argparse.Namespace`
     * Abstract class
 
     - Properties:
@@ -33,16 +33,18 @@
         if len(arguments) > 0:
             configs = parser.parse_args(arguments, namespace=cls())
         else:
             configs = parser.parse_args(namespace=cls())
 
         # initialize logging
         log_dir = os.path.join("experiments", configs.experiment)
-        if configs.replace_experiment and os.path.exists(log_dir) and os.path.isdir(log_dir):
+        if os.path.exists(log_dir) and configs.replace_experiment:
             shutil.rmtree(log_dir)
+        elif os.path.exists(log_dir) and not configs.replace_experiment:
+            raise IOError(f"Path '{log_dir}' has already existed.")
         os.makedirs(log_dir, exist_ok=True)
         log_file = os.path.basename(configs.experiment.replace(".exp", ".log"))
         log_path = os.path.join(log_dir, log_file)
         view.set_log_path(log_path=log_path)
         configs.format_arguments()
 
         # show configs summarize
@@ -61,8 +63,8 @@
         return parser
     
     def show_environments(self) -> None:
         view.logger.info(f"torch={torch.__version__}, torchmanager={VERSION}")
     
     @abc.abstractmethod
     def show_settings(self) -> None:
-        raise NotImplementedError
+        pass
```

### Comparing `torchmanager-nightly-1.2b2/lib/data/dataset.py` & `torchmanager-nightly-1.2b3/lib/data/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     @property
     def batched_len(self) -> int:
         if self.drop_last:
             return int(self.unbatched_len / self.batch_size)
         else:
             return math.ceil(self.unbatched_len / self.batch_size)
 
-    def __init__(self, batch_size: int, device: torch.device = devices.CPU, drop_last: bool = False, shuffle: bool = False) -> None:
+    def __init__(self, batch_size: int, /, *, device: torch.device = devices.CPU, drop_last: bool = False, shuffle: bool = False) -> None:
         """
         Constructor
 
         - Parameters:
             - batch_size: An `int` of batch size for the current dataset
             - device: A `torch.device` for the data to be pinned during iteration
             - drop_last: A `bool` flag of if drop the last data that not enought for the batch size
```

### Comparing `torchmanager-nightly-1.2b2/lib/data/utils/sliding.py` & `torchmanager-nightly-1.2b3/lib/data/sliding.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,49 @@
 from itertools import product
 from torchmanager_core import torch, _raise
 from torchmanager_core.typing import List, Tuple
 
-def sliding_window(image: torch.Tensor, window_size: Tuple[int, ...], stride: Tuple[int, ...]) -> torch.Tensor:
+def sliding_window(image: torch.Tensor, /, window_size: Tuple[int, ...], stride: Tuple[int, ...]) -> torch.Tensor:
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

### Comparing `torchmanager-nightly-1.2b2/lib/losses/cross_entropy.py` & `torchmanager-nightly-1.2b3/lib/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager-nightly-1.2b2/lib/losses/dice.py` & `torchmanager-nightly-1.2b3/lib/losses/dice.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     The dice loss
 
     * extends: `.loss.Loss`
     """
     _smooth: int
     _softmax_input: bool
 
-    def __init__(self, smooth: int = 1, softmax_input: bool = True, **kwargs: Any) -> None:
+    def __init__(self, smooth: int = 1, *, softmax_input: bool = True, **kwargs: Any) -> None:
         """
         Constructor
 
         - Parameters:
             - smooth: An `int` of smooth value to avoid dividing zero
             - softmax_input: A `bool` flag of if softmax the input
         """
```

### Comparing `torchmanager-nightly-1.2b2/lib/losses/loss.py` & `torchmanager-nightly-1.2b3/lib/losses/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         return self.__weight
 
     @weight.setter
     def weight(self, w: float) -> None:
         assert w >= 0, f"Weight must be a non-negative number, got {w}."
         self.__weight = w
 
-    def __init__(self, loss_fn: Optional[Callable[[Any, Any], torch.Tensor]] = None, target: Optional[str] = None, weight: float = 1) -> None:
+    def __init__(self, loss_fn: Optional[Callable[[Any, Any], torch.Tensor]] = None, *, target: Optional[str] = None, weight: float = 1) -> None:
         """
         Constructor
 
         - Parameters:
             - loss_fn: An optional `Callable` function that accepts input or `y_pred` in `Any` kind and target or `y_true` in `Any` kind as inputs and gives a loss in `torch.Tensor`
             - target: An optional `str` of target name in `input` and `target` during direct calling
             - weight: A `float` of the loss weight
@@ -80,15 +80,15 @@
 
     __losses: torch.nn.ModuleList
 
     @property
     def losses(self) -> torch.nn.ModuleList:
         return self.__losses
 
-    def __init__(self, losses: List[Loss], target: Optional[str] = None, weight: float = 1) -> None:
+    def __init__(self, losses: List[Loss], *, target: Optional[str] = None, weight: float = 1) -> None:
         """
         Constructor
 
         - Parameters:
             - losses: A `list` of `Loss` function
             - target: An optional `str` of target name in `input` and `target` during direct calling
             - weight: A `float` of the loss weight
```

### Comparing `torchmanager-nightly-1.2b2/lib/losses/mse.py` & `torchmanager-nightly-1.2b3/lib/losses/mse.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     - Properties:
         - reduction: A `.loss.Reduction` of reduction method
         - replace_nan: A `boolean` flag of if replacing nan results to zeros
     """
     reduction: Reduction
     replace_nan: bool
 
-    def __init__(self, loss_fn: Optional[Callable[[Any, Any], torch.Tensor]] = None, reduction: Reduction = Reduction.MEAN, replace_nan: bool = False, target: Optional[str] = None, weight: float = 1) -> None:
+    def __init__(self, loss_fn: Optional[Callable[[Any, Any], torch.Tensor]] = None, *, reduction: Reduction = Reduction.MEAN, replace_nan: bool = False, target: Optional[str] = None, weight: float = 1) -> None:
         """
         Constructor
 
         - Parameters:
             - reduction: A `.loss.Reduction` of reduction method
             - replace_nan: A `boolean` flag of if replacing nan results to zeros
             - target: An optional `str` of target name in `input` and `target` during direct calling
@@ -47,15 +47,15 @@
             return loss
 
 
 class MAE(_ReductableLoss):
     """
     The MSE loss
     """
-    def __init__(self, reduction: Reduction = Reduction.MEAN, replace_nan: bool = False, target: Optional[str] = None, weight: float = 1) -> None:
+    def __init__(self, *, reduction: Reduction = Reduction.MEAN, replace_nan: bool = False, target: Optional[str] = None, weight: float = 1) -> None:
         """
         Constructor
 
         - Parameters:
             - reduction: A `.loss.Reduction` of reduction method
             - replace_nan: A `boolean` flag of if replacing nan results to zeros
             - target: An optional `str` of target name in `input` and `target` during direct calling
@@ -65,15 +65,15 @@
         super().__init__(l1, reduction=reduction, replace_nan=replace_nan, target=target, weight=weight)
 
 
 class MSE(_ReductableLoss):
     """
     The MSE loss
     """
-    def __init__(self, reduction: Reduction = Reduction.MEAN, replace_nan: bool = False, target: Optional[str] = None, weight: float = 1) -> None:
+    def __init__(self, *, reduction: Reduction = Reduction.MEAN, replace_nan: bool = False, target: Optional[str] = None, weight: float = 1) -> None:
         """
         Constructor
 
         - Parameters:
             - reduction: A `.loss.Reduction` of reduction method
             - replace_nan: A `boolean` flag of if replacing nan results to zeros
             - target: An optional `str` of target name in `input` and `target` during direct calling
```

### Comparing `torchmanager-nightly-1.2b2/lib/metrics/accuracy.py` & `torchmanager-nightly-1.2b3/lib/metrics/accuracy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from torchmanager_core import torch, deprecated
-from torchmanager_core.typing import Optional
+from torchmanager_core import torch
+from torchmanager_core.typing import Optional, Tuple
 
+from .conf_met import BinaryConfusionMetric
 from .metric import Metric, Reduction
 
 
 class Accuracy(Metric):
     """
     The traditional accuracy metric to compare two `torch.Tensor`
 
     * extends: `.metric.Metric`
     """
     reduction: Reduction
 
-    def __init__(self, reduction: Reduction = Reduction.MEAN, target: Optional[str] = None) -> None:
+    def __init__(self, *, reduction: Reduction = Reduction.MEAN, target: Optional[str] = None) -> None:
         super().__init__(target=target)
         self.reduction = reduction
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         if self.reduction == Reduction.MEAN:
             return input.eq(target).to(torch.float32).mean()
         elif self.reduction == Reduction.SUM:
@@ -26,23 +27,22 @@
 
 
 class SparseCategoricalAccuracy(Accuracy):
     """
     The accuracy metric for normal integer labels
 
     * extends: `Accuracy`
-    * [Deprecation Warning]: The property `dim` has been deprecated from v1.1.0, and no longer be available in v1.2.0
 
     - Properties:
         - dim: An `int` of the probability dim index for the input
     """
 
     _dim: int
 
-    def __init__(self, dim: int = -1, target: Optional[str] = None) -> None:
+    def __init__(self, dim: int = -1, *, target: Optional[str] = None) -> None:
         """
         Constructor
 
         - Parameters:
             - dim: An `int` of the classification dimension
             - target: A `str` of target name in `input` and `target` during direct calling
         """
@@ -62,26 +62,45 @@
     """
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         target = target.argmax(dim=self._dim)
         return super().forward(input, target)
 
 
+class F1(BinaryConfusionMetric):
+    """
+    The F1 metrics
+    """
+
+    def forward(self, input: Tuple[torch.Tensor, torch.Tensor, torch.Tensor], target: torch.Tensor) -> torch.Tensor:
+        # extract input
+        tp, fp, fn = input
+
+        # calculate precision and recall
+        precision = tp / (tp + fp + self._eps)
+        recall = tp / (tp + fn + self._eps)
+
+        # calculate F1
+        f1 = 2 * precision * recall / (precision + recall + self._eps)
+        f1 = torch.mean(f1)
+        return f1
+
+
 class MAE(Metric):
     """
     The Mean Absolute Error metric
 
     * extends: `.metrics.Metric`
 
     - Properties:
         - reduction: A `.loss.Reduction` of reduction method
     """
     reduction: Reduction
 
-    def __init__(self, reduction: Reduction = Reduction.MEAN, target: Optional[str] = None) -> None:
+    def __init__(self, *, reduction: Reduction = Reduction.MEAN, target: Optional[str] = None) -> None:
         """
         Constructor
 
         - Parameters:
             - reduction: A `.loss.Reduction` of reduction method
             - target: An optional `str` of target name in `input` and `target` during direct calling
         """
@@ -96,7 +115,27 @@
         # error reduction
         if self.reduction == Reduction.MEAN:
             return error.mean()
         elif self.reduction == Reduction.SUM:
             return error.sum()
         else:
             return error
+
+
+class Precision(BinaryConfusionMetric):
+    """
+    The Precision metrics
+    """
+
+    def forward(self, input: Tuple[torch.Tensor, torch.Tensor, torch.Tensor], target: torch.Tensor) -> torch.Tensor:
+        tp, fp, _ = input
+        return tp / (tp + fp + self._eps)
+
+
+class Recall(BinaryConfusionMetric):
+    """
+    The Recall metrics
+    """
+
+    def forward(self, input: Tuple[torch.Tensor, torch.Tensor, torch.Tensor], target: torch.Tensor) -> torch.Tensor:
+        tp, _, fn = input
+        return tp / (tp + fn + self._eps)
```

### Comparing `torchmanager-nightly-1.2b2/lib/metrics/fid.py` & `torchmanager-nightly-1.2b3/lib/metrics/extractor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,49 @@
-from torchmanager_core import torch, view
-from torchmanager_core.typing import Generic, List, Module, Optional
+from torchmanager_core import torch, view, _raise
+from torchmanager_core.typing import Any, Callable, Generic, List, Module, Optional
 
 from .metric import Metric
 
+try:
+    from scipy import linalg  # type: ignore
+except ImportError:
+    linalg = NotImplemented
 
-class FID(Metric, Generic[Module]):
+
+class FeatureMetric(Metric, Generic[Module]):
     """
-    Fréchet Inception Distance (FID) metric
+    A metric that extracts inputs and targets with feature extractor and evaluates the extracted features instead of raw inputs
 
     * Extends: `.metric.Metric`
     * Generic class of `Module`
 
     - Parameters:
         - feature_extractor: A `Module` to extract the features
-        - input_features: A `list` of current features for generated images that extracted in `torch.Tensor`
-        - result: A `torch.Tensor` of the current FID result
-        - return_when_forwarding: A `bool` flag of if returning results when calculating the metrics, a `torch.nan` will be returned if set to `False` during forwarding
-        - target_features: A `list` of current features for real images that extracted in `torch.Tensor`
     """
     feature_extractor: Optional[Module]
     """A `Module` to extract the features"""
-    input_features: List[torch.Tensor]
-    """A `list` of current features for generated images that extracted in `torch.Tensor`"""
-    return_when_forwarding: bool
-    """A `bool` flag of if returning results when calculating the metrics, a `torch.nan` will be returned if set to `False` during forwarding"""
-    target_features: List[torch.Tensor]
-    """A `list` of current features for real images that extracted in `torch.Tensor`"""
-
-    @property
-    def result(self) -> torch.Tensor:
-        """A `torch.Tensor` of the current FID result"""
-        # concat input and target
-        input = torch.cat(self.input_features)
-        target = torch.cat(self.target_features)
-
-        # calculate mean and covariance
-        mu_real = target.mean(0)
-        mu_gen = input.mean(0)
-        sigma_real = target.cov() / (target.shape[0] - 1)
-        sigma_gen = input.cov() / (input.shape[0] - 1)
-        sigma = sigma_real @ sigma_gen
-        diff = mu_real - mu_gen
-
-        # square root of sigma
-        try:
-            from scipy import linalg
-            covmean = linalg.sqrtm(sigma)
-            assert not isinstance(covmean, tuple), "The square root of `sigma` should not contain errest number."
-            sigma = torch.from_numpy(covmean.real).to(sigma.device)
-        except ImportError:
-            view.warnings.warn("The `scipy` package is not installed to calculate matrix square root. The matrix square root will be calculated as an element-wise square root, which may result in different calculation results than the actual matrix square root.")
-            sigma = sigma.sqrt()
-
-        # Calculate the squared Euclidean distance between the means
-        return diff @ diff + torch.trace(sigma_real + sigma_gen - 2 * sigma)
 
-    def __init__(self, feature_extractor: Optional[Module] = None, return_when_forwarding: bool = True, target: Optional[str] = None) -> None:
+    def __init__(self, metric_fn: Optional[Callable[[Any, Any], torch.Tensor]] = None, feature_extractor: Optional[Module] = None, *, target: Optional[str] = None) -> None:
         """
         Constructor
 
         - Parameters:
             - feature_extractor: An optional `Module` to extract features, a pre-trained InceptionV3 will be used if not given
-            - return_when_forwarding: A `bool` flag of if returning results when calculating the metrics, a `torch.nan` will be returned if set to `False` during forwarding
             - target: A `str` of target name in `input` and `target` during direct calling
         """
-        super().__init__(target=target)
+        super().__init__(metric_fn, target=target)
         self.feature_extractor = feature_extractor
-        self.input_features = []
-        self.return_when_forwarding = return_when_forwarding
-        self.target_features = []
 
-    def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
+    def __call__(self, input: Any, target: Any) -> torch.Tensor:
         input_features = self.forward_features(input)
         target_features = self.forward_features(target)
-        self.input_features += [input_features.cpu().detach()]
-        self.target_features += [target_features.cpu().detach()]
-        return self.result if self.return_when_forwarding else torch.tensor(torch.nan)
+        return super().__call__(input_features, target_features)
 
     @torch.no_grad()
-    def forward_features(self, x: torch.Tensor) -> torch.Tensor:
+    def forward_features(self, x: torch.Tensor, /) -> torch.Tensor:
         """
         Extract features
 
         - Parameters:
             - x: A `torch.Tensor` to extract
         - Returns: A `torch.Tensor` of features if feature extractor is given
         """
@@ -92,11 +53,75 @@
         else:
             return x
 
     def train(self, mode: bool = True):
         self.training = mode
         return self
 
+
+class ExtractorScore(FeatureMetric[Module]):
+    """
+    A general feature score metric which can be used as `InceptionScore` by taking the `feature_extractor` as an InceptionV3 model
+
+    * Extends: `FeatureExtractorMetric`
+    * Generic class of `Module`
+    * When forwarding this metric, `target` (real images) parameter is not required
+    """
+
+    def __call__(self, input: Any, target: Any = None) -> torch.Tensor:
+        input_features = self.forward_features(input)
+        return super().__call__(input_features, target)
+
+    def forward(self, input: torch.Tensor, **kwargs: Any) -> torch.Tensor:
+        scores = input.softmax(1).mean(0)
+        scores = scores * (scores / scores.mean()).log2()
+        scores = torch.exp(scores.sum())
+        return scores
+
+
+class FID(FeatureMetric[Module]):
+    """
+    Fréchet Inception Distance (FID) metric
+
+    * Extends: `FeatureExtractorMetric`
+    * Generic class of `Module`
+    """
+    use_linalg: bool
+    """use_linalg: A `bool` flag of if use `scipy.linalg` package"""
+
+    def __init__(self, feature_extractor: Optional[Module] = None, *, use_linalg: bool = True, target: Optional[str] = None) -> None:
+        """
+        Constructor
+
+        - Parameters:
+            - feature_extractor: An optional `Module` to extract features, a pre-trained InceptionV3 will be used if not given
+            - return_when_forwarding: A `bool` flag of if returning results when calculating the metrics, a `torch.nan` will be returned if set to `False` during forwarding
+            - target: A `str` of target name in `input` and `target` during direct calling
+            - use_linalg: A `bool` flag of if use `scipy.linalg` package
+        """
+        super().__init__(feature_extractor=feature_extractor, target=target)
+        self.use_linalg = use_linalg
+
+    def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
+        # calculate mean and covariance
+        mu_real = target.mean(0)
+        mu_gen = input.mean(0)
+        sigma_real = target.cov() / (target.shape[0] - 1)
+        sigma_gen = input.cov() / (input.shape[0] - 1)
+        diff = mu_real - mu_gen
+
+        # square root of sigma
+        if linalg is NotImplemented or not self.use_linalg:
+            view.warnings.warn("The `scipy` package is not installed to calculate matrix square root or `use_linalg` is set to `False`. The matrix times and square root of sigma will be calculated element-wisely, which may result in different calculation results than the actual matrix square root.")
+            sigma = sigma_real * sigma_gen
+            sigma = sigma.sqrt()
+        else:
+            sigma = sigma_real @ sigma_gen
+            covmean = linalg.sqrtm(sigma.cpu().numpy())
+            assert not isinstance(covmean, tuple), _raise(TypeError("The square root of `covmean` should not contain errest number."))
+            sigma = torch.from_numpy(covmean.real).to(sigma.device)
+
+        # Calculate the squared Euclidean distance between the means
+        return diff @ diff + torch.trace(sigma_real + sigma_gen - 2 * sigma)
+
     def reset(self) -> None:
         super().reset()
-        self.input_features.clear()
-        self.target_features.clear()
```

### Comparing `torchmanager-nightly-1.2b2/lib/metrics/iou.py` & `torchmanager-nightly-1.2b3/lib/metrics/iou.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,39 +8,35 @@
 class InstanceIoU(ConfusionMetrics):
     """
     The iIoU metric for segmentation
 
     * extends: `.conf_met.ConfusionMetrics`
     """
 
-    def __init__(self, num_classes: int, target: Optional[str] = None) -> None:
+    def __init__(self, num_classes: int, /, *, target: Optional[str] = None) -> None:
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
 
     * extends: `torch.nn.Module`
     * [Deprecation Warning]: The old `MIoU` metric in v1.0.3 calculates iIoU has been renamed to `InstanceIoU` in v1.1.0, and will be removed in v1.2.0.
     """
     _dim: int
     _smooth: float
     _threshold: float
 
-    def __init__(self, dim: int = 1, smooth: float = 1e-4, threshold: float = 0, target: Optional[str] = None) -> None:
+    def __init__(self, dim: int = 1, smooth: float = 1e-4, threshold: float = 0, *, target: Optional[str] = None) -> None:
         """
         Constructor
 
         - Parameters:
             - dim: An `int` of class dimension
             - smooth: A `float` of smooth value to avoid zero devision
         """
```

### Comparing `torchmanager-nightly-1.2b2/lib/metrics/metric.py` & `torchmanager-nightly-1.2b3/lib/metrics/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     @property
     def results(self) -> Optional[torch.Tensor]:
         if len(self._results) > 0:
             return torch.concat(self._results)
         else:
             return None
 
-    def __init__(self, metric_fn: Optional[Callable[[Any, Any], torch.Tensor]] = None, target: Optional[str] = None) -> None:
+    def __init__(self, metric_fn: Optional[Callable[[Any, Any], torch.Tensor]] = None, *, target: Optional[str] = None) -> None:
         """
         Constructor
 
         - Parameters:
             - metric_fn: An optional `Callable` metrics function that accepts `Any` kind of prediction input and target and returns a metric `torch.Tensor`. A `call` method must be overriden if this parameter is set as `None`.
             - target: A `str` of target name in `input` and `target` during direct calling
         """
```

### Comparing `torchmanager-nightly-1.2b2/lib/testing.py` & `torchmanager-nightly-1.2b3/lib/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,26 @@
     """
     model: Union[Module, torch.nn.parallel.DataParallel]
 
     @property
     def compiled_metrics(self) -> Dict[str, Resulting]:
         return {name: m for name, m in self.metric_fns.items() if "loss" not in name}
 
+    def forward(self, x_train: Any) -> Any:
+        """
+        Forward pass function
+
+        - Parameters:
+            - x_train: The training data
+        - Returns: `Any` kind of model output
+        """
+        return self.model(x_train)
+
     @torch.no_grad()
-    def predict(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection[Any]], device: Optional[Union[torch.device, List[torch.device]]] = None, use_multi_gpus: bool = False, show_verbose: bool = False) -> List[Any]:
+    def predict(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection[Any]], /, *, device: Optional[Union[torch.device, List[torch.device]]] = None, use_multi_gpus: bool = False, show_verbose: bool = False) -> List[Any]:
         '''
         Predict the whole dataset
 
         - Parameters:
             - dataset: A `torch.utils.data.DataLoader` dataset to predict
             - device: An optional `torch.device` to test on if not using multi-GPUs or an optional default `torch.device` for testing otherwise
             - use_multi_gpus: A `bool` flag to use multi gpus during testing
@@ -67,15 +77,15 @@
             self.to(device)
 
             # loop the dataset
             for data in dataset:
                 x, _ = self.unpack_data(data)
                 if use_multi_gpus is not True:
                     x = devices.move_to_device(x, device)
-                y = self.model(x)
+                y = self.forward(x)
                 predictions.append(y)
                 if progress_bar is not None:
                     progress_bar.update()
 
             # reset model and loss
             return predictions
         except KeyboardInterrupt:
@@ -91,15 +101,15 @@
                 progress_bar.close()
 
             # empty cache
             self.model = self.raw_model.to(cpu)
             devices.empty_cache()
 
     @torch.no_grad()
-    def test(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection[Any]], device: Optional[Union[torch.device, List[torch.device]]] = None, empty_cache: bool = True, use_multi_gpus: bool = False, show_verbose: bool = False) -> Dict[str, float]:
+    def test(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection[Any]],  /, *,device: Optional[Union[torch.device, List[torch.device]]] = None, empty_cache: bool = True, use_multi_gpus: bool = False, show_verbose: bool = False) -> Dict[str, float]:
         """
         Test target model
 
         - Parameters:
             - dataset: A `torch.utils.data.DataLoader` or `.data.Dataset` dataset
             - device: An optional `torch.device` to test on if not using multi-GPUs or an optional default `torch.device` for testing otherwise
             - empyt_cache: A `bool` flag to empty cache after testing
@@ -203,15 +213,15 @@
             - y_train: The testing label in `torch.Tensor`
         - Returns: A `dict` of validation summary
         """
         # initialize
         summary: Dict[str, float] = {}
 
         # forward pass
-        y = self.model(x_test)
+        y = self.forward(x_test)
 
         # forward metrics
         for name, fn in self.compiled_metrics.items():
             if name.startswith("val_"):
                 name = name.replace("val_", "")
             elif "loss" in name:
                 continue
```

### Comparing `torchmanager-nightly-1.2b2/lib/train/checkpoint.py` & `torchmanager-nightly-1.2b3/lib/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchmanager-nightly-1.2b2/lib/train/learning_rate.py` & `torchmanager-nightly-1.2b3/lib/train/learning_rate.py`

 * *Files identical despite different names*

### Comparing `torchmanager-nightly-1.2b2/lib/training.py` & `torchmanager-nightly-1.2b3/lib/training.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from torch.utils.data import DataLoader
 from torchmanager_core import devices, errors, math, torch, view
 from torchmanager_core.protocols import Resulting
-from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Self, Union
+from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Self, Tuple, Union
 
 from .callbacks import Callback
 from .data import Dataset
 from .losses import Loss, ParallelLoss
 from .metrics import Metric
-from .train import Checkpoint, update_lr
+from .train import Checkpoint
 from .testing import Manager as _Manager
 
 
 class Manager(_Manager[Module]):
     """
     A training manager
 
@@ -51,15 +51,15 @@
         assert self.optimizer is not None, errors._raise(NotImplementedError("The manager is not compiled properly, `optimizer` is missing."))
         return self.optimizer
 
     def __init__(self, model: Module, optimizer: Optional[torch.optim.Optimizer] = None, loss_fn: Optional[Union[Loss, Dict[str, Loss]]] = None, metrics: Dict[str, Metric] = {}) -> None:
         super().__init__(model, optimizer, loss_fn, metrics)
         self.__current_epoch = 0
 
-    def _train(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection], iterations: Optional[int] = None, device: torch.device = devices.CPU, use_multi_gpus: bool = False, show_verbose: bool = False, verbose_type: view.VerboseType = view.VerboseType.ALL, callbacks_list: List[Callback] = []) -> Dict[str, float]:
+    def _train(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection], /, iterations: Optional[int] = None, *, device: torch.device = devices.CPU, use_multi_gpus: bool = False, show_verbose: bool = False, verbose_type: view.VerboseType = view.VerboseType.ALL, callbacks_list: List[Callback] = []) -> Dict[str, float]:
         """
         The single training step for an epoch
 
         - Parameters:
             - dataset: A `torch.utils.data.DataLoader` or `.data.Dataset` training dataset
             - iterations: An optional `int` of total training iterations, must be smaller than the size of dataset
             - device: A `torch.device` where the data is moved to, should be same as the model
@@ -130,27 +130,35 @@
                 progress_bar.close()
 
         # summarize
         summary = {name: float(fn.result.detach()) for name, fn in self.metric_fns.items() if not name.startswith("val_")}
         summary["loss"] = float(self.compiled_losses.result.detach())
         return summary
 
-    def fit(self, training_dataset: Union[DataLoader[Any], Dataset[Any], Collection], epochs: Optional[int] = None, iterations: Optional[int] = None, initial_epoch: Optional[int] = None, lr_scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None, val_dataset: Optional[Union[DataLoader[Any], Dataset[Any], Collection]] = None, device: Optional[Union[torch.device, List[torch.device]]] = None, use_multi_gpus: bool = False, callbacks_list: List[Callback] = [], **kwargs) -> Module:
+    def backward(self, loss: torch.Tensor) -> None:
+        """
+        Backward function to calculate the gradients
+        
+        - Parameters:
+            - loss: A `torch.Tensor` of loss value
+        """
+        loss.backward()
+
+    def fit(self, training_dataset: Union[DataLoader[Any], Dataset[Any], Collection], /, epochs: Optional[int] = None, val_dataset: Optional[Union[DataLoader[Any], Dataset[Any], Collection]] = None, callbacks_list: List[Callback] = [], *, iterations: Optional[int] = None, initial_epoch: Optional[int] = None, device: Optional[Union[torch.device, List[torch.device]]] = None, use_multi_gpus: bool = False, **kwargs) -> Module:
         """
         Training algorithm
 
         - Parameters:
             - training_dataset: Any kind of training dataset in `torch.utils.data.DataLoader` or `.data.Dataset`
-            - epochs: An optional `int` number of training epochs
-            - iterations: An optional `int` number of training iterations
-            - lr_scheduelr: An optioanl `torch.optim.lr_scheduler._LRScheduler` to update the lr per epoch
+            - epochs: An optional `int` number of training epochs (`iterations` must be not given)
             - val_dataset: An optional validation `Any`
+            - callbacks_list: A `list` of callbacks in `Callback`
+            - iterations: An optional `int` number of training iterations (`epochs` must be not given)
             - device: An optional `torch.device` to test on if not using multi-GPUs or an optional default `torch.device` for testing otherwise
             - use_multi_gpus: A `bool` flag of if using multi gpus
-            - callbacks_list: A `list` of callbacks in `Callback`
             - **kwargs: Additional keyword arguments that will be passed to `train` method.
         - Returns: A trained `torch.nn.Module`
         """
         # arguments checking
         dataset_len = training_dataset.batched_len if isinstance(training_dataset, Dataset) else len(training_dataset)
         assert self.compiled is True, errors._raise(ValueError("Manager has not yet been compiled. Either loss_fn or optimizer, or both, are not given."))
         if epochs is not None:
@@ -173,16 +181,14 @@
             initial_epoch = self.current_epoch
 
         # initialize training
         cpu, device, target_devices = devices.search(device)
         if device == cpu and len(target_devices) < 2:
             use_multi_gpus = False
         devices.set_default(target_devices[0])
-        if lr_scheduler is not None:
-            view.warnings.warn("Parameter `lr_scheduler` has been deprecated after v1.1.0 and will be removed from v1.2.0, use `.callbacks.LrScheduler` callback instead.", DeprecationWarning)
         for c in callbacks_list:
             c.on_train_start(initial_epoch)
 
         try:
             # multi gpus support for model
             if use_multi_gpus and not isinstance(self.model, torch.nn.parallel.DataParallel):
                 model, use_multi_gpus = devices.data_parallel(self.model, devices=target_devices)
@@ -225,19 +231,14 @@
                         c.on_epoch_end(self.current_epoch, summary=summary, val_summary=val_summary)
                     except errors.StopTraining:
                         # on train end
                         for c in callbacks_list:
                             c.on_train_end(self.raw_model)
                         return self.raw_model
 
-                # step lr scheduler
-                if lr_scheduler is not None:
-                    lr_summary = update_lr(lr_scheduler)
-                    summary.update(lr_summary)
-
                 # print summary info
                 val_message = f"Epoch {self.current_epoch + 1}/{epochs}: "
                 summary.update({f"val_{name}": value for name, value in val_summary.items()})
                 for i, (name, value) in enumerate(summary.items()):
                     if i > 0:
                         val_message += ", "
                     val_message += f"{name}={value:.4f}"
@@ -266,25 +267,25 @@
         - Parameters:
             - x_train: The training data
             - y_train: The training label
         - Returns: A summary of `dict` with keys as `str` and values as `float`
         """
         # forward pass
         summary: Dict[str, float] = {}
-        y = self.model(x_train)
+        y = self.forward(x_train)
         loss = self.compiled_losses(y, y_train)
 
         # forward metrics
         for name, fn in self.compiled_metrics.items():
             if not name.startswith("val_") and "loss" not in name:
                 fn(y, y_train)
 
         # backward pass
         self.compiled_optimizer.zero_grad()
-        loss.backward()
+        self.backward(loss)
         self.compiled_optimizer.step()
 
         # summary result
         try:
             summary["loss"] = float(self.compiled_losses.result.detach())
         except Exception as e:
             raise errors.LossError() from e
```

### Comparing `torchmanager-nightly-1.2b2/setup.py` & `torchmanager-nightly-1.2b3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 from distutils.core import setup
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='torchmanager-nightly',
-    version="1.2b2",
-    description="PyTorch Training Manager v1.2 (Beta 2)",
+    version="1.2b3",
+    description="PyTorch Training Manager v1.2 (Beta 3)",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Kison Ho',
     author_email='unfit-gothic.0q@icloud.com',
     packages=[
         'torchmanager',
         'torchmanager.callbacks',
         'torchmanager.configs',
         'torchmanager.data',
-        'torchmanager.data.utils',
         'torchmanager.losses',
         'torchmanager.metrics',
         'torchmanager.train',
         'torchmanager_core',
         'torchmanager_core.devices',
         'torchmanager_core.errors',
         'torchmanager_core.random',
         'torchmanager_core.view',
     ],
     package_dir={
         'torchmanager': 'lib',
         'torchmanager.callbacks': 'lib/callbacks',
         'torchmanager.configs': 'lib/configs',
         'torchmanager.data': 'lib/data',
-        'torchmanager.data.utils': 'lib/data/utils',
         'torchmanager.losses': 'lib/losses',
         'torchmanager.metrics': 'lib/metrics',
         'torchmanager.train': 'lib/train',
         'torchmanager_core': 'core',
         'torchmanager_core.devices': 'core/devices',
         'torchmanager_core.errors': 'core/errors',
         'torchmanager_core.random': 'core/random',
```

### Comparing `torchmanager-nightly-1.2b2/torchmanager_nightly.egg-info/PKG-INFO` & `torchmanager-nightly-1.2b3/torchmanager_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torchmanager-nightly
-Version: 1.2b2
-Summary: PyTorch Training Manager v1.2 (Beta 2)
+Version: 1.2b3
+Summary: PyTorch Training Manager v1.2 (Beta 3)
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Kison Ho
 Author-email: unfit-gothic.0q@icloud.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `torchmanager-nightly-1.2b2/torchmanager_nightly.egg-info/SOURCES.txt` & `torchmanager-nightly-1.2b3/torchmanager_nightly.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,29 +28,30 @@
 lib/callbacks/experiment.py
 lib/callbacks/lr.py
 lib/callbacks/tensorboard.py
 lib/configs/__init__.py
 lib/configs/basic.py
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
-lib/metrics/fid.py
+lib/metrics/extractor.py
 lib/metrics/iou.py
 lib/metrics/metric.py
 lib/train/__init__.py
 lib/train/checkpoint.py
 lib/train/learning_rate.py
+tests/test_0101.py
 tests/test_0102.py
+tests/test_base.py
 torchmanager_nightly.egg-info/PKG-INFO
 torchmanager_nightly.egg-info/SOURCES.txt
 torchmanager_nightly.egg-info/dependency_links.txt
 torchmanager_nightly.egg-info/requires.txt
 torchmanager_nightly.egg-info/top_level.txt
```

