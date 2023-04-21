# Comparing `tmp/funasr-0.4.1.tar.gz` & `tmp/funasr-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/funasr-0.4.1.tar", last modified: Fri Apr 14 15:33:48 2023, max compression
+gzip compressed data, was "dist/funasr-0.4.2.tar", last modified: Fri Apr 21 11:15:55 2023, max compression
```

## Comparing `funasr-0.4.1.tar` & `funasr-0.4.2.tar`

### file list

```diff
@@ -1,437 +1,437 @@
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1063 2023-02-24 12:39:00.000000 funasr-0.4.1/LICENSE
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6614 2023-04-14 15:33:48.000000 funasr-0.4.1/PKG-INFO
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5601 2023-04-14 15:32:13.000000 funasr-0.4.1/README.md
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:47.000000 funasr-0.4.1/funasr/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      203 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/__init__.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/bin/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/__init__.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     3798 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/aggregate_stats_dirs.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    21262 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/bin/asr_inference.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9781 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/asr_inference_launch.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    25900 2023-03-17 12:37:43.000000 funasr-0.4.1/funasr/bin/asr_inference_mfcca.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    37621 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/bin/asr_inference_paraformer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    33372 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/bin/asr_inference_paraformer_streaming.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    19177 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/bin/asr_inference_paraformer_vad.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    32909 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/bin/asr_inference_paraformer_vad_punc.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    34244 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/bin/asr_inference_rnnt.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    23884 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/bin/asr_inference_uniasr.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    23931 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/bin/asr_inference_uniasr_vad.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1006 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/asr_train.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1027 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/asr_train_paraformer.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1024 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/asr_train_uniasr.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5309 2023-03-16 11:52:36.000000 funasr-0.4.1/funasr/bin/build_trainer.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1012 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/data2vec_train.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     5365 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/diar_inference_launch.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1010 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/bin/diar_train.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)    14072 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/bin/eend_ola_inference.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     6814 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/lm_calc_perplexity.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    14615 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/lm_inference.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3989 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/lm_inference_launch.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1019 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/lm_train.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     3049 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/modelscope_infer.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     3767 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/punc_inference_launch.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      828 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/bin/punc_train.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12002 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/bin/punctuation_infer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    11193 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/punctuation_infer_vadrealtime.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)    20635 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/bin/sond_inference.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)    14771 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/bin/sv_inference.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     4756 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/sv_inference_launch.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     8449 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/bin/tokenize_text.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12520 2023-03-22 05:51:29.000000 funasr-0.4.1/funasr/bin/tp_inference.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4048 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/tp_inference_launch.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12389 2023-03-22 05:51:29.000000 funasr-0.4.1/funasr/bin/vad_inference.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4275 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/bin/vad_inference_launch.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    11682 2023-04-06 02:32:27.000000 funasr-0.4.1/funasr/bin/vad_inference_online.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/datasets/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4338 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/collate_fn.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    15174 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/datasets/dataset.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    15562 2023-03-17 12:37:43.000000 funasr-0.4.1/funasr/datasets/iterable_dataset.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12671 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/iterable_dataset_modelscope.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/datasets/large_datasets/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3488 2023-03-22 05:51:29.000000 funasr-0.4.1/funasr/datasets/large_datasets/build_dataloader.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/datasets/large_datasets/datapipes/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8298 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/datapipes/batch.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      519 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/datapipes/filter.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      453 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/datapipes/map.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8055 2023-03-22 05:51:29.000000 funasr-0.4.1/funasr/datasets/large_datasets/dataset.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/datasets/large_datasets/utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1382 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/utils/clipping.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1013 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/utils/filter.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      948 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1201 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/datasets/large_datasets/utils/padding.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2037 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/datasets/large_datasets/utils/tokenize.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1281 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/datasets/ms_dataset.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    30767 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/datasets/preprocessor.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10833 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/export/export_model.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/models/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5091 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/export/models/CT_Transformer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1540 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/export/models/__init__.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/models/decoder/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/models/decoder/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6326 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/export/models/decoder/sanm_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5470 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/export/models/decoder/transformer_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8441 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/export/models/e2e_asr_paraformer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2047 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/models/e2e_vad.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/models/encoder/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/models/encoder/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3881 2023-03-15 12:41:42.000000 funasr-0.4.1/funasr/export/models/encoder/conformer_encoder.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     9141 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/models/encoder/fsmn_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7524 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/export/models/encoder/sanm_encoder.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/models/modules/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/models/modules/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1931 2023-03-15 12:41:42.000000 funasr-0.4.1/funasr/export/models/modules/decoder_layer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2354 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/export/models/modules/encoder_layer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      658 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/models/modules/feedforward.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8644 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/export/models/modules/multihead_att.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/models/predictor/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/models/predictor/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9917 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/export/models/predictor/cif.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/test/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/test/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      785 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/test/test_onnx.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      702 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/test/test_onnx_punc.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      966 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1046 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/test/test_onnx_vad.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      477 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/export/test/test_torchscripts.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/torch_quant/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      642 2023-03-10 03:02:25.000000 funasr-0.4.1/funasr/export/torch_quant/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2385 2023-03-16 11:05:28.000000 funasr-0.4.1/funasr/export/torch_quant/amp_module.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    18267 2023-03-15 12:46:52.000000 funasr-0.4.1/funasr/export/torch_quant/graph.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7297 2023-03-15 12:46:52.000000 funasr-0.4.1/funasr/export/torch_quant/module.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2063 2023-03-15 12:46:52.000000 funasr-0.4.1/funasr/export/torch_quant/observed_module.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    30293 2023-03-15 12:46:52.000000 funasr-0.4.1/funasr/export/torch_quant/observer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10070 2023-03-15 12:46:52.000000 funasr-0.4.1/funasr/export/torch_quant/quantizer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      620 2023-03-10 03:02:25.000000 funasr-0.4.1/funasr/export/torch_quant/version.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/export/utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2620 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/export/utils/torch_function.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/fileio/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/fileio/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2383 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/fileio/datadir_writer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2357 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/fileio/npy_scp.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2361 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/fileio/rand_gen_dataset.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2273 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/fileio/read_text.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3479 2023-03-16 11:52:36.000000 funasr-0.4.1/funasr/fileio/sound_scp.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/iterators/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/iterators/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      234 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/iterators/abs_iter_factory.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7808 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/iterators/chunk_iter_factory.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1140 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/iterators/multiple_iter_factory.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5236 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/iterators/sequence_iter_factory.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/layers/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      359 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/abs_normalize.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6717 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/complex_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3503 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/global_mvn.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      349 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/inversible_interface.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2539 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/layers/label_aggregation.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2564 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/log_mel.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10488 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/mask_along_axis.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9033 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/sinc_conv.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8436 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/stft.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2513 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/time_warp.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2309 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/layers/utterance_mvn.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/lm/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/lm/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5436 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/lm/abs_model.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5904 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/lm/seq_rnn_lm.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4243 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/lm/transformer_lm.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/losses/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/losses/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2804 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/losses/label_smoothing_loss.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/main_funcs/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/main_funcs/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4687 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/main_funcs/average_nbest_models.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5610 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/main_funcs/calculate_all_attentions.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5029 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/main_funcs/collect_stats.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9906 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/main_funcs/pack_funcs.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6541 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/ctc.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5298 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/data2vec.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/decoder/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/decoder/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      473 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/decoder/abs_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    40834 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/decoder/contextual_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12133 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/decoder/rnn_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    75199 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/decoder/sanm_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1389 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/decoder/sv_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    28528 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/decoder/transformer_decoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    16707 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/e2e_asr.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8572 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/e2e_asr_common.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    11630 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/models/e2e_asr_mfcca.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    67325 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/e2e_asr_paraformer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10238 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/models/e2e_diar_eend_ola.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    20581 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/models/e2e_diar_sond.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10098 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/models/e2e_sv.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6710 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/e2e_tp.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    51737 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/e2e_uni_asr.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    31090 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/e2e_vad.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/encoder/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      503 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/abs_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    23724 2023-02-24 16:26:34.000000 funasr-0.4.1/funasr/models/encoder/conformer_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    20993 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/data2vec_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    19855 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10164 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/encoder_layer_mfcca.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     9281 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/models/encoder/fsmn_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    17514 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/mfcca_encoder.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/encoder/opennmt_encoders/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      909 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    11046 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    13971 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    21170 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    41077 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/models/encoder/resnet34_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3634 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/rnn_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    53220 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/encoder/sanm_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    26890 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/encoder/transformer_encoder.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/frontend/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/frontend/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      400 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/frontend/abs_frontend.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8895 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/frontend/default.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1405 2023-03-16 11:52:36.000000 funasr-0.4.1/funasr/models/frontend/eend_ola_feature.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5759 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/frontend/fused.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4990 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/frontend/s3prl.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    20552 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/models/frontend/wav_frontend.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6322 2023-02-24 16:26:34.000000 funasr-0.4.1/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2817 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/frontend/windowing.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/pooling/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/pooling/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3546 2023-03-16 11:52:36.000000 funasr-0.4.1/funasr/models/pooling/statistic_pooling.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/postencoder/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/postencoder/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      403 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/postencoder/abs_postencoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3626 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/predictor/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/predictor/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    34651 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/models/predictor/cif.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/preencoder/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/preencoder/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      402 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/preencoder/abs_preencoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1042 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/preencoder/linear.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10296 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/preencoder/sinc.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/models/specaug/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/specaug/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      426 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/specaug/abs_specaug.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6607 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/models/specaug/specaug.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4661 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/target_delay_transformer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4715 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/models/vad_realtime_transformer.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      940 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/add_sos_eos.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    28945 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/modules/attention.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/beam_search/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/beam_search/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    13305 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/beam_search/batch_beam_search.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    10175 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    53592 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/beam_search/beam_search.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/data2vec/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5831 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/data_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4474 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/ema_module.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      442 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/grad_multiply.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    26458 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/multihead_attention.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4021 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/quant_noise.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4858 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12734 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/data2vec/wav2vec2.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4244 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/dynamic_conv.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4863 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/dynamic_conv2d.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8572 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/e2e_asr_common.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/eend_ola/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-16 11:52:36.000000 funasr-0.4.1/funasr/modules/eend_ola/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5287 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/modules/eend_ola/encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2768 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/modules/eend_ola/encoder_decoder_attractor.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    14578 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/modules/embedding.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/frontends/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       30 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/frontends/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2731 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/frontends/beamformer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5540 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/frontends/dnn_beamformer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2825 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/frontends/dnn_wpe.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7958 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/frontends/feature_transform.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4585 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/frontends/frontend.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2648 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/frontends/mask_estimator.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      958 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/layer_norm.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3590 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/lightconv.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4230 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/lightconv2d.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1654 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/modules/mask.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4800 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/multi_layer_conv.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    16630 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/nets_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1936 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/positionwise_feed_forward.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      703 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/repeat.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/rnn/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       30 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/rnn/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4080 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/rnn/argument.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    66987 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/rnn/attentions.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    49387 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/rnn/decoders.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    14180 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/rnn/encoders.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/scorers/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       30 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/scorers/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5026 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/scorers/ctc.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    13951 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/scorers/ctc_prefix_score.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1787 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/scorers/length_bonus.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5938 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/scorers/scorer_interface.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/modules/streaming_utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/streaming_utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    17409 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/modules/streaming_utils/chunk_utilis.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1809 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/streaming_utils/load_fr_tf.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2399 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/streaming_utils/utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    14104 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/subsampling.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1898 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/modules/subsampling_without_posenc.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/optimizers/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/optimizers/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5643 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/optimizers/fairseq_adam.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      828 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/optimizers/sgd.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/runtime/__init__.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/python/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/runtime/python/__init__.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/python/libtorch/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/runtime/python/libtorch/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      544 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/runtime/python/libtorch/demo.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      752 2023-04-06 02:53:05.000000 funasr-0.4.1/funasr/runtime/python/libtorch/demo_gpu.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       65 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8172 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     5123 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7040 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4845 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1433 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/runtime/python/libtorch/setup.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      845 2023-04-06 02:55:18.000000 funasr-0.4.1/funasr/runtime/python/libtorch/test_rtf.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      617 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/demo.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      751 2023-04-06 02:45:07.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/demo_gpu.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      740 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      932 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      383 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      969 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      218 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7786 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12135 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    28927 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    15845 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-29 02:53:52.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9176 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9707 2023-04-14 03:21:54.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      658 2023-02-27 05:06:50.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/infer_onnx.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1384 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/setup.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      451 2023-03-29 03:37:22.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/test_pipeline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1473 2023-03-29 05:24:31.000000 funasr-0.4.1/funasr/runtime/python/onnxruntime/test_pipeline_online.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/samplers/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      425 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/abs_sampler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6231 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/build_batch_sampler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5716 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/folded_batch_sampler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5168 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/length_batch_sampler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5680 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/num_elements_batch_sampler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3144 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/sorted_batch_sampler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2940 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/samplers/unsorted_batch_sampler.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/schedulers/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/schedulers/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1679 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/schedulers/abs_scheduler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2067 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/schedulers/noam_lr.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3658 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/schedulers/tri_stage_scheduler.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1494 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/schedulers/warmup_lr.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/tasks/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/tasks/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    73893 2023-04-14 02:00:09.000000 funasr-0.4.1/funasr/tasks/abs_task.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    47984 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/tasks/asr.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12089 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/tasks/data2vec.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    32463 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/tasks/diar.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6782 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/tasks/lm.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8029 2023-04-14 01:58:44.000000 funasr-0.4.1/funasr/tasks/punctuation.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    18814 2023-04-14 15:16:16.000000 funasr-0.4.1/funasr/tasks/sv.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12527 2023-04-07 14:32:06.000000 funasr-0.4.1/funasr/tasks/vad.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/text/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      347 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/abs_tokenizer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2205 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/build_tokenizer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2230 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/char_tokenizer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1479 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/cleaner.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1968 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/korean_cleaner.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    16601 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/phoneme_tokenizer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1294 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/sentencepiece_tokenizer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2100 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/token_id_converter.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2074 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/text/word_tokenizer.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/torch_utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      987 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/add_gradient_noise.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2681 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/device_funcs.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1052 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/forward_adaptor.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3788 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/initialize.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3815 2023-03-16 11:52:44.000000 funasr-0.4.1/funasr/torch_utils/load_pretrained_model.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2498 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/model_summary.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      468 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/pytorch_version.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1615 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/recursive_op.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      167 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/torch_utils/set_all_random_seed.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/train/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/train/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1764 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/train/abs_espnet_model.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7280 2023-04-07 13:46:02.000000 funasr-0.4.1/funasr/train/abs_model.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3017 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/train/class_choices.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    14493 2023-03-09 02:53:43.000000 funasr-0.4.1/funasr/train/distributed_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    18344 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/train/reporter.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    35996 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/train/trainer.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/funasr/utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2664 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/asr_env_checking.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    11612 2023-03-17 12:37:43.000000 funasr-0.4.1/funasr/utils/asr_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      582 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/build_dataclass.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1380 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/cli_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2078 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/compute_eer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6714 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/compute_min_dcf.py
--rwxrwxr-x   0 gzf       (1006) gzf       (1007)     5189 2023-04-07 06:55:12.000000 funasr-0.4.1/funasr/utils/compute_wer.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1760 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/config_argparse.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1830 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/get_default_kwargs.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     5632 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/griffin_lim.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4001 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/job_runner.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1607 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/misc.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1357 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/modelscope_param.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3598 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/nested_dict_action.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7735 2023-04-06 02:32:27.000000 funasr-0.4.1/funasr/utils/postprocess_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2027 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/sized_dict.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    13178 2023-03-22 05:51:29.000000 funasr-0.4.1/funasr/utils/timestamp_tools.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4185 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/types.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    11759 2023-03-16 11:52:36.000000 funasr-0.4.1/funasr/utils/wav_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      380 2023-02-24 12:39:00.000000 funasr-0.4.1/funasr/utils/yaml_no_alias_safe_dump.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        6 2023-04-14 15:32:13.000000 funasr-0.4.1/funasr/version.txt
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:47.000000 funasr-0.4.1/funasr.egg-info/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     6614 2023-04-14 15:33:47.000000 funasr-0.4.1/funasr.egg-info/PKG-INFO
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    13807 2023-04-14 15:33:47.000000 funasr-0.4.1/funasr.egg-info/SOURCES.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-04-14 15:33:47.000000 funasr-0.4.1/funasr.egg-info/dependency_links.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      857 2023-04-14 15:33:47.000000 funasr-0.4.1/funasr.egg-info/requires.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        7 2023-04-14 15:33:47.000000 funasr-0.4.1/funasr.egg-info/top_level.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       38 2023-04-14 15:33:48.000000 funasr-0.4.1/setup.cfg
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     4562 2023-04-06 02:32:27.000000 funasr-0.4.1/setup.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/test/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      494 2023-03-31 07:25:30.000000 funasr-0.4.1/test/test_moddelscope_punc.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1028 2023-03-31 07:26:37.000000 funasr-0.4.1/test/test_moddelscope_punc_online.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      537 2023-03-31 14:17:23.000000 funasr-0.4.1/test/test_modelscope_paraformer_long.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      809 2023-04-14 02:06:28.000000 funasr-0.4.1/test/test_modelscope_pipeline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1399 2023-03-31 14:15:12.000000 funasr-0.4.1/test/test_modelscope_vad.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2514 2023-04-13 11:54:40.000000 funasr-0.4.1/test/test_onnx_encoder.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1773 2023-03-13 12:16:53.000000 funasr-0.4.1/test/test_rtf.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:33:48.000000 funasr-0.4.1/tests/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    25268 2023-04-14 02:00:09.000000 funasr-0.4.1/tests/test_asr_inference_pipeline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1210 2023-03-16 11:52:36.000000 funasr-0.4.1/tests/test_asr_vad_punc_inference_pipeline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2083 2023-03-09 02:53:43.000000 funasr-0.4.1/tests/test_inference_pipeline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      804 2023-03-16 11:52:36.000000 funasr-0.4.1/tests/test_lm_pipeline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2055 2023-04-14 02:00:09.000000 funasr-0.4.1/tests/test_punctuation_pipeline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1949 2023-03-17 07:00:20.000000 funasr-0.4.1/tests/test_sv_inference_pipeline.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1250 2023-03-16 11:52:36.000000 funasr-0.4.1/tests/test_vad_inference_pipeline.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1063 2023-02-24 12:39:00.000000 funasr-0.4.2/LICENSE
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7855 2023-04-21 11:15:55.000000 funasr-0.4.2/PKG-INFO
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6813 2023-04-21 03:10:43.000000 funasr-0.4.2/README.md
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      203 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/__init__.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/bin/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/bin/__init__.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     3798 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/bin/aggregate_stats_dirs.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    21327 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/asr_inference.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    11203 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/asr_inference_launch.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    25965 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/asr_inference_mfcca.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    37755 2023-04-21 03:10:43.000000 funasr-0.4.2/funasr/bin/asr_inference_paraformer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    33456 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/asr_inference_paraformer_streaming.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    19242 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/asr_inference_paraformer_vad.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    32974 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/asr_inference_paraformer_vad_punc.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    25059 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/asr_inference_rnnt.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    23949 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/asr_inference_uniasr.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    23931 2023-04-07 06:55:12.000000 funasr-0.4.2/funasr/bin/asr_inference_uniasr_vad.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1006 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/bin/asr_train.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1027 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/bin/asr_train_paraformer.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1036 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/asr_train_transducer.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1024 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/bin/asr_train_uniasr.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5309 2023-03-16 11:52:36.000000 funasr-0.4.2/funasr/bin/build_trainer.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1012 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/bin/data2vec_train.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     5327 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/diar_inference_launch.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1010 2023-03-09 02:53:43.000000 funasr-0.4.2/funasr/bin/diar_train.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)    14137 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/eend_ola_inference.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     6814 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/bin/lm_calc_perplexity.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    14544 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/lm_inference.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3816 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/lm_inference_launch.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     1019 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/bin/lm_train.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     3049 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/bin/modelscope_infer.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     3593 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/punc_inference_launch.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      828 2023-03-09 02:53:43.000000 funasr-0.4.2/funasr/bin/punc_train.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    11940 2023-04-21 11:13:25.000000 funasr-0.4.2/funasr/bin/punctuation_infer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    11121 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/punctuation_infer_vadrealtime.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)    20700 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/sond_inference.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)    14841 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/sv_inference.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     4718 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/sv_inference_launch.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     8449 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/bin/tokenize_text.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12597 2023-04-21 03:10:43.000000 funasr-0.4.2/funasr/bin/tp_inference.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3874 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/tp_inference_launch.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    20031 2023-04-21 11:13:25.000000 funasr-0.4.2/funasr/bin/vad_inference.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4282 2023-04-21 11:13:25.000000 funasr-0.4.2/funasr/bin/vad_inference_launch.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    11752 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/bin/vad_inference_online.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/datasets/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/datasets/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4338 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/datasets/collate_fn.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    15174 2023-04-14 02:00:09.000000 funasr-0.4.2/funasr/datasets/dataset.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    15562 2023-03-17 12:37:43.000000 funasr-0.4.2/funasr/datasets/iterable_dataset.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12671 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/datasets/iterable_dataset_modelscope.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/datasets/large_datasets/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/datasets/large_datasets/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3488 2023-03-22 05:51:29.000000 funasr-0.4.2/funasr/datasets/large_datasets/build_dataloader.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/datasets/large_datasets/datapipes/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8298 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      519 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      453 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/datasets/large_datasets/datapipes/map.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8055 2023-03-22 05:51:29.000000 funasr-0.4.2/funasr/datasets/large_datasets/dataset.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/datasets/large_datasets/utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/datasets/large_datasets/utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1382 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/datasets/large_datasets/utils/clipping.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1013 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/datasets/large_datasets/utils/filter.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      948 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1201 2023-03-09 02:53:43.000000 funasr-0.4.2/funasr/datasets/large_datasets/utils/padding.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2003 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1281 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/datasets/ms_dataset.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    30718 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/datasets/preprocessor.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/export/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/export/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10833 2023-04-14 01:58:44.000000 funasr-0.4.2/funasr/export/export_model.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/export/models/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5091 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/export/models/CT_Transformer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1540 2023-04-14 02:00:09.000000 funasr-0.4.2/funasr/export/models/__init__.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/export/models/decoder/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/export/models/decoder/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6326 2023-04-14 01:58:44.000000 funasr-0.4.2/funasr/export/models/decoder/sanm_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5470 2023-03-09 02:53:43.000000 funasr-0.4.2/funasr/export/models/decoder/transformer_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8441 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/export/models/e2e_asr_paraformer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2047 2023-04-07 13:46:02.000000 funasr-0.4.2/funasr/export/models/e2e_vad.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/export/models/encoder/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/export/models/encoder/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3881 2023-03-15 12:41:42.000000 funasr-0.4.2/funasr/export/models/encoder/conformer_encoder.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     9141 2023-04-07 13:46:02.000000 funasr-0.4.2/funasr/export/models/encoder/fsmn_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7524 2023-04-14 01:58:44.000000 funasr-0.4.2/funasr/export/models/encoder/sanm_encoder.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/export/models/modules/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/export/models/modules/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1931 2023-03-15 12:41:42.000000 funasr-0.4.2/funasr/export/models/modules/decoder_layer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2354 2023-03-16 11:52:44.000000 funasr-0.4.2/funasr/export/models/modules/encoder_layer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      658 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/export/models/modules/feedforward.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8644 2023-04-14 01:58:44.000000 funasr-0.4.2/funasr/export/models/modules/multihead_att.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/export/models/predictor/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/export/models/predictor/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9917 2023-04-14 01:58:44.000000 funasr-0.4.2/funasr/export/models/predictor/cif.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/export/test/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-04-07 13:46:02.000000 funasr-0.4.2/funasr/export/test/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      785 2023-04-07 13:46:02.000000 funasr-0.4.2/funasr/export/test/test_onnx.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      702 2023-04-07 13:46:02.000000 funasr-0.4.2/funasr/export/test/test_onnx_punc.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      966 2023-04-07 13:46:02.000000 funasr-0.4.2/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1046 2023-04-07 13:46:02.000000 funasr-0.4.2/funasr/export/test/test_onnx_vad.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      477 2023-04-07 13:46:02.000000 funasr-0.4.2/funasr/export/test/test_torchscripts.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/export/torch_quant/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      642 2023-03-10 03:02:25.000000 funasr-0.4.2/funasr/export/torch_quant/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2385 2023-03-16 11:05:28.000000 funasr-0.4.2/funasr/export/torch_quant/amp_module.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    18267 2023-03-15 12:46:52.000000 funasr-0.4.2/funasr/export/torch_quant/graph.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7297 2023-03-15 12:46:52.000000 funasr-0.4.2/funasr/export/torch_quant/module.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2063 2023-03-15 12:46:52.000000 funasr-0.4.2/funasr/export/torch_quant/observed_module.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    30293 2023-03-15 12:46:52.000000 funasr-0.4.2/funasr/export/torch_quant/observer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10070 2023-03-15 12:46:52.000000 funasr-0.4.2/funasr/export/torch_quant/quantizer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      620 2023-03-10 03:02:25.000000 funasr-0.4.2/funasr/export/torch_quant/version.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/export/utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/export/utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2620 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/export/utils/torch_function.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/fileio/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/fileio/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2383 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/fileio/datadir_writer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2357 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/fileio/npy_scp.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2361 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/fileio/rand_gen_dataset.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2273 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/fileio/read_text.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3479 2023-03-16 11:52:36.000000 funasr-0.4.2/funasr/fileio/sound_scp.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/iterators/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/iterators/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      234 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/iterators/abs_iter_factory.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7808 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/iterators/chunk_iter_factory.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1140 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/iterators/multiple_iter_factory.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5236 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/iterators/sequence_iter_factory.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/layers/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/layers/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      359 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/layers/abs_normalize.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6717 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/layers/complex_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3503 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/layers/global_mvn.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      349 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/layers/inversible_interface.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2539 2023-03-09 02:53:43.000000 funasr-0.4.2/funasr/layers/label_aggregation.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2564 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/layers/log_mel.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10488 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/layers/mask_along_axis.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9033 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/layers/sinc_conv.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8436 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/layers/stft.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2513 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/layers/time_warp.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2309 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/layers/utterance_mvn.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/lm/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/lm/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5436 2023-04-07 13:46:02.000000 funasr-0.4.2/funasr/lm/abs_model.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5904 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/lm/seq_rnn_lm.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4243 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/lm/transformer_lm.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/losses/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/losses/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2804 2023-03-09 02:53:43.000000 funasr-0.4.2/funasr/losses/label_smoothing_loss.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/main_funcs/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/main_funcs/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4687 2023-03-16 11:52:44.000000 funasr-0.4.2/funasr/main_funcs/average_nbest_models.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5610 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/main_funcs/calculate_all_attentions.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5029 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/main_funcs/collect_stats.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9906 2023-03-16 11:52:44.000000 funasr-0.4.2/funasr/main_funcs/pack_funcs.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/models/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6541 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/ctc.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5298 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/data2vec.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/models/decoder/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/decoder/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      473 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/decoder/abs_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    40834 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/models/decoder/contextual_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12133 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/decoder/rnn_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7917 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/models/decoder/rnnt_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    75199 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/models/decoder/sanm_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1389 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/decoder/sv_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    28528 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/models/decoder/transformer_decoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    16707 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/e2e_asr.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8572 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/e2e_asr_common.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    11630 2023-04-14 02:00:09.000000 funasr-0.4.2/funasr/models/e2e_asr_mfcca.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    74061 2023-04-17 08:57:55.000000 funasr-0.4.2/funasr/models/e2e_asr_paraformer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    34689 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/models/e2e_asr_transducer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10238 2023-03-16 11:52:44.000000 funasr-0.4.2/funasr/models/e2e_diar_eend_ola.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    20581 2023-04-14 15:16:16.000000 funasr-0.4.2/funasr/models/e2e_diar_sond.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10098 2023-04-14 15:16:16.000000 funasr-0.4.2/funasr/models/e2e_sv.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6710 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/models/e2e_tp.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    51737 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/models/e2e_uni_asr.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    31100 2023-04-21 11:13:25.000000 funasr-0.4.2/funasr/models/e2e_vad.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/models/encoder/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/encoder/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      503 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/encoder/abs_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    43611 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/models/encoder/conformer_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    20993 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/encoder/data2vec_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    19855 2023-03-09 02:53:43.000000 funasr-0.4.2/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10164 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     9281 2023-03-09 02:53:43.000000 funasr-0.4.2/funasr/models/encoder/fsmn_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    17514 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/encoder/mfcca_encoder.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/models/encoder/opennmt_encoders/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      909 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    11046 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    13971 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    21170 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    41077 2023-04-14 15:16:16.000000 funasr-0.4.2/funasr/models/encoder/resnet34_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3634 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/encoder/rnn_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    53339 2023-04-17 08:57:55.000000 funasr-0.4.2/funasr/models/encoder/sanm_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    26890 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/encoder/transformer_encoder.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/models/frontend/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/frontend/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      400 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/frontend/abs_frontend.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8895 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/frontend/default.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1405 2023-03-16 11:52:36.000000 funasr-0.4.2/funasr/models/frontend/eend_ola_feature.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5759 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/frontend/fused.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4990 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/frontend/s3prl.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    20470 2023-04-21 11:13:25.000000 funasr-0.4.2/funasr/models/frontend/wav_frontend.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6322 2023-02-24 16:26:34.000000 funasr-0.4.2/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2817 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/frontend/windowing.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/models/joint_net/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-04-21 03:10:43.000000 funasr-0.4.2/funasr/models/joint_net/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1855 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/models/joint_net/joint_network.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/models/pooling/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/pooling/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3546 2023-03-16 11:52:36.000000 funasr-0.4.2/funasr/models/pooling/statistic_pooling.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/models/postencoder/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/postencoder/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      403 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/postencoder/abs_postencoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3626 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/models/predictor/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/predictor/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    34651 2023-04-14 15:16:16.000000 funasr-0.4.2/funasr/models/predictor/cif.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/models/preencoder/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/preencoder/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      402 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/preencoder/abs_preencoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1042 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/preencoder/linear.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10296 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/preencoder/sinc.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/models/specaug/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/specaug/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      426 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/specaug/abs_specaug.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6607 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/models/specaug/specaug.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4661 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/models/target_delay_transformer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4715 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/models/vad_realtime_transformer.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/modules/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      940 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/add_sos_eos.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    36791 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/modules/attention.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/modules/beam_search/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/beam_search/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    13305 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/beam_search/batch_beam_search.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    10175 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    53592 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/beam_search/beam_search.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    23002 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/modules/beam_search/beam_search_transducer.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/modules/data2vec/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/data2vec/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5831 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/data2vec/data_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4474 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/data2vec/ema_module.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      442 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/data2vec/grad_multiply.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    26458 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/data2vec/multihead_attention.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4021 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/data2vec/quant_noise.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4858 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/data2vec/utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12734 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/data2vec/wav2vec2.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4244 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/dynamic_conv.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4863 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/dynamic_conv2d.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    13504 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/modules/e2e_asr_common.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/modules/eend_ola/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-16 11:52:36.000000 funasr-0.4.2/funasr/modules/eend_ola/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5287 2023-03-16 11:52:44.000000 funasr-0.4.2/funasr/modules/eend_ola/encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2768 2023-03-16 11:52:44.000000 funasr-0.4.2/funasr/modules/eend_ola/encoder_decoder_attractor.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    18008 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/modules/embedding.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/modules/frontends/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       30 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/frontends/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2731 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/frontends/beamformer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5540 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/frontends/dnn_beamformer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2825 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/frontends/dnn_wpe.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7958 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/frontends/feature_transform.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4585 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/frontends/frontend.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2648 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/frontends/mask_estimator.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      958 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/layer_norm.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3590 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/lightconv.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4230 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/lightconv2d.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1654 2023-03-09 02:53:43.000000 funasr-0.4.2/funasr/modules/mask.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4800 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/multi_layer_conv.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    22115 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/modules/nets_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1936 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/positionwise_feed_forward.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3649 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/modules/repeat.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/modules/rnn/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       30 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/rnn/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4080 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/rnn/argument.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    66987 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/rnn/attentions.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    49387 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/rnn/decoders.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    14180 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/rnn/encoders.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/modules/scorers/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       30 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/scorers/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5026 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/scorers/ctc.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    13951 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/scorers/ctc_prefix_score.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1787 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/scorers/length_bonus.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5938 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/scorers/scorer_interface.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/modules/streaming_utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/streaming_utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    17409 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1809 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2399 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/streaming_utils/utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    21441 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/modules/subsampling.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1898 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/modules/subsampling_without_posenc.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/optimizers/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/optimizers/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5643 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/optimizers/fairseq_adam.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      828 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/optimizers/sgd.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/runtime/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/runtime/__init__.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/runtime/python/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/runtime/python/__init__.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/runtime/python/libtorch/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-09 02:53:43.000000 funasr-0.4.2/funasr/runtime/python/libtorch/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      544 2023-04-07 06:55:12.000000 funasr-0.4.2/funasr/runtime/python/libtorch/demo.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      752 2023-04-06 02:53:05.000000 funasr-0.4.2/funasr/runtime/python/libtorch/demo_gpu.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       65 2023-03-29 02:53:52.000000 funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8172 2023-04-14 02:00:09.000000 funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-29 02:53:52.000000 funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     5123 2023-03-29 02:53:52.000000 funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7040 2023-03-29 02:53:52.000000 funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-29 02:53:52.000000 funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-29 02:53:52.000000 funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4845 2023-04-14 02:00:09.000000 funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1443 2023-04-17 02:17:43.000000 funasr-0.4.2/funasr/runtime/python/libtorch/setup.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      845 2023-04-06 02:55:18.000000 funasr-0.4.2/funasr/runtime/python/libtorch/test_rtf.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      617 2023-04-07 13:46:02.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/demo.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      751 2023-04-06 02:45:07.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/demo_gpu.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      740 2023-04-07 13:46:02.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      932 2023-04-07 13:46:02.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      383 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      969 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      218 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7786 2023-04-14 02:00:09.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12135 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-29 02:53:52.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    28927 2023-04-14 02:00:09.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    15848 2023-04-21 11:13:25.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-29 02:53:52.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-29 02:53:52.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9176 2023-04-14 02:00:09.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9707 2023-04-14 03:21:54.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      658 2023-02-27 05:06:50.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/infer_onnx.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1393 2023-04-21 11:13:25.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/setup.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      451 2023-03-29 03:37:22.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/test_pipeline.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1473 2023-03-29 05:24:31.000000 funasr-0.4.2/funasr/runtime/python/onnxruntime/test_pipeline_online.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/samplers/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/samplers/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      425 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/samplers/abs_sampler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6231 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/samplers/build_batch_sampler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5716 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/samplers/folded_batch_sampler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5168 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/samplers/length_batch_sampler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5680 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/samplers/num_elements_batch_sampler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3144 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/samplers/sorted_batch_sampler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2940 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/samplers/unsorted_batch_sampler.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/schedulers/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/schedulers/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1679 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/schedulers/abs_scheduler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2067 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/schedulers/noam_lr.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3658 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/schedulers/tri_stage_scheduler.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1494 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/schedulers/warmup_lr.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/tasks/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/tasks/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    73890 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/tasks/abs_task.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    60627 2023-04-18 13:28:07.000000 funasr-0.4.2/funasr/tasks/asr.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12089 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/tasks/data2vec.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    32463 2023-04-14 15:16:16.000000 funasr-0.4.2/funasr/tasks/diar.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6782 2023-04-07 13:46:02.000000 funasr-0.4.2/funasr/tasks/lm.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     8029 2023-04-14 01:58:44.000000 funasr-0.4.2/funasr/tasks/punctuation.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    18814 2023-04-14 15:16:16.000000 funasr-0.4.2/funasr/tasks/sv.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12527 2023-04-07 14:32:06.000000 funasr-0.4.2/funasr/tasks/vad.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/text/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/text/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      347 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/text/abs_tokenizer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2205 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/text/build_tokenizer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2230 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/text/char_tokenizer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1479 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/text/cleaner.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1968 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/text/korean_cleaner.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    16601 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/text/phoneme_tokenizer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1294 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/text/sentencepiece_tokenizer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2100 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/text/token_id_converter.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2074 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/text/word_tokenizer.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/torch_utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/torch_utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      987 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/torch_utils/add_gradient_noise.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2681 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/torch_utils/device_funcs.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1052 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/torch_utils/forward_adaptor.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3788 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/torch_utils/initialize.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3815 2023-03-16 11:52:44.000000 funasr-0.4.2/funasr/torch_utils/load_pretrained_model.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2498 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/torch_utils/model_summary.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      468 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/torch_utils/pytorch_version.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1615 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/torch_utils/recursive_op.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      167 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/torch_utils/set_all_random_seed.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/train/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/train/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1764 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/train/abs_espnet_model.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7280 2023-04-07 13:46:02.000000 funasr-0.4.2/funasr/train/abs_model.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3017 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/train/class_choices.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    14493 2023-03-09 02:53:43.000000 funasr-0.4.2/funasr/train/distributed_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    18344 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/train/reporter.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    36453 2023-04-21 03:10:43.000000 funasr-0.4.2/funasr/train/trainer.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr/utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2664 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/asr_env_checking.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    11612 2023-03-17 12:37:43.000000 funasr-0.4.2/funasr/utils/asr_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      582 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/build_dataclass.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1380 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/cli_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2078 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/compute_eer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6714 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/compute_min_dcf.py
+-rwxrwxr-x   0 gzf       (1006) gzf       (1007)     5189 2023-04-07 06:55:12.000000 funasr-0.4.2/funasr/utils/compute_wer.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1760 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/config_argparse.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1830 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/get_default_kwargs.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     5632 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/griffin_lim.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4001 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/job_runner.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1607 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/misc.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1357 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/modelscope_param.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3598 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/nested_dict_action.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7735 2023-04-06 02:32:27.000000 funasr-0.4.2/funasr/utils/postprocess_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2027 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/sized_dict.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    13178 2023-03-22 05:51:29.000000 funasr-0.4.2/funasr/utils/timestamp_tools.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4185 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/types.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    11759 2023-03-16 11:52:36.000000 funasr-0.4.2/funasr/utils/wav_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      380 2023-02-24 12:39:00.000000 funasr-0.4.2/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        6 2023-04-21 11:13:25.000000 funasr-0.4.2/funasr/version.txt
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr.egg-info/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7855 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr.egg-info/PKG-INFO
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    13837 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr.egg-info/SOURCES.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr.egg-info/dependency_links.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      857 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr.egg-info/requires.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        7 2023-04-21 11:15:55.000000 funasr-0.4.2/funasr.egg-info/top_level.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       38 2023-04-21 11:15:55.000000 funasr-0.4.2/setup.cfg
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     4571 2023-04-17 02:17:43.000000 funasr-0.4.2/setup.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:15:55.000000 funasr-0.4.2/test/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      494 2023-03-31 07:25:30.000000 funasr-0.4.2/test/test_moddelscope_punc.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1028 2023-03-31 07:26:37.000000 funasr-0.4.2/test/test_moddelscope_punc_online.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      411 2023-04-18 14:25:37.000000 funasr-0.4.2/test/test_modelscope_paraformer_large.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      537 2023-03-31 14:17:23.000000 funasr-0.4.2/test/test_modelscope_paraformer_long.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      825 2023-04-18 13:29:54.000000 funasr-0.4.2/test/test_modelscope_pipeline.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1399 2023-03-31 14:15:12.000000 funasr-0.4.2/test/test_modelscope_vad.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2514 2023-04-13 11:54:40.000000 funasr-0.4.2/test/test_onnx_encoder.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1773 2023-03-13 12:16:53.000000 funasr-0.4.2/test/test_rtf.py
```

### Comparing `funasr-0.4.1/LICENSE` & `funasr-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/PKG-INFO` & `funasr-0.4.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,414 +1,426 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6675 6e61  : 2.1.Name: funa
-00000020: 7372 0a56 6572 7369 6f6e 3a20 302e 342e  sr.Version: 0.4.
-00000030: 310a 5375 6d6d 6172 793a 2046 756e 4153  1.Summary: FunAS
-00000040: 523a 2041 2046 756e 6461 6d65 6e74 616c  R: A Fundamental
-00000050: 2045 6e64 2d74 6f2d 456e 6420 5370 6565   End-to-End Spee
-00000060: 6368 2052 6563 6f67 6e69 7469 6f6e 2054  ch Recognition T
-00000070: 6f6f 6c6b 6974 0a48 6f6d 652d 7061 6765  oolkit.Home-page
-00000080: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-00000090: 2e63 6f6d 2f61 6c69 6261 6261 2d64 616d  .com/alibaba-dam
-000000a0: 6f2d 6163 6164 656d 792f 4675 6e41 5352  o-academy/FunASR
-000000b0: 2e67 6974 0a41 7574 686f 723a 2053 7065  .git.Author: Spe
-000000c0: 6563 6820 4c61 622c 2041 6c69 6261 6261  ech Lab, Alibaba
-000000d0: 2047 726f 7570 2c20 4368 696e 610a 4175   Group, China.Au
-000000e0: 7468 6f72 2d65 6d61 696c 3a20 6675 6e61  thor-email: funa
-000000f0: 7372 406c 6973 742e 616c 6962 6162 612d  sr@list.alibaba-
-00000100: 696e 632e 636f 6d0a 4c69 6365 6e73 653a  inc.com.License:
-00000110: 2054 6865 204d 4954 204c 6963 656e 7365   The MIT License
-00000120: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000130: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000140: 6520 3a3a 2050 7974 686f 6e0a 436c 6173  e :: Python.Clas
-00000150: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000160: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000170: 5079 7468 6f6e 203a 3a20 330a 436c 6173  Python :: 3.Clas
-00000180: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000190: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000001a0: 5079 7468 6f6e 203a 3a20 332e 370a 436c  Python :: 3.7.Cl
-000001b0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000001c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001d0: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
-000001e0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-000001f0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000200: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000210: 390a 436c 6173 7369 6669 6572 3a20 4465  9.Classifier: De
-00000220: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-00000230: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
-00000240: 6f6e 2f53 7461 626c 650a 436c 6173 7369  on/Stable.Classi
-00000250: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
-00000260: 7564 6965 6e63 6520 3a3a 2053 6369 656e  udience :: Scien
-00000270: 6365 2f52 6573 6561 7263 680a 436c 6173  ce/Research.Clas
-00000280: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
-00000290: 6720 5379 7374 656d 203a 3a20 504f 5349  g System :: POSI
-000002a0: 5820 3a3a 204c 696e 7578 0a43 6c61 7373  X :: Linux.Class
-000002b0: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-000002c0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-000002d0: 3a20 4170 6163 6865 2053 6f66 7477 6172  : Apache Softwar
-000002e0: 6520 4c69 6365 6e73 650a 436c 6173 7369  e License.Classi
-000002f0: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
-00000300: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
-00000310: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
-00000320: 203a 3a20 5079 7468 6f6e 204d 6f64 756c   :: Python Modul
-00000330: 6573 0a52 6571 7569 7265 732d 5079 7468  es.Requires-Pyth
-00000340: 6f6e 3a20 3e3d 332e 372e 300a 4465 7363  on: >=3.7.0.Desc
-00000350: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-00000360: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-00000370: 6f77 6e0a 5072 6f76 6964 6573 2d45 7874  own.Provides-Ext
-00000380: 7261 3a20 7472 6169 6e0a 5072 6f76 6964  ra: train.Provid
-00000390: 6573 2d45 7874 7261 3a20 7265 6369 7065  es-Extra: recipe
-000003a0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-000003b0: 2061 6c6c 0a50 726f 7669 6465 732d 4578   all.Provides-Ex
-000003c0: 7472 613a 2074 6573 740a 5072 6f76 6964  tra: test.Provid
-000003d0: 6573 2d45 7874 7261 3a20 646f 630a 4c69  es-Extra: doc.Li
-000003e0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-000003f0: 4e53 450a 0a5b 2f2f 5d3a 2023 2028 3c64  NSE..[//]: # (<d
-00000400: 6976 2061 6c69 676e 3d22 6c65 6674 223e  iv align="left">
-00000410: 3c69 6d67 2073 7263 3d22 646f 6373 2f69  <img src="docs/i
-00000420: 6d61 6765 732f 6675 6e61 7372 5f6c 6f67  mages/funasr_log
-00000430: 6f2e 6a70 6722 2077 6964 7468 3d22 3430  o.jpg" width="40
-00000440: 3022 2f3e 3c2f 6469 763e 290a 0a23 2046  0"/></div>)..# F
-00000450: 756e 4153 523a 2041 2046 756e 6461 6d65  unASR: A Fundame
-00000460: 6e74 616c 2045 6e64 2d74 6f2d 456e 6420  ntal End-to-End 
-00000470: 5370 6565 6368 2052 6563 6f67 6e69 7469  Speech Recogniti
-00000480: 6f6e 2054 6f6f 6c6b 6974 0a0a 3c73 7472  on Toolkit..<str
-00000490: 6f6e 673e 4675 6e41 5352 3c2f 7374 726f  ong>FunASR</stro
-000004a0: 6e67 3e20 686f 7065 7320 746f 2062 7569  ng> hopes to bui
-000004b0: 6c64 2061 2062 7269 6467 6520 6265 7477  ld a bridge betw
-000004c0: 6565 6e20 6163 6164 656d 6963 2072 6573  een academic res
-000004d0: 6561 7263 6820 616e 6420 696e 6475 7374  earch and indust
-000004e0: 7269 616c 2061 7070 6c69 6361 7469 6f6e  rial application
-000004f0: 7320 6f6e 2073 7065 6563 6820 7265 636f  s on speech reco
-00000500: 676e 6974 696f 6e2e 2042 7920 7375 7070  gnition. By supp
-00000510: 6f72 7469 6e67 2074 6865 2074 7261 696e  orting the train
-00000520: 696e 6720 2620 6669 6e65 7475 6e69 6e67  ing & finetuning
-00000530: 206f 6620 7468 6520 696e 6475 7374 7269   of the industri
-00000540: 616c 2d67 7261 6465 2073 7065 6563 6820  al-grade speech 
-00000550: 7265 636f 676e 6974 696f 6e20 6d6f 6465  recognition mode
-00000560: 6c20 7265 6c65 6173 6564 206f 6e20 5b4d  l released on [M
-00000570: 6f64 656c 5363 6f70 655d 2868 7474 7073  odelScope](https
-00000580: 3a2f 2f77 7777 2e6d 6f64 656c 7363 6f70  ://www.modelscop
-00000590: 652e 636e 2f6d 6f64 656c 733f 7061 6765  e.cn/models?page
-000005a0: 3d31 2674 6173 6b73 3d61 7574 6f2d 7370  =1&tasks=auto-sp
-000005b0: 6565 6368 2d72 6563 6f67 6e69 7469 6f6e  eech-recognition
-000005c0: 292c 2072 6573 6561 7263 6865 7273 2061  ), researchers a
-000005d0: 6e64 2064 6576 656c 6f70 6572 7320 6361  nd developers ca
-000005e0: 6e20 636f 6e64 7563 7420 7265 7365 6172  n conduct resear
-000005f0: 6368 2061 6e64 2070 726f 6475 6374 696f  ch and productio
-00000600: 6e20 6f66 2073 7065 6563 6820 7265 636f  n of speech reco
-00000610: 676e 6974 696f 6e20 6d6f 6465 6c73 206d  gnition models m
-00000620: 6f72 6520 636f 6e76 656e 6965 6e74 6c79  ore conveniently
-00000630: 2c20 616e 6420 7072 6f6d 6f74 6520 7468  , and promote th
-00000640: 6520 6465 7665 6c6f 706d 656e 7420 6f66  e development of
-00000650: 2073 7065 6563 6820 7265 636f 676e 6974   speech recognit
-00000660: 696f 6e20 6563 6f6c 6f67 792e 2041 5352  ion ecology. ASR
-00000670: 2066 6f72 2046 756e efbc 810a 0a5b 2a2a   for Fun.....[**
-00000680: 4e65 7773 2a2a 5d28 6874 7470 733a 2f2f  News**](https://
-00000690: 6769 7468 7562 2e63 6f6d 2f61 6c69 6261  github.com/aliba
-000006a0: 6261 2d64 616d 6f2d 6163 6164 656d 792f  ba-damo-academy/
-000006b0: 4675 6e41 5352 2377 6861 7473 2d6e 6577  FunASR#whats-new
-000006c0: 2920 0a7c 205b 2a2a 4869 6768 6c69 6768  ) .| [**Highligh
-000006d0: 7473 2a2a 5d28 2368 6967 686c 6967 6874  ts**](#highlight
-000006e0: 7329 0a7c 205b 2a2a 496e 7374 616c 6c61  s).| [**Installa
-000006f0: 7469 6f6e 2a2a 5d28 2369 6e73 7461 6c6c  tion**](#install
-00000700: 6174 696f 6e29 0a7c 205b 2a2a 446f 6373  ation).| [**Docs
-00000710: 5f45 4e2a 2a5d 2868 7474 7073 3a2f 2f61  _EN**](https://a
-00000720: 6c69 6261 6261 2d64 616d 6f2d 6163 6164  libaba-damo-acad
-00000730: 656d 792e 6769 7468 7562 2e69 6f2f 4675  emy.github.io/Fu
-00000740: 6e41 5352 2f65 6e2f 696e 6465 782e 6874  nASR/en/index.ht
-00000750: 6d6c 290a 7c20 5b2a 2a54 7574 6f72 6961  ml).| [**Tutoria
-00000760: 6c2a 2a5d 2868 7474 7073 3a2f 2f67 6974  l**](https://git
-00000770: 6875 622e 636f 6d2f 616c 6962 6162 612d  hub.com/alibaba-
-00000780: 6461 6d6f 2d61 6361 6465 6d79 2f46 756e  damo-academy/Fun
-00000790: 4153 522f 7769 6b69 2366 756e 6173 7225  ASR/wiki#funasr%
-000007a0: 4537 2539 3425 4138 2545 3625 3838 2542  E7%94%A8%E6%88%B
-000007b0: 3725 4536 2538 3925 3842 2545 3525 3836  7%E6%89%8B%E5%86
-000007c0: 2538 4329 0a7c 205b 2a2a 5061 7065 7273  %8C).| [**Papers
-000007d0: 2a2a 5d28 6874 7470 733a 2f2f 6769 7468  **](https://gith
-000007e0: 7562 2e63 6f6d 2f61 6c69 6261 6261 2d64  ub.com/alibaba-d
-000007f0: 616d 6f2d 6163 6164 656d 792f 4675 6e41  amo-academy/FunA
-00000800: 5352 2363 6974 6174 696f 6e73 290a 7c20  SR#citations).| 
-00000810: 5b2a 2a52 756e 7469 6d65 2a2a 5d28 6874  [**Runtime**](ht
-00000820: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000830: 2f61 6c69 6261 6261 2d64 616d 6f2d 6163  /alibaba-damo-ac
-00000840: 6164 656d 792f 4675 6e41 5352 2f74 7265  ademy/FunASR/tre
-00000850: 652f 6d61 696e 2f66 756e 6173 722f 7275  e/main/funasr/ru
-00000860: 6e74 696d 6529 0a7c 205b 2a2a 4d6f 6465  ntime).| [**Mode
-00000870: 6c20 5a6f 6f2a 2a5d 2868 7474 7073 3a2f  l Zoo**](https:/
-00000880: 2f67 6974 6875 622e 636f 6d2f 616c 6962  /github.com/alib
-00000890: 6162 612d 6461 6d6f 2d61 6361 6465 6d79  aba-damo-academy
-000008a0: 2f46 756e 4153 522f 626c 6f62 2f6d 6169  /FunASR/blob/mai
-000008b0: 6e2f 646f 6373 2f6d 6f64 656c 7363 6f70  n/docs/modelscop
-000008c0: 655f 6d6f 6465 6c73 2e6d 6429 0a7c 205b  e_models.md).| [
-000008d0: 2a2a 436f 6e74 6163 742a 2a5d 2823 636f  **Contact**](#co
-000008e0: 6e74 6163 7429 0a0a 0a23 2320 5768 6174  ntact)...## What
-000008f0: 2773 206e 6577 3a20 0a0a 466f 7220 7468  's new: ..For th
-00000900: 6520 7265 6c65 6173 6520 6e6f 7465 732c  e release notes,
-00000910: 2070 6c65 6173 6520 7265 6620 746f 205b   please ref to [
-00000920: 6e65 7773 5d28 6874 7470 733a 2f2f 6769  news](https://gi
-00000930: 7468 7562 2e63 6f6d 2f61 6c69 6261 6261  thub.com/alibaba
-00000940: 2d64 616d 6f2d 6163 6164 656d 792f 4675  -damo-academy/Fu
-00000950: 6e41 5352 2f72 656c 6561 7365 7329 0a0a  nASR/releases)..
-00000960: 2323 2048 6967 686c 6967 6874 730a 2d20  ## Highlights.- 
-00000970: 4d61 6e79 2074 7970 6573 206f 6620 7479  Many types of ty
-00000980: 7069 6361 6c20 6d6f 6465 6c73 2061 7265  pical models are
-00000990: 2073 7570 706f 7274 6564 2c20 652e 672e   supported, e.g.
-000009a0: 2c20 5b54 7261 6e66 6f72 6d65 725d 2868  , [Tranformer](h
-000009b0: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-000009c0: 2f61 6273 2f31 3730 362e 3033 3736 3229  /abs/1706.03762)
-000009d0: 2c20 5b43 6f6e 666f 726d 6572 5d28 6874  , [Conformer](ht
-000009e0: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-000009f0: 6162 732f 3230 3035 2e30 3831 3030 292c  abs/2005.08100),
-00000a00: 205b 5061 7261 666f 726d 6572 5d28 6874   [Paraformer](ht
-00000a10: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-00000a20: 6162 732f 3232 3036 2e30 3833 3137 292e  abs/2206.08317).
-00000a30: 0a2d 2057 6520 6861 7665 2072 656c 6561  .- We have relea
-00000a40: 7365 6420 6c61 7267 6520 6e75 6d62 6572  sed large number
-00000a50: 206f 6620 6163 6164 656d 6963 2061 6e64   of academic and
-00000a60: 2069 6e64 7573 7472 6961 6c20 7072 6574   industrial pret
-00000a70: 7261 696e 6564 206d 6f64 656c 7320 6f6e  rained models on
-00000a80: 205b 4d6f 6465 6c53 636f 7065 5d28 6874   [ModelScope](ht
-00000a90: 7470 733a 2f2f 7777 772e 6d6f 6465 6c73  tps://www.models
-00000aa0: 636f 7065 2e63 6e2f 6d6f 6465 6c73 3f70  cope.cn/models?p
-00000ab0: 6167 653d 3126 7461 736b 733d 6175 746f  age=1&tasks=auto
-00000ac0: 2d73 7065 6563 682d 7265 636f 676e 6974  -speech-recognit
-00000ad0: 696f 6e29 0a2d 2054 6865 2070 7265 7472  ion).- The pretr
-00000ae0: 6169 6e65 6420 6d6f 6465 6c20 5b50 6172  ained model [Par
-00000af0: 6166 6f72 6d65 722d 6c61 7267 655d 2868  aformer-large](h
-00000b00: 7474 7073 3a2f 2f77 7777 2e6d 6f64 656c  ttps://www.model
-00000b10: 7363 6f70 652e 636e 2f6d 6f64 656c 732f  scope.cn/models/
-00000b20: 6461 6d6f 2f73 7065 6563 685f 7061 7261  damo/speech_para
-00000b30: 666f 726d 6572 2d6c 6172 6765 5f61 7372  former-large_asr
-00000b40: 5f6e 6174 2d7a 682d 636e 2d31 366b 2d63  _nat-zh-cn-16k-c
-00000b50: 6f6d 6d6f 6e2d 766f 6361 6238 3430 342d  ommon-vocab8404-
-00000b60: 7079 746f 7263 682f 7375 6d6d 6172 7929  pytorch/summary)
-00000b70: 206f 6274 6169 6e73 2074 6865 2062 6573   obtains the bes
-00000b80: 7420 7065 7266 6f72 6d61 6e63 6520 6f6e  t performance on
-00000b90: 206d 616e 7920 7461 736b 7320 696e 205b   many tasks in [
-00000ba0: 5370 6565 6368 494f 206c 6561 6465 7262  SpeechIO leaderb
-00000bb0: 6f61 7264 5d28 6874 7470 733a 2f2f 6769  oard](https://gi
-00000bc0: 7468 7562 2e63 6f6d 2f53 7065 6563 6843  thub.com/SpeechC
-00000bd0: 6f6c 6162 2f4c 6561 6465 7262 6f61 7264  olab/Leaderboard
-00000be0: 290a 2d20 4675 6e41 5352 2073 7570 706c  ).- FunASR suppl
-00000bf0: 6965 7320 6120 6561 7379 2d74 6f2d 7573  ies a easy-to-us
-00000c00: 6520 7069 7065 6c69 6e65 2074 6f20 6669  e pipeline to fi
-00000c10: 6e65 7475 6e65 2070 7265 7472 6169 6e65  netune pretraine
-00000c20: 6420 6d6f 6465 6c73 2066 726f 6d20 5b4d  d models from [M
-00000c30: 6f64 656c 5363 6f70 655d 2868 7474 7073  odelScope](https
-00000c40: 3a2f 2f77 7777 2e6d 6f64 656c 7363 6f70  ://www.modelscop
-00000c50: 652e 636e 2f6d 6f64 656c 733f 7061 6765  e.cn/models?page
-00000c60: 3d31 2674 6173 6b73 3d61 7574 6f2d 7370  =1&tasks=auto-sp
-00000c70: 6565 6368 2d72 6563 6f67 6e69 7469 6f6e  eech-recognition
-00000c80: 290a 2d20 436f 6d70 6172 6564 2074 6f20  ).- Compared to 
-00000c90: 5b45 7370 6e65 745d 2868 7474 7073 3a2f  [Espnet](https:/
-00000ca0: 2f67 6974 6875 622e 636f 6d2f 6573 706e  /github.com/espn
-00000cb0: 6574 2f65 7370 6e65 7429 2066 7261 6d65  et/espnet) frame
-00000cc0: 776f 726b 2c20 7468 6520 7472 6169 6e69  work, the traini
-00000cd0: 6e67 2073 7065 6564 206f 6620 6c61 7267  ng speed of larg
-00000ce0: 652d 7363 616c 6520 6461 7461 7365 7473  e-scale datasets
-00000cf0: 2069 6e20 4675 6e41 5352 2069 7320 6d75   in FunASR is mu
-00000d00: 6368 2066 6173 7465 7220 6f77 6e69 6e67  ch faster owning
-00000d10: 2074 6f20 7468 6520 6f70 7469 6d69 7a65   to the optimize
-00000d20: 6420 6461 7461 6c6f 6164 6572 2e0a 0a23  d dataloader...#
-00000d30: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
-00000d40: 496e 7374 616c 6c20 6672 6f6d 2070 6970  Install from pip
-00000d50: 0a60 6060 7368 656c 6c0a 7069 7020 696e  .```shell.pip in
-00000d60: 7374 616c 6c20 2d55 2066 756e 6173 7220  stall -U funasr 
-00000d70: 2d69 2068 7474 7073 3a2f 2f70 7970 692e  -i https://pypi.
-00000d80: 5079 7468 6f6e 2e6f 7267 2f73 696d 706c  Python.org/simpl
-00000d90: 650a 6060 600a 0a4f 7220 696e 7374 616c  e.```..Or instal
-00000da0: 6c20 6672 6f6d 2073 6f75 7263 6520 636f  l from source co
-00000db0: 6465 0a0a 0a60 6060 2073 680a 6769 7420  de...``` sh.git 
-00000dc0: 636c 6f6e 6520 6874 7470 733a 2f2f 6769  clone https://gi
-00000dd0: 7468 7562 2e63 6f6d 2f61 6c69 6261 6261  thub.com/alibaba
-00000de0: 2f46 756e 4153 522e 6769 7420 2626 2063  /FunASR.git && c
-00000df0: 6420 4675 6e41 5352 0a70 6970 2069 6e73  d FunASR.pip ins
-00000e00: 7461 6c6c 202d 6520 2e2f 0a60 6060 0a49  tall -e ./.```.I
-00000e10: 6620 796f 7520 7761 6e74 2074 6f20 7573  f you want to us
-00000e20: 6520 7468 6520 7072 6574 7261 696e 6564  e the pretrained
-00000e30: 206d 6f64 656c 7320 696e 204d 6f64 656c   models in Model
-00000e40: 5363 6f70 652c 2079 6f75 2073 686f 756c  Scope, you shoul
-00000e50: 6420 696e 7374 616c 6c20 7468 6520 6d6f  d install the mo
-00000e60: 6465 6c73 636f 7065 3a0a 0a60 6060 7368  delscope:..```sh
-00000e70: 656c 6c0a 7069 7020 696e 7374 616c 6c20  ell.pip install 
-00000e80: 2d55 206d 6f64 656c 7363 6f70 650a 2320  -U modelscope.# 
-00000e90: 466f 7220 7468 6520 7573 6572 7320 696e  For the users in
-00000ea0: 2043 6869 6e61 2c20 796f 7520 636f 756c   China, you coul
-00000eb0: 6420 696e 7374 616c 6c20 7769 7468 2074  d install with t
-00000ec0: 6865 2063 6f6d 6d61 6e64 3a0a 2320 7069  he command:.# pi
-00000ed0: 7020 696e 7374 616c 6c20 2d55 206d 6f64  p install -U mod
-00000ee0: 656c 7363 6f70 6520 2d66 2068 7474 7073  elscope -f https
-00000ef0: 3a2f 2f6d 6f64 656c 7363 6f70 652e 6f73  ://modelscope.os
-00000f00: 732d 636e 2d62 6569 6a69 6e67 2e61 6c69  s-cn-beijing.ali
-00000f10: 7975 6e63 732e 636f 6d2f 7265 6c65 6173  yuncs.com/releas
-00000f20: 6573 2f72 6570 6f2e 6874 6d6c 202d 6920  es/repo.html -i 
-00000f30: 6874 7470 733a 2f2f 6d69 7272 6f72 2e73  https://mirror.s
-00000f40: 6a74 752e 6564 752e 636e 2f70 7970 692f  jtu.edu.cn/pypi/
-00000f50: 7765 622f 7369 6d70 6c65 0a60 6060 0a0a  web/simple.```..
-00000f60: 466f 7220 6d6f 7265 2064 6574 6169 6c73  For more details
-00000f70: 2c20 706c 6561 7365 2072 6566 2074 6f20  , please ref to 
-00000f80: 5b69 6e73 7461 6c6c 6174 696f 6e5d 2868  [installation](h
-00000f90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000fa0: 6d2f 616c 6962 6162 612d 6461 6d6f 2d61  m/alibaba-damo-a
-00000fb0: 6361 6465 6d79 2f46 756e 4153 522f 7769  cademy/FunASR/wi
-00000fc0: 6b69 290a 0a23 2320 5573 6167 650a 466f  ki)..## Usage.Fo
-00000fd0: 7220 7573 6572 7320 7768 6f20 6172 6520  r users who are 
-00000fe0: 6e65 7720 746f 2046 756e 4153 5220 616e  new to FunASR an
-00000ff0: 6420 4d6f 6465 6c53 636f 7065 2c20 706c  d ModelScope, pl
-00001000: 6561 7365 2072 6566 6572 2074 6f20 4675  ease refer to Fu
-00001010: 6e41 5352 2044 6f63 7328 5b43 4e5d 2868  nASR Docs([CN](h
-00001020: 7474 7073 3a2f 2f61 6c69 6261 6261 2d64  ttps://alibaba-d
-00001030: 616d 6f2d 6163 6164 656d 792e 6769 7468  amo-academy.gith
-00001040: 7562 2e69 6f2f 4675 6e41 5352 2f63 6e2f  ub.io/FunASR/cn/
-00001050: 696e 6465 782e 6874 6d6c 2920 2f20 5b45  index.html) / [E
-00001060: 4e5d 2868 7474 7073 3a2f 2f61 6c69 6261  N](https://aliba
-00001070: 6261 2d64 616d 6f2d 6163 6164 656d 792e  ba-damo-academy.
-00001080: 6769 7468 7562 2e69 6f2f 4675 6e41 5352  github.io/FunASR
-00001090: 2f65 6e2f 696e 6465 782e 6874 6d6c 2929  /en/index.html))
-000010a0: 0a0a 2323 2043 6f6e 7461 6374 0a0a 4966  ..## Contact..If
-000010b0: 2079 6f75 2068 6176 6520 616e 7920 7175   you have any qu
-000010c0: 6573 7469 6f6e 7320 6162 6f75 7420 4675  estions about Fu
-000010d0: 6e41 5352 2c20 706c 6561 7365 2063 6f6e  nASR, please con
-000010e0: 7461 6374 2075 7320 6279 0a0a 2d20 656d  tact us by..- em
-000010f0: 6169 6c3a 205b 6675 6e61 7372 406c 6973  ail: [funasr@lis
-00001100: 742e 616c 6962 6162 612d 696e 632e 636f  t.alibaba-inc.co
-00001110: 6d5d 2866 756e 6173 7240 6c69 7374 2e61  m](funasr@list.a
-00001120: 6c69 6261 6261 2d69 6e63 2e63 6f6d 290a  libaba-inc.com).
-00001130: 0a7c 4469 6e67 6469 6e67 2067 726f 7570  .|Dingding group
-00001140: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00001150: 2020 2020 2020 2057 6563 6861 7420 6772         Wechat gr
-00001160: 6f75 7020 2020 2020 2020 2020 2020 2020  oup             
-00001170: 2020 2020 2020 2020 207c 0a7c 3a2d 2d2d           |.|:---
-00001180: 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :|:-------------
-00001190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000011a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000011b0: 2d2d 2d2d 2d2d 2d2d 3a7c 0a7c 3c64 6976  --------:|.|<div
-000011c0: 2061 6c69 676e 3d22 6c65 6674 223e 3c69   align="left"><i
-000011d0: 6d67 2073 7263 3d22 646f 6373 2f69 6d61  mg src="docs/ima
-000011e0: 6765 732f 6469 6e67 6469 6e67 2e6a 7067  ges/dingding.jpg
-000011f0: 2220 7769 6474 683d 2232 3530 222f 3e20  " width="250"/> 
-00001200: 7c20 3c69 6d67 2073 7263 3d22 646f 6373  | <img src="docs
-00001210: 2f69 6d61 6765 732f 7765 6368 6174 2e70  /images/wechat.p
-00001220: 6e67 2220 7769 6474 683d 2232 3332 222f  ng" width="232"/
-00001230: 3e3c 2f64 6976 3e20 7c0a 0a23 2320 436f  ></div> |..## Co
-00001240: 6e74 7269 6275 746f 7273 0a0a 7c20 3c64  ntributors..| <d
-00001250: 6976 2061 6c69 676e 3d22 6c65 6674 223e  iv align="left">
-00001260: 3c69 6d67 2073 7263 3d22 646f 6373 2f69  <img src="docs/i
-00001270: 6d61 6765 732f 6461 6d6f 2e70 6e67 2220  mages/damo.png" 
-00001280: 7769 6474 683d 2231 3830 222f 3e20 7c20  width="180"/> | 
-00001290: 3c64 6976 2061 6c69 676e 3d22 6c65 6674  <div align="left
-000012a0: 223e 3c69 6d67 2073 7263 3d22 646f 6373  "><img src="docs
-000012b0: 2f69 6d61 6765 732f 6e77 7075 2e70 6e67  /images/nwpu.png
-000012c0: 2220 7769 6474 683d 2232 3630 222f 3e20  " width="260"/> 
-000012d0: 7c20 3c69 6d67 2073 7263 3d22 646f 6373  | <img src="docs
-000012e0: 2f69 6d61 6765 732f 4465 6570 5363 6965  /images/DeepScie
-000012f0: 6e63 652e 706e 6722 2077 6964 7468 3d22  nce.png" width="
-00001300: 3230 3022 2f3e 203c 2f64 6976 3e20 7c0a  200"/> </div> |.
-00001310: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
-00001320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001350: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -:|:------------
-00001360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001390: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
-000013a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013d0: 2d3a 7c0a 0a23 2320 4163 6b6e 6f77 6c65  -:|..## Acknowle
-000013e0: 6467 650a 0a31 2e20 5765 2062 6f72 726f  dge..1. We borro
-000013f0: 7765 6420 6120 6c6f 7420 6f66 2063 6f64  wed a lot of cod
-00001400: 6520 6672 6f6d 205b 4b61 6c64 695d 2868  e from [Kaldi](h
-00001410: 7474 703a 2f2f 6b61 6c64 692d 6173 722e  ttp://kaldi-asr.
-00001420: 6f72 672f 2920 666f 7220 6461 7461 2070  org/) for data p
-00001430: 7265 7061 7261 7469 6f6e 2e0a 322e 2057  reparation..2. W
-00001440: 6520 626f 7272 6f77 6564 2061 206c 6f74  e borrowed a lot
-00001450: 206f 6620 636f 6465 2066 726f 6d20 5b45   of code from [E
-00001460: 5350 6e65 745d 2868 7474 7073 3a2f 2f67  SPnet](https://g
-00001470: 6974 6875 622e 636f 6d2f 6573 706e 6574  ithub.com/espnet
-00001480: 2f65 7370 6e65 7429 2e20 4675 6e41 5352  /espnet). FunASR
-00001490: 2066 6f6c 6c6f 7773 2075 7020 7468 6520   follows up the 
-000014a0: 7472 6169 6e69 6e67 2061 6e64 2066 696e  training and fin
-000014b0: 6574 756e 696e 6720 7069 7065 6c69 6e65  etuning pipeline
-000014c0: 7320 6f66 2045 5350 6e65 742e 0a33 2e20  s of ESPnet..3. 
-000014d0: 5765 2072 6566 6572 7265 6420 5b57 656e  We referred [Wen
-000014e0: 6574 5d28 6874 7470 733a 2f2f 6769 7468  et](https://gith
-000014f0: 7562 2e63 6f6d 2f77 656e 6574 2d65 3265  ub.com/wenet-e2e
-00001500: 2f77 656e 6574 2920 666f 7220 6275 696c  /wenet) for buil
-00001510: 6469 6e67 2064 6174 616c 6f61 6465 7220  ding dataloader 
-00001520: 666f 7220 6c61 7267 6520 7363 616c 6520  for large scale 
-00001530: 6461 7461 2074 7261 696e 696e 672e 0a34  data training..4
-00001540: 2e20 5765 2061 636b 6e6f 776c 6564 6765  . We acknowledge
-00001550: 205b 4465 6570 5363 6965 6e63 655d 2868   [DeepScience](h
-00001560: 7474 7073 3a2f 2f77 7777 2e64 6565 7073  ttps://www.deeps
-00001570: 6369 656e 6365 2e63 6e29 2066 6f72 2063  cience.cn) for c
-00001580: 6f6e 7472 6962 7574 696e 6720 7468 6520  ontributing the 
-00001590: 6772 7063 2073 6572 7669 6365 2e0a 0a23  grpc service...#
-000015a0: 2320 4c69 6365 6e73 650a 5468 6973 2070  # License.This p
-000015b0: 726f 6a65 6374 2069 7320 6c69 6365 6e73  roject is licens
-000015c0: 6564 2075 6e64 6572 2074 6865 205b 5468  ed under the [Th
-000015d0: 6520 4d49 5420 4c69 6365 6e73 655d 2868  e MIT License](h
-000015e0: 7474 7073 3a2f 2f6f 7065 6e73 6f75 7263  ttps://opensourc
-000015f0: 652e 6f72 672f 6c69 6365 6e73 6573 2f4d  e.org/licenses/M
-00001600: 4954 292e 2046 756e 4153 5220 616c 736f  IT). FunASR also
-00001610: 2063 6f6e 7461 696e 7320 7661 7269 6f75   contains variou
-00001620: 7320 7468 6972 642d 7061 7274 7920 636f  s third-party co
-00001630: 6d70 6f6e 656e 7473 2061 6e64 2073 6f6d  mponents and som
-00001640: 6520 636f 6465 206d 6f64 6966 6965 6420  e code modified 
-00001650: 6672 6f6d 206f 7468 6572 2072 6570 6f73  from other repos
-00001660: 2075 6e64 6572 206f 7468 6572 206f 7065   under other ope
-00001670: 6e20 736f 7572 6365 206c 6963 656e 7365  n source license
-00001680: 732e 0a0a 2323 2043 6974 6174 696f 6e73  s...## Citations
-00001690: 0a0a 6060 6020 6269 6274 6578 0a40 696e  ..``` bibtex.@in
-000016a0: 7072 6f63 6565 6469 6e67 737b 6761 6f32  proceedings{gao2
-000016b0: 3032 3075 6e69 7665 7273 616c 2c0a 2020  020universal,.  
-000016c0: 7469 746c 653d 7b55 6e69 7665 7273 616c  title={Universal
-000016d0: 2041 5352 3a20 556e 6966 7969 6e67 2053   ASR: Unifying S
-000016e0: 7472 6561 6d69 6e67 2061 6e64 204e 6f6e  treaming and Non
-000016f0: 2d53 7472 6561 6d69 6e67 2041 5352 2055  -Streaming ASR U
-00001700: 7369 6e67 2061 2053 696e 676c 6520 456e  sing a Single En
-00001710: 636f 6465 722d 4465 636f 6465 7220 4d6f  coder-Decoder Mo
-00001720: 6465 6c7d 2c0a 2020 6175 7468 6f72 3d7b  del},.  author={
-00001730: 4761 6f2c 205a 6869 6675 2061 6e64 205a  Gao, Zhifu and Z
-00001740: 6861 6e67 2c20 5368 696c 6961 6e67 2061  hang, Shiliang a
-00001750: 6e64 204c 6569 2c20 4d69 6e67 2061 6e64  nd Lei, Ming and
-00001760: 204d 634c 6f75 6768 6c69 6e2c 2049 616e   McLoughlin, Ian
-00001770: 7d2c 0a20 2062 6f6f 6b74 6974 6c65 3d7b  },.  booktitle={
-00001780: 6172 5869 7620 7072 6570 7269 6e74 2061  arXiv preprint a
-00001790: 7258 6976 3a32 3031 302e 3134 3039 397d  rXiv:2010.14099}
-000017a0: 2c0a 2020 7965 6172 3d7b 3230 3230 7d0a  ,.  year={2020}.
-000017b0: 7d0a 0a40 696e 7072 6f63 6565 6469 6e67  }..@inproceeding
-000017c0: 737b 6761 6f32 3032 3270 6172 6166 6f72  s{gao2022parafor
-000017d0: 6d65 722c 0a20 2074 6974 6c65 3d7b 5061  mer,.  title={Pa
-000017e0: 7261 666f 726d 6572 3a20 4661 7374 2061  raformer: Fast a
-000017f0: 6e64 2041 6363 7572 6174 6520 5061 7261  nd Accurate Para
-00001800: 6c6c 656c 2054 7261 6e73 666f 726d 6572  llel Transformer
-00001810: 2066 6f72 204e 6f6e 2d61 7574 6f72 6567   for Non-autoreg
-00001820: 7265 7373 6976 6520 456e 642d 746f 2d45  ressive End-to-E
-00001830: 6e64 2053 7065 6563 6820 5265 636f 676e  nd Speech Recogn
-00001840: 6974 696f 6e7d 2c0a 2020 6175 7468 6f72  ition},.  author
-00001850: 3d7b 4761 6f2c 205a 6869 6675 2061 6e64  ={Gao, Zhifu and
-00001860: 205a 6861 6e67 2c20 5368 696c 6961 6e67   Zhang, Shiliang
-00001870: 2061 6e64 204d 634c 6f75 6768 6c69 6e2c   and McLoughlin,
-00001880: 2049 616e 2061 6e64 2059 616e 2c20 5a68   Ian and Yan, Zh
-00001890: 696a 6965 7d2c 0a20 2062 6f6f 6b74 6974  ijie},.  booktit
-000018a0: 6c65 3d7b 494e 5445 5253 5045 4543 487d  le={INTERSPEECH}
-000018b0: 2c0a 2020 7965 6172 3d7b 3230 3232 7d0a  ,.  year={2022}.
-000018c0: 7d0a 4069 6e70 726f 6365 6564 696e 6773  }.@inproceedings
-000018d0: 7b53 6869 3230 3233 4163 6869 6576 696e  {Shi2023Achievin
-000018e0: 6754 502c 0a20 2074 6974 6c65 3d7b 4163  gTP,.  title={Ac
-000018f0: 6869 6576 696e 6720 5469 6d65 7374 616d  hieving Timestam
-00001900: 7020 5072 6564 6963 7469 6f6e 2057 6869  p Prediction Whi
-00001910: 6c65 2052 6563 6f67 6e69 7a69 6e67 2077  le Recognizing w
-00001920: 6974 6820 4e6f 6e2d 4175 746f 7265 6772  ith Non-Autoregr
-00001930: 6573 7369 7665 2045 6e64 2d74 6f2d 456e  essive End-to-En
-00001940: 6420 4153 5220 4d6f 6465 6c7d 2c0a 2020  d ASR Model},.  
-00001950: 6175 7468 6f72 3d7b 5869 616e 2053 6869  author={Xian Shi
-00001960: 2061 6e64 2059 616e 6e69 2043 6865 6e20   and Yanni Chen 
-00001970: 616e 6420 5368 696c 6961 6e67 205a 6861  and Shiliang Zha
-00001980: 6e67 2061 6e64 205a 6869 6a69 6520 5961  ng and Zhijie Ya
-00001990: 6e7d 2c0a 2020 626f 6f6b 7469 746c 653d  n},.  booktitle=
-000019a0: 7b61 7258 6976 2070 7265 7072 696e 7420  {arXiv preprint 
-000019b0: 6172 5869 763a 3233 3031 2e31 3233 3433  arXiv:2301.12343
-000019c0: 7d0a 2020 7965 6172 3d7b 3230 3233 7d0a  }.  year={2023}.
-000019d0: 7d0a 6060 600a                           }.```.
+00000000: 5b2f 2f5d 3a20 2320 283c 6469 7620 616c  [//]: # (<div al
+00000010: 6967 6e3d 226c 6566 7422 3e3c 696d 6720  ign="left"><img 
+00000020: 7372 633d 2264 6f63 732f 696d 6167 6573  src="docs/images
+00000030: 2f66 756e 6173 725f 6c6f 676f 2e6a 7067  /funasr_logo.jpg
+00000040: 2220 7769 6474 683d 2234 3030 222f 3e3c  " width="400"/><
+00000050: 2f64 6976 3e29 0a0a 2320 4675 6e41 5352  /div>)..# FunASR
+00000060: 3a20 4120 4675 6e64 616d 656e 7461 6c20  : A Fundamental 
+00000070: 456e 642d 746f 2d45 6e64 2053 7065 6563  End-to-End Speec
+00000080: 6820 5265 636f 676e 6974 696f 6e20 546f  h Recognition To
+00000090: 6f6c 6b69 740a 3c70 2061 6c69 676e 3d22  olkit.<p align="
+000000a0: 6c65 6674 223e 0a20 2020 203c 6120 6872  left">.    <a hr
+000000b0: 6566 3d22 223e 3c69 6d67 2073 7263 3d22  ef=""><img src="
+000000c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000000d0: 6c64 732e 696f 2f62 6164 6765 2f4f 532d  lds.io/badge/OS-
+000000e0: 4c69 6e75 7825 3243 2532 3057 696e 2532  Linux%2C%20Win%2
+000000f0: 4325 3230 4d61 632d 6272 6967 6874 6772  C%20Mac-brightgr
+00000100: 6565 6e2e 7376 6722 3e3c 2f61 3e0a 2020  een.svg"></a>.  
+00000110: 2020 3c61 2068 7265 663d 2222 3e3c 696d    <a href=""><im
+00000120: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000130: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000140: 6467 652f 5079 7468 6f6e 2d3e 3d33 2e37  dge/Python->=3.7
+00000150: 2c3c 3d33 2e31 302d 6166 662e 7376 6722  ,<=3.10-aff.svg"
+00000160: 3e3c 2f61 3e0a 2020 2020 3c61 2068 7265  ></a>.    <a hre
+00000170: 663d 2222 3e3c 696d 6720 7372 633d 2268  f=""><img src="h
+00000180: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000190: 6473 2e69 6f2f 6261 6467 652f 5079 746f  ds.io/badge/Pyto
+000001a0: 7263 682d 2533 4525 3344 312e 3131 2d62  rch-%3E%3D1.11-b
+000001b0: 6c75 6522 3e3c 2f61 3e0a 3c2f 703e 0a0a  lue"></a>.</p>..
+000001c0: 3c73 7472 6f6e 673e 4675 6e41 5352 3c2f  <strong>FunASR</
+000001d0: 7374 726f 6e67 3e20 686f 7065 7320 746f  strong> hopes to
+000001e0: 2062 7569 6c64 2061 2062 7269 6467 6520   build a bridge 
+000001f0: 6265 7477 6565 6e20 6163 6164 656d 6963  between academic
+00000200: 2072 6573 6561 7263 6820 616e 6420 696e   research and in
+00000210: 6475 7374 7269 616c 2061 7070 6c69 6361  dustrial applica
+00000220: 7469 6f6e 7320 6f6e 2073 7065 6563 6820  tions on speech 
+00000230: 7265 636f 676e 6974 696f 6e2e 2042 7920  recognition. By 
+00000240: 7375 7070 6f72 7469 6e67 2074 6865 2074  supporting the t
+00000250: 7261 696e 696e 6720 2620 6669 6e65 7475  raining & finetu
+00000260: 6e69 6e67 206f 6620 7468 6520 696e 6475  ning of the indu
+00000270: 7374 7269 616c 2d67 7261 6465 2073 7065  strial-grade spe
+00000280: 6563 6820 7265 636f 676e 6974 696f 6e20  ech recognition 
+00000290: 6d6f 6465 6c20 7265 6c65 6173 6564 206f  model released o
+000002a0: 6e20 5b4d 6f64 656c 5363 6f70 655d 2868  n [ModelScope](h
+000002b0: 7474 7073 3a2f 2f77 7777 2e6d 6f64 656c  ttps://www.model
+000002c0: 7363 6f70 652e 636e 2f6d 6f64 656c 733f  scope.cn/models?
+000002d0: 7061 6765 3d31 2674 6173 6b73 3d61 7574  page=1&tasks=aut
+000002e0: 6f2d 7370 6565 6368 2d72 6563 6f67 6e69  o-speech-recogni
+000002f0: 7469 6f6e 292c 2072 6573 6561 7263 6865  tion), researche
+00000300: 7273 2061 6e64 2064 6576 656c 6f70 6572  rs and developer
+00000310: 7320 6361 6e20 636f 6e64 7563 7420 7265  s can conduct re
+00000320: 7365 6172 6368 2061 6e64 2070 726f 6475  search and produ
+00000330: 6374 696f 6e20 6f66 2073 7065 6563 6820  ction of speech 
+00000340: 7265 636f 676e 6974 696f 6e20 6d6f 6465  recognition mode
+00000350: 6c73 206d 6f72 6520 636f 6e76 656e 6965  ls more convenie
+00000360: 6e74 6c79 2c20 616e 6420 7072 6f6d 6f74  ntly, and promot
+00000370: 6520 7468 6520 6465 7665 6c6f 706d 656e  e the developmen
+00000380: 7420 6f66 2073 7065 6563 6820 7265 636f  t of speech reco
+00000390: 676e 6974 696f 6e20 6563 6f6c 6f67 792e  gnition ecology.
+000003a0: 2041 5352 2066 6f72 2046 756e efbc 810a   ASR for Fun....
+000003b0: 0a5b 2a2a 4e65 7773 2a2a 5d28 6874 7470  .[**News**](http
+000003c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+000003d0: 6c69 6261 6261 2d64 616d 6f2d 6163 6164  libaba-damo-acad
+000003e0: 656d 792f 4675 6e41 5352 2377 6861 7473  emy/FunASR#whats
+000003f0: 2d6e 6577 2920 0a7c 205b 2a2a 4869 6768  -new) .| [**High
+00000400: 6c69 6768 7473 2a2a 5d28 2368 6967 686c  lights**](#highl
+00000410: 6967 6874 7329 0a7c 205b 2a2a 496e 7374  ights).| [**Inst
+00000420: 616c 6c61 7469 6f6e 2a2a 5d28 2369 6e73  allation**](#ins
+00000430: 7461 6c6c 6174 696f 6e29 0a7c 205b 2a2a  tallation).| [**
+00000440: 446f 6373 2a2a 5d28 6874 7470 733a 2f2f  Docs**](https://
+00000450: 616c 6962 6162 612d 6461 6d6f 2d61 6361  alibaba-damo-aca
+00000460: 6465 6d79 2e67 6974 6875 622e 696f 2f46  demy.github.io/F
+00000470: 756e 4153 522f 656e 2f69 6e64 6578 2e68  unASR/en/index.h
+00000480: 746d 6c29 0a7c 205b 2a2a 5475 746f 7269  tml).| [**Tutori
+00000490: 616c 2a2a 5d28 6874 7470 733a 2f2f 6769  al**](https://gi
+000004a0: 7468 7562 2e63 6f6d 2f61 6c69 6261 6261  thub.com/alibaba
+000004b0: 2d64 616d 6f2d 6163 6164 656d 792f 4675  -damo-academy/Fu
+000004c0: 6e41 5352 2f77 696b 6923 6675 6e61 7372  nASR/wiki#funasr
+000004d0: 2545 3725 3934 2541 3825 4536 2538 3825  %E7%94%A8%E6%88%
+000004e0: 4237 2545 3625 3839 2538 4225 4535 2538  B7%E6%89%8B%E5%8
+000004f0: 3625 3843 290a 7c20 5b2a 2a50 6170 6572  6%8C).| [**Paper
+00000500: 732a 2a5d 2868 7474 7073 3a2f 2f67 6974  s**](https://git
+00000510: 6875 622e 636f 6d2f 616c 6962 6162 612d  hub.com/alibaba-
+00000520: 6461 6d6f 2d61 6361 6465 6d79 2f46 756e  damo-academy/Fun
+00000530: 4153 5223 6369 7461 7469 6f6e 7329 0a7c  ASR#citations).|
+00000540: 205b 2a2a 5275 6e74 696d 652a 2a5d 2868   [**Runtime**](h
+00000550: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000560: 6d2f 616c 6962 6162 612d 6461 6d6f 2d61  m/alibaba-damo-a
+00000570: 6361 6465 6d79 2f46 756e 4153 522f 7472  cademy/FunASR/tr
+00000580: 6565 2f6d 6169 6e2f 6675 6e61 7372 2f72  ee/main/funasr/r
+00000590: 756e 7469 6d65 290a 7c20 5b2a 2a4d 6f64  untime).| [**Mod
+000005a0: 656c 205a 6f6f 2a2a 5d28 6874 7470 733a  el Zoo**](https:
+000005b0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6c69  //github.com/ali
+000005c0: 6261 6261 2d64 616d 6f2d 6163 6164 656d  baba-damo-academ
+000005d0: 792f 4675 6e41 5352 2f62 6c6f 622f 6d61  y/FunASR/blob/ma
+000005e0: 696e 2f64 6f63 732f 6d6f 6465 6c73 636f  in/docs/modelsco
+000005f0: 7065 5f6d 6f64 656c 732e 6d64 290a 7c20  pe_models.md).| 
+00000600: 5b2a 2a43 6f6e 7461 6374 2a2a 5d28 2363  [**Contact**](#c
+00000610: 6f6e 7461 6374 290a 7c0a 5b2a 2a4d 324d  ontact).|.[**M2M
+00000620: 4554 322e 3020 4775 6964 656e 6365 5f43  ET2.0 Guidence_C
+00000630: 4e2a 2a5d 2868 7474 7073 3a2f 2f61 6c69  N**](https://ali
+00000640: 6261 6261 2d64 616d 6f2d 6163 6164 656d  baba-damo-academ
+00000650: 792e 6769 7468 7562 2e69 6f2f 4675 6e41  y.github.io/FunA
+00000660: 5352 2f6d 326d 6574 325f 636e 2f69 6e64  SR/m2met2_cn/ind
+00000670: 6578 2e68 746d 6c29 0a7c 205b 2a2a 4d32  ex.html).| [**M2
+00000680: 4d45 5432 2e30 2047 7569 6465 6e63 655f  MET2.0 Guidence_
+00000690: 454e 2a2a 5d28 6874 7470 733a 2f2f 616c  EN**](https://al
+000006a0: 6962 6162 612d 6461 6d6f 2d61 6361 6465  ibaba-damo-acade
+000006b0: 6d79 2e67 6974 6875 622e 696f 2f46 756e  my.github.io/Fun
+000006c0: 4153 522f 6d32 6d65 7432 2f69 6e64 6578  ASR/m2met2/index
+000006d0: 2e68 746d 6c29 0a0a 2323 204d 756c 7469  .html)..## Multi
+000006e0: 2d43 6861 6e6e 656c 204d 756c 7469 2d50  -Channel Multi-P
+000006f0: 6172 7479 204d 6565 7469 6e67 2054 7261  arty Meeting Tra
+00000700: 6e73 6372 6970 7469 6f6e 2032 2e30 2028  nscription 2.0 (
+00000710: 4d32 4d45 5432 2e30 2920 4368 616c 6c65  M2MET2.0) Challe
+00000720: 6e67 650a 5765 2061 7265 2070 6c65 6173  nge.We are pleas
+00000730: 6564 2074 6f20 616e 6e6f 756e 6365 2074  ed to announce t
+00000740: 6861 7420 7468 6520 4d32 4d65 5432 2e30  hat the M2MeT2.0
+00000750: 2063 6861 6c6c 656e 6765 2077 696c 6c20   challenge will 
+00000760: 6265 2068 656c 6420 696e 2074 6865 206e  be held in the n
+00000770: 6561 7220 6675 7475 7265 2e20 5468 6520  ear future. The 
+00000780: 6261 7365 6c69 6e65 2073 7973 7465 6d20  baseline system 
+00000790: 6973 2063 6f6e 6475 6374 6564 206f 6e20  is conducted on 
+000007a0: 4675 6e41 5352 2061 6e64 2069 7320 7072  FunASR and is pr
+000007b0: 6f76 6964 6564 2061 7320 6120 7265 6365  ovided as a rece
+000007c0: 6970 6520 6f66 2041 6c69 4d65 6574 696e  ipe of AliMeetin
+000007d0: 6720 636f 7270 7573 2e20 466f 7220 6d6f  g corpus. For mo
+000007e0: 7265 2064 6574 6169 6c73 2079 6f75 2063  re details you c
+000007f0: 616e 2073 6565 2074 6865 2067 7569 6465  an see the guide
+00000800: 6e63 6520 6f66 204d 324d 4554 322e 3020  nce of M2MET2.0 
+00000810: 285b 434e 5d28 6874 7470 733a 2f2f 616c  ([CN](https://al
+00000820: 6962 6162 612d 6461 6d6f 2d61 6361 6465  ibaba-damo-acade
+00000830: 6d79 2e67 6974 6875 622e 696f 2f46 756e  my.github.io/Fun
+00000840: 4153 522f 6d32 6d65 7432 5f63 6e2f 696e  ASR/m2met2_cn/in
+00000850: 6465 782e 6874 6d6c 292f 5b45 4e5d 2868  dex.html)/[EN](h
+00000860: 7474 7073 3a2f 2f61 6c69 6261 6261 2d64  ttps://alibaba-d
+00000870: 616d 6f2d 6163 6164 656d 792e 6769 7468  amo-academy.gith
+00000880: 7562 2e69 6f2f 4675 6e41 5352 2f6d 326d  ub.io/FunASR/m2m
+00000890: 6574 322f 696e 6465 782e 6874 6d6c 2929  et2/index.html))
+000008a0: 2e0a 2323 2057 6861 7427 7320 6e65 773a  ..## What's new:
+000008b0: 200a 0a46 6f72 2074 6865 2072 656c 6561   ..For the relea
+000008c0: 7365 206e 6f74 6573 2c20 706c 6561 7365  se notes, please
+000008d0: 2072 6566 2074 6f20 5b6e 6577 735d 2868   ref to [news](h
+000008e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000008f0: 6d2f 616c 6962 6162 612d 6461 6d6f 2d61  m/alibaba-damo-a
+00000900: 6361 6465 6d79 2f46 756e 4153 522f 7265  cademy/FunASR/re
+00000910: 6c65 6173 6573 290a 0a23 2320 4869 6768  leases)..## High
+00000920: 6c69 6768 7473 0a2d 2046 756e 4153 5220  lights.- FunASR 
+00000930: 7375 7070 6f72 7473 2073 7065 6563 6820  supports speech 
+00000940: 7265 636f 676e 6974 696f 6e28 4153 5229  recognition(ASR)
+00000950: 2c20 4d75 6c74 692d 7461 6c6b 6572 2041  , Multi-talker A
+00000960: 5352 2c20 566f 6963 6520 4163 7469 7669  SR, Voice Activi
+00000970: 7479 2044 6574 6563 7469 6f6e 2856 4144  ty Detection(VAD
+00000980: 292c 2050 756e 6374 7561 7469 6f6e 2052  ), Punctuation R
+00000990: 6573 746f 7261 7469 6f6e 2c20 4c61 6e67  estoration, Lang
+000009a0: 7561 6765 204d 6f64 656c 732c 2053 7065  uage Models, Spe
+000009b0: 616b 6572 2056 6572 6966 6963 6174 696f  aker Verificatio
+000009c0: 6e20 616e 6420 5370 6561 6b65 7220 6469  n and Speaker di
+000009d0: 6172 697a 6174 696f 6e2e 2020 200a 2d20  arization.   .- 
+000009e0: 5765 2068 6176 6520 7265 6c65 6173 6564  We have released
+000009f0: 206c 6172 6765 206e 756d 6265 7220 6f66   large number of
+00000a00: 2061 6361 6465 6d69 6320 616e 6420 696e   academic and in
+00000a10: 6475 7374 7269 616c 2070 7265 7472 6169  dustrial pretrai
+00000a20: 6e65 6420 6d6f 6465 6c73 206f 6e20 5b4d  ned models on [M
+00000a30: 6f64 656c 5363 6f70 655d 2868 7474 7073  odelScope](https
+00000a40: 3a2f 2f77 7777 2e6d 6f64 656c 7363 6f70  ://www.modelscop
+00000a50: 652e 636e 2f6d 6f64 656c 733f 7061 6765  e.cn/models?page
+00000a60: 3d31 2674 6173 6b73 3d61 7574 6f2d 7370  =1&tasks=auto-sp
+00000a70: 6565 6368 2d72 6563 6f67 6e69 7469 6f6e  eech-recognition
+00000a80: 290a 2d20 5468 6520 7072 6574 7261 696e  ).- The pretrain
+00000a90: 6564 206d 6f64 656c 205b 5061 7261 666f  ed model [Parafo
+00000aa0: 726d 6572 2d6c 6172 6765 5d28 6874 7470  rmer-large](http
+00000ab0: 733a 2f2f 7777 772e 6d6f 6465 6c73 636f  s://www.modelsco
+00000ac0: 7065 2e63 6e2f 6d6f 6465 6c73 2f64 616d  pe.cn/models/dam
+00000ad0: 6f2f 7370 6565 6368 5f70 6172 6166 6f72  o/speech_parafor
+00000ae0: 6d65 722d 6c61 7267 655f 6173 725f 6e61  mer-large_asr_na
+00000af0: 742d 7a68 2d63 6e2d 3136 6b2d 636f 6d6d  t-zh-cn-16k-comm
+00000b00: 6f6e 2d76 6f63 6162 3834 3034 2d70 7974  on-vocab8404-pyt
+00000b10: 6f72 6368 2f73 756d 6d61 7279 2920 6f62  orch/summary) ob
+00000b20: 7461 696e 7320 7468 6520 6265 7374 2070  tains the best p
+00000b30: 6572 666f 726d 616e 6365 206f 6e20 6d61  erformance on ma
+00000b40: 6e79 2074 6173 6b73 2069 6e20 5b53 7065  ny tasks in [Spe
+00000b50: 6563 6849 4f20 6c65 6164 6572 626f 6172  echIO leaderboar
+00000b60: 645d 2868 7474 7073 3a2f 2f67 6974 6875  d](https://githu
+00000b70: 622e 636f 6d2f 5370 6565 6368 436f 6c61  b.com/SpeechCola
+00000b80: 622f 4c65 6164 6572 626f 6172 6429 0a2d  b/Leaderboard).-
+00000b90: 2046 756e 4153 5220 7375 7070 6c69 6573   FunASR supplies
+00000ba0: 2061 2065 6173 792d 746f 2d75 7365 2070   a easy-to-use p
+00000bb0: 6970 656c 696e 6520 746f 2066 696e 6574  ipeline to finet
+00000bc0: 756e 6520 7072 6574 7261 696e 6564 206d  une pretrained m
+00000bd0: 6f64 656c 7320 6672 6f6d 205b 4d6f 6465  odels from [Mode
+00000be0: 6c53 636f 7065 5d28 6874 7470 733a 2f2f  lScope](https://
+00000bf0: 7777 772e 6d6f 6465 6c73 636f 7065 2e63  www.modelscope.c
+00000c00: 6e2f 6d6f 6465 6c73 3f70 6167 653d 3126  n/models?page=1&
+00000c10: 7461 736b 733d 6175 746f 2d73 7065 6563  tasks=auto-speec
+00000c20: 682d 7265 636f 676e 6974 696f 6e29 0a2d  h-recognition).-
+00000c30: 2043 6f6d 7061 7265 6420 746f 205b 4573   Compared to [Es
+00000c40: 706e 6574 5d28 6874 7470 733a 2f2f 6769  pnet](https://gi
+00000c50: 7468 7562 2e63 6f6d 2f65 7370 6e65 742f  thub.com/espnet/
+00000c60: 6573 706e 6574 2920 6672 616d 6577 6f72  espnet) framewor
+00000c70: 6b2c 2074 6865 2074 7261 696e 696e 6720  k, the training 
+00000c80: 7370 6565 6420 6f66 206c 6172 6765 2d73  speed of large-s
+00000c90: 6361 6c65 2064 6174 6173 6574 7320 696e  cale datasets in
+00000ca0: 2046 756e 4153 5220 6973 206d 7563 6820   FunASR is much 
+00000cb0: 6661 7374 6572 206f 776e 696e 6720 746f  faster owning to
+00000cc0: 2074 6865 206f 7074 696d 697a 6564 2064   the optimized d
+00000cd0: 6174 616c 6f61 6465 722e 0a0a 2323 2049  ataloader...## I
+00000ce0: 6e73 7461 6c6c 6174 696f 6e0a 0a49 6e73  nstallation..Ins
+00000cf0: 7461 6c6c 2066 726f 6d20 7069 700a 6060  tall from pip.``
+00000d00: 6073 6865 6c6c 0a70 6970 2069 6e73 7461  `shell.pip insta
+00000d10: 6c6c 202d 5520 6675 6e61 7372 0a23 2046  ll -U funasr.# F
+00000d20: 6f72 2074 6865 2075 7365 7273 2069 6e20  or the users in 
+00000d30: 4368 696e 612c 2079 6f75 2063 6f75 6c64  China, you could
+00000d40: 2069 6e73 7461 6c6c 2077 6974 6820 7468   install with th
+00000d50: 6520 636f 6d6d 616e 643a 0a23 2070 6970  e command:.# pip
+00000d60: 2069 6e73 7461 6c6c 202d 5520 6675 6e61   install -U funa
+00000d70: 7372 202d 6920 6874 7470 733a 2f2f 6d69  sr -i https://mi
+00000d80: 7272 6f72 2e73 6a74 752e 6564 752e 636e  rror.sjtu.edu.cn
+00000d90: 2f70 7970 692f 7765 622f 7369 6d70 6c65  /pypi/web/simple
+00000da0: 0a60 6060 0a0a 4f72 2069 6e73 7461 6c6c  .```..Or install
+00000db0: 2066 726f 6d20 736f 7572 6365 2063 6f64   from source cod
+00000dc0: 650a 0a0a 6060 6020 7368 0a67 6974 2063  e...``` sh.git c
+00000dd0: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+00000de0: 6875 622e 636f 6d2f 616c 6962 6162 612f  hub.com/alibaba/
+00000df0: 4675 6e41 5352 2e67 6974 2026 2620 6364  FunASR.git && cd
+00000e00: 2046 756e 4153 520a 7069 7020 696e 7374   FunASR.pip inst
+00000e10: 616c 6c20 2d65 202e 2f0a 2320 466f 7220  all -e ./.# For 
+00000e20: 7468 6520 7573 6572 7320 696e 2043 6869  the users in Chi
+00000e30: 6e61 2c20 796f 7520 636f 756c 6420 696e  na, you could in
+00000e40: 7374 616c 6c20 7769 7468 2074 6865 2063  stall with the c
+00000e50: 6f6d 6d61 6e64 3a0a 2320 7069 7020 696e  ommand:.# pip in
+00000e60: 7374 616c 6c20 2d65 202e 2f20 2d69 2068  stall -e ./ -i h
+00000e70: 7474 7073 3a2f 2f6d 6972 726f 722e 736a  ttps://mirror.sj
+00000e80: 7475 2e65 6475 2e63 6e2f 7079 7069 2f77  tu.edu.cn/pypi/w
+00000e90: 6562 2f73 696d 706c 650a 0a60 6060 0a49  eb/simple..```.I
+00000ea0: 6620 796f 7520 7761 6e74 2074 6f20 7573  f you want to us
+00000eb0: 6520 7468 6520 7072 6574 7261 696e 6564  e the pretrained
+00000ec0: 206d 6f64 656c 7320 696e 204d 6f64 656c   models in Model
+00000ed0: 5363 6f70 652c 2079 6f75 2073 686f 756c  Scope, you shoul
+00000ee0: 6420 696e 7374 616c 6c20 7468 6520 6d6f  d install the mo
+00000ef0: 6465 6c73 636f 7065 3a0a 0a60 6060 7368  delscope:..```sh
+00000f00: 656c 6c0a 7069 7020 696e 7374 616c 6c20  ell.pip install 
+00000f10: 2d55 206d 6f64 656c 7363 6f70 650a 2320  -U modelscope.# 
+00000f20: 466f 7220 7468 6520 7573 6572 7320 696e  For the users in
+00000f30: 2043 6869 6e61 2c20 796f 7520 636f 756c   China, you coul
+00000f40: 6420 696e 7374 616c 6c20 7769 7468 2074  d install with t
+00000f50: 6865 2063 6f6d 6d61 6e64 3a0a 2320 7069  he command:.# pi
+00000f60: 7020 696e 7374 616c 6c20 2d55 206d 6f64  p install -U mod
+00000f70: 656c 7363 6f70 6520 2d66 2068 7474 7073  elscope -f https
+00000f80: 3a2f 2f6d 6f64 656c 7363 6f70 652e 6f73  ://modelscope.os
+00000f90: 732d 636e 2d62 6569 6a69 6e67 2e61 6c69  s-cn-beijing.ali
+00000fa0: 7975 6e63 732e 636f 6d2f 7265 6c65 6173  yuncs.com/releas
+00000fb0: 6573 2f72 6570 6f2e 6874 6d6c 202d 6920  es/repo.html -i 
+00000fc0: 6874 7470 733a 2f2f 6d69 7272 6f72 2e73  https://mirror.s
+00000fd0: 6a74 752e 6564 752e 636e 2f70 7970 692f  jtu.edu.cn/pypi/
+00000fe0: 7765 622f 7369 6d70 6c65 0a60 6060 0a0a  web/simple.```..
+00000ff0: 466f 7220 6d6f 7265 2064 6574 6169 6c73  For more details
+00001000: 2c20 706c 6561 7365 2072 6566 2074 6f20  , please ref to 
+00001010: 5b69 6e73 7461 6c6c 6174 696f 6e5d 2868  [installation](h
+00001020: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001030: 6d2f 616c 6962 6162 612d 6461 6d6f 2d61  m/alibaba-damo-a
+00001040: 6361 6465 6d79 2f46 756e 4153 522f 7769  cademy/FunASR/wi
+00001050: 6b69 290a 0a5b 2f2f 5d3a 2023 2028 290a  ki)..[//]: # ().
+00001060: 5b2f 2f5d 3a20 2320 2823 2320 5573 6167  [//]: # (## Usag
+00001070: 6529 0a0a 5b2f 2f5d 3a20 2320 2846 6f72  e)..[//]: # (For
+00001080: 2075 7365 7273 2077 686f 2061 7265 206e   users who are n
+00001090: 6577 2074 6f20 4675 6e41 5352 2061 6e64  ew to FunASR and
+000010a0: 204d 6f64 656c 5363 6f70 652c 2070 6c65   ModelScope, ple
+000010b0: 6173 6520 7265 6665 7220 746f 2046 756e  ase refer to Fun
+000010c0: 4153 5220 446f 6373 2623 3430 3b5b 434e  ASR Docs&#40;[CN
+000010d0: 5d26 2334 303b 6874 7470 733a 2f2f 616c  ]&#40;https://al
+000010e0: 6962 6162 612d 6461 6d6f 2d61 6361 6465  ibaba-damo-acade
+000010f0: 6d79 2e67 6974 6875 622e 696f 2f46 756e  my.github.io/Fun
+00001100: 4153 522f 636e 2f69 6e64 6578 2e68 746d  ASR/cn/index.htm
+00001110: 6c26 2334 313b 202f 205b 454e 5d26 2334  l&#41; / [EN]&#4
+00001120: 303b 6874 7470 733a 2f2f 616c 6962 6162  0;https://alibab
+00001130: 612d 6461 6d6f 2d61 6361 6465 6d79 2e67  a-damo-academy.g
+00001140: 6974 6875 622e 696f 2f46 756e 4153 522f  ithub.io/FunASR/
+00001150: 656e 2f69 6e64 6578 2e68 746d 6c26 2334  en/index.html&#4
+00001160: 313b 2623 3431 3b29 0a0a 2323 2043 6f6e  1;&#41;)..## Con
+00001170: 7461 6374 0a0a 4966 2079 6f75 2068 6176  tact..If you hav
+00001180: 6520 616e 7920 7175 6573 7469 6f6e 7320  e any questions 
+00001190: 6162 6f75 7420 4675 6e41 5352 2c20 706c  about FunASR, pl
+000011a0: 6561 7365 2063 6f6e 7461 6374 2075 7320  ease contact us 
+000011b0: 6279 0a0a 2d20 656d 6169 6c3a 205b 6675  by..- email: [fu
+000011c0: 6e61 7372 406c 6973 742e 616c 6962 6162  nasr@list.alibab
+000011d0: 612d 696e 632e 636f 6d5d 2866 756e 6173  a-inc.com](funas
+000011e0: 7240 6c69 7374 2e61 6c69 6261 6261 2d69  r@list.alibaba-i
+000011f0: 6e63 2e63 6f6d 290a 0a7c 4469 6e67 6469  nc.com)..|Dingdi
+00001200: 6e67 2067 726f 7570 207c 2020 2020 2020  ng group |      
+00001210: 2020 2020 2020 2020 2020 2020 2020 2057                 W
+00001220: 6563 6861 7420 6772 6f75 7020 2020 2020  echat group     
+00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001240: 207c 0a7c 3a2d 2d2d 3a7c 3a2d 2d2d 2d2d   |.|:---:|:-----
+00001250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001280: 3a7c 0a7c 3c64 6976 2061 6c69 676e 3d22  :|.|<div align="
+00001290: 6c65 6674 223e 3c69 6d67 2073 7263 3d22  left"><img src="
+000012a0: 646f 6373 2f69 6d61 6765 732f 6469 6e67  docs/images/ding
+000012b0: 6469 6e67 2e6a 7067 2220 7769 6474 683d  ding.jpg" width=
+000012c0: 2232 3530 222f 3e20 7c20 3c69 6d67 2073  "250"/> | <img s
+000012d0: 7263 3d22 646f 6373 2f69 6d61 6765 732f  rc="docs/images/
+000012e0: 7765 6368 6174 2e70 6e67 2220 7769 6474  wechat.png" widt
+000012f0: 683d 2232 3332 222f 3e3c 2f64 6976 3e20  h="232"/></div> 
+00001300: 7c0a 0a23 2320 436f 6e74 7269 6275 746f  |..## Contributo
+00001310: 7273 0a0a 7c20 3c64 6976 2061 6c69 676e  rs..| <div align
+00001320: 3d22 6c65 6674 223e 3c69 6d67 2073 7263  ="left"><img src
+00001330: 3d22 646f 6373 2f69 6d61 6765 732f 6461  ="docs/images/da
+00001340: 6d6f 2e70 6e67 2220 7769 6474 683d 2231  mo.png" width="1
+00001350: 3830 222f 3e20 7c20 3c64 6976 2061 6c69  80"/> | <div ali
+00001360: 676e 3d22 6c65 6674 223e 3c69 6d67 2073  gn="left"><img s
+00001370: 7263 3d22 646f 6373 2f69 6d61 6765 732f  rc="docs/images/
+00001380: 6e77 7075 2e70 6e67 2220 7769 6474 683d  nwpu.png" width=
+00001390: 2232 3630 222f 3e20 7c20 3c69 6d67 2073  "260"/> | <img s
+000013a0: 7263 3d22 646f 6373 2f69 6d61 6765 732f  rc="docs/images/
+000013b0: 4465 6570 5363 6965 6e63 652e 706e 6722  DeepScience.png"
+000013c0: 2077 6964 7468 3d22 3230 3022 2f3e 203c   width="200"/> <
+000013d0: 2f64 6976 3e20 7c0a 7c3a 2d2d 2d2d 2d2d  /div> |.|:------
+000013e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000013f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001410: 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d  ---------:|:----
+00001420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  -----------:|:--
+00001460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001490: 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a 0a23 2320  ---------:|..## 
+000014a0: 4163 6b6e 6f77 6c65 6467 650a 0a31 2e20  Acknowledge..1. 
+000014b0: 5765 2062 6f72 726f 7765 6420 6120 6c6f  We borrowed a lo
+000014c0: 7420 6f66 2063 6f64 6520 6672 6f6d 205b  t of code from [
+000014d0: 4b61 6c64 695d 2868 7474 703a 2f2f 6b61  Kaldi](http://ka
+000014e0: 6c64 692d 6173 722e 6f72 672f 2920 666f  ldi-asr.org/) fo
+000014f0: 7220 6461 7461 2070 7265 7061 7261 7469  r data preparati
+00001500: 6f6e 2e0a 322e 2057 6520 626f 7272 6f77  on..2. We borrow
+00001510: 6564 2061 206c 6f74 206f 6620 636f 6465  ed a lot of code
+00001520: 2066 726f 6d20 5b45 5350 6e65 745d 2868   from [ESPnet](h
+00001530: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001540: 6d2f 6573 706e 6574 2f65 7370 6e65 7429  m/espnet/espnet)
+00001550: 2e20 4675 6e41 5352 2066 6f6c 6c6f 7773  . FunASR follows
+00001560: 2075 7020 7468 6520 7472 6169 6e69 6e67   up the training
+00001570: 2061 6e64 2066 696e 6574 756e 696e 6720   and finetuning 
+00001580: 7069 7065 6c69 6e65 7320 6f66 2045 5350  pipelines of ESP
+00001590: 6e65 742e 0a33 2e20 5765 2072 6566 6572  net..3. We refer
+000015a0: 7265 6420 5b57 656e 6574 5d28 6874 7470  red [Wenet](http
+000015b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f77  s://github.com/w
+000015c0: 656e 6574 2d65 3265 2f77 656e 6574 2920  enet-e2e/wenet) 
+000015d0: 666f 7220 6275 696c 6469 6e67 2064 6174  for building dat
+000015e0: 616c 6f61 6465 7220 666f 7220 6c61 7267  aloader for larg
+000015f0: 6520 7363 616c 6520 6461 7461 2074 7261  e scale data tra
+00001600: 696e 696e 672e 0a34 2e20 5765 2061 636b  ining..4. We ack
+00001610: 6e6f 776c 6564 6765 205b 4465 6570 5363  nowledge [DeepSc
+00001620: 6965 6e63 655d 2868 7474 7073 3a2f 2f77  ience](https://w
+00001630: 7777 2e64 6565 7073 6369 656e 6365 2e63  ww.deepscience.c
+00001640: 6e29 2066 6f72 2063 6f6e 7472 6962 7574  n) for contribut
+00001650: 696e 6720 7468 6520 6772 7063 2073 6572  ing the grpc ser
+00001660: 7669 6365 2e0a 0a23 2320 4c69 6365 6e73  vice...## Licens
+00001670: 650a 5468 6973 2070 726f 6a65 6374 2069  e.This project i
+00001680: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
+00001690: 2074 6865 205b 5468 6520 4d49 5420 4c69   the [The MIT Li
+000016a0: 6365 6e73 655d 2868 7474 7073 3a2f 2f6f  cense](https://o
+000016b0: 7065 6e73 6f75 7263 652e 6f72 672f 6c69  pensource.org/li
+000016c0: 6365 6e73 6573 2f4d 4954 292e 2046 756e  censes/MIT). Fun
+000016d0: 4153 5220 616c 736f 2063 6f6e 7461 696e  ASR also contain
+000016e0: 7320 7661 7269 6f75 7320 7468 6972 642d  s various third-
+000016f0: 7061 7274 7920 636f 6d70 6f6e 656e 7473  party components
+00001700: 2061 6e64 2073 6f6d 6520 636f 6465 206d   and some code m
+00001710: 6f64 6966 6965 6420 6672 6f6d 206f 7468  odified from oth
+00001720: 6572 2072 6570 6f73 2075 6e64 6572 206f  er repos under o
+00001730: 7468 6572 206f 7065 6e20 736f 7572 6365  ther open source
+00001740: 206c 6963 656e 7365 732e 0a0a 2323 2043   licenses...## C
+00001750: 6974 6174 696f 6e73 0a0a 6060 6020 6269  itations..``` bi
+00001760: 6274 6578 0a40 696e 7072 6f63 6565 6469  btex.@inproceedi
+00001770: 6e67 737b 6761 6f32 3032 3270 6172 6166  ngs{gao2022paraf
+00001780: 6f72 6d65 722c 0a20 2074 6974 6c65 3d7b  ormer,.  title={
+00001790: 5061 7261 666f 726d 6572 3a20 4661 7374  Paraformer: Fast
+000017a0: 2061 6e64 2041 6363 7572 6174 6520 5061   and Accurate Pa
+000017b0: 7261 6c6c 656c 2054 7261 6e73 666f 726d  rallel Transform
+000017c0: 6572 2066 6f72 204e 6f6e 2d61 7574 6f72  er for Non-autor
+000017d0: 6567 7265 7373 6976 6520 456e 642d 746f  egressive End-to
+000017e0: 2d45 6e64 2053 7065 6563 6820 5265 636f  -End Speech Reco
+000017f0: 676e 6974 696f 6e7d 2c0a 2020 6175 7468  gnition},.  auth
+00001800: 6f72 3d7b 4761 6f2c 205a 6869 6675 2061  or={Gao, Zhifu a
+00001810: 6e64 205a 6861 6e67 2c20 5368 696c 6961  nd Zhang, Shilia
+00001820: 6e67 2061 6e64 204d 634c 6f75 6768 6c69  ng and McLoughli
+00001830: 6e2c 2049 616e 2061 6e64 2059 616e 2c20  n, Ian and Yan, 
+00001840: 5a68 696a 6965 7d2c 0a20 2062 6f6f 6b74  Zhijie},.  bookt
+00001850: 6974 6c65 3d7b 494e 5445 5253 5045 4543  itle={INTERSPEEC
+00001860: 487d 2c0a 2020 7965 6172 3d7b 3230 3232  H},.  year={2022
+00001870: 7d0a 7d0a 4069 6e70 726f 6365 6564 696e  }.}.@inproceedin
+00001880: 6773 7b67 616f 3230 3230 756e 6976 6572  gs{gao2020univer
+00001890: 7361 6c2c 0a20 2074 6974 6c65 3d7b 556e  sal,.  title={Un
+000018a0: 6976 6572 7361 6c20 4153 523a 2055 6e69  iversal ASR: Uni
+000018b0: 6679 696e 6720 5374 7265 616d 696e 6720  fying Streaming 
+000018c0: 616e 6420 4e6f 6e2d 5374 7265 616d 696e  and Non-Streamin
+000018d0: 6720 4153 5220 5573 696e 6720 6120 5369  g ASR Using a Si
+000018e0: 6e67 6c65 2045 6e63 6f64 6572 2d44 6563  ngle Encoder-Dec
+000018f0: 6f64 6572 204d 6f64 656c 7d2c 0a20 2061  oder Model},.  a
+00001900: 7574 686f 723d 7b47 616f 2c20 5a68 6966  uthor={Gao, Zhif
+00001910: 7520 616e 6420 5a68 616e 672c 2053 6869  u and Zhang, Shi
+00001920: 6c69 616e 6720 616e 6420 4c65 692c 204d  liang and Lei, M
+00001930: 696e 6720 616e 6420 4d63 4c6f 7567 686c  ing and McLoughl
+00001940: 696e 2c20 4961 6e7d 2c0a 2020 626f 6f6b  in, Ian},.  book
+00001950: 7469 746c 653d 7b61 7258 6976 2070 7265  title={arXiv pre
+00001960: 7072 696e 7420 6172 5869 763a 3230 3130  print arXiv:2010
+00001970: 2e31 3430 3939 7d2c 0a20 2079 6561 723d  .14099},.  year=
+00001980: 7b32 3032 307d 0a7d 0a40 696e 7072 6f63  {2020}.}.@inproc
+00001990: 6565 6469 6e67 737b 5368 6932 3032 3341  eedings{Shi2023A
+000019a0: 6368 6965 7669 6e67 5450 2c0a 2020 7469  chievingTP,.  ti
+000019b0: 746c 653d 7b41 6368 6965 7669 6e67 2054  tle={Achieving T
+000019c0: 696d 6573 7461 6d70 2050 7265 6469 6374  imestamp Predict
+000019d0: 696f 6e20 5768 696c 6520 5265 636f 676e  ion While Recogn
+000019e0: 697a 696e 6720 7769 7468 204e 6f6e 2d41  izing with Non-A
+000019f0: 7574 6f72 6567 7265 7373 6976 6520 456e  utoregressive En
+00001a00: 642d 746f 2d45 6e64 2041 5352 204d 6f64  d-to-End ASR Mod
+00001a10: 656c 7d2c 0a20 2061 7574 686f 723d 7b58  el},.  author={X
+00001a20: 6961 6e20 5368 6920 616e 6420 5961 6e6e  ian Shi and Yann
+00001a30: 6920 4368 656e 2061 6e64 2053 6869 6c69  i Chen and Shili
+00001a40: 616e 6720 5a68 616e 6720 616e 6420 5a68  ang Zhang and Zh
+00001a50: 696a 6965 2059 616e 7d2c 0a20 2062 6f6f  ijie Yan},.  boo
+00001a60: 6b74 6974 6c65 3d7b 6172 5869 7620 7072  ktitle={arXiv pr
+00001a70: 6570 7269 6e74 2061 7258 6976 3a32 3330  eprint arXiv:230
+00001a80: 312e 3132 3334 337d 0a20 2079 6561 723d  1.12343}.  year=
+00001a90: 7b32 3032 337d 0a7d 0a60 6060 0a         {2023}.}.```.
```

### Comparing `funasr-0.4.1/README.md` & `funasr-0.4.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,351 +1,491 @@
-00000000: 5b2f 2f5d 3a20 2320 283c 6469 7620 616c  [//]: # (<div al
-00000010: 6967 6e3d 226c 6566 7422 3e3c 696d 6720  ign="left"><img 
-00000020: 7372 633d 2264 6f63 732f 696d 6167 6573  src="docs/images
-00000030: 2f66 756e 6173 725f 6c6f 676f 2e6a 7067  /funasr_logo.jpg
-00000040: 2220 7769 6474 683d 2234 3030 222f 3e3c  " width="400"/><
-00000050: 2f64 6976 3e29 0a0a 2320 4675 6e41 5352  /div>)..# FunASR
-00000060: 3a20 4120 4675 6e64 616d 656e 7461 6c20  : A Fundamental 
-00000070: 456e 642d 746f 2d45 6e64 2053 7065 6563  End-to-End Speec
-00000080: 6820 5265 636f 676e 6974 696f 6e20 546f  h Recognition To
-00000090: 6f6c 6b69 740a 0a3c 7374 726f 6e67 3e46  olkit..<strong>F
-000000a0: 756e 4153 523c 2f73 7472 6f6e 673e 2068  unASR</strong> h
-000000b0: 6f70 6573 2074 6f20 6275 696c 6420 6120  opes to build a 
-000000c0: 6272 6964 6765 2062 6574 7765 656e 2061  bridge between a
-000000d0: 6361 6465 6d69 6320 7265 7365 6172 6368  cademic research
-000000e0: 2061 6e64 2069 6e64 7573 7472 6961 6c20   and industrial 
-000000f0: 6170 706c 6963 6174 696f 6e73 206f 6e20  applications on 
-00000100: 7370 6565 6368 2072 6563 6f67 6e69 7469  speech recogniti
-00000110: 6f6e 2e20 4279 2073 7570 706f 7274 696e  on. By supportin
-00000120: 6720 7468 6520 7472 6169 6e69 6e67 2026  g the training &
-00000130: 2066 696e 6574 756e 696e 6720 6f66 2074   finetuning of t
-00000140: 6865 2069 6e64 7573 7472 6961 6c2d 6772  he industrial-gr
-00000150: 6164 6520 7370 6565 6368 2072 6563 6f67  ade speech recog
-00000160: 6e69 7469 6f6e 206d 6f64 656c 2072 656c  nition model rel
-00000170: 6561 7365 6420 6f6e 205b 4d6f 6465 6c53  eased on [ModelS
-00000180: 636f 7065 5d28 6874 7470 733a 2f2f 7777  cope](https://ww
-00000190: 772e 6d6f 6465 6c73 636f 7065 2e63 6e2f  w.modelscope.cn/
-000001a0: 6d6f 6465 6c73 3f70 6167 653d 3126 7461  models?page=1&ta
-000001b0: 736b 733d 6175 746f 2d73 7065 6563 682d  sks=auto-speech-
-000001c0: 7265 636f 676e 6974 696f 6e29 2c20 7265  recognition), re
-000001d0: 7365 6172 6368 6572 7320 616e 6420 6465  searchers and de
-000001e0: 7665 6c6f 7065 7273 2063 616e 2063 6f6e  velopers can con
-000001f0: 6475 6374 2072 6573 6561 7263 6820 616e  duct research an
-00000200: 6420 7072 6f64 7563 7469 6f6e 206f 6620  d production of 
-00000210: 7370 6565 6368 2072 6563 6f67 6e69 7469  speech recogniti
-00000220: 6f6e 206d 6f64 656c 7320 6d6f 7265 2063  on models more c
-00000230: 6f6e 7665 6e69 656e 746c 792c 2061 6e64  onveniently, and
-00000240: 2070 726f 6d6f 7465 2074 6865 2064 6576   promote the dev
-00000250: 656c 6f70 6d65 6e74 206f 6620 7370 6565  elopment of spee
-00000260: 6368 2072 6563 6f67 6e69 7469 6f6e 2065  ch recognition e
-00000270: 636f 6c6f 6779 2e20 4153 5220 666f 7220  cology. ASR for 
-00000280: 4675 6eef bc81 0a0a 5b2a 2a4e 6577 732a  Fun.....[**News*
-00000290: 2a5d 2868 7474 7073 3a2f 2f67 6974 6875  *](https://githu
-000002a0: 622e 636f 6d2f 616c 6962 6162 612d 6461  b.com/alibaba-da
-000002b0: 6d6f 2d61 6361 6465 6d79 2f46 756e 4153  mo-academy/FunAS
-000002c0: 5223 7768 6174 732d 6e65 7729 200a 7c20  R#whats-new) .| 
-000002d0: 5b2a 2a48 6967 686c 6967 6874 732a 2a5d  [**Highlights**]
-000002e0: 2823 6869 6768 6c69 6768 7473 290a 7c20  (#highlights).| 
-000002f0: 5b2a 2a49 6e73 7461 6c6c 6174 696f 6e2a  [**Installation*
-00000300: 2a5d 2823 696e 7374 616c 6c61 7469 6f6e  *](#installation
-00000310: 290a 7c20 5b2a 2a44 6f63 735f 454e 2a2a  ).| [**Docs_EN**
-00000320: 5d28 6874 7470 733a 2f2f 616c 6962 6162  ](https://alibab
-00000330: 612d 6461 6d6f 2d61 6361 6465 6d79 2e67  a-damo-academy.g
-00000340: 6974 6875 622e 696f 2f46 756e 4153 522f  ithub.io/FunASR/
-00000350: 656e 2f69 6e64 6578 2e68 746d 6c29 0a7c  en/index.html).|
-00000360: 205b 2a2a 5475 746f 7269 616c 2a2a 5d28   [**Tutorial**](
-00000370: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000380: 6f6d 2f61 6c69 6261 6261 2d64 616d 6f2d  om/alibaba-damo-
-00000390: 6163 6164 656d 792f 4675 6e41 5352 2f77  academy/FunASR/w
-000003a0: 696b 6923 6675 6e61 7372 2545 3725 3934  iki#funasr%E7%94
-000003b0: 2541 3825 4536 2538 3825 4237 2545 3625  %A8%E6%88%B7%E6%
-000003c0: 3839 2538 4225 4535 2538 3625 3843 290a  89%8B%E5%86%8C).
-000003d0: 7c20 5b2a 2a50 6170 6572 732a 2a5d 2868  | [**Papers**](h
-000003e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000003f0: 6d2f 616c 6962 6162 612d 6461 6d6f 2d61  m/alibaba-damo-a
-00000400: 6361 6465 6d79 2f46 756e 4153 5223 6369  cademy/FunASR#ci
-00000410: 7461 7469 6f6e 7329 0a7c 205b 2a2a 5275  tations).| [**Ru
-00000420: 6e74 696d 652a 2a5d 2868 7474 7073 3a2f  ntime**](https:/
-00000430: 2f67 6974 6875 622e 636f 6d2f 616c 6962  /github.com/alib
-00000440: 6162 612d 6461 6d6f 2d61 6361 6465 6d79  aba-damo-academy
-00000450: 2f46 756e 4153 522f 7472 6565 2f6d 6169  /FunASR/tree/mai
-00000460: 6e2f 6675 6e61 7372 2f72 756e 7469 6d65  n/funasr/runtime
-00000470: 290a 7c20 5b2a 2a4d 6f64 656c 205a 6f6f  ).| [**Model Zoo
-00000480: 2a2a 5d28 6874 7470 733a 2f2f 6769 7468  **](https://gith
-00000490: 7562 2e63 6f6d 2f61 6c69 6261 6261 2d64  ub.com/alibaba-d
-000004a0: 616d 6f2d 6163 6164 656d 792f 4675 6e41  amo-academy/FunA
-000004b0: 5352 2f62 6c6f 622f 6d61 696e 2f64 6f63  SR/blob/main/doc
-000004c0: 732f 6d6f 6465 6c73 636f 7065 5f6d 6f64  s/modelscope_mod
-000004d0: 656c 732e 6d64 290a 7c20 5b2a 2a43 6f6e  els.md).| [**Con
-000004e0: 7461 6374 2a2a 5d28 2363 6f6e 7461 6374  tact**](#contact
-000004f0: 290a 0a0a 2323 2057 6861 7427 7320 6e65  )...## What's ne
-00000500: 773a 200a 0a46 6f72 2074 6865 2072 656c  w: ..For the rel
-00000510: 6561 7365 206e 6f74 6573 2c20 706c 6561  ease notes, plea
-00000520: 7365 2072 6566 2074 6f20 5b6e 6577 735d  se ref to [news]
-00000530: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000540: 636f 6d2f 616c 6962 6162 612d 6461 6d6f  com/alibaba-damo
-00000550: 2d61 6361 6465 6d79 2f46 756e 4153 522f  -academy/FunASR/
-00000560: 7265 6c65 6173 6573 290a 0a23 2320 4869  releases)..## Hi
-00000570: 6768 6c69 6768 7473 0a2d 204d 616e 7920  ghlights.- Many 
-00000580: 7479 7065 7320 6f66 2074 7970 6963 616c  types of typical
-00000590: 206d 6f64 656c 7320 6172 6520 7375 7070   models are supp
-000005a0: 6f72 7465 642c 2065 2e67 2e2c 205b 5472  orted, e.g., [Tr
-000005b0: 616e 666f 726d 6572 5d28 6874 7470 733a  anformer](https:
-000005c0: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
-000005d0: 3137 3036 2e30 3337 3632 292c 205b 436f  1706.03762), [Co
-000005e0: 6e66 6f72 6d65 725d 2868 7474 7073 3a2f  nformer](https:/
-000005f0: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
-00000600: 3030 352e 3038 3130 3029 2c20 5b50 6172  005.08100), [Par
-00000610: 6166 6f72 6d65 725d 2868 7474 7073 3a2f  aformer](https:/
-00000620: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
-00000630: 3230 362e 3038 3331 3729 2e0a 2d20 5765  206.08317)..- We
-00000640: 2068 6176 6520 7265 6c65 6173 6564 206c   have released l
-00000650: 6172 6765 206e 756d 6265 7220 6f66 2061  arge number of a
-00000660: 6361 6465 6d69 6320 616e 6420 696e 6475  cademic and indu
-00000670: 7374 7269 616c 2070 7265 7472 6169 6e65  strial pretraine
-00000680: 6420 6d6f 6465 6c73 206f 6e20 5b4d 6f64  d models on [Mod
-00000690: 656c 5363 6f70 655d 2868 7474 7073 3a2f  elScope](https:/
-000006a0: 2f77 7777 2e6d 6f64 656c 7363 6f70 652e  /www.modelscope.
-000006b0: 636e 2f6d 6f64 656c 733f 7061 6765 3d31  cn/models?page=1
-000006c0: 2674 6173 6b73 3d61 7574 6f2d 7370 6565  &tasks=auto-spee
-000006d0: 6368 2d72 6563 6f67 6e69 7469 6f6e 290a  ch-recognition).
-000006e0: 2d20 5468 6520 7072 6574 7261 696e 6564  - The pretrained
-000006f0: 206d 6f64 656c 205b 5061 7261 666f 726d   model [Paraform
-00000700: 6572 2d6c 6172 6765 5d28 6874 7470 733a  er-large](https:
-00000710: 2f2f 7777 772e 6d6f 6465 6c73 636f 7065  //www.modelscope
-00000720: 2e63 6e2f 6d6f 6465 6c73 2f64 616d 6f2f  .cn/models/damo/
-00000730: 7370 6565 6368 5f70 6172 6166 6f72 6d65  speech_paraforme
-00000740: 722d 6c61 7267 655f 6173 725f 6e61 742d  r-large_asr_nat-
-00000750: 7a68 2d63 6e2d 3136 6b2d 636f 6d6d 6f6e  zh-cn-16k-common
-00000760: 2d76 6f63 6162 3834 3034 2d70 7974 6f72  -vocab8404-pytor
-00000770: 6368 2f73 756d 6d61 7279 2920 6f62 7461  ch/summary) obta
-00000780: 696e 7320 7468 6520 6265 7374 2070 6572  ins the best per
-00000790: 666f 726d 616e 6365 206f 6e20 6d61 6e79  formance on many
-000007a0: 2074 6173 6b73 2069 6e20 5b53 7065 6563   tasks in [Speec
-000007b0: 6849 4f20 6c65 6164 6572 626f 6172 645d  hIO leaderboard]
-000007c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000007d0: 636f 6d2f 5370 6565 6368 436f 6c61 622f  com/SpeechColab/
-000007e0: 4c65 6164 6572 626f 6172 6429 0a2d 2046  Leaderboard).- F
-000007f0: 756e 4153 5220 7375 7070 6c69 6573 2061  unASR supplies a
-00000800: 2065 6173 792d 746f 2d75 7365 2070 6970   easy-to-use pip
-00000810: 656c 696e 6520 746f 2066 696e 6574 756e  eline to finetun
-00000820: 6520 7072 6574 7261 696e 6564 206d 6f64  e pretrained mod
-00000830: 656c 7320 6672 6f6d 205b 4d6f 6465 6c53  els from [ModelS
-00000840: 636f 7065 5d28 6874 7470 733a 2f2f 7777  cope](https://ww
-00000850: 772e 6d6f 6465 6c73 636f 7065 2e63 6e2f  w.modelscope.cn/
-00000860: 6d6f 6465 6c73 3f70 6167 653d 3126 7461  models?page=1&ta
-00000870: 736b 733d 6175 746f 2d73 7065 6563 682d  sks=auto-speech-
-00000880: 7265 636f 676e 6974 696f 6e29 0a2d 2043  recognition).- C
-00000890: 6f6d 7061 7265 6420 746f 205b 4573 706e  ompared to [Espn
-000008a0: 6574 5d28 6874 7470 733a 2f2f 6769 7468  et](https://gith
-000008b0: 7562 2e63 6f6d 2f65 7370 6e65 742f 6573  ub.com/espnet/es
-000008c0: 706e 6574 2920 6672 616d 6577 6f72 6b2c  pnet) framework,
-000008d0: 2074 6865 2074 7261 696e 696e 6720 7370   the training sp
-000008e0: 6565 6420 6f66 206c 6172 6765 2d73 6361  eed of large-sca
-000008f0: 6c65 2064 6174 6173 6574 7320 696e 2046  le datasets in F
-00000900: 756e 4153 5220 6973 206d 7563 6820 6661  unASR is much fa
-00000910: 7374 6572 206f 776e 696e 6720 746f 2074  ster owning to t
-00000920: 6865 206f 7074 696d 697a 6564 2064 6174  he optimized dat
-00000930: 616c 6f61 6465 722e 0a0a 2323 2049 6e73  aloader...## Ins
-00000940: 7461 6c6c 6174 696f 6e0a 0a49 6e73 7461  tallation..Insta
-00000950: 6c6c 2066 726f 6d20 7069 700a 6060 6073  ll from pip.```s
-00000960: 6865 6c6c 0a70 6970 2069 6e73 7461 6c6c  hell.pip install
-00000970: 202d 5520 6675 6e61 7372 202d 6920 6874   -U funasr -i ht
-00000980: 7470 733a 2f2f 7079 7069 2e50 7974 686f  tps://pypi.Pytho
-00000990: 6e2e 6f72 672f 7369 6d70 6c65 0a60 6060  n.org/simple.```
-000009a0: 0a0a 4f72 2069 6e73 7461 6c6c 2066 726f  ..Or install fro
-000009b0: 6d20 736f 7572 6365 2063 6f64 650a 0a0a  m source code...
-000009c0: 6060 6020 7368 0a67 6974 2063 6c6f 6e65  ``` sh.git clone
-000009d0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000009e0: 636f 6d2f 616c 6962 6162 612f 4675 6e41  com/alibaba/FunA
-000009f0: 5352 2e67 6974 2026 2620 6364 2046 756e  SR.git && cd Fun
-00000a00: 4153 520a 7069 7020 696e 7374 616c 6c20  ASR.pip install 
-00000a10: 2d65 202e 2f0a 6060 600a 4966 2079 6f75  -e ./.```.If you
-00000a20: 2077 616e 7420 746f 2075 7365 2074 6865   want to use the
-00000a30: 2070 7265 7472 6169 6e65 6420 6d6f 6465   pretrained mode
-00000a40: 6c73 2069 6e20 4d6f 6465 6c53 636f 7065  ls in ModelScope
-00000a50: 2c20 796f 7520 7368 6f75 6c64 2069 6e73  , you should ins
-00000a60: 7461 6c6c 2074 6865 206d 6f64 656c 7363  tall the modelsc
-00000a70: 6f70 653a 0a0a 6060 6073 6865 6c6c 0a70  ope:..```shell.p
-00000a80: 6970 2069 6e73 7461 6c6c 202d 5520 6d6f  ip install -U mo
-00000a90: 6465 6c73 636f 7065 0a23 2046 6f72 2074  delscope.# For t
-00000aa0: 6865 2075 7365 7273 2069 6e20 4368 696e  he users in Chin
-00000ab0: 612c 2079 6f75 2063 6f75 6c64 2069 6e73  a, you could ins
-00000ac0: 7461 6c6c 2077 6974 6820 7468 6520 636f  tall with the co
-00000ad0: 6d6d 616e 643a 0a23 2070 6970 2069 6e73  mmand:.# pip ins
-00000ae0: 7461 6c6c 202d 5520 6d6f 6465 6c73 636f  tall -U modelsco
-00000af0: 7065 202d 6620 6874 7470 733a 2f2f 6d6f  pe -f https://mo
-00000b00: 6465 6c73 636f 7065 2e6f 7373 2d63 6e2d  delscope.oss-cn-
-00000b10: 6265 696a 696e 672e 616c 6979 756e 6373  beijing.aliyuncs
-00000b20: 2e63 6f6d 2f72 656c 6561 7365 732f 7265  .com/releases/re
-00000b30: 706f 2e68 746d 6c20 2d69 2068 7474 7073  po.html -i https
-00000b40: 3a2f 2f6d 6972 726f 722e 736a 7475 2e65  ://mirror.sjtu.e
-00000b50: 6475 2e63 6e2f 7079 7069 2f77 6562 2f73  du.cn/pypi/web/s
-00000b60: 696d 706c 650a 6060 600a 0a46 6f72 206d  imple.```..For m
-00000b70: 6f72 6520 6465 7461 696c 732c 2070 6c65  ore details, ple
-00000b80: 6173 6520 7265 6620 746f 205b 696e 7374  ase ref to [inst
-00000b90: 616c 6c61 7469 6f6e 5d28 6874 7470 733a  allation](https:
-00000ba0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6c69  //github.com/ali
-00000bb0: 6261 6261 2d64 616d 6f2d 6163 6164 656d  baba-damo-academ
-00000bc0: 792f 4675 6e41 5352 2f77 696b 6929 0a0a  y/FunASR/wiki)..
-00000bd0: 2323 2055 7361 6765 0a46 6f72 2075 7365  ## Usage.For use
-00000be0: 7273 2077 686f 2061 7265 206e 6577 2074  rs who are new t
-00000bf0: 6f20 4675 6e41 5352 2061 6e64 204d 6f64  o FunASR and Mod
-00000c00: 656c 5363 6f70 652c 2070 6c65 6173 6520  elScope, please 
-00000c10: 7265 6665 7220 746f 2046 756e 4153 5220  refer to FunASR 
-00000c20: 446f 6373 285b 434e 5d28 6874 7470 733a  Docs([CN](https:
-00000c30: 2f2f 616c 6962 6162 612d 6461 6d6f 2d61  //alibaba-damo-a
-00000c40: 6361 6465 6d79 2e67 6974 6875 622e 696f  cademy.github.io
-00000c50: 2f46 756e 4153 522f 636e 2f69 6e64 6578  /FunASR/cn/index
-00000c60: 2e68 746d 6c29 202f 205b 454e 5d28 6874  .html) / [EN](ht
-00000c70: 7470 733a 2f2f 616c 6962 6162 612d 6461  tps://alibaba-da
-00000c80: 6d6f 2d61 6361 6465 6d79 2e67 6974 6875  mo-academy.githu
-00000c90: 622e 696f 2f46 756e 4153 522f 656e 2f69  b.io/FunASR/en/i
-00000ca0: 6e64 6578 2e68 746d 6c29 290a 0a23 2320  ndex.html))..## 
-00000cb0: 436f 6e74 6163 740a 0a49 6620 796f 7520  Contact..If you 
-00000cc0: 6861 7665 2061 6e79 2071 7565 7374 696f  have any questio
-00000cd0: 6e73 2061 626f 7574 2046 756e 4153 522c  ns about FunASR,
-00000ce0: 2070 6c65 6173 6520 636f 6e74 6163 7420   please contact 
-00000cf0: 7573 2062 790a 0a2d 2065 6d61 696c 3a20  us by..- email: 
-00000d00: 5b66 756e 6173 7240 6c69 7374 2e61 6c69  [funasr@list.ali
-00000d10: 6261 6261 2d69 6e63 2e63 6f6d 5d28 6675  baba-inc.com](fu
-00000d20: 6e61 7372 406c 6973 742e 616c 6962 6162  nasr@list.alibab
-00000d30: 612d 696e 632e 636f 6d29 0a0a 7c44 696e  a-inc.com)..|Din
-00000d40: 6764 696e 6720 6772 6f75 7020 7c20 2020  gding group |   
-00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d60: 2020 5765 6368 6174 2067 726f 7570 2020    Wechat group  
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 2020 2020 7c0a 7c3a 2d2d 2d3a 7c3a 2d2d      |.|:---:|:--
-00000d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000dc0: 2d2d 2d3a 7c0a 7c3c 6469 7620 616c 6967  ---:|.|<div alig
-00000dd0: 6e3d 226c 6566 7422 3e3c 696d 6720 7372  n="left"><img sr
-00000de0: 633d 2264 6f63 732f 696d 6167 6573 2f64  c="docs/images/d
-00000df0: 696e 6764 696e 672e 6a70 6722 2077 6964  ingding.jpg" wid
-00000e00: 7468 3d22 3235 3022 2f3e 207c 203c 696d  th="250"/> | <im
-00000e10: 6720 7372 633d 2264 6f63 732f 696d 6167  g src="docs/imag
-00000e20: 6573 2f77 6563 6861 742e 706e 6722 2077  es/wechat.png" w
-00000e30: 6964 7468 3d22 3233 3222 2f3e 3c2f 6469  idth="232"/></di
-00000e40: 763e 207c 0a0a 2323 2043 6f6e 7472 6962  v> |..## Contrib
-00000e50: 7574 6f72 730a 0a7c 203c 6469 7620 616c  utors..| <div al
-00000e60: 6967 6e3d 226c 6566 7422 3e3c 696d 6720  ign="left"><img 
-00000e70: 7372 633d 2264 6f63 732f 696d 6167 6573  src="docs/images
-00000e80: 2f64 616d 6f2e 706e 6722 2077 6964 7468  /damo.png" width
-00000e90: 3d22 3138 3022 2f3e 207c 203c 6469 7620  ="180"/> | <div 
-00000ea0: 616c 6967 6e3d 226c 6566 7422 3e3c 696d  align="left"><im
-00000eb0: 6720 7372 633d 2264 6f63 732f 696d 6167  g src="docs/imag
-00000ec0: 6573 2f6e 7770 752e 706e 6722 2077 6964  es/nwpu.png" wid
-00000ed0: 7468 3d22 3236 3022 2f3e 207c 203c 696d  th="260"/> | <im
-00000ee0: 6720 7372 633d 2264 6f63 732f 696d 6167  g src="docs/imag
-00000ef0: 6573 2f44 6565 7053 6369 656e 6365 2e70  es/DeepScience.p
-00000f00: 6e67 2220 7769 6474 683d 2232 3030 222f  ng" width="200"/
-00000f10: 3e20 3c2f 6469 763e 207c 0a7c 3a2d 2d2d  > </div> |.|:---
-00000f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d  ------------:|:-
-00000f60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  --------------:|
-00000fa0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
-00000fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000fd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 0a0a  ------------:|..
-00000fe0: 2323 2041 636b 6e6f 776c 6564 6765 0a0a  ## Acknowledge..
-00000ff0: 312e 2057 6520 626f 7272 6f77 6564 2061  1. We borrowed a
-00001000: 206c 6f74 206f 6620 636f 6465 2066 726f   lot of code fro
-00001010: 6d20 5b4b 616c 6469 5d28 6874 7470 3a2f  m [Kaldi](http:/
-00001020: 2f6b 616c 6469 2d61 7372 2e6f 7267 2f29  /kaldi-asr.org/)
-00001030: 2066 6f72 2064 6174 6120 7072 6570 6172   for data prepar
-00001040: 6174 696f 6e2e 0a32 2e20 5765 2062 6f72  ation..2. We bor
-00001050: 726f 7765 6420 6120 6c6f 7420 6f66 2063  rowed a lot of c
-00001060: 6f64 6520 6672 6f6d 205b 4553 506e 6574  ode from [ESPnet
-00001070: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001080: 2e63 6f6d 2f65 7370 6e65 742f 6573 706e  .com/espnet/espn
-00001090: 6574 292e 2046 756e 4153 5220 666f 6c6c  et). FunASR foll
-000010a0: 6f77 7320 7570 2074 6865 2074 7261 696e  ows up the train
-000010b0: 696e 6720 616e 6420 6669 6e65 7475 6e69  ing and finetuni
-000010c0: 6e67 2070 6970 656c 696e 6573 206f 6620  ng pipelines of 
-000010d0: 4553 506e 6574 2e0a 332e 2057 6520 7265  ESPnet..3. We re
-000010e0: 6665 7272 6564 205b 5765 6e65 745d 2868  ferred [Wenet](h
-000010f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001100: 6d2f 7765 6e65 742d 6532 652f 7765 6e65  m/wenet-e2e/wene
-00001110: 7429 2066 6f72 2062 7569 6c64 696e 6720  t) for building 
-00001120: 6461 7461 6c6f 6164 6572 2066 6f72 206c  dataloader for l
-00001130: 6172 6765 2073 6361 6c65 2064 6174 6120  arge scale data 
-00001140: 7472 6169 6e69 6e67 2e0a 342e 2057 6520  training..4. We 
-00001150: 6163 6b6e 6f77 6c65 6467 6520 5b44 6565  acknowledge [Dee
-00001160: 7053 6369 656e 6365 5d28 6874 7470 733a  pScience](https:
-00001170: 2f2f 7777 772e 6465 6570 7363 6965 6e63  //www.deepscienc
-00001180: 652e 636e 2920 666f 7220 636f 6e74 7269  e.cn) for contri
-00001190: 6275 7469 6e67 2074 6865 2067 7270 6320  buting the grpc 
-000011a0: 7365 7276 6963 652e 0a0a 2323 204c 6963  service...## Lic
-000011b0: 656e 7365 0a54 6869 7320 7072 6f6a 6563  ense.This projec
-000011c0: 7420 6973 206c 6963 656e 7365 6420 756e  t is licensed un
-000011d0: 6465 7220 7468 6520 5b54 6865 204d 4954  der the [The MIT
-000011e0: 204c 6963 656e 7365 5d28 6874 7470 733a   License](https:
-000011f0: 2f2f 6f70 656e 736f 7572 6365 2e6f 7267  //opensource.org
-00001200: 2f6c 6963 656e 7365 732f 4d49 5429 2e20  /licenses/MIT). 
-00001210: 4675 6e41 5352 2061 6c73 6f20 636f 6e74  FunASR also cont
-00001220: 6169 6e73 2076 6172 696f 7573 2074 6869  ains various thi
-00001230: 7264 2d70 6172 7479 2063 6f6d 706f 6e65  rd-party compone
-00001240: 6e74 7320 616e 6420 736f 6d65 2063 6f64  nts and some cod
-00001250: 6520 6d6f 6469 6669 6564 2066 726f 6d20  e modified from 
-00001260: 6f74 6865 7220 7265 706f 7320 756e 6465  other repos unde
-00001270: 7220 6f74 6865 7220 6f70 656e 2073 6f75  r other open sou
-00001280: 7263 6520 6c69 6365 6e73 6573 2e0a 0a23  rce licenses...#
-00001290: 2320 4369 7461 7469 6f6e 730a 0a60 6060  # Citations..```
-000012a0: 2062 6962 7465 780a 4069 6e70 726f 6365   bibtex.@inproce
-000012b0: 6564 696e 6773 7b67 616f 3230 3230 756e  edings{gao2020un
-000012c0: 6976 6572 7361 6c2c 0a20 2074 6974 6c65  iversal,.  title
-000012d0: 3d7b 556e 6976 6572 7361 6c20 4153 523a  ={Universal ASR:
-000012e0: 2055 6e69 6679 696e 6720 5374 7265 616d   Unifying Stream
-000012f0: 696e 6720 616e 6420 4e6f 6e2d 5374 7265  ing and Non-Stre
-00001300: 616d 696e 6720 4153 5220 5573 696e 6720  aming ASR Using 
-00001310: 6120 5369 6e67 6c65 2045 6e63 6f64 6572  a Single Encoder
-00001320: 2d44 6563 6f64 6572 204d 6f64 656c 7d2c  -Decoder Model},
-00001330: 0a20 2061 7574 686f 723d 7b47 616f 2c20  .  author={Gao, 
-00001340: 5a68 6966 7520 616e 6420 5a68 616e 672c  Zhifu and Zhang,
-00001350: 2053 6869 6c69 616e 6720 616e 6420 4c65   Shiliang and Le
-00001360: 692c 204d 696e 6720 616e 6420 4d63 4c6f  i, Ming and McLo
-00001370: 7567 686c 696e 2c20 4961 6e7d 2c0a 2020  ughlin, Ian},.  
-00001380: 626f 6f6b 7469 746c 653d 7b61 7258 6976  booktitle={arXiv
-00001390: 2070 7265 7072 696e 7420 6172 5869 763a   preprint arXiv:
-000013a0: 3230 3130 2e31 3430 3939 7d2c 0a20 2079  2010.14099},.  y
-000013b0: 6561 723d 7b32 3032 307d 0a7d 0a0a 4069  ear={2020}.}..@i
-000013c0: 6e70 726f 6365 6564 696e 6773 7b67 616f  nproceedings{gao
-000013d0: 3230 3232 7061 7261 666f 726d 6572 2c0a  2022paraformer,.
-000013e0: 2020 7469 746c 653d 7b50 6172 6166 6f72    title={Parafor
-000013f0: 6d65 723a 2046 6173 7420 616e 6420 4163  mer: Fast and Ac
-00001400: 6375 7261 7465 2050 6172 616c 6c65 6c20  curate Parallel 
-00001410: 5472 616e 7366 6f72 6d65 7220 666f 7220  Transformer for 
-00001420: 4e6f 6e2d 6175 746f 7265 6772 6573 7369  Non-autoregressi
-00001430: 7665 2045 6e64 2d74 6f2d 456e 6420 5370  ve End-to-End Sp
-00001440: 6565 6368 2052 6563 6f67 6e69 7469 6f6e  eech Recognition
-00001450: 7d2c 0a20 2061 7574 686f 723d 7b47 616f  },.  author={Gao
-00001460: 2c20 5a68 6966 7520 616e 6420 5a68 616e  , Zhifu and Zhan
-00001470: 672c 2053 6869 6c69 616e 6720 616e 6420  g, Shiliang and 
-00001480: 4d63 4c6f 7567 686c 696e 2c20 4961 6e20  McLoughlin, Ian 
-00001490: 616e 6420 5961 6e2c 205a 6869 6a69 657d  and Yan, Zhijie}
-000014a0: 2c0a 2020 626f 6f6b 7469 746c 653d 7b49  ,.  booktitle={I
-000014b0: 4e54 4552 5350 4545 4348 7d2c 0a20 2079  NTERSPEECH},.  y
-000014c0: 6561 723d 7b32 3032 327d 0a7d 0a40 696e  ear={2022}.}.@in
-000014d0: 7072 6f63 6565 6469 6e67 737b 5368 6932  proceedings{Shi2
-000014e0: 3032 3341 6368 6965 7669 6e67 5450 2c0a  023AchievingTP,.
-000014f0: 2020 7469 746c 653d 7b41 6368 6965 7669    title={Achievi
-00001500: 6e67 2054 696d 6573 7461 6d70 2050 7265  ng Timestamp Pre
-00001510: 6469 6374 696f 6e20 5768 696c 6520 5265  diction While Re
-00001520: 636f 676e 697a 696e 6720 7769 7468 204e  cognizing with N
-00001530: 6f6e 2d41 7574 6f72 6567 7265 7373 6976  on-Autoregressiv
-00001540: 6520 456e 642d 746f 2d45 6e64 2041 5352  e End-to-End ASR
-00001550: 204d 6f64 656c 7d2c 0a20 2061 7574 686f   Model},.  autho
-00001560: 723d 7b58 6961 6e20 5368 6920 616e 6420  r={Xian Shi and 
-00001570: 5961 6e6e 6920 4368 656e 2061 6e64 2053  Yanni Chen and S
-00001580: 6869 6c69 616e 6720 5a68 616e 6720 616e  hiliang Zhang an
-00001590: 6420 5a68 696a 6965 2059 616e 7d2c 0a20  d Zhijie Yan},. 
-000015a0: 2062 6f6f 6b74 6974 6c65 3d7b 6172 5869   booktitle={arXi
-000015b0: 7620 7072 6570 7269 6e74 2061 7258 6976  v preprint arXiv
-000015c0: 3a32 3330 312e 3132 3334 337d 0a20 2079  :2301.12343}.  y
-000015d0: 6561 723d 7b32 3032 337d 0a7d 0a60 6060  ear={2023}.}.```
-000015e0: 0a                                       .
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6675 6e61  : 2.1.Name: funa
+00000020: 7372 0a56 6572 7369 6f6e 3a20 302e 342e  sr.Version: 0.4.
+00000030: 320a 5375 6d6d 6172 793a 2046 756e 4153  2.Summary: FunAS
+00000040: 523a 2041 2046 756e 6461 6d65 6e74 616c  R: A Fundamental
+00000050: 2045 6e64 2d74 6f2d 456e 6420 5370 6565   End-to-End Spee
+00000060: 6368 2052 6563 6f67 6e69 7469 6f6e 2054  ch Recognition T
+00000070: 6f6f 6c6b 6974 0a48 6f6d 652d 7061 6765  oolkit.Home-page
+00000080: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000090: 2e63 6f6d 2f61 6c69 6261 6261 2d64 616d  .com/alibaba-dam
+000000a0: 6f2d 6163 6164 656d 792f 4675 6e41 5352  o-academy/FunASR
+000000b0: 2e67 6974 0a41 7574 686f 723a 2053 7065  .git.Author: Spe
+000000c0: 6563 6820 4c61 6220 6f66 2044 414d 4f20  ech Lab of DAMO 
+000000d0: 4163 6164 656d 792c 2041 6c69 6261 6261  Academy, Alibaba
+000000e0: 2047 726f 7570 0a41 7574 686f 722d 656d   Group.Author-em
+000000f0: 6169 6c3a 2066 756e 6173 7240 6c69 7374  ail: funasr@list
+00000100: 2e61 6c69 6261 6261 2d69 6e63 2e63 6f6d  .alibaba-inc.com
+00000110: 0a4c 6963 656e 7365 3a20 5468 6520 4d49  .License: The MI
+00000120: 5420 4c69 6365 6e73 650a 506c 6174 666f  T License.Platfo
+00000130: 726d 3a20 554e 4b4e 4f57 4e0a 436c 6173  rm: UNKNOWN.Clas
+00000140: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000150: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000160: 5079 7468 6f6e 0a43 6c61 7373 6966 6965  Python.Classifie
+00000170: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000180: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000190: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
+000001a0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000001b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001c0: 6e20 3a3a 2033 2e37 0a43 6c61 7373 6966  n :: 3.7.Classif
+000001d0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000001e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001f0: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
+00000200: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000210: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000220: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+00000230: 7373 6966 6965 723a 2044 6576 656c 6f70  ssifier: Develop
+00000240: 6d65 6e74 2053 7461 7475 7320 3a3a 2035  ment Status :: 5
+00000250: 202d 2050 726f 6475 6374 696f 6e2f 5374   - Production/St
+00000260: 6162 6c65 0a43 6c61 7373 6966 6965 723a  able.Classifier:
+00000270: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
+00000280: 6365 203a 3a20 5363 6965 6e63 652f 5265  ce :: Science/Re
+00000290: 7365 6172 6368 0a43 6c61 7373 6966 6965  search.Classifie
+000002a0: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+000002b0: 7465 6d20 3a3a 2050 4f53 4958 203a 3a20  tem :: POSIX :: 
+000002c0: 4c69 6e75 780a 436c 6173 7369 6669 6572  Linux.Classifier
+000002d0: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
+000002e0: 2041 7070 726f 7665 6420 3a3a 2041 7061   Approved :: Apa
+000002f0: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
+00000300: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
+00000310: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
+00000320: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
+00000330: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
+00000340: 7974 686f 6e20 4d6f 6475 6c65 730a 5265  ython Modules.Re
+00000350: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
+00000360: 3d33 2e37 2e30 0a44 6573 6372 6970 7469  =3.7.0.Descripti
+00000370: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00000380: 2074 6578 742f 6d61 726b 646f 776e 0a50   text/markdown.P
+00000390: 726f 7669 6465 732d 4578 7472 613a 2074  rovides-Extra: t
+000003a0: 7261 696e 0a50 726f 7669 6465 732d 4578  rain.Provides-Ex
+000003b0: 7472 613a 2072 6563 6970 650a 5072 6f76  tra: recipe.Prov
+000003c0: 6964 6573 2d45 7874 7261 3a20 616c 6c0a  ides-Extra: all.
+000003d0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+000003e0: 7465 7374 0a50 726f 7669 6465 732d 4578  test.Provides-Ex
+000003f0: 7472 613a 2064 6f63 0a4c 6963 656e 7365  tra: doc.License
+00000400: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
+00000410: 5b2f 2f5d 3a20 2320 283c 6469 7620 616c  [//]: # (<div al
+00000420: 6967 6e3d 226c 6566 7422 3e3c 696d 6720  ign="left"><img 
+00000430: 7372 633d 2264 6f63 732f 696d 6167 6573  src="docs/images
+00000440: 2f66 756e 6173 725f 6c6f 676f 2e6a 7067  /funasr_logo.jpg
+00000450: 2220 7769 6474 683d 2234 3030 222f 3e3c  " width="400"/><
+00000460: 2f64 6976 3e29 0a0a 2320 4675 6e41 5352  /div>)..# FunASR
+00000470: 3a20 4120 4675 6e64 616d 656e 7461 6c20  : A Fundamental 
+00000480: 456e 642d 746f 2d45 6e64 2053 7065 6563  End-to-End Speec
+00000490: 6820 5265 636f 676e 6974 696f 6e20 546f  h Recognition To
+000004a0: 6f6c 6b69 740a 3c70 2061 6c69 676e 3d22  olkit.<p align="
+000004b0: 6c65 6674 223e 0a20 2020 203c 6120 6872  left">.    <a hr
+000004c0: 6566 3d22 223e 3c69 6d67 2073 7263 3d22  ef=""><img src="
+000004d0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000004e0: 6c64 732e 696f 2f62 6164 6765 2f4f 532d  lds.io/badge/OS-
+000004f0: 4c69 6e75 7825 3243 2532 3057 696e 2532  Linux%2C%20Win%2
+00000500: 4325 3230 4d61 632d 6272 6967 6874 6772  C%20Mac-brightgr
+00000510: 6565 6e2e 7376 6722 3e3c 2f61 3e0a 2020  een.svg"></a>.  
+00000520: 2020 3c61 2068 7265 663d 2222 3e3c 696d    <a href=""><im
+00000530: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000540: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000550: 6467 652f 5079 7468 6f6e 2d3e 3d33 2e37  dge/Python->=3.7
+00000560: 2c3c 3d33 2e31 302d 6166 662e 7376 6722  ,<=3.10-aff.svg"
+00000570: 3e3c 2f61 3e0a 2020 2020 3c61 2068 7265  ></a>.    <a hre
+00000580: 663d 2222 3e3c 696d 6720 7372 633d 2268  f=""><img src="h
+00000590: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000005a0: 6473 2e69 6f2f 6261 6467 652f 5079 746f  ds.io/badge/Pyto
+000005b0: 7263 682d 2533 4525 3344 312e 3131 2d62  rch-%3E%3D1.11-b
+000005c0: 6c75 6522 3e3c 2f61 3e0a 3c2f 703e 0a0a  lue"></a>.</p>..
+000005d0: 3c73 7472 6f6e 673e 4675 6e41 5352 3c2f  <strong>FunASR</
+000005e0: 7374 726f 6e67 3e20 686f 7065 7320 746f  strong> hopes to
+000005f0: 2062 7569 6c64 2061 2062 7269 6467 6520   build a bridge 
+00000600: 6265 7477 6565 6e20 6163 6164 656d 6963  between academic
+00000610: 2072 6573 6561 7263 6820 616e 6420 696e   research and in
+00000620: 6475 7374 7269 616c 2061 7070 6c69 6361  dustrial applica
+00000630: 7469 6f6e 7320 6f6e 2073 7065 6563 6820  tions on speech 
+00000640: 7265 636f 676e 6974 696f 6e2e 2042 7920  recognition. By 
+00000650: 7375 7070 6f72 7469 6e67 2074 6865 2074  supporting the t
+00000660: 7261 696e 696e 6720 2620 6669 6e65 7475  raining & finetu
+00000670: 6e69 6e67 206f 6620 7468 6520 696e 6475  ning of the indu
+00000680: 7374 7269 616c 2d67 7261 6465 2073 7065  strial-grade spe
+00000690: 6563 6820 7265 636f 676e 6974 696f 6e20  ech recognition 
+000006a0: 6d6f 6465 6c20 7265 6c65 6173 6564 206f  model released o
+000006b0: 6e20 5b4d 6f64 656c 5363 6f70 655d 2868  n [ModelScope](h
+000006c0: 7474 7073 3a2f 2f77 7777 2e6d 6f64 656c  ttps://www.model
+000006d0: 7363 6f70 652e 636e 2f6d 6f64 656c 733f  scope.cn/models?
+000006e0: 7061 6765 3d31 2674 6173 6b73 3d61 7574  page=1&tasks=aut
+000006f0: 6f2d 7370 6565 6368 2d72 6563 6f67 6e69  o-speech-recogni
+00000700: 7469 6f6e 292c 2072 6573 6561 7263 6865  tion), researche
+00000710: 7273 2061 6e64 2064 6576 656c 6f70 6572  rs and developer
+00000720: 7320 6361 6e20 636f 6e64 7563 7420 7265  s can conduct re
+00000730: 7365 6172 6368 2061 6e64 2070 726f 6475  search and produ
+00000740: 6374 696f 6e20 6f66 2073 7065 6563 6820  ction of speech 
+00000750: 7265 636f 676e 6974 696f 6e20 6d6f 6465  recognition mode
+00000760: 6c73 206d 6f72 6520 636f 6e76 656e 6965  ls more convenie
+00000770: 6e74 6c79 2c20 616e 6420 7072 6f6d 6f74  ntly, and promot
+00000780: 6520 7468 6520 6465 7665 6c6f 706d 656e  e the developmen
+00000790: 7420 6f66 2073 7065 6563 6820 7265 636f  t of speech reco
+000007a0: 676e 6974 696f 6e20 6563 6f6c 6f67 792e  gnition ecology.
+000007b0: 2041 5352 2066 6f72 2046 756e efbc 810a   ASR for Fun....
+000007c0: 0a5b 2a2a 4e65 7773 2a2a 5d28 6874 7470  .[**News**](http
+000007d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+000007e0: 6c69 6261 6261 2d64 616d 6f2d 6163 6164  libaba-damo-acad
+000007f0: 656d 792f 4675 6e41 5352 2377 6861 7473  emy/FunASR#whats
+00000800: 2d6e 6577 2920 0a7c 205b 2a2a 4869 6768  -new) .| [**High
+00000810: 6c69 6768 7473 2a2a 5d28 2368 6967 686c  lights**](#highl
+00000820: 6967 6874 7329 0a7c 205b 2a2a 496e 7374  ights).| [**Inst
+00000830: 616c 6c61 7469 6f6e 2a2a 5d28 2369 6e73  allation**](#ins
+00000840: 7461 6c6c 6174 696f 6e29 0a7c 205b 2a2a  tallation).| [**
+00000850: 446f 6373 2a2a 5d28 6874 7470 733a 2f2f  Docs**](https://
+00000860: 616c 6962 6162 612d 6461 6d6f 2d61 6361  alibaba-damo-aca
+00000870: 6465 6d79 2e67 6974 6875 622e 696f 2f46  demy.github.io/F
+00000880: 756e 4153 522f 656e 2f69 6e64 6578 2e68  unASR/en/index.h
+00000890: 746d 6c29 0a7c 205b 2a2a 5475 746f 7269  tml).| [**Tutori
+000008a0: 616c 2a2a 5d28 6874 7470 733a 2f2f 6769  al**](https://gi
+000008b0: 7468 7562 2e63 6f6d 2f61 6c69 6261 6261  thub.com/alibaba
+000008c0: 2d64 616d 6f2d 6163 6164 656d 792f 4675  -damo-academy/Fu
+000008d0: 6e41 5352 2f77 696b 6923 6675 6e61 7372  nASR/wiki#funasr
+000008e0: 2545 3725 3934 2541 3825 4536 2538 3825  %E7%94%A8%E6%88%
+000008f0: 4237 2545 3625 3839 2538 4225 4535 2538  B7%E6%89%8B%E5%8
+00000900: 3625 3843 290a 7c20 5b2a 2a50 6170 6572  6%8C).| [**Paper
+00000910: 732a 2a5d 2868 7474 7073 3a2f 2f67 6974  s**](https://git
+00000920: 6875 622e 636f 6d2f 616c 6962 6162 612d  hub.com/alibaba-
+00000930: 6461 6d6f 2d61 6361 6465 6d79 2f46 756e  damo-academy/Fun
+00000940: 4153 5223 6369 7461 7469 6f6e 7329 0a7c  ASR#citations).|
+00000950: 205b 2a2a 5275 6e74 696d 652a 2a5d 2868   [**Runtime**](h
+00000960: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000970: 6d2f 616c 6962 6162 612d 6461 6d6f 2d61  m/alibaba-damo-a
+00000980: 6361 6465 6d79 2f46 756e 4153 522f 7472  cademy/FunASR/tr
+00000990: 6565 2f6d 6169 6e2f 6675 6e61 7372 2f72  ee/main/funasr/r
+000009a0: 756e 7469 6d65 290a 7c20 5b2a 2a4d 6f64  untime).| [**Mod
+000009b0: 656c 205a 6f6f 2a2a 5d28 6874 7470 733a  el Zoo**](https:
+000009c0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6c69  //github.com/ali
+000009d0: 6261 6261 2d64 616d 6f2d 6163 6164 656d  baba-damo-academ
+000009e0: 792f 4675 6e41 5352 2f62 6c6f 622f 6d61  y/FunASR/blob/ma
+000009f0: 696e 2f64 6f63 732f 6d6f 6465 6c73 636f  in/docs/modelsco
+00000a00: 7065 5f6d 6f64 656c 732e 6d64 290a 7c20  pe_models.md).| 
+00000a10: 5b2a 2a43 6f6e 7461 6374 2a2a 5d28 2363  [**Contact**](#c
+00000a20: 6f6e 7461 6374 290a 7c0a 5b2a 2a4d 324d  ontact).|.[**M2M
+00000a30: 4554 322e 3020 4775 6964 656e 6365 5f43  ET2.0 Guidence_C
+00000a40: 4e2a 2a5d 2868 7474 7073 3a2f 2f61 6c69  N**](https://ali
+00000a50: 6261 6261 2d64 616d 6f2d 6163 6164 656d  baba-damo-academ
+00000a60: 792e 6769 7468 7562 2e69 6f2f 4675 6e41  y.github.io/FunA
+00000a70: 5352 2f6d 326d 6574 325f 636e 2f69 6e64  SR/m2met2_cn/ind
+00000a80: 6578 2e68 746d 6c29 0a7c 205b 2a2a 4d32  ex.html).| [**M2
+00000a90: 4d45 5432 2e30 2047 7569 6465 6e63 655f  MET2.0 Guidence_
+00000aa0: 454e 2a2a 5d28 6874 7470 733a 2f2f 616c  EN**](https://al
+00000ab0: 6962 6162 612d 6461 6d6f 2d61 6361 6465  ibaba-damo-acade
+00000ac0: 6d79 2e67 6974 6875 622e 696f 2f46 756e  my.github.io/Fun
+00000ad0: 4153 522f 6d32 6d65 7432 2f69 6e64 6578  ASR/m2met2/index
+00000ae0: 2e68 746d 6c29 0a0a 2323 204d 756c 7469  .html)..## Multi
+00000af0: 2d43 6861 6e6e 656c 204d 756c 7469 2d50  -Channel Multi-P
+00000b00: 6172 7479 204d 6565 7469 6e67 2054 7261  arty Meeting Tra
+00000b10: 6e73 6372 6970 7469 6f6e 2032 2e30 2028  nscription 2.0 (
+00000b20: 4d32 4d45 5432 2e30 2920 4368 616c 6c65  M2MET2.0) Challe
+00000b30: 6e67 650a 5765 2061 7265 2070 6c65 6173  nge.We are pleas
+00000b40: 6564 2074 6f20 616e 6e6f 756e 6365 2074  ed to announce t
+00000b50: 6861 7420 7468 6520 4d32 4d65 5432 2e30  hat the M2MeT2.0
+00000b60: 2063 6861 6c6c 656e 6765 2077 696c 6c20   challenge will 
+00000b70: 6265 2068 656c 6420 696e 2074 6865 206e  be held in the n
+00000b80: 6561 7220 6675 7475 7265 2e20 5468 6520  ear future. The 
+00000b90: 6261 7365 6c69 6e65 2073 7973 7465 6d20  baseline system 
+00000ba0: 6973 2063 6f6e 6475 6374 6564 206f 6e20  is conducted on 
+00000bb0: 4675 6e41 5352 2061 6e64 2069 7320 7072  FunASR and is pr
+00000bc0: 6f76 6964 6564 2061 7320 6120 7265 6365  ovided as a rece
+00000bd0: 6970 6520 6f66 2041 6c69 4d65 6574 696e  ipe of AliMeetin
+00000be0: 6720 636f 7270 7573 2e20 466f 7220 6d6f  g corpus. For mo
+00000bf0: 7265 2064 6574 6169 6c73 2079 6f75 2063  re details you c
+00000c00: 616e 2073 6565 2074 6865 2067 7569 6465  an see the guide
+00000c10: 6e63 6520 6f66 204d 324d 4554 322e 3020  nce of M2MET2.0 
+00000c20: 285b 434e 5d28 6874 7470 733a 2f2f 616c  ([CN](https://al
+00000c30: 6962 6162 612d 6461 6d6f 2d61 6361 6465  ibaba-damo-acade
+00000c40: 6d79 2e67 6974 6875 622e 696f 2f46 756e  my.github.io/Fun
+00000c50: 4153 522f 6d32 6d65 7432 5f63 6e2f 696e  ASR/m2met2_cn/in
+00000c60: 6465 782e 6874 6d6c 292f 5b45 4e5d 2868  dex.html)/[EN](h
+00000c70: 7474 7073 3a2f 2f61 6c69 6261 6261 2d64  ttps://alibaba-d
+00000c80: 616d 6f2d 6163 6164 656d 792e 6769 7468  amo-academy.gith
+00000c90: 7562 2e69 6f2f 4675 6e41 5352 2f6d 326d  ub.io/FunASR/m2m
+00000ca0: 6574 322f 696e 6465 782e 6874 6d6c 2929  et2/index.html))
+00000cb0: 2e0a 2323 2057 6861 7427 7320 6e65 773a  ..## What's new:
+00000cc0: 200a 0a46 6f72 2074 6865 2072 656c 6561   ..For the relea
+00000cd0: 7365 206e 6f74 6573 2c20 706c 6561 7365  se notes, please
+00000ce0: 2072 6566 2074 6f20 5b6e 6577 735d 2868   ref to [news](h
+00000cf0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000d00: 6d2f 616c 6962 6162 612d 6461 6d6f 2d61  m/alibaba-damo-a
+00000d10: 6361 6465 6d79 2f46 756e 4153 522f 7265  cademy/FunASR/re
+00000d20: 6c65 6173 6573 290a 0a23 2320 4869 6768  leases)..## High
+00000d30: 6c69 6768 7473 0a2d 2046 756e 4153 5220  lights.- FunASR 
+00000d40: 7375 7070 6f72 7473 2073 7065 6563 6820  supports speech 
+00000d50: 7265 636f 676e 6974 696f 6e28 4153 5229  recognition(ASR)
+00000d60: 2c20 4d75 6c74 692d 7461 6c6b 6572 2041  , Multi-talker A
+00000d70: 5352 2c20 566f 6963 6520 4163 7469 7669  SR, Voice Activi
+00000d80: 7479 2044 6574 6563 7469 6f6e 2856 4144  ty Detection(VAD
+00000d90: 292c 2050 756e 6374 7561 7469 6f6e 2052  ), Punctuation R
+00000da0: 6573 746f 7261 7469 6f6e 2c20 4c61 6e67  estoration, Lang
+00000db0: 7561 6765 204d 6f64 656c 732c 2053 7065  uage Models, Spe
+00000dc0: 616b 6572 2056 6572 6966 6963 6174 696f  aker Verificatio
+00000dd0: 6e20 616e 6420 5370 6561 6b65 7220 6469  n and Speaker di
+00000de0: 6172 697a 6174 696f 6e2e 2020 200a 2d20  arization.   .- 
+00000df0: 5765 2068 6176 6520 7265 6c65 6173 6564  We have released
+00000e00: 206c 6172 6765 206e 756d 6265 7220 6f66   large number of
+00000e10: 2061 6361 6465 6d69 6320 616e 6420 696e   academic and in
+00000e20: 6475 7374 7269 616c 2070 7265 7472 6169  dustrial pretrai
+00000e30: 6e65 6420 6d6f 6465 6c73 206f 6e20 5b4d  ned models on [M
+00000e40: 6f64 656c 5363 6f70 655d 2868 7474 7073  odelScope](https
+00000e50: 3a2f 2f77 7777 2e6d 6f64 656c 7363 6f70  ://www.modelscop
+00000e60: 652e 636e 2f6d 6f64 656c 733f 7061 6765  e.cn/models?page
+00000e70: 3d31 2674 6173 6b73 3d61 7574 6f2d 7370  =1&tasks=auto-sp
+00000e80: 6565 6368 2d72 6563 6f67 6e69 7469 6f6e  eech-recognition
+00000e90: 290a 2d20 5468 6520 7072 6574 7261 696e  ).- The pretrain
+00000ea0: 6564 206d 6f64 656c 205b 5061 7261 666f  ed model [Parafo
+00000eb0: 726d 6572 2d6c 6172 6765 5d28 6874 7470  rmer-large](http
+00000ec0: 733a 2f2f 7777 772e 6d6f 6465 6c73 636f  s://www.modelsco
+00000ed0: 7065 2e63 6e2f 6d6f 6465 6c73 2f64 616d  pe.cn/models/dam
+00000ee0: 6f2f 7370 6565 6368 5f70 6172 6166 6f72  o/speech_parafor
+00000ef0: 6d65 722d 6c61 7267 655f 6173 725f 6e61  mer-large_asr_na
+00000f00: 742d 7a68 2d63 6e2d 3136 6b2d 636f 6d6d  t-zh-cn-16k-comm
+00000f10: 6f6e 2d76 6f63 6162 3834 3034 2d70 7974  on-vocab8404-pyt
+00000f20: 6f72 6368 2f73 756d 6d61 7279 2920 6f62  orch/summary) ob
+00000f30: 7461 696e 7320 7468 6520 6265 7374 2070  tains the best p
+00000f40: 6572 666f 726d 616e 6365 206f 6e20 6d61  erformance on ma
+00000f50: 6e79 2074 6173 6b73 2069 6e20 5b53 7065  ny tasks in [Spe
+00000f60: 6563 6849 4f20 6c65 6164 6572 626f 6172  echIO leaderboar
+00000f70: 645d 2868 7474 7073 3a2f 2f67 6974 6875  d](https://githu
+00000f80: 622e 636f 6d2f 5370 6565 6368 436f 6c61  b.com/SpeechCola
+00000f90: 622f 4c65 6164 6572 626f 6172 6429 0a2d  b/Leaderboard).-
+00000fa0: 2046 756e 4153 5220 7375 7070 6c69 6573   FunASR supplies
+00000fb0: 2061 2065 6173 792d 746f 2d75 7365 2070   a easy-to-use p
+00000fc0: 6970 656c 696e 6520 746f 2066 696e 6574  ipeline to finet
+00000fd0: 756e 6520 7072 6574 7261 696e 6564 206d  une pretrained m
+00000fe0: 6f64 656c 7320 6672 6f6d 205b 4d6f 6465  odels from [Mode
+00000ff0: 6c53 636f 7065 5d28 6874 7470 733a 2f2f  lScope](https://
+00001000: 7777 772e 6d6f 6465 6c73 636f 7065 2e63  www.modelscope.c
+00001010: 6e2f 6d6f 6465 6c73 3f70 6167 653d 3126  n/models?page=1&
+00001020: 7461 736b 733d 6175 746f 2d73 7065 6563  tasks=auto-speec
+00001030: 682d 7265 636f 676e 6974 696f 6e29 0a2d  h-recognition).-
+00001040: 2043 6f6d 7061 7265 6420 746f 205b 4573   Compared to [Es
+00001050: 706e 6574 5d28 6874 7470 733a 2f2f 6769  pnet](https://gi
+00001060: 7468 7562 2e63 6f6d 2f65 7370 6e65 742f  thub.com/espnet/
+00001070: 6573 706e 6574 2920 6672 616d 6577 6f72  espnet) framewor
+00001080: 6b2c 2074 6865 2074 7261 696e 696e 6720  k, the training 
+00001090: 7370 6565 6420 6f66 206c 6172 6765 2d73  speed of large-s
+000010a0: 6361 6c65 2064 6174 6173 6574 7320 696e  cale datasets in
+000010b0: 2046 756e 4153 5220 6973 206d 7563 6820   FunASR is much 
+000010c0: 6661 7374 6572 206f 776e 696e 6720 746f  faster owning to
+000010d0: 2074 6865 206f 7074 696d 697a 6564 2064   the optimized d
+000010e0: 6174 616c 6f61 6465 722e 0a0a 2323 2049  ataloader...## I
+000010f0: 6e73 7461 6c6c 6174 696f 6e0a 0a49 6e73  nstallation..Ins
+00001100: 7461 6c6c 2066 726f 6d20 7069 700a 6060  tall from pip.``
+00001110: 6073 6865 6c6c 0a70 6970 2069 6e73 7461  `shell.pip insta
+00001120: 6c6c 202d 5520 6675 6e61 7372 0a23 2046  ll -U funasr.# F
+00001130: 6f72 2074 6865 2075 7365 7273 2069 6e20  or the users in 
+00001140: 4368 696e 612c 2079 6f75 2063 6f75 6c64  China, you could
+00001150: 2069 6e73 7461 6c6c 2077 6974 6820 7468   install with th
+00001160: 6520 636f 6d6d 616e 643a 0a23 2070 6970  e command:.# pip
+00001170: 2069 6e73 7461 6c6c 202d 5520 6675 6e61   install -U funa
+00001180: 7372 202d 6920 6874 7470 733a 2f2f 6d69  sr -i https://mi
+00001190: 7272 6f72 2e73 6a74 752e 6564 752e 636e  rror.sjtu.edu.cn
+000011a0: 2f70 7970 692f 7765 622f 7369 6d70 6c65  /pypi/web/simple
+000011b0: 0a60 6060 0a0a 4f72 2069 6e73 7461 6c6c  .```..Or install
+000011c0: 2066 726f 6d20 736f 7572 6365 2063 6f64   from source cod
+000011d0: 650a 0a0a 6060 6020 7368 0a67 6974 2063  e...``` sh.git c
+000011e0: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+000011f0: 6875 622e 636f 6d2f 616c 6962 6162 612f  hub.com/alibaba/
+00001200: 4675 6e41 5352 2e67 6974 2026 2620 6364  FunASR.git && cd
+00001210: 2046 756e 4153 520a 7069 7020 696e 7374   FunASR.pip inst
+00001220: 616c 6c20 2d65 202e 2f0a 2320 466f 7220  all -e ./.# For 
+00001230: 7468 6520 7573 6572 7320 696e 2043 6869  the users in Chi
+00001240: 6e61 2c20 796f 7520 636f 756c 6420 696e  na, you could in
+00001250: 7374 616c 6c20 7769 7468 2074 6865 2063  stall with the c
+00001260: 6f6d 6d61 6e64 3a0a 2320 7069 7020 696e  ommand:.# pip in
+00001270: 7374 616c 6c20 2d65 202e 2f20 2d69 2068  stall -e ./ -i h
+00001280: 7474 7073 3a2f 2f6d 6972 726f 722e 736a  ttps://mirror.sj
+00001290: 7475 2e65 6475 2e63 6e2f 7079 7069 2f77  tu.edu.cn/pypi/w
+000012a0: 6562 2f73 696d 706c 650a 0a60 6060 0a49  eb/simple..```.I
+000012b0: 6620 796f 7520 7761 6e74 2074 6f20 7573  f you want to us
+000012c0: 6520 7468 6520 7072 6574 7261 696e 6564  e the pretrained
+000012d0: 206d 6f64 656c 7320 696e 204d 6f64 656c   models in Model
+000012e0: 5363 6f70 652c 2079 6f75 2073 686f 756c  Scope, you shoul
+000012f0: 6420 696e 7374 616c 6c20 7468 6520 6d6f  d install the mo
+00001300: 6465 6c73 636f 7065 3a0a 0a60 6060 7368  delscope:..```sh
+00001310: 656c 6c0a 7069 7020 696e 7374 616c 6c20  ell.pip install 
+00001320: 2d55 206d 6f64 656c 7363 6f70 650a 2320  -U modelscope.# 
+00001330: 466f 7220 7468 6520 7573 6572 7320 696e  For the users in
+00001340: 2043 6869 6e61 2c20 796f 7520 636f 756c   China, you coul
+00001350: 6420 696e 7374 616c 6c20 7769 7468 2074  d install with t
+00001360: 6865 2063 6f6d 6d61 6e64 3a0a 2320 7069  he command:.# pi
+00001370: 7020 696e 7374 616c 6c20 2d55 206d 6f64  p install -U mod
+00001380: 656c 7363 6f70 6520 2d66 2068 7474 7073  elscope -f https
+00001390: 3a2f 2f6d 6f64 656c 7363 6f70 652e 6f73  ://modelscope.os
+000013a0: 732d 636e 2d62 6569 6a69 6e67 2e61 6c69  s-cn-beijing.ali
+000013b0: 7975 6e63 732e 636f 6d2f 7265 6c65 6173  yuncs.com/releas
+000013c0: 6573 2f72 6570 6f2e 6874 6d6c 202d 6920  es/repo.html -i 
+000013d0: 6874 7470 733a 2f2f 6d69 7272 6f72 2e73  https://mirror.s
+000013e0: 6a74 752e 6564 752e 636e 2f70 7970 692f  jtu.edu.cn/pypi/
+000013f0: 7765 622f 7369 6d70 6c65 0a60 6060 0a0a  web/simple.```..
+00001400: 466f 7220 6d6f 7265 2064 6574 6169 6c73  For more details
+00001410: 2c20 706c 6561 7365 2072 6566 2074 6f20  , please ref to 
+00001420: 5b69 6e73 7461 6c6c 6174 696f 6e5d 2868  [installation](h
+00001430: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001440: 6d2f 616c 6962 6162 612d 6461 6d6f 2d61  m/alibaba-damo-a
+00001450: 6361 6465 6d79 2f46 756e 4153 522f 7769  cademy/FunASR/wi
+00001460: 6b69 290a 0a5b 2f2f 5d3a 2023 2028 290a  ki)..[//]: # ().
+00001470: 5b2f 2f5d 3a20 2320 2823 2320 5573 6167  [//]: # (## Usag
+00001480: 6529 0a0a 5b2f 2f5d 3a20 2320 2846 6f72  e)..[//]: # (For
+00001490: 2075 7365 7273 2077 686f 2061 7265 206e   users who are n
+000014a0: 6577 2074 6f20 4675 6e41 5352 2061 6e64  ew to FunASR and
+000014b0: 204d 6f64 656c 5363 6f70 652c 2070 6c65   ModelScope, ple
+000014c0: 6173 6520 7265 6665 7220 746f 2046 756e  ase refer to Fun
+000014d0: 4153 5220 446f 6373 2623 3430 3b5b 434e  ASR Docs&#40;[CN
+000014e0: 5d26 2334 303b 6874 7470 733a 2f2f 616c  ]&#40;https://al
+000014f0: 6962 6162 612d 6461 6d6f 2d61 6361 6465  ibaba-damo-acade
+00001500: 6d79 2e67 6974 6875 622e 696f 2f46 756e  my.github.io/Fun
+00001510: 4153 522f 636e 2f69 6e64 6578 2e68 746d  ASR/cn/index.htm
+00001520: 6c26 2334 313b 202f 205b 454e 5d26 2334  l&#41; / [EN]&#4
+00001530: 303b 6874 7470 733a 2f2f 616c 6962 6162  0;https://alibab
+00001540: 612d 6461 6d6f 2d61 6361 6465 6d79 2e67  a-damo-academy.g
+00001550: 6974 6875 622e 696f 2f46 756e 4153 522f  ithub.io/FunASR/
+00001560: 656e 2f69 6e64 6578 2e68 746d 6c26 2334  en/index.html&#4
+00001570: 313b 2623 3431 3b29 0a0a 2323 2043 6f6e  1;&#41;)..## Con
+00001580: 7461 6374 0a0a 4966 2079 6f75 2068 6176  tact..If you hav
+00001590: 6520 616e 7920 7175 6573 7469 6f6e 7320  e any questions 
+000015a0: 6162 6f75 7420 4675 6e41 5352 2c20 706c  about FunASR, pl
+000015b0: 6561 7365 2063 6f6e 7461 6374 2075 7320  ease contact us 
+000015c0: 6279 0a0a 2d20 656d 6169 6c3a 205b 6675  by..- email: [fu
+000015d0: 6e61 7372 406c 6973 742e 616c 6962 6162  nasr@list.alibab
+000015e0: 612d 696e 632e 636f 6d5d 2866 756e 6173  a-inc.com](funas
+000015f0: 7240 6c69 7374 2e61 6c69 6261 6261 2d69  r@list.alibaba-i
+00001600: 6e63 2e63 6f6d 290a 0a7c 4469 6e67 6469  nc.com)..|Dingdi
+00001610: 6e67 2067 726f 7570 207c 2020 2020 2020  ng group |      
+00001620: 2020 2020 2020 2020 2020 2020 2020 2057                 W
+00001630: 6563 6861 7420 6772 6f75 7020 2020 2020  echat group     
+00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001650: 207c 0a7c 3a2d 2d2d 3a7c 3a2d 2d2d 2d2d   |.|:---:|:-----
+00001660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001690: 3a7c 0a7c 3c64 6976 2061 6c69 676e 3d22  :|.|<div align="
+000016a0: 6c65 6674 223e 3c69 6d67 2073 7263 3d22  left"><img src="
+000016b0: 646f 6373 2f69 6d61 6765 732f 6469 6e67  docs/images/ding
+000016c0: 6469 6e67 2e6a 7067 2220 7769 6474 683d  ding.jpg" width=
+000016d0: 2232 3530 222f 3e20 7c20 3c69 6d67 2073  "250"/> | <img s
+000016e0: 7263 3d22 646f 6373 2f69 6d61 6765 732f  rc="docs/images/
+000016f0: 7765 6368 6174 2e70 6e67 2220 7769 6474  wechat.png" widt
+00001700: 683d 2232 3332 222f 3e3c 2f64 6976 3e20  h="232"/></div> 
+00001710: 7c0a 0a23 2320 436f 6e74 7269 6275 746f  |..## Contributo
+00001720: 7273 0a0a 7c20 3c64 6976 2061 6c69 676e  rs..| <div align
+00001730: 3d22 6c65 6674 223e 3c69 6d67 2073 7263  ="left"><img src
+00001740: 3d22 646f 6373 2f69 6d61 6765 732f 6461  ="docs/images/da
+00001750: 6d6f 2e70 6e67 2220 7769 6474 683d 2231  mo.png" width="1
+00001760: 3830 222f 3e20 7c20 3c64 6976 2061 6c69  80"/> | <div ali
+00001770: 676e 3d22 6c65 6674 223e 3c69 6d67 2073  gn="left"><img s
+00001780: 7263 3d22 646f 6373 2f69 6d61 6765 732f  rc="docs/images/
+00001790: 6e77 7075 2e70 6e67 2220 7769 6474 683d  nwpu.png" width=
+000017a0: 2232 3630 222f 3e20 7c20 3c69 6d67 2073  "260"/> | <img s
+000017b0: 7263 3d22 646f 6373 2f69 6d61 6765 732f  rc="docs/images/
+000017c0: 4465 6570 5363 6965 6e63 652e 706e 6722  DeepScience.png"
+000017d0: 2077 6964 7468 3d22 3230 3022 2f3e 203c   width="200"/> <
+000017e0: 2f64 6976 3e20 7c0a 7c3a 2d2d 2d2d 2d2d  /div> |.|:------
+000017f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001820: 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d  ---------:|:----
+00001830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  -----------:|:--
+00001870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000018a0: 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a 0a23 2320  ---------:|..## 
+000018b0: 4163 6b6e 6f77 6c65 6467 650a 0a31 2e20  Acknowledge..1. 
+000018c0: 5765 2062 6f72 726f 7765 6420 6120 6c6f  We borrowed a lo
+000018d0: 7420 6f66 2063 6f64 6520 6672 6f6d 205b  t of code from [
+000018e0: 4b61 6c64 695d 2868 7474 703a 2f2f 6b61  Kaldi](http://ka
+000018f0: 6c64 692d 6173 722e 6f72 672f 2920 666f  ldi-asr.org/) fo
+00001900: 7220 6461 7461 2070 7265 7061 7261 7469  r data preparati
+00001910: 6f6e 2e0a 322e 2057 6520 626f 7272 6f77  on..2. We borrow
+00001920: 6564 2061 206c 6f74 206f 6620 636f 6465  ed a lot of code
+00001930: 2066 726f 6d20 5b45 5350 6e65 745d 2868   from [ESPnet](h
+00001940: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001950: 6d2f 6573 706e 6574 2f65 7370 6e65 7429  m/espnet/espnet)
+00001960: 2e20 4675 6e41 5352 2066 6f6c 6c6f 7773  . FunASR follows
+00001970: 2075 7020 7468 6520 7472 6169 6e69 6e67   up the training
+00001980: 2061 6e64 2066 696e 6574 756e 696e 6720   and finetuning 
+00001990: 7069 7065 6c69 6e65 7320 6f66 2045 5350  pipelines of ESP
+000019a0: 6e65 742e 0a33 2e20 5765 2072 6566 6572  net..3. We refer
+000019b0: 7265 6420 5b57 656e 6574 5d28 6874 7470  red [Wenet](http
+000019c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f77  s://github.com/w
+000019d0: 656e 6574 2d65 3265 2f77 656e 6574 2920  enet-e2e/wenet) 
+000019e0: 666f 7220 6275 696c 6469 6e67 2064 6174  for building dat
+000019f0: 616c 6f61 6465 7220 666f 7220 6c61 7267  aloader for larg
+00001a00: 6520 7363 616c 6520 6461 7461 2074 7261  e scale data tra
+00001a10: 696e 696e 672e 0a34 2e20 5765 2061 636b  ining..4. We ack
+00001a20: 6e6f 776c 6564 6765 205b 4465 6570 5363  nowledge [DeepSc
+00001a30: 6965 6e63 655d 2868 7474 7073 3a2f 2f77  ience](https://w
+00001a40: 7777 2e64 6565 7073 6369 656e 6365 2e63  ww.deepscience.c
+00001a50: 6e29 2066 6f72 2063 6f6e 7472 6962 7574  n) for contribut
+00001a60: 696e 6720 7468 6520 6772 7063 2073 6572  ing the grpc ser
+00001a70: 7669 6365 2e0a 0a23 2320 4c69 6365 6e73  vice...## Licens
+00001a80: 650a 5468 6973 2070 726f 6a65 6374 2069  e.This project i
+00001a90: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
+00001aa0: 2074 6865 205b 5468 6520 4d49 5420 4c69   the [The MIT Li
+00001ab0: 6365 6e73 655d 2868 7474 7073 3a2f 2f6f  cense](https://o
+00001ac0: 7065 6e73 6f75 7263 652e 6f72 672f 6c69  pensource.org/li
+00001ad0: 6365 6e73 6573 2f4d 4954 292e 2046 756e  censes/MIT). Fun
+00001ae0: 4153 5220 616c 736f 2063 6f6e 7461 696e  ASR also contain
+00001af0: 7320 7661 7269 6f75 7320 7468 6972 642d  s various third-
+00001b00: 7061 7274 7920 636f 6d70 6f6e 656e 7473  party components
+00001b10: 2061 6e64 2073 6f6d 6520 636f 6465 206d   and some code m
+00001b20: 6f64 6966 6965 6420 6672 6f6d 206f 7468  odified from oth
+00001b30: 6572 2072 6570 6f73 2075 6e64 6572 206f  er repos under o
+00001b40: 7468 6572 206f 7065 6e20 736f 7572 6365  ther open source
+00001b50: 206c 6963 656e 7365 732e 0a0a 2323 2043   licenses...## C
+00001b60: 6974 6174 696f 6e73 0a0a 6060 6020 6269  itations..``` bi
+00001b70: 6274 6578 0a40 696e 7072 6f63 6565 6469  btex.@inproceedi
+00001b80: 6e67 737b 6761 6f32 3032 3270 6172 6166  ngs{gao2022paraf
+00001b90: 6f72 6d65 722c 0a20 2074 6974 6c65 3d7b  ormer,.  title={
+00001ba0: 5061 7261 666f 726d 6572 3a20 4661 7374  Paraformer: Fast
+00001bb0: 2061 6e64 2041 6363 7572 6174 6520 5061   and Accurate Pa
+00001bc0: 7261 6c6c 656c 2054 7261 6e73 666f 726d  rallel Transform
+00001bd0: 6572 2066 6f72 204e 6f6e 2d61 7574 6f72  er for Non-autor
+00001be0: 6567 7265 7373 6976 6520 456e 642d 746f  egressive End-to
+00001bf0: 2d45 6e64 2053 7065 6563 6820 5265 636f  -End Speech Reco
+00001c00: 676e 6974 696f 6e7d 2c0a 2020 6175 7468  gnition},.  auth
+00001c10: 6f72 3d7b 4761 6f2c 205a 6869 6675 2061  or={Gao, Zhifu a
+00001c20: 6e64 205a 6861 6e67 2c20 5368 696c 6961  nd Zhang, Shilia
+00001c30: 6e67 2061 6e64 204d 634c 6f75 6768 6c69  ng and McLoughli
+00001c40: 6e2c 2049 616e 2061 6e64 2059 616e 2c20  n, Ian and Yan, 
+00001c50: 5a68 696a 6965 7d2c 0a20 2062 6f6f 6b74  Zhijie},.  bookt
+00001c60: 6974 6c65 3d7b 494e 5445 5253 5045 4543  itle={INTERSPEEC
+00001c70: 487d 2c0a 2020 7965 6172 3d7b 3230 3232  H},.  year={2022
+00001c80: 7d0a 7d0a 4069 6e70 726f 6365 6564 696e  }.}.@inproceedin
+00001c90: 6773 7b67 616f 3230 3230 756e 6976 6572  gs{gao2020univer
+00001ca0: 7361 6c2c 0a20 2074 6974 6c65 3d7b 556e  sal,.  title={Un
+00001cb0: 6976 6572 7361 6c20 4153 523a 2055 6e69  iversal ASR: Uni
+00001cc0: 6679 696e 6720 5374 7265 616d 696e 6720  fying Streaming 
+00001cd0: 616e 6420 4e6f 6e2d 5374 7265 616d 696e  and Non-Streamin
+00001ce0: 6720 4153 5220 5573 696e 6720 6120 5369  g ASR Using a Si
+00001cf0: 6e67 6c65 2045 6e63 6f64 6572 2d44 6563  ngle Encoder-Dec
+00001d00: 6f64 6572 204d 6f64 656c 7d2c 0a20 2061  oder Model},.  a
+00001d10: 7574 686f 723d 7b47 616f 2c20 5a68 6966  uthor={Gao, Zhif
+00001d20: 7520 616e 6420 5a68 616e 672c 2053 6869  u and Zhang, Shi
+00001d30: 6c69 616e 6720 616e 6420 4c65 692c 204d  liang and Lei, M
+00001d40: 696e 6720 616e 6420 4d63 4c6f 7567 686c  ing and McLoughl
+00001d50: 696e 2c20 4961 6e7d 2c0a 2020 626f 6f6b  in, Ian},.  book
+00001d60: 7469 746c 653d 7b61 7258 6976 2070 7265  title={arXiv pre
+00001d70: 7072 696e 7420 6172 5869 763a 3230 3130  print arXiv:2010
+00001d80: 2e31 3430 3939 7d2c 0a20 2079 6561 723d  .14099},.  year=
+00001d90: 7b32 3032 307d 0a7d 0a40 696e 7072 6f63  {2020}.}.@inproc
+00001da0: 6565 6469 6e67 737b 5368 6932 3032 3341  eedings{Shi2023A
+00001db0: 6368 6965 7669 6e67 5450 2c0a 2020 7469  chievingTP,.  ti
+00001dc0: 746c 653d 7b41 6368 6965 7669 6e67 2054  tle={Achieving T
+00001dd0: 696d 6573 7461 6d70 2050 7265 6469 6374  imestamp Predict
+00001de0: 696f 6e20 5768 696c 6520 5265 636f 676e  ion While Recogn
+00001df0: 697a 696e 6720 7769 7468 204e 6f6e 2d41  izing with Non-A
+00001e00: 7574 6f72 6567 7265 7373 6976 6520 456e  utoregressive En
+00001e10: 642d 746f 2d45 6e64 2041 5352 204d 6f64  d-to-End ASR Mod
+00001e20: 656c 7d2c 0a20 2061 7574 686f 723d 7b58  el},.  author={X
+00001e30: 6961 6e20 5368 6920 616e 6420 5961 6e6e  ian Shi and Yann
+00001e40: 6920 4368 656e 2061 6e64 2053 6869 6c69  i Chen and Shili
+00001e50: 616e 6720 5a68 616e 6720 616e 6420 5a68  ang Zhang and Zh
+00001e60: 696a 6965 2059 616e 7d2c 0a20 2062 6f6f  ijie Yan},.  boo
+00001e70: 6b74 6974 6c65 3d7b 6172 5869 7620 7072  ktitle={arXiv pr
+00001e80: 6570 7269 6e74 2061 7258 6976 3a32 3330  eprint arXiv:230
+00001e90: 312e 3132 3334 337d 0a20 2079 6561 723d  1.12343}.  year=
+00001ea0: 7b32 3032 337d 0a7d 0a60 6060 0a0a 0a    {2023}.}.```...
```

### Comparing `funasr-0.4.1/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.4.2/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/bin/asr_inference.py` & `funasr-0.4.2/funasr/bin/asr_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,14 +342,16 @@
     ngram_weight: float = 0.9,
     nbest: int = 1,
     num_workers: int = 1,
     param_dict: dict = None,
     **kwargs,
 ):
     assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
```

### Comparing `funasr-0.4.1/funasr/bin/asr_inference_launch.py` & `funasr-0.4.2/funasr/bin/asr_inference_launch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,8 @@
 #!/usr/bin/env python3
-# Copyright ESPnet (https://github.com/espnet/espnet). All Rights Reserved.
-#  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
-
-import torch
-torch.set_num_threads(1)
 
 import argparse
 import logging
 import os
 import sys
 from typing import Union, Dict, Any
 
@@ -130,14 +125,19 @@
     )
     group.add_argument(
         "--model_tag",
         type=str,
         help="Pretrained model tag. If specify this option, *_train_config and "
              "*_file will be overwritten",
     )
+    group.add_argument(
+        "--beam_search_config",
+        default={},
+        help="The keyword arguments for transducer beam search.",
+    )
 
     group = parser.add_argument_group("Beam-search related")
     group.add_argument(
         "--batch_size",
         type=int,
         default=1,
         help="The batch size for inference",
@@ -167,14 +167,49 @@
         type=float,
         default=0.0,
         help="CTC weight in joint decoding",
     )
     group.add_argument("--lm_weight", type=float, default=1.0, help="RNNLM weight")
     group.add_argument("--ngram_weight", type=float, default=0.9, help="ngram weight")
     group.add_argument("--streaming", type=str2bool, default=False)
+    group.add_argument("--simu_streaming", type=str2bool, default=False)
+    group.add_argument("--chunk_size", type=int, default=16)
+    group.add_argument("--left_context", type=int, default=16)
+    group.add_argument("--right_context", type=int, default=0)
+    group.add_argument(
+        "--display_partial_hypotheses",
+        type=bool,
+        default=False,
+        help="Whether to display partial hypotheses during chunk-by-chunk inference.",
+    )    
+   
+    group = parser.add_argument_group("Dynamic quantization related")
+    group.add_argument(
+        "--quantize_asr_model",
+        type=bool,
+        default=False,
+        help="Apply dynamic quantization to ASR model.",
+    )
+    group.add_argument(
+        "--quantize_modules",
+        nargs="*",
+        default=None,
+        help="""Module names to apply dynamic quantization on.
+        The module names are provided as a list, where each name is separated
+        by a comma (e.g.: --quantize-config=[Linear,LSTM,GRU]).
+        Each specified name should be an attribute of 'torch.nn', e.g.:
+        torch.nn.Linear, torch.nn.LSTM, torch.nn.GRU, ...""",
+    )
+    group.add_argument(
+        "--quantize_dtype",
+        type=str,
+        default="qint8",
+        choices=["float16", "qint8"],
+        help="Dtype for dynamic quantization.",
+    )    
 
     group = parser.add_argument_group("Text converter related")
     group.add_argument(
         "--token_type",
         type=str_or_none,
         default=None,
         choices=["char", "bpe", None],
@@ -264,14 +299,17 @@
         return inference(**kwargs)
     elif mode == "vad":
         from funasr.bin.vad_inference import inference
         return inference(**kwargs)
     elif mode == "mfcca":
         from funasr.bin.asr_inference_mfcca import inference_modelscope
         return inference_modelscope(**kwargs)
+    elif mode == "rnnt":
+        from funasr.bin.asr_inference_rnnt import inference
+        return inference(**kwargs)
     else:
         logging.info("Unknown decoding mode: {}".format(mode))
         return None
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
```

### Comparing `funasr-0.4.1/funasr/bin/asr_inference_mfcca.py` & `funasr-0.4.2/funasr/bin/asr_inference_mfcca.py`

 * *Files 1% similar despite different names*

```diff
@@ -468,14 +468,16 @@
     ngram_weight: float = 0.9,
     nbest: int = 1,
     num_workers: int = 1,
     param_dict: dict = None,
     **kwargs,
 ):
     assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
```

### Comparing `funasr-0.4.1/funasr/bin/asr_inference_paraformer.py` & `funasr-0.4.2/funasr/bin/asr_inference_paraformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -608,15 +608,17 @@
         output_dir: Optional[str] = None,
         timestamp_infer_config: Union[Path, str] = None,
         timestamp_model_file: Union[Path, str] = None,
         param_dict: dict = None,
         **kwargs,
 ):
     assert check_argument_types()
-
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
+    
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
         level=log_level,
@@ -625,15 +627,17 @@
     
     export_mode = False
     if param_dict is not None:
         hotword_list_or_file = param_dict.get('hotword')
         export_mode = param_dict.get("export_mode", False)
     else:
         hotword_list_or_file = None
-
+    
+    if kwargs.get("device", None) == "cpu":
+        ngpu = 0
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
         batch_size = 1
 
     # 1. Set random-seed
```

### Comparing `funasr-0.4.1/funasr/bin/asr_inference_paraformer_streaming.py` & `funasr-0.4.2/funasr/bin/asr_inference_paraformer_streaming.py`

 * *Files 1% similar despite different names*

```diff
@@ -532,14 +532,16 @@
         nbest: int = 1,
         num_workers: int = 1,
         output_dir: Optional[str] = None,
         param_dict: dict = None,
         **kwargs,
 ):
     assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
 
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
@@ -605,14 +607,15 @@
             fs: dict = None,
             param_dict: dict = None,
             **kwargs,
     ):
 
         # 3. Build data-iterator
         is_final = False
+        cache = {}
         if param_dict is not None and "cache" in param_dict:
             cache = param_dict["cache"]
         if param_dict is not None and "is_final" in param_dict:
             is_final = param_dict["is_final"]
 
         if data_path_and_name_and_type is not None and data_path_and_name_and_type[2] == "bytes":
             raw_inputs = _load_bytes(data_path_and_name_and_type[0])
```

### Comparing `funasr-0.4.1/funasr/bin/asr_inference_paraformer_vad.py` & `funasr-0.4.2/funasr/bin/asr_inference_paraformer_vad.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,16 @@
     punc_infer_config: Optional[str] = None,
     punc_model_file: Optional[str] = None,
     outputs_dict: Optional[bool] = True,
     param_dict: dict = None,
     **kwargs,
 ):
     assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
     
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
     
     logging.basicConfig(
```

### Comparing `funasr-0.4.1/funasr/bin/asr_inference_paraformer_vad_punc.py` & `funasr-0.4.2/funasr/bin/asr_inference_paraformer_vad_punc.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,14 +480,16 @@
         punc_infer_config: Optional[str] = None,
         punc_model_file: Optional[str] = None,
         outputs_dict: Optional[bool] = True,
         param_dict: dict = None,
         **kwargs,
 ):
     assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
 
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
```

### Comparing `funasr-0.4.1/funasr/bin/asr_inference_rnnt.py` & `funasr-0.4.2/funasr/tasks/diar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,946 +1,918 @@
-#!/usr/bin/env python3
+"""
+Author: Speech Lab, Alibaba Group, China
+SOND: Speaker Overlap-aware Neural Diarization for Multi-party Meeting Analysis
+https://arxiv.org/abs/2211.10243
+TOLD: A Novel Two-Stage Overlap-Aware Framework for Speaker Diarization
+https://arxiv.org/abs/2303.05397
+"""
+
 import argparse
 import logging
-import sys
-import time
-import copy
 import os
-import codecs
-import tempfile
-import requests
 from pathlib import Path
+from typing import Callable
+from typing import Collection
+from typing import Dict
+from typing import List
 from typing import Optional
-from typing import Sequence
 from typing import Tuple
 from typing import Union
-from typing import Dict
-from typing import Any
-from typing import List
 
 import numpy as np
 import torch
+import yaml
 from typeguard import check_argument_types
+from typeguard import check_return_type
 
-from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.modules.beam_search.beam_search import BeamSearchPara as BeamSearch
-from funasr.modules.beam_search.beam_search import Hypothesis
-from funasr.modules.scorers.ctc import CTCPrefixScorer
-from funasr.modules.scorers.length_bonus import LengthBonus
-from funasr.modules.subsampling import TooShortUttError
-from funasr.tasks.asr import ASRTaskParaformer as ASRTask
-from funasr.tasks.lm import LMTask
-from funasr.text.build_tokenizer import build_tokenizer
-from funasr.text.token_id_converter import TokenIDConverter
-from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
+from funasr.datasets.collate_fn import CommonCollateFn
+from funasr.datasets.preprocessor import CommonPreprocessor
+from funasr.layers.abs_normalize import AbsNormalize
+from funasr.layers.global_mvn import GlobalMVN
+from funasr.layers.label_aggregation import LabelAggregate
+from funasr.layers.utterance_mvn import UtteranceMVN
+from funasr.models.e2e_diar_sond import DiarSondModel
+from funasr.models.e2e_diar_eend_ola import DiarEENDOLAModel
+from funasr.models.encoder.abs_encoder import AbsEncoder
+from funasr.models.encoder.conformer_encoder import ConformerEncoder
+from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
+from funasr.models.encoder.ecapa_tdnn_encoder import ECAPA_TDNN
+from funasr.models.encoder.opennmt_encoders.ci_scorers import DotScorer, CosScorer
+from funasr.models.encoder.opennmt_encoders.conv_encoder import ConvEncoder
+from funasr.models.encoder.opennmt_encoders.fsmn_encoder import FsmnEncoder
+from funasr.models.encoder.opennmt_encoders.self_attention_encoder import SelfAttentionEncoder
+from funasr.models.encoder.resnet34_encoder import ResNet34Diar, ResNet34SpL2RegDiar
+from funasr.models.encoder.rnn_encoder import RNNEncoder
+from funasr.models.encoder.sanm_encoder import SANMEncoder, SANMEncoderChunkOpt
+from funasr.models.encoder.transformer_encoder import TransformerEncoder
+from funasr.models.frontend.abs_frontend import AbsFrontend
+from funasr.models.frontend.default import DefaultFrontend
+from funasr.models.frontend.fused import FusedFrontends
+from funasr.models.frontend.s3prl import S3prlFrontend
+from funasr.models.frontend.wav_frontend import WavFrontend
+from funasr.models.frontend.wav_frontend import WavFrontendMel23
+from funasr.models.frontend.windowing import SlidingWindow
+from funasr.models.specaug.abs_specaug import AbsSpecAug
+from funasr.models.specaug.specaug import SpecAug
+from funasr.models.specaug.specaug import SpecAugLFR
+from funasr.modules.eend_ola.encoder import EENDOLATransformerEncoder
+from funasr.modules.eend_ola.encoder_decoder_attractor import EncoderDecoderAttractor
+from funasr.tasks.abs_task import AbsTask
+from funasr.torch_utils.initialize import initialize
+from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.train.class_choices import ClassChoices
+from funasr.train.trainer import Trainer
+from funasr.utils.types import float_or_none
+from funasr.utils.types import int_or_none
 from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.utils import asr_utils, wav_utils, postprocess_utils
-from funasr.models.frontend.wav_frontend import WavFrontend
-from funasr.models.e2e_asr_paraformer import BiCifParaformer, ContextualParaformer
-from funasr.export.models.e2e_asr_paraformer import Paraformer as Paraformer_export
 
+frontend_choices = ClassChoices(
+    name="frontend",
+    classes=dict(
+        default=DefaultFrontend,
+        sliding_window=SlidingWindow,
+        s3prl=S3prlFrontend,
+        fused=FusedFrontends,
+        wav_frontend=WavFrontend,
+        wav_frontend_mel23=WavFrontendMel23,
+    ),
+    type_check=AbsFrontend,
+    default="default",
+)
+specaug_choices = ClassChoices(
+    name="specaug",
+    classes=dict(
+        specaug=SpecAug,
+        specaug_lfr=SpecAugLFR,
+    ),
+    type_check=AbsSpecAug,
+    default=None,
+    optional=True,
+)
+normalize_choices = ClassChoices(
+    "normalize",
+    classes=dict(
+        global_mvn=GlobalMVN,
+        utterance_mvn=UtteranceMVN,
+    ),
+    type_check=AbsNormalize,
+    default=None,
+    optional=True,
+)
+label_aggregator_choices = ClassChoices(
+    "label_aggregator",
+    classes=dict(
+        label_aggregator=LabelAggregate
+    ),
+    type_check=torch.nn.Module,
+    default=None,
+    optional=True,
+)
+model_choices = ClassChoices(
+    "model",
+    classes=dict(
+        sond=DiarSondModel,
+        eend_ola=DiarEENDOLAModel,
+    ),
+    type_check=AbsESPnetModel,
+    default="sond",
+)
+encoder_choices = ClassChoices(
+    "encoder",
+    classes=dict(
+        conformer=ConformerEncoder,
+        transformer=TransformerEncoder,
+        rnn=RNNEncoder,
+        sanm=SANMEncoder,
+        san=SelfAttentionEncoder,
+        fsmn=FsmnEncoder,
+        conv=ConvEncoder,
+        resnet34=ResNet34Diar,
+        resnet34_sp_l2reg=ResNet34SpL2RegDiar,
+        sanm_chunk_opt=SANMEncoderChunkOpt,
+        data2vec_encoder=Data2VecEncoder,
+        ecapa_tdnn=ECAPA_TDNN,
+        eend_ola_transformer=EENDOLATransformerEncoder,
+    ),
+    type_check=torch.nn.Module,
+    default="resnet34",
+)
+speaker_encoder_choices = ClassChoices(
+    "speaker_encoder",
+    classes=dict(
+        conformer=ConformerEncoder,
+        transformer=TransformerEncoder,
+        rnn=RNNEncoder,
+        sanm=SANMEncoder,
+        san=SelfAttentionEncoder,
+        fsmn=FsmnEncoder,
+        conv=ConvEncoder,
+        sanm_chunk_opt=SANMEncoderChunkOpt,
+        data2vec_encoder=Data2VecEncoder,
+    ),
+    type_check=AbsEncoder,
+    default=None,
+    optional=True
+)
+cd_scorer_choices = ClassChoices(
+    "cd_scorer",
+    classes=dict(
+        san=SelfAttentionEncoder,
+    ),
+    type_check=AbsEncoder,
+    default=None,
+    optional=True,
+)
+ci_scorer_choices = ClassChoices(
+    "ci_scorer",
+    classes=dict(
+        dot=DotScorer,
+        cosine=CosScorer,
+        conv=ConvEncoder,
+    ),
+    type_check=torch.nn.Module,
+    default=None,
+    optional=True,
+)
+# decoder is used for output (e.g. post_net in SOND)
+decoder_choices = ClassChoices(
+    "decoder",
+    classes=dict(
+        rnn=RNNEncoder,
+        fsmn=FsmnEncoder,
+    ),
+    type_check=torch.nn.Module,
+    default="fsmn",
+)
+# encoder_decoder_attractor is used for EEND-OLA
+encoder_decoder_attractor_choices = ClassChoices(
+    "encoder_decoder_attractor",
+    classes=dict(
+        eda=EncoderDecoderAttractor,
+    ),
+    type_check=torch.nn.Module,
+    default="eda",
+)
+
+
+class DiarTask(AbsTask):
+    # If you need more than 1 optimizer, change this value
+    num_optimizers: int = 1
+
+    # Add variable objects configurations
+    class_choices_list = [
+        # --frontend and --frontend_conf
+        frontend_choices,
+        # --specaug and --specaug_conf
+        specaug_choices,
+        # --normalize and --normalize_conf
+        normalize_choices,
+        # --label_aggregator and --label_aggregator_conf
+        label_aggregator_choices,
+        # --model and --model_conf
+        model_choices,
+        # --encoder and --encoder_conf
+        encoder_choices,
+        # --speaker_encoder and --speaker_encoder_conf
+        speaker_encoder_choices,
+        # --cd_scorer and cd_scorer_conf
+        cd_scorer_choices,
+        # --ci_scorer and ci_scorer_conf
+        ci_scorer_choices,
+        # --decoder and --decoder_conf
+        decoder_choices,
+    ]
+
+    # If you need to modify train() or eval() procedures, change Trainer class here
+    trainer = Trainer
+
+    @classmethod
+    def add_task_arguments(cls, parser: argparse.ArgumentParser):
+        group = parser.add_argument_group(description="Task related")
+
+        # NOTE(kamo): add_arguments(..., required=True) can't be used
+        # to provide --print_config mode. Instead of it, do as
+        # required = parser.get_default("required")
+        # required += ["token_list"]
+
+        group.add_argument(
+            "--token_list",
+            type=str_or_none,
+            default=None,
+            help="A text mapping int-id to token",
+        )
+        group.add_argument(
+            "--split_with_space",
+            type=str2bool,
+            default=True,
+            help="whether to split text using <space>",
+        )
+        group.add_argument(
+            "--seg_dict_file",
+            type=str,
+            default=None,
+            help="seg_dict_file for text processing",
+        )
+        group.add_argument(
+            "--init",
+            type=lambda x: str_or_none(x.lower()),
+            default=None,
+            help="The initialization method",
+            choices=[
+                "chainer",
+                "xavier_uniform",
+                "xavier_normal",
+                "kaiming_uniform",
+                "kaiming_normal",
+                None,
+            ],
+        )
 
-class Speech2Text:
-    """Speech2Text class
+        group.add_argument(
+            "--input_size",
+            type=int_or_none,
+            default=None,
+            help="The number of input dimension of the feature",
+        )
 
-    Examples:
-            >>> import soundfile
-            >>> speech2text = Speech2Text("asr_config.yml", "asr.pb")
-            >>> audio, rate = soundfile.read("speech.wav")
-            >>> speech2text(audio)
-            [(text, token, token_int, hypothesis object), ...]
-
-    """
-
-    def __init__(
-            self,
-            asr_train_config: Union[Path, str] = None,
-            asr_model_file: Union[Path, str] = None,
-            cmvn_file: Union[Path, str] = None,
-            lm_train_config: Union[Path, str] = None,
-            lm_file: Union[Path, str] = None,
-            token_type: str = None,
-            bpemodel: str = None,
-            device: str = "cpu",
-            maxlenratio: float = 0.0,
-            minlenratio: float = 0.0,
-            dtype: str = "float32",
-            beam_size: int = 20,
-            ctc_weight: float = 0.5,
-            lm_weight: float = 1.0,
-            ngram_weight: float = 0.9,
-            penalty: float = 0.0,
-            nbest: int = 1,
-            frontend_conf: dict = None,
-            hotword_list_or_file: str = None,
-            **kwargs,
-    ):
+        group = parser.add_argument_group(description="Preprocess related")
+        group.add_argument(
+            "--use_preprocessor",
+            type=str2bool,
+            default=True,
+            help="Apply preprocessing to data or not",
+        )
+        group.add_argument(
+            "--token_type",
+            type=str,
+            default="char",
+            choices=["char"],
+            help="The text will be tokenized in the specified level token",
+        )
+        parser.add_argument(
+            "--speech_volume_normalize",
+            type=float_or_none,
+            default=None,
+            help="Scale the maximum amplitude to the given value.",
+        )
+        parser.add_argument(
+            "--rir_scp",
+            type=str_or_none,
+            default=None,
+            help="The file path of rir scp file.",
+        )
+        parser.add_argument(
+            "--rir_apply_prob",
+            type=float,
+            default=1.0,
+            help="THe probability for applying RIR convolution.",
+        )
+        parser.add_argument(
+            "--cmvn_file",
+            type=str_or_none,
+            default=None,
+            help="The file path of noise scp file.",
+        )
+        parser.add_argument(
+            "--noise_scp",
+            type=str_or_none,
+            default=None,
+            help="The file path of noise scp file.",
+        )
+        parser.add_argument(
+            "--noise_apply_prob",
+            type=float,
+            default=1.0,
+            help="The probability applying Noise adding.",
+        )
+        parser.add_argument(
+            "--noise_db_range",
+            type=str,
+            default="13_15",
+            help="The range of noise decibel level.",
+        )
+
+        for class_choices in cls.class_choices_list:
+            # Append --<name> and --<name>_conf.
+            # e.g. --encoder and --encoder_conf
+            class_choices.add_arguments(group)
+
+    @classmethod
+    def build_collate_fn(
+            cls, args: argparse.Namespace, train: bool
+    ) -> Callable[
+        [Collection[Tuple[str, Dict[str, np.ndarray]]]],
+        Tuple[List[str], Dict[str, torch.Tensor]],
+    ]:
         assert check_argument_types()
+        # NOTE(kamo): int value = 0 is reserved by CTC-blank symbol
+        return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
 
-        # 1. Build ASR model
-        scorers = {}
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file, device
-        )
-        frontend = None
-        if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
-            frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
-
-        logging.info("asr_model: {}".format(asr_model))
-        logging.info("asr_train_args: {}".format(asr_train_args))
-        asr_model.to(dtype=getattr(torch, dtype)).eval()
-
-        if asr_model.ctc != None:
-            ctc = CTCPrefixScorer(ctc=asr_model.ctc, eos=asr_model.eos)
-            scorers.update(
-                ctc=ctc
+    @classmethod
+    def build_preprocess_fn(
+            cls, args: argparse.Namespace, train: bool
+    ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
+        assert check_argument_types()
+        if args.use_preprocessor:
+            retval = CommonPreprocessor(
+                train=train,
+                token_type=args.token_type,
+                token_list=args.token_list,
+                bpemodel=None,
+                non_linguistic_symbols=None,
+                text_cleaner=None,
+                g2p_type=None,
+                split_with_space=args.split_with_space if hasattr(args, "split_with_space") else False,
+                seg_dict_file=args.seg_dict_file if hasattr(args, "seg_dict_file") else None,
+                # NOTE(kamo): Check attribute existence for backward compatibility
+                rir_scp=args.rir_scp if hasattr(args, "rir_scp") else None,
+                rir_apply_prob=args.rir_apply_prob
+                if hasattr(args, "rir_apply_prob")
+                else 1.0,
+                noise_scp=args.noise_scp if hasattr(args, "noise_scp") else None,
+                noise_apply_prob=args.noise_apply_prob
+                if hasattr(args, "noise_apply_prob")
+                else 1.0,
+                noise_db_range=args.noise_db_range
+                if hasattr(args, "noise_db_range")
+                else "13_15",
+                speech_volume_normalize=args.speech_volume_normalize
+                if hasattr(args, "rir_scp")
+                else None,
             )
-        token_list = asr_model.token_list
-        scorers.update(
-            length_bonus=LengthBonus(len(token_list)),
-        )
+        else:
+            retval = None
+        assert check_return_type(retval)
+        return retval
+
+    @classmethod
+    def required_data_names(
+            cls, train: bool = True, inference: bool = False
+    ) -> Tuple[str, ...]:
+        if not inference:
+            retval = ("speech", "profile", "binary_labels")
+        else:
+            # Recognition mode
+            retval = ("speech", "profile")
+        return retval
+
+    @classmethod
+    def optional_data_names(
+            cls, train: bool = True, inference: bool = False
+    ) -> Tuple[str, ...]:
+        retval = ()
+        assert check_return_type(retval)
+        return retval
 
-        # 2. Build Language model
-        if lm_train_config is not None:
-            lm, lm_train_args = LMTask.build_model_from_file(
-                lm_train_config, lm_file, device
-            )
-            scorers["lm"] = lm.lm
+    @classmethod
+    def build_model(cls, args: argparse.Namespace):
+        assert check_argument_types()
+        if isinstance(args.token_list, str):
+            with open(args.token_list, encoding="utf-8") as f:
+                token_list = [line.rstrip() for line in f]
+
+            # Overwriting token_list to keep it as "portable".
+            args.token_list = list(token_list)
+        elif isinstance(args.token_list, (tuple, list)):
+            token_list = list(args.token_list)
+        else:
+            raise RuntimeError("token_list must be str or list")
+        vocab_size = len(token_list)
+        logging.info(f"Vocabulary size: {vocab_size}")
+
+        # 1. frontend
+        if args.input_size is None:
+            # Extract features in the model
+            frontend_class = frontend_choices.get_class(args.frontend)
+            if args.frontend == 'wav_frontend':
+                frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
+            else:
+                frontend = frontend_class(**args.frontend_conf)
+            input_size = frontend.output_size()
+        else:
+            # Give features from data-loader
+            args.frontend = None
+            args.frontend_conf = {}
+            frontend = None
+            input_size = args.input_size
+
+        # 2. Data augmentation for spectrogram
+        if args.specaug is not None:
+            specaug_class = specaug_choices.get_class(args.specaug)
+            specaug = specaug_class(**args.specaug_conf)
+        else:
+            specaug = None
+
+        # 3. Normalization layer
+        if args.normalize is not None:
+            normalize_class = normalize_choices.get_class(args.normalize)
+            normalize = normalize_class(**args.normalize_conf)
+        else:
+            normalize = None
+
+        # 4. Encoder
+        encoder_class = encoder_choices.get_class(args.encoder)
+        encoder = encoder_class(input_size=input_size, **args.encoder_conf)
+
+        # 5. speaker encoder
+        if getattr(args, "speaker_encoder", None) is not None:
+            speaker_encoder_class = speaker_encoder_choices.get_class(args.speaker_encoder)
+            speaker_encoder = speaker_encoder_class(**args.speaker_encoder_conf)
+        else:
+            speaker_encoder = None
 
-        # 3. Build ngram model
-        # ngram is not supported now
-        ngram = None
-        scorers["ngram"] = ngram
-
-        # 4. Build BeamSearch object
-        # transducer is not supported now
-        beam_search_transducer = None
-
-        weights = dict(
-            decoder=1.0 - ctc_weight,
-            ctc=ctc_weight,
-            lm=lm_weight,
-            ngram=ngram_weight,
-            length_bonus=penalty,
-        )
-        beam_search = BeamSearch(
-            beam_size=beam_size,
-            weights=weights,
-            scorers=scorers,
-            sos=asr_model.sos,
-            eos=asr_model.eos,
-            vocab_size=len(token_list),
+        # 6. CI & CD scorer
+        if getattr(args, "ci_scorer", None) is not None:
+            ci_scorer_class = ci_scorer_choices.get_class(args.ci_scorer)
+            ci_scorer = ci_scorer_class(**args.ci_scorer_conf)
+        else:
+            ci_scorer = None
+
+        if getattr(args, "cd_scorer", None) is not None:
+            cd_scorer_class = cd_scorer_choices.get_class(args.cd_scorer)
+            cd_scorer = cd_scorer_class(**args.cd_scorer_conf)
+        else:
+            cd_scorer = None
+
+        # 7. Decoder
+        decoder_class = decoder_choices.get_class(args.decoder)
+        decoder = decoder_class(**args.decoder_conf)
+
+        if getattr(args, "label_aggregator", None) is not None:
+            label_aggregator_class = label_aggregator_choices.get_class(args.label_aggregator)
+            label_aggregator = label_aggregator_class(**args.label_aggregator_conf)
+        else:
+            label_aggregator = None
+
+        # 9. Build model
+        model_class = model_choices.get_class(args.model)
+        model = model_class(
+            vocab_size=vocab_size,
+            frontend=frontend,
+            specaug=specaug,
+            normalize=normalize,
+            label_aggregator=label_aggregator,
+            encoder=encoder,
+            speaker_encoder=speaker_encoder,
+            ci_scorer=ci_scorer,
+            cd_scorer=cd_scorer,
+            decoder=decoder,
             token_list=token_list,
-            pre_beam_score_key=None if ctc_weight == 1.0 else "full",
+            **args.model_conf,
         )
 
-        beam_search.to(device=device, dtype=getattr(torch, dtype)).eval()
-        for scorer in scorers.values():
-            if isinstance(scorer, torch.nn.Module):
-                scorer.to(device=device, dtype=getattr(torch, dtype)).eval()
-
-        logging.info(f"Decoding device={device}, dtype={dtype}")
-
-        # 5. [Optional] Build Text converter: e.g. bpe-sym -> Text
-        if token_type is None:
-            token_type = asr_train_args.token_type
-        if bpemodel is None:
-            bpemodel = asr_train_args.bpemodel
-
-        if token_type is None:
-            tokenizer = None
-        elif token_type == "bpe":
-            if bpemodel is not None:
-                tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
-            else:
-                tokenizer = None
-        else:
-            tokenizer = build_tokenizer(token_type=token_type)
-        converter = TokenIDConverter(token_list=token_list)
-        logging.info(f"Text tokenizer: {tokenizer}")
-
-        self.asr_model = asr_model
-        self.asr_train_args = asr_train_args
-        self.converter = converter
-        self.tokenizer = tokenizer
-
-        # 6. [Optional] Build hotword list from str, local file or url
-        self.hotword_list = None
-        self.hotword_list = self.generate_hotwords_list(hotword_list_or_file)
-
-        is_use_lm = lm_weight != 0.0 and lm_file is not None
-        if (ctc_weight == 0.0 or asr_model.ctc == None) and not is_use_lm:
-            beam_search = None
-        self.beam_search = beam_search
-        logging.info(f"Beam_search: {self.beam_search}")
-        self.beam_search_transducer = beam_search_transducer
-        self.maxlenratio = maxlenratio
-        self.minlenratio = minlenratio
-        self.device = device
-        self.dtype = dtype
-        self.nbest = nbest
-        self.frontend = frontend
-        self.encoder_downsampling_factor = 1
-        if asr_train_args.encoder == "data2vec_encoder" or asr_train_args.encoder_conf["input_layer"] == "conv2d":
-            self.encoder_downsampling_factor = 4
-
-    @torch.no_grad()
-    def __call__(
-            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None
+        # 10. Initialize
+        if args.init is not None:
+            initialize(model, args.init)
+
+        assert check_return_type(model)
+        return model
+
+    # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
+    @classmethod
+    def build_model_from_file(
+            cls,
+            config_file: Union[Path, str] = None,
+            model_file: Union[Path, str] = None,
+            cmvn_file: Union[Path, str] = None,
+            device: Union[str, torch.device] = "cpu",
     ):
-        """Inference
+        """Build model from the files.
+
+        This method is used for inference or fine-tuning.
 
         Args:
-                speech: Input speech data
-        Returns:
-                text, token, token_int, hyp
+            config_file: The yaml file saved when training.
+            model_file: The model file saved when training.
+            cmvn_file: The cmvn file for front-end
+            device: Device type, "cpu", "cuda", or "cuda:N".
 
         """
         assert check_argument_types()
+        if config_file is None:
+            assert model_file is not None, (
+                "The argument 'model_file' must be provided "
+                "if the argument 'config_file' is not specified."
+            )
+            config_file = Path(model_file).parent / "config.yaml"
+        else:
+            config_file = Path(config_file)
 
-        # Input as audio signal
-        if isinstance(speech, np.ndarray):
-            speech = torch.tensor(speech)
-
-        if self.frontend is not None:
-            feats, feats_len = self.frontend.forward(speech, speech_lengths)
-            feats = to_device(feats, device=self.device)
-            feats_len = feats_len.int()
-            self.asr_model.frontend = None
-        else:
-            feats = speech
-            feats_len = speech_lengths
-        lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
-        batch = {"speech": feats, "speech_lengths": feats_len}
-
-        # a. To device
-        batch = to_device(batch, device=self.device)
-
-        # b. Forward Encoder
-        enc, enc_len = self.asr_model.encode(**batch)
-        if isinstance(enc, tuple):
-            enc = enc[0]
-        # assert len(enc) == 1, len(enc)
-        enc_len_batch_total = torch.sum(enc_len).item() * self.encoder_downsampling_factor
-
-        predictor_outs = self.asr_model.calc_predictor(enc, enc_len)
-        pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index = predictor_outs[0], predictor_outs[1], \
-                                                                        predictor_outs[2], predictor_outs[3]
-        pre_token_length = pre_token_length.round().long()
-        if torch.max(pre_token_length) < 1:
-            return []
-        if not isinstance(self.asr_model, ContextualParaformer):
-            if self.hotword_list:
-                logging.warning("Hotword is given but asr model is not a ContextualParaformer.")
-            decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds, pre_token_length)
-            decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
-        else:
-            decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds, pre_token_length, hw_list=self.hotword_list)
-            decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
-
-        results = []
-        b, n, d = decoder_out.size()
-        for i in range(b):
-            x = enc[i, :enc_len[i], :]
-            am_scores = decoder_out[i, :pre_token_length[i], :]
-            if self.beam_search is not None:
-                nbest_hyps = self.beam_search(
-                    x=x, am_scores=am_scores, maxlenratio=self.maxlenratio, minlenratio=self.minlenratio
-                )
-
-                nbest_hyps = nbest_hyps[: self.nbest]
-            else:
-                yseq = am_scores.argmax(dim=-1)
-                score = am_scores.max(dim=-1)[0]
-                score = torch.sum(score, dim=-1)
-                # pad with mask tokens to ensure compatibility with sos/eos tokens
-                yseq = torch.tensor(
-                    [self.asr_model.sos] + yseq.tolist() + [self.asr_model.eos], device=yseq.device
-                )
-                nbest_hyps = [Hypothesis(yseq=yseq, score=score)]
-
-            for hyp in nbest_hyps:
-                assert isinstance(hyp, (Hypothesis)), type(hyp)
-
-                # remove sos/eos and get results
-                last_pos = -1
-                if isinstance(hyp.yseq, list):
-                    token_int = hyp.yseq[1:last_pos]
+        with config_file.open("r", encoding="utf-8") as f:
+            args = yaml.safe_load(f)
+        if cmvn_file is not None:
+            args["cmvn_file"] = cmvn_file
+        args = argparse.Namespace(**args)
+        model = cls.build_model(args)
+        if not isinstance(model, AbsESPnetModel):
+            raise RuntimeError(
+                f"model must inherit {AbsESPnetModel.__name__}, but got {type(model)}"
+            )
+        model.to(device)
+        model_dict = dict()
+        model_name_pth = None
+        if model_file is not None:
+            logging.info("model_file is {}".format(model_file))
+            if device == "cuda":
+                device = f"cuda:{torch.cuda.current_device()}"
+            model_dir = os.path.dirname(model_file)
+            model_name = os.path.basename(model_file)
+            if "model.ckpt-" in model_name or ".bin" in model_name:
+                if ".bin" in model_name:
+                    model_name_pth = os.path.join(model_dir, model_name.replace('.bin', '.pb'))
                 else:
-                    token_int = hyp.yseq[1:last_pos].tolist()
-
-                # remove blank symbol id, which is assumed to be 0
-                token_int = list(filter(lambda x: x != 0 and x != 2, token_int))
-
-                # Change integer-ids to tokens
-                token = self.converter.ids2tokens(token_int)
-
-                if self.tokenizer is not None:
-                    text = self.tokenizer.tokens2text(token)
+                    model_name_pth = os.path.join(model_dir, "{}.pb".format(model_name))
+                if os.path.exists(model_name_pth):
+                    logging.info("model_file is load from pth: {}".format(model_name_pth))
+                    model_dict = torch.load(model_name_pth, map_location=device)
                 else:
-                    text = None
-
-                results.append((text, token, token_int, hyp, enc_len_batch_total, lfr_factor))
-
-        # assert check_return_type(results)
-        return results
-
-    def generate_hotwords_list(self, hotword_list_or_file):
-        # for None
-        if hotword_list_or_file is None:
-            hotword_list = None
-        # for local txt inputs
-        elif os.path.exists(hotword_list_or_file) and hotword_list_or_file.endswith('.txt'):
-            logging.info("Attempting to parse hotwords from local txt...")
-            hotword_list = []
-            hotword_str_list = []
-            with codecs.open(hotword_list_or_file, 'r') as fin:
-                for line in fin.readlines():
-                    hw = line.strip()
-                    hotword_str_list.append(hw)
-                    hotword_list.append(self.converter.tokens2ids([i for i in hw]))
-                hotword_list.append([self.asr_model.sos])
-                hotword_str_list.append('<s>')
-            logging.info("Initialized hotword list from file: {}, hotword list: {}."
-                         .format(hotword_list_or_file, hotword_str_list))
-        # for url, download and generate txt
-        elif hotword_list_or_file.startswith('http'):
-            logging.info("Attempting to parse hotwords from url...")
-            work_dir = tempfile.TemporaryDirectory().name
-            if not os.path.exists(work_dir):
-                os.makedirs(work_dir)
-            text_file_path = os.path.join(work_dir, os.path.basename(hotword_list_or_file))
-            local_file = requests.get(hotword_list_or_file)
-            open(text_file_path, "wb").write(local_file.content)
-            hotword_list_or_file = text_file_path
-            hotword_list = []
-            hotword_str_list = []
-            with codecs.open(hotword_list_or_file, 'r') as fin:
-                for line in fin.readlines():
-                    hw = line.strip()
-                    hotword_str_list.append(hw)
-                    hotword_list.append(self.converter.tokens2ids([i for i in hw]))
-                hotword_list.append([self.asr_model.sos])
-                hotword_str_list.append('<s>')
-            logging.info("Initialized hotword list from file: {}, hotword list: {}."
-                         .format(hotword_list_or_file, hotword_str_list))
-        # for text str input
-        elif not hotword_list_or_file.endswith('.txt'):
-            logging.info("Attempting to parse hotwords as str...")
-            hotword_list = []
-            hotword_str_list = []
-            for hw in hotword_list_or_file.strip().split():
-                hotword_str_list.append(hw)
-                hotword_list.append(self.converter.tokens2ids([i for i in hw]))
-            hotword_list.append([self.asr_model.sos])
-            hotword_str_list.append('<s>')
-            logging.info("Hotword list: {}.".format(hotword_str_list))
-        else:
-            hotword_list = None
-        return hotword_list
-
-class Speech2TextExport:
-    """Speech2TextExport class
-
-    """
-
-    def __init__(
-            self,
-            asr_train_config: Union[Path, str] = None,
-            asr_model_file: Union[Path, str] = None,
-            cmvn_file: Union[Path, str] = None,
-            lm_train_config: Union[Path, str] = None,
-            lm_file: Union[Path, str] = None,
-            token_type: str = None,
-            bpemodel: str = None,
-            device: str = "cpu",
-            maxlenratio: float = 0.0,
-            minlenratio: float = 0.0,
-            dtype: str = "float32",
-            beam_size: int = 20,
-            ctc_weight: float = 0.5,
-            lm_weight: float = 1.0,
-            ngram_weight: float = 0.9,
-            penalty: float = 0.0,
-            nbest: int = 1,
-            frontend_conf: dict = None,
-            hotword_list_or_file: str = None,
-            **kwargs,
+                    model_dict = cls.convert_tf2torch(model, model_file)
+                model.load_state_dict(model_dict)
+            else:
+                model_dict = torch.load(model_file, map_location=device)
+        model_dict = cls.fileter_model_dict(model_dict, model.state_dict())
+        model.load_state_dict(model_dict)
+        if model_name_pth is not None and not os.path.exists(model_name_pth):
+            torch.save(model_dict, model_name_pth)
+            logging.info("model_file is saved to pth: {}".format(model_name_pth))
+
+        return model, args
+
+    @classmethod
+    def fileter_model_dict(cls, src_dict: dict, dest_dict: dict):
+        from collections import OrderedDict
+        new_dict = OrderedDict()
+        for key, value in src_dict.items():
+            if key in dest_dict:
+                new_dict[key] = value
+            else:
+                logging.info("{} is no longer needed in this model.".format(key))
+        for key, value in dest_dict.items():
+            if key not in new_dict:
+                logging.warning("{} is missed in checkpoint.".format(key))
+        return new_dict
+
+    @classmethod
+    def convert_tf2torch(
+            cls,
+            model,
+            ckpt,
     ):
-
-        # 1. Build ASR model
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file, device
+        logging.info("start convert tf model to torch model")
+        from funasr.modules.streaming_utils.load_fr_tf import load_tf_dict
+        var_dict_tf = load_tf_dict(ckpt)
+        var_dict_torch = model.state_dict()
+        var_dict_torch_update = dict()
+        # speech encoder
+        if model.encoder is not None:
+            var_dict_torch_update_local = model.encoder.convert_tf2torch(var_dict_tf, var_dict_torch)
+            var_dict_torch_update.update(var_dict_torch_update_local)
+        # speaker encoder
+        if model.speaker_encoder is not None:
+            var_dict_torch_update_local = model.speaker_encoder.convert_tf2torch(var_dict_tf, var_dict_torch)
+            var_dict_torch_update.update(var_dict_torch_update_local)
+        # cd scorer
+        if model.cd_scorer is not None:
+            var_dict_torch_update_local = model.cd_scorer.convert_tf2torch(var_dict_tf, var_dict_torch)
+            var_dict_torch_update.update(var_dict_torch_update_local)
+        # ci scorer
+        if model.ci_scorer is not None:
+            var_dict_torch_update_local = model.ci_scorer.convert_tf2torch(var_dict_tf, var_dict_torch)
+            var_dict_torch_update.update(var_dict_torch_update_local)
+        # decoder
+        if model.decoder is not None:
+            var_dict_torch_update_local = model.decoder.convert_tf2torch(var_dict_tf, var_dict_torch)
+            var_dict_torch_update.update(var_dict_torch_update_local)
+
+        return var_dict_torch_update
+
+
+class EENDOLADiarTask(AbsTask):
+    # If you need more than 1 optimizer, change this value
+    num_optimizers: int = 1
+
+    # Add variable objects configurations
+    class_choices_list = [
+        # --frontend and --frontend_conf
+        frontend_choices,
+        # --specaug and --specaug_conf
+        model_choices,
+        # --encoder and --encoder_conf
+        encoder_choices,
+        # --speaker_encoder and --speaker_encoder_conf
+        encoder_decoder_attractor_choices,
+    ]
+
+    # If you need to modify train() or eval() procedures, change Trainer class here
+    trainer = Trainer
+
+    @classmethod
+    def add_task_arguments(cls, parser: argparse.ArgumentParser):
+        group = parser.add_argument_group(description="Task related")
+
+        # NOTE(kamo): add_arguments(..., required=True) can't be used
+        # to provide --print_config mode. Instead of it, do as
+        # required = parser.get_default("required")
+        # required += ["token_list"]
+
+        group.add_argument(
+            "--token_list",
+            type=str_or_none,
+            default=None,
+            help="A text mapping int-id to token",
+        )
+        group.add_argument(
+            "--split_with_space",
+            type=str2bool,
+            default=True,
+            help="whether to split text using <space>",
+        )
+        group.add_argument(
+            "--seg_dict_file",
+            type=str,
+            default=None,
+            help="seg_dict_file for text processing",
+        )
+        group.add_argument(
+            "--init",
+            type=lambda x: str_or_none(x.lower()),
+            default=None,
+            help="The initialization method",
+            choices=[
+                "chainer",
+                "xavier_uniform",
+                "xavier_normal",
+                "kaiming_uniform",
+                "kaiming_normal",
+                None,
+            ],
         )
-        frontend = None
-        if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
-            frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
-
-        logging.info("asr_model: {}".format(asr_model))
-        logging.info("asr_train_args: {}".format(asr_train_args))
-        asr_model.to(dtype=getattr(torch, dtype)).eval()
 
-        token_list = asr_model.token_list
+        group.add_argument(
+            "--input_size",
+            type=int_or_none,
+            default=None,
+            help="The number of input dimension of the feature",
+        )
 
+        group = parser.add_argument_group(description="Preprocess related")
+        group.add_argument(
+            "--use_preprocessor",
+            type=str2bool,
+            default=True,
+            help="Apply preprocessing to data or not",
+        )
+        group.add_argument(
+            "--token_type",
+            type=str,
+            default="char",
+            choices=["char"],
+            help="The text will be tokenized in the specified level token",
+        )
+        parser.add_argument(
+            "--speech_volume_normalize",
+            type=float_or_none,
+            default=None,
+            help="Scale the maximum amplitude to the given value.",
+        )
+        parser.add_argument(
+            "--rir_scp",
+            type=str_or_none,
+            default=None,
+            help="The file path of rir scp file.",
+        )
+        parser.add_argument(
+            "--rir_apply_prob",
+            type=float,
+            default=1.0,
+            help="THe probability for applying RIR convolution.",
+        )
+        parser.add_argument(
+            "--cmvn_file",
+            type=str_or_none,
+            default=None,
+            help="The file path of noise scp file.",
+        )
+        parser.add_argument(
+            "--noise_scp",
+            type=str_or_none,
+            default=None,
+            help="The file path of noise scp file.",
+        )
+        parser.add_argument(
+            "--noise_apply_prob",
+            type=float,
+            default=1.0,
+            help="The probability applying Noise adding.",
+        )
+        parser.add_argument(
+            "--noise_db_range",
+            type=str,
+            default="13_15",
+            help="The range of noise decibel level.",
+        )
 
+        for class_choices in cls.class_choices_list:
+            # Append --<name> and --<name>_conf.
+            # e.g. --encoder and --encoder_conf
+            class_choices.add_arguments(group)
+
+    @classmethod
+    def build_collate_fn(
+            cls, args: argparse.Namespace, train: bool
+    ) -> Callable[
+        [Collection[Tuple[str, Dict[str, np.ndarray]]]],
+        Tuple[List[str], Dict[str, torch.Tensor]],
+    ]:
+        assert check_argument_types()
+        # NOTE(kamo): int value = 0 is reserved by CTC-blank symbol
+        return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
 
-        logging.info(f"Decoding device={device}, dtype={dtype}")
+    @classmethod
+    def build_preprocess_fn(
+            cls, args: argparse.Namespace, train: bool
+    ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
+        assert check_argument_types()
+        # if args.use_preprocessor:
+        #     retval = CommonPreprocessor(
+        #         train=train,
+        #         token_type=args.token_type,
+        #         token_list=args.token_list,
+        #         bpemodel=None,
+        #         non_linguistic_symbols=None,
+        #         text_cleaner=None,
+        #         g2p_type=None,
+        #         split_with_space=args.split_with_space if hasattr(args, "split_with_space") else False,
+        #         seg_dict_file=args.seg_dict_file if hasattr(args, "seg_dict_file") else None,
+        #         # NOTE(kamo): Check attribute existence for backward compatibility
+        #         rir_scp=args.rir_scp if hasattr(args, "rir_scp") else None,
+        #         rir_apply_prob=args.rir_apply_prob
+        #         if hasattr(args, "rir_apply_prob")
+        #         else 1.0,
+        #         noise_scp=args.noise_scp if hasattr(args, "noise_scp") else None,
+        #         noise_apply_prob=args.noise_apply_prob
+        #         if hasattr(args, "noise_apply_prob")
+        #         else 1.0,
+        #         noise_db_range=args.noise_db_range
+        #         if hasattr(args, "noise_db_range")
+        #         else "13_15",
+        #         speech_volume_normalize=args.speech_volume_normalize
+        #         if hasattr(args, "rir_scp")
+        #         else None,
+        #     )
+        # else:
+        #     retval = None
+        # assert check_return_type(retval)
+        return None
+
+    @classmethod
+    def required_data_names(
+            cls, train: bool = True, inference: bool = False
+    ) -> Tuple[str, ...]:
+        if not inference:
+            retval = ("speech", )
+        else:
+            # Recognition mode
+            retval = ("speech", )
+        return retval
+
+    @classmethod
+    def optional_data_names(
+            cls, train: bool = True, inference: bool = False
+    ) -> Tuple[str, ...]:
+        retval = ()
+        assert check_return_type(retval)
+        return retval
 
-        # 5. [Optional] Build Text converter: e.g. bpe-sym -> Text
-        if token_type is None:
-            token_type = asr_train_args.token_type
-        if bpemodel is None:
-            bpemodel = asr_train_args.bpemodel
+    @classmethod
+    def build_model(cls, args: argparse.Namespace):
+        assert check_argument_types()
 
-        if token_type is None:
-            tokenizer = None
-        elif token_type == "bpe":
-            if bpemodel is not None:
-                tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
+        # 1. frontend
+        if args.input_size is None or args.frontend == "wav_frontend_mel23":
+            # Extract features in the model
+            frontend_class = frontend_choices.get_class(args.frontend)
+            if args.frontend == 'wav_frontend':
+                frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
             else:
-                tokenizer = None
+                frontend = frontend_class(**args.frontend_conf)
+            input_size = frontend.output_size()
         else:
-            tokenizer = build_tokenizer(token_type=token_type)
-        converter = TokenIDConverter(token_list=token_list)
-        logging.info(f"Text tokenizer: {tokenizer}")
-
-        # self.asr_model = asr_model
-        self.asr_train_args = asr_train_args
-        self.converter = converter
-        self.tokenizer = tokenizer
-
-        self.device = device
-        self.dtype = dtype
-        self.nbest = nbest
-        self.frontend = frontend
-
-        model = Paraformer_export(asr_model, onnx=False)
-        self.asr_model = model
-        
-    @torch.no_grad()
-    def __call__(
-            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None
+            # Give features from data-loader
+            args.frontend = None
+            args.frontend_conf = {}
+            frontend = None
+            input_size = args.input_size
+
+        # 2. Encoder
+        encoder_class = encoder_choices.get_class(args.encoder)
+        encoder = encoder_class(**args.encoder_conf)
+
+        # 3. EncoderDecoderAttractor
+        encoder_decoder_attractor_class = encoder_decoder_attractor_choices.get_class(args.encoder_decoder_attractor)
+        encoder_decoder_attractor = encoder_decoder_attractor_class(**args.encoder_decoder_attractor_conf)
+
+        # 9. Build model
+        model_class = model_choices.get_class(args.model)
+        model = model_class(
+            frontend=frontend,
+            encoder=encoder,
+            encoder_decoder_attractor=encoder_decoder_attractor,
+            **args.model_conf,
+        )
+
+        # 10. Initialize
+        if args.init is not None:
+            initialize(model, args.init)
+
+        assert check_return_type(model)
+        return model
+
+    # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
+    @classmethod
+    def build_model_from_file(
+            cls,
+            config_file: Union[Path, str] = None,
+            model_file: Union[Path, str] = None,
+            cmvn_file: Union[Path, str] = None,
+            device: str = "cpu",
     ):
-        """Inference
+        """Build model from the files.
+
+        This method is used for inference or fine-tuning.
 
         Args:
-                speech: Input speech data
-        Returns:
-                text, token, token_int, hyp
+            config_file: The yaml file saved when training.
+            model_file: The model file saved when training.
+            cmvn_file: The cmvn file for front-end
+            device: Device type, "cpu", "cuda", or "cuda:N".
 
         """
         assert check_argument_types()
-
-        # Input as audio signal
-        if isinstance(speech, np.ndarray):
-            speech = torch.tensor(speech)
-
-        if self.frontend is not None:
-            feats, feats_len = self.frontend.forward(speech, speech_lengths)
-            feats = to_device(feats, device=self.device)
-            feats_len = feats_len.int()
-            self.asr_model.frontend = None
-        else:
-            feats = speech
-            feats_len = speech_lengths
-
-        enc_len_batch_total = feats_len.sum()
-        lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
-        batch = {"speech": feats, "speech_lengths": feats_len}
-
-        # a. To device
-        batch = to_device(batch, device=self.device)
-
-        decoder_outs = self.asr_model(**batch)
-        decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
-        
-        results = []
-        b, n, d = decoder_out.size()
-        for i in range(b):
-            am_scores = decoder_out[i, :ys_pad_lens[i], :]
-
-            yseq = am_scores.argmax(dim=-1)
-            score = am_scores.max(dim=-1)[0]
-            score = torch.sum(score, dim=-1)
-            # pad with mask tokens to ensure compatibility with sos/eos tokens
-            yseq = torch.tensor(
-                yseq.tolist(), device=yseq.device
+        if config_file is None:
+            assert model_file is not None, (
+                "The argument 'model_file' must be provided "
+                "if the argument 'config_file' is not specified."
             )
-            nbest_hyps = [Hypothesis(yseq=yseq, score=score)]
-
-            for hyp in nbest_hyps:
-                assert isinstance(hyp, (Hypothesis)), type(hyp)
-
-                # remove sos/eos and get results
-                last_pos = -1
-                if isinstance(hyp.yseq, list):
-                    token_int = hyp.yseq[1:last_pos]
-                else:
-                    token_int = hyp.yseq[1:last_pos].tolist()
-
-                # remove blank symbol id, which is assumed to be 0
-                token_int = list(filter(lambda x: x != 0 and x != 2, token_int))
-
-                # Change integer-ids to tokens
-                token = self.converter.ids2tokens(token_int)
-
-                if self.tokenizer is not None:
-                    text = self.tokenizer.tokens2text(token)
-                else:
-                    text = None
-
-                results.append((text, token, token_int, hyp, enc_len_batch_total, lfr_factor))
-
-        return results
-
-
-def inference(
-        maxlenratio: float,
-        minlenratio: float,
-        batch_size: int,
-        beam_size: int,
-        ngpu: int,
-        ctc_weight: float,
-        lm_weight: float,
-        penalty: float,
-        log_level: Union[int, str],
-        data_path_and_name_and_type,
-        asr_train_config: Optional[str],
-        asr_model_file: Optional[str],
-        cmvn_file: Optional[str] = None,
-        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        lm_train_config: Optional[str] = None,
-        lm_file: Optional[str] = None,
-        token_type: Optional[str] = None,
-        key_file: Optional[str] = None,
-        word_lm_train_config: Optional[str] = None,
-        bpemodel: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        streaming: bool = False,
-        output_dir: Optional[str] = None,
-        dtype: str = "float32",
-        seed: int = 0,
-        ngram_weight: float = 0.9,
-        nbest: int = 1,
-        num_workers: int = 1,
-
-        **kwargs,
-):
-    inference_pipeline = inference_modelscope(
-        maxlenratio=maxlenratio,
-        minlenratio=minlenratio,
-        batch_size=batch_size,
-        beam_size=beam_size,
-        ngpu=ngpu,
-        ctc_weight=ctc_weight,
-        lm_weight=lm_weight,
-        penalty=penalty,
-        log_level=log_level,
-        asr_train_config=asr_train_config,
-        asr_model_file=asr_model_file,
-        cmvn_file=cmvn_file,
-        raw_inputs=raw_inputs,
-        lm_train_config=lm_train_config,
-        lm_file=lm_file,
-        token_type=token_type,
-        key_file=key_file,
-        word_lm_train_config=word_lm_train_config,
-        bpemodel=bpemodel,
-        allow_variable_data_keys=allow_variable_data_keys,
-        streaming=streaming,
-        output_dir=output_dir,
-        dtype=dtype,
-        seed=seed,
-        ngram_weight=ngram_weight,
-        nbest=nbest,
-        num_workers=num_workers,
-
-        **kwargs,
-    )
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs)
-
-
-def inference_modelscope(
-        maxlenratio: float,
-        minlenratio: float,
-        batch_size: int,
-        beam_size: int,
-        ngpu: int,
-        ctc_weight: float,
-        lm_weight: float,
-        penalty: float,
-        log_level: Union[int, str],
-        # data_path_and_name_and_type,
-        asr_train_config: Optional[str],
-        asr_model_file: Optional[str],
-        cmvn_file: Optional[str] = None,
-        lm_train_config: Optional[str] = None,
-        lm_file: Optional[str] = None,
-        token_type: Optional[str] = None,
-        key_file: Optional[str] = None,
-        word_lm_train_config: Optional[str] = None,
-        bpemodel: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        dtype: str = "float32",
-        seed: int = 0,
-        ngram_weight: float = 0.9,
-        nbest: int = 1,
-        num_workers: int = 1,
-        output_dir: Optional[str] = None,
-        param_dict: dict = None,
-        **kwargs,
-):
-    assert check_argument_types()
-
-    if word_lm_train_config is not None:
-        raise NotImplementedError("Word LM is not implemented")
-    if ngpu > 1:
-        raise NotImplementedError("only single GPU decoding is supported")
-
-    logging.basicConfig(
-        level=log_level,
-        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
-    )
-    
-    export_mode = False
-    if param_dict is not None:
-        hotword_list_or_file = param_dict.get('hotword')
-        export_mode = param_dict.get("export_mode", False)
-    else:
-        hotword_list_or_file = None
-
-    if ngpu >= 1 and torch.cuda.is_available():
-        device = "cuda"
-    else:
-        device = "cpu"
-        batch_size = 1
-
-    # 1. Set random-seed
-    set_all_random_seed(seed)
-
-    # 2. Build speech2text
-    speech2text_kwargs = dict(
-        asr_train_config=asr_train_config,
-        asr_model_file=asr_model_file,
-        cmvn_file=cmvn_file,
-        lm_train_config=lm_train_config,
-        lm_file=lm_file,
-        token_type=token_type,
-        bpemodel=bpemodel,
-        device=device,
-        maxlenratio=maxlenratio,
-        minlenratio=minlenratio,
-        dtype=dtype,
-        beam_size=beam_size,
-        ctc_weight=ctc_weight,
-        lm_weight=lm_weight,
-        ngram_weight=ngram_weight,
-        penalty=penalty,
-        nbest=nbest,
-        hotword_list_or_file=hotword_list_or_file,
-    )
-    if export_mode:
-        speech2text = Speech2TextExport(**speech2text_kwargs)
-    else:
-        speech2text = Speech2Text(**speech2text_kwargs)
-
-    def _forward(
-            data_path_and_name_and_type,
-            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-            output_dir_v2: Optional[str] = None,
-            fs: dict = None,
-            param_dict: dict = None,
-            **kwargs,
-    ):
+            config_file = Path(model_file).parent / "config.yaml"
+        else:
+            config_file = Path(config_file)
 
-        hotword_list_or_file = None
-        if param_dict is not None:
-            hotword_list_or_file = param_dict.get('hotword')
-        if 'hotword' in kwargs:
-            hotword_list_or_file = kwargs['hotword']
-        if hotword_list_or_file is not None or 'hotword' in kwargs:
-            speech2text.hotword_list = speech2text.generate_hotwords_list(hotword_list_or_file)
-        cache = None
-        if 'cache' in param_dict:
-            cache = param_dict['cache']
-        # 3. Build data-iterator
-        if data_path_and_name_and_type is None and raw_inputs is not None:
-            if isinstance(raw_inputs, torch.Tensor):
-                raw_inputs = raw_inputs.numpy()
-            data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = ASRTask.build_streaming_iterator(
-            data_path_and_name_and_type,
-            dtype=dtype,
-            fs=fs,
-            batch_size=batch_size,
-            key_file=key_file,
-            num_workers=num_workers,
-            preprocess_fn=ASRTask.build_preprocess_fn(speech2text.asr_train_args, False),
-            collate_fn=ASRTask.build_collate_fn(speech2text.asr_train_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
-        )
-
-        forward_time_total = 0.0
-        length_total = 0.0
-        finish_count = 0
-        file_count = 1
-        # 7 .Start for-loop
-        # FIXME(kamo): The output format should be discussed about
-        asr_result_list = []
-        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
-        if output_path is not None:
-            writer = DatadirWriter(output_path)
-        else:
-            writer = None
-
-        for keys, batch in loader:
-            assert isinstance(batch, dict), type(batch)
-            assert all(isinstance(s, str) for s in keys), keys
-            _bs = len(next(iter(batch.values())))
-            assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-            # batch = {k: v for k, v in batch.items() if not k.endswith("_lengths")}
-
-            logging.info("decoding, utt_id: {}".format(keys))
-            # N-best list of (text, token, token_int, hyp_object)
-
-            time_beg = time.time()
-            results = speech2text(cache=cache, **batch)
-            if len(results) < 1:
-                hyp = Hypothesis(score=0.0, scores={}, states={}, yseq=[])
-                results = [[" ", ["sil"], [2], hyp, 10, 6]] * nbest
-            time_end = time.time()
-            forward_time = time_end - time_beg
-            lfr_factor = results[0][-1]
-            length = results[0][-2]
-            forward_time_total += forward_time
-            length_total += length
-            rtf_cur = "decoding, feature length: {}, forward_time: {:.4f}, rtf: {:.4f}".format(length, forward_time, 100 * forward_time / (length * lfr_factor))
-            logging.info(rtf_cur)
-
-            for batch_id in range(_bs):
-                result = [results[batch_id][:-2]]
-
-                key = keys[batch_id]
-                for n, (text, token, token_int, hyp) in zip(range(1, nbest + 1), result):
-                    # Create a directory: outdir/{n}best_recog
-                    if writer is not None:
-                        ibest_writer = writer[f"{n}best_recog"]
-
-                        # Write the result to each file
-                        ibest_writer["token"][key] = " ".join(token)
-                        # ibest_writer["token_int"][key] = " ".join(map(str, token_int))
-                        ibest_writer["score"][key] = str(hyp.score)
-                        ibest_writer["rtf"][key] = rtf_cur
-
-                    if text is not None:
-                        text_postprocessed, word_lists = postprocess_utils.sentence_postprocess(token)
-                        item = {'key': key, 'value': text_postprocessed}
-                        asr_result_list.append(item)
-                        finish_count += 1
-                        # asr_utils.print_progress(finish_count / file_count)
-                        if writer is not None:
-                            ibest_writer["text"][key] = " ".join(word_lists)
-
-                    logging.info("decoding, utt: {}, predictions: {}".format(key, text))
-        rtf_avg = "decoding, feature length total: {}, forward_time total: {:.4f}, rtf avg: {:.4f}".format(length_total, forward_time_total, 100 * forward_time_total / (length_total * lfr_factor))
-        logging.info(rtf_avg)
-        if writer is not None:
-            ibest_writer["rtf"]["rtf_avf"] = rtf_avg
-        return asr_result_list
-
-    return _forward
-
-
-def get_parser():
-    parser = config_argparse.ArgumentParser(
-        description="ASR Decoding",
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-    )
-
-    # Note(kamo): Use '_' instead of '-' as separator.
-    # '-' is confusing if written in yaml.
-    parser.add_argument(
-        "--log_level",
-        type=lambda x: x.upper(),
-        default="INFO",
-        choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
-        help="The verbose level of logging",
-    )
-
-    parser.add_argument("--output_dir", type=str, required=True)
-    parser.add_argument(
-        "--ngpu",
-        type=int,
-        default=0,
-        help="The number of gpus. 0 indicates CPU mode",
-    )
-    parser.add_argument("--seed", type=int, default=0, help="Random seed")
-    parser.add_argument(
-        "--dtype",
-        default="float32",
-        choices=["float16", "float32", "float64"],
-        help="Data type",
-    )
-    parser.add_argument(
-        "--num_workers",
-        type=int,
-        default=1,
-        help="The number of workers used for DataLoader",
-    )
-    parser.add_argument(
-        "--hotword",
-        type=str_or_none,
-        default=None,
-        help="hotword file path or hotwords seperated by space"
-    )
-    group = parser.add_argument_group("Input data related")
-    group.add_argument(
-        "--data_path_and_name_and_type",
-        type=str2triple_str,
-        required=False,
-        action="append",
-    )
-    group.add_argument("--key_file", type=str_or_none)
-    group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
-
-    group = parser.add_argument_group("The model configuration related")
-    group.add_argument(
-        "--asr_train_config",
-        type=str,
-        help="ASR training configuration",
-    )
-    group.add_argument(
-        "--asr_model_file",
-        type=str,
-        help="ASR model parameter file",
-    )
-    group.add_argument(
-        "--cmvn_file",
-        type=str,
-        help="Global cmvn file",
-    )
-    group.add_argument(
-        "--lm_train_config",
-        type=str,
-        help="LM training configuration",
-    )
-    group.add_argument(
-        "--lm_file",
-        type=str,
-        help="LM parameter file",
-    )
-    group.add_argument(
-        "--word_lm_train_config",
-        type=str,
-        help="Word LM training configuration",
-    )
-    group.add_argument(
-        "--word_lm_file",
-        type=str,
-        help="Word LM parameter file",
-    )
-    group.add_argument(
-        "--ngram_file",
-        type=str,
-        help="N-gram parameter file",
-    )
-    group.add_argument(
-        "--model_tag",
-        type=str,
-        help="Pretrained model tag. If specify this option, *_train_config and "
-             "*_file will be overwritten",
-    )
-
-    group = parser.add_argument_group("Beam-search related")
-    group.add_argument(
-        "--batch_size",
-        type=int,
-        default=1,
-        help="The batch size for inference",
-    )
-    group.add_argument("--nbest", type=int, default=1, help="Output N-best hypotheses")
-    group.add_argument("--beam_size", type=int, default=20, help="Beam size")
-    group.add_argument("--penalty", type=float, default=0.0, help="Insertion penalty")
-    group.add_argument(
-        "--maxlenratio",
-        type=float,
-        default=0.0,
-        help="Input length ratio to obtain max output length. "
-             "If maxlenratio=0.0 (default), it uses a end-detect "
-             "function "
-             "to automatically find maximum hypothesis lengths."
-             "If maxlenratio<0.0, its absolute value is interpreted"
-             "as a constant max output length",
-    )
-    group.add_argument(
-        "--minlenratio",
-        type=float,
-        default=0.0,
-        help="Input length ratio to obtain min output length",
-    )
-    group.add_argument(
-        "--ctc_weight",
-        type=float,
-        default=0.5,
-        help="CTC weight in joint decoding",
-    )
-    group.add_argument("--lm_weight", type=float, default=1.0, help="RNNLM weight")
-    group.add_argument("--ngram_weight", type=float, default=0.9, help="ngram weight")
-    group.add_argument("--streaming", type=str2bool, default=False)
-
-    group.add_argument(
-        "--frontend_conf",
-        default=None,
-        help="",
-    )
-    group.add_argument("--raw_inputs", type=list, default=None)
-    # example=[{'key':'EdevDEWdIYQ_0021','file':'/mnt/data/jiangyu.xzy/test_data/speech_io/SPEECHIO_ASR_ZH00007_zhibodaihuo/wav/EdevDEWdIYQ_0021.wav'}])
-
-    group = parser.add_argument_group("Text converter related")
-    group.add_argument(
-        "--token_type",
-        type=str_or_none,
-        default=None,
-        choices=["char", "bpe", None],
-        help="The token type for ASR model. "
-             "If not given, refers from the training args",
-    )
-    group.add_argument(
-        "--bpemodel",
-        type=str_or_none,
-        default=None,
-        help="The model path of sentencepiece. "
-             "If not given, refers from the training args",
-    )
-
-    return parser
-
-
-def main(cmd=None):
-    print(get_commandline_args(), file=sys.stderr)
-    parser = get_parser()
-    args = parser.parse_args(cmd)
-    param_dict = {'hotword': args.hotword}
-    kwargs = vars(args)
-    kwargs.pop("config", None)
-    kwargs['param_dict'] = param_dict
-    inference(**kwargs)
-
-
-if __name__ == "__main__":
-    main()
-
-    # from modelscope.pipelines import pipeline
-    # from modelscope.utils.constant import Tasks
-    #
-    # inference_16k_pipline = pipeline(
-    #     task=Tasks.auto_speech_recognition,
-    #     model='damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch')
-    #
-    # rec_result = inference_16k_pipline(audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav')
-    # print(rec_result)
+        with config_file.open("r", encoding="utf-8") as f:
+            args = yaml.safe_load(f)
+        args = argparse.Namespace(**args)
+        model = cls.build_model(args)
+        if not isinstance(model, AbsESPnetModel):
+            raise RuntimeError(
+                f"model must inherit {AbsESPnetModel.__name__}, but got {type(model)}"
+            )
+        if model_file is not None:
+            if device == "cuda":
+                device = f"cuda:{torch.cuda.current_device()}"
+            checkpoint = torch.load(model_file, map_location=device)
+            if "state_dict" in checkpoint.keys():
+                model.load_state_dict(checkpoint["state_dict"])
+            else:
+                model.load_state_dict(checkpoint)
+        model.to(device)
+        return model, args
```

### Comparing `funasr-0.4.1/funasr/bin/asr_inference_uniasr.py` & `funasr-0.4.2/funasr/bin/asr_inference_uniasr.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,14 +375,16 @@
         token_num_relax: int = 1,
         decoding_ind: int = 0,
         decoding_mode: str = "model1",
         param_dict: dict = None,
         **kwargs,
 ):
     assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
```

### Comparing `funasr-0.4.1/funasr/bin/asr_inference_uniasr_vad.py` & `funasr-0.4.2/funasr/bin/asr_inference_uniasr_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/bin/asr_train.py` & `funasr-0.4.2/funasr/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/bin/asr_train_paraformer.py` & `funasr-0.4.2/funasr/bin/asr_train_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/bin/asr_train_uniasr.py` & `funasr-0.4.2/funasr/bin/asr_train_uniasr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/bin/build_trainer.py` & `funasr-0.4.2/funasr/bin/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/bin/data2vec_train.py` & `funasr-0.4.2/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/bin/diar_inference_launch.py` & `funasr-0.4.2/funasr/bin/diar_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python3
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
-import torch
-torch.set_num_threads(1)
 
 import argparse
 import logging
 import os
 import sys
 from typing import Union, Dict, Any
```

### Comparing `funasr-0.4.1/funasr/bin/diar_train.py` & `funasr-0.4.2/funasr/bin/diar_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/bin/eend_ola_inference.py` & `funasr-0.4.2/funasr/bin/eend_ola_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,14 +154,16 @@
         model_tag: Optional[str] = None,
         allow_variable_data_keys: bool = True,
         streaming: bool = False,
         param_dict: Optional[dict] = None,
         **kwargs,
 ):
     assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
         level=log_level,
```

### Comparing `funasr-0.4.1/funasr/bin/lm_calc_perplexity.py` & `funasr-0.4.2/funasr/bin/lm_calc_perplexity.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/bin/lm_inference.py` & `funasr-0.4.2/funasr/bin/lm_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,18 +85,17 @@
     split_with_space: Optional[bool] = False,
     seg_dict_file: Optional[str] = None,
     output_dir: Optional[str] = None,
     param_dict: dict = None,
     **kwargs,
 ):
     assert check_argument_types()
-    logging.basicConfig(
-        level=log_level,
-        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
-    )
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
+
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
 
     # 1. Set random-seed
```

### Comparing `funasr-0.4.1/funasr/bin/lm_inference_launch.py` & `funasr-0.4.2/funasr/bin/lm_inference_launch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 #!/usr/bin/env python3
-# Copyright ESPnet (https://github.com/espnet/espnet). All Rights Reserved.
-#  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
-import torch
-torch.set_num_threads(1)
+
 
 import argparse
 import logging
 import os
 import sys
 from typing import Union, Dict, Any
```

### Comparing `funasr-0.4.1/funasr/bin/lm_train.py` & `funasr-0.4.2/funasr/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/bin/modelscope_infer.py` & `funasr-0.4.2/funasr/bin/modelscope_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/bin/punc_inference_launch.py` & `funasr-0.4.2/funasr/bin/punc_inference_launch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 #!/usr/bin/env python3
-# Copyright ESPnet (https://github.com/espnet/espnet). All Rights Reserved.
-#  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
-import torch
-torch.set_num_threads(1)
 
 import argparse
 import logging
 import os
 import sys
 from typing import Union, Dict, Any
```

### Comparing `funasr-0.4.1/funasr/bin/punc_train.py` & `funasr-0.4.2/funasr/bin/punc_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/bin/punctuation_infer.py` & `funasr-0.4.2/funasr/bin/punctuation_infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
             token_list=train_args.token_list,
             bpemodel=train_args.bpemodel,
             text_cleaner=train_args.cleaner,
             g2p_type=train_args.g2p,
             text_name="text",
             non_linguistic_symbols=train_args.non_linguistic_symbols,
         )
-        print("start decoding!!!")
 
     @torch.no_grad()
     def __call__(self, text: Union[list, str], split_size=20):
         data = {"text": text}
         result = self.preprocessor(data=data, uid="12938712838719")
         split_text = self.preprocessor.pop_split_text_data(result)
         mini_sentences = split_to_mini_sentence(split_text, split_size)
@@ -219,15 +218,14 @@
             if line == "":
                 item = {'key': key, 'value': ""}
                 results.append(item)
                 return results
             result, _ = text2punc(line)
             item = {'key': key, 'value': result}
             results.append(item)
-            print(results)
             return results
 
         for inference_text, _, _ in data_path_and_name_and_type:
             with open(inference_text, "r", encoding="utf-8") as fin:
                 for line in fin:
                     line = line.strip()
                     segs = line.split("\t")
```

### Comparing `funasr-0.4.1/funasr/bin/punctuation_infer_vadrealtime.py` & `funasr-0.4.2/funasr/bin/punctuation_infer_vadrealtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,18 +199,16 @@
     train_config: Optional[str],
     model_file: Optional[str],
     output_dir: Optional[str] = None,
     param_dict: dict = None,
     **kwargs,
 ):
     assert check_argument_types()
-    logging.basicConfig(
-        level=log_level,
-        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
-    )
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
 
     # 1. Set random-seed
```

### Comparing `funasr-0.4.1/funasr/bin/sond_inference.py` & `funasr-0.4.2/funasr/bin/sond_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,16 @@
         dur_threshold: int = 10,
         out_format: str = "vad",
         param_dict: Optional[dict] = None,
         mode: str = "sond",
         **kwargs,
 ):
     assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
         level=log_level,
```

### Comparing `funasr-0.4.1/funasr/bin/sv_inference.py` & `funasr-0.4.2/funasr/bin/sv_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,17 @@
         streaming: bool = False,
         embedding_node: str = "resnet1_dense",
         sv_threshold: float = 0.9465,
         param_dict: Optional[dict] = None,
         **kwargs,
 ):
     assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
+    
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
         level=log_level,
```

### Comparing `funasr-0.4.1/funasr/bin/sv_inference_launch.py` & `funasr-0.4.2/funasr/bin/sv_inference_launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python3
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
-import torch
-torch.set_num_threads(1)
 
 import argparse
 import logging
 import os
 import sys
 from typing import Union, Dict, Any
```

### Comparing `funasr-0.4.1/funasr/bin/tokenize_text.py` & `funasr-0.4.2/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/bin/tp_inference.py` & `funasr-0.4.2/funasr/bin/tp_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         device: str = "cpu",
         dtype: str = "float32",
         **kwargs,
     ):
         assert check_argument_types()
         # 1. Build ASR model
         tp_model, tp_train_args = ASRTask.build_model_from_file(
-            timestamp_infer_config, timestamp_model_file, device
+            timestamp_infer_config, timestamp_model_file, device=device
         )
         if 'cuda' in device:
             tp_model = tp_model.cuda()  # force model to cuda
 
         frontend = None
         if tp_train_args.frontend is not None:
             frontend = WavFrontend(cmvn_file=timestamp_cmvn_file, **tp_train_args.frontend_conf)
@@ -175,14 +175,17 @@
         seed: int = 0,
         num_workers: int = 1,
         split_with_space: bool = True,
         seg_dict_file: Optional[str] = None,
         **kwargs,
 ):
     assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
+    
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
         level=log_level,
```

### Comparing `funasr-0.4.1/funasr/bin/tp_inference_launch.py` & `funasr-0.4.2/funasr/bin/vad_inference_launch.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 
 
 def get_parser():
     parser = config_argparse.ArgumentParser(
-        description="Timestamp Prediction Inference",
+        description="VAD Decoding",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Note(kamo): Use '_' instead of '-' as separator.
     # '-' is confusing if written in yaml.
     parser.add_argument(
         "--log_level",
         type=lambda x: x.upper(),
         default="INFO",
         choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
         help="The verbose level of logging",
     )
 
-    parser.add_argument("--output_dir", type=str, required=False)
+    parser.add_argument("--output_dir", type=str, required=True)
     parser.add_argument(
         "--ngpu",
         type=int,
         default=0,
         help="The number of gpus. 0 indicates CPU mode",
     )
     parser.add_argument(
@@ -75,54 +75,62 @@
         action="append",
     )
     group.add_argument("--key_file", type=str_or_none)
     group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
 
     group = parser.add_argument_group("The model configuration related")
     group.add_argument(
-        "--timestamp_infer_config",
+        "--vad_infer_config",
         type=str,
         help="VAD infer configuration",
     )
     group.add_argument(
-        "--timestamp_model_file",
+        "--vad_model_file",
         type=str,
         help="VAD model parameter file",
     )
     group.add_argument(
-        "--timestamp_cmvn_file",
+        "--vad_cmvn_file",
         type=str,
         help="Global CMVN file",
     )
+    group.add_argument(
+        "--vad_train_config",
+        type=str,
+        help="VAD training configuration",
+    )
 
     group = parser.add_argument_group("The inference configuration related")
     group.add_argument(
         "--batch_size",
         type=int,
         default=1,
         help="The batch size for inference",
     )
     return parser
 
 
 def inference_launch(mode, **kwargs):
-    if mode == "tp_norm":
-        from funasr.bin.tp_inference import inference_modelscope
+    if mode == "offline":
+        from funasr.bin.vad_inference import inference_modelscope
         return inference_modelscope(**kwargs)
+    elif mode == "online":
+        from funasr.bin.vad_inference import inference_modelscope_online
+        return inference_modelscope_online(**kwargs)
     else:
         logging.info("Unknown decoding mode: {}".format(mode))
         return None
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
     parser.add_argument(
         "--mode",
         type=str,
-        default="tp_norm",
+        default="vad",
         help="The decoding mode",
     )
     args = parser.parse_args(cmd)
     kwargs = vars(args)
     kwargs.pop("config", None)
 
     # set logging messages
```

### Comparing `funasr-0.4.1/funasr/bin/vad_inference.py` & `funasr-0.4.2/funasr/bin/vad_inference_online.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,139 +8,98 @@
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 from typing import Dict
 
-import math
 import numpy as np
 import torch
 from typeguard import check_argument_types
 from typeguard import check_return_type
 
 from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.modules.scorers.scorer_interface import BatchScorerInterface
-from funasr.modules.subsampling import TooShortUttError
 from funasr.tasks.vad import VADTask
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.utils import asr_utils, wav_utils, postprocess_utils
+from funasr.models.frontend.wav_frontend import WavFrontendOnline
 from funasr.models.frontend.wav_frontend import WavFrontend
+from funasr.bin.vad_inference import Speech2VadSegment
 
 header_colors = '\033[95m'
 end_colors = '\033[0m'
 
-global_asr_language: str = 'zh-cn'
-global_sample_rate: Union[int, Dict[Any, int]] = {
-    'audio_fs': 16000,
-    'model_fs': 16000
-}
 
-
-class Speech2VadSegment:
-    """Speech2VadSegment class
+class Speech2VadSegmentOnline(Speech2VadSegment):
+    """Speech2VadSegmentOnline class
 
     Examples:
         >>> import soundfile
-        >>> speech2segment = Speech2VadSegment("vad_config.yml", "vad.pt")
+        >>> speech2segment = Speech2VadSegmentOnline("vad_config.yml", "vad.pt")
         >>> audio, rate = soundfile.read("speech.wav")
         >>> speech2segment(audio)
         [[10, 230], [245, 450], ...]
 
     """
+    def __init__(self, **kwargs):
+        super(Speech2VadSegmentOnline, self).__init__(**kwargs)
+        vad_cmvn_file = kwargs.get('vad_cmvn_file', None)
+        self.frontend = None
+        if self.vad_infer_args.frontend is not None:
+            self.frontend = WavFrontendOnline(cmvn_file=vad_cmvn_file, **self.vad_infer_args.frontend_conf)
 
-    def __init__(
-            self,
-            vad_infer_config: Union[Path, str] = None,
-            vad_model_file: Union[Path, str] = None,
-            vad_cmvn_file: Union[Path, str] = None,
-            device: str = "cpu",
-            batch_size: int = 1,
-            dtype: str = "float32",
-            **kwargs,
-    ):
-        assert check_argument_types()
-
-        # 1. Build vad model
-        vad_model, vad_infer_args = VADTask.build_model_from_file(
-            vad_infer_config, vad_model_file, device
-        )
-        frontend = None
-        if vad_infer_args.frontend is not None:
-            frontend = WavFrontend(cmvn_file=vad_cmvn_file, **vad_infer_args.frontend_conf)
-
-        logging.info("vad_model: {}".format(vad_model))
-        logging.info("vad_infer_args: {}".format(vad_infer_args))
-        vad_model.to(dtype=getattr(torch, dtype)).eval()
-
-        self.vad_model = vad_model
-        self.vad_infer_args = vad_infer_args
-        self.device = device
-        self.dtype = dtype
-        self.frontend = frontend
-        self.batch_size = batch_size
 
     @torch.no_grad()
     def __call__(
             self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None,
-            in_cache: Dict[str, torch.Tensor] = dict()
-    ) -> Tuple[List[List[int]], Dict[str, torch.Tensor]]:
+            in_cache: Dict[str, torch.Tensor] = dict(), is_final: bool = False, max_end_sil: int = 800
+    ) -> Tuple[torch.Tensor, List[List[int]], torch.Tensor]:
         """Inference
 
         Args:
             speech: Input speech data
         Returns:
             text, token, token_int, hyp
 
         """
         assert check_argument_types()
 
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
-
+        batch_size = speech.shape[0]
+        segments = [[]] * batch_size
         if self.frontend is not None:
-            self.frontend.filter_length_max = math.inf
-            fbanks, fbanks_len = self.frontend.forward_fbank(speech, speech_lengths)
-            feats, feats_len = self.frontend.forward_lfr_cmvn(fbanks, fbanks_len)
-            fbanks = to_device(fbanks, device=self.device)
-            feats = to_device(feats, device=self.device)
-            feats_len = feats_len.int()
+            feats, feats_len = self.frontend.forward(speech, speech_lengths, is_final)
+            fbanks, _ = self.frontend.get_fbank()
         else:
             raise Exception("Need to extract feats first, please configure frontend configuration")
+        if feats.shape[0]:
+            feats = to_device(feats, device=self.device)
+            feats_len = feats_len.int()
+            waveforms = self.frontend.get_waveforms()
 
-        # b. Forward Encoder streaming
-        t_offset = 0
-        step = min(feats_len.max(), 6000)
-        segments = [[]] * self.batch_size
-        for t_offset in range(0, feats_len, min(step, feats_len - t_offset)):
-            if t_offset + step >= feats_len - 1:
-                step = feats_len - t_offset
-                is_final = True
-            else:
-                is_final = False
             batch = {
-                "feats": feats[:, t_offset:t_offset + step, :],
-                "waveform": speech[:, t_offset * 160:min(speech.shape[-1], (t_offset + step - 1) * 160 + 400)],
+                "feats": feats,
+                "waveform": waveforms,
+                "in_cache": in_cache,
                 "is_final": is_final,
-                "in_cache": in_cache
+                "max_end_sil": max_end_sil
             }
             # a. To device
             batch = to_device(batch, device=self.device)
-            segments_part, in_cache = self.vad_model(**batch)
-            if segments_part:
-                for batch_num in range(0, self.batch_size):
-                    segments[batch_num] += segments_part[batch_num]
-        return fbanks, segments
+            segments, in_cache = self.vad_model.forward_online(**batch)
+            # in_cache.update(batch['in_cache'])
+            # in_cache = {key: value for key, value in batch['in_cache'].items()}
+        return fbanks, segments, in_cache
 
 
 def inference(
         batch_size: int,
         ngpu: int,
         log_level: Union[int, str],
         data_path_and_name_and_type,
@@ -188,14 +147,17 @@
         output_dir: Optional[str] = None,
         dtype: str = "float32",
         seed: int = 0,
         num_workers: int = 1,
         **kwargs,
 ):
     assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
+    
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
         level=log_level,
@@ -215,22 +177,22 @@
         vad_infer_config=vad_infer_config,
         vad_model_file=vad_model_file,
         vad_cmvn_file=vad_cmvn_file,
         device=device,
         dtype=dtype,
     )
     logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
-    speech2vadsegment = Speech2VadSegment(**speech2vadsegment_kwargs)
+    speech2vadsegment = Speech2VadSegmentOnline(**speech2vadsegment_kwargs)
 
     def _forward(
             data_path_and_name_and_type,
             raw_inputs: Union[np.ndarray, torch.Tensor] = None,
             output_dir_v2: Optional[str] = None,
             fs: dict = None,
-            param_dict: dict = None
+            param_dict: dict = None,
     ):
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
         loader = VADTask.build_streaming_iterator(
@@ -254,30 +216,39 @@
             writer = DatadirWriter(output_path)
             ibest_writer = writer[f"1best_recog"]
         else:
             writer = None
             ibest_writer = None
 
         vad_results = []
+        batch_in_cache = param_dict['in_cache'] if param_dict is not None else dict()
+        is_final = param_dict.get('is_final', False) if param_dict is not None else False
+        max_end_sil = param_dict.get('max_end_sil', 800) if param_dict is not None else 800
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
+            batch['in_cache'] = batch_in_cache
+            batch['is_final'] = is_final
+            batch['max_end_sil'] = max_end_sil
 
             # do vad segment
-            _, results = speech2vadsegment(**batch)
-            for i, _ in enumerate(keys):
-                if "MODELSCOPE_ENVIRONMENT" in os.environ and os.environ["MODELSCOPE_ENVIRONMENT"] == "eas":
-                    results[i] = json.dumps(results[i])
-                item = {'key': keys[i], 'value': results[i]}
-                vad_results.append(item)
-                if writer is not None:
-                    results[i] = json.loads(results[i])
-                    ibest_writer["text"][keys[i]] = "{}".format(results[i])
+            _, results, param_dict['in_cache'] = speech2vadsegment(**batch)
+            # param_dict['in_cache'] = batch['in_cache']
+            if results:
+                for i, _ in enumerate(keys):
+                    if results[i]:
+                        if "MODELSCOPE_ENVIRONMENT" in os.environ and os.environ["MODELSCOPE_ENVIRONMENT"] == "eas":
+                            results[i] = json.dumps(results[i])
+                        item = {'key': keys[i], 'value': results[i]}
+                        vad_results.append(item)
+                        if writer is not None:
+                            results[i] = json.loads(results[i])
+                            ibest_writer["text"][keys[i]] = "{}".format(results[i])
 
         return vad_results
 
     return _forward
 
 
 def get_parser():
```

### Comparing `funasr-0.4.1/funasr/bin/vad_inference_launch.py` & `funasr-0.4.2/funasr/bin/tp_inference_launch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 #!/usr/bin/env python3
-# Copyright ESPnet (https://github.com/espnet/espnet). All Rights Reserved.
-#  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
-import torch
-torch.set_num_threads(1)
 
 import argparse
 import logging
 import os
 import sys
 from typing import Union, Dict, Any
 
@@ -16,29 +12,29 @@
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 
 
 def get_parser():
     parser = config_argparse.ArgumentParser(
-        description="VAD Decoding",
+        description="Timestamp Prediction Inference",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Note(kamo): Use '_' instead of '-' as separator.
     # '-' is confusing if written in yaml.
     parser.add_argument(
         "--log_level",
         type=lambda x: x.upper(),
         default="INFO",
         choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
         help="The verbose level of logging",
     )
 
-    parser.add_argument("--output_dir", type=str, required=True)
+    parser.add_argument("--output_dir", type=str, required=False)
     parser.add_argument(
         "--ngpu",
         type=int,
         default=0,
         help="The number of gpus. 0 indicates CPU mode",
     )
     parser.add_argument(
@@ -75,62 +71,54 @@
         action="append",
     )
     group.add_argument("--key_file", type=str_or_none)
     group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
 
     group = parser.add_argument_group("The model configuration related")
     group.add_argument(
-        "--vad_infer_config",
+        "--timestamp_infer_config",
         type=str,
         help="VAD infer configuration",
     )
     group.add_argument(
-        "--vad_model_file",
+        "--timestamp_model_file",
         type=str,
         help="VAD model parameter file",
     )
     group.add_argument(
-        "--vad_cmvn_file",
+        "--timestamp_cmvn_file",
         type=str,
         help="Global CMVN file",
     )
-    group.add_argument(
-        "--vad_train_config",
-        type=str,
-        help="VAD training configuration",
-    )
 
     group = parser.add_argument_group("The inference configuration related")
     group.add_argument(
         "--batch_size",
         type=int,
         default=1,
         help="The batch size for inference",
     )
     return parser
 
 
 def inference_launch(mode, **kwargs):
-    if mode == "offline":
-        from funasr.bin.vad_inference import inference_modelscope
-        return inference_modelscope(**kwargs)
-    elif mode == "online":
-        from funasr.bin.vad_inference_online import inference_modelscope
+    if mode == "tp_norm":
+        from funasr.bin.tp_inference import inference_modelscope
         return inference_modelscope(**kwargs)
     else:
         logging.info("Unknown decoding mode: {}".format(mode))
         return None
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
     parser.add_argument(
         "--mode",
         type=str,
-        default="vad",
+        default="tp_norm",
         help="The decoding mode",
     )
     args = parser.parse_args(cmd)
     kwargs = vars(args)
     kwargs.pop("config", None)
 
     # set logging messages
```

### Comparing `funasr-0.4.1/funasr/bin/vad_inference_online.py` & `funasr-0.4.2/funasr/tasks/vad.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,344 +1,363 @@
 import argparse
 import logging
-import os
-import sys
-import json
-from pathlib import Path
-from typing import Any
+from typing import Callable
+from typing import Collection
+from typing import Dict
 from typing import List
 from typing import Optional
-from typing import Sequence
+from typing import Tuple
+import os
+from pathlib import Path
 from typing import Tuple
 from typing import Union
-from typing import Dict
-
+import yaml
 import numpy as np
 import torch
 from typeguard import check_argument_types
 from typeguard import check_return_type
 
-from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.tasks.vad import VADTask
-from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
+from funasr.datasets.collate_fn import CommonCollateFn
+from funasr.datasets.preprocessor import CommonPreprocessor
+from funasr.models.ctc import CTC
+from funasr.models.decoder.abs_decoder import AbsDecoder
+from funasr.models.decoder.rnn_decoder import RNNDecoder
+from funasr.models.decoder.transformer_decoder import (
+    DynamicConvolution2DTransformerDecoder,  # noqa: H301
+)
+from funasr.models.decoder.transformer_decoder import DynamicConvolutionTransformerDecoder
+from funasr.models.decoder.transformer_decoder import (
+    LightweightConvolution2DTransformerDecoder,  # noqa: H301
+)
+from funasr.models.decoder.transformer_decoder import (
+    LightweightConvolutionTransformerDecoder,  # noqa: H301
+)
+from funasr.models.decoder.transformer_decoder import TransformerDecoder
+from funasr.models.encoder.abs_encoder import AbsEncoder
+from funasr.models.encoder.conformer_encoder import ConformerEncoder
+from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
+from funasr.models.encoder.rnn_encoder import RNNEncoder
+from funasr.models.encoder.transformer_encoder import TransformerEncoder
+from funasr.models.frontend.abs_frontend import AbsFrontend
+from funasr.models.frontend.default import DefaultFrontend
+from funasr.models.frontend.fused import FusedFrontends
+from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
+from funasr.models.frontend.s3prl import S3prlFrontend
+from funasr.models.frontend.windowing import SlidingWindow
+from funasr.models.postencoder.abs_postencoder import AbsPostEncoder
+from funasr.models.postencoder.hugging_face_transformers_postencoder import (
+    HuggingFaceTransformersPostEncoder,  # noqa: H301
+)
+from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
+from funasr.models.preencoder.linear import LinearProjection
+from funasr.models.preencoder.sinc import LightweightSincConvs
+from funasr.models.specaug.abs_specaug import AbsSpecAug
+from funasr.models.specaug.specaug import SpecAug
+from funasr.layers.abs_normalize import AbsNormalize
+from funasr.layers.global_mvn import GlobalMVN
+from funasr.layers.utterance_mvn import UtteranceMVN
+from funasr.tasks.abs_task import AbsTask
+from funasr.text.phoneme_tokenizer import g2p_choices
+from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.train.class_choices import ClassChoices
+from funasr.train.trainer import Trainer
+from funasr.utils.get_default_kwargs import get_default_kwargs
+from funasr.utils.nested_dict_action import NestedDictAction
+from funasr.utils.types import float_or_none
+from funasr.utils.types import int_or_none
 from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.models.frontend.wav_frontend import WavFrontendOnline
-from funasr.models.frontend.wav_frontend import WavFrontend
-from funasr.bin.vad_inference import Speech2VadSegment
-
-header_colors = '\033[95m'
-end_colors = '\033[0m'
-
-
-class Speech2VadSegmentOnline(Speech2VadSegment):
-    """Speech2VadSegmentOnline class
-
-    Examples:
-        >>> import soundfile
-        >>> speech2segment = Speech2VadSegmentOnline("vad_config.yml", "vad.pt")
-        >>> audio, rate = soundfile.read("speech.wav")
-        >>> speech2segment(audio)
-        [[10, 230], [245, 450], ...]
-
-    """
-    def __init__(self, **kwargs):
-        super(Speech2VadSegmentOnline, self).__init__(**kwargs)
-        vad_cmvn_file = kwargs.get('vad_cmvn_file', None)
-        self.frontend = None
-        if self.vad_infer_args.frontend is not None:
-            self.frontend = WavFrontendOnline(cmvn_file=vad_cmvn_file, **self.vad_infer_args.frontend_conf)
-
-
-    @torch.no_grad()
-    def __call__(
-            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None,
-            in_cache: Dict[str, torch.Tensor] = dict(), is_final: bool = False, max_end_sil: int = 800
-    ) -> Tuple[torch.Tensor, List[List[int]], torch.Tensor]:
-        """Inference
 
-        Args:
-            speech: Input speech data
-        Returns:
-            text, token, token_int, hyp
+from funasr.models.specaug.specaug import SpecAugLFR
+from funasr.models.predictor.cif import CifPredictor, CifPredictorV2
+from funasr.modules.subsampling import Conv1dSubsampling
+from funasr.models.e2e_vad import E2EVadModel
+from funasr.models.encoder.fsmn_encoder import FSMN
+
+frontend_choices = ClassChoices(
+    name="frontend",
+    classes=dict(
+        default=DefaultFrontend,
+        sliding_window=SlidingWindow,
+        s3prl=S3prlFrontend,
+        fused=FusedFrontends,
+        wav_frontend=WavFrontend,
+        wav_frontend_online=WavFrontendOnline,
+    ),
+    type_check=AbsFrontend,
+    default="default",
+)
+specaug_choices = ClassChoices(
+    name="specaug",
+    classes=dict(
+        specaug=SpecAug,
+        specaug_lfr=SpecAugLFR,
+    ),
+    type_check=AbsSpecAug,
+    default=None,
+    optional=True,
+)
+normalize_choices = ClassChoices(
+    "normalize",
+    classes=dict(
+        global_mvn=GlobalMVN,
+        utterance_mvn=UtteranceMVN,
+    ),
+    type_check=AbsNormalize,
+    default=None,
+    optional=True,
+)
+model_choices = ClassChoices(
+    "model",
+    classes=dict(
+        e2evad=E2EVadModel,
+    ),
+    type_check=object,
+    default="e2evad",
+)
+
+encoder_choices = ClassChoices(
+    "encoder",
+    classes=dict(
+        fsmn=FSMN,
+    ),
+    type_check=torch.nn.Module,
+    default="fsmn",
+)
+
+
+class VADTask(AbsTask):
+    # If you need more than one optimizers, change this value
+    num_optimizers: int = 1
+
+    # Add variable objects configurations
+    class_choices_list = [
+        # --frontend and --frontend_conf
+        frontend_choices,
+        # --model and --model_conf
+        model_choices,
+    ]
+
+    # If you need to modify train() or eval() procedures, change Trainer class here
+    trainer = Trainer
+
+    @classmethod
+    def add_task_arguments(cls, parser: argparse.ArgumentParser):
+        group = parser.add_argument_group(description="Task related")
+
+        # NOTE(kamo): add_arguments(..., required=True) can't be used
+        # to provide --print_config mode. Instead of it, do as
+        # required = parser.get_default("required")
+        # required += ["token_list"]
+
+        group.add_argument(
+            "--init",
+            type=lambda x: str_or_none(x.lower()),
+            default=None,
+            help="The initialization method",
+            choices=[
+                "chainer",
+                "xavier_uniform",
+                "xavier_normal",
+                "kaiming_uniform",
+                "kaiming_normal",
+                None,
+            ],
+        )
 
-        """
+        group.add_argument(
+            "--input_size",
+            type=int_or_none,
+            default=None,
+            help="The number of input dimension of the feature",
+        )
+
+        group = parser.add_argument_group(description="Preprocess related")
+        parser.add_argument(
+            "--speech_volume_normalize",
+            type=float_or_none,
+            default=None,
+            help="Scale the maximum amplitude to the given value.",
+        )
+        parser.add_argument(
+            "--rir_scp",
+            type=str_or_none,
+            default=None,
+            help="The file path of rir scp file.",
+        )
+        parser.add_argument(
+            "--rir_apply_prob",
+            type=float,
+            default=1.0,
+            help="THe probability for applying RIR convolution.",
+        )
+        parser.add_argument(
+            "--cmvn_file",
+            type=str_or_none,
+            default=None,
+            help="The file path of noise scp file.",
+        )
+        parser.add_argument(
+            "--noise_scp",
+            type=str_or_none,
+            default=None,
+            help="The file path of noise scp file.",
+        )
+        parser.add_argument(
+            "--noise_apply_prob",
+            type=float,
+            default=1.0,
+            help="The probability applying Noise adding.",
+        )
+        parser.add_argument(
+            "--noise_db_range",
+            type=str,
+            default="13_15",
+            help="The range of noise decibel level.",
+        )
+
+        for class_choices in cls.class_choices_list:
+            # Append --<name> and --<name>_conf.
+            # e.g. --encoder and --encoder_conf
+            class_choices.add_arguments(group)
+
+    @classmethod
+    def build_collate_fn(
+            cls, args: argparse.Namespace, train: bool
+    ) -> Callable[
+        [Collection[Tuple[str, Dict[str, np.ndarray]]]],
+        Tuple[List[str], Dict[str, torch.Tensor]],
+    ]:
         assert check_argument_types()
+        # NOTE(kamo): int value = 0 is reserved by CTC-blank symbol
+        return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
 
-        # Input as audio signal
-        if isinstance(speech, np.ndarray):
-            speech = torch.tensor(speech)
-        batch_size = speech.shape[0]
-        segments = [[]] * batch_size
-        if self.frontend is not None:
-            feats, feats_len = self.frontend.forward(speech, speech_lengths, is_final)
-            fbanks, _ = self.frontend.get_fbank()
+    @classmethod
+    def build_preprocess_fn(
+            cls, args: argparse.Namespace, train: bool
+    ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
+        assert check_argument_types()
+        # if args.use_preprocessor:
+        #    retval = CommonPreprocessor(
+        #        train=train,
+        #        # NOTE(kamo): Check attribute existence for backward compatibility
+        #        rir_scp=args.rir_scp if hasattr(args, "rir_scp") else None,
+        #        rir_apply_prob=args.rir_apply_prob
+        #        if hasattr(args, "rir_apply_prob")
+        #        else 1.0,
+        #        noise_scp=args.noise_scp if hasattr(args, "noise_scp") else None,
+        #        noise_apply_prob=args.noise_apply_prob
+        #        if hasattr(args, "noise_apply_prob")
+        #        else 1.0,
+        #        noise_db_range=args.noise_db_range
+        #        if hasattr(args, "noise_db_range")
+        #        else "13_15",
+        #        speech_volume_normalize=args.speech_volume_normalize
+        #        if hasattr(args, "rir_scp")
+        #        else None,
+        #    )
+        # else:
+        #    retval = None
+        retval = None
+        assert check_return_type(retval)
+        return retval
+
+    @classmethod
+    def required_data_names(
+            cls, train: bool = True, inference: bool = False
+    ) -> Tuple[str, ...]:
+        if not inference:
+            retval = ("speech", "text")
         else:
-            raise Exception("Need to extract feats first, please configure frontend configuration")
-        if feats.shape[0]:
-            feats = to_device(feats, device=self.device)
-            feats_len = feats_len.int()
-            waveforms = self.frontend.get_waveforms()
-
-            batch = {
-                "feats": feats,
-                "waveform": waveforms,
-                "in_cache": in_cache,
-                "is_final": is_final,
-                "max_end_sil": max_end_sil
-            }
-            # a. To device
-            batch = to_device(batch, device=self.device)
-            segments, in_cache = self.vad_model.forward_online(**batch)
-            # in_cache.update(batch['in_cache'])
-            # in_cache = {key: value for key, value in batch['in_cache'].items()}
-        return fbanks, segments, in_cache
-
-
-def inference(
-        batch_size: int,
-        ngpu: int,
-        log_level: Union[int, str],
-        data_path_and_name_and_type,
-        vad_infer_config: Optional[str],
-        vad_model_file: Optional[str],
-        vad_cmvn_file: Optional[str] = None,
-        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        key_file: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        output_dir: Optional[str] = None,
-        dtype: str = "float32",
-        seed: int = 0,
-        num_workers: int = 1,
-        **kwargs,
-):
-    inference_pipeline = inference_modelscope(
-        batch_size=batch_size,
-        ngpu=ngpu,
-        log_level=log_level,
-        vad_infer_config=vad_infer_config,
-        vad_model_file=vad_model_file,
-        vad_cmvn_file=vad_cmvn_file,
-        key_file=key_file,
-        allow_variable_data_keys=allow_variable_data_keys,
-        output_dir=output_dir,
-        dtype=dtype,
-        seed=seed,
-        num_workers=num_workers,
-        **kwargs,
-    )
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs)
-
-
-def inference_modelscope(
-        batch_size: int,
-        ngpu: int,
-        log_level: Union[int, str],
-        # data_path_and_name_and_type,
-        vad_infer_config: Optional[str],
-        vad_model_file: Optional[str],
-        vad_cmvn_file: Optional[str] = None,
-        # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        key_file: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        output_dir: Optional[str] = None,
-        dtype: str = "float32",
-        seed: int = 0,
-        num_workers: int = 1,
-        **kwargs,
-):
-    assert check_argument_types()
-    if batch_size > 1:
-        raise NotImplementedError("batch decoding is not implemented")
-    if ngpu > 1:
-        raise NotImplementedError("only single GPU decoding is supported")
-
-    logging.basicConfig(
-        level=log_level,
-        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
-    )
-
-    if ngpu >= 1 and torch.cuda.is_available():
-        device = "cuda"
-    else:
-        device = "cpu"
-
-    # 1. Set random-seed
-    set_all_random_seed(seed)
-
-    # 2. Build speech2vadsegment
-    speech2vadsegment_kwargs = dict(
-        vad_infer_config=vad_infer_config,
-        vad_model_file=vad_model_file,
-        vad_cmvn_file=vad_cmvn_file,
-        device=device,
-        dtype=dtype,
-    )
-    logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
-    speech2vadsegment = Speech2VadSegmentOnline(**speech2vadsegment_kwargs)
-
-    def _forward(
-            data_path_and_name_and_type,
-            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-            output_dir_v2: Optional[str] = None,
-            fs: dict = None,
-            param_dict: dict = None,
-    ):
-        # 3. Build data-iterator
-        if data_path_and_name_and_type is None and raw_inputs is not None:
-            if isinstance(raw_inputs, torch.Tensor):
-                raw_inputs = raw_inputs.numpy()
-            data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = VADTask.build_streaming_iterator(
-            data_path_and_name_and_type,
-            dtype=dtype,
-            batch_size=batch_size,
-            key_file=key_file,
-            num_workers=num_workers,
-            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
-            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
-        )
+            # Recognition mode
+            retval = ("speech",)
+        return retval
+
+    @classmethod
+    def optional_data_names(
+            cls, train: bool = True, inference: bool = False
+    ) -> Tuple[str, ...]:
+        retval = ()
+        assert check_return_type(retval)
+        return retval
 
-        finish_count = 0
-        file_count = 1
-        # 7 .Start for-loop
-        # FIXME(kamo): The output format should be discussed about
-        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
-        if output_path is not None:
-            writer = DatadirWriter(output_path)
-            ibest_writer = writer[f"1best_recog"]
+    @classmethod
+    def build_model(cls, args: argparse.Namespace):
+        assert check_argument_types()
+        # 4. Encoder
+        encoder_class = encoder_choices.get_class(args.encoder)
+        encoder = encoder_class(**args.encoder_conf)
+
+        # 5. Build model
+        try:
+            model_class = model_choices.get_class(args.model)
+        except AttributeError:
+            model_class = model_choices.get_class("e2evad")
+        
+        # 1. frontend
+        if args.input_size is None:
+            # Extract features in the model
+            frontend_class = frontend_choices.get_class(args.frontend)
+            if args.frontend == 'wav_frontend':
+                frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
+            else:
+                frontend = frontend_class(**args.frontend_conf)
+            input_size = frontend.output_size()
         else:
-            writer = None
-            ibest_writer = None
+            # Give features from data-loader
+            args.frontend = None
+            args.frontend_conf = {}
+            frontend = None
+            input_size = args.input_size
+        
+        model = model_class(encoder=encoder, vad_post_args=args.vad_post_conf, frontend=frontend)
+
+        return model
+
+    # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
+    @classmethod
+    def build_model_from_file(
+            cls,
+            config_file: Union[Path, str] = None,
+            model_file: Union[Path, str] = None,
+            device: str = "cpu",
+            cmvn_file: Union[Path, str] = None,
+    ):
+        """Build model from the files.
+
+        This method is used for inference or fine-tuning.
+
+        Args:
+            config_file: The yaml file saved when training.
+            model_file: The model file saved when training.
+            device: Device type, "cpu", "cuda", or "cuda:N".
 
-        vad_results = []
-        batch_in_cache = param_dict['in_cache'] if param_dict is not None else dict()
-        is_final = param_dict.get('is_final', False) if param_dict is not None else False
-        max_end_sil = param_dict.get('max_end_sil', 800) if param_dict is not None else 800
-        for keys, batch in loader:
-            assert isinstance(batch, dict), type(batch)
-            assert all(isinstance(s, str) for s in keys), keys
-            _bs = len(next(iter(batch.values())))
-            assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-            batch['in_cache'] = batch_in_cache
-            batch['is_final'] = is_final
-            batch['max_end_sil'] = max_end_sil
-
-            # do vad segment
-            _, results, param_dict['in_cache'] = speech2vadsegment(**batch)
-            # param_dict['in_cache'] = batch['in_cache']
-            if results:
-                for i, _ in enumerate(keys):
-                    if results[i]:
-                        if "MODELSCOPE_ENVIRONMENT" in os.environ and os.environ["MODELSCOPE_ENVIRONMENT"] == "eas":
-                            results[i] = json.dumps(results[i])
-                        item = {'key': keys[i], 'value': results[i]}
-                        vad_results.append(item)
-                        if writer is not None:
-                            results[i] = json.loads(results[i])
-                            ibest_writer["text"][keys[i]] = "{}".format(results[i])
-
-        return vad_results
-
-    return _forward
-
-
-def get_parser():
-    parser = config_argparse.ArgumentParser(
-        description="VAD Decoding",
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-    )
-
-    # Note(kamo): Use '_' instead of '-' as separator.
-    # '-' is confusing if written in yaml.
-    parser.add_argument(
-        "--log_level",
-        type=lambda x: x.upper(),
-        default="INFO",
-        choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
-        help="The verbose level of logging",
-    )
-
-    parser.add_argument("--output_dir", type=str, required=False)
-    parser.add_argument(
-        "--ngpu",
-        type=int,
-        default=0,
-        help="The number of gpus. 0 indicates CPU mode",
-    )
-    parser.add_argument(
-        "--gpuid_list",
-        type=str,
-        default="",
-        help="The visible gpus",
-    )
-    parser.add_argument("--seed", type=int, default=0, help="Random seed")
-    parser.add_argument(
-        "--dtype",
-        default="float32",
-        choices=["float16", "float32", "float64"],
-        help="Data type",
-    )
-    parser.add_argument(
-        "--num_workers",
-        type=int,
-        default=1,
-        help="The number of workers used for DataLoader",
-    )
-
-    group = parser.add_argument_group("Input data related")
-    group.add_argument(
-        "--data_path_and_name_and_type",
-        type=str2triple_str,
-        required=False,
-        action="append",
-    )
-    group.add_argument("--raw_inputs", type=list, default=None)
-    # example=[{'key':'EdevDEWdIYQ_0021','file':'/mnt/data/jiangyu.xzy/test_data/speech_io/SPEECHIO_ASR_ZH00007_zhibodaihuo/wav/EdevDEWdIYQ_0021.wav'}])
-    group.add_argument("--key_file", type=str_or_none)
-    group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
-
-    group = parser.add_argument_group("The model configuration related")
-    group.add_argument(
-        "--vad_infer_config",
-        type=str,
-        help="VAD infer configuration",
-    )
-    group.add_argument(
-        "--vad_model_file",
-        type=str,
-        help="VAD model parameter file",
-    )
-    group.add_argument(
-        "--vad_cmvn_file",
-        type=str,
-        help="Global cmvn file",
-    )
-
-    group = parser.add_argument_group("infer related")
-    group.add_argument(
-        "--batch_size",
-        type=int,
-        default=1,
-        help="The batch size for inference",
-    )
-
-    return parser
-
-
-def main(cmd=None):
-    print(get_commandline_args(), file=sys.stderr)
-    parser = get_parser()
-    args = parser.parse_args(cmd)
-    kwargs = vars(args)
-    kwargs.pop("config", None)
-    inference(**kwargs)
+        """
+        assert check_argument_types()
+        if config_file is None:
+            assert model_file is not None, (
+                "The argument 'model_file' must be provided "
+                "if the argument 'config_file' is not specified."
+            )
+            config_file = Path(model_file).parent / "config.yaml"
+        else:
+            config_file = Path(config_file)
 
+        with config_file.open("r", encoding="utf-8") as f:
+            args = yaml.safe_load(f)
+        #if cmvn_file is not None:
+        args["cmvn_file"] = cmvn_file
+        args = argparse.Namespace(**args)
+        model = cls.build_model(args)
+        model.to(device)
+        model_dict = dict()
+        model_name_pth = None
+        if model_file is not None:
+            logging.info("model_file is {}".format(model_file))
+            if device == "cuda":
+                device = f"cuda:{torch.cuda.current_device()}"
+            model_dir = os.path.dirname(model_file)
+            model_name = os.path.basename(model_file)
+            model_dict = torch.load(model_file, map_location=device)
+        model.encoder.load_state_dict(model_dict)
 
-if __name__ == "__main__":
-    main()
+        return model, args
```

### Comparing `funasr-0.4.1/funasr/datasets/collate_fn.py` & `funasr-0.4.2/funasr/datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/datasets/dataset.py` & `funasr-0.4.2/funasr/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/datasets/iterable_dataset.py` & `funasr-0.4.2/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/datasets/iterable_dataset_modelscope.py` & `funasr-0.4.2/funasr/datasets/iterable_dataset_modelscope.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.4.2/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.4.2/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.4.2/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/datasets/large_datasets/dataset.py` & `funasr-0.4.2/funasr/datasets/large_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.4.2/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.4.2/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.4.2/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.4.2/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.4.2/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         word_list.append(longest_word)
         i += len(longest_word)
     return word_list
 
 def seg_tokenize(txt, seg_dict):
     out_txt = ""
     for word in txt:
+        word = word.lower()
         if word in seg_dict:
             out_txt += seg_dict[word] + " "
         else:
             out_txt += "<unk>" + " "
     return out_txt.strip().split()
 
 def tokenize(data,
@@ -37,16 +38,15 @@
     vad = -2
 
     if bpe_tokenizer is not None:
         text = bpe_tokenizer.text2tokens("".join(text))
 
     if seg_dict is not None:
         assert isinstance(seg_dict, dict)
-        txt = forward_segment("".join(text).lower(), seg_dict)
-        text = seg_tokenize(txt, seg_dict)
+        text = seg_tokenize(text, seg_dict)
 
     length = len(text)
     for i in range(length):
         x = text[i]
         if i == length-1 and "punc" in data and x.startswith("vad:"):
             vad = x[4:]
             if len(vad) == 0:
```

### Comparing `funasr-0.4.1/funasr/datasets/ms_dataset.py` & `funasr-0.4.2/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/datasets/preprocessor.py` & `funasr-0.4.2/funasr/datasets/preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         i += len(longest_word)
     return word_list
 
 
 def seg_tokenize(txt, seg_dict):
     out_txt = ""
     for word in txt:
+        word = word.lower()
         if word in seg_dict:
             out_txt += seg_dict[word] + " "
         else:
             out_txt += "<unk>" + " "
     return out_txt.strip().split()
 
 def seg_tokenize_wo_pattern(txt, seg_dict):
@@ -355,15 +356,14 @@
     ) -> Dict[str, np.ndarray]:
         if self.text_name in data and self.tokenizer is not None:
             text = data[self.text_name]
             text = self.text_cleaner(text)
             if self.split_with_space:
                 tokens = text.strip().split(" ")
                 if self.seg_dict is not None:
-                    tokens = forward_segment("".join(tokens), self.seg_dict)
                     tokens = seg_tokenize(tokens, self.seg_dict)
             else:
                 tokens = self.tokenizer.text2tokens(text)
             text_ints = self.token_id_converter.tokens2ids(tokens)
             data[self.text_name] = np.array(text_ints, dtype=np.int64)
         assert check_return_type(data)
         return data
```

### Comparing `funasr-0.4.1/funasr/export/export_model.py` & `funasr-0.4.2/funasr/export/export_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/models/CT_Transformer.py` & `funasr-0.4.2/funasr/export/models/CT_Transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/models/__init__.py` & `funasr-0.4.2/funasr/export/models/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.4.2/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.4.2/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.4.2/funasr/export/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/models/e2e_vad.py` & `funasr-0.4.2/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.4.2/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.4.2/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.4.2/funasr/export/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/models/modules/decoder_layer.py` & `funasr-0.4.2/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/models/modules/encoder_layer.py` & `funasr-0.4.2/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/models/modules/feedforward.py` & `funasr-0.4.2/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/models/modules/multihead_att.py` & `funasr-0.4.2/funasr/export/models/modules/multihead_att.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/models/predictor/cif.py` & `funasr-0.4.2/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/test/test_onnx.py` & `funasr-0.4.2/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/test/test_onnx_punc.py` & `funasr-0.4.2/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.4.2/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/test/test_onnx_vad.py` & `funasr-0.4.2/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/torch_quant/__init__.py` & `funasr-0.4.2/funasr/export/torch_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/torch_quant/amp_module.py` & `funasr-0.4.2/funasr/export/torch_quant/amp_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/torch_quant/graph.py` & `funasr-0.4.2/funasr/export/torch_quant/graph.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/torch_quant/module.py` & `funasr-0.4.2/funasr/export/torch_quant/module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/torch_quant/observed_module.py` & `funasr-0.4.2/funasr/export/torch_quant/observed_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/torch_quant/observer.py` & `funasr-0.4.2/funasr/export/torch_quant/observer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/torch_quant/quantizer.py` & `funasr-0.4.2/funasr/export/torch_quant/quantizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/torch_quant/version.py` & `funasr-0.4.2/funasr/export/torch_quant/version.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/export/utils/torch_function.py` & `funasr-0.4.2/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/fileio/datadir_writer.py` & `funasr-0.4.2/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/fileio/npy_scp.py` & `funasr-0.4.2/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/fileio/rand_gen_dataset.py` & `funasr-0.4.2/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/fileio/read_text.py` & `funasr-0.4.2/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/fileio/sound_scp.py` & `funasr-0.4.2/funasr/fileio/sound_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/iterators/chunk_iter_factory.py` & `funasr-0.4.2/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/iterators/multiple_iter_factory.py` & `funasr-0.4.2/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/iterators/sequence_iter_factory.py` & `funasr-0.4.2/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/layers/complex_utils.py` & `funasr-0.4.2/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/layers/global_mvn.py` & `funasr-0.4.2/funasr/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/layers/label_aggregation.py` & `funasr-0.4.2/funasr/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/layers/log_mel.py` & `funasr-0.4.2/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/layers/mask_along_axis.py` & `funasr-0.4.2/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/layers/sinc_conv.py` & `funasr-0.4.2/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/layers/stft.py` & `funasr-0.4.2/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/layers/time_warp.py` & `funasr-0.4.2/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/layers/utterance_mvn.py` & `funasr-0.4.2/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/lm/abs_model.py` & `funasr-0.4.2/funasr/lm/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/lm/seq_rnn_lm.py` & `funasr-0.4.2/funasr/lm/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/lm/transformer_lm.py` & `funasr-0.4.2/funasr/lm/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/losses/label_smoothing_loss.py` & `funasr-0.4.2/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/main_funcs/average_nbest_models.py` & `funasr-0.4.2/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.4.2/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/main_funcs/collect_stats.py` & `funasr-0.4.2/funasr/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/main_funcs/pack_funcs.py` & `funasr-0.4.2/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/ctc.py` & `funasr-0.4.2/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/data2vec.py` & `funasr-0.4.2/funasr/models/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/decoder/contextual_decoder.py` & `funasr-0.4.2/funasr/models/decoder/contextual_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/decoder/rnn_decoder.py` & `funasr-0.4.2/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/decoder/sanm_decoder.py` & `funasr-0.4.2/funasr/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/decoder/sv_decoder.py` & `funasr-0.4.2/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/decoder/transformer_decoder.py` & `funasr-0.4.2/funasr/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/e2e_asr.py` & `funasr-0.4.2/funasr/models/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/e2e_asr_common.py` & `funasr-0.4.2/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/e2e_asr_mfcca.py` & `funasr-0.4.2/funasr/models/e2e_asr_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/e2e_asr_paraformer.py` & `funasr-0.4.2/funasr/models/e2e_asr_paraformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,94 +321,31 @@
         )
 
         if intermediate_outs is not None:
             return (encoder_out, intermediate_outs), encoder_out_lens
 
         return encoder_out, encoder_out_lens
 
-    def encode_chunk(
-            self, speech: torch.Tensor, speech_lengths: torch.Tensor, cache: dict = None
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
-        """Frontend + Encoder. Note that this method is used by asr_inference.py
-
-        Args:
-                speech: (Batch, Length, ...)
-                speech_lengths: (Batch, )
-        """
-        with autocast(False):
-            # 1. Extract feats
-            feats, feats_lengths = self._extract_feats(speech, speech_lengths)
-
-            # 2. Data augmentation
-            if self.specaug is not None and self.training:
-                feats, feats_lengths = self.specaug(feats, feats_lengths)
-
-            # 3. Normalization for feature: e.g. Global-CMVN, Utterance-CMVN
-            if self.normalize is not None:
-                feats, feats_lengths = self.normalize(feats, feats_lengths)
-
-        # Pre-encoder, e.g. used for raw input data
-        if self.preencoder is not None:
-            feats, feats_lengths = self.preencoder(feats, feats_lengths)
-
-        # 4. Forward encoder
-        # feats: (Batch, Length, Dim)
-        # -> encoder_out: (Batch, Length2, Dim2)
-        if self.encoder.interctc_use_conditioning:
-            encoder_out, encoder_out_lens, _ = self.encoder.forward_chunk(
-                feats, feats_lengths, cache=cache["encoder"], ctc=self.ctc
-            )
-        else:
-            encoder_out, encoder_out_lens, _ = self.encoder.forward_chunk(feats, feats_lengths, cache=cache["encoder"])
-        intermediate_outs = None
-        if isinstance(encoder_out, tuple):
-            intermediate_outs = encoder_out[1]
-            encoder_out = encoder_out[0]
-
-        # Post-encoder, e.g. NLU
-        if self.postencoder is not None:
-            encoder_out, encoder_out_lens = self.postencoder(
-                encoder_out, encoder_out_lens
-            )
-
-        if intermediate_outs is not None:
-            return (encoder_out, intermediate_outs), encoder_out_lens
-
-        return encoder_out, torch.tensor([encoder_out.size(1)])
-
     def calc_predictor(self, encoder_out, encoder_out_lens):
 
         encoder_out_mask = (~make_pad_mask(encoder_out_lens, maxlen=encoder_out.size(1))[:, None, :]).to(
             encoder_out.device)
         pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index = self.predictor(encoder_out, None, encoder_out_mask,
                                                                                   ignore_id=self.ignore_id)
         return pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index
 
-    def calc_predictor_chunk(self, encoder_out, cache=None):
-
-        pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index = self.predictor.forward_chunk(encoder_out, cache["encoder"])
-        return pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index
-
     def cal_decoder_with_predictor(self, encoder_out, encoder_out_lens, sematic_embeds, ys_pad_lens):
 
         decoder_outs = self.decoder(
             encoder_out, encoder_out_lens, sematic_embeds, ys_pad_lens
         )
         decoder_out = decoder_outs[0]
         decoder_out = torch.log_softmax(decoder_out, dim=-1)
         return decoder_out, ys_pad_lens
 
-    def cal_decoder_with_predictor_chunk(self, encoder_out, sematic_embeds, cache=None):
-        decoder_outs = self.decoder.forward_chunk(
-            encoder_out, sematic_embeds, cache["decoder"]
-        )
-        decoder_out = decoder_outs
-        decoder_out = torch.log_softmax(decoder_out, dim=-1)
-        return decoder_out
-
     def _extract_feats(
             self, speech: torch.Tensor, speech_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         assert speech_lengths.dim() == 1, speech_lengths.shape
 
         # for data-parallel
         speech = speech[:, : speech_lengths.max()]
@@ -606,14 +543,192 @@
         cer_ctc = None
         if not self.training and self.error_calculator is not None:
             ys_hat = self.ctc.argmax(encoder_out).data
             cer_ctc = self.error_calculator(ys_hat.cpu(), ys_pad.cpu(), is_ctc=True)
         return loss_ctc, cer_ctc
 
 
+class ParaformerOnline(Paraformer):
+    """
+    Author: Speech Lab, Alibaba Group, China
+    Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition
+    https://arxiv.org/abs/2206.08317
+    """
+
+    def __init__(
+            self, *args, **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+
+    def forward(
+            self,
+            speech: torch.Tensor,
+            speech_lengths: torch.Tensor,
+            text: torch.Tensor,
+            text_lengths: torch.Tensor,
+    ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], torch.Tensor]:
+        """Frontend + Encoder + Decoder + Calc loss
+        Args:
+                speech: (Batch, Length, ...)
+                speech_lengths: (Batch, )
+                text: (Batch, Length)
+                text_lengths: (Batch,)
+        """
+        assert text_lengths.dim() == 1, text_lengths.shape
+        # Check that batch_size is unified
+        assert (
+                speech.shape[0]
+                == speech_lengths.shape[0]
+                == text.shape[0]
+                == text_lengths.shape[0]
+        ), (speech.shape, speech_lengths.shape, text.shape, text_lengths.shape)
+        batch_size = speech.shape[0]
+        self.step_cur += 1
+        # for data-parallel
+        text = text[:, : text_lengths.max()]
+        speech = speech[:, :speech_lengths.max()]
+
+        # 1. Encoder
+        encoder_out, encoder_out_lens = self.encode(speech, speech_lengths)
+        intermediate_outs = None
+        if isinstance(encoder_out, tuple):
+            intermediate_outs = encoder_out[1]
+            encoder_out = encoder_out[0]
+
+        loss_att, acc_att, cer_att, wer_att = None, None, None, None
+        loss_ctc, cer_ctc = None, None
+        loss_pre = None
+        stats = dict()
+
+        # 1. CTC branch
+        if self.ctc_weight != 0.0:
+            loss_ctc, cer_ctc = self._calc_ctc_loss(
+                encoder_out, encoder_out_lens, text, text_lengths
+            )
+
+            # Collect CTC branch stats
+            stats["loss_ctc"] = loss_ctc.detach() if loss_ctc is not None else None
+            stats["cer_ctc"] = cer_ctc
+
+        # Intermediate CTC (optional)
+        loss_interctc = 0.0
+        if self.interctc_weight != 0.0 and intermediate_outs is not None:
+            for layer_idx, intermediate_out in intermediate_outs:
+                # we assume intermediate_out has the same length & padding
+                # as those of encoder_out
+                loss_ic, cer_ic = self._calc_ctc_loss(
+                    intermediate_out, encoder_out_lens, text, text_lengths
+                )
+                loss_interctc = loss_interctc + loss_ic
+
+                # Collect Intermedaite CTC stats
+                stats["loss_interctc_layer{}".format(layer_idx)] = (
+                    loss_ic.detach() if loss_ic is not None else None
+                )
+                stats["cer_interctc_layer{}".format(layer_idx)] = cer_ic
+
+            loss_interctc = loss_interctc / len(intermediate_outs)
+
+            # calculate whole encoder loss
+            loss_ctc = (
+                               1 - self.interctc_weight
+                       ) * loss_ctc + self.interctc_weight * loss_interctc
+
+        # 2b. Attention decoder branch
+        if self.ctc_weight != 1.0:
+            loss_att, acc_att, cer_att, wer_att, loss_pre = self._calc_att_loss(
+                encoder_out, encoder_out_lens, text, text_lengths
+            )
+
+        # 3. CTC-Att loss definition
+        if self.ctc_weight == 0.0:
+            loss = loss_att + loss_pre * self.predictor_weight
+        elif self.ctc_weight == 1.0:
+            loss = loss_ctc
+        else:
+            loss = self.ctc_weight * loss_ctc + (1 - self.ctc_weight) * loss_att + loss_pre * self.predictor_weight
+
+        # Collect Attn branch stats
+        stats["loss_att"] = loss_att.detach() if loss_att is not None else None
+        stats["acc"] = acc_att
+        stats["cer"] = cer_att
+        stats["wer"] = wer_att
+        stats["loss_pre"] = loss_pre.detach().cpu() if loss_pre is not None else None
+
+        stats["loss"] = torch.clone(loss.detach())
+
+        # force_gatherable: to-device and to-tensor if scalar for DataParallel
+        loss, stats, weight = force_gatherable((loss, stats, batch_size), loss.device)
+        return loss, stats, weight
+
+    def encode_chunk(
+            self, speech: torch.Tensor, speech_lengths: torch.Tensor, cache: dict = None
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        """Frontend + Encoder. Note that this method is used by asr_inference.py
+
+        Args:
+                speech: (Batch, Length, ...)
+                speech_lengths: (Batch, )
+        """
+        with autocast(False):
+            # 1. Extract feats
+            feats, feats_lengths = self._extract_feats(speech, speech_lengths)
+
+            # 2. Data augmentation
+            if self.specaug is not None and self.training:
+                feats, feats_lengths = self.specaug(feats, feats_lengths)
+
+            # 3. Normalization for feature: e.g. Global-CMVN, Utterance-CMVN
+            if self.normalize is not None:
+                feats, feats_lengths = self.normalize(feats, feats_lengths)
+
+        # Pre-encoder, e.g. used for raw input data
+        if self.preencoder is not None:
+            feats, feats_lengths = self.preencoder(feats, feats_lengths)
+
+        # 4. Forward encoder
+        # feats: (Batch, Length, Dim)
+        # -> encoder_out: (Batch, Length2, Dim2)
+        if self.encoder.interctc_use_conditioning:
+            encoder_out, encoder_out_lens, _ = self.encoder.forward_chunk(
+                feats, feats_lengths, cache=cache["encoder"], ctc=self.ctc
+            )
+        else:
+            encoder_out, encoder_out_lens, _ = self.encoder.forward_chunk(feats, feats_lengths, cache=cache["encoder"])
+        intermediate_outs = None
+        if isinstance(encoder_out, tuple):
+            intermediate_outs = encoder_out[1]
+            encoder_out = encoder_out[0]
+
+        # Post-encoder, e.g. NLU
+        if self.postencoder is not None:
+            encoder_out, encoder_out_lens = self.postencoder(
+                encoder_out, encoder_out_lens
+            )
+
+        if intermediate_outs is not None:
+            return (encoder_out, intermediate_outs), encoder_out_lens
+
+        return encoder_out, torch.tensor([encoder_out.size(1)])
+
+    def calc_predictor_chunk(self, encoder_out, cache=None):
+
+        pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index = \
+            self.predictor.forward_chunk(encoder_out, cache["encoder"])
+        return pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index
+
+    def cal_decoder_with_predictor_chunk(self, encoder_out, sematic_embeds, cache=None):
+        decoder_outs = self.decoder.forward_chunk(
+            encoder_out, sematic_embeds, cache["decoder"]
+        )
+        decoder_out = decoder_outs
+        decoder_out = torch.log_softmax(decoder_out, dim=-1)
+        return decoder_out
+
+
 class ParaformerBert(Paraformer):
     """
     Author: Speech Lab of DAMO Academy, Alibaba Group
     Paraformer2: advanced paraformer with LFMMI and bert for non-autoregressive end-to-end speech recognition
     """
 
     def __init__(
@@ -973,14 +1088,67 @@
             ys_pad_lens = ys_pad_lens + self.predictor_bias
         _, _, _, _, pre_token_length2 = self.predictor(encoder_out, ys_pad, encoder_out_mask, ignore_id=self.ignore_id)
 
         # loss_pre = self.criterion_pre(ys_pad_lens.type_as(pre_token_length), pre_token_length)
         loss_pre2 = self.criterion_pre(ys_pad_lens.type_as(pre_token_length2), pre_token_length2)
 
         return loss_pre2
+
+    def _calc_att_loss(
+            self,
+            encoder_out: torch.Tensor,
+            encoder_out_lens: torch.Tensor,
+            ys_pad: torch.Tensor,
+            ys_pad_lens: torch.Tensor,
+    ):
+        encoder_out_mask = (~make_pad_mask(encoder_out_lens, maxlen=encoder_out.size(1))[:, None, :]).to(
+            encoder_out.device)
+        if self.predictor_bias == 1:
+            _, ys_pad = add_sos_eos(ys_pad, self.sos, self.eos, self.ignore_id)
+            ys_pad_lens = ys_pad_lens + self.predictor_bias
+        pre_acoustic_embeds, pre_token_length, _, pre_peak_index, _ = self.predictor(encoder_out, ys_pad, encoder_out_mask,
+                                                                                  ignore_id=self.ignore_id)
+
+        # 0. sampler
+        decoder_out_1st = None
+        if self.sampling_ratio > 0.0:
+            if self.step_cur < 2:
+                logging.info("enable sampler in paraformer, sampling_ratio: {}".format(self.sampling_ratio))
+            sematic_embeds, decoder_out_1st = self.sampler(encoder_out, encoder_out_lens, ys_pad, ys_pad_lens,
+                                                           pre_acoustic_embeds)
+        else:
+            if self.step_cur < 2:
+                logging.info("disable sampler in paraformer, sampling_ratio: {}".format(self.sampling_ratio))
+            sematic_embeds = pre_acoustic_embeds
+
+        # 1. Forward decoder
+        decoder_outs = self.decoder(
+            encoder_out, encoder_out_lens, sematic_embeds, ys_pad_lens
+        )
+        decoder_out, _ = decoder_outs[0], decoder_outs[1]
+
+        if decoder_out_1st is None:
+            decoder_out_1st = decoder_out
+        # 2. Compute attention loss
+        loss_att = self.criterion_att(decoder_out, ys_pad)
+        acc_att = th_accuracy(
+            decoder_out_1st.view(-1, self.vocab_size),
+            ys_pad,
+            ignore_label=self.ignore_id,
+        )
+        loss_pre = self.criterion_pre(ys_pad_lens.type_as(pre_token_length), pre_token_length)
+
+        # Compute cer/wer using attention-decoder
+        if self.training or self.error_calculator is None:
+            cer_att, wer_att = None, None
+        else:
+            ys_hat = decoder_out_1st.argmax(dim=-1)
+            cer_att, wer_att = self.error_calculator(ys_hat.cpu(), ys_pad.cpu())
+
+        return loss_att, acc_att, cer_att, wer_att, loss_pre
     
     def calc_predictor(self, encoder_out, encoder_out_lens):
 
         encoder_out_mask = (~make_pad_mask(encoder_out_lens, maxlen=encoder_out.size(1))[:, None, :]).to(
             encoder_out.device)
         pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index, pre_token_length2 = self.predictor(encoder_out, None, encoder_out_mask,
                                                                                   ignore_id=self.ignore_id)
```

### Comparing `funasr-0.4.1/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.4.2/funasr/models/e2e_diar_eend_ola.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/e2e_diar_sond.py` & `funasr-0.4.2/funasr/models/e2e_diar_sond.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/e2e_sv.py` & `funasr-0.4.2/funasr/models/e2e_sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/e2e_tp.py` & `funasr-0.4.2/funasr/models/e2e_tp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/e2e_uni_asr.py` & `funasr-0.4.2/funasr/models/e2e_uni_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/e2e_vad.py` & `funasr-0.4.2/funasr/models/e2e_vad.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
             self.data_buf_all = torch.cat((self.data_buf_all, self.waveform[0]))
         for offset in range(0, self.waveform.shape[1] - frame_sample_length + 1, frame_shift_length):
             self.decibel.append(
                 10 * math.log10((self.waveform[0][offset: offset + frame_sample_length]).square().sum() + \
                                 0.000001))
 
     def ComputeScores(self, feats: torch.Tensor, in_cache: Dict[str, torch.Tensor]) -> None:
-        scores = self.encoder(feats, in_cache)  # return B * T * D
+        scores = self.encoder(feats, in_cache).to('cpu')  # return B * T * D
         assert scores.shape[1] == feats.shape[1], "The shape between feats and scores does not match"
         self.vad_opts.nn_eval_block_size = scores.shape[1]
         self.frm_cnt += scores.shape[1]  # count total frames
         if self.scores is None:
             self.scores = scores  # the first calculation
         else:
             self.scores = torch.cat((self.scores, scores), dim=1)
```

### Comparing `funasr-0.4.1/funasr/models/encoder/conformer_encoder.py` & `funasr-0.4.2/funasr/models/encoder/transformer_encoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,136 +1,57 @@
-# Copyright 2020 Tomoki Hayashi
+# Copyright 2019 Shigeki Karita
 #  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
-"""Conformer encoder definition."""
+"""Transformer encoder definition."""
 
-import logging
 from typing import List
 from typing import Optional
 from typing import Tuple
-from typing import Union
 
 import torch
 from torch import nn
 from typeguard import check_argument_types
+import logging
 
 from funasr.models.ctc import CTC
 from funasr.models.encoder.abs_encoder import AbsEncoder
-from funasr.modules.attention import (
-    MultiHeadedAttention,  # noqa: H301
-    RelPositionMultiHeadedAttention,  # noqa: H301
-    LegacyRelPositionMultiHeadedAttention,  # noqa: H301
-)
-from funasr.modules.embedding import (
-    PositionalEncoding,  # noqa: H301
-    ScaledPositionalEncoding,  # noqa: H301
-    RelPositionalEncoding,  # noqa: H301
-    LegacyRelPositionalEncoding,  # noqa: H301
-)
+from funasr.modules.attention import MultiHeadedAttention
+from funasr.modules.embedding import PositionalEncoding
 from funasr.modules.layer_norm import LayerNorm
 from funasr.modules.multi_layer_conv import Conv1dLinear
 from funasr.modules.multi_layer_conv import MultiLayeredConv1d
-from funasr.modules.nets_utils import get_activation
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.modules.positionwise_feed_forward import (
     PositionwiseFeedForward,  # noqa: H301
 )
 from funasr.modules.repeat import repeat
+from funasr.modules.nets_utils import rename_state_dict
+from funasr.modules.dynamic_conv import DynamicConvolution
+from funasr.modules.dynamic_conv2d import DynamicConvolution2D
+from funasr.modules.lightconv import LightweightConvolution
+from funasr.modules.lightconv2d import LightweightConvolution2D
 from funasr.modules.subsampling import Conv2dSubsampling
 from funasr.modules.subsampling import Conv2dSubsampling2
 from funasr.modules.subsampling import Conv2dSubsampling6
 from funasr.modules.subsampling import Conv2dSubsampling8
 from funasr.modules.subsampling import TooShortUttError
 from funasr.modules.subsampling import check_short_utt
-from funasr.modules.subsampling import Conv2dSubsamplingPad
-class ConvolutionModule(nn.Module):
-    """ConvolutionModule in Conformer model.
-
-    Args:
-        channels (int): The number of channels of conv layers.
-        kernel_size (int): Kernerl size of conv layers.
-
-    """
-
-    def __init__(self, channels, kernel_size, activation=nn.ReLU(), bias=True):
-        """Construct an ConvolutionModule object."""
-        super(ConvolutionModule, self).__init__()
-        # kernerl_size should be a odd number for 'SAME' padding
-        assert (kernel_size - 1) % 2 == 0
-
-        self.pointwise_conv1 = nn.Conv1d(
-            channels,
-            2 * channels,
-            kernel_size=1,
-            stride=1,
-            padding=0,
-            bias=bias,
-        )
-        self.depthwise_conv = nn.Conv1d(
-            channels,
-            channels,
-            kernel_size,
-            stride=1,
-            padding=(kernel_size - 1) // 2,
-            groups=channels,
-            bias=bias,
-        )
-        self.norm = nn.BatchNorm1d(channels)
-        self.pointwise_conv2 = nn.Conv1d(
-            channels,
-            channels,
-            kernel_size=1,
-            stride=1,
-            padding=0,
-            bias=bias,
-        )
-        self.activation = activation
-
-    def forward(self, x):
-        """Compute convolution module.
-
-        Args:
-            x (torch.Tensor): Input tensor (#batch, time, channels).
-
-        Returns:
-            torch.Tensor: Output tensor (#batch, time, channels).
-
-        """
-        # exchange the temporal dimension and the feature dimension
-        x = x.transpose(1, 2)
-
-        # GLU mechanism
-        x = self.pointwise_conv1(x)  # (batch, 2*channel, dim)
-        x = nn.functional.glu(x, dim=1)  # (batch, channel, dim)
-
-        # 1D Depthwise Conv
-        x = self.depthwise_conv(x)
-        x = self.activation(self.norm(x))
-
-        x = self.pointwise_conv2(x)
-
-        return x.transpose(1, 2)
 
 
 class EncoderLayer(nn.Module):
     """Encoder layer module.
 
     Args:
         size (int): Input dimension.
         self_attn (torch.nn.Module): Self-attention module instance.
             `MultiHeadedAttention` or `RelPositionMultiHeadedAttention` instance
             can be used as the argument.
         feed_forward (torch.nn.Module): Feed-forward module instance.
             `PositionwiseFeedForward`, `MultiLayeredConv1d`, or `Conv1dLinear` instance
             can be used as the argument.
-        feed_forward_macaron (torch.nn.Module): Additional feed-forward module instance.
-            `PositionwiseFeedForward`, `MultiLayeredConv1d`, or `Conv1dLinear` instance
-            can be used as the argument.
-        conv_module (torch.nn.Module): Convolution module instance.
-            `ConvlutionModule` instance can be used as the argument.
         dropout_rate (float): Dropout rate.
         normalize_before (bool): Whether to use layer_norm before the first block.
         concat_after (bool): Whether to concat attention layer's input and output.
             if True, additional linear will be applied.
             i.e. x -> x + linear(concat(x, att(x)))
             if False, no additional linear will be applied. i.e. x -> x + att(x)
         stochastic_depth_rate (float): Proability to skip this layer.
@@ -139,309 +60,178 @@
     """
 
     def __init__(
             self,
             size,
             self_attn,
             feed_forward,
-            feed_forward_macaron,
-            conv_module,
             dropout_rate,
             normalize_before=True,
             concat_after=False,
             stochastic_depth_rate=0.0,
     ):
         """Construct an EncoderLayer object."""
         super(EncoderLayer, self).__init__()
         self.self_attn = self_attn
         self.feed_forward = feed_forward
-        self.feed_forward_macaron = feed_forward_macaron
-        self.conv_module = conv_module
-        self.norm_ff = LayerNorm(size)  # for the FNN module
-        self.norm_mha = LayerNorm(size)  # for the MHA module
-        if feed_forward_macaron is not None:
-            self.norm_ff_macaron = LayerNorm(size)
-            self.ff_scale = 0.5
-        else:
-            self.ff_scale = 1.0
-        if self.conv_module is not None:
-            self.norm_conv = LayerNorm(size)  # for the CNN module
-            self.norm_final = LayerNorm(size)  # for the final output of the block
+        self.norm1 = LayerNorm(size)
+        self.norm2 = LayerNorm(size)
         self.dropout = nn.Dropout(dropout_rate)
         self.size = size
         self.normalize_before = normalize_before
         self.concat_after = concat_after
         if self.concat_after:
             self.concat_linear = nn.Linear(size + size, size)
         self.stochastic_depth_rate = stochastic_depth_rate
 
-    def forward(self, x_input, mask, cache=None):
+    def forward(self, x, mask, cache=None):
         """Compute encoded features.
 
         Args:
-            x_input (Union[Tuple, torch.Tensor]): Input tensor w/ or w/o pos emb.
-                - w/ pos emb: Tuple of tensors [(#batch, time, size), (1, time, size)].
-                - w/o pos emb: Tensor (#batch, time, size).
+            x_input (torch.Tensor): Input tensor (#batch, time, size).
             mask (torch.Tensor): Mask tensor for the input (#batch, time).
             cache (torch.Tensor): Cache tensor of the input (#batch, time - 1, size).
 
         Returns:
             torch.Tensor: Output tensor (#batch, time, size).
             torch.Tensor: Mask tensor (#batch, time).
 
         """
-        if isinstance(x_input, tuple):
-            x, pos_emb = x_input[0], x_input[1]
-        else:
-            x, pos_emb = x_input, None
-
         skip_layer = False
         # with stochastic depth, residual connection `x + f(x)` becomes
         # `x <- x + 1 / (1 - p) * f(x)` at training time.
         stoch_layer_coeff = 1.0
         if self.training and self.stochastic_depth_rate > 0:
             skip_layer = torch.rand(1).item() < self.stochastic_depth_rate
             stoch_layer_coeff = 1.0 / (1 - self.stochastic_depth_rate)
 
         if skip_layer:
             if cache is not None:
                 x = torch.cat([cache, x], dim=1)
-            if pos_emb is not None:
-                return (x, pos_emb), mask
             return x, mask
 
-        # whether to use macaron style
-        if self.feed_forward_macaron is not None:
-            residual = x
-            if self.normalize_before:
-                x = self.norm_ff_macaron(x)
-            x = residual + stoch_layer_coeff * self.ff_scale * self.dropout(
-                self.feed_forward_macaron(x)
-            )
-            if not self.normalize_before:
-                x = self.norm_ff_macaron(x)
-
-        # multi-headed self-attention module
         residual = x
         if self.normalize_before:
-            x = self.norm_mha(x)
+            x = self.norm1(x)
 
         if cache is None:
             x_q = x
         else:
             assert cache.shape == (x.shape[0], x.shape[1] - 1, self.size)
             x_q = x[:, -1:, :]
             residual = residual[:, -1:, :]
             mask = None if mask is None else mask[:, -1:, :]
 
-        if pos_emb is not None:
-            x_att = self.self_attn(x_q, x, x, pos_emb, mask)
-        else:
-            x_att = self.self_attn(x_q, x, x, mask)
-
         if self.concat_after:
-            x_concat = torch.cat((x, x_att), dim=-1)
+            x_concat = torch.cat((x, self.self_attn(x_q, x, x, mask)), dim=-1)
             x = residual + stoch_layer_coeff * self.concat_linear(x_concat)
         else:
-            x = residual + stoch_layer_coeff * self.dropout(x_att)
+            x = residual + stoch_layer_coeff * self.dropout(
+                self.self_attn(x_q, x, x, mask)
+            )
         if not self.normalize_before:
-            x = self.norm_mha(x)
+            x = self.norm1(x)
 
-        # convolution module
-        if self.conv_module is not None:
-            residual = x
-            if self.normalize_before:
-                x = self.norm_conv(x)
-            x = residual + stoch_layer_coeff * self.dropout(self.conv_module(x))
-            if not self.normalize_before:
-                x = self.norm_conv(x)
-
-        # feed forward module
         residual = x
         if self.normalize_before:
-            x = self.norm_ff(x)
-        x = residual + stoch_layer_coeff * self.ff_scale * self.dropout(
-            self.feed_forward(x)
-        )
+            x = self.norm2(x)
+        x = residual + stoch_layer_coeff * self.dropout(self.feed_forward(x))
         if not self.normalize_before:
-            x = self.norm_ff(x)
-
-        if self.conv_module is not None:
-            x = self.norm_final(x)
+            x = self.norm2(x)
 
         if cache is not None:
             x = torch.cat([cache, x], dim=1)
 
-        if pos_emb is not None:
-            return (x, pos_emb), mask
-
         return x, mask
 
 
-class ConformerEncoder(AbsEncoder):
-    """Conformer encoder module.
+class TransformerEncoder(AbsEncoder):
+    """Transformer encoder module.
 
     Args:
-        input_size (int): Input dimension.
-        output_size (int): Dimension of attention.
-        attention_heads (int): The number of heads of multi head attention.
-        linear_units (int): The number of units of position-wise feed forward.
-        num_blocks (int): The number of decoder blocks.
-        dropout_rate (float): Dropout rate.
-        attention_dropout_rate (float): Dropout rate in attention.
-        positional_dropout_rate (float): Dropout rate after adding positional encoding.
-        input_layer (Union[str, torch.nn.Module]): Input layer type.
-        normalize_before (bool): Whether to use layer_norm before the first block.
-        concat_after (bool): Whether to concat attention layer's input and output.
-            If True, additional linear will be applied.
+        input_size: input dim
+        output_size: dimension of attention
+        attention_heads: the number of heads of multi head attention
+        linear_units: the number of units of position-wise feed forward
+        num_blocks: the number of decoder blocks
+        dropout_rate: dropout rate
+        attention_dropout_rate: dropout rate in attention
+        positional_dropout_rate: dropout rate after adding positional encoding
+        input_layer: input layer type
+        pos_enc_class: PositionalEncoding or ScaledPositionalEncoding
+        normalize_before: whether to use layer_norm before the first block
+        concat_after: whether to concat attention layer's input and output
+            if True, additional linear will be applied.
             i.e. x -> x + linear(concat(x, att(x)))
-            If False, no additional linear will be applied. i.e. x -> x + att(x)
-        positionwise_layer_type (str): "linear", "conv1d", or "conv1d-linear".
-        positionwise_conv_kernel_size (int): Kernel size of positionwise conv1d layer.
-        rel_pos_type (str): Whether to use the latest relative positional encoding or
-            the legacy one. The legacy relative positional encoding will be deprecated
-            in the future. More Details can be found in
-            https://github.com/espnet/espnet/pull/2816.
-        encoder_pos_enc_layer_type (str): Encoder positional encoding layer type.
-        encoder_attn_layer_type (str): Encoder attention layer type.
-        activation_type (str): Encoder activation function type.
-        macaron_style (bool): Whether to use macaron style for positionwise layer.
-        use_cnn_module (bool): Whether to use convolution module.
-        zero_triu (bool): Whether to zero the upper triangular part of attention matrix.
-        cnn_module_kernel (int): Kernerl size of convolution module.
-        padding_idx (int): Padding idx for input_layer=embed.
-
+            if False, no additional linear will be applied.
+            i.e. x -> x + att(x)
+        positionwise_layer_type: linear of conv1d
+        positionwise_conv_kernel_size: kernel size of positionwise conv1d layer
+        padding_idx: padding_idx for input_layer=embed
     """
 
     def __init__(
             self,
             input_size: int,
             output_size: int = 256,
             attention_heads: int = 4,
             linear_units: int = 2048,
             num_blocks: int = 6,
             dropout_rate: float = 0.1,
             positional_dropout_rate: float = 0.1,
             attention_dropout_rate: float = 0.0,
-            input_layer: str = "conv2d",
+            input_layer: Optional[str] = "conv2d",
+            pos_enc_class=PositionalEncoding,
             normalize_before: bool = True,
             concat_after: bool = False,
             positionwise_layer_type: str = "linear",
-            positionwise_conv_kernel_size: int = 3,
-            macaron_style: bool = False,
-            rel_pos_type: str = "legacy",
-            pos_enc_layer_type: str = "rel_pos",
-            selfattention_layer_type: str = "rel_selfattn",
-            activation_type: str = "swish",
-            use_cnn_module: bool = True,
-            zero_triu: bool = False,
-            cnn_module_kernel: int = 31,
+            positionwise_conv_kernel_size: int = 1,
             padding_idx: int = -1,
             interctc_layer_idx: List[int] = [],
             interctc_use_conditioning: bool = False,
-            stochastic_depth_rate: Union[float, List[float]] = 0.0,
     ):
         assert check_argument_types()
         super().__init__()
         self._output_size = output_size
 
-        if rel_pos_type == "legacy":
-            if pos_enc_layer_type == "rel_pos":
-                pos_enc_layer_type = "legacy_rel_pos"
-            if selfattention_layer_type == "rel_selfattn":
-                selfattention_layer_type = "legacy_rel_selfattn"
-        elif rel_pos_type == "latest":
-            assert selfattention_layer_type != "legacy_rel_selfattn"
-            assert pos_enc_layer_type != "legacy_rel_pos"
-        else:
-            raise ValueError("unknown rel_pos_type: " + rel_pos_type)
-
-        activation = get_activation(activation_type)
-        if pos_enc_layer_type == "abs_pos":
-            pos_enc_class = PositionalEncoding
-        elif pos_enc_layer_type == "scaled_abs_pos":
-            pos_enc_class = ScaledPositionalEncoding
-        elif pos_enc_layer_type == "rel_pos":
-            assert selfattention_layer_type == "rel_selfattn"
-            pos_enc_class = RelPositionalEncoding
-        elif pos_enc_layer_type == "legacy_rel_pos":
-            assert selfattention_layer_type == "legacy_rel_selfattn"
-            pos_enc_class = LegacyRelPositionalEncoding
-            logging.warning(
-                "Using legacy_rel_pos and it will be deprecated in the future."
-            )
-        else:
-            raise ValueError("unknown pos_enc_layer: " + pos_enc_layer_type)
-
         if input_layer == "linear":
             self.embed = torch.nn.Sequential(
                 torch.nn.Linear(input_size, output_size),
                 torch.nn.LayerNorm(output_size),
                 torch.nn.Dropout(dropout_rate),
+                torch.nn.ReLU(),
                 pos_enc_class(output_size, positional_dropout_rate),
             )
         elif input_layer == "conv2d":
-            self.embed = Conv2dSubsampling(
-                input_size,
-                output_size,
-                dropout_rate,
-                pos_enc_class(output_size, positional_dropout_rate),
-            )
-        elif input_layer == "conv2dpad":
-            self.embed = Conv2dSubsamplingPad(
-                input_size,
-                output_size,
-                dropout_rate,
-                pos_enc_class(output_size, positional_dropout_rate),
-            )
+            self.embed = Conv2dSubsampling(input_size, output_size, dropout_rate)
         elif input_layer == "conv2d2":
-            self.embed = Conv2dSubsampling2(
-                input_size,
-                output_size,
-                dropout_rate,
-                pos_enc_class(output_size, positional_dropout_rate),
-            )
+            self.embed = Conv2dSubsampling2(input_size, output_size, dropout_rate)
         elif input_layer == "conv2d6":
-            self.embed = Conv2dSubsampling6(
-                input_size,
-                output_size,
-                dropout_rate,
-                pos_enc_class(output_size, positional_dropout_rate),
-            )
+            self.embed = Conv2dSubsampling6(input_size, output_size, dropout_rate)
         elif input_layer == "conv2d8":
-            self.embed = Conv2dSubsampling8(
-                input_size,
-                output_size,
-                dropout_rate,
-                pos_enc_class(output_size, positional_dropout_rate),
-            )
+            self.embed = Conv2dSubsampling8(input_size, output_size, dropout_rate)
         elif input_layer == "embed":
             self.embed = torch.nn.Sequential(
                 torch.nn.Embedding(input_size, output_size, padding_idx=padding_idx),
                 pos_enc_class(output_size, positional_dropout_rate),
             )
-        elif isinstance(input_layer, torch.nn.Module):
-            self.embed = torch.nn.Sequential(
-                input_layer,
-                pos_enc_class(output_size, positional_dropout_rate),
-            )
         elif input_layer is None:
-            self.embed = torch.nn.Sequential(
-                pos_enc_class(output_size, positional_dropout_rate)
-            )
+            if input_size == output_size:
+                self.embed = None
+            else:
+                self.embed = torch.nn.Linear(input_size, output_size)
         else:
             raise ValueError("unknown input_layer: " + input_layer)
         self.normalize_before = normalize_before
         if positionwise_layer_type == "linear":
             positionwise_layer = PositionwiseFeedForward
             positionwise_layer_args = (
                 output_size,
                 linear_units,
                 dropout_rate,
-                activation,
             )
         elif positionwise_layer_type == "conv1d":
             positionwise_layer = MultiLayeredConv1d
             positionwise_layer_args = (
                 output_size,
                 linear_units,
                 positionwise_conv_kernel_size,
@@ -453,69 +243,25 @@
                 output_size,
                 linear_units,
                 positionwise_conv_kernel_size,
                 dropout_rate,
             )
         else:
             raise NotImplementedError("Support only linear or conv1d.")
-
-        if selfattention_layer_type == "selfattn":
-            encoder_selfattn_layer = MultiHeadedAttention
-            encoder_selfattn_layer_args = (
-                attention_heads,
-                output_size,
-                attention_dropout_rate,
-            )
-        elif selfattention_layer_type == "legacy_rel_selfattn":
-            assert pos_enc_layer_type == "legacy_rel_pos"
-            encoder_selfattn_layer = LegacyRelPositionMultiHeadedAttention
-            encoder_selfattn_layer_args = (
-                attention_heads,
-                output_size,
-                attention_dropout_rate,
-            )
-            logging.warning(
-                "Using legacy_rel_selfattn and it will be deprecated in the future."
-            )
-        elif selfattention_layer_type == "rel_selfattn":
-            assert pos_enc_layer_type == "rel_pos"
-            encoder_selfattn_layer = RelPositionMultiHeadedAttention
-            encoder_selfattn_layer_args = (
-                attention_heads,
-                output_size,
-                attention_dropout_rate,
-                zero_triu,
-            )
-        else:
-            raise ValueError("unknown encoder_attn_layer: " + selfattention_layer_type)
-
-        convolution_layer = ConvolutionModule
-        convolution_layer_args = (output_size, cnn_module_kernel, activation)
-
-        if isinstance(stochastic_depth_rate, float):
-            stochastic_depth_rate = [stochastic_depth_rate] * num_blocks
-
-        if len(stochastic_depth_rate) != num_blocks:
-            raise ValueError(
-                f"Length of stochastic_depth_rate ({len(stochastic_depth_rate)}) "
-                f"should be equal to num_blocks ({num_blocks})"
-            )
-
         self.encoders = repeat(
             num_blocks,
             lambda lnum: EncoderLayer(
                 output_size,
-                encoder_selfattn_layer(*encoder_selfattn_layer_args),
+                MultiHeadedAttention(
+                    attention_heads, output_size, attention_dropout_rate
+                ),
                 positionwise_layer(*positionwise_layer_args),
-                positionwise_layer(*positionwise_layer_args) if macaron_style else None,
-                convolution_layer(*convolution_layer_args) if use_cnn_module else None,
                 dropout_rate,
                 normalize_before,
                 concat_after,
-                stochastic_depth_rate[lnum],
             ),
         )
         if self.normalize_before:
             self.after_norm = LayerNorm(output_size)
 
         self.interctc_layer_idx = interctc_layer_idx
         if len(interctc_layer_idx) > 0:
@@ -529,35 +275,32 @@
     def forward(
             self,
             xs_pad: torch.Tensor,
             ilens: torch.Tensor,
             prev_states: torch.Tensor = None,
             ctc: CTC = None,
     ) -> Tuple[torch.Tensor, torch.Tensor, Optional[torch.Tensor]]:
-        """Calculate forward propagation.
+        """Embed positions in tensor.
 
         Args:
-            xs_pad (torch.Tensor): Input tensor (#batch, L, input_size).
-            ilens (torch.Tensor): Input length (#batch).
-            prev_states (torch.Tensor): Not to be used now.
-
+            xs_pad: input tensor (B, L, D)
+            ilens: input length (B)
+            prev_states: Not to be used now.
         Returns:
-            torch.Tensor: Output tensor (#batch, L, output_size).
-            torch.Tensor: Output length (#batch).
-            torch.Tensor: Not to be used now.
-
+            position embedded tensor and mask
         """
         masks = (~make_pad_mask(ilens)[:, None, :]).to(xs_pad.device)
 
-        if (
+        if self.embed is None:
+            xs_pad = xs_pad
+        elif (
                 isinstance(self.embed, Conv2dSubsampling)
                 or isinstance(self.embed, Conv2dSubsampling2)
                 or isinstance(self.embed, Conv2dSubsampling6)
                 or isinstance(self.embed, Conv2dSubsampling8)
-                or isinstance(self.embed, Conv2dSubsamplingPad)
         ):
             short_status, limit_size = check_short_utt(self.embed, xs_pad.size(1))
             if short_status:
                 raise TooShortUttError(
                     f"has {xs_pad.size(1)} frames and is too short for subsampling "
                     + f"(it needs more than {limit_size} frames), return empty results",
                     xs_pad.size(1),
@@ -572,35 +315,370 @@
             xs_pad, masks = self.encoders(xs_pad, masks)
         else:
             for layer_idx, encoder_layer in enumerate(self.encoders):
                 xs_pad, masks = encoder_layer(xs_pad, masks)
 
                 if layer_idx + 1 in self.interctc_layer_idx:
                     encoder_out = xs_pad
-                    if isinstance(encoder_out, tuple):
-                        encoder_out = encoder_out[0]
 
                     # intermediate outputs are also normalized
                     if self.normalize_before:
                         encoder_out = self.after_norm(encoder_out)
 
                     intermediate_outs.append((layer_idx + 1, encoder_out))
 
                     if self.interctc_use_conditioning:
                         ctc_out = ctc.softmax(encoder_out)
+                        xs_pad = xs_pad + self.conditioning_layer(ctc_out)
 
-                        if isinstance(xs_pad, tuple):
-                            x, pos_emb = xs_pad
-                            x = x + self.conditioning_layer(ctc_out)
-                            xs_pad = (x, pos_emb)
-                        else:
-                            xs_pad = xs_pad + self.conditioning_layer(ctc_out)
-
-        if isinstance(xs_pad, tuple):
-            xs_pad = xs_pad[0]
         if self.normalize_before:
             xs_pad = self.after_norm(xs_pad)
 
         olens = masks.squeeze(1).sum(1)
         if len(intermediate_outs) > 0:
             return (xs_pad, intermediate_outs), olens, None
         return xs_pad, olens, None
+
+
+def _pre_hook(
+    state_dict,
+    prefix,
+    local_metadata,
+    strict,
+    missing_keys,
+    unexpected_keys,
+    error_msgs,
+):
+    # https://github.com/espnet/espnet/commit/21d70286c354c66c0350e65dc098d2ee236faccc#diff-bffb1396f038b317b2b64dd96e6d3563
+    rename_state_dict(prefix + "input_layer.", prefix + "embed.", state_dict)
+    # https://github.com/espnet/espnet/commit/3d422f6de8d4f03673b89e1caef698745ec749ea#diff-bffb1396f038b317b2b64dd96e6d3563
+    rename_state_dict(prefix + "norm.", prefix + "after_norm.", state_dict)
+
+
+class TransformerEncoder_s0(torch.nn.Module):
+    """Transformer encoder module.
+
+    Args:
+        idim (int): Input dimension.
+        attention_dim (int): Dimension of attention.
+        attention_heads (int): The number of heads of multi head attention.
+        conv_wshare (int): The number of kernel of convolution. Only used in
+            selfattention_layer_type == "lightconv*" or "dynamiconv*".
+        conv_kernel_length (Union[int, str]): Kernel size str of convolution
+            (e.g. 71_71_71_71_71_71). Only used in selfattention_layer_type
+            == "lightconv*" or "dynamiconv*".
+        conv_usebias (bool): Whether to use bias in convolution. Only used in
+            selfattention_layer_type == "lightconv*" or "dynamiconv*".
+        linear_units (int): The number of units of position-wise feed forward.
+        num_blocks (int): The number of decoder blocks.
+        dropout_rate (float): Dropout rate.
+        positional_dropout_rate (float): Dropout rate after adding positional encoding.
+        attention_dropout_rate (float): Dropout rate in attention.
+        input_layer (Union[str, torch.nn.Module]): Input layer type.
+        pos_enc_class (torch.nn.Module): Positional encoding module class.
+            `PositionalEncoding `or `ScaledPositionalEncoding`
+        normalize_before (bool): Whether to use layer_norm before the first block.
+        concat_after (bool): Whether to concat attention layer's input and output.
+            if True, additional linear will be applied.
+            i.e. x -> x + linear(concat(x, att(x)))
+            if False, no additional linear will be applied. i.e. x -> x + att(x)
+        positionwise_layer_type (str): "linear", "conv1d", or "conv1d-linear".
+        positionwise_conv_kernel_size (int): Kernel size of positionwise conv1d layer.
+        selfattention_layer_type (str): Encoder attention layer type.
+        padding_idx (int): Padding idx for input_layer=embed.
+        stochastic_depth_rate (float): Maximum probability to skip the encoder layer.
+        intermediate_layers (Union[List[int], None]): indices of intermediate CTC layer.
+            indices start from 1.
+            if not None, intermediate outputs are returned (which changes return type
+            signature.)
+
+    """
+
+    def __init__(
+        self,
+        idim,
+        attention_dim=256,
+        attention_heads=4,
+        conv_wshare=4,
+        conv_kernel_length="11",
+        conv_usebias=False,
+        linear_units=2048,
+        num_blocks=6,
+        dropout_rate=0.1,
+        positional_dropout_rate=0.1,
+        attention_dropout_rate=0.0,
+        input_layer="conv2d",
+        pos_enc_class=PositionalEncoding,
+        normalize_before=True,
+        concat_after=False,
+        positionwise_layer_type="linear",
+        positionwise_conv_kernel_size=1,
+        selfattention_layer_type="selfattn",
+        padding_idx=-1,
+        stochastic_depth_rate=0.0,
+        intermediate_layers=None,
+        ctc_softmax=None,
+        conditioning_layer_dim=None,
+    ):
+        """Construct an Encoder object."""
+        super(TransformerEncoder_s0, self).__init__()
+        self._register_load_state_dict_pre_hook(_pre_hook)
+
+        self.conv_subsampling_factor = 1
+        if input_layer == "linear":
+            self.embed = torch.nn.Sequential(
+                torch.nn.Linear(idim, attention_dim),
+                torch.nn.LayerNorm(attention_dim),
+                torch.nn.Dropout(dropout_rate),
+                torch.nn.ReLU(),
+                pos_enc_class(attention_dim, positional_dropout_rate),
+            )
+        elif input_layer == "conv2d":
+            self.embed = Conv2dSubsampling(idim, attention_dim, dropout_rate)
+            self.conv_subsampling_factor = 4
+        elif input_layer == "conv2d-scaled-pos-enc":
+            self.embed = Conv2dSubsampling(
+                idim,
+                attention_dim,
+                dropout_rate,
+                pos_enc_class(attention_dim, positional_dropout_rate),
+            )
+            self.conv_subsampling_factor = 4
+        elif input_layer == "conv2d6":
+            self.embed = Conv2dSubsampling6(idim, attention_dim, dropout_rate)
+            self.conv_subsampling_factor = 6
+        elif input_layer == "conv2d8":
+            self.embed = Conv2dSubsampling8(idim, attention_dim, dropout_rate)
+            self.conv_subsampling_factor = 8
+        elif input_layer == "embed":
+            self.embed = torch.nn.Sequential(
+                torch.nn.Embedding(idim, attention_dim, padding_idx=padding_idx),
+                pos_enc_class(attention_dim, positional_dropout_rate),
+            )
+        elif isinstance(input_layer, torch.nn.Module):
+            self.embed = torch.nn.Sequential(
+                input_layer,
+                pos_enc_class(attention_dim, positional_dropout_rate),
+            )
+        elif input_layer is None:
+            self.embed = torch.nn.Sequential(
+                pos_enc_class(attention_dim, positional_dropout_rate)
+            )
+        else:
+            raise ValueError("unknown input_layer: " + input_layer)
+        self.normalize_before = normalize_before
+        positionwise_layer, positionwise_layer_args = self.get_positionwise_layer(
+            positionwise_layer_type,
+            attention_dim,
+            linear_units,
+            dropout_rate,
+            positionwise_conv_kernel_size,
+        )
+        if selfattention_layer_type in [
+            "selfattn",
+            "rel_selfattn",
+            "legacy_rel_selfattn",
+        ]:
+            logging.info("encoder self-attention layer type = self-attention")
+            encoder_selfattn_layer = MultiHeadedAttention
+            encoder_selfattn_layer_args = [
+                (
+                    attention_heads,
+                    attention_dim,
+                    attention_dropout_rate,
+                )
+            ] * num_blocks
+        elif selfattention_layer_type == "lightconv":
+            logging.info("encoder self-attention layer type = lightweight convolution")
+            encoder_selfattn_layer = LightweightConvolution
+            encoder_selfattn_layer_args = [
+                (
+                    conv_wshare,
+                    attention_dim,
+                    attention_dropout_rate,
+                    int(conv_kernel_length.split("_")[lnum]),
+                    False,
+                    conv_usebias,
+                )
+                for lnum in range(num_blocks)
+            ]
+        elif selfattention_layer_type == "lightconv2d":
+            logging.info(
+                "encoder self-attention layer "
+                "type = lightweight convolution 2-dimensional"
+            )
+            encoder_selfattn_layer = LightweightConvolution2D
+            encoder_selfattn_layer_args = [
+                (
+                    conv_wshare,
+                    attention_dim,
+                    attention_dropout_rate,
+                    int(conv_kernel_length.split("_")[lnum]),
+                    False,
+                    conv_usebias,
+                )
+                for lnum in range(num_blocks)
+            ]
+        elif selfattention_layer_type == "dynamicconv":
+            logging.info("encoder self-attention layer type = dynamic convolution")
+            encoder_selfattn_layer = DynamicConvolution
+            encoder_selfattn_layer_args = [
+                (
+                    conv_wshare,
+                    attention_dim,
+                    attention_dropout_rate,
+                    int(conv_kernel_length.split("_")[lnum]),
+                    False,
+                    conv_usebias,
+                )
+                for lnum in range(num_blocks)
+            ]
+        elif selfattention_layer_type == "dynamicconv2d":
+            logging.info(
+                "encoder self-attention layer type = dynamic convolution 2-dimensional"
+            )
+            encoder_selfattn_layer = DynamicConvolution2D
+            encoder_selfattn_layer_args = [
+                (
+                    conv_wshare,
+                    attention_dim,
+                    attention_dropout_rate,
+                    int(conv_kernel_length.split("_")[lnum]),
+                    False,
+                    conv_usebias,
+                )
+                for lnum in range(num_blocks)
+            ]
+        else:
+            raise NotImplementedError(selfattention_layer_type)
+
+        self.encoders = repeat(
+            num_blocks,
+            lambda lnum: EncoderLayer(
+                attention_dim,
+                encoder_selfattn_layer(*encoder_selfattn_layer_args[lnum]),
+                positionwise_layer(*positionwise_layer_args),
+                dropout_rate,
+                normalize_before,
+                concat_after,
+                stochastic_depth_rate * float(1 + lnum) / num_blocks,
+            ),
+        )
+        if self.normalize_before:
+            self.after_norm = LayerNorm(attention_dim)
+
+        self.intermediate_layers = intermediate_layers
+        self.use_conditioning = True if ctc_softmax is not None else False
+        if self.use_conditioning:
+            self.ctc_softmax = ctc_softmax
+            self.conditioning_layer = torch.nn.Linear(
+                conditioning_layer_dim, attention_dim
+            )
+
+    def get_positionwise_layer(
+        self,
+        positionwise_layer_type="linear",
+        attention_dim=256,
+        linear_units=2048,
+        dropout_rate=0.1,
+        positionwise_conv_kernel_size=1,
+    ):
+        """Define positionwise layer."""
+        if positionwise_layer_type == "linear":
+            positionwise_layer = PositionwiseFeedForward
+            positionwise_layer_args = (attention_dim, linear_units, dropout_rate)
+        elif positionwise_layer_type == "conv1d":
+            positionwise_layer = MultiLayeredConv1d
+            positionwise_layer_args = (
+                attention_dim,
+                linear_units,
+                positionwise_conv_kernel_size,
+                dropout_rate,
+            )
+        elif positionwise_layer_type == "conv1d-linear":
+            positionwise_layer = Conv1dLinear
+            positionwise_layer_args = (
+                attention_dim,
+                linear_units,
+                positionwise_conv_kernel_size,
+                dropout_rate,
+            )
+        else:
+            raise NotImplementedError("Support only linear or conv1d.")
+        return positionwise_layer, positionwise_layer_args
+
+    def forward(self, xs, masks):
+        """Encode input sequence.
+
+        Args:
+            xs (torch.Tensor): Input tensor (#batch, time, idim).
+            masks (torch.Tensor): Mask tensor (#batch, time).
+
+        Returns:
+            torch.Tensor: Output tensor (#batch, time, attention_dim).
+            torch.Tensor: Mask tensor (#batch, time).
+
+        """
+        if isinstance(
+            self.embed,
+            (Conv2dSubsampling, Conv2dSubsampling6, Conv2dSubsampling8),
+        ):
+            xs, masks = self.embed(xs, masks)
+        else:
+            xs = self.embed(xs)
+
+        if self.intermediate_layers is None:
+            xs, masks = self.encoders(xs, masks)
+        else:
+            intermediate_outputs = []
+            for layer_idx, encoder_layer in enumerate(self.encoders):
+                xs, masks = encoder_layer(xs, masks)
+
+                if (
+                    self.intermediate_layers is not None
+                    and layer_idx + 1 in self.intermediate_layers
+                ):
+                    encoder_output = xs
+                    # intermediate branches also require normalization.
+                    if self.normalize_before:
+                        encoder_output = self.after_norm(encoder_output)
+                    intermediate_outputs.append(encoder_output)
+
+                    if self.use_conditioning:
+                        intermediate_result = self.ctc_softmax(encoder_output)
+                        xs = xs + self.conditioning_layer(intermediate_result)
+
+        if self.normalize_before:
+            xs = self.after_norm(xs)
+
+        if self.intermediate_layers is not None:
+            return xs, masks, intermediate_outputs
+        return xs, masks
+
+    def forward_one_step(self, xs, masks, cache=None):
+        """Encode input frame.
+
+        Args:
+            xs (torch.Tensor): Input tensor.
+            masks (torch.Tensor): Mask tensor.
+            cache (List[torch.Tensor]): List of cache tensors.
+
+        Returns:
+            torch.Tensor: Output tensor.
+            torch.Tensor: Mask tensor.
+            List[torch.Tensor]: List of new cache tensors.
+
+        """
+        if isinstance(self.embed, Conv2dSubsampling):
+            xs, masks = self.embed(xs, masks)
+        else:
+            xs = self.embed(xs)
+        if cache is None:
+            cache = [None for _ in range(len(self.encoders))]
+        new_cache = []
+        for c, e in zip(cache, self.encoders):
+            xs, masks = e(xs, masks, cache=c)
+            new_cache.append(xs)
+        if self.normalize_before:
+            xs = self.after_norm(xs)
+        return xs, masks, new_cache
+
```

### Comparing `funasr-0.4.1/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.4.2/funasr/models/encoder/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.4.2/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.4.2/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.4.2/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.4.2/funasr/models/encoder/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.4.2/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.4.2/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.4.2/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.4.2/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.4.2/funasr/models/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/encoder/rnn_encoder.py` & `funasr-0.4.2/funasr/models/encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/encoder/sanm_encoder.py` & `funasr-0.4.2/funasr/models/encoder/sanm_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import torch
 import torch.nn as nn
 from funasr.modules.streaming_utils.chunk_utilis import overlap_chunk
 from typeguard import check_argument_types
 import numpy as np
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.modules.attention import MultiHeadedAttention, MultiHeadedAttentionSANM, MultiHeadedAttentionSANMwithMask
-from funasr.modules.embedding import SinusoidalPositionEncoder
+from funasr.modules.embedding import SinusoidalPositionEncoder, StreamSinusoidalPositionEncoder
 from funasr.modules.layer_norm import LayerNorm
 from funasr.modules.multi_layer_conv import Conv1dLinear
 from funasr.modules.multi_layer_conv import MultiLayeredConv1d
 from funasr.modules.positionwise_feed_forward import (
     PositionwiseFeedForward,  # noqa: H301
 )
 from funasr.modules.repeat import repeat
@@ -176,14 +176,16 @@
         elif input_layer is None:
             if input_size == output_size:
                 self.embed = None
             else:
                 self.embed = torch.nn.Linear(input_size, output_size)
         elif input_layer == "pe":
             self.embed = SinusoidalPositionEncoder()
+        elif input_layer == "pe_online":
+            self.embed = StreamSinusoidalPositionEncoder()
         else:
             raise ValueError("unknown input_layer: " + input_layer)
         self.normalize_before = normalize_before
         if positionwise_layer_type == "linear":
             positionwise_layer = PositionwiseFeedForward
             positionwise_layer_args = (
                 output_size,
@@ -353,15 +355,15 @@
                       cache: dict = None,
                       ctc: CTC = None,
                       ):
         xs_pad *= self.output_size() ** 0.5
         if self.embed is None:
             xs_pad = xs_pad
         else:
-            xs_pad = self.embed.forward_chunk(xs_pad, cache)
+            xs_pad = self.embed(xs_pad, cache)
 
         encoder_outs = self.encoders0(xs_pad, None, None, None, None)
         xs_pad, masks = encoder_outs[0], encoder_outs[1]
         intermediate_outs = []
         if len(self.interctc_layer_idx) == 0:
             encoder_outs = self.encoders(xs_pad, None, None, None, None)
             xs_pad, masks = encoder_outs[0], encoder_outs[1]
```

### Comparing `funasr-0.4.1/funasr/models/frontend/default.py` & `funasr-0.4.2/funasr/models/frontend/default.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.4.2/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/frontend/fused.py` & `funasr-0.4.2/funasr/models/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/frontend/s3prl.py` & `funasr-0.4.2/funasr/models/frontend/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/frontend/wav_frontend.py` & `funasr-0.4.2/funasr/models/frontend/wav_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,31 +30,31 @@
             if line_item[0] == '<LearnRateCoef>':
                 rescale_line = line_item[3:(len(line_item) - 1)]
                 vars_list = list(rescale_line)
                 continue
     means = np.array(means_list).astype(np.float)
     vars = np.array(vars_list).astype(np.float)
     cmvn = np.array([means, vars])
-    cmvn = torch.as_tensor(cmvn)
+    cmvn = torch.as_tensor(cmvn, dype=torch.float32)
     return cmvn
 
 
 def apply_cmvn(inputs, cmvn):  # noqa
     """
     Apply CMVN with mvn data
     """
 
     device = inputs.device
     dtype = inputs.dtype
     frame, dim = inputs.shape
 
-    means = np.tile(cmvn[0:1, :dim], (frame, 1))
-    vars = np.tile(cmvn[1:2, :dim], (frame, 1))
-    inputs += torch.from_numpy(means).type(dtype).to(device)
-    inputs *= torch.from_numpy(vars).type(dtype).to(device)
+    means = cmvn[0:1, :dim]
+    vars = cmvn[1:2, :dim]
+    inputs += means.to(device)
+    inputs *= vars.to(device)
 
     return inputs.type(torch.float32)
 
 
 def apply_lfr(inputs, lfr_m, lfr_n):
     LFR_inputs = []
     T = inputs.shape[0]
```

### Comparing `funasr-0.4.1/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.4.2/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/frontend/windowing.py` & `funasr-0.4.2/funasr/models/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/pooling/statistic_pooling.py` & `funasr-0.4.2/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.4.2/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/predictor/cif.py` & `funasr-0.4.2/funasr/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/preencoder/linear.py` & `funasr-0.4.2/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/preencoder/sinc.py` & `funasr-0.4.2/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/specaug/specaug.py` & `funasr-0.4.2/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/target_delay_transformer.py` & `funasr-0.4.2/funasr/models/target_delay_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/models/vad_realtime_transformer.py` & `funasr-0.4.2/funasr/models/vad_realtime_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/add_sos_eos.py` & `funasr-0.4.2/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/attention.py` & `funasr-0.4.2/funasr/modules/attention.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """Multi-Head Attention layer definition."""
 
 import math
 
 import numpy
 import torch
 from torch import nn
-
+from typing import Optional, Tuple
 
 class MultiHeadedAttention(nn.Module):
     """Multi-Head Attention layer.
 
     Args:
         n_head (int): The number of heads.
         n_feat (int): The number of features.
@@ -737,7 +737,225 @@
 
         """
         q_h, k_h, v_h, v = self.forward_qkv(x)
         q_h = q_h * self.d_k ** (-0.5)
         scores = torch.matmul(q_h, k_h.transpose(-2, -1))
         att_outs = self.forward_attention(v_h, scores, mask, mask_att_chunk_encoder)
         return att_outs
+
+class RelPositionMultiHeadedAttentionChunk(torch.nn.Module):
+    """RelPositionMultiHeadedAttention definition.
+    Args:
+        num_heads: Number of attention heads.
+        embed_size: Embedding size.
+        dropout_rate: Dropout rate.
+    """
+
+    def __init__(
+        self,
+        num_heads: int,
+        embed_size: int,
+        dropout_rate: float = 0.0,
+        simplified_attention_score: bool = False,
+    ) -> None:
+        """Construct an MultiHeadedAttention object."""
+        super().__init__()
+
+        self.d_k = embed_size // num_heads
+        self.num_heads = num_heads
+
+        assert self.d_k * num_heads == embed_size, (
+            "embed_size (%d) must be divisible by num_heads (%d)",
+            (embed_size, num_heads),
+        )
+
+        self.linear_q = torch.nn.Linear(embed_size, embed_size)
+        self.linear_k = torch.nn.Linear(embed_size, embed_size)
+        self.linear_v = torch.nn.Linear(embed_size, embed_size)
+
+        self.linear_out = torch.nn.Linear(embed_size, embed_size)
+
+        if simplified_attention_score:
+            self.linear_pos = torch.nn.Linear(embed_size, num_heads)
+
+            self.compute_att_score = self.compute_simplified_attention_score
+        else:
+            self.linear_pos = torch.nn.Linear(embed_size, embed_size, bias=False)
+
+            self.pos_bias_u = torch.nn.Parameter(torch.Tensor(num_heads, self.d_k))
+            self.pos_bias_v = torch.nn.Parameter(torch.Tensor(num_heads, self.d_k))
+            torch.nn.init.xavier_uniform_(self.pos_bias_u)
+            torch.nn.init.xavier_uniform_(self.pos_bias_v)
+
+            self.compute_att_score = self.compute_attention_score
+
+        self.dropout = torch.nn.Dropout(p=dropout_rate)
+        self.attn = None
+
+    def rel_shift(self, x: torch.Tensor, left_context: int = 0) -> torch.Tensor:
+        """Compute relative positional encoding.
+        Args:
+            x: Input sequence. (B, H, T_1, 2 * T_1 - 1)
+            left_context: Number of frames in left context.
+        Returns:
+            x: Output sequence. (B, H, T_1, T_2)
+        """
+        batch_size, n_heads, time1, n = x.shape
+        time2 = time1 + left_context
+
+        batch_stride, n_heads_stride, time1_stride, n_stride = x.stride()
+
+        return x.as_strided(
+            (batch_size, n_heads, time1, time2),
+            (batch_stride, n_heads_stride, time1_stride - n_stride, n_stride),
+            storage_offset=(n_stride * (time1 - 1)),
+        )
+
+    def compute_simplified_attention_score(
+        self,
+        query: torch.Tensor,
+        key: torch.Tensor,
+        pos_enc: torch.Tensor,
+        left_context: int = 0,
+    ) -> torch.Tensor:
+        """Simplified attention score computation.
+        Reference: https://github.com/k2-fsa/icefall/pull/458
+        Args:
+            query: Transformed query tensor. (B, H, T_1, d_k)
+            key: Transformed key tensor. (B, H, T_2, d_k)
+            pos_enc: Positional embedding tensor. (B, 2 * T_1 - 1, size)
+            left_context: Number of frames in left context.
+        Returns:
+            : Attention score. (B, H, T_1, T_2)
+        """
+        pos_enc = self.linear_pos(pos_enc)
+
+        matrix_ac = torch.matmul(query, key.transpose(2, 3))
+
+        matrix_bd = self.rel_shift(
+            pos_enc.transpose(1, 2).unsqueeze(2).repeat(1, 1, query.size(2), 1),
+            left_context=left_context,
+        )
+
+        return (matrix_ac + matrix_bd) / math.sqrt(self.d_k)
+
+    def compute_attention_score(
+        self,
+        query: torch.Tensor,
+        key: torch.Tensor,
+        pos_enc: torch.Tensor,
+        left_context: int = 0,
+    ) -> torch.Tensor:
+        """Attention score computation.
+        Args:
+            query: Transformed query tensor. (B, H, T_1, d_k)
+            key: Transformed key tensor. (B, H, T_2, d_k)
+            pos_enc: Positional embedding tensor. (B, 2 * T_1 - 1, size)
+            left_context: Number of frames in left context.
+        Returns:
+            : Attention score. (B, H, T_1, T_2)
+        """
+        p = self.linear_pos(pos_enc).view(pos_enc.size(0), -1, self.num_heads, self.d_k)
+
+        query = query.transpose(1, 2)
+        q_with_bias_u = (query + self.pos_bias_u).transpose(1, 2)
+        q_with_bias_v = (query + self.pos_bias_v).transpose(1, 2)
+
+        matrix_ac = torch.matmul(q_with_bias_u, key.transpose(-2, -1))
+
+        matrix_bd = torch.matmul(q_with_bias_v, p.permute(0, 2, 3, 1))
+        matrix_bd = self.rel_shift(matrix_bd, left_context=left_context)
+
+        return (matrix_ac + matrix_bd) / math.sqrt(self.d_k)
+
+    def forward_qkv(
+        self, query: torch.Tensor, key: torch.Tensor, value: torch.Tensor
+    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        """Transform query, key and value.
+        Args:
+            query: Query tensor. (B, T_1, size)
+            key: Key tensor. (B, T_2, size)
+            v: Value tensor. (B, T_2, size)
+        Returns:
+            q: Transformed query tensor. (B, H, T_1, d_k)
+            k: Transformed key tensor. (B, H, T_2, d_k)
+            v: Transformed value tensor. (B, H, T_2, d_k)
+        """
+        n_batch = query.size(0)
+
+        q = (
+            self.linear_q(query)
+            .view(n_batch, -1, self.num_heads, self.d_k)
+            .transpose(1, 2)
+        )
+        k = (
+            self.linear_k(key)
+            .view(n_batch, -1, self.num_heads, self.d_k)
+            .transpose(1, 2)
+        )
+        v = (
+            self.linear_v(value)
+            .view(n_batch, -1, self.num_heads, self.d_k)
+            .transpose(1, 2)
+        )
+
+        return q, k, v
+
+    def forward_attention(
+        self,
+        value: torch.Tensor,
+        scores: torch.Tensor,
+        mask: torch.Tensor,
+        chunk_mask: Optional[torch.Tensor] = None,
+    ) -> torch.Tensor:
+        """Compute attention context vector.
+        Args:
+            value: Transformed value. (B, H, T_2, d_k)
+            scores: Attention score. (B, H, T_1, T_2)
+            mask: Source mask. (B, T_2)
+            chunk_mask: Chunk mask. (T_1, T_1)
+        Returns:
+           attn_output: Transformed value weighted by attention score. (B, T_1, H * d_k)
+        """
+        batch_size = scores.size(0)
+        mask = mask.unsqueeze(1).unsqueeze(2)
+        if chunk_mask is not None:
+            mask = chunk_mask.unsqueeze(0).unsqueeze(1) | mask
+        scores = scores.masked_fill(mask, float("-inf"))
+        self.attn = torch.softmax(scores, dim=-1).masked_fill(mask, 0.0)
+
+        attn_output = self.dropout(self.attn)
+        attn_output = torch.matmul(attn_output, value)
+
+        attn_output = self.linear_out(
+            attn_output.transpose(1, 2)
+            .contiguous()
+            .view(batch_size, -1, self.num_heads * self.d_k)
+        )
+
+        return attn_output
+
+    def forward(
+        self,
+        query: torch.Tensor,
+        key: torch.Tensor,
+        value: torch.Tensor,
+        pos_enc: torch.Tensor,
+        mask: torch.Tensor,
+        chunk_mask: Optional[torch.Tensor] = None,
+        left_context: int = 0,
+    ) -> torch.Tensor:
+        """Compute scaled dot product attention with rel. positional encoding.
+        Args:
+            query: Query tensor. (B, T_1, size)
+            key: Key tensor. (B, T_2, size)
+            value: Value tensor. (B, T_2, size)
+            pos_enc: Positional embedding tensor. (B, 2 * T_1 - 1, size)
+            mask: Source mask. (B, T_2)
+            chunk_mask: Chunk mask. (T_1, T_1)
+            left_context: Number of frames in left context.
+        Returns:
+            : Output tensor. (B, T_1, H * d_k)
+        """
+        q, k, v = self.forward_qkv(query, key, value)
+        scores = self.compute_att_score(q, k, pos_enc, left_context=left_context)
+        return self.forward_attention(v, scores, mask, chunk_mask=chunk_mask)
```

### Comparing `funasr-0.4.1/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.4.2/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.4.2/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/beam_search/beam_search.py` & `funasr-0.4.2/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/data2vec/data_utils.py` & `funasr-0.4.2/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/data2vec/ema_module.py` & `funasr-0.4.2/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.4.2/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/data2vec/quant_noise.py` & `funasr-0.4.2/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/data2vec/utils.py` & `funasr-0.4.2/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.4.2/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/dynamic_conv.py` & `funasr-0.4.2/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/dynamic_conv2d.py` & `funasr-0.4.2/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/eend_ola/encoder.py` & `funasr-0.4.2/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.4.2/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/embedding.py` & `funasr-0.4.2/funasr/modules/embedding.py`

 * *Files 11% similar despite different names*

```diff
@@ -403,24 +403,116 @@
     def forward(self, x):
         batch_size, timesteps, input_dim = x.size()
         positions = torch.arange(1, timesteps+1)[None, :]
         position_encoding = self.encode(positions, input_dim, x.dtype).to(x.device)
 
         return x + position_encoding
 
-    def forward_chunk(self, x, cache=None):
+class StreamSinusoidalPositionEncoder(torch.nn.Module):
+    '''
+
+    '''
+    def __int__(self, d_model=80, dropout_rate=0.1):
+        pass
+
+    def encode(self, positions: torch.Tensor = None, depth: int = None, dtype: torch.dtype = torch.float32):
+        batch_size = positions.size(0)
+        positions = positions.type(dtype)
+        log_timescale_increment = torch.log(torch.tensor([10000], dtype=dtype)) / (depth / 2 - 1)
+        inv_timescales = torch.exp(torch.arange(depth / 2).type(dtype) * (-log_timescale_increment))
+        inv_timescales = torch.reshape(inv_timescales, [batch_size, -1])
+        scaled_time = torch.reshape(positions, [1, -1, 1]) * torch.reshape(inv_timescales, [1, 1, -1])
+        encoding = torch.cat([torch.sin(scaled_time), torch.cos(scaled_time)], dim=2)
+        return encoding.type(dtype)
+
+    def forward(self, x, cache=None):
         start_idx = 0
         pad_left = 0
         pad_right = 0
         batch_size, timesteps, input_dim = x.size()
         if cache is not None:
             start_idx = cache["start_idx"]
             pad_left = cache["left"]
             pad_right = cache["right"]
         positions = torch.arange(1, timesteps+start_idx+1)[None, :]
         position_encoding = self.encode(positions, input_dim, x.dtype).to(x.device)
         outputs = x + position_encoding[:, start_idx: start_idx + timesteps]
-        outputs = outputs.transpose(1,2)
+        outputs = outputs.transpose(1, 2)
         outputs = F.pad(outputs, (pad_left, pad_right))
-        outputs = outputs.transpose(1,2)
+        outputs = outputs.transpose(1, 2)
         return outputs
-       
+
+class StreamingRelPositionalEncoding(torch.nn.Module):
+    """Relative positional encoding.
+    Args:
+        size: Module size.
+        max_len: Maximum input length.
+        dropout_rate: Dropout rate.
+    """
+
+    def __init__(
+        self, size: int, dropout_rate: float = 0.0, max_len: int = 5000
+    ) -> None:
+        """Construct a RelativePositionalEncoding object."""
+        super().__init__()
+
+        self.size = size
+
+        self.pe = None
+        self.dropout = torch.nn.Dropout(p=dropout_rate)
+
+        self.extend_pe(torch.tensor(0.0).expand(1, max_len))
+        self._register_load_state_dict_pre_hook(_pre_hook)
+
+    def extend_pe(self, x: torch.Tensor, left_context: int = 0) -> None:
+        """Reset positional encoding.
+        Args:
+            x: Input sequences. (B, T, ?)
+            left_context: Number of frames in left context.
+        """
+        time1 = x.size(1) + left_context
+
+        if self.pe is not None:
+            if self.pe.size(1) >= time1 * 2 - 1:
+                if self.pe.dtype != x.dtype or self.pe.device != x.device:
+                    self.pe = self.pe.to(device=x.device, dtype=x.dtype)
+                return
+
+        pe_positive = torch.zeros(time1, self.size)
+        pe_negative = torch.zeros(time1, self.size)
+
+        position = torch.arange(0, time1, dtype=torch.float32).unsqueeze(1)
+        div_term = torch.exp(
+            torch.arange(0, self.size, 2, dtype=torch.float32)
+            * -(math.log(10000.0) / self.size)
+        )
+
+        pe_positive[:, 0::2] = torch.sin(position * div_term)
+        pe_positive[:, 1::2] = torch.cos(position * div_term)
+        pe_positive = torch.flip(pe_positive, [0]).unsqueeze(0)
+
+        pe_negative[:, 0::2] = torch.sin(-1 * position * div_term)
+        pe_negative[:, 1::2] = torch.cos(-1 * position * div_term)
+        pe_negative = pe_negative[1:].unsqueeze(0)
+
+        self.pe = torch.cat([pe_positive, pe_negative], dim=1).to(
+            dtype=x.dtype, device=x.device
+        )
+
+    def forward(self, x: torch.Tensor, left_context: int = 0) -> torch.Tensor:
+        """Compute positional encoding.
+        Args:
+            x: Input sequences. (B, T, ?)
+            left_context: Number of frames in left context.
+        Returns:
+            pos_enc: Positional embedding sequences. (B, 2 * (T - 1), ?)
+        """
+        self.extend_pe(x, left_context=left_context)
+
+        time1 = x.size(1) + left_context
+
+        pos_enc = self.pe[
+            :, self.pe.size(1) // 2 - time1 + 1 : self.pe.size(1) // 2 + x.size(1)
+        ]
+        pos_enc = self.dropout(pos_enc)
+
+        return pos_enc
```

### Comparing `funasr-0.4.1/funasr/modules/frontends/beamformer.py` & `funasr-0.4.2/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.4.2/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.4.2/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/frontends/feature_transform.py` & `funasr-0.4.2/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/frontends/frontend.py` & `funasr-0.4.2/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/frontends/mask_estimator.py` & `funasr-0.4.2/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/layer_norm.py` & `funasr-0.4.2/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/lightconv.py` & `funasr-0.4.2/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/lightconv2d.py` & `funasr-0.4.2/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/mask.py` & `funasr-0.4.2/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/multi_layer_conv.py` & `funasr-0.4.2/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/positionwise_feed_forward.py` & `funasr-0.4.2/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/rnn/argument.py` & `funasr-0.4.2/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/rnn/attentions.py` & `funasr-0.4.2/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/rnn/decoders.py` & `funasr-0.4.2/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/rnn/encoders.py` & `funasr-0.4.2/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/scorers/ctc.py` & `funasr-0.4.2/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.4.2/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/scorers/length_bonus.py` & `funasr-0.4.2/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/scorers/scorer_interface.py` & `funasr-0.4.2/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.4.2/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.4.2/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/streaming_utils/utils.py` & `funasr-0.4.2/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/modules/subsampling_without_posenc.py` & `funasr-0.4.2/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/optimizers/fairseq_adam.py` & `funasr-0.4.2/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/optimizers/sgd.py` & `funasr-0.4.2/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/libtorch/demo.py` & `funasr-0.4.2/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/libtorch/demo_gpu.py` & `funasr-0.4.2/funasr/runtime/python/libtorch/demo_gpu.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.4.2/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/libtorch/setup.py` & `funasr-0.4.2/funasr/runtime/python/libtorch/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 
 
 setuptools.setup(
     name='funasr_torch',
     version='0.0.4',
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
-    author="Speech Lab, Alibaba Group, China",
+    author="Speech Lab of DAMO Academy, Alibaba Group",
     author_email="funasr@list.alibaba-inc.com",
     description="FunASR: A Fundamental End-to-End Speech Recognition Toolkit",
     license="The MIT License",
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=["librosa", "onnxruntime>=1.7.0",
                       "scipy", "numpy>=1.19.3",
                       "typeguard", "kaldi-native-fbank",
                       "PyYAML>=5.1.2", "torch-quant >= 0.4.0"],
     packages=find_packages(include=["torch_paraformer*"]),
     keywords=[
-        'funasr,paraformer, funasr_torch'
+        'funasr, paraformer, funasr_torch'
     ],
     classifiers=[
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

### Comparing `funasr-0.4.1/funasr/runtime/python/libtorch/test_rtf.py` & `funasr-0.4.2/funasr/runtime/python/libtorch/test_rtf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/demo.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/demo_gpu.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/demo_gpu.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         batch_size = input.shape[0]
         if self.input_cache is None:
             self.input_cache = np.empty((batch_size, 0), dtype=np.float32)
         input = np.concatenate((self.input_cache, input), axis=1)
         frame_num = self.compute_frame_num(input.shape[-1], self.frame_sample_length, self.frame_shift_sample_length)
         # update self.in_cache
         self.input_cache = input[:, -(input.shape[-1] - frame_num * self.frame_shift_sample_length):]
-        waveforms = np.empty(0, dtype=np.int16)
+        waveforms = np.empty(0, dtype=np.float32)
         feats_pad = np.empty(0, dtype=np.float32)
         feats_lens = np.empty(0, dtype=np.int32)
         if frame_num:
             waveforms = []
             feats = []
             feats_lens = []
             for i in range(batch_size):
@@ -233,15 +233,15 @@
                 self.fbank_fn.accept_waveform(self.opts.frame_opts.samp_freq, waveform.tolist())
                 frames = self.fbank_fn.num_frames_ready
                 mat = np.empty([frames, self.opts.mel_opts.num_bins])
                 for i in range(frames):
                     mat[i, :] = self.fbank_fn.get_frame(i)
                 feat = mat.astype(np.float32)
                 feat_len = np.array(mat.shape[0]).astype(np.int32)
-                feats.append(mat)
+                feats.append(feat)
                 feats_lens.append(feat_len)
 
             waveforms = np.stack(waveforms)
             feats_lens = np.array(feats_lens)
             feats_pad = np.array(feats)
         self.fbanks = feats_pad
         self.fbanks_lens = copy.deepcopy(feats_lens)
```

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/infer_onnx.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/infer_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     print(readme_path)
     with open(readme_path, 'r', encoding='utf-8') as f:
         readme = f.read()
     return readme
 
 
 MODULE_NAME = 'funasr_onnx'
-VERSION_NUM = '0.0.5'
+VERSION_NUM = '0.0.6'
 
 setuptools.setup(
     name=MODULE_NAME,
     version=VERSION_NUM,
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
-    author="Speech Lab, Alibaba Group, China",
+    author="Speech Lab of DAMO Academy, Alibaba Group",
     author_email="funasr@list.alibaba-inc.com",
     description="FunASR: A Fundamental End-to-End Speech Recognition Toolkit",
     license='MIT',
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=["librosa", "onnxruntime>=1.7.0",
```

### Comparing `funasr-0.4.1/funasr/runtime/python/onnxruntime/test_pipeline_online.py` & `funasr-0.4.2/funasr/runtime/python/onnxruntime/test_pipeline_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/samplers/build_batch_sampler.py` & `funasr-0.4.2/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/samplers/folded_batch_sampler.py` & `funasr-0.4.2/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/samplers/length_batch_sampler.py` & `funasr-0.4.2/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.4.2/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.4.2/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.4.2/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/schedulers/abs_scheduler.py` & `funasr-0.4.2/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/schedulers/noam_lr.py` & `funasr-0.4.2/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.4.2/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/schedulers/warmup_lr.py` & `funasr-0.4.2/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/tasks/abs_task.py` & `funasr-0.4.2/funasr/tasks/abs_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,15 +463,15 @@
             type=int,
             default=sys.maxsize,
             help="The maximum number update step to train",
         )
         parser.add_argument(
             "--batch_interval",
             type=int,
-            default=10000,
+            default=-1,
             help="The batch interval for saving model.",
         )
         group.add_argument(
             "--patience",
             type=int_or_none,
             default=None,
             help="Number of epochs to wait without improvement "
```

### Comparing `funasr-0.4.1/funasr/tasks/asr.py` & `funasr-0.4.2/funasr/tasks/asr.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,21 +34,24 @@
 )
 from funasr.models.decoder.transformer_decoder import (
     LightweightConvolutionTransformerDecoder,  # noqa: H301
 )
 from funasr.models.decoder.transformer_decoder import ParaformerDecoderSAN
 from funasr.models.decoder.transformer_decoder import TransformerDecoder
 from funasr.models.decoder.contextual_decoder import ContextualParaformerDecoder
+from funasr.models.decoder.rnnt_decoder import RNNTDecoder
+from funasr.models.joint_net.joint_network import JointNetwork
 from funasr.models.e2e_asr import ESPnetASRModel
-from funasr.models.e2e_asr_paraformer import Paraformer, ParaformerBert, BiCifParaformer, ContextualParaformer
+from funasr.models.e2e_asr_paraformer import Paraformer, ParaformerOnline, ParaformerBert, BiCifParaformer, ContextualParaformer
 from funasr.models.e2e_tp import TimestampPredictor
 from funasr.models.e2e_asr_mfcca import MFCCA
 from funasr.models.e2e_uni_asr import UniASR
+from funasr.models.e2e_asr_transducer import TransducerModel, UnifiedTransducerModel
 from funasr.models.encoder.abs_encoder import AbsEncoder
-from funasr.models.encoder.conformer_encoder import ConformerEncoder
+from funasr.models.encoder.conformer_encoder import ConformerEncoder, ConformerChunkEncoder
 from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
 from funasr.models.encoder.rnn_encoder import RNNEncoder
 from funasr.models.encoder.sanm_encoder import SANMEncoder, SANMEncoderChunkOpt
 from funasr.models.encoder.transformer_encoder import TransformerEncoder
 from funasr.models.encoder.mfcca_encoder import MFCCAEncoder
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.frontend.default import DefaultFrontend
@@ -117,14 +120,15 @@
 )
 model_choices = ClassChoices(
     "model",
     classes=dict(
         asr=ESPnetASRModel,
         uniasr=UniASR,
         paraformer=Paraformer,
+        paraformer_online=ParaformerOnline,
         paraformer_bert=ParaformerBert,
         bicif_paraformer=BiCifParaformer,
         contextual_paraformer=ContextualParaformer,
         mfcca=MFCCA,
         timestamp_prediction=TimestampPredictor,
     ),
     type_check=AbsESPnetModel,
@@ -146,14 +150,15 @@
         conformer=ConformerEncoder,
         transformer=TransformerEncoder,
         rnn=RNNEncoder,
         sanm=SANMEncoder,
         sanm_chunk_opt=SANMEncoderChunkOpt,
         data2vec_encoder=Data2VecEncoder,
         mfcca_enc=MFCCAEncoder,
+        chunk_conformer=ConformerChunkEncoder,
     ),
     type_check=AbsEncoder,
     default="rnn",
 )
 encoder_choices2 = ClassChoices(
     "encoder2",
     classes=dict(
@@ -203,14 +208,24 @@
         rnn=RNNDecoder,
         fsmn_scama_opt=FsmnDecoderSCAMAOpt,
         paraformer_decoder_sanm=ParaformerSANMDecoder,
     ),
     type_check=AbsDecoder,
     default="rnn",
 )
+
+rnnt_decoder_choices = ClassChoices(
+    "rnnt_decoder",
+    classes=dict(
+        rnnt=RNNTDecoder,
+    ),
+    type_check=RNNTDecoder,
+    default="rnnt",
+)
+
 predictor_choices = ClassChoices(
     name="predictor",
     classes=dict(
         cif_predictor=CifPredictor,
         ctc_predictor=None,
         cif_predictor_v2=CifPredictorV2,
         cif_predictor_v3=CifPredictorV3,
@@ -1327,7 +1342,382 @@
 
     @classmethod
     def required_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ("speech", "text")
         return retval
+
+
+class ASRTransducerTask(AbsTask):
+    """ASR Transducer Task definition."""
+
+    num_optimizers: int = 1
+
+    class_choices_list = [
+        frontend_choices,
+        specaug_choices,
+        normalize_choices,
+        encoder_choices,
+        rnnt_decoder_choices,
+    ]
+
+    trainer = Trainer
+
+    @classmethod
+    def add_task_arguments(cls, parser: argparse.ArgumentParser):
+        """Add Transducer task arguments.
+        Args:
+            cls: ASRTransducerTask object.
+            parser: Transducer arguments parser.
+        """
+        group = parser.add_argument_group(description="Task related.")
+
+        # required = parser.get_default("required")
+        # required += ["token_list"]
+
+        group.add_argument(
+            "--token_list",
+            type=str_or_none,
+            default=None,
+            help="Integer-string mapper for tokens.",
+        )
+        group.add_argument(
+            "--split_with_space",
+            type=str2bool,
+            default=True,
+            help="whether to split text using <space>",
+        )
+        group.add_argument(
+            "--input_size",
+            type=int_or_none,
+            default=None,
+            help="The number of dimensions for input features.",
+        )
+        group.add_argument(
+            "--init",
+            type=str_or_none,
+            default=None,
+            help="Type of model initialization to use.",
+        )
+        group.add_argument(
+            "--model_conf",
+            action=NestedDictAction,
+            default=get_default_kwargs(TransducerModel),
+            help="The keyword arguments for the model class.",
+        )
+        # group.add_argument(
+        #     "--encoder_conf",
+        #     action=NestedDictAction,
+        #     default={},
+        #     help="The keyword arguments for the encoder class.",
+        # )
+        group.add_argument(
+            "--joint_network_conf",
+            action=NestedDictAction,
+            default={},
+            help="The keyword arguments for the joint network class.",
+        )
+        group = parser.add_argument_group(description="Preprocess related.")
+        group.add_argument(
+            "--use_preprocessor",
+            type=str2bool,
+            default=True,
+            help="Whether to apply preprocessing to input data.",
+        )
+        group.add_argument(
+            "--token_type",
+            type=str,
+            default="bpe",
+            choices=["bpe", "char", "word", "phn"],
+            help="The type of tokens to use during tokenization.",
+        )
+        group.add_argument(
+            "--bpemodel",
+            type=str_or_none,
+            default=None,
+            help="The path of the sentencepiece model.",
+        )
+        parser.add_argument(
+            "--non_linguistic_symbols",
+            type=str_or_none,
+            help="The 'non_linguistic_symbols' file path.",
+        )
+        parser.add_argument(
+            "--cleaner",
+            type=str_or_none,
+            choices=[None, "tacotron", "jaconv", "vietnamese"],
+            default=None,
+            help="Text cleaner to use.",
+        )
+        parser.add_argument(
+            "--g2p",
+            type=str_or_none,
+            choices=g2p_choices,
+            default=None,
+            help="g2p method to use if --token_type=phn.",
+        )
+        parser.add_argument(
+            "--speech_volume_normalize",
+            type=float_or_none,
+            default=None,
+            help="Normalization value for maximum amplitude scaling.",
+        )
+        parser.add_argument(
+            "--rir_scp",
+            type=str_or_none,
+            default=None,
+            help="The RIR SCP file path.",
+        )
+        parser.add_argument(
+            "--rir_apply_prob",
+            type=float,
+            default=1.0,
+            help="The probability of the applied RIR convolution.",
+        )
+        parser.add_argument(
+            "--noise_scp",
+            type=str_or_none,
+            default=None,
+            help="The path of noise SCP file.",
+        )
+        parser.add_argument(
+            "--noise_apply_prob",
+            type=float,
+            default=1.0,
+            help="The probability of the applied noise addition.",
+        )
+        parser.add_argument(
+            "--noise_db_range",
+            type=str,
+            default="13_15",
+            help="The range of the noise decibel level.",
+        )
+        for class_choices in cls.class_choices_list:
+            # Append --<name> and --<name>_conf.
+            # e.g. --decoder and --decoder_conf
+            class_choices.add_arguments(group)
+
+    @classmethod
+    def build_collate_fn(
+        cls, args: argparse.Namespace, train: bool
+    ) -> Callable[
+        [Collection[Tuple[str, Dict[str, np.ndarray]]]],
+        Tuple[List[str], Dict[str, torch.Tensor]],
+    ]:
+        """Build collate function.
+        Args:
+            cls: ASRTransducerTask object.
+            args: Task arguments.
+            train: Training mode.
+        Return:
+            : Callable collate function.
+        """
+        assert check_argument_types()
+
+        return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
+
+    @classmethod
+    def build_preprocess_fn(
+        cls, args: argparse.Namespace, train: bool
+    ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
+        """Build pre-processing function.
+        Args:
+            cls: ASRTransducerTask object.
+            args: Task arguments.
+            train: Training mode.
+        Return:
+            : Callable pre-processing function.
+        """
+        assert check_argument_types()
+
+        if args.use_preprocessor:
+            retval = CommonPreprocessor(
+                train=train,
+                token_type=args.token_type,
+                token_list=args.token_list,
+                bpemodel=args.bpemodel,
+                non_linguistic_symbols=args.non_linguistic_symbols,
+                text_cleaner=args.cleaner,
+                g2p_type=args.g2p,
+                split_with_space=args.split_with_space if hasattr(args, "split_with_space") else False,
+                rir_scp=args.rir_scp if hasattr(args, "rir_scp") else None,
+                rir_apply_prob=args.rir_apply_prob
+                if hasattr(args, "rir_apply_prob")
+                else 1.0,
+                noise_scp=args.noise_scp if hasattr(args, "noise_scp") else None,
+                noise_apply_prob=args.noise_apply_prob
+                if hasattr(args, "noise_apply_prob")
+                else 1.0,
+                noise_db_range=args.noise_db_range
+                if hasattr(args, "noise_db_range")
+                else "13_15",
+                speech_volume_normalize=args.speech_volume_normalize
+                if hasattr(args, "rir_scp")
+                else None,
+            )
+        else:
+            retval = None
+
+        assert check_return_type(retval)
+        return retval
+
+    @classmethod
+    def required_data_names(
+        cls, train: bool = True, inference: bool = False
+    ) -> Tuple[str, ...]:
+        """Required data depending on task mode.
+        Args:
+            cls: ASRTransducerTask object.
+            train: Training mode.
+            inference: Inference mode.
+        Return:
+            retval: Required task data.
+        """
+        if not inference:
+            retval = ("speech", "text")
+        else:
+            retval = ("speech",)
+
+        return retval
+
+    @classmethod
+    def optional_data_names(
+        cls, train: bool = True, inference: bool = False
+    ) -> Tuple[str, ...]:
+        """Optional data depending on task mode.
+        Args:
+            cls: ASRTransducerTask object.
+            train: Training mode.
+            inference: Inference mode.
+        Return:
+            retval: Optional task data.
+        """
+        retval = ()
+        assert check_return_type(retval)
+
+        return retval
+
+    @classmethod
+    def build_model(cls, args: argparse.Namespace) -> TransducerModel:
+        """Required data depending on task mode.
+        Args:
+            cls: ASRTransducerTask object.
+            args: Task arguments.
+        Return:
+            model: ASR Transducer model.
+        """
+        assert check_argument_types()
+
+        if isinstance(args.token_list, str):
+            with open(args.token_list, encoding="utf-8") as f:
+                token_list = [line.rstrip() for line in f]
+
+            # Overwriting token_list to keep it as "portable".
+            args.token_list = list(token_list)
+        elif isinstance(args.token_list, (tuple, list)):
+            token_list = list(args.token_list)
+        else:
+            raise RuntimeError("token_list must be str or list")
+        vocab_size = len(token_list)
+        logging.info(f"Vocabulary size: {vocab_size }")
+
+        # 1. frontend
+        if args.input_size is None:
+            # Extract features in the model
+            frontend_class = frontend_choices.get_class(args.frontend)
+            frontend = frontend_class(**args.frontend_conf)
+            input_size = frontend.output_size()
+        else:
+            # Give features from data-loader
+            frontend = None
+            input_size = args.input_size
+
+        # 2. Data augmentation for spectrogram
+        if args.specaug is not None:
+            specaug_class = specaug_choices.get_class(args.specaug)
+            specaug = specaug_class(**args.specaug_conf)
+        else:
+            specaug = None
+
+        # 3. Normalization layer
+        if args.normalize is not None:
+            normalize_class = normalize_choices.get_class(args.normalize)
+            normalize = normalize_class(**args.normalize_conf)
+        else:
+            normalize = None
+
+        # 4. Encoder
+
+        if getattr(args, "encoder", None) is not None:
+            encoder_class = encoder_choices.get_class(args.encoder)
+            encoder = encoder_class(input_size, **args.encoder_conf)
+        else:
+            encoder = Encoder(input_size, **args.encoder_conf)
+        encoder_output_size = encoder.output_size()
+
+        # 5. Decoder
+        rnnt_decoder_class = rnnt_decoder_choices.get_class(args.rnnt_decoder)
+        decoder = rnnt_decoder_class(
+            vocab_size,
+            **args.rnnt_decoder_conf,
+        )
+        decoder_output_size = decoder.output_size
+
+        if getattr(args, "decoder", None) is not None:
+            att_decoder_class = decoder_choices.get_class(args.att_decoder)
+
+            att_decoder = att_decoder_class(
+                vocab_size=vocab_size,
+                encoder_output_size=encoder_output_size,
+                **args.decoder_conf,
+            )
+        else:
+            att_decoder = None
+        # 6. Joint Network
+        joint_network = JointNetwork(
+            vocab_size,
+            encoder_output_size,
+            decoder_output_size,
+            **args.joint_network_conf,
+        )
+
+        # 7. Build model
+
+        if encoder.unified_model_training:
+            model = UnifiedTransducerModel(
+                vocab_size=vocab_size,
+                token_list=token_list,
+                frontend=frontend,
+                specaug=specaug,
+                normalize=normalize,
+                encoder=encoder,
+                decoder=decoder,
+                att_decoder=att_decoder,
+                joint_network=joint_network,
+                **args.model_conf,
+            )
+
+        else:
+            model = TransducerModel(
+                vocab_size=vocab_size,
+                token_list=token_list,
+                frontend=frontend,
+                specaug=specaug,
+                normalize=normalize,
+                encoder=encoder,
+                decoder=decoder,
+                att_decoder=att_decoder,
+                joint_network=joint_network,
+                **args.model_conf,
+            )
+
+        # 8. Initialize model
+        if args.init is not None:
+            raise NotImplementedError(
+                "Currently not supported.",
+                "Initialization part will be reworked in a short future.",
+            )
+
+        #assert check_return_type(model)
+
+        return model
```

### Comparing `funasr-0.4.1/funasr/tasks/data2vec.py` & `funasr-0.4.2/funasr/tasks/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/tasks/diar.py` & `funasr-0.4.2/funasr/tasks/sv.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 """
 Author: Speech Lab, Alibaba Group, China
-SOND: Speaker Overlap-aware Neural Diarization for Multi-party Meeting Analysis
-https://arxiv.org/abs/2211.10243
-TOLD: A Novel Two-Stage Overlap-Aware Framework for Speaker Diarization
-https://arxiv.org/abs/2303.05397
 """
 
 import argparse
 import logging
 import os
 from pathlib import Path
 from typing import Callable
@@ -24,70 +20,64 @@
 from typeguard import check_argument_types
 from typeguard import check_return_type
 
 from funasr.datasets.collate_fn import CommonCollateFn
 from funasr.datasets.preprocessor import CommonPreprocessor
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.layers.global_mvn import GlobalMVN
-from funasr.layers.label_aggregation import LabelAggregate
 from funasr.layers.utterance_mvn import UtteranceMVN
-from funasr.models.e2e_diar_sond import DiarSondModel
-from funasr.models.e2e_diar_eend_ola import DiarEENDOLAModel
+from funasr.models.e2e_asr import ESPnetASRModel
+from funasr.models.decoder.abs_decoder import AbsDecoder
 from funasr.models.encoder.abs_encoder import AbsEncoder
-from funasr.models.encoder.conformer_encoder import ConformerEncoder
-from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
-from funasr.models.encoder.ecapa_tdnn_encoder import ECAPA_TDNN
-from funasr.models.encoder.opennmt_encoders.ci_scorers import DotScorer, CosScorer
-from funasr.models.encoder.opennmt_encoders.conv_encoder import ConvEncoder
-from funasr.models.encoder.opennmt_encoders.fsmn_encoder import FsmnEncoder
-from funasr.models.encoder.opennmt_encoders.self_attention_encoder import SelfAttentionEncoder
-from funasr.models.encoder.resnet34_encoder import ResNet34Diar, ResNet34SpL2RegDiar
 from funasr.models.encoder.rnn_encoder import RNNEncoder
-from funasr.models.encoder.sanm_encoder import SANMEncoder, SANMEncoderChunkOpt
-from funasr.models.encoder.transformer_encoder import TransformerEncoder
+from funasr.models.encoder.resnet34_encoder import ResNet34, ResNet34_SP_L2Reg
+from funasr.models.pooling.statistic_pooling import StatisticPooling
+from funasr.models.decoder.sv_decoder import DenseDecoder
+from funasr.models.e2e_sv import ESPnetSVModel
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.frontend.default import DefaultFrontend
 from funasr.models.frontend.fused import FusedFrontends
 from funasr.models.frontend.s3prl import S3prlFrontend
-from funasr.models.frontend.wav_frontend import WavFrontend
-from funasr.models.frontend.wav_frontend import WavFrontendMel23
 from funasr.models.frontend.windowing import SlidingWindow
+from funasr.models.postencoder.abs_postencoder import AbsPostEncoder
+from funasr.models.postencoder.hugging_face_transformers_postencoder import (
+    HuggingFaceTransformersPostEncoder,  # noqa: H301
+)
+from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
+from funasr.models.preencoder.linear import LinearProjection
+from funasr.models.preencoder.sinc import LightweightSincConvs
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.models.specaug.specaug import SpecAug
-from funasr.models.specaug.specaug import SpecAugLFR
-from funasr.modules.eend_ola.encoder import EENDOLATransformerEncoder
-from funasr.modules.eend_ola.encoder_decoder_attractor import EncoderDecoderAttractor
 from funasr.tasks.abs_task import AbsTask
 from funasr.torch_utils.initialize import initialize
 from funasr.train.abs_espnet_model import AbsESPnetModel
 from funasr.train.class_choices import ClassChoices
 from funasr.train.trainer import Trainer
 from funasr.utils.types import float_or_none
 from funasr.utils.types import int_or_none
 from funasr.utils.types import str2bool
 from funasr.utils.types import str_or_none
+from funasr.models.frontend.wav_frontend import WavFrontend
 
 frontend_choices = ClassChoices(
     name="frontend",
     classes=dict(
         default=DefaultFrontend,
         sliding_window=SlidingWindow,
         s3prl=S3prlFrontend,
         fused=FusedFrontends,
         wav_frontend=WavFrontend,
-        wav_frontend_mel23=WavFrontendMel23,
     ),
     type_check=AbsFrontend,
     default="default",
 )
 specaug_choices = ClassChoices(
     name="specaug",
     classes=dict(
         specaug=SpecAug,
-        specaug_lfr=SpecAugLFR,
     ),
     type_check=AbsSpecAug,
     default=None,
     optional=True,
 )
 normalize_choices = ClassChoices(
     "normalize",
@@ -95,167 +85,112 @@
         global_mvn=GlobalMVN,
         utterance_mvn=UtteranceMVN,
     ),
     type_check=AbsNormalize,
     default=None,
     optional=True,
 )
-label_aggregator_choices = ClassChoices(
-    "label_aggregator",
-    classes=dict(
-        label_aggregator=LabelAggregate
-    ),
-    type_check=torch.nn.Module,
-    default=None,
-    optional=True,
-)
 model_choices = ClassChoices(
     "model",
     classes=dict(
-        sond=DiarSondModel,
-        eend_ola=DiarEENDOLAModel,
+        espnet=ESPnetSVModel,
     ),
     type_check=AbsESPnetModel,
-    default="sond",
+    default="espnet",
 )
-encoder_choices = ClassChoices(
-    "encoder",
+preencoder_choices = ClassChoices(
+    name="preencoder",
     classes=dict(
-        conformer=ConformerEncoder,
-        transformer=TransformerEncoder,
-        rnn=RNNEncoder,
-        sanm=SANMEncoder,
-        san=SelfAttentionEncoder,
-        fsmn=FsmnEncoder,
-        conv=ConvEncoder,
-        resnet34=ResNet34Diar,
-        resnet34_sp_l2reg=ResNet34SpL2RegDiar,
-        sanm_chunk_opt=SANMEncoderChunkOpt,
-        data2vec_encoder=Data2VecEncoder,
-        ecapa_tdnn=ECAPA_TDNN,
-        eend_ola_transformer=EENDOLATransformerEncoder,
+        sinc=LightweightSincConvs,
+        linear=LinearProjection,
     ),
-    type_check=torch.nn.Module,
-    default="resnet34",
+    type_check=AbsPreEncoder,
+    default=None,
+    optional=True,
 )
-speaker_encoder_choices = ClassChoices(
-    "speaker_encoder",
+encoder_choices = ClassChoices(
+    "encoder",
     classes=dict(
-        conformer=ConformerEncoder,
-        transformer=TransformerEncoder,
+        resnet34=ResNet34,
+        resnet34_sp_l2reg=ResNet34_SP_L2Reg,
         rnn=RNNEncoder,
-        sanm=SANMEncoder,
-        san=SelfAttentionEncoder,
-        fsmn=FsmnEncoder,
-        conv=ConvEncoder,
-        sanm_chunk_opt=SANMEncoderChunkOpt,
-        data2vec_encoder=Data2VecEncoder,
     ),
     type_check=AbsEncoder,
-    default=None,
-    optional=True
+    default="resnet34",
 )
-cd_scorer_choices = ClassChoices(
-    "cd_scorer",
+postencoder_choices = ClassChoices(
+    name="postencoder",
     classes=dict(
-        san=SelfAttentionEncoder,
+        hugging_face_transformers=HuggingFaceTransformersPostEncoder,
     ),
-    type_check=AbsEncoder,
+    type_check=AbsPostEncoder,
     default=None,
     optional=True,
 )
-ci_scorer_choices = ClassChoices(
-    "ci_scorer",
+pooling_choices = ClassChoices(
+    name="pooling_type",
     classes=dict(
-        dot=DotScorer,
-        cosine=CosScorer,
-        conv=ConvEncoder,
+        statistic=StatisticPooling,
     ),
     type_check=torch.nn.Module,
-    default=None,
-    optional=True,
+    default="statistic",
 )
-# decoder is used for output (e.g. post_net in SOND)
 decoder_choices = ClassChoices(
     "decoder",
     classes=dict(
-        rnn=RNNEncoder,
-        fsmn=FsmnEncoder,
-    ),
-    type_check=torch.nn.Module,
-    default="fsmn",
-)
-# encoder_decoder_attractor is used for EEND-OLA
-encoder_decoder_attractor_choices = ClassChoices(
-    "encoder_decoder_attractor",
-    classes=dict(
-        eda=EncoderDecoderAttractor,
+        dense=DenseDecoder,
     ),
-    type_check=torch.nn.Module,
-    default="eda",
+    type_check=AbsDecoder,
+    default="dense",
 )
 
 
-class DiarTask(AbsTask):
-    # If you need more than 1 optimizer, change this value
+class SVTask(AbsTask):
+    # If you need more than one optimizers, change this value
     num_optimizers: int = 1
 
     # Add variable objects configurations
     class_choices_list = [
         # --frontend and --frontend_conf
         frontend_choices,
         # --specaug and --specaug_conf
         specaug_choices,
         # --normalize and --normalize_conf
         normalize_choices,
-        # --label_aggregator and --label_aggregator_conf
-        label_aggregator_choices,
         # --model and --model_conf
         model_choices,
+        # --preencoder and --preencoder_conf
+        preencoder_choices,
         # --encoder and --encoder_conf
         encoder_choices,
-        # --speaker_encoder and --speaker_encoder_conf
-        speaker_encoder_choices,
-        # --cd_scorer and cd_scorer_conf
-        cd_scorer_choices,
-        # --ci_scorer and ci_scorer_conf
-        ci_scorer_choices,
+        # --postencoder and --postencoder_conf
+        postencoder_choices,
+        # --pooling and --pooling_conf
+        pooling_choices,
         # --decoder and --decoder_conf
         decoder_choices,
     ]
 
     # If you need to modify train() or eval() procedures, change Trainer class here
     trainer = Trainer
 
     @classmethod
     def add_task_arguments(cls, parser: argparse.ArgumentParser):
         group = parser.add_argument_group(description="Task related")
 
         # NOTE(kamo): add_arguments(..., required=True) can't be used
         # to provide --print_config mode. Instead of it, do as
-        # required = parser.get_default("required")
-        # required += ["token_list"]
+        required = parser.get_default("required")
+        required += ["token_list"]
 
         group.add_argument(
             "--token_list",
             type=str_or_none,
             default=None,
-            help="A text mapping int-id to token",
-        )
-        group.add_argument(
-            "--split_with_space",
-            type=str2bool,
-            default=True,
-            help="whether to split text using <space>",
-        )
-        group.add_argument(
-            "--seg_dict_file",
-            type=str,
-            default=None,
-            help="seg_dict_file for text processing",
+            help="A text mapping int-id to speaker name",
         )
         group.add_argument(
             "--init",
             type=lambda x: str_or_none(x.lower()),
             default=None,
             help="The initialization method",
             choices=[
@@ -278,20 +213,20 @@
         group = parser.add_argument_group(description="Preprocess related")
         group.add_argument(
             "--use_preprocessor",
             type=str2bool,
             default=True,
             help="Apply preprocessing to data or not",
         )
-        group.add_argument(
-            "--token_type",
-            type=str,
-            default="char",
-            choices=["char"],
-            help="The text will be tokenized in the specified level token",
+        parser.add_argument(
+            "--cleaner",
+            type=str_or_none,
+            choices=[None, "tacotron", "jaconv", "vietnamese"],
+            default=None,
+            help="Apply text cleaning",
         )
         parser.add_argument(
             "--speech_volume_normalize",
             type=float_or_none,
             default=None,
             help="Scale the maximum amplitude to the given value.",
         )
@@ -304,20 +239,14 @@
         parser.add_argument(
             "--rir_apply_prob",
             type=float,
             default=1.0,
             help="THe probability for applying RIR convolution.",
         )
         parser.add_argument(
-            "--cmvn_file",
-            type=str_or_none,
-            default=None,
-            help="The file path of noise scp file.",
-        )
-        parser.add_argument(
             "--noise_scp",
             type=str_or_none,
             default=None,
             help="The file path of noise scp file.",
         )
         parser.add_argument(
             "--noise_apply_prob",
@@ -352,22 +281,20 @@
     def build_preprocess_fn(
             cls, args: argparse.Namespace, train: bool
     ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
         assert check_argument_types()
         if args.use_preprocessor:
             retval = CommonPreprocessor(
                 train=train,
-                token_type=args.token_type,
-                token_list=args.token_list,
+                token_type=None,
+                token_list=None,
                 bpemodel=None,
                 non_linguistic_symbols=None,
-                text_cleaner=None,
+                text_cleaner=args.cleaner,
                 g2p_type=None,
-                split_with_space=args.split_with_space if hasattr(args, "split_with_space") else False,
-                seg_dict_file=args.seg_dict_file if hasattr(args, "seg_dict_file") else None,
                 # NOTE(kamo): Check attribute existence for backward compatibility
                 rir_scp=args.rir_scp if hasattr(args, "rir_scp") else None,
                 rir_apply_prob=args.rir_apply_prob
                 if hasattr(args, "rir_apply_prob")
                 else 1.0,
                 noise_scp=args.noise_scp if hasattr(args, "noise_scp") else None,
                 noise_apply_prob=args.noise_apply_prob
@@ -386,52 +313,51 @@
         return retval
 
     @classmethod
     def required_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         if not inference:
-            retval = ("speech", "profile", "binary_labels")
+            retval = ("speech", "text")
         else:
             # Recognition mode
-            retval = ("speech", "profile")
+            retval = ("speech",)
         return retval
 
     @classmethod
     def optional_data_names(
             cls, train: bool = True, inference: bool = False
     ) -> Tuple[str, ...]:
         retval = ()
+        if inference:
+            retval = ("ref_speech",)
         assert check_return_type(retval)
         return retval
 
     @classmethod
-    def build_model(cls, args: argparse.Namespace):
+    def build_model(cls, args: argparse.Namespace) -> ESPnetSVModel:
         assert check_argument_types()
         if isinstance(args.token_list, str):
             with open(args.token_list, encoding="utf-8") as f:
                 token_list = [line.rstrip() for line in f]
 
             # Overwriting token_list to keep it as "portable".
             args.token_list = list(token_list)
         elif isinstance(args.token_list, (tuple, list)):
             token_list = list(args.token_list)
         else:
             raise RuntimeError("token_list must be str or list")
         vocab_size = len(token_list)
-        logging.info(f"Vocabulary size: {vocab_size}")
+        logging.info(f"Speaker number: {vocab_size}")
 
         # 1. frontend
         if args.input_size is None:
             # Extract features in the model
             frontend_class = frontend_choices.get_class(args.frontend)
-            if args.frontend == 'wav_frontend':
-                frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
-            else:
-                frontend = frontend_class(**args.frontend_conf)
+            frontend = frontend_class(**args.frontend_conf)
             input_size = frontend.output_size()
         else:
             # Give features from data-loader
             args.frontend = None
             args.frontend_conf = {}
             frontend = None
             input_size = args.input_size
@@ -446,80 +372,98 @@
         # 3. Normalization layer
         if args.normalize is not None:
             normalize_class = normalize_choices.get_class(args.normalize)
             normalize = normalize_class(**args.normalize_conf)
         else:
             normalize = None
 
-        # 4. Encoder
+        # 4. Pre-encoder input block
+        # NOTE(kan-bayashi): Use getattr to keep the compatibility
+        if getattr(args, "preencoder", None) is not None:
+            preencoder_class = preencoder_choices.get_class(args.preencoder)
+            preencoder = preencoder_class(**args.preencoder_conf)
+            input_size = preencoder.output_size()
+        else:
+            preencoder = None
+
+        # 5. Encoder
         encoder_class = encoder_choices.get_class(args.encoder)
         encoder = encoder_class(input_size=input_size, **args.encoder_conf)
 
-        # 5. speaker encoder
-        if getattr(args, "speaker_encoder", None) is not None:
-            speaker_encoder_class = speaker_encoder_choices.get_class(args.speaker_encoder)
-            speaker_encoder = speaker_encoder_class(**args.speaker_encoder_conf)
-        else:
-            speaker_encoder = None
-
-        # 6. CI & CD scorer
-        if getattr(args, "ci_scorer", None) is not None:
-            ci_scorer_class = ci_scorer_choices.get_class(args.ci_scorer)
-            ci_scorer = ci_scorer_class(**args.ci_scorer_conf)
+        # 6. Post-encoder block
+        # NOTE(kan-bayashi): Use getattr to keep the compatibility
+        encoder_output_size = encoder.output_size()
+        if getattr(args, "postencoder", None) is not None:
+            postencoder_class = postencoder_choices.get_class(args.postencoder)
+            postencoder = postencoder_class(
+                input_size=encoder_output_size, **args.postencoder_conf
+            )
+            encoder_output_size = postencoder.output_size()
         else:
-            ci_scorer = None
+            postencoder = None
 
-        if getattr(args, "cd_scorer", None) is not None:
-            cd_scorer_class = cd_scorer_choices.get_class(args.cd_scorer)
-            cd_scorer = cd_scorer_class(**args.cd_scorer_conf)
-        else:
-            cd_scorer = None
+        # 7. Pooling layer
+        pooling_class = pooling_choices.get_class(args.pooling_type)
+        pooling_dim = (2, 3)
+        eps = 1e-12
+        if hasattr(args, "pooling_type_conf"):
+            if "pooling_dim" in args.pooling_type_conf:
+                pooling_dim = args.pooling_type_conf["pooling_dim"]
+            if "eps" in args.pooling_type_conf:
+                eps = args.pooling_type_conf["eps"]
+        pooling_layer = pooling_class(
+            pooling_dim=pooling_dim,
+            eps=eps,
+        )
+        if args.pooling_type == "statistic":
+            encoder_output_size *= 2
 
-        # 7. Decoder
+        # 8. Decoder
         decoder_class = decoder_choices.get_class(args.decoder)
-        decoder = decoder_class(**args.decoder_conf)
-
-        if getattr(args, "label_aggregator", None) is not None:
-            label_aggregator_class = label_aggregator_choices.get_class(args.label_aggregator)
-            label_aggregator = label_aggregator_class(**args.label_aggregator_conf)
-        else:
-            label_aggregator = None
+        decoder = decoder_class(
+            vocab_size=vocab_size,
+            encoder_output_size=encoder_output_size,
+            **args.decoder_conf,
+        )
 
-        # 9. Build model
-        model_class = model_choices.get_class(args.model)
+        # 7. Build model
+        try:
+            model_class = model_choices.get_class(args.model)
+        except AttributeError:
+            model_class = model_choices.get_class("espnet")
         model = model_class(
             vocab_size=vocab_size,
+            token_list=token_list,
             frontend=frontend,
             specaug=specaug,
             normalize=normalize,
-            label_aggregator=label_aggregator,
+            preencoder=preencoder,
             encoder=encoder,
-            speaker_encoder=speaker_encoder,
-            ci_scorer=ci_scorer,
-            cd_scorer=cd_scorer,
+            postencoder=postencoder,
+            pooling_layer=pooling_layer,
             decoder=decoder,
-            token_list=token_list,
             **args.model_conf,
         )
 
-        # 10. Initialize
+        # FIXME(kamo): Should be done in model?
+        # 8. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
         assert check_return_type(model)
         return model
 
     # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
     @classmethod
     def build_model_from_file(
             cls,
             config_file: Union[Path, str] = None,
             model_file: Union[Path, str] = None,
             cmvn_file: Union[Path, str] = None,
-            device: Union[str, torch.device] = "cpu",
+            device: str = "cpu",
     ):
         """Build model from the files.
 
         This method is used for inference or fine-tuning.
 
         Args:
             config_file: The yaml file saved when training.
@@ -566,353 +510,36 @@
                     logging.info("model_file is load from pth: {}".format(model_name_pth))
                     model_dict = torch.load(model_name_pth, map_location=device)
                 else:
                     model_dict = cls.convert_tf2torch(model, model_file)
                 model.load_state_dict(model_dict)
             else:
                 model_dict = torch.load(model_file, map_location=device)
-        model_dict = cls.fileter_model_dict(model_dict, model.state_dict())
         model.load_state_dict(model_dict)
         if model_name_pth is not None and not os.path.exists(model_name_pth):
             torch.save(model_dict, model_name_pth)
             logging.info("model_file is saved to pth: {}".format(model_name_pth))
 
         return model, args
 
     @classmethod
-    def fileter_model_dict(cls, src_dict: dict, dest_dict: dict):
-        from collections import OrderedDict
-        new_dict = OrderedDict()
-        for key, value in src_dict.items():
-            if key in dest_dict:
-                new_dict[key] = value
-            else:
-                logging.info("{} is no longer needed in this model.".format(key))
-        for key, value in dest_dict.items():
-            if key not in new_dict:
-                logging.warning("{} is missed in checkpoint.".format(key))
-        return new_dict
-
-    @classmethod
     def convert_tf2torch(
             cls,
             model,
             ckpt,
     ):
         logging.info("start convert tf model to torch model")
         from funasr.modules.streaming_utils.load_fr_tf import load_tf_dict
         var_dict_tf = load_tf_dict(ckpt)
         var_dict_torch = model.state_dict()
         var_dict_torch_update = dict()
         # speech encoder
-        if model.encoder is not None:
-            var_dict_torch_update_local = model.encoder.convert_tf2torch(var_dict_tf, var_dict_torch)
-            var_dict_torch_update.update(var_dict_torch_update_local)
-        # speaker encoder
-        if model.speaker_encoder is not None:
-            var_dict_torch_update_local = model.speaker_encoder.convert_tf2torch(var_dict_tf, var_dict_torch)
-            var_dict_torch_update.update(var_dict_torch_update_local)
-        # cd scorer
-        if model.cd_scorer is not None:
-            var_dict_torch_update_local = model.cd_scorer.convert_tf2torch(var_dict_tf, var_dict_torch)
-            var_dict_torch_update.update(var_dict_torch_update_local)
-        # ci scorer
-        if model.ci_scorer is not None:
-            var_dict_torch_update_local = model.ci_scorer.convert_tf2torch(var_dict_tf, var_dict_torch)
-            var_dict_torch_update.update(var_dict_torch_update_local)
+        var_dict_torch_update_local = model.encoder.convert_tf2torch(var_dict_tf, var_dict_torch)
+        var_dict_torch_update.update(var_dict_torch_update_local)
+        # pooling layer
+        var_dict_torch_update_local = model.pooling_layer.convert_tf2torch(var_dict_tf, var_dict_torch)
+        var_dict_torch_update.update(var_dict_torch_update_local)
         # decoder
-        if model.decoder is not None:
-            var_dict_torch_update_local = model.decoder.convert_tf2torch(var_dict_tf, var_dict_torch)
-            var_dict_torch_update.update(var_dict_torch_update_local)
+        var_dict_torch_update_local = model.decoder.convert_tf2torch(var_dict_tf, var_dict_torch)
+        var_dict_torch_update.update(var_dict_torch_update_local)
 
         return var_dict_torch_update
-
-
-class EENDOLADiarTask(AbsTask):
-    # If you need more than 1 optimizer, change this value
-    num_optimizers: int = 1
-
-    # Add variable objects configurations
-    class_choices_list = [
-        # --frontend and --frontend_conf
-        frontend_choices,
-        # --specaug and --specaug_conf
-        model_choices,
-        # --encoder and --encoder_conf
-        encoder_choices,
-        # --speaker_encoder and --speaker_encoder_conf
-        encoder_decoder_attractor_choices,
-    ]
-
-    # If you need to modify train() or eval() procedures, change Trainer class here
-    trainer = Trainer
-
-    @classmethod
-    def add_task_arguments(cls, parser: argparse.ArgumentParser):
-        group = parser.add_argument_group(description="Task related")
-
-        # NOTE(kamo): add_arguments(..., required=True) can't be used
-        # to provide --print_config mode. Instead of it, do as
-        # required = parser.get_default("required")
-        # required += ["token_list"]
-
-        group.add_argument(
-            "--token_list",
-            type=str_or_none,
-            default=None,
-            help="A text mapping int-id to token",
-        )
-        group.add_argument(
-            "--split_with_space",
-            type=str2bool,
-            default=True,
-            help="whether to split text using <space>",
-        )
-        group.add_argument(
-            "--seg_dict_file",
-            type=str,
-            default=None,
-            help="seg_dict_file for text processing",
-        )
-        group.add_argument(
-            "--init",
-            type=lambda x: str_or_none(x.lower()),
-            default=None,
-            help="The initialization method",
-            choices=[
-                "chainer",
-                "xavier_uniform",
-                "xavier_normal",
-                "kaiming_uniform",
-                "kaiming_normal",
-                None,
-            ],
-        )
-
-        group.add_argument(
-            "--input_size",
-            type=int_or_none,
-            default=None,
-            help="The number of input dimension of the feature",
-        )
-
-        group = parser.add_argument_group(description="Preprocess related")
-        group.add_argument(
-            "--use_preprocessor",
-            type=str2bool,
-            default=True,
-            help="Apply preprocessing to data or not",
-        )
-        group.add_argument(
-            "--token_type",
-            type=str,
-            default="char",
-            choices=["char"],
-            help="The text will be tokenized in the specified level token",
-        )
-        parser.add_argument(
-            "--speech_volume_normalize",
-            type=float_or_none,
-            default=None,
-            help="Scale the maximum amplitude to the given value.",
-        )
-        parser.add_argument(
-            "--rir_scp",
-            type=str_or_none,
-            default=None,
-            help="The file path of rir scp file.",
-        )
-        parser.add_argument(
-            "--rir_apply_prob",
-            type=float,
-            default=1.0,
-            help="THe probability for applying RIR convolution.",
-        )
-        parser.add_argument(
-            "--cmvn_file",
-            type=str_or_none,
-            default=None,
-            help="The file path of noise scp file.",
-        )
-        parser.add_argument(
-            "--noise_scp",
-            type=str_or_none,
-            default=None,
-            help="The file path of noise scp file.",
-        )
-        parser.add_argument(
-            "--noise_apply_prob",
-            type=float,
-            default=1.0,
-            help="The probability applying Noise adding.",
-        )
-        parser.add_argument(
-            "--noise_db_range",
-            type=str,
-            default="13_15",
-            help="The range of noise decibel level.",
-        )
-
-        for class_choices in cls.class_choices_list:
-            # Append --<name> and --<name>_conf.
-            # e.g. --encoder and --encoder_conf
-            class_choices.add_arguments(group)
-
-    @classmethod
-    def build_collate_fn(
-            cls, args: argparse.Namespace, train: bool
-    ) -> Callable[
-        [Collection[Tuple[str, Dict[str, np.ndarray]]]],
-        Tuple[List[str], Dict[str, torch.Tensor]],
-    ]:
-        assert check_argument_types()
-        # NOTE(kamo): int value = 0 is reserved by CTC-blank symbol
-        return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
-
-    @classmethod
-    def build_preprocess_fn(
-            cls, args: argparse.Namespace, train: bool
-    ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
-        assert check_argument_types()
-        # if args.use_preprocessor:
-        #     retval = CommonPreprocessor(
-        #         train=train,
-        #         token_type=args.token_type,
-        #         token_list=args.token_list,
-        #         bpemodel=None,
-        #         non_linguistic_symbols=None,
-        #         text_cleaner=None,
-        #         g2p_type=None,
-        #         split_with_space=args.split_with_space if hasattr(args, "split_with_space") else False,
-        #         seg_dict_file=args.seg_dict_file if hasattr(args, "seg_dict_file") else None,
-        #         # NOTE(kamo): Check attribute existence for backward compatibility
-        #         rir_scp=args.rir_scp if hasattr(args, "rir_scp") else None,
-        #         rir_apply_prob=args.rir_apply_prob
-        #         if hasattr(args, "rir_apply_prob")
-        #         else 1.0,
-        #         noise_scp=args.noise_scp if hasattr(args, "noise_scp") else None,
-        #         noise_apply_prob=args.noise_apply_prob
-        #         if hasattr(args, "noise_apply_prob")
-        #         else 1.0,
-        #         noise_db_range=args.noise_db_range
-        #         if hasattr(args, "noise_db_range")
-        #         else "13_15",
-        #         speech_volume_normalize=args.speech_volume_normalize
-        #         if hasattr(args, "rir_scp")
-        #         else None,
-        #     )
-        # else:
-        #     retval = None
-        # assert check_return_type(retval)
-        return None
-
-    @classmethod
-    def required_data_names(
-            cls, train: bool = True, inference: bool = False
-    ) -> Tuple[str, ...]:
-        if not inference:
-            retval = ("speech", )
-        else:
-            # Recognition mode
-            retval = ("speech", )
-        return retval
-
-    @classmethod
-    def optional_data_names(
-            cls, train: bool = True, inference: bool = False
-    ) -> Tuple[str, ...]:
-        retval = ()
-        assert check_return_type(retval)
-        return retval
-
-    @classmethod
-    def build_model(cls, args: argparse.Namespace):
-        assert check_argument_types()
-
-        # 1. frontend
-        if args.input_size is None or args.frontend == "wav_frontend_mel23":
-            # Extract features in the model
-            frontend_class = frontend_choices.get_class(args.frontend)
-            if args.frontend == 'wav_frontend':
-                frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
-            else:
-                frontend = frontend_class(**args.frontend_conf)
-            input_size = frontend.output_size()
-        else:
-            # Give features from data-loader
-            args.frontend = None
-            args.frontend_conf = {}
-            frontend = None
-            input_size = args.input_size
-
-        # 2. Encoder
-        encoder_class = encoder_choices.get_class(args.encoder)
-        encoder = encoder_class(**args.encoder_conf)
-
-        # 3. EncoderDecoderAttractor
-        encoder_decoder_attractor_class = encoder_decoder_attractor_choices.get_class(args.encoder_decoder_attractor)
-        encoder_decoder_attractor = encoder_decoder_attractor_class(**args.encoder_decoder_attractor_conf)
-
-        # 9. Build model
-        model_class = model_choices.get_class(args.model)
-        model = model_class(
-            frontend=frontend,
-            encoder=encoder,
-            encoder_decoder_attractor=encoder_decoder_attractor,
-            **args.model_conf,
-        )
-
-        # 10. Initialize
-        if args.init is not None:
-            initialize(model, args.init)
-
-        assert check_return_type(model)
-        return model
-
-    # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
-    @classmethod
-    def build_model_from_file(
-            cls,
-            config_file: Union[Path, str] = None,
-            model_file: Union[Path, str] = None,
-            cmvn_file: Union[Path, str] = None,
-            device: str = "cpu",
-    ):
-        """Build model from the files.
-
-        This method is used for inference or fine-tuning.
-
-        Args:
-            config_file: The yaml file saved when training.
-            model_file: The model file saved when training.
-            cmvn_file: The cmvn file for front-end
-            device: Device type, "cpu", "cuda", or "cuda:N".
-
-        """
-        assert check_argument_types()
-        if config_file is None:
-            assert model_file is not None, (
-                "The argument 'model_file' must be provided "
-                "if the argument 'config_file' is not specified."
-            )
-            config_file = Path(model_file).parent / "config.yaml"
-        else:
-            config_file = Path(config_file)
-
-        with config_file.open("r", encoding="utf-8") as f:
-            args = yaml.safe_load(f)
-        args = argparse.Namespace(**args)
-        model = cls.build_model(args)
-        if not isinstance(model, AbsESPnetModel):
-            raise RuntimeError(
-                f"model must inherit {AbsESPnetModel.__name__}, but got {type(model)}"
-            )
-        if model_file is not None:
-            if device == "cuda":
-                device = f"cuda:{torch.cuda.current_device()}"
-            checkpoint = torch.load(model_file, map_location=device)
-            if "state_dict" in checkpoint.keys():
-                model.load_state_dict(checkpoint["state_dict"])
-            else:
-                model.load_state_dict(checkpoint)
-        model.to(device)
-        return model, args
```

### Comparing `funasr-0.4.1/funasr/tasks/lm.py` & `funasr-0.4.2/funasr/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/tasks/punctuation.py` & `funasr-0.4.2/funasr/tasks/punctuation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/text/build_tokenizer.py` & `funasr-0.4.2/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/text/char_tokenizer.py` & `funasr-0.4.2/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/text/cleaner.py` & `funasr-0.4.2/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/text/korean_cleaner.py` & `funasr-0.4.2/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/text/phoneme_tokenizer.py` & `funasr-0.4.2/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.4.2/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/text/token_id_converter.py` & `funasr-0.4.2/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/text/word_tokenizer.py` & `funasr-0.4.2/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.4.2/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/torch_utils/device_funcs.py` & `funasr-0.4.2/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/torch_utils/forward_adaptor.py` & `funasr-0.4.2/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/torch_utils/initialize.py` & `funasr-0.4.2/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.4.2/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/torch_utils/model_summary.py` & `funasr-0.4.2/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/torch_utils/recursive_op.py` & `funasr-0.4.2/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/train/abs_espnet_model.py` & `funasr-0.4.2/funasr/train/abs_espnet_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/train/abs_model.py` & `funasr-0.4.2/funasr/train/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/train/class_choices.py` & `funasr-0.4.2/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/train/distributed_utils.py` & `funasr-0.4.2/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/train/reporter.py` & `funasr-0.4.2/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/train/trainer.py` & `funasr-0.4.2/funasr/train/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,17 +182,14 @@
         if isinstance(trainer_options.keep_nbest_models, int):
             keep_nbest_models = [trainer_options.keep_nbest_models]
         else:
             if len(trainer_options.keep_nbest_models) == 0:
                 logging.warning("No keep_nbest_models is given. Change to [1]")
                 trainer_options.keep_nbest_models = [1]
             keep_nbest_models = trainer_options.keep_nbest_models
-     
-        #assert batch_interval is set and >0
-        assert trainer_options.batch_interval > 0
  
         output_dir = Path(trainer_options.output_dir)
         reporter = Reporter()
         if trainer_options.use_amp:
             if LooseVersion(torch.__version__) < LooseVersion("1.6.0"):
                 raise RuntimeError(
                     "Require torch>=1.6.0 for  Automatic Mixed Precision"
@@ -567,31 +564,39 @@
         #get the rank
         rank = distributed_option.dist_rank
         #get the num batch updates
         num_batch_updates = 0
         #ouput dir
         output_dir = Path(options.output_dir)
         #batch interval
-        batch_interval = options.batch_interval       
-        assert batch_interval > 0
+        batch_interval = options.batch_interval
  
         start_time = time.perf_counter()
         for iiter, (_, batch) in enumerate(
             reporter.measure_iter_time(iterator, "iter_time"), 1
         ):
             assert isinstance(batch, dict), type(batch)
 
-            if rank == 0:
+            if batch_interval > 0 and (not distributed_option.distributed or rank == 0):
                 if hasattr(model, "num_updates") or (hasattr(model, "module") and hasattr(model.module, "num_updates")):
                     num_batch_updates = model.get_num_updates() if hasattr(model,"num_updates") else model.module.get_num_updates()
-                if (num_batch_updates%batch_interval == 0) and (options.oss_bucket is not None) and options.use_pai:
-                    buffer = BytesIO()
-                    torch.save(model.state_dict(), buffer)
-                    options.oss_bucket.put_object(os.path.join(output_dir, f"{num_batch_updates}batch.pth"), buffer.getvalue())
- 
+                if num_batch_updates % batch_interval == 0:
+                    if options.use_pai and options.oss_bucket is not None:
+                        buffer = BytesIO()
+                        if hasattr(model, "module"):
+                            torch.save(model.module.state_dict(), buffer)
+                        else:
+                            torch.save(model.state_dict(), buffer)
+                        options.oss_bucket.put_object(os.path.join(output_dir, f"{num_batch_updates}step.pb"), buffer.getvalue())
+                    else:
+                        if hasattr(model, "module"):
+                            torch.save(model.module.state_dict(), os.path.join(output_dir, f"{num_batch_updates}step.pb"))
+                        else:
+                            torch.save(model.state_dict(), os.path.join(output_dir, f"{num_batch_updates}step.pb"))
+
             if distributed:
                 torch.distributed.all_reduce(iterator_stop, ReduceOp.SUM)
                 if iterator_stop > 0:
                     break
 
             batch = to_device(batch, "cuda" if ngpu > 0 else "cpu")
             if no_forward_run:
```

### Comparing `funasr-0.4.1/funasr/utils/asr_env_checking.py` & `funasr-0.4.2/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/asr_utils.py` & `funasr-0.4.2/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/build_dataclass.py` & `funasr-0.4.2/funasr/utils/build_dataclass.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/cli_utils.py` & `funasr-0.4.2/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/compute_eer.py` & `funasr-0.4.2/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/compute_min_dcf.py` & `funasr-0.4.2/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/compute_wer.py` & `funasr-0.4.2/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/config_argparse.py` & `funasr-0.4.2/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/get_default_kwargs.py` & `funasr-0.4.2/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/griffin_lim.py` & `funasr-0.4.2/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/job_runner.py` & `funasr-0.4.2/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/misc.py` & `funasr-0.4.2/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/modelscope_param.py` & `funasr-0.4.2/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/nested_dict_action.py` & `funasr-0.4.2/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/postprocess_utils.py` & `funasr-0.4.2/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/sized_dict.py` & `funasr-0.4.2/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/timestamp_tools.py` & `funasr-0.4.2/funasr/utils/timestamp_tools.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/types.py` & `funasr-0.4.2/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr/utils/wav_utils.py` & `funasr-0.4.2/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/funasr.egg-info/PKG-INFO` & `funasr-0.4.2/funasr.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,414 +1,491 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6675 6e61  : 2.1.Name: funa
 00000020: 7372 0a56 6572 7369 6f6e 3a20 302e 342e  sr.Version: 0.4.
-00000030: 310a 5375 6d6d 6172 793a 2046 756e 4153  1.Summary: FunAS
+00000030: 320a 5375 6d6d 6172 793a 2046 756e 4153  2.Summary: FunAS
 00000040: 523a 2041 2046 756e 6461 6d65 6e74 616c  R: A Fundamental
 00000050: 2045 6e64 2d74 6f2d 456e 6420 5370 6565   End-to-End Spee
 00000060: 6368 2052 6563 6f67 6e69 7469 6f6e 2054  ch Recognition T
 00000070: 6f6f 6c6b 6974 0a48 6f6d 652d 7061 6765  oolkit.Home-page
 00000080: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
 00000090: 2e63 6f6d 2f61 6c69 6261 6261 2d64 616d  .com/alibaba-dam
 000000a0: 6f2d 6163 6164 656d 792f 4675 6e41 5352  o-academy/FunASR
 000000b0: 2e67 6974 0a41 7574 686f 723a 2053 7065  .git.Author: Spe
-000000c0: 6563 6820 4c61 622c 2041 6c69 6261 6261  ech Lab, Alibaba
-000000d0: 2047 726f 7570 2c20 4368 696e 610a 4175   Group, China.Au
-000000e0: 7468 6f72 2d65 6d61 696c 3a20 6675 6e61  thor-email: funa
-000000f0: 7372 406c 6973 742e 616c 6962 6162 612d  sr@list.alibaba-
-00000100: 696e 632e 636f 6d0a 4c69 6365 6e73 653a  inc.com.License:
-00000110: 2054 6865 204d 4954 204c 6963 656e 7365   The MIT License
-00000120: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000130: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000140: 6520 3a3a 2050 7974 686f 6e0a 436c 6173  e :: Python.Clas
-00000150: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000160: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000170: 5079 7468 6f6e 203a 3a20 330a 436c 6173  Python :: 3.Clas
-00000180: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000190: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000001a0: 5079 7468 6f6e 203a 3a20 332e 370a 436c  Python :: 3.7.Cl
-000001b0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000001c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001d0: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
-000001e0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-000001f0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000200: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000210: 390a 436c 6173 7369 6669 6572 3a20 4465  9.Classifier: De
-00000220: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-00000230: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
-00000240: 6f6e 2f53 7461 626c 650a 436c 6173 7369  on/Stable.Classi
-00000250: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
-00000260: 7564 6965 6e63 6520 3a3a 2053 6369 656e  udience :: Scien
-00000270: 6365 2f52 6573 6561 7263 680a 436c 6173  ce/Research.Clas
-00000280: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
-00000290: 6720 5379 7374 656d 203a 3a20 504f 5349  g System :: POSI
-000002a0: 5820 3a3a 204c 696e 7578 0a43 6c61 7373  X :: Linux.Class
-000002b0: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-000002c0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-000002d0: 3a20 4170 6163 6865 2053 6f66 7477 6172  : Apache Softwar
-000002e0: 6520 4c69 6365 6e73 650a 436c 6173 7369  e License.Classi
-000002f0: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
-00000300: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
-00000310: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
-00000320: 203a 3a20 5079 7468 6f6e 204d 6f64 756c   :: Python Modul
-00000330: 6573 0a52 6571 7569 7265 732d 5079 7468  es.Requires-Pyth
-00000340: 6f6e 3a20 3e3d 332e 372e 300a 4465 7363  on: >=3.7.0.Desc
-00000350: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-00000360: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-00000370: 6f77 6e0a 5072 6f76 6964 6573 2d45 7874  own.Provides-Ext
-00000380: 7261 3a20 7472 6169 6e0a 5072 6f76 6964  ra: train.Provid
-00000390: 6573 2d45 7874 7261 3a20 7265 6369 7065  es-Extra: recipe
-000003a0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-000003b0: 2061 6c6c 0a50 726f 7669 6465 732d 4578   all.Provides-Ex
-000003c0: 7472 613a 2074 6573 740a 5072 6f76 6964  tra: test.Provid
-000003d0: 6573 2d45 7874 7261 3a20 646f 630a 4c69  es-Extra: doc.Li
-000003e0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-000003f0: 4e53 450a 0a5b 2f2f 5d3a 2023 2028 3c64  NSE..[//]: # (<d
-00000400: 6976 2061 6c69 676e 3d22 6c65 6674 223e  iv align="left">
-00000410: 3c69 6d67 2073 7263 3d22 646f 6373 2f69  <img src="docs/i
-00000420: 6d61 6765 732f 6675 6e61 7372 5f6c 6f67  mages/funasr_log
-00000430: 6f2e 6a70 6722 2077 6964 7468 3d22 3430  o.jpg" width="40
-00000440: 3022 2f3e 3c2f 6469 763e 290a 0a23 2046  0"/></div>)..# F
-00000450: 756e 4153 523a 2041 2046 756e 6461 6d65  unASR: A Fundame
-00000460: 6e74 616c 2045 6e64 2d74 6f2d 456e 6420  ntal End-to-End 
-00000470: 5370 6565 6368 2052 6563 6f67 6e69 7469  Speech Recogniti
-00000480: 6f6e 2054 6f6f 6c6b 6974 0a0a 3c73 7472  on Toolkit..<str
-00000490: 6f6e 673e 4675 6e41 5352 3c2f 7374 726f  ong>FunASR</stro
-000004a0: 6e67 3e20 686f 7065 7320 746f 2062 7569  ng> hopes to bui
-000004b0: 6c64 2061 2062 7269 6467 6520 6265 7477  ld a bridge betw
-000004c0: 6565 6e20 6163 6164 656d 6963 2072 6573  een academic res
-000004d0: 6561 7263 6820 616e 6420 696e 6475 7374  earch and indust
-000004e0: 7269 616c 2061 7070 6c69 6361 7469 6f6e  rial application
-000004f0: 7320 6f6e 2073 7065 6563 6820 7265 636f  s on speech reco
-00000500: 676e 6974 696f 6e2e 2042 7920 7375 7070  gnition. By supp
-00000510: 6f72 7469 6e67 2074 6865 2074 7261 696e  orting the train
-00000520: 696e 6720 2620 6669 6e65 7475 6e69 6e67  ing & finetuning
-00000530: 206f 6620 7468 6520 696e 6475 7374 7269   of the industri
-00000540: 616c 2d67 7261 6465 2073 7065 6563 6820  al-grade speech 
-00000550: 7265 636f 676e 6974 696f 6e20 6d6f 6465  recognition mode
-00000560: 6c20 7265 6c65 6173 6564 206f 6e20 5b4d  l released on [M
-00000570: 6f64 656c 5363 6f70 655d 2868 7474 7073  odelScope](https
-00000580: 3a2f 2f77 7777 2e6d 6f64 656c 7363 6f70  ://www.modelscop
-00000590: 652e 636e 2f6d 6f64 656c 733f 7061 6765  e.cn/models?page
-000005a0: 3d31 2674 6173 6b73 3d61 7574 6f2d 7370  =1&tasks=auto-sp
-000005b0: 6565 6368 2d72 6563 6f67 6e69 7469 6f6e  eech-recognition
-000005c0: 292c 2072 6573 6561 7263 6865 7273 2061  ), researchers a
-000005d0: 6e64 2064 6576 656c 6f70 6572 7320 6361  nd developers ca
-000005e0: 6e20 636f 6e64 7563 7420 7265 7365 6172  n conduct resear
-000005f0: 6368 2061 6e64 2070 726f 6475 6374 696f  ch and productio
-00000600: 6e20 6f66 2073 7065 6563 6820 7265 636f  n of speech reco
-00000610: 676e 6974 696f 6e20 6d6f 6465 6c73 206d  gnition models m
-00000620: 6f72 6520 636f 6e76 656e 6965 6e74 6c79  ore conveniently
-00000630: 2c20 616e 6420 7072 6f6d 6f74 6520 7468  , and promote th
-00000640: 6520 6465 7665 6c6f 706d 656e 7420 6f66  e development of
-00000650: 2073 7065 6563 6820 7265 636f 676e 6974   speech recognit
-00000660: 696f 6e20 6563 6f6c 6f67 792e 2041 5352  ion ecology. ASR
-00000670: 2066 6f72 2046 756e efbc 810a 0a5b 2a2a   for Fun.....[**
-00000680: 4e65 7773 2a2a 5d28 6874 7470 733a 2f2f  News**](https://
-00000690: 6769 7468 7562 2e63 6f6d 2f61 6c69 6261  github.com/aliba
-000006a0: 6261 2d64 616d 6f2d 6163 6164 656d 792f  ba-damo-academy/
-000006b0: 4675 6e41 5352 2377 6861 7473 2d6e 6577  FunASR#whats-new
-000006c0: 2920 0a7c 205b 2a2a 4869 6768 6c69 6768  ) .| [**Highligh
-000006d0: 7473 2a2a 5d28 2368 6967 686c 6967 6874  ts**](#highlight
-000006e0: 7329 0a7c 205b 2a2a 496e 7374 616c 6c61  s).| [**Installa
-000006f0: 7469 6f6e 2a2a 5d28 2369 6e73 7461 6c6c  tion**](#install
-00000700: 6174 696f 6e29 0a7c 205b 2a2a 446f 6373  ation).| [**Docs
-00000710: 5f45 4e2a 2a5d 2868 7474 7073 3a2f 2f61  _EN**](https://a
-00000720: 6c69 6261 6261 2d64 616d 6f2d 6163 6164  libaba-damo-acad
-00000730: 656d 792e 6769 7468 7562 2e69 6f2f 4675  emy.github.io/Fu
-00000740: 6e41 5352 2f65 6e2f 696e 6465 782e 6874  nASR/en/index.ht
-00000750: 6d6c 290a 7c20 5b2a 2a54 7574 6f72 6961  ml).| [**Tutoria
-00000760: 6c2a 2a5d 2868 7474 7073 3a2f 2f67 6974  l**](https://git
-00000770: 6875 622e 636f 6d2f 616c 6962 6162 612d  hub.com/alibaba-
-00000780: 6461 6d6f 2d61 6361 6465 6d79 2f46 756e  damo-academy/Fun
-00000790: 4153 522f 7769 6b69 2366 756e 6173 7225  ASR/wiki#funasr%
-000007a0: 4537 2539 3425 4138 2545 3625 3838 2542  E7%94%A8%E6%88%B
-000007b0: 3725 4536 2538 3925 3842 2545 3525 3836  7%E6%89%8B%E5%86
-000007c0: 2538 4329 0a7c 205b 2a2a 5061 7065 7273  %8C).| [**Papers
-000007d0: 2a2a 5d28 6874 7470 733a 2f2f 6769 7468  **](https://gith
-000007e0: 7562 2e63 6f6d 2f61 6c69 6261 6261 2d64  ub.com/alibaba-d
-000007f0: 616d 6f2d 6163 6164 656d 792f 4675 6e41  amo-academy/FunA
-00000800: 5352 2363 6974 6174 696f 6e73 290a 7c20  SR#citations).| 
-00000810: 5b2a 2a52 756e 7469 6d65 2a2a 5d28 6874  [**Runtime**](ht
-00000820: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000830: 2f61 6c69 6261 6261 2d64 616d 6f2d 6163  /alibaba-damo-ac
-00000840: 6164 656d 792f 4675 6e41 5352 2f74 7265  ademy/FunASR/tre
-00000850: 652f 6d61 696e 2f66 756e 6173 722f 7275  e/main/funasr/ru
-00000860: 6e74 696d 6529 0a7c 205b 2a2a 4d6f 6465  ntime).| [**Mode
-00000870: 6c20 5a6f 6f2a 2a5d 2868 7474 7073 3a2f  l Zoo**](https:/
-00000880: 2f67 6974 6875 622e 636f 6d2f 616c 6962  /github.com/alib
-00000890: 6162 612d 6461 6d6f 2d61 6361 6465 6d79  aba-damo-academy
-000008a0: 2f46 756e 4153 522f 626c 6f62 2f6d 6169  /FunASR/blob/mai
-000008b0: 6e2f 646f 6373 2f6d 6f64 656c 7363 6f70  n/docs/modelscop
-000008c0: 655f 6d6f 6465 6c73 2e6d 6429 0a7c 205b  e_models.md).| [
-000008d0: 2a2a 436f 6e74 6163 742a 2a5d 2823 636f  **Contact**](#co
-000008e0: 6e74 6163 7429 0a0a 0a23 2320 5768 6174  ntact)...## What
-000008f0: 2773 206e 6577 3a20 0a0a 466f 7220 7468  's new: ..For th
-00000900: 6520 7265 6c65 6173 6520 6e6f 7465 732c  e release notes,
-00000910: 2070 6c65 6173 6520 7265 6620 746f 205b   please ref to [
-00000920: 6e65 7773 5d28 6874 7470 733a 2f2f 6769  news](https://gi
-00000930: 7468 7562 2e63 6f6d 2f61 6c69 6261 6261  thub.com/alibaba
-00000940: 2d64 616d 6f2d 6163 6164 656d 792f 4675  -damo-academy/Fu
-00000950: 6e41 5352 2f72 656c 6561 7365 7329 0a0a  nASR/releases)..
-00000960: 2323 2048 6967 686c 6967 6874 730a 2d20  ## Highlights.- 
-00000970: 4d61 6e79 2074 7970 6573 206f 6620 7479  Many types of ty
-00000980: 7069 6361 6c20 6d6f 6465 6c73 2061 7265  pical models are
-00000990: 2073 7570 706f 7274 6564 2c20 652e 672e   supported, e.g.
-000009a0: 2c20 5b54 7261 6e66 6f72 6d65 725d 2868  , [Tranformer](h
-000009b0: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-000009c0: 2f61 6273 2f31 3730 362e 3033 3736 3229  /abs/1706.03762)
-000009d0: 2c20 5b43 6f6e 666f 726d 6572 5d28 6874  , [Conformer](ht
-000009e0: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-000009f0: 6162 732f 3230 3035 2e30 3831 3030 292c  abs/2005.08100),
-00000a00: 205b 5061 7261 666f 726d 6572 5d28 6874   [Paraformer](ht
-00000a10: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-00000a20: 6162 732f 3232 3036 2e30 3833 3137 292e  abs/2206.08317).
-00000a30: 0a2d 2057 6520 6861 7665 2072 656c 6561  .- We have relea
-00000a40: 7365 6420 6c61 7267 6520 6e75 6d62 6572  sed large number
-00000a50: 206f 6620 6163 6164 656d 6963 2061 6e64   of academic and
-00000a60: 2069 6e64 7573 7472 6961 6c20 7072 6574   industrial pret
-00000a70: 7261 696e 6564 206d 6f64 656c 7320 6f6e  rained models on
-00000a80: 205b 4d6f 6465 6c53 636f 7065 5d28 6874   [ModelScope](ht
-00000a90: 7470 733a 2f2f 7777 772e 6d6f 6465 6c73  tps://www.models
-00000aa0: 636f 7065 2e63 6e2f 6d6f 6465 6c73 3f70  cope.cn/models?p
-00000ab0: 6167 653d 3126 7461 736b 733d 6175 746f  age=1&tasks=auto
-00000ac0: 2d73 7065 6563 682d 7265 636f 676e 6974  -speech-recognit
-00000ad0: 696f 6e29 0a2d 2054 6865 2070 7265 7472  ion).- The pretr
-00000ae0: 6169 6e65 6420 6d6f 6465 6c20 5b50 6172  ained model [Par
-00000af0: 6166 6f72 6d65 722d 6c61 7267 655d 2868  aformer-large](h
-00000b00: 7474 7073 3a2f 2f77 7777 2e6d 6f64 656c  ttps://www.model
-00000b10: 7363 6f70 652e 636e 2f6d 6f64 656c 732f  scope.cn/models/
-00000b20: 6461 6d6f 2f73 7065 6563 685f 7061 7261  damo/speech_para
-00000b30: 666f 726d 6572 2d6c 6172 6765 5f61 7372  former-large_asr
-00000b40: 5f6e 6174 2d7a 682d 636e 2d31 366b 2d63  _nat-zh-cn-16k-c
-00000b50: 6f6d 6d6f 6e2d 766f 6361 6238 3430 342d  ommon-vocab8404-
-00000b60: 7079 746f 7263 682f 7375 6d6d 6172 7929  pytorch/summary)
-00000b70: 206f 6274 6169 6e73 2074 6865 2062 6573   obtains the bes
-00000b80: 7420 7065 7266 6f72 6d61 6e63 6520 6f6e  t performance on
-00000b90: 206d 616e 7920 7461 736b 7320 696e 205b   many tasks in [
-00000ba0: 5370 6565 6368 494f 206c 6561 6465 7262  SpeechIO leaderb
-00000bb0: 6f61 7264 5d28 6874 7470 733a 2f2f 6769  oard](https://gi
-00000bc0: 7468 7562 2e63 6f6d 2f53 7065 6563 6843  thub.com/SpeechC
-00000bd0: 6f6c 6162 2f4c 6561 6465 7262 6f61 7264  olab/Leaderboard
-00000be0: 290a 2d20 4675 6e41 5352 2073 7570 706c  ).- FunASR suppl
-00000bf0: 6965 7320 6120 6561 7379 2d74 6f2d 7573  ies a easy-to-us
-00000c00: 6520 7069 7065 6c69 6e65 2074 6f20 6669  e pipeline to fi
-00000c10: 6e65 7475 6e65 2070 7265 7472 6169 6e65  netune pretraine
-00000c20: 6420 6d6f 6465 6c73 2066 726f 6d20 5b4d  d models from [M
-00000c30: 6f64 656c 5363 6f70 655d 2868 7474 7073  odelScope](https
-00000c40: 3a2f 2f77 7777 2e6d 6f64 656c 7363 6f70  ://www.modelscop
-00000c50: 652e 636e 2f6d 6f64 656c 733f 7061 6765  e.cn/models?page
-00000c60: 3d31 2674 6173 6b73 3d61 7574 6f2d 7370  =1&tasks=auto-sp
-00000c70: 6565 6368 2d72 6563 6f67 6e69 7469 6f6e  eech-recognition
-00000c80: 290a 2d20 436f 6d70 6172 6564 2074 6f20  ).- Compared to 
-00000c90: 5b45 7370 6e65 745d 2868 7474 7073 3a2f  [Espnet](https:/
-00000ca0: 2f67 6974 6875 622e 636f 6d2f 6573 706e  /github.com/espn
-00000cb0: 6574 2f65 7370 6e65 7429 2066 7261 6d65  et/espnet) frame
-00000cc0: 776f 726b 2c20 7468 6520 7472 6169 6e69  work, the traini
-00000cd0: 6e67 2073 7065 6564 206f 6620 6c61 7267  ng speed of larg
-00000ce0: 652d 7363 616c 6520 6461 7461 7365 7473  e-scale datasets
-00000cf0: 2069 6e20 4675 6e41 5352 2069 7320 6d75   in FunASR is mu
-00000d00: 6368 2066 6173 7465 7220 6f77 6e69 6e67  ch faster owning
-00000d10: 2074 6f20 7468 6520 6f70 7469 6d69 7a65   to the optimize
-00000d20: 6420 6461 7461 6c6f 6164 6572 2e0a 0a23  d dataloader...#
-00000d30: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
-00000d40: 496e 7374 616c 6c20 6672 6f6d 2070 6970  Install from pip
-00000d50: 0a60 6060 7368 656c 6c0a 7069 7020 696e  .```shell.pip in
-00000d60: 7374 616c 6c20 2d55 2066 756e 6173 7220  stall -U funasr 
-00000d70: 2d69 2068 7474 7073 3a2f 2f70 7970 692e  -i https://pypi.
-00000d80: 5079 7468 6f6e 2e6f 7267 2f73 696d 706c  Python.org/simpl
-00000d90: 650a 6060 600a 0a4f 7220 696e 7374 616c  e.```..Or instal
-00000da0: 6c20 6672 6f6d 2073 6f75 7263 6520 636f  l from source co
-00000db0: 6465 0a0a 0a60 6060 2073 680a 6769 7420  de...``` sh.git 
-00000dc0: 636c 6f6e 6520 6874 7470 733a 2f2f 6769  clone https://gi
-00000dd0: 7468 7562 2e63 6f6d 2f61 6c69 6261 6261  thub.com/alibaba
-00000de0: 2f46 756e 4153 522e 6769 7420 2626 2063  /FunASR.git && c
-00000df0: 6420 4675 6e41 5352 0a70 6970 2069 6e73  d FunASR.pip ins
-00000e00: 7461 6c6c 202d 6520 2e2f 0a60 6060 0a49  tall -e ./.```.I
-00000e10: 6620 796f 7520 7761 6e74 2074 6f20 7573  f you want to us
-00000e20: 6520 7468 6520 7072 6574 7261 696e 6564  e the pretrained
-00000e30: 206d 6f64 656c 7320 696e 204d 6f64 656c   models in Model
-00000e40: 5363 6f70 652c 2079 6f75 2073 686f 756c  Scope, you shoul
-00000e50: 6420 696e 7374 616c 6c20 7468 6520 6d6f  d install the mo
-00000e60: 6465 6c73 636f 7065 3a0a 0a60 6060 7368  delscope:..```sh
-00000e70: 656c 6c0a 7069 7020 696e 7374 616c 6c20  ell.pip install 
-00000e80: 2d55 206d 6f64 656c 7363 6f70 650a 2320  -U modelscope.# 
-00000e90: 466f 7220 7468 6520 7573 6572 7320 696e  For the users in
-00000ea0: 2043 6869 6e61 2c20 796f 7520 636f 756c   China, you coul
-00000eb0: 6420 696e 7374 616c 6c20 7769 7468 2074  d install with t
-00000ec0: 6865 2063 6f6d 6d61 6e64 3a0a 2320 7069  he command:.# pi
-00000ed0: 7020 696e 7374 616c 6c20 2d55 206d 6f64  p install -U mod
-00000ee0: 656c 7363 6f70 6520 2d66 2068 7474 7073  elscope -f https
-00000ef0: 3a2f 2f6d 6f64 656c 7363 6f70 652e 6f73  ://modelscope.os
-00000f00: 732d 636e 2d62 6569 6a69 6e67 2e61 6c69  s-cn-beijing.ali
-00000f10: 7975 6e63 732e 636f 6d2f 7265 6c65 6173  yuncs.com/releas
-00000f20: 6573 2f72 6570 6f2e 6874 6d6c 202d 6920  es/repo.html -i 
-00000f30: 6874 7470 733a 2f2f 6d69 7272 6f72 2e73  https://mirror.s
-00000f40: 6a74 752e 6564 752e 636e 2f70 7970 692f  jtu.edu.cn/pypi/
-00000f50: 7765 622f 7369 6d70 6c65 0a60 6060 0a0a  web/simple.```..
-00000f60: 466f 7220 6d6f 7265 2064 6574 6169 6c73  For more details
-00000f70: 2c20 706c 6561 7365 2072 6566 2074 6f20  , please ref to 
-00000f80: 5b69 6e73 7461 6c6c 6174 696f 6e5d 2868  [installation](h
-00000f90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000fa0: 6d2f 616c 6962 6162 612d 6461 6d6f 2d61  m/alibaba-damo-a
-00000fb0: 6361 6465 6d79 2f46 756e 4153 522f 7769  cademy/FunASR/wi
-00000fc0: 6b69 290a 0a23 2320 5573 6167 650a 466f  ki)..## Usage.Fo
-00000fd0: 7220 7573 6572 7320 7768 6f20 6172 6520  r users who are 
-00000fe0: 6e65 7720 746f 2046 756e 4153 5220 616e  new to FunASR an
-00000ff0: 6420 4d6f 6465 6c53 636f 7065 2c20 706c  d ModelScope, pl
-00001000: 6561 7365 2072 6566 6572 2074 6f20 4675  ease refer to Fu
-00001010: 6e41 5352 2044 6f63 7328 5b43 4e5d 2868  nASR Docs([CN](h
-00001020: 7474 7073 3a2f 2f61 6c69 6261 6261 2d64  ttps://alibaba-d
-00001030: 616d 6f2d 6163 6164 656d 792e 6769 7468  amo-academy.gith
-00001040: 7562 2e69 6f2f 4675 6e41 5352 2f63 6e2f  ub.io/FunASR/cn/
-00001050: 696e 6465 782e 6874 6d6c 2920 2f20 5b45  index.html) / [E
-00001060: 4e5d 2868 7474 7073 3a2f 2f61 6c69 6261  N](https://aliba
-00001070: 6261 2d64 616d 6f2d 6163 6164 656d 792e  ba-damo-academy.
-00001080: 6769 7468 7562 2e69 6f2f 4675 6e41 5352  github.io/FunASR
-00001090: 2f65 6e2f 696e 6465 782e 6874 6d6c 2929  /en/index.html))
-000010a0: 0a0a 2323 2043 6f6e 7461 6374 0a0a 4966  ..## Contact..If
-000010b0: 2079 6f75 2068 6176 6520 616e 7920 7175   you have any qu
-000010c0: 6573 7469 6f6e 7320 6162 6f75 7420 4675  estions about Fu
-000010d0: 6e41 5352 2c20 706c 6561 7365 2063 6f6e  nASR, please con
-000010e0: 7461 6374 2075 7320 6279 0a0a 2d20 656d  tact us by..- em
-000010f0: 6169 6c3a 205b 6675 6e61 7372 406c 6973  ail: [funasr@lis
-00001100: 742e 616c 6962 6162 612d 696e 632e 636f  t.alibaba-inc.co
-00001110: 6d5d 2866 756e 6173 7240 6c69 7374 2e61  m](funasr@list.a
-00001120: 6c69 6261 6261 2d69 6e63 2e63 6f6d 290a  libaba-inc.com).
-00001130: 0a7c 4469 6e67 6469 6e67 2067 726f 7570  .|Dingding group
-00001140: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00001150: 2020 2020 2020 2057 6563 6861 7420 6772         Wechat gr
-00001160: 6f75 7020 2020 2020 2020 2020 2020 2020  oup             
-00001170: 2020 2020 2020 2020 207c 0a7c 3a2d 2d2d           |.|:---
-00001180: 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :|:-------------
-00001190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000011a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000011b0: 2d2d 2d2d 2d2d 2d2d 3a7c 0a7c 3c64 6976  --------:|.|<div
-000011c0: 2061 6c69 676e 3d22 6c65 6674 223e 3c69   align="left"><i
-000011d0: 6d67 2073 7263 3d22 646f 6373 2f69 6d61  mg src="docs/ima
-000011e0: 6765 732f 6469 6e67 6469 6e67 2e6a 7067  ges/dingding.jpg
-000011f0: 2220 7769 6474 683d 2232 3530 222f 3e20  " width="250"/> 
-00001200: 7c20 3c69 6d67 2073 7263 3d22 646f 6373  | <img src="docs
-00001210: 2f69 6d61 6765 732f 7765 6368 6174 2e70  /images/wechat.p
-00001220: 6e67 2220 7769 6474 683d 2232 3332 222f  ng" width="232"/
-00001230: 3e3c 2f64 6976 3e20 7c0a 0a23 2320 436f  ></div> |..## Co
-00001240: 6e74 7269 6275 746f 7273 0a0a 7c20 3c64  ntributors..| <d
-00001250: 6976 2061 6c69 676e 3d22 6c65 6674 223e  iv align="left">
-00001260: 3c69 6d67 2073 7263 3d22 646f 6373 2f69  <img src="docs/i
-00001270: 6d61 6765 732f 6461 6d6f 2e70 6e67 2220  mages/damo.png" 
-00001280: 7769 6474 683d 2231 3830 222f 3e20 7c20  width="180"/> | 
-00001290: 3c64 6976 2061 6c69 676e 3d22 6c65 6674  <div align="left
-000012a0: 223e 3c69 6d67 2073 7263 3d22 646f 6373  "><img src="docs
-000012b0: 2f69 6d61 6765 732f 6e77 7075 2e70 6e67  /images/nwpu.png
-000012c0: 2220 7769 6474 683d 2232 3630 222f 3e20  " width="260"/> 
-000012d0: 7c20 3c69 6d67 2073 7263 3d22 646f 6373  | <img src="docs
-000012e0: 2f69 6d61 6765 732f 4465 6570 5363 6965  /images/DeepScie
-000012f0: 6e63 652e 706e 6722 2077 6964 7468 3d22  nce.png" width="
-00001300: 3230 3022 2f3e 203c 2f64 6976 3e20 7c0a  200"/> </div> |.
-00001310: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
-00001320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001350: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -:|:------------
-00001360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001390: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
-000013a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000013d0: 2d3a 7c0a 0a23 2320 4163 6b6e 6f77 6c65  -:|..## Acknowle
-000013e0: 6467 650a 0a31 2e20 5765 2062 6f72 726f  dge..1. We borro
-000013f0: 7765 6420 6120 6c6f 7420 6f66 2063 6f64  wed a lot of cod
-00001400: 6520 6672 6f6d 205b 4b61 6c64 695d 2868  e from [Kaldi](h
-00001410: 7474 703a 2f2f 6b61 6c64 692d 6173 722e  ttp://kaldi-asr.
-00001420: 6f72 672f 2920 666f 7220 6461 7461 2070  org/) for data p
-00001430: 7265 7061 7261 7469 6f6e 2e0a 322e 2057  reparation..2. W
-00001440: 6520 626f 7272 6f77 6564 2061 206c 6f74  e borrowed a lot
-00001450: 206f 6620 636f 6465 2066 726f 6d20 5b45   of code from [E
-00001460: 5350 6e65 745d 2868 7474 7073 3a2f 2f67  SPnet](https://g
-00001470: 6974 6875 622e 636f 6d2f 6573 706e 6574  ithub.com/espnet
-00001480: 2f65 7370 6e65 7429 2e20 4675 6e41 5352  /espnet). FunASR
-00001490: 2066 6f6c 6c6f 7773 2075 7020 7468 6520   follows up the 
-000014a0: 7472 6169 6e69 6e67 2061 6e64 2066 696e  training and fin
-000014b0: 6574 756e 696e 6720 7069 7065 6c69 6e65  etuning pipeline
-000014c0: 7320 6f66 2045 5350 6e65 742e 0a33 2e20  s of ESPnet..3. 
-000014d0: 5765 2072 6566 6572 7265 6420 5b57 656e  We referred [Wen
-000014e0: 6574 5d28 6874 7470 733a 2f2f 6769 7468  et](https://gith
-000014f0: 7562 2e63 6f6d 2f77 656e 6574 2d65 3265  ub.com/wenet-e2e
-00001500: 2f77 656e 6574 2920 666f 7220 6275 696c  /wenet) for buil
-00001510: 6469 6e67 2064 6174 616c 6f61 6465 7220  ding dataloader 
-00001520: 666f 7220 6c61 7267 6520 7363 616c 6520  for large scale 
-00001530: 6461 7461 2074 7261 696e 696e 672e 0a34  data training..4
-00001540: 2e20 5765 2061 636b 6e6f 776c 6564 6765  . We acknowledge
-00001550: 205b 4465 6570 5363 6965 6e63 655d 2868   [DeepScience](h
-00001560: 7474 7073 3a2f 2f77 7777 2e64 6565 7073  ttps://www.deeps
-00001570: 6369 656e 6365 2e63 6e29 2066 6f72 2063  cience.cn) for c
-00001580: 6f6e 7472 6962 7574 696e 6720 7468 6520  ontributing the 
-00001590: 6772 7063 2073 6572 7669 6365 2e0a 0a23  grpc service...#
-000015a0: 2320 4c69 6365 6e73 650a 5468 6973 2070  # License.This p
-000015b0: 726f 6a65 6374 2069 7320 6c69 6365 6e73  roject is licens
-000015c0: 6564 2075 6e64 6572 2074 6865 205b 5468  ed under the [Th
-000015d0: 6520 4d49 5420 4c69 6365 6e73 655d 2868  e MIT License](h
-000015e0: 7474 7073 3a2f 2f6f 7065 6e73 6f75 7263  ttps://opensourc
-000015f0: 652e 6f72 672f 6c69 6365 6e73 6573 2f4d  e.org/licenses/M
-00001600: 4954 292e 2046 756e 4153 5220 616c 736f  IT). FunASR also
-00001610: 2063 6f6e 7461 696e 7320 7661 7269 6f75   contains variou
-00001620: 7320 7468 6972 642d 7061 7274 7920 636f  s third-party co
-00001630: 6d70 6f6e 656e 7473 2061 6e64 2073 6f6d  mponents and som
-00001640: 6520 636f 6465 206d 6f64 6966 6965 6420  e code modified 
-00001650: 6672 6f6d 206f 7468 6572 2072 6570 6f73  from other repos
-00001660: 2075 6e64 6572 206f 7468 6572 206f 7065   under other ope
-00001670: 6e20 736f 7572 6365 206c 6963 656e 7365  n source license
-00001680: 732e 0a0a 2323 2043 6974 6174 696f 6e73  s...## Citations
-00001690: 0a0a 6060 6020 6269 6274 6578 0a40 696e  ..``` bibtex.@in
-000016a0: 7072 6f63 6565 6469 6e67 737b 6761 6f32  proceedings{gao2
-000016b0: 3032 3075 6e69 7665 7273 616c 2c0a 2020  020universal,.  
-000016c0: 7469 746c 653d 7b55 6e69 7665 7273 616c  title={Universal
-000016d0: 2041 5352 3a20 556e 6966 7969 6e67 2053   ASR: Unifying S
-000016e0: 7472 6561 6d69 6e67 2061 6e64 204e 6f6e  treaming and Non
-000016f0: 2d53 7472 6561 6d69 6e67 2041 5352 2055  -Streaming ASR U
-00001700: 7369 6e67 2061 2053 696e 676c 6520 456e  sing a Single En
-00001710: 636f 6465 722d 4465 636f 6465 7220 4d6f  coder-Decoder Mo
-00001720: 6465 6c7d 2c0a 2020 6175 7468 6f72 3d7b  del},.  author={
-00001730: 4761 6f2c 205a 6869 6675 2061 6e64 205a  Gao, Zhifu and Z
-00001740: 6861 6e67 2c20 5368 696c 6961 6e67 2061  hang, Shiliang a
-00001750: 6e64 204c 6569 2c20 4d69 6e67 2061 6e64  nd Lei, Ming and
-00001760: 204d 634c 6f75 6768 6c69 6e2c 2049 616e   McLoughlin, Ian
-00001770: 7d2c 0a20 2062 6f6f 6b74 6974 6c65 3d7b  },.  booktitle={
-00001780: 6172 5869 7620 7072 6570 7269 6e74 2061  arXiv preprint a
-00001790: 7258 6976 3a32 3031 302e 3134 3039 397d  rXiv:2010.14099}
-000017a0: 2c0a 2020 7965 6172 3d7b 3230 3230 7d0a  ,.  year={2020}.
-000017b0: 7d0a 0a40 696e 7072 6f63 6565 6469 6e67  }..@inproceeding
-000017c0: 737b 6761 6f32 3032 3270 6172 6166 6f72  s{gao2022parafor
-000017d0: 6d65 722c 0a20 2074 6974 6c65 3d7b 5061  mer,.  title={Pa
-000017e0: 7261 666f 726d 6572 3a20 4661 7374 2061  raformer: Fast a
-000017f0: 6e64 2041 6363 7572 6174 6520 5061 7261  nd Accurate Para
-00001800: 6c6c 656c 2054 7261 6e73 666f 726d 6572  llel Transformer
-00001810: 2066 6f72 204e 6f6e 2d61 7574 6f72 6567   for Non-autoreg
-00001820: 7265 7373 6976 6520 456e 642d 746f 2d45  ressive End-to-E
-00001830: 6e64 2053 7065 6563 6820 5265 636f 676e  nd Speech Recogn
-00001840: 6974 696f 6e7d 2c0a 2020 6175 7468 6f72  ition},.  author
-00001850: 3d7b 4761 6f2c 205a 6869 6675 2061 6e64  ={Gao, Zhifu and
-00001860: 205a 6861 6e67 2c20 5368 696c 6961 6e67   Zhang, Shiliang
-00001870: 2061 6e64 204d 634c 6f75 6768 6c69 6e2c   and McLoughlin,
-00001880: 2049 616e 2061 6e64 2059 616e 2c20 5a68   Ian and Yan, Zh
-00001890: 696a 6965 7d2c 0a20 2062 6f6f 6b74 6974  ijie},.  booktit
-000018a0: 6c65 3d7b 494e 5445 5253 5045 4543 487d  le={INTERSPEECH}
-000018b0: 2c0a 2020 7965 6172 3d7b 3230 3232 7d0a  ,.  year={2022}.
-000018c0: 7d0a 4069 6e70 726f 6365 6564 696e 6773  }.@inproceedings
-000018d0: 7b53 6869 3230 3233 4163 6869 6576 696e  {Shi2023Achievin
-000018e0: 6754 502c 0a20 2074 6974 6c65 3d7b 4163  gTP,.  title={Ac
-000018f0: 6869 6576 696e 6720 5469 6d65 7374 616d  hieving Timestam
-00001900: 7020 5072 6564 6963 7469 6f6e 2057 6869  p Prediction Whi
-00001910: 6c65 2052 6563 6f67 6e69 7a69 6e67 2077  le Recognizing w
-00001920: 6974 6820 4e6f 6e2d 4175 746f 7265 6772  ith Non-Autoregr
-00001930: 6573 7369 7665 2045 6e64 2d74 6f2d 456e  essive End-to-En
-00001940: 6420 4153 5220 4d6f 6465 6c7d 2c0a 2020  d ASR Model},.  
-00001950: 6175 7468 6f72 3d7b 5869 616e 2053 6869  author={Xian Shi
-00001960: 2061 6e64 2059 616e 6e69 2043 6865 6e20   and Yanni Chen 
-00001970: 616e 6420 5368 696c 6961 6e67 205a 6861  and Shiliang Zha
-00001980: 6e67 2061 6e64 205a 6869 6a69 6520 5961  ng and Zhijie Ya
-00001990: 6e7d 2c0a 2020 626f 6f6b 7469 746c 653d  n},.  booktitle=
-000019a0: 7b61 7258 6976 2070 7265 7072 696e 7420  {arXiv preprint 
-000019b0: 6172 5869 763a 3233 3031 2e31 3233 3433  arXiv:2301.12343
-000019c0: 7d0a 2020 7965 6172 3d7b 3230 3233 7d0a  }.  year={2023}.
-000019d0: 7d0a 6060 600a                           }.```.
+000000c0: 6563 6820 4c61 6220 6f66 2044 414d 4f20  ech Lab of DAMO 
+000000d0: 4163 6164 656d 792c 2041 6c69 6261 6261  Academy, Alibaba
+000000e0: 2047 726f 7570 0a41 7574 686f 722d 656d   Group.Author-em
+000000f0: 6169 6c3a 2066 756e 6173 7240 6c69 7374  ail: funasr@list
+00000100: 2e61 6c69 6261 6261 2d69 6e63 2e63 6f6d  .alibaba-inc.com
+00000110: 0a4c 6963 656e 7365 3a20 5468 6520 4d49  .License: The MI
+00000120: 5420 4c69 6365 6e73 650a 506c 6174 666f  T License.Platfo
+00000130: 726d 3a20 554e 4b4e 4f57 4e0a 436c 6173  rm: UNKNOWN.Clas
+00000140: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000150: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000160: 5079 7468 6f6e 0a43 6c61 7373 6966 6965  Python.Classifie
+00000170: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000180: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000190: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
+000001a0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000001b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001c0: 6e20 3a3a 2033 2e37 0a43 6c61 7373 6966  n :: 3.7.Classif
+000001d0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000001e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001f0: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
+00000200: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000210: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000220: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+00000230: 7373 6966 6965 723a 2044 6576 656c 6f70  ssifier: Develop
+00000240: 6d65 6e74 2053 7461 7475 7320 3a3a 2035  ment Status :: 5
+00000250: 202d 2050 726f 6475 6374 696f 6e2f 5374   - Production/St
+00000260: 6162 6c65 0a43 6c61 7373 6966 6965 723a  able.Classifier:
+00000270: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
+00000280: 6365 203a 3a20 5363 6965 6e63 652f 5265  ce :: Science/Re
+00000290: 7365 6172 6368 0a43 6c61 7373 6966 6965  search.Classifie
+000002a0: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+000002b0: 7465 6d20 3a3a 2050 4f53 4958 203a 3a20  tem :: POSIX :: 
+000002c0: 4c69 6e75 780a 436c 6173 7369 6669 6572  Linux.Classifier
+000002d0: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
+000002e0: 2041 7070 726f 7665 6420 3a3a 2041 7061   Approved :: Apa
+000002f0: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
+00000300: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
+00000310: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
+00000320: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
+00000330: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
+00000340: 7974 686f 6e20 4d6f 6475 6c65 730a 5265  ython Modules.Re
+00000350: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
+00000360: 3d33 2e37 2e30 0a44 6573 6372 6970 7469  =3.7.0.Descripti
+00000370: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00000380: 2074 6578 742f 6d61 726b 646f 776e 0a50   text/markdown.P
+00000390: 726f 7669 6465 732d 4578 7472 613a 2074  rovides-Extra: t
+000003a0: 7261 696e 0a50 726f 7669 6465 732d 4578  rain.Provides-Ex
+000003b0: 7472 613a 2072 6563 6970 650a 5072 6f76  tra: recipe.Prov
+000003c0: 6964 6573 2d45 7874 7261 3a20 616c 6c0a  ides-Extra: all.
+000003d0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+000003e0: 7465 7374 0a50 726f 7669 6465 732d 4578  test.Provides-Ex
+000003f0: 7472 613a 2064 6f63 0a4c 6963 656e 7365  tra: doc.License
+00000400: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
+00000410: 5b2f 2f5d 3a20 2320 283c 6469 7620 616c  [//]: # (<div al
+00000420: 6967 6e3d 226c 6566 7422 3e3c 696d 6720  ign="left"><img 
+00000430: 7372 633d 2264 6f63 732f 696d 6167 6573  src="docs/images
+00000440: 2f66 756e 6173 725f 6c6f 676f 2e6a 7067  /funasr_logo.jpg
+00000450: 2220 7769 6474 683d 2234 3030 222f 3e3c  " width="400"/><
+00000460: 2f64 6976 3e29 0a0a 2320 4675 6e41 5352  /div>)..# FunASR
+00000470: 3a20 4120 4675 6e64 616d 656e 7461 6c20  : A Fundamental 
+00000480: 456e 642d 746f 2d45 6e64 2053 7065 6563  End-to-End Speec
+00000490: 6820 5265 636f 676e 6974 696f 6e20 546f  h Recognition To
+000004a0: 6f6c 6b69 740a 3c70 2061 6c69 676e 3d22  olkit.<p align="
+000004b0: 6c65 6674 223e 0a20 2020 203c 6120 6872  left">.    <a hr
+000004c0: 6566 3d22 223e 3c69 6d67 2073 7263 3d22  ef=""><img src="
+000004d0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000004e0: 6c64 732e 696f 2f62 6164 6765 2f4f 532d  lds.io/badge/OS-
+000004f0: 4c69 6e75 7825 3243 2532 3057 696e 2532  Linux%2C%20Win%2
+00000500: 4325 3230 4d61 632d 6272 6967 6874 6772  C%20Mac-brightgr
+00000510: 6565 6e2e 7376 6722 3e3c 2f61 3e0a 2020  een.svg"></a>.  
+00000520: 2020 3c61 2068 7265 663d 2222 3e3c 696d    <a href=""><im
+00000530: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000540: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000550: 6467 652f 5079 7468 6f6e 2d3e 3d33 2e37  dge/Python->=3.7
+00000560: 2c3c 3d33 2e31 302d 6166 662e 7376 6722  ,<=3.10-aff.svg"
+00000570: 3e3c 2f61 3e0a 2020 2020 3c61 2068 7265  ></a>.    <a hre
+00000580: 663d 2222 3e3c 696d 6720 7372 633d 2268  f=""><img src="h
+00000590: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000005a0: 6473 2e69 6f2f 6261 6467 652f 5079 746f  ds.io/badge/Pyto
+000005b0: 7263 682d 2533 4525 3344 312e 3131 2d62  rch-%3E%3D1.11-b
+000005c0: 6c75 6522 3e3c 2f61 3e0a 3c2f 703e 0a0a  lue"></a>.</p>..
+000005d0: 3c73 7472 6f6e 673e 4675 6e41 5352 3c2f  <strong>FunASR</
+000005e0: 7374 726f 6e67 3e20 686f 7065 7320 746f  strong> hopes to
+000005f0: 2062 7569 6c64 2061 2062 7269 6467 6520   build a bridge 
+00000600: 6265 7477 6565 6e20 6163 6164 656d 6963  between academic
+00000610: 2072 6573 6561 7263 6820 616e 6420 696e   research and in
+00000620: 6475 7374 7269 616c 2061 7070 6c69 6361  dustrial applica
+00000630: 7469 6f6e 7320 6f6e 2073 7065 6563 6820  tions on speech 
+00000640: 7265 636f 676e 6974 696f 6e2e 2042 7920  recognition. By 
+00000650: 7375 7070 6f72 7469 6e67 2074 6865 2074  supporting the t
+00000660: 7261 696e 696e 6720 2620 6669 6e65 7475  raining & finetu
+00000670: 6e69 6e67 206f 6620 7468 6520 696e 6475  ning of the indu
+00000680: 7374 7269 616c 2d67 7261 6465 2073 7065  strial-grade spe
+00000690: 6563 6820 7265 636f 676e 6974 696f 6e20  ech recognition 
+000006a0: 6d6f 6465 6c20 7265 6c65 6173 6564 206f  model released o
+000006b0: 6e20 5b4d 6f64 656c 5363 6f70 655d 2868  n [ModelScope](h
+000006c0: 7474 7073 3a2f 2f77 7777 2e6d 6f64 656c  ttps://www.model
+000006d0: 7363 6f70 652e 636e 2f6d 6f64 656c 733f  scope.cn/models?
+000006e0: 7061 6765 3d31 2674 6173 6b73 3d61 7574  page=1&tasks=aut
+000006f0: 6f2d 7370 6565 6368 2d72 6563 6f67 6e69  o-speech-recogni
+00000700: 7469 6f6e 292c 2072 6573 6561 7263 6865  tion), researche
+00000710: 7273 2061 6e64 2064 6576 656c 6f70 6572  rs and developer
+00000720: 7320 6361 6e20 636f 6e64 7563 7420 7265  s can conduct re
+00000730: 7365 6172 6368 2061 6e64 2070 726f 6475  search and produ
+00000740: 6374 696f 6e20 6f66 2073 7065 6563 6820  ction of speech 
+00000750: 7265 636f 676e 6974 696f 6e20 6d6f 6465  recognition mode
+00000760: 6c73 206d 6f72 6520 636f 6e76 656e 6965  ls more convenie
+00000770: 6e74 6c79 2c20 616e 6420 7072 6f6d 6f74  ntly, and promot
+00000780: 6520 7468 6520 6465 7665 6c6f 706d 656e  e the developmen
+00000790: 7420 6f66 2073 7065 6563 6820 7265 636f  t of speech reco
+000007a0: 676e 6974 696f 6e20 6563 6f6c 6f67 792e  gnition ecology.
+000007b0: 2041 5352 2066 6f72 2046 756e efbc 810a   ASR for Fun....
+000007c0: 0a5b 2a2a 4e65 7773 2a2a 5d28 6874 7470  .[**News**](http
+000007d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+000007e0: 6c69 6261 6261 2d64 616d 6f2d 6163 6164  libaba-damo-acad
+000007f0: 656d 792f 4675 6e41 5352 2377 6861 7473  emy/FunASR#whats
+00000800: 2d6e 6577 2920 0a7c 205b 2a2a 4869 6768  -new) .| [**High
+00000810: 6c69 6768 7473 2a2a 5d28 2368 6967 686c  lights**](#highl
+00000820: 6967 6874 7329 0a7c 205b 2a2a 496e 7374  ights).| [**Inst
+00000830: 616c 6c61 7469 6f6e 2a2a 5d28 2369 6e73  allation**](#ins
+00000840: 7461 6c6c 6174 696f 6e29 0a7c 205b 2a2a  tallation).| [**
+00000850: 446f 6373 2a2a 5d28 6874 7470 733a 2f2f  Docs**](https://
+00000860: 616c 6962 6162 612d 6461 6d6f 2d61 6361  alibaba-damo-aca
+00000870: 6465 6d79 2e67 6974 6875 622e 696f 2f46  demy.github.io/F
+00000880: 756e 4153 522f 656e 2f69 6e64 6578 2e68  unASR/en/index.h
+00000890: 746d 6c29 0a7c 205b 2a2a 5475 746f 7269  tml).| [**Tutori
+000008a0: 616c 2a2a 5d28 6874 7470 733a 2f2f 6769  al**](https://gi
+000008b0: 7468 7562 2e63 6f6d 2f61 6c69 6261 6261  thub.com/alibaba
+000008c0: 2d64 616d 6f2d 6163 6164 656d 792f 4675  -damo-academy/Fu
+000008d0: 6e41 5352 2f77 696b 6923 6675 6e61 7372  nASR/wiki#funasr
+000008e0: 2545 3725 3934 2541 3825 4536 2538 3825  %E7%94%A8%E6%88%
+000008f0: 4237 2545 3625 3839 2538 4225 4535 2538  B7%E6%89%8B%E5%8
+00000900: 3625 3843 290a 7c20 5b2a 2a50 6170 6572  6%8C).| [**Paper
+00000910: 732a 2a5d 2868 7474 7073 3a2f 2f67 6974  s**](https://git
+00000920: 6875 622e 636f 6d2f 616c 6962 6162 612d  hub.com/alibaba-
+00000930: 6461 6d6f 2d61 6361 6465 6d79 2f46 756e  damo-academy/Fun
+00000940: 4153 5223 6369 7461 7469 6f6e 7329 0a7c  ASR#citations).|
+00000950: 205b 2a2a 5275 6e74 696d 652a 2a5d 2868   [**Runtime**](h
+00000960: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000970: 6d2f 616c 6962 6162 612d 6461 6d6f 2d61  m/alibaba-damo-a
+00000980: 6361 6465 6d79 2f46 756e 4153 522f 7472  cademy/FunASR/tr
+00000990: 6565 2f6d 6169 6e2f 6675 6e61 7372 2f72  ee/main/funasr/r
+000009a0: 756e 7469 6d65 290a 7c20 5b2a 2a4d 6f64  untime).| [**Mod
+000009b0: 656c 205a 6f6f 2a2a 5d28 6874 7470 733a  el Zoo**](https:
+000009c0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6c69  //github.com/ali
+000009d0: 6261 6261 2d64 616d 6f2d 6163 6164 656d  baba-damo-academ
+000009e0: 792f 4675 6e41 5352 2f62 6c6f 622f 6d61  y/FunASR/blob/ma
+000009f0: 696e 2f64 6f63 732f 6d6f 6465 6c73 636f  in/docs/modelsco
+00000a00: 7065 5f6d 6f64 656c 732e 6d64 290a 7c20  pe_models.md).| 
+00000a10: 5b2a 2a43 6f6e 7461 6374 2a2a 5d28 2363  [**Contact**](#c
+00000a20: 6f6e 7461 6374 290a 7c0a 5b2a 2a4d 324d  ontact).|.[**M2M
+00000a30: 4554 322e 3020 4775 6964 656e 6365 5f43  ET2.0 Guidence_C
+00000a40: 4e2a 2a5d 2868 7474 7073 3a2f 2f61 6c69  N**](https://ali
+00000a50: 6261 6261 2d64 616d 6f2d 6163 6164 656d  baba-damo-academ
+00000a60: 792e 6769 7468 7562 2e69 6f2f 4675 6e41  y.github.io/FunA
+00000a70: 5352 2f6d 326d 6574 325f 636e 2f69 6e64  SR/m2met2_cn/ind
+00000a80: 6578 2e68 746d 6c29 0a7c 205b 2a2a 4d32  ex.html).| [**M2
+00000a90: 4d45 5432 2e30 2047 7569 6465 6e63 655f  MET2.0 Guidence_
+00000aa0: 454e 2a2a 5d28 6874 7470 733a 2f2f 616c  EN**](https://al
+00000ab0: 6962 6162 612d 6461 6d6f 2d61 6361 6465  ibaba-damo-acade
+00000ac0: 6d79 2e67 6974 6875 622e 696f 2f46 756e  my.github.io/Fun
+00000ad0: 4153 522f 6d32 6d65 7432 2f69 6e64 6578  ASR/m2met2/index
+00000ae0: 2e68 746d 6c29 0a0a 2323 204d 756c 7469  .html)..## Multi
+00000af0: 2d43 6861 6e6e 656c 204d 756c 7469 2d50  -Channel Multi-P
+00000b00: 6172 7479 204d 6565 7469 6e67 2054 7261  arty Meeting Tra
+00000b10: 6e73 6372 6970 7469 6f6e 2032 2e30 2028  nscription 2.0 (
+00000b20: 4d32 4d45 5432 2e30 2920 4368 616c 6c65  M2MET2.0) Challe
+00000b30: 6e67 650a 5765 2061 7265 2070 6c65 6173  nge.We are pleas
+00000b40: 6564 2074 6f20 616e 6e6f 756e 6365 2074  ed to announce t
+00000b50: 6861 7420 7468 6520 4d32 4d65 5432 2e30  hat the M2MeT2.0
+00000b60: 2063 6861 6c6c 656e 6765 2077 696c 6c20   challenge will 
+00000b70: 6265 2068 656c 6420 696e 2074 6865 206e  be held in the n
+00000b80: 6561 7220 6675 7475 7265 2e20 5468 6520  ear future. The 
+00000b90: 6261 7365 6c69 6e65 2073 7973 7465 6d20  baseline system 
+00000ba0: 6973 2063 6f6e 6475 6374 6564 206f 6e20  is conducted on 
+00000bb0: 4675 6e41 5352 2061 6e64 2069 7320 7072  FunASR and is pr
+00000bc0: 6f76 6964 6564 2061 7320 6120 7265 6365  ovided as a rece
+00000bd0: 6970 6520 6f66 2041 6c69 4d65 6574 696e  ipe of AliMeetin
+00000be0: 6720 636f 7270 7573 2e20 466f 7220 6d6f  g corpus. For mo
+00000bf0: 7265 2064 6574 6169 6c73 2079 6f75 2063  re details you c
+00000c00: 616e 2073 6565 2074 6865 2067 7569 6465  an see the guide
+00000c10: 6e63 6520 6f66 204d 324d 4554 322e 3020  nce of M2MET2.0 
+00000c20: 285b 434e 5d28 6874 7470 733a 2f2f 616c  ([CN](https://al
+00000c30: 6962 6162 612d 6461 6d6f 2d61 6361 6465  ibaba-damo-acade
+00000c40: 6d79 2e67 6974 6875 622e 696f 2f46 756e  my.github.io/Fun
+00000c50: 4153 522f 6d32 6d65 7432 5f63 6e2f 696e  ASR/m2met2_cn/in
+00000c60: 6465 782e 6874 6d6c 292f 5b45 4e5d 2868  dex.html)/[EN](h
+00000c70: 7474 7073 3a2f 2f61 6c69 6261 6261 2d64  ttps://alibaba-d
+00000c80: 616d 6f2d 6163 6164 656d 792e 6769 7468  amo-academy.gith
+00000c90: 7562 2e69 6f2f 4675 6e41 5352 2f6d 326d  ub.io/FunASR/m2m
+00000ca0: 6574 322f 696e 6465 782e 6874 6d6c 2929  et2/index.html))
+00000cb0: 2e0a 2323 2057 6861 7427 7320 6e65 773a  ..## What's new:
+00000cc0: 200a 0a46 6f72 2074 6865 2072 656c 6561   ..For the relea
+00000cd0: 7365 206e 6f74 6573 2c20 706c 6561 7365  se notes, please
+00000ce0: 2072 6566 2074 6f20 5b6e 6577 735d 2868   ref to [news](h
+00000cf0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000d00: 6d2f 616c 6962 6162 612d 6461 6d6f 2d61  m/alibaba-damo-a
+00000d10: 6361 6465 6d79 2f46 756e 4153 522f 7265  cademy/FunASR/re
+00000d20: 6c65 6173 6573 290a 0a23 2320 4869 6768  leases)..## High
+00000d30: 6c69 6768 7473 0a2d 2046 756e 4153 5220  lights.- FunASR 
+00000d40: 7375 7070 6f72 7473 2073 7065 6563 6820  supports speech 
+00000d50: 7265 636f 676e 6974 696f 6e28 4153 5229  recognition(ASR)
+00000d60: 2c20 4d75 6c74 692d 7461 6c6b 6572 2041  , Multi-talker A
+00000d70: 5352 2c20 566f 6963 6520 4163 7469 7669  SR, Voice Activi
+00000d80: 7479 2044 6574 6563 7469 6f6e 2856 4144  ty Detection(VAD
+00000d90: 292c 2050 756e 6374 7561 7469 6f6e 2052  ), Punctuation R
+00000da0: 6573 746f 7261 7469 6f6e 2c20 4c61 6e67  estoration, Lang
+00000db0: 7561 6765 204d 6f64 656c 732c 2053 7065  uage Models, Spe
+00000dc0: 616b 6572 2056 6572 6966 6963 6174 696f  aker Verificatio
+00000dd0: 6e20 616e 6420 5370 6561 6b65 7220 6469  n and Speaker di
+00000de0: 6172 697a 6174 696f 6e2e 2020 200a 2d20  arization.   .- 
+00000df0: 5765 2068 6176 6520 7265 6c65 6173 6564  We have released
+00000e00: 206c 6172 6765 206e 756d 6265 7220 6f66   large number of
+00000e10: 2061 6361 6465 6d69 6320 616e 6420 696e   academic and in
+00000e20: 6475 7374 7269 616c 2070 7265 7472 6169  dustrial pretrai
+00000e30: 6e65 6420 6d6f 6465 6c73 206f 6e20 5b4d  ned models on [M
+00000e40: 6f64 656c 5363 6f70 655d 2868 7474 7073  odelScope](https
+00000e50: 3a2f 2f77 7777 2e6d 6f64 656c 7363 6f70  ://www.modelscop
+00000e60: 652e 636e 2f6d 6f64 656c 733f 7061 6765  e.cn/models?page
+00000e70: 3d31 2674 6173 6b73 3d61 7574 6f2d 7370  =1&tasks=auto-sp
+00000e80: 6565 6368 2d72 6563 6f67 6e69 7469 6f6e  eech-recognition
+00000e90: 290a 2d20 5468 6520 7072 6574 7261 696e  ).- The pretrain
+00000ea0: 6564 206d 6f64 656c 205b 5061 7261 666f  ed model [Parafo
+00000eb0: 726d 6572 2d6c 6172 6765 5d28 6874 7470  rmer-large](http
+00000ec0: 733a 2f2f 7777 772e 6d6f 6465 6c73 636f  s://www.modelsco
+00000ed0: 7065 2e63 6e2f 6d6f 6465 6c73 2f64 616d  pe.cn/models/dam
+00000ee0: 6f2f 7370 6565 6368 5f70 6172 6166 6f72  o/speech_parafor
+00000ef0: 6d65 722d 6c61 7267 655f 6173 725f 6e61  mer-large_asr_na
+00000f00: 742d 7a68 2d63 6e2d 3136 6b2d 636f 6d6d  t-zh-cn-16k-comm
+00000f10: 6f6e 2d76 6f63 6162 3834 3034 2d70 7974  on-vocab8404-pyt
+00000f20: 6f72 6368 2f73 756d 6d61 7279 2920 6f62  orch/summary) ob
+00000f30: 7461 696e 7320 7468 6520 6265 7374 2070  tains the best p
+00000f40: 6572 666f 726d 616e 6365 206f 6e20 6d61  erformance on ma
+00000f50: 6e79 2074 6173 6b73 2069 6e20 5b53 7065  ny tasks in [Spe
+00000f60: 6563 6849 4f20 6c65 6164 6572 626f 6172  echIO leaderboar
+00000f70: 645d 2868 7474 7073 3a2f 2f67 6974 6875  d](https://githu
+00000f80: 622e 636f 6d2f 5370 6565 6368 436f 6c61  b.com/SpeechCola
+00000f90: 622f 4c65 6164 6572 626f 6172 6429 0a2d  b/Leaderboard).-
+00000fa0: 2046 756e 4153 5220 7375 7070 6c69 6573   FunASR supplies
+00000fb0: 2061 2065 6173 792d 746f 2d75 7365 2070   a easy-to-use p
+00000fc0: 6970 656c 696e 6520 746f 2066 696e 6574  ipeline to finet
+00000fd0: 756e 6520 7072 6574 7261 696e 6564 206d  une pretrained m
+00000fe0: 6f64 656c 7320 6672 6f6d 205b 4d6f 6465  odels from [Mode
+00000ff0: 6c53 636f 7065 5d28 6874 7470 733a 2f2f  lScope](https://
+00001000: 7777 772e 6d6f 6465 6c73 636f 7065 2e63  www.modelscope.c
+00001010: 6e2f 6d6f 6465 6c73 3f70 6167 653d 3126  n/models?page=1&
+00001020: 7461 736b 733d 6175 746f 2d73 7065 6563  tasks=auto-speec
+00001030: 682d 7265 636f 676e 6974 696f 6e29 0a2d  h-recognition).-
+00001040: 2043 6f6d 7061 7265 6420 746f 205b 4573   Compared to [Es
+00001050: 706e 6574 5d28 6874 7470 733a 2f2f 6769  pnet](https://gi
+00001060: 7468 7562 2e63 6f6d 2f65 7370 6e65 742f  thub.com/espnet/
+00001070: 6573 706e 6574 2920 6672 616d 6577 6f72  espnet) framewor
+00001080: 6b2c 2074 6865 2074 7261 696e 696e 6720  k, the training 
+00001090: 7370 6565 6420 6f66 206c 6172 6765 2d73  speed of large-s
+000010a0: 6361 6c65 2064 6174 6173 6574 7320 696e  cale datasets in
+000010b0: 2046 756e 4153 5220 6973 206d 7563 6820   FunASR is much 
+000010c0: 6661 7374 6572 206f 776e 696e 6720 746f  faster owning to
+000010d0: 2074 6865 206f 7074 696d 697a 6564 2064   the optimized d
+000010e0: 6174 616c 6f61 6465 722e 0a0a 2323 2049  ataloader...## I
+000010f0: 6e73 7461 6c6c 6174 696f 6e0a 0a49 6e73  nstallation..Ins
+00001100: 7461 6c6c 2066 726f 6d20 7069 700a 6060  tall from pip.``
+00001110: 6073 6865 6c6c 0a70 6970 2069 6e73 7461  `shell.pip insta
+00001120: 6c6c 202d 5520 6675 6e61 7372 0a23 2046  ll -U funasr.# F
+00001130: 6f72 2074 6865 2075 7365 7273 2069 6e20  or the users in 
+00001140: 4368 696e 612c 2079 6f75 2063 6f75 6c64  China, you could
+00001150: 2069 6e73 7461 6c6c 2077 6974 6820 7468   install with th
+00001160: 6520 636f 6d6d 616e 643a 0a23 2070 6970  e command:.# pip
+00001170: 2069 6e73 7461 6c6c 202d 5520 6675 6e61   install -U funa
+00001180: 7372 202d 6920 6874 7470 733a 2f2f 6d69  sr -i https://mi
+00001190: 7272 6f72 2e73 6a74 752e 6564 752e 636e  rror.sjtu.edu.cn
+000011a0: 2f70 7970 692f 7765 622f 7369 6d70 6c65  /pypi/web/simple
+000011b0: 0a60 6060 0a0a 4f72 2069 6e73 7461 6c6c  .```..Or install
+000011c0: 2066 726f 6d20 736f 7572 6365 2063 6f64   from source cod
+000011d0: 650a 0a0a 6060 6020 7368 0a67 6974 2063  e...``` sh.git c
+000011e0: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+000011f0: 6875 622e 636f 6d2f 616c 6962 6162 612f  hub.com/alibaba/
+00001200: 4675 6e41 5352 2e67 6974 2026 2620 6364  FunASR.git && cd
+00001210: 2046 756e 4153 520a 7069 7020 696e 7374   FunASR.pip inst
+00001220: 616c 6c20 2d65 202e 2f0a 2320 466f 7220  all -e ./.# For 
+00001230: 7468 6520 7573 6572 7320 696e 2043 6869  the users in Chi
+00001240: 6e61 2c20 796f 7520 636f 756c 6420 696e  na, you could in
+00001250: 7374 616c 6c20 7769 7468 2074 6865 2063  stall with the c
+00001260: 6f6d 6d61 6e64 3a0a 2320 7069 7020 696e  ommand:.# pip in
+00001270: 7374 616c 6c20 2d65 202e 2f20 2d69 2068  stall -e ./ -i h
+00001280: 7474 7073 3a2f 2f6d 6972 726f 722e 736a  ttps://mirror.sj
+00001290: 7475 2e65 6475 2e63 6e2f 7079 7069 2f77  tu.edu.cn/pypi/w
+000012a0: 6562 2f73 696d 706c 650a 0a60 6060 0a49  eb/simple..```.I
+000012b0: 6620 796f 7520 7761 6e74 2074 6f20 7573  f you want to us
+000012c0: 6520 7468 6520 7072 6574 7261 696e 6564  e the pretrained
+000012d0: 206d 6f64 656c 7320 696e 204d 6f64 656c   models in Model
+000012e0: 5363 6f70 652c 2079 6f75 2073 686f 756c  Scope, you shoul
+000012f0: 6420 696e 7374 616c 6c20 7468 6520 6d6f  d install the mo
+00001300: 6465 6c73 636f 7065 3a0a 0a60 6060 7368  delscope:..```sh
+00001310: 656c 6c0a 7069 7020 696e 7374 616c 6c20  ell.pip install 
+00001320: 2d55 206d 6f64 656c 7363 6f70 650a 2320  -U modelscope.# 
+00001330: 466f 7220 7468 6520 7573 6572 7320 696e  For the users in
+00001340: 2043 6869 6e61 2c20 796f 7520 636f 756c   China, you coul
+00001350: 6420 696e 7374 616c 6c20 7769 7468 2074  d install with t
+00001360: 6865 2063 6f6d 6d61 6e64 3a0a 2320 7069  he command:.# pi
+00001370: 7020 696e 7374 616c 6c20 2d55 206d 6f64  p install -U mod
+00001380: 656c 7363 6f70 6520 2d66 2068 7474 7073  elscope -f https
+00001390: 3a2f 2f6d 6f64 656c 7363 6f70 652e 6f73  ://modelscope.os
+000013a0: 732d 636e 2d62 6569 6a69 6e67 2e61 6c69  s-cn-beijing.ali
+000013b0: 7975 6e63 732e 636f 6d2f 7265 6c65 6173  yuncs.com/releas
+000013c0: 6573 2f72 6570 6f2e 6874 6d6c 202d 6920  es/repo.html -i 
+000013d0: 6874 7470 733a 2f2f 6d69 7272 6f72 2e73  https://mirror.s
+000013e0: 6a74 752e 6564 752e 636e 2f70 7970 692f  jtu.edu.cn/pypi/
+000013f0: 7765 622f 7369 6d70 6c65 0a60 6060 0a0a  web/simple.```..
+00001400: 466f 7220 6d6f 7265 2064 6574 6169 6c73  For more details
+00001410: 2c20 706c 6561 7365 2072 6566 2074 6f20  , please ref to 
+00001420: 5b69 6e73 7461 6c6c 6174 696f 6e5d 2868  [installation](h
+00001430: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001440: 6d2f 616c 6962 6162 612d 6461 6d6f 2d61  m/alibaba-damo-a
+00001450: 6361 6465 6d79 2f46 756e 4153 522f 7769  cademy/FunASR/wi
+00001460: 6b69 290a 0a5b 2f2f 5d3a 2023 2028 290a  ki)..[//]: # ().
+00001470: 5b2f 2f5d 3a20 2320 2823 2320 5573 6167  [//]: # (## Usag
+00001480: 6529 0a0a 5b2f 2f5d 3a20 2320 2846 6f72  e)..[//]: # (For
+00001490: 2075 7365 7273 2077 686f 2061 7265 206e   users who are n
+000014a0: 6577 2074 6f20 4675 6e41 5352 2061 6e64  ew to FunASR and
+000014b0: 204d 6f64 656c 5363 6f70 652c 2070 6c65   ModelScope, ple
+000014c0: 6173 6520 7265 6665 7220 746f 2046 756e  ase refer to Fun
+000014d0: 4153 5220 446f 6373 2623 3430 3b5b 434e  ASR Docs&#40;[CN
+000014e0: 5d26 2334 303b 6874 7470 733a 2f2f 616c  ]&#40;https://al
+000014f0: 6962 6162 612d 6461 6d6f 2d61 6361 6465  ibaba-damo-acade
+00001500: 6d79 2e67 6974 6875 622e 696f 2f46 756e  my.github.io/Fun
+00001510: 4153 522f 636e 2f69 6e64 6578 2e68 746d  ASR/cn/index.htm
+00001520: 6c26 2334 313b 202f 205b 454e 5d26 2334  l&#41; / [EN]&#4
+00001530: 303b 6874 7470 733a 2f2f 616c 6962 6162  0;https://alibab
+00001540: 612d 6461 6d6f 2d61 6361 6465 6d79 2e67  a-damo-academy.g
+00001550: 6974 6875 622e 696f 2f46 756e 4153 522f  ithub.io/FunASR/
+00001560: 656e 2f69 6e64 6578 2e68 746d 6c26 2334  en/index.html&#4
+00001570: 313b 2623 3431 3b29 0a0a 2323 2043 6f6e  1;&#41;)..## Con
+00001580: 7461 6374 0a0a 4966 2079 6f75 2068 6176  tact..If you hav
+00001590: 6520 616e 7920 7175 6573 7469 6f6e 7320  e any questions 
+000015a0: 6162 6f75 7420 4675 6e41 5352 2c20 706c  about FunASR, pl
+000015b0: 6561 7365 2063 6f6e 7461 6374 2075 7320  ease contact us 
+000015c0: 6279 0a0a 2d20 656d 6169 6c3a 205b 6675  by..- email: [fu
+000015d0: 6e61 7372 406c 6973 742e 616c 6962 6162  nasr@list.alibab
+000015e0: 612d 696e 632e 636f 6d5d 2866 756e 6173  a-inc.com](funas
+000015f0: 7240 6c69 7374 2e61 6c69 6261 6261 2d69  r@list.alibaba-i
+00001600: 6e63 2e63 6f6d 290a 0a7c 4469 6e67 6469  nc.com)..|Dingdi
+00001610: 6e67 2067 726f 7570 207c 2020 2020 2020  ng group |      
+00001620: 2020 2020 2020 2020 2020 2020 2020 2057                 W
+00001630: 6563 6861 7420 6772 6f75 7020 2020 2020  echat group     
+00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001650: 207c 0a7c 3a2d 2d2d 3a7c 3a2d 2d2d 2d2d   |.|:---:|:-----
+00001660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001690: 3a7c 0a7c 3c64 6976 2061 6c69 676e 3d22  :|.|<div align="
+000016a0: 6c65 6674 223e 3c69 6d67 2073 7263 3d22  left"><img src="
+000016b0: 646f 6373 2f69 6d61 6765 732f 6469 6e67  docs/images/ding
+000016c0: 6469 6e67 2e6a 7067 2220 7769 6474 683d  ding.jpg" width=
+000016d0: 2232 3530 222f 3e20 7c20 3c69 6d67 2073  "250"/> | <img s
+000016e0: 7263 3d22 646f 6373 2f69 6d61 6765 732f  rc="docs/images/
+000016f0: 7765 6368 6174 2e70 6e67 2220 7769 6474  wechat.png" widt
+00001700: 683d 2232 3332 222f 3e3c 2f64 6976 3e20  h="232"/></div> 
+00001710: 7c0a 0a23 2320 436f 6e74 7269 6275 746f  |..## Contributo
+00001720: 7273 0a0a 7c20 3c64 6976 2061 6c69 676e  rs..| <div align
+00001730: 3d22 6c65 6674 223e 3c69 6d67 2073 7263  ="left"><img src
+00001740: 3d22 646f 6373 2f69 6d61 6765 732f 6461  ="docs/images/da
+00001750: 6d6f 2e70 6e67 2220 7769 6474 683d 2231  mo.png" width="1
+00001760: 3830 222f 3e20 7c20 3c64 6976 2061 6c69  80"/> | <div ali
+00001770: 676e 3d22 6c65 6674 223e 3c69 6d67 2073  gn="left"><img s
+00001780: 7263 3d22 646f 6373 2f69 6d61 6765 732f  rc="docs/images/
+00001790: 6e77 7075 2e70 6e67 2220 7769 6474 683d  nwpu.png" width=
+000017a0: 2232 3630 222f 3e20 7c20 3c69 6d67 2073  "260"/> | <img s
+000017b0: 7263 3d22 646f 6373 2f69 6d61 6765 732f  rc="docs/images/
+000017c0: 4465 6570 5363 6965 6e63 652e 706e 6722  DeepScience.png"
+000017d0: 2077 6964 7468 3d22 3230 3022 2f3e 203c   width="200"/> <
+000017e0: 2f64 6976 3e20 7c0a 7c3a 2d2d 2d2d 2d2d  /div> |.|:------
+000017f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001820: 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d  ---------:|:----
+00001830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  -----------:|:--
+00001870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000018a0: 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a 0a23 2320  ---------:|..## 
+000018b0: 4163 6b6e 6f77 6c65 6467 650a 0a31 2e20  Acknowledge..1. 
+000018c0: 5765 2062 6f72 726f 7765 6420 6120 6c6f  We borrowed a lo
+000018d0: 7420 6f66 2063 6f64 6520 6672 6f6d 205b  t of code from [
+000018e0: 4b61 6c64 695d 2868 7474 703a 2f2f 6b61  Kaldi](http://ka
+000018f0: 6c64 692d 6173 722e 6f72 672f 2920 666f  ldi-asr.org/) fo
+00001900: 7220 6461 7461 2070 7265 7061 7261 7469  r data preparati
+00001910: 6f6e 2e0a 322e 2057 6520 626f 7272 6f77  on..2. We borrow
+00001920: 6564 2061 206c 6f74 206f 6620 636f 6465  ed a lot of code
+00001930: 2066 726f 6d20 5b45 5350 6e65 745d 2868   from [ESPnet](h
+00001940: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001950: 6d2f 6573 706e 6574 2f65 7370 6e65 7429  m/espnet/espnet)
+00001960: 2e20 4675 6e41 5352 2066 6f6c 6c6f 7773  . FunASR follows
+00001970: 2075 7020 7468 6520 7472 6169 6e69 6e67   up the training
+00001980: 2061 6e64 2066 696e 6574 756e 696e 6720   and finetuning 
+00001990: 7069 7065 6c69 6e65 7320 6f66 2045 5350  pipelines of ESP
+000019a0: 6e65 742e 0a33 2e20 5765 2072 6566 6572  net..3. We refer
+000019b0: 7265 6420 5b57 656e 6574 5d28 6874 7470  red [Wenet](http
+000019c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f77  s://github.com/w
+000019d0: 656e 6574 2d65 3265 2f77 656e 6574 2920  enet-e2e/wenet) 
+000019e0: 666f 7220 6275 696c 6469 6e67 2064 6174  for building dat
+000019f0: 616c 6f61 6465 7220 666f 7220 6c61 7267  aloader for larg
+00001a00: 6520 7363 616c 6520 6461 7461 2074 7261  e scale data tra
+00001a10: 696e 696e 672e 0a34 2e20 5765 2061 636b  ining..4. We ack
+00001a20: 6e6f 776c 6564 6765 205b 4465 6570 5363  nowledge [DeepSc
+00001a30: 6965 6e63 655d 2868 7474 7073 3a2f 2f77  ience](https://w
+00001a40: 7777 2e64 6565 7073 6369 656e 6365 2e63  ww.deepscience.c
+00001a50: 6e29 2066 6f72 2063 6f6e 7472 6962 7574  n) for contribut
+00001a60: 696e 6720 7468 6520 6772 7063 2073 6572  ing the grpc ser
+00001a70: 7669 6365 2e0a 0a23 2320 4c69 6365 6e73  vice...## Licens
+00001a80: 650a 5468 6973 2070 726f 6a65 6374 2069  e.This project i
+00001a90: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
+00001aa0: 2074 6865 205b 5468 6520 4d49 5420 4c69   the [The MIT Li
+00001ab0: 6365 6e73 655d 2868 7474 7073 3a2f 2f6f  cense](https://o
+00001ac0: 7065 6e73 6f75 7263 652e 6f72 672f 6c69  pensource.org/li
+00001ad0: 6365 6e73 6573 2f4d 4954 292e 2046 756e  censes/MIT). Fun
+00001ae0: 4153 5220 616c 736f 2063 6f6e 7461 696e  ASR also contain
+00001af0: 7320 7661 7269 6f75 7320 7468 6972 642d  s various third-
+00001b00: 7061 7274 7920 636f 6d70 6f6e 656e 7473  party components
+00001b10: 2061 6e64 2073 6f6d 6520 636f 6465 206d   and some code m
+00001b20: 6f64 6966 6965 6420 6672 6f6d 206f 7468  odified from oth
+00001b30: 6572 2072 6570 6f73 2075 6e64 6572 206f  er repos under o
+00001b40: 7468 6572 206f 7065 6e20 736f 7572 6365  ther open source
+00001b50: 206c 6963 656e 7365 732e 0a0a 2323 2043   licenses...## C
+00001b60: 6974 6174 696f 6e73 0a0a 6060 6020 6269  itations..``` bi
+00001b70: 6274 6578 0a40 696e 7072 6f63 6565 6469  btex.@inproceedi
+00001b80: 6e67 737b 6761 6f32 3032 3270 6172 6166  ngs{gao2022paraf
+00001b90: 6f72 6d65 722c 0a20 2074 6974 6c65 3d7b  ormer,.  title={
+00001ba0: 5061 7261 666f 726d 6572 3a20 4661 7374  Paraformer: Fast
+00001bb0: 2061 6e64 2041 6363 7572 6174 6520 5061   and Accurate Pa
+00001bc0: 7261 6c6c 656c 2054 7261 6e73 666f 726d  rallel Transform
+00001bd0: 6572 2066 6f72 204e 6f6e 2d61 7574 6f72  er for Non-autor
+00001be0: 6567 7265 7373 6976 6520 456e 642d 746f  egressive End-to
+00001bf0: 2d45 6e64 2053 7065 6563 6820 5265 636f  -End Speech Reco
+00001c00: 676e 6974 696f 6e7d 2c0a 2020 6175 7468  gnition},.  auth
+00001c10: 6f72 3d7b 4761 6f2c 205a 6869 6675 2061  or={Gao, Zhifu a
+00001c20: 6e64 205a 6861 6e67 2c20 5368 696c 6961  nd Zhang, Shilia
+00001c30: 6e67 2061 6e64 204d 634c 6f75 6768 6c69  ng and McLoughli
+00001c40: 6e2c 2049 616e 2061 6e64 2059 616e 2c20  n, Ian and Yan, 
+00001c50: 5a68 696a 6965 7d2c 0a20 2062 6f6f 6b74  Zhijie},.  bookt
+00001c60: 6974 6c65 3d7b 494e 5445 5253 5045 4543  itle={INTERSPEEC
+00001c70: 487d 2c0a 2020 7965 6172 3d7b 3230 3232  H},.  year={2022
+00001c80: 7d0a 7d0a 4069 6e70 726f 6365 6564 696e  }.}.@inproceedin
+00001c90: 6773 7b67 616f 3230 3230 756e 6976 6572  gs{gao2020univer
+00001ca0: 7361 6c2c 0a20 2074 6974 6c65 3d7b 556e  sal,.  title={Un
+00001cb0: 6976 6572 7361 6c20 4153 523a 2055 6e69  iversal ASR: Uni
+00001cc0: 6679 696e 6720 5374 7265 616d 696e 6720  fying Streaming 
+00001cd0: 616e 6420 4e6f 6e2d 5374 7265 616d 696e  and Non-Streamin
+00001ce0: 6720 4153 5220 5573 696e 6720 6120 5369  g ASR Using a Si
+00001cf0: 6e67 6c65 2045 6e63 6f64 6572 2d44 6563  ngle Encoder-Dec
+00001d00: 6f64 6572 204d 6f64 656c 7d2c 0a20 2061  oder Model},.  a
+00001d10: 7574 686f 723d 7b47 616f 2c20 5a68 6966  uthor={Gao, Zhif
+00001d20: 7520 616e 6420 5a68 616e 672c 2053 6869  u and Zhang, Shi
+00001d30: 6c69 616e 6720 616e 6420 4c65 692c 204d  liang and Lei, M
+00001d40: 696e 6720 616e 6420 4d63 4c6f 7567 686c  ing and McLoughl
+00001d50: 696e 2c20 4961 6e7d 2c0a 2020 626f 6f6b  in, Ian},.  book
+00001d60: 7469 746c 653d 7b61 7258 6976 2070 7265  title={arXiv pre
+00001d70: 7072 696e 7420 6172 5869 763a 3230 3130  print arXiv:2010
+00001d80: 2e31 3430 3939 7d2c 0a20 2079 6561 723d  .14099},.  year=
+00001d90: 7b32 3032 307d 0a7d 0a40 696e 7072 6f63  {2020}.}.@inproc
+00001da0: 6565 6469 6e67 737b 5368 6932 3032 3341  eedings{Shi2023A
+00001db0: 6368 6965 7669 6e67 5450 2c0a 2020 7469  chievingTP,.  ti
+00001dc0: 746c 653d 7b41 6368 6965 7669 6e67 2054  tle={Achieving T
+00001dd0: 696d 6573 7461 6d70 2050 7265 6469 6374  imestamp Predict
+00001de0: 696f 6e20 5768 696c 6520 5265 636f 676e  ion While Recogn
+00001df0: 697a 696e 6720 7769 7468 204e 6f6e 2d41  izing with Non-A
+00001e00: 7574 6f72 6567 7265 7373 6976 6520 456e  utoregressive En
+00001e10: 642d 746f 2d45 6e64 2041 5352 204d 6f64  d-to-End ASR Mod
+00001e20: 656c 7d2c 0a20 2061 7574 686f 723d 7b58  el},.  author={X
+00001e30: 6961 6e20 5368 6920 616e 6420 5961 6e6e  ian Shi and Yann
+00001e40: 6920 4368 656e 2061 6e64 2053 6869 6c69  i Chen and Shili
+00001e50: 616e 6720 5a68 616e 6720 616e 6420 5a68  ang Zhang and Zh
+00001e60: 696a 6965 2059 616e 7d2c 0a20 2062 6f6f  ijie Yan},.  boo
+00001e70: 6b74 6974 6c65 3d7b 6172 5869 7620 7072  ktitle={arXiv pr
+00001e80: 6570 7269 6e74 2061 7258 6976 3a32 3330  eprint arXiv:230
+00001e90: 312e 3132 3334 337d 0a20 2079 6561 723d  1.12343}.  year=
+00001ea0: 7b32 3032 337d 0a7d 0a60 6060 0a0a 0a    {2023}.}.```...
```

### Comparing `funasr-0.4.1/funasr.egg-info/SOURCES.txt` & `funasr-0.4.2/funasr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 funasr/bin/asr_inference_paraformer_vad.py
 funasr/bin/asr_inference_paraformer_vad_punc.py
 funasr/bin/asr_inference_rnnt.py
 funasr/bin/asr_inference_uniasr.py
 funasr/bin/asr_inference_uniasr_vad.py
 funasr/bin/asr_train.py
 funasr/bin/asr_train_paraformer.py
+funasr/bin/asr_train_transducer.py
 funasr/bin/asr_train_uniasr.py
 funasr/bin/build_trainer.py
 funasr/bin/data2vec_train.py
 funasr/bin/diar_inference_launch.py
 funasr/bin/diar_train.py
 funasr/bin/eend_ola_inference.py
 funasr/bin/lm_calc_perplexity.py
@@ -139,26 +140,28 @@
 funasr/models/__init__.py
 funasr/models/ctc.py
 funasr/models/data2vec.py
 funasr/models/e2e_asr.py
 funasr/models/e2e_asr_common.py
 funasr/models/e2e_asr_mfcca.py
 funasr/models/e2e_asr_paraformer.py
+funasr/models/e2e_asr_transducer.py
 funasr/models/e2e_diar_eend_ola.py
 funasr/models/e2e_diar_sond.py
 funasr/models/e2e_sv.py
 funasr/models/e2e_tp.py
 funasr/models/e2e_uni_asr.py
 funasr/models/e2e_vad.py
 funasr/models/target_delay_transformer.py
 funasr/models/vad_realtime_transformer.py
 funasr/models/decoder/__init__.py
 funasr/models/decoder/abs_decoder.py
 funasr/models/decoder/contextual_decoder.py
 funasr/models/decoder/rnn_decoder.py
+funasr/models/decoder/rnnt_decoder.py
 funasr/models/decoder/sanm_decoder.py
 funasr/models/decoder/sv_decoder.py
 funasr/models/decoder/transformer_decoder.py
 funasr/models/encoder/__init__.py
 funasr/models/encoder/abs_encoder.py
 funasr/models/encoder/conformer_encoder.py
 funasr/models/encoder/data2vec_encoder.py
@@ -180,14 +183,16 @@
 funasr/models/frontend/default.py
 funasr/models/frontend/eend_ola_feature.py
 funasr/models/frontend/fused.py
 funasr/models/frontend/s3prl.py
 funasr/models/frontend/wav_frontend.py
 funasr/models/frontend/wav_frontend_kaldifeat.py
 funasr/models/frontend/windowing.py
+funasr/models/joint_net/__init__.py
+funasr/models/joint_net/joint_network.py
 funasr/models/pooling/__init__.py
 funasr/models/pooling/statistic_pooling.py
 funasr/models/postencoder/__init__.py
 funasr/models/postencoder/abs_postencoder.py
 funasr/models/postencoder/hugging_face_transformers_postencoder.py
 funasr/models/predictor/__init__.py
 funasr/models/predictor/cif.py
@@ -215,14 +220,15 @@
 funasr/modules/repeat.py
 funasr/modules/subsampling.py
 funasr/modules/subsampling_without_posenc.py
 funasr/modules/beam_search/__init__.py
 funasr/modules/beam_search/batch_beam_search.py
 funasr/modules/beam_search/batch_beam_search_online_sim.py
 funasr/modules/beam_search/beam_search.py
+funasr/modules/beam_search/beam_search_transducer.py
 funasr/modules/data2vec/__init__.py
 funasr/modules/data2vec/data_utils.py
 funasr/modules/data2vec/ema_module.py
 funasr/modules/data2vec/grad_multiply.py
 funasr/modules/data2vec/multihead_attention.py
 funasr/modules/data2vec/quant_noise.py
 funasr/modules/data2vec/utils.py
@@ -358,19 +364,13 @@
 funasr/utils/sized_dict.py
 funasr/utils/timestamp_tools.py
 funasr/utils/types.py
 funasr/utils/wav_utils.py
 funasr/utils/yaml_no_alias_safe_dump.py
 test/test_moddelscope_punc.py
 test/test_moddelscope_punc_online.py
+test/test_modelscope_paraformer_large.py
 test/test_modelscope_paraformer_long.py
 test/test_modelscope_pipeline.py
 test/test_modelscope_vad.py
 test/test_onnx_encoder.py
-test/test_rtf.py
-tests/test_asr_inference_pipeline.py
-tests/test_asr_vad_punc_inference_pipeline.py
-tests/test_inference_pipeline.py
-tests/test_lm_pipeline.py
-tests/test_punctuation_pipeline.py
-tests/test_sv_inference_pipeline.py
-tests/test_vad_inference_pipeline.py
+test/test_rtf.py
```

### Comparing `funasr-0.4.1/funasr.egg-info/requires.txt` & `funasr-0.4.2/funasr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/setup.py` & `funasr-0.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 version_file = os.path.join(dirname, "funasr", "version.txt")
 with open(version_file, "r") as f:
     version = f.read().strip()
 setup(
     name="funasr",
     version=version,
     url="https://github.com/alibaba-damo-academy/FunASR.git",
-    author="Speech Lab, Alibaba Group, China",
+    author="Speech Lab of DAMO Academy, Alibaba Group",
     author_email="funasr@list.alibaba-inc.com",
     description="FunASR: A Fundamental End-to-End Speech Recognition Toolkit",
     long_description=open(os.path.join(dirname, "README.md"), encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     license="The MIT License",
     packages=find_packages(include=["funasr*"]),
     package_data={"funasr": ["version.txt"]},
```

### Comparing `funasr-0.4.1/test/test_moddelscope_punc_online.py` & `funasr-0.4.2/test/test_moddelscope_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/test/test_modelscope_paraformer_long.py` & `funasr-0.4.2/test/test_modelscope_paraformer_long.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/test/test_modelscope_pipeline.py` & `funasr-0.4.2/test/test_modelscope_pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,11 +7,12 @@
     audio_in="/home/gzf/video.wav"
     output_dir = None
     inference_pipeline = pipeline(
         task=Tasks.auto_speech_recognition,
         model='damo/speech_paraformer-large-vad-punc_asr_nat-zh-cn-16k-common-vocab8404-pytorch',
         #vad_model='damo/speech_fsmn_vad_zh-cn-16k-common-pytorch',
         #punc_model='damo/punc_ct-transformer_zh-cn-common-vocab272727-pytorch',
-        ngpu=1,
+        ngpu=0,
+        ncpu=8,
     )
     rec_result = inference_pipeline(audio_in=audio_in)
     print(rec_result)
```

### Comparing `funasr-0.4.1/test/test_modelscope_vad.py` & `funasr-0.4.2/test/test_modelscope_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/test/test_onnx_encoder.py` & `funasr-0.4.2/test/test_onnx_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.1/test/test_rtf.py` & `funasr-0.4.2/test/test_rtf.py`

 * *Files identical despite different names*

