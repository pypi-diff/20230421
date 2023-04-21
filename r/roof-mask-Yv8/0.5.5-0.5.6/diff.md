# Comparing `tmp/roof_mask_Yv8-0.5.5.tar.gz` & `tmp/roof_mask_Yv8-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roof_mask_Yv8-0.5.5.tar", last modified: Thu Apr 20 18:48:17 2023, max compression
+gzip compressed data, was "roof_mask_Yv8-0.5.6.tar", last modified: Thu Apr 20 20:41:21 2023, max compression
```

## Comparing `roof_mask_Yv8-0.5.5.tar` & `roof_mask_Yv8-0.5.6.tar`

### file list

```diff
@@ -1,273 +1,301 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:39.270524 roof_mask_Yv8-0.5.5/
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-20 18:44:18.000000 roof_mask_Yv8-0.5.5/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      426 2023-04-20 18:48:17.132324 roof_mask_Yv8-0.5.5/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:39.549364 roof_mask_Yv8-0.5.5/detectron2/
--rwxrwxrwx   0 root         (0) root         (0)      258 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:39.624321 roof_mask_Yv8-0.5.5/detectron2/checkpoint/
--rwxrwxrwx   0 root         (0) root         (0)      347 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/checkpoint/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    17782 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/checkpoint/c2_model_loading.py
--rwxrwxrwx   0 root         (0) root         (0)     5685 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/checkpoint/catalog.py
--rwxrwxrwx   0 root         (0) root         (0)     5258 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/checkpoint/detection_checkpoint.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:39.692281 roof_mask_Yv8-0.5.5/detectron2/config/
--rwxrwxrwx   0 root         (0) root         (0)      599 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/config/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7890 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/config/compat.py
--rwxrwxrwx   0 root         (0) root         (0)     9211 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/config/config.py
--rwxrwxrwx   0 root         (0) root         (0)    29512 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/config/defaults.py
--rwxrwxrwx   0 root         (0) root         (0)     2719 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/config/instantiate.py
--rwxrwxrwx   0 root         (0) root         (0)    14944 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/config/lazy.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:39.759242 roof_mask_Yv8-0.5.5/detectron2/data/
--rwxrwxrwx   0 root         (0) root         (0)      644 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7378 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/data/benchmark.py
--rwxrwxrwx   0 root         (0) root         (0)    20605 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/data/build.py
--rwxrwxrwx   0 root         (0) root         (0)     7224 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/data/catalog.py
--rwxrwxrwx   0 root         (0) root         (0)     9164 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/data/common.py
--rwxrwxrwx   0 root         (0) root         (0)     8169 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.5/detectron2/data/dataset_mapper.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:39.821206 roof_mask_Yv8-0.5.5/detectron2/data/datasets/
--rwxrwxrwx   0 root         (0) root         (0)      523 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/datasets/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10174 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/datasets/builtin.py
--rwxrwxrwx   0 root         (0) root         (0)    21841 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/datasets/builtin_meta.py
--rwxrwxrwx   0 root         (0) root         (0)    13167 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/datasets/cityscapes.py
--rwxrwxrwx   0 root         (0) root         (0)     7821 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/datasets/cityscapes_panoptic.py
--rwxrwxrwx   0 root         (0) root         (0)    23465 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/datasets/coco.py
--rwxrwxrwx   0 root         (0) root         (0)     8977 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/datasets/coco_panoptic.py
--rwxrwxrwx   0 root         (0) root         (0)     9623 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/datasets/lvis.py
--rwxrwxrwx   0 root         (0) root         (0)   223757 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/datasets/lvis_v0_5_categories.py
--rwxrwxrwx   0 root         (0) root         (0)   219177 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/datasets/lvis_v1_categories.py
--rwxrwxrwx   0 root         (0) root         (0)    39414 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/datasets/lvis_v1_category_image_count.py
--rwxrwxrwx   0 root         (0) root         (0)     3128 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/datasets/pascal_voc.py
--rwxrwxrwx   0 root         (0) root         (0)      169 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/datasets/register_coco.py
--rwxrwxrwx   0 root         (0) root         (0)    22841 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/detection_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:39.912154 roof_mask_Yv8-0.5.5/detectron2/data/samplers/
--rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/samplers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11789 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/samplers/distributed_sampler.py
--rwxrwxrwx   0 root         (0) root         (0)     1944 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/samplers/grouped_batch_sampler.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:39.988110 roof_mask_Yv8-0.5.5/detectron2/data/transforms/
--rwxrwxrwx   0 root         (0) root         (0)      466 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/transforms/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14117 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/transforms/augmentation.py
--rwxrwxrwx   0 root         (0) root         (0)    23069 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/transforms/augmentation_impl.py
--rwxrwxrwx   0 root         (0) root         (0)    12629 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/data/transforms/transform.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.038081 roof_mask_Yv8-0.5.5/detectron2/engine/
--rwxrwxrwx   0 root         (0) root         (0)      340 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/engine/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    26868 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/engine/defaults.py
--rwxrwxrwx   0 root         (0) root         (0)    25497 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/engine/hooks.py
--rwxrwxrwx   0 root         (0) root         (0)     4089 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/engine/launch.py
--rwxrwxrwx   0 root         (0) root         (0)    14104 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/engine/train_loop.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.116036 roof_mask_Yv8-0.5.5/detectron2/evaluation/
--rwxrwxrwx   0 root         (0) root         (0)      671 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/evaluation/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8369 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/evaluation/cityscapes_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)    30423 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/evaluation/coco_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     8156 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.5/detectron2/evaluation/evaluator.py
--rwxrwxrwx   0 root         (0) root         (0)     5078 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/evaluation/fast_eval_api.py
--rwxrwxrwx   0 root         (0) root         (0)    15018 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/evaluation/lvis_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     7500 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/evaluation/panoptic_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)    10862 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/evaluation/pascal_voc_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     7608 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/evaluation/rotated_coco_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     8191 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/evaluation/sem_seg_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     2614 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/evaluation/testing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.184997 roof_mask_Yv8-0.5.5/detectron2/export/
--rwxrwxrwx   0 root         (0) root         (0)      336 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9280 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/export/api.py
--rwxrwxrwx   0 root         (0) root         (0)    21035 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/export/c10.py
--rwxrwxrwx   0 root         (0) root         (0)     7803 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/export/caffe2_export.py
--rwxrwxrwx   0 root         (0) root         (0)     6674 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/export/caffe2_inference.py
--rwxrwxrwx   0 root         (0) root         (0)    17034 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/export/caffe2_modeling.py
--rwxrwxrwx   0 root         (0) root         (0)     5033 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/export/caffe2_patch.py
--rwxrwxrwx   0 root         (0) root         (0)    11807 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/export/flatten.py
--rwxrwxrwx   0 root         (0) root         (0)    38071 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/export/shared.py
--rwxrwxrwx   0 root         (0) root         (0)     5008 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/export/torchscript.py
--rwxrwxrwx   0 root         (0) root         (0)    11526 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/export/torchscript_patch.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.250958 roof_mask_Yv8-0.5.5/detectron2/layers/
--rwxrwxrwx   0 root         (0) root         (0)      839 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/layers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5764 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/layers/aspp.py
--rwxrwxrwx   0 root         (0) root         (0)    12131 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/layers/batch_norm.py
--rwxrwxrwx   0 root         (0) root         (0)     3024 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.5/detectron2/layers/blocks.py
--rwxrwxrwx   0 root         (0) root         (0)    16978 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/layers/deform_conv.py
--rwxrwxrwx   0 root         (0) root         (0)     4204 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/layers/losses.py
--rwxrwxrwx   0 root         (0) root         (0)    10881 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/layers/mask_ops.py
--rwxrwxrwx   0 root         (0) root         (0)     6490 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/layers/nms.py
--rwxrwxrwx   0 root         (0) root         (0)     3098 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/layers/roi_align.py
--rwxrwxrwx   0 root         (0) root         (0)     3302 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/layers/roi_align_rotated.py
--rwxrwxrwx   0 root         (0) root         (0)      652 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/layers/rotated_boxes.py
--rwxrwxrwx   0 root         (0) root         (0)      661 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/layers/shape_spec.py
--rwxrwxrwx   0 root         (0) root         (0)     4893 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/layers/wrappers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.318919 roof_mask_Yv8-0.5.5/detectron2/modeling/
--rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    15443 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/anchor_generator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.390878 roof_mask_Yv8-0.5.5/detectron2/modeling/backbone/
--rwxrwxrwx   0 root         (0) root         (0)      475 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/backbone/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1543 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/backbone/backbone.py
--rwxrwxrwx   0 root         (0) root         (0)     1015 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/backbone/build.py
--rwxrwxrwx   0 root         (0) root         (0)    10055 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/backbone/fpn.py
--rwxrwxrwx   0 root         (0) root         (0)    16656 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/backbone/regnet.py
--rwxrwxrwx   0 root         (0) root         (0)    23658 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/backbone/resnet.py
--rwxrwxrwx   0 root         (0) root         (0)    15123 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/box_regression.py
--rwxrwxrwx   0 root         (0) root         (0)     6264 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/matcher.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.445845 roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/
--rwxrwxrwx   0 root         (0) root         (0)      508 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      814 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/build.py
--rwxrwxrwx   0 root         (0) root         (0)    11550 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/dense_detector.py
--rwxrwxrwx   0 root         (0) root         (0)    13213 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/fcos.py
--rwxrwxrwx   0 root         (0) root         (0)    10335 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/panoptic_fpn.py
--rwxrwxrwx   0 root         (0) root         (0)    13710 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    18265 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/retinanet.py
--rwxrwxrwx   0 root         (0) root         (0)     9720 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/semantic_seg.py
--rwxrwxrwx   0 root         (0) root         (0)    10832 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/mmdet_wrapper.py
--rwxrwxrwx   0 root         (0) root         (0)    11316 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/poolers.py
--rwxrwxrwx   0 root         (0) root         (0)     4046 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/postprocessing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.500815 roof_mask_Yv8-0.5.5/detectron2/modeling/proposal_generator/
--rwxrwxrwx   0 root         (0) root         (0)      231 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/proposal_generator/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      836 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/proposal_generator/build.py
--rwxrwxrwx   0 root         (0) root         (0)     8128 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/proposal_generator/proposal_utils.py
--rwxrwxrwx   0 root         (0) root         (0)    23814 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/proposal_generator/rpn.py
--rwxrwxrwx   0 root         (0) root         (0)     8807 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/proposal_generator/rrpn.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.559780 roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/
--rwxrwxrwx   0 root         (0) root         (0)      768 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4077 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/box_head.py
--rwxrwxrwx   0 root         (0) root         (0)    12990 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/cascade_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    25274 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/fast_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    11156 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/keypoint_head.py
--rwxrwxrwx   0 root         (0) root         (0)    12169 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/mask_head.py
--rwxrwxrwx   0 root         (0) root         (0)    37701 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/roi_heads.py
--rwxrwxrwx   0 root         (0) root         (0)    11158 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)     2334 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/sampling.py
--rwxrwxrwx   0 root         (0) root         (0)    12416 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/modeling/test_time_augmentation.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.594759 roof_mask_Yv8-0.5.5/detectron2/solver/
--rwxrwxrwx   0 root         (0) root         (0)      298 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/solver/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11127 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/solver/build.py
--rwxrwxrwx   0 root         (0) root         (0)     8648 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.5/detectron2/solver/lr_scheduler.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.716688 roof_mask_Yv8-0.5.5/detectron2/structures/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/detectron2/structures/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14429 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/detectron2/structures/boxes.py
--rwxrwxrwx   0 root         (0) root         (0)     4557 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/detectron2/structures/image_list.py
--rwxrwxrwx   0 root         (0) root         (0)     6542 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/detectron2/structures/instances.py
--rwxrwxrwx   0 root         (0) root         (0)     9030 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/detectron2/structures/keypoints.py
--rwxrwxrwx   0 root         (0) root         (0)    19802 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/detectron2/structures/masks.py
--rwxrwxrwx   0 root         (0) root         (0)    18853 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/detectron2/structures/rotated_boxes.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.825626 roof_mask_Yv8-0.5.5/detectron2/tracking/
--rwxrwxrwx   0 root         (0) root         (0)      580 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/detectron2/tracking/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2216 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/detectron2/tracking/base_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)    11858 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/detectron2/tracking/bbox_iou_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     7486 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/detectron2/tracking/hungarian_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     4142 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     1106 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/detectron2/tracking/utils.py
--rwxrwxrwx   0 root         (0) root         (0)     5288 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.892587 roof_mask_Yv8-0.5.5/detectron2/utils/
--rwxrwxrwx   0 root         (0) root         (0)       51 2023-04-18 18:45:50.000000 roof_mask_Yv8-0.5.5/detectron2/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6017 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.5/detectron2/utils/analysis.py
--rwxrwxrwx   0 root         (0) root         (0)     8391 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.5/detectron2/utils/collect_env.py
--rwxrwxrwx   0 root         (0) root         (0)     4096 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.5/detectron2/utils/colormap.py
--rwxrwxrwx   0 root         (0) root         (0)     5610 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.5/detectron2/utils/comm.py
--rwxrwxrwx   0 root         (0) root         (0)     1838 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.5/detectron2/utils/develop.py
--rwxrwxrwx   0 root         (0) root         (0)     5644 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.5/detectron2/utils/env.py
--rwxrwxrwx   0 root         (0) root         (0)    17024 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.5/detectron2/utils/events.py
--rwxrwxrwx   0 root         (0) root         (0)     1189 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.5/detectron2/utils/file_io.py
--rwxrwxrwx   0 root         (0) root         (0)     7807 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.5/detectron2/utils/logger.py
--rwxrwxrwx   0 root         (0) root         (0)     2583 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.5/detectron2/utils/memory.py
--rwxrwxrwx   0 root         (0) root         (0)     1874 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.5/detectron2/utils/registry.py
--rwxrwxrwx   0 root         (0) root         (0)     1064 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.5/detectron2/utils/serialize.py
--rwxrwxrwx   0 root         (0) root         (0)     4833 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.5/detectron2/utils/testing.py
--rwxrwxrwx   0 root         (0) root         (0)    11319 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.5/detectron2/utils/video_visualizer.py
--rwxrwxrwx   0 root         (0) root         (0)    51159 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.5/detectron2/utils/visualizer.py
--rwxrwxrwx   0 root         (0) root         (0)    52915 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.5/detectron2/utils/visualizer_new.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.930565 roof_mask_Yv8-0.5.5/roof_mask_Yv8.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      426 2023-04-20 18:47:37.000000 roof_mask_Yv8-0.5.5/roof_mask_Yv8.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     8268 2023-04-20 18:47:39.000000 roof_mask_Yv8-0.5.5/roof_mask_Yv8.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-20 18:47:38.000000 roof_mask_Yv8-0.5.5/roof_mask_Yv8.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-20 18:47:38.000000 roof_mask_Yv8-0.5.5/roof_mask_Yv8.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-20 18:48:17.216324 roof_mask_Yv8-0.5.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      601 2023-04-20 18:47:09.000000 roof_mask_Yv8-0.5.5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:40.995527 roof_mask_Yv8-0.5.5/tests/
--rwxrwxrwx   0 root         (0) root         (0)     3211 2023-04-19 15:22:00.000000 roof_mask_Yv8-0.5.5/tests/test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.062489 roof_mask_Yv8-0.5.5/ultralytics/
--rwxrwxrwx   0 root         (0) root         (0)      295 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/ultralytics/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.144442 roof_mask_Yv8-0.5.5/ultralytics/hub/
--rwxrwxrwx   0 root         (0) root         (0)     3421 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/ultralytics/hub/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5206 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/ultralytics/hub/auth.py
--rwxrwxrwx   0 root         (0) root         (0)     8690 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/ultralytics/hub/session.py
--rwxrwxrwx   0 root         (0) root         (0)     9723 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/ultralytics/hub/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.206406 roof_mask_Yv8-0.5.5/ultralytics/nn/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/ultralytics/nn/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    24083 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/ultralytics/nn/autobackend.py
--rwxrwxrwx   0 root         (0) root         (0)    11839 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/ultralytics/nn/autoshape.py
--rwxrwxrwx   0 root         (0) root         (0)    20062 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/ultralytics/nn/modules.py
--rwxrwxrwx   0 root         (0) root         (0)    26619 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/ultralytics/nn/tasks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.275366 roof_mask_Yv8-0.5.5/ultralytics/yolo/
--rwxrwxrwx   0 root         (0) root         (0)       93 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.337330 roof_mask_Yv8-0.5.5/ultralytics/yolo/cfg/
--rwxrwxrwx   0 root         (0) root         (0)    17582 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/cfg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6237 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/cfg/default.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.405291 roof_mask_Yv8-0.5.5/ultralytics/yolo/data/
--rwxrwxrwx   0 root         (0) root         (0)      483 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    31285 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/data/augment.py
--rwxrwxrwx   0 root         (0) root         (0)     8919 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/data/base.py
--rwxrwxrwx   0 root         (0) root         (0)     8614 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/data/build.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.474251 roof_mask_Yv8-0.5.5/ultralytics/yolo/data/dataloaders/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/data/dataloaders/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    15194 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/data/dataloaders/stream_loaders.py
--rwxrwxrwx   0 root         (0) root         (0)    17226 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/data/dataloaders/v5augmentations.py
--rwxrwxrwx   0 root         (0) root         (0)    49861 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/data/dataloaders/v5loader.py
--rwxrwxrwx   0 root         (0) root         (0)    12740 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/data/dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/data/dataset_wrappers.py
--rwxrwxrwx   0 root         (0) root         (0)    22728 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/data/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.532218 roof_mask_Yv8-0.5.5/ultralytics/yolo/engine/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/engine/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    41854 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/engine/exporter.py
--rwxrwxrwx   0 root         (0) root         (0)    21469 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/engine/model.py
--rwxrwxrwx   0 root         (0) root         (0)    14720 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/engine/predictor.py
--rwxrwxrwx   0 root         (0) root         (0)    17378 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/engine/results.py
--rwxrwxrwx   0 root         (0) root         (0)    29843 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/engine/trainer.py
--rwxrwxrwx   0 root         (0) root         (0)    10358 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/engine/validator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.604176 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/
--rwxrwxrwx   0 root         (0) root         (0)    25215 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3823 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/autobatch.py
--rwxrwxrwx   0 root         (0) root         (0)     5414 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/benchmarks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.670138 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/
--rwxrwxrwx   0 root         (0) root         (0)      171 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3783 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/base.py
--rwxrwxrwx   0 root         (0) root         (0)     5286 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/clearml.py
--rwxrwxrwx   0 root         (0) root         (0)    11929 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/comet.py
--rwxrwxrwx   0 root         (0) root         (0)     3189 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/hub.py
--rwxrwxrwx   0 root         (0) root         (0)     2512 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/mlflow.py
--rwxrwxrwx   0 root         (0) root         (0)      385 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/raytune.py
--rwxrwxrwx   0 root         (0) root         (0)     1297 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/tensorboard.py
--rwxrwxrwx   0 root         (0) root         (0)     1593 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/wb.py
--rwxrwxrwx   0 root         (0) root         (0)    14190 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/checks.py
--rwxrwxrwx   0 root         (0) root         (0)     2412 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/dist.py
--rwxrwxrwx   0 root         (0) root         (0)    10052 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/downloads.py
--rwxrwxrwx   0 root         (0) root         (0)      251 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/errors.py
--rwxrwxrwx   0 root         (0) root         (0)     3105 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/files.py
--rwxrwxrwx   0 root         (0) root         (0)    11394 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/instance.py
--rwxrwxrwx   0 root         (0) root         (0)     2889 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/loss.py
--rwxrwxrwx   0 root         (0) root         (0)    35693 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/metrics.py
--rwxrwxrwx   0 root         (0) root         (0)    28503 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/ops.py
--rwxrwxrwx   0 root         (0) root         (0)    20613 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/plotting.py
--rwxrwxrwx   0 root         (0) root         (0)    10233 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/tal.py
--rwxrwxrwx   0 root         (0) root         (0)    19694 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/torch_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     2302 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/tuner.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.712114 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/
--rwxrwxrwx   0 root         (0) root         (0)      157 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.770080 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/classify/
--rwxrwxrwx   0 root         (0) root         (0)      390 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/classify/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1459 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/classify/predict.py
--rwxrwxrwx   0 root         (0) root         (0)     6388 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/classify/train.py
--rwxrwxrwx   0 root         (0) root         (0)     2933 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/classify/val.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.821051 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/detect/
--rwxrwxrwx   0 root         (0) root         (0)      276 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/detect/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2005 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/detect/predict.py
--rwxrwxrwx   0 root         (0) root         (0)     9886 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/detect/train.py
--rwxrwxrwx   0 root         (0) root         (0)    12516 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/detect/val.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.892009 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/pose/
--rwxrwxrwx   0 root         (0) root         (0)      246 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/pose/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2076 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/pose/predict.py
--rwxrwxrwx   0 root         (0) root         (0)     7145 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/pose/train.py
--rwxrwxrwx   0 root         (0) root         (0)    10050 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/pose/val.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.956972 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/segment/
--rwxrwxrwx   0 root         (0) root         (0)      294 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/segment/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2657 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/segment/predict.py
--rwxrwxrwx   0 root         (0) root         (0)     7664 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/segment/train.py
--rwxrwxrwx   0 root         (0) root         (0)    11922 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/segment/val.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 18:47:41.989953 roof_mask_Yv8-0.5.5/yolo_roof/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.5/yolo_roof/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    33279 2023-04-19 14:59:59.000000 roof_mask_Yv8-0.5.5/yolo_roof/detect_functions.py
--rwxrwxrwx   0 root         (0) root         (0)    21374 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.5/yolo_roof/geo_functions.py
--rwxrwxrwx   0 root         (0) root         (0)    41759 2023-04-18 18:11:13.000000 roof_mask_Yv8-0.5.5/yolo_roof/report_functions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.067653 roof_mask_Yv8-0.5.6/
+-rwxrwxrwx   0 root         (0) root         (0)      143 2023-04-19 16:56:54.000000 roof_mask_Yv8-0.5.6/.gitignore
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-20 18:44:18.000000 roof_mask_Yv8-0.5.6/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      473 2023-04-20 20:41:21.375303 roof_mask_Yv8-0.5.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.106630 roof_mask_Yv8-0.5.6/detectron2/
+-rwxrwxrwx   0 root         (0) root         (0)      258 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.154603 roof_mask_Yv8-0.5.6/detectron2/checkpoint/
+-rwxrwxrwx   0 root         (0) root         (0)      347 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/checkpoint/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17782 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/checkpoint/c2_model_loading.py
+-rwxrwxrwx   0 root         (0) root         (0)     5685 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/checkpoint/catalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     5258 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/checkpoint/detection_checkpoint.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.204574 roof_mask_Yv8-0.5.6/detectron2/config/
+-rwxrwxrwx   0 root         (0) root         (0)      599 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/config/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7890 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/config/compat.py
+-rwxrwxrwx   0 root         (0) root         (0)     9211 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/config/config.py
+-rwxrwxrwx   0 root         (0) root         (0)    29512 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/config/defaults.py
+-rwxrwxrwx   0 root         (0) root         (0)     2719 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/config/instantiate.py
+-rwxrwxrwx   0 root         (0) root         (0)    14944 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/config/lazy.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.255545 roof_mask_Yv8-0.5.6/detectron2/data/
+-rwxrwxrwx   0 root         (0) root         (0)      644 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7378 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/data/benchmark.py
+-rwxrwxrwx   0 root         (0) root         (0)    20605 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/data/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     7224 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/data/catalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     9164 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/data/common.py
+-rwxrwxrwx   0 root         (0) root         (0)     8169 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.6/detectron2/data/dataset_mapper.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.309514 roof_mask_Yv8-0.5.6/detectron2/data/datasets/
+-rwxrwxrwx   0 root         (0) root         (0)      347 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/datasets/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      523 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/datasets/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10174 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/datasets/builtin.py
+-rwxrwxrwx   0 root         (0) root         (0)    21841 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/datasets/builtin_meta.py
+-rwxrwxrwx   0 root         (0) root         (0)    13167 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/datasets/cityscapes.py
+-rwxrwxrwx   0 root         (0) root         (0)     7821 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/datasets/cityscapes_panoptic.py
+-rwxrwxrwx   0 root         (0) root         (0)    23465 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/datasets/coco.py
+-rwxrwxrwx   0 root         (0) root         (0)     8977 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/datasets/coco_panoptic.py
+-rwxrwxrwx   0 root         (0) root         (0)     9623 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/datasets/lvis.py
+-rwxrwxrwx   0 root         (0) root         (0)   223757 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/datasets/lvis_v0_5_categories.py
+-rwxrwxrwx   0 root         (0) root         (0)   219177 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/datasets/lvis_v1_categories.py
+-rwxrwxrwx   0 root         (0) root         (0)    39414 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rwxrwxrwx   0 root         (0) root         (0)     3128 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/datasets/pascal_voc.py
+-rwxrwxrwx   0 root         (0) root         (0)      169 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/datasets/register_coco.py
+-rwxrwxrwx   0 root         (0) root         (0)    22841 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/detection_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.358486 roof_mask_Yv8-0.5.6/detectron2/data/samplers/
+-rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/samplers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11789 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/samplers/distributed_sampler.py
+-rwxrwxrwx   0 root         (0) root         (0)     1944 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/samplers/grouped_batch_sampler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.409457 roof_mask_Yv8-0.5.6/detectron2/data/transforms/
+-rwxrwxrwx   0 root         (0) root         (0)      466 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/transforms/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14117 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/transforms/augmentation.py
+-rwxrwxrwx   0 root         (0) root         (0)    23069 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/transforms/augmentation_impl.py
+-rwxrwxrwx   0 root         (0) root         (0)    12629 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/data/transforms/transform.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.444437 roof_mask_Yv8-0.5.6/detectron2/engine/
+-rwxrwxrwx   0 root         (0) root         (0)      340 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/engine/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    26868 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/engine/defaults.py
+-rwxrwxrwx   0 root         (0) root         (0)    25497 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/engine/hooks.py
+-rwxrwxrwx   0 root         (0) root         (0)     4089 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/engine/launch.py
+-rwxrwxrwx   0 root         (0) root         (0)    14104 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/engine/train_loop.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.490410 roof_mask_Yv8-0.5.6/detectron2/evaluation/
+-rwxrwxrwx   0 root         (0) root         (0)      671 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/evaluation/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8369 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/evaluation/cityscapes_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)    30423 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/evaluation/coco_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     8156 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.6/detectron2/evaluation/evaluator.py
+-rwxrwxrwx   0 root         (0) root         (0)     5078 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/evaluation/fast_eval_api.py
+-rwxrwxrwx   0 root         (0) root         (0)    15018 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/evaluation/lvis_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     7500 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/evaluation/panoptic_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)    10862 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/evaluation/pascal_voc_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     7608 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/evaluation/rotated_coco_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     8191 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/evaluation/sem_seg_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     2614 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/evaluation/testing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.552373 roof_mask_Yv8-0.5.6/detectron2/export/
+-rwxrwxrwx   0 root         (0) root         (0)      513 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/export/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      336 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9280 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/export/api.py
+-rwxrwxrwx   0 root         (0) root         (0)    21035 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/export/c10.py
+-rwxrwxrwx   0 root         (0) root         (0)     7803 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/export/caffe2_export.py
+-rwxrwxrwx   0 root         (0) root         (0)     6674 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/export/caffe2_inference.py
+-rwxrwxrwx   0 root         (0) root         (0)    17034 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/export/caffe2_modeling.py
+-rwxrwxrwx   0 root         (0) root         (0)     5033 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/export/caffe2_patch.py
+-rwxrwxrwx   0 root         (0) root         (0)    11807 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/export/flatten.py
+-rwxrwxrwx   0 root         (0) root         (0)    38071 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/export/shared.py
+-rwxrwxrwx   0 root         (0) root         (0)     5008 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/export/torchscript.py
+-rwxrwxrwx   0 root         (0) root         (0)    11526 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/export/torchscript_patch.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.619335 roof_mask_Yv8-0.5.6/detectron2/layers/
+-rwxrwxrwx   0 root         (0) root         (0)      839 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/layers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5764 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/layers/aspp.py
+-rwxrwxrwx   0 root         (0) root         (0)    12131 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/layers/batch_norm.py
+-rwxrwxrwx   0 root         (0) root         (0)     3024 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/layers/blocks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.665309 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/
+-rwxrwxrwx   0 root         (0) root         (0)      122 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.730272 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/ROIAlignRotated/
+-rwxrwxrwx   0 root         (0) root         (0)     2870 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated.h
+-rwxrwxrwx   0 root         (0) root         (0)    16031 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cpu.cpp
+-rwxrwxrwx   0 root         (0) root         (0)    13876 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cuda.cu
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.776245 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/box_iou_rotated/
+-rwxrwxrwx   0 root         (0) root         (0)      988 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated.h
+-rwxrwxrwx   0 root         (0) root         (0)     1090 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cpu.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     4454 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cuda.cu
+-rwxrwxrwx   0 root         (0) root         (0)    10844 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_utils.h
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.839210 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/cocoeval/
+-rwxrwxrwx   0 root         (0) root         (0)    20746 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/cocoeval/cocoeval.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     3515 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/cocoeval/cocoeval.h
+-rwxrwxrwx   0 root         (0) root         (0)      622 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/cuda_version.cu
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.917163 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/deformable/
+-rwxrwxrwx   0 root         (0) root         (0)     8384 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/deformable/deform_conv.h
+-rwxrwxrwx   0 root         (0) root         (0)    31785 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/deformable/deform_conv_cuda.cu
+-rwxrwxrwx   0 root         (0) root         (0)    44279 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/deformable/deform_conv_cuda_kernel.cu
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:40.978129 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/nms_rotated/
+-rwxrwxrwx   0 root         (0) root         (0)     1089 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/nms_rotated/nms_rotated.h
+-rwxrwxrwx   0 root         (0) root         (0)     2307 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/nms_rotated/nms_rotated_cpu.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     4859 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/nms_rotated/nms_rotated_cuda.cu
+-rwxrwxrwx   0 root         (0) root         (0)     3167 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/csrc/vision.cpp
+-rwxrwxrwx   0 root         (0) root         (0)    16978 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/deform_conv.py
+-rwxrwxrwx   0 root         (0) root         (0)     4204 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/losses.py
+-rwxrwxrwx   0 root         (0) root         (0)    10881 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/mask_ops.py
+-rwxrwxrwx   0 root         (0) root         (0)     6490 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/nms.py
+-rwxrwxrwx   0 root         (0) root         (0)     3098 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/roi_align.py
+-rwxrwxrwx   0 root         (0) root         (0)     3302 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/roi_align_rotated.py
+-rwxrwxrwx   0 root         (0) root         (0)      652 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/rotated_boxes.py
+-rwxrwxrwx   0 root         (0) root         (0)      661 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/shape_spec.py
+-rwxrwxrwx   0 root         (0) root         (0)     4893 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/layers/wrappers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.015108 roof_mask_Yv8-0.5.6/detectron2/modeling/
+-rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15443 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/anchor_generator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.082069 roof_mask_Yv8-0.5.6/detectron2/modeling/backbone/
+-rwxrwxrwx   0 root         (0) root         (0)      475 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/backbone/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1543 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/backbone/backbone.py
+-rwxrwxrwx   0 root         (0) root         (0)     1015 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/backbone/build.py
+-rwxrwxrwx   0 root         (0) root         (0)    10055 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/backbone/fpn.py
+-rwxrwxrwx   0 root         (0) root         (0)    16656 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/backbone/regnet.py
+-rwxrwxrwx   0 root         (0) root         (0)    23658 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/backbone/resnet.py
+-rwxrwxrwx   0 root         (0) root         (0)    15123 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/box_regression.py
+-rwxrwxrwx   0 root         (0) root         (0)     6264 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/matcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.152029 roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/
+-rwxrwxrwx   0 root         (0) root         (0)      508 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      814 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/build.py
+-rwxrwxrwx   0 root         (0) root         (0)    11550 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/dense_detector.py
+-rwxrwxrwx   0 root         (0) root         (0)    13213 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/fcos.py
+-rwxrwxrwx   0 root         (0) root         (0)    10335 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rwxrwxrwx   0 root         (0) root         (0)    13710 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    18265 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/retinanet.py
+-rwxrwxrwx   0 root         (0) root         (0)     9720 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/semantic_seg.py
+-rwxrwxrwx   0 root         (0) root         (0)    10832 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/mmdet_wrapper.py
+-rwxrwxrwx   0 root         (0) root         (0)    11316 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/poolers.py
+-rwxrwxrwx   0 root         (0) root         (0)     4046 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/postprocessing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.206997 roof_mask_Yv8-0.5.6/detectron2/modeling/proposal_generator/
+-rwxrwxrwx   0 root         (0) root         (0)      231 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/proposal_generator/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      836 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/proposal_generator/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     8128 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/proposal_generator/proposal_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    23814 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/proposal_generator/rpn.py
+-rwxrwxrwx   0 root         (0) root         (0)     8807 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/proposal_generator/rrpn.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.257968 roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/
+-rwxrwxrwx   0 root         (0) root         (0)      768 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4077 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/box_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    12990 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    25274 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/fast_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    11156 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/keypoint_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    12169 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/mask_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    37701 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/roi_heads.py
+-rwxrwxrwx   0 root         (0) root         (0)    11158 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)     2334 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/sampling.py
+-rwxrwxrwx   0 root         (0) root         (0)    12416 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/modeling/test_time_augmentation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.314936 roof_mask_Yv8-0.5.6/detectron2/solver/
+-rwxrwxrwx   0 root         (0) root         (0)      298 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/solver/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11127 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/solver/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     8648 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.6/detectron2/solver/lr_scheduler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.372902 roof_mask_Yv8-0.5.6/detectron2/structures/
+-rwxrwxrwx   0 root         (0) root         (0)      645 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/detectron2/structures/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14429 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/detectron2/structures/boxes.py
+-rwxrwxrwx   0 root         (0) root         (0)     4557 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/detectron2/structures/image_list.py
+-rwxrwxrwx   0 root         (0) root         (0)     6542 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/detectron2/structures/instances.py
+-rwxrwxrwx   0 root         (0) root         (0)     9030 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/detectron2/structures/keypoints.py
+-rwxrwxrwx   0 root         (0) root         (0)    19802 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/detectron2/structures/masks.py
+-rwxrwxrwx   0 root         (0) root         (0)    18853 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/detectron2/structures/rotated_boxes.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.419875 roof_mask_Yv8-0.5.6/detectron2/tracking/
+-rwxrwxrwx   0 root         (0) root         (0)      580 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/detectron2/tracking/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2216 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/detectron2/tracking/base_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)    11858 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/detectron2/tracking/bbox_iou_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     7486 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/detectron2/tracking/hungarian_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     4142 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     1106 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/detectron2/tracking/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     5288 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.464849 roof_mask_Yv8-0.5.6/detectron2/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      175 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.6/detectron2/utils/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       51 2023-04-18 18:45:50.000000 roof_mask_Yv8-0.5.6/detectron2/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6017 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.6/detectron2/utils/analysis.py
+-rwxrwxrwx   0 root         (0) root         (0)     8391 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.6/detectron2/utils/collect_env.py
+-rwxrwxrwx   0 root         (0) root         (0)     4096 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.6/detectron2/utils/colormap.py
+-rwxrwxrwx   0 root         (0) root         (0)     5610 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.6/detectron2/utils/comm.py
+-rwxrwxrwx   0 root         (0) root         (0)     1838 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.6/detectron2/utils/develop.py
+-rwxrwxrwx   0 root         (0) root         (0)     5644 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.6/detectron2/utils/env.py
+-rwxrwxrwx   0 root         (0) root         (0)    17024 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.6/detectron2/utils/events.py
+-rwxrwxrwx   0 root         (0) root         (0)     1189 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.6/detectron2/utils/file_io.py
+-rwxrwxrwx   0 root         (0) root         (0)     7807 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.6/detectron2/utils/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     2583 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.6/detectron2/utils/memory.py
+-rwxrwxrwx   0 root         (0) root         (0)     1874 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.6/detectron2/utils/registry.py
+-rwxrwxrwx   0 root         (0) root         (0)     1064 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.6/detectron2/utils/serialize.py
+-rwxrwxrwx   0 root         (0) root         (0)     4833 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.6/detectron2/utils/testing.py
+-rwxrwxrwx   0 root         (0) root         (0)    11319 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.6/detectron2/utils/video_visualizer.py
+-rwxrwxrwx   0 root         (0) root         (0)    51159 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.6/detectron2/utils/visualizer.py
+-rwxrwxrwx   0 root         (0) root         (0)    52915 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.6/detectron2/utils/visualizer_new.py
+-rwxrwxrwx   0 root         (0) root         (0)      107 2023-04-17 21:19:17.000000 roof_mask_Yv8-0.5.6/readme.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.496830 roof_mask_Yv8-0.5.6/roof_mask_Yv8.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      473 2023-04-20 20:41:10.000000 roof_mask_Yv8-0.5.6/roof_mask_Yv8.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     9323 2023-04-20 20:40:40.000000 roof_mask_Yv8-0.5.6/roof_mask_Yv8.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-20 20:41:10.000000 roof_mask_Yv8-0.5.6/roof_mask_Yv8.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-20 20:41:10.000000 roof_mask_Yv8-0.5.6/roof_mask_Yv8.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-20 20:41:21.439303 roof_mask_Yv8-0.5.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      632 2023-04-20 20:36:55.000000 roof_mask_Yv8-0.5.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.545802 roof_mask_Yv8-0.5.6/ultralytics/
+-rwxrwxrwx   0 root         (0) root         (0)      295 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/ultralytics/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.593775 roof_mask_Yv8-0.5.6/ultralytics/hub/
+-rwxrwxrwx   0 root         (0) root         (0)     3421 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/ultralytics/hub/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5206 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/ultralytics/hub/auth.py
+-rwxrwxrwx   0 root         (0) root         (0)     8690 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/ultralytics/hub/session.py
+-rwxrwxrwx   0 root         (0) root         (0)     9723 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/ultralytics/hub/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.641747 roof_mask_Yv8-0.5.6/ultralytics/nn/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/ultralytics/nn/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    24083 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/ultralytics/nn/autobackend.py
+-rwxrwxrwx   0 root         (0) root         (0)    11839 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/ultralytics/nn/autoshape.py
+-rwxrwxrwx   0 root         (0) root         (0)    20062 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/ultralytics/nn/modules.py
+-rwxrwxrwx   0 root         (0) root         (0)    26619 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/ultralytics/nn/tasks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.688720 roof_mask_Yv8-0.5.6/ultralytics/yolo/
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.734694 roof_mask_Yv8-0.5.6/ultralytics/yolo/cfg/
+-rwxrwxrwx   0 root         (0) root         (0)    17582 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/cfg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6237 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/cfg/default.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.798657 roof_mask_Yv8-0.5.6/ultralytics/yolo/data/
+-rwxrwxrwx   0 root         (0) root         (0)      483 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    31285 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/data/augment.py
+-rwxrwxrwx   0 root         (0) root         (0)     8919 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/data/base.py
+-rwxrwxrwx   0 root         (0) root         (0)     8614 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/data/build.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.853625 roof_mask_Yv8-0.5.6/ultralytics/yolo/data/dataloaders/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/data/dataloaders/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15194 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/data/dataloaders/stream_loaders.py
+-rwxrwxrwx   0 root         (0) root         (0)    17226 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/data/dataloaders/v5augmentations.py
+-rwxrwxrwx   0 root         (0) root         (0)    49861 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/data/dataloaders/v5loader.py
+-rwxrwxrwx   0 root         (0) root         (0)    12740 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/data/dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/data/dataset_wrappers.py
+-rwxrwxrwx   0 root         (0) root         (0)    22728 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/data/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.887606 roof_mask_Yv8-0.5.6/ultralytics/yolo/engine/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/engine/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    41854 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/engine/exporter.py
+-rwxrwxrwx   0 root         (0) root         (0)    21469 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/engine/model.py
+-rwxrwxrwx   0 root         (0) root         (0)    14720 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/engine/predictor.py
+-rwxrwxrwx   0 root         (0) root         (0)    17378 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/engine/results.py
+-rwxrwxrwx   0 root         (0) root         (0)    29843 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/engine/trainer.py
+-rwxrwxrwx   0 root         (0) root         (0)    10358 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/engine/validator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.934579 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/
+-rwxrwxrwx   0 root         (0) root         (0)    25215 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3823 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/autobatch.py
+-rwxrwxrwx   0 root         (0) root         (0)     5414 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/benchmarks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:41.986549 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/
+-rwxrwxrwx   0 root         (0) root         (0)      171 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3783 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/base.py
+-rwxrwxrwx   0 root         (0) root         (0)     5286 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/clearml.py
+-rwxrwxrwx   0 root         (0) root         (0)    11929 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/comet.py
+-rwxrwxrwx   0 root         (0) root         (0)     3189 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/hub.py
+-rwxrwxrwx   0 root         (0) root         (0)     2512 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/mlflow.py
+-rwxrwxrwx   0 root         (0) root         (0)      385 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/raytune.py
+-rwxrwxrwx   0 root         (0) root         (0)     1297 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/tensorboard.py
+-rwxrwxrwx   0 root         (0) root         (0)     1593 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/wb.py
+-rwxrwxrwx   0 root         (0) root         (0)    14190 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/checks.py
+-rwxrwxrwx   0 root         (0) root         (0)     2412 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/dist.py
+-rwxrwxrwx   0 root         (0) root         (0)    10052 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/downloads.py
+-rwxrwxrwx   0 root         (0) root         (0)      251 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/errors.py
+-rwxrwxrwx   0 root         (0) root         (0)     3105 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/files.py
+-rwxrwxrwx   0 root         (0) root         (0)    11394 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/instance.py
+-rwxrwxrwx   0 root         (0) root         (0)     2889 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/loss.py
+-rwxrwxrwx   0 root         (0) root         (0)    35693 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/metrics.py
+-rwxrwxrwx   0 root         (0) root         (0)    28503 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/ops.py
+-rwxrwxrwx   0 root         (0) root         (0)    20613 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/plotting.py
+-rwxrwxrwx   0 root         (0) root         (0)    10233 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/tal.py
+-rwxrwxrwx   0 root         (0) root         (0)    19694 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/torch_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     2302 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/tuner.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:42.035521 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/
+-rwxrwxrwx   0 root         (0) root         (0)      157 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:42.104481 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/classify/
+-rwxrwxrwx   0 root         (0) root         (0)      390 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/classify/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1459 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/classify/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     6388 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/classify/train.py
+-rwxrwxrwx   0 root         (0) root         (0)     2933 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/classify/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:42.152454 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/detect/
+-rwxrwxrwx   0 root         (0) root         (0)      276 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/detect/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2005 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/detect/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     9886 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/detect/train.py
+-rwxrwxrwx   0 root         (0) root         (0)    12516 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/detect/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:42.207422 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/pose/
+-rwxrwxrwx   0 root         (0) root         (0)      246 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/pose/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2076 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/pose/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     7145 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/pose/train.py
+-rwxrwxrwx   0 root         (0) root         (0)    10050 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/pose/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:42.257393 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/segment/
+-rwxrwxrwx   0 root         (0) root         (0)      294 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/segment/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2657 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/segment/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     7664 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/segment/train.py
+-rwxrwxrwx   0 root         (0) root         (0)    11922 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/segment/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 20:40:42.296371 roof_mask_Yv8-0.5.6/yolo_roof/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.6/yolo_roof/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    33279 2023-04-19 14:59:59.000000 roof_mask_Yv8-0.5.6/yolo_roof/detect_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)    21374 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.6/yolo_roof/geo_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)    41759 2023-04-18 18:11:13.000000 roof_mask_Yv8-0.5.6/yolo_roof/report_functions.py
```

### Comparing `roof_mask_Yv8-0.5.5/detectron2/checkpoint/c2_model_loading.py` & `roof_mask_Yv8-0.5.6/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/checkpoint/catalog.py` & `roof_mask_Yv8-0.5.6/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/checkpoint/detection_checkpoint.py` & `roof_mask_Yv8-0.5.6/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/config/__init__.py` & `roof_mask_Yv8-0.5.6/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/config/compat.py` & `roof_mask_Yv8-0.5.6/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/config/config.py` & `roof_mask_Yv8-0.5.6/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/config/defaults.py` & `roof_mask_Yv8-0.5.6/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/config/instantiate.py` & `roof_mask_Yv8-0.5.6/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/config/lazy.py` & `roof_mask_Yv8-0.5.6/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/__init__.py` & `roof_mask_Yv8-0.5.6/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/benchmark.py` & `roof_mask_Yv8-0.5.6/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/build.py` & `roof_mask_Yv8-0.5.6/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/catalog.py` & `roof_mask_Yv8-0.5.6/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/common.py` & `roof_mask_Yv8-0.5.6/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/dataset_mapper.py` & `roof_mask_Yv8-0.5.6/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/datasets/__init__.py` & `roof_mask_Yv8-0.5.6/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/datasets/builtin.py` & `roof_mask_Yv8-0.5.6/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/datasets/builtin_meta.py` & `roof_mask_Yv8-0.5.6/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/datasets/cityscapes.py` & `roof_mask_Yv8-0.5.6/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/datasets/cityscapes_panoptic.py` & `roof_mask_Yv8-0.5.6/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/datasets/coco.py` & `roof_mask_Yv8-0.5.6/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/datasets/coco_panoptic.py` & `roof_mask_Yv8-0.5.6/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/datasets/lvis.py` & `roof_mask_Yv8-0.5.6/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/datasets/lvis_v0_5_categories.py` & `roof_mask_Yv8-0.5.6/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/datasets/lvis_v1_categories.py` & `roof_mask_Yv8-0.5.6/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/datasets/lvis_v1_category_image_count.py` & `roof_mask_Yv8-0.5.6/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/datasets/pascal_voc.py` & `roof_mask_Yv8-0.5.6/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/detection_utils.py` & `roof_mask_Yv8-0.5.6/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/samplers/distributed_sampler.py` & `roof_mask_Yv8-0.5.6/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/samplers/grouped_batch_sampler.py` & `roof_mask_Yv8-0.5.6/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/transforms/augmentation.py` & `roof_mask_Yv8-0.5.6/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/transforms/augmentation_impl.py` & `roof_mask_Yv8-0.5.6/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/data/transforms/transform.py` & `roof_mask_Yv8-0.5.6/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/engine/defaults.py` & `roof_mask_Yv8-0.5.6/detectron2/engine/defaults.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/engine/hooks.py` & `roof_mask_Yv8-0.5.6/detectron2/engine/hooks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/engine/launch.py` & `roof_mask_Yv8-0.5.6/detectron2/engine/launch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/engine/train_loop.py` & `roof_mask_Yv8-0.5.6/detectron2/engine/train_loop.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/evaluation/__init__.py` & `roof_mask_Yv8-0.5.6/detectron2/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/evaluation/cityscapes_evaluation.py` & `roof_mask_Yv8-0.5.6/detectron2/evaluation/cityscapes_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/evaluation/coco_evaluation.py` & `roof_mask_Yv8-0.5.6/detectron2/evaluation/coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/evaluation/evaluator.py` & `roof_mask_Yv8-0.5.6/detectron2/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/evaluation/fast_eval_api.py` & `roof_mask_Yv8-0.5.6/detectron2/evaluation/fast_eval_api.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/evaluation/lvis_evaluation.py` & `roof_mask_Yv8-0.5.6/detectron2/evaluation/lvis_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/evaluation/panoptic_evaluation.py` & `roof_mask_Yv8-0.5.6/detectron2/evaluation/panoptic_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/evaluation/pascal_voc_evaluation.py` & `roof_mask_Yv8-0.5.6/detectron2/evaluation/pascal_voc_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/evaluation/rotated_coco_evaluation.py` & `roof_mask_Yv8-0.5.6/detectron2/evaluation/rotated_coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/evaluation/sem_seg_evaluation.py` & `roof_mask_Yv8-0.5.6/detectron2/evaluation/sem_seg_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/evaluation/testing.py` & `roof_mask_Yv8-0.5.6/detectron2/evaluation/testing.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/export/api.py` & `roof_mask_Yv8-0.5.6/detectron2/export/api.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/export/c10.py` & `roof_mask_Yv8-0.5.6/detectron2/export/c10.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/export/caffe2_export.py` & `roof_mask_Yv8-0.5.6/detectron2/export/caffe2_export.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/export/caffe2_inference.py` & `roof_mask_Yv8-0.5.6/detectron2/export/caffe2_inference.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/export/caffe2_modeling.py` & `roof_mask_Yv8-0.5.6/detectron2/export/caffe2_modeling.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/export/caffe2_patch.py` & `roof_mask_Yv8-0.5.6/detectron2/export/caffe2_patch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/export/flatten.py` & `roof_mask_Yv8-0.5.6/detectron2/export/flatten.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/export/shared.py` & `roof_mask_Yv8-0.5.6/detectron2/export/shared.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/export/torchscript.py` & `roof_mask_Yv8-0.5.6/detectron2/export/torchscript.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/export/torchscript_patch.py` & `roof_mask_Yv8-0.5.6/detectron2/export/torchscript_patch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/layers/__init__.py` & `roof_mask_Yv8-0.5.6/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/layers/aspp.py` & `roof_mask_Yv8-0.5.6/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/layers/batch_norm.py` & `roof_mask_Yv8-0.5.6/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/layers/blocks.py` & `roof_mask_Yv8-0.5.6/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/layers/deform_conv.py` & `roof_mask_Yv8-0.5.6/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/layers/losses.py` & `roof_mask_Yv8-0.5.6/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/layers/mask_ops.py` & `roof_mask_Yv8-0.5.6/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/layers/nms.py` & `roof_mask_Yv8-0.5.6/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/layers/roi_align.py` & `roof_mask_Yv8-0.5.6/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/layers/roi_align_rotated.py` & `roof_mask_Yv8-0.5.6/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/layers/rotated_boxes.py` & `roof_mask_Yv8-0.5.6/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/layers/shape_spec.py` & `roof_mask_Yv8-0.5.6/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/layers/wrappers.py` & `roof_mask_Yv8-0.5.6/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/__init__.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/anchor_generator.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/backbone/backbone.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/backbone/build.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/backbone/fpn.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/backbone/regnet.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/backbone/resnet.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/box_regression.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/matcher.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/build.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/dense_detector.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/fcos.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/panoptic_fpn.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/rcnn.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/retinanet.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/meta_arch/semantic_seg.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/mmdet_wrapper.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/poolers.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/postprocessing.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/proposal_generator/build.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/proposal_generator/proposal_utils.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/proposal_generator/rpn.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/proposal_generator/rrpn.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/__init__.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/box_head.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/cascade_rcnn.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/fast_rcnn.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/keypoint_head.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/mask_head.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/roi_heads.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/sampling.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/modeling/test_time_augmentation.py` & `roof_mask_Yv8-0.5.6/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/solver/build.py` & `roof_mask_Yv8-0.5.6/detectron2/solver/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/solver/lr_scheduler.py` & `roof_mask_Yv8-0.5.6/detectron2/solver/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/structures/__init__.py` & `roof_mask_Yv8-0.5.6/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/structures/boxes.py` & `roof_mask_Yv8-0.5.6/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/structures/image_list.py` & `roof_mask_Yv8-0.5.6/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/structures/instances.py` & `roof_mask_Yv8-0.5.6/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/structures/keypoints.py` & `roof_mask_Yv8-0.5.6/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/structures/masks.py` & `roof_mask_Yv8-0.5.6/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/structures/rotated_boxes.py` & `roof_mask_Yv8-0.5.6/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/tracking/__init__.py` & `roof_mask_Yv8-0.5.6/detectron2/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/tracking/base_tracker.py` & `roof_mask_Yv8-0.5.6/detectron2/tracking/base_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/tracking/bbox_iou_tracker.py` & `roof_mask_Yv8-0.5.6/detectron2/tracking/bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/tracking/hungarian_tracker.py` & `roof_mask_Yv8-0.5.6/detectron2/tracking/hungarian_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py` & `roof_mask_Yv8-0.5.6/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/tracking/utils.py` & `roof_mask_Yv8-0.5.6/detectron2/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py` & `roof_mask_Yv8-0.5.6/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/analysis.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/collect_env.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/colormap.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/comm.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/develop.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/env.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/events.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/file_io.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/logger.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/memory.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/registry.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/serialize.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/testing.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/video_visualizer.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/visualizer.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/detectron2/utils/visualizer_new.py` & `roof_mask_Yv8-0.5.6/detectron2/utils/visualizer_new.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/roof_mask_Yv8.egg-info/SOURCES.txt` & `roof_mask_Yv8-0.5.6/roof_mask_Yv8.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+.gitignore
 MANIFEST.in
+__init__.py
+readme.txt
 setup.py
 detectron2/__init__.py
 detectron2/checkpoint/__init__.py
 detectron2/checkpoint/c2_model_loading.py
 detectron2/checkpoint/catalog.py
 detectron2/checkpoint/detection_checkpoint.py
 detectron2/config/__init__.py
@@ -14,14 +17,15 @@
 detectron2/data/__init__.py
 detectron2/data/benchmark.py
 detectron2/data/build.py
 detectron2/data/catalog.py
 detectron2/data/common.py
 detectron2/data/dataset_mapper.py
 detectron2/data/detection_utils.py
+detectron2/data/datasets/README.md
 detectron2/data/datasets/__init__.py
 detectron2/data/datasets/builtin.py
 detectron2/data/datasets/builtin_meta.py
 detectron2/data/datasets/cityscapes.py
 detectron2/data/datasets/cityscapes_panoptic.py
 detectron2/data/datasets/coco.py
 detectron2/data/datasets/coco_panoptic.py
@@ -50,14 +54,15 @@
 detectron2/evaluation/fast_eval_api.py
 detectron2/evaluation/lvis_evaluation.py
 detectron2/evaluation/panoptic_evaluation.py
 detectron2/evaluation/pascal_voc_evaluation.py
 detectron2/evaluation/rotated_coco_evaluation.py
 detectron2/evaluation/sem_seg_evaluation.py
 detectron2/evaluation/testing.py
+detectron2/export/README.md
 detectron2/export/__init__.py
 detectron2/export/api.py
 detectron2/export/c10.py
 detectron2/export/caffe2_export.py
 detectron2/export/caffe2_inference.py
 detectron2/export/caffe2_modeling.py
 detectron2/export/caffe2_patch.py
@@ -74,14 +79,32 @@
 detectron2/layers/mask_ops.py
 detectron2/layers/nms.py
 detectron2/layers/roi_align.py
 detectron2/layers/roi_align_rotated.py
 detectron2/layers/rotated_boxes.py
 detectron2/layers/shape_spec.py
 detectron2/layers/wrappers.py
+detectron2/layers/csrc/README.md
+detectron2/layers/csrc/cuda_version.cu
+detectron2/layers/csrc/vision.cpp
+detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated.h
+detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cpu.cpp
+detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cuda.cu
+detectron2/layers/csrc/box_iou_rotated/box_iou_rotated.h
+detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cpu.cpp
+detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cuda.cu
+detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_utils.h
+detectron2/layers/csrc/cocoeval/cocoeval.cpp
+detectron2/layers/csrc/cocoeval/cocoeval.h
+detectron2/layers/csrc/deformable/deform_conv.h
+detectron2/layers/csrc/deformable/deform_conv_cuda.cu
+detectron2/layers/csrc/deformable/deform_conv_cuda_kernel.cu
+detectron2/layers/csrc/nms_rotated/nms_rotated.h
+detectron2/layers/csrc/nms_rotated/nms_rotated_cpu.cpp
+detectron2/layers/csrc/nms_rotated/nms_rotated_cuda.cu
 detectron2/modeling/__init__.py
 detectron2/modeling/anchor_generator.py
 detectron2/modeling/box_regression.py
 detectron2/modeling/matcher.py
 detectron2/modeling/mmdet_wrapper.py
 detectron2/modeling/poolers.py
 detectron2/modeling/postprocessing.py
@@ -127,14 +150,15 @@
 detectron2/tracking/__init__.py
 detectron2/tracking/base_tracker.py
 detectron2/tracking/bbox_iou_tracker.py
 detectron2/tracking/hungarian_tracker.py
 detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py
 detectron2/tracking/utils.py
 detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py
+detectron2/utils/README.md
 detectron2/utils/__init__.py
 detectron2/utils/analysis.py
 detectron2/utils/collect_env.py
 detectron2/utils/colormap.py
 detectron2/utils/comm.py
 detectron2/utils/develop.py
 detectron2/utils/env.py
@@ -148,15 +172,14 @@
 detectron2/utils/video_visualizer.py
 detectron2/utils/visualizer.py
 detectron2/utils/visualizer_new.py
 roof_mask_Yv8.egg-info/PKG-INFO
 roof_mask_Yv8.egg-info/SOURCES.txt
 roof_mask_Yv8.egg-info/dependency_links.txt
 roof_mask_Yv8.egg-info/top_level.txt
-tests/test.py
 ultralytics/__init__.py
 ultralytics/hub/__init__.py
 ultralytics/hub/auth.py
 ultralytics/hub/session.py
 ultralytics/hub/utils.py
 ultralytics/nn/__init__.py
 ultralytics/nn/autobackend.py
```

### Comparing `roof_mask_Yv8-0.5.5/setup.py` & `roof_mask_Yv8-0.5.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 ## test upload
 import setuptools
 
 setuptools.setup(
     name = "roof_mask_Yv8",
-    version = "0.5.5",
+    version = "0.5.6",
     author = "Ruixu",
     author_email = "lrxjason@gmail.com",
     description = "upload pip package test",
     long_description = 'package supporing Yolo_v8 roof model backend.',
     long_description_content_type="text/markdown",
     url="https://github.com/lrxjason/roof_model_test/",
     packages=setuptools.find_packages(),
+    include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/hub/__init__.py` & `roof_mask_Yv8-0.5.6/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/hub/auth.py` & `roof_mask_Yv8-0.5.6/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/hub/session.py` & `roof_mask_Yv8-0.5.6/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/hub/utils.py` & `roof_mask_Yv8-0.5.6/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/nn/autobackend.py` & `roof_mask_Yv8-0.5.6/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/nn/autoshape.py` & `roof_mask_Yv8-0.5.6/ultralytics/nn/autoshape.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/nn/modules.py` & `roof_mask_Yv8-0.5.6/ultralytics/nn/modules.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/nn/tasks.py` & `roof_mask_Yv8-0.5.6/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/cfg/__init__.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/cfg/default.yaml` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/data/augment.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/data/augment.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/data/base.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/data/base.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/data/build.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/data/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/data/dataloaders/stream_loaders.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/data/dataloaders/stream_loaders.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/data/dataloaders/v5augmentations.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/data/dataloaders/v5augmentations.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/data/dataloaders/v5loader.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/data/dataloaders/v5loader.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/data/dataset.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/data/dataset_wrappers.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/data/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/data/utils.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/data/utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/engine/exporter.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/engine/model.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/engine/model.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/engine/predictor.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/engine/results.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/engine/results.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/engine/trainer.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/engine/validator.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/engine/validator.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/__init__.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/autobatch.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/benchmarks.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/base.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/clearml.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/comet.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/hub.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/mlflow.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/tensorboard.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/callbacks/wb.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/checks.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/checks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/dist.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/downloads.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/files.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/files.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/instance.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/loss.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/loss.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/metrics.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/ops.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/ops.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/plotting.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/tal.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/tal.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/torch_utils.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/utils/tuner.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/classify/predict.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/classify/predict.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/classify/train.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/classify/train.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/classify/val.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/classify/val.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/detect/predict.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/detect/predict.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/detect/train.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/detect/train.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/detect/val.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/detect/val.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/pose/predict.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/pose/predict.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/pose/train.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/pose/train.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/pose/val.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/pose/val.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/segment/predict.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/segment/predict.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/segment/train.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/segment/train.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/ultralytics/yolo/v8/segment/val.py` & `roof_mask_Yv8-0.5.6/ultralytics/yolo/v8/segment/val.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/yolo_roof/detect_functions.py` & `roof_mask_Yv8-0.5.6/yolo_roof/detect_functions.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/yolo_roof/geo_functions.py` & `roof_mask_Yv8-0.5.6/yolo_roof/geo_functions.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.5/yolo_roof/report_functions.py` & `roof_mask_Yv8-0.5.6/yolo_roof/report_functions.py`

 * *Files identical despite different names*

