# Comparing `tmp/e2eAIOK-1.0.1b2023042000.tar.gz` & `tmp/e2eAIOK-1.0.1b2023042100.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/e2eAIOK-1.0.1b2023042000.tar", last modified: Thu Apr 20 00:02:48 2023, max compression
+gzip compressed data, was "dist/e2eAIOK-1.0.1b2023042100.tar", last modified: Fri Apr 21 00:02:47 2023, max compression
```

## Comparing `e2eAIOK-1.0.1b2023042000.tar` & `e2eAIOK-1.0.1b2023042100.tar`

### file list

```diff
@@ -1,280 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/
--rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/TransformerBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/TransformerLM.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/asr_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/asr_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/augment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/dataio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/dataio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/dataio/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/dataio/dataio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/dataio/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/dataio/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/dataio/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/dataio/wer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/librispeech_prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30974 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/processing/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/processing/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/processing/speech_augmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/decoders/ctc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/decoders/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/init_asr_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/lib/CNN.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/lib/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/lib/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/model_builder_denas_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/supernet_asr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/trainer/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/trainer/schedulers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/Accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/asr_nas.py
--rw-r--r--   0 runner    (1001) docker     (123)    37493 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/edit_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/metric_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/parameter_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/DeNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/benchmark_network_latency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/cv_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/model_builder_denas_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/supernet_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResIDWEXKX.py
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResK1KXK1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResKXKX.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55629 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/basic_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/global_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/net_struct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/super_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/ZenNet.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/utils/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/utils/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/Linear_base.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/asr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/asr/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/asr/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/asr/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/asr/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/asr/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/asr/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/asr/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/attention_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/cv/
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/cv/Linear_super.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/cv/embedding_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/cv/layernorm_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/cv/multihead_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/cv/qkv_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/cv/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/embedding_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/layernorm_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/Linear_super.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/bert_attention_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/bert_embedding_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/bert_encoder_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/bert_intermediate_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/bert_pooler_super.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/layernorm_super.py
--rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    16607 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/nlp/bert_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/nlp/model_builder_denas_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19589 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/nlp/supernet_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/nlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/nlp/utils_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/scores/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/scores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/scores/basic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/scores/compute_de_score.py
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/scores/transformer_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/BaseSearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/EvolutionarySearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/MOSigoptSearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/RandomSearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/SearchEngineFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    20453 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/SigoptSearchEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/thirdparty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/thirdparty/supernet_hf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/thirdparty/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/backbone/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/backbone/unet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/backbone/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/dataset/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/dataset/composed_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/dataset/office31.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/default_ma.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/finetunner/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/finetunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/training/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/training/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/training/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/SDA.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/BERTAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/BaseModelAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/DIENAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/DLRMAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/MiniGoAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/RNNTAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/RegisteredAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/ResNetAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/TestAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/TwitterRecSysAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/UPMAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/WnDAdvisor.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/default.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/asr/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/cv/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/data_builder_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/data_builder_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/data_builder_nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/data_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/data_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/data_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/data_utils/image_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/data_utils/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/cv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/cv/lenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/cv/resnet_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/model_builder_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/model_builder_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/model_builder_nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/model_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/model_utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/torch_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/utils/extend_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/dataloader/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/dataloader/hydrodataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/hydroDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/hydroautolearner.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/hydroconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/hydroconnector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/hydromodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/hydromodelzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/hydroserver.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 00:02:40.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/hydroweblistener.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 00:02:47.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/e2eAIOK.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 00:02:48.000000 e2eAIOK-1.0.1b2023042000/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-20 00:02:41.000000 e2eAIOK-1.0.1b2023042000/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/TransformerBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/TransformerLM.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/asr_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/asr_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/augment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/dataio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/dataio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/dataio/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/dataio/dataio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/dataio/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/dataio/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/dataio/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/dataio/wer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/librispeech_prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30974 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/processing/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/processing/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/processing/speech_augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/decoders/ctc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/decoders/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/init_asr_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/lib/CNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/lib/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/lib/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/model_builder_denas_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/supernet_asr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/trainer/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/trainer/schedulers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/Accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/asr_nas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37493 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/metric_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/parameter_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/DeNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/benchmark_network_latency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/cv_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/model_builder_denas_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/supernet_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResIDWEXKX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResK1KXK1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResKXKX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55629 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/basic_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/global_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/net_struct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/super_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/ZenNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/utils/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/utils/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/Linear_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/asr/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/asr/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/asr/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/asr/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/asr/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/asr/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/asr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/attention_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/cv/Linear_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/cv/embedding_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/cv/layernorm_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/cv/multihead_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/cv/qkv_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/cv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/embedding_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/layernorm_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/Linear_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/bert_attention_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/bert_embedding_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/bert_encoder_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/bert_intermediate_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/bert_pooler_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/layernorm_super.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16607 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/nlp/bert_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/nlp/model_builder_denas_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19589 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/nlp/supernet_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/nlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/nlp/utils_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/scores/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/scores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/scores/basic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/scores/compute_de_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/scores/transformer_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/BaseSearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/EvolutionarySearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/MOSigoptSearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/RandomSearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/SearchEngineFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20453 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/SigoptSearchEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/thirdparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/thirdparty/supernet_hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/thirdparty/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/backbone/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/backbone/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/backbone/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/dataset/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/dataset/composed_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/dataset/office31.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/default_ma.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/finetunner/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/finetunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/training/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/training/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/training/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/SDA.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/BERTAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/BaseModelAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/DIENAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/DLRMAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/MiniGoAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16404 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/RNNTAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/RegisteredAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/ResNetAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/TestAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/TwitterRecSysAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/UPMAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/WnDAdvisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/default.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/data_builder_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/data_builder_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/data_builder_nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/data_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/data_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/data_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/data_utils/image_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/data_utils/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/cv/lenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/cv/resnet_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/model_builder_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/model_builder_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/model_builder_nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/model_utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/torch_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/utils/extend_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/dataloader/hydrodataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/hydroDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/hydroautolearner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/hydroconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/hydroconnector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/hydromodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/hydromodelzoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/hydroserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/hydroweblistener.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 00:02:45.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/e2eAIOK.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 00:02:47.000000 e2eAIOK-1.0.1b2023042100/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-21 00:02:38.000000 e2eAIOK-1.0.1b2023042100/setup.py
```

### Comparing `e2eAIOK-1.0.1b2023042000/PKG-INFO` & `e2eAIOK-1.0.1b2023042100/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2eAIOK
-Version: 1.0.1b2023042000
+Version: 1.0.1b2023042100
 Summary: Intel® End-to-End AI Optimization Kit
 Home-page: https://github.com/intel/e2eAIOK
 Author: INTEL
 License: Apache License
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/issues
 Description: # [Intel® End-to-End AI Optimization Kit](https://github.com/intel/e2eAIOK)
         
@@ -101,14 +101,21 @@
                * [Finetuner](demo/ma/finetuner/Model_Adapter_Finetuner_Walkthrough_ResNet50_CIFAR100.ipynb) - Computer Vision, Image Classification, ResNet50, PyTorch
                * [Distiller](demo/ma/distiller/Model_Adapter_Distiller_Walkthrough_VIT_to_ResNet18_CIFAR100.ipynb) - Computer Vision, Image Classification, ResNet18, PyTorch
                * [Domain Adapter](demo/ma/domain_adapter/Model_Adapter_Domain_Adapter_Walkthrough_Unet_KITS19.ipynb) - Computer Vision, Medical Segmentation, 3D Unet, PyTorch
         
         ## Performance
         
         Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
+        For [DeNAS](e2eAIOK/DeNas/README.md) CNN and ViT, Intel® End-to-End AI Optimization Kit delivered 40.73x and 35.63x search time speedup, 82.57x and 4.44x training time speedup over [ZenNAS](https://github.com/idstcv/ZenNAS) and [AutoFormer](https://github.com/microsoft/Cream/tree/main/AutoFormer) respectively. For DeNAS searched CNN, ViT, BERT and ASR model, Intel® End-to-End AI Optimization Kit delivered 9.86x, 4.44x, 7.68x and 59.12x training time speedup with 0.03x, 1.20x, 0.62x and 0.81x model size respectively. Please refer to DeNAS link for detailed test dataset and test method.
+        > Noted: Optimized lighter models' accuracy are slightly lower: CNN -3% accuracy, ViT -5% accuracy, BERT -4% F1 score.
+        
+        ![Performance](./docs/source/e2eaiok_v10_performance_nas.png "Intel® End-to-End AI Optimization Kit Performance")
+        ![Performance](./docs/source/e2eaiok_v10_performance_stock.png "Intel® End-to-End AI Optimization Kit Performance")
+        
+        Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
         For [MiniGO](modelzoo/minigo/README.md), [BERT](modelzoo/bert/README.md), [ResNet](modelzoo/resnet/README.md), [RNN-T](modelzoo/rnnt/README.md), Intel® End-to-End AI Optimization Kit delivered 13.06x, 10.10x, 8.77x and 14.19x training time speedup respecitvely through E2E optimizations. Please refer to corresponding model link for detailed test dataset and test method. 
         > Noted: Optimized lighter models' accuracy are slightly lower: ResNet -5% accuracy, BERT -1% F1 score.
         
         ![Performance](./docs/source/e2eaiok_v02_performance.png "Intel® End-to-End AI Optimization Kit Performance")
         
         Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
         For [WnD](modelzoo/WnD/README.md), [DIEN](modelzoo/dien/README.md) and [DLRM](modelzoo/dlrm/README.md), Intel® End-to-End AI Optimization Kit delivered 51.01x(5.02x ELT & 113.03x training), 12.67x(14.86x ELT & 11.91x training) and 71.16x(86.40x ELT & 42.31x training) E2E time speedup, 21.18x, 14.11x and 124.98x inference throughput speedup respectively. Please refer to corresponding model link for detailed test dataset and test method.
```

### Comparing `e2eAIOK-1.0.1b2023042000/README.md` & `e2eAIOK-1.0.1b2023042100/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -93,14 +93,21 @@
        * [Finetuner](demo/ma/finetuner/Model_Adapter_Finetuner_Walkthrough_ResNet50_CIFAR100.ipynb) - Computer Vision, Image Classification, ResNet50, PyTorch
        * [Distiller](demo/ma/distiller/Model_Adapter_Distiller_Walkthrough_VIT_to_ResNet18_CIFAR100.ipynb) - Computer Vision, Image Classification, ResNet18, PyTorch
        * [Domain Adapter](demo/ma/domain_adapter/Model_Adapter_Domain_Adapter_Walkthrough_Unet_KITS19.ipynb) - Computer Vision, Medical Segmentation, 3D Unet, PyTorch
 
 ## Performance
 
 Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
+For [DeNAS](e2eAIOK/DeNas/README.md) CNN and ViT, Intel® End-to-End AI Optimization Kit delivered 40.73x and 35.63x search time speedup, 82.57x and 4.44x training time speedup over [ZenNAS](https://github.com/idstcv/ZenNAS) and [AutoFormer](https://github.com/microsoft/Cream/tree/main/AutoFormer) respectively. For DeNAS searched CNN, ViT, BERT and ASR model, Intel® End-to-End AI Optimization Kit delivered 9.86x, 4.44x, 7.68x and 59.12x training time speedup with 0.03x, 1.20x, 0.62x and 0.81x model size respectively. Please refer to DeNAS link for detailed test dataset and test method.
+> Noted: Optimized lighter models' accuracy are slightly lower: CNN -3% accuracy, ViT -5% accuracy, BERT -4% F1 score.
+
+![Performance](./docs/source/e2eaiok_v10_performance_nas.png "Intel® End-to-End AI Optimization Kit Performance")
+![Performance](./docs/source/e2eaiok_v10_performance_stock.png "Intel® End-to-End AI Optimization Kit Performance")
+
+Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
 For [MiniGO](modelzoo/minigo/README.md), [BERT](modelzoo/bert/README.md), [ResNet](modelzoo/resnet/README.md), [RNN-T](modelzoo/rnnt/README.md), Intel® End-to-End AI Optimization Kit delivered 13.06x, 10.10x, 8.77x and 14.19x training time speedup respecitvely through E2E optimizations. Please refer to corresponding model link for detailed test dataset and test method. 
 > Noted: Optimized lighter models' accuracy are slightly lower: ResNet -5% accuracy, BERT -1% F1 score.
 
 ![Performance](./docs/source/e2eaiok_v02_performance.png "Intel® End-to-End AI Optimization Kit Performance")
 
 Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
 For [WnD](modelzoo/WnD/README.md), [DIEN](modelzoo/dien/README.md) and [DLRM](modelzoo/dlrm/README.md), Intel® End-to-End AI Optimization Kit delivered 51.01x(5.02x ELT & 113.03x training), 12.67x(14.86x ELT & 11.91x training) and 71.16x(86.40x ELT & 42.31x training) E2E time speedup, 21.18x, 14.11x and 124.98x inference throughput speedup respectively. Please refer to corresponding model link for detailed test dataset and test method.
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/TransformerBase.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/TransformerBase.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/TransformerLM.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/TransformerLM.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/asr_model_builder.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/asr_model_builder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/asr_trainer.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/asr_trainer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/augment.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/augment.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/dataio/batch.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/dataio/batch.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/dataio/dataio.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/dataio/dataio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import torch
 import logging
 import numpy as np
-import pickle
+import pickle #nosec
 import csv
 import time
 import torchaudio
 import json
 import re
 logger = logging.getLogger(__name__)
 
@@ -212,15 +212,15 @@
         else:
             break
 
     try:
         with open(file + ".lock", "w"):
             pass
         with open(file, "rb") as f:
-            return pickle.load(f)
+            return pickle.load(f) #nosec
     finally:
         if os.path.isfile(file + ".lock"):
             os.remove(file + ".lock")
 
 
 def merge_char(sequences, space="_"):
     """Merge characters sequences into word sequences.
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/dataio/dataloader.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/dataio/dataloader.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/dataio/dataset.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/dataio/dataset.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/dataio/sampler.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/dataio/sampler.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/dataio/wer.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/dataio/wer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/features.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/features.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/librispeech_prepare.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/librispeech_prepare.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/processing/features.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/processing/features.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/processing/signal_processing.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/processing/signal_processing.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/data/processing/speech_augmentation.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/data/processing/speech_augmentation.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/decoders/ctc.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/decoders/ctc.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/decoders/seq2seq.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/decoders/seq2seq.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/init_asr_parser.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/init_asr_parser.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/lib/CNN.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/lib/CNN.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/lib/containers.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/lib/containers.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/lib/convolution.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/lib/convolution.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/model_builder_denas_asr.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/model_builder_denas_asr.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/supernet_asr.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/supernet_asr.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/trainer/losses.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/trainer/losses.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/trainer/schedulers.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/trainer/schedulers.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/Accuracy.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/Accuracy.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/asr_nas.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/asr_nas.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,55 +28,55 @@
         return False, info['params'] < params.min_param_limits
     info['visited'] = True
     return True, super_net
 
 def asr_populate_random_func(search_space):
     cand_tuple = list()
     dimensions = ['mlp_ratio', 'num_heads']
-    depth = random.choice(search_space['depth'])
+    depth = random.choice(search_space['depth']) #nosec
     cand_tuple.append(depth)
     for dimension in dimensions:
         for i in range(depth):
-            cand_tuple.append(random.choice(search_space[dimension]))
-    cand_tuple.append(random.choice(search_space['embed_dim']))
+            cand_tuple.append(random.choice(search_space[dimension])) #nosec
+    cand_tuple.append(random.choice(search_space['embed_dim'])) #nosec
     return tuple(cand_tuple)
 
 def asr_mutation_random_func(m_prob, s_prob, search_space, top_candidates):
-    cand = list(random.choice(top_candidates))
+    cand = list(random.choice(top_candidates)) #nosec
     depth, mlp_ratio, num_heads, embed_dim = asr_decode_cand_tuple(cand)
-    random_s = random.random()
+    random_s = random.random() #nosec
     # depth
     if random_s < s_prob:
-        new_depth = random.choice(search_space['depth'])
+        new_depth = random.choice(search_space['depth']) #nosec
         if new_depth > depth:
-            mlp_ratio = mlp_ratio + [random.choice(search_space['mlp_ratio']) for _ in range(new_depth - depth)]
-            num_heads = num_heads + [random.choice(search_space['num_heads']) for _ in range(new_depth - depth)]
+            mlp_ratio = mlp_ratio + [random.choice(search_space['mlp_ratio']) for _ in range(new_depth - depth)] #nosec
+            num_heads = num_heads + [random.choice(search_space['num_heads']) for _ in range(new_depth - depth)] #nosec
         else:
             mlp_ratio = mlp_ratio[:new_depth]
             num_heads = num_heads[:new_depth]
         depth = new_depth
     # mlp_ratio
     for i in range(depth):
-        random_s = random.random()
+        random_s = random.random() #nosec
         if random_s < m_prob:
-            mlp_ratio[i] = random.choice(search_space['mlp_ratio'])
+            mlp_ratio[i] = random.choice(search_space['mlp_ratio']) #nosec
     # num_heads
     for i in range(depth):
-        random_s = random.random()
+        random_s = random.random() #nosec
         if random_s < m_prob:
-            num_heads[i] = random.choice(search_space['num_heads'])
+            num_heads[i] = random.choice(search_space['num_heads']) #nosec
     # embed_dim
-    random_s = random.random()
+    random_s = random.random() #nosec
     if random_s < s_prob:
-        embed_dim = random.choice(search_space['embed_dim'])
+        embed_dim = random.choice(search_space['embed_dim']) #nosec
     result_cand = [depth] + mlp_ratio + num_heads + [embed_dim]
     return tuple(result_cand)
 
 def asr_crossover_random_func(top_candidates):
-    p1 = random.choice(top_candidates)
-    p2 = random.choice(top_candidates)
+    p1 = random.choice(top_candidates) #nosec
+    p2 = random.choice(top_candidates) #nosec
     max_iters_tmp = 50
     while len(p1) != len(p2) and max_iters_tmp > 0:
         max_iters_tmp -= 1
-        p1 = random.choice(top_candidates)
-        p2 = random.choice(top_candidates)
-    return tuple(random.choice([i, j]) for i, j in zip(p1, p2))
+        p1 = random.choice(top_candidates) #nosec
+        p2 = random.choice(top_candidates) #nosec
+    return tuple(random.choice([i, j]) for i, j in zip(p1, p2)) #nosec
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/checkpoints.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/checkpoints.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/data_pipeline.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/data_utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,17 +174,15 @@
                 print(f"Downloading {source} to {dest}")
                 with DownloadProgressBar(
                     unit="B",
                     unit_scale=True,
                     miniters=1,
                     desc=source.split("/")[-1],
                 ) as t:
-                    urllib.request.urlretrieve(
-                        source, filename=dest, reporthook=t.update_to
-                    )
+                    urllib.request.urlretrieve(source, filename=dest, reporthook=t.update_to) #nosec
             else:
                 print(f"{dest} exists. Skipping download")
 
             # Unpack if necessary
             if unpack:
                 if dest_unpack is None:
                     dest_unpack = os.path.dirname(dest)
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/depgraph.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/depgraph.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/distributed.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/edit_distance.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/edit_distance.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/metric_stats.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/metric_stats.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/parameter_transfer.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/parameter_transfer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/asr/utils/utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/asr/utils/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/benchmark_network_latency.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/benchmark_network_latency.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/cv_trainer.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/cv_trainer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/model_builder_denas_cv.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/model_builder_denas_cv.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,10 +31,10 @@
             depth, mlp_ratio, num_heads, embed_dim = decode_arch_tuple(arch)
             model_config = {}
             model_config['layer_num'] = depth
             model_config['mlp_ratio'] = mlp_ratio
             model_config['num_heads'] = num_heads
             model_config['embed_dim'] = [embed_dim]*depth
             n_parameters = model.get_sampled_params_numel(model_config)
-            print("model parameters size: {}".format(n_parameters))
+            print(f"model parameters size: {n_parameters}")
         return model
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/supernet_transformer.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/supernet_transformer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResIDWEXKX.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResIDWEXKX.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResK1KXK1.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResK1KXK1.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResKXKX.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/SuperResKXKX.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/__init__.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/__init__.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/basic_blocks.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/global_utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/global_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/net_struct_utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/net_struct_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/PlainNet/super_blocks.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/PlainNet/super_blocks.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/third_party/ZenNet.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/third_party/ZenNet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/utils/cnn.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/utils/cnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,35 +40,35 @@
     random_structure_str = get_new_random_structure_str(super_net, search_space, num_classes, structure_str=str(super_net(num_classes=num_classes, plainnet_struct = plainnet_struct, no_create=True, no_reslink=no_reslink, no_BN=no_BN, use_se=use_se)), num_replaces=1)
     return get_splitted_structure_str(super_net, num_classes, random_structure_str)
 
 def cnn_mutation_random_func(top_candidates, super_net, search_space, num_classes, plainnet_struct):
     if len(top_candidates) <= 10:
         tmp_random_structure_str = plainnet_struct
     else:
-        tmp_idx = random.choice(range(0, len(top_candidates) - 1))
+        tmp_idx = random.choice(range(0, len(top_candidates) - 1)) #nosec
         tmp_random_structure_str = top_candidates[tmp_idx]
 
     random_structure_str = get_new_random_structure_str(super_net, search_space, num_classes, structure_str=tmp_random_structure_str, num_replaces=2)
     return get_splitted_structure_str(super_net, num_classes, random_structure_str)
 
 def cnn_crossover_random_func(super_net, search_space, num_classes, plainnet_struct, no_reslink, no_BN, use_se):
     random_structure_str = get_new_random_structure_str(super_net, search_space, num_classes, structure_str=str(super_net(num_classes=num_classes, plainnet_struct = plainnet_struct, no_create=True, no_reslink=no_reslink, no_BN=no_BN, use_se=use_se)), num_replaces=1)
     return get_splitted_structure_str(super_net, num_classes, random_structure_str)
 
 def get_new_random_structure_str(super_net, search_space, num_classes, structure_str, num_replaces=1):
     the_net = super_net(num_classes, plainnet_struct=structure_str, no_create=True)
     selected_random_id_set = set()
     for replace_count in range(num_replaces):
-        random_id = random.choice(range(0, len(the_net.block_list) - 1))
+        random_id = random.choice(range(0, len(the_net.block_list) - 1)) #nosec
         if random_id in selected_random_id_set:
             continue
         selected_random_id_set.add(random_id)
         to_search_student_blocks_list_list = search_space.gen_search_space(the_net.block_list, random_id)
         to_search_student_blocks_list = [x for sublist in to_search_student_blocks_list_list for x in sublist]
-        new_student_block_str = random.choice(to_search_student_blocks_list)
+        new_student_block_str = random.choice(to_search_student_blocks_list) #nosec
         if len(new_student_block_str) > 0:
             new_student_block = super_net.create_netblock_list_from_str(new_student_block_str, no_create=True)
             assert len(new_student_block) == 1
             new_student_block = new_student_block[0]
             if random_id > 0:
                 last_block_out_channels = the_net.block_list[random_id - 1].out_channels
                 new_student_block.set_in_channels(last_block_out_channels)
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/cv/utils/vit.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/cv/utils/vit.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,55 +24,55 @@
         return False
     info['visited'] = True
     return True
 
 def vit_populate_random_func(search_space):
     cand_tuple = list()
     dimensions = ['mlp_ratio', 'num_heads']
-    depth = random.choice(search_space['depth'])
+    depth = random.choice(search_space['depth']) #nosec
     cand_tuple.append(depth)
     for dimension in dimensions:
         for i in range(depth):
-            cand_tuple.append(random.choice(search_space[dimension]))
-    cand_tuple.append(random.choice(search_space['embed_dim']))
+            cand_tuple.append(random.choice(search_space[dimension])) #nosec
+    cand_tuple.append(random.choice(search_space['embed_dim'])) #nosec
     return tuple(cand_tuple)
 
 def vit_mutation_random_func(m_prob, s_prob, search_space, top_candidates):
-    cand = list(random.choice(top_candidates))
+    cand = list(random.choice(top_candidates)) #nosec
     depth, mlp_ratio, num_heads, embed_dim = vit_decode_cand_tuple(cand)
-    random_s = random.random()
+    random_s = random.random() #nosec
     # depth
     if random_s < s_prob:
-        new_depth = random.choice(search_space['depth'])
+        new_depth = random.choice(search_space['depth']) #nosec
         if new_depth > depth:
-            mlp_ratio = mlp_ratio + [random.choice(search_space['mlp_ratio']) for _ in range(new_depth - depth)]
-            num_heads = num_heads + [random.choice(search_space['num_heads']) for _ in range(new_depth - depth)]
+            mlp_ratio = mlp_ratio + [random.choice(search_space['mlp_ratio']) for _ in range(new_depth - depth)] #nosec
+            num_heads = num_heads + [random.choice(search_space['num_heads']) for _ in range(new_depth - depth)] #nosec
         else:
             mlp_ratio = mlp_ratio[:new_depth]
             num_heads = num_heads[:new_depth]
         depth = new_depth
     # mlp_ratio
     for i in range(depth):
-        random_s = random.random()
+        random_s = random.random() #nosec
         if random_s < m_prob:
-            mlp_ratio[i] = random.choice(search_space['mlp_ratio'])
+            mlp_ratio[i] = random.choice(search_space['mlp_ratio']) #nosec
     # num_heads
     for i in range(depth):
-        random_s = random.random()
+        random_s = random.random() #nosec
         if random_s < m_prob:
-            num_heads[i] = random.choice(search_space['num_heads'])
+            num_heads[i] = random.choice(search_space['num_heads']) #nosec
     # embed_dim
-    random_s = random.random()
+    random_s = random.random() #nosec
     if random_s < s_prob:
-        embed_dim = random.choice(search_space['embed_dim'])
+        embed_dim = random.choice(search_space['embed_dim']) #nosec
     result_cand = [depth] + mlp_ratio + num_heads + [embed_dim]
     return tuple(result_cand)
 
 def vit_crossover_random_func(top_candidates):
-    p1 = random.choice(top_candidates)
-    p2 = random.choice(top_candidates)
+    p1 = random.choice(top_candidates) #nosec
+    p2 = random.choice(top_candidates) #nosec
     max_iters_tmp = 50
     while len(p1) != len(p2) and max_iters_tmp > 0:
         max_iters_tmp -= 1
-        p1 = random.choice(top_candidates)
-        p2 = random.choice(top_candidates)
-    return tuple(random.choice([i, j]) for i, j in zip(p1, p2))
+        p1 = random.choice(top_candidates) #nosec
+        p2 = random.choice(top_candidates) #nosec
+    return tuple(random.choice([i, j]) for i, j in zip(p1, p2)) #nosec
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/asr/attention.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/asr/attention.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/asr/decoder.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/asr/decoder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/asr/encoder.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/asr/encoder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/asr/normalization.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/asr/normalization.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/asr/utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/asr/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/cv/Linear_super.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/cv/Linear_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/cv/embedding_super.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/cv/embedding_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/cv/layernorm_super.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/cv/layernorm_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/cv/multihead_super.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/cv/multihead_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/cv/qkv_super.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/cv/qkv_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/cv/utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/cv/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/Linear_super.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/Linear_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/bert_attention_super.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/bert_attention_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/bert_embedding_super.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/bert_embedding_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/bert_encoder_super.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/bert_encoder_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/bert_intermediate_super.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/bert_intermediate_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/bert_pooler_super.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/bert_pooler_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/layernorm_super.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/layernorm_super.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/optimization.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/optimization.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/module/nlp/tokenization.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/module/nlp/tokenization.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/nlp/bert_trainer.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/nlp/bert_trainer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/nlp/model_builder_denas_nlp.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/nlp/model_builder_denas_nlp.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/nlp/supernet_bert.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/nlp/supernet_bert.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/nlp/utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/nlp/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,26 +49,26 @@
             line = line.strip()
             subbert_config = get_subconfig(ast.literal_eval(line))
     return subbert_config
 
 def bert_populate_random_func(search_space):
     cand_tuple = list() #[layer_num, [num_attention_heads]*layer_num, [qkv_sizes]*layer_num, hidden_size, [intermediate_sizes]*layer_num]
     dimensions = ['head_num', 'hidden_size', 'ffn_size']
-    depth = random.choice(search_space['layer_num'])
+    depth = random.choice(search_space['layer_num']) #nosec
     cand_tuple.append(depth)
     for dimension in dimensions:
         if dimension == 'head_num':
-            head_num = random.choice(search_space[dimension])
+            head_num = random.choice(search_space[dimension]) #nosec
             qkv_size = head_num * 64
             cand_tuple.append(head_num)
             cand_tuple.append(qkv_size)
         elif dimension == 'hidden_size':
-            cand_tuple.append(random.choice(search_space['hidden_size']))
+            cand_tuple.append(random.choice(search_space['hidden_size'])) #nosec
         elif dimension == 'ffn_size':
-            cand_tuple.append(random.choice(search_space['ffn_size']))
+            cand_tuple.append(random.choice(search_space['ffn_size'])) #nosec
 
     return tuple(cand_tuple)
 
 def bert_is_legal(cand, vis_dict, params, super_net):
     if cand not in vis_dict:
         vis_dict[cand] = {}
     info = vis_dict[cand]
@@ -82,60 +82,60 @@
         return False
     if info['params'] < params.min_param_limits:
         return False
     info['visited'] = True
     return True
 
 def bert_mutation_random_func(m_prob, s_prob, search_space, top_candidates):
-    cand = list(random.choice(top_candidates))
+    cand = list(random.choice(top_candidates)) #nosec
     depth, num_heads, qkv_sizes, hidden_size, ffn_sizes = cand[0], cand[1], cand[2], cand[3], cand[4]
-    random_s = random.random()
+    random_s = random.random() #nosec
     # depth
     if random_s < s_prob:
-        new_depth = random.choice(search_space['layer_num'])
+        new_depth = random.choice(search_space['layer_num']) #nosec
         depth = new_depth
-        num_heads = random.choice(search_space['head_num'])
+        num_heads = random.choice(search_space['head_num']) #nosec
         qkv_sizes = num_heads * 64
-        hidden_size = random.choice(search_space['hidden_size'])
-        ffn_sizes = random.choice(search_space['ffn_size'])
-    random_s = random.random()
+        hidden_size = random.choice(search_space['hidden_size']) #nosec
+        ffn_sizes = random.choice(search_space['ffn_size']) #nosec
+    random_s = random.random() #nosec
     if random_s < m_prob:
         # num_heads
-        num_heads = random.choice(search_space['head_num'])
+        num_heads = random.choice(search_space['head_num']) #nosec
         # qkv_sizes
         qkv_sizes = num_heads * 64
     # hidden_size
-    random_s = random.random()
+    random_s = random.random() #nosec
     if random_s < s_prob:
-        hidden_size = random.choice(search_space['hidden_size'])
+        hidden_size = random.choice(search_space['hidden_size']) #nosec
     # ffn_sizes
-    random_s = random.random()
+    random_s = random.random() #nosec
     if random_s < s_prob:
-        ffn_sizes = random.choice(search_space['ffn_size'])
+        ffn_sizes = random.choice(search_space['ffn_size']) #nosec
 
     result_cand = [depth] + [num_heads] + [qkv_sizes] + [hidden_size] + [ffn_sizes]
     return tuple(result_cand)
 
 def bert_crossover_random_func(top_candidates):
-    p1 = random.choice(top_candidates)
-    p2 = random.choice(top_candidates)
+    p1 = random.choice(top_candidates) #nosec
+    p2 = random.choice(top_candidates) #nosec
     max_iters_tmp = 50
     while len(p1) != len(p2) and max_iters_tmp > 0:
         max_iters_tmp -= 1
-        p1 = random.choice(top_candidates)
-        p2 = random.choice(top_candidates)
+        p1 = random.choice(top_candidates) #nosec
+        p2 = random.choice(top_candidates) #nosec
     cand = []
     for ind, it in enumerate(zip(p1, p2)):
         if ind == 2:
             continue
         elif ind == 1:
-            cand.append(random.choice(it))
+            cand.append(random.choice(it)) #nosec
             cand.append(cand[-1] * 64)
         else:
-            cand.append(random.choice(it))
+            cand.append(random.choice(it)) #nosec
     return tuple(cand)
 
 def get_bert_latency(model, batch_size, max_seq_length, gpu, infer_cnt):
     if gpu is None:
         device = 'cpu'
     else:
         device = 'cuda'
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/nlp/utils_eval.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/nlp/utils_eval.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/scores/basic_utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/scores/basic_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/scores/compute_de_score.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/scores/compute_de_score.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/scores/transformer_proxy.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/scores/transformer_proxy.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/BaseSearchEngine.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/BaseSearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/EvolutionarySearchEngine.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/EvolutionarySearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/MOSigoptSearchEngine.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/MOSigoptSearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/RandomSearchEngine.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/RandomSearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/SearchEngineFactory.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/SearchEngineFactory.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/SigoptSearchEngine.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/SigoptSearchEngine.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search/utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/search.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/search.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/thirdparty/supernet_hf.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/thirdparty/supernet_hf.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/thirdparty/utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/thirdparty/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             line = line.strip()
             subhf_config = ast.literal_eval(line)
     return subhf_config
 
 def hf_populate_random_func(search_space):
     cand_tuple = dict()
     for search_key in search_space:
-        cand_tuple[search_key] = random.choice(search_space[search_key])
+        cand_tuple[search_key] = random.choice(search_space[search_key]) #nosec
 
     cand_tuple["hidden_size"] = int(cand_tuple["hidden_size"]/cand_tuple["num_attention_heads"]) * cand_tuple["num_attention_heads"]
 
     return json.dumps(cand_tuple)
 
 def hf_is_legal(cand, vis_dict, params):
     if cand not in vis_dict:
@@ -53,43 +53,43 @@
         return False
     if info['params'] < params.min_param_limits:
         return False
     info['visited'] = True
     return True
 
 def hf_mutation_random_func(m_prob, s_prob, search_space, top_candidates):
-    cand = random.choice(top_candidates)
-    random_s = random.random()
+    cand = random.choice(top_candidates) #nosec
+    random_s = random.random() #nosec
     result_cand = json.loads(cand)
     
     if random_s < m_prob:
         # num_heads
-        result_cand['num_attention_heads'] = random.choice(search_space['num_attention_heads'])
+        result_cand['num_attention_heads'] = random.choice(search_space['num_attention_heads']) #nosec
     for search_key in search_space:
         if search_key == 'num_attention_heads':
             continue
-        random_s = random.random()
+        random_s = random.random() #nosec
         if random_s < s_prob:
-            result_cand[search_key] = random.choice(search_space[search_key])
+            result_cand[search_key] = random.choice(search_space[search_key]) #nosec
 
     result_cand["hidden_size"] = int(result_cand["hidden_size"]/result_cand["num_attention_heads"]) * result_cand["num_attention_heads"]
 
     return json.dumps(result_cand)
 
 def hf_crossover_random_func(top_candidates):
-    p1 = json.loads(random.choice(top_candidates))
-    p2 = json.loads(random.choice(top_candidates))
+    p1 = json.loads(random.choice(top_candidates)) #nosec
+    p2 = json.loads(random.choice(top_candidates)) #nosec
     max_iters_tmp = 50
     while len(p1) != len(p2) and max_iters_tmp > 0:
         max_iters_tmp -= 1
-        p1 = json.loads(random.choice(top_candidates))
-        p2 = json.loads(random.choice(top_candidates))
+        p1 = json.loads(random.choice(top_candidates)) #nosec
+        p2 = json.loads(random.choice(top_candidates)) #nosec
     cand = {}
     for it1, it2 in zip(p1, p2):
-        select_item = random.choice([p1[it1], p2[it2]])
+        select_item = random.choice([p1[it1], p2[it2]]) #nosec
         cand[it1] = select_item
     cand["hidden_size"] = int(cand["hidden_size"]/cand["num_attention_heads"]) * cand["num_attention_heads"]
     return json.dumps(cand)
 
 def get_hf_latency(model, batch_size, max_seq_length, gpu, infer_cnt):
     if gpu is None:
         device = 'cpu'
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/train.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/train.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/DeNas/utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/DeNas/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/backbone/factory.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/backbone/factory.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/dataset/__init__.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/dataset/cifar.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/dataset/cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/dataset/composed_dataset.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/dataset/composed_dataset.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/dataset/office31.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/dataset/office31.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/default_ma.conf` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/default_ma.conf`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,20 +64,20 @@
     # inline: random module
     @staticmethod
     def random():
         return RNG.random()
 
     @staticmethod
     def uniform(a, b):
-        return random.random() * (b - a) + a
+        return random.random() * (b - a) + a #nosec
 
     @staticmethod
     def randint(a, b):
         # [low, high]
-        return min(int(random.random() * (b - a + 1)) + a, b)
+        return min(int(random.random() * (b - a + 1)) + a, b) #nosec
 
     @staticmethod
     def gauss(mu, sigma):
         return RNG.normal(mu, sigma)
 
 
 class np_random:
@@ -86,16 +86,16 @@
     def choice(a, size, *args, **kwargs):
         return RNG.choice(a, size, *args, **kwargs)
 
     @staticmethod
     def randint(low, high, size=None, dtype=int):
         # [low, high)
         if size is None:
-            return dtype(random.randint(low, high - 1))
-        out = [random.randint(low, high - 1) for _ in range(size)]
+            return dtype(random.randint(low, high - 1)) #nosec
+        out = [random.randint(low, high - 1) for _ in range(size)] #nosec
         return np.array(out, dtype=dtype)
 
     @staticmethod
     def rand(*shape):
         return RNG.random(shape)
 
     @staticmethod
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/main.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/main.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/training/task.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/training/task.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/ModelAdapter/training/train.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/ModelAdapter/training/train.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/SDA.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/SDA.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,25 +54,25 @@
             used with e2eaiok, optional.
         """
         self.model = model
         if data_loader is None and 'data_path' in settings:
             data_loader = HydroDataLoaderAdvisor.create_data_loader(
                 settings['data_path'], self.model)
         self.data_loader = data_loader
-        self.custom_result_path = custom_result_path
+        self.custom_result_path = custom_result_path if custom_result_path is not None else "./"
         if self.data_loader != None:
             self.dataset_meta = self.data_loader.get_meta()
             self.dataset_train = self.data_loader.get_train()
             self.dataset_valid = self.data_loader.get_valid()
         else:
             self.dataset_meta = None
             self.dataset_train = None
             self.dataset_valid = None
         self.settings = default_settings(model, settings)
-        self.hydro_model = hydro_model
+        self.hydro_model = hydro_model if hydro_model is not None else HydroModel(settings)
         logging.basicConfig(
             level=logging.INFO,
             format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
         self.logger = logging.getLogger('E2EAIOK.SDA')
         self.logger.info("""### Ready to submit current task  ###""")
 
     def __del__(self):
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/BERTAdvisor.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/BERTAdvisor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess
+import subprocess #nosec
 import yaml
 import logging
 import os
 
 from e2eAIOK.common.utils import *
 from e2eAIOK.SDA.modeladvisor.BaseModelAdvisor import BaseModelAdvisor
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/BaseModelAdvisor.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/BaseModelAdvisor.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/DIENAdvisor.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/DIENAdvisor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-import subprocess
+import subprocess #nosec
 import yaml
 
 from e2eAIOK.common.utils import *
 from e2eAIOK.SDA.modeladvisor.BaseModelAdvisor import BaseModelAdvisor
 import psutil
 
 class DIENAdvisor(BaseModelAdvisor):
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/DLRMAdvisor.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/DLRMAdvisor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess
+import subprocess #nosec
 import yaml
 import logging
 import time
 import os
 
 from e2eAIOK.common.utils import *
 from e2eAIOK.SDA.modeladvisor.BaseModelAdvisor import BaseModelAdvisor
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/MiniGoAdvisor.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/MiniGoAdvisor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess
+import subprocess #nosec
 import yaml
 import logging
 import time
 import os
 
 from e2eAIOK.common.utils import *
 from e2eAIOK.SDA.modeladvisor.BaseModelAdvisor import BaseModelAdvisor
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/RNNTAdvisor.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/RNNTAdvisor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess
+import subprocess #nosec
 import yaml
 import logging
 import time
 
 from e2eAIOK.common.utils import *
 from e2eAIOK.SDA.modeladvisor.BaseModelAdvisor import BaseModelAdvisor
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/RegisteredAdvisor.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/RegisteredAdvisor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess
+import subprocess #nosec
 import yaml
 import logging
 import time
 
 from e2eAIOK.common.utils import *
 from e2eAIOK.utils.hydroconfig import default_settings
 from e2eAIOK.SDA.modeladvisor.BaseModelAdvisor import BaseModelAdvisor
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/ResNetAdvisor.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/ResNetAdvisor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess
+import subprocess #nosec
 import yaml
 import logging
 import time
 import sys
 
 from e2eAIOK.common.utils import *
 from e2eAIOK.SDA.modeladvisor.BaseModelAdvisor import BaseModelAdvisor
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/TestAdvisor.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/TestAdvisor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess
+import subprocess #nosec
 import yaml
 import logging
 import time
 
 
 from e2eAIOK.common.utils import *
 from e2eAIOK.utils.hydroconfig import default_settings
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/TwitterRecSysAdvisor.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/TwitterRecSysAdvisor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess
+import subprocess #nosec
 import yaml
 import logging
 import time
 
 from e2eAIOK.common.utils import *
 from e2eAIOK.SDA.modeladvisor.BaseModelAdvisor import BaseModelAdvisor
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/UPMAdvisor.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/UPMAdvisor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess
+import subprocess #nosec
 import yaml
 import logging
 import time
 
 from e2eAIOK.common.utils import *
 from e2eAIOK.SDA.modeladvisor.BaseModelAdvisor import BaseModelAdvisor
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/SDA/modeladvisor/WnDAdvisor.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/SDA/modeladvisor/WnDAdvisor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess
+import subprocess #nosec
 import yaml
 import logging
 import time
 
 from e2eAIOK.common.utils import *
 from e2eAIOK.SDA.modeladvisor.BaseModelAdvisor import BaseModelAdvisor
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/default.conf` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/default.conf`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/data_builder_asr.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/data_builder_asr.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/data_builder_cv.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/data_builder_cv.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/data_builder_nlp.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/data_builder_nlp.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/data_utils/data_utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/data_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/data_utils/image_list.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/data_utils/image_list.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/data_builder.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/data_builder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/cv/lenet.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/cv/lenet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/cv/resnet_cifar.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/cv/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model/model_utils/model_utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model/model_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/model_builder.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/model_builder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/torch_trainer.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/torch_trainer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/utils/extend_distributed.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/utils/extend_distributed.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/trainer/utils/utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/trainer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/common/utils.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/common/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/dataloader/hydrodataloader.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/dataloader/hydrodataloader.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/hydroDB.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/hydroDB.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/hydroautolearner.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/hydroautolearner.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/hydroconfig.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/hydroconfig.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/hydromodel.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/hydromodel.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK/utils/hydroserver.py` & `e2eAIOK-1.0.1b2023042100/e2eAIOK/utils/hydroserver.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK.egg-info/PKG-INFO` & `e2eAIOK-1.0.1b2023042100/e2eAIOK.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2eAIOK
-Version: 1.0.1b2023042000
+Version: 1.0.1b2023042100
 Summary: Intel® End-to-End AI Optimization Kit
 Home-page: https://github.com/intel/e2eAIOK
 Author: INTEL
 License: Apache License
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/issues
 Description: # [Intel® End-to-End AI Optimization Kit](https://github.com/intel/e2eAIOK)
         
@@ -101,14 +101,21 @@
                * [Finetuner](demo/ma/finetuner/Model_Adapter_Finetuner_Walkthrough_ResNet50_CIFAR100.ipynb) - Computer Vision, Image Classification, ResNet50, PyTorch
                * [Distiller](demo/ma/distiller/Model_Adapter_Distiller_Walkthrough_VIT_to_ResNet18_CIFAR100.ipynb) - Computer Vision, Image Classification, ResNet18, PyTorch
                * [Domain Adapter](demo/ma/domain_adapter/Model_Adapter_Domain_Adapter_Walkthrough_Unet_KITS19.ipynb) - Computer Vision, Medical Segmentation, 3D Unet, PyTorch
         
         ## Performance
         
         Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
+        For [DeNAS](e2eAIOK/DeNas/README.md) CNN and ViT, Intel® End-to-End AI Optimization Kit delivered 40.73x and 35.63x search time speedup, 82.57x and 4.44x training time speedup over [ZenNAS](https://github.com/idstcv/ZenNAS) and [AutoFormer](https://github.com/microsoft/Cream/tree/main/AutoFormer) respectively. For DeNAS searched CNN, ViT, BERT and ASR model, Intel® End-to-End AI Optimization Kit delivered 9.86x, 4.44x, 7.68x and 59.12x training time speedup with 0.03x, 1.20x, 0.62x and 0.81x model size respectively. Please refer to DeNAS link for detailed test dataset and test method.
+        > Noted: Optimized lighter models' accuracy are slightly lower: CNN -3% accuracy, ViT -5% accuracy, BERT -4% F1 score.
+        
+        ![Performance](./docs/source/e2eaiok_v10_performance_nas.png "Intel® End-to-End AI Optimization Kit Performance")
+        ![Performance](./docs/source/e2eaiok_v10_performance_stock.png "Intel® End-to-End AI Optimization Kit Performance")
+        
+        Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
         For [MiniGO](modelzoo/minigo/README.md), [BERT](modelzoo/bert/README.md), [ResNet](modelzoo/resnet/README.md), [RNN-T](modelzoo/rnnt/README.md), Intel® End-to-End AI Optimization Kit delivered 13.06x, 10.10x, 8.77x and 14.19x training time speedup respecitvely through E2E optimizations. Please refer to corresponding model link for detailed test dataset and test method. 
         > Noted: Optimized lighter models' accuracy are slightly lower: ResNet -5% accuracy, BERT -1% F1 score.
         
         ![Performance](./docs/source/e2eaiok_v02_performance.png "Intel® End-to-End AI Optimization Kit Performance")
         
         Performance results are evaluated on 4-node cluster configured with Intel(R) Xeon(R) Platinum 8358 Scalable processor.
         For [WnD](modelzoo/WnD/README.md), [DIEN](modelzoo/dien/README.md) and [DLRM](modelzoo/dlrm/README.md), Intel® End-to-End AI Optimization Kit delivered 51.01x(5.02x ELT & 113.03x training), 12.67x(14.86x ELT & 11.91x training) and 71.16x(86.40x ELT & 42.31x training) E2E time speedup, 21.18x, 14.11x and 124.98x inference throughput speedup respectively. Please refer to corresponding model link for detailed test dataset and test method.
```

### Comparing `e2eAIOK-1.0.1b2023042000/e2eAIOK.egg-info/SOURCES.txt` & `e2eAIOK-1.0.1b2023042100/e2eAIOK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e2eAIOK-1.0.1b2023042000/setup.py` & `e2eAIOK-1.0.1b2023042100/setup.py`

 * *Files identical despite different names*

