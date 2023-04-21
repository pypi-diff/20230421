# Comparing `tmp/antgo-0.1.0.tar.gz` & `tmp/antgo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antgo-0.1.0.tar", last modified: Fri Apr 14 06:35:03 2023, max compression
+gzip compressed data, was "antgo-0.1.1.tar", last modified: Fri Apr 21 08:48:21 2023, max compression
```

## Comparing `antgo-0.1.0.tar` & `antgo-0.1.1.tar`

### file list

```diff
@@ -1,922 +1,927 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.280702 antgo-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/LICENSE.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-04-14 06:32:18.000000 antgo-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-14 06:35:03.280702 antgo-0.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4480 2023-04-14 06:32:18.000000 antgo-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.920694 antgo-0.1.0/antgo/
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.928694 antgo-0.1.0/antgo/ant/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25864 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/activelearning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/activelearning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/activelearning_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9805 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/batch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14101 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/browser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28324 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)    34652 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    22044 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/environment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/flags.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44521 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/ant/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      228 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/config.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)     8645 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.932694 antgo-0.1.0/antgo/crowdsource/
--rwxr-xr-x   0 runner    (1001) docker     (123)      206 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/crowdsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/crowdsource/activelearning_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/crowdsource/base_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/crowdsource/batch_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43022 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/crowdsource/browser_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6412 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/crowdsource/crowdsource_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    27245 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/crowdsource/demo_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/crowdsource/ensemble_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    33823 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/crowdsource/label_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/crowdsource/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8055 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/crowdsource/watch_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.936694 antgo-0.1.0/antgo/cutils/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8249 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/cutils/maskApi.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2176 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/cutils/maskApi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.936694 antgo-0.1.0/antgo/dataflow/
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5412 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/basic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22875 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14235 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.952695 antgo-0.1.0/antgo/dataflow/dataset/
--rwxr-xr-x   0 runner    (1001) docker     (123)      491 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/ade20k.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14996 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/celeba.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6412 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/clsdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    28849 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/coco2017.py
--rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/cusdomcls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29159 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/empty_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/fashionai_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/fashionai_landmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/flic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3139 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/horse2zebra.py
--rw-r--r--   0 runner    (1001) docker     (123)    35321 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/interhand26M.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/iphone2dslr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9328 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/lfw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/lip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/lsp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5843 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/mnist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3725 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/omniglot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/parallel_read.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14380 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/pascal_voc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/proxy_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/queue_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/random_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14453 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4465 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/simpleimages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/simplevideos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/spider_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5861 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/standard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2970 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/svhn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5964 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/vggface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/dataset/visalso.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/datasetio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.952695 antgo-0.1.0/antgo/dataflow/datasynth/
--rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/datasynth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.960695 antgo-0.1.0/antgo/dataflow/imgaug/
--rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/imgaug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65619 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/imgaug/autoaugment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    46247 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/imgaug/batch_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/imgaug/colorspace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3274 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/imgaug/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    25279 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/imgaug/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/imgaug/gridmask_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/imgaug/op_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)   103609 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/imgaug/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/imgaug/operators_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/imgaug/photometric.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10813 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/imgaug/regular.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/imgaug/util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21369 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/dataflow/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.960695 antgo-0.1.0/antgo/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.964695 antgo-0.1.0/antgo/framework/helper/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/activelearning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.964695 antgo-0.1.0/antgo/framework/helper/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/apis/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/base_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.968695 antgo-0.1.0/antgo/framework/helper/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.968695 antgo-0.1.0/antgo/framework/helper/cnn/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/backbone/ddr_lcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/backbone/ddr_mobilenet_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.980695 antgo-0.1.0/antgo/framework/helper/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)    37224 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.984695 antgo-0.1.0/antgo/framework/helper/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/utils/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)    26005 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/utils/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.984695 antgo-0.1.0/antgo/framework/helper/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.984695 antgo-0.1.0/antgo/framework/helper/configs/activelearning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/configs/activelearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/configs/activelearning/ac_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.984695 antgo-0.1.0/antgo/framework/helper/configs/adda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/configs/adda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/configs/adda/adda_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.988695 antgo-0.1.0/antgo/framework/helper/configs/semi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/configs/semi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/configs/semi/dense_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/configs/semi/detmpl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/configs/semi/mpl_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.988695 antgo-0.1.0/antgo/framework/helper/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/dataset_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/dataset_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/kvdataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.992695 antgo-0.1.0/antgo/framework/helper/dataset/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37456 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/pipelines/auto_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/pipelines/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/pipelines/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    29127 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/pipelines/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.996696 antgo-0.1.0/antgo/framework/helper/dataset/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/samplers/class_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/samplers/distributed_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/samplers/group_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/samplers/infinite_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/samplers/kv_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    22421 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/dataset/tfdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.996696 antgo-0.1.0/antgo/framework/helper/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.000696 antgo-0.1.0/antgo/framework/helper/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.000696 antgo-0.1.0/antgo/framework/helper/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/metrics/kp2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/metrics/seg2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.004696 antgo-0.1.0/antgo/framework/helper/models/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.004696 antgo-0.1.0/antgo/framework/helper/models/activelearning/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/activelearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/activelearning/acnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.004696 antgo-0.1.0/antgo/framework/helper/models/adda/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/adda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/adda/adda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.004696 antgo-0.1.0/antgo/framework/helper/models/classification/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.008696 antgo-0.1.0/antgo/framework/helper/models/classification/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23127 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23751 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/backbones/resnext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.008696 antgo-0.1.0/antgo/framework/helper/models/classification/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/heads/cls_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/heads/stacked_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.008696 antgo-0.1.0/antgo/framework/helper/models/classification/losses/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.012696 antgo-0.1.0/antgo/framework/helper/models/classification/model/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/classification/model/classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.012696 antgo-0.1.0/antgo/framework/helper/models/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.012696 antgo-0.1.0/antgo/framework/helper/models/detectors/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.016696 antgo-0.1.0/antgo/framework/helper/models/detectors/core/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.020696 antgo-0.1.0/antgo/framework/helper/models/detectors/core/anchor/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/anchor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/anchor/anchor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/anchor/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/anchor/point_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/anchor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.020696 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.024696 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/approx_max_iou_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/assign_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/atss_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/base_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/center_region_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/grid_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/hungarian_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/max_iou_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/point_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/region_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/sim_ota_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/uniform_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.028696 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/base_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/bucketing_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/delta_xywh_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/distance_point_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/legacy_delta_xywh_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/pseudo_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/tblr_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/yolo_bbox_coder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.032696 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/iou2d_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.032696 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/match_costs/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/match_costs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/match_costs/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/match_costs/match_cost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.036697 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/combined_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/instance_balanced_pos_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/iou_balanced_neg_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/ohem_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/pseudo_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/sampling_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/score_hlr_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.040696 antgo-0.1.0/antgo/framework/helper/models/detectors/core/mask/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/mask/mask_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    40231 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/mask/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/mask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.040696 antgo-0.1.0/antgo/framework/helper/models/detectors/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/utils/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.044697 antgo-0.1.0/antgo/framework/helper/models/detectors/head/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/head/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/head/base_dense_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    21597 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/head/fcos_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.052697 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/ae_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/balanced_l1_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/gaussian_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/gfocal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/ghm_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/iou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/kd_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/mse_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/pisa_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/seesaw_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/smooth_l1_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/losses/varifocal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.052697 antgo-0.1.0/antgo/framework/helper/models/detectors/model/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/model/ttfnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.052697 antgo-0.1.0/antgo/framework/helper/models/detectors/neck/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/neck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/neck/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/single_stage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.052697 antgo-0.1.0/antgo/framework/helper/models/detectors/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/utils/gaussian_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/utils/util_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/detectors/utils/util_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.056697 antgo-0.1.0/antgo/framework/helper/models/distillation/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/detection_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/experts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.064697 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/ab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/afd.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/at.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/bss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/cc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/crd.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/dml.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/fitnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/fsp.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/ft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/irg.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/logits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/lwm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/mgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/nst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/ofd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/pkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/rkd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/sobolev.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/sp.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/st.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/distillation/loss/vid.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/dummy_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/ema_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.064697 antgo-0.1.0/antgo/framework/helper/models/nas/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.064697 antgo-0.1.0/antgo/framework/helper/models/nas/elastic_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/elastic_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.068697 antgo-0.1.0/antgo/framework/helper/models/nas/elastic_nn/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/elastic_nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/elastic_nn/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/model_zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.068697 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.068697 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/baseline/fastdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/baseline/mobilenet_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.068697 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/networks/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/networks/ofa_fastdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/networks/ofa_mbv3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.072697 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/training/epoch_based_sampling_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/training/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/ofa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.072697 antgo-0.1.0/antgo/framework/helper/models/nas/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.072697 antgo-0.1.0/antgo/framework/helper/models/nas/search/accuracy_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/search/accuracy_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/search/accuracy_predictor/arch_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.072697 antgo-0.1.0/antgo/framework/helper/models/nas/search/efficiency_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/search/efficiency_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/search/efficiency_predictor/latency_lookup_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.076697 antgo-0.1.0/antgo/framework/helper/models/nas/search/search_algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/search/search_algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/search/search_algorithm/evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.076697 antgo-0.1.0/antgo/framework/helper/models/nas/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/tutorial/accuracy_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/tutorial/evolution_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/tutorial/flops_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/tutorial/imagenet_eval_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/tutorial/latency_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.080697 antgo-0.1.0/antgo/framework/helper/models/nas/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/utils/common_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24233 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/utils/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/utils/my_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/utils/pytorch_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/nas/utils/pytorch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.084698 antgo-0.1.0/antgo/framework/helper/models/pose3d/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.084698 antgo-0.1.0/antgo/framework/helper/models/pose3d/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/backbone/QNetLite0_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/backbone/QNetLite0_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/backbone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.084698 antgo-0.1.0/antgo/framework/helper/models/pose3d/head/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/head/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/head/handpose_qnet_lite0_pose_heatmap2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/head/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/head/twohand_3dpose_latent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.088698 antgo-0.1.0/antgo/framework/helper/models/pose3d/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/losses/gaussian_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.088698 antgo-0.1.0/antgo/framework/helper/models/pose3d/model/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/model/ddr_twohand_pose3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/model/keynet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.088698 antgo-0.1.0/antgo/framework/helper/models/pose3d/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/pose3d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/proxy_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.088698 antgo-0.1.0/antgo/framework/helper/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.088698 antgo-0.1.0/antgo/framework/helper/models/segmentation/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/segmentation/backbone/DDRQNetLite0.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/segmentation/backbone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.088698 antgo-0.1.0/antgo/framework/helper/models/segmentation/head/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/segmentation/head/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/segmentation/head/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/segmentation/head/simple_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.092698 antgo-0.1.0/antgo/framework/helper/models/segmentation/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/segmentation/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.092698 antgo-0.1.0/antgo/framework/helper/models/segmentation/model/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/segmentation/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/segmentation/model/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.092698 antgo-0.1.0/antgo/framework/helper/models/semi/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/semi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/semi/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/semi/detmpl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.092698 antgo-0.1.0/antgo/framework/helper/models/semi/hook/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/semi/hook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/semi/hook/mean_teacher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.092698 antgo-0.1.0/antgo/framework/helper/models/semi/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/semi/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/semi/losses/quality_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/semi/mpl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.100698 antgo-0.1.0/antgo/framework/helper/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/brick_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/ckpt_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/conv_upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/csp_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/gaussian_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/normed_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/panoptic_gt_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/structure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    40231 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/models/utils/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/multi_stream_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.104698 antgo-0.1.0/antgo/framework/helper/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/parallel/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/parallel/data_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/parallel/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/parallel/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/parallel/scatter_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.108698 antgo-0.1.0/antgo/framework/helper/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19868 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    27539 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/epoch_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/fp16_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.112698 antgo-0.1.0/antgo/framework/helper/runner/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    23377 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/iter_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.116698 antgo-0.1.0/antgo/framework/helper/runner/hooks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/logger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/logger/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/logger/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    24618 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/momentum_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/sampler_seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.116698 antgo-0.1.0/antgo/framework/helper/runner/hooks/samplingmethods/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/samplingmethods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/samplingmethods/kcenter_greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/samplingmethods/sampling_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/submodules_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/sync_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/hooks/weight_adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/iter_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/log_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.116698 antgo-0.1.0/antgo/framework/helper/runner/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/runner/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/task_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.120698 antgo-0.1.0/antgo/framework/helper/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/tools/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/tools/exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/tools/export_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/tools/schedule_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/tools/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    27342 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.128698 antgo-0.1.0/antgo/framework/helper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/compat_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    27018 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/device_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    19158 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/math_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/util_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/helper/utils/version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.128698 antgo-0.1.0/antgo/framework/paddle2torch/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/paddle2torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.136699 antgo-0.1.0/antgo/framework/paddle2torch/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/paddle2torch/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/paddle2torch/mapper/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/paddle2torch/mapper/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/paddle2torch/mapper/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/paddle2torch/mapper/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/paddle2torch/mapper/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.136699 antgo-0.1.0/antgo/framework/paddle2torch/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/paddle2torch/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/paddle2torch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.136699 antgo-0.1.0/antgo/framework/paddle2torch/vision/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/paddle2torch/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.136699 antgo-0.1.0/antgo/framework/torch2paddle/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.140699 antgo-0.1.0/antgo/framework/torch2paddle/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.144699 antgo-0.1.0/antgo/framework/torch2paddle/mapper/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/cuda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/cuda/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/nn_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/nn_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/nn_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/parambase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.144699 antgo-0.1.0/antgo/framework/torch2paddle/mapper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/mapper/varbase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.144699 antgo-0.1.0/antgo/framework/torch2paddle/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28762 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/tools/ast_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/tools/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/tools/dependency_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.144699 antgo-0.1.0/antgo/framework/torch2paddle/vision/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/vision/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/vision/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/framework/torch2paddle/vision/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    15294 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/interactcontext.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29707 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20912 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/main_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.160699 antgo-0.1.0/antgo/measures/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2528 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/ali_fashion_attribute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/ali_fashion_landmark_ne.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5903 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/average_precision.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4744 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/binary_c.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/binomial_deviance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2060 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/confusion_matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21500 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/crowdsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9002 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/deep_analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6339 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/face_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1985 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/kdd_average_precision.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3456 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/matting_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/moving_statistic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4826 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/multi_c.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4348 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/multic_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/multil_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/normalized_error.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45355 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/objdect_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2826 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/pck.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/person_search_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6784 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/precision_recall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8696 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/quadratic_weighted_kappa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2438 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/regression_metric.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/regression_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13252 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/repeat_statistic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      192 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/retrieval_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5448 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/segmentation_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3467 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/significance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7540 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/topk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/track_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4010 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/measures/yesno_crowdsource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.160699 antgo-0.1.0/antgo/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.164699 antgo-0.1.0/antgo/pipeline/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.164699 antgo-0.1.0/antgo/pipeline/engine/execution/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/engine/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/engine/execution/base_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/engine/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/engine/operator_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/engine/operator_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/engine/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.164699 antgo-0.1.0/antgo/pipeline/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.168699 antgo-0.1.0/antgo/pipeline/functional/common/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/common/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17173 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/data_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.168699 antgo-0.1.0/antgo/pipeline/functional/image/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/image/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/image/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/image/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.172700 antgo-0.1.0/antgo/pipeline/functional/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/mixins/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/mixins/computer_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/mixins/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/mixins/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/mixins/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/mixins/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/mixins/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/mixins/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/mixins/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/mixins/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/mixins/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/mixins/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/mixins/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/functional/storages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.176699 antgo-0.1.0/antgo/pipeline/hparam/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hparam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hparam/hyperparameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.176699 antgo-0.1.0/antgo/pipeline/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.176699 antgo-0.1.0/antgo/pipeline/hub/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hub/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.176699 antgo-0.1.0/antgo/pipeline/hub/builtin/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hub/builtin/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hub/builtin/operators/inference_model_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hub/builtin/operators/inference_onnx_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hub/builtin/operators/runas_op.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.176699 antgo-0.1.0/antgo/pipeline/hub/external/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hub/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.180700 antgo-0.1.0/antgo/pipeline/hub/external/mm/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hub/external/mm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hub/external/mm/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hub/external/mm/inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hub/external/mm/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hub/external/mm/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hub/external/mm/restoration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/hub/external/mm/segmentor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.180700 antgo-0.1.0/antgo/pipeline/models/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.908694 antgo-0.1.0/antgo/pipeline/models/cfg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.180700 antgo-0.1.0/antgo/pipeline/models/cfg/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/cfg/dataset/coco.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.184700 antgo-0.1.0/antgo/pipeline/models/cfg/detector/
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/cfg/detector/yolov7-e6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/cfg/detector/yolov7-w6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/cfg/detector/yolov7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/cfg/detector/yolov7x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.184700 antgo-0.1.0/antgo/pipeline/models/detector/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/detector/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.184700 antgo-0.1.0/antgo/pipeline/models/detector/yolov7/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/detector/yolov7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/detector/yolov7/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/detector/yolov7/yolov7.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.184700 antgo-0.1.0/antgo/pipeline/models/pose/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/pose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.184700 antgo-0.1.0/antgo/pipeline/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.188700 antgo-0.1.0/antgo/pipeline/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86819 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/models/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.188700 antgo-0.1.0/antgo/pipeline/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/operators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/operators/nop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.188700 antgo-0.1.0/antgo/pipeline/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.188700 antgo-0.1.0/antgo/pipeline/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/pipeline/utils/repo_normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.192700 antgo-0.1.0/antgo/resource/
--rwxr-xr-x   0 runner    (1001) docker     (123)      200 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.192700 antgo-0.1.0/antgo/resource/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.192700 antgo-0.1.0/antgo/resource/app/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/css/359.32c5c11e.css
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/css/385.1759eef9.css
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/css/854.9e012a59.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/css/app.48eb9280.css
--rw-r--r--   0 runner    (1001) docker     (123)   219463 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/css/chunk-vendors.1944359c.css
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.208700 antgo-0.1.0/antgo/resource/app/js/
--rw-r--r--   0 runner    (1001) docker     (123)   182502 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/359.afb86915.js
--rw-r--r--   0 runner    (1001) docker     (123)   828443 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/359.afb86915.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/385.90ba0f66.js
--rw-r--r--   0 runner    (1001) docker     (123)    31358 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/385.90ba0f66.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/532.f949def3.js
--rw-r--r--   0 runner    (1001) docker     (123)    24678 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/532.f949def3.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/651.c5601578.js
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/651.c5601578.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/769.b7247054.js
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/769.b7247054.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/854.d3c0e54f.js
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/854.d3c0e54f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/880.cba02e88.js
--rw-r--r--   0 runner    (1001) docker     (123)    19810 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/880.cba02e88.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/app.f01f9b7a.js
--rw-r--r--   0 runner    (1001) docker     (123)    33636 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/app.f01f9b7a.js.map
--rw-r--r--   0 runner    (1001) docker     (123)  1289477 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/chunk-vendors.18913786.js
--rw-r--r--   0 runner    (1001) docker     (123)  3750898 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/app/js/chunk-vendors.18913786.js.map
--rwxr-xr-x   0 runner    (1001) docker     (123)    23363 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.228701 antgo-0.1.0/antgo/resource/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/static/antgo.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     9662 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/static/antgo.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/static/antgo.js
--rw-r--r--   0 runner    (1001) docker     (123)   236514 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/static/apply.png
--rw-r--r--   0 runner    (1001) docker     (123)   292973 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/static/banner.png
--rw-r--r--   0 runner    (1001) docker     (123)    32806 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/static/card.png
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/static/crowdsource.js
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/static/error.json
--rw-r--r--   0 runner    (1001) docker     (123)    85624 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/static/filetree.png
--rw-r--r--   0 runner    (1001) docker     (123)    32294 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/static/holder.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   106186 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/static/register.png
--rw-r--r--   0 runner    (1001) docker     (123)   244247 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/static/start-experiment.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.236701 antgo-0.1.0/antgo/resource/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/activelearning.html
--rwxr-xr-x   0 runner    (1001) docker     (123)    16328 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/crowdsource.html
--rw-r--r--   0 runner    (1001) docker     (123)    22287 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/demo.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.240701 antgo-0.1.0/antgo/resource/templates/mvp/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.240701 antgo-0.1.0/antgo/resource/templates/mvp/cifar10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.240701 antgo-0.1.0/antgo/resource/templates/mvp/cifar10/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/cifar10/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/cifar10/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/cifar10/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    18693 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/cifar10/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/cifar10/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.240701 antgo-0.1.0/antgo/resource/templates/mvp/cifar10/models/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/cifar10/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/cifar10/models/wideres.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/install.sh
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/launch.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/lsp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/pascal_voc_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/mvp/visalso_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/project.json
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/sample_gt.json
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/sample_meta.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    61982 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/statistic-report.html
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/task.template
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/task_main_file.template
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/task_main_param.template
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/task_shell.template
--rw-r--r--   0 runner    (1001) docker     (123)    30333 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/trainmaster.html
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/trainworker.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     1867 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/resource/templates/yesno_crowdsource.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.260702 antgo-0.1.0/antgo/sandbox/
--rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/sandbox/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2542 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/sandbox/sandbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.264701 antgo-0.1.0/antgo/script/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/script/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/script/custom_submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/script/data_convert_cifar10_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/script/data_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/script/local_submit.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/script/ssh-launch.sh
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/script/ssh-submit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/script/ssh-submit.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/script/ssh_submit.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/script/submit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/script/test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.264701 antgo-0.1.0/antgo/task/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/task/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12291 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/task/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.268702 antgo-0.1.0/antgo/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/tools/browser_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/tools/download_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/tools/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/tools/filter_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25756 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/tools/label_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/tools/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.276702 antgo-0.1.0/antgo/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      402 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/_bbox.pyx
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/_encode_png.pyx
--rwxr-xr-x   0 runner    (1001) docker     (123)    11418 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/_mask.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/args.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/argscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/colormap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8104 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/concurrency.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1887 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/cpu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1242 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/encode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3819 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/fs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2915 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/gpu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4076 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4553 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/mask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9588 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/netvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10128 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/parallel_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/pickledb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/processbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/sample_gt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1372 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.276702 antgo-0.1.0/antgo/utils/shared_queue/
--rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/shared_queue/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3163 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/shared_queue/queue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17513 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/shared_queue/sharedmemory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/timer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3959 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-04-14 06:32:18.000000 antgo-0.1.0/antgo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:02.920694 antgo-0.1.0/antgo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-14 06:35:02.000000 antgo-0.1.0/antgo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35493 2023-04-14 06:35:02.000000 antgo-0.1.0/antgo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:35:02.000000 antgo-0.1.0/antgo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 06:35:02.000000 antgo-0.1.0/antgo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:35:02.000000 antgo-0.1.0/antgo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 06:35:02.000000 antgo-0.1.0/antgo.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-14 06:32:18.000000 antgo-0.1.0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-04-14 06:32:18.000000 antgo-0.1.0/roadmap.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 06:35:03.280702 antgo-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-04-14 06:32:18.000000 antgo-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:35:03.280702 antgo-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-14 06:32:18.000000 antgo-0.1.0/test/test_antgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-14 06:32:18.000000 antgo-0.1.0/test/test_paddle_c.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-14 06:32:18.000000 antgo-0.1.0/test/test_torch_c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.475451 antgo-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/LICENSE.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-04-21 08:45:32.000000 antgo-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-21 08:48:21.475451 antgo-0.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4480 2023-04-21 08:45:32.000000 antgo-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.151447 antgo-0.1.1/antgo/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.159447 antgo-0.1.1/antgo/ant/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25864 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/activelearning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/activelearning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/activelearning_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9805 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/batch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14101 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/browser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28324 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34652 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22044 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/environment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/flags.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44521 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/ant/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      228 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/config.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8645 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.167447 antgo-0.1.1/antgo/crowdsource/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      206 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/crowdsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/crowdsource/activelearning_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/crowdsource/base_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/crowdsource/batch_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43022 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/crowdsource/browser_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6412 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/crowdsource/crowdsource_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27245 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/crowdsource/demo_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/crowdsource/ensemble_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33823 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/crowdsource/label_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/crowdsource/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8055 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/crowdsource/watch_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.167447 antgo-0.1.1/antgo/cutils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8249 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/cutils/maskApi.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2176 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/cutils/maskApi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.171447 antgo-0.1.1/antgo/dataflow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5412 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/basic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22875 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14235 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.183448 antgo-0.1.1/antgo/dataflow/dataset/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/ade20k.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14996 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/celeba.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5425 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/cityscape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/clsdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/coco2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/cusdomcls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29220 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/empty_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/fashionai_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/fashionai_landmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/flic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3139 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/horse2zebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35327 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/interhand26M.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/iphone2dslr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8328 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/lfw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/lip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/lsp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/mnist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3725 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/omniglot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/parallel_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12810 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/pascal_voc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/proxy_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/queue_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/random_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14554 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4465 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/simpleimages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/simplevideos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/spider_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3559 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/vggface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/dataset/visalso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/datasetio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.183448 antgo-0.1.1/antgo/dataflow/datasynth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/datasynth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.191448 antgo-0.1.1/antgo/dataflow/imgaug/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      943 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/imgaug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65619 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/imgaug/autoaugment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46247 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/imgaug/batch_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/imgaug/colorspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3274 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/imgaug/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25279 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/imgaug/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/imgaug/gridmask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/imgaug/op_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104772 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/imgaug/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/imgaug/operators_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/imgaug/photometric.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10813 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/imgaug/regular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/imgaug/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21369 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/dataflow/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.191448 antgo-0.1.1/antgo/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.195448 antgo-0.1.1/antgo/framework/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/activelearning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.195448 antgo-0.1.1/antgo/framework/helper/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/apis/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/base_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.199448 antgo-0.1.1/antgo/framework/helper/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.199448 antgo-0.1.1/antgo/framework/helper/cnn/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/backbone/ddr_lcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/backbone/ddr_mobilenet_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.211448 antgo-0.1.1/antgo/framework/helper/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37224 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.215448 antgo-0.1.1/antgo/framework/helper/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/utils/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26005 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/utils/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.215448 antgo-0.1.1/antgo/framework/helper/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.215448 antgo-0.1.1/antgo/framework/helper/configs/activelearning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/configs/activelearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/configs/activelearning/ac_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.215448 antgo-0.1.1/antgo/framework/helper/configs/adda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/configs/adda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/configs/adda/adda_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.215448 antgo-0.1.1/antgo/framework/helper/configs/distillation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/configs/distillation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/configs/distillation/reviewkd_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.219448 antgo-0.1.1/antgo/framework/helper/configs/semi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/configs/semi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/configs/semi/dense_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/configs/semi/detmpl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/configs/semi/mpl_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.219448 antgo-0.1.1/antgo/framework/helper/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/dataset_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/dataset_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/kvdataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.223448 antgo-0.1.1/antgo/framework/helper/dataset/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37456 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/pipelines/auto_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/pipelines/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/pipelines/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29127 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/pipelines/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.227448 antgo-0.1.1/antgo/framework/helper/dataset/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/samplers/class_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/samplers/distributed_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/samplers/group_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/samplers/infinite_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/samplers/kv_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22421 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/dataset/tfdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.227448 antgo-0.1.1/antgo/framework/helper/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.231448 antgo-0.1.1/antgo/framework/helper/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.231448 antgo-0.1.1/antgo/framework/helper/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/metrics/kp2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/metrics/seg2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.235448 antgo-0.1.1/antgo/framework/helper/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.235448 antgo-0.1.1/antgo/framework/helper/models/activelearning/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/activelearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/activelearning/acnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.235448 antgo-0.1.1/antgo/framework/helper/models/adda/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/adda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/adda/adda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.235448 antgo-0.1.1/antgo/framework/helper/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.239448 antgo-0.1.1/antgo/framework/helper/models/classification/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23127 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23751 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/backbones/resnext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.239448 antgo-0.1.1/antgo/framework/helper/models/classification/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/heads/cls_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/heads/stacked_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.239448 antgo-0.1.1/antgo/framework/helper/models/classification/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.243448 antgo-0.1.1/antgo/framework/helper/models/classification/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/classification/model/classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.243448 antgo-0.1.1/antgo/framework/helper/models/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.243448 antgo-0.1.1/antgo/framework/helper/models/detectors/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.243448 antgo-0.1.1/antgo/framework/helper/models/detectors/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.247448 antgo-0.1.1/antgo/framework/helper/models/detectors/core/anchor/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/anchor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/anchor/anchor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/anchor/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/anchor/point_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/anchor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.247448 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.255448 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/approx_max_iou_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/assign_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/atss_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/base_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/center_region_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/grid_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/hungarian_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/max_iou_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/point_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/region_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/sim_ota_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/uniform_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.255448 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/base_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/bucketing_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/delta_xywh_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/distance_point_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/legacy_delta_xywh_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/pseudo_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/tblr_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/yolo_bbox_coder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.259449 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/iou2d_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.259449 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/match_costs/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/match_costs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/match_costs/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/match_costs/match_cost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.263449 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/combined_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/instance_balanced_pos_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/iou_balanced_neg_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/ohem_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/pseudo_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/sampling_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/score_hlr_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.267449 antgo-0.1.1/antgo/framework/helper/models/detectors/core/mask/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/mask/mask_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40231 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/mask/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/mask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.267449 antgo-0.1.1/antgo/framework/helper/models/detectors/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/utils/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.267449 antgo-0.1.1/antgo/framework/helper/models/detectors/head/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/head/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/head/base_dense_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20169 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/head/fcos_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21834 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/head/focs_head_ml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.275449 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/ae_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/balanced_l1_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/gaussian_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/gfocal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/ghm_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/iou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/kd_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/mse_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/pisa_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/seesaw_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/smooth_l1_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/losses/varifocal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.279449 antgo-0.1.1/antgo/framework/helper/models/detectors/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/model/ttfnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.279449 antgo-0.1.1/antgo/framework/helper/models/detectors/neck/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/neck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/neck/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/single_stage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.279449 antgo-0.1.1/antgo/framework/helper/models/detectors/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/utils/gaussian_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/utils/util_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/detectors/utils/util_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.279449 antgo-0.1.1/antgo/framework/helper/models/distillation/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/distillation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.287449 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/ab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/afd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/bss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/crd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/dml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/fitnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/fsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/ft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/hcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/irg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/logits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/lwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/mgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/nst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/ofd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/pkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/rkd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/sobolev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/sp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/st.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/distillation/loss/vid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/dummy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/ema_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.291449 antgo-0.1.1/antgo/framework/helper/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.291449 antgo-0.1.1/antgo/framework/helper/models/nas/elastic_nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/elastic_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.291449 antgo-0.1.1/antgo/framework/helper/models/nas/elastic_nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/elastic_nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/elastic_nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/model_zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.291449 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.291449 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/baseline/fastdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/baseline/mobilenet_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.295449 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/networks/ofa_fastdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/networks/ofa_mbv3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.295449 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/training/epoch_based_sampling_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/training/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/ofa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.295449 antgo-0.1.1/antgo/framework/helper/models/nas/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.295449 antgo-0.1.1/antgo/framework/helper/models/nas/search/accuracy_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/search/accuracy_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/search/accuracy_predictor/arch_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.299449 antgo-0.1.1/antgo/framework/helper/models/nas/search/efficiency_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/search/efficiency_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/search/efficiency_predictor/latency_lookup_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.299449 antgo-0.1.1/antgo/framework/helper/models/nas/search/search_algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/search/search_algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/search/search_algorithm/evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.299449 antgo-0.1.1/antgo/framework/helper/models/nas/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/tutorial/accuracy_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/tutorial/evolution_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/tutorial/flops_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/tutorial/imagenet_eval_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/tutorial/latency_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.303449 antgo-0.1.1/antgo/framework/helper/models/nas/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/utils/common_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24233 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/utils/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/utils/my_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/utils/pytorch_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/nas/utils/pytorch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.303449 antgo-0.1.1/antgo/framework/helper/models/pose3d/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.303449 antgo-0.1.1/antgo/framework/helper/models/pose3d/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/backbone/QNetLite0_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/backbone/QNetLite0_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/backbone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.307449 antgo-0.1.1/antgo/framework/helper/models/pose3d/head/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/head/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/head/handpose_qnet_lite0_pose_heatmap2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/head/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/head/twohand_3dpose_latent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.307449 antgo-0.1.1/antgo/framework/helper/models/pose3d/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/losses/gaussian_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.307449 antgo-0.1.1/antgo/framework/helper/models/pose3d/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/model/ddr_twohand_pose3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/model/keynet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.311449 antgo-0.1.1/antgo/framework/helper/models/pose3d/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/pose3d/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/proxy_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.311449 antgo-0.1.1/antgo/framework/helper/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.311449 antgo-0.1.1/antgo/framework/helper/models/segmentation/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/segmentation/backbone/DDRQNetLite0.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/segmentation/backbone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.311449 antgo-0.1.1/antgo/framework/helper/models/segmentation/head/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/segmentation/head/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/segmentation/head/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/segmentation/head/simple_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.311449 antgo-0.1.1/antgo/framework/helper/models/segmentation/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/segmentation/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.311449 antgo-0.1.1/antgo/framework/helper/models/segmentation/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/segmentation/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/segmentation/model/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.315449 antgo-0.1.1/antgo/framework/helper/models/semi/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/semi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/semi/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/semi/detmpl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.315449 antgo-0.1.1/antgo/framework/helper/models/semi/hook/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/semi/hook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/semi/hook/mean_teacher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.315449 antgo-0.1.1/antgo/framework/helper/models/semi/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/semi/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/semi/losses/quality_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/semi/mpl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.323449 antgo-0.1.1/antgo/framework/helper/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/brick_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/ckpt_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/conv_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/csp_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/gaussian_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/normed_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/panoptic_gt_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/structure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40231 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/models/utils/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/multi_stream_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.327449 antgo-0.1.1/antgo/framework/helper/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/parallel/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/parallel/data_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/parallel/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/parallel/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/parallel/scatter_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.331449 antgo-0.1.1/antgo/framework/helper/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19868 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27545 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/epoch_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/fp16_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.339450 antgo-0.1.1/antgo/framework/helper/runner/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23377 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/iter_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.339450 antgo-0.1.1/antgo/framework/helper/runner/hooks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/logger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/logger/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/logger/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24618 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/momentum_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/sampler_seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.343449 antgo-0.1.1/antgo/framework/helper/runner/hooks/samplingmethods/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/samplingmethods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/samplingmethods/kcenter_greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/samplingmethods/sampling_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/submodules_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/sync_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/hooks/weight_adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/iter_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/log_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.343449 antgo-0.1.1/antgo/framework/helper/runner/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/runner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/task_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.347450 antgo-0.1.1/antgo/framework/helper/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/tools/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/tools/exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/tools/export_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/tools/schedule_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/tools/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27342 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.355450 antgo-0.1.1/antgo/framework/helper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/compat_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27018 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/device_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19158 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/math_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/util_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/helper/utils/version_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.355450 antgo-0.1.1/antgo/framework/paddle2torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/paddle2torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.355450 antgo-0.1.1/antgo/framework/paddle2torch/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/paddle2torch/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/paddle2torch/mapper/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/paddle2torch/mapper/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/paddle2torch/mapper/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/paddle2torch/mapper/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/paddle2torch/mapper/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.355450 antgo-0.1.1/antgo/framework/paddle2torch/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/paddle2torch/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/paddle2torch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.359450 antgo-0.1.1/antgo/framework/paddle2torch/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/paddle2torch/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.359450 antgo-0.1.1/antgo/framework/torch2paddle/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.363450 antgo-0.1.1/antgo/framework/torch2paddle/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.363450 antgo-0.1.1/antgo/framework/torch2paddle/mapper/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/cuda/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/nn_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/nn_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/nn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/parambase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.363450 antgo-0.1.1/antgo/framework/torch2paddle/mapper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/mapper/varbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.367450 antgo-0.1.1/antgo/framework/torch2paddle/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28762 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/tools/ast_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/tools/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/tools/dependency_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.367450 antgo-0.1.1/antgo/framework/torch2paddle/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/vision/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/vision/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/framework/torch2paddle/vision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24659 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15294 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/interactcontext.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29707 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20912 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/main_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.379450 antgo-0.1.1/antgo/measures/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2528 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/ali_fashion_attribute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/ali_fashion_landmark_ne.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5903 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/average_precision.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4744 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/binary_c.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/binomial_deviance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2060 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/confusion_matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21500 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/crowdsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9002 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/deep_analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6339 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/face_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1985 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/kdd_average_precision.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3456 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/matting_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/moving_statistic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4826 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/multi_c.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4348 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/multic_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/multil_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/normalized_error.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45355 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/objdect_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2826 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/pck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/person_search_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6784 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/precision_recall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8696 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/quadratic_weighted_kappa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2438 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/regression_metric.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/regression_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13252 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/repeat_statistic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      192 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/retrieval_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5448 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/segmentation_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3467 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/significance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7540 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/track_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4010 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/measures/yesno_crowdsource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.383450 antgo-0.1.1/antgo/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.383450 antgo-0.1.1/antgo/pipeline/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.383450 antgo-0.1.1/antgo/pipeline/engine/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/engine/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/engine/execution/base_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/engine/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/engine/operator_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/engine/operator_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/engine/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.387450 antgo-0.1.1/antgo/pipeline/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.387450 antgo-0.1.1/antgo/pipeline/functional/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/common/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17173 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/data_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.387450 antgo-0.1.1/antgo/pipeline/functional/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/image/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/image/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.395450 antgo-0.1.1/antgo/pipeline/functional/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/mixins/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/mixins/computer_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/mixins/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/mixins/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/mixins/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/mixins/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/mixins/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/mixins/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/mixins/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/mixins/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/mixins/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/mixins/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/mixins/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/functional/storages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.395450 antgo-0.1.1/antgo/pipeline/hparam/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hparam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hparam/hyperparameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.395450 antgo-0.1.1/antgo/pipeline/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.395450 antgo-0.1.1/antgo/pipeline/hub/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hub/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.395450 antgo-0.1.1/antgo/pipeline/hub/builtin/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hub/builtin/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hub/builtin/operators/inference_model_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hub/builtin/operators/inference_onnx_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hub/builtin/operators/runas_op.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.395450 antgo-0.1.1/antgo/pipeline/hub/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hub/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.399450 antgo-0.1.1/antgo/pipeline/hub/external/mm/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hub/external/mm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hub/external/mm/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hub/external/mm/inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hub/external/mm/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hub/external/mm/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hub/external/mm/restoration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/hub/external/mm/segmentor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.399450 antgo-0.1.1/antgo/pipeline/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.139447 antgo-0.1.1/antgo/pipeline/models/cfg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.399450 antgo-0.1.1/antgo/pipeline/models/cfg/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/cfg/dataset/coco.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.399450 antgo-0.1.1/antgo/pipeline/models/cfg/detector/
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/cfg/detector/yolov7-e6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/cfg/detector/yolov7-w6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/cfg/detector/yolov7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/cfg/detector/yolov7x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.403450 antgo-0.1.1/antgo/pipeline/models/detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/detector/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.403450 antgo-0.1.1/antgo/pipeline/models/detector/yolov7/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/detector/yolov7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/detector/yolov7/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/detector/yolov7/yolov7.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.403450 antgo-0.1.1/antgo/pipeline/models/pose/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/pose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.403450 antgo-0.1.1/antgo/pipeline/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.407450 antgo-0.1.1/antgo/pipeline/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86819 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/models/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.407450 antgo-0.1.1/antgo/pipeline/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/operators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/operators/nop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.407450 antgo-0.1.1/antgo/pipeline/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.407450 antgo-0.1.1/antgo/pipeline/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/pipeline/utils/repo_normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.411450 antgo-0.1.1/antgo/resource/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      200 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.411450 antgo-0.1.1/antgo/resource/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.411450 antgo-0.1.1/antgo/resource/app/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/css/359.32c5c11e.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/css/385.1759eef9.css
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/css/854.9e012a59.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/css/app.48eb9280.css
+-rw-r--r--   0 runner    (1001) docker     (123)   219463 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/css/chunk-vendors.1944359c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.427451 antgo-0.1.1/antgo/resource/app/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   182502 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/359.afb86915.js
+-rw-r--r--   0 runner    (1001) docker     (123)   828443 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/359.afb86915.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/385.90ba0f66.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31358 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/385.90ba0f66.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/532.f949def3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24678 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/532.f949def3.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/651.c5601578.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/651.c5601578.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/769.b7247054.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/769.b7247054.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/854.d3c0e54f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/854.d3c0e54f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/880.cba02e88.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19810 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/880.cba02e88.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/app.f01f9b7a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33636 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/app.f01f9b7a.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)  1289477 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/chunk-vendors.18913786.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3750898 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/app/js/chunk-vendors.18913786.js.map
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23363 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.443451 antgo-0.1.1/antgo/resource/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/static/antgo.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9662 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/static/antgo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/static/antgo.js
+-rw-r--r--   0 runner    (1001) docker     (123)   236514 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/static/apply.png
+-rw-r--r--   0 runner    (1001) docker     (123)   292973 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/static/banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32806 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/static/card.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/static/crowdsource.js
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/static/error.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85624 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/static/filetree.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32294 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/static/holder.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   106186 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/static/register.png
+-rw-r--r--   0 runner    (1001) docker     (123)   244247 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/static/start-experiment.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.451451 antgo-0.1.1/antgo/resource/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/activelearning.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16328 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/crowdsource.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22287 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/demo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.455451 antgo-0.1.1/antgo/resource/templates/mvp/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.455451 antgo-0.1.1/antgo/resource/templates/mvp/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.455451 antgo-0.1.1/antgo/resource/templates/mvp/cifar10/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/cifar10/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/cifar10/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/cifar10/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19161 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/cifar10/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/cifar10/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.455451 antgo-0.1.1/antgo/resource/templates/mvp/cifar10/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/cifar10/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/cifar10/models/wideres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/coco_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/launch.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/lsp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/pascal_voc_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/mvp/visalso_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/project.json
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/sample_gt.json
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/sample_meta.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61982 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/statistic-report.html
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/task.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/task_main_file.template
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/task_main_param.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/task_shell.template
+-rw-r--r--   0 runner    (1001) docker     (123)    30333 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/trainmaster.html
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/trainworker.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1867 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/resource/templates/yesno_crowdsource.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.459451 antgo-0.1.1/antgo/sandbox/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/sandbox/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2542 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/sandbox/sandbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.463451 antgo-0.1.1/antgo/script/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/script/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/script/custom_submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/script/data_convert_cifar10_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/script/data_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/script/local_submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/script/ssh-launch.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/script/ssh-submit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/script/ssh-submit.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/script/ssh_submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/script/submit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/script/test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.463451 antgo-0.1.1/antgo/task/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/task/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12291 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/task/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.463451 antgo-0.1.1/antgo/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/tools/browser_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/tools/download_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/tools/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/tools/filter_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25713 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/tools/label_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/tools/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.471451 antgo-0.1.1/antgo/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      402 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/_bbox.pyx
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/_encode_png.pyx
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11418 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/_mask.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/args.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/argscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/colormap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8104 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/concurrency.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1887 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/cpu.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1242 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/encode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3819 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/fs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2915 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/gpu.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4076 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4553 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9588 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/netvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10128 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/parallel_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/pickledb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/processbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/sample_gt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1372 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.475451 antgo-0.1.1/antgo/utils/shared_queue/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/shared_queue/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3163 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/shared_queue/queue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17513 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/shared_queue/sharedmemory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3959 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-04-21 08:45:32.000000 antgo-0.1.1/antgo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.151447 antgo-0.1.1/antgo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-21 08:48:20.000000 antgo-0.1.1/antgo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35727 2023-04-21 08:48:21.000000 antgo-0.1.1/antgo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:48:20.000000 antgo-0.1.1/antgo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 08:48:20.000000 antgo-0.1.1/antgo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:48:20.000000 antgo-0.1.1/antgo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 08:48:20.000000 antgo-0.1.1/antgo.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      352 2023-04-21 08:45:32.000000 antgo-0.1.1/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-04-21 08:45:32.000000 antgo-0.1.1/roadmap.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:48:21.475451 antgo-0.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-04-21 08:45:32.000000 antgo-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:21.475451 antgo-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-21 08:45:32.000000 antgo-0.1.1/test/test_antgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-21 08:45:32.000000 antgo-0.1.1/test/test_paddle_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-21 08:45:32.000000 antgo-0.1.1/test/test_torch_c.py
```

### Comparing `antgo-0.1.0/PKG-INFO` & `antgo-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: antgo
-Version: 0.1.0
+Version: 0.1.1
 Summary: machine learning experiment platform
 Home-page: https://github.com/jianzfb/antgo
 Author: jian
 Author-email: jian@mltalker.com
-License: UNKNOWN
-Platform: UNKNOWN
 License-File: LICENSE.md
 
 ======================
 Antgo
 ======================
 
 .. image:: https://raw.githubusercontent.com/jianzfb/antgo/master/antgo/resource/static/card.png
@@ -176,8 +174,7 @@
 
 antgo train exp
 
 
 5.step Run Challenge Task
 
 antgo challenge exp experiment_uuid
-
```

### Comparing `antgo-0.1.0/README.rst` & `antgo-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/activelearning.py` & `antgo-0.1.1/antgo/ant/activelearning.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/activelearning_api.py` & `antgo-0.1.1/antgo/ant/activelearning_api.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/activelearning_v2.py` & `antgo-0.1.1/antgo/ant/activelearning_v2.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/base.py` & `antgo-0.1.1/antgo/ant/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/batch.py` & `antgo-0.1.1/antgo/ant/batch.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/browser.py` & `antgo-0.1.1/antgo/ant/browser.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/challenge.py` & `antgo-0.1.1/antgo/ant/challenge.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/client.py` & `antgo-0.1.1/antgo/ant/client.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/debug.py` & `antgo-0.1.1/antgo/ant/debug.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/demo.py` & `antgo-0.1.1/antgo/ant/demo.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/download.py` & `antgo-0.1.1/antgo/ant/download.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/ensemble.py` & `antgo-0.1.1/antgo/ant/ensemble.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/environment.py` & `antgo-0.1.1/antgo/ant/environment.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/flags.py` & `antgo-0.1.1/antgo/ant/flags.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/train.py` & `antgo-0.1.1/antgo/ant/train.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/utils.py` & `antgo-0.1.1/antgo/ant/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/ant/watch.py` & `antgo-0.1.1/antgo/ant/watch.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/config.py` & `antgo-0.1.1/antgo/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/context.py` & `antgo-0.1.1/antgo/context.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/crowdsource/activelearning_server.py` & `antgo-0.1.1/antgo/crowdsource/activelearning_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/crowdsource/base_server.py` & `antgo-0.1.1/antgo/crowdsource/base_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/crowdsource/batch_server.py` & `antgo-0.1.1/antgo/crowdsource/batch_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/crowdsource/browser_server.py` & `antgo-0.1.1/antgo/crowdsource/browser_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/crowdsource/crowdsource_server.py` & `antgo-0.1.1/antgo/crowdsource/crowdsource_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/crowdsource/demo_server.py` & `antgo-0.1.1/antgo/crowdsource/demo_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/crowdsource/ensemble_server.py` & `antgo-0.1.1/antgo/crowdsource/ensemble_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/crowdsource/label_server.py` & `antgo-0.1.1/antgo/crowdsource/label_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/crowdsource/utils.py` & `antgo-0.1.1/antgo/crowdsource/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/crowdsource/watch_server.py` & `antgo-0.1.1/antgo/crowdsource/watch_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/cutils/maskApi.c` & `antgo-0.1.1/antgo/cutils/maskApi.c`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/cutils/maskApi.h` & `antgo-0.1.1/antgo/cutils/maskApi.h`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/basic.py` & `antgo-0.1.1/antgo/dataflow/basic.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/common.py` & `antgo-0.1.1/antgo/dataflow/common.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/core.py` & `antgo-0.1.1/antgo/dataflow/core.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/celeba.py` & `antgo-0.1.1/antgo/dataflow/dataset/celeba.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/cifar.py` & `antgo-0.1.1/antgo/dataflow/dataset/cifar.py`

 * *Files 24% similar despite different names*

```diff
@@ -61,25 +61,20 @@
 
 class CifarBase(Dataset):
   """
   Return [image, label],
       image is 32x32x3 in the range [0,255]
   """
   def __init__(self, train_or_test, dir=None, params=None, cifar_classnum=10):
-    assert train_or_test in ['train', 'test', 'sample']
     assert cifar_classnum == 10 or cifar_classnum == 100
     super(CifarBase,self).__init__(train_or_test,dir)
     self.train_or_test = train_or_test
     self.cifar_classnum = cifar_classnum
     self.dir = dir
 
-    if self.train_or_test == 'sample':
-      self.data_samples, self.ids = self.load_samples()
-      return
-
     if not os.path.exists(self.dir):
       os.makedirs(self.dir)
 
     # fixed seed
     self.seed = time.time()
 
     """Download and extract the tarball from Alex's website."""
@@ -116,46 +111,15 @@
   def get_cat_ids(self, idx):
     return self.label[idx]
   
   def get_ann_info(self, idx):
     return {'label': self.label[idx]}
   
   def at(self, id):
-    if self.train_or_test == 'sample':
-      return self.data_samples[id]
     return self.image[id], self.label[id]
-  
-  def data_pool(self):
-    if self.train_or_test == 'sample':
-      sample_idxs = copy.deepcopy(self.ids)
-      if self.rng:
-        self.rng.shuffle(sample_idxs)
-
-      for index in sample_idxs:
-        yield self.data_samples[index]
-      return
-
-    self.epoch = 0
-    while True:
-      max_epoches = self.epochs if self.epochs is not None else 1
-      if self.epoch >= max_epoches:
-        break
-      self.epoch += 1
-
-      ids = copy.copy(self.ids)
-      if self.rng:
-        self.rng.shuffle(ids)
-
-      # filter by ids
-      filter_ids = getattr(self, 'filter', None)
-      if filter_ids is not None:
-        ids = [i for i in ids if i in filter_ids]
-
-      for id in ids:
-          yield [copy.deepcopy(self.image[id]), self.label[id]]
 
 
 class Cifar10(CifarBase):
   def __init__(self, train_or_test, dir=None, params=None):
     super(Cifar10, self).__init__(train_or_test, dir, params,10)
 
   def split(self, split_params={}, split_method='holdout'):
```

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/clsdataset.py` & `antgo-0.1.1/antgo/dataflow/dataset/clsdataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/cusdomcls.py` & `antgo-0.1.1/antgo/dataflow/dataset/cusdomcls.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/dataset.py` & `antgo-0.1.1/antgo/dataflow/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,20 +357,24 @@
     return self.at(index)
 
   def at(self, id):
     raise NotImplementedError
 
   def get_ann_info(self, idx=None):
     raise NotImplementedError
-    
+
   def get_cat_ids(self, idx):
     raise NotImplementedError
   
   def sample(self, id):
     image, annotation = self.at(id)
+    if image is None:
+      # None 跳过
+      return None
+    
     if not isinstance(annotation, dict):
       annotation = {'label': annotation}
 
     if image is not None:
       annotation['image'] = image
     return annotation
```

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/empty_dataset.py` & `antgo-0.1.1/antgo/dataflow/dataset/empty_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/fashionai_attribute.py` & `antgo-0.1.1/antgo/dataflow/dataset/fashionai_attribute.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/fashionai_landmark.py` & `antgo-0.1.1/antgo/dataflow/dataset/fashionai_landmark.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/horse2zebra.py` & `antgo-0.1.1/antgo/dataflow/dataset/horse2zebra.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/imagenet.py` & `antgo-0.1.1/antgo/dataflow/dataset/imagenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1050,10 +1050,10 @@
         super().__init__(
             train_or_test,
             dir,
             params=params
         )
 
 
-if __name__ == '__main__':
-    print('hell')
-    pass
+# if __name__ == '__main__':
+#     print('hell')
+#     pass
```

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/interhand26M.py` & `antgo-0.1.1/antgo/dataflow/dataset/interhand26M.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/iphone2dslr.py` & `antgo-0.1.1/antgo/dataflow/dataset/iphone2dslr.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/lfw.py` & `antgo-0.1.1/antgo/dataflow/dataset/lfw.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,247 +1,202 @@
 # -*- coding: UTF-8 -*-
 # @Time    : 17-12-27
 # @File    : lfw.py
 # @Author  : jian<jian@mltalker.com>
 from __future__ import division
 from __future__ import unicode_literals
 from __future__ import print_function
+import sys
 from antgo.dataflow.dataset import *
 import os
 import numpy as np
+import time
+import copy
+import cv2
+from antgo.framework.helper.fileio.file_client import *
+
 
 __all__ = ['LFW']
 
-LFW_URL = 'http://vis-www.cs.umass.edu/lfw/index.html#download'
 class LFW(Dataset):
-  def __init__(self, train_or_test, dir=None, params=None):
-    super(LFW, self).__init__(train_or_test, dir, params)
-    assert(train_or_test in ['train', 'test','sample'])
-
-    # read sample data
-    if self.train_or_test == 'sample':
-      self.data_samples, self.ids = self.load_samples()
-      return
-
-    self.image_flag = getattr(self, 'image', 'align')
-    # 0.step maybe download
-    if self.image_flag == 'align':
-      if not os.path.exists(os.path.join(self.dir, 'lfw-deepfunneled')):
-        self.download(self.dir,
-                      file_names=[],
-                      default_url='http://vis-www.cs.umass.edu/lfw/lfw-deepfunneled.tgz',
-                      auto_untar=True,
-                      is_gz=True)
-    else:
-      if not os.path.exists(os.path.join(self.dir, 'lfw')):
-        self.download(self.dir,
-                      file_names=[],
-                      default_url='http://vis-www.cs.umass.edu/lfw/lfw.tgz',
-                      auto_untar=True,
-                      is_gz=True)
-    
+  def __init__(self, train_or_test, dir=None, ext_params=None):
+    super(LFW, self).__init__(train_or_test, dir, ext_params)
+    assert(train_or_test in ['train', 'val', 'test'])
+    if not os.path.exists(self.dir):
+      os.makedirs(self.dir)
+
+    if not os.path.exists(os.path.join(self.dir, 'lfw-deepfunneled')):
+      ali = AliBackend()
+      ali.download('ali:///dataset/lfw/lfw-deepfunneled.tgz', self.dir)
+      ali.download('ali:///dataset/lfw/pairsDevTest.txt', self.dir)
+      ali.download('ali:///dataset/lfw/pairsDevTrain.txt', self.dir)
+      ali.download('ali:///dataset/lfw/peopleDevTest.txt', self.dir)
+      ali.download('ali:///dataset/lfw/peopleDevTrain.txt', self.dir)
+      ali.download('ali:///dataset/lfw/pairs.txt', self.dir)
+      ali.download('ali:///dataset/lfw/people.txt', self.dir)
+
+      os.system(f'cd {self.dir} && tar -xf lfw-deepfunneled.tgz')
+
+    self.purpose = getattr(self, 'purpose', 'development')
+    assert(self.purpose in ['development', 'benchmark'])
+
     # 1.step data folder (wild or align)
-    if self.image_flag == 'align':
-      self._data_folder = os.path.join(self.dir, 'lfw-deepfunneled')
-    else:
-      self._data_folder = os.path.join(self.dir, 'lfw')
-    
+    self._data_folder = os.path.join(self.dir, 'lfw-deepfunneled')
+
     # 2.step data files
     self._persons_list = []
     self._persons_id_str = []
     self._persons_id = []
     for person_id_str in os.listdir(self._data_folder):
       if person_id_str[0] == '.':
         continue
       for person_image in os.listdir(os.path.join(self._data_folder, person_id_str)):
         self._persons_list.append(os.path.join(self._data_folder, person_id_str, person_image))
         self._persons_id_str.append(person_id_str)
-    
+
     id_set = set(self._persons_id_str)
     self.person_id_map = {}
     for s_i, s in enumerate(id_set):
       self.person_id_map[s] = s_i
-    
+
     for person_id_str in self._persons_id_str:
       person_id = self.person_id_map[person_id_str]
       self._persons_id.append(person_id)
-    
     self.ids = list(range(len(self._persons_list)))
 
-    # fixed seed
-    self.seed = time.time()
-
-    self.view = int(getattr(self, 'view', 0))
-    self.pairs = []
-    if self.view == 1:
+    self.same_pairs = []
+    self.diff_pairs = []
+    if self.purpose == 'development':
+      # 区分训练和测试
       if self.train_or_test == 'train':
         with open(os.path.join(self.dir, 'pairsDevTrain.txt')) as fp:
           same_pair_num = fp.readline()
           same_pair_num = int(same_pair_num.strip())
           for pair_i in range(same_pair_num):
             content = fp.readline()
             person_name, image_a, image_b = content.strip().split('\t')
             person_a_image = '%s/%s_%04d.jpg'%(person_name, person_name, int(image_a))
             person_b_image = '%s/%s_%04d.jpg'%(person_name, person_name, int(image_b))
 
-            self.pairs.append((person_a_image, person_b_image))
+            self.same_pairs.append((person_a_image, person_b_image))
 
           content = fp.readline()
           while content:
             content = content.strip()
             if content == '':
               break
             diff_person_a_name, diff_person_a_index, diff_person_b_name, diff_person_b_index = \
               content.split('\t')
 
             diff_person_a_image = '%s/%s_%04d.jpg'%(diff_person_a_name, diff_person_a_name, int(diff_person_a_index))
             diff_person_b_image = '%s/%s_%04d.jpg'%(diff_person_b_name, diff_person_b_name, int(diff_person_b_index))
-            self.pairs.append((diff_person_a_image, diff_person_b_image))
+            self.diff_pairs.append((diff_person_a_image, diff_person_b_image))
 
             content = fp.readline()
       elif self.train_or_test == 'test':
         with open(os.path.join(self.dir, 'pairsDevTest.txt')) as fp:
           same_pair_num = fp.readline()
           same_pair_num = int(same_pair_num.strip())
           for pair_i in range(same_pair_num):
             content = fp.readline()
             person_name, image_a, image_b = content.strip().split('\t')
             person_a_image = '%s/%s_%04d.jpg' % (person_name, person_name, int(image_a))
             person_b_image = '%s/%s_%04d.jpg' % (person_name, person_name, int(image_b))
 
-            self.pairs.append((person_a_image, person_b_image))
+            self.same_pairs.append((person_a_image, person_b_image))
 
           content = fp.readline()
           while content:
             content = content.strip()
             if content == '':
               break
             diff_person_a_name, diff_person_a_index, diff_person_b_name, diff_person_b_index = \
               content.split('\t')
 
             diff_person_a_image = '%s/%s_%04d.jpg' % (diff_person_a_name, diff_person_a_name, int(diff_person_a_index))
             diff_person_b_image = '%s/%s_%04d.jpg' % (diff_person_b_name, diff_person_b_name, int(diff_person_b_index))
-            self.pairs.append((diff_person_a_image, diff_person_b_image))
+            self.diff_pairs.append((diff_person_a_image, diff_person_b_image))
 
             content = fp.readline()
     else:
-      if os.path.exists(os.path.join(self.dir, 'pairs.txt')):
-        pass
-      if os.path.exists(os.path.join(self.dir, 'people.txt')):
-        pass
-    
+      # 不区分训练和测试
+      with open(os.path.join(self.dir, 'pairs.txt')) as fp:
+          for line in fp.readlines()[1:]:
+              pair = line.strip().split()
+              if len(pair) == 3:
+                # same
+                person_name, image_a, image_b = pair
+                person_a_image = '%s/%s_%04d.jpg'%(person_name, person_name, int(image_a))
+                person_b_image = '%s/%s_%04d.jpg'%(person_name, person_name, int(image_b))
+                self.same_pairs.append((person_a_image, person_b_image))
+              else:
+                # diff
+                diff_person_a_name, diff_person_a_index, diff_person_b_name, diff_person_b_index = pair
+                diff_person_a_image = '%s/%s_%04d.jpg' % (diff_person_a_name, diff_person_a_name, int(diff_person_a_index))
+                diff_person_b_image = '%s/%s_%04d.jpg' % (diff_person_b_name, diff_person_b_name, int(diff_person_b_index))
+                self.diff_pairs.append((diff_person_a_image, diff_person_b_image))
+
   @property
   def size(self):
-    if self.view == 0:
-      return len(self.ids)
-    elif self.view == 1:
-      return len(self.pairs)
-    else:
-      return 0
-  
-  def data_pool(self):
-    if self.train_or_test == 'sample':
-      sample_idxs = copy.deepcopy(self.ids)
-      if self.rng:
-        self.rng.shuffle(sample_idxs)
-
-      for index in sample_idxs:
-        yield self.data_samples[index]
-      return
-
-    epoch = 0
-    while True:
-      max_epoches = self.epochs if self.epochs is not None else 1
-      if epoch >= max_epoches:
-        break
-      epoch += 1
-    
-      if self.view == 0:
-        idxs = copy.deepcopy(self.ids)
-        if self.rng:
-          self.rng.shuffle(idxs)
-
-        for k in idxs:
-          person_file = self._persons_list[k]
-          person_image = imread(person_file)
-          person_id_str = self._persons_id_str[k]
-          person_id = self._persons_id[k]
-
-          yield [person_image, {'category_id': person_id,
-                                'category': person_id_str,
-                                'id': k,
-                                'info': [person_image.shape[0], person_image.shape[1], person_image.shape[2]]}]
-      elif self.view == 1:
-        pair_ids = list(range(len(self.pairs)))
-        if self.rng:
-          self.rng.shuffle(pair_ids)
-        for pair_i in pair_ids:
-          person_a, person_b = self.pairs[pair_i]
-          person_a_name = person_a.split('/')[0]
-          person_b_name = person_b.split('/')[0]
-          person_a_path = os.path.join(self._data_folder, person_a)
-          person_a_image = imread(person_a_path)
-          person_b_path = os.path.join(self._data_folder, person_b)
-          person_b_image = imread(person_b_path)
-
-          data = np.stack([person_a_image, person_b_image],0)
-          yield data, {'a_category': person_a_name,
-                       'a_category_id': self.person_id_map[person_a_name],
-                       'b_category': person_b_name,
-                       'b_category_id': self.person_id_map[person_b_name],
-                       'id': pair_i}
-      else:
-        pass
+    return len(self.same_pairs) + len(self.diff_pairs)
 
   def at(self, id):
-    if self.train_or_test == 'sample':
-      return self.data_samples[id]
-
-    if self.view == 0:
-      person_file = self._persons_list[id]
-      person_image = imread(person_file)
-      person_id_str = self._persons_id_str[id]
-      person_id = self._persons_id[id]
-
-      return person_image, {'category_id': person_id,
-                            'category': person_id_str,
-                            'id': id,
-                            'info': [person_image.shape[0], person_image.shape[1], person_image.shape[2]]}
-    elif self.view == 1:
-      pair_i = id
-      person_a, person_b = self.pairs[pair_i]
-      person_a_name = person_a.split('/')[0]
-      person_b_name = person_b.split('/')[0]
-      person_a_path = os.path.join(self.dir, person_a)
-      person_a_image = imread(person_a_path)
-      person_b_path = os.path.join(self.dir, person_b)
-      person_b_image = imread(person_b_path)
-
-      data = np.stack([person_a_image, person_b_image], 0)
-      return data, {'a_category': person_a_name,
-                   'a_category_id': self.person_id_map[person_a_name],
-                   'b_category': person_b_name,
-                   'b_category_id': self.person_id_map[person_b_name],
-                   'id': pair_i}
-    else:
-      pass
-  
-  def split(self, split_params={}, split_method=''):
-    assert (self.train_or_test == 'train')
-    assert (split_method in ['repeated-holdout', 'bootstrap', 'kfold'])
-    
-    category_ids = None
-    if split_method == 'kfold':
-      np.random.seed(np.int64(self.seed))
-      category_ids = [i for i in range(len(self.ids))]
-      np.random.shuffle(category_ids)
-    else:
-      category_ids = [self._persons_id[i] for i in range(len(self.ids))]
-    
-    train_ids, val_ids = self._split(category_ids, split_params, split_method)
-    train_dataset = LFW(self.train_or_test, self.dir, self.ext_params)
-    train_dataset.ids = train_ids
-    
-    val_dataset = LFW(self.train_or_test, self.dir, self.ext_params)
-    val_dataset.ids = val_ids
-    
-    return train_dataset, val_dataset
+    pair_i = id
+    if pair_i < len(self.same_pairs):
+      same_person_a, same_person_b = self.same_pairs[pair_i]
+      same_person_a_path = os.path.join(self._data_folder, same_person_a)
+      same_person_a_image = cv2.imread(same_person_a_path)
+      same_person_b_path = os.path.join(self._data_folder, same_person_b)
+      same_person_b_image = cv2.imread(same_person_b_path)
+      
+      cx = same_person_a_image.shape[1]/2
+      cy = same_person_a_image.shape[0]/2
+      left_t_x = int(cx - 64)
+      left_t_y = int(cy - 64)
+      
+      right_b_x = int(cx + 64)
+      right_b_y = int(cy + 64)
+      
+      crop_a_image = same_person_a_image[left_t_y:right_b_y, left_t_x:right_b_x]
+      crop_b_image = same_person_b_image[left_t_y:right_b_y, left_t_x:right_b_x]
+      return crop_a_image, {
+        'issame': 1,
+        'image_2': crop_b_image,
+        'image_meta': {
+          'image_shape': (crop_a_image.shape[0], crop_a_image.shape[1]),
+          'image_file': same_person_a_path
+        }
+      }
+    else:
+      diff_person_a, diff_person_b = self.diff_pairs[pair_i-len(self.same_pairs)]
+      diff_person_a_path = os.path.join(self._data_folder, diff_person_a)
+      diff_person_a_image = cv2.imread(diff_person_a_path)
+      diff_person_b_path = os.path.join(self._data_folder, diff_person_b)
+      diff_person_b_image = cv2.imread(diff_person_b_path)
+      
+      cx = diff_person_a_image.shape[1]/2
+      cy = diff_person_a_image.shape[0]/2
+      left_t_x = int(cx - 64)
+      left_t_y = int(cy - 64)
+      
+      right_b_x = int(cx + 64)
+      right_b_y = int(cy + 64)
+      
+      crop_a_image = diff_person_a_image[left_t_y:right_b_y, left_t_x:right_b_x]
+      crop_b_image = diff_person_b_image[left_t_y:right_b_y, left_t_x:right_b_x]      
+      return crop_a_image, {
+        'issame': 0,
+        'image_2': crop_b_image,
+        'image_meta': {
+          'image_shape': (crop_a_image.shape[0], crop_a_image.shape[1]),
+          'image_file': diff_person_a_path
+        }
+      }
+
+# lfw = LFW('train', '/root/workspace/dataset/lfw', ext_params={'purpose': 'benchmark'})
+# num = lfw.size
+# for i in range(num):
+#   data = lfw.sample(i)
+#   # print(data.keys())
+#   cv2.imwrite('./a1.png', data['image'][0])
+#   cv2.imwrite('./b1.png', data['image'][1])
+#   print(i)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/lsp.py` & `antgo-0.1.1/antgo/dataflow/dataset/lsp.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from __future__ import print_function
 import sys
 from antgo.dataflow.dataset import *
 import scipy.io as io
 import os
 import numpy as np
 import cv2
+from antgo.framework.helper.fileio.file_client import *
 
 
 __all__ = ['LSP']
 
 class LSP(Dataset):
     def __init__(self, train_or_test, dir=None, ext_params=None):
         super(LSP, self).__init__(train_or_test, dir, ext_params)
@@ -48,32 +49,43 @@
     @property
     def size(self):
         return 2000
 
     def at(self, id):
         image_file = os.path.join(self.dir, 'images', 'im%04d.jpg'%(id+1))
         image = cv2.imread(image_file)
-
+        
+        joints2d = np.transpose(self.dataset[:2,:,id], [1,0])
+        visible = 1-self.dataset[2,:,id]
+        visible_pos = np.where(visible == 1)
+        bboxes = np.array([[
+          np.min(joints2d[visible_pos, 0]), 
+          np.min(joints2d[visible_pos, 1]), 
+          np.max(joints2d[visible_pos, 0]), 
+          np.max(joints2d[visible_pos, 1])
+        ]])
         anno = {
-            'joints2d': np.transpose(self.dataset[:2,:,id], [1,0]),
-            'joints_vis': 1-self.dataset[2,:,id]
+            'bboxes': bboxes,
+            'labels': np.zeros((1), dtype=np.int32),
+            'joints2d': np.expand_dims(joints2d, 0),
+            'joints_vis': np.expand_dims(visible, 0)
         }
         return (image, anno)
 
     def split(self, split_params={}, split_method=''):
         raise NotImplementedError
 
-# lsp = LSP('train', '/root/workspace/handtracking/lsp_dataset')
+# lsp = LSP('train', '/root/workspace/dataset/lsp_dataset')
 # for i in range(10):
 #     data = lsp.sample(i)
 #     image = data['image']
 #     joints2d = data['joints2d']
 #     joints_vis = data['joints_vis']
     
-#     for joint_i, (x,y) in enumerate(joints2d):
+#     for joint_i, (x,y) in enumerate(joints2d[0]):
 #         x, y = int(x), int(y)
         
-#         if joints_vis[joint_i]:
+#         if joints_vis[0][joint_i]:
 #             cv2.circle(image, (x, y), radius=2, color=(0,0,255), thickness=1)
 
 #     cv2.imwrite(f'./aabb/aabb_{i}.png', image)
 #     print(i)
```

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/mnist.py` & `antgo-0.1.1/antgo/dataflow/dataset/mnist.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # -*- coding: UTF-8 -*-
 # File: mnist.py
 # Author: jian(jian@mltalker.com)
 from __future__ import division
 from __future__ import unicode_literals
 from __future__ import print_function
-
+import sys
 import os
 import gzip
 import random
 import numpy as np
-from ...utils import logger
-from .dataset import Dataset
+from antgo.dataflow.dataset.dataset import *
 import time
 import copy
 
 __all__ = ['Mnist']
 MINIST_URL = 'http://yann.lecun.com/exdb/mnist/'
 
 def _read32(bytestream):
@@ -84,45 +83,36 @@
 
 
 class Mnist(Dataset):
   """
   Return [image, label],
       image is 28x28 in the range [0,1]
   """
-  def __init__(self, train_or_test, dir=None, params=None):
+  def __init__(self, train_or_test, dir=None, ext_params=None):
     """
     Args:
         train_or_test: string either 'train' or 'test'
     """
-    super(Mnist,self).__init__(train_or_test, dir, params)
-    assert(train_or_test != 'val')
+    super(Mnist,self).__init__(train_or_test, dir, ext_params=ext_params)
     self.train_or_test = train_or_test
 
-    # read sample data
-    if self.train_or_test == 'sample':
-      self.data_samples, self.ids = self.load_samples()
-      return
-
-    # fixed seed
-    self.seed = time.time()
-
     if self.train_or_test == "train":
       self.download(self.dir, file_names=['train-images-idx3-ubyte.gz'], default_url=MINIST_URL)
       self.train_images = extract_images(os.path.join(self.dir, 'train-images-idx3-ubyte.gz'))
 
-      self.download(self.dir, file_names=['train-labels-idx1-ubyte.gz'])
+      self.download(self.dir, file_names=['train-labels-idx1-ubyte.gz'], default_url=MINIST_URL)
       self.train_labels = extract_labels(os.path.join(self.dir, 'train-labels-idx1-ubyte.gz'))
       self.train = DataSet(self.train_images, self.train_labels)
 
       self.ids = [i for i in range(self.train.num_examples)]
     else:
       self.download(self.dir, file_names=['t10k-images-idx3-ubyte.gz'], default_url=MINIST_URL)
       test_images = extract_images(os.path.join(self.dir,'t10k-images-idx3-ubyte.gz'))
 
-      self.download(self.dir, file_names=['t10k-labels-idx1-ubyte.gz'])
+      self.download(self.dir, file_names=['t10k-labels-idx1-ubyte.gz'], default_url=MINIST_URL)
       test_labels = extract_labels(os.path.join(self.dir, 't10k-labels-idx1-ubyte.gz'))
       self.test = DataSet(test_images, test_labels)
 
       self.ids = [i for i in range(self.test.num_examples)]
 
   def split(self, split_params={}, split_method='holdout'):
       assert(self.train_or_test == 'train')
@@ -131,62 +121,26 @@
       return self, val_dataset
 
   @property
   def size(self):
     return len(self.ids)
 
   def at(self, id):
-    if self.train_or_test == 'sample':
-      return self.data_samples[id]
-
     if self.train_or_test == 'train':
       img = self.train.images[id].reshape((28, 28,1))
       img = np.concatenate([img,img,img],-1)
       img = img.astype(np.uint8)
       label = self.train.labels[id]
 
-      return img, {'id': id, 'category_id': label}
+      return img, label
     else:
       img = self.test.images[id].reshape((28, 28,1))
       img = np.concatenate([img, img, img], -1)
       img = img.astype(np.uint8)
       label = self.test.labels[id]
 
-      return img, {'id': id, 'category_id': label}
-
-  def data_pool(self):
-    if self.train_or_test == 'sample':
-      sample_idxs = copy.deepcopy(self.ids)
-      if self.rng:
-        self.rng.shuffle(sample_idxs)
-
-      for index in sample_idxs:
-        yield self.data_samples[index]
-      return
-
-    ds = None
-    if self.train_or_test == 'train':
-      ds = self.train
-    else:
-      ds = self.test
-
-    self.epoch = 0
-    while True:
-      max_epoches = self.epochs if self.epochs is not None else 1
-      if self.epoch >= max_epoches:
-        break
-      self.epoch += 1
-
-      ids = copy.copy(self.ids)
-      if self.rng:
-        self.rng.shuffle(ids)
-
-      # filter by ids
-      filter_ids = getattr(self, 'filter', None)
-      if filter_ids is not None:
-        ids = [i for i in ids if i in filter_ids]
-
-      for id in ids:
-        img = ds.images[id].reshape((28, 28, 1))
-        label = ds.labels[id]
+      return img, label
 
-        yield img, {'id': id, 'category_id': label}
+# mnist = Mnist('val', "/root/workspace/dataset/temp_dataset")
+# for i in range(mnist.size):
+#   data = mnist.sample(i)
+#   print(i)
```

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/omniglot.py` & `antgo-0.1.1/antgo/dataflow/dataset/omniglot.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/parallel_read.py` & `antgo-0.1.1/antgo/dataflow/dataset/parallel_read.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/pascal_voc.py` & `antgo-0.1.1/antgo/dataflow/dataset/pascal_voc.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,65 +2,58 @@
 # File: pascal_voc.py
 # Author: jian<jian@mltalker.com>
 from __future__ import division
 from __future__ import unicode_literals
 
 import os, sys
 import numpy as np
-import random
-import six
-from six.moves import urllib, range
-import copy
-import logging
 import tarfile
 import xml.etree.ElementTree as ET
-import scipy.sparse
-from antgo.utils.fs import download
 from antgo.utils.fs import maybe_here_match_format
-from antgo.utils import logger, get_rng
 from antgo.dataflow.dataset.dataset import *
-
-__all__ = ['Pascal2007', 'Pascal2012']
-
-PASCAL2007_URL="http://host.robots.ox.ac.uk/pascal/VOC/voc2007"
-PASCAL2012_URL="http://host.robots.ox.ac.uk/pascal/VOC/voc2012"
+from antgo.framework.helper.fileio.file_client import *
 
 
+__all__ = ['Pascal2007', 'Pascal2012']
 class PascalBase(Dataset):
   def __init__(self, year, image_set, dir=None, ext_params=None):
     super(PascalBase, self).__init__(image_set, dir, ext_params)
     if not os.path.exists(self.dir):
       os.makedirs(self.dir)
 
     self._year = year
     self._image_set = image_set
     self._devkit_path = dir
 
-    # read sample data
-    if self.train_or_test == 'sample':
-      self.data_samples, self._image_index = self.load_samples()
-      return
-
     if self._year == '2007':
       if not os.path.exists(os.path.join(self._devkit_path, 'VOCdevkit')):
-        self.download(self.dir, ['VOCtrainval_06-Nov-2007.tar', 'VOCtest_06-Nov-2007.tar'], default_url=PASCAL2007_URL)
+        # self.download(self.dir, ['VOCtrainval_06-Nov-2007.tar', 'VOCtest_06-Nov-2007.tar'], default_url=PASCAL2007_URL)
+        ali = AliBackend()
+        ali.download('ali:///dataset/voc/VOCtrainval_06-Nov-2007.tar', self.dir)
+        ali.download('ali:///dataset/voc/VOCtest_06-Nov-2007.tar', self.dir)
+
       maybe_data_path = maybe_here_match_format(self._devkit_path, 'VOC' + self._year)
       if maybe_data_path is None:
         # auto untar
         tar = tarfile.open(os.path.join(self.dir,'VOCtrainval_06-Nov-2007.tar'), 'r')
         tar.extractall(self.dir)
         tar.close()
 
         tar = tarfile.open(os.path.join(self.dir, 'VOCtest_06-Nov-2007.tar'), 'r')
         tar.extractall(self.dir)
         tar.close()
     else:
       if not os.path.exists(os.path.join(self._devkit_path, 'VOCdevkit')):
-        self.download(self.dir, ['VOCtrainval_11-May-2012.tar'], default_url=PASCAL2012_URL)
-        self.download(self.dir, ['VOC2012test.tar'], default_url='http://host.robots.ox.ac.uk:8080/eval/downloads/')
+        # self.download(self.dir, ['VOCtrainval_11-May-2012.tar'], default_url=PASCAL2012_URL)
+        # self.download(self.dir, ['VOC2012test.tar'], default_url='http://host.robots.ox.ac.uk:8080/eval/downloads/')
+        ali = AliBackend()
+        ali.download('ali:///dataset/voc/VOCtrainval_11-May-2012.tar', self.dir)
+        ali.download('ali:///dataset/voc/VOC2012test.tar', self.dir)
+        ali.download('ali:///dataset/voc/SegmentationClassAug.zip', self.dir)
+        ali.download('ali:///dataset/voc/trainaug.txt', self.dir)
 
       maybe_data_path = maybe_here_match_format(self._devkit_path, 'VOC' + self._year)
       if maybe_data_path is None:
         # auto untar
         try:
           tar = tarfile.open(os.path.join(self.dir, 'VOCtrainval_11-May-2012.tar'), 'r')
           tar.extractall(self.dir)
@@ -71,14 +64,17 @@
         try:
           tar = tarfile.open(os.path.join(self.dir, 'VOC2012test.tar'), 'r')
           tar.extractall(self.dir)
           tar.close()
         except:
           print(f'Untar {os.path.join(self.dir, "VOC2012test.tar")} fail')
 
+        # unzip aug class 
+        os.system(f"cd {self.dir} && unzip SegmentationClassAug.zip")
+   
     self._data_path = os.path.join(self.dir,'VOCdevkit', 'VOC' + self._year)
     self._classes = ('background',
                      'aeroplane',
                      'bicycle',
                      'bird',
                      'boat',
                      'bottle',
@@ -149,99 +145,73 @@
                    'rpn_file': None,
                    'min_size': 2}
 
     assert os.path.exists(self._data_path), 'path does not exist: {}'.format(self._data_path)
 
     self._aug_dataset = []
     self._aug_seg = []
-    if self._year == '2012':
-      train_aug = getattr(self, 'aug', None)
-      task_type = getattr(self, 'task_type', None)
-      if train_aug is not None and task_type == 'SEGMENTATION':
-        if not os.path.exists(os.path.join(self.dir, 'SegmentationClassAug')):
-          os.system(f'cd {self.dir} && wget http://vllab1.ucmerced.edu/~whung/adv-semi-seg/SegmentationClassAug.zip && unzip SegmentationClassAug.zip')
-
-        if not os.path.exists(os.path.join(self.dir, 'trainaug.txt')):
-          os.system(f'cd {self.dir} && wget https://gist.githubusercontent.com/sun11/2dbda6b31acc7c6292d14a872d0c90b7/raw/5f5a5270089239ef2f6b65b1cc55208355b5acca/trainaug.txt')
-  
-        assert(os.path.exists(os.path.join(self.dir, 'SegmentationClassAug')))
-        assert(os.path.exists(os.path.join(self.dir, 'trainaug.txt')))
-        with open(os.path.join(self.dir, 'trainaug.txt'), 'r') as fp:
-          content = fp.readline()
+    if self._year == '2012' and self.train_or_test == 'train':
+      with open(os.path.join(self.dir, 'trainaug.txt'), 'r') as fp:
+        content = fp.readline()
+
+        while(content):
+          content = content.strip()
+          if content == "":
+            break
 
-          while(content):
-            content = content.strip()
-            if content == "":
-              break
-
-            self._aug_dataset.append(os.path.join(self.dir, 'VOCdevkit/VOC2012/JPEGImages', '%s.jpg'%content))
-            self._aug_seg.append(os.path.join(self.dir, 'SegmentationClassAug', '%s.png'%content))
-            content = fp.readline()
+          self._aug_dataset.append(os.path.join(self.dir, 'VOCdevkit/VOC2012/JPEGImages', '%s.jpg'%content))
+          self._aug_seg.append(os.path.join(self.dir, 'SegmentationClassAug', '%s.png'%content))
+          content = fp.readline()
 
   @property
   def size(self):
     return self._image_index_num + len(self._aug_dataset)
 
   def data_pool(self):
     raise NotImplemented
-  
-  def at(self, id):
-    if self.train_or_test == 'sample':
-      return self.data_samples[id]
 
+  def at(self, id):
     if id >= self._image_index_num:
         image_path = self._aug_dataset[id - self._image_index_num]
         image_seg_path = self._aug_seg[id - self._image_index_num]
-        image = imread(image_path)
-        seg_img = imread(image_seg_path)
-        if len(seg_img.shape) == 3:
-          seg_img = seg_img[:,:,0]
-        return [image, {'segments': seg_img}]
+        image = cv2.imread(image_path)
+        seg_img = cv2.imread(image_seg_path, cv2.IMREAD_GRAYSCALE)
+        return (
+          image, 
+          {
+            'segments': seg_img,
+            'image_meta': {
+              'image_shape': (image.shape[0], image.shape[1])
+            }            
+          }
+        )
 
     index = self._image_index[id]
     gt_roidb = self._load_roidb(index)
-    task_type = getattr(self, 'task_type', None)
-    if task_type is not None:
-      if task_type == 'ACTION_CLASSIFICATION':
-        keep_index = []
-        for obj_index, obj_name in enumerate(gt_roidb['category']):
-          if obj_name == 'person':
-            keep_index.append(obj_index)
-
-        if len(keep_index) == 0:
-          return [None, None]
-
-        keep_index = [ki for ki in keep_index if gt_roidb['person_action'][ki] is not None]
-        if len(keep_index) == 0:
-          return [None, None]
-
-        gt_roidb['category_id'] = np.concatenate([gt_roidb['person_action'][ki].reshape((1, -1)) for ki in keep_index])
-        gt_roidb['bbox'] = gt_roidb['bbox'][keep_index, :]
-        gt_roidb['area'] = gt_roidb['area'][keep_index]
-        gt_roidb['difficult'] = [gt_roidb['difficult'][ki] for ki in keep_index]
-
-        gt_roidb.pop('person_action')
-
-    image = imread(self.image_path_from_index(index))
-    gt_roidb['info'] = (image.shape[0], image.shape[1], image.shape[2])
-    gt_roidb['id'] = id
-
-    # [img,groundtruth]
-    return [image, gt_roidb]
-  
+    image = cv2.imread(self.image_path_from_index(index))
+    annos = {
+      'bboxes': gt_roidb['bbox'].astype(np.float32),
+      'labels': gt_roidb['category_id'],
+      'segments': gt_roidb['segments'],
+      'image_meta': {
+        'image_shape': (image.shape[0], image.shape[1])
+      }
+    }
+    return (image, annos)
+
   def image_path_from_index(self, index):
     """
     Construct an image path from the image's "index" identifier.
     """
     image_path = os.path.join(self._data_path, 'JPEGImages',
                               index + self._image_ext)
     assert os.path.exists(image_path), \
             'Path does not exist: {}'.format(image_path)
     return image_path
-    
+
   def image_path_at(self, i):
     """
     Return the absolute path to image i in the image sequence.
     """
     return self.image_path_from_index(self._image_index[i])
 
   def _load_roidb(self, index):
@@ -252,29 +222,22 @@
     Load the indexes listed in this dataset's image set file.
     """
     # Example path to image set file:
     # self._devkit_path + /VOCdevkit2007/VOC2007/ImageSets/Main/val.txt
     image_set_file = os.path.join(self._data_path, 'ImageSets', 'Main',
                                   self._image_set + '.txt')
 
-    task_type = getattr(self, 'task_type', None)
-    if task_type is not None:
-      if task_type == 'ACTION_CLASSIFICATION':
-        image_set_file = os.path.join(self._data_path, 'ImageSets', 'Action',
-                                  self._image_set + '.txt')
-      elif task_type == 'SEGMENTATION':
-        image_set_file = os.path.join(self._data_path, 'ImageSets', 'Segmentation',
-                                  self._image_set + '.txt')
-
+    image_set_file = \
+      os.path.join(self._data_path, 'ImageSets', 'Segmentation', self._image_set + '.txt')
     assert os.path.exists(image_set_file), \
             'Path Does not Exist: {}'.format(image_set_file)
     with open(image_set_file) as f:
         image_index = [x.strip() for x in f.readlines()]
     return image_index
-    
+
   def _load_pascal_annotation(self, index):
     """
     Load image and bounding boxes info from XML file in the PASCAL VOC
     format.
     """
     filename = os.path.join(self._data_path, 'Annotations', index + '.xml')
     tree = ET.parse(filename)
@@ -376,16 +339,18 @@
   def split(self, split_params={}, split_method='holdout'):
     assert (self.train_or_test == 'train')
     assert (split_method == 'holdout')
     validation_pascal2012 = Pascal2012('val', self.dir)
 
     return self, validation_pascal2012
 
-# p2012 = Pascal2012('train', '/root/workspace/dataset/temp_dataset', ext_params={'task_type': 'SEGMENTATION', 'aug': True})
+# p2012 = Pascal2012('val', '/root/workspace/dataset/temp_dataset')
 # print(f'p2012 size {p2012.size}')
 # for i in range(p2012.size):
 #   result = p2012.sample(i)
+#   # ss = result['segments']
+#   # cv2.imwrite('./1234.png', (ss/20*255).astype(np.uint8))
 #   print(i)
 # value = p2012.sample(0)
 # print(value.keys())
 # value = p2012.sample(1)
 # print(value)
```

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/proxy_dataset.py` & `antgo-0.1.1/antgo/dataflow/dataset/proxy_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/queue_dataset.py` & `antgo-0.1.1/antgo/dataflow/dataset/queue_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/random_dataset.py` & `antgo-0.1.1/antgo/dataflow/dataset/random_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/reader.py` & `antgo-0.1.1/antgo/dataflow/dataset/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,14 +326,18 @@
         bs = 0
         while bs != self._batch_size:
             if self._pos >= self.size():
                 break
             
             pos = self.indexes[self._pos]
             sample = self._dataset.sample(pos)
+            if sample is None:
+                # None，需要直接跳过
+                continue
+
             sample["curr_iter"] = self._curr_iter
             self._pos += 1
 
             if self._drop_empty and self._fields and 'gt_mask' in self._fields:
                 if _has_empty(_segm(sample)):
                     #logger.warn('gt_mask is empty or not valid in {}'.format(
                     #    sample['im_file']))
```

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/simpleimages.py` & `antgo-0.1.1/antgo/dataflow/dataset/simpleimages.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/simplevideos.py` & `antgo-0.1.1/antgo/dataflow/dataset/simplevideos.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/spider_dataset.py` & `antgo-0.1.1/antgo/dataflow/dataset/spider_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/dataset/visalso.py` & `antgo-0.1.1/antgo/dataflow/dataset/visalso.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     @property
     def size(self):
         return len(self.image_file_list)
     
     def at(self, id):
         image = cv2.imread(self.image_file_list[id])
         bboxes, labels = self.bboxes_list[id]
-        return (image, {'bboxes': bboxes, 'labels': labels})
+        return (image, {'bboxes': bboxes, 'labels': labels, 'image_meta': {'image_shape': (image.shape[0], image.shape[1])}})
     
     def split(self, split_params={}, split_method=''):
         raise NotImplementedError
 
 # vso = VisalSO('train', './visalso_dataset')
 # for i in range(4):
 #     info = vso.sample(i)
```

### Comparing `antgo-0.1.0/antgo/dataflow/datasetio.py` & `antgo-0.1.1/antgo/dataflow/datasetio.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/imgaug/__init__.py` & `antgo-0.1.1/antgo/dataflow/imgaug/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,15 @@
   ResizeRangeScaling,
   ResizeStepScaling,
   AutoAugmentImage,
   Permute,
   UnSqueeze,
   ConvertRandomObjJointsAndOffset,
   ResizeByShort,
+  RGB2BGR,
   FixedCrop)
 
 __all__ = [
   'DecodeImage', 
   'ResizeS',
   'RandomFlipImage', 
   'RandomDistort', 
@@ -44,9 +45,10 @@
   'ResizeRangeScaling',
   'ResizeStepScaling',
   'AutoAugmentImage',
   'UnSqueeze',
   'ConvertRandomObjJointsAndOffset',
   'ResizeByShort',
   'FixedCrop',
+  'RGB2BGR',
   'Meta'
 ]
```

### Comparing `antgo-0.1.0/antgo/dataflow/imgaug/autoaugment_utils.py` & `antgo-0.1.1/antgo/dataflow/imgaug/autoaugment_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/imgaug/batch_operators.py` & `antgo-0.1.1/antgo/dataflow/imgaug/batch_operators.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/imgaug/colorspace.py` & `antgo-0.1.1/antgo/dataflow/imgaug/colorspace.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/imgaug/functional.py` & `antgo-0.1.1/antgo/dataflow/imgaug/functional.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/imgaug/geometric.py` & `antgo-0.1.1/antgo/dataflow/imgaug/geometric.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/imgaug/gridmask_utils.py` & `antgo-0.1.1/antgo/dataflow/imgaug/gridmask_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/imgaug/op_helper.py` & `antgo-0.1.1/antgo/dataflow/imgaug/op_helper.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/imgaug/operators.py` & `antgo-0.1.1/antgo/dataflow/imgaug/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1381,27 +1381,14 @@
             
             if 'image_meta' in sample and 'transform_matrix' in sample['image_meta']:
                 base_trans = sample['image_meta']['transform_matrix']
                 crop_trans = self.gen_trans_from_bbox((xmin+xmax)/2.0, (ymin+ymax)/2.0, im_width, im_height, im.shape[1], im.shape[0], 1.0, 0.0, inv=False)
                 crop_trans = np.matmul(crop_trans, base_trans)
                 sample['image_meta']['transform_matrix'] = crop_trans
 
-            # # 测试可视化
-            # for bi in range(len(crop_bbox)):
-            #     x0,y0,x1,y1 = sample['gt_bbox'][bi]
-            #     cls_label = crop_class[bi]
-            #     x0=(int)(x0)
-            #     y0=(int)(y0)
-            #     x1=(int)(x1)
-            #     y1=(int)(y1)
-            #     color_v = (255,0,0)
-            #     if cls_label == 0:
-            #         color_v = (0,0,255)
-            #     cv2.rectangle(im, (x0,y0),(x1,y1), color_v, 4)
-            # cv2.imwrite("./crop_show.png", im)
             return sample
         return sample
 
 
 # FINISH FIX
 class NormalizeBox(BaseOperator):
     # FINISH CORRET (JIAN)
@@ -1450,36 +1437,48 @@
         self.channel_first = channel_first
         if not (isinstance(self.to_bgr, bool) and
                 isinstance(self.channel_first, bool)):
             raise TypeError("{}: input type is invalid.".format(self))
 
     def __call__(self, sample, context=None):
         assert 'image' in sample, "image data not found"
-        for k in sample.keys():
-            # hard code
-            if k == 'image':
-                im = sample[k]
-                if self.channel_first:
-                    im = np.swapaxes(im, 1, 2)
-                    im = np.swapaxes(im, 1, 0)
-                if self.to_bgr:
-                    im = im[[2, 1, 0], :, :]
-                sample[k] = im
-                
-            if k == 'segments':
-                label = sample[k]
-                if self.channel_first:
-                    label = np.expand_dims(label, 0)
-                else:
-                    label = np.expand_dims(label, -1)
-                sample[k] = label
-
+        if 'image' in sample.keys():
+            im = sample["image"]
+            if self.channel_first:
+                im = np.swapaxes(im, 1, 2)
+                im = np.swapaxes(im, 1, 0)
+            if self.to_bgr:
+                im = im[[2, 1, 0], :, :]
+            sample["image"] = im
+
+        if 'segments' in sample.keys():
+            label = sample['segments']
+            if self.channel_first:
+                label = np.expand_dims(label, 0)
+            else:
+                label = np.expand_dims(label, -1)
+            sample['segments'] = label
         return sample
 
 
+class RGB2BGR(BaseOperator):
+    # FINISH CORRET (JIAN)
+    def __init__(self, inputs=None):
+        super(RGB2BGR, self).__init__(inputs=inputs)
+
+    def __call__(self, sample, context=None):
+        assert 'image' in sample, "image data not found"
+        if 'image' in sample.keys():
+            sample["image"] = cv2.cvtColor(sample["image"], cv2.COLOR_BGR2RGB)
+        
+        if 'image_2' in sample.keys():
+            sample["image_2"] = cv2.cvtColor(sample["image_2"], cv2.COLOR_BGR2RGB)
+
+        return sample
+
 # FINISH FIX
 class MixupImage(BaseOperator):
     def __init__(self, prob=0.5, alpha=1.5, beta=1.5, inputs=None):
         """ Mixup image and gt_bbbox/gt_score
         Args:
             alpha (float): alpha parameter of beta distribute
             beta (float): beta parameter of beta distribute
@@ -1797,26 +1796,22 @@
         sample['image_meta']['image_shape'] = (resize_h, resize_w)
         sample['image_meta']['scale_factor'] =  [scale_x, scale_y] * 2
         sample['height'] = resize_h
         sample['width'] = resize_w
         sample['image'] = cv2.resize(
             sample['image'], (resize_w, resize_h), interpolation=self.interp_dict[interp])
         
+        if 'image_2' in sample:
+            sample['image_2'] = cv2.resize(
+                sample['image_2'], (resize_w, resize_h), interpolation=self.interp_dict[interp])
+
         # vis_2d_boxes_in_image(sample['image'], sample['bboxes'],sample['labels'], './b.png')
         return sample
 
-    def reset(self, target_dim):
-        if type(target_dim) == list or type(target_dim) == tuple:
-            self.target_dim = target_dim                # w,h
-        else:
-            self.target_dim = [target_dim, target_dim]  # w,h
-
-    def get(self):
-        return self.target_dim
-
+    
 # FINSH FIX
 class ColorDistort(BaseOperator):
     """Random color distortion.
     Args:
         hue (list): hue settings.
             in [lower, upper, probability] format.
         saturation (list): saturation settings.
@@ -2482,14 +2477,15 @@
             sample['joints2d'] = joints2d            
 
         if 'segments' in sample and sample['segments'].size != 0:
             segments = sample['segments']
             segments = resize(segments, (w, h), cv2.INTER_NEAREST)
             sample['segments'] = segments
 
+        sample['image_meta']['image_shape'] = sample['image'].shape[:2]
         return sample
 
 
 # FINISH FIX
 class ResizeRangeScaling(BaseOperator):
     """对图像长边随机resize到指定范围内，短边按比例进行缩放。当存在标注图像时，则同步进行处理。
 
@@ -2542,57 +2538,82 @@
             sample['joints2d'] = joints2d            
         
         if 'segments' in sample and sample['segments'].size != 0:
             segments = sample['segments']
             segments, _ = resize_long(segments, random_size, cv2.INTER_NEAREST)
             sample['segments'] = segments
 
+        sample['image_meta']['image_shape'] = sample['image'].shape[:2]
         return sample
 
 
 # FINISH FIX
 class ResizeByShort(BaseOperator):
-    def __init__(self, short_size, inputs=None):
+    def __init__(self, short_size, max_size=1024,inputs=None):
         super().__init__(inputs=inputs)
         self.short_size = short_size
+        self.max_size = max_size
+        self.is_range = False
+        if isinstance(self.short_size, list) or isinstance(self.short_size, tuple):
+            self.is_range = True
 
     def __call__(self, sample, context=None):
         im = sample['image']
-        im, scale = resize_short(im, self.short_size)
+        short_size = self.short_size
+        if self.is_range:
+            short_size = np.random.choice(self.short_size)
+        
+        value = min(im.shape[0], im.shape[1])
+        scale = float(short_size) / float(value)
+        newh = im.shape[0] * scale
+        neww = im.shape[1] * scale
+        if max(newh, neww) > self.max_size:
+            scale = self.max_size * 1.0 / max(newh, neww)
+            newh = newh * scale
+            neww = neww * scale
+            short_size = min(newh, neww)
+
+        # 短边resize
+        im, scale = resize_short(im, short_size)
         sample['image'] = im
 
         if 'bboxes' in sample and len(sample['bboxes']) > 0:
             scale_array = np.array([scale, scale] * 2, dtype=np.float32)      
             boxes = sample['bboxes'] * scale_array
             sample['bboxes'] = boxes
 
         if 'joints2d' in sample and len(sample['joints2d']) > 0:
             scale_array = np.array([scale, scale], dtype=np.float32).reshape(1,1,2) 
             joints2d = sample['joints2d'] * scale_array
             sample['joints2d'] = joints2d            
 
         if 'segments' in sample and sample['segments'].size != 0:
             segments = sample['segments']
-            segments, _ = resize_long(segments, self.short_size, cv2.INTER_NEAREST)
+            segments, _ = resize_short(segments, short_size, cv2.INTER_NEAREST)
             sample['segments'] = segments
 
+        sample['image_meta']['image_shape'] = sample['image'].shape[:2]
+        # vis_2d_boxes_in_image(sample['image'].copy(), sample['bboxes'],sample['labels'], './b.png')
         return sample
 
 
 # FINISH FIX
 class ResizeByLong(BaseOperator):
     """对图像长边resize到固定值，短边按比例进行缩放。当存在标注图像时，则同步进行处理。
 
     Args:
         long_size (int): resize后图像的长边大小。
     """
 
     def __init__(self, long_size, inputs=None):
         super(ResizeByLong, self).__init__(inputs=inputs)
         self.long_size = long_size
+        self.is_range = False
+        if isinstance(self.long_size, list) or isinstance(self.long_size, tuple):
+            self.is_range = True
 
     def __call__(self, sample, context=None):
         """
         Args:
             im (np.ndarray): 图像np.ndarray数据。
             im_info (dict): 存储与图像相关的信息。
             label (np.ndarray): 标注图像np.ndarray数据。
@@ -2601,26 +2622,31 @@
             tuple: 当label为空时，返回的tuple为(im, im_info)，分别对应图像np.ndarray数据、存储与图像相关信息的字典；
                 当label不为空时，返回的tuple为(im, im_info, label)，分别对应图像np.ndarray数据、
                 存储与图像相关信息的字典和标注图像np.ndarray数据。
                 其中，im_info新增字段为：
                     -shape_before_resize (tuple): 保存resize之前图像的形状(h, w）。
         """
         im = sample['image']
-        im, scale = resize_long(im, self.long_size)
+        long_size = self.long_size
+        if self.is_range:
+            long_size = np.random.choice(self.long_size)
+        
+        im, scale = resize_long(im, long_size)
         sample['image'] = im
                 
         if 'bboxes' in sample and len(sample['bboxes']) > 0:
             scale_array = np.array([scale, scale] * 2, dtype=np.float32)      
             boxes = sample['bboxes'] * scale_array
             sample['bboxes'] = boxes
         
         if 'joints2d' in sample and len(sample['joints2d']) > 0:
             scale_array = np.array([scale, scale], dtype=np.float32).reshape(1,1,2) 
             joints2d = sample['joints2d'] * scale_array
             sample['joints2d'] = joints2d            
         
         if 'segments' in sample and sample['segments'].size != 0:
             segments = sample['segments']
-            segments, _ = resize_long(segments, self.long_size, cv2.INTER_NEAREST)
+            segments, _ = resize_long(segments, long_size, cv2.INTER_NEAREST)
             sample['segments'] = segments
 
+        sample['image_meta']['image_shape'] = sample['image'].shape[:2]
         return sample
```

### Comparing `antgo-0.1.0/antgo/dataflow/imgaug/operators_3d.py` & `antgo-0.1.1/antgo/dataflow/imgaug/operators_3d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/imgaug/photometric.py` & `antgo-0.1.1/antgo/dataflow/imgaug/photometric.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/imgaug/regular.py` & `antgo-0.1.1/antgo/dataflow/imgaug/regular.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/imgaug/util.py` & `antgo-0.1.1/antgo/dataflow/imgaug/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/recorder.py` & `antgo-0.1.1/antgo/dataflow/recorder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/dataflow/vis.py` & `antgo-0.1.1/antgo/dataflow/vis.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/activelearning.py` & `antgo-0.1.1/antgo/framework/helper/activelearning.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/apis/train.py` & `antgo-0.1.1/antgo/framework/helper/apis/train.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/base_module.py` & `antgo-0.1.1/antgo/framework/helper/base_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/base_trainer.py` & `antgo-0.1.1/antgo/framework/helper/base_trainer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/__init__.py` & `antgo-0.1.1/antgo/framework/helper/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/alexnet.py` & `antgo-0.1.1/antgo/framework/helper/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/backbone/ddr_lcnet.py` & `antgo-0.1.1/antgo/framework/helper/cnn/backbone/ddr_lcnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/backbone/ddr_mobilenet_v2.py` & `antgo-0.1.1/antgo/framework/helper/cnn/backbone/ddr_mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/__init__.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/activation.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/context_block.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/conv.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/conv2d_adaptive_padding.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/conv_module.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/conv_ws.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/depthwise_separable_conv_module.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/drop.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/generalized_attention.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/hsigmoid.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/hswish.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/inverted_residual.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/make_divisible.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/make_divisible.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/non_local.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/norm.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/padding.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/plugin.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/registry.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/registry.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/scale.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/se_layer.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/se_layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/transformer.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/upsample.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/waterfall.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/waterfall.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/bricks/wrappers.py` & `antgo-0.1.1/antgo/framework/helper/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/resnet.py` & `antgo-0.1.1/antgo/framework/helper/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/utils/__init__.py` & `antgo-0.1.1/antgo/framework/helper/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/utils/flops_counter.py` & `antgo-0.1.1/antgo/framework/helper/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/utils/fuse_conv_bn.py` & `antgo-0.1.1/antgo/framework/helper/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/utils/sync_bn.py` & `antgo-0.1.1/antgo/framework/helper/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/utils/weight_init.py` & `antgo-0.1.1/antgo/framework/helper/cnn/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/cnn/vgg.py` & `antgo-0.1.1/antgo/framework/helper/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/configs/activelearning/ac_config.py` & `antgo-0.1.1/antgo/framework/helper/configs/activelearning/ac_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/configs/adda/adda_config.py` & `antgo-0.1.1/antgo/framework/helper/configs/adda/adda_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/configs/semi/dense_config.py` & `antgo-0.1.1/antgo/framework/helper/configs/semi/dense_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 # 学习率调度配置
 lr_config = dict(
     policy='CosineAnnealing',
     min_lr=1e-5,
 )
 
+# 日志配置
+log_config = dict(
+    interval=1,    
+    hooks=[
+        dict(type='TextLoggerHook'),
+    ])
+
 # 模型配置
 # model 字段根据具体模型进行设置
 model = dict(
     type='DenseTeacher',
     train_cfg=dict(
         key=0,
         use_sigmoid=True,
```

### Comparing `antgo-0.1.0/antgo/framework/helper/configs/semi/mpl_config.py` & `antgo-0.1.1/antgo/framework/helper/configs/semi/mpl_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/__init__.py` & `antgo-0.1.1/antgo/framework/helper/dataset/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .dataset_wrappers import (ConcatDataset, IterConcatDataset, RepeatDataset)
 from .pipelines import *
 from .dataset_split import DatasetSamplingByClass
 from .dataset_filter import IterableDatasetFilter
 from .tfdataset import *
 from antgo.dataflow import dataset as local_dataset
 from antgo.framework.helper.reader import *
+import torchvision
 
 
 def register_antgo_dataset():
     for dataset_module_name in local_dataset.__all__:
         if dataset_module_name == 'Dataset':
             continue
 
@@ -26,10 +27,33 @@
             )
         DATASETS.register_module()(dataset_module_reader)
 
 
 register_antgo_dataset()
 
 
+def register_torchvision_dataset():
+    needed_torchvision_dataset = ['ImageFolder']
+    for dataset_module_name in needed_torchvision_dataset:
+        if dataset_module_name.startswith('__'):
+            continue
+
+        dataset_module_reader = \
+            type(
+                dataset_module_name, 
+                (TVReader,), 
+                {   
+                    'name': dataset_module_name,
+                    '__doc__': f'{dataset_module_name} reader', 
+                    '__init__': lambda self, pipeline=None, weak_pipeline=None, strong_pipeline=None, inputs_def=None, **kwargs: 
+                        TVReader.__init__(self, getattr(torchvision.datasets, self.name)(**kwargs), pipeline=pipeline, weak_pipeline=weak_pipeline, strong_pipeline=strong_pipeline, inputs_def=inputs_def)
+                }
+            )
+        DATASETS.register_module()(dataset_module_reader)
+
+
+register_torchvision_dataset()
+
+
 __all__ = [
     'DATASETS','build_dataloader','build_dataset','ConcatDataset', 'IterConcatDataset','RepeatDataset', 'TFDataset', 'DatasetSamplingByClass', 'IterableDatasetFilter'
 ]
```

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/builder.py` & `antgo-0.1.1/antgo/framework/helper/dataset/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
     elif persistent_workers is True:
         warnings.warn('persistent_workers is invalid because your pytorch '
                       'version is lower than 1.7.0')
 
     init_fn = partial(
         worker_init_fn, num_workers=num_workers, rank=rank,
         seed=seed) if seed is not None else None
-        
+
     data_loader = DataLoader(
         dataset,
         batch_size=int(batch_size),
         sampler=sampler,
         num_workers=num_workers,
         batch_sampler=batch_sampler,
         collate_fn=partial(collate, samples_per_gpu=samples_per_gpu, ignore_stack=ignore_stack),
```

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/dataset_filter.py` & `antgo-0.1.1/antgo/framework/helper/dataset/dataset_filter.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/dataset_split.py` & `antgo-0.1.1/antgo/framework/helper/dataset/dataset_split.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/dataset_wrappers.py` & `antgo-0.1.1/antgo/framework/helper/dataset/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/kvdataset.py` & `antgo-0.1.1/antgo/framework/helper/dataset/kvdataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/pipelines/auto_augment.py` & `antgo-0.1.1/antgo/framework/helper/dataset/pipelines/auto_augment.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/pipelines/builder.py` & `antgo-0.1.1/antgo/framework/helper/dataset/pipelines/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/pipelines/formatting.py` & `antgo-0.1.1/antgo/framework/helper/dataset/pipelines/formatting.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/pipelines/transforms.py` & `antgo-0.1.1/antgo/framework/helper/dataset/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/samplers/__init__.py` & `antgo-0.1.1/antgo/framework/helper/dataset/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/samplers/class_aware_sampler.py` & `antgo-0.1.1/antgo/framework/helper/dataset/samplers/class_aware_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/samplers/distributed_sampler.py` & `antgo-0.1.1/antgo/framework/helper/dataset/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/samplers/group_sampler.py` & `antgo-0.1.1/antgo/framework/helper/dataset/samplers/group_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/samplers/infinite_sampler.py` & `antgo-0.1.1/antgo/framework/helper/dataset/samplers/infinite_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/samplers/kv_sampler.py` & `antgo-0.1.1/antgo/framework/helper/dataset/samplers/kv_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 
 # 将 index iterable 转化为 batch index iterable
 # 如 chunk([4, 2, 3, 1], 2) ==> [[4, 2], [3, 1]]
 def _chunk(iterable, chunk_size):
     ret = []
     for record in iterable:
+        if record is None:
+            # 跳过 None，会造成组成的batch中，不满足预先指定的方案
+            continue
+
         ret.append(record)
         if len(ret) == chunk_size:
             yield ret
             ret = []
     if ret:
         yield ret
```

### Comparing `antgo-0.1.0/antgo/framework/helper/dataset/tfdataset.py` & `antgo-0.1.1/antgo/framework/helper/dataset/tfdataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/exporter.py` & `antgo-0.1.1/antgo/framework/helper/exporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,44 @@
 import os
 import torch
 from antgo.framework.helper.utils.config import Config
 from antgo.framework.helper.runner.builder import *
 from antgo.framework.helper.models.builder import *
 from thop import profile
 import json
-
+from collections import OrderedDict
+import re
 
 class Exporter(object):
     def __init__(self, cfg, work_dir):
         if isinstance(cfg, dict):
             self.cfg = Config.fromstring(json.dumps(cfg), '.json')
         else:
             self.cfg = cfg
         self.work_dir = work_dir
 
-    def export(self, input_tensor_list, input_name_list, output_name_list=None, checkpoint=None, model_builder=None, prefix='model'):
+    def export(self, input_tensor_list, input_name_list, output_name_list=None, checkpoint=None, model_builder=None, prefix='model', revise_keys=[]):
         model = None
         if model_builder is not None:
             model = model_builder()
         else:
             model = build_model(self.cfg.model)
 
         # 加载checkpoint
         if checkpoint is not None:
             ckpt = torch.load(checkpoint, map_location='cpu')
-            model.load_state_dict(ckpt['state_dict'], strict=True)
+            state_dict = ckpt
+            if 'state_dict' in ckpt:
+                state_dict = ckpt['state_dict']
+
+            for p, r in revise_keys:
+                state_dict = OrderedDict(
+                    {re.sub(p, r, k): v
+                    for k, v in state_dict.items()})
+            model.load_state_dict(state_dict, strict=True)
 
         # 获得浮点模型的 FLOPS、PARAMS
         model.eval()
         model.forward = model.onnx_export
         model = model.to('cpu')
         if isinstance(input_tensor_list, list):
             for i in range(len(input_tensor_list)):
```

### Comparing `antgo-0.1.0/antgo/framework/helper/fileio/__init__.py` & `antgo-0.1.1/antgo/framework/helper/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/fileio/file_client.py` & `antgo-0.1.1/antgo/framework/helper/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/fileio/handlers/base.py` & `antgo-0.1.1/antgo/framework/helper/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/fileio/handlers/json_handler.py` & `antgo-0.1.1/antgo/framework/helper/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/fileio/handlers/pickle_handler.py` & `antgo-0.1.1/antgo/framework/helper/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/fileio/handlers/yaml_handler.py` & `antgo-0.1.1/antgo/framework/helper/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/fileio/io.py` & `antgo-0.1.1/antgo/framework/helper/fileio/io.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/fileio/parse.py` & `antgo-0.1.1/antgo/framework/helper/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/metrics/kp2d.py` & `antgo-0.1.1/antgo/framework/helper/metrics/kp2d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/metrics/metrics.py` & `antgo-0.1.1/antgo/framework/helper/metrics/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 dataset = gt_ann
             self.dataset = dataset
             self.createIndex()    
 
 
 @MEASURES.register_module()
 class COCOCompatibleEval(object):
-    def __init__(self, categories=[{'name': 'left', 'id': 1},{'name': 'right', 'id': 2}], without_background=True):
+    def __init__(self, categories, without_background=True):
         self.categories = categories
         for c in self.categories:
             if 'supercategory' not in c:
                 c['supercategory'] = 'default'
         
         self.without_background = without_background
     
@@ -74,16 +74,16 @@
                     "category_id": category_id,
                     "id": bbox_id+1,
                     'ignore': 0
                 })
                 bbox_id += 1
 
             images.append({
-                'height': 480,
-                'width': 640,
+                'height': gt['image_meta']['image_shape'][0],
+                'width': gt['image_meta']['image_shape'][1],
                 'id': image_id+1,
                 'file_name': image_file
             })
 
         gt_coco = COCOWarp({
             'images': images,
             'categories': self.categories,
```

### Comparing `antgo-0.1.0/antgo/framework/helper/metrics/seg2d.py` & `antgo-0.1.1/antgo/framework/helper/metrics/seg2d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/activelearning/acnet.py` & `antgo-0.1.1/antgo/framework/helper/models/activelearning/acnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/adda/adda.py` & `antgo-0.1.1/antgo/framework/helper/models/adda/adda.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/builder.py` & `antgo-0.1.1/antgo/framework/helper/models/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/classification/backbones/hrnet.py` & `antgo-0.1.1/antgo/framework/helper/models/classification/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/classification/backbones/mobilenet_v2.py` & `antgo-0.1.1/antgo/framework/helper/models/classification/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/classification/backbones/resnet.py` & `antgo-0.1.1/antgo/framework/helper/models/classification/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/classification/backbones/resnext.py` & `antgo-0.1.1/antgo/framework/helper/models/classification/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/classification/heads/cls_head.py` & `antgo-0.1.1/antgo/framework/helper/models/classification/heads/cls_head.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,56 +19,38 @@
         cal_acc (bool): Whether to calculate accuracy during training.
             If you use Mixup/CutMix or something like that during training,
             it is not reasonable to calculate accuracy. Defaults to False.
     """
 
     def __init__(self,
                  loss=dict(type='CrossEntropyLoss', loss_weight=1.0, class_weight=None),
-                 topk=(1, ),
-                 cal_acc=False,
-                 init_cfg=None):
+                 init_cfg=dict(use_softmax=True)):
         super().__init__()
 
         assert isinstance(loss, dict)
-        assert isinstance(topk, (int, tuple))
-        if isinstance(topk, int):
-            topk = (topk, )
-        for _topk in topk:
-            assert _topk > 0, 'Top-k should be larger than 0'
-        self.topk = topk
-
         self.compute_loss = CrossEntropyLoss(loss_weight=loss['loss_weight'], class_weight=loss['class_weight'])
-        self.compute_accuracy = Accuracy(topk=self.topk)
-        self.cal_acc = cal_acc
+        self.use_softmax = init_cfg.get('use_softmax', True)
 
     def loss(self, cls_score, gt_label, **kwargs):
         num_samples = len(cls_score)
         losses = dict()
         # compute loss
         loss = self.compute_loss(
             cls_score, gt_label, avg_factor=num_samples, **kwargs)
-        if self.cal_acc:
-            # compute accuracy
-            acc = self.compute_accuracy(cls_score, gt_label)
-            assert len(acc) == len(self.topk)
-            losses['accuracy'] = {
-                f'top-{k}': a
-                for k, a in zip(self.topk, acc)
-            }
         losses['loss'] = loss
         return losses
 
     def forward_train(self, cls_score, gt_label, **kwargs):
         if isinstance(cls_score, tuple):
             cls_score = cls_score[-1]
             
         losses = self.loss(cls_score, gt_label.view(-1), **kwargs)
         return losses
 
-    def simple_test(self, x, softmax=True, post_process=True, **kwargs):
+    def simple_test(self, x):
         """Inference without augmentation.
 
     Args:
             x (tuple[Tensor]): The input features.
                 Multi-stage inputs are acceptable but only the last stage will
                 be used to classify. The shape of every item should be
                 ``(num_samples, in_channels)``.
@@ -82,23 +64,18 @@
                 - If no post processing, the output is a tensor with shape
                   ``(num_samples, num_classes)``.
                 - If post processing, the output is a multi-dimentional list of
                   float and the dimensions are ``(num_samples, num_classes)``.
         """
         cls_score = self.pre_logits(x)
 
-        if softmax:
+        if self.use_softmax:
             pred = (
                 F.softmax(cls_score, dim=1) if cls_score is not None else None)
         else:
             pred = cls_score
         return pred
 
     def pre_logits(self, x):
         if isinstance(x, tuple):
             x = x[-1]
-
-        warnings.warn(
-            'The input of ClsHead should be already logits. '
-            'Please modify the backbone if you want to get pre-logits feature.'
-        )
         return x
```

### Comparing `antgo-0.1.0/antgo/framework/helper/models/classification/heads/stacked_head.py` & `antgo-0.1.1/antgo/framework/helper/models/classification/heads/stacked_head.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/classification/losses/accuracy.py` & `antgo-0.1.1/antgo/framework/helper/models/classification/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/classification/losses/cross_entropy_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/classification/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/classification/losses/utils.py` & `antgo-0.1.1/antgo/framework/helper/models/classification/losses/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/classification/model/base.py` & `antgo-0.1.1/antgo/framework/helper/models/classification/model/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/base.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,17 +58,15 @@
             image_meta (list[dict]): List of image info dict where each dict
                 has: 'img_shape', 'scale_factor', 'flip', and may also contain
                 'filename', 'ori_shape', 'pad_shape', and 'img_norm_cfg'.
                 For details on the values of these keys, see
                 :class:`mmdet.datasets.pipelines.Collect`.
             kwargs (keyword arguments): Specific to concrete implementation.
         """
-        batch_input_shape = tuple(image[0].size()[-2:])
-        for img_meta in image_meta:
-            img_meta['batch_input_shape'] = batch_input_shape
+        pass
 
     @abstractmethod
     def simple_test(self, image, image_meta, **kwargs):
         pass
 
     def forward_test(self, image, image_meta, **kwargs):
         """
@@ -76,19 +74,14 @@
             image (List[Tensor]): the outer list indicates test-time
                 augmentations and inner Tensor should have a shape NxCxHxW,
                 which contains all images in the batch.
             image_meta (List[List[dict]]): the outer list indicates test-time
                 augs (multiscale, flip, etc.) and the inner list indicates
                 images in a batch.
         """
-        batch_size = len(image_meta)
-        for img_id in range(batch_size):
-            image_meta[img_id]['batch_input_shape'] = tuple(image.size()[-2:])
-
-        # assert(num_augs == 1)
         return self.simple_test(image, image_meta, **kwargs)
 
     def forward(self, image, image_meta, return_loss=True, **kwargs):
         """Calls either :func:`forward_train` or :func:`forward_test` depending
         on whether ``return_loss`` is ``True``.
 
         Note this setting will change the expected inputs. When
```

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/anchor/__init__.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/anchor/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/anchor/anchor_generator.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/anchor/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/anchor/builder.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/anchor/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/anchor/point_generator.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/anchor/point_generator.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/anchor/utils.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/anchor/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/__init__.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/__init__.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/approx_max_iou_assigner.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/approx_max_iou_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/assign_result.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/assign_result.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/atss_assigner.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/atss_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/center_region_assigner.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/center_region_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/grid_assigner.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/grid_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/hungarian_assigner.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/hungarian_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/max_iou_assigner.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/max_iou_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/point_assigner.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/point_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/region_assigner.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/region_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/sim_ota_assigner.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/sim_ota_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/assigners/uniform_assigner.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/assigners/uniform_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/builder.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/__init__.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/bucketing_bbox_coder.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/bucketing_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/delta_xywh_bbox_coder.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/delta_xywh_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/distance_point_bbox_coder.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/distance_point_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/legacy_delta_xywh_bbox_coder.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/legacy_delta_xywh_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/pseudo_bbox_coder.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/pseudo_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/tblr_bbox_coder.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/tblr_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/coder/yolo_bbox_coder.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/coder/yolo_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/iou2d_calculator.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/iou2d_calculator.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/match_costs/match_cost.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/match_costs/match_cost.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/__init__.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/base_sampler.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/base_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/combined_sampler.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/combined_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/instance_balanced_pos_sampler.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/instance_balanced_pos_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/iou_balanced_neg_sampler.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/iou_balanced_neg_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/ohem_sampler.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/ohem_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/pseudo_sampler.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/pseudo_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/random_sampler.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/sampling_result.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/sampling_result.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/samplers/score_hlr_sampler.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/samplers/score_hlr_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/bbox/transforms.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/bbox/transforms.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/mask/mask_target.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/mask/mask_target.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/mask/structures.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/mask/structures.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/mask/utils.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/mask/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/utils/__init__.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/utils/dist_utils.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/utils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/core/utils/misc.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/head/base_dense_head.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/head/base_dense_head.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/head/fcos_head.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/head/fcos_head.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,35 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch
 import torch.nn as nn
 from antgo.framework.helper.cnn import bias_init_with_prob, normal_init
 from antgo.framework.helper.models.builder import HEADS, build_loss
 from antgo.framework.helper.models.detectors.core.utils import multi_apply
 from torchvision.ops import batched_nms 
 from ..utils.gaussian_target import gaussian_radius, gen_gaussian_target
 from ..utils.gaussian_target import (get_local_maximum, get_topk_from_heatmap,
                                      transpose_and_gather_feat)
 from .base_dense_head import BaseDenseHead
 import torch.nn.functional as F
-import numpy as np
-import cv2 
 
 
-def sigmoid_focal_loss(
-    inputs: torch.Tensor,
-    targets: torch.Tensor,
-    alpha: float = -1,
-    gamma: float = 2,
-    reduction: str = "none",
-) -> torch.Tensor:
-    """
-    Loss used in RetinaNet for dense detection: https://arxiv.org/abs/1708.02002.
+def iou_loss(preds, targets):
+    '''
     Args:
-        inputs: A float tensor of arbitrary shape.
-                The predictions for each example.
-        targets: A float tensor with the same shape as inputs. Stores the binary
-                 classification label for each element in inputs
-                (0 for the negative class and 1 for the positive class).
-        alpha: (optional) Weighting factor in range (0,1) to balance
-                positive vs negative examples. Default = -1 (no weighting).
-        gamma: Exponent of the modulating factor (1 - p_t) to
-               balance easy vs hard examples.
-        reduction: 'none' | 'mean' | 'sum'
-                 'none': No reduction will be applied to the output.
-                 'mean': The output will be averaged.
-                 'sum': The output will be summed.
-    Returns:
-        Loss tensor with the reduction option applied.
-    """
-    inputs = inputs.float()
-    targets = targets.float()
-    p = torch.sigmoid(inputs)
-    ce_loss = F.binary_cross_entropy_with_logits(inputs, targets, reduction="none")
-    p_t = p * targets + (1 - p) * (1 - targets)
-    loss = ce_loss * ((1 - p_t) ** gamma)
-
-    if alpha >= 0:
-        alpha_t = alpha * targets + (1 - alpha) * (1 - targets)
-        loss = alpha_t * loss
-
-    if reduction == "mean":
-        loss = loss.mean()
-    elif reduction == "sum":
-        loss = loss.sum()
-
-    return loss
-
+    preds: [n,4] ltrb
+    targets: [n,4]
+    '''
+    lt = torch.min(preds[:, :2], targets[:, :2])
+    rb = torch.min(preds[:, 2:], targets[:, 2:])
+    wh = (rb + lt).clamp(min=0)
+    overlap = wh[:, 0] * wh[:, 1]  # [n]
+    area1 = (preds[:, 2] + preds[:, 0]) * (preds[:, 3] + preds[:, 1])
+    area2 = (targets[:, 2] + targets[:, 0]) * (targets[:, 3] + targets[:, 1])
+    iou = overlap / (area1 + area2 - overlap)
+    loss = -iou.clamp(min=1e-6).log()
+    return loss.sum()
 
 
 @HEADS.register_module()
 class FcosHead(BaseDenseHead):
     """Objects as Points Head. CenterHead use center_point to indicate object's
     position. Paper link <https://arxiv.org/abs/1904.07850>
 
@@ -86,56 +54,28 @@
                  feat_channel,
                  num_classes,
                  down_stride,
                  rescale=1.0,
                  score_thresh=0.15,
                  loss_ch=dict(
                      type='GaussianFocalLoss', loss_weight=1.0),
-                 loss_wh=dict(type='L1Loss', loss_weight=0.1),
                  train_cfg=None,
                  test_cfg=None,
                  init_cfg=None):
         super(FcosHead, self).__init__(init_cfg)
         self.num_classes = num_classes
         self.rescale_x, self.rescale_y = rescale if type(rescale) == list or type(rescale) == tuple else (rescale, rescale)
         self.score_thresh = score_thresh
         self.down_stride = down_stride
         self.in_channel = in_channel  
         self.feat_channel = feat_channel
         self._build_head()
         self.loss_center_heatmap=build_loss(loss_ch)
-        self.loss_reg = build_loss(loss_wh)
         self.train_cfg = train_cfg
-        self.test_cfg = test_cfg
-        self.register_buffer('center_offset_yx', torch.from_numpy(np.array([
-                [-2,-2],
-                [-2,-1],
-                [-2,0],
-                [-2,1],
-                [-2,2],
-                [-1,-2],
-                [-1,-1],
-                [-1,0],
-                [-1,1],
-                [-1,2],   
-                [0,-2],
-                [0,-1],
-                [0,1],
-                [0,2],
-                [1,-2],
-                [1,-1],
-                [1,0],
-                [1,1],
-                [1,2],
-                [2,-2],
-                [2,-1],
-                [2,0],
-                [2,1],
-                [2,2],                
-            ])).unsqueeze(0).unsqueeze(0)) # 1x24x2        
+        self.test_cfg = test_cfg      
 
     def _build_head(self):
         self.heatmap_head = nn.Sequential(
             nn.Conv2d(self.in_channel, self.feat_channel, kernel_size=3, stride=1, padding=1),
             nn.ReLU(inplace=True),
             nn.Conv2d(self.feat_channel, self.num_classes, kernel_size=1, bias=True))
 
@@ -188,35 +128,45 @@
         return center_heatmap_pred, reg_pred
 
     def loss(self,
              center_heatmap_pred,
              reg_pred,
              bboxes,
              labels,
-             image_meta,
-             gt_bboxes_ignore=None):
+             image_meta, gt_bboxes_ignore=None):
         target_result, avg_factor = \
             self.get_targets(bboxes, labels, center_heatmap_pred.shape, image_meta, center_heatmap_pred.device)
 
         center_heatmap_target = target_result['center_heatmap_target']
         reg_targets = target_result['reg_targets']
         reg_weights = target_result['reg_weights']
 
-        loss_center_heatmap = self.loss_center_heatmap(
-            center_heatmap_pred.sigmoid(), center_heatmap_target, avg_factor=avg_factor)
-        loss_reg_v = self.loss_reg(
-            reg_pred,
-            reg_targets,
-            reg_weights,
-            avg_factor=avg_factor*2)
+        loss_center_heatmap = \
+            self.loss_center_heatmap(center_heatmap_pred.sigmoid(), center_heatmap_target, avg_factor=avg_factor)
+
+        batch_size = center_heatmap_pred.shape[0]
+        pred = reg_pred.permute(0, 2, 3, 1)
+        pred = torch.reshape(pred, [batch_size, -1, 4])
+
+        gt = reg_targets.permute(0, 2, 3, 1)
+        gt = torch.reshape(gt, [batch_size, -1, 4])
+
+        loss_reg_offset = []
+        for batch_index in range(batch_size):
+            pred_pos = pred[batch_index][reg_weights[batch_index,0].view(-1).to(torch.bool)]  # [num_pos_b,4]
+            target_pos = gt[batch_index][reg_weights[batch_index,0].view(-1).to(torch.bool)]  # [num_pos_b,4]
+            loss_reg_offset.append(iou_loss(pred_pos, target_pos).view(1))
+
+        num_pos = torch.sum(reg_weights).clamp_(min=1).float()
+        loss_reg_offset = torch.cat(loss_reg_offset, dim=0) / num_pos
 
         # 
         total_loss = dict(
             loss_center_heatmap=loss_center_heatmap,
-            loss_reg=loss_reg_v)
+            loss_reg=loss_reg_offset)
 
         return total_loss
 
     def coords_fmap(self, h, w):
         stride = 1
         shifts_x = torch.arange(0, w * stride, stride, dtype=torch.float32)
         shifts_y = torch.arange(0, h * stride, stride, dtype=torch.float32)
@@ -261,32 +211,31 @@
         for batch_id in range(bs):
             gt_bbox = gt_bboxes[batch_id]       # gt_bbox shape: Nx4
             if gt_bbox.shape[0] == 0:
                 # 防止无目标样本
                 reg_target_list.append(torch.zeros([4, feat_h, feat_w], dtype=torch.float32, device=device))
                 reg_weight_list.append(torch.zeros([1, feat_h, feat_w], dtype=torch.float32, device=device))
                 continue
-            
+
             coords = self.coords_fmap(h=feat_h, w=feat_w).to(device=center_heatmap_target.device) #[h*w,2]
             x = coords[:, 0]
             y = coords[:, 1]
             l_off = x[:,None] - gt_bbox[...,0][None,:]*width_ratio    #[h*w,1]-[1,m]-->[h*w,m]
             t_off = y[:,None] - gt_bbox[...,1][None,:]*height_ratio
             r_off = gt_bbox[...,2][None,:]*width_ratio - x[:,None]
             b_off = gt_bbox[...,3][None,:]*height_ratio - y[:,None]
             ltrb_off = torch.stack([l_off,t_off,r_off,b_off],dim=-1)                        #[h*w,m,4]
             areas = (ltrb_off[...,0]+ltrb_off[...,2])*(ltrb_off[...,1]+ltrb_off[...,3])     #[h*w,m]
 
             off_min = torch.min(ltrb_off,dim=-1)[0]     #[h*w,m]
             off_max = torch.max(ltrb_off,dim=-1)[0]     #[h*w,m]
-
             mask_in_gtboxes = off_min>0
-            mask_in_level = (off_max>0)&(off_max<=80)   # 设置最大尺寸和最小尺寸约束
+            mask_in_level = (off_max>-1)&(off_max<=64)   # 设置最大尺寸和最小尺寸约束 (stride=8)
 
-            radiu = 8
+            radiu = 8 * 1.5
             gt_center_x = (gt_bbox[...,0]+gt_bbox[...,2])*width_ratio/2
             gt_center_y = (gt_bbox[...,1]+gt_bbox[...,3])*height_ratio/2
             c_l_off = x[:,None] - gt_center_x[None,:]#[h*w,1]-[1,m]-->[h*w,m]
             c_t_off = y[:,None] - gt_center_y[None,:]
             c_r_off = gt_center_x[None,:] - x[:,None]
             c_b_off = gt_center_y[None,:] - y[:,None]
             c_ltrb_off = torch.stack([c_l_off,c_t_off,c_r_off,c_b_off],dim=-1)#[h*w,m,4]
@@ -302,16 +251,16 @@
             mask_pos_2 = mask_pos.long().sum(dim=-1)            #[h*w]
             mask_pos_2 = mask_pos_2 >= 1
             
             reg_target[~(mask_pos_2.to(torch.bool))] = 0
 
             # reshape
             reg_target = reg_target.reshape(feat_h, feat_w, 4).permute(2,0,1)
-            mask_pos_2 = mask_pos_2.to(torch.float32).reshape(1, feat_h,feat_w)
 
+            mask_pos_2 = mask_pos_2.to(torch.float32).reshape(1, feat_h,feat_w)
             gt_label = gt_labels[batch_id]
             center_x = (gt_bbox[:, [0]] + gt_bbox[:, [2]]) * width_ratio / 2
             center_y = (gt_bbox[:, [1]] + gt_bbox[:, [3]]) * height_ratio / 2
             gt_centers = torch.cat((center_x, center_y), dim=1)
 
             for j, ct in enumerate(gt_centers):
                 ctx_int, cty_int = ct.int()
@@ -423,15 +372,15 @@
 
         if rescale:
             det_bboxes[..., :4] *= det_bboxes.new_tensor((self.rescale_x, self.rescale_y, self.rescale_x, self.rescale_y))
 
         if 'nms' in self.test_cfg or with_nms:
             det_bboxes, det_labels = \
                 self._bboxes_nms(det_bboxes, det_labels, self.test_cfg)
-        
+
         # only for debug
         # image = cv2.imread(img_meta['image_file'])
         # det_bboxes_numpy = det_bboxes.detach().cpu().numpy()
         # for i in range(det_bboxes_numpy.shape[0]):
         #     x0,y0,x1,y1,_ = det_bboxes_numpy[i]
         #     cv2.rectangle(image, ((int)(x0),(int)(y0)), ((int)(x1),(int)(y1)), (255,0,0), 2)
         # cv2.imwrite('./aa.png', image)
```

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/__init__.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/accuracy.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/ae_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/ae_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/balanced_l1_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/balanced_l1_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/cross_entropy_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/dice_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/focal_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/gaussian_focal_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/gaussian_focal_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/gfocal_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/gfocal_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/ghm_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/ghm_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/iou_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/iou_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/kd_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/kd_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/mse_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/mse_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/pisa_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/pisa_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/seesaw_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/seesaw_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/smooth_l1_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/smooth_l1_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/utils.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/losses/varifocal_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/losses/varifocal_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/model/ttfnet.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/model/ttfnet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from antgo.framework.helper.models.builder import DETECTORS
-from ..single_stage import SingleStageDetector
+from ..single_stage import SingleStageDetector, to_image_list
 import torch
 from torch import nn
 import torch.nn.functional as F
 
 
 @DETECTORS.register_module()
 class TTFNet(SingleStageDetector):
@@ -14,38 +14,41 @@
                  train_cfg=None,
                  test_cfg=None,
                  pretrained=None,
                  init_cfg=None):
         super(TTFNet, self).__init__(backbone, neck, bbox_head,
                                      train_cfg, test_cfg, pretrained, init_cfg)
 
-    def simple_test(self, img, img_metas, rescale=True, **kwargs):
+    def simple_test(self, image, image_meta, rescale=True, **kwargs):
         """Test function without test-time augmentation.
 
         Args:
             img (torch.Tensor): Images with shape (N, C, H, W).
             img_metas (list[dict]): List of image information.
             rescale (bool, optional): Whether to rescale the results.
                 Defaults to False.
 
         Returns:
             list[list[np.ndarray]]: BBox results of each image and classes.
                 The outer list corresponds to each image. The inner list
                 corresponds to each class.
         """
-        feat = self.extract_feat(img)
+        image_list, image_meta = to_image_list(image, image_meta)
+        image = image_list.tensors
+        
+        feat = self.extract_feat(image)
         results_list = self.bbox_head.simple_test(
-            feat, img_metas, rescale=rescale)
+            feat, image_meta, rescale=rescale)
 
         bbox_results = {
             'box': [a for a, _ in results_list],
             'label': [b for _, b in results_list],
         }
         # {'box', 'label'}
         return bbox_results
 
-    def onnx_export(self, img):
-        feat = self.extract_feat(img)
+    def onnx_export(self, image):
+        feat = self.extract_feat(image)
         local_cls, local_reg = self.bbox_head(feat)
         local_cls = torch.sigmoid(local_cls)
         local_cls = F.max_pool2d(local_cls, 3, stride=1, padding=(3 - 1) // 2)
         return local_cls, local_reg
```

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/neck/fpn.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/neck/fpn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/utils/gaussian_target.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/utils/gaussian_target.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/utils/util_mixins.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/utils/util_mixins.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/detectors/utils/util_random.py` & `antgo-0.1.1/antgo/framework/helper/models/detectors/utils/util_random.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/ab.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/ab.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/afd.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/afd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/at.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/at.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/bss.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/bss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/cc.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/cc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/crd.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/crd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/dml.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/dml.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/fsp.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/fsp.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/ft.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/ft.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/irg.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/irg.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/logits.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/logits.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/lwm.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/lwm.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/mgd.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/mgd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/nst.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/nst.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/ofd.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/ofd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/pkt.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/pkt.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/rkd.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/rkd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/sobolev.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/sobolev.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/sp.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/sp.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/st.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/st.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/distillation/loss/vid.py` & `antgo-0.1.1/antgo/framework/helper/models/distillation/loss/vid.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/dummy_module.py` & `antgo-0.1.1/antgo/framework/helper/models/dummy_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/ema_module.py` & `antgo-0.1.1/antgo/framework/helper/models/ema_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_layers.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_layers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_op.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_op.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/elastic_nn/utils.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/elastic_nn/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/model_zoo.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/model_zoo.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/ofa/baseline/mobilenet_v3.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/ofa/baseline/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/ofa/networks/ofa_mbv3.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/ofa/networks/ofa_mbv3.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/ofa/training/epoch_based_sampling_runner.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/ofa/training/epoch_based_sampling_runner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/ofa/training/evaluation.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/ofa/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/ofa/utils.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/ofa/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_dataset.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_predictor.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_predictor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/search/accuracy_predictor/arch_encoder.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/search/accuracy_predictor/arch_encoder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/search/efficiency_predictor/__init__.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/search/efficiency_predictor/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/search/efficiency_predictor/latency_lookup_table.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/search/efficiency_predictor/latency_lookup_table.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/search/search_algorithm/evolution.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/search/search_algorithm/evolution.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/test.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/test.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/tutorial/accuracy_predictor.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/tutorial/accuracy_predictor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/tutorial/evolution_finder.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/tutorial/evolution_finder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/tutorial/flops_table.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/tutorial/flops_table.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/tutorial/imagenet_eval_helper.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/tutorial/imagenet_eval_helper.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/tutorial/latency_table.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/tutorial/latency_table.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/utils/common_tools.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/utils/common_tools.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/utils/flops_counter.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/utils/layers.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/utils/layers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/utils/my_modules.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/utils/my_modules.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/utils/pytorch_modules.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/utils/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/nas/utils/pytorch_utils.py` & `antgo-0.1.1/antgo/framework/helper/models/nas/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/pose3d/backbone/QNetLite0_alpha.py` & `antgo-0.1.1/antgo/framework/helper/models/pose3d/backbone/QNetLite0_alpha.py`

 * *Files 4% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         return out
 
 
 @BACKBONES.register_module()
 class KetNetF(nn.Module):
     """KetNetF"""
 
-    def __init__(self, architecture, in_channels=1):
+    def __init__(self, architecture, in_channels=1, out_indices=[1,2,3,4]):
         super(KetNetF, self).__init__()
         self.norm_layer = nn.BatchNorm2d
         self.stage_with_dcn=(False, False, False, False, False, False, False, False)
         assert architecture in ["resnet18", "resnet34", "resnet50", "resnet101", "resnet152"]
         layers = {
             "resnet34": [1, 1, 1, 2, 2, 1, 4, 4],
         }
@@ -216,14 +216,15 @@
         if architecture == "resnet18" or architecture == "resnet34":
             self.block = InverseBottleneck
         else:
             self.block = InverseBottleneck
         self.layers = layers[architecture]
         stage_dcn = [None for with_dcn in self.stage_with_dcn]
 
+        self.out_indices = sorted(out_indices)
         self.conv1 = nn.Conv2d(in_channels, 32, kernel_size=5, stride=2, padding=2, bias=False)
         self.bn1 = self.norm_layer(32, eps=1e-5, momentum=0.1, affine=True)
         self.relu1 = nn.ReLU(inplace=True)
 
         self.block.exp = 3
         self.layer1 = self.make_layer(self.block, 32, self.layers[0], stride=1, dcn=stage_dcn[0])
         self.layer2 = self.make_layer(self.block, 32, self.layers[1], stride=2, dcn=stage_dcn[1])
@@ -236,22 +237,35 @@
         self.block.exp = 6
         self.layer7 = self.make_layer(self.block, 128, self.layers[6], stride=1, dcn=stage_dcn[6])
         self.layer8 = self.make_layer(self.block, 160, self.layers[7], stride=2, dcn=stage_dcn[7])
 
     def forward(self, x):
         x = self.relu1(self.bn1(self.conv1(x)))  # 32 * h/4 * w/4
         x = self.layer1(x)
+        outs = []
+        if 0 in self.out_indices:
+            outs.append(x)
         x32 = self.layer2(x)  # 32 * h/4 * w/4
         x32 = self.layer3(x32)  # 64 * h/4 * w/4
+        if 1 in self.out_indices:
+            outs.append(x32)
         x16 = self.layer4(x32)  # 64 * h/8 * w/8
         x16 = self.layer5(x16)  # 96 * h/8 * w/8
+        if 2 in self.out_indices:
+            outs.append(x16)
+        
         x8 = self.layer6(x16)  # 128 * h/16 * w/16
         x8 = self.layer7(x8)  # 128 * h/16 * w/16
+        if 3 in self.out_indices:
+            outs.append(x8)
+
         x4 = self.layer8(x8)  # 160 * h/32 * w/32
-        return [x32, x16, x8, x4]
+        if 4 in self.out_indices:
+            outs.append(x4)
+        return outs
 
     def stages(self):
         return [self.layer1, self.layer2, self.layer3, self.layer4]
 
     def make_layer(self, block, planes, blocks, stride=1, dcn=None):
         downsample = None
         if stride != 1 or self.inplanes != planes * block.expansion:
```

### Comparing `antgo-0.1.0/antgo/framework/helper/models/pose3d/backbone/QNetLite0_beta.py` & `antgo-0.1.1/antgo/framework/helper/models/pose3d/backbone/QNetLite0_beta.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/pose3d/head/handpose_qnet_lite0_pose_heatmap2d.py` & `antgo-0.1.1/antgo/framework/helper/models/pose3d/head/handpose_qnet_lite0_pose_heatmap2d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/pose3d/head/layer.py` & `antgo-0.1.1/antgo/framework/helper/models/pose3d/head/layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/pose3d/head/twohand_3dpose_latent.py` & `antgo-0.1.1/antgo/framework/helper/models/pose3d/head/twohand_3dpose_latent.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/pose3d/losses/gaussian_focal_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/pose3d/losses/gaussian_focal_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/pose3d/losses/loss.py` & `antgo-0.1.1/antgo/framework/helper/models/pose3d/losses/loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/pose3d/losses/utils.py` & `antgo-0.1.1/antgo/framework/helper/models/pose3d/losses/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/pose3d/model/ddr_twohand_pose3d.py` & `antgo-0.1.1/antgo/framework/helper/models/pose3d/model/ddr_twohand_pose3d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/pose3d/model/keynet_model.py` & `antgo-0.1.1/antgo/framework/helper/models/pose3d/model/keynet_model.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/proxy_module.py` & `antgo-0.1.1/antgo/framework/helper/models/proxy_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/segmentation/backbone/DDRQNetLite0.py` & `antgo-0.1.1/antgo/framework/helper/models/segmentation/backbone/DDRQNetLite0.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/segmentation/head/aspp_head.py` & `antgo-0.1.1/antgo/framework/helper/models/segmentation/head/aspp_head.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import torch
 import torch.nn as nn
-from mmcv.cnn import ConvModule
 from antgo.framework.helper.cnn.bricks import *
 from antgo.framework.helper.models.builder import HEADS, MODELS, build_loss
 from antgo.framework.helper.runner import BaseModule
 import torch.nn.functional as F
 
 
 class ASPPModule(nn.ModuleList):
```

### Comparing `antgo-0.1.0/antgo/framework/helper/models/segmentation/head/simple_head.py` & `antgo-0.1.1/antgo/framework/helper/models/segmentation/head/simple_head.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import torch
 import torch.nn as nn
-from mmcv.cnn import ConvModule
 from antgo.framework.helper.cnn.bricks import *
 from antgo.framework.helper.models.builder import HEADS, MODELS, build_loss
 from antgo.framework.helper.runner import BaseModule
 import torch.nn.functional as F
 
 
 @HEADS.register_module()
```

### Comparing `antgo-0.1.0/antgo/framework/helper/models/segmentation/model/encoder_decoder.py` & `antgo-0.1.1/antgo/framework/helper/models/segmentation/model/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/semi/dense.py` & `antgo-0.1.1/antgo/framework/helper/models/semi/dense.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,17 +65,17 @@
                 weight=mask,
                 reduction="mean",
             )
         )
 
         return {"loss_heatmap": loss_heatmap}
 
-    def forward_train(self, images, image_meta, **kwargs):
+    def forward_train(self, image, image_meta, **kwargs):
         label_images, unlabel_weak_strong_images = \
-            torch.split(images, [self.label_batch_size, self.unlabel_batch_size+self.unlabel_batch_size],dim=0) 
+            torch.split(image, [self.label_batch_size, self.unlabel_batch_size+self.unlabel_batch_size],dim=0) 
         label_metas = image_meta[:self.label_batch_size]
 
         unlabel_weak_images=torch.index_select(unlabel_weak_strong_images,dim=0,index=torch.tensor([i for i in range(0,2*self.unlabel_batch_size,2)]))
         unlabel_strong_images=torch.index_select(unlabel_weak_strong_images,dim=0,index=torch.tensor([i for i in range(1,2*self.unlabel_batch_size,2)]))
 
         unlabel_weak_strong_metas = image_meta[self.label_batch_size:]
         unlabel_weak_metas = [unlabel_weak_strong_metas[i] for i in range(0, 2*self.unlabel_batch_size, 2)]
@@ -148,16 +148,16 @@
         )
 
         unsup_loss = {"unlabeled_" + k: v*self.semi_loss_w for k, v in unsup_loss.items()}
         losses.update(**unsup_loss)
 
         return losses
     
-    def simple_test(self, images, image_meta, rescale=True, **kwargs):
-        return self.teacher(images, image_meta, rescale, **kwargs)
+    def simple_test(self, image, image_meta, rescale=True, **kwargs):
+        return self.teacher(image, image_meta, rescale, **kwargs)
 
     def _load_from_state_dict(
         self,
         state_dict,
         prefix,
         local_metadata,
         strict,
```

### Comparing `antgo-0.1.0/antgo/framework/helper/models/semi/detmpl.py` & `antgo-0.1.1/antgo/framework/helper/models/semi/detmpl.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/semi/hook/mean_teacher.py` & `antgo-0.1.1/antgo/framework/helper/models/semi/hook/mean_teacher.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/semi/losses/quality_focal_loss.py` & `antgo-0.1.1/antgo/framework/helper/models/semi/losses/quality_focal_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/semi/mpl.py` & `antgo-0.1.1/antgo/framework/helper/models/semi/mpl.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/__init__.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/box_utils.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/box_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/brick_wrappers.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/brick_wrappers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/builder.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/ckpt_convert.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/ckpt_convert.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/conv_upsample.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/conv_upsample.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/csp_layer.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/csp_layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/gaussian_target.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/gaussian_target.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/inverted_residual.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/make_divisible.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/misc.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/misc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/normed_predictor.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/normed_predictor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/panoptic_gt_processing.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/panoptic_gt_processing.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/positional_encoding.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/res_layer.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/se_layer.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/structure_utils.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/structure_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/models/utils/structures.py` & `antgo-0.1.1/antgo/framework/helper/models/utils/structures.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/multi_stream_module.py` & `antgo-0.1.1/antgo/framework/helper/multi_stream_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/parallel/_functions.py` & `antgo-0.1.1/antgo/framework/helper/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/parallel/collate.py` & `antgo-0.1.1/antgo/framework/helper/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/parallel/data_container.py` & `antgo-0.1.1/antgo/framework/helper/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/parallel/data_parallel.py` & `antgo-0.1.1/antgo/framework/helper/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/parallel/distributed.py` & `antgo-0.1.1/antgo/framework/helper/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/parallel/scatter_gather.py` & `antgo-0.1.1/antgo/framework/helper/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/parallel/utils.py` & `antgo-0.1.1/antgo/framework/helper/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/reader.py` & `antgo-0.1.1/antgo/framework/helper/reader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import division
 from __future__ import division
 from __future__ import unicode_literals
 from __future__ import print_function
+import logging
 import os
 import typing
 import torch.utils.data
 import torchvision.transforms as transforms
 import numpy as np
 import copy
-import cv2
-from antgo.framework.helper.runner.dist_utils import get_dist_info
 from antgo.framework.helper.utils import build_from_cfg
 
 
 def register(cls):
     class ProxyReader(Reader):
         def __init__(self, train_or_test, dir='', params={}, pipeline=None, inputs_def=None, **kwargs):
             super().__init__(
@@ -109,15 +108,14 @@
                 if isinstance(transform, dict):
                     self.pipeline_types.append(transform['type'])
                     transform = build_from_cfg(transform, PIPELINES)
                     self.pipeline.append(transform)
                 else:
                     raise TypeError('pipeline must be a dict')
 
-
             if weak_pipeline is not None and strong_pipeline is not None:
                 for transform in weak_pipeline:
                     if isinstance(transform, dict):
                         transform = build_from_cfg(transform, PIPELINES)
                         self.weak_pipeline.append(transform)
                     else:
                         raise TypeError('weak_pipeline must be a dict')
@@ -161,25 +159,37 @@
             return warp_ins
         
         warp_ins = {}
         for alia, field in zip(alias, fields):
             warp_ins[alia] = sample[field]
 
         return warp_ins
-    
+
     def __len__(self):
         return self.proxy_dataset.size
-    
+
     def __getitem__(self, idx):
         sample = None
         try:
             sample = self.proxy_dataset.sample(idx)
+            if sample is None:
+                fail_count = 0
+                while True:
+                    # 随机选择，找到有效样本
+                    random_i = np.random.randint(0,self.proxy_dataset.size)
+                    sample = self.proxy_dataset.sample(random_i)
+                    if sample is not None:
+                        break
+
+                    fail_count += 1
+                    if fail_count > 10:
+                        logging.warn(f'Fail find correct sample and exceed count {fail_count}.')
         except:
             print(f'sample error {idx}')
-        
+
         weak_sample = None
         strong_sample = None
         if len(self.weak_pipeline) > 0 or len(self.strong_pipeline) > 0:
             weak_sample = copy.deepcopy(sample)
             for transform in self.weak_pipeline:
                 weak_sample = transform(weak_sample)
             strong_sample = copy.deepcopy(weak_sample)
@@ -209,7 +219,136 @@
         return self.proxy_dataset.get_cat_ids(idx)
 
     def get_ann_info(self, idx):
         return self.proxy_dataset.get_ann_info(idx)
 
     def evaluate(self, preds,**kwargs):
         return self.proxy_dataset.evaluate(preds, **kwargs)
+
+
+class TVReader(torch.utils.data.Dataset):
+    def __init__(self, dataset, pipeline=None, weak_pipeline=None, strong_pipeline=None, inputs_def=None):
+        self.proxy_dataset = dataset
+        self.pipeline = []
+        self.pipeline_types = []
+        self.weak_pipeline = []
+        self.strong_pipeline = []        
+        if pipeline is not None:
+            from antgo.framework.helper.dataset import PIPELINES
+            for transform in pipeline:
+                if isinstance(transform, dict):
+                    self.pipeline_types.append(transform['type'])
+                    transform = build_from_cfg(transform, PIPELINES)
+                    self.pipeline.append(transform)
+                else:
+                    raise TypeError('pipeline must be a dict')
+
+            if weak_pipeline is not None and strong_pipeline is not None:
+                for transform in weak_pipeline:
+                    if isinstance(transform, dict):
+                        transform = build_from_cfg(transform, PIPELINES)
+                        self.weak_pipeline.append(transform)
+                    else:
+                        raise TypeError('weak_pipeline must be a dict')
+                
+                for transform in strong_pipeline:
+                    if isinstance(transform, dict):
+                        transform = build_from_cfg(transform, PIPELINES)
+                        self.strong_pipeline.append(transform)
+                    else:
+                        raise TypeError('strong_pipeline must be a dict')
+
+        self._fields = copy.deepcopy(inputs_def['fields']) if inputs_def else None
+        self._alias = None
+        if self._fields is not None and 'alias' in inputs_def:
+            self._alias = copy.deepcopy(inputs_def['alias'])
+        
+        if self._fields is not None:
+            if self._alias is None:
+                self._alias = copy.deepcopy(self._fields)
+
+        self.flag = np.zeros(len(self), dtype=np.uint8)
+        if hasattr(self.proxy_dataset, 'flag'):
+            self.flag = self.proxy_dataset.flag
+
+        self.CLASSES = 1
+        if hasattr(self.proxy_dataset, 'CLASSES'):
+            self.CLASSES = self.proxy_dataset.CLASSES
+
+    def _arrange(self, sample, fields, alias):
+        if fields is None:
+            return sample      
+          
+        if type(fields[0]) == list or type(fields[0]) == tuple:
+            warp_ins = []
+            for alia, field in zip(alias, fields):
+                one_ins = {}
+                for aa, ff in zip(alia, field):
+                    one_ins[aa] = sample[ff]
+                
+                warp_ins.append(one_ins)
+            return warp_ins
+        
+        warp_ins = {}
+        for alia, field in zip(alias, fields):
+            warp_ins[alia] = sample[field]
+
+        return warp_ins
+    
+    def __len__(self):
+        return len(self.proxy_dataset)
+    
+    def __getitem__(self, idx):
+        sample = None
+        try:
+            sample = self.proxy_dataset[idx]
+            if sample is None:
+                fail_count = 0
+                while True:
+                    # 随机选择，找到有效样本
+                    random_i = np.random.randint(0,self.proxy_dataset.size)
+                    sample = self.proxy_dataset.sample(random_i)
+                    if sample is not None:
+                        break
+
+                    fail_count += 1
+                    if fail_count > 10:
+                        logging.warn(f'Fail find correct sample and exceed count {fail_count}.')            
+
+            if isinstance(sample, tuple) or isinstance(sample, list):
+                temp = {}
+                for data, name in zip(sample, self._alias):
+                    temp[name] = data
+                sample = temp
+            else:
+                sample = {self._alias[0]: sample}
+        except:
+            print(f'sample error {idx}')
+        
+        weak_sample = None
+        strong_sample = None
+        if len(self.weak_pipeline) > 0 or len(self.strong_pipeline) > 0:
+            weak_sample = copy.deepcopy(sample)
+            for transform in self.weak_pipeline:
+                weak_sample = transform(weak_sample)
+            strong_sample = copy.deepcopy(weak_sample)
+            for transform in self.strong_pipeline:
+                strong_sample = transform(strong_sample)
+
+        if weak_sample is not None and strong_sample is not None:
+            for transform in self.pipeline:
+                weak_sample = transform(weak_sample)
+
+            for transform in self.pipeline:
+                strong_sample = transform(strong_sample)
+
+            # arange warp
+            weak_sample = self._arrange(weak_sample, self._fields, self._alias)
+            strong_sample = self._arrange(strong_sample, self._fields, self._alias)
+            return [weak_sample, strong_sample]
+        else:
+            for transform in self.pipeline:
+                sample = transform(sample)
+
+            # arange warp
+            sample = self._arrange(sample, self._fields, self._alias)
+            return sample
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/__init__.py` & `antgo-0.1.1/antgo/framework/helper/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/base_runner.py` & `antgo-0.1.1/antgo/framework/helper/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/builder.py` & `antgo-0.1.1/antgo/framework/helper/runner/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/checkpoint.py` & `antgo-0.1.1/antgo/framework/helper/runner/checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -597,17 +597,17 @@
         state_dict = OrderedDict(
             {re.sub(p, r, k): v
              for k, v in state_dict.items()})
     # Keep metadata in state_dict
     state_dict._metadata = metadata
 
     # load state_dict
-    module = model
-    if is_module_wrapper(module):
-        module = module.module    
+    # module = model
+    # if is_module_wrapper(module):
+    #     module = module.module    
     # if getattr(module, "load_state_dict", None) is not None:
     #     result = module.load_state_dict(state_dict)
     #     if result:
     #         return checkpoint
 
     load_state_dict(model, state_dict, strict, logger)
     return checkpoint
```

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/default_constructor.py` & `antgo-0.1.1/antgo/framework/helper/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/dist_utils.py` & `antgo-0.1.1/antgo/framework/helper/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/epoch_based_runner.py` & `antgo-0.1.1/antgo/framework/helper/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/fp16_utils.py` & `antgo-0.1.1/antgo/framework/helper/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/__init__.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/checkpoint.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/ema.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/evaluation.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/hook.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/logger/base.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/logger/neptune.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/logger/text.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/lr_updater.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/memory.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/momentum_updater.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/optimizer.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/profiler.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/sampler_seed.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/samplingmethods/kcenter_greedy.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/samplingmethods/kcenter_greedy.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/samplingmethods/sampling_def.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/samplingmethods/sampling_def.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/submodules_evaluation.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/submodules_evaluation.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/sync_buffer.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/hooks/weight_adjust.py` & `antgo-0.1.1/antgo/framework/helper/runner/hooks/weight_adjust.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/iter_based_runner.py` & `antgo-0.1.1/antgo/framework/helper/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/log_buffer.py` & `antgo-0.1.1/antgo/framework/helper/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/optimizer/builder.py` & `antgo-0.1.1/antgo/framework/helper/runner/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/optimizer/default_constructor.py` & `antgo-0.1.1/antgo/framework/helper/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/priority.py` & `antgo-0.1.1/antgo/framework/helper/runner/priority.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/test.py` & `antgo-0.1.1/antgo/framework/helper/runner/test.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/runner/utils.py` & `antgo-0.1.1/antgo/framework/helper/runner/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/task_flag.py` & `antgo-0.1.1/antgo/framework/helper/task_flag.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/tester.py` & `antgo-0.1.1/antgo/framework/helper/tester.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/tools/evaluate.py` & `antgo-0.1.1/antgo/framework/helper/tools/evaluate.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/tools/exp.py` & `antgo-0.1.1/antgo/framework/helper/tools/exp.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/tools/export_onnx.py` & `antgo-0.1.1/antgo/framework/helper/tools/export_onnx.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/tools/train.py` & `antgo-0.1.1/antgo/framework/helper/tools/train.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/tools/util.py` & `antgo-0.1.1/antgo/framework/helper/tools/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/trainer.py` & `antgo-0.1.1/antgo/framework/helper/trainer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/__init__.py` & `antgo-0.1.1/antgo/framework/helper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/compat_config.py` & `antgo-0.1.1/antgo/framework/helper/utils/compat_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/config.py` & `antgo-0.1.1/antgo/framework/helper/utils/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/dist_utils.py` & `antgo-0.1.1/antgo/framework/helper/utils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/env.py` & `antgo-0.1.1/antgo/framework/helper/utils/env.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/ext_loader.py` & `antgo-0.1.1/antgo/framework/helper/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/hub.py` & `antgo-0.1.1/antgo/framework/helper/utils/hub.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/logging.py` & `antgo-0.1.1/antgo/framework/helper/utils/logging.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/math_3d.py` & `antgo-0.1.1/antgo/framework/helper/utils/math_3d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/misc.py` & `antgo-0.1.1/antgo/framework/helper/utils/misc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/parrots_jit.py` & `antgo-0.1.1/antgo/framework/helper/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/parrots_wrapper.py` & `antgo-0.1.1/antgo/framework/helper/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/path.py` & `antgo-0.1.1/antgo/framework/helper/utils/path.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/progressbar.py` & `antgo-0.1.1/antgo/framework/helper/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/registry.py` & `antgo-0.1.1/antgo/framework/helper/utils/registry.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/seed.py` & `antgo-0.1.1/antgo/framework/helper/utils/seed.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/setup_env.py` & `antgo-0.1.1/antgo/framework/helper/utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/testing.py` & `antgo-0.1.1/antgo/framework/helper/utils/testing.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/timer.py` & `antgo-0.1.1/antgo/framework/helper/utils/timer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/trace.py` & `antgo-0.1.1/antgo/framework/helper/utils/trace.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/util_distribution.py` & `antgo-0.1.1/antgo/framework/helper/utils/util_distribution.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/helper/utils/version_utils.py` & `antgo-0.1.1/antgo/framework/helper/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/paddle2torch/mapper/io.py` & `antgo-0.1.1/antgo/framework/paddle2torch/mapper/io.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/paddle2torch/mapper/nn.py` & `antgo-0.1.1/antgo/framework/paddle2torch/mapper/nn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/paddle2torch/mapper/ops.py` & `antgo-0.1.1/antgo/framework/paddle2torch/mapper/ops.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/paddle2torch/mapper/optimizer.py` & `antgo-0.1.1/antgo/framework/paddle2torch/mapper/optimizer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/paddle2torch/utils.py` & `antgo-0.1.1/antgo/framework/paddle2torch/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/mapper/__init__.py` & `antgo-0.1.1/antgo/framework/torch2paddle/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/mapper/device.py` & `antgo-0.1.1/antgo/framework/torch2paddle/mapper/device.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/mapper/distributed.py` & `antgo-0.1.1/antgo/framework/torch2paddle/mapper/distributed.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/mapper/io.py` & `antgo-0.1.1/antgo/framework/torch2paddle/mapper/io.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/mapper/layer.py` & `antgo-0.1.1/antgo/framework/torch2paddle/mapper/layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/mapper/nn.py` & `antgo-0.1.1/antgo/framework/torch2paddle/mapper/nn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/mapper/nn_functional.py` & `antgo-0.1.1/antgo/framework/torch2paddle/mapper/nn_functional.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/mapper/nn_init.py` & `antgo-0.1.1/antgo/framework/torch2paddle/mapper/nn_init.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/mapper/nn_utils.py` & `antgo-0.1.1/antgo/framework/torch2paddle/mapper/nn_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/mapper/ops.py` & `antgo-0.1.1/antgo/framework/torch2paddle/mapper/ops.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/mapper/optimizer.py` & `antgo-0.1.1/antgo/framework/torch2paddle/mapper/optimizer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/mapper/parambase.py` & `antgo-0.1.1/antgo/framework/torch2paddle/mapper/parambase.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/mapper/tensor.py` & `antgo-0.1.1/antgo/framework/torch2paddle/mapper/tensor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/mapper/varbase.py` & `antgo-0.1.1/antgo/framework/torch2paddle/mapper/varbase.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/tools/ast_update.py` & `antgo-0.1.1/antgo/framework/torch2paddle/tools/ast_update.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/tools/convert.py` & `antgo-0.1.1/antgo/framework/torch2paddle/tools/convert.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/tools/dependency_analyzer.py` & `antgo-0.1.1/antgo/framework/torch2paddle/tools/dependency_analyzer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/tools/utils.py` & `antgo-0.1.1/antgo/framework/torch2paddle/tools/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/utils.py` & `antgo-0.1.1/antgo/framework/torch2paddle/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/vision/datasets.py` & `antgo-0.1.1/antgo/framework/torch2paddle/vision/datasets.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/vision/transforms.py` & `antgo-0.1.1/antgo/framework/torch2paddle/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/framework/torch2paddle/vision/utils.py` & `antgo-0.1.1/antgo/framework/torch2paddle/vision/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/help.py` & `antgo-0.1.1/antgo/help.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,14 +120,16 @@
         shutil.copy(os.path.join(template_project_folder, 'install.sh'), target_folder)
     if not os.path.exists(os.path.join(target_folder, 'launch.sh')):
         shutil.copy(os.path.join(template_project_folder, 'launch.sh'), target_folder)
     if not os.path.exists(os.path.join(target_folder, 'requirements.txt')):
         shutil.copy(os.path.join(template_project_folder, 'requirements.txt'), target_folder)
     if not os.path.exists(os.path.join(target_folder, 'README.md')):
         shutil.copy(os.path.join(template_project_folder, 'README.md'), target_folder)
+    if not os.path.exists(os.path.join(target_folder, '.gitignore')):
+        shutil.copy(os.path.join(template_project_folder, '.gitignore'), target_folder)
 
 
 def project_add_action(action_name, args):
     if args.project == '':
         logging.error('Must set --project')
         return
     
@@ -479,15 +481,15 @@
             with open(os.path.join(config.AntConfig.task_factory,f'{args.project}.json'), 'w') as fp:
                 json.dump(project_info, fp)
             logging.info(f'Success remove {sub_action_name} config')    
             get_lock().release()          
             return    
 
         if not os.path.exists(args.config):
-            if args.name not in ['dense', 'detmpl', 'mpl']:
+            if args.name not in ['reviewkd']:
                 logging.error(f'Missing config file, {sub_action_name} couldnt config')
                 get_lock().release()
                 return
             else:
                 args.config = os.path.join(os.path.dirname(__file__), 'framework', 'helper', 'configs', sub_action_name.split('/')[-1], f'{args.name}_config.py')
 
         if not os.path.exists(args.config):
```

### Comparing `antgo-0.1.0/antgo/interactcontext.py` & `antgo-0.1.1/antgo/interactcontext.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/main.py` & `antgo-0.1.1/antgo/main.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/main_backup.py` & `antgo-0.1.1/antgo/main_backup.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/__init__.py` & `antgo-0.1.1/antgo/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/ali_fashion_attribute_error.py` & `antgo-0.1.1/antgo/measures/ali_fashion_attribute_error.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/ali_fashion_landmark_ne.py` & `antgo-0.1.1/antgo/measures/ali_fashion_landmark_ne.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/average_precision.py` & `antgo-0.1.1/antgo/measures/average_precision.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/base.py` & `antgo-0.1.1/antgo/measures/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/binary_c.py` & `antgo-0.1.1/antgo/measures/binary_c.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/binomial_deviance.py` & `antgo-0.1.1/antgo/measures/binomial_deviance.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/confusion_matrix.py` & `antgo-0.1.1/antgo/measures/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/crowdsource.py` & `antgo-0.1.1/antgo/measures/crowdsource.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/deep_analysis.py` & `antgo-0.1.1/antgo/measures/deep_analysis.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/error.py` & `antgo-0.1.1/antgo/measures/error.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/face_task.py` & `antgo-0.1.1/antgo/measures/face_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/kdd_average_precision.py` & `antgo-0.1.1/antgo/measures/kdd_average_precision.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/matting_task.py` & `antgo-0.1.1/antgo/measures/matting_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/moving_statistic.py` & `antgo-0.1.1/antgo/measures/moving_statistic.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/multi_c.py` & `antgo-0.1.1/antgo/measures/multi_c.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/multic_task.py` & `antgo-0.1.1/antgo/measures/multic_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/multil_task.py` & `antgo-0.1.1/antgo/measures/multil_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/objdect_task.py` & `antgo-0.1.1/antgo/measures/objdect_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/pck.py` & `antgo-0.1.1/antgo/measures/pck.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/person_search_task.py` & `antgo-0.1.1/antgo/measures/person_search_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/precision_recall.py` & `antgo-0.1.1/antgo/measures/precision_recall.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/quadratic_weighted_kappa.py` & `antgo-0.1.1/antgo/measures/quadratic_weighted_kappa.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/regression_metric.py` & `antgo-0.1.1/antgo/measures/regression_metric.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/regression_task.py` & `antgo-0.1.1/antgo/measures/regression_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/repeat_statistic.py` & `antgo-0.1.1/antgo/measures/repeat_statistic.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/roc_auc.py` & `antgo-0.1.1/antgo/measures/roc_auc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/segmentation_task.py` & `antgo-0.1.1/antgo/measures/segmentation_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/significance.py` & `antgo-0.1.1/antgo/measures/significance.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/statistic.py` & `antgo-0.1.1/antgo/measures/statistic.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/topk.py` & `antgo-0.1.1/antgo/measures/topk.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/track_task.py` & `antgo-0.1.1/antgo/measures/track_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/measures/yesno_crowdsource.py` & `antgo-0.1.1/antgo/measures/yesno_crowdsource.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/engine/__init__.py` & `antgo-0.1.1/antgo/pipeline/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/engine/execution/base_execution.py` & `antgo-0.1.1/antgo/pipeline/engine/execution/base_execution.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/engine/factory.py` & `antgo-0.1.1/antgo/pipeline/engine/factory.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/engine/operator_loader.py` & `antgo-0.1.1/antgo/pipeline/engine/operator_loader.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/engine/operator_registry.py` & `antgo-0.1.1/antgo/pipeline/engine/operator_registry.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/engine/uri.py` & `antgo-0.1.1/antgo/pipeline/engine/uri.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/__init__.py` & `antgo-0.1.1/antgo/pipeline/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/common/util.py` & `antgo-0.1.1/antgo/pipeline/functional/common/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/data_collection.py` & `antgo-0.1.1/antgo/pipeline/functional/data_collection.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/entity.py` & `antgo-0.1.1/antgo/pipeline/functional/entity.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/image/__init__.py` & `antgo-0.1.1/antgo/pipeline/functional/image/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/image/io.py` & `antgo-0.1.1/antgo/pipeline/functional/image/io.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/image/plot.py` & `antgo-0.1.1/antgo/pipeline/functional/image/plot.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/image/process.py` & `antgo-0.1.1/antgo/pipeline/functional/image/process.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/mixins/__init__.py` & `antgo-0.1.1/antgo/pipeline/functional/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/mixins/column.py` & `antgo-0.1.1/antgo/pipeline/functional/mixins/column.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/mixins/computer_vision.py` & `antgo-0.1.1/antgo/pipeline/functional/mixins/computer_vision.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/mixins/config.py` & `antgo-0.1.1/antgo/pipeline/functional/mixins/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/mixins/dag.py` & `antgo-0.1.1/antgo/pipeline/functional/mixins/dag.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/mixins/data_processing.py` & `antgo-0.1.1/antgo/pipeline/functional/mixins/data_processing.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/mixins/dataframe.py` & `antgo-0.1.1/antgo/pipeline/functional/mixins/dataframe.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/mixins/dataset.py` & `antgo-0.1.1/antgo/pipeline/functional/mixins/dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/mixins/demo.py` & `antgo-0.1.1/antgo/pipeline/functional/mixins/demo.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/mixins/dispatcher.py` & `antgo-0.1.1/antgo/pipeline/functional/mixins/dispatcher.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/mixins/list.py` & `antgo-0.1.1/antgo/pipeline/functional/mixins/list.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/mixins/serve.py` & `antgo-0.1.1/antgo/pipeline/functional/mixins/serve.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/mixins/show.py` & `antgo-0.1.1/antgo/pipeline/functional/mixins/show.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/mixins/stream.py` & `antgo-0.1.1/antgo/pipeline/functional/mixins/stream.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/option.py` & `antgo-0.1.1/antgo/pipeline/functional/option.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/functional/storages.py` & `antgo-0.1.1/antgo/pipeline/functional/storages.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/hparam/__init__.py` & `antgo-0.1.1/antgo/pipeline/hparam/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/hparam/hyperparameter.py` & `antgo-0.1.1/antgo/pipeline/hparam/hyperparameter.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/hub/builtin/operators/inference_model_op.py` & `antgo-0.1.1/antgo/pipeline/hub/builtin/operators/inference_model_op.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/hub/builtin/operators/inference_onnx_op.py` & `antgo-0.1.1/antgo/pipeline/hub/builtin/operators/inference_onnx_op.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/hub/builtin/operators/runas_op.py` & `antgo-0.1.1/antgo/pipeline/hub/builtin/operators/runas_op.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/hub/external/mm/detector.py` & `antgo-0.1.1/antgo/pipeline/hub/external/mm/detector.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/hub/external/mm/inpainting.py` & `antgo-0.1.1/antgo/pipeline/hub/external/mm/inpainting.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/hub/external/mm/ocr.py` & `antgo-0.1.1/antgo/pipeline/hub/external/mm/ocr.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/hub/external/mm/pose.py` & `antgo-0.1.1/antgo/pipeline/hub/external/mm/pose.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/hub/external/mm/restoration.py` & `antgo-0.1.1/antgo/pipeline/hub/external/mm/restoration.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/hub/external/mm/segmentor.py` & `antgo-0.1.1/antgo/pipeline/hub/external/mm/segmentor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/models/cfg/dataset/coco.yaml` & `antgo-0.1.1/antgo/pipeline/models/cfg/dataset/coco.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/models/cfg/detector/yolov7-e6.yaml` & `antgo-0.1.1/antgo/pipeline/models/cfg/detector/yolov7-e6.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/models/cfg/detector/yolov7-w6.yaml` & `antgo-0.1.1/antgo/pipeline/models/cfg/detector/yolov7-w6.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/models/cfg/detector/yolov7.yaml` & `antgo-0.1.1/antgo/pipeline/models/cfg/detector/yolov7.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/models/cfg/detector/yolov7x.yaml` & `antgo-0.1.1/antgo/pipeline/models/cfg/detector/yolov7x.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/models/detector/util.py` & `antgo-0.1.1/antgo/pipeline/models/detector/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/models/detector/yolov7/util.py` & `antgo-0.1.1/antgo/pipeline/models/detector/yolov7/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/models/detector/yolov7/yolov7.py` & `antgo-0.1.1/antgo/pipeline/models/detector/yolov7/yolov7.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/models/utils/common.py` & `antgo-0.1.1/antgo/pipeline/models/utils/common.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/models/utils/preprocess.py` & `antgo-0.1.1/antgo/pipeline/models/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/models/utils/utils.py` & `antgo-0.1.1/antgo/pipeline/models/utils/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/operators/base.py` & `antgo-0.1.1/antgo/pipeline/operators/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/operators/nop.py` & `antgo-0.1.1/antgo/pipeline/operators/nop.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/pipeline/utils/repo_normalize.py` & `antgo-0.1.1/antgo/pipeline/utils/repo_normalize.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/css/359.32c5c11e.css` & `antgo-0.1.1/antgo/resource/app/css/359.32c5c11e.css`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/css/385.1759eef9.css` & `antgo-0.1.1/antgo/resource/app/css/385.1759eef9.css`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/css/chunk-vendors.1944359c.css` & `antgo-0.1.1/antgo/resource/app/css/chunk-vendors.1944359c.css`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/favicon.ico` & `antgo-0.1.1/antgo/resource/app/favicon.ico`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/index.html` & `antgo-0.1.1/antgo/resource/app/index.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/359.afb86915.js` & `antgo-0.1.1/antgo/resource/app/js/359.afb86915.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/359.afb86915.js.map` & `antgo-0.1.1/antgo/resource/app/js/359.afb86915.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/385.90ba0f66.js` & `antgo-0.1.1/antgo/resource/app/js/385.90ba0f66.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/385.90ba0f66.js.map` & `antgo-0.1.1/antgo/resource/app/js/385.90ba0f66.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/532.f949def3.js` & `antgo-0.1.1/antgo/resource/app/js/532.f949def3.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/532.f949def3.js.map` & `antgo-0.1.1/antgo/resource/app/js/532.f949def3.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/651.c5601578.js` & `antgo-0.1.1/antgo/resource/app/js/651.c5601578.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/651.c5601578.js.map` & `antgo-0.1.1/antgo/resource/app/js/651.c5601578.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/769.b7247054.js` & `antgo-0.1.1/antgo/resource/app/js/769.b7247054.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/769.b7247054.js.map` & `antgo-0.1.1/antgo/resource/app/js/769.b7247054.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/854.d3c0e54f.js` & `antgo-0.1.1/antgo/resource/app/js/854.d3c0e54f.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/854.d3c0e54f.js.map` & `antgo-0.1.1/antgo/resource/app/js/854.d3c0e54f.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/880.cba02e88.js` & `antgo-0.1.1/antgo/resource/app/js/880.cba02e88.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/880.cba02e88.js.map` & `antgo-0.1.1/antgo/resource/app/js/880.cba02e88.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/app.f01f9b7a.js` & `antgo-0.1.1/antgo/resource/app/js/app.f01f9b7a.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/app.f01f9b7a.js.map` & `antgo-0.1.1/antgo/resource/app/js/app.f01f9b7a.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/chunk-vendors.18913786.js` & `antgo-0.1.1/antgo/resource/app/js/chunk-vendors.18913786.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/app/js/chunk-vendors.18913786.js.map` & `antgo-0.1.1/antgo/resource/app/js/chunk-vendors.18913786.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/html.py` & `antgo-0.1.1/antgo/resource/html.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/static/antgo.ico` & `antgo-0.1.1/antgo/resource/static/antgo.ico`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/static/antgo.js` & `antgo-0.1.1/antgo/resource/static/antgo.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/static/apply.png` & `antgo-0.1.1/antgo/resource/static/apply.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/static/banner.png` & `antgo-0.1.1/antgo/resource/static/banner.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/static/card.png` & `antgo-0.1.1/antgo/resource/static/card.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/static/filetree.png` & `antgo-0.1.1/antgo/resource/static/filetree.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/static/holder.min.js` & `antgo-0.1.1/antgo/resource/static/holder.min.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/static/register.png` & `antgo-0.1.1/antgo/resource/static/register.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/static/start-experiment.png` & `antgo-0.1.1/antgo/resource/static/start-experiment.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/activelearning.html` & `antgo-0.1.1/antgo/resource/templates/activelearning.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/crowdsource.html` & `antgo-0.1.1/antgo/resource/templates/crowdsource.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/demo.html` & `antgo-0.1.1/antgo/resource/templates/demo.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/mvp/README.md` & `antgo-0.1.1/antgo/resource/templates/mvp/README.md`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/mvp/cifar10/configs/config.py` & `antgo-0.1.1/antgo/resource/templates/mvp/cifar10/configs/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/mvp/cifar10/dataset.py` & `antgo-0.1.1/antgo/resource/templates/mvp/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/mvp/cifar10/hooks.py` & `antgo-0.1.1/antgo/resource/templates/mvp/cifar10/hooks.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/mvp/cifar10/main.py` & `antgo-0.1.1/antgo/resource/templates/mvp/cifar10/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,31 +240,38 @@
                 cfg.data.test.data_path_list = unlabel_local_path_list
 
             # step3.4: 模型配置扩展
             if 'model' in extra_config:
                 # 更新默认配置
                 default_model_cfg = cfg.model
                 if 'model' in extra_config['model'] and \
-                    'student' in extra_config['model']['model'] and \
                     'teacher' in extra_config['model']['model']:
                     cfg.model = dict(
                         type=extra_config['model']['type'],
                         model=dict(
                             teacher=extra_config['model']['model']['teacher'],
-                            student=extra_config['model']['model']['student']
+                            student=default_model_cfg
                         ),
                         train_cfg=extra_config['model']['train_cfg'] if 'train_cfg' in extra_config['model'] else None,
                         test_cfg=extra_config['model']['test_cfg'] if 'test_cfg' in extra_config['model'] else None,
                         init_cfg=extra_config['model']['init_cfg'] if 'init_cfg' in extra_config['model'] else None
                     )
                     
                     if cfg.model.model.teacher is None:
                         cfg.model.model.teacher = default_model_cfg
                     if cfg.model.model.student is None:
                         cfg.model.model.student = default_model_cfg
+                        
+                    if cfg.model.train_cfg is not None:
+                        if 'student' in cfg.model.train_cfg:
+                            align_name = cfg.model.train_cfg.align
+                            if 'channels' in cfg.model.train_cfg.student:
+                                cfg.model.train_cfg.student.channels = cfg.info.get(align_name).channels
+                            if 'shapes' in cfg.model.train_cfg.student:
+                                cfg.model.train_cfg.student.shapes = cfg.info.get(align_name).shapes 
                 else:
                     cfg.model = dict(
                         type=extra_config['model']['type'],
                         model=default_model_cfg,
                         train_cfg=extra_config['model']['train_cfg'] if 'train_cfg' in extra_config['model'] else None,
                         test_cfg=extra_config['model']['test_cfg'] if 'test_cfg' in extra_config['model'] else None,
                         init_cfg=extra_config['model']['init_cfg'] if 'init_cfg' in extra_config['model'] else None
```

### Comparing `antgo-0.1.0/antgo/resource/templates/mvp/cifar10/metrics.py` & `antgo-0.1.1/antgo/resource/templates/mvp/cifar10/metrics.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/mvp/cifar10/models/wideres.py` & `antgo-0.1.1/antgo/resource/templates/mvp/cifar10/models/wideres.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/mvp/config.py` & `antgo-0.1.1/antgo/resource/templates/mvp/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/mvp/lsp_config.py` & `antgo-0.1.1/antgo/resource/templates/mvp/lsp_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,22 @@
     head=dict(
         type='SimpleQNetLite0PoseHeatmap2D',
         num_deconv_filters=[128, 128, 128],
         num_joints=14
     )
 )
 
+# 描述模型基本信息
+info = dict(
+    backbone=dict(
+        channels=[96,128,160],
+        shapes=[16,8,4]
+    )
+)
+
 # checkpoint配置
 checkpoint_config = dict(interval=1, out_dir='./output/')       
 
 # 数据配置
 data=dict(
     train=dict(
         type='LSP',
```

### Comparing `antgo-0.1.0/antgo/resource/templates/mvp/pascal_voc_config.py` & `antgo-0.1.1/antgo/resource/templates/mvp/pascal_voc_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,22 @@
         in_channels=32,
         channels=32,
         out_channels=21,
         ignore_index=255
     )
 )
 
+# 描述模型基本信息
+info = dict(
+    backbone=dict(
+        channels=[96,128,160],
+        shapes=[32,16,8]
+    )
+)
+
 # checkpoint配置
 checkpoint_config = dict(interval=1, out_dir='./output/')       
 
 # 数据配置
 data=dict(
     train=dict(
         type='Pascal2012',
```

### Comparing `antgo-0.1.0/antgo/resource/templates/mvp/system.py` & `antgo-0.1.1/antgo/resource/templates/mvp/system.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/mvp/visalso_config.py` & `antgo-0.1.1/antgo/resource/templates/mvp/visalso_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,30 +29,36 @@
         in_channel=32,
         feat_channel=32,
         num_classes=4,
         down_stride=4,
         score_thresh=0.2,
         train_cfg=None,
         test_cfg=dict(topk=100, local_maximum_kernel=3),
-        loss_ch=dict(type='GaussianFocalLoss', loss_weight=1.0),
-        loss_wh=dict(type='L1Loss', loss_weight=1.0)
+        loss_ch=dict(type='GaussianFocalLoss', loss_weight=1.0)
     ),  
 )
 
+# 描述模型基本信息
+info = dict(
+    backbone=dict(
+        channels=[512, 1024, 2048],
+        shapes=[32,16,8]
+    )
+)
+
 # checkpoint配置
 checkpoint_config = dict(interval=1, out_dir='./output/')       
 
 # 数据配置
 data=dict(
     train=dict(
         type='VisalSO',
         train_or_test='train',
         dir='./visalso_dataset',
         pipeline=[
-            dict(type="Meta"),
             dict(type="ResizeByShort", short_size=256),
             dict(type="RandomScaledCrop", target_size=(256,256)),
             dict(type="Rotation", degree=15),
             dict(type='ResizeS', target_dim=[256,256]),
             dict(type='ColorDistort', hue=[-5,5,0.3], saturation=[0.8,1.2,0.3], contrast=[0.8,1.2,0.3], brightness=[0.8,1.2,0.3]),
             dict(type='RandomFlipImage', swap_labels=[]),
             dict(type='INormalize', mean=[128.0,128.0,128.0], std=[128.0,128.0,128.0],to_rgb=False, keys=['image']),
@@ -70,15 +76,14 @@
         ignore_stack=['bboxes', 'labels', 'image_meta']
     ),
     val=dict(
         type='VisalSO',
         train_or_test='val',
         dir='./visalso_dataset',
         pipeline=[
-            dict(type="Meta"),
             dict(type="ResizeByShort", short_size=256),
             dict(type='FixedCrop', target_size=(256,256), align='center'),
             dict(type='ResizeS', target_dim=[256,256]),
             dict(type='INormalize', mean=[128.0,128.0,128.0], std=[128.0,128.0,128.0],to_rgb=False, keys=['image']),
             dict(type='IImageToTensor', keys=['image'])
         ],
         inputs_def=dict(
@@ -93,15 +98,14 @@
         ignore_stack=['bboxes', 'labels', 'image_meta']
     ),
     test=dict(
         type='VisalSO',
         train_or_test='test',
         dir='./visalso_dataset',
         pipeline=[
-            dict(type="Meta"),
             dict(type="ResizeByShort", short_size=256),
             dict(type='FixedCrop', target_size=(256,256), align='center'),
             dict(type='ResizeS', target_dim=[256,256]),
             dict(type='INormalize', mean=[128.0,128.0,128.0], std=[128.0,128.0,128.0],to_rgb=False, keys=['image']),
             dict(type='IImageToTensor', keys=['image'])
         ],
         inputs_def=dict(
@@ -119,15 +123,15 @@
 
 # 评估方案配置
 evaluation=dict(
     out_dir='./output/', 
     interval=1, 
     metric=dict(
         type='COCOCompatibleEval', 
-        categories=[{'name': 'left', 'id': 1}, {'name': 'left', 'id': 2}]
+        categories=[{'name': f'{label}', 'id': label} for label in range(4)]
     ), 
     save_best='AP@[ IoU=0.50:0.95 | area= all | maxDets=100 ]',
     rule='greater'
 )
 
 # 导出配置
 export=dict(
```

### Comparing `antgo-0.1.0/antgo/resource/templates/project.json` & `antgo-0.1.1/antgo/resource/templates/project.json`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/sample_gt.json` & `antgo-0.1.1/antgo/resource/templates/sample_gt.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9714285714285714%*

 * *Differences: {'delete': "['has_segments']"}*

```diff
@@ -8,15 +8,14 @@
     "cam_param": {},
     "clip_tag": "",
     "has_bboxes3d": false,
     "has_cam_param": false,
     "has_dof": [],
     "has_joints2d": [],
     "has_joints3d": [],
-    "has_segments": [],
     "height": 0,
     "image_file": "",
     "image_label": -1,
     "image_label_name": "",
     "image_url": "",
     "joints2d": [],
     "joints3d": [],
```

### Comparing `antgo-0.1.0/antgo/resource/templates/statistic-report.html` & `antgo-0.1.1/antgo/resource/templates/statistic-report.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/task_main_file.template` & `antgo-0.1.1/antgo/resource/templates/task_main_file.template`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/task_main_param.template` & `antgo-0.1.1/antgo/resource/templates/task_main_param.template`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/task_shell.template` & `antgo-0.1.1/antgo/resource/templates/task_shell.template`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/trainmaster.html` & `antgo-0.1.1/antgo/resource/templates/trainmaster.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/resource/templates/yesno_crowdsource.html` & `antgo-0.1.1/antgo/resource/templates/yesno_crowdsource.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/sandbox/sandbox.py` & `antgo-0.1.1/antgo/sandbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/script/base.py` & `antgo-0.1.1/antgo/script/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -64,21 +64,41 @@
         # 检查是否有蒸馏学习配置
         if len(project_info['tool']['distillation']['config']) == 0:
             logging.error(f"Missing {task_name} config, couldnt launch task")
             return None
 
         # 检查是否有标签数据  
         if len(project_info['dataset']['train']['label']) == 0:
-            logging.error(f"No eough label data.")
+            logging.error(f"No enough label data.")
             return None
 
         # 扩展数据源 (蒸馏学习涉及，标签数据，伪标签数据)
         # label, pseudo-label, unlabel
         extra_config['source'] = {
             "label": project_info["dataset"]["train"]["label"],
             "pseudo-label": project_info["dataset"]["train"]["pseudo-label"],
         }
 
         # 扩展模型配置/优化器/学习率等
-        extra_config.update( project_info['tool']['distillation']['config'])
+        extra_config.update(project_info['tool']['distillation']['config'])
+        
+        # 更新专家模型配置
+        if len(project_info['expert']) == 0:
+            logging.error("No enough expert model config")
+            return None
+        # 专家模型配置样式
+        # {
+        #     'config': dict(model=dict(), info=dict()),
+        #     'checkpoint': '',
+        # }
+        extra_config['model']['model']['teacher'] = project_info['expert'][0]['config']['model']
+        extra_config['model']['init_cfg'] = {'checkpoint': project_info['expert'][0]['checkpoint']}
+        
+        info =  project_info['expert'][0]['config']['info']
+        if 'channels' in extra_config['model']['train_cfg']['teacher']:
+            align_name = extra_config['model']['train_cfg']['align']
+            extra_config['model']['train_cfg']['teacher']['channels'] = info.get(align_name).get('channels')
+        if 'shapes' in extra_config['model']['train_cfg']['teacher']:
+            align_name = extra_config['model']['train_cfg']['align']
+            extra_config['model']['train_cfg']['teacher']['shapes'] = info.get(align_name).get('shapes')
 
     return extra_config
```

### Comparing `antgo-0.1.0/antgo/script/custom_submit.py` & `antgo-0.1.1/antgo/script/custom_submit.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/script/data_convert_cifar10_tfrecord.py` & `antgo-0.1.1/antgo/script/data_convert_cifar10_tfrecord.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/script/data_prepare.py` & `antgo-0.1.1/antgo/script/data_prepare.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/script/local_submit.py` & `antgo-0.1.1/antgo/script/local_submit.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/script/ssh-submit.sh` & `antgo-0.1.1/antgo/script/ssh-submit.sh`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/script/ssh_submit.py` & `antgo-0.1.1/antgo/script/ssh_submit.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/task/task.py` & `antgo-0.1.1/antgo/task/task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/tools/__init__.py` & `antgo-0.1.1/antgo/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/tools/browser_funcs.py` & `antgo-0.1.1/antgo/tools/browser_funcs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/tools/download_funcs.py` & `antgo-0.1.1/antgo/tools/download_funcs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/tools/extract.py` & `antgo-0.1.1/antgo/tools/extract.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/tools/filter_funcs.py` & `antgo-0.1.1/antgo/tools/filter_funcs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/tools/label_funcs.py` & `antgo-0.1.1/antgo/tools/label_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     # 检查参数
     assert(tags is not None)
 
     if tgt_folder is None:
         tgt_folder = './output'
 
     # 如果设置root and exp, 则按照规定规则读取等待标注数据。忽略src_json_file。
-    if root is not None and exp is not None:
+    if root is not None and exp is not None and root != '' and exp != '':
         # 开始标记
         running_flag(os.path.join(root, 'label', exp))
         if file_client_exists(os.path.join(root, 'label', exp, 'data.tar')):
             if not os.path.exists('./label'):
                 os.mkdir('./label')
             
             file_client_get(os.path.join(root, 'label', exp, 'data.tar'), './label/')
@@ -54,17 +54,14 @@
             user_name, password = t.split(':')
             white_users.update({
                 user_name: {'password': password}
             })
     if len(white_users) == 0:
         white_users = None
 
-    if label_type == 'POINT':
-        logging.error(f'Now not support {label_type}')
-        return 
     if label_type is None:
         label_type = ''
 
     assert(label_type in ['', 'RECT','POINT','POLYGON'])
 
     # label_name:0,label_name;1,...
     label_name_and_label_id_map = {}
@@ -198,15 +195,15 @@
          with open(os.path.join(tgt_folder, 'meta.json'), 'r', encoding="utf-8") as fp:
              meta_info = json.load(fp)
 
     meta_info['extent']['total'] = len(total_gt_list)
     with open(os.path.join(tgt_folder, 'meta.json'), 'w', encoding="utf-8") as fp:
         json.dump(meta_info, fp)
 
-    if root is not None and exp is not None:
+    if root is not None and exp is not None and root != '' and exp != '':
         # 仅在设置root and exp后，起作用
         # 1. 打包到tfrecord格式
         package_to_tfrecord(
             os.path.join(tgt_folder, anno_json_file_name), 
             os.path.join(tgt_folder, 'package'),
             prefix=exp,
             size_in_shard=40000,
```

### Comparing `antgo-0.1.0/antgo/tools/package.py` & `antgo-0.1.1/antgo/tools/package.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/_bbox.pyx` & `antgo-0.1.1/antgo/utils/_bbox.pyx`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/_encode_png.pyx` & `antgo-0.1.1/antgo/utils/_encode_png.pyx`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/_mask.pyx` & `antgo-0.1.1/antgo/utils/_mask.pyx`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/args.py` & `antgo-0.1.1/antgo/utils/args.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/argscope.py` & `antgo-0.1.1/antgo/utils/argscope.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/colormap.py` & `antgo-0.1.1/antgo/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/concurrency.py` & `antgo-0.1.1/antgo/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/cpu.py` & `antgo-0.1.1/antgo/utils/cpu.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/encode.py` & `antgo-0.1.1/antgo/utils/encode.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/fs.py` & `antgo-0.1.1/antgo/utils/fs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/gpu.py` & `antgo-0.1.1/antgo/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/logger.py` & `antgo-0.1.1/antgo/utils/logger.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/mask.py` & `antgo-0.1.1/antgo/utils/mask.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/netvis.py` & `antgo-0.1.1/antgo/utils/netvis.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/parallel_map.py` & `antgo-0.1.1/antgo/utils/parallel_map.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/pickledb.py` & `antgo-0.1.1/antgo/utils/pickledb.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/processbar.py` & `antgo-0.1.1/antgo/utils/processbar.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/sample_gt.py` & `antgo-0.1.1/antgo/utils/sample_gt.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/serialize.py` & `antgo-0.1.1/antgo/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/shared_queue/__init__.py` & `antgo-0.1.1/antgo/utils/shared_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/shared_queue/queue.py` & `antgo-0.1.1/antgo/utils/shared_queue/queue.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/shared_queue/sharedmemory.py` & `antgo-0.1.1/antgo/utils/shared_queue/sharedmemory.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/timer.py` & `antgo-0.1.1/antgo/utils/timer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo/utils/utils.py` & `antgo-0.1.1/antgo/utils/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/antgo.egg-info/PKG-INFO` & `antgo-0.1.1/antgo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: antgo
-Version: 0.1.0
+Version: 0.1.1
 Summary: machine learning experiment platform
 Home-page: https://github.com/jianzfb/antgo
 Author: jian
 Author-email: jian@mltalker.com
-License: UNKNOWN
-Platform: UNKNOWN
 License-File: LICENSE.md
 
 ======================
 Antgo
 ======================
 
 .. image:: https://raw.githubusercontent.com/jianzfb/antgo/master/antgo/resource/static/card.png
@@ -176,8 +174,7 @@
 
 antgo train exp
 
 
 5.step Run Challenge Task
 
 antgo challenge exp experiment_uuid
-
```

### Comparing `antgo-0.1.0/antgo.egg-info/SOURCES.txt` & `antgo-0.1.1/antgo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

```diff
@@ -59,14 +59,15 @@
 antgo/dataflow/datasetio.py
 antgo/dataflow/recorder.py
 antgo/dataflow/vis.py
 antgo/dataflow/dataset/__init__.py
 antgo/dataflow/dataset/ade20k.py
 antgo/dataflow/dataset/celeba.py
 antgo/dataflow/dataset/cifar.py
+antgo/dataflow/dataset/cityscape.py
 antgo/dataflow/dataset/clsdataset.py
 antgo/dataflow/dataset/coco2017.py
 antgo/dataflow/dataset/cusdomcls.py
 antgo/dataflow/dataset/dataset.py
 antgo/dataflow/dataset/empty_dataset.py
 antgo/dataflow/dataset/fashionai_attribute.py
 antgo/dataflow/dataset/fashionai_landmark.py
@@ -85,16 +86,14 @@
 antgo/dataflow/dataset/proxy_dataset.py
 antgo/dataflow/dataset/queue_dataset.py
 antgo/dataflow/dataset/random_dataset.py
 antgo/dataflow/dataset/reader.py
 antgo/dataflow/dataset/simpleimages.py
 antgo/dataflow/dataset/simplevideos.py
 antgo/dataflow/dataset/spider_dataset.py
-antgo/dataflow/dataset/standard.py
-antgo/dataflow/dataset/svhn.py
 antgo/dataflow/dataset/vggface.py
 antgo/dataflow/dataset/visalso.py
 antgo/dataflow/datasynth/__init__.py
 antgo/dataflow/imgaug/__init__.py
 antgo/dataflow/imgaug/autoaugment_utils.py
 antgo/dataflow/imgaug/batch_operators.py
 antgo/dataflow/imgaug/colorspace.py
@@ -160,14 +159,16 @@
 antgo/framework/helper/cnn/utils/sync_bn.py
 antgo/framework/helper/cnn/utils/weight_init.py
 antgo/framework/helper/configs/__init__.py
 antgo/framework/helper/configs/activelearning/__init__.py
 antgo/framework/helper/configs/activelearning/ac_config.py
 antgo/framework/helper/configs/adda/__init__.py
 antgo/framework/helper/configs/adda/adda_config.py
+antgo/framework/helper/configs/distillation/__init__.py
+antgo/framework/helper/configs/distillation/reviewkd_config.py
 antgo/framework/helper/configs/semi/__init__.py
 antgo/framework/helper/configs/semi/dense_config.py
 antgo/framework/helper/configs/semi/detmpl_config.py
 antgo/framework/helper/configs/semi/mpl_config.py
 antgo/framework/helper/dataset/__init__.py
 antgo/framework/helper/dataset/builder.py
 antgo/framework/helper/dataset/dataset_filter.py
@@ -281,14 +282,15 @@
 antgo/framework/helper/models/detectors/core/mask/utils.py
 antgo/framework/helper/models/detectors/core/utils/__init__.py
 antgo/framework/helper/models/detectors/core/utils/dist_utils.py
 antgo/framework/helper/models/detectors/core/utils/misc.py
 antgo/framework/helper/models/detectors/head/__init__.py
 antgo/framework/helper/models/detectors/head/base_dense_head.py
 antgo/framework/helper/models/detectors/head/fcos_head.py
+antgo/framework/helper/models/detectors/head/focs_head_ml.py
 antgo/framework/helper/models/detectors/losses/__init__.py
 antgo/framework/helper/models/detectors/losses/accuracy.py
 antgo/framework/helper/models/detectors/losses/ae_loss.py
 antgo/framework/helper/models/detectors/losses/balanced_l1_loss.py
 antgo/framework/helper/models/detectors/losses/cross_entropy_loss.py
 antgo/framework/helper/models/detectors/losses/dice_loss.py
 antgo/framework/helper/models/detectors/losses/focal_loss.py
@@ -308,27 +310,27 @@
 antgo/framework/helper/models/detectors/neck/__init__.py
 antgo/framework/helper/models/detectors/neck/fpn.py
 antgo/framework/helper/models/detectors/utils/__init__.py
 antgo/framework/helper/models/detectors/utils/gaussian_target.py
 antgo/framework/helper/models/detectors/utils/util_mixins.py
 antgo/framework/helper/models/detectors/utils/util_random.py
 antgo/framework/helper/models/distillation/__init__.py
-antgo/framework/helper/models/distillation/detection_distiller.py
-antgo/framework/helper/models/distillation/experts.py
+antgo/framework/helper/models/distillation/distillation_model.py
 antgo/framework/helper/models/distillation/loss/__init__.py
 antgo/framework/helper/models/distillation/loss/ab.py
 antgo/framework/helper/models/distillation/loss/afd.py
 antgo/framework/helper/models/distillation/loss/at.py
 antgo/framework/helper/models/distillation/loss/bss.py
 antgo/framework/helper/models/distillation/loss/cc.py
 antgo/framework/helper/models/distillation/loss/crd.py
 antgo/framework/helper/models/distillation/loss/dml.py
 antgo/framework/helper/models/distillation/loss/fitnet.py
 antgo/framework/helper/models/distillation/loss/fsp.py
 antgo/framework/helper/models/distillation/loss/ft.py
+antgo/framework/helper/models/distillation/loss/hcl.py
 antgo/framework/helper/models/distillation/loss/irg.py
 antgo/framework/helper/models/distillation/loss/logits.py
 antgo/framework/helper/models/distillation/loss/lwm.py
 antgo/framework/helper/models/distillation/loss/mgd.py
 antgo/framework/helper/models/distillation/loss/nst.py
 antgo/framework/helper/models/distillation/loss/ofd.py
 antgo/framework/helper/models/distillation/loss/pkt.py
@@ -703,15 +705,17 @@
 antgo/resource/templates/task.template
 antgo/resource/templates/task_main_file.template
 antgo/resource/templates/task_main_param.template
 antgo/resource/templates/task_shell.template
 antgo/resource/templates/trainmaster.html
 antgo/resource/templates/trainworker.html
 antgo/resource/templates/yesno_crowdsource.html
+antgo/resource/templates/mvp/.gitignore
 antgo/resource/templates/mvp/README.md
+antgo/resource/templates/mvp/coco_config.py
 antgo/resource/templates/mvp/config.py
 antgo/resource/templates/mvp/install.sh
 antgo/resource/templates/mvp/launch.sh
 antgo/resource/templates/mvp/lsp_config.py
 antgo/resource/templates/mvp/pascal_voc_config.py
 antgo/resource/templates/mvp/requirements.txt
 antgo/resource/templates/mvp/system.py
```

### Comparing `antgo-0.1.0/setup.py` & `antgo-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 def read_requirements(filename):
     return [line.strip() for line in read_file(filename).splitlines()
             if not line.startswith('#')]
 
 
 setup(name='antgo',
-      version='0.1.0',
+      version='0.1.1',
       description='machine learning experiment platform',
       __short_description__='machine learning experiment platform',
       url='https://github.com/jianzfb/antgo',
       author='jian',
       author_email='jian@mltalker.com',
       setup_requires=[
         # Setuptools 18.0 properly handles Cython extensions.
```

### Comparing `antgo-0.1.0/test/test_antgo.py` & `antgo-0.1.1/test/test_antgo.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/test/test_paddle_c.py` & `antgo-0.1.1/test/test_paddle_c.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.0/test/test_torch_c.py` & `antgo-0.1.1/test/test_torch_c.py`

 * *Files identical despite different names*

