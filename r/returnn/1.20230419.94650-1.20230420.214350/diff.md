# Comparing `tmp/returnn-1.20230419.94650.tar.gz` & `tmp/returnn-1.20230420.214350.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230419.94650.tar", last modified: Wed Apr 19 08:05:41 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230420.214350.tar", last modified: Thu Apr 20 19:58:28 2023, max compression
```

## Comparing `returnn-1.20230419.94650.tar` & `returnn-1.20230420.214350.tar`

### file list

```diff
@@ -1,433 +1,433 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-19 08:05:19.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-19 08:05:23.000000 returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34980 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20833 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97723 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   155376 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tensor/tensor_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151440 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35293 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    69825 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   588881 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   538888 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   293047 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51711 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144922 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:05:41.000000 returnn-1.20230419.94650/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-19 08:05:17.000000 returnn-1.20230419.94650/tools/tf_inspect_summary_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 19:58:03.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-20 19:58:07.000000 returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/extern/graph_editor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34898 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16971 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20833 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97723 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157144 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tensor/tensor_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151440 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35293 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69825 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   588881 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   539812 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   293047 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21969 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52325 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144922 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:58:28.000000 returnn-1.20230420.214350/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-20 19:58:01.000000 returnn-1.20230420.214350/tools/tf_inspect_summary_log.py
```

### Comparing `returnn-1.20230419.94650/.gitignore` & `returnn-1.20230420.214350/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/.gitmodules` & `returnn-1.20230420.214350/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/CHANGELOG.md` & `returnn-1.20230420.214350/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/CODEOWNERS` & `returnn-1.20230420.214350/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/CONTRIBUTING.md` & `returnn-1.20230420.214350/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/LICENSE` & `returnn-1.20230420.214350/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/MANIFEST.in` & `returnn-1.20230420.214350/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/PKG-INFO` & `returnn-1.20230420.214350/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230419.94650
+Version: 1.20230420.214350
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230419.94650/README.rst` & `returnn-1.20230420.214350/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/__init__.py` & `returnn-1.20230420.214350/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/12AX.cluster_map` & `returnn-1.20230420.214350/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-fwd.config` & `returnn-1.20230420.214350/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-horovod-mpi.py` & `returnn-1.20230420.214350/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230420.214350/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-hyper-param-tuning.config` & `returnn-1.20230420.214350/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-iter-dataset.py` & `returnn-1.20230420.214350/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-list-devices.py` & `returnn-1.20230420.214350/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-lua-torch-layer.config` & `returnn-1.20230420.214350/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230420.214350/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-returnn-as-framework.py` & `returnn-1.20230420.214350/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-rf.config` & `returnn-1.20230420.214350/demos/demo-rf.config`

 * *Files 20% similar despite different names*

```diff
@@ -29,33 +29,38 @@
 batching = "random"
 batch_size = 5000
 max_seqs = 10
 
 class Model(rf.Module):
     def __init__(self):
         super().__init__()
-        self.layer1 = rf.Linear(in_dim, Dim(50, name="hidden"))
-        self.layer2 = rf.Linear(self.layer1.out_dim, Dim(100, name="hidden2"))
-        self.layer3 = rf.Linear(self.layer2.out_dim, out_dim)
-
-    def __call__(self, x: Tensor):
-        x = rf.relu(self.layer1(x))
-        x = rf.relu(self.layer2(x))
-        x = self.layer3(x)
+        hidden_dim = Dim(50, name="hidden")
+        hidden2_dim = Dim(100, name="hidden2")
+        self.layers = rf.ModuleList(
+            rf.Conv1d(in_dim, hidden_dim, 5, padding="same"),
+            rf.Conv1d(hidden_dim, hidden2_dim, 5, padding="same"),
+            rf.Conv1d(hidden2_dim, out_dim, 5, padding="same"),
+        )
+
+    def __call__(self, x: Tensor, *, spatial_dim: Dim):
+        for layer in self.layers[:-1]:
+            x, _ = layer(x, in_spatial_dim=spatial_dim)
+            x = rf.relu(x)
+        x, _ = self.layers[-1](x, in_spatial_dim=spatial_dim)
         return x  # logits
 
 def get_model(**_kwargs):
     return Model()
 
 def train_step(*, model: Model, extern_data, **_kwargs):
     data = extern_data["data"]
-    logits = model(data)
-    logits_packed, pack_dim = rf.pack(logits, dims=(batch_dim, time_dim), enforce_sorted=False)
+    logits = model(data, spatial_dim=time_dim)
+    logits_packed, pack_dim = rf.pack_padded(logits, dims=(batch_dim, time_dim), enforce_sorted=False)
     targets = extern_data["classes"]
-    targets_packed, _ = rf.pack(targets, dims=(batch_dim, time_dim), enforce_sorted=False, out_dim=pack_dim)
+    targets_packed, _ = rf.pack_padded(targets, dims=(batch_dim, time_dim), enforce_sorted=False, out_dim=pack_dim)
     loss = rf.cross_entropy(estimated=logits_packed, estimated_type="logits", target=targets_packed, axis=out_dim)
     loss.mark_as_loss(name="ce")
     best = rf.reduce_argmax(logits_packed, axis=out_dim)
     frame_error = best != targets_packed
     frame_error.mark_as_loss(name="fer", as_error=True)
```

### Comparing `returnn-1.20230419.94650/demos/demo-rhn-enwik8.config` & `returnn-1.20230420.214350/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-sprint-interface.py` & `returnn-1.20230420.214350/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-att-copy.config` & `returnn-1.20230420.214350/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-attention.config` & `returnn-1.20230420.214350/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230420.214350/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230420.214350/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-enc-dec.config` & `returnn-1.20230420.214350/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230420.214350/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230420.214350/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230420.214350/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230420.214350/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230420.214350/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230420.214350/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230420.214350/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230420.214350/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230420.214350/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230420.214350/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-rec-self-att.config` & `returnn-1.20230420.214350/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230420.214350/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230420.214350/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230420.214350/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-torch.config` & `returnn-1.20230420.214350/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230420.214350/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/demo.sh` & `returnn-1.20230420.214350/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230420.214350/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230420.214350/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230420.214350/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/IAM/README.txt` & `returnn-1.20230420.214350/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/IAM/config_demo` & `returnn-1.20230420.214350/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230420.214350/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/IAM/config_real` & `returnn-1.20230420.214350/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230420.214350/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/IAM/decode.py` & `returnn-1.20230420.214350/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230420.214350/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230420.214350/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230420.214350/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230420.214350/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230420.214350/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230420.214350/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230420.214350/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230420.214350/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230420.214350/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230420.214350/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/__init__.py` & `returnn-1.20230420.214350/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/__main__.py` & `returnn-1.20230420.214350/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/__old_mod_loader__.py` & `returnn-1.20230420.214350/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/__setup__.py` & `returnn-1.20230420.214350/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/config.py` & `returnn-1.20230420.214350/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/audio.py` & `returnn-1.20230420.214350/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/basic.py` & `returnn-1.20230420.214350/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/bundle_file.py` & `returnn-1.20230420.214350/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/cached.py` & `returnn-1.20230420.214350/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/cached2.py` & `returnn-1.20230420.214350/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/generating.py` & `returnn-1.20230420.214350/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/hdf.py` & `returnn-1.20230420.214350/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/lm.py` & `returnn-1.20230420.214350/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/map.py` & `returnn-1.20230420.214350/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/meta.py` & `returnn-1.20230420.214350/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/multi_proc.py` & `returnn-1.20230420.214350/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/normalization_data.py` & `returnn-1.20230420.214350/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/numpy_dump.py` & `returnn-1.20230420.214350/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/raw_wav.py` & `returnn-1.20230420.214350/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/sprint.py` & `returnn-1.20230420.214350/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/stereo.py` & `returnn-1.20230420.214350/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230420.214350/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/datasets/util/vocabulary.py` & `returnn-1.20230420.214350/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/engine/base.py` & `returnn-1.20230420.214350/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/engine/batch.py` & `returnn-1.20230420.214350/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230420.214350/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230420.214350/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230420.214350/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230420.214350/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/graph_editor/edit.py` & `returnn-1.20230420.214350/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230420.214350/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/graph_editor/select.py` & `returnn-1.20230420.214350/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230420.214350/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/graph_editor/transform.py` & `returnn-1.20230420.214350/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/extern/graph_editor/util.py` & `returnn-1.20230420.214350/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/__init__.py` & `returnn-1.20230420.214350/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/_backend.py` & `returnn-1.20230420.214350/returnn/frontend/_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,17 +200,16 @@
         """
         :param tensor: tensor
         :param perm: permutation
         :param allow_int: allow int as axis in perm
         :return: transposed tensor
         """
         # Default implementation using transpose_raw.
-        out = tensor.copy_template_transpose(perm, allow_int=allow_int)
+        out, perm_ = tensor.copy_template_transpose(perm, allow_int=allow_int)
         backend = get_backend_by_tensor(tensor)
-        perm_ = [tensor.get_axis_from_description(a, allow_int=allow_int) for a in perm]
         out.raw_tensor = backend.transpose_raw(tensor.raw_tensor, perm_)
         return out
 
     @staticmethod
     def expand_dims_raw(raw_tensor: T, axis: int) -> T:
         """
         :param raw_tensor:
```

### Comparing `returnn-1.20230419.94650/returnn/frontend/_numpy_backend.py` & `returnn-1.20230420.214350/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/_utils.py` & `returnn-1.20230420.214350/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/array_.py` & `returnn-1.20230420.214350/returnn/frontend/array_.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "reshape",
     "split",
     "expand_dim",
     "concat",
     "pad",
     "cum_concat_step",
     "masked_select",
-    "pack",
+    "pack_padded",
     "gather",
     "slice",
 ]
 
 
 def convert_to_tensor(
     value: Union[Tensor, T, RawTensorTypes],
@@ -308,15 +308,15 @@
         the new dim is also returned.
         if mask==True for all elements, the returned tensor would be simply the flattened input tensor.
     """
     # noinspection PyProtectedMember
     return tensor._raw_backend.masked_select(tensor, mask=mask, dims=dims, out_dim=out_dim)
 
 
-def pack(
+def pack_padded(
     source: Tensor, *, dims: Sequence[Dim], enforce_sorted: bool = True, out_dim: Optional[Dim] = None
 ) -> Tuple[Tensor, Dim]:
     """
     Like pack_padded_sequence. Usually the sequences are padded when they have different lengths.
     Packing means to only store the non-padded frames.
     This uses :func:`masked_select` internally based on the mask of non-masked frames.
```

### Comparing `returnn-1.20230419.94650/returnn/frontend/attention.py` & `returnn-1.20230420.214350/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/cond.py` & `returnn-1.20230420.214350/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/const.py` & `returnn-1.20230420.214350/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/container.py` & `returnn-1.20230420.214350/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/conv.py` & `returnn-1.20230420.214350/returnn/frontend/conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
           the input data ndim must match, or you can add dimensions via input_expand_dims or input_add_feature_dim.
           it will automatically swap the batch-dim to the first axis of the input data.
         :param padding: "same" or "valid"
         :param with_bias:
         """
         super().__init__()
         assert isinstance(in_dim, Dim) and isinstance(out_dim, Dim)
-        self.in_dim = in_dim
+        self.in_dim = rf.dim_match_priority_when_needed(in_dim, out_dim)
         self.out_dim = out_dim
         if isinstance(filter_size, (int, Dim)):
             if self.nd in (None, 1):
                 filter_size = [filter_size]
             else:
                 filter_size = [filter_size] * self.nd
         assert isinstance(filter_size, (tuple, list))
```

### Comparing `returnn-1.20230419.94650/returnn/frontend/dims.py` & `returnn-1.20230420.214350/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/dropout.py` & `returnn-1.20230420.214350/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/dtype.py` & `returnn-1.20230420.214350/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/encoder/base.py` & `returnn-1.20230420.214350/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/encoder/conformer.py` & `returnn-1.20230420.214350/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/init.py` & `returnn-1.20230420.214350/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/linear.py` & `returnn-1.20230420.214350/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/loop.py` & `returnn-1.20230420.214350/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/loss.py` & `returnn-1.20230420.214350/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/math_.py` & `returnn-1.20230420.214350/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/matmul.py` & `returnn-1.20230420.214350/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/module.py` & `returnn-1.20230420.214350/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/normalization.py` & `returnn-1.20230420.214350/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/parameter.py` & `returnn-1.20230420.214350/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/rand.py` & `returnn-1.20230420.214350/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/rec.py` & `returnn-1.20230420.214350/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/reduce.py` & `returnn-1.20230420.214350/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/run_ctx.py` & `returnn-1.20230420.214350/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/state.py` & `returnn-1.20230420.214350/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/frontend/types.py` & `returnn-1.20230420.214350/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/import_/common.py` & `returnn-1.20230420.214350/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/import_/git.py` & `returnn-1.20230420.214350/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/import_/import_.py` & `returnn-1.20230420.214350/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/learning_rate_control.py` & `returnn-1.20230420.214350/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/log.py` & `returnn-1.20230420.214350/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/native_op.cpp` & `returnn-1.20230420.214350/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/native_op.py` & `returnn-1.20230420.214350/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/pretrain.py` & `returnn-1.20230420.214350/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/sprint/cache.py` & `returnn-1.20230420.214350/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/sprint/control.py` & `returnn-1.20230420.214350/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/sprint/error_signals.py` & `returnn-1.20230420.214350/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/sprint/extern_interface.py` & `returnn-1.20230420.214350/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/sprint/interface.py` & `returnn-1.20230420.214350/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tensor/_dim_extra.py` & `returnn-1.20230420.214350/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tensor/_tensor_extra.py` & `returnn-1.20230420.214350/returnn/tensor/_tensor_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -655,41 +655,72 @@
         """
         :param perm: permutation of the axes. Maps the new axes to the old axes
         :param allow_int: allow int as axis, otherwise only :class:`Dim`
         :return: copy of myself with permuted axes
         """
         if self.raw_tensor is not None:
             return self._raw_backend.transpose(self, perm, allow_int=allow_int)
-        return self.copy_template_transpose(perm, allow_int=allow_int)
+        out, _ = self.copy_template_transpose(perm, allow_int=allow_int)
+        return out
 
-    def copy_template_transpose(self: Tensor, perm: Sequence[Union[int, Dim]], *, allow_int: bool = True) -> _t.Tensor:
+    def copy_template_transpose(
+        self: Tensor, perm: Sequence[Union[int, Dim]], *, allow_int: bool = True
+    ) -> Tuple[_t.Tensor, List[int]]:
         """
         :param perm: permutation of the axes. Maps the new axes to the old axes
         :param allow_int: allow int as axis, otherwise only :class:`Dim`
-        :return: copy of myself with permuted axes
+        :return: copy of myself with permuted axes, raw permutation (list of original axes)
         """
         assert len(perm) == self.batch_ndim, f"{self}: invalid perm {perm!r} length"
         perm_ = perm
-        perm = [self.get_axis_from_description(a, allow_int=allow_int) for a in perm]
+        if len(set(self.dims)) == len(self.dims) or all(isinstance(a, int) for a in perm):  # all dims are unique?
+            perm = [self.get_axis_from_description(a, allow_int=allow_int) for a in perm]
+        else:
+            # We can have cases where dim tags are not unique.
+            # Using the normal get_axis_from_description logic with match_priority
+            # does not really work for this case.
+            perm = []
+            for a in perm_:
+                if isinstance(a, int):
+                    if not allow_int:
+                        raise ValueError(f"{self} transpose {perm}, axis {a} not allowed with allow_int=False")
+                    if a < 0:
+                        a += self.batch_ndim
+                    assert 0 <= a < self.batch_ndim, f"{self} transpose {perm}, axis {a} out of range"
+                elif isinstance(a, Dim):
+                    matching_dims = [(i, d) for i, d in enumerate(self.dims) if d == a]
+                    if len(matching_dims) == 0:
+                        raise ValueError(f"{self} transpose {perm}, axis {a} not found")
+                    elif len(matching_dims) == 1:
+                        ((a, d),) = matching_dims
+                    else:  # multiple matches
+                        matching_dims_ = [(i, d) for i, d in matching_dims if d.match_priority == a.match_priority]
+                        if len(matching_dims_) == 1:
+                            ((a, d),) = matching_dims_
+                        else:
+                            raise ValueError(f"{self} transpose {perm}, axis {a} multiple matches")
+                else:
+                    raise TypeError(f"{self} transpose {perm}, axis {a} invalid type {type(a)}")
+                perm.append(a)
         assert set(perm) == set(range(self.batch_ndim)), f"{self}: invalid perm {perm_!r} (axes: {perm!r})"
         if all(perm[axis] == axis for axis in range(self.batch_ndim)):
-            return self.copy()
+            return self.copy(), perm
 
         data_opts = self.get_kwargs(include_special_axes=False)
         if self._raw_tensor is not None:
             data_opts["raw_tensor"] = self._raw_backend.transpose_raw(self._raw_tensor, perm)
         data_opts["dims"] = tuple(self.dim_tags[perm[i]] for i in range(self.batch_ndim))
         data = _t.Tensor(**data_opts)
         inv_perm = {j: i for (i, j) in enumerate(perm)}
         if self.version == 1:
             if inv_perm.get(self.time_dim_axis, None) != data.time_dim_axis:
                 data.time_dim_axis = inv_perm.get(self.time_dim_axis, None)
         if inv_perm.get(self.feature_dim_axis, None) != data.feature_dim_axis:
             data.feature_dim_axis = inv_perm.get(self.feature_dim_axis, None)
-        return data
+        return data, perm
 
     def copy_move_axis(self, old_axis, new_axis) -> _t.Tensor:
         """
         :param int old_axis: counted with batch-dim
         :param int new_axis: counted with batch-dim
         :return: copy of myself with moved axis (see :func:`move_axis`)
         """
```

### Comparing `returnn-1.20230419.94650/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230420.214350/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230420.214350/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230420.214350/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tensor/dim.py` & `returnn-1.20230420.214350/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tensor/marked_dim.py` & `returnn-1.20230420.214350/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tensor/tensor.py` & `returnn-1.20230420.214350/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tensor/tensor_dict.py` & `returnn-1.20230420.214350/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/compat.py` & `returnn-1.20230420.214350/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/data_pipeline.py` & `returnn-1.20230420.214350/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/distributed.py` & `returnn-1.20230420.214350/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/engine.py` & `returnn-1.20230420.214350/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230420.214350/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230420.214350/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230420.214350/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230420.214350/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230420.214350/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230420.214350/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230420.214350/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230420.214350/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230420.214350/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/horovod.py` & `returnn-1.20230420.214350/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230420.214350/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/layers/base.py` & `returnn-1.20230420.214350/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/layers/basic.py` & `returnn-1.20230420.214350/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/layers/rec.py` & `returnn-1.20230420.214350/returnn/tf/layers/rec.py`

 * *Files 0% similar despite different names*

```diff
@@ -10910,33 +10910,53 @@
 
     Refs:
 
       https://github.com/Rayhane-mamah/Tacotron-2
       https://arxiv.org/pdf/1606.01305.pdf
     """
 
-    def __init__(self, num_units, zoneout_factor_cell=0.0, zoneout_factor_output=0.0):
+    def __init__(
+        self,
+        num_units: int,
+        zoneout_factor_cell: float = 0.0,
+        zoneout_factor_output: float = 0.0,
+        use_zoneout_output: bool = NotSpecified,
+    ):
         """
         Initializer with possibility to set different zoneout values for cell/hidden states.
 
-        :param int num_units: number of hidden units
-        :param float zoneout_factor_cell: cell zoneout factor
-        :param float zoneout_factor_output: output zoneout factor
+        :param num_units: number of hidden units
+        :param zoneout_factor_cell: cell zoneout factor
+        :param zoneout_factor_output: output zoneout factor
+        :param use_zoneout_output: If False, return the direct output of the underlying LSTM,
+            without applying zoneout. So the output is different from h.
+            This is different from the original Zoneout LSTM paper.
+            If True, h is the same as output, and it is the same as the original Zoneout LSTM paper.
+            This was False in our earlier implementation,
+            and up to behavior version 16.
+            Since behavior version 17, the default is True.
         """
+        from returnn.tf.network import TFNetwork
+        from returnn.util.basic import BehaviorVersion
+
         super(ZoneoutLSTMCell, self).__init__()
 
         zm = min(zoneout_factor_output, zoneout_factor_cell)
         zs = max(zoneout_factor_output, zoneout_factor_cell)
         if zm < 0.0 or zs > 1.0:
             raise ValueError("One/both provided Zoneout factors are not in [0, 1]")
 
         self._cell = rnn_cell.LSTMCell(num_units, state_is_tuple=True)
         self._zoneout_cell = zoneout_factor_cell
         self._zoneout_outputs = zoneout_factor_output
-        from returnn.tf.network import TFNetwork
+
+        if use_zoneout_output is NotSpecified:
+            use_zoneout_output = BehaviorVersion.get() >= 17
+        assert isinstance(use_zoneout_output, bool)
+        self._use_zoneout_output = use_zoneout_output
 
         self.is_training = TFNetwork.get_current_network().train_flag
 
     @property
     def state_size(self):
         """
         :rtype: int
@@ -10982,14 +11002,17 @@
             * tf_compat.v1.nn.dropout(new_h - prev_h, keep_prob=(1 - self._zoneout_outputs))
             + prev_h,
             lambda: (1 - self._zoneout_outputs) * new_h + self._zoneout_outputs * prev_h,
         )
 
         new_state = rnn_cell.LSTMStateTuple(c, h)
 
+        if self._use_zoneout_output:
+            output = h
+
         return output, new_state
 
 
 class RelativePositionalEncodingLayer(_ConcatInputLayer):
     """
     Relative positioning term as introduced by Shaw et al., 2018
```

### Comparing `returnn-1.20230419.94650/returnn/tf/layers/segmental_model.py` & `returnn-1.20230420.214350/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/layers/signal_processing.py` & `returnn-1.20230420.214350/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/native_op.py` & `returnn-1.20230420.214350/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/network.py` & `returnn-1.20230420.214350/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/sprint.py` & `returnn-1.20230420.214350/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/updater.py` & `returnn-1.20230420.214350/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/util/basic.py` & `returnn-1.20230420.214350/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/util/data.py` & `returnn-1.20230420.214350/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/util/ken_lm.py` & `returnn-1.20230420.214350/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/tf/util/open_fst.py` & `returnn-1.20230420.214350/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/torch/data/pipeline.py` & `returnn-1.20230420.214350/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230420.214350/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/torch/data/tensor_utils.py` & `returnn-1.20230420.214350/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/torch/engine.py` & `returnn-1.20230420.214350/returnn/torch/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from torchdata.dataloader2 import DataLoader2
 from random import random
 
 from returnn.config import Config
 from returnn.log import log
 from returnn.engine.base import EngineBase
 import returnn.frontend as rf
-from returnn.tensor import TensorDict, Tensor, batch_dim
+from returnn.tensor import TensorDict, Tensor
 from returnn.datasets.basic import init_dataset, Dataset
 from returnn.util import basic as util
 from returnn.util import NumbersDict
 from .updater import Updater
 from .data import pipeline as data_pipeline
 from .data import returnn_dataset_wrapper
 from .frontend.bridge import rf_module_to_pt_module
@@ -49,15 +49,16 @@
         self._final_epoch = None  # type: Optional[int]
         self._orig_model = None  # type: Optional[Union[rf.Module, torch.nn.Module]]
         self._pt_model = None  # type: Optional[torch.nn.Module]
         self._train_step_func = None  # type: Optional[Callable]
         self._save_model_epoch_interval = 1
         self._updater = None  # type: Optional[Updater]
 
-        self._device = "cuda" if torch.cuda.is_available() else "cpu"
+        self._device = _get_device_from_config(config)
+        print("Using device:", self._device, file=log.v2)
 
     def init_train_from_config(
         self,
         config: Optional[Config] = None,
         train_data: Optional[Dataset] = None,
         dev_data: Optional[Dataset] = None,
         eval_data: Optional[Dataset] = None,
@@ -282,27 +283,34 @@
             return DataLoader2(batches_dataset)
         except TypeError as exc:
             try:
                 # noinspection PyPackageRequirements
                 import dill
             except ImportError:
                 raise ModuleNotFoundError("Possible type error in DataLoader2 due to missing module 'dill'") from exc
+            raise
 
     def _run_step(self, extern_data_raw: Dict[str, torch.Tensor], *, train_flag: bool = False):
         """
         :param dict[str, torch.Tensor] extern_data_raw: model inputs for the step
         """
         assert isinstance(extern_data_raw, dict) and extern_data_raw
+        batch_dim = next(iter(self.extern_data.data.values())).dims[0]
+        batch_dim.dyn_size_ext = None  # if it is dynamic, reset now, and set it below
         extern_data = TensorDict()
         for k, data in self.extern_data.data.items():
             data = data.copy_template()
             raw_tensor = extern_data_raw[k].to(self._device)
             data.dtype = str(raw_tensor.dtype).split(".")[-1]  # just overwrite for now...
             data.raw_tensor = raw_tensor
 
+            if batch_dim.size is None and batch_dim.dyn_size_ext is None:
+                batch_dim.dyn_size_ext = Tensor(batch_dim.name or "batch", dims=[], dtype="int32")
+                batch_dim.dyn_size_ext.raw_tensor = torch.tensor(extern_data_raw[k].shape[0], dtype=torch.int32)
+
             if k + ":seq_len" in extern_data_raw:
                 # Sequence lengths have to be on CPU for the later call to rnn.pack_padded_sequence
                 size = extern_data_raw[k + ":seq_len"].cpu()
                 size_dtype = str(size.dtype).split(".")[-1]
                 if data.dims[1].dyn_size_ext is None:
                     data.dims[1].dyn_size_ext = Tensor(data.dims[1].name or "time", dims=[batch_dim], dtype=size_dtype)
                 data.dims[1].dyn_size_ext.dtype = size_dtype
@@ -478,7 +486,29 @@
     :return: score(s) as str
     """
     if not score:
         return "None"
     if len(score) == 1:
         return str(list(score.values())[0])
     return " ".join(["%s %s" % (key.split(":", 2)[-1], str(score[key])) for key in sorted(score.keys())])
+
+
+def _get_gpu_device() -> Optional[str]:
+    if torch.cuda.is_available():
+        return "cuda"
+    if hasattr(torch.backends, "mps") and torch.backends.mps.is_available() and torch.backends.mps.is_built():
+        return "mps"
+    return None
+
+
+def _get_device_from_config(config: Config) -> str:
+    device = config.value("device", None)
+    if not device:
+        device = _get_gpu_device()
+        if device:
+            return device
+        return "cpu"
+    if device == "gpu":
+        device = _get_gpu_device()
+        if not device:
+            raise Exception("No GPU device found, but config requested 'gpu' device.")
+    return device
```

### Comparing `returnn-1.20230419.94650/returnn/torch/frontend/_backend.py` & `returnn-1.20230420.214350/returnn/torch/frontend/_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -918,15 +918,22 @@
         assert mask.dtype == "bool"
         assert set(mask.dims) == set(dims)
         assert set(mask.dims).issubset(set(tensor.dims))
         remaining_dims = [d for d in tensor.dims if d not in mask.dims]
         tensor_templ = tensor.copy_template_new_dim_tags(tuple(dims) + tuple(remaining_dims))
         tensor = tensor.copy_compatible_to(tensor_templ, add_dims=False)
         mask = mask.copy_compatible_to(tensor_templ, check_dtype=False, check_sparse=False)
-        out_raw = torch.masked_select(tensor.raw_tensor, mask.raw_tensor)
+        in_raw = tensor.raw_tensor
+        # We have a very strange problem with the gradient of masked_select,
+        # when used together with some specific other operations before that,
+        # like convolution.
+        # This clone() with contiguous_format seems to fix the problem.
+        # https://github.com/pytorch/pytorch/issues/99638
+        in_raw = in_raw.clone(memory_format=torch.contiguous_format)
+        out_raw = torch.masked_select(in_raw, mask.raw_tensor)
         remaining_shape = [d.get_dim_value() for d in remaining_dims]
         remaining_num_elements = numpy.prod(remaining_shape) if remaining_shape else 1
         assert out_raw.numel() % remaining_num_elements == 0
         flattened_num_elements = out_raw.numel() // remaining_num_elements
         out_raw = torch.reshape(out_raw, [flattened_num_elements] + remaining_shape)
         if not out_dim:
             out_dim = TorchBackend.get_new_dim_raw(out_raw, 0, name="masked_select")
@@ -1154,20 +1161,23 @@
     ) -> Tuple[_TT, Tuple[_TT, _TT]]:
         """
         Wraps the functional LSTM from PyTorch.
 
         :return: Tuple consisting of two elements: the result as a :class:`Tensor`
             and the new state as a :class:`State` (different from the previous one).
         """
+        # The order in the parameters for lstm_params is specified as follows:
+        # Feed-forward has priority over recurrent, and weights have priority over biases: (w_ih, w_hh, b_ih, b_hh).
+        # See https://github.com/pytorch/pytorch/blob/c263bd43/torch/nn/modules/rnn.py#L107.
+        # Alternatively see the implementation of LSTMCell:
+        # https://github.com/pytorch/pytorch/blob/4bead64/aten/src/ATen/native/RNN.cpp#L1458.
         if bias is None:
             lstm_params = (ff_weight.raw_tensor, rec_weight.raw_tensor)
             has_biases = False
         else:
-            # Feed-forward has priority over recurrent, and weights have priority over biases. See the torch docstring
-            # or torch LSTMCell: https://github.com/pytorch/pytorch/blob/4bead64/aten/src/ATen/native/RNN.cpp#L1458
             # Note that the mathematical definition of the model does not require two bias terms.
             # PyTorch just follows what CuDNN does here.
             # I don't really understand why CuDNN have two bias terms:
             # https://stackoverflow.com/questions/76051800/why-does-the-cudnn-lstm-requires-two-biases-b-ih-and-b-hh
             # It looks like an oversight by the CuDNN devs.
             # I'm not sure if the two bias terms get the same gradient or not.
             # If they do not, that would be mathematical incorrect, but maybe that's how CuDNN works.
```

### Comparing `returnn-1.20230419.94650/returnn/torch/frontend/_rand.py` & `returnn-1.20230420.214350/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/torch/frontend/bridge.py` & `returnn-1.20230420.214350/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/torch/updater.py` & `returnn-1.20230420.214350/returnn/torch/updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,15 @@
         elif callable(optimizer_opts):
             optimizer_opts = {"class": optimizer_opts}
         else:
             if not isinstance(optimizer_opts, dict):
                 raise ValueError("'optimizer' must of type dict, callable or torch.optim.Optimizer instance.")
             if "class" not in optimizer_opts:
                 raise ValueError("'class' field of 'optimizer' dict was not set (use e.g. 'SGD', 'Adam', ...)")
+            optimizer_opts = optimizer_opts.copy()
 
         # Resolve the optimizer class
         optim_class_name = optimizer_opts.pop("class")
         optim_class = get_optimizer_class(optim_class_name)
 
         # Resolve the optimizer arguments
         opt_kwargs = optimizer_opts.copy()
```

### Comparing `returnn-1.20230419.94650/returnn/util/basic.py` & `returnn-1.20230420.214350/returnn/util/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,15 @@
 00001550: 6c20 6265 2073 6574 2061 6674 6572 2074  l be set after t
 00001560: 6865 2063 6f6e 6669 6720 6973 2064 6566  he config is def
 00001570: 696e 6564 2061 7420 5f5f 6d61 696e 5f5f  ined at __main__
 00001580: 2e69 6e69 745f 636f 6e66 6967 2829 206f  .init_config() o
 00001590: 7220 456e 6769 6e65 2e5f 5f69 6e69 745f  r Engine.__init_
 000015a0: 5f28 290a 2020 2020 2222 220a 0a20 2020  _().    """..   
 000015b0: 205f 6c61 7465 7374 5f62 6568 6176 696f   _latest_behavio
-000015c0: 725f 7665 7273 696f 6e20 3d20 3136 0a20  r_version = 16. 
+000015c0: 725f 7665 7273 696f 6e20 3d20 3137 0a20  r_version = 17. 
 000015d0: 2020 205f 6265 6861 7669 6f72 5f76 6572     _behavior_ver
 000015e0: 7369 6f6e 203d 204e 6f6e 6520 2023 2074  sion = None  # t
 000015f0: 7970 653a 2074 7970 696e 672e 4f70 7469  ype: typing.Opti
 00001600: 6f6e 616c 5b69 6e74 5d0a 2020 2020 5f6d  onal[int].    _m
 00001610: 696e 5f62 6568 6176 696f 725f 7665 7273  in_behavior_vers
 00001620: 696f 6e20 3d20 3020 2023 2074 7970 653a  ion = 0  # type:
 00001630: 2069 6e74 0a0a 2020 2020 4063 6c61 7373   int..    @class
```

### Comparing `returnn-1.20230419.94650/returnn/util/better_exchook.py` & `returnn-1.20230420.214350/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/util/bpe.py` & `returnn-1.20230420.214350/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/util/debug.py` & `returnn-1.20230420.214350/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/util/debug_helpers.py` & `returnn-1.20230420.214350/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/util/fsa.py` & `returnn-1.20230420.214350/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230420.214350/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/util/pprint.py` & `returnn-1.20230420.214350/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/util/py-to-pickle.cpp` & `returnn-1.20230420.214350/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/util/sig_proc.py` & `returnn-1.20230420.214350/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn/util/task_system.py` & `returnn-1.20230420.214350/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/returnn.egg-info/PKG-INFO` & `returnn-1.20230420.214350/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230419.94650
+Version: 1.20230420.214350
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230419.94650/returnn.egg-info/SOURCES.txt` & `returnn-1.20230420.214350/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/setup.py` & `returnn-1.20230420.214350/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/DummySprintExec.py` & `returnn-1.20230420.214350/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230420.214350/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230420.214350/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230420.214350/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/_set_num_threads1.py` & `returnn-1.20230420.214350/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/_setup_test_env.py` & `returnn-1.20230420.214350/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/bpe-unicode-demo.codes` & `returnn-1.20230420.214350/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/bpe-unicode-demo.vocab` & `returnn-1.20230420.214350/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/lexicon_opt.isyms` & `returnn-1.20230420.214350/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/lexicon_opt.jpg` & `returnn-1.20230420.214350/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/lint_common.py` & `returnn-1.20230420.214350/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/pycharm-inspect.py` & `returnn-1.20230420.214350/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/pylint.py` & `returnn-1.20230420.214350/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/returnn-as-framework.py` & `returnn-1.20230420.214350/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/rf_utils.py` & `returnn-1.20230420.214350/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/spelling.dic` & `returnn-1.20230420.214350/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_Config.py` & `returnn-1.20230420.214350/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_Dataset.py` & `returnn-1.20230420.214350/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_Fsa.py` & `returnn-1.20230420.214350/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_GeneratingDataset.py` & `returnn-1.20230420.214350/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_HDFDataset.py` & `returnn-1.20230420.214350/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_LearningRateControl.py` & `returnn-1.20230420.214350/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_Log.py` & `returnn-1.20230420.214350/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_MultiProcDataset.py` & `returnn-1.20230420.214350/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_PTDataset.py` & `returnn-1.20230420.214350/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_Pretrain.py` & `returnn-1.20230420.214350/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_ResNet.py` & `returnn-1.20230420.214350/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_SprintDataset.py` & `returnn-1.20230420.214350/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_SprintInterface.py` & `returnn-1.20230420.214350/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_TFEngine.py` & `returnn-1.20230420.214350/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_TFNativeOp.py` & `returnn-1.20230420.214350/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_TFNetworkLayer.py` & `returnn-1.20230420.214350/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230420.214350/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230420.214350/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_TFUpdater.py` & `returnn-1.20230420.214350/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_TFUtil.py` & `returnn-1.20230420.214350/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_TF_determinism.py` & `returnn-1.20230420.214350/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_TaskSystem.py` & `returnn-1.20230420.214350/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230420.214350/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_TranslationDataset.py` & `returnn-1.20230420.214350/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_Util.py` & `returnn-1.20230420.214350/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_demos.py` & `returnn-1.20230420.214350/tests/test_demos.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,25 +152,25 @@
 @unittest.skipIf(not torch, "no PyTorch")
 def test_demo_rf_torch_task12ax():
     cleanup_tmp_models("demos/demo-rf.config")
     out = run(py, "rnn.py", "demos/demo-rf.config", print_stdout=True)
     # Currently this just uses linear layers, so it's not very good.
     # Also see test_demo_tf_task12ax above.
     fer = parse_last_fer(out)
-    assert_less(fer, 0.15)
+    assert_less(fer, 0.02)
 
 
 @unittest.skipIf(not tf, "no TF")
 def test_demo_rf_tf_task12ax():
     cleanup_tmp_models("demos/demo-rf.config")
     out = run(py, "rnn.py", "demos/demo-rf.config", "++backend", "tensorflow-net-dict", print_stdout=True)
     # Currently this just uses linear layers, so it's not very good.
     # Also see test_demo_tf_task12ax above.
     fer = parse_last_fer(out)
-    assert_less(fer, 0.15)
+    assert_less(fer, 0.02)
 
 
 def test_demo_iter_dataset_task12ax():
     # there should be no actual TF dependency, we just iterate the dataset
     cleanup_tmp_models("demos/demo-tf-vanilla-lstm.12ax.config")
     # pick any 12ax config for the dataset test
     out = run(py, "demos/demo-iter-dataset.py", "demos/demo-tf-vanilla-lstm.12ax.config")
```

### Comparing `returnn-1.20230419.94650/tests/test_fork_exec.py` & `returnn-1.20230420.214350/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_hdf_dump.py` & `returnn-1.20230420.214350/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_rf_array.py` & `returnn-1.20230420.214350/tests/test_rf_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from typing import Tuple
 import _setup_test_env  # noqa
 import returnn.frontend as rf
 from returnn.tensor import Tensor, Dim, TensorDict, batch_dim
 from rf_utils import run_model
 
 
-def test_pack():
+def test_pack_padded():
     time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
     in_dim = Dim(7, name="in")
     extern_data = TensorDict(
         {
             "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
         }
     )
 
     class _Net(rf.Module):
         def __call__(self, x: Tensor) -> Tuple[Tensor, Dim]:
-            pack, pack_dim = rf.pack(x, dims=[batch_dim, time_dim], enforce_sorted=False)
+            pack, pack_dim = rf.pack_padded(x, dims=[batch_dim, time_dim], enforce_sorted=False)
             return pack, pack_dim
 
     # noinspection PyShadowingNames
     def _forward_step(*, model: _Net, extern_data: TensorDict):
         out, pack_dim = model(extern_data["data"])
         out.mark_as_default_output(shape=(pack_dim, in_dim))
```

### Comparing `returnn-1.20230419.94650/tests/test_rf_attention.py` & `returnn-1.20230420.214350/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_rf_base.py` & `returnn-1.20230420.214350/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_rf_container.py` & `returnn-1.20230420.214350/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_rf_conv.py` & `returnn-1.20230420.214350/tests/test_rf_conv.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,14 +33,40 @@
     def _forward_step(*, model: _Net, extern_data: TensorDict):
         out, dim = model(extern_data["data"])
         out.mark_as_default_output(shape=(batch_dim, dim, out_dim))
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
 
 
+def test_conv1d_same_out():
+    time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
+    in_dim = Dim(7, name="in")
+    extern_data = TensorDict(
+        {
+            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
+        }
+    )
+
+    class _Net(rf.Module):
+        def __init__(self):
+            super().__init__()
+            self.conv = rf.Conv1d(in_dim, in_dim, 4, padding="same")
+
+        def __call__(self, x: rf.Tensor) -> Tensor:
+            x, _ = self.conv(x, in_spatial_dim=time_dim)
+            return x
+
+    # noinspection PyShadowingNames
+    def _forward_step(*, model: _Net, extern_data: TensorDict):
+        out = model(extern_data["data"])
+        out.mark_as_default_output(shape=(batch_dim, time_dim, in_dim))
+
+    run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
+
+
 def test_conv1d_depthwise():
     time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
     in_dim = Dim(7, name="in")
     out_dim = Dim(7 * 3, name="out")
     extern_data = TensorDict(
         {
             "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
```

### Comparing `returnn-1.20230419.94650/tests/test_rf_encoder_conformer.py` & `returnn-1.20230420.214350/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_rf_math.py` & `returnn-1.20230420.214350/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_rf_normalization.py` & `returnn-1.20230420.214350/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_rf_rec.py` & `returnn-1.20230420.214350/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_tensor.py` & `returnn-1.20230420.214350/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_tools.py` & `returnn-1.20230420.214350/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tests/test_torch_internal_frontend.py` & `returnn-1.20230420.214350/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/analyze-dataset-batches.py` & `returnn-1.20230420.214350/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/bliss-collect-seq-lens.py` & `returnn-1.20230420.214350/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/bliss-dump-text.py` & `returnn-1.20230420.214350/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/bliss-get-segment-names.py` & `returnn-1.20230420.214350/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/bliss-to-ogg-zip.py` & `returnn-1.20230420.214350/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/bpe-create-lexicon.py` & `returnn-1.20230420.214350/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/calculate-word-error-rate.py` & `returnn-1.20230420.214350/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/cleanup-old-models.py` & `returnn-1.20230420.214350/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/collect-orth-symbols.py` & `returnn-1.20230420.214350/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/collect-words.py` & `returnn-1.20230420.214350/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/compile_native_op.py` & `returnn-1.20230420.214350/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/compile_tf_graph.py` & `returnn-1.20230420.214350/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/debug-dump-search-scores.py` & `returnn-1.20230420.214350/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/debug-plot-search-scores.py` & `returnn-1.20230420.214350/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/dump-dataset-raw-strings.py` & `returnn-1.20230420.214350/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/dump-dataset.py` & `returnn-1.20230420.214350/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/dump-forward-stats.py` & `returnn-1.20230420.214350/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/dump-forward.py` & `returnn-1.20230420.214350/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/dump-network-json.py` & `returnn-1.20230420.214350/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/dump-pickle.py` & `returnn-1.20230420.214350/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230420.214350/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/get-attention-weights.py` & `returnn-1.20230420.214350/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/get-best-model-epoch.py` & `returnn-1.20230420.214350/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/hdf_dump.py` & `returnn-1.20230420.214350/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230420.214350/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/import-blocks-mt-model.py` & `returnn-1.20230420.214350/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/import-t2t-mt-model.py` & `returnn-1.20230420.214350/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/lattice_rescorer/Makefile` & `returnn-1.20230420.214350/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/lattice_rescorer/README.md` & `returnn-1.20230420.214350/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/lattice_rescorer/example/README.md` & `returnn-1.20230420.214350/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230420.214350/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230420.214350/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230420.214350/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/lattice_rescorer/file.h` & `returnn-1.20230420.214350/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230420.214350/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230420.214350/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/lattice_rescorer/main.cc` & `returnn-1.20230420.214350/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230420.214350/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230420.214350/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230420.214350/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/tf_avg_checkpoints.py` & `returnn-1.20230420.214350/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/tf_inspect_checkpoint.py` & `returnn-1.20230420.214350/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230419.94650/tools/tf_inspect_summary_log.py` & `returnn-1.20230420.214350/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

