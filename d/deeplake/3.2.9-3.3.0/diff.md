# Comparing `tmp/deeplake-3.2.9.tar.gz` & `tmp/deeplake-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.2.9.tar", last modified: Mon Feb 20 14:49:33 2023, max compression
+gzip compressed data, was "deeplake-3.3.0.tar", last modified: Fri Apr 21 16:42:44 2023, max compression
```

## Comparing `deeplake-3.2.9.tar` & `deeplake-3.3.0.tar`

### file list

```diff
@@ -1,351 +1,359 @@
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.205627 deeplake-3.2.9/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       36 2023-02-20 14:48:58.000000 deeplake-3.2.9/MANIFEST.in
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    24618 2023-02-20 14:49:33.206317 deeplake-3.2.9/PKG-INFO
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    20858 2023-02-20 14:48:58.000000 deeplake-3.2.9/README.md
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.078952 deeplake-3.2.9/deeplake/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2632 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/__init__.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.083572 deeplake-3.2.9/deeplake/api/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    76117 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4701 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/info.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1203 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/link.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1698 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/link_tiled.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2703 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/read.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.096909 deeplake-3.2.9/deeplake/api/tests/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3038 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2098 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    78746 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_api.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6439 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    11715 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2654 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1797 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2997 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1500 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6192 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      953 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_events.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5218 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      247 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6514 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_info.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6911 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6823 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_json.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    21293 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_link.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3223 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1789 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_linking.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1024 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1235 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_meta.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3951 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6352 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_none.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      952 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1605 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5750 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3308 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    10121 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_pop.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1228 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    17553 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4578 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2331 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_text.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    14194 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     7289 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_video.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3068 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_views.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1368 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tiled.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.097162 deeplake-3.2.9/deeplake/auto/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/__init__.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.097829 deeplake-3.2.9/deeplake/auto/structured/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/structured/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      635 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/structured/base.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2229 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.099290 deeplake-3.2.9/deeplake/auto/tests/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/tests/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6951 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6135 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5371 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5117 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.101429 deeplake-3.2.9/deeplake/auto/unstructured/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      537 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.103091 deeplake-3.2.9/deeplake/auto/unstructured/coco/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6963 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      669 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1709 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5184 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6575 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3533 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4514 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.105469 deeplake-3.2.9/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      278 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     7346 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    12793 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.108383 deeplake-3.2.9/deeplake/cli/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/cli/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5741 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/cli/auth.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      410 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/cli/commands.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      931 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/cli/test_cli.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.110464 deeplake-3.2.9/deeplake/client/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/client/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    17015 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/client/client.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1245 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/client/config.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      690 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/client/log.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1536 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/client/test_client.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3293 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/client/utils.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3872 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/compression.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5350 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/constants.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.121952 deeplake-3.2.9/deeplake/core/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       23 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/__init__.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.126452 deeplake-3.2.9/deeplake/core/chunk/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    23752 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    25277 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6168 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4926 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4494 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5446 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     9598 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)   100393 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk_engine.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    38985 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/compression.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.128979 deeplake-3.2.9/deeplake/core/compute/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/compute/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      911 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/compute/process.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2243 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/compute/provider.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      640 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/compute/ray.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      742 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/compute/serial.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      576 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/compute/thread.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.134867 deeplake-3.2.9/deeplake/core/dataset/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      903 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/dataset/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)   160825 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/dataset/dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    13657 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      760 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4031 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4242 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.135595 deeplake-3.2.9/deeplake/core/index/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      138 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/index/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    17507 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/index/index.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    18555 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/io.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4121 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/ipc.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     9825 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/link_creds.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    16161 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1971 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/linked_sample.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2677 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     9763 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/lock.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.137228 deeplake-3.2.9/deeplake/core/meta/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       97 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3595 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.139880 deeplake-3.2.9/deeplake/core/meta/encode/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    25591 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3915 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    13495 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1551 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      941 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      683 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.142207 deeplake-3.2.9/deeplake/core/meta/encode/tests/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      226 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2237 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1452 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2114 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3673 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2810 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     7515 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      503 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/meta.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    13358 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      906 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/partial_reader.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      961 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/partial_sample.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5003 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/polygon.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.143676 deeplake-3.2.9/deeplake/core/query/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       82 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/query/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    12021 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/query/autocomplete.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    14324 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/query/filter.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     8905 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/query/query.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    19656 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/sample.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    22548 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/serialize.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.148200 deeplake-3.2.9/deeplake/core/storage/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      382 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      929 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    18306 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/gcs.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    12815 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/google_drive.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     8273 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/local.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    18687 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3526 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/memory.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6549 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/provider.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    22659 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/s3.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    47714 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tensor.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     7191 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tensor_link.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5152 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/test_serialize.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.151251 deeplake-3.2.9/deeplake/core/tests/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tests/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     7544 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tests/test_compression.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      691 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tests/test_compute.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      913 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tests/test_io.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4209 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tests/test_locking.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      654 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1425 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.153305 deeplake-3.2.9/deeplake/core/tiling/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tiling/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4547 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1701 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4731 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2893 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tiling/serialize.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1950 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2367 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.155973 deeplake-3.2.9/deeplake/core/transform/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      111 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/transform/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    39500 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/transform/test_transform.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    24686 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/transform/transform.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1560 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6267 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.158520 deeplake-3.2.9/deeplake/core/version_control/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/version_control/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1954 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5774 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2068 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4828 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    18757 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    82757 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.164086 deeplake-3.2.9/deeplake/enterprise/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      257 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5698 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    27064 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/dataloader.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3892 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    21065 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1664 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/test_query.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    22446 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1595 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/util.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1590 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/hooks.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4617 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/htype.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.164441 deeplake-3.2.9/deeplake/integrations/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       99 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/__init__.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.165111 deeplake-3.2.9/deeplake/integrations/huggingface/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       44 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4100 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.166735 deeplake-3.2.9/deeplake/integrations/mmdet/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      118 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    59631 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    19171 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.168899 deeplake-3.2.9/deeplake/integrations/pytorch/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       40 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4937 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    16740 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4994 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5010 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.170319 deeplake-3.2.9/deeplake/integrations/tf/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      135 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1224 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/tf/common.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2423 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5330 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.170924 deeplake-3.2.9/deeplake/integrations/wandb/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       21 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    11856 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.172026 deeplake-3.2.9/deeplake/requirements/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      294 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/requirements/common.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       71 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/requirements/docs.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      357 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/requirements/plugins.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      179 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/requirements/tests.txt
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.174083 deeplake-3.2.9/deeplake/tests/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/tests/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1404 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2547 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/tests/client_fixtures.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3931 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/tests/common.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3357 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    14022 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/tests/path_fixtures.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2248 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.194915 deeplake-3.2.9/deeplake/util/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       86 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3499 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/access_method.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      971 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/agreement.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1567 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/array_list.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      619 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2961 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/auto.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5329 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/bugout_reporter.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       54 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/bugout_token.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3606 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/cache_chain.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4435 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/casting.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      310 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/check_installation.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1197 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/check_latest_version.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3172 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/chunk_engine.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4534 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/class_label.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      231 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/compression.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1197 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/compute.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5381 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/connect_dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      351 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/creds.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      775 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      443 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/delete_entry.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    15912 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/diff.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4638 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/downsample.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       84 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/empty_sample.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    13964 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/encoder.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    28248 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/exceptions.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2026 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/exif.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1813 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/from_tfds.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      136 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/generate_id.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      306 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/hash.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2799 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/htype.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1517 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/image.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      873 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/invalid_view_op.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      154 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1001 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/iteration_warning.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      507 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/join_chunks.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6422 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/json.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6644 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/keys.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2949 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/link.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1646 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/logging.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    35704 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/merge.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2426 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/modified.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      903 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/notebook.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.201283 deeplake-3.2.9/deeplake/util/object_3d/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        1 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3374 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      185 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      185 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1021 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      695 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1323 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6188 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1663 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3221 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    10213 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     7187 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1160 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3669 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/path.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3337 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/pretty_print.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2682 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/remove_cache.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4007 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/scheduling.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2892 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/shape_interval.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      182 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/shuffle.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1153 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/split.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6762 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/storage.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1131 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tag.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      354 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/testing.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.204328 deeplake-3.2.9/deeplake/util/tests/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1476 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_auto.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1757 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1239 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      892 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_read.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1071 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      407 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      698 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_split.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      266 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_token.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2428 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      276 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/threading.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      381 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/token.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    19516 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/transform.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    23486 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/version_control.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      927 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/video.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      167 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/warnings.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.205289 deeplake-3.2.9/deeplake/visualizer/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       34 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/visualizer/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6466 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6680 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.080690 deeplake-3.2.9/deeplake.egg-info/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    24618 2023-02-20 14:49:32.000000 deeplake-3.2.9/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    10542 2023-02-20 14:49:33.000000 deeplake-3.2.9/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        1 2023-02-20 14:49:32.000000 deeplake-3.2.9/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       58 2023-02-20 14:49:32.000000 deeplake-3.2.9/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        1 2023-02-20 14:49:32.000000 deeplake-3.2.9/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      903 2023-02-20 14:49:32.000000 deeplake-3.2.9/deeplake.egg-info/requires.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        9 2023-02-20 14:49:32.000000 deeplake-3.2.9/deeplake.egg-info/top_level.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      311 2023-02-20 14:49:33.207116 deeplake-3.2.9/setup.cfg
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3329 2023-02-20 14:48:58.000000 deeplake-3.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.899397 deeplake-3.3.0/
+-rw-r--r--   0 root         (0) root         (0)    15975 2023-04-21 16:17:02.000000 deeplake-3.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-21 16:17:02.000000 deeplake-3.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    22282 2023-04-21 16:42:44.899397 deeplake-3.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21602 2023-04-21 16:17:02.000000 deeplake-3.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.866897 deeplake-3.3.0/deeplake/
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.866897 deeplake-3.3.0/deeplake/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    88813 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/info.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/link.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/api/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    79221 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     6439 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    23071 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 root         (0) root         (0)     6352 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_none.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     3308 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)    17730 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 root         (0) root         (0)     2331 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_text.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 root         (0) root         (0)     7389 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_video.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/api/tiled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/auto/structured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/structured/base.py
+-rw-r--r--   0 root         (0) root         (0)     6666 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/auto/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 root         (0) root         (0)    12440 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/auto/unstructured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7081 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4514 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12918 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5926 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/cli/auth.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/cli/commands.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/cli/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17970 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/client/config.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/client/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/compression.py
+-rw-r--r--   0 root         (0) root         (0)     5936 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/core/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/core/chunk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24150 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 root         (0) root         (0)     9632 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)   108709 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)    39478 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/compression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/core/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/compute/process.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/compute/provider.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/compute/ray.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/compute/serial.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/compute/thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   166412 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    14750 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11405 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.877730 deeplake-3.3.0/deeplake/core/index/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/index/index.py
+-rw-r--r--   0 root         (0) root         (0)    18879 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/io.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    11242 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/link_creds.py
+-rw-r--r--   0 root         (0) root         (0)    15953 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/linked_sample.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/meta/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/meta/encode/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25591 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     7515 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/meta.py
+-rw-r--r--   0 root         (0) root         (0)    13294 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/partial_reader.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/partial_sample.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/polygon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/query/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/query/filter.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    19976 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/sample.py
+-rw-r--r--   0 root         (0) root         (0)    23069 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/storage/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 root         (0) root         (0)    18475 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/gcs.py
+-rw-r--r--   0 root         (0) root         (0)    13053 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/local.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/memory.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/provider.py
+-rw-r--r--   0 root         (0) root         (0)    24900 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/storage/s3.py
+-rw-r--r--   0 root         (0) root         (0)    48988 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7404 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tensor_link.py
+-rw-r--r--   0 root         (0) root         (0)     5152 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    10122 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/tiling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4547 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/transform/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47159 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)    28835 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/transform/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5373 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/core/version_control/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 root         (0) root         (0)     5774 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 root         (0) root         (0)    19402 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)    84800 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/enterprise/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5745 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 root         (0) root         (0)    28992 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4349 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 root         (0) root         (0)    24153 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/test_query.py
+-rw-r--r--   0 root         (0) root         (0)    22695 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/enterprise/util.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     4890 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/htype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/integrations/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/integrations/huggingface/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5463 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/integrations/mmdet/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    61310 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/integrations/pytorch/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6052 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 root         (0) root         (0)     7073 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4053 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     5010 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/integrations/tf/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/tf/common.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/integrations/wandb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/requirements/
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/requirements/common.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      390 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/requirements/plugins.txt
+-rw-r--r--   0 root         (0) root         (0)      179 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/requirements/tests.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.888563 deeplake-3.3.0/deeplake/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)    15328 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.899397 deeplake-3.3.0/deeplake/util/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/access_method.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/agreement.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/array_list.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/auto.py
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-04-21 16:19:35.000000 deeplake-3.3.0/deeplake/util/bugout_token.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/cache_chain.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/casting.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/check_installation.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/check_latest_version.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/class_label.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/compression.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/compute.py
+-rw-r--r--   0 root         (0) root         (0)     5381 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/delete_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15912 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/diff.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/downsample.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/empty_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    34379 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/exif.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/from_tfds.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/generate_id.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/hash.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/htype.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/image.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/iteration_warning.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/join_chunks.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/json.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/keys.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/link.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/logging.py
+-rw-r--r--   0 root         (0) root         (0)    37298 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/merge.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/modified.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.899397 deeplake-3.3.0/deeplake/util/object_3d/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/pretty_print.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/remove_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     4206 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/split.py
+-rw-r--r--   0 root         (0) root         (0)     6762 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/storage.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tag.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.899397 deeplake-3.3.0/deeplake/util/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/threading.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/token.py
+-rw-r--r--   0 root         (0) root         (0)    23774 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/transform.py
+-rw-r--r--   0 root         (0) root         (0)    31017 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/version_control.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/video.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/util/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.899397 deeplake-3.3.0/deeplake/visualizer/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/visualizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-04-21 16:17:02.000000 deeplake-3.3.0/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 16:42:44.866897 deeplake-3.3.0/deeplake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22282 2023-04-21 16:42:44.000000 deeplake-3.3.0/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10849 2023-04-21 16:42:44.000000 deeplake-3.3.0/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 16:42:44.000000 deeplake-3.3.0/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-04-21 16:42:44.000000 deeplake-3.3.0/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 16:38:18.000000 deeplake-3.3.0/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      918 2023-04-21 16:42:44.000000 deeplake-3.3.0/deeplake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-21 16:42:44.000000 deeplake-3.3.0/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-04-21 16:42:44.899397 deeplake-3.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-04-21 16:17:02.000000 deeplake-3.3.0/setup.py
```

### Comparing `deeplake-3.2.9/PKG-INFO` & `deeplake-3.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,408 +1,413 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.2.9
+Version: 3.3.0
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
-Description: <img src="https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82" /><p align="center">
-             <img src="https://i.postimg.cc/rsjcWc3S/deeplake-logo.png" width="400"/>
-        </h1>
-            </br>
-            <h1 align="center">Deep Lake: Data Lake for Deep Learning
-         </h1>
-        <p align="center">
-            <a href="https://github.com/activeloopai/Hub/actions/workflows/test-pr-on-label.yml"><img src="https://github.com/activeloopai/Hub/actions/workflows/test-push.yml/badge.svg" alt="PyPI version" height="18"></a>
-            <a href="https://pypi.org/project/deeplake/"><img src="https://badge.fury.io/py/deeplake.svg" alt="PyPI version" height="18"></a>
-            <a href='https://docs.deeplake.ai/en/latest/?badge=latest'>
-             <img src='https://readthedocs.org/projects/deep-lake/badge/?version=latest' alt='Documentation Status' />
-             </a>
-            <a href="https://pepy.tech/project/deeplake"><img src="https://static.pepy.tech/personalized-badge/deeplake?period=month&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="PyPI version" height="18"></a>
-             <a href="https://github.com/activeloopai/deeplake/issues">
-            <img alt="GitHub issues" src="https://img.shields.io/github/issues/activeloopai/deeplake"> </a>
-            <a href="https://codecov.io/gh/activeloopai/deeplake/branch/main"><img src="https://codecov.io/gh/activeloopai/deeplake/branch/main/graph/badge.svg" alt="codecov" height="18"></a>
-          <h3 align="center">
-           <a href="https://docs.activeloop.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Documentation</b></a> &bull;
-           <a href="https://docs.activeloop.ai/getting-started/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Getting Started</b></a> &bull;
-           <a href="https://docs.deeplake.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>API Reference</b></a> &bull;  
-           <a href="https://github.com/activeloopai/examples/"><b>Examples</b></a> &bull; 
-           <a href="https://www.activeloop.ai/resources/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Blog</b></a> &bull; 
-           <a href="https://www.deeplake.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Whitepaper</b></a> &bull;  
-          <a href="http://slack.activeloop.ai"><b>Slack Community</b></a> &bull;
-          <a href="https://twitter.com/intent/tweet?text=The%20dataset%20format%20for%20AI.%20Stream%20data%20to%20PyTorch%20and%20Tensorflow%20datasets&url=https://activeloop.ai/&via=activeloopai&hashtags=opensource,pytorch,tensorflow,data,datascience,datapipelines,activeloop,databaseforAI"><b>Twitter</b></a>
-         </h3>
-         
-        
-        *Read this in other languages: [简体中文](README.zh-cn.md)*
-        
-        ## About Deep Lake
-        
-        Deep Lake (formerly known as Activeloop Hub) is a data lake for deep learning applications. Our open-source dataset format is optimized for rapid streaming and querying of data while training models at scale, and it includes a simple API for creating, storing, and collaborating on AI datasets of any size. It can be deployed locally or in the cloud, and it enables you to store all of your data in one place, ranging from simple annotations to large videos. Deep Lake is used by Google, Waymo, Red Cross, Omdena, Yale, & Oxford. Deep Lake includes the following features:
-        
-        <details>
-          <summary><b>Storage Agnostic API</b></summary>
-        Use one API to upload, download, and stream datasets to/from AWS S3/S3-compatible storage, GCP, Activeloop cloud, or local storage.
-        </details>
-        <details>
-          <summary><b>Native Compression</b></summary>
-        Store images, audios and videos in their native compression. Deeplake automatically decompresses them to raw data only when needed, e.g., when training a model.
-        </details>
-        <details>
-          <summary><b>Lazy NumPy-like Indexing</b></summary>
-        Treat your cloud datasets as if they are a collection of NumPy arrays in your system's memory. Slice them, index them, or iterate through them. Only the bytes you ask for will be downloaded!
-        </details>
-        <details>
-          <summary><b>Dataset Version Control</b></summary>
-        Commits, branches, checkout - Concepts you are already familiar with in your code repositories can now be applied to your datasets as well!
-        </details>
-        <details>
-          <summary><b>Dataloaders for Popular Deep Learning Frameworks</b></summary>
-        Deep Lake comes with built-in dataloaders for Pytorch and Tensorflow. Train your model with a few lines of code - we even take care of dataset shuffling. :)
-        </details>
-        <details>
-          <summary><b>Distributed Transformations</b></summary>
-        Rapidly apply transformations on your datasets using multi-threading, multi-processing, or our built-in <a href="https://www.ray.io/">Ray</a> integration.</details>
-        <details>
-          <summary><b>100+ most-popular image, video, and audio datasets available in seconds</b></summary>
-        Deep Lake community has uploaded <a href="https://docs.activeloop.ai/datasets/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">100+ image, video and audio datasets</a> like <a href="https://docs.activeloop.ai/datasets/mnist/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">MNIST</a>, <a href="https://docs.activeloop.ai/datasets/coco-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">COCO</a>,  <a href="https://docs.activeloop.ai/datasets/imagenet-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">ImageNet</a>,  <a href="https://docs.activeloop.ai/datasets/cifar-10-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">CIFAR</a>,  <a href="https://docs.activeloop.ai/datasets/gtzan-genre-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">GTZAN</a> and others.
-        </details>
-        </details>
-        <details>
-          <summary><b>Instant Visualization Support in <a href="https://app.activeloop.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">Activeloop Platform</a></b></summary>
-        Deep Lake datasets are instantly visualized with bounding boxes, masks, annotations, etc. in <a href="https://app.activeloop.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">Deep Lake Visualizer</a> (see below).
-        </details>
-        
-        <div align="center">
-        <a href="https://www.youtube.com/watch?v=SxsofpSIw3k"><img src="https://www.linkpicture.com/q/ReadMe.gif" type="image"></a>
-        </div>
-        
-            
-        ## 🚀 Performance
-        
-        Deep Lake's efficient enterprise dataloaders built in C++ speeds up data streaming by >2x compared to Hub 2.x (Ofeidis et al. 2022, Hambardzumyan et al. 2023) 
-        
-        <div align="center">
-        <a href="https://arxiv.org/pdf/2209.10785.pdf"><img src="docs/source/_static/img/benchmarks.png" type="image"></a>
-        </div>
-        
-        
-        ## Getting Started with Deep Lake
-        
-        
-        ### 🚀 How to install Deep Lake
-        Deep Lake's core is efficiently built in C++ and can be quickly installed using pip.
-        
-        ```sh
-        pip3 install deeplake
-        ```
-        
-        **By default, Deep Lake does not install dependencies for audio, video, google-cloud, and other features. Details on all installation options are [available here](https://docs.deeplake.ai/en/latest/Installation.html).**
-        
-        ### 🧠 How to Train a PyTorch model on a Deep Lake dataset
-        
-        #### Load CIFAR 10, one of the readily available datasets in Deep Lake:
-        
-        ```python
-        import deeplake
-        import torch
-        from torchvision import transforms, models
-        
-        ds = deeplake.load('hub://activeloop/cifar10-train')
-        ```
-        
-        #### Inspect tensors in the dataset:
-        
-        ```python
-        ds.tensors.keys()    # dict_keys(['images', 'labels'])
-        ds.labels[0].numpy() # array([6], dtype=uint32)
-        ```
-        
-        #### Train a PyTorch model on the CIFAR 10 dataset without the need to download it
-        
-        First, define a transform for the images and use Deep Lake's built-in PyTorch one-line dataloader to connect the data to the compute:
-        
-        ```python
-        tform = transforms.Compose([
-            transforms.ToTensor(),
-            transforms.Normalize([0.5, 0.5, 0.5], [0.5, 0.5, 0.5]),
-        ])
-        
-        deeplake_loader = ds.pytorch(num_workers=0, batch_size=4, transform={
-                                'images': tform, 'labels': None}, shuffle=True)
-        ```
-        
-        Next, define the model, loss and optimizer:
-        
-        ```python
-        net = models.resnet18(pretrained=False)
-        net.fc = torch.nn.Linear(net.fc.in_features, len(ds.labels.info.class_names))
-            
-        criterion = torch.nn.CrossEntropyLoss()
-        optimizer = torch.optim.SGD(net.parameters(), lr=0.001, momentum=0.9)
-        ```
-        
-        Finally, the training loop for 2 epochs:
-        
-        ```python
-        for epoch in range(2):
-            running_loss = 0.0
-            for i, data in enumerate(deeplake_loader):
-                images, labels = data['images'], data['labels']
-                
-                # zero the parameter gradients
-                optimizer.zero_grad()
-        
-                # forward + backward + optimize
-                outputs = net(images)
-                loss = criterion(outputs, labels.reshape(-1))
-                loss.backward()
-                optimizer.step()
-                
-                # print statistics
-                running_loss += loss.item()
-                if i % 100 == 99:    # print every 100 mini-batches
-                    print('[%d, %5d] loss: %.3f' %
-                        (epoch + 1, i + 1, running_loss / 100))
-                    running_loss = 0.0
-        ```
-        
-        
-        ### 🏗️ How to create a Deep Lake Dataset
-        
-        A Deep Lake dataset can be created in various locations (Storage providers). This is how the paths for each of them would look like:
-        
-        | Storage provider        | Example path                   |
-        | ----------------------- | ------------------------------ |
-        | Activeloop cloud        | hub://user_name/dataset_name   |
-        | AWS S3 / S3 compatible  | s3://bucket_name/dataset_name  |
-        | GCP                     | gcp://bucket_name/dataset_name |
-        | Google Drive            | gdrive://path_to_dataset
-        | Local storage           | path to local directory        |
-        | In-memory               | mem://dataset_name             |
-        
-        
-        
-        Let's create a dataset in the Activeloop cloud. Activeloop cloud provides free storage up to 300 GB per user (more info [here](#-for-students-and-educators)). Create a new account with Deep Lake from the terminal using `activeloop register` or in the [Deep Lake UI](https://app.activeloop.ai/register/). You will be asked for a user name, email ID, and password.
-        
-        ```sh
-        $ activeloop register
-        Enter your details. Your password must be at least 6 characters long.
-        Username:
-        Email:
-        Password:
-        ```
-        
-        After registration, an ORGANIZATION is automatically created that shares your username. You can use it for creating and managing your datasets, or you can create a new one for your company or team.
-        
-        Initialize an empty dataset in the Activeloop Cloud:
-        
-        ```python
-        import deeplake
-        
-        ds = deeplake.empty('hub://<ORGANIZATION_NAME>/test-dataset')
-        ```
-        
-        
-        Next, create a tensor to hold images in the dataset we just initialized:
-        
-        ```python
-        images = ds.create_tensor('images', htype='image', sample_compression='jpg')
-        ```
-        
-        Assuming you have a list of image file paths, let's upload them to the dataset:
-        
-        ```python
-        image_paths = ...
-        with ds:
-            for image_path in image_paths:
-                image = deeplake.read(image_path)
-                ds.images.append(image)
-        ```
-        
-        Alternatively, you can also upload numpy arrays. Since the `images` tensor was created with `sample_compression='jpg'`, the arrays will be compressed with jpeg compression.
-        
-        
-        ```python
-        import numpy as np
-        
-        with ds:
-            for _ in range(1000):  # 1000 random images
-                random_image = np.random.randint(0, 256, (100, 100, 3), dtype=np.uint8)  # 100x100 image with 3 channels
-                ds.images.append(random_image)
-        ```
-        
-        
-        
-        ### 🚀 How to load a Deep Lake Dataset
-        
-        
-        You can load the dataset you just created with a single line of code:
-        
-        ```python
-        import deeplake
-        
-        ds = deeplake.load('hub://<ORGANIZATION_NAME>/test-dataset')
-        ```
-        
-        You can also access one of the <a href="https://docs.activeloop.ai/datasets/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">100+ image, video and audio datasets in Deep Lake format</a>, not just the ones you created. Here is how you would load the [Objectron Bikes Dataset](https://github.com/google-research-datasets/Objectron):
-        
-        ```python
-        import deeplake
-        
-        ds = deeplake.load('hub://activeloop/objectron_bike_train')
-        ```
-        
-        To get the first image in the Objectron Bikes dataset in numpy format:
-        
-        
-        ```python
-        image_arr = ds.image[0].numpy()
-        ```
-        
-        ## ⚙️ Integrations
-        Deep Lake offers integrations with other tools in order to streamline your deep learning workflows. Current integrations include:
-        
-        * **Model Training**
-          * Stream data while training thousands of pre-built models using [MMDetection](https://github.com/open-mmlab/mmdetection), a popular open-source object detection toolbox based on PyTorch. Learn more in [this tutorial](https://docs.activeloop.ai/tutorials/training-models/training-models-using-mmdetection).
-          
-        * **Experiment Tracking**
-          * Track experiments and achieve full model reproducibility using Deep Lake and [Weights & Biases](https://wandb.ai/). Our integration automatically pushes dataset-related information (uri, commit hash, view id) to your W&B runs. Further details are available [in our model-reproducibility playbook](https://docs.activeloop.ai/playbooks/training-reproducibility-with-wandb).
-        
-        ## 📚 Documentation
-        Getting started guides, examples, tutorials, API reference, and other useful information can be found on our [documentation page](http://docs.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme). 
-        
-        ## 🎓 For Students and Educators
-        Deep Lake users can access and visualize a variety of popular datasets through a free integration with Activeloop's Platform. Users can also create and store their own datasets and make them available to the public. Free storage of up to 300 GB is available for students and educators:
-        
-        | <!-- -->    | <!-- -->    |
-        | ---------------------------------------------------- | ------------- |
-        | Storage for public datasets hosted by Activeloop     | 200GB Free    |
-        | Storage for private datasets hosted by Activeloop    | 100GB Free    |
-        
-        
-        
-        ## 👩‍💻 Comparisons to Familiar Tools
-        
-        
-        <details>
-          <summary><b>Deep Lake vs DVC</b></summary>
-          
-        Deep Lake and DVC offer dataset version control similar to git for data, but their methods for storing data differ significantly. Deep Lake converts and stores data as chunked compressed arrays, which enables rapid streaming to ML models, whereas DVC operates on top of data stored in less efficient traditional file structures. The Deep Lake format makes dataset versioning significantly easier compared to traditional file structures by DVC when datasets are composed of many files (i.e., many images). An additional distinction is that DVC primarily uses a command-line interface, whereas Deep Lake is a Python package. Lastly, Deep Lake offers an API to easily connect datasets to ML frameworks and other common ML tools and enables instant dataset visualization through [Activeloop's visualization tool](http://app.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme).
-        
-        </details>
-        
-        
-        <details>
-          <summary><b>Deep Lake vs TensorFlow Datasets (TFDS)</b></summary>
-          
-        Deep Lake and TFDS seamlessly connect popular datasets to ML frameworks. Deep Lake datasets are compatible with both PyTorch and TensorFlow, whereas TFDS are only compatible with TensorFlow. A key difference between Deep Lake and TFDS is that Deep Lake datasets are designed for streaming from the cloud, whereas TFDS must be downloaded locally prior to use. As a result, with Deep Lake, one can import datasets directly from TensorFlow Datasets and stream them either to PyTorch or TensorFlow. In addition to providing access to popular publicly available datasets, Deep Lake also offers powerful tools for creating custom datasets, storing them on a variety of cloud storage providers, and collaborating with others via simple API. TFDS is primarily focused on giving the public easy access to commonly available datasets, and management of custom datasets is not the primary focus. A full comparison article can be found [here](https://www.activeloop.ai/resources/tensor-flow-tf-data-activeloop-hub-how-to-implement-your-tensor-flow-data-pipelines-with-hub/).
-        
-        </details>
-        
-        
-        
-        <details>
-          <summary><b>Deep Lake vs HuggingFace</b></summary>
-        Deep Lake and HuggingFace offer access to popular datasets, but Deep Lake primarily focuses on computer vision, whereas HuggingFace focuses on natural language processing. HuggingFace Transforms and other computational tools for NLP are not analogous to features offered by Deep Lake.
-        
-        
-        </details>
-        
-        <details>
-          <summary><b>Deep Lake vs WebDatasets</b></summary>
-        Deep Lake and WebDatasets both offer rapid data streaming across networks. They have nearly identical steaming speeds because the underlying network requests and data structures are very similar. However, Deep Lake offers superior random access and shuffling, its simple API is in python instead of command-line, and Deep Lake enables simple indexing and modification of the dataset without having to recreate it.
-        
-        
-        </details>
-        
-        <details>
-          <summary><b>Deep Lake vs Zarr</b></summary>
-        Deep Lake and Zarr both offer storage of data as chunked arrays. However, Deep Lake is primarily designed for returning data as arrays using a simple API, rather than actually storing raw arrays (even though that's also possible). Deep Lake stores data in use-case-optimized formats, such as jpeg or png for images, or mp4 for video, and the user treats the data as if it's an array, because Deep Lake handles all the data processing in between. Deep Lake offers more flexibility for storing arrays with dynamic shape (ragged tensors), and it provides several features that are not naively available in Zarr such as version control, data streaming, and connecting data to ML Frameworks.
-        
-        
-        </details>
-        
-        ## Community
-        
-        Join our [**Slack community**](https://join.slack.com/t/hubdb/shared_invite/zt-ivhsj8sz-GWv9c5FLBDVw8vn~sxRKqQ) to learn more about unstructured dataset management using Deep Lake and to get help from the Activeloop team and other users.
-        
-        We'd love your feedback by completing our 3-minute [**survey**](https://forms.gle/rLi4w33dow6CSMcm9).
-        
-        As always, thanks to our amazing contributors!    
-        
-        <a href="https://github.com/activeloopai/deeplake/graphs/contributors">
-          <img src="https://contrib.rocks/image?repo=activeloopai/hub" />
-        </a>
-        
-        Made with [contributors-img](https://contrib.rocks).
-        
-        Please read [CONTRIBUTING.md](CONTRIBUTING.md) to get started with making contributions to Deep Lake.
-        
-        
-        ## README Badge
-        
-        Using Deep Lake? Add a README badge to let everyone know: 
-        
-        
-        [![deeplake](https://img.shields.io/badge/powered%20by-Deep%20Lake%20-ff5a1f.svg)](https://github.com/activeloopai/deeplake)
-        
-        ```
-        [![deeplake](https://img.shields.io/badge/powered%20by-Deep%20Lake%20-ff5a1f.svg)](https://github.com/activeloopai/deeplake)
-        ```
-        
-        
-        
-        ## Disclaimers
-        
-        <details>
-          <summary><b> Dataset Licenses</b></summary>
-          
-        Deep Lake users may have access to a variety of publicly available datasets. We do not host or distribute these datasets, vouch for their quality or fairness, or claim that you have a license to use the datasets. It is your responsibility to determine whether you have permission to use the datasets under their license.
-        
-        If you're a dataset owner and do not want your dataset to be included in this library, please get in touch through a [GitHub issue](https://github.com/activeloopai/deeplake/issues/new). Thank you for your contribution to the ML community!
-        
-        </details>
-        
-        <details>
-          <summary><b> Usage Tracking</b></summary>
-        
-        By default, we collect usage data using Bugout (here's the [code](https://github.com/activeloopai/deeplake/blob/853456a314b4fb5623c936c825601097b0685119/deeplake/__init__.py#L24) that does it). It does not collect user data other than anonymized IP address data, and it only logs the Deep Lake library's own actions. This helps our team understand how the tool is used and how to build features that matter to you! After you register with Activeloop, data is no longer anonymous. You can always opt-out of reporting using the CLI command below, or by setting an environmental variable ```BUGGER_OFF``` to ```True```:
-        
-        ```
-        activeloop reporting --off
-        ```
-        </details>
-        
-        ## Citation
-        If you use Deep Lake in your research, please cite Activeloop using:
-        
-        ```
-        @article{deeplake,
-          title = {Deep Lake: a Lakehouse for Deep Learning},
-          author = {Hambardzumyan, Sasun and Tuli, Abhinav and Ghukasyan, Levon and Rahman, Fariz and Topchyan, Hrant and Isayan, David and Harutyunyan, Mikayel and Hakobyan, Tatevik and Stranic, Ivo and Buniatyan, Davit},
-          url = {https://www.cidrdb.org/cidr2023/papers/p69-buniatyan.pdf},
-          booktitle={Proceedings of CIDR},
-          year = {2023},
-        }
-        ```
-        
-        ## Acknowledgment
-        This technology was inspired by our research work at Princeton University. We would like to thank William Silversmith @SeungLab for his awesome [cloud-volume](https://github.com/seung-lab/cloud-volume) tool.
-        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Description-Content-Type: text/markdown
+Provides-Extra: all
 Provides-Extra: audio
-Provides-Extra: video
 Provides-Extra: av
-Provides-Extra: gcp
 Provides-Extra: dicom
-Provides-Extra: medical
-Provides-Extra: visualizer
+Provides-Extra: gcp
 Provides-Extra: gdrive
+Provides-Extra: medical
 Provides-Extra: point_cloud
-Provides-Extra: all
-Provides-Extra: enterprise
+Provides-Extra: video
+Provides-Extra: visualizer
+License-File: LICENSE
+
+<img src="https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82" /><p align="center">
+     <img src="https://i.postimg.cc/rsjcWc3S/deeplake-logo.png" width="400"/>
+</h1>
+    </br>
+    <h1 align="center">Deep Lake: Data Lake for Deep Learning
+ </h1>
+<p align="center">
+    <a href="https://github.com/activeloopai/Hub/actions/workflows/test-pr-on-label.yml"><img src="https://github.com/activeloopai/Hub/actions/workflows/test-push.yml/badge.svg" alt="PyPI version" height="18"></a>
+    <a href="https://pypi.org/project/deeplake/"><img src="https://badge.fury.io/py/deeplake.svg" alt="PyPI version" height="18"></a>
+    <a href='https://docs.deeplake.ai/en/latest/?badge=latest'>
+     <img src='https://readthedocs.org/projects/deep-lake/badge/?version=latest' alt='Documentation Status' />
+     </a>
+    <a href="https://pepy.tech/project/deeplake"><img src="https://static.pepy.tech/badge/deeplake" alt="PyPI version" height="18"></a>
+     <a href="https://github.com/activeloopai/deeplake/issues">
+    <img alt="GitHub issues" src="https://img.shields.io/github/issues/activeloopai/deeplake"> </a>
+    <a href="https://codecov.io/gh/activeloopai/deeplake/branch/main"><img src="https://codecov.io/gh/activeloopai/deeplake/branch/main/graph/badge.svg" alt="codecov" height="18"></a>
+  <h3 align="center">
+   <a href="https://docs.activeloop.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Documentation</b></a> &bull;
+   <a href="https://docs.activeloop.ai/getting-started/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Getting Started</b></a> &bull;
+   <a href="https://docs.deeplake.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>API Reference</b></a> &bull;  
+   <a href="https://github.com/activeloopai/examples/"><b>Examples</b></a> &bull; 
+   <a href="https://www.activeloop.ai/resources/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Blog</b></a> &bull; 
+   <a href="https://www.deeplake.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Whitepaper</b></a> &bull;  
+  <a href="http://slack.activeloop.ai"><b>Slack Community</b></a> &bull;
+  <a href="https://twitter.com/intent/tweet?text=The%20dataset%20format%20for%20AI.%20Stream%20data%20to%20PyTorch%20and%20Tensorflow%20datasets&url=https://activeloop.ai/&via=activeloopai&hashtags=opensource,pytorch,tensorflow,data,datascience,datapipelines,activeloop,databaseforAI"><b>Twitter</b></a>
+ </h3>
+ 
+
+*Read this in other languages: [简体中文](README.zh-cn.md)*
+
+## About Deep Lake
+
+Deep Lake (formerly known as Activeloop Hub) is a data lake for deep learning applications. Our open-source dataset format is optimized for rapid streaming and querying of data while training models at scale, and it includes a simple API for creating, storing, and collaborating on AI datasets of any size. It can be deployed locally or in the cloud, and it enables you to store all of your data in one place, ranging from simple annotations to large videos. Deep Lake is used by Google, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep Lake includes the following features:
+
+<details>
+  <summary><b>Storage Agnostic API</b></summary>
+Use one API to upload, download, and stream datasets to/from AWS S3/S3-compatible storage, GCP, Activeloop cloud, or local storage.
+</details>
+<details>
+  <summary><b>Native Compression with Lazy NumPy-like Indexing</b></summary>
+Store images, audios and videos in their native compression. Slide, index, iterate and interact with your data like a collection of NumPy arrays in your system's memory. Deep Lake lazily loads data only when needed, e.g., when training a model.
+</details>
+<details>
+  <summary><b>Dataset Version Control</b></summary>
+Commits, branches, checkout - Concepts you are already familiar with in your code repositories can now be applied to your datasets as well!
+</details>
+<details>
+  <summary><b>Dataloaders for Popular Deep Learning Frameworks</b></summary>
+Deep Lake comes with built-in dataloaders for Pytorch and Tensorflow. Train your model with a few lines of code - we even take care of dataset shuffling. :)
+</details>
+<details>
+  <summary><b>Integrations with Popular Tools</b></summary>
+Deep Lake has integrations with <a href="https://github.com/hwchase17/langchain">Langchain</a> as a vector store for LLM apps, <a href="https://wandb.ai/">Weights & Biases</a> for data lineage during model training, and <a href="https://github.com/open-mmlab/mmdetection">MMDetection</a> for training object detection models.
+</details>
+<details>
+  <summary><b>Distributed Transformations</b></summary>
+Rapidly apply transformations on your datasets using multi-threading, multi-processing, or our built-in <a href="https://www.ray.io/">Ray</a> integration.</details>
+<details>
+  <summary><b>100+ most-popular image, video, and audio datasets available in seconds</b></summary>
+Deep Lake community has uploaded <a href="https://docs.activeloop.ai/datasets/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">100+ image, video and audio datasets</a> like <a href="https://docs.activeloop.ai/datasets/mnist/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">MNIST</a>, <a href="https://docs.activeloop.ai/datasets/coco-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">COCO</a>,  <a href="https://docs.activeloop.ai/datasets/imagenet-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">ImageNet</a>,  <a href="https://docs.activeloop.ai/datasets/cifar-10-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">CIFAR</a>,  <a href="https://docs.activeloop.ai/datasets/gtzan-genre-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">GTZAN</a> and others.
+</details>
+</details>
+<details>
+  <summary><b>Instant Visualization Support in <a href="https://app.activeloop.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">Activeloop Platform</a></b></summary>
+Deep Lake datasets are instantly visualized with bounding boxes, masks, annotations, etc. in <a href="https://app.activeloop.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">Deep Lake Visualizer</a> (see below).
+</details>
+
+<div align="center">
+<a href="https://www.youtube.com/watch?v=SxsofpSIw3k"><img src="https://www.linkpicture.com/q/ReadMe.gif" type="image"></a>
+</div>
+
+    
+## 🚀 Performance
+
+Deep Lake's efficient enterprise dataloaders built in C++ speeds up data streaming by >2x compared to Hub 2.x (Ofeidis et al. 2022, Hambardzumyan et al. 2023) 
+
+<div align="center">
+<a href="https://arxiv.org/pdf/2209.10785.pdf"><img src="docs/source/_static/img/benchmarks.png" type="image"></a>
+</div>
+
+
+## Getting Started with Deep Lake
+
+
+### 🚀 How to install Deep Lake
+Deep Lake's core is efficiently built in C++ and can be quickly installed using pip.
+
+```sh
+pip3 install deeplake
+```
+
+**By default, Deep Lake does not install dependencies for audio, video, google-cloud, and other features. Details on all installation options are [available here](https://docs.deeplake.ai/en/latest/Installation.html).**
+
+### 🧠 How to Train a PyTorch model on a Deep Lake dataset
+
+#### Load CIFAR 10, one of the readily available datasets in Deep Lake:
+
+```python
+import deeplake
+import torch
+from torchvision import transforms, models
+
+ds = deeplake.load('hub://activeloop/cifar10-train')
+```
+
+#### Inspect tensors in the dataset:
+
+```python
+ds.tensors.keys()    # dict_keys(['images', 'labels'])
+ds.labels[0].numpy() # array([6], dtype=uint32)
+```
+
+#### Train a PyTorch model on the CIFAR 10 dataset without the need to download it
+
+First, define a transform for the images and use Deep Lake's built-in PyTorch one-line dataloader to connect the data to the compute:
+
+```python
+tform = transforms.Compose([
+    transforms.ToTensor(),
+    transforms.Normalize([0.5, 0.5, 0.5], [0.5, 0.5, 0.5]),
+])
+
+deeplake_loader = ds.pytorch(num_workers=0, batch_size=4, transform={
+                        'images': tform, 'labels': None}, shuffle=True)
+```
+
+Next, define the model, loss and optimizer:
+
+```python
+net = models.resnet18(pretrained=False)
+net.fc = torch.nn.Linear(net.fc.in_features, len(ds.labels.info.class_names))
+    
+criterion = torch.nn.CrossEntropyLoss()
+optimizer = torch.optim.SGD(net.parameters(), lr=0.001, momentum=0.9)
+```
+
+Finally, the training loop for 2 epochs:
+
+```python
+for epoch in range(2):
+    running_loss = 0.0
+    for i, data in enumerate(deeplake_loader):
+        images, labels = data['images'], data['labels']
+        
+        # zero the parameter gradients
+        optimizer.zero_grad()
+
+        # forward + backward + optimize
+        outputs = net(images)
+        loss = criterion(outputs, labels.reshape(-1))
+        loss.backward()
+        optimizer.step()
+        
+        # print statistics
+        running_loss += loss.item()
+        if i % 100 == 99:    # print every 100 mini-batches
+            print('[%d, %5d] loss: %.3f' %
+                (epoch + 1, i + 1, running_loss / 100))
+            running_loss = 0.0
+```
+
+
+### 🏗️ How to create a Deep Lake Dataset
+
+A Deep Lake dataset can be created in various locations (Storage providers). This is how the paths for each of them would look like:
+
+| Storage provider        | Example path                   |
+| ----------------------- | ------------------------------ |
+| Activeloop cloud        | hub://user_name/dataset_name   |
+| AWS S3 / S3 compatible  | s3://bucket_name/dataset_name  |
+| GCP                     | gcp://bucket_name/dataset_name |
+| Google Drive            | gdrive://path_to_dataset
+| Local storage           | path to local directory        |
+| In-memory               | mem://dataset_name             |
+
+
+
+Let's create a dataset in the Activeloop cloud. Activeloop cloud provides free storage up to 300 GB per user (more info [here](#-for-students-and-educators)). Create a new account with Deep Lake from the terminal using `activeloop register` or in the [Deep Lake UI](https://app.activeloop.ai/register/). You will be asked for a user name, email ID, and password.
+
+```sh
+$ activeloop register
+Enter your details. Your password must be at least 6 characters long.
+Username:
+Email:
+Password:
+```
+
+After registration, an ORGANIZATION is automatically created that shares your username. You can use it for creating and managing your datasets, or you can create a new one for your company or team.
+
+Initialize an empty dataset in the Activeloop Cloud:
+
+```python
+import deeplake
+
+ds = deeplake.empty('hub://<ORGANIZATION_NAME>/test-dataset')
+```
+
+
+Next, create a tensor to hold images in the dataset we just initialized:
+
+```python
+images = ds.create_tensor('images', htype='image', sample_compression='jpg')
+```
+
+Assuming you have a list of image file paths, let's upload them to the dataset:
+
+```python
+image_paths = ...
+with ds:
+    for image_path in image_paths:
+        image = deeplake.read(image_path)
+        ds.images.append(image)
+```
+
+Alternatively, you can also upload numpy arrays. Since the `images` tensor was created with `sample_compression='jpg'`, the arrays will be compressed with jpeg compression.
+
+
+```python
+import numpy as np
+
+with ds:
+    for _ in range(1000):  # 1000 random images
+        random_image = np.random.randint(0, 256, (100, 100, 3), dtype=np.uint8)  # 100x100 image with 3 channels
+        ds.images.append(random_image)
+```
+
+
+
+### 🚀 How to load a Deep Lake Dataset
+
+
+You can load the dataset you just created with a single line of code:
+
+```python
+import deeplake
+
+ds = deeplake.load('hub://<ORGANIZATION_NAME>/test-dataset')
+```
+
+You can also access one of the <a href="https://docs.activeloop.ai/datasets/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">100+ image, video and audio datasets in Deep Lake format</a>, not just the ones you created. Here is how you would load the [Objectron Bikes Dataset](https://github.com/google-research-datasets/Objectron):
+
+```python
+import deeplake
+
+ds = deeplake.load('hub://activeloop/objectron_bike_train')
+```
+
+To get the first image in the Objectron Bikes dataset in numpy format:
+
+
+```python
+image_arr = ds.image[0].numpy()
+```
+
+## ⚙️ Integrations
+Deep Lake offers integrations with other tools in order to streamline your deep learning workflows. Current integrations include:
+
+* **Model Training**
+  * Stream data while training thousands of pre-built models using [MMDetection](https://github.com/open-mmlab/mmdetection), a popular open-source object detection toolbox based on PyTorch. Learn more in [this tutorial](https://docs.activeloop.ai/tutorials/training-models/training-models-using-mmdetection).
+  
+* **Experiment Tracking**
+  * Track experiments and achieve full model reproducibility using Deep Lake and [Weights & Biases](https://wandb.ai/). Our integration automatically pushes dataset-related information (uri, commit hash, view id) to your W&B runs. Further details are available [in our model-reproducibility playbook](https://docs.activeloop.ai/playbooks/training-reproducibility-with-wandb).
+  
+* **LLM Apps**
+  * Use [Deep Lake as a vector store for LLM apps](https://www.activeloop.ai/resources/ultimate-guide-to-lang-chain-deep-lake-build-chat-gpt-to-answer-questions-on-your-financial-data/). Our integration combines the [Langchain](https://github.com/hwchase17/langchain) [VectorStores API](https://python.langchain.com/en/latest/reference/modules/vectorstore.html?highlight=pinecone#langchain.vectorstores.DeepLake) with Deep Lake datasets as the underlying data storage. The integration is a serverless vector store that can be deployed locally or in a cloud of your choice. 
+
+## 📚 Documentation
+Getting started guides, examples, tutorials, API reference, and other useful information can be found on our [documentation page](http://docs.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme). 
+
+## 🎓 For Students and Educators
+Deep Lake users can access and visualize a variety of popular datasets through a free integration with Activeloop's Platform. Users can also create and store their own datasets and make them available to the public. Free storage of up to 300 GB is available for students and educators:
+
+| <!-- -->    | <!-- -->    |
+| ---------------------------------------------------- | ------------- |
+| Storage for public datasets hosted by Activeloop     | 200GB Free    |
+| Storage for private datasets hosted by Activeloop    | 100GB Free    |
+
+
+
+## 👩‍💻 Comparisons to Familiar Tools
+
+
+<details>
+  <summary><b>Deep Lake vs DVC</b></summary>
+  
+Deep Lake and DVC offer dataset version control similar to git for data, but their methods for storing data differ significantly. Deep Lake converts and stores data as chunked compressed arrays, which enables rapid streaming to ML models, whereas DVC operates on top of data stored in less efficient traditional file structures. The Deep Lake format makes dataset versioning significantly easier compared to traditional file structures by DVC when datasets are composed of many files (i.e., many images). An additional distinction is that DVC primarily uses a command-line interface, whereas Deep Lake is a Python package. Lastly, Deep Lake offers an API to easily connect datasets to ML frameworks and other common ML tools and enables instant dataset visualization through [Activeloop's visualization tool](http://app.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme).
+
+</details>
+
+
+<details>
+  <summary><b>Deep Lake vs TensorFlow Datasets (TFDS)</b></summary>
+  
+Deep Lake and TFDS seamlessly connect popular datasets to ML frameworks. Deep Lake datasets are compatible with both PyTorch and TensorFlow, whereas TFDS are only compatible with TensorFlow. A key difference between Deep Lake and TFDS is that Deep Lake datasets are designed for streaming from the cloud, whereas TFDS must be downloaded locally prior to use. As a result, with Deep Lake, one can import datasets directly from TensorFlow Datasets and stream them either to PyTorch or TensorFlow. In addition to providing access to popular publicly available datasets, Deep Lake also offers powerful tools for creating custom datasets, storing them on a variety of cloud storage providers, and collaborating with others via simple API. TFDS is primarily focused on giving the public easy access to commonly available datasets, and management of custom datasets is not the primary focus. A full comparison article can be found [here](https://www.activeloop.ai/resources/tensor-flow-tf-data-activeloop-hub-how-to-implement-your-tensor-flow-data-pipelines-with-hub/).
+
+</details>
+
+
+
+<details>
+  <summary><b>Deep Lake vs HuggingFace</b></summary>
+Deep Lake and HuggingFace offer access to popular datasets, but Deep Lake primarily focuses on computer vision, whereas HuggingFace focuses on natural language processing. HuggingFace Transforms and other computational tools for NLP are not analogous to features offered by Deep Lake.
+
+
+</details>
+
+<details>
+  <summary><b>Deep Lake vs WebDatasets</b></summary>
+Deep Lake and WebDatasets both offer rapid data streaming across networks. They have nearly identical steaming speeds because the underlying network requests and data structures are very similar. However, Deep Lake offers superior random access and shuffling, its simple API is in python instead of command-line, and Deep Lake enables simple indexing and modification of the dataset without having to recreate it.
+
+
+</details>
+
+<details>
+  <summary><b>Deep Lake vs Zarr</b></summary>
+Deep Lake and Zarr both offer storage of data as chunked arrays. However, Deep Lake is primarily designed for returning data as arrays using a simple API, rather than actually storing raw arrays (even though that's also possible). Deep Lake stores data in use-case-optimized formats, such as jpeg or png for images, or mp4 for video, and the user treats the data as if it's an array, because Deep Lake handles all the data processing in between. Deep Lake offers more flexibility for storing arrays with dynamic shape (ragged tensors), and it provides several features that are not naively available in Zarr such as version control, data streaming, and connecting data to ML Frameworks.
+
+
+</details>
+
+## Community
+
+Join our [**Slack community**](https://join.slack.com/t/hubdb/shared_invite/zt-ivhsj8sz-GWv9c5FLBDVw8vn~sxRKqQ) to learn more about unstructured dataset management using Deep Lake and to get help from the Activeloop team and other users.
+
+We'd love your feedback by completing our 3-minute [**survey**](https://forms.gle/rLi4w33dow6CSMcm9).
+
+As always, thanks to our amazing contributors!    
+
+<a href="https://github.com/activeloopai/deeplake/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=activeloopai/hub" />
+</a>
+
+Made with [contributors-img](https://contrib.rocks).
+
+Please read [CONTRIBUTING.md](CONTRIBUTING.md) to get started with making contributions to Deep Lake.
+
+
+## README Badge
+
+Using Deep Lake? Add a README badge to let everyone know: 
+
+
+[![deeplake](https://img.shields.io/badge/powered%20by-Deep%20Lake%20-ff5a1f.svg)](https://github.com/activeloopai/deeplake)
+
+```
+[![deeplake](https://img.shields.io/badge/powered%20by-Deep%20Lake%20-ff5a1f.svg)](https://github.com/activeloopai/deeplake)
+```
+
+
+
+## Disclaimers
+
+<details>
+  <summary><b> Dataset Licenses</b></summary>
+  
+Deep Lake users may have access to a variety of publicly available datasets. We do not host or distribute these datasets, vouch for their quality or fairness, or claim that you have a license to use the datasets. It is your responsibility to determine whether you have permission to use the datasets under their license.
+
+If you're a dataset owner and do not want your dataset to be included in this library, please get in touch through a [GitHub issue](https://github.com/activeloopai/deeplake/issues/new). Thank you for your contribution to the ML community!
+
+</details>
+
+<details>
+  <summary><b> Usage Tracking</b></summary>
+
+By default, we collect usage data using Bugout (here's the [code](https://github.com/activeloopai/deeplake/blob/853456a314b4fb5623c936c825601097b0685119/deeplake/__init__.py#L24) that does it). It does not collect user data other than anonymized IP address data, and it only logs the Deep Lake library's own actions. This helps our team understand how the tool is used and how to build features that matter to you! After you register with Activeloop, data is no longer anonymous. You can always opt-out of reporting using the CLI command below, or by setting an environmental variable ```BUGGER_OFF``` to ```True```:
+
+```
+activeloop reporting --off
+```
+</details>
+
+## Citation
+If you use Deep Lake in your research, please cite Activeloop using:
+
+```
+@article{deeplake,
+  title = {Deep Lake: a Lakehouse for Deep Learning},
+  author = {Hambardzumyan, Sasun and Tuli, Abhinav and Ghukasyan, Levon and Rahman, Fariz and Topchyan, Hrant and Isayan, David and Harutyunyan, Mikayel and Hakobyan, Tatevik and Stranic, Ivo and Buniatyan, Davit},
+  url = {https://www.cidrdb.org/cidr2023/papers/p69-buniatyan.pdf},
+  booktitle={Proceedings of CIDR},
+  year = {2023},
+}
+```
+
+## Acknowledgment
+This technology was inspired by our research work at Princeton University. We would like to thank William Silversmith @SeungLab for his awesome [cloud-volume](https://github.com/seung-lab/cloud-volume) tool.
+
+
```

#### html2text {}

```diff
@@ -1,47 +1,53 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.2.9 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.3.0 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
-deeplake Description: [https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-
-b8ea-f711c4d35b82]
+deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
+Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
+Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
+Provides-Extra: gcp Provides-Extra: gdrive Provides-Extra: medical Provides-
+Extra: point_cloud Provides-Extra: video Provides-Extra: visualizer License-
+File: LICENSE [https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-
+f711c4d35b82]
                [https://i.postimg.cc/rsjcWc3S/deeplake-logo.png]
              ****** Deep Lake: Data Lake for Deep Learning ******
   [PyPI_version] [PyPI_version] [Documentation_Status] [PyPI_version] [GitHub
                                issues] [codecov]
    **** Documentation • Getting_Started • API_Reference • Examples • Blog •
                   Whitepaper • Slack_Community • Twitter ****
 *Read this in other languages: [ç®ä½ä¸­æ](README.zh-cn.md)* ## About Deep
 Lake Deep Lake (formerly known as Activeloop Hub) is a data lake for deep
 learning applications. Our open-source dataset format is optimized for rapid
 streaming and querying of data while training models at scale, and it includes
 a simple API for creating, storing, and collaborating on AI datasets of any
 size. It can be deployed locally or in the cloud, and it enables you to store
 all of your data in one place, ranging from simple annotations to large videos.
-Deep Lake is used by Google, Waymo, Red Cross, Omdena, Yale, & Oxford. Deep
+Deep Lake is used by Google, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep
 Lake includes the following features:  Storage Agnostic API Use one API to
 upload, download, and stream datasets to/from AWS S3/S3-compatible storage,
-GCP, Activeloop cloud, or local storage.   Native Compression Store images,
-audios and videos in their native compression. Deeplake automatically
-decompresses them to raw data only when needed, e.g., when training a model.
-Lazy NumPy-like Indexing Treat your cloud datasets as if they are a collection
-of NumPy arrays in your system's memory. Slice them, index them, or iterate
-through them. Only the bytes you ask for will be downloaded!   Dataset Version
-Control Commits, branches, checkout - Concepts you are already familiar with in
-your code repositories can now be applied to your datasets as well!
-Dataloaders for Popular Deep Learning Frameworks Deep Lake comes with built-in
-dataloaders for Pytorch and Tensorflow. Train your model with a few lines of
-code - we even take care of dataset shuffling. :)   Distributed Transformations
-Rapidly apply transformations on your datasets using multi-threading, multi-
-processing, or our built-in Ray integration.  100+ most-popular image, video,
-and audio datasets available in seconds Deep Lake community has uploaded 100+
-image,_video_and_audio_datasets like MNIST, COCO, ImageNet, CIFAR, GTZAN and
-others.    Instant Visualization Support in Activeloop_Platform Deep Lake
-datasets are instantly visualized with bounding boxes, masks, annotations, etc.
-in Deep_Lake_Visualizer (see below).
+GCP, Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-
+like Indexing Store images, audios and videos in their native compression.
+Slide, index, iterate and interact with your data like a collection of NumPy
+arrays in your system's memory. Deep Lake lazily loads data only when needed,
+e.g., when training a model.   Dataset Version Control Commits, branches,
+checkout - Concepts you are already familiar with in your code repositories can
+now be applied to your datasets as well!   Dataloaders for Popular Deep
+Learning Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
+Tensorflow. Train your model with a few lines of code - we even take care of
+dataset shuffling. :)   Integrations with Popular Tools Deep Lake has
+integrations with Langchain as a vector store for LLM apps, Weights_&_Biases
+for data lineage during model training, and MMDetection for training object
+detection models.   Distributed Transformations Rapidly apply transformations
+on your datasets using multi-threading, multi-processing, or our built-in Ray
+integration.  100+ most-popular image, video, and audio datasets available in
+seconds Deep Lake community has uploaded 100+_image,_video_and_audio_datasets
+like MNIST, COCO, ImageNet, CIFAR, GTZAN and others.    Instant Visualization
+Support in Activeloop_Platform Deep Lake datasets are instantly visualized with
+bounding boxes, masks, annotations, etc. in Deep_Lake_Visualizer (see below).
                   [https://www.linkpicture.com/q/ReadMe.gif]
 ## ð Performance Deep Lake's efficient enterprise dataloaders built in C++
 speeds up data streaming by >2x compared to Hub 2.x (Ofeidis et al. 2022,
 Hambardzumyan et al. 2023)
                    [docs/source/_static/img/benchmarks.png]
 ## Getting Started with Deep Lake ### ð How to install Deep Lake Deep Lake's
 core is efficiently built in C++ and can be quickly installed using pip. ```sh
@@ -114,15 +120,23 @@
 mmlab/mmdetection), a popular open-source object detection toolbox based on
 PyTorch. Learn more in [this tutorial](https://docs.activeloop.ai/tutorials/
 training-models/training-models-using-mmdetection). * **Experiment Tracking** *
 Track experiments and achieve full model reproducibility using Deep Lake and
 [Weights & Biases](https://wandb.ai/). Our integration automatically pushes
 dataset-related information (uri, commit hash, view id) to your W&B runs.
 Further details are available [in our model-reproducibility playbook](https://
-docs.activeloop.ai/playbooks/training-reproducibility-with-wandb). ## ð
+docs.activeloop.ai/playbooks/training-reproducibility-with-wandb). * **LLM
+Apps** * Use [Deep Lake as a vector store for LLM apps](https://
+www.activeloop.ai/resources/ultimate-guide-to-lang-chain-deep-lake-build-chat-
+gpt-to-answer-questions-on-your-financial-data/). Our integration combines the
+[Langchain](https://github.com/hwchase17/langchain) [VectorStores API](https://
+python.langchain.com/en/latest/reference/modules/
+vectorstore.html?highlight=pinecone#langchain.vectorstores.DeepLake) with Deep
+Lake datasets as the underlying data storage. The integration is a serverless
+vector store that can be deployed locally or in a cloud of your choice. ## ð
 Documentation Getting started guides, examples, tutorials, API reference, and
 other useful information can be found on our [documentation page](http://
 docs.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme). ##
 ð For Students and Educators Deep Lake users can access and visualize a
 variety of popular datasets through a free integration with Activeloop's
 Platform. Users can also create and store their own datasets and make them
 available to the public. Free storage of up to 300 GB is available for students
@@ -209,13 +223,8 @@
 Deep Learning}, author = {Hambardzumyan, Sasun and Tuli, Abhinav and Ghukasyan,
 Levon and Rahman, Fariz and Topchyan, Hrant and Isayan, David and Harutyunyan,
 Mikayel and Hakobyan, Tatevik and Stranic, Ivo and Buniatyan, Davit}, url =
 {https://www.cidrdb.org/cidr2023/papers/p69-buniatyan.pdf}, booktitle=
 {Proceedings of CIDR}, year = {2023}, } ``` ## Acknowledgment This technology
 was inspired by our research work at Princeton University. We would like to
 thank William Silversmith @SeungLab for his awesome [cloud-volume](https://
-github.com/seung-lab/cloud-volume) tool. Platform: UNKNOWN Classifier: License
-:: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0) Description-Content-
-Type: text/markdown Provides-Extra: audio Provides-Extra: video Provides-Extra:
-av Provides-Extra: gcp Provides-Extra: dicom Provides-Extra: medical Provides-
-Extra: visualizer Provides-Extra: gdrive Provides-Extra: point_cloud Provides-
-Extra: all Provides-Extra: enterprise
+github.com/seung-lab/cloud-volume) tool.
```

### Comparing `deeplake-3.2.9/README.md` & `deeplake-3.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
  </h1>
 <p align="center">
     <a href="https://github.com/activeloopai/Hub/actions/workflows/test-pr-on-label.yml"><img src="https://github.com/activeloopai/Hub/actions/workflows/test-push.yml/badge.svg" alt="PyPI version" height="18"></a>
     <a href="https://pypi.org/project/deeplake/"><img src="https://badge.fury.io/py/deeplake.svg" alt="PyPI version" height="18"></a>
     <a href='https://docs.deeplake.ai/en/latest/?badge=latest'>
      <img src='https://readthedocs.org/projects/deep-lake/badge/?version=latest' alt='Documentation Status' />
      </a>
-    <a href="https://pepy.tech/project/deeplake"><img src="https://static.pepy.tech/personalized-badge/deeplake?period=month&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="PyPI version" height="18"></a>
+    <a href="https://pepy.tech/project/deeplake"><img src="https://static.pepy.tech/badge/deeplake" alt="PyPI version" height="18"></a>
      <a href="https://github.com/activeloopai/deeplake/issues">
     <img alt="GitHub issues" src="https://img.shields.io/github/issues/activeloopai/deeplake"> </a>
     <a href="https://codecov.io/gh/activeloopai/deeplake/branch/main"><img src="https://codecov.io/gh/activeloopai/deeplake/branch/main/graph/badge.svg" alt="codecov" height="18"></a>
   <h3 align="center">
    <a href="https://docs.activeloop.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Documentation</b></a> &bull;
    <a href="https://docs.activeloop.ai/getting-started/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Getting Started</b></a> &bull;
    <a href="https://docs.deeplake.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>API Reference</b></a> &bull;  
@@ -26,37 +26,37 @@
  </h3>
  
 
 *Read this in other languages: [简体中文](README.zh-cn.md)*
 
 ## About Deep Lake
 
-Deep Lake (formerly known as Activeloop Hub) is a data lake for deep learning applications. Our open-source dataset format is optimized for rapid streaming and querying of data while training models at scale, and it includes a simple API for creating, storing, and collaborating on AI datasets of any size. It can be deployed locally or in the cloud, and it enables you to store all of your data in one place, ranging from simple annotations to large videos. Deep Lake is used by Google, Waymo, Red Cross, Omdena, Yale, & Oxford. Deep Lake includes the following features:
+Deep Lake (formerly known as Activeloop Hub) is a data lake for deep learning applications. Our open-source dataset format is optimized for rapid streaming and querying of data while training models at scale, and it includes a simple API for creating, storing, and collaborating on AI datasets of any size. It can be deployed locally or in the cloud, and it enables you to store all of your data in one place, ranging from simple annotations to large videos. Deep Lake is used by Google, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep Lake includes the following features:
 
 <details>
   <summary><b>Storage Agnostic API</b></summary>
 Use one API to upload, download, and stream datasets to/from AWS S3/S3-compatible storage, GCP, Activeloop cloud, or local storage.
 </details>
 <details>
-  <summary><b>Native Compression</b></summary>
-Store images, audios and videos in their native compression. Deeplake automatically decompresses them to raw data only when needed, e.g., when training a model.
-</details>
-<details>
-  <summary><b>Lazy NumPy-like Indexing</b></summary>
-Treat your cloud datasets as if they are a collection of NumPy arrays in your system's memory. Slice them, index them, or iterate through them. Only the bytes you ask for will be downloaded!
+  <summary><b>Native Compression with Lazy NumPy-like Indexing</b></summary>
+Store images, audios and videos in their native compression. Slide, index, iterate and interact with your data like a collection of NumPy arrays in your system's memory. Deep Lake lazily loads data only when needed, e.g., when training a model.
 </details>
 <details>
   <summary><b>Dataset Version Control</b></summary>
 Commits, branches, checkout - Concepts you are already familiar with in your code repositories can now be applied to your datasets as well!
 </details>
 <details>
   <summary><b>Dataloaders for Popular Deep Learning Frameworks</b></summary>
 Deep Lake comes with built-in dataloaders for Pytorch and Tensorflow. Train your model with a few lines of code - we even take care of dataset shuffling. :)
 </details>
 <details>
+  <summary><b>Integrations with Popular Tools</b></summary>
+Deep Lake has integrations with <a href="https://github.com/hwchase17/langchain">Langchain</a> as a vector store for LLM apps, <a href="https://wandb.ai/">Weights & Biases</a> for data lineage during model training, and <a href="https://github.com/open-mmlab/mmdetection">MMDetection</a> for training object detection models.
+</details>
+<details>
   <summary><b>Distributed Transformations</b></summary>
 Rapidly apply transformations on your datasets using multi-threading, multi-processing, or our built-in <a href="https://www.ray.io/">Ray</a> integration.</details>
 <details>
   <summary><b>100+ most-popular image, video, and audio datasets available in seconds</b></summary>
 Deep Lake community has uploaded <a href="https://docs.activeloop.ai/datasets/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">100+ image, video and audio datasets</a> like <a href="https://docs.activeloop.ai/datasets/mnist/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">MNIST</a>, <a href="https://docs.activeloop.ai/datasets/coco-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">COCO</a>,  <a href="https://docs.activeloop.ai/datasets/imagenet-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">ImageNet</a>,  <a href="https://docs.activeloop.ai/datasets/cifar-10-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">CIFAR</a>,  <a href="https://docs.activeloop.ai/datasets/gtzan-genre-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">GTZAN</a> and others.
 </details>
 </details>
@@ -256,14 +256,17 @@
 Deep Lake offers integrations with other tools in order to streamline your deep learning workflows. Current integrations include:
 
 * **Model Training**
   * Stream data while training thousands of pre-built models using [MMDetection](https://github.com/open-mmlab/mmdetection), a popular open-source object detection toolbox based on PyTorch. Learn more in [this tutorial](https://docs.activeloop.ai/tutorials/training-models/training-models-using-mmdetection).
   
 * **Experiment Tracking**
   * Track experiments and achieve full model reproducibility using Deep Lake and [Weights & Biases](https://wandb.ai/). Our integration automatically pushes dataset-related information (uri, commit hash, view id) to your W&B runs. Further details are available [in our model-reproducibility playbook](https://docs.activeloop.ai/playbooks/training-reproducibility-with-wandb).
+  
+* **LLM Apps**
+  * Use [Deep Lake as a vector store for LLM apps](https://www.activeloop.ai/resources/ultimate-guide-to-lang-chain-deep-lake-build-chat-gpt-to-answer-questions-on-your-financial-data/). Our integration combines the [Langchain](https://github.com/hwchase17/langchain) [VectorStores API](https://python.langchain.com/en/latest/reference/modules/vectorstore.html?highlight=pinecone#langchain.vectorstores.DeepLake) with Deep Lake datasets as the underlying data storage. The integration is a serverless vector store that can be deployed locally or in a cloud of your choice. 
 
 ## 📚 Documentation
 Getting started guides, examples, tutorials, API reference, and other useful information can be found on our [documentation page](http://docs.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme). 
 
 ## 🎓 For Students and Educators
 Deep Lake users can access and visualize a variety of popular datasets through a free integration with Activeloop's Platform. Users can also create and store their own datasets and make them available to the public. Free storage of up to 300 GB is available for students and educators:
```

#### html2text {}

```diff
@@ -8,35 +8,36 @@
 *Read this in other languages: [ç®ä½ä¸­æ](README.zh-cn.md)* ## About Deep
 Lake Deep Lake (formerly known as Activeloop Hub) is a data lake for deep
 learning applications. Our open-source dataset format is optimized for rapid
 streaming and querying of data while training models at scale, and it includes
 a simple API for creating, storing, and collaborating on AI datasets of any
 size. It can be deployed locally or in the cloud, and it enables you to store
 all of your data in one place, ranging from simple annotations to large videos.
-Deep Lake is used by Google, Waymo, Red Cross, Omdena, Yale, & Oxford. Deep
+Deep Lake is used by Google, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep
 Lake includes the following features:  Storage Agnostic API Use one API to
 upload, download, and stream datasets to/from AWS S3/S3-compatible storage,
-GCP, Activeloop cloud, or local storage.   Native Compression Store images,
-audios and videos in their native compression. Deeplake automatically
-decompresses them to raw data only when needed, e.g., when training a model.
-Lazy NumPy-like Indexing Treat your cloud datasets as if they are a collection
-of NumPy arrays in your system's memory. Slice them, index them, or iterate
-through them. Only the bytes you ask for will be downloaded!   Dataset Version
-Control Commits, branches, checkout - Concepts you are already familiar with in
-your code repositories can now be applied to your datasets as well!
-Dataloaders for Popular Deep Learning Frameworks Deep Lake comes with built-in
-dataloaders for Pytorch and Tensorflow. Train your model with a few lines of
-code - we even take care of dataset shuffling. :)   Distributed Transformations
-Rapidly apply transformations on your datasets using multi-threading, multi-
-processing, or our built-in Ray integration.  100+ most-popular image, video,
-and audio datasets available in seconds Deep Lake community has uploaded 100+
-image,_video_and_audio_datasets like MNIST, COCO, ImageNet, CIFAR, GTZAN and
-others.    Instant Visualization Support in Activeloop_Platform Deep Lake
-datasets are instantly visualized with bounding boxes, masks, annotations, etc.
-in Deep_Lake_Visualizer (see below).
+GCP, Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-
+like Indexing Store images, audios and videos in their native compression.
+Slide, index, iterate and interact with your data like a collection of NumPy
+arrays in your system's memory. Deep Lake lazily loads data only when needed,
+e.g., when training a model.   Dataset Version Control Commits, branches,
+checkout - Concepts you are already familiar with in your code repositories can
+now be applied to your datasets as well!   Dataloaders for Popular Deep
+Learning Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
+Tensorflow. Train your model with a few lines of code - we even take care of
+dataset shuffling. :)   Integrations with Popular Tools Deep Lake has
+integrations with Langchain as a vector store for LLM apps, Weights_&_Biases
+for data lineage during model training, and MMDetection for training object
+detection models.   Distributed Transformations Rapidly apply transformations
+on your datasets using multi-threading, multi-processing, or our built-in Ray
+integration.  100+ most-popular image, video, and audio datasets available in
+seconds Deep Lake community has uploaded 100+_image,_video_and_audio_datasets
+like MNIST, COCO, ImageNet, CIFAR, GTZAN and others.    Instant Visualization
+Support in Activeloop_Platform Deep Lake datasets are instantly visualized with
+bounding boxes, masks, annotations, etc. in Deep_Lake_Visualizer (see below).
                   [https://www.linkpicture.com/q/ReadMe.gif]
 ## ð Performance Deep Lake's efficient enterprise dataloaders built in C++
 speeds up data streaming by >2x compared to Hub 2.x (Ofeidis et al. 2022,
 Hambardzumyan et al. 2023)
                    [docs/source/_static/img/benchmarks.png]
 ## Getting Started with Deep Lake ### ð How to install Deep Lake Deep Lake's
 core is efficiently built in C++ and can be quickly installed using pip. ```sh
@@ -109,15 +110,23 @@
 mmlab/mmdetection), a popular open-source object detection toolbox based on
 PyTorch. Learn more in [this tutorial](https://docs.activeloop.ai/tutorials/
 training-models/training-models-using-mmdetection). * **Experiment Tracking** *
 Track experiments and achieve full model reproducibility using Deep Lake and
 [Weights & Biases](https://wandb.ai/). Our integration automatically pushes
 dataset-related information (uri, commit hash, view id) to your W&B runs.
 Further details are available [in our model-reproducibility playbook](https://
-docs.activeloop.ai/playbooks/training-reproducibility-with-wandb). ## ð
+docs.activeloop.ai/playbooks/training-reproducibility-with-wandb). * **LLM
+Apps** * Use [Deep Lake as a vector store for LLM apps](https://
+www.activeloop.ai/resources/ultimate-guide-to-lang-chain-deep-lake-build-chat-
+gpt-to-answer-questions-on-your-financial-data/). Our integration combines the
+[Langchain](https://github.com/hwchase17/langchain) [VectorStores API](https://
+python.langchain.com/en/latest/reference/modules/
+vectorstore.html?highlight=pinecone#langchain.vectorstores.DeepLake) with Deep
+Lake datasets as the underlying data storage. The integration is a serverless
+vector store that can be deployed locally or in a cloud of your choice. ## ð
 Documentation Getting started guides, examples, tutorials, API reference, and
 other useful information can be found on our [documentation page](http://
 docs.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme). ##
 ð For Students and Educators Deep Lake users can access and visualize a
 variety of popular datasets through a free integration with Activeloop's
 Platform. Users can also create and store their own datasets and make them
 available to the public. Free storage of up to 300 GB is available for students
```

### Comparing `deeplake-3.2.9/deeplake/__init__.py` & `deeplake-3.3.0/deeplake/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 load = api_dataset.load
 empty = api_dataset.empty
 like = api_dataset.like
 delete = api_dataset.delete
 rename = api_dataset.rename
 copy = api_dataset.copy
 deepcopy = api_dataset.deepcopy
-ingest = api_dataset.ingest
 connect = api_dataset.connect
+ingest_classification = api_dataset.ingest_classification
 ingest_coco = api_dataset.ingest_coco
 ingest_yolo = api_dataset.ingest_yolo
 ingest_kaggle = api_dataset.ingest_kaggle
 ingest_dataframe = api_dataset.ingest_dataframe
 ingest_huggingface = huggingface.ingest_huggingface
 dataset = api_dataset.init  # type: ignore
 tensor = Tensor
@@ -75,15 +75,15 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.2.9"
+__version__ = "3.3.0"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
 deeplake_reporter.system_report(publish=True)
```

### Comparing `deeplake-3.2.9/deeplake/api/dataset.py` & `deeplake-3.3.0/deeplake/api/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,27 @@
 from deeplake.auto.unstructured.coco.coco import CocoDataset
 from deeplake.auto.unstructured.yolo.yolo import YoloDataset
 from deeplake.client.client import DeepLakeBackendClient
 from deeplake.client.log import logger
 from deeplake.core.dataset import Dataset, dataset_factory
 from deeplake.core.meta.dataset_meta import DatasetMeta
 from deeplake.util.connect_dataset import connect_dataset_entry
-from deeplake.util.path import convert_pathlib_to_string_if_needed, verify_dataset_name
+from deeplake.util.version_control import (
+    load_version_info,
+    rebuild_version_info,
+    get_parent_and_reset_commit_ids,
+    replace_head,
+    integrity_check,
+)
+from deeplake.util.spinner import spinner
+from deeplake.util.path import (
+    convert_pathlib_to_string_if_needed,
+    verify_dataset_name,
+    process_dataset_path,
+)
 from deeplake.hooks import (
     dataset_created,
     dataset_loaded,
     dataset_written,
     dataset_committed,
 )
 from deeplake.constants import (
@@ -39,58 +51,76 @@
 from deeplake.util.exceptions import (
     AgreementError,
     DatasetHandlerError,
     InvalidFileExtension,
     InvalidPathException,
     PathNotEmptyException,
     SamePathException,
-    AuthorizationException,
     UserNotLoggedInException,
     TokenPermissionError,
     UnsupportedParameterException,
+    DatasetCorruptError,
+    CheckoutError,
+    ReadOnlyModeError,
+    LockedException,
 )
 from deeplake.util.storage import (
     get_storage_and_cache_chain,
     storage_provider_from_path,
 )
 from deeplake.util.compute import get_compute_provider
 from deeplake.util.remove_cache import get_base_storage
 from deeplake.util.cache_chain import generate_chain
 from deeplake.core.storage.deeplake_memory_object import DeepLakeMemoryObject
 
 
 class dataset:
     @staticmethod
+    @spinner
     def init(
         path: Union[str, pathlib.Path],
         read_only: Optional[bool] = None,
         overwrite: bool = False,
         public: bool = False,
         memory_cache_size: int = DEFAULT_MEMORY_CACHE_SIZE,
         local_cache_size: int = DEFAULT_LOCAL_CACHE_SIZE,
         creds: Optional[Union[Dict, str]] = None,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         verbose: bool = True,
         access_method: str = "stream",
+        reset: bool = False,
     ):
         """Returns a :class:`~deeplake.core.dataset.Dataset` object referencing either a new or existing dataset.
 
         Examples:
 
             >>> ds = deeplake.dataset("hub://username/dataset")
             >>> ds = deeplake.dataset("s3://mybucket/my_dataset")
             >>> ds = deeplake.dataset("./datasets/my_dataset", overwrite=True)
 
+            Loading to a specfic version:
+
+            >>> ds = deeplake.dataset("hub://username/dataset@new_branch")
+            >>> ds = deeplake.dataset("hub://username/dataset@3e49cded62b6b335c74ff07e97f8451a37aca7b2)
+
+            >>> my_commit_id = "3e49cded62b6b335c74ff07e97f8451a37aca7b2"
+            >>> ds = deeplake.dataset(f"hub://username/dataset@{my_commit_id}")
+
         Args:
             path (str, pathlib.Path): - The full path to the dataset. Can be:
                 - a Deep Lake cloud path of the form ``hub://username/datasetname``. To write to Deep Lake cloud datasets, ensure that you are logged in to Deep Lake (use 'activeloop login' from command line)
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
+                - Loading to a specific version:
+
+                    - You can also specify a ``commit_id`` or ``branch`` to load the dataset to that version directly by using the ``@`` symbol.
+                    - The path will then be of the form ``hub://username/dataset@{branch}`` or ``hub://username/dataset@{commit_id}``.
+                    - See examples above.
             read_only (bool, optional): Opens dataset in read only mode if this is passed as ``True``. Defaults to ``False``.
                 Datasets stored on Deep Lake cloud that your account does not have write access to will automatically open in read mode.
             overwrite (bool): If set to ``True`` this overwrites the dataset if it already exists. Defaults to ``False``.
             public (bool): Defines if the dataset will have public access. Applicable only if Deep Lake cloud storage is used and a new Dataset is being created. Defaults to ``True``.
             memory_cache_size (int): The size of the memory cache to be used in MB.
             local_cache_size (int): The size of the local filesystem cache to be used in MB.
             creds (dict, optional): - A dictionary containing credentials used to access the dataset at the path.
@@ -117,37 +147,48 @@
                     - 'local'
 
                         - Downloads the dataset if it doesn't already exist, otherwise loads from local storage.
                         - Raises an exception if ``DEEPLAKE_DOWNLOAD_PATH`` environment variable is not set.
                         - The 'local' access method can be modified to specify num_workers and/or scheduler to be used in case dataset needs to be downloaded.
                           If dataset needs to be downloaded, 'local:2:processed' will use 2 workers and use processed scheduler, while 'local:3' will use 3 workers
                           and default scheduler (threaded), and 'local:processed' will use a single worker and use processed scheduler.
+            reset (bool): If the specified dataset cannot be loaded due to a corrupted HEAD state of the branch being loaded,
+                          setting ``reset=True`` will reset HEAD changes and load the previous version.
+
+        ..
+            # noqa: DAR101
 
         Returns:
             Dataset: Dataset created using the arguments provided.
 
         Raises:
             AgreementError: When agreement is rejected
             UserNotLoggedInException: When user is not logged in
             InvalidTokenException: If the specified token is invalid
             TokenPermissionError: When there are permission or other errors related to token
+            CheckoutError: If version address specified in the path cannot be found
+            DatasetCorruptError: If loading the dataset failed due to corruption and ``reset`` is not ``True``
+            ValueError: If version is specified in the path when creating a dataset
+            ReadOnlyModeError: If reset is attempted in read-only mode
+            LockedException: When attempting to open a dataset for writing when it is locked by another machine
+            Exception: Re-raises caught exception if reset cannot fix the issue
 
         Danger:
             Setting ``overwrite`` to ``True`` will delete all of your data if it exists! Be very careful when setting this parameter.
 
         Warning:
             Setting ``access_method`` to download will overwrite the local copy of the dataset if it was previously downloaded.
 
         Note:
             Any changes made to the dataset in download / local mode will only be made to the local copy and will not be reflected in the original dataset.
         """
         access_method, num_workers, scheduler = parse_access_method(access_method)
         check_access_method(access_method, overwrite)
-        path = convert_pathlib_to_string_if_needed(path)
 
+        path, address = process_dataset_path(path)
         verify_dataset_name(path)
 
         if creds is None:
             creds = {}
 
         try:
             storage, cache_chain = get_storage_and_cache_chain(
@@ -158,66 +199,84 @@
                 memory_cache_size=memory_cache_size,
                 local_cache_size=local_cache_size,
             )
 
             feature_report_path(path, "dataset", {"Overwrite": overwrite}, token=token)
         except Exception as e:
             if isinstance(e, UserNotLoggedInException):
-                message = (
-                    f"Please log in through the CLI in order to create this dataset, "
-                    "or create an API token in the UI and pass it to this method using "
-                    "the ‘token’ parameter. The CLI commands are ‘activeloop login’ and "
-                    "‘activeloop register."
-                )
-                raise UserNotLoggedInException(message)
+                raise UserNotLoggedInException from None
             raise
         ds_exists = dataset_exists(cache_chain)
 
         if ds_exists:
             if overwrite:
                 cache_chain.clear()
                 create = True
             else:
                 create = False
         else:
             create = True
 
-        try:
-            if access_method == "stream":
-                ret = dataset_factory(
-                    path=path,
-                    storage=cache_chain,
-                    read_only=read_only,
-                    public=public,
-                    token=token,
-                    org_id=org_id,
-                    verbose=verbose,
-                )
-                if create:
-                    dataset_created(ret)
-                else:
-                    dataset_loaded(ret)
-                return ret
+        if create and address:
+            raise ValueError(
+                "deeplake.dataset does not accept version address when writing a dataset."
+            )
 
-            return get_local_dataset(
-                access_method=access_method,
-                path=path,
-                read_only=read_only,
-                memory_cache_size=memory_cache_size,
-                local_cache_size=local_cache_size,
-                creds=creds,
-                token=token,
-                org_id=org_id,
-                verbose=verbose,
-                ds_exists=ds_exists,
-                num_workers=num_workers,
-                scheduler=scheduler,
+        dataset_kwargs: Dict[str, Union[None, str, bool, int, Dict]] = {
+            "path": path,
+            "read_only": read_only,
+            "token": token,
+            "org_id": org_id,
+            "verbose": verbose,
+        }
+
+        if access_method == "stream":
+            dataset_kwargs.update(
+                {
+                    "address": address,
+                    "storage": cache_chain,
+                    "public": public,
+                }
+            )
+        else:
+            dataset_kwargs.update(
+                {
+                    "access_method": access_method,
+                    "memory_cache_size": memory_cache_size,
+                    "local_cache_size": local_cache_size,
+                    "creds": creds,
+                    "ds_exists": ds_exists,
+                    "num_workers": num_workers,
+                    "scheduler": scheduler,
+                    "reset": reset,
+                }
             )
-        except AgreementError as e:
+
+        try:
+            return dataset._load(dataset_kwargs, access_method, create)
+        except (AgreementError, CheckoutError, LockedException) as e:
             raise e from None
+        except Exception as e:
+            if create:
+                raise e
+            if access_method == "stream":
+                if not reset:
+                    if isinstance(e, DatasetCorruptError):
+                        raise DatasetCorruptError(
+                            message=e.message,
+                            action="Try using `reset=True` to reset HEAD changes and load the previous commit.",
+                            cause=e.__cause__,
+                        )
+                    raise DatasetCorruptError(
+                        "Exception occured (see Traceback). The dataset maybe corrupted. "
+                        "Try using `reset=True` to reset HEAD changes and load the previous commit."
+                    ) from e
+                return dataset._reset_and_load(
+                    cache_chain, access_method, dataset_kwargs, address, e
+                )
 
     @staticmethod
     def exists(
         path: Union[str, pathlib.Path],
         creds: Optional[dict] = None,
         token: Optional[str] = None,
     ) -> bool:
@@ -226,16 +285,24 @@
         Args:
             path (str, pathlib.Path): the path which needs to be checked.
             creds (dict, optional): A dictionary containing credentials used to access the dataset at the path.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
 
         Returns:
             A boolean confirming whether the dataset exists or not at the given path.
+
+        Raises:
+            ValueError: If version is specified in the path
         """
-        path = convert_pathlib_to_string_if_needed(path)
+        path, address = process_dataset_path(path)
+
+        if address:
+            raise ValueError(
+                "deeplake.exists does not accept version address in the dataset path."
+            )
 
         if creds is None:
             creds = {}
         try:
             storage, cache_chain = get_storage_and_cache_chain(
                 path=path,
                 read_only=True,
@@ -284,19 +351,25 @@
             Dataset: Dataset created using the arguments provided.
 
         Raises:
             DatasetHandlerError: If a Dataset already exists at the given path and overwrite is False.
             UserNotLoggedInException: When user is not logged in
             InvalidTokenException: If the specified toke is invalid
             TokenPermissionError: When there are permission or other errors related to token
+            ValueError: If version is specified in the path
 
         Danger:
             Setting ``overwrite`` to ``True`` will delete all of your data if it exists! Be very careful when setting this parameter.
         """
-        path = convert_pathlib_to_string_if_needed(path)
+        path, address = process_dataset_path(path)
+
+        if address:
+            raise ValueError(
+                "deeplake.empty does not accept version address in the dataset path."
+            )
 
         verify_dataset_name(path)
 
         if creds is None:
             creds = {}
 
         try:
@@ -308,63 +381,79 @@
                 memory_cache_size=memory_cache_size,
                 local_cache_size=local_cache_size,
             )
 
             feature_report_path(path, "empty", {"Overwrite": overwrite}, token=token)
         except Exception as e:
             if isinstance(e, UserNotLoggedInException):
-                message = (
-                    f"Please log in through the CLI in order to create this dataset, "
-                    f"or create an API token in the UI and pass it to this method using the "
-                    f"‘token’ parameter. The CLI commands are ‘activeloop login’ and ‘activeloop register’."
-                )
-                raise UserNotLoggedInException(message)
+                raise UserNotLoggedInException from None
             raise
 
         if overwrite and dataset_exists(cache_chain):
             cache_chain.clear()
         elif dataset_exists(cache_chain):
             raise DatasetHandlerError(
                 f"A dataset already exists at the given path ({path}). If you want to create"
                 f" a new empty dataset, either specify another path or use overwrite=True. "
                 f"If you want to load the dataset that exists at this path, use deeplake.load() instead."
             )
-        read_only = storage.read_only
-        ret = dataset_factory(
-            path=path,
-            storage=cache_chain,
-            read_only=read_only,
-            public=public,
-            token=token,
-            org_id=org_id,
-            verbose=verbose,
-        )
-        dataset_created(ret)
+
+        dataset_kwargs = {
+            "path": path,
+            "storage": cache_chain,
+            "read_only": storage.read_only,
+            "public": public,
+            "token": token,
+            "org_id": org_id,
+            "verbose": verbose,
+        }
+        ret = dataset._load(dataset_kwargs)
         return ret
 
     @staticmethod
+    @spinner
     def load(
         path: Union[str, pathlib.Path],
         read_only: Optional[bool] = None,
         memory_cache_size: int = DEFAULT_MEMORY_CACHE_SIZE,
         local_cache_size: int = DEFAULT_LOCAL_CACHE_SIZE,
         creds: Optional[dict] = None,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         verbose: bool = True,
         access_method: str = "stream",
+        reset: bool = False,
     ) -> Dataset:
         """Loads an existing dataset
 
+        Examples:
+
+            >>> ds = deeplake.load("hub://username/dataset")
+            >>> ds = deeplake.load("s3://mybucket/my_dataset")
+            >>> ds = deeplake.load("./datasets/my_dataset", overwrite=True)
+
+            Loading to a specfic version:
+
+            >>> ds = deeplake.load("hub://username/dataset@new_branch")
+            >>> ds = deeplake.load("hub://username/dataset@3e49cded62b6b335c74ff07e97f8451a37aca7b2)
+
+            >>> my_commit_id = "3e49cded62b6b335c74ff07e97f8451a37aca7b2"
+            >>> ds = deeplake.load(f"hub://username/dataset@{my_commit_id}")
+
         Args:
             path (str, pathlib.Path): - The full path to the dataset. Can be:
                 - a Deep Lake cloud path of the form ``hub://username/datasetname``. To write to Deep Lake cloud datasets, ensure that you are logged in to Deep Lake (use 'activeloop login' from command line)
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
+                - Loading to a specific version:
+
+                        - You can also specify a ``commit_id`` or ``branch`` to load the dataset to that version directly by using the ``@`` symbol.
+                        - The path will then be of the form ``hub://username/dataset@{branch}`` or ``hub://username/dataset@{commit_id}``.
+                        - See examples above.
             read_only (bool, optional): Opens dataset in read only mode if this is passed as ``True``. Defaults to ``False``.
                 Datasets stored on Deep Lake cloud that your account does not have write access to will automatically open in read mode.
             memory_cache_size (int): The size of the memory cache to be used in MB.
             local_cache_size (int): The size of the local filesystem cache to be used in MB.
             creds (dict, optional): - A dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
@@ -389,92 +478,182 @@
                     - 'local'
 
                         - Downloads the dataset if it doesn't already exist, otherwise loads from local storage.
                         - Raises an exception if ``DEEPLAKE_DOWNLOAD_PATH`` environment variable is not set.
                         - The 'local' access method can be modified to specify num_workers and/or scheduler to be used in case dataset needs to be downloaded.
                           If dataset needs to be downloaded, 'local:2:processed' will use 2 workers and use processed scheduler, while 'local:3' will use 3 workers
                           and default scheduler (threaded), and 'local:processed' will use a single worker and use processed scheduler.
+            reset (bool): If the specified dataset cannot be loaded due to a corrupted HEAD state of the branch being loaded,
+                          setting ``reset=True`` will reset HEAD changes and load the previous version.
+
+        ..
+            # noqa: DAR101
 
         Returns:
             Dataset: Dataset loaded using the arguments provided.
 
         Raises:
             DatasetHandlerError: If a Dataset does not exist at the given path.
             AgreementError: When agreement is rejected
             UserNotLoggedInException: When user is not logged in
             InvalidTokenException: If the specified toke is invalid
             TokenPermissionError: When there are permission or other errors related to token
+            CheckoutError: If version address specified in the path cannot be found
+            DatasetCorruptError: If loading the dataset failed due to corruption and ``reset`` is not ``True``
+            ReadOnlyModeError: If reset is attempted in read-only mode
+            LockedException: When attempting to open a dataset for writing when it is locked by another machine
+            Exception: Re-raises caught exception if reset cannot fix the issue
 
         Warning:
             Setting ``access_method`` to download will overwrite the local copy of the dataset if it was previously downloaded.
 
         Note:
             Any changes made to the dataset in download / local mode will only be made to the local copy and will not be reflected in the original dataset.
         """
         access_method, num_workers, scheduler = parse_access_method(access_method)
         check_access_method(access_method, overwrite=False)
-        path = convert_pathlib_to_string_if_needed(path)
+
+        path, address = process_dataset_path(path)
 
         if creds is None:
             creds = {}
 
         try:
             storage, cache_chain = get_storage_and_cache_chain(
                 path=path,
                 read_only=read_only,
                 creds=creds,
                 token=token,
                 memory_cache_size=memory_cache_size,
                 local_cache_size=local_cache_size,
             )
-
             feature_report_path(path, "load", {}, token=token)
         except Exception as e:
             if isinstance(e, UserNotLoggedInException):
-                message = (
-                    "Please log in through the CLI in order to load this dataset, "
-                    "or create an API token in the UI and pass it to this method using "
-                    "the ‘token’ parameter. The CLI commands are ‘activeloop login’ and "
-                    "‘activeloop register’."
-                )
-                raise UserNotLoggedInException(message)
+                raise UserNotLoggedInException from None
             raise
         if not dataset_exists(cache_chain):
             raise DatasetHandlerError(
                 f"A Deep Lake dataset does not exist at the given path ({path}). Check the path provided or in case you want to create a new dataset, use deeplake.empty()."
             )
 
+        dataset_kwargs: Dict[str, Union[None, str, bool, int, Dict]] = {
+            "path": path,
+            "read_only": read_only,
+            "token": token,
+            "org_id": org_id,
+            "verbose": verbose,
+        }
+
+        if access_method == "stream":
+            dataset_kwargs.update(
+                {
+                    "address": address,
+                    "storage": cache_chain,
+                }
+            )
+        else:
+            dataset_kwargs.update(
+                {
+                    "access_method": access_method,
+                    "memory_cache_size": memory_cache_size,
+                    "local_cache_size": local_cache_size,
+                    "creds": creds,
+                    "ds_exists": True,
+                    "num_workers": num_workers,
+                    "scheduler": scheduler,
+                    "reset": reset,
+                }
+            )
+
         try:
+            return dataset._load(dataset_kwargs, access_method)
+        except (AgreementError, CheckoutError, LockedException) as e:
+            raise e from None
+        except Exception as e:
             if access_method == "stream":
-                ret = dataset_factory(
-                    path=path,
-                    storage=cache_chain,
-                    read_only=read_only,
-                    token=token,
-                    org_id=org_id,
-                    verbose=verbose,
+                if not reset:
+                    if isinstance(e, DatasetCorruptError):
+                        raise DatasetCorruptError(
+                            message=e.message,
+                            action="Try using `reset=True` to reset HEAD changes and load the previous commit.",
+                            cause=e.__cause__,
+                        )
+                    raise DatasetCorruptError(
+                        "Exception occured (see Traceback). The dataset maybe corrupted. "
+                        "Try using `reset=True` to reset HEAD changes and load the previous commit. "
+                        "This will delete all uncommitted changes on the branch you are trying to load."
+                    ) from e
+                return dataset._reset_and_load(
+                    cache_chain, access_method, dataset_kwargs, address, e
                 )
+            raise e
+
+    @staticmethod
+    def _reset_and_load(storage, access_method, dataset_kwargs, address, err):
+        """Reset and then load the dataset. Only called when loading dataset errored out with ``err``."""
+        if access_method != "stream":
+            dataset_kwargs["reset"] = True
+            ds = dataset._load(dataset_kwargs, access_method)
+            return ds
+
+        try:
+            version_info = load_version_info(storage)
+        except Exception:
+            raise err
+
+        address = address or "main"
+        parent_commit_id, reset_commit_id = get_parent_and_reset_commit_ids(
+            version_info, address
+        )
+        if parent_commit_id is False:
+            # non-head node corrupted
+            raise err
+        if storage.read_only:
+            msg = "Cannot reset when loading dataset in read-only mode."
+            if parent_commit_id:
+                msg += f" However, you can try loading the previous commit using "
+                msg += f"`deeplake.load('{dataset_kwargs.get('path')}@{parent_commit_id}')`."
+            raise ReadOnlyModeError(msg)
+        if parent_commit_id is None:
+            # no commits in the dataset
+            storage.clear()
+            ds = dataset._load(dataset_kwargs, access_method)
+            return ds
+
+        # load previous version, replace head and checkout to new head
+        dataset_kwargs["address"] = parent_commit_id
+        ds = dataset._load(dataset_kwargs, access_method)
+        new_commit_id = replace_head(storage, ds.version_state, reset_commit_id)
+        ds.checkout(new_commit_id)
+
+        current_node = ds.version_state["commit_node_map"][ds.commit_id]
+        verbose = dataset_kwargs.get("verbose")
+        if verbose:
+            logger.info(f"HEAD reset. Current version:\n{current_node}")
+        return ds
+
+    @staticmethod
+    def _load(dataset_kwargs, access_method=None, create=False):
+        if access_method in ("stream", None):
+            ret = dataset_factory(**dataset_kwargs)
+            if create:
+                dataset_created(ret)
+            else:
                 dataset_loaded(ret)
-                return ret
-            return get_local_dataset(
-                access_method=access_method,
-                path=path,
-                read_only=read_only,
-                memory_cache_size=memory_cache_size,
-                local_cache_size=local_cache_size,
-                creds=creds,
-                token=token,
-                org_id=org_id,
-                verbose=verbose,
-                ds_exists=True,
-                num_workers=num_workers,
-                scheduler=scheduler,
-            )
-        except AgreementError as e:
-            raise e from None
+
+            integrity_check(ret)
+
+            verbose = dataset_kwargs.get("verbose")
+            path = dataset_kwargs.get("path")
+            if verbose:
+                logger.info(f"{path} loaded successfully.")
+        else:
+            ret = get_local_dataset(**dataset_kwargs)
+        return ret
 
     @staticmethod
     def rename(
         old_path: Union[str, pathlib.Path],
         new_path: Union[str, pathlib.Path],
         creds: Optional[dict] = None,
         token: Optional[str] = None,
@@ -510,14 +689,15 @@
 
         ds = deeplake.load(old_path, verbose=False, token=token, creds=creds)
         ds.rename(new_path)
 
         return ds  # type: ignore
 
     @staticmethod
+    @spinner
     def delete(
         path: Union[str, pathlib.Path],
         force: bool = False,
         large_ok: bool = False,
         creds: Optional[dict] = None,
         token: Optional[str] = None,
         verbose: bool = False,
@@ -533,20 +713,27 @@
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             verbose (bool): If True, logs will be printed. Defaults to True.
 
         Raises:
             DatasetHandlerError: If a Dataset does not exist at the given path and ``force = False``.
+            UserNotLoggedInException: When user is not logged in.
             NotImplementedError: When attempting to delete a managed view.
+            ValueError: If version is specified in the path
 
         Warning:
             This is an irreversible operation. Data once deleted cannot be recovered.
         """
-        path = convert_pathlib_to_string_if_needed(path)
+        path, address = process_dataset_path(path)
+
+        if address:
+            raise ValueError(
+                "deeplake.delete does not accept version address in the dataset path."
+            )
 
         if creds is None:
             creds = {}
 
         feature_report_path(
             path, "delete", {"Force": force, "Large_OK": large_ok}, token=token
         )
@@ -554,15 +741,18 @@
         try:
             qtokens = ["/.queries/", "\\.queries\\"]
             for qt in qtokens:
                 if qt in path:
                     raise NotImplementedError(
                         "Deleting managed views by path is not supported. Load the source dataset and do `ds.delete_view(id)` instead."
                     )
-            ds = deeplake.load(path, verbose=False, token=token, creds=creds)
+            try:
+                ds = deeplake.load(path, verbose=False, token=token, creds=creds)
+            except UserNotLoggedInException:
+                raise UserNotLoggedInException from None
             ds.delete(large_ok=large_ok)
             if verbose:
                 logger.info(f"{path} dataset deleted successfully.")
         except Exception as e:
             if force:
                 base_storage = storage_provider_from_path(
                     path=path,
@@ -580,14 +770,15 @@
                         "A Deep Lake dataset wasn't found at the specified path. "
                         "This may be due to a corrupt dataset or a wrong path. "
                         "If you want to delete the data at the path regardless, use force=True"
                     )
                 raise
 
     @staticmethod
+    @spinner
     def like(
         dest: Union[str, pathlib.Path],
         src: Union[str, Dataset, pathlib.Path],
         tensors: Optional[List[str]] = None,
         overwrite: bool = False,
         creds: Optional[dict] = None,
         token: Optional[str] = None,
@@ -807,14 +998,15 @@
         Returns:
             Dataset: New dataset object.
 
         Raises:
             DatasetHandlerError: If a dataset already exists at destination path and overwrite is False.
             TypeError: If source is not a path to a dataset.
             UnsupportedParameterException: If parameter that is no longer supported is beeing called.
+            DatasetCorruptError: If loading source dataset fails with DatasetCorruptedError
         """
 
         if "src_token" in kwargs:
             raise UnsupportedParameterException(
                 "src_token is now not supported. You should use `token` instead."
             )
 
@@ -840,17 +1032,25 @@
             "Progressbar": progressbar,
             "Public": public,
         }
         if dest.startswith("hub://"):
             report_params["Dest"] = dest
         feature_report_path(src, "deepcopy", report_params, token=token)
 
-        src_ds = deeplake.load(
-            src, read_only=True, creds=src_creds, token=token, verbose=False
-        )
+        try:
+            src_ds = deeplake.load(
+                src, read_only=True, creds=src_creds, token=token, verbose=False
+            )
+        except DatasetCorruptError as e:
+            raise DatasetCorruptError(
+                "The source dataset is corrupted.",
+                "You can try to fix this by loading the dataset with `reset=True` "
+                "which will attempt to reset uncommitted HEAD changes and load the previous version.",
+                e.__cause__,
+            )
         src_storage = get_base_storage(src_ds.storage)
 
         dest_storage, cache_chain = get_storage_and_cache_chain(
             dest,
             creds=dest_creds,
             token=token,
             read_only=False,
@@ -945,15 +1145,15 @@
         if num_workers <= 1:
             keys = [keys]
         else:
             keys = [keys[i::num_workers] for i in range(num_workers)]
         compute_provider = get_compute_provider(scheduler, num_workers)
         try:
             if progressbar:
-                compute_provider.map_with_progressbar(
+                compute_provider.map_with_progress_bar(
                     copy_func_with_progress_bar,
                     keys,
                     len_keys,
                     "Copying dataset",
                 )
             else:
                 compute_provider.map(copy_func, keys)
@@ -971,14 +1171,15 @@
         dataset_created(ret)
         dataset_written(ret)
         if not ret.has_head_changes:
             dataset_committed(ret)
         return ret
 
     @staticmethod
+    @spinner
     def connect(
         src_path: str,
         creds_key: str,
         dest_path: Optional[str] = None,
         org_id: Optional[str] = None,
         ds_name: Optional[str] = None,
         token: Optional[str] = None,
@@ -1030,41 +1231,42 @@
         ignore_keys: Optional[List[str]] = None,
         image_params: Optional[Dict] = None,
         image_creds_key: Optional[str] = None,
         src_creds: Optional[Dict] = None,
         dest_creds: Optional[Dict] = None,
         inspect_limit: int = 1000000,
         progressbar: bool = True,
+        shuffle: bool = False,
         num_workers: int = 0,
         token: Optional[str] = None,
         connect_kwargs: Optional[Dict] = None,
         **dataset_kwargs,
     ) -> Dataset:
-        """Ingest images and annotations in COCO format to a Deep Lake Dataset.
+        """Ingest images and annotations in COCO format to a Deep Lake Dataset. The source data can be stored locally or in the cloud.
 
         Examples:
             >>> ds = deeplake.ingest_coco(
             >>>     "path/to/images/directory",
             >>>     ["path/to/annotation/file1.json", "path/to/annotation/file2.json"],
             >>>     dest="hub://org_id/dataset",
             >>>     key_to_tensor_mapping={"category_id": "labels", "bbox": "boxes"},
             >>>     file_to_group_mapping={"file1.json": "group1", "file2.json": "group2"},
             >>>     ignore_keys=["area", "image_id", "id"],
             >>>     token="my_activeloop_token",
             >>>     num_workers=4,
             >>> )
-            >>> # or ingest data from cloud
+            >>> # or ingest data from the cloud
             >>> ds = deeplake.ingest_coco(
             >>>     "s3://bucket/images/directory",
             >>>     "s3://bucket/annotation/file1.json",
             >>>     dest="hub://org_id/dataset_name",
             >>>     ignore_one_group=True,
             >>>     ignore_keys=["area", "image_id", "id"],
             >>>     image_settings={"name": "images", "htype": "link[image]", "sample_compression": "jpeg"},
-            >>>     image_creds_key="my_managed_creds"
+            >>>     image_creds_key="my_s3_managed_credentials"
             >>>     src_creds=aws_creds, # Can also be inferred from environment
             >>>     token="my_activeloop_token",
             >>>     num_workers=4,
             >>> )
 
         Args:
             images_directory (str, pathlib.Path): The path to the directory containing images.
@@ -1076,19 +1278,20 @@
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
             key_to_tensor_mapping (Optional[Dict]): A one-to-one mapping between COCO keys and Dataset tensor names.
             file_to_group_mapping (Optional[Dict]): A one-to-one mapping between COCO annotation file names and Dataset group names.
             ignore_one_group (bool): Skip creation of group in case of a single annotation file. Set to ``False`` by default.
             ignore_keys (List[str]): A list of COCO keys to ignore.
             image_params (Optional[Dict]): A dictionary containing parameters for the images tensor.
-            image_creds_key (Optional[str]): The name of the managed credentials to use for accessing the images directory via linked tensor.
-            src_creds (Optional[Dict]): Credentials to access the source path. If not provided, will be inferred from the environment.
+            image_creds_key (Optional[str]): The name of the managed credentials to use for accessing the images in the linked tensor (is applicable).
+            src_creds (Optional[Dict]): Credentials to access the source data. If not provided, will be inferred from the environment.
             dest_creds (Optional[Dict]): A dictionary containing credentials used to access the destination path of the dataset.
             inspect_limit (int): The maximum number of samples to inspect in the annotations json, in order to generate the set of COCO annotation keys. Set to ``1000000`` by default.
             progressbar (bool): Enables or disables ingestion progress bar. Set to ``True`` by default.
+            shuffle (bool): Shuffles the input data prior to ingestion. Set to ``False`` by default.
             num_workers (int): The number of workers to use for ingestion. Set to ``0`` by default.
             token (Optional[str]): The token to use for accessing the dataset and/or connecting it to Deep Lake.
             connect_kwargs (Optional[Dict]): If specified, the dataset will be connected to Deep Lake, and connect_kwargs will be passed to :meth:`Dataset.connect <deeplake.core.dataset.Dataset.connect>`.
             **dataset_kwargs: Any arguments passed here will be forwarded to the dataset creator function. See :func:`deeplake.empty`.
 
         Returns:
             Dataset: The Dataset created from images and COCO annotations.
@@ -1125,24 +1328,20 @@
         )
         structure = unstructured.prepare_structure(inspect_limit)
 
         ds = deeplake.empty(
             dest, creds=dest_creds, verbose=False, token=token, **dataset_kwargs
         )
         if connect_kwargs is not None:
-            connect_kwargs["token"] = token or connect_kwargs.get(token)
+            connect_kwargs["token"] = token or connect_kwargs.get("token")
             ds.connect(**connect_kwargs)
 
         structure.create_missing(ds)
 
-        unstructured.structure(
-            ds,
-            progressbar,
-            num_workers,
-        )
+        unstructured.structure(ds, progressbar, num_workers, shuffle)
 
         return ds
 
     @staticmethod
     def ingest_yolo(
         data_directory: Union[str, pathlib.Path],
         dest: Union[str, pathlib.Path],
@@ -1153,35 +1352,36 @@
         label_params: Optional[Dict] = None,
         coordinates_params: Optional[Dict] = None,
         src_creds: Optional[Dict] = None,
         dest_creds: Optional[Dict] = None,
         image_creds_key: Optional[str] = None,
         inspect_limit: int = 1000,
         progressbar: bool = True,
+        shuffle: bool = False,
         num_workers: int = 0,
         token: Optional[str] = None,
         connect_kwargs: Optional[Dict] = None,
         **dataset_kwargs,
     ) -> Dataset:
-        """Ingest images and annotations (bounding boxes or polygons) in YOLO format to a Deep Lake Dataset.
+        """Ingest images and annotations (bounding boxes or polygons) in YOLO format to a Deep Lake Dataset. The source data can be stored locally or in the cloud.
 
         Examples:
             >>> ds = deeplake.ingest_yolo(
             >>>     "path/to/data/directory",
             >>>     dest="hub://org_id/dataset",
             >>>     allow_no_annotation=True,
             >>>     token="my_activeloop_token",
             >>>     num_workers=4,
             >>> )
-            >>> # or ingest data from cloud
+            >>> # or ingest data from the cloud
             >>> ds = deeplake.ingest_yolo(
             >>>     "s3://bucket/data_directory",
             >>>     dest="hub://org_id/dataset",
             >>>     image_params={"name": "image_links", "htype": "link[image]"},
-            >>>     image_creds_key='my_s3_managed_crerendials",
+            >>>     image_creds_key="my_s3_managed_credentials",
             >>>     src_creds=aws_creds, # Can also be inferred from environment
             >>>     token="my_activeloop_token",
             >>>     num_workers=4,
             >>> )
 
         Args:
             data_directory (str, pathlib.Path): The path to the directory containing the data (images files and annotation files(see 'annotations_directory' input for specifying annotations in a separate directory).
@@ -1193,19 +1393,20 @@
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
             class_names_file: Path to the file containing the class names on separate lines. This is typically a file titled classes.names.
             annotations_directory (Optional[Union[str, pathlib.Path]]): Path to directory containing the annotations. If specified, the 'data_directory' will not be examined for annotations.
             allow_no_annotation (bool): Flag to determine whether missing annotations files corresponding to an image should be treated as empty annoations. Set to ``False`` by default.
             image_params (Optional[Dict]): A dictionary containing parameters for the images tensor.
             label_params (Optional[Dict]): A dictionary containing parameters for the labels tensor.
             coordinates_params (Optional[Dict]): A dictionary containing parameters for the ccoordinates tensor. This tensor either contains bounding boxes or polygons.
-            src_creds (Optional[Dict]): Credentials to access the source path. If not provided, will be inferred from the environment.
+            src_creds (Optional[Dict]): Credentials to access the source data. If not provided, will be inferred from the environment.
             dest_creds (Optional[Dict]): A dictionary containing credentials used to access the destination path of the dataset.
             image_creds_key (Optional[str]): creds_key for linked tensors, applicable if the htype for the images tensor is specified as 'link[image]' in the 'image_params' input.
             inspect_limit (int): The maximum number of annotations to inspect, in order to infer whether they are bounding boxes of polygons. This in put is ignored if the htype is specfied in the 'coordinates_params'.
             progressbar (bool): Enables or disables ingestion progress bar. Set to ``True`` by default.
+            shuffle (bool): Shuffles the input data prior to ingestion. Set to ``False`` by default.
             num_workers (int): The number of workers to use for ingestion. Set to ``0`` by default.
             token (Optional[str]): The token to use for accessing the dataset and/or connecting it to Deep Lake.
             connect_kwargs (Optional[Dict]): If specified, the dataset will be connected to Deep Lake, and connect_kwargs will be passed to :meth:`Dataset.connect <deeplake.core.dataset.Dataset.connect>`.
             **dataset_kwargs: Any arguments passed here will be forwarded to the dataset creator function. See :func:`deeplake.empty`.
 
         Returns:
             Dataset: The Dataset created from the images and YOLO annotations.
@@ -1260,42 +1461,53 @@
 
         structure.create_missing(ds)
 
         unstructured.structure(
             ds,
             progressbar,
             num_workers,
+            shuffle,
         )
 
         return ds
 
     @staticmethod
-    def ingest(
+    def ingest_classification(
         src: Union[str, pathlib.Path],
         dest: Union[str, pathlib.Path],
-        images_compression: str = "auto",
+        image_params: Optional[Dict] = None,
+        label_params: Optional[Dict] = None,
         dest_creds: Optional[Dict] = None,
         progressbar: bool = True,
         summary: bool = True,
+        num_workers: int = 0,
+        shuffle: bool = True,
+        token: Optional[str] = None,
+        connect_kwargs: Optional[Dict] = None,
         **dataset_kwargs,
     ) -> Dataset:
-        """Ingests a dataset from a source and stores it as a structured dataset to destination.
+        """Ingest a dataset of images from a local folder to a Deep Lake Dataset. Images should be stored in subfolders by class name.
 
         Args:
-            src (str, pathlib.Path): Local path to where the unstructured dataset is stored or path to csv file.
+            src (str, pathlib.Path): Local path to where the unstructured dataset of images is stored or path to csv file.
             dest (str, pathlib.Path): - The full path to the dataset. Can be:
-                - a Deep Lake cloud path of the form ``hub://username/datasetname``. To write to Deep Lake cloud datasets, ensure that you are logged in to Deep Lake (use 'activeloop login' from command line)
+                - a Deep Lake cloud path of the form ``hub://org_id/datasetname``. To write to Deep Lake cloud datasets, ensure that you are logged in to Deep Lake (use 'activeloop login' from command line)
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
-            images_compression (str): For image classification datasets, this compression will be used for the `images` tensor. If ``images_compression`` is "auto", compression will be automatically determined by the most common extension in the directory.
+            image_params (Optional[Dict]): A dictionary containing parameters for the images tensor.
+            label_params (Optional[Dict]): A dictionary containing parameters for the labels tensor.
             dest_creds (Optional[Dict]): A dictionary containing credentials used to access the destination path of the dataset.
             progressbar (bool): Enables or disables ingestion progress bar. Defaults to ``True``.
             summary (bool): If ``True``, a summary of skipped files will be printed after completion. Defaults to ``True``.
-            **dataset_kwargs: Any arguments passed here will be forwarded to the dataset creator function.
+            num_workers (int): The number of workers to use for ingestion. Set to ``0`` by default.
+            shuffle (bool): Shuffles the input data prior to ingestion. Since data arranged in folders by class is highly non-random, shuffling is important in order to produce optimal results when training. Defaults to ``True``.
+            token (Optional[str]): The token to use for accessing the dataset.
+            connect_kwargs (Optional[Dict]): If specified, the dataset will be connected to Deep Lake, and connect_kwargs will be passed to :meth:`Dataset.connect <deeplake.core.dataset.Dataset.connect>`.
+            **dataset_kwargs: Any arguments passed here will be forwarded to the dataset creator function see :func:`deeplake.empty`.
 
         Returns:
             Dataset: New dataset object with structured dataset.
 
         Raises:
             InvalidPathException: If the source directory does not exist.
             SamePathException: If the source and destination path are same.
@@ -1342,73 +1554,93 @@
             - Classes defined as sub-directories can be accessed at ``ds["test/labels"].info.class_names``.
             - Support for train and test sub directories is present under ``ds["train/images"]``, ``ds["train/labels"]`` and ``ds["test/images"]``, ``ds["test/labels"]``.
             - Mapping filenames to classes from an external file is currently not supported.
         """
         dest = convert_pathlib_to_string_if_needed(dest)
         feature_report_path(
             dest,
-            "ingest",
+            "ingest_classification",
             {
-                "Images_Compression": images_compression,
                 "Progressbar": progressbar,
                 "Summary": summary,
             },
-            token=dataset_kwargs.get("token", None),
+            token=token,
         )
 
         src = convert_pathlib_to_string_if_needed(src)
 
         if isinstance(src, str):
             if os.path.isdir(dest) and os.path.samefile(src, dest):
                 raise SamePathException(src)
 
-            if src.endswith(".csv"):
+            if src.lower().endswith((".csv", ".txt")):
                 import pandas as pd  # type:ignore
 
                 if not os.path.isfile(src):
                     raise InvalidPathException(src)
                 source = pd.read_csv(src, quotechar='"', skipinitialspace=True)
                 ds = dataset.ingest_dataframe(
-                    source, dest, dest_creds, progressbar, **dataset_kwargs
+                    source,
+                    dest,
+                    dest_creds=dest_creds,
+                    progressbar=progressbar,
+                    token=token,
+                    **dataset_kwargs,
                 )
                 return ds
 
             if not os.path.isdir(src):
                 raise InvalidPathException(src)
 
-            if images_compression == "auto":
+            if image_params is None:
+                image_params = {}
+            if label_params is None:
+                label_params = {}
+
+            if not image_params.get("sample_compression", None):
                 images_compression = get_most_common_extension(src)
                 if images_compression is None:
                     raise InvalidFileExtension(src)
+                image_params["sample_compression"] = images_compression
 
             # TODO: support more than just image classification (and update docstring)
             unstructured = ImageClassification(source=src)
 
-            ds = deeplake.dataset(dest, creds=dest_creds, **dataset_kwargs)
+            ds = deeplake.empty(
+                dest, creds=dest_creds, token=token, verbose=False, **dataset_kwargs
+            )
+            if connect_kwargs is not None:
+                connect_kwargs["token"] = token or connect_kwargs.get("token")
+                ds.connect(**connect_kwargs)
 
             # TODO: auto detect compression
             unstructured.structure(
                 ds,  # type: ignore
                 progressbar=progressbar,
                 generate_summary=summary,
-                image_tensor_args={"sample_compression": images_compression},
+                image_tensor_args=image_params,
+                label_tensor_args=label_params,
+                num_workers=num_workers,
+                shuffle=shuffle,
             )
+
         return ds  # type: ignore
 
     @staticmethod
     def ingest_kaggle(
         tag: str,
         src: Union[str, pathlib.Path],
         dest: Union[str, pathlib.Path],
         exist_ok: bool = False,
         images_compression: str = "auto",
         dest_creds: Optional[Dict] = None,
         kaggle_credentials: Optional[dict] = None,
         progressbar: bool = True,
         summary: bool = True,
+        shuffle: bool = True,
         **dataset_kwargs,
     ) -> Dataset:
         """Download and ingest a kaggle dataset and store it as a structured dataset to destination.
 
         Args:
             tag (str): Kaggle dataset tag. Example: ``"coloradokb/dandelionimages"`` points to https://www.kaggle.com/coloradokb/dandelionimages
             src (str, pathlib.Path): Local path to where the raw kaggle dataset will be downlaoded to.
@@ -1419,14 +1651,15 @@
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
             exist_ok (bool): If the kaggle dataset was already downloaded and ``exist_ok`` is ``True``, ingestion will proceed without error.
             images_compression (str): For image classification datasets, this compression will be used for the ``images`` tensor. If ``images_compression`` is "auto", compression will be automatically determined by the most common extension in the directory.
             dest_creds (Optional[Dict]): A dictionary containing credentials used to access the destination path of the dataset.
             kaggle_credentials (dict): A dictionary containing kaggle credentials {"username":"YOUR_USERNAME", "key": "YOUR_KEY"}. If ``None``, environment variables/the kaggle.json file will be used if available.
             progressbar (bool): Enables or disables ingestion progress bar. Set to ``True`` by default.
             summary (bool): Generates ingestion summary. Set to ``True`` by default.
+            shuffle (bool): Shuffles the input data prior to ingestion. Since data arranged in folders by class is highly non-random, shuffling is important in order to produce optimal results when training. Defaults to ``True``.
             **dataset_kwargs: Any arguments passed here will be forwarded to the dataset creator function. See :func:`deeplake.dataset`.
 
         Returns:
             Dataset: New dataset object with structured dataset.
 
         Raises:
             SamePathException: If the source and destination path are same.
@@ -1456,70 +1689,104 @@
         download_kaggle_dataset(
             tag,
             local_path=src,
             kaggle_credentials=kaggle_credentials,
             exist_ok=exist_ok,
         )
 
-        ds = deeplake.ingest(
+        ds = deeplake.ingest_classification(
             src=src,
             dest=dest,
-            images_compression=images_compression,
+            image_params={"sample_compression": images_compression},
             dest_creds=dest_creds,
             progressbar=progressbar,
             summary=summary,
+            shuffle=shuffle,
             **dataset_kwargs,
         )
 
         return ds
 
     @staticmethod
     def ingest_dataframe(
         src,
-        dest: Union[str, pathlib.Path, Dataset],
+        dest: Union[str, pathlib.Path],
+        column_params: Optional[Dict] = None,
+        src_creds: Optional[Dict] = None,
         dest_creds: Optional[Dict] = None,
+        creds_key: Optional[Dict] = None,
         progressbar: bool = True,
+        token: Optional[str] = None,
+        connect_kwargs: Optional[Dict] = None,
         **dataset_kwargs,
     ):
-        """Convert pandas dataframe to a Deep Lake Dataset.
+        """Convert pandas dataframe to a Deep Lake Dataset. The contents of the dataframe can be parsed literally, or can be treated as links to local or cloud files.
+
+        Examples:
+            >>> ds = deeplake.dataframe(
+            >>>     df,
+            >>>     dest="hub://org_id/dataset",
+            >>> )
+            >>> # or ingest data as images from the cloud
+            >>> ds = deeplake.dataframe(
+            >>>     df,
+            >>>     dest="hub://org_id/dataset",
+            >>>     column_params={"df_column_with_cloud_paths": {"name": "images", "htype": "image"}}
+            >>>     src_creds=aws_creds
+            >>> )
+            >>> # or ingest data as linked images in the cloud
+            >>> ds = deeplake.dataframe(
+            >>>     df,
+            >>>     dest="hub://org_id/dataset",
+            >>>     column_params={"df_column_with_cloud_paths": {"name": "image_links", "htype": "link[image]"}}
+            >>>     creds_key="my_s3_managed_credentials"
+            >>> )
 
         Args:
             src (pd.DataFrame): The pandas dataframe to be converted.
-            dest (str, pathlib.Path, Dataset):
+            dest (str, pathlib.Path):
                 - A Dataset or The full path to the dataset. Can be:
                 - a Deep Lake cloud path of the form ``hub://username/datasetname``. To write to Deep Lake cloud datasets, ensure that you are logged in to Deep Lake (use 'activeloop login' from command line)
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
+            column_params (Optional[Dict]): A dictionary containing parameters for the tensors corresponding to the dataframe columns.
+            src_creds (Optional[Dict]): Credentials to access the source data. If not provided, will be inferred from the environment.
             dest_creds (Optional[Dict]): A dictionary containing credentials used to access the destination path of the dataset.
+            creds_key (Optional[str]): creds_key for linked tensors, applicable if the htype any tensor is specified as 'link[...]' in the 'column_params' input.
             progressbar (bool): Enables or disables ingestion progress bar. Set to ``True`` by default.
-            **dataset_kwargs: Any arguments passed here will be forwarded to the dataset creator function. See :func:`deeplake.dataset`.
+            token (Optional[str]): The token to use for accessing the dataset.
+            connect_kwargs (Optional[Dict]): A dictionary containing arguments to be passed to the dataset connect method. See :meth:`Dataset.connect`.
+            **dataset_kwargs: Any arguments passed here will be forwarded to the dataset creator function. See :func:`deeplake.empty`.
 
         Returns:
             Dataset: New dataset created from the dataframe.
 
         Raises:
             Exception: If ``src`` is not a valid pandas dataframe object.
         """
         import pandas as pd
         from deeplake.auto.structured.dataframe import DataFrame
 
         feature_report_path(
             convert_pathlib_to_string_if_needed(dest),
             "ingest_dataframe",
             {},
-            token=dataset_kwargs.get("token", None),
+            token=token,
         )
 
         if not isinstance(src, pd.DataFrame):
             raise Exception("Source provided is not a valid pandas dataframe object")
 
-        structured = DataFrame(src)
+        structured = DataFrame(src, column_params, src_creds, creds_key)
 
-        if isinstance(dest, Dataset):
-            ds = dest
-        else:
-            dest = convert_pathlib_to_string_if_needed(dest)
-            ds = deeplake.dataset(dest, creds=dest_creds, **dataset_kwargs)
+        dest = convert_pathlib_to_string_if_needed(dest)
+        ds = deeplake.empty(
+            dest, creds=dest_creds, token=token, verbose=False, **dataset_kwargs
+        )
+        if connect_kwargs is not None:
+            connect_kwargs["token"] = token or connect_kwargs.get("token")
+            ds.connect(**connect_kwargs)
 
         structured.fill_dataset(ds, progressbar)  # type: ignore
+
         return ds  # type: ignore
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `deeplake-3.2.9/deeplake/api/info.py` & `deeplake-3.3.0/deeplake/api/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             else:
                 ds._dataset_diff.modify_info()
             self.is_dirty = True
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self._dataset is not None:
-            self._dataset.storage.maybe_flush()
+            self._dataset.maybe_flush()
 
     @property
     def nbytes(self):
         """Returns size of info stored in bytes."""
         return len(self.tobytes())
 
     def __len__(self):
```

### Comparing `deeplake-3.2.9/deeplake/api/link.py` & `deeplake-3.3.0/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/link_tiled.py` & `deeplake-3.3.0/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/read.py` & `deeplake-3.3.0/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_access_method.py` & `deeplake-3.3.0/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_agreement.py` & `deeplake-3.3.0/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_api.py` & `deeplake-3.3.0/deeplake/api/tests/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,40 +11,38 @@
     is_opt_true,
     get_dummy_data_path,
     requires_libdeeplake,
 )
 from deeplake.tests.storage_fixtures import enabled_remote_storages
 from deeplake.core.storage import GCSProvider
 from deeplake.util.exceptions import (
-    BadLinkError,
     GroupInfoNotSupportedError,
     InvalidOperationError,
-    TensorDtypeMismatchError,
+    SampleAppendError,
     TensorDoesNotExistError,
     TensorAlreadyExistsError,
     TensorGroupDoesNotExistError,
     TensorGroupAlreadyExistsError,
-    TensorInvalidSampleShapeError,
     DatasetHandlerError,
     TransformError,
     UnsupportedCompressionError,
     InvalidTensorNameError,
     InvalidTensorGroupNameError,
     RenameError,
     PathNotEmptyException,
     BadRequestException,
-    ReadOnlyModeError,
     EmptyTensorError,
     InvalidTokenException,
     TokenPermissionError,
     UserNotLoggedInException,
     SampleAppendingError,
     DatasetTooLargeToDelete,
     InvalidDatasetNameException,
     UnsupportedParameterException,
+    DynamicTensorNumpyError,
 )
 from deeplake.util.path import convert_string_to_pathlib_if_needed, verify_dataset_name
 from deeplake.util.testing import assert_array_equal
 from deeplake.util.pretty_print import summary_tensor, summary_dataset
 from deeplake.constants import GDRIVE_OPT, MB
 from deeplake.client.config import REPORTING_CONFIG_FILE_PATH
 
@@ -99,18 +97,25 @@
     ds.create_tensor("image")
 
     ds_new = local_ds_generator()
     assert set(ds_new.storage.keys()) == {
         "dataset_meta.json",
         "image/commit_diff",
         "image/tensor_meta.json",
+        "image/chunks_index/unsharded",
+        "image/tiles_index/unsharded",
         "_image_id/tensor_meta.json",
         "_image_id/commit_diff",
+        "_image_id/chunks_index/unsharded",
+        "_image_id/tiles_index/unsharded",
         "_image_shape/tensor_meta.json",
         "_image_shape/commit_diff",
+        "_image_shape/chunks_index/unsharded",
+        "_image_shape/tiles_index/unsharded",
+        "version_control_info.json",
     }
 
 
 def test_persist_with(local_ds_generator):
     with local_ds_generator() as ds:
         ds.create_tensor("image")
         ds.image.extend(np.ones((4, 224, 224, 3)))
@@ -199,19 +204,21 @@
     ds.image.extend(np.ones((4, 4)))
 
     ds.summary()
     assert (
         capsys.readouterr().out
         == "Dataset(path='mem://hub_pytest/test_api/test_stringify', tensors=['image'])\n\n tensor    htype    shape    dtype  compression\n -------  -------  -------  -------  ------- \n  image   generic  (4, 4)    None     None   \n"
     )
+
     ds[1:2].summary()
     assert (
         capsys.readouterr().out
         == "Dataset(path='mem://hub_pytest/test_api/test_stringify', index=Index([slice(1, 2, None)]), tensors=['image'])\n\n tensor    htype    shape    dtype  compression\n -------  -------  -------  -------  ------- \n  image   generic  (1, 4)    None     None   \n"
     )
+
     ds.image.summary()
     assert (
         capsys.readouterr().out
         == "Tensor(key='image')\n\n  htype    shape    dtype  compression\n -------  -------  -------  ------- \n generic  (4, 4)    None     None   \n"
     )
     ds[1:2].image.summary()
     assert (
@@ -331,27 +338,27 @@
 def test_safe_downcasting(local_ds):
     int_tensor = local_ds.create_tensor("int", dtype="uint8")
     int_tensor.append(0)
     int_tensor.append(1)
     int_tensor.extend([2, 3, 4])
     int_tensor.extend([5, 6, np.uint8(7)])
     int_tensor.append(np.zeros((0,), dtype="uint64"))
-    with pytest.raises(TensorDtypeMismatchError):
+    with pytest.raises(SampleAppendError):
         int_tensor.append(-8)
     int_tensor.append(np.array([1]))
     assert len(int_tensor) == 10
-    with pytest.raises(TensorDtypeMismatchError):
+    with pytest.raises(SampleAppendError):
         int_tensor.append(np.array([1.0]))
 
     float_tensor = local_ds.create_tensor("float", dtype="float32")
     float_tensor.append(0)
     float_tensor.append(1)
     float_tensor.extend([2, 3.0, 4.0])
     float_tensor.extend([5.0, 6.0, np.float32(7.0)])
-    with pytest.raises(TensorDtypeMismatchError):
+    with pytest.raises(SampleAppendError):
         float_tensor.append(float(np.finfo(np.float32).max + 1))
     float_tensor.append(np.array([1]))
     float_tensor.append(np.array([1.0]))
     assert len(float_tensor) == 10
 
 
 def test_scalar_samples(local_ds):
@@ -359,24 +366,24 @@
 
     assert tensor.meta.dtype is None
 
     # first sample sets dtype
     tensor.append(5)
     assert tensor.meta.dtype == MAX_INT_DTYPE
 
-    with pytest.raises(TensorDtypeMismatchError):
+    with pytest.raises(SampleAppendError):
         tensor.append(5.1)
 
     tensor.append(10)
     tensor.append(-99)
     tensor.append(np.array(4))
 
     tensor.append(np.int16(4))
 
-    with pytest.raises(TensorDtypeMismatchError):
+    with pytest.raises(SampleAppendError):
         tensor.append(np.float32(4))
 
     tensor.append(np.uint8(3))
 
     tensor.extend([10, 1, 4])
     tensor.extend([1])
     tensor.extend(np.array([1, 2, 3], dtype=MAX_INT_DTYPE))
@@ -388,15 +395,15 @@
     assert tensor.shape == (16, 1)
 
     tensor.append([1])
     tensor.append([1, 2, 3])
     tensor.extend([[1], [2], [3, 4]])
     tensor.append(np.empty(0, dtype=int))
 
-    with pytest.raises(TensorInvalidSampleShapeError):
+    with pytest.raises(SampleAppendError):
         tensor.append([[[1]]])
 
     expected = [
         [5],
         [10],
         [-99],
         [4],
@@ -565,32 +572,39 @@
     assert fixed.shape_interval.upper == (22, 28, 28)
     assert not fixed.is_dynamic
 
 
 def test_htype(memory_ds: Dataset):
     image = memory_ds.create_tensor("image", htype="image", sample_compression="png")
     bbox = memory_ds.create_tensor("bbox", htype="bbox")
-    label = memory_ds.create_tensor("label", htype="class_label")
+    label = memory_ds.create_tensor(
+        "label", htype="class_label", class_names=["a", "b", "c", "d", "e", "f"]
+    )
     video = memory_ds.create_tensor("video", htype="video", sample_compression="mkv")
     bin_mask = memory_ds.create_tensor("bin_mask", htype="binary_mask")
-    segment_mask = memory_ds.create_tensor("segment_mask", htype="segment_mask")
-    keypoints_coco = memory_ds.create_tensor("keypoints_coco", htype="keypoints_coco")
+    segment_mask = memory_ds.create_tensor(
+        "segment_mask", htype="segment_mask", class_names=["a", "b", "c"]
+    )
+    keypoints_coco = memory_ds.create_tensor(
+        "keypoints_coco",
+        htype="keypoints_coco",
+        keypoints=["arm", "leg", "torso"],
+        connections=[[0, 2], [1, 2]],
+    )
     point = memory_ds.create_tensor("point", htype="point")
     point_cloud = memory_ds.create_tensor(
         "point_cloud", htype="point_cloud", sample_compression="las"
     )
-    memory_ds.create_tensor(
-        "point_cloud_calibration_matrix", htype="point_cloud.calibration_matrix"
-    )
+    memory_ds.create_tensor("intrinsics", htype="intrinsics")
 
     image.append(np.ones((28, 28, 3), dtype=np.uint8))
     bbox.append(np.array([1.0, 1.0, 0.0, 0.5], dtype=np.float32))
     # label.append(5)
     label.append(np.array(5, dtype=np.uint32))
-    with pytest.raises(NotImplementedError):
+    with pytest.raises(SampleAppendError):
         video.append(np.ones((10, 28, 28, 3), dtype=np.uint8))
     bin_mask.append(np.zeros((28, 28), dtype=bool))
     segment_mask.append(np.ones((28, 28), dtype=np.uint32))
     keypoints_coco.append(np.ones((51, 2), dtype=np.int32))
     point.append(np.ones((11, 2), dtype=np.int32))
 
     point_cloud.append(
@@ -598,17 +612,15 @@
             os.path.join(get_dummy_data_path("point_cloud"), "point_cloud.las")
         )
     )
     point_cloud_dummy_data_path = pathlib.Path(get_dummy_data_path("point_cloud"))
     point_cloud.append(deeplake.read(point_cloud_dummy_data_path / "point_cloud.las"))
     # Along the forst direcection three matrices are concatenated, the first matrix is P,
     # the second one is Tr and the third one is R
-    memory_ds.point_cloud_calibration_matrix.append(
-        np.zeros((3, 4, 4), dtype=np.float32)
-    )
+    memory_ds.intrinsics.append(np.zeros((3, 4, 4), dtype=np.float32))
 
 
 def test_dtype(memory_ds: Dataset):
     tensor = memory_ds.create_tensor("tensor")
     dtyped_tensor = memory_ds.create_tensor("dtyped_tensor", dtype="uint8")
     np_dtyped_tensor = memory_ds.create_tensor(
         "np_dtyped_tensor", dtype=MAX_FLOAT_DTYPE
@@ -634,18 +646,18 @@
     np_dtyped_tensor.append(np.ones((10, 10), dtype=MAX_FLOAT_DTYPE))
     py_dtyped_tensor.append(np.ones((10, 10), dtype=MAX_FLOAT_DTYPE))
 
     # test auto upcasting
     np_dtyped_tensor.append(np.ones((10, 10), dtype="float32"))
     py_dtyped_tensor.append(np.ones((10, 10), dtype="float32"))
 
-    with pytest.raises(TensorDtypeMismatchError):
+    with pytest.raises(SampleAppendError):
         tensor.append(np.ones((10, 10), dtype="float64"))
 
-    with pytest.raises(TensorDtypeMismatchError):
+    with pytest.raises(SampleAppendError):
         dtyped_tensor.append(np.ones((10, 10), dtype="uint64") * 256)
 
     assert tensor.dtype == np.float32
     assert dtyped_tensor.dtype == np.uint8
     assert np_dtyped_tensor.dtype == MAX_FLOAT_DTYPE
     assert py_dtyped_tensor.dtype == MAX_FLOAT_DTYPE
 
@@ -872,21 +884,22 @@
     "path,hub_token",
     [
         ["local_path", "hub_cloud_dev_token"],
         ["hub_cloud_path", "hub_cloud_dev_token"],
     ],
     indirect=True,
 )
-@pytest.mark.parametrize("num_workers", [0, 2])
-@pytest.mark.parametrize("progressbar", [True, False])
+@pytest.mark.parametrize("num_workers", [2])
+@pytest.mark.parametrize("progressbar", [True])
 def test_dataset_deepcopy(path, hub_token, num_workers, progressbar):
-    src_path = "_".join((path, "src"))
-    dest_path = "_".join((path, "dest"))
+    src_path = "_".join((path, "src1"))
+    dest_path = "_".join((path, "dest1"))
 
     src_ds = deeplake.empty(src_path, overwrite=True, token=hub_token)
+    # dest_ds = deeplake.empty(dest_path, overwrite=True, token=hub_token)
 
     with src_ds:
         src_ds.info.update(key=0)
 
         src_ds.create_tensor("a", htype="image", sample_compression="png")
         src_ds.create_tensor("b", htype="class_label")
         src_ds.create_tensor("c")
@@ -896,15 +909,14 @@
 
         src_ds["a"].append(np.ones((28, 28), dtype="uint8"))
         src_ds["b"].append(0)
 
     dest_ds = deeplake.deepcopy(
         src_path,
         dest_path,
-        overwrite=True,
         token=hub_token,
         num_workers=num_workers,
         progressbar=progressbar,
     )
 
     assert list(dest_ds.tensors) == ["a", "b", "c", "d"]
     assert dest_ds.a.meta.htype == "image"
@@ -915,86 +927,65 @@
 
     assert dest_ds.info.key == 0
     assert dest_ds.d.info.key == 1
 
     for tensor in dest_ds.meta.tensors:
         assert_array_equal(src_ds[tensor].numpy(), dest_ds[tensor].numpy())
 
+    deeplake.delete(src_path, token=hub_token)
+    deeplake.delete(dest_path, token=hub_token)
+
+
+@pytest.mark.parametrize(
+    "path,hub_token",
+    [
+        ["local_path", "hub_cloud_dev_token"],
+        ["hub_cloud_path", "hub_cloud_dev_token"],
+    ],
+    indirect=True,
+)
+def test_deepcopy_errors(path, hub_token):
+    src_path = "_".join((path, "src"))
+    dest_path = "_".join((path, "dest"))
+
+    src_ds = deeplake.empty(src_path, overwrite=True, token=hub_token)
+    dest_ds = deeplake.empty(dest_path, overwrite=True, token=hub_token)
+
+    with src_ds:
+        src_ds.info.update(key=0)
+
+        src_ds.create_tensor("a", htype="image", sample_compression="png")
+        src_ds.create_tensor("b", htype="class_label")
+        src_ds.create_tensor("c")
+        src_ds.create_tensor("d", dtype=bool)
+
+        src_ds.d.info.update(key=1)
+
+        src_ds["a"].append(np.ones((28, 28), dtype="uint8"))
+        src_ds["b"].append(0)
+
     with pytest.raises(DatasetHandlerError):
         deeplake.deepcopy(src_path, dest_path, token=hub_token)
 
-    deeplake.deepcopy(
-        src_path,
-        dest_path,
-        overwrite=True,
-        token=hub_token,
-        num_workers=num_workers,
-        progressbar=progressbar,
-    )
-
     with pytest.raises(UnsupportedParameterException):
         deeplake.deepcopy(
             src_path,
             dest_path,
             overwrite=True,
             src_token=hub_token,
-            num_workers=num_workers,
-            progressbar=progressbar,
         )
 
     with pytest.raises(UnsupportedParameterException):
         deeplake.deepcopy(
             src_path,
             dest_path,
             overwrite=True,
             dest_token=hub_token,
-            num_workers=num_workers,
-            progressbar=progressbar,
         )
 
-    assert list(dest_ds.tensors) == ["a", "b", "c", "d"]
-    for tensor in dest_ds.tensors:
-        assert_array_equal(src_ds[tensor].numpy(), dest_ds[tensor].numpy())
-
-    # test fot dataset.load:
-    dest_ds = deeplake.load(dest_path, token=hub_token)
-    assert list(dest_ds.tensors) == ["a", "b", "c", "d"]
-    for tensor in dest_ds.tensors.keys():
-        assert_array_equal(src_ds[tensor].numpy(), dest_ds[tensor].numpy())
-
-    deeplake.deepcopy(
-        src_path,
-        dest_path,
-        overwrite=True,
-        token=hub_token,
-        num_workers=num_workers,
-        progressbar=progressbar,
-    )
-    dest_ds = deeplake.load(dest_path, token=hub_token)
-
-    assert list(dest_ds.tensors) == ["a", "b", "c", "d"]
-    for tensor in dest_ds.tensors:
-        assert_array_equal(src_ds[tensor].numpy(), dest_ds[tensor].numpy())
-
-    deeplake.deepcopy(
-        src_path,
-        dest_path,
-        tensors=["a", "d"],
-        overwrite=True,
-        token=hub_token,
-        num_workers=num_workers,
-        progressbar=progressbar,
-    )
-    dest_ds = deeplake.load(dest_path, token=hub_token)
-    assert list(dest_ds.tensors) == ["a", "d"]
-    for tensor in dest_ds.tensors:
-        assert_array_equal(src_ds[tensor].numpy(), dest_ds[tensor].numpy())
-    deeplake.delete(src_path, token=hub_token)
-    deeplake.delete(dest_path, token=hub_token)
-
 
 def test_cloud_delete_doesnt_exist(hub_cloud_path, hub_cloud_dev_token):
     username = hub_cloud_path.split("/")[2]
     # this dataset doesn't exist
     new_path = f"hub://{username}/doesntexist123"
     deeplake.delete(new_path, token=hub_cloud_dev_token, force=True)
 
@@ -1004,15 +995,15 @@
         memory_ds.create_tensor("group/version_state")
     with pytest.raises(InvalidTensorNameError):
         memory_ds.create_tensor("info")
 
 
 def test_compressions_list():
     assert deeplake.compressions == [
-        "apng",
+        # "apng",
         "avi",
         "bmp",
         "dcm",
         "dib",
         "eps",
         "flac",
         "fli",
@@ -1054,22 +1045,22 @@
         "class_label",
         "dicom",
         "generic",
         "image",
         "image.gray",
         "image.rgb",
         "instance_label",
+        "intrinsics",
         "json",
         "keypoints_coco",
         "list",
         "mesh",
         "nifti",
         "point",
         "point_cloud",
-        "point_cloud.calibration_matrix",
         "polygon",
         "segment_mask",
         "text",
         "video",
     ]
 
 
@@ -1128,33 +1119,33 @@
 
 
 def test_tensor_delete(local_ds_generator):
     ds = local_ds_generator()
     ds.create_tensor("x", max_chunk_size=2 * MB)
     ds.x.extend(np.ones((3, 253, 501, 5)))
     ds.delete_tensor("x")
-    assert list(ds.storage.keys()) == ["dataset_meta.json"]
+    assert set(ds.storage.keys()) == {"dataset_meta.json", "version_control_info.json"}
     assert ds.tensors == {}
 
     ds.create_tensor("x/y")
     ds.delete_tensor("x/y")
     ds.create_tensor("x/y")
     ds["x"].delete_tensor("y")
     ds.delete_group("x")
-    assert list(ds.storage.keys()) == ["dataset_meta.json"]
+    assert set(ds.storage.keys()) == {"dataset_meta.json", "version_control_info.json"}
     assert ds.tensors == {}
 
     ds.create_tensor("x/y/z")
     ds.delete_group("x")
     ds.create_tensor("x/y/z")
     ds["x"].delete_group("y")
     ds.create_tensor("x/y/z")
     ds["x/y"].delete_tensor("z")
     ds.delete_group("x")
-    assert list(ds.storage.keys()) == ["dataset_meta.json"]
+    assert set(ds.storage.keys()) == {"dataset_meta.json", "version_control_info.json"}
     assert ds.tensors == {}
     assert ds.meta.hidden_tensors == []
 
 
 def test_group_delete_bug(local_ds_generator):
     with local_ds_generator() as ds:
         ds.create_tensor("abc/first")
@@ -1369,25 +1360,25 @@
 )
 @pytest.mark.parametrize("x_size", [5, (32 * 1000)])
 @pytest.mark.parametrize("htype", ["generic", "sequence"])
 def test_ds_append(memory_ds, x_args, y_args, x_size, htype):
     ds = memory_ds
     ds.create_tensor("x", **x_args, max_chunk_size=2**20, htype=htype)
     ds.create_tensor("y", dtype="uint8", htype=htype, **y_args)
-    with pytest.raises(TensorDtypeMismatchError):
+    with pytest.raises(SampleAppendError):
         ds.append({"x": np.ones(2), "y": np.zeros(1)})
     ds.append({"x": np.ones(2), "y": [1, 2, 3]})
     ds.create_tensor("z", htype=htype)
     with pytest.raises(KeyError):
         ds.append({"x": np.ones(2), "y": [4, 5, 6, 7]})
     ds.append({"x": np.ones(3), "y": [8, 9, 10]}, skip_ok=True)
     ds.append({"x": np.ones(4), "y": [2, 3, 4]}, skip_ok=True)
     with pytest.raises(ValueError):
         ds.append({"x": np.ones(2), "y": [4, 5], "z": np.ones(4)})
-    with pytest.raises(TensorDtypeMismatchError):
+    with pytest.raises(SampleAppendError):
         ds.append({"x": np.ones(x_size), "y": np.zeros(2)}, skip_ok=True)
     assert len(ds.x) == 3
     assert len(ds.y) == 3
     assert len(ds.z) == 0
     assert ds.x.chunk_engine.commit_diff.num_samples_added == 3
     assert ds.y.chunk_engine.commit_diff.num_samples_added == 3
     assert ds.z.chunk_engine.commit_diff.num_samples_added == 0
@@ -1681,14 +1672,22 @@
 
 def test_shape_bug(memory_ds):
     ds = memory_ds
     ds.create_tensor("x")
     ds.x.extend(np.ones((5, 9, 2)))
     assert ds.x[1:4, 3:7].shape == (3, 4, 2)
 
+    ds.x.extend(np.ones((5, 9, 3)))
+
+    assert ds.x[1:2].shape == (1, 9, 2)
+    assert ds.x[3:8].shape == (5, 9, None)
+    assert ds.x[1:4, 2:4, :1].shape == (3, 2, 1)
+    assert ds.x[3:7, 2:4, :1].shape == (4, 2, 1)
+    assert ds.x[3:7, 2:4, :3].shape == (4, 2, None)
+
 
 def test_hidden_tensors(local_ds_generator):
     ds = local_ds_generator()
     with ds:
         ds.create_tensor("x", hidden=True)
         ds.x.append(1)
         assert ds.tensors == {}
@@ -1775,29 +1774,19 @@
     assert deeplake.exists(f"{path}_does_not_exist", token=hub_token) == False
 
 
 def test_pyav_not_installed(local_ds, video_paths):
     pyav_installed = deeplake.core.compression._PYAV_INSTALLED
     deeplake.core.compression._PYAV_INSTALLED = False
     local_ds.create_tensor("videos", htype="video", sample_compression="mp4")
-    with pytest.raises(deeplake.util.exceptions.CorruptedSampleError):
+    with pytest.raises(SampleAppendError):
         local_ds.videos.append(deeplake.read(video_paths["mp4"][0]))
     deeplake.core.compression._PYAV_INSTALLED = pyav_installed
 
 
-def test_create_branch_when_locked_out(local_ds):
-    local_ds.read_only = True
-    local_ds._locked_out = True
-    with pytest.raises(ReadOnlyModeError):
-        local_ds.create_tensor("x")
-    local_ds.checkout("branch", create=True)
-    assert local_ds.branch == "branch"
-    local_ds.create_tensor("x")
-
-
 def test_partial_read_then_write(s3_ds_generator):
     ds = s3_ds_generator()
     with ds:
         ds.create_tensor("xyz")
         for i in range(10):
             ds.xyz.append(i * np.ones((1000, 1000)))
 
@@ -1946,16 +1935,17 @@
 
         verify_label_data(ds)
 
     ds = local_ds_generator()
     verify_label_data(ds)
 
 
+@pytest.mark.parametrize("scheduler", ["threaded", "processed"])
 @pytest.mark.parametrize("num_workers", [0, 2])
-def test_text_labels_transform(local_ds_generator, num_workers):
+def test_text_labels_transform(local_ds_generator, scheduler, num_workers):
     with local_ds_generator() as ds:
         ds.create_tensor("labels", htype="class_label")
         ds.create_tensor("multiple_labels", htype="class_label")
         ds.create_tensor("seq_labels", htype="sequence[class_label]")
 
     labels = ["car", "ship", "train"]
     multiple_labels = [["car", "train"], ["ship", "car"], ["train", "ship"]]
@@ -1970,15 +1960,17 @@
         return ds
 
     def convert_to_idx(data, label_idx_map):
         if isinstance(data, str):
             return label_idx_map[data]
         return [convert_to_idx(label, label_idx_map) for label in data]
 
-    upload().eval(data, ds, num_workers=num_workers)
+    upload().eval(data, ds, scheduler=scheduler, num_workers=num_workers)
+
+    assert all(not tensor.startswith("__temp") for tensor in ds._tensors())
 
     for tensor in ("labels", "multiple_labels", "seq_labels"):
         class_names = ds[tensor].info.class_names
         label_idx_map = {class_names[i]: i for i in range(len(class_names))}
         if tensor == "labels":
             arr = ds[tensor].numpy()
             assert class_names == ["car", "ship", "train"]
@@ -2034,15 +2026,18 @@
             create_id_tensor=False,
         )
         ds.__temptensor.append(123)
 
     with deeplake.load(local_path) as ds:
         assert list(ds.tensors) == []
         assert ds.meta.hidden_tensors == []
-        assert list(ds.storage.keys()) == ["dataset_meta.json"]
+        assert set(ds.storage.keys()) == {
+            "dataset_meta.json",
+            "version_control_info.json",
+        }
 
     with deeplake.dataset(local_path, overwrite=True) as ds:
         ds.create_tensor(
             "__temptensor",
             htype="class_label",
             hidden=True,
             create_sample_info_tensor=False,
@@ -2172,15 +2167,15 @@
     invalid_token_exception_check()
     user_not_logged_in_exception_check(runner)
     dataset_handler_error_check(runner, username, password)
 
 
 def test_incompat_dtype_msg(local_ds, capsys):
     local_ds.create_tensor("abc", dtype="uint32")
-    with pytest.raises(TensorDtypeMismatchError):
+    with pytest.raises(SampleAppendError):
         local_ds.abc.append([0.0])
     captured = capsys.readouterr()
     assert "True" not in captured
 
 
 def test_ellipsis(memory_ds):
     with memory_ds as ds:
@@ -2197,15 +2192,15 @@
 def test_copy_label_sync_disabled(local_ds, capsys):
     abc = local_ds.create_tensor("abc", htype="class_label")
     abc.extend([1, 2, 3, 4, 5])
     ds = local_ds.copy(
         f"{local_ds.path}_copy", overwrite=True, progressbar=False, num_workers=2
     )
     captured = capsys.readouterr().out
-    assert captured == ""
+    assert captured.strip() == ""
 
 
 def test_class_label_bug(memory_ds):
     with memory_ds as ds:
         ds.create_tensor("abc", htype="class_label", class_names=["a", "b"])
         ds.abc.append([0, 1])
         ds.abc.append([1, 0])
@@ -2240,15 +2235,15 @@
 @pytest.mark.parametrize("verify", [True, False])
 def test_bad_link(local_ds_generator, verify):
     with local_ds_generator() as ds:
         ds.create_tensor(
             "images", htype="link[image]", sample_compression="jpg", verify=verify
         )
         ds.images.append(deeplake.link("https://picsum.photos/200/200"))
-        with pytest.raises(BadLinkError):
+        with pytest.raises(SampleAppendError):
             ds.images.append(deeplake.link("https://picsum.photos/lalala"))
 
     with local_ds_generator() as ds:
         assert len(ds) == 1
 
 
 def test_rich(memory_ds):
@@ -2370,18 +2365,17 @@
         ds.__temp_123.extend([1, 2, 3, 4, 5])
 
     pickle.dump(local_ds, file)
 
     file.seek(0)
     ds = pickle.load(file)
 
-    with pytest.raises(TensorDoesNotExistError):
-        ds["__temp_123"].numpy()
-
-    assert ds._temp_tensors == []
+    np.testing.assert_array_equal(
+        ds["__temp_123"].numpy(), np.array([1, 2, 3, 4, 5]).reshape(-1, 1)
+    )
 
 
 def test_max_view(memory_ds):
     with memory_ds as ds:
         ds.create_tensor("abc")
         ds.create_tensor("xyz")
         ds.create_tensor("pqr")
@@ -2435,7 +2429,27 @@
         ds.xyz.append(1)
 
         data = ds.xyz.numpy(aslist=True)
         expected = [[]] * 5 + [1]
 
         for i in range(len(data)):
             np.testing.assert_array_equal(data[i], expected[i])
+
+
+def test_np_array_in_info():
+    info = deeplake.api.info.Info()
+    x = np.random.random((3, 4))
+    info["x"] = x
+    info2 = deeplake.api.info.Info.frombuffer(info.tobytes())
+    np.testing.assert_array_equal(x, info2["x"])
+
+
+def test_sequence_numpy_bug(memory_ds):
+    with memory_ds as ds:
+        ds.create_tensor("abc", htype="sequence")
+        # issue was when number of samples (flattened) was a multiple of length of tensor
+        ds.abc.extend([[1, 2], [1, 2, 3], [1, 2, 3, 4]])
+
+        with pytest.raises(DynamicTensorNumpyError):
+            ds.abc.numpy()
+
+        assert ds.abc.numpy(aslist=True) == [[1, 2], [1, 2, 3], [1, 2, 3, 4]]
```

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.3.0/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.3.0/deeplake/api/tests/test_api_with_compression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import sys
 from deeplake.constants import KB, MB
 from deeplake.util.exceptions import (
-    SampleCompressionError,
+    SampleAppendError,
     TensorMetaMissingRequiredValue,
     TensorMetaMutuallyExclusiveKeysError,
     UnsupportedCompressionError,
-    SampleHtypeMismatchError,
 )
 import pytest
 from deeplake.core.tensor import Tensor
 from deeplake.tests.common import TENSOR_KEY, assert_images_close
 import numpy as np
 
 import deeplake
@@ -113,15 +112,15 @@
         for i in range(10):
             ds.xyz.append(i * np.ones((100, 100, 100)))
 
     for i in range(10):
         np.testing.assert_array_equal(ds.xyz[i].numpy(), i * np.ones((100, 100, 100)))
 
 
-@pytest.mark.xfail(raises=SampleCompressionError, strict=True)
+@pytest.mark.xfail(raises=SampleAppendError, strict=True)
 @pytest.mark.parametrize(
     "bad_shape",
     [
         # raises OSError: cannot write mode LA as JPEG
         (100, 100, 2),
         # raises OSError: cannot write mode RGBA as JPE
         (100, 100, 4),
@@ -324,27 +323,27 @@
 
         gray_png.append(deeplake.read(flower_path))
         gray_png.append(np.ones((10, 10, 4), dtype=np.uint8))
 
         rgb_png.append(deeplake.read(flower_path))
         rgb_png.append(np.ones((10, 10, 4), dtype=np.uint8))
 
-        with pytest.raises(SampleHtypeMismatchError):
+        with pytest.raises(SampleAppendError):
             rgb_png.append(1)
 
         with pytest.raises(TensorMetaMissingRequiredValue):
             ds.create_tensor("abc", htype="image.rgb")
 
         with pytest.raises(TensorMetaMissingRequiredValue):
             ds.create_tensor("abc", htype="image.gray")
 
     for sample in gray:
-        assert len(sample.shape) == 2
+        assert len(sample.shape) == 3
 
     for sample in rgb:
         assert len(sample.shape) == 3
 
     for sample in gray_png:
-        assert len(sample.shape) == 2
+        assert len(sample.shape) == 3
 
     for sample in rgb_png:
         assert len(sample.shape) == 3
```

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.3.0/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.3.0/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_dataset.py` & `deeplake-3.3.0/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_dicom.py` & `deeplake-3.3.0/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_downsample.py` & `deeplake-3.3.0/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_events.py` & `deeplake-3.3.0/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_grayscale.py` & `deeplake-3.3.0/deeplake/api/tests/test_grayscale.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 import deeplake
-from deeplake.util.exceptions import TensorInvalidSampleShapeError
+from deeplake.util.exceptions import SampleAppendError
 
 WARNING_STR = "Grayscale images will be reshaped"
 
 
 @pytest.fixture(params=["jpeg"])
 def deeplake_read_images(request, grayscale_image_paths, color_image_paths):
     gray_path = grayscale_image_paths[request.param]
@@ -63,15 +63,14 @@
     assert ds.images._sample_shape_tensor.shape == (2, 3)
     for i in range(2):
         assert ds.images[i].numpy().shape == ds.images[i].shape
     assert ds.images.meta.min_shape[-1] == 1
     assert ds.images.meta.max_shape[-1] == 3
 
 
-@pytest.mark.xfail(raises=TensorInvalidSampleShapeError, strict=True)
 def test_append_grayscale_first(local_ds_generator, deeplake_read_images):
     "Append a gray first, color second."
     ds = local_ds_generator()
     imgtype, gray, color = deeplake_read_images
     make_tensor_and_append(ds, "image", imgtype, [gray, color])
 
 
@@ -82,15 +81,15 @@
     with pytest.warns(UserWarning, match=WARNING_STR):
         make_tensor_and_append(ds, "generic", imgtype, [color, gray])
     assert ds.images._sample_shape_tensor.shape == (2, 3)
     for i in range(2):
         assert ds.images[i].numpy().shape == ds.images[i].shape
 
 
-@pytest.mark.xfail(raises=TensorInvalidSampleShapeError, strict=True)
+@pytest.mark.xfail(raises=SampleAppendError, strict=True)
 def test_append_grayscale_second_generic_ds_unspecified_comp(
     local_ds_generator, deeplake_read_images
 ):
     "Append with htype=generic and sample_compression=unspecified."
     ds = local_ds_generator()
     _, gray, color = deeplake_read_images
     make_tensor_and_append(ds, "generic", "unspecified", [color, gray])
@@ -98,27 +97,25 @@
 
 def test_append_two_grayscale(local_ds_generator, deeplake_read_images):
     "Append two deeplake.read grayscale images.  There should be no warning."
     ds = local_ds_generator()
     imgtype, gray, _ = deeplake_read_images
     make_tensor_and_append(ds, "image", imgtype, [gray, gray])
     assert len(ds.images) == 2
-    assert ds.images._sample_shape_tensor.shape == (2, 2)
+    assert ds.images._sample_shape_tensor.shape == (2, 3)
     for i in range(2):
         assert ds.images[i].numpy().shape == ds.images[i].shape
-    assert len(ds.images.meta.min_shape) == 2
-    assert list(ds.images.meta.min_shape) == list(gray.shape)
-    assert list(ds.images.meta.max_shape) == list(gray.shape)
+    assert list(ds.images.meta.min_shape) == list(gray.shape) + [1]
+    assert list(ds.images.meta.max_shape) == list(gray.shape) + [1]
 
 
 def test_append_many_grayscale(local_ds_generator, deeplake_read_images):
     "Append two deeplake.read grayscale images."
     ds = local_ds_generator()
     imgtype, gray, _ = deeplake_read_images
     make_tensor_and_append(ds, "image", imgtype, [gray, gray, gray, gray])
     assert len(ds.images) == 4
-    assert ds.images._sample_shape_tensor.shape == (4, 2)
+    assert ds.images._sample_shape_tensor.shape == (4, 3)
     for i in range(4):
         assert ds.images[i].numpy().shape == ds.images[i].shape
-    assert len(ds.images.meta.min_shape) == 2
-    assert list(ds.images.meta.min_shape) == list(gray.shape)
-    assert list(ds.images.meta.max_shape) == list(gray.shape)
+    assert list(ds.images.meta.min_shape) == list(gray.shape) + [1]
+    assert list(ds.images.meta.max_shape) == list(gray.shape) + [1]
```

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_info.py` & `deeplake-3.3.0/deeplake/api/tests/test_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,14 @@
 def test_info_persistence_bug(local_ds_generator):
     ds = local_ds_generator()
     with ds:
         ds.create_tensor("xyz")
     ds.commit()
     ds.xyz.info.update(abc=123)
     assert ds.xyz.info.abc == 123
-
     ds = local_ds_generator()
     assert ds.xyz.info.abc == 123
 
 
 def test_info_has_head_changes_bug(local_ds):
     with local_ds as ds:
         ds.info["tst"] = 42
```

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.3.0/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_json.py` & `deeplake-3.3.0/deeplake/api/tests/test_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import deeplake
 import pytest
-from deeplake.util.json import JsonValidationError
+from deeplake.util.exceptions import SampleAppendError
 from deeplake.tests.dataset_fixtures import (
     enabled_non_gcs_gdrive_datasets,
     enabled_non_gcs_datasets,
 )
 from typing import Any, Optional, Union, List, Dict
 
 
@@ -164,17 +164,17 @@
         assert ds.list[i].data()["value"] == items[i % 2]
 
 
 def test_json_with_schema(memory_ds):
     ds = memory_ds
     ds.create_tensor("json", htype="json", dtype=List[Dict[str, int]])
     ds.json.append([{"x": 1, "y": 2}])
-    with pytest.raises(JsonValidationError):
+    with pytest.raises(SampleAppendError):
         ds.json.append({"x": 1, "y": 2})
-    with pytest.raises(JsonValidationError):
+    with pytest.raises(SampleAppendError):
         ds.json.append([{"x": 1, "y": "2"}])
 
     assert ds.json.numpy()[0, 0] == [{"x": 1, "y": 2}]
 
     ds.create_tensor("json2", htype="json", dtype=Optional[List[Dict[str, int]]])
     items = [
         [{"x": 1, "y": 2}],
```

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_link.py` & `deeplake-3.3.0/deeplake/api/tests/test_link.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from deeplake.core.link_creds import LinkCreds
 from deeplake.core.meta.encode.creds import CredsEncoder
 from deeplake.core.storage.gcs import GCSProvider
 from deeplake.core.storage.s3 import S3Provider
 from deeplake.tests.common import is_opt_true
 from deeplake.util.exceptions import (
     ManagedCredentialsNotFoundError,
+    MissingCredsError,
+    SampleAppendError,
     TensorMetaInvalidHtype,
     UnableToReadFromUrlError,
 )
 
 from deeplake.util.htype import parse_complex_htype  # type: ignore
 
 
@@ -78,48 +80,47 @@
 
     with pytest.raises(ValueError):
         link_creds.add_creds_key("abc")
 
     link_creds.populate_creds("abc", {})
     link_creds.populate_creds("def", {})
 
-    with pytest.raises(KeyError):
+    with pytest.raises(MissingCredsError):
         link_creds.populate_creds("ghi", {})
 
-    assert link_creds.get_encoding("ENV") == 0
     assert link_creds.get_encoding(None) == 0
     with pytest.raises(ValueError):
         link_creds.get_encoding(None, "s3://my_bucket/my_key")
     assert link_creds.get_encoding("abc") == 1
     assert link_creds.get_encoding("def") == 2
-    with pytest.raises(ValueError):
+    with pytest.raises(MissingCredsError):
         link_creds.get_encoding("ghi")
 
     assert link_creds.get_creds_key(0) is None
     assert link_creds.get_creds_key(1) == "abc"
     assert link_creds.get_creds_key(2) == "def"
     with pytest.raises(KeyError):
         link_creds.get_creds_key(3)
 
     assert len(link_creds) == 2
     assert link_creds.missing_keys == []
 
     link_creds.add_creds_key("ghi")
     assert link_creds.missing_keys == ["ghi"]
 
-    with pytest.raises(KeyError):
+    with pytest.raises(MissingCredsError):
         link_creds.get_storage_provider("xyz", "s3")
 
-    with pytest.raises(ValueError):
+    with pytest.raises(MissingCredsError):
         link_creds.get_storage_provider("ghi", "s3")
 
     if is_opt_true(request, GCS_OPT):
         assert isinstance(link_creds.get_storage_provider("def", "gcs"), GCSProvider)
         assert isinstance(link_creds.get_storage_provider("def", "gcs"), GCSProvider)
-        assert isinstance(link_creds.get_storage_provider("ENV", "gcs"), GCSProvider)
+        assert isinstance(link_creds.get_storage_provider(None, "gcs"), GCSProvider)
     if is_opt_true(request, S3_OPT):
         assert isinstance(link_creds.get_storage_provider("abc", "s3"), S3Provider)
         assert isinstance(link_creds.get_storage_provider("abc", "s3"), S3Provider)
         assert isinstance(link_creds.get_storage_provider(None, "s3"), S3Provider)
 
     pickled = pickle.dumps(link_creds)
     unpickled_link_creds = pickle.loads(pickled)
@@ -186,16 +187,14 @@
     local_ds = local_ds_generator()
     with local_ds as ds:
         ds.create_tensor("xyz", htype="link[image]", sample_compression="jpg")
         ds.add_creds_key("my_s3_key")
         ds.populate_creds("my_s3_key", {})
         ds.xyz.append(deeplake.link(cat_path))
         assert ds.link_creds.used_creds_keys == set()
-        ds.xyz.append(deeplake.link(cat_path, "ENV"))
-        assert ds.link_creds.used_creds_keys == set()
         ds.xyz.append(deeplake.link(cat_path, "my_s3_key"))
         assert ds.link_creds.used_creds_keys == {"my_s3_key"}
 
     ds = local_ds_generator()
     assert ds.link_creds.used_creds_keys == {"my_s3_key"}
 
 
@@ -207,15 +206,15 @@
         ds.create_tensor(
             "linked_images",
             htype="link[image]",
             create_shape_tensor=create_shape_tensor,
             verify=verify,
             sample_compression="png",
         )
-        with pytest.raises(TypeError):
+        with pytest.raises(SampleAppendError):
             ds.linked_images.append(np.ones((100, 100, 3)))
 
         for _ in range(10):
             sample = deeplake.link(flower_path)
             ds.linked_images.append(sample)
         assert ds.linked_images.meta.sample_compression == "png"
 
@@ -309,14 +308,16 @@
 @pytest.mark.parametrize("verify", [True, False])
 @pytest.mark.skipif(
     os.name == "nt" and sys.version_info < (3, 7), reason="requires python 3.7 or above"
 )
 def test_video(request, local_ds_generator, create_shape_tensor, verify):
     local_ds = local_ds_generator()
     with local_ds as ds:
+        ds.add_creds_key("ENV")
+        ds.populate_creds("ENV", from_environment=True)
         ds.create_tensor(
             "linked_videos",
             htype="link[video]",
             sample_compression="mp4",
             create_shape_tensor=create_shape_tensor,
             verify=verify,
         )
@@ -336,14 +337,15 @@
                 "gcs://gtv-videos-bucket/sample/ForBiggerJoyrides.mp4", creds_key="ENV"
             )
             ds.linked_videos.append(sample)
             assert len(ds.linked_videos) == 4
             assert ds.linked_videos[3].shape == (361, 720, 1280, 3)
     # checking persistence
     ds = local_ds_generator()
+    ds.populate_creds("ENV", from_environment=True)
     for i in range(3):
         assert ds.linked_videos[i].shape == (361, 720, 1280, 3)
 
     if is_opt_true(request, GCS_OPT):
         assert len(ds.linked_videos) == 4
         assert ds.linked_videos[3].shape == (361, 720, 1280, 3)
 
@@ -503,37 +505,37 @@
     assert key_name in ds.link_creds.managed_creds_keys
     assert key_name in ds.link_creds.used_creds_keys
 
     shape_target = (900, 900, 3)
     assert ds.img[0].shape == shape_target
     assert ds.img[0].numpy().shape == shape_target
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ManagedCredentialsNotFoundError):
         # managed creds_key can't be updated
         ds.update_creds_key(key_name, "something_else")
 
     with pytest.raises(KeyError):
-        ds.change_creds_management("random_key", False)
+        ds.update_creds_key("random_key", managed=False)
 
     # this is a no-op
-    ds.change_creds_management(key_name, True)
+    ds.update_creds_key(key_name, managed=True)
 
     # no longer managed
-    ds.change_creds_management(key_name, False)
+    ds.update_creds_key(key_name, managed=False)
 
     ds = hub_cloud_ds_generator()
     with pytest.raises(ValueError):
         ds.img[0].numpy()
 
     ds.populate_creds(key_name, {})
     assert ds.img[0].shape == shape_target
     assert ds.img[0].numpy().shape == shape_target
 
     ds = hub_cloud_ds_generator()
-    ds.change_creds_management(key_name, True)
+    ds.update_creds_key(key_name, managed=True)
     assert ds.img[0].shape == shape_target
     assert ds.img[0].numpy().shape == shape_target
 
     new_key = "some_random_key"
     with pytest.raises(ManagedCredentialsNotFoundError):
         ds.add_creds_key(new_key, managed=True)
 
@@ -614,7 +616,50 @@
             create_shape_tensor=shape_tensor,
         )
         for _ in range(3):
             ds.img.append(deeplake.link(cat_path))
         assert ds.img.shape_interval.astuple() == (3, 900, 900, 3)
         ds.img[1] = deeplake.link(flower_path)
         assert ds.img.meta.max_shape == [900, 900, 4]
+
+
+def test_rgb_gray(local_ds, cat_path, hopper_gray_path):
+    with local_ds as ds:
+        ds.create_tensor("abc", "link[image]", sample_compression="jpeg")
+        ds.abc.append(deeplake.link(cat_path))
+        ds.abc.append(deeplake.link(hopper_gray_path))
+
+        assert len(ds.abc.meta.max_shape) == 3
+        assert len(ds.abc.meta.min_shape) == 3
+        assert len(ds.abc[0].shape) == 3
+        assert len(ds.abc[1].shape) == 3
+        assert len(ds.abc[0].numpy().shape) == 3
+        assert len(ds.abc[1].numpy().shape) == 3
+        ds.commit()
+        ds.save_view(id="testing", optimize=True)
+
+        ds = ds.load_view("testing")
+        assert len(ds.abc.meta.max_shape) == 3
+        assert len(ds.abc.meta.min_shape) == 3
+        assert len(ds.abc[0].shape) == 3
+        assert len(ds.abc[1].shape) == 3
+        assert len(ds.abc[0].numpy().shape) == 3
+        assert len(ds.abc[1].numpy().shape) == 3
+
+
+def test_creds(hub_cloud_ds_generator, cat_path):
+    creds_key = "ENV"
+    ds = hub_cloud_ds_generator()
+    ds.add_creds_key(creds_key)
+    ds.populate_creds(creds_key, from_environment=True)
+    with ds:
+        tensor = ds.create_tensor("abc", "link[image]", sample_compression="jpeg")
+        tensor.append(deeplake.link(cat_path, creds_key))
+
+    assert tensor[0].creds_key() == creds_key
+    ds.add_creds_key("my_s3_creds", True)
+    assert ds.get_managed_creds_keys() == ["my_s3_creds"]
+    assert set(ds.get_creds_keys()) == {"my_s3_creds", "ENV"}
+    ds.update_creds_key("my_s3_creds", managed=True)
+    ds = hub_cloud_ds_generator()
+    assert ds.get_managed_creds_keys() == ["my_s3_creds"]
+    assert set(ds.get_creds_keys()) == {"my_s3_creds", "ENV"}
```

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.3.0/deeplake/api/tests/test_link_tiled.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import deeplake
 import itertools
 import numpy as np
 import pytest
 
+from deeplake.util.exceptions import SampleUpdateError
+
 
 @deeplake.compute
 def add_link_tiled(sample_in, samples_out):
     arr = np.empty((10, 10), dtype=object)
     for j, i in itertools.product(range(10), range(10)):
         arr[j, i] = sample_in
     samples_out.image.append(deeplake.link_tiled(arr))
@@ -62,15 +64,15 @@
         )
         ds.image.append(linked_sample)
 
     actual_data = deeplake.read(cat_path).array
     ds = local_ds_generator()
     index = 0
     check_data(actual_data, ds, index, downsampled=True)
-    with pytest.raises(ValueError):
+    with pytest.raises(SampleUpdateError):
         ds.image[index][100:1000, 100:1000, :] = deeplake.link(cat_path)
 
     with ds:
         ds.image.extend([linked_sample, linked_sample])
     check_data(actual_data, ds, 1, downsampled=True)
     check_data(actual_data, ds, 2, downsampled=True)
 
@@ -85,9 +87,9 @@
         ds.create_tensor("image", htype="link[image]", sample_compression="jpeg")
         add_link_tiled().eval(data_in, ds, num_workers=2)
 
     actual_data = deeplake.read(cat_path).array
     ds = local_ds_generator()
     for index in range(2):
         check_data(actual_data, ds, index)
-        with pytest.raises(ValueError):
+        with pytest.raises(SampleUpdateError):
             ds.image[index][100:1000, 100:1000, :] = deeplake.link(cat_path)
```

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_linking.py` & `deeplake-3.3.0/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_mesh.py` & `deeplake-3.3.0/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_meta.py` & `deeplake-3.3.0/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_nifti.py` & `deeplake-3.3.0/deeplake/api/tests/test_nifti.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from deeplake.util.exceptions import SampleAppendError
 from nibabel.testing import data_path  # type: ignore
 
 import nibabel as nib  # type: ignore
 import numpy as np
 
 import deeplake
 import pytest
@@ -79,39 +80,41 @@
         assert ds.nifti2.shape == (1, *sample.shape)
 
 
 def test_nifti_raw_compress(memory_ds):
     with memory_ds as ds:
         ds.create_tensor("abc", htype="nifti", sample_compression="nii.gz")
 
-        with pytest.raises(NotImplementedError):
+        with pytest.raises(SampleAppendError):
             ds.abc.append(np.ones((40, 40, 10)))
 
         ds.create_tensor("xyz", htype="nifti", sample_compression=None)
         ds.xyz.append(np.ones((40, 40, 10)))
 
         np.testing.assert_array_equal(ds.xyz[0].numpy(), np.ones((40, 40, 10)))
 
 
 def test_nifti_cloud(memory_ds, s3_root_storage):
     with memory_ds as ds:
+        ds.add_creds_key("ENV")
+        ds.populate_creds("ENV", from_environment=True)
         nii_gz_4d = os.path.join(data_path, "example4d.nii.gz")
         img = nib.load(nii_gz_4d)
         with open(nii_gz_4d, "rb") as f:
             data = f.read()
         s3_root_storage["example4d.nii.gz"] = data
 
         ds.create_tensor("abc", htype="nifti", sample_compression="nii.gz")
         ds.create_tensor(
             "nifti_linked", htype="link[nifti]", sample_compression="nii.gz"
         )
         ds.abc.append(
             deeplake.read(f"{s3_root_storage.root}/example4d.nii.gz", verify=True)
         )
         ds.nifti_linked.append(
-            deeplake.link(f"{s3_root_storage.root}/example4d.nii.gz")
+            deeplake.link(f"{s3_root_storage.root}/example4d.nii.gz", creds_key="ENV")
         )
 
         assert ds.abc[0].numpy().shape == img.shape
         assert ds.nifti_linked[0].numpy().shape == img.shape
 
         del s3_root_storage["example4d.nii.gz"]
```

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_none.py` & `deeplake-3.3.0/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.3.0/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_pickle.py` & `deeplake-3.3.0/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.3.0/deeplake/api/tests/test_point_cloud.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import pytest
 
 import deeplake
 from deeplake.core.dataset import Dataset
 from deeplake.core.compression import compress_multiple
 from deeplake.tests.common import get_dummy_data_path
-from deeplake.util.exceptions import CorruptedSampleError
-from deeplake.util.exceptions import DynamicTensorNumpyError
-
+from deeplake.util.exceptions import SampleAppendError
 import numpy as np
 
 
 def test_point_cloud(local_ds, point_cloud_paths):
     for i, (compression, path) in enumerate(point_cloud_paths.items()):
         if compression == "las":
             tensor = local_ds.create_tensor(
@@ -79,20 +77,20 @@
     assert len(local_ds.point_cloud_without_sample_compression.numpy(aslist=True)) == 2
     assert len(local_ds.point_cloud_without_sample_compression.data(aslist=True)) == 2
     local_ds.create_tensor(
         "point_cloud_with_sample_compression",
         htype="point_cloud",
         sample_compression="las",
     )
-    with pytest.raises(NotImplementedError):
+    with pytest.raises(SampleAppendError):
         local_ds.point_cloud_with_sample_compression.append(
             np.zeros((1000, 3), dtype=np.float32)
         )
 
-    with pytest.raises(CorruptedSampleError):
+    with pytest.raises(SampleAppendError):
         local_ds.point_cloud_with_sample_compression.append(
             deeplake.read(get_dummy_data_path("point_cloud/corrupted_point_cloud.las"))
         )
 
     local_ds.point_cloud_with_sample_compression.append(
         deeplake.read(path, verify=True)
     )
```

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_polygons.py` & `deeplake-3.3.0/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_pop.py` & `deeplake-3.3.0/deeplake/api/tests/test_pop.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from deeplake.core.version_control.test_version_control import (
     compare_dataset_diff,
     compare_tensor_diff,
     get_default_tensor_diff,
     get_default_dataset_diff,
 )
+from deeplake.util.version_control import integrity_check
 
 
 @deeplake.compute
 def pop_fn(sample_in, samples_out):
     samples_out.x.append(sample_in)
 
 
@@ -301,7 +302,22 @@
     arrs.pop(1)
     for arr, sample in zip(arrs, ds.x):
         np.testing.assert_array_equal(sample, arr)
 
     assert not ds.x.chunk_engine._is_tiled_sample(0)
     assert ds.x.chunk_engine._is_tiled_sample(1)
     assert not ds.x.chunk_engine._is_tiled_sample(2)
+
+
+def test_sequence_pop_bug(local_ds_generator):
+    with local_ds_generator() as ds:
+        ds.create_tensor("abc", htype="sequence")
+        ds.abc.extend([[0, 1], [1, 2, 3], [1, 2]])
+        ds.pop(0)
+
+        assert len(ds._abc_shape.numpy()) == 5
+        integrity_check(ds)
+
+    ds = local_ds_generator()
+    assert len(ds._abc_shape.numpy()) == 5
+
+    integrity_check(ds)
```

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_readonly.py` & `deeplake-3.3.0/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_rechunk.py` & `deeplake-3.3.0/deeplake/api/tests/test_rechunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,18 @@
     samples_out.abc.append(sample_in)
 
 
 def test_rechunk_text(local_ds_generator):
     with local_ds_generator() as ds:
         ds.create_tensor("abc", "text")
         add_sample_in().eval(
-            ["hello", "world", "abc", "def", "ghi", "yo"], ds, num_workers=2
+            ["hello", "world", "abc", "def", "ghi", "yo"],
+            ds,
+            num_workers=2,
+            disable_rechunk=True,
         )
 
         assert len(ds.abc.chunk_engine.chunk_id_encoder.array) == 2
         ds.abc[0] = "bye"
         np.testing.assert_array_equal(
             ds.abc.numpy(),
             np.array([["bye"], ["world"], ["abc"], ["def"], ["ghi"], ["yo"]]),
@@ -148,15 +151,18 @@
     assert len(ds.abc.chunk_engine.chunk_id_encoder.array) == 1
 
 
 def test_rechunk_json(local_ds_generator):
     with local_ds_generator() as ds:
         ds.create_tensor("abc", "json")
         add_sample_in().eval(
-            [{"one": "if"}, {"two": "elif"}, {"three": "else"}], ds, num_workers=2
+            [{"one": "if"}, {"two": "elif"}, {"three": "else"}],
+            ds,
+            num_workers=2,
+            disable_rechunk=True,
         )
 
         assert len(ds.abc.chunk_engine.chunk_id_encoder.array) == 2
         ds.abc[0] = {"four": "finally"}
         np.testing.assert_array_equal(
             ds.abc.numpy(),
             np.array([[{"four": "finally"}], [{"two": "elif"}], [{"three": "else"}]]),
@@ -171,15 +177,18 @@
     assert len(ds.abc.chunk_engine.chunk_id_encoder.array) == 1
 
 
 def test_rechunk_list(local_ds_generator):
     with local_ds_generator() as ds:
         ds.create_tensor("abc", "list")
         add_sample_in().eval(
-            [["hello", "world"], ["abc", "def", "ghi"], ["yo"]], ds, num_workers=2
+            [["hello", "world"], ["abc", "def", "ghi"], ["yo"]],
+            ds,
+            num_workers=2,
+            disable_rechunk=True,
         )
 
         assert len(ds.abc.chunk_engine.chunk_id_encoder.array) == 2
         ds.abc[0] = ["bye"]
         np.testing.assert_array_equal(ds.abc[0].numpy(), np.array(["bye"]))
         np.testing.assert_array_equal(
             ds.abc[1].numpy(), np.array(["abc", "def", "ghi"])
```

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_sample_info.py` & `deeplake-3.3.0/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_text.py` & `deeplake-3.3.0/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_update_samples.py` & `deeplake-3.3.0/deeplake/api/tests/test_update_samples.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from deeplake.constants import KB
-from deeplake.util.exceptions import TensorInvalidSampleShapeError
+from deeplake.util.exceptions import SampleUpdateError
 import pytest
 from typing import Callable
 from deeplake.tests.common import assert_array_lists_equal
 import numpy as np
 import deeplake
 
 
@@ -206,39 +206,42 @@
     assert len(tensor) == 6
 
 
 def test_failures(memory_ds):
     _add_dummy_mnist(memory_ds)
 
     # primary axis doesn't match
-    with pytest.raises(ValueError):
+    with pytest.raises(SampleUpdateError):
         memory_ds.images[0:3] = np.zeros((25, 30), dtype="uint8")
-    with pytest.raises(ValueError):
+    with pytest.raises(SampleUpdateError):
         memory_ds.images[0:3] = np.zeros((2, 25, 30), dtype="uint8")
-    with pytest.raises(TensorInvalidSampleShapeError):
+    with pytest.raises(SampleUpdateError):
         memory_ds.images[0] = np.zeros((2, 25, 30), dtype="uint8")
-    with pytest.raises(ValueError):
+    with pytest.raises(SampleUpdateError):
         memory_ds.labels[0:3] = [1, 2, 3, 4]
 
     # dimensionality doesn't match
-    with pytest.raises(TensorInvalidSampleShapeError):
-        memory_ds.images[0:5] = np.zeros((5, 30), dtype="uint8")
-    with pytest.raises(TensorInvalidSampleShapeError):
+
+    memory_ds.images[0:5] = np.zeros((5, 30), dtype="uint8")
+    with pytest.raises(SampleUpdateError):
         memory_ds.labels[0:5] = np.zeros((5, 2, 3), dtype="uint8")
 
     # make sure no data changed
     assert len(memory_ds.images) == 10
     assert len(memory_ds.labels) == 10
     np.testing.assert_array_equal(
-        memory_ds.images.numpy(), np.ones((10, 28, 28), dtype="uint8")
+        memory_ds.images[:5].numpy(), np.zeros((5, 30, 1), dtype="uint8")
+    )
+    np.testing.assert_array_equal(
+        memory_ds.images[5:].numpy(), np.ones((5, 28, 28), dtype="uint8")
     )
     np.testing.assert_array_equal(
         memory_ds.labels.numpy(), np.ones((10, 1), dtype="uint8")
     )
-    assert memory_ds.images.shape == (10, 28, 28)
+    assert memory_ds.images.shape == (10, None, None)
     assert memory_ds.labels.shape == (10, 1)
 
 
 def test_warnings(memory_ds):
     tensor = memory_ds.create_tensor(
         "tensor", max_chunk_size=8 * KB, tiling_threshold=4 * KB
     )
@@ -362,18 +365,24 @@
         ds.create_tensor("x", htype="sequence[image]", sample_compression="png")
         for i in range(5):
             if i % 2:
                 ds.x.append(imgs)
             else:
                 ds.x.append(arrs)
     ds.x[0][1] = new_imgs[1]
-    np.testing.assert_array_equal(ds.x[0][1].numpy(), new_imgs[1].array)
+    if len(new_imgs[1].shape) == 2:
+        np.testing.assert_array_equal(ds.x[0][1].numpy().squeeze(), new_imgs[1].array)
+    else:
+        np.testing.assert_array_equal(ds.x[0][1].numpy(), new_imgs[1].array)
     ds.x[1] = new_imgs
     for t, img in zip(ds.x[1], new_imgs):
-        np.testing.assert_array_equal(t.numpy(), img.array)
+        if len(img.shape) == 2:
+            np.testing.assert_array_equal(t.numpy().squeeze(), img.array)
+        else:
+            np.testing.assert_array_equal(t.numpy(), img.array)
 
 
 def test_byte_positions_encoder_update_bug(memory_ds):
     ds = memory_ds
     with ds:
         ds.create_tensor("abc")
         for i in range(11):
@@ -399,19 +408,19 @@
 @pytest.mark.parametrize("htype", ["generic", "sequence"])
 def test_update_partial(memory_ds, htype, args):
     ds = memory_ds
     with ds:
         ds.create_tensor("x", htype=htype, **args)
         ds.x.append(np.ones((10, 10, 3), dtype=np.uint8))
         ds.x[0][0:2, 0:3, :1] = np.zeros((2, 3, 1), dtype=np.uint8)
-    assert ds.x[0].shape == (10, 10, 3)
+    assert ds.x[0].shape[:3] == (10, 10, 3)
     arr = ds.x[0].numpy()
     exp = np.ones((10, 10, 3), dtype=np.uint8)
     exp[0:2, 0:3, 0] *= 0
-    np.testing.assert_array_equal(arr, exp)
+    np.testing.assert_array_equal(arr.reshape(-1), exp.reshape(-1))
     with ds:
         ds.x[0][1] += 1
         ds.x[0][1] *= 3
     exp[1] += 1
     exp[1] *= 3
     arr = ds.x[0].numpy()
-    np.testing.assert_array_equal(arr, exp)
+    np.testing.assert_array_equal(arr.reshape(-1), exp.reshape(-1))
```

### Comparing `deeplake-3.2.9/deeplake/api/tests/test_video.py` & `deeplake-3.3.0/deeplake/api/tests/test_video.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,14 +181,16 @@
 
 
 @pytest.mark.skipif(
     os.name == "nt" and sys.version_info < (3, 7), reason="requires python 3.7 or above"
 )
 def test_linked_video_timestamps(local_ds):
     with local_ds as ds:
+        local_ds.add_creds_key("ENV")
+        local_ds.populate_creds("ENV", from_environment=True)
         ds.create_tensor("videos", htype="link[video]", sample_compression="mp4")
         ds.videos.append(
             deeplake.link(
                 "http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ForBiggerBlazes.mp4",
                 creds_key="ENV",
             )
         )
```

### Comparing `deeplake-3.2.9/deeplake/api/tiled.py` & `deeplake-3.3.0/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/auto/structured/base.py` & `deeplake-3.3.0/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.3.0/deeplake/auto/tests/test_coco_template.py`

 * *Files 13% similar despite different names*

```diff
@@ -92,54 +92,93 @@
     assert len(tensors) == 7
     assert "tensor1" in tensors
     assert "annotations/keypoints" in tensors
     assert "annotations/masks" in tensors
     assert "annotations/sub_annotations/sub_tensor1" in tensors
 
 
-def test_minimal_coco_ingestion(local_path, coco_ingestion_data):
+@pytest.mark.parametrize("shuffle", [True, False])
+def test_minimal_coco_ingestion(local_path, coco_ingestion_data, shuffle):
     key_to_tensor = {"segmentation": "mask", "bbox": "bboxes"}
     file_to_group = {"annotations1": "group1", "annotations2": "group2"}
     ignore_keys = ["area", "iscrowd"]
 
     ds = deeplake.ingest_coco(
         **coco_ingestion_data,
         dest=local_path,
         key_to_tensor_mapping=key_to_tensor,
         file_to_group_mapping=file_to_group,
         ignore_keys=ignore_keys,
         ignore_one_group=False,
+        shuffle=shuffle,
     )
 
     assert ds.path == local_path
     assert "images" in ds.tensors
     assert "group1/category_id" in ds.tensors
     assert "group2/category_id" in ds.tensors
     assert "group1/mask" in ds.tensors
     assert "group2/mask" in ds.tensors
     assert "group1/bboxes" in ds.tensors
     assert "group2/bboxes" in ds.tensors
     assert "group1/iscrowd" not in ds.tensors
     assert "group2/iscrowd" not in ds.tensors
 
 
-def test_coco_ingestion_with_linked_images(local_path, coco_ingestion_data):
+def test_minimal_coco_with_connect(
+    s3_path,
+    coco_ingestion_data,
+    hub_cloud_path,
+    hub_cloud_dev_token,
+    hub_cloud_dev_managed_creds_key,
+):
+    params = {**coco_ingestion_data}
+
+    ds = deeplake.ingest_coco(
+        **params,
+        dest=s3_path,
+        connect_kwargs={
+            "dest_path": hub_cloud_path,
+            "creds_key": hub_cloud_dev_managed_creds_key,
+            "token": hub_cloud_dev_token,
+        },
+    )
+
+    assert ds.path == hub_cloud_path
+    assert "images" in ds.tensors
+    assert "annotations1/bbox" in ds.tensors
+
+
+def test_coco_ingestion_with_linked_images(
+    s3_path,
+    coco_ingestion_data,
+    hub_cloud_path,
+    hub_cloud_dev_token,
+    hub_cloud_dev_managed_creds_key,
+):
     file_to_group = {"annotations1.json": "base_annotations"}
     ds = deeplake.ingest_coco(
         **coco_ingestion_data,
         file_to_group_mapping=file_to_group,
-        dest=local_path,
+        dest=s3_path,
         image_params={"name": "linked_images", "htype": "link[image]"},
+        image_creds_key=hub_cloud_dev_managed_creds_key,
+        connect_kwargs={
+            "dest_path": hub_cloud_path,
+            "creds_key": hub_cloud_dev_managed_creds_key,
+            "token": hub_cloud_dev_token,
+        },
     )
 
-    assert ds.path == local_path
+    assert ds.path == hub_cloud_path
     assert "linked_images" in ds.tensors
+    assert ds.linked_images.num_samples > 0
+    assert ds.linked_images.htype == "link[image]"
     assert "base_annotations/bbox" in ds.tensors
     assert "base_annotations/segmentation" in ds.tensors
-    assert ds.linked_images.htype == "link[image]"
 
 
 def test_flat_coco_ingestion(local_path, coco_ingestion_data):
     params = {**coco_ingestion_data}
     params["annotation_files"] = params["annotation_files"][0]
     ds = deeplake.ingest_coco(**params, dest=local_path, ignore_one_group=True)
```

### Comparing `deeplake-3.2.9/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.3.0/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.3.0/deeplake/auto/tests/test_yolo_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import deeplake
 import pytest
 from deeplake.util.exceptions import IngestionError
 
 
-def test_minimal_yolo_ingestion(local_path, yolo_ingestion_data):
+@pytest.mark.parametrize("shuffle", [True, False])
+def test_minimal_yolo_ingestion(local_path, yolo_ingestion_data, shuffle):
     params = {
         "data_directory": yolo_ingestion_data["data_directory"],
         "class_names_file": yolo_ingestion_data["class_names_file"],
     }
 
-    ds = deeplake.ingest_yolo(**params, dest=local_path)
+    ds = deeplake.ingest_yolo(**params, shuffle=shuffle, dest=local_path)
 
     assert ds.path == local_path
     assert "images" in ds.tensors
     assert "boxes" in ds.tensors
     assert "labels" in ds.tensors
     assert len(ds.labels.info["class_names"]) > 0
     assert ds.boxes.htype == "bbox"
@@ -107,59 +108,71 @@
     assert "images" in ds.tensors
     assert "polygons" in ds.tensors
     assert "labels" in ds.tensors
     assert len(ds.labels.info["class_names"]) > 0
     assert ds.polygons.htype == "polygon"
 
 
-def test_minimal_yolo_ingestion_with_linked_images(local_path, yolo_ingestion_data):
+def test_minimal_yolo_with_connect(
+    s3_path,
+    yolo_ingestion_data,
+    hub_cloud_path,
+    hub_cloud_dev_token,
+    hub_cloud_dev_managed_creds_key,
+):
     params = {
         "data_directory": yolo_ingestion_data["data_directory"],
         "class_names_file": yolo_ingestion_data["class_names_file"],
     }
 
     ds = deeplake.ingest_yolo(
         **params,
-        dest=local_path,
-        image_params={
-            "name": "linked_images",
-            "htype": "link[image]",
-            "sample_compression": "png",
+        dest=s3_path,
+        connect_kwargs={
+            "dest_path": hub_cloud_path,
+            "creds_key": hub_cloud_dev_managed_creds_key,
+            "token": hub_cloud_dev_token,
         },
     )
 
-    assert ds.path == local_path
-    assert "linked_images" in ds.tensors
+    assert ds.path == hub_cloud_path
+    assert "images" in ds.tensors
     assert "boxes" in ds.tensors
     assert "labels" in ds.tensors
     assert len(ds.labels.info["class_names"]) > 0
-    assert ds.linked_images.htype == "link[image]"
+    assert ds.boxes.htype == "bbox"
 
 
-def test_minimal_yolo_with_connect(
+def test_minimal_yolo_ingestion_with_linked_images(
     s3_path,
     yolo_ingestion_data,
     hub_cloud_path,
     hub_cloud_dev_token,
     hub_cloud_dev_managed_creds_key,
 ):
     params = {
         "data_directory": yolo_ingestion_data["data_directory"],
         "class_names_file": yolo_ingestion_data["class_names_file"],
     }
 
     ds = deeplake.ingest_yolo(
         **params,
         dest=s3_path,
+        image_params={
+            "name": "linked_images",
+            "htype": "link[image]",
+            "sample_compression": "png",
+        },
+        image_creds_key=hub_cloud_dev_managed_creds_key,
         connect_kwargs={
             "dest_path": hub_cloud_path,
             "creds_key": hub_cloud_dev_managed_creds_key,
             "token": hub_cloud_dev_token,
         },
     )
 
     assert ds.path == hub_cloud_path
-    assert "images" in ds.tensors
+    assert "linked_images" in ds.tensors
     assert "boxes" in ds.tensors
     assert "labels" in ds.tensors
     assert len(ds.labels.info["class_names"]) > 0
-    assert ds.boxes.htype == "bbox"
+    assert ds.linked_images.htype == "link[image]"
```

### Comparing `deeplake-3.2.9/deeplake/auto/unstructured/base.py` & `deeplake-3.3.0/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.3.0/deeplake/auto/unstructured/coco/coco.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from deeplake.util.exceptions import IngestionError
 
 from ..base import UnstructuredDataset
 from ..util import DatasetStructure, GroupStructure, TensorStructure
 from .utils import CocoAnnotation, CocoImages
 from .convert import coco_to_deeplake
 
+from random import shuffle as rshuffle
+
 from .constants import (
     DEFAULT_GENERIC_TENSOR_PARAMS,
     DEFAULT_COCO_TENSOR_PARAMS,
     DEFAULT_IMAGE_TENSOR_PARAMS,
 )
 
 
@@ -133,16 +135,20 @@
         structure = DatasetStructure(ignore_one_group=self.ignore_one_group)
         self._add_annotation_tensors(structure, inspect_limit=inspect_limit)
         self._add_images_tensor(structure)
 
         self._structure = structure
         return structure
 
-    def structure(self, ds: Dataset, progressbar: bool = True, num_workers: int = 0):  # type: ignore
+    def structure(self, ds: Dataset, progressbar: bool = True, num_workers: int = 0, shuffle: bool = True):  # type: ignore
         image_files = self.images.supported_images
+
+        if shuffle:
+            rshuffle(image_files)
+
         tensors = ds.tensors
 
         if self._image_creds_key is not None:
             ds.add_creds_key(self._image_creds_key, managed=True)
 
         @deeplake.compute
         def append_samples(
```

### Comparing `deeplake-3.2.9/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.3.0/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.3.0/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.3.0/deeplake/auto/unstructured/coco/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,33 +105,33 @@
 
     def parse_images(self) -> Tuple[List[str], Optional[str]]:
         """Parses the given directory to generate a list of image paths.
         Returns:
             A tuple with, respectively, list of supported images, the most frequent extension
         """
         supported_image_extensions = tuple(
-            HTYPE_SUPPORTED_COMPRESSIONS["image"] + ["jpg"]
+            "." + fmt for fmt in HTYPE_SUPPORTED_COMPRESSIONS["image"] + ["jpg"]
         )
         supported_images = []
         invalid_files = []
         extensions: DefaultDict[str, int] = defaultdict(int)
 
         for file in self.provider:
-            if file.endswith(supported_image_extensions):
+            if file.lower().endswith(supported_image_extensions):
                 supported_images.append(file)
-                ext = pathlib.Path(file).suffix[
-                    1:
-                ]  # Get extension without the . symbol
+                ext = file.rsplit(".", 1)[1]
                 extensions[ext] += 1
             else:
                 invalid_files.append(file)
 
         if len(invalid_files) > 0:
             logger.warning(
                 f"Encountered {len(invalid_files)} unsupported files in images directory."
+                + "\nUp to first 10 invalid files are:\n"
+                + "\n".join(invalid_files[0:10])
             )
 
         if len(supported_images) == 0:
             raise IngestionError(
                 f"No supported images found in {self.root}. Supported extensions are: {supported_image_extensions}"
             )
```

### Comparing `deeplake-3.2.9/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.3.0/deeplake/auto/unstructured/image_classification.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import warnings
 import numpy as np
 from pathlib import Path
+from random import shuffle as rshuffle
 import os
 import glob
-from typing import Dict, List, Sequence, Tuple, Union
+from typing import List, Tuple, Union
 
 from deeplake.util.auto import ingestion_summary
 from deeplake.util.exceptions import (
     InvalidPathException,
     TensorInvalidSampleShapeError,
 )
 from deeplake.core.dataset import Dataset
 
-from tqdm import tqdm  # type: ignore
 
 from .base import UnstructuredDataset
 
 import deeplake
 
 IMAGES_TENSOR_NAME = "images"
 LABELS_TENSOR_NAME = "labels"
@@ -79,35 +78,41 @@
         # TODO: move outside class
         set_names = set()
         for file_path in self._abs_file_paths:
             set_names.add(_set_name_from_path(file_path))
         return tuple(sorted(set_names))  # TODO: lexicographical sorting
 
     # TODO: make lazy/memoized property
-    def get_class_names(self) -> Tuple[str, ...]:
+    def get_class_names(self) -> List[str]:
         # TODO: move outside class
         class_names = set()
         for file_path in self._abs_file_paths:
             class_names.add(_class_name_from_path(file_path))
-        return tuple(sorted(class_names))  # TODO: lexicographical sorting
+        return list(sorted(class_names))  # TODO: lexicographical sorting
 
     def structure(  # type: ignore
         self,
         ds: Dataset,
         progressbar: bool = True,
         generate_summary: bool = True,
+        shuffle: bool = True,
         image_tensor_args: dict = {},
+        label_tensor_args: dict = {},
+        num_workers: int = 0,
     ) -> Dataset:
         """Create a structured dataset.
 
         Args:
-            ds (Dataset) : A Deep Lake dataset object.
+            ds (Dataset): A Deep Lake dataset object.
             progressbar (bool): Defines if the method uses a progress bar. Defaults to True.
             generate_summary (bool): Defines if the method generates ingestion summary. Defaults to True.
-            image_tensor_args (dict): Defines the sample compression of the dataset (jpeg or png).
+            shuffle (bool): Defines if the file paths should be shuffled prior to ingestion. Defaults to True.
+            image_tensor_args (dict): Defines the parameters for the images tensor.
+            label_tensor_args (dict): Defines the parameters for the class_labels tensor.
+            num_workers (int): The number of workers passed to compute.
 
         Returns:
             A Deep Lake dataset.
 
         """
 
         images_tensor_map = {}
@@ -115,68 +120,65 @@
 
         use_set_prefix = len(self.set_names) > 1
 
         for set_name in self.set_names:
             if not use_set_prefix:
                 set_name = ""
 
-            images_tensor_name = os.path.join(set_name, IMAGES_TENSOR_NAME)
-            labels_tensor_name = os.path.join(set_name, LABELS_TENSOR_NAME)
+            images_tensor_name = os.path.join(
+                set_name, image_tensor_args.pop("name", IMAGES_TENSOR_NAME)
+            )
+            labels_tensor_name = os.path.join(
+                set_name, label_tensor_args.pop("name", LABELS_TENSOR_NAME)
+            )
             images_tensor_map[set_name] = images_tensor_name.replace("\\", "/")
             labels_tensor_map[set_name] = labels_tensor_name.replace("\\", "/")
 
             # TODO: infer sample_compression
             ds.create_tensor(
                 images_tensor_name.replace("\\", "/"),
                 htype="image",
                 **image_tensor_args,
             )
             ds.create_tensor(
                 labels_tensor_name.replace("\\", "/"),
                 htype="class_label",
                 class_names=self.class_names,
+                **label_tensor_args,
             )
 
-            paths = self._abs_file_paths
-            skipped_files: list = []
-
-            iterator = tqdm(
-                paths,
-                desc='Ingesting "%s" (%i files skipped)'
-                % (self.source.name, len(skipped_files)),
-                total=len(paths),
-                disable=not progressbar,
-            )
-
-        with ds, iterator:
-            for file_path in iterator:
-                image = deeplake.read(file_path)
-
-                class_name = _class_name_from_path(file_path)
-
-                label = np.uint32(self.class_names.index(class_name))
-
-                set_name = _set_name_from_path(file_path) if use_set_prefix else ""
-
-                # TODO: try to get all len(shape)s to match.
-                # if appending fails because of a shape mismatch, expand dims (might also fail)
-                try:
-                    ds[images_tensor_map[set_name]].append(image)
-
-                except TensorInvalidSampleShapeError:
-                    im = image.array
-                    reshaped_image = np.expand_dims(im, -1)
-                    ds[images_tensor_map[set_name]].append(reshaped_image)
-
-                except Exception:
-                    skipped_files.append(file_path.name)
-                    iterator.set_description(
-                        'Ingesting "%s" (%i files skipped)'
-                        % (self.source.name, len(skipped_files))
-                    )
-                    continue
-
-                ds[labels_tensor_map[set_name]].append(label)
-
-            if generate_summary:
-                ingestion_summary(str(self.source), skipped_files)
-            return ds
+        paths = self._abs_file_paths
+        if shuffle:
+            rshuffle(paths)
+
+        skipped_files: List[str] = []
+
+        @deeplake.compute
+        def ingest_classification(file_path: Path, ds: Dataset):
+            image = deeplake.read(file_path)
+            class_name = _class_name_from_path(file_path)
+            set_name = _set_name_from_path(file_path) if use_set_prefix else ""
+
+            # if appending fails because of a shape mismatch, expand dims (might also fail)
+            try:
+                ds[images_tensor_map[set_name]].append(image)
+            except TensorInvalidSampleShapeError:
+                im = image.array
+                reshaped_image = np.expand_dims(im, -1)
+                ds[images_tensor_map[set_name]].append(reshaped_image)
+            except Exception:
+                skipped_files.append(file_path.name)
+                ds[images_tensor_map[set_name]].append(None)
+
+            ds[labels_tensor_map[set_name]].append(class_name)
+
+        ingest_classification().eval(
+            paths,
+            ds,
+            skip_ok=True,
+            progressbar=progressbar,
+            num_workers=num_workers,
+        )
+
+        if generate_summary:
+            ingestion_summary(str(self.source), skipped_files)
+        return ds
```

### Comparing `deeplake-3.2.9/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.3.0/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/auto/unstructured/util.py` & `deeplake-3.3.0/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.3.0/deeplake/auto/unstructured/yolo/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,34 +67,32 @@
         self,
     ) -> Tuple[List[str], List[str], List[str], List[str], Optional[str]]:
         """Parses the given directory to generate a list of image and annotation paths.
         Returns:
             A tuple with, respectively, list of supported images, list of encountered invalid files, list of encountered extensions and the most frequent extension
         """
         supported_image_extensions = tuple(
-            HTYPE_SUPPORTED_COMPRESSIONS["image"] + ["jpg"]
+            "." + fmt for fmt in HTYPE_SUPPORTED_COMPRESSIONS["image"] + ["jpg"]
         )
         supported_images = []
         supported_annotations = []
         invalid_files = []
         image_extensions: DefaultDict[str, int] = defaultdict(int)
 
         if self.separate_annotations:
             for file in self.provider_annotations:
-                if file.endswith(".txt"):
+                if file.lower().endswith(".txt"):
                     supported_annotations.append(file)
                 else:
                     invalid_files.append(file)
 
             for file in self.provider:
                 if file.endswith(supported_image_extensions):
                     supported_images.append(file)
-                    ext = pathlib.Path(file).suffix[
-                        1:
-                    ]  # Get extension without the . symbol
+                    ext = file.rsplit(".", 1)[1]
                     image_extensions[ext] += 1
                 else:
                     invalid_files.append(file)
 
         else:
             for file in self.provider:
                 if file.endswith(".txt"):
@@ -106,15 +104,17 @@
                     ]  # Get extension without the . symbol
                     image_extensions[ext] += 1
                 else:
                     invalid_files.append(file)
 
         if len(invalid_files) > 0:
             logger.warning(
-                f"Encountered {len(invalid_files)} unsupported files the data folders and annotation folders (if specified)."
+                f"Encountered {len(invalid_files)} unsupported files in the data folders and annotation folders (if specified)."
+                + "\nUp to first 10 invalid files are:\n"
+                + "\n".join(invalid_files[0:10])
             )
 
         most_frequent_image_extension = max(
             image_extensions, key=lambda k: image_extensions[k], default=None
         )
 
         return (
```

### Comparing `deeplake-3.2.9/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.3.0/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 from ..base import UnstructuredDataset
 from ..util import DatasetStructure, TensorStructure
 from .utils import YoloData
 
 import numpy as np
 
+from random import shuffle as rshuffle
+
 from .constants import (
     DEFAULT_YOLO_COORDINATES_TENSOR_PARAMS,
     DEFAULT_YOLO_LABEL_TENSOR_PARAMS,
     DEFAULT_IMAGE_TENSOR_PARAMS,
 )
 
 
@@ -292,26 +294,29 @@
             append_data_polygon(tensor_meta=tensor_meta).eval(
                 self.ingestion_data,
                 ds,
                 progressbar=progressbar,
                 num_workers=num_workers,
             )
 
-    def structure(self, ds: Dataset, progressbar: bool = True, num_workers: int = 0):  # type: ignore
+    def structure(self, ds: Dataset, progressbar: bool = True, num_workers: int = 0, shuffle: bool = True):  # type: ignore
         # Set class names in the dataset
         if self.data.class_names:
             ds[self.label_params["name"]].info["class_names"] = self.data.class_names
 
         # Set bounding box format in the dataset
         if ds[self.coordinates_params["name"]].meta.htype == "bbox":
             ds[self.coordinates_params["name"]].info["coords"] = {
                 "type": "fractional",
                 "mode": "CCWH",
             }
 
+        if shuffle:
+            rshuffle(self.ingestion_data)
+
         self._ingest_data(ds, progressbar, num_workers)
 
         if self.verify_class_names and self.data.class_names:
             labels = ds[self.label_params.get("name")].numpy(aslist=True)
 
             max_label = max(
                 [l.max(initial=0) for l in labels]
```

### Comparing `deeplake-3.2.9/deeplake/cli/auth.py` & `deeplake-3.3.0/deeplake/cli/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from deeplake.client.client import DeepLakeBackendClient
 from deeplake.client.utils import remove_username_from_config, write_token, remove_token
 from deeplake.util.bugout_reporter import (
     save_reporting_config,
     get_reporting_config,
     deeplake_reporter,
+    set_username,
 )
 from deeplake.util.exceptions import AuthenticationException, LoginException
 
 
 @click.command()
 @click.option("--username", "-u", default=None, help="Your Activeloop Username")
 @click.option("--password", "-p", default=None, help="Your Activeloop Password")
@@ -29,14 +30,15 @@
                 click.echo("Login to Activeloop using your credentials.")
                 click.echo(
                     "If you don't have an account, register by using the 'activeloop register' command or by going to "
                     f"{HUB_REST_ENDPOINT}/register."
                 )
                 username = click.prompt("Username")
                 password = click.prompt("Password", hide_input=True)
+                # username_reporting = username
             if not password:
                 password = click.prompt(
                     f"Please enter password for user {username}", hide_input=True
                 )
             username = username.strip()
             password = password.strip()
         try:
@@ -48,18 +50,20 @@
                 client = DeepLakeBackendClient(token)
                 orgs = client.get_user_organizations()
                 if orgs == ["public"]:
                     raise LoginException(
                         "Invalid API token. Please make sure the token is correct and try again."
                     )
                 write_token(token)
+                username = client.get_user_profile()["name"]
             click.echo("Successfully logged in to Activeloop.")
             reporting_config = get_reporting_config()
             if reporting_config.get("username") != username:
                 save_reporting_config(True, username=username)
+                set_username(deeplake_reporter, username)
             break
         except AuthenticationException:
             chances -= 1
             if chances:
                 print("Login failed. Check username and password.")
                 username = ""
                 password = ""
```

### Comparing `deeplake-3.2.9/deeplake/cli/test_cli.py` & `deeplake-3.3.0/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/client/client.py` & `deeplake-3.3.0/deeplake/client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,20 @@
     ManagedCredentialsNotFoundError,
     NotLoggedInAgreementError,
     ResourceNotFoundException,
     InvalidTokenException,
     UserNotLoggedInException,
     TokenPermissionError,
 )
-from deeplake.client.utils import check_response_status, write_token, read_token
+from deeplake.client.utils import (
+    check_response_status,
+    write_token,
+    read_token,
+    remove_token,
+)
 from deeplake.client.config import (
     ACCEPT_AGREEMENTS_SUFFIX,
     REJECT_AGREEMENTS_SUFFIX,
     GET_MANAGED_CREDS_SUFFIX,
     HUB_REST_ENDPOINT,
     HUB_REST_ENDPOINT_LOCAL,
     HUB_REST_ENDPOINT_DEV,
@@ -41,29 +46,50 @@
 retry_status_codes = {502}
 
 
 class DeepLakeBackendClient:
     """Communicates with Activeloop Backend"""
 
     def __init__(self, token: Optional[str] = None):
+        from deeplake.util.bugout_reporter import (
+            save_reporting_config,
+            get_reporting_config,
+            deeplake_reporter,
+            set_username,
+        )
+
         self.version = deeplake.__version__
+        self._token_from_env = False
         self.auth_header = None
-        if token is None:
-            self.token = self.get_token()
-        else:
-            self.token = token
+        self.token = token or self.get_token()
         self.auth_header = f"Bearer {self.token}"
 
+        # remove public token, otherwise env var will be ignored
+        # we can remove this after a while
+        orgs = self.get_user_organizations()
+        if orgs == ["public"]:
+            remove_token()
+            self.token = token or self.get_token()
+            self.auth_header = f"Bearer {self.token}"
+        if self._token_from_env:
+            username = self.get_user_profile()["name"]
+            if get_reporting_config().get("username") != username:
+                save_reporting_config(True, username=username)
+                set_username(deeplake_reporter, username)
+
     def get_token(self):
         """Returns a token"""
-        token = read_token()
+        self._token_from_env = False
+        token = read_token(from_env=False)
         if token is None:
-            token = self.request_auth_token(username="public", password="")
-            write_token(token)
-
+            token = read_token(from_env=True)
+            if token is None:
+                token = self.request_auth_token(username="public", password="")
+            else:
+                self._token_from_env = True
         return token
 
     def request(
         self,
         method: str,
         relative_url: str,
         endpoint: Optional[str] = None,
@@ -270,15 +296,15 @@
                 "rewrite": True,
                 "meta": meta,
             },
             endpoint=self.endpoint(),
         )
 
         if response.status_code == 200:
-            logger.info("Your Hub dataset has been successfully created!")
+            logger.info("Your Deep Lake dataset has been successfully created!")
             if public is False:
                 logger.info("The dataset is private so make sure you are logged in!")
 
     def get_managed_creds(self, org_id, creds_key):
         """Retrieves the managed credentials for the given org_id and creds_key.
 
         Args:
```

### Comparing `deeplake-3.2.9/deeplake/client/config.py` & `deeplake-3.3.0/deeplake/client/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 ACCEPT_AGREEMENTS_SUFFIX = "/api/organization/{}/dataset/{}/agree"
 REJECT_AGREEMENTS_SUFFIX = "/api/organization/{}/dataset/{}/disagree"
 GET_USER_PROFILE = "/api/user/profile"
 CONNECT_DATASET_SUFFIX = "/api/dataset/connect"
 
 DEFAULT_REQUEST_TIMEOUT = 170
 
-HUB_AUTH_TOKEN = "HUB_AUTH_TOKEN"
+DEEPLAKE_AUTH_TOKEN = "ACTIVELOOP_TOKEN"
```

### Comparing `deeplake-3.2.9/deeplake/client/log.py` & `deeplake-3.3.0/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/client/test_client.py` & `deeplake-3.3.0/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/client/utils.py` & `deeplake-3.3.0/deeplake/client/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import requests
 from pathlib import Path
 
 
 from deeplake.client.config import (
     REPORTING_CONFIG_FILE_PATH,
     TOKEN_FILE_PATH,
-    HUB_AUTH_TOKEN,
+    DEEPLAKE_AUTH_TOKEN,
 )
 from deeplake.util.exceptions import (
     AuthenticationException,
     AuthorizationException,
     BadGatewayException,
     BadRequestException,
     GatewayTimeoutException,
@@ -31,23 +31,22 @@
         raise EmptyTokenException
     path = Path(TOKEN_FILE_PATH)
     os.makedirs(path.parent, exist_ok=True)
     with open(TOKEN_FILE_PATH, "w") as f:
         f.write(token)
 
 
-def read_token():
+def read_token(from_env=True):
     """Returns the token. Searches for the token first in token file and then in enviroment variables."""
     token = None
     if os.path.exists(TOKEN_FILE_PATH):
         with open(TOKEN_FILE_PATH) as f:
             token = f.read()
-    else:
-        token = os.environ.get(HUB_AUTH_TOKEN)
-
+    elif from_env:
+        token = os.environ.get(DEEPLAKE_AUTH_TOKEN)
     return token
 
 
 def remove_token():
     """Deletes the token file"""
     if os.path.isfile(TOKEN_FILE_PATH):
         os.remove(TOKEN_FILE_PATH)
```

### Comparing `deeplake-3.2.9/deeplake/compression.py` & `deeplake-3.3.0/deeplake/compression.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "tiff",
     "webp",
     "wmf",
     "xbm",
 ]
 
 IMAGE_COMPRESSION_EXT_DICT = {
-    "apng": [".png"],
+    # "apng": [".png"],
     "bmp": [".bmp"],
     "eps": [".eps"],
     "fli": [".fli"],
     "dib": [".dib"],
     "gif": [".gif"],
     "ico": [".ico"],
     "im": [".im"],
@@ -108,15 +108,15 @@
 # Pillow plugins for some formats might not be installed:
 Image.init()
 IMAGE_COMPRESSIONS = [
     c for c in IMAGE_COMPRESSIONS if c.upper() in Image.SAVE and c.upper() in Image.OPEN
 ]
 
 
-IMAGE_COMPRESSIONS.insert(0, "apng")
+# IMAGE_COMPRESSIONS.insert(0, "apng")
 IMAGE_COMPRESSIONS.insert(1, "dcm")
 IMAGE_COMPRESSIONS.insert(2, "mpo")
 IMAGE_COMPRESSIONS.insert(3, "fli")
 
 SUPPORTED_COMPRESSIONS = [
     *BYTE_COMPRESSIONS,
     *IMAGE_COMPRESSIONS,
```

### Comparing `deeplake-3.2.9/deeplake/constants.py` & `deeplake-3.3.0/deeplake/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import sys
+
 import numpy as np
 
 
 BYTE_PADDING = b"\0"
 
 # number of bytes per unit
 B = 1
@@ -46,14 +48,15 @@
 DATASET_META_FILENAME = "dataset_meta.json"
 TENSOR_META_FILENAME = "tensor_meta.json"
 
 # info is user-defined information, entirely optional. may be used by the visualizer
 DATASET_INFO_FILENAME = "dataset_info.json"
 TENSOR_INFO_FILENAME = "tensor_info.json"
 
+COMMIT_INFO_FILENAME = "commit_info.json"
 DATASET_LOCK_FILENAME = "dataset_lock.lock"
 DATASET_DIFF_FILENAME = "dataset_diff"
 TENSOR_COMMIT_CHUNK_MAP_FILENAME = "chunk_set"
 TENSOR_COMMIT_DIFF_FILENAME = "commit_diff"
 TIMESTAMP_FILENAME = "local_download_timestamp"
 
 
@@ -64,14 +67,16 @@
 META_ENCODING = "utf8"
 
 CHUNKS_FOLDER = "chunks"
 ENCODED_TILE_NAMES_FOLDER = "tiles_index"
 ENCODED_CREDS_FOLDER = "creds_index"
 ENCODED_CHUNK_NAMES_FOLDER = "chunks_index"
 ENCODED_SEQUENCE_NAMES_FOLDER = "sequence_index"
+ENCODED_PAD_NAMES_FOLDER = "pad_index"
+
 # unsharded naming will help with backwards compatibility
 UNSHARDED_ENCODER_FILENAME = "unsharded"
 
 ENCODING_DTYPE = np.uint32
 
 # environment variables
 ENV_HUB_DEV_USERNAME = "ACTIVELOOP_HUB_USERNAME"
@@ -158,7 +163,23 @@
 
 _UNLINK_VIDEOS = False
 
 WANDB_INTEGRATION_ENABLED = True
 WANDB_JSON_FILENMAE = "wandb.json"
 
 SHOW_ITERATION_WARNING = True
+RETURN_DUMMY_DATA_FOR_DATALOADER = False
+
+# Delay before spinner starts on time consuming functions (in seconds)
+SPINNER_START_DELAY = 2
+
+PYTEST_ENABLED = os.environ.get("DEEPLAKE_PYTEST_ENABLED", "").lower().strip() == "true"
+
+SPINNER_ENABLED = not PYTEST_ENABLED
+
+LOCK_LOCAL_DATASETS = not PYTEST_ENABLED
+
+# Rechunk after transform if average chunk size is less than
+# this fraction of min chunk size
+TRANSFORM_RECHUNK_AVG_SIZE_BOUND = 0.1
+
+TIME_INTERVAL_FOR_CUDA_MEMORY_CLEANING = 10 * 60
```

### Comparing `deeplake-3.2.9/deeplake/core/chunk/base_chunk.py` & `deeplake-3.3.0/deeplake/core/chunk/base_chunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,21 @@
     serialize_partial_sample_object,
     get_header_from_url,
     serialize_text_sample_object,
     serialize_polygons,
 )
 from deeplake.core.storage.deeplake_memory_object import DeepLakeMemoryObject
 from deeplake.core.tiling.sample_tiles import SampleTiles
-from deeplake.util.exceptions import TensorInvalidSampleShapeError, EmptyTensorError
+from deeplake.util.exceptions import (
+    ReadSampleFromChunkError,
+    TensorInvalidSampleShapeError,
+    EmptyTensorError,
+)
 from deeplake.core.polygon import Polygons
-from functools import reduce
+from functools import reduce, wraps
 from operator import mul
 
 InputSample = Union[
     Sample,
     np.ndarray,
     int,
     float,
@@ -400,20 +404,21 @@
             raise TypeError(msg)
         shape = self.convert_to_rgb(shape)
         shape = self.normalize_shape(shape)
         return incoming_sample, shape  # type: ignore
 
     def convert_to_rgb(self, shape):
         if shape is not None and self.is_convert_candidate and CONVERT_GRAYSCALE:
+            ndim = len(shape)
             if self.num_dims is None:
-                self.num_dims = len(shape)
-            if len(shape) == 2 and self.num_dims == 3:
+                self.num_dims = max(3, ndim)
+            if ndim < self.num_dims:
                 message = "Grayscale images will be reshaped from (H, W) to (H, W, 1) to match tensor dimensions. This warning will be shown only once."
                 warnings.warn(message)
-                shape += (1,)  # type: ignore[assignment]
+                shape += (1,) * (self.num_dims - ndim)  # type: ignore[assignment]
         return shape
 
     def can_fit_sample(self, sample_nbytes, buffer_nbytes=0):
         if self.num_data_bytes == 0:
             if self.tiling_threshold < 0:  # tiling disabled
                 return True
             else:
@@ -609,7 +614,20 @@
 
     def check_empty_before_read(self):
         if self.is_empty_tensor:
             raise EmptyTensorError(
                 "This tensor has only been populated with empty samples. "
                 "Need to add at least one non-empty sample before retrieving data."
             )
+
+
+def catch_chunk_read_error(fn):
+    @wraps(fn)
+    def wrapper(self, *args, **kwargs):
+        try:
+            return fn(self, *args, **kwargs)
+        except EmptyTensorError:
+            raise
+        except Exception as e:
+            raise ReadSampleFromChunkError(self.key) from e
+
+    return wrapper
```

### Comparing `deeplake-3.2.9/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.3.0/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from deeplake.core.meta.encode.shape import ShapeEncoder
 from deeplake.core.serialize import bytes_to_text, check_sample_shape
 from deeplake.core.partial_sample import PartialSample
 from deeplake.core.tiling.sample_tiles import SampleTiles
 from deeplake.core.polygon import Polygons
 from deeplake.util.casting import intelligent_cast
 from deeplake.util.compression import get_compression_ratio
-from deeplake.util.exceptions import EmptyTensorError, TensorDtypeMismatchError
-from .base_chunk import BaseChunk, InputSample
+from deeplake.util.exceptions import TensorDtypeMismatchError
+from .base_chunk import BaseChunk, InputSample, catch_chunk_read_error
 from deeplake.core.serialize import infer_chunk_num_bytes
 from deeplake.constants import ENCODING_DTYPE
 import deeplake
 
 
 class ChunkCompressedChunk(BaseChunk):
     def __init__(self, *args, **kwargs):
@@ -355,14 +355,15 @@
             return None
         if as_bytes is None:
             as_bytes = self.is_byte_compression
         return super(ChunkCompressedChunk, self)._get_partial_sample_tile(
             as_bytes=as_bytes
         )
 
+    @catch_chunk_read_error
     def read_sample(
         self,
         local_index: int,
         cast: bool = True,
         copy: bool = False,
         decompress: bool = True,
         is_tile: bool = False,
```

### Comparing `deeplake-3.2.9/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.3.0/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 from deeplake.core.sample import Sample  # type: ignore
 from deeplake.core.serialize import (
     check_sample_shape,
     bytes_to_text,
 )
 from deeplake.core.tiling.sample_tiles import SampleTiles
 from deeplake.core.polygon import Polygons
-from deeplake.util.exceptions import EmptyTensorError
 from deeplake.util.video import normalize_index
-from .base_chunk import BaseChunk, InputSample
-import numpy as np
+from .base_chunk import BaseChunk, InputSample, catch_chunk_read_error
 
 
 class SampleCompressedChunk(BaseChunk):
     def extend_if_has_space(self, incoming_samples: List[InputSample], update_tensor_meta: bool = True, **kwargs) -> float:  # type: ignore
         self.prepare_for_write()
         num_samples: float = 0
         dtype = self.dtype if self.is_byte_compression else None
@@ -52,14 +50,15 @@
                             buffer=serialized_sample, compression=compr, shape=shape, dtype=dtype  # type: ignore
                         )
                         sample.htype = self.htype
                         incoming_samples[i] = sample
                     break
         return num_samples
 
+    @catch_chunk_read_error
     def read_sample(  # type: ignore
         self,
         local_index: int,
         cast: bool = True,
         copy: bool = False,
         sub_index: Optional[Union[int, slice]] = None,
         stream: bool = False,
```

### Comparing `deeplake-3.2.9/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.3.0/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.3.0/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.3.0/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.3.0/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from deeplake.core.serialize import (
     check_sample_shape,
     bytes_to_text,
     deserialize_linked_tiled_sample,
 )
 from deeplake.core.tiling.sample_tiles import SampleTiles
 from deeplake.core.polygon import Polygons
-from deeplake.util.exceptions import EmptyTensorError, TensorDtypeMismatchError
+from deeplake.util.exceptions import TensorDtypeMismatchError
 from deeplake.constants import ENCODING_DTYPE
-from .base_chunk import BaseChunk, InputSample
+from .base_chunk import BaseChunk, InputSample, catch_chunk_read_error
 
 
 class UncompressedChunk(BaseChunk):
     def extend_if_has_space(  # type: ignore
         self,
         incoming_samples: Union[List[InputSample], np.ndarray],
         update_tensor_meta: bool = True,
@@ -180,14 +180,15 @@
 
                     num_samples += 1
                 else:
                     break
 
         return num_samples
 
+    @catch_chunk_read_error
     def read_sample(
         self,
         local_index: int,
         cast: bool = True,
         copy: bool = False,
         decompress: bool = True,
         is_tile: bool = False,
```

### Comparing `deeplake-3.2.9/deeplake/core/chunk_engine.py` & `deeplake-3.3.0/deeplake/core/chunk_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,41 +57,48 @@
 from deeplake.core.chunk.chunk_compressed_chunk import ChunkCompressedChunk
 from deeplake.core.chunk.sample_compressed_chunk import SampleCompressedChunk
 from deeplake.core.chunk.uncompressed_chunk import UncompressedChunk
 from deeplake.core.fast_forwarding import ffw_chunk_id_encoder
 from deeplake.core.index.index import Index, IndexEntry
 from deeplake.core.meta.encode.chunk_id import CHUNK_ID_COLUMN, ChunkIdEncoder
 from deeplake.core.meta.encode.sequence import SequenceEncoder
+from deeplake.core.meta.encode.pad import PadEncoder
 from deeplake.core.meta.tensor_meta import TensorMeta
 from deeplake.core.storage.lru_cache import LRUCache
 from deeplake.util.casting import get_dtype, get_htype
 from deeplake.core.sample import Sample
 from deeplake.util.chunk_engine import (
     check_samples_type,
     make_sequence,
     check_suboptimal_chunks,
     check_sample_shape,
 )
 from deeplake.util.keys import (
     get_chunk_id_encoder_key,
     get_sequence_encoder_key,
+    get_pad_encoder_key,
     get_tensor_commit_diff_key,
     get_tensor_meta_key,
     get_chunk_key,
     get_tensor_commit_chunk_map_key,
     get_tensor_commit_chunk_map_key,
     get_tensor_meta_key,
     get_tensor_tile_encoder_key,
     get_tensor_info_key,
 )
 from deeplake.util.exceptions import (
+    GetChunkError,
     CorruptedMetaError,
     DynamicTensorNumpyError,
+    GetDataFromLinkError,
     ReadOnlyModeError,
+    ReadSampleFromChunkError,
+    SampleAppendError,
     SampleHtypeMismatchError,
+    SampleUpdateError,
 )
 from deeplake.util.remove_cache import get_base_storage
 from deeplake.util.image import convert_sample, convert_img_arr
 from deeplake.util.class_label import convert_to_idx, convert_to_hash
 from deeplake.compression import (
     BYTE_COMPRESSION,
     VIDEO_COMPRESSIONS,
@@ -169,26 +176,30 @@
         """
 
         self.key = key
         self.cache = cache
         self.base_storage = get_base_storage(cache)
         self._meta_cache = meta_cache
         self.version_state = version_state
+        self.name = version_state["tensor_names"].get(self.key)
         self.compression = None
         self.chunk_class = BaseChunk
 
         self._tensor_meta: Optional[TensorMeta] = None
         self._tensor_meta_commit_id: Optional[str] = None
 
         self._chunk_id_encoder: Optional[ChunkIdEncoder] = None
         self._chunk_id_encoder_commit_id: Optional[str] = None
 
         self._sequence_encoder: Optional[SequenceEncoder] = None
         self._sequence_encoder_commit_id: Optional[str] = None
 
+        self._pad_encoder: Optional[PadEncoder] = None
+        self._pad_encoder_commit_id: Optional[str] = None
+
         self._tile_encoder: Optional[TileEncoder] = None
         self._tile_encoder_commit_id: Optional[str] = None
 
         self._commit_chunk_map: Optional[CommitChunkMap] = None
         self._commit_chunk_map_commit_id: Optional[str] = None
 
         self._commit_diff: Optional[CommitDiff] = None
@@ -203,14 +214,15 @@
         self._all_chunk_engines: Optional[Dict[str, ChunkEngine]] = None
         self._is_temp_label_tensor: bool = False
         self._hash_label_map: Dict[int, str] = OrderedDict()
         self._sample_compression = None
         self._chunk_compression = None
 
         tensor_meta = self.tensor_meta
+        self.name = tensor_meta.name or self.key
         numpy_extend_optimization_enabled = False
 
         if tensor_meta.sample_compression:
             self._sample_compression = self.compression = tensor_meta.sample_compression
             self.chunk_class = SampleCompressedChunk
 
         elif tensor_meta.chunk_compression:
@@ -555,23 +567,27 @@
         if not partial_chunk_bytes and isinstance(chunk.data_bytes, PartialReader):
             chunk._make_data_bytearray()
         return chunk
 
     def get_chunk_from_chunk_id(
         self, chunk_id, copy: bool = False, partial_chunk_bytes=0
     ) -> BaseChunk:
-        chunk_name = ChunkIdEncoder.name_from_id(chunk_id)
-        chunk_commit_id, tkey = self.get_chunk_commit(chunk_name)
-        chunk_key = get_chunk_key(tkey, chunk_name, chunk_commit_id)
-        chunk = self.get_chunk(chunk_key, partial_chunk_bytes=partial_chunk_bytes)
-        chunk.key = chunk_key
-        chunk.id = chunk_id
-        if copy and chunk_commit_id != self.commit_id:
-            chunk = self.copy_chunk_to_new_commit(chunk, chunk_name)
-        return chunk
+        chunk_key = None
+        try:
+            chunk_name = ChunkIdEncoder.name_from_id(chunk_id)
+            chunk_commit_id, tkey = self.get_chunk_commit(chunk_name)
+            chunk_key = get_chunk_key(tkey, chunk_name, chunk_commit_id)
+            chunk = self.get_chunk(chunk_key, partial_chunk_bytes=partial_chunk_bytes)
+            chunk.key = chunk_key
+            chunk.id = chunk_id
+            if copy and chunk_commit_id != self.commit_id:
+                chunk = self.copy_chunk_to_new_commit(chunk, chunk_name)
+            return chunk
+        except Exception as e:
+            raise GetChunkError(chunk_key) from e
 
     def get_video_chunk(self, chunk_id, copy: bool = False):
         """Returns video chunks. Chunk will contain presigned url to the video instead of data if the chunk is large."""
         chunk_name = ChunkIdEncoder.name_from_id(chunk_id)
         chunk_commit_id, tkey = self.get_chunk_commit(chunk_name)
         chunk_key = get_chunk_key(tkey, chunk_name, chunk_commit_id)
 
@@ -644,17 +660,18 @@
     def _write_initialization(self):
         ffw_chunk_id_encoder(self.chunk_id_encoder)
 
     def _convert_to_list(self, samples):
         return False
 
     def check_each_sample(self, samples, verify=True):
+        # overridden in LinkedChunkEngine
         return
 
-    def _sanitize_samples(self, samples, verify=True):
+    def _sanitize_samples(self, samples, verify=True, pg_callback=None):
         check_samples_type(samples)
         if isinstance(samples, list):
             samples = [
                 None
                 if is_empty_list(sample)
                 or (
                     isinstance(sample, deeplake.core.tensor.Tensor)
@@ -974,15 +991,17 @@
                     update_commit_diff=update_commit_diff,
                     progressbar=False,
                     pg_callback=pg_callback,
                 )  # TODO optimize this
             return
         if len(samples) == 0:
             return
-        samples, verified_samples = self._sanitize_samples(samples)
+        samples, verified_samples = self._sanitize_samples(
+            samples, pg_callback=pg_callback
+        )
         self._samples_to_chunks(
             samples,
             start_chunk=self.last_appended_chunk(),
             register=True,
             progressbar=progressbar,
             update_commit_diff=update_commit_diff,
             pg_callback=pg_callback,
@@ -992,73 +1011,86 @@
     def extend(
         self,
         samples,
         progressbar: bool = False,
         link_callback: Optional[Callable] = None,
         pg_callback=None,
     ):
-        assert not (progressbar and pg_callback)
-        self.check_link_ready()
-        if not self.write_initialization_done:
-            self._write_initialization()
-            self.write_initialization_done = True
-
-        initial_autoflush = self.cache.autoflush
-        self.cache.autoflush = False
-
-        if self.is_sequence:
-            samples = tqdm(samples) if progressbar else samples
-            verified_samples = []
-            for sample in samples:
-                if sample is None:
-                    sample = []
-                verified_sample = self._extend(
-                    sample, progressbar=False, update_commit_diff=False
-                )
-                self.sequence_encoder.register_samples(len(sample), 1)
-                self.commit_diff.add_data(1)
-                verified_samples.append(verified_sample or sample)
-            if link_callback:
-                samples = [None if is_empty_list(s) else s for s in verified_samples]
-                link_callback(
-                    verified_samples,
-                    flat=False,
-                    progressbar=progressbar,
-                )
-                for s in verified_samples:
+        try:
+            assert not (progressbar and pg_callback)
+            self.check_link_ready()
+            if not self.write_initialization_done:
+                self._write_initialization()
+                self.write_initialization_done = True
+
+            initial_autoflush = self.cache.autoflush
+            self.cache.autoflush = False
+
+            if self.is_sequence:
+                samples = tqdm(samples) if progressbar else samples
+                verified_samples = []
+                num_samples_added = 0
+                try:
+                    for sample in samples:
+                        if sample is None:
+                            sample = []
+                        verified_sample = self._extend(
+                            sample, progressbar=False, update_commit_diff=False
+                        )
+                        self.sequence_encoder.register_samples(len(sample), 1)
+                        self.commit_diff.add_data(1)
+                        num_samples_added += 1
+                        verified_samples.append(verified_sample or sample)
+                except Exception:
+                    for _ in range(num_samples_added):
+                        self.pop()
+                    raise
+                if link_callback:
+                    samples = [
+                        None if is_empty_list(s) else s for s in verified_samples
+                    ]
                     link_callback(
-                        s,
-                        flat=True,
+                        verified_samples,
+                        flat=False,
                         progressbar=progressbar,
                     )
-
-        else:
-            verified_samples = (
-                self._extend(samples, progressbar, pg_callback=pg_callback) or samples
-            )
-            if link_callback:
-                if not isinstance(verified_samples, np.ndarray):
-                    samples = [
-                        None
-                        if is_empty_list(s)
-                        or (
-                            isinstance(s, deeplake.core.tensor.Tensor)
-                            and s.is_empty_tensor
+                    for s in verified_samples:
+                        link_callback(
+                            s,
+                            flat=True,
+                            progressbar=progressbar,
                         )
-                        else s
-                        for s in verified_samples
-                    ]
-                link_callback(
-                    samples,
-                    flat=None,
-                    progressbar=progressbar,
+
+            else:
+                verified_samples = (
+                    self._extend(samples, progressbar, pg_callback=pg_callback)
+                    or samples
                 )
+                if link_callback:
+                    if not isinstance(verified_samples, np.ndarray):
+                        samples = [
+                            None
+                            if is_empty_list(s)
+                            or (
+                                isinstance(s, deeplake.core.tensor.Tensor)
+                                and s.is_empty_tensor
+                            )
+                            else s
+                            for s in verified_samples
+                        ]
+                    link_callback(
+                        samples,
+                        flat=None,
+                        progressbar=progressbar,
+                    )
 
-        self.cache.autoflush = initial_autoflush
-        self.cache.maybe_flush()
+            self.cache.autoflush = initial_autoflush
+            self.cache.maybe_flush()
+        except Exception as e:
+            raise SampleAppendError(self.name) from e
 
     def _create_new_chunk(self, register=True, row: Optional[int] = None) -> BaseChunk:
         """Creates and returns a new `Chunk`. Automatically creates an ID for it and puts a reference in the cache."""
         chunk_id = self.chunk_id_encoder.generate_chunk_id(register=register, row=row)
         chunk = self.chunk_class(*self.chunk_args)  # type: ignore
         chunk_name = ChunkIdEncoder.name_from_id(chunk_id)  # type: ignore
         chunk_key = get_chunk_key(self.key, chunk_name, self.commit_id)
@@ -1181,26 +1213,33 @@
         chunk = self.get_chunks_for_sample(global_sample_index, copy=True)[0]
         local_sample_index = enc.translate_index_relative_to_chunks(global_sample_index)
 
         if len(index.values) <= 1 + int(self.is_sequence):
             chunk.update_sample(local_sample_index, sample)
         else:
             orig_sample = chunk.read_sample(local_sample_index, copy=True)
-            orig_sample[tuple(e.value for e in index.values[1:])] = sample
+            sample = np.array(sample)
+            lhs = orig_sample[tuple(e.value for e in index.values[1:])]
+            if lhs.ndim > sample.ndim:
+                sample = np.expand_dims(sample, tuple(range(sample.ndim, lhs.ndim)))
+            lhs[:] = sample
             chunk.update_sample(local_sample_index, orig_sample)
         if (
             self.active_updated_chunk is not None
             and self.active_updated_chunk.key != chunk.key  # type: ignore
         ):
             self.write_chunk_to_storage(self.active_updated_chunk)
         self.active_updated_chunk = chunk
 
         # only care about deltas if it isn't the last chunk
         if chunk.key != self.last_chunk_key:  # type: ignore
             nbytes_after_updates.append(chunk.nbytes)
+
+        self.pad_encoder.unpad(global_sample_index)
+
         self._check_rechunk(
             chunk, chunk_row=enc.__getitem__(global_sample_index, True)[0][1]
         )
 
     def pad_and_append(
         self,
         num_samples_to_pad: int,
@@ -1208,21 +1247,22 @@
         extend_link_callback=None,
         update_link_callback=None,
     ):
         """Pads the tensor with empty samples and appends value at the end."""
         self.check_link_ready()
         self.start_chunk = self.last_appended_chunk()  # type: ignore
         update_first_sample = False
+        num_samples = self.num_samples
+        orig_num_samples_to_pad = num_samples_to_pad
         if num_samples_to_pad > 0:
-            if self.num_samples == 0:
+            if num_samples == 0:
                 # set htype, dtype, shape, we later update it with empty sample
                 self.extend([value], link_callback=extend_link_callback)
                 num_samples_to_pad -= 1
                 update_first_sample = True
-
             htype = self.tensor_meta.htype
             if htype in ("json", "text", "list"):
                 empty_sample = get_empty_text_like_sample(htype)
                 empty_samples = [empty_sample] * num_samples_to_pad
             elif self.tensor_meta.is_link:
                 empty_sample = None
                 empty_samples = [None] * num_samples_to_pad
@@ -1233,35 +1273,37 @@
                 shape = tuple([num_samples_to_pad] + [0] * ndim)
                 dtype = self.tensor_meta.dtype
                 empty_sample = np.zeros(shape[1:], dtype=dtype)
                 empty_samples = np.zeros(shape, dtype=dtype)  # type: ignore
 
             if update_first_sample:
                 self.update(Index(0), empty_sample, link_callback=update_link_callback)
-
             # pad
             self.extend(empty_samples, link_callback=extend_link_callback)
-
+            self.pad_encoder.add_padding(num_samples, orig_num_samples_to_pad)
         self.extend([value], link_callback=extend_link_callback)
 
     def update(
         self,
         index: Index,
         samples: Union[np.ndarray, Sequence[InputSample], InputSample],
         operator: Optional[str] = None,
         link_callback: Optional[Callable] = None,
     ):
         """Update data at `index` with `samples`."""
-        self.check_link_ready()
-        (self._sequence_update if self.is_sequence else self._update)(  # type: ignore
-            index,
-            samples,
-            operator,
-            link_callback=link_callback,
-        )
+        try:
+            self.check_link_ready()
+            (self._sequence_update if self.is_sequence else self._update)(  # type: ignore
+                index,
+                samples,
+                operator,
+                link_callback=link_callback,
+            )
+        except Exception as e:
+            raise SampleUpdateError(self.name) from e
 
     def _get_samples_to_move(self, chunk) -> List[Sample]:
         decompress = isinstance(chunk, ChunkCompressedChunk)
         samples_to_move: List[Sample] = []
         sum_bytes = 0
 
         for idx in range(chunk.num_samples - 1, 1, -1):
@@ -1273,21 +1315,25 @@
             new_sample = self._get_sample_object(
                 sample_data, sample_shape, chunk.compression, chunk.dtype, decompress
             )
             samples_to_move.append(new_sample)
         samples_to_move.reverse()
         return samples_to_move
 
-    def _get_chunk_samples(self, chunk) -> List[Sample]:
+    def _get_chunk_samples(self, chunk) -> List[Optional[Sample]]:
         decompress = isinstance(chunk, ChunkCompressedChunk)
-        all_samples_in_chunk: List[Sample] = []
+        all_samples_in_chunk: List[Optional[Sample]] = []
 
         for idx in range(chunk.num_samples):
             sample_data = chunk.read_sample(idx, decompress=decompress)
-            sample_shape = chunk.shapes_encoder[idx]
+            try:
+                sample_shape = chunk.shapes_encoder[idx]
+            except IndexError:
+                all_samples_in_chunk.append(None)
+                continue
             new_sample = self._get_sample_object(
                 sample_data, sample_shape, chunk.compression, chunk.dtype, decompress
             )
             all_samples_in_chunk.append(new_sample)
 
         return all_samples_in_chunk
 
@@ -1353,24 +1399,25 @@
         samples, _ = self._sanitize_samples(samples_to_move, verify=False)
         to_chunk.is_dirty = True
         self.active_updated_chunk = to_chunk
         self._samples_to_chunks(
             samples,
             start_chunk=to_chunk,
             register=True,
-            update_commit_diff=True,
+            update_commit_diff=False,  # merging chunks should not update diff
             update_tensor_meta=False,
             start_chunk_row=to_chunk_row,
             register_creds=False,
         )
         self.chunk_id_encoder.delete_chunk_id(row=from_chunk_row)
         try:
             del self.cache[from_chunk.key]  # type: ignore
         except KeyError:
             pass
+        self.cache[to_chunk.key] = to_chunk  # type: ignore
         return True
 
     def _is_tiled(self, row: int) -> bool:
         """checkes whether the chunk is tiled or not
 
         Args:
             row (int): Represents the row of the chunk.
@@ -1400,15 +1447,19 @@
         next_chunk_commit_id, tkey = self.get_chunk_commit(next_chunk_name)
         chunk_key = get_chunk_key(tkey, next_chunk_name, next_chunk_commit_id)
         next_chunk_size = self.cache.get_object_size(chunk_key)
         next_chunk = self.get_chunk_from_chunk_id(int(next_chunk_id))
         if next_chunk_size + chunk.num_data_bytes < next_chunk.min_chunk_size:
             if next_chunk_commit_id != self.commit_id:
                 next_chunk = self.copy_chunk_to_new_commit(next_chunk, next_chunk_name)
-            # merge with next chunk
+            chunk_id = chunk.id
+            chunk_name = ChunkIdEncoder.name_from_id(chunk_id)
+            chunk_commit_id, tkey = self.get_chunk_commit(chunk_name)
+            if chunk_commit_id != self.commit_id:
+                chunk = self.copy_chunk_to_new_commit(chunk, chunk_name)
             return self._merge_chunks(
                 from_chunk=next_chunk,
                 from_chunk_row=next_chunk_row,
                 to_chunk=chunk,
                 to_chunk_row=row,
             )
         return False
@@ -1426,14 +1477,19 @@
         prev_chunk_commit_id, tkey = self.get_chunk_commit(prev_chunk_name)
         prev_chunk_key = get_chunk_key(tkey, prev_chunk_name, prev_chunk_commit_id)
         prev_chunk_size = self.cache.get_object_size(prev_chunk_key)
         prev_chunk = self.get_chunk_from_chunk_id(int(prev_chunk_id))
         if prev_chunk_size + chunk.num_data_bytes < prev_chunk.min_chunk_size:
             if prev_chunk_commit_id != self.commit_id:
                 prev_chunk = self.copy_chunk_to_new_commit(prev_chunk, prev_chunk_name)
+            chunk_id = chunk.id
+            chunk_name = ChunkIdEncoder.name_from_id(chunk_id)
+            chunk_commit_id, tkey = self.get_chunk_commit(chunk_name)
+            if chunk_commit_id != self.commit_id:
+                chunk = self.copy_chunk_to_new_commit(chunk, chunk_name)
             # merge with previous chunk
             return self._merge_chunks(
                 from_chunk=chunk,
                 from_chunk_row=row,
                 to_chunk=prev_chunk,
                 to_chunk_row=prev_chunk_row,
             )
@@ -1667,15 +1723,15 @@
             stop = index.values[0].value.stop or self.num_samples
             step = index.values[0].value.step or 1
 
             if start < 0:
                 start = self.num_samples + start
 
             if stop < 0:
-                stop = self.num_samples + start
+                stop = self.num_samples + stop
 
             numpy_array_length = (stop - start) // step
             return numpy_array_length > threshold
         return False
 
     def numpy(
         self,
@@ -1861,34 +1917,51 @@
                 This will always be True even if specified as False in the following cases:
                 - The tensor is ChunkCompressed
                 - The chunk which is being accessed has more than 128 samples.
             pad_tensor (bool): If True, any index out of bounds will not throw an error, but instead will return an empty sample.
 
         Raises:
             DynamicTensorNumpyError: If shapes of the samples being read are not all the same.
+            GetChunkError: If a chunk cannot be retrieved from the storage.
+            ReadSampleFromChunkError: If a sample cannot be read from a chunk.
+            GetDataFromLinkError: If data cannot be retrieved from a link.
 
         Returns:
             Union[np.ndarray, List[np.ndarray]]: Either a list of numpy arrays or a single numpy array (depending on the `aslist` argument).
         """
         length = self.num_samples
         last_shape = None
         ispolygon = self.tensor_meta.htype == "polygon"
         if ispolygon:
             aslist = True
         if use_data_cache and self.is_data_cachable:
             samples = self.numpy_from_data_cache(index, length, aslist, pad_tensor)
         else:
             samples = []
             for global_sample_index in index.values[0].indices(length):
-                sample = self.get_single_sample(
-                    global_sample_index,
-                    index,
-                    fetch_chunks=fetch_chunks,
-                    pad_tensor=pad_tensor,
-                )
+                try:
+                    sample = self.get_single_sample(
+                        global_sample_index,
+                        index,
+                        fetch_chunks=fetch_chunks,
+                        pad_tensor=pad_tensor,
+                    )
+                except GetChunkError as e:
+                    raise GetChunkError(
+                        e.chunk_key, global_sample_index, self.name
+                    ) from e
+                except ReadSampleFromChunkError as e:
+                    raise ReadSampleFromChunkError(
+                        e.chunk_key, global_sample_index, self.name
+                    ) from e
+                except GetDataFromLinkError as e:
+                    raise GetDataFromLinkError(
+                        e.link, global_sample_index, self.name
+                    ) from e
+
                 check_sample_shape(sample.shape, last_shape, self.key, index, aslist)
                 last_shape = sample.shape
                 if ispolygon:
                     sample = [p.__array__() for p in sample]
                 samples.append(sample)
         if aslist and all(map(np.isscalar, samples)):
             samples = list(arr.item() for arr in samples)
@@ -1984,14 +2057,17 @@
                 f"'{tkey}' and '{ikey}' have a record of different numbers of samples. Got {tensor_meta_length} and {chunk_id_num_samples} respectively."
             )
 
     def list_all_chunks(self) -> List[str]:
         """Return list of all chunks for current `version_state['commit_id']` and tensor"""
         commit_id = self.commit_id
         if commit_id == FIRST_COMMIT_ID:
+            arr = self.chunk_id_encoder._encoded
+            if not arr.size:
+                return []
             return [
                 ChunkIdEncoder.name_from_id(chunk_id)
                 for chunk_id in self.chunk_id_encoder._encoded[:, CHUNK_ID_COLUMN]
             ]  # type: ignore
         else:
             return [k for (k, v) in self.commit_chunk_map.chunks.items() if not v]  # type: ignore
 
@@ -2023,36 +2099,49 @@
 
     def clear_unusd_chunks(self, storage: StorageProvider):
         # storage.delete_multiple(self.list_orphaned_chunks(storage))
         raise NotImplementedError(
             "requires StorageProvider to be able to list all chunks"
         )
 
-    def pop(self, global_sample_index: int):
+    def pop(
+        self,
+        global_sample_index: Optional[int] = None,
+        link_callback: Optional[Callable] = None,
+    ):
+        if global_sample_index is None:
+            if self.is_sequence:
+                global_sample_index = self.sequence_encoder.num_samples - 1
+            else:
+                global_sample_index = self.num_samples - 1
         self._write_initialization()
         if self.tensor_meta.length == 0:
             raise ValueError("There are no samples to pop")
         if global_sample_index < 0 or global_sample_index >= self.tensor_meta.length:
             raise IndexError(
                 f"Index {global_sample_index} is out of range for tensor of length {self.tensor_meta.length}"
             )
 
         self.cached_data = None
         initial_autoflush = self.cache.autoflush
         self.cache.autoflush = False
 
+        # pop links
+        if link_callback:
+            link_callback(global_sample_index)
+
         self.commit_diff.pop(global_sample_index)
         if self.is_sequence:
             # pop in reverse order else indices get shifted
             for idx in reversed(range(*self.sequence_encoder[global_sample_index])):
                 self.pop_item(idx)
             self.sequence_encoder.pop(global_sample_index)
         else:
             self.pop_item(global_sample_index)
-
+        self.pad_encoder.pop(global_sample_index)
         self.cache.autoflush = initial_autoflush
         self.cache.maybe_flush()
 
     def pop_item(self, global_sample_index):
         enc = self.chunk_id_encoder
         if not self._is_tiled_sample(global_sample_index):
             local_sample_index = enc.translate_index_relative_to_chunks(
@@ -2117,16 +2206,30 @@
             key = get_sequence_encoder_key(self.key, commit_id)
             self.meta_cache[key]
             return True
         except KeyError:
             return False
 
     @property
+    def pad_encoder_exists(self) -> bool:
+        commit_id = self.commit_id
+        if self._pad_encoder is not None and self._pad_encoder_commit_id == commit_id:
+            return True
+        try:
+            key = get_pad_encoder_key(self.key, commit_id)
+            self.meta_cache[key]
+            return True
+        except KeyError:
+            return False
+
+    @property
     def _sequence_length(self):
-        return self.sequence_encoder.num_samples
+        if self.is_sequence:
+            return self.sequence_encoder.num_samples
+        return
 
     @property
     def sequence_encoder(self) -> SequenceEncoder:
         """Gets the shape encoder from cache, if one is not found it creates a blank encoder.
 
         Raises:
             CorruptedMetaError: If shape encoding was corrupted.
@@ -2153,14 +2256,33 @@
             else:
                 enc = self.meta_cache.get_deeplake_object(key, SequenceEncoder)
             self._sequence_encoder = enc
             self._sequence_encoder_commit_id = commit_id
             self.meta_cache.register_deeplake_object(key, enc)
         return self._sequence_encoder
 
+    @property
+    def pad_encoder(self) -> PadEncoder:
+        commit_id = self.commit_id
+        if self._pad_encoder is None or self._pad_encoder_commit_id != commit_id:
+            commit_id = self.commit_id
+            key = get_pad_encoder_key(self.key, commit_id)
+            if not self.pad_encoder_exists:
+                enc = PadEncoder()
+                try:
+                    self.meta_cache[key] = enc
+                except ReadOnlyModeError:
+                    pass
+            else:
+                enc = self.meta_cache.get_deeplake_object(key, PadEncoder)
+            self._pad_encoder = enc
+            self._pad_encoder_commit_id = commit_id
+            self.meta_cache.register_deeplake_object(key, enc)
+        return self._pad_encoder
+
     def _sequence_numpy(
         self,
         index: Index,
         aslist: bool = False,
         use_data_cache: bool = True,
         fetch_chunks: bool = False,
         pad_tensor: bool = False,
@@ -2171,31 +2293,36 @@
             use_data_cache=use_data_cache,
             fetch_chunks=fetch_chunks,
             pad_tensor=pad_tensor,
         )
         if isinstance(arr, np.ndarray) and arr.size == 0:
             return self.get_empty_sample()
         if index.subscriptable_at(0) and index.subscriptable_at(1):
+            item_lengths = []
+            for i in index.values[0].indices(self._sequence_length):
+                item_length = index.length_at(
+                    1, -int(np.subtract(*self.sequence_encoder[i]))
+                )
+                item_lengths.append(item_length)
+
             if aslist:
-                _item_length = self._sequence_item_length
                 ret = []
-                for i in index.values[0].indices(self._sequence_length):
-                    item_length = _item_length or index.length_at(
-                        1, -int(np.subtract(*self.sequence_encoder[i]))
-                    )
+                for item_length in item_lengths:
                     ret.append(arr[:item_length])
                     arr = arr[item_length:]
                 return ret
             else:
+                if len(set(item_lengths)) > 1:
+                    raise DynamicTensorNumpyError(self.name, index, "shape")
                 try:
                     return arr.reshape(  # type: ignore
                         index.length_at(0, self._sequence_length), -1, *arr.shape[1:]  # type: ignore
                     )
                 except ValueError as ve:
-                    raise DynamicTensorNumpyError(self.key, index, "shape") from ve
+                    raise DynamicTensorNumpyError(self.name, index, "shape") from ve
         return arr
 
     def _translate_2d_index(
         self, x: Optional[IndexEntry] = None, y: Optional[IndexEntry] = None
     ) -> IndexEntry:
         x = x or IndexEntry()
         y = y or IndexEntry()
@@ -2361,74 +2488,114 @@
 
     def check_link_ready(self):
         return
 
     def shape(
         self, index: Index, sample_shape_provider: Optional[Callable] = None
     ) -> Tuple[Optional[int], ...]:
-        shape = self.shape_interval.astuple()
-        idxs = index.values
-        skip_dims = 0
+        shape = self.shape_interval(index).astuple()[1:]
+        index_0, sample_index = index.values[0], index.values[1:]
+        sample_indices = list(
+            index_0.indices(self._sequence_length or self.num_samples)
+        )
+        num_samples = len(sample_indices)
+
+        if num_samples == 0:
+            return (0, *shape)
+
+        sample_ndim = self.ndim() - 1
+        sample_shapes = np.zeros((num_samples, sample_ndim), dtype=np.int32)
+
+        if len(sample_index) > sample_ndim:
+            raise IndexError(
+                f"Too many indices for tensor. Tensor is rank {sample_ndim + 1} but {len(sample_index) + 1} indices were provided."
+            )
+
         if None in shape or self.tensor_meta.is_link:
-            if not idxs[0].subscriptable():
+            for i, idx in enumerate(sample_indices):
                 if self.tensor_meta.htype in ("text", "json"):
                     shape = (1,)
                 else:
                     if sample_shape_provider:
                         try:
-                            shape = sample_shape_provider(idxs[0].value)  # type: ignore
+                            shape = sample_shape_provider(idx)  # type: ignore
+                            if isinstance(shape, tuple) and shape == ():
+                                shape = (1,)
                             if self.is_sequence:
-                                if len(idxs) > 1 and not idxs[1].subscriptable():
-                                    shape = tuple(shape[idxs[1].value].tolist())  # type: ignore
-                                    skip_dims += 1
+                                if sample_index and not sample_index[0].subscriptable():
+                                    shape = (1, *tuple(shape[sample_index[0].value].tolist()))  # type: ignore
                                 else:
+                                    is_same = np.all(shape == shape[0, :], axis=0)  # type: ignore
                                     shape = (len(shape),) + (
                                         tuple(
                                             int(shape[0, i])  # type: ignore
-                                            if np.all(shape[:, i] == shape[0, i])  # type: ignore
-                                            else None
+                                            if is_same[i]  # type: ignore
+                                            else -1
                                             for i in range(shape.shape[1])  # type: ignore
                                         )
                                         or (1,)
                                     )
 
                         except (
                             IndexError
                         ):  # Happens during transforms, sample shape tensor is not populated yet
-                            shape = self.read_shape_for_sample(idxs[0].value)  # type: ignore
+                            shape = self.read_shape_for_sample(idx)  # type: ignore
                     else:
                         self.check_link_ready()
-                        shape = self.read_shape_for_sample(idxs[0].value)  # type: ignore
-                skip_dims += 1
-        elif not idxs[0].subscriptable():
-            shape = shape[1:]
-            skip_dims += 1
-        shape = list(shape)  # type: ignore
+                        shape = self.read_shape_for_sample(idx)  # type: ignore
+                        # if link verification was not done
+                        if len(shape) > sample_ndim:
+                            sample_ndim = len(shape)
+                            sample_shapes = np.zeros(
+                                (num_samples, sample_ndim), dtype=np.int32
+                            )
+                    sample_shapes[i] = shape
+        else:
+            sample_shapes[:] = shape
+
         squeeze_dims = set()
-        for i, idx in enumerate(idxs[skip_dims:]):
-            if idx.subscriptable():
-                shape[i] = idx.length(shape[i])  # type: ignore
-            else:
-                squeeze_dims.add(i)
+        for i in range(num_samples):
+            for j in range(len(sample_index)):
+                if sample_index[j].subscriptable():
+                    if sample_shapes[i, j] != -1:
+                        sample_shapes[i, j] = sample_index[j].length(
+                            sample_shapes[i, j]
+                        )
+                else:
+                    squeeze_dims.add(j)
+
+        is_same = np.all(sample_shapes == sample_shapes[0, :], axis=0)
+        shape = [  # type: ignore
+            int(sample_shapes[0, i])
+            if sample_shapes[0, i] != -1 and is_same[i]
+            else None
+            for i in range(sample_ndim)
+        ]
+
+        if index_0.subscriptable():
+            shape = [num_samples, *shape]  # type: ignore
+
         return tuple(shape[i] for i in range(len(shape)) if i not in squeeze_dims)
 
     def ndim(self, index: Optional[Index] = None) -> int:
         ndim = len(self.tensor_meta.min_shape) + 1
         if self.is_sequence:
             ndim += 1
         if index:
             for idx in index.values:
                 if not idx.subscriptable():
                     ndim -= 1
         return ndim
 
-    @property
-    def shape_interval(self) -> ShapeInterval:
+    def shape_interval(self, index: Index) -> ShapeInterval:
         """Returns a `ShapeInterval` object that describes this tensor's shape more accurately. Length is included.
 
+        Args:
+            index (Index): Index to use for shape calculation.
+
         Note:
             If you are expecting a `tuple`, use `tensor.shape` instead.
 
         Example:
             >>> tensor.append(np.zeros((10, 10)))
             >>> tensor.append(np.zeros((10, 15)))
             >>> tensor.shape_interval
@@ -2437,20 +2604,20 @@
             (2, 10, 10:15)
 
         Returns:
             ShapeInterval: Object containing `lower` and `upper` properties.
         """
         meta = self.tensor_meta
         if self.is_sequence:
-            seq_length = self._sequence_length
+            seq_length = index.length(self._sequence_length)
             min_item_length, max_item_length = self._sequence_item_length_range
             min_length = [seq_length, min_item_length]
             max_length = [seq_length, max_item_length]
         else:
-            min_length = max_length = [meta.length]
+            min_length = max_length = [index.length(meta.length)]
         min_shape = min_length + list(meta.min_shape)
         max_shape = max_length + list(meta.max_shape)
 
         return ShapeInterval(min_shape, max_shape)
 
     def _transform_callback(
         self, samples, flat: Optional[bool], progressbar: bool = False
@@ -2480,14 +2647,32 @@
                         vs = cast_to_type(vs, dtype)
                     else:
                         vs = [cast_to_type(v, dtype) for v in vs]
                 chunk_engine = self._all_chunk_engines[k]
                 chunk_engine.extend(vs)
                 chunk_engine._transform_callback(vs, flat)
 
+    def _transform_pop_callback(self, index: int):
+        if self._all_chunk_engines:
+            if self.is_sequence:
+                flat_links: List[str] = []
+                links: List[str] = []
+                for link, props in self.tensor_meta.links.items():
+                    (flat_links if props["flatten_sequence"] else links).append(link)
+
+                if flat_links:
+                    seq_enc = self.sequence_encoder
+                    for link in flat_links:
+                        link_chunk_engine = self._all_chunk_engines[link]
+                        for idx in reversed(range(*seq_enc[index])):
+                            link_chunk_engine.pop(idx)
+            else:
+                links = list(self.tensor_meta.links.keys())
+            [self._all_chunk_engines[link].pop() for link in links]
+
     def get_empty_sample(self):
         if self.num_samples == 0:
             raise ValueError("This tensor has no samples, cannot get empty sample.")
         htype = self.tensor_meta.htype
         dtype = self.tensor_meta.dtype
         if htype in ("text", "json", "list"):
             return get_empty_text_like_sample(htype)
@@ -2511,7 +2696,17 @@
         ):
             self.active_appended_chunk = None
         if (
             self.active_updated_chunk is not None
             and self.active_updated_chunk.key == chunk_key
         ):
             self.active_updated_chunk = None
+
+    def get_avg_chunk_size(self):
+        num_chunks, num_samples = self.num_chunks, self.num_samples
+        max_shape = self.tensor_meta.max_shape
+        dtype = self.tensor_meta.dtype
+        if dtype in ("Any", "List", None):
+            return None
+        nbytes = np.prod([num_samples] + max_shape) * np.dtype(dtype).itemsize
+        avg_chunk_size = nbytes / num_chunks
+        return avg_chunk_size
```

### Comparing `deeplake-3.2.9/deeplake/core/compression.py` & `deeplake-3.3.0/deeplake/core/compression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from logging import warning
 import deeplake
 from deeplake.util.exceptions import (
     SampleCompressionError,
     SampleDecompressionError,
+    SampleReadError,
     UnsupportedCompressionError,
     CorruptedSampleError,
 )
 from deeplake.util.object_3d.read_3d_data import (
     read_3d_data,
 )
 from deeplake.compression import (
@@ -245,14 +246,16 @@
         raise NotImplementedError(
             "In order to store nifti data, you should use `deeplake.read(path_to_file)` or specify sample_compression=None. "
             "Compressing raw data is not yet supported."
         )
     if compression == "apng":
         return _compress_apng(array)
     try:
+        if array.shape == (1, 1, 1):
+            array = array[0]
         img = to_image(array)
         out = BytesIO()
         out._close = out.close  # type: ignore
         out.close = (  # type: ignore
             lambda: None
         )  # sgi save handler will try to close the stream (see https://github.com/python-pillow/Pillow/pull/5645)
         kwargs = {"sizes": [img.size]} if compression == "ico" else {}
@@ -271,14 +274,15 @@
     dtype: Optional[str] = None,
     compression: Optional[str] = None,
     start_idx: Optional[int] = None,
     end_idx: Optional[int] = None,
     step: Optional[int] = None,
     reverse: bool = False,
     to_pil: bool = False,
+    path: Optional[str] = None,
 ) -> Union[np.ndarray, Image.Image]:
     """Decompress some buffer into a numpy array. It is expected that all meta information is
     stored inside `buffer`.
 
     Note:
         `compress_array` may be used to get the `buffer` input.
 
@@ -289,65 +293,69 @@
         dtype (str, Optional): Applicable only for byte compressions. Expected dtype of decompressed array.
         compression (str, Optional): Applicable only for byte compressions. Compression used to compression the given buffer.
         start_idx: (int, Optional): Applicable only for video compressions. Index of first frame.
         end_idx: (int, Optional): Applicable only for video compressions. Index of last frame (exclusive).
         step: (int, Optional): Applicable only for video compressions. Step size for seeking.
         reverse (bool): Applicable only for video compressions. Reverses output numpy array if set to True.
         to_pil (bool): If True, will return a PIL image instead of a numpy array.
+        path (str, Optional): Path to file to be decompressed. Only used for error handling.
 
     Raises:
         SampleDecompressionError: If decompression fails.
         ValueError: If dtype and shape are not specified for byte compression.
 
     Returns:
         Union[np.ndarray, Image.Image]: Decompressed array or PIL image.
     """
     compr_type = get_compression_type(compression)
-    if compr_type == BYTE_COMPRESSION:
-        if dtype is None or shape is None:
-            raise ValueError("dtype and shape must be specified for byte compressions.")
-        try:
+
+    try:
+        if compr_type == BYTE_COMPRESSION:
+            if dtype is None or shape is None:
+                raise ValueError(
+                    "dtype and shape must be specified for byte compressions."
+                )
             decompressed_bytes = decompress_bytes(buffer, compression)  # type: ignore
             return np.frombuffer(decompressed_bytes, dtype=dtype).reshape(shape)
-        except Exception:
-            raise SampleDecompressionError()
-    elif compr_type == AUDIO_COMPRESSION:
-        return _decompress_audio(buffer)
-    elif compr_type == VIDEO_COMPRESSION:
-        return _decompress_video(buffer, start_idx, end_idx, step, reverse)  # type: ignore
-    elif compr_type in [POINT_CLOUD_COMPRESSION, MESH_COMPRESSION]:
-        return _decompress_3d_data(buffer)
-
-    if compression == "apng":
-        return _decompress_apng(buffer)  # type: ignore
-    if compression == "dcm":
-        return _decompress_dicom(buffer)  # type: ignore
-    if compression == "nii":
-        return _decompress_nifti(buffer)
-    if compression == "nii.gz":
-        return _decompress_nifti(buffer, gz=True)
-    if compression is None and isinstance(buffer, memoryview) and shape is not None:
-        assert buffer is not None
-        assert shape is not None
-        return np.frombuffer(buffer=buffer, dtype=dtype).reshape(shape)
+        elif compr_type == AUDIO_COMPRESSION:
+            return _decompress_audio(buffer)
+        elif compr_type == VIDEO_COMPRESSION:
+            return _decompress_video(buffer, start_idx, end_idx, step, reverse)  # type: ignore
+        elif compr_type in [POINT_CLOUD_COMPRESSION, MESH_COMPRESSION]:
+            return _decompress_3d_data(buffer)
+
+        if compression == "apng":
+            return _decompress_apng(buffer)  # type: ignore
+        if compression == "dcm":
+            return _decompress_dicom(buffer)  # type: ignore
+        if compression == "nii":
+            return _decompress_nifti(buffer)
+        if compression == "nii.gz":
+            return _decompress_nifti(buffer, gz=True)
+        if compression is None and isinstance(buffer, memoryview) and shape is not None:
+            assert buffer is not None
+            assert shape is not None
+            return np.frombuffer(buffer=buffer, dtype=dtype).reshape(shape)
+    except Exception as e:
+        raise SampleDecompressionError(path) from e
 
     try:
         if shape is not None and 0 in shape:
             return np.zeros(shape, dtype=dtype)
         if not isinstance(buffer, str):
             buffer = BytesIO(buffer)  # type: ignore
         img = Image.open(buffer)  # type: ignore
         if to_pil:
             return img
         arr = np.array(img)
         if shape is not None:
             arr = arr.reshape(shape)
         return arr
     except Exception:
-        raise SampleDecompressionError()
+        raise SampleDecompressionError(path)
 
 
 def _get_bounding_shape(shapes: Sequence[Tuple[int, ...]]) -> Tuple[int, int, int]:
     """Gets the shape of a bounding box that can contain the given the shapes tiled horizontally."""
     if len(shapes) == 0:
         return (0, 0, 0)
     channels_shape = None
@@ -448,15 +456,17 @@
     file: Union[str, BinaryIO, bytes, memoryview], compression: str
 ) -> Union[Tuple[Tuple[int, ...], str], None]:
     """Verify the contents of an image file
     Args:
         file (Union[str, BinaryIO, bytes, memoryview]): Path to the file or file like object or contents of the file
         compression (str): Expected compression of the image file
     """
+    path = None
     if isinstance(file, str):
+        path = file
         file = open(file, "rb")
         close = True
     elif hasattr(file, "read"):
         close = False
         file.seek(0)  # type: ignore
     else:
         close = False
@@ -480,15 +490,15 @@
                 file = file.read()
             return _read_nifti_shape_and_dtype(file, gz=compression == "nii.gz")
         elif compression in ("las", "ply"):
             return _read_3d_data_shape_and_dtype(file)
         else:
             return _fast_decompress(file)
     except Exception as e:
-        raise CorruptedSampleError(compression)
+        raise CorruptedSampleError(compression, path)
     finally:
         if close:
             file.close()  # type: ignore
 
     return None
 
 
@@ -645,66 +655,70 @@
     return Image._conv_type_shape(img)
 
 
 def read_meta_from_compressed_file(
     file, compression: Optional[str] = None
 ) -> Tuple[str, Tuple[int], str]:
     """Reads shape, dtype and format without decompressing or verifying the sample."""
+    path = None
     if isinstance(file, (str, Path)):
-        f = open(file, "rb")
+        path = str(file)
+        try:
+            f = open(file, "rb")
+        except FileNotFoundError as e:
+            raise SampleReadError(path) from e
         isfile = True
         close = True
     elif hasattr(file, "read"):
         f = file
         close = False
         isfile = True
         f.seek(0)
     else:
         isfile = False
         f = file
         close = False
     try:
         if compression is None:
-            path = file if isinstance(file, str) else None
             if hasattr(f, "read"):
                 compression = get_compression(f.read(32), path)
                 f.seek(0)
             else:
                 compression = get_compression(f[:32], path)  # type: ignore
         if compression == "jpeg":
             try:
                 shape, typestr = _read_jpeg_shape(f), "|u1"
             except Exception:
-                raise CorruptedSampleError("jpeg")
+                raise CorruptedSampleError("jpeg", path)
         elif compression == "png":
             try:
                 shape, typestr = _read_png_shape_and_dtype(f)
             except Exception:
-                raise CorruptedSampleError("png")
+                raise CorruptedSampleError("png", path)
         elif compression == "dcm":
             shape, typestr = _read_dicom_shape_and_dtype(f)
         elif compression == "nii":
             shape, typestr = _read_nifti_shape_and_dtype(file)
         elif compression == "nii.gz":
             shape, typestr = _read_nifti_shape_and_dtype(file, gz=True)
         elif get_compression_type(compression) == AUDIO_COMPRESSION:
             try:
                 shape, typestr = _read_audio_shape(file), "<f4"
             except Exception as e:
-                raise CorruptedSampleError(compression)
+                raise CorruptedSampleError(compression, path)
         elif compression in ("mp4", "mkv", "avi"):
             try:
                 shape, typestr = _read_video_shape(file), "|u1"  # type: ignore
             except Exception as e:
-                raise CorruptedSampleError(compression)
+                raise CorruptedSampleError(compression, path)
         elif compression in ("las", "ply"):
             try:
                 shape, typestr = _read_3d_data_shape_and_dtype(file)
             except Exception as e:
-                raise CorruptedSampleError(compression) from e
+                raise CorruptedSampleError(compression, path) from e
         else:
             img = Image.open(f) if isfile else Image.open(BytesIO(f))  # type: ignore
             shape, typestr = Image._conv_type_shape(img)
             compression = img.format.lower()
         return compression, shape, typestr  # type: ignore
     finally:
         if close:
@@ -1101,17 +1115,15 @@
     meta["duration"] = astream.duration or container.duration
     meta["frame_size"] = astream.frame_size
     meta["nchannels"] = astream.channels
     meta["sample_format"] = astream.format.name
     return meta
 
 
-def _decompress_audio(
-    file: Union[bytes, memoryview, str],
-):
+def _decompress_audio(file: Union[bytes, memoryview, str]):
     container, astream = _open_audio(file)
     shape = _read_shape_from_astream(container, astream)
 
     if shape[0] == 0:
         audio = None
         for frame in container.decode(audio=0):
             if not frame.is_corrupt:
```

### Comparing `deeplake-3.2.9/deeplake/core/compute/process.py` & `deeplake-3.3.0/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/compute/provider.py` & `deeplake-3.3.0/deeplake/core/compute/provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,75 @@
 from abc import ABC, abstractmethod
 from typing import Optional
+import threading
+import warnings
+from tqdm.std import tqdm  # type: ignore
+from tqdm import TqdmWarning  # type: ignore
+
+
+def get_progress_bar(total_length, desc):
+    warnings.simplefilter("ignore", TqdmWarning)
+
+    return tqdm(
+        total=total_length,
+        desc=desc,
+        bar_format="{desc}: {percentage:.0f}%|{bar}| {n:.0f}/{total_fmt} [{elapsed}<{remaining}",
+    )
+
+
+def get_progress_thread(progress_bar, progress_queue):
+    def update_pg(bar, queue):
+        while True:
+            r = queue.get()
+            if r is not None:
+                bar.update(r)
+            else:
+                break
+
+    progress_thread = threading.Thread(
+        target=update_pg, args=(progress_bar, progress_queue)
+    )
+    progress_thread.start()
+    return progress_thread
 
 
 class ComputeProvider(ABC):
     """An abstract base class for implementing a compute provider."""
 
     def __init__(self, workers):
         self.workers = workers
 
-    def get_progressbar(self, total_length, desc):
-        import warnings
-        from tqdm.std import tqdm  # type: ignore
-        from tqdm import TqdmWarning  # type: ignore
-
-        warnings.simplefilter("ignore", TqdmWarning)
-
-        progress_bar = tqdm(
-            total=total_length,
-            desc=desc,
-            bar_format="{desc}: {percentage:.0f}%|{bar}| {n:.0f}/{total_fmt} [{elapsed}<{remaining}",
-        )
-        return progress_bar
-
-    def map_with_progressbar(
-        self, func, iterable, total_length: int, desc: Optional[str] = None
+    def map_with_progress_bar(
+        self,
+        func,
+        iterable,
+        total_length: int,
+        desc: Optional[str] = None,
+        pbar=None,
+        pqueue=None,
     ):
-        import threading
-        from threading import Thread
-
-        progress_bar = self.get_progressbar(total_length, desc)
-        progress_queue = self.create_queue()
+        progress_bar = pbar or get_progress_bar(total_length, desc)
+        progress_queue = pqueue or self.create_queue()
 
         def sub_func(*args, **kwargs):
             def pg_callback(value: int):
                 progress_queue.put(value)  # type: ignore[trust]
-                pass
 
             return func(pg_callback, *args, **kwargs)
 
-        def update_pg(bar, queue):
-            while True:
-                r = queue.get()
-                if r is not None:
-                    bar.update(r)
-                else:
-                    break
-
-        progress_thread: Thread = threading.Thread(
-            target=update_pg, args=(progress_bar, progress_queue)
-        )
-        progress_thread.start()
+        progress_thread = get_progress_thread(progress_bar, progress_queue)
 
         try:
             result = self.map(sub_func, iterable)
         finally:
             progress_queue.put(None)  # type: ignore[trust]
+            if pqueue is None and hasattr(progress_queue, "close"):
+                progress_queue.close()
             progress_thread.join()
-            progress_bar.close()
-
-            if hasattr(progress_queue, "close"):
+            if pbar is None:
                 progress_bar.close()
 
         return result
 
     @abstractmethod
     def create_queue(self):
         """Creates queue for specific provider"""
```

### Comparing `deeplake-3.2.9/deeplake/core/compute/ray.py` & `deeplake-3.3.0/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/compute/thread.py` & `deeplake-3.3.0/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/dataset/__init__.py` & `deeplake-3.3.0/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/dataset/dataset.py` & `deeplake-3.3.0/deeplake/core/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,47 +5,56 @@
 import posixpath
 from logging import warning
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 from functools import partial
 
 import pathlib
 import numpy as np
-from time import time
+from time import time, sleep
 from tqdm import tqdm  # type: ignore
 
 import deeplake
 from deeplake.core.index.index import IndexEntry
 from deeplake.core.link_creds import LinkCreds
 from deeplake.util.connect_dataset import connect_dataset_entry
 from deeplake.util.downsample import validate_downsampling
+from deeplake.util.version_control import (
+    save_version_info,
+    integrity_check,
+    save_commit_info,
+    rebuild_version_info,
+)
 from deeplake.util.invalid_view_op import invalid_view_op
+from deeplake.util.spinner import spinner
 from deeplake.util.iteration_warning import (
     suppress_iteration_warning,
     check_if_iteration,
 )
 from deeplake.api.info import load_info
 from deeplake.client.log import logger
 from deeplake.client.utils import get_user_name
 from deeplake.constants import (
     FIRST_COMMIT_ID,
     DEFAULT_MEMORY_CACHE_SIZE,
     DEFAULT_LOCAL_CACHE_SIZE,
     MB,
     SAMPLE_INFO_TENSOR_MAX_CHUNK_SIZE,
     DEFAULT_READONLY,
+    ENV_HUB_DEV_USERNAME,
 )
 from deeplake.core.fast_forwarding import ffw_dataset_meta
 from deeplake.core.index import Index
 from deeplake.core.lock import lock_dataset, unlock_dataset, Lock
 from deeplake.core.meta.dataset_meta import DatasetMeta
 from deeplake.core.storage import (
     LRUCache,
     S3Provider,
     GCSProvider,
     MemoryProvider,
+    LocalProvider,
 )
 from deeplake.core.tensor import Tensor, create_tensor, delete_tensor
 from deeplake.core.version_control.commit_node import CommitNode  # type: ignore
 from deeplake.core.version_control.dataset_diff import load_dataset_diff
 from deeplake.htype import (
     HTYPE_CONFIGURATIONS,
     UNSPECIFIED,
@@ -78,69 +87,61 @@
     InvalidTensorGroupNameError,
     LockedException,
     TensorGroupAlreadyExistsError,
     ReadOnlyModeError,
     RenameError,
     EmptyCommitError,
     DatasetViewSavingError,
-    DatasetHandlerError,
     SampleAppendingError,
     DatasetTooLargeToDelete,
     TensorTooLargeToDelete,
     GroupInfoNotSupportedError,
     TokenPermissionError,
+    CheckoutError,
+    DatasetCorruptError,
 )
 from deeplake.util.keys import (
     dataset_exists,
     get_dataset_info_key,
     get_dataset_meta_key,
     tensor_exists,
     get_queries_key,
     get_queries_lock_key,
     get_sample_id_tensor_key,
     get_sample_info_tensor_key,
     get_sample_shape_tensor_key,
     get_downsampled_tensor_key,
     filter_name,
-    get_tensor_meta_key,
-    get_tensor_commit_diff_key,
-    get_tensor_tile_encoder_key,
-    get_tensor_info_key,
-    get_tensor_commit_chunk_map_key,
-    get_chunk_id_encoder_key,
-    get_dataset_diff_key,
-    get_sequence_encoder_key,
     get_dataset_linked_creds_key,
 )
 from deeplake.util.path import get_path_from_storage
 from deeplake.util.remove_cache import get_base_storage
 from deeplake.util.diff import get_all_changes_string, get_changes_and_messages
 from deeplake.util.version_control import (
     auto_checkout,
     checkout,
     commit,
     current_commit_has_change,
     load_meta,
     warn_node_checkout,
     load_version_info,
-    copy_metas,
-    create_commit_chunk_maps,
     save_version_info,
-    generate_hash,
+    replace_head,
+    reset_and_checkout,
 )
 from deeplake.util.pretty_print import summary_dataset
 from deeplake.core.dataset.view_entry import ViewEntry
 from deeplake.core.dataset.invalid_view import InvalidView
 from deeplake.hooks import dataset_read
 from itertools import chain
 import warnings
 import jwt
 
 
-_LOCKABLE_STORAGES = {S3Provider, GCSProvider}
+_LOCKABLE_STORAGES = {S3Provider, GCSProvider, LocalProvider}
 
 
 class Dataset:
     def __init__(
         self,
         storage: LRUCache,
         index: Optional[Index] = None,
@@ -148,14 +149,15 @@
         read_only: Optional[bool] = None,
         public: Optional[bool] = False,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         verbose: bool = True,
         version_state: Optional[Dict[str, Any]] = None,
         path: Optional[Union[str, pathlib.Path]] = None,
+        address: Optional[str] = None,
         is_iteration: bool = False,
         link_creds=None,
         pad_tensors: bool = False,
         lock: bool = True,
         enabled_tensors: Optional[List[str]] = None,
         view_base: Optional["Dataset"] = None,
         libdeeplake_dataset=None,
@@ -171,14 +173,15 @@
                 Datasets stored on Deep Lake cloud that your account does not have write access to will automatically open in read mode.
             public (bool, Optional): Applied only if storage is Deep Lake cloud storage and a new Dataset is being created. Defines if the dataset will have public access.
             token (str, Optional): Activeloop token, used for fetching credentials for Deep Lake datasets. This is Optional, tokens are normally autogenerated.
             org_id (str, Optional): Organization id to be used for enabling enterprise features. Only applicable for local datasets.
             verbose (bool): If ``True``, logs will be printed. Defaults to True.
             version_state (Dict[str, Any], Optional): The version state of the dataset, includes commit_id, commit_node, branch, branch_commit_map and commit_node_map.
             path (str, pathlib.Path): The path to the dataset.
+            address (Optional[str]): The version address of the dataset.
             is_iteration (bool): If this Dataset is being used as an iterator.
             link_creds (LinkCreds, Optional): The LinkCreds object used to access tensors that have external data linked to them.
             pad_tensors (bool): If ``True``, shorter tensors will be padded to the length of the longest tensor.
             **kwargs: Passing subclass variables through without errors.
             lock (bool): Whether the dataset should be locked for writing. Only applicable for S3, Deep Lake storage and GCS datasets. No effect if read_only=True.
             enabled_tensors (List[str], Optional): List of tensors that are enabled in this view. By default all tensors are enabled.
             view_base (Optional["Dataset"]): Base dataset of this view.
@@ -225,19 +228,20 @@
         d["_update_hooks"] = {}
         d["_commit_hooks"] = {}
         d["_checkout_hooks"] = {}
         d["_parent_dataset"] = None
         d["_pad_tensors"] = pad_tensors
         d["_locking_enabled"] = lock
         d["_temp_tensors"] = []
+        d["_vc_info_updated"] = True
         dct = self.__dict__
         dct.update(d)
 
         try:
-            self._set_derived_attributes()
+            self._set_derived_attributes(address=address)
         except LockedException:
             raise LockedException(
                 "This dataset cannot be open for writing as it is locked by another machine. Try loading the dataset with `read_only=True`."
             )
         except ReadOnlyModeError as e:
             raise ReadOnlyModeError(
                 "This dataset cannot be open for writing as you don't have permissions. Try loading the dataset with `read_only=True."
@@ -269,17 +273,27 @@
 
     def __enter__(self):
         self._initial_autoflush.append(self.storage.autoflush)
         self.storage.autoflush = False
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.storage.autoflush = self._initial_autoflush.pop()
+        autoflush = self._initial_autoflush.pop()
+        if not self._read_only and autoflush:
+            if self._vc_info_updated:
+                self._flush_vc_info()
+            spinner(self.storage.flush)()
+        self.storage.autoflush = autoflush
+
+    def maybe_flush(self):
         if not self._read_only:
-            self.storage.maybe_flush()
+            if self.storage.autoflush:
+                if self._vc_info_updated:
+                    self._flush_vc_info()
+                self.storage.flush()
 
     @property
     def num_samples(self) -> int:
         """Returns the length of the smallest tensor.
         Ignores any applied indexing and returns the total length.
         """
         return min(
@@ -378,25 +392,23 @@
         state["_view_base"] = None
         state["_update_hooks"] = {}
         state["_commit_hooks"] = {}
         state["_checkout_hooks"] = {}
         state["_client"] = state["org_id"] = state["ds_name"] = None
         state["_temp_tensors"] = []
         state["libdeeplake_dataset"] = None
+        state["_vc_info_updated"] = False
+        state["_locked_out"] = False
         self.__dict__.update(state)
         self.__dict__["base_storage"] = get_base_storage(self.storage)
         # clear cache while restoring
         self.storage.clear_cache_without_flush()
         self._set_derived_attributes(verbose=False)
         self._indexing_history = []
 
-        for temp_tensor in self._temp_tensors:
-            self.delete_tensor(temp_tensor, large_ok=True)
-        self._temp_tensors = []
-
     def _reload_version_state(self):
         version_state = self.version_state
         # share version state if at HEAD
         if (
             not self._view_use_parent_commit
             and self._view_base
             and version_state["commit_node"].is_head_node
@@ -503,14 +515,18 @@
                 group_index = self.group_index
                 enabled_tensors = [
                     posixpath.join(
                         group_index, (x if isinstance(x, str) else "/".join(x))
                     )
                     for x in item
                 ]
+                for x in enabled_tensors:
+                    enabled_tensors.extend(
+                        self[posixpath.relpath(x, self.group_index)].meta.links.keys()
+                    )
                 ret = self.__class__(
                     storage=self.storage,
                     index=self.index,
                     group_index=self.group_index,
                     read_only=self._read_only,
                     token=self._token,
                     verbose=False,
@@ -1197,29 +1213,55 @@
     def __iter__(self):
         dataset_read(self)
         for i in range(len(self)):
             yield self.__getitem__(
                 i, is_iteration=not isinstance(self.index.values[0], list)
             )
 
-    def _load_version_info(self):
+    def _load_version_info(self, address=None):
         """Loads data from version_control_file otherwise assume it doesn't exist and load all empty"""
         if self.version_state:
             return
 
-        branch = "main"
-        version_state = {"branch": branch}
+        if address is None:
+            address = "main"
+
+        version_state = {}
         try:
-            version_info = load_version_info(self.storage)
+            try:
+                version_info = load_version_info(self.storage)
+            except Exception as e:
+                version_info = rebuild_version_info(self.storage)
+                if version_info is None:
+                    raise e
             version_state["branch_commit_map"] = version_info["branch_commit_map"]
             version_state["commit_node_map"] = version_info["commit_node_map"]
-            commit_id = version_state["branch_commit_map"][branch]
+
+            if address in version_state["branch_commit_map"]:
+                branch = address
+                commit_id = version_state["branch_commit_map"][branch]
+            elif address in version_state["commit_node_map"]:
+                commit_id = address
+            else:
+                raise CheckoutError(
+                    f"Address {address} not found. Ensure the commit id / branch name is correct."
+                )
+
             version_state["commit_id"] = commit_id
             version_state["commit_node"] = version_state["commit_node_map"][commit_id]
-        except Exception:
+            version_state["branch"] = version_state["commit_node"].branch
+        except Exception as e:
+            if isinstance(e, CheckoutError):
+                raise e from None
+            if address != "main":
+                raise CheckoutError(
+                    f"Address {address} not found. Ensure the commit id / branch name is correct."
+                )
+            branch = "main"
+            version_state["branch"] = branch
             version_state["branch_commit_map"] = {}
             version_state["commit_node_map"] = {}
             # used to identify that this is the first commit so its data will not be in similar directory structure to the rest
             commit_id = FIRST_COMMIT_ID
             commit_node = CommitNode(branch, commit_id)
             version_state["commit_id"] = commit_id
             version_state["commit_node"] = commit_node
@@ -1242,25 +1284,29 @@
         if data_bytes is None:
             link_creds = LinkCreds()
         else:
             link_creds = LinkCreds.frombuffer(data_bytes)
         self.link_creds = link_creds
 
     def _lock(self, err=False, verbose=True):
-        if not self._locking_enabled:
+        if not self.is_head_node or not self._locking_enabled:
             return True
         storage = self.base_storage
         if storage.read_only and not self._locked_out:
             if err:
                 raise ReadOnlyModeError()
             return False
 
         if isinstance(storage, tuple(_LOCKABLE_STORAGES)) and (
             not self.read_only or self._locked_out
         ):
+            if not deeplake.constants.LOCK_LOCAL_DATASETS and isinstance(
+                storage, LocalProvider
+            ):
+                return True
             try:
                 # temporarily disable read only on base storage, to try to acquire lock, if exception, it will be again made readonly
                 storage.disable_readonly()
                 lock_dataset(
                     self,
                     lock_lost_callback=self._lock_lost_handler,
                 )
@@ -1297,14 +1343,15 @@
             except KeyError:
                 pass
         try:
             self._unlock()
         except Exception:  # python shutting down
             pass
 
+    @spinner
     @invalid_view_op
     def commit(self, message: Optional[str] = None, allow_empty=False) -> str:
         """Stores a snapshot of the current state of the dataset.
 
         Args:
             message (str, Optional): Used to describe the commit.
             allow_empty (bool): If ``True``, commit even if there are no changes.
@@ -1321,17 +1368,18 @@
             - This same behaviour will happen if new samples are added or existing samples are updated from a non-head node.
         """
         if not allow_empty and not self.has_head_changes:
             raise EmptyCommitError(
                 "There are no changes, commit is not done. Try again with allow_empty=True."
             )
 
-        return self._commit(message)
+        return self._commit(message, None, False)
 
     @deeplake_reporter.record_call
+    @spinner
     @invalid_view_op
     @suppress_iteration_warning
     def merge(
         self,
         target_id: str,
         conflict_resolution: Optional[str] = None,
         delete_removed_tensors: bool = False,
@@ -1370,55 +1418,68 @@
                 f"conflict_resolution must be one of None, 'ours', or 'theirs'. Got {conflict_resolution}"
             )
 
         try_flushing(self)
 
         self._initial_autoflush.append(self.storage.autoflush)
         self.storage.autoflush = False
-
         merge(self, target_id, conflict_resolution, delete_removed_tensors, force)
-
         self.storage.autoflush = self._initial_autoflush.pop()
+        self.storage.maybe_flush()
 
-    def _commit(self, message: Optional[str] = None, hash: Optional[str] = None) -> str:
+    def _commit(
+        self,
+        message: Optional[str] = None,
+        hash: Optional[str] = None,
+        flush_version_control_info: bool = True,
+    ) -> str:
         if self._is_filtered_view:
             raise Exception(
                 "Cannot perform version control operations on a filtered dataset view."
             )
 
         try_flushing(self)
 
         self._initial_autoflush.append(self.storage.autoflush)
         self.storage.autoflush = False
         try:
             self._unlock()
-            commit(self, message, hash)
+            commit(self, message, hash, flush_version_control_info)
+            if not flush_version_control_info:
+                self.__dict__["_vc_info_updated"] = True
             self._lock()
         finally:
             self.storage.autoflush = self._initial_autoflush.pop()
         self._info = None
         self._ds_diff = None
         [f() for f in list(self._commit_hooks.values())]
         # do not store commit message
         deeplake_reporter.feature_report(feature_name="commit", parameters={})
-
+        self.maybe_flush()
         return self.commit_id  # type: ignore
 
     @invalid_view_op
-    def checkout(self, address: str, create: bool = False) -> Optional[str]:
+    def checkout(
+        self, address: str, create: bool = False, reset: bool = False
+    ) -> Optional[str]:
         """Checks out to a specific commit_id or branch. If ``create = True``, creates a new branch with name ``address``.
 
         Args:
             address (str): The commit_id or branch to checkout to.
             create (bool): If ``True``, creates a new branch with name as address.
+            reset (bool): If checkout fails due to a corrupted HEAD state of the branch, setting ``reset=True`` will
+                          reset HEAD changes and attempt the checkout again.
 
         Returns:
             Optional[str]: The commit_id of the dataset after checkout.
 
         Raises:
+            CheckoutError: If ``address`` could not be found.
+            ReadOnlyModeError: If branch creation or reset is attempted in read-only mode.
+            DatasetCorruptError: If checkout failed due to dataset corruption and ``reset`` is not ``True``.
             Exception: If the dataset is a filtered view.
 
         Examples:
 
             >>> ds = deeplake.empty("../test/test_ds")
             >>> ds.create_tensor("abc")
             Tensor(key='abc')
@@ -1434,62 +1495,79 @@
             'firstdbf9474d461a19e9333c2fd19b46115348f'
             >>> ds.abc.numpy()
             array([[1, 2, 3]])
 
         Note:
             Checkout from a head node in any branch that contains uncommitted data will lead to an automatic commit before the checkout.
         """
-        return self._checkout(address, create)
+        try:
+            ret = self._checkout(address, create, None, False)
+            integrity_check(self)
+            return ret
+        except (ReadOnlyModeError, CheckoutError) as e:
+            raise e from None
+        except Exception as e:
+            if create:
+                raise e
+            if not reset:
+                if isinstance(e, DatasetCorruptError):
+                    raise DatasetCorruptError(
+                        message=e.message,
+                        action="Try using `reset=True` to reset HEAD changes and load the previous commit.",
+                        cause=e.__cause__,
+                    )
+                raise DatasetCorruptError(
+                    "Exception occured (see Traceback). The branch you are checking out to maybe corrupted."
+                    "Try using `reset=True` to reset HEAD changes and load the previous commit."
+                    "This will delete all uncommitted changes on the branch you are trying to load."
+                ) from e
+            if self.read_only:
+                raise ReadOnlyModeError("Cannot reset HEAD in read-only mode.")
+            return reset_and_checkout(self, address, e)
 
     def _checkout(
         self,
         address: str,
         create: bool = False,
         hash: Optional[str] = None,
-        verbose=True,
+        verbose: bool = True,
+        flush_version_control_info: bool = False,
     ) -> Optional[str]:
         if self._is_filtered_view:
             raise Exception(
                 "Cannot perform version control operations on a filtered dataset view."
             )
-        if self._locked_out:
-            self.storage.disable_readonly()
-            self._read_only = False
-            self.base_storage.disable_readonly()
+        read_only = self._read_only
+        if read_only and create:
+            raise ReadOnlyModeError()
         try_flushing(self)
         self._initial_autoflush.append(self.storage.autoflush)
         self.storage.autoflush = False
-        err = False
         try:
             self._unlock()
-            checkout(self, address, create, hash)
-        except Exception as e:
-            err = True
-            if self._locked_out:
-                self.storage.enable_readonly()
-                self._read_only = True
-                self.base_storage.enable_readonly()
-            raise e
+            checkout(self, address, create, hash, flush_version_control_info)
+            if not flush_version_control_info and create:
+                self.__dict__["_vc_info_updated"] = True
         finally:
-            if not (err and self._locked_out):
-                self._lock(verbose=verbose)
+            self._set_read_only(read_only, err=True)
             self.storage.autoflush = self._initial_autoflush.pop()
         self._info = None
         self._ds_diff = None
 
         [f() for f in list(self._checkout_hooks.values())]
 
         # do not store address
         deeplake_reporter.feature_report(
             feature_name="checkout", parameters={"Create": str(create)}
         )
         commit_node = self.version_state["commit_node"]
         if self.verbose:
             warn_node_checkout(commit_node, create)
-
+        if create:
+            self.maybe_flush()
         return self.commit_id
 
     @deeplake_reporter.record_call
     def log(self):
         """Displays the details of all the past commits."""
         commit_node = self.version_state["commit_node"]
         print("---------------\nDeep Lake Version Log\n---------------\n")
@@ -1556,16 +1634,14 @@
         all_changes = get_all_changes_string(*res)
         print(all_changes)
         return None
 
     def _populate_meta(self, verbose=True):
         """Populates the meta information for the dataset."""
         if dataset_exists(self.storage):
-            if verbose and self.verbose:
-                logger.info(f"{self.path} loaded successfully.")
             load_meta(self)
 
         elif not self.storage.empty():
             # dataset does not exist, but the path was not empty
             raise PathNotEmptyException
 
         else:
@@ -1576,15 +1652,16 @@
             key = get_dataset_meta_key(self.version_state["commit_id"])
             self.version_state["meta"] = meta
             self.storage.register_deeplake_object(key, meta)
             self._register_dataset()
             self.flush()
 
     def _register_dataset(self):
-        """overridden in DeepLakeCloudDataset"""
+        if not self.__dict__["org_id"]:
+            self.org_id = os.environ.get(ENV_HUB_DEV_USERNAME)
 
     def _send_query_progress(self, *args, **kwargs):
         """overridden in DeepLakeCloudDataset"""
 
     def _send_compute_progress(self, *args, **kwargs):
         """overridden in DeepLakeCloudDataset"""
 
@@ -1620,36 +1697,51 @@
     @property
     def has_head_changes(self):
         """Returns True if currently at head node and uncommitted changes are present."""
         return self.is_head_node and current_commit_has_change(
             self.version_state, self.storage
         )
 
+    def _acquire_lock(self, timeout: Optional[int] = None):
+        if timeout is not None:
+            start_time = time()
+        while True:
+            try:
+                self._set_read_only(False, True)
+                return
+            except LockedException:
+                if timeout is not None and time() - start_time > timeout:
+                    raise LockedException()
+                sleep(1)
+
     def _set_read_only(self, value: bool, err: bool):
         storage = self.storage
         self.__dict__["_read_only"] = value
+
         if value:
             storage.enable_readonly()
             if isinstance(storage, LRUCache) and storage.next_storage is not None:
                 storage.next_storage.enable_readonly()
+            self._unlock()
         else:
             try:
                 locked = self._lock(err=err)
                 if locked:
                     self.storage.disable_readonly()
                     if (
                         isinstance(storage, LRUCache)
                         and storage.next_storage is not None
                     ):
                         storage.next_storage.disable_readonly()
                 else:
                     self.__dict__["_read_only"] = True
             except LockedException as e:
                 self.__dict__["_read_only"] = True
-                raise e
+                if err:
+                    raise e
 
     @read_only.setter
     @invalid_view_op
     def read_only(self, value: bool):
         self._set_read_only(value, True)
 
     @deeplake_reporter.record_call
@@ -1958,19 +2050,21 @@
     def _get_total_meta(self):
         """Returns tensor metas all together"""
         return {
             tensor_key: tensor_value.meta
             for tensor_key, tensor_value in self.version_state["full_tensors"].items()
         }
 
-    def _set_derived_attributes(self, verbose: bool = True):
+    def _set_derived_attributes(
+        self, verbose: bool = True, address: Optional[str] = None
+    ):
         """Sets derived attributes during init and unpickling."""
         if self.is_first_load:
             self.storage.autoflush = True
-            self._load_version_info()
+            self._load_version_info(address)
             self._load_link_creds()
             self._set_read_only(
                 self._read_only, err=self._read_only_error
             )  # TODO: weird fix for dataset unpickling
             self._populate_meta(verbose)  # TODO: use the same scheme as `load_info`
             if self.index.is_trivial():
                 self.index = Index.from_json(self.meta.default_index)
@@ -2036,22 +2130,32 @@
             tf.data.Dataset object that can be used for tensorflow training.
         """
         dataset_read(self)
         return dataset_to_tensorflow(
             self, tensors=tensors, tobytes=tobytes, fetch_chunks=fetch_chunks
         )
 
+    @spinner
     def flush(self):
         """Necessary operation after writes if caches are being used.
         Writes all the dirty data from the cache layers (if any) to the underlying storage.
         Here dirty data corresponds to data that has been changed/assigned and but hasn't yet been sent to the
         underlying storage.
         """
+        self._flush_vc_info()
         self.storage.flush()
 
+    def _flush_vc_info(self):
+        if self._vc_info_updated:
+            save_version_info(self.version_state, self.storage)
+            for node in self.version_state["commit_node_map"].values():
+                if node._info_updated:
+                    save_commit_info(node, self.storage)
+            self.__dict__["_vc_info_updated"] = False
+
     def clear_cache(self):
         """
         - Flushes (see :func:`Dataset.flush`) the contents of the cache layers (if any) and then deletes contents of all the layers of it.
         - This doesn't delete data from the actual storage.
         - This is useful if you have multiple datasets with memory caches open, taking up too much RAM.
         - Also useful when local cache is no longer needed for certain datasets and is taking up storage space.
         """
@@ -2117,14 +2221,15 @@
                 raise DatasetTooLargeToDelete(self.path)
 
         self._unlock()
         self.storage.clear()
 
     def summary(self):
         """Prints a summary of the dataset."""
+
         pretty_print = summary_dataset(self)
 
         print(self)
         print(pretty_print)
 
     def __str__(self):
         path_str = ""
@@ -2460,14 +2565,15 @@
             self,
             num_workers=num_workers,
             scheduler=scheduler,
             progressbar=progressbar,
             skip_ok=True,
             extend_only=True,
             disable_label_sync=True,
+            disable_rechunk=True,
         )
 
     # the below methods are used by cloudpickle dumps
     def __origin__(self):
         return None
 
     def __values__(self):
@@ -2545,45 +2651,46 @@
             >>> ds.create_tensor('data')
             Tensor(key='data')
             >>> ds.create_tensor('labels')
             Tensor(key='labels')
             >>> ds.append({"data": [1, 2, 3, 4], "labels":[0, 1, 2, 3]})
 
         """
+        tensors = self.tensors
         if isinstance(sample, Dataset):
             sample = sample.tensors
         if not isinstance(sample, dict):
             raise SampleAppendingError()
 
-        skipped_tensors = [k for k in self.tensors if k not in sample]
+        skipped_tensors = [k for k in tensors if k not in sample]
         if skipped_tensors and not skip_ok and not append_empty:
             raise KeyError(
                 f"Required tensors not provided: {skipped_tensors}. Pass either `skip_ok=True` to skip tensors or `append_empty=True` to append empty samples to unspecified tensors."
             )
         for k in sample:
-            if k not in self._tensors():
+            if k not in tensors:
                 raise TensorDoesNotExistError(k)
-        tensors_to_check_length = self.tensors if append_empty else sample
-        if len(set(map(len, (self[k] for k in tensors_to_check_length)))) != 1:
+        tensors_to_check_length = tensors if append_empty else sample
+        if len(set(map(len, (tensors[k] for k in tensors_to_check_length)))) != 1:
             raise ValueError(
                 "When appending using Dataset.append, all tensors being updated are expected to have the same length."
             )
         [f() for f in list(self._update_hooks.values())]
         tensors_appended = []
         with self:
-            for k in self.tensors:
+            for k in tensors:
                 if k in sample:
                     v = sample[k]
                 else:
                     if skip_ok:
                         continue
                     else:
                         v = None
                 try:
-                    tensor = self[k]
+                    tensor = tensors[k]
                     enc = tensor.chunk_engine.chunk_id_encoder
                     num_chunks = enc.num_chunks
                     tensor.append(v)
                     tensors_appended.append(k)
                 except Exception as e:
                     new_num_chunks = enc.num_chunks
                     num_chunks_added = new_num_chunks - num_chunks
@@ -2596,25 +2703,26 @@
                     elif num_chunks_added == 1:
                         enc._encoded = enc._encoded[:-1]
                     for k in tensors_appended:
                         try:
                             self[k].pop()
                         except Exception as e2:
                             raise Exception(
-                                "Error while attepting to rollback appends"
+                                "Error while attempting to rollback appends"
                             ) from e2
                     raise e
 
     def _view_hash(self) -> str:
         """Generates a unique hash for a filtered dataset view."""
         return hash_inputs(
             self.path,
             *[e.value for e in self.index.values],
             self.pending_commit_id,
             getattr(self, "_query", None),
+            getattr(self, "_tql_query", None),
         )
 
     def _get_view_info(
         self,
         id: Optional[str] = None,
         message: Optional[str] = None,
         copy: bool = False,
@@ -2635,26 +2743,30 @@
         }
         if message is not None:
             info["message"] = message
         query = getattr(self, "_query", None)
         if query:
             info["query"] = query
             info["source-dataset-index"] = getattr(self, "_source_ds_idx", None)
+        tql_query = getattr(self, "_tql_query", None)
+        if tql_query:
+            info["tql_query"] = tql_query
+            info["source-dataset-index"] = getattr(self, "_source_ds_idx", None)
         return info
 
     def _lock_queries_json(self):
         class _LockQueriesJson:
             def __enter__(self2):
                 storage = self.base_storage
                 self2.storage_read_only = storage.read_only
                 if self._locked_out:
                     # Ignore storage level lock since we have file level lock
                     storage.read_only = False
                 lock = Lock(storage, get_queries_lock_key())
-                lock.acquire(timeout=10, force=True)
+                lock.acquire(timeout=10)
                 self2.lock = lock
 
             def __exit__(self2, *_, **__):
                 self2.lock.release()
                 self.base_storage.read_only = self2.storage_read_only
 
         return _LockQueriesJson()
@@ -2825,19 +2937,22 @@
 
         Returns:
             str: Path to the saved VDS.
 
         Raises:
             ReadOnlyModeError: When attempting to save a view inplace and the user doesn't have write access.
             DatasetViewSavingError: If HEAD node has uncommitted changes.
+            TypeError: If ``id`` is not of type ``str``.
 
         Note:
             Specifying ``path`` makes the view external. External views cannot be accessed using the parent dataset's :func:`Dataset.get_view`,
             :func:`Dataset.load_view`, :func:`Dataset.delete_view` methods. They have to be loaded using :func:`deeplake.load`.
         """
+        if id is not None and not isinstance(id, str):
+            raise TypeError(f"id {id} is of type {type(id)}, expected `str`.")
         return self._save_view(
             path,
             id,
             message,
             optimize,
             tensors,
             num_workers,
@@ -2882,32 +2997,34 @@
 
         Raises:
             ReadOnlyModeError: When attempting to save a view inplace and the user doesn't have write access.
             NotImplementedError: When attempting to save in-memory datasets.
         """
 
         path = convert_pathlib_to_string_if_needed(path)
-
         ds_args["verbose"] = False
         vds = None
         if path is None and hasattr(self, "_vds"):
             vds = self._vds
             vds_id = vds.info["id"]
             if id is not None and vds_id != id:
                 vds = None
                 warnings.warn(
                     f"This view is already saved with id '{vds_id}'. A copy of this view will be created with the provided id '{id}'"
                 )
+        base = self._view_base or self
+        if not base._read_only:
+            base.flush()
         if vds is None:
             if path is None:
                 if isinstance(self, MemoryProvider):
                     raise NotImplementedError(
                         "Saving views inplace is not supported for in-memory datasets."
                     )
-                if self.read_only and not (self._view_base or self)._locked_out:
+                if self.read_only and not base._locked_out:
                     if isinstance(self, deeplake.core.dataset.DeepLakeCloudDataset):
                         try:
                             with self._temp_write_access():
                                 vds = self._save_view_in_subdir(
                                     id,
                                     message,
                                     optimize,
@@ -2972,14 +3089,15 @@
                 creds=creds,
                 read_only=True,
                 token=self._token,
             )
         )
 
         ds.index = Index()
+        ds.version_state = ds.version_state.copy()
         ds._checkout(commit_id, verbose=False)
         first_index_subscriptable = self.info.get("first-index-subscriptable", True)
         if first_index_subscriptable:
             index_entries = [IndexEntry(self.VDS_INDEX.numpy().reshape(-1).tolist())]
         else:
             index_entries = [IndexEntry(int(self.VDS_INDEX.numpy()))]
         sub_sample_index = self.info.get("sub-sample-index")
@@ -3012,29 +3130,25 @@
         return view._save_view(vds_path, _ret_ds=True, **vds_args)
 
     def get_views(self, commit_id: Optional[str] = None) -> List[ViewEntry]:
         """Returns list of views stored in this Dataset.
 
         Args:
             commit_id (str, optional): - Commit from which views should be returned.
-                - If not specified, views from current commit is returned.
-                - If not specified, views from the currently checked out commit will be returned.
+                - If not specified, views from all commits are returned.
 
         Returns:
             List[ViewEntry]: List of :class:`ViewEntry` instances.
         """
-        commit_id = commit_id or self.commit_id
         queries = self._read_queries_json()
-        f = lambda x: x["source-dataset-version"] == commit_id
-        ret = map(
-            partial(ViewEntry, dataset=self),
-            filter(f, queries),
-        )
-
-        return list(ret)
+        if commit_id is not None:
+            queries = filter(
+                lambda x: x["source-dataset-version"] == commit_id, queries
+            )
+        return list(map(partial(ViewEntry, dataset=self), queries))
 
     def get_view(self, id: str) -> ViewEntry:
         """Returns the dataset view corresponding to ``id``.
 
         Examples:
             >>> # save view
             >>> ds[:100].save_view(id="first_100")
@@ -3084,26 +3198,23 @@
 
         Returns:
             Dataset: The loaded view.
 
         Raises:
             KeyError: if view with given id does not exist.
         """
+        view = self.get_view(id)
         if optimize:
-            return (
-                self.get_view(id)
-                .optimize(
-                    tensors=tensors,
-                    num_workers=num_workers,
-                    scheduler=scheduler,
-                    progressbar=progressbar,
-                )
-                .load()
-            )
-        return self.get_view(id).load()
+            return view.optimize(
+                tensors=tensors,
+                num_workers=num_workers,
+                scheduler=scheduler,
+                progressbar=progressbar,
+            ).load()
+        return view.load()
 
     def delete_view(self, id: str):
         """Deletes the view with given view id.
 
         Args:
             id (str): Id of the view to delete.
 
@@ -3153,15 +3264,15 @@
 
         Returns:
             Sub dataset
 
         Note:
             Virtual datasets are returned as such, they are not converted to views.
         """
-        sub_storage = self.base_storage.subdir(path)
+        sub_storage = self.base_storage.subdir(path, read_only=read_only)
 
         if empty:
             sub_storage.clear()
 
         if self.path.startswith("hub://"):
             path = posixpath.join(self.path, path)
             cls = deeplake.core.dataset.DeepLakeCloudDataset
@@ -3434,64 +3545,50 @@
             num_workers,
             scheduler,
             progressbar,
             public,
         )
 
     @invalid_view_op
-    def reset(self):
+    @spinner
+    def reset(self, force: bool = False):
         """Resets the uncommitted changes present in the branch.
 
         Note:
             The uncommitted data is deleted from underlying storage, this is not a reversible operation.
         """
         storage, version_state = self.storage, self.version_state
         if version_state["commit_node"].children:
             print("You are not at the head node of the branch, cannot reset.")
             return
-        if not self.has_head_changes:
+        if not self.has_head_changes and not force:
             print("There are no uncommitted changes on this branch.")
             return
 
         if self.commit_id is None:
             storage.clear()
             self._populate_meta()
             load_meta(self)
         else:
-            reset_commit_id = self.pending_commit_id
-            deletion_folder = "/".join(("versions", reset_commit_id))
-            new_commit_id = generate_hash()
-            new_branch = self.branch
-
             parent_commit_id = self.commit_id
+            reset_commit_id = self.pending_commit_id
 
             # checkout to get list of tensors in previous commit, needed for copying metas and create_commit_chunk_set
             self.checkout(parent_commit_id)
 
-            # populate new commit folder
-            copy_metas(parent_commit_id, new_commit_id, storage, version_state)
-            create_commit_chunk_maps(new_commit_id, storage, version_state)
-
-            # update and save version state
-            parent_node: CommitNode = version_state["commit_node"]
-            new_node = CommitNode(new_branch, new_commit_id)
-            new_node.parent = parent_node
-            version_state["branch_commit_map"][new_branch] = new_commit_id
-            version_state["commit_node_map"][new_commit_id] = new_node
-            del version_state["commit_node_map"][reset_commit_id]
-            for i, child in enumerate(parent_node.children):
-                if child.commit_id == reset_commit_id:
-                    parent_node.children[i] = new_node
-                    break
-            save_version_info(version_state, storage)
+            new_commit_id = replace_head(storage, version_state, reset_commit_id)
 
-            # clear the old folder
-            storage.clear(prefix=deletion_folder)
             self.checkout(new_commit_id)
 
+    def fix_vc(self):
+        """Rebuilds version control info. To be used when the version control info is corrupted."""
+        version_info = rebuild_version_info(self.storage)
+        self.version_state["commit_node_map"] = version_info["commit_node_map"]
+        self.version_state["branch_commit_map"] = version_info["branch_commit_map"]
+
     def connect(
         self,
         creds_key: str,
         dest_path: Optional[str] = None,
         org_id: Optional[str] = None,
         ds_name: Optional[str] = None,
         token: Optional[str] = None,
@@ -3559,68 +3656,96 @@
         if managed:
             raise ValueError(
                 "Managed creds are not supported for datasets that are not connected to activeloop platform."
             )
         self.link_creds.add_creds_key(creds_key)
         save_link_creds(self.link_creds, self.storage)
 
-    def populate_creds(self, creds_key: str, creds: dict):
+    def populate_creds(
+        self,
+        creds_key: str,
+        creds: Optional[dict] = None,
+        from_environment: bool = False,
+    ):
         """Populates the creds key added in add_creds_key with the given creds. These creds are used to fetch the external data.
         This needs to be done everytime the dataset is reloaded for datasets that contain links to external data.
 
         Examples:
 
             >>> # create/load a dataset
             >>> ds = deeplake.dataset("path/to/dataset")
             >>> # add a new creds key
             >>> ds.add_creds_key("my_s3_key")
             >>> # populate the creds
             >>> ds.populate_creds("my_s3_key", {"aws_access_key_id": "my_access_key", "aws_secret_access_key": "my_secret_key"})
+            >>> # or
+            >>> ds.populate_creds("my_s3_key", from_environment=True)
 
         """
+        if creds and from_environment:
+            raise ValueError(
+                "Only one of creds or from_environment can be provided. Both cannot be provided at the same time."
+            )
+        if from_environment:
+            creds = {}
         self.link_creds.populate_creds(creds_key, creds)
 
-    def update_creds_key(self, old_creds_key: str, new_creds_key: str):
-        """Replaces the old creds key with the new creds key. This is used to replace the creds key used for external data."""
-        replaced_index = self.link_creds.replace_creds(old_creds_key, new_creds_key)
-        save_link_creds(self.link_creds, self.storage, replaced_index=replaced_index)
-
-    def change_creds_management(self, creds_key: str, managed: bool):
-        """Changes the management status of the creds key.
+    def update_creds_key(
+        self,
+        creds_key: str,
+        new_creds_key: Optional[str] = None,
+        managed: Optional[bool] = None,
+    ):
+        """Updates the name and/or management status of a creds key.
 
         Args:
-            creds_key (str): The key whose management status is to be changed.
+            creds_key (str): The key whose name and/or management status is to be changed.
+            new_creds_key (str, optional): The new key to replace the old key. If not provided, the old key will be used.
             managed (bool): The target management status. If ``True``, the creds corresponding to the key will be fetched from activeloop platform.
 
         Raises:
             ValueError: If the dataset is not connected to activeloop platform.
+            ValueError: If both ``new_creds_key`` and ``managed`` are ``None``.
             KeyError: If the creds key is not present in the dataset.
 
         Examples:
 
             >>> # create/load a dataset
             >>> ds = deeplake.dataset("path/to/dataset")
             >>> # add a new creds key
             >>> ds.add_creds_key("my_s3_key")
             >>> # Populate the name added with creds dictionary
             >>> # These creds are only present temporarily and will have to be repopulated on every reload
             >>> ds.populate_creds("my_s3_key", {})
-            >>> # Change the management status of the key to True. Before doing this, ensure that the creds have been created on activeloop platform
+            >>> # Rename the key and change the management status of the key to True. Before doing this, ensure that the creds have been created on activeloop platform
             >>> # Now, this key will no longer use the credentials populated in the previous step but will instead fetch them from activeloop platform
             >>> # These creds don't have to be populated again on every reload and will be fetched every time the dataset is loaded
-            >>> ds.change_creds_management("my_s3_key", True)
+            >>> ds.update_creds_key("my_s3_key", "my_managed_key", True)
 
         """
-        raise ValueError(
-            "Managed creds are not supported for datasets that are not connected to activeloop platform."
-        )
+        if new_creds_key is None and managed is None:
+            raise ValueError(
+                "Atleast one of new_creds_key or managed must be provided."
+            )
+        if managed:
+            raise ValueError(
+                "Managed creds are not supported for datasets that are not connected to activeloop platform."
+            )
+        replaced_index = self.link_creds.replace_creds(creds_key, new_creds_key)
+        save_link_creds(self.link_creds, self.storage, replaced_index=replaced_index)
 
     def get_creds_keys(self) -> List[str]:
         """Returns the list of creds keys added to the dataset. These are used to fetch external data in linked tensors"""
-        return self.link_creds.creds_keys
+        return list(self.link_creds.creds_keys)
+
+    def get_managed_creds_keys(self) -> List[str]:
+        """Returns the list of creds keys added to the dataset that are managed by Activeloop platform. These are used to fetch external data in linked tensors."""
+        raise ValueError(
+            "Managed creds are not supported for datasets that are not connected to activeloop platform."
+        )
 
     def visualize(
         self, width: Union[int, str, None] = None, height: Union[int, str, None] = None
     ):
         """
         Visualizes the dataset in the Jupyter notebook.
 
@@ -3781,14 +3906,18 @@
         return (
             not self.index.is_trivial()
             or hasattr(self, "_vds")
             or hasattr(self, "_view_entry")
         )
 
     @property
+    def is_optimized(self) -> bool:
+        return not getattr(getattr(self, "_view_entry", None), "virtual", True)
+
+    @property
     def min_view(self):
         """Returns a view of the dataset in which all tensors are sliced to have the same length as
         the shortest tensor.
 
         Example:
 
             Creating a dataset with 5 images and 4 labels. ``ds.min_view`` will return a view in which tensors are
```

### Comparing `deeplake-3.2.9/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.3.0/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import posixpath
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 from deeplake.client.utils import get_user_name
 from deeplake.constants import HUB_CLOUD_DEV_USERNAME
 from deeplake.core.dataset import Dataset
 from deeplake.client.client import DeepLakeBackendClient
 from deeplake.util.bugout_reporter import deeplake_reporter
 from deeplake.util.exceptions import (
     InvalidSourcePathError,
@@ -276,60 +276,83 @@
                 Note, this is only applicable for datasets that are connected to activeloop platform.
                 Defaults to ``False``.
         """
         self.link_creds.add_creds_key(creds_key, managed=managed)
         save_link_creds(self.link_creds, self.storage)
         self.link_creds.warn_missing_managed_creds()
 
-    def update_creds_key(self, old_creds_key: str, new_creds_key: str):
-        """Replaces the old creds key with the new creds key. This is used to replace the creds key used for external data."""
-        if old_creds_key in self.link_creds.managed_creds_keys:
-            raise ValueError(
-                f"""Cannot update managed creds key directly. If you want to update it, follow these steps:-
-                1. ds.change_creds_management("{old_creds_key}", False)
-                2. ds.update_creds_key("{old_creds_key}", "{new_creds_key}")
-                3. [OPTIONAL] ds.change_creds_management("{new_creds_key}", True)
-                """
-            )
-        super().update_creds_key(old_creds_key, new_creds_key)
-        self.link_creds.warn_missing_managed_creds()
-
-    def change_creds_management(self, creds_key: str, managed: bool):
-        """Changes the management status of the creds key.
+    def update_creds_key(
+        self,
+        creds_key: str,
+        new_creds_key: Optional[str] = None,
+        managed: Optional[bool] = None,
+    ):
+        """Updates the name and/or management status of a creds key.
 
         Args:
             creds_key (str): The key whose management status is to be changed.
+            new_creds_key (str, optional): The new key to replace the old key. If not provided, the old key will be used.
             managed (bool): The target management status. If ``True``, the creds corresponding to the key will be fetched from activeloop platform.
 
         Raises:
             ValueError: If the dataset is not connected to activeloop platform.
+            ValueError: If both ``new_creds_key`` and ``managed`` are ``None``.
             KeyError: If the creds key is not present in the dataset.
+            Exception: All other errors such as during population of managed creds.
 
         Examples:
 
             >>> # create/load a dataset
-            >>> ds = deeplake.dataset("hub://username/dataset")
+            >>> ds = deeplake.dataset("path/to/dataset")
             >>> # add a new creds key
             >>> ds.add_creds_key("my_s3_key")
             >>> # Populate the name added with creds dictionary
             >>> # These creds are only present temporarily and will have to be repopulated on every reload
             >>> ds.populate_creds("my_s3_key", {})
-            >>> # Change the management status of the key to True. Before doing this, ensure that the creds have been created on activeloop platform
+            >>> # Rename the key and change the management status of the key to True. Before doing this, ensure that the creds have been created on activeloop platform
             >>> # Now, this key will no longer use the credentials populated in the previous step but will instead fetch them from activeloop platform
             >>> # These creds don't have to be populated again on every reload and will be fetched every time the dataset is loaded
-            >>> ds.change_creds_management("my_s3_key", True)
-
+            >>> ds.update_creds_key("my_s3_key", "my_managed_key", True)
         """
-
-        key_index = self.link_creds.creds_mapping[creds_key] - 1
-        changed = self.link_creds.change_creds_management(creds_key, managed)
-        if changed:
-            save_link_creds(
-                self.link_creds, self.storage, managed_info=(managed, key_index)
+        if new_creds_key is None and managed is None:
+            raise ValueError(
+                "Atleast one of new_creds_key or managed must be provided."
             )
+        key_index = self.link_creds.creds_mapping[creds_key] - 1
+        managed_info, replaced_index = None, None
+        original_creds_key = creds_key
+        original_key_is_managed = (
+            original_creds_key in self.link_creds.managed_creds_keys
+        )
+
+        if new_creds_key is not None and new_creds_key != creds_key:
+            replaced_index = self.link_creds.replace_creds(creds_key, new_creds_key)
+            creds_key = new_creds_key
+
+        try:
+            if managed is not None:
+                management_changed = self.link_creds.change_creds_management(
+                    creds_key, managed
+                )
+                if management_changed:
+                    managed_info = (managed, key_index)
+            if original_key_is_managed and managed is not False:
+                self.link_creds.populate_single_managed_creds(creds_key)
+        except Exception:
+            if replaced_index is not None:
+                # revert the change
+                self.link_creds.replace_creds(new_creds_key, original_creds_key)
+            raise
+        save_link_creds(
+            self.link_creds,
+            self.storage,
+            replaced_index=replaced_index,
+            managed_info=managed_info,
+        )
+        self.link_creds.warn_missing_managed_creds()
 
     def _load_link_creds(self):
         """Loads the link creds from the storage."""
         super()._load_link_creds()
         if self.link_creds.client is None:
             self._set_org_and_name()
             self.link_creds.org_id = self.org_id
@@ -356,7 +379,11 @@
 
         return _TmpWriteAccess()
 
     def connect(self, *args, **kwargs):
         raise InvalidSourcePathError(
             f"The dataset being connected is already accessible via Deep Lake path {self.path}"
         )
+
+    def get_managed_creds_keys(self) -> List[str]:
+        """Returns the list of creds keys added to the dataset that are managed by Activeloop platform. These are used to fetch external data in linked tensors."""
+        return list(self.link_creds.managed_creds_keys)
```

### Comparing `deeplake-3.2.9/deeplake/core/dataset/invalid_view.py` & `deeplake-3.3.0/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/dataset/view_entry.py` & `deeplake-3.3.0/deeplake/core/dataset/view_entry.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,20 +25,28 @@
         return self.info["id"].split("]")[-1]
 
     @property
     def query(self) -> Optional[str]:
         return self.info.get("query")
 
     @property
+    def tql_query(self) -> Optional[str]:
+        return self.info.get("tql_query")
+
+    @property
     def message(self) -> str:
         """Returns the message with which the view was saved."""
         return self.info.get("message", "")
 
+    @property
+    def commit_id(self) -> str:
+        return self.info["source-dataset-version"]
+
     def __str__(self):
-        return f"View(id='{self.id}', message='{self.message}', virtual={self.virtual})"
+        return f"View(id='{self.id}', message='{self.message}', virtual={self.virtual}, commit_id={self.commit_id}, query='{self.query}, tql_query='{self.tql_query}')"
 
     __repr__ = __str__
 
     @property
     def virtual(self) -> bool:
         return self.info["virtual-datasource"]
 
@@ -47,23 +55,33 @@
 
         Args:
             verbose (bool): If ``True``, logs will be printed. Defaults to ``True``.
 
         Returns:
             Dataset: Loaded dataset view.
         """
+        if self.commit_id != self._ds.commit_id:
+            print(f"Loading view from commit id {self.commit_id}.")
+
         ds = self._ds._sub_ds(
             ".queries/" + (self.info.get("path") or self.info["id"]),
             lock=False,
             verbose=False,
             token=self._src_ds.token,
+            read_only=True,
         )
+
         sub_ds_path = ds.path
         if self.virtual:
             ds = ds._get_view(inherit_creds=not self._external)
+
+        if not self.tql_query is None:
+            query_str = self.tql_query
+            ds = ds.query(query_str)
+
         ds._view_entry = self
         if verbose:
             log_visualizer_link(sub_ds_path, source_ds_url=self.info["source-dataset"])
         return ds
 
     def optimize(
         self,
@@ -93,15 +111,21 @@
             num_workers (int): Number of workers to be used for the optimization process. Defaults to 0.
             scheduler (str): The scheduler to be used for optimization. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
                 Only applicable if ``optimize=True``. Defaults to 'threaded'.
             progressbar (bool): Whether to display a progressbar.
 
         Returns:
             :class:`ViewEntry`
+
+        Raises:
+            Exception: When query view cannot be optimized.
+
         """
+        if not self.tql_query is None:
+            raise Exception("Optimizing nonlinear query views is not supported")
         self.info = self._ds._optimize_saved_view(
             self.info["id"],
             tensors=tensors,
             external=self._external,
             unlink=unlink,
             num_workers=num_workers,
             scheduler=scheduler,
```

### Comparing `deeplake-3.2.9/deeplake/core/fast_forwarding.py` & `deeplake-3.3.0/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/index/index.py` & `deeplake-3.3.0/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/io.py` & `deeplake-3.3.0/deeplake/core/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,15 @@
     LRUCache,
     MemoryProvider,
     StorageProvider,
     LocalProvider,
 )
 from deeplake.core.tiling.deserialize import combine_chunks
 from deeplake.integrations.pytorch.common import check_tensors, validate_decode_method
-from deeplake.util.exceptions import (
-    DatasetUnsupportedPytorch,
-    SampleDecompressionError,
-)
+from deeplake.util.exceptions import DatasetUnsupportedPytorch, ReadSampleFromChunkError
 from deeplake.util.keys import get_chunk_key, get_tensor_meta_key
 from deeplake.util.remove_cache import get_base_storage
 from deeplake.util.storage import get_pytorch_local_storage
 from PIL import Image  # type: ignore
 
 
 ChunkEngineMap = Dict[str, ChunkEngine]
@@ -121,27 +118,31 @@
             thread1: [2, 6]
             thread2: [3]
             thread3: [4]
 
         So that initial order would be reconstructed by the DataLoader
     """
 
-    def __init__(self, num_workers: int) -> None:
+    def __init__(self, num_workers: int, batch_size: int = 1) -> None:
         super().__init__()
         self.num_workers = num_workers
+        self.batch_size = batch_size
 
     def schedule(self, jobs: List[IOBlock]) -> List[Schedule]:
         per_worker: List[List[IOBlock]] = [list() for _ in range(self.num_workers)]
         assigned_worker = iter(cycle(range(self.num_workers)))
 
+        index_count = 0
         for job in jobs:
             split: List[List[int]] = [list() for _ in range(self.num_workers)]
-
-            for ind in job.indices():
-                split[next(assigned_worker)].append(ind)
+            for i, index in enumerate(job.indices()):
+                if index_count % self.batch_size == 0:
+                    worker = next(assigned_worker)
+                split[worker].append(index)
+                index_count += 1
 
             for worker_id, idx_list in enumerate(split):
                 if len(idx_list) > 0:
                     worker_block = IOBlock(job.chunks(), idx_list)
                     per_worker[worker_id].append(worker_block)
 
         return [Schedule(worker_jobs) for worker_jobs in per_worker]
@@ -259,15 +260,14 @@
 
 class SampleStreaming(Streaming):
     def __init__(
         self,
         dataset,
         tensors: Sequence[str],
         use_local_cache: bool = False,
-        return_index: bool = True,
         pad_tensors: bool = False,
         decode_method: Optional[Dict[str, str]] = None,
         tobytes: Union[bool, Sequence[str]] = False,
     ) -> None:
         super().__init__()
 
         self.dataset = dataset
@@ -281,22 +281,32 @@
             raise DatasetUnsupportedPytorch(
                 "The underlying storage is MemoryProvider which isn't supported."
             )
 
         self.tensors = tensors
         self.pad_tensors = pad_tensors
         self.decode_method = decode_method
-        self.return_index = return_index
 
-        jpeg_png_compressed_tensors = check_tensors(self.dataset, tensors)
-        raw_tensors, compressed_tensors = validate_decode_method(
-            self.decode_method, tensors, jpeg_png_compressed_tensors
+        jpeg_png_compressed_tensors, json_tensors, list_tensors = check_tensors(
+            self.dataset, tensors
+        )
+        (
+            raw_tensors,
+            pil_compressed_tensors,
+            json_tensors,
+            list_tensors,
+        ) = validate_decode_method(
+            self.decode_method,
+            tensors,
+            jpeg_png_compressed_tensors,
+            json_tensors,
+            list_tensors,
         )
         self.raw_tensors = set(raw_tensors)
-        self.compressed_tensors = set(compressed_tensors)
+        self.pil_compressed_tensors = set(pil_compressed_tensors)
 
         self.chunk_engines: ChunkEngineMap = self._map_chunk_engines(self.tensors)
 
         self.local_caches: Optional[CachesMap] = (
             ({tensor: self._use_cache(self.local_storage) for tensor in self.tensors})
             if self.local_storage is not None
             else None
@@ -314,15 +324,15 @@
         for idx in block.indices():
             sample = dict()
             valid_sample_flag = True
 
             for keyid, (key, engine) in enumerate(self.chunk_engines.items()):
                 rel_key = key[self._group_index_length :]
                 decompress = key not in self.raw_tensors
-                to_pil = key in self.compressed_tensors
+                to_pil = key in self.pil_compressed_tensors
                 chunk_class = engine.chunk_class
                 try:
                     chunks: List[BaseChunk] = []
                     c_names = block.chunk_names(keyid)
                     if c_names == [None]:
                         sample[rel_key] = engine.get_empty_sample()
                         continue
@@ -361,24 +371,23 @@
                             data = Image.fromarray(data)  # type: ignore
 
                     if data is not None:
                         sample[rel_key] = data
                     else:
                         valid_sample_flag = False
                         break
-                except SampleDecompressionError:
+                except ReadSampleFromChunkError:
                     warn(
                         f"Skipping corrupt {engine.tensor_meta.sample_compression} sample at dataset.{key}[{idx}]"
                     )
                     valid_sample_flag = False
                     break
 
             if valid_sample_flag:
-                if self.return_index:
-                    sample["index"] = np.array([idx])
+                sample["index"] = np.array([idx])
                 yield sample
 
     def _get_block_for_single_sample(self, idx):
         chunks = []
         for engine in self.chunk_engines.values():
             enc = engine.chunk_id_encoder
             try:
```

### Comparing `deeplake-3.2.9/deeplake/core/ipc.py` & `deeplake-3.3.0/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/link_creds.py` & `deeplake-3.3.0/deeplake/core/link_creds.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import json
 from typing import Optional
 import warnings
 from deeplake.constants import ALL_CLOUD_PREFIXES
 from deeplake.core.storage.deeplake_memory_object import DeepLakeMemoryObject
-from deeplake.core.storage.provider import StorageProvider
+from deeplake.core.storage import StorageProvider, storage_factory
 from deeplake.core.storage.s3 import S3Provider
+from deeplake.util.exceptions import (
+    ManagedCredentialsNotFoundError,
+    MissingCredsError,
+    MissingManagedCredsError,
+)
 from deeplake.util.token import expires_in_to_expires_at, is_expired_token
 from deeplake.client.log import logger
 
 
 class LinkCreds(DeepLakeMemoryObject):
     def __init__(self):
         self.creds_keys = []
@@ -19,22 +24,27 @@
         self.storage_providers = {}
         self.default_s3_provider = None
         self.default_gcs_provider = None
         self.client = None
         self.org_id = None
 
     def get_creds(self, key: Optional[str]):
-        if key in {"ENV", None}:
+        if key is None:
             return {}
         if key not in self.creds_keys:
-            raise KeyError(f"Creds key {key} does not exist")
+            raise MissingCredsError(f"Creds key {key} does not exist")
         if key not in self.creds_dict:
-            raise ValueError(
-                f"Creds key {key} hasn't been populated. Populate it using ds.populate_creds()"
-            )
+            if key not in self.managed_creds_keys:
+                raise MissingCredsError(
+                    f"Creds key {key} hasn't been populated. Populate it using ds.populate_creds()"
+                )
+            else:
+                raise MissingManagedCredsError(
+                    f"Managed creds key {key} hasn't been fetched."
+                )
         if (
             self.client is not None
             and key in self.managed_creds_keys
             and is_expired_token(self.creds_dict[key])
         ):
             self.refresh_managed_creds(key)  # type: ignore
         return self.creds_dict[key]
@@ -45,47 +55,51 @@
         creds = self.fetch_managed_creds(creds_key)
         self.populate_creds(creds_key, creds)
         return True
 
     def get_default_provider(self, provider_type: str):
         if provider_type == "s3":
             if self.default_s3_provider is None:
-                self.default_s3_provider = S3Provider("s3://bucket/path")
+                self.default_s3_provider = storage_factory(
+                    S3Provider, "s3://bucket/path"
+                )
             return self.default_s3_provider
         else:
             if self.default_gcs_provider is None:
                 from deeplake.core.storage.gcs import GCSProvider
 
-                self.default_gcs_provider = GCSProvider("gcs://bucket/path")
+                self.default_gcs_provider = storage_factory(
+                    GCSProvider, "gcs://bucket/path"
+                )
             return self.default_gcs_provider
 
     def get_storage_provider(self, key: Optional[str], provider_type: str):
         assert provider_type in {"s3", "gcs"}
-        if key in {"ENV", None}:
+        if key is None:
             return self.get_default_provider(provider_type)
 
         provider: StorageProvider
         creds = self.get_creds(key)
 
         if provider_type == "s3":
             if key in self.storage_providers:
                 provider = self.storage_providers[key]
                 if isinstance(provider, S3Provider):
                     return provider
 
-            provider = S3Provider("s3://bucket/path", **creds)
+            provider = storage_factory(S3Provider, "s3://bucket/path", **creds)
         else:
             from deeplake.core.storage.gcs import GCSProvider
 
             if key in self.storage_providers:
                 provider = self.storage_providers[key]
                 if isinstance(provider, GCSProvider):
                     return provider
 
-            provider = GCSProvider("gcs://bucket/path", **creds)
+            provider = storage_factory(GCSProvider, "gcs://bucket/path", **creds)
         self.storage_providers[key] = provider
         return provider
 
     def add_creds_key(self, creds_key: str, managed: bool = False):
         if creds_key in self.creds_keys:
             raise ValueError(f"Creds key {creds_key} already exists")
         if managed:
@@ -126,15 +140,15 @@
                 old_creds_key
             ]
             del self.storage_providers[old_creds_key]
         return replaced_index
 
     def populate_creds(self, creds_key: str, creds):
         if creds_key not in self.creds_keys:
-            raise KeyError(f"Creds key {creds_key} does not exist")
+            raise MissingCredsError(f"Creds key {creds_key} does not exist")
         expires_in_to_expires_at(creds)
         self.creds_dict[creds_key] = creds
         self.storage_providers.pop(creds_key, None)
 
     def add_to_used_creds(self, creds_key: Optional[str]):
         if creds_key is None or creds_key in self.used_creds_keys:
             return False
@@ -154,27 +168,28 @@
         obj = cls()
         if buffer:
             d = json.loads(buffer.decode("utf-8"))
             obj.creds_keys = list(d["creds_keys"])
             obj.creds_mapping = {k: i + 1 for i, k in enumerate(obj.creds_keys)}
             obj.managed_creds_keys = set(d["managed_creds_keys"])
             obj.used_creds_keys = set(d["used_creds_keys"])
+            if "ENV" in obj.used_creds_keys and "ENV" not in obj.creds_keys:
+                obj.creds_keys = ["ENV"] + obj.creds_keys
+                obj.creds_mapping["ENV"] = 0
         obj.is_dirty = False
         return obj
 
     def get_encoding(self, key: Optional[str] = None, path: Optional[str] = None):
-        if key == "ENV":
-            return 0
         if key is None:
             if path and path.startswith(ALL_CLOUD_PREFIXES):
                 raise ValueError("Creds key must always be specified for cloud storage")
             return 0
 
         if key not in self.creds_keys:
-            raise ValueError(f"Creds key {key} does not exist")
+            raise MissingCredsError(f"Creds key {key} does not exist")
         return self.creds_mapping[key]
 
     def get_creds_key(self, encoding):
         if encoding > len(self.creds_keys):
             raise KeyError(f"Encoding {encoding} not found.")
         return None if encoding == 0 else self.creds_keys[encoding - 1]
 
@@ -209,16 +224,28 @@
     def missing_keys(self) -> list:
         return [key for key in self.creds_keys if key not in self.creds_dict]
 
     def populate_all_managed_creds(self, verbose: bool = True):
         assert self.client is not None
         assert self.org_id is not None
         for creds_key in self.managed_creds_keys:
-            creds = self.fetch_managed_creds(creds_key, verbose=verbose)
-            self.populate_creds(creds_key, creds)
+            try:
+                self.populate_single_managed_creds(creds_key, verbose=verbose)
+            except ManagedCredentialsNotFoundError:
+                logger.warning(
+                    f"Credentials '{creds_key}' not found in Activeloop platform. "
+                    f"Please make sure the credentials are added to the platform and reload the dataset. "
+                    f"Alternatively, use ds.update_creds_key(key_name, managed=False) to disable the managed credentials.)"
+                )
+
+    def populate_single_managed_creds(self, creds_key: str, verbose: bool = True):
+        assert self.client is not None
+        assert self.org_id is not None
+        creds = self.fetch_managed_creds(creds_key, verbose=verbose)
+        self.populate_creds(creds_key, creds)
 
     def fetch_managed_creds(self, creds_key: str, verbose: bool = True):
         creds = self.client.get_managed_creds(self.org_id, creds_key)
         if verbose:
             logger.info(f"Loaded credentials '{creds_key}' from Activeloop platform.")
         return creds
 
@@ -230,15 +257,16 @@
             return False
         if managed:
             creds = self.fetch_managed_creds(creds_key)
             self.managed_creds_keys.add(creds_key)
             self.populate_creds(creds_key, creds)
         else:
             self.managed_creds_keys.discard(creds_key)
-
+            self.creds_dict.pop(creds_key, None)
+            self.storage_providers.pop(creds_key, None)
         return True
 
     def warn_missing_managed_creds(self):
         """Warns about any missing managed creds that were added in parallel by someone else."""
         missing_creds = self.missing_keys
 
         missing_managed_creds = [
```

### Comparing `deeplake-3.2.9/deeplake/core/linked_chunk_engine.py` & `deeplake-3.3.0/deeplake/core/linked_chunk_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     coalesce_tiles,
     np_list_to_sample,
     translate_slices,
 )
 from deeplake.core.linked_sample import read_linked_sample
 from deeplake.util.exceptions import (
     BadLinkError,
+    GetDataFromLinkError,
     ReadOnlyModeError,
-    UnableToReadFromUrlError,
 )
 from deeplake.util.keys import get_creds_encoder_key
 from deeplake.util.link import get_path_creds_key, save_link_creds
 from deeplake.util.video import normalize_index
 import numpy as np
 from typing import Optional, Dict, Any, Tuple, Union
 from PIL import Image  # type: ignore
@@ -92,17 +92,15 @@
     @property
     def is_data_cachable(self):
         return False
 
     def linked_sample(
         self, global_sample_index: int
     ) -> Union[LinkedSample, LinkedTiledSample]:
-        creds_encoder = self.creds_encoder
-        sample_creds_encoded = creds_encoder.get_encoded_creds_key(global_sample_index)
-        sample_creds_key = self.link_creds.get_creds_key(sample_creds_encoded)  # type: ignore
+        sample_creds_key = self.creds_key(global_sample_index)
         if self._is_tiled_sample(global_sample_index):
             path_array: np.ndarray = (
                 super()
                 .get_basic_sample(
                     global_sample_index,
                     Index(global_sample_index),
                     fetch_chunks=True,
@@ -110,46 +108,53 @@
                 )
                 .path_array
             )
             return LinkedTiledSample(path_array, sample_creds_key)
         sample_path = self.get_path(global_sample_index, fetch_chunks=True)
         return LinkedSample(sample_path, sample_creds_key)
 
+    def creds_key(self, global_sample_index: int):
+        sample_creds_encoded = self.creds_encoder.get_encoded_creds_key(
+            global_sample_index
+        )
+        return self.link_creds.get_creds_key(sample_creds_encoded)  # type: ignore
+
     def get_video_url(self, global_sample_index):
-        creds_encoder = self.creds_encoder
         sample_path = self.get_path(global_sample_index)
-        sample_creds_encoded = creds_encoder.get_encoded_creds_key(global_sample_index)
-        sample_creds_key = self.link_creds.get_creds_key(sample_creds_encoded)
+        sample_creds_key = self.creds_key(global_sample_index)
         storage = None
         if sample_path.startswith(("gcs://", "gcp://", "s3://")):
             provider_type = "s3" if sample_path.startswith("s3://") else "gcs"
             storage = self.link_creds.get_storage_provider(
                 sample_creds_key, provider_type
             )
             url = storage.get_presigned_url(sample_path, full=True)
         else:
             url = sample_path
-        return url
+        return url, sample_path
 
     def get_video_sample(self, global_sample_index, index):
-        url = self.get_video_url(global_sample_index)
-        squeeze = isinstance(index, int)
-        shape = _read_video_shape(url)
-        sub_index = index.values[1].value if len(index.values) > 1 else None  # type: ignore
-        start, stop, step, reverse = normalize_index(sub_index, shape[0])
-        video_sample = _decompress_video(
-            url,
-            start,
-            stop,
-            step,
-            reverse,
-        )
-        if squeeze:
-            video_sample.squeeze(0)
-        return video_sample
+        url, path = self.get_video_url(global_sample_index)
+        try:
+            squeeze = isinstance(index, int)
+            shape = _read_video_shape(url)
+            sub_index = index.values[1].value if len(index.values) > 1 else None  # type: ignore
+            start, stop, step, reverse = normalize_index(sub_index, shape[0])
+            video_sample = _decompress_video(
+                url,
+                start,
+                stop,
+                step,
+                reverse,
+            )
+            if squeeze:
+                video_sample.squeeze(0)
+            return video_sample
+        except Exception as e:
+            raise GetDataFromLinkError(path)
 
     def get_full_tiled_sample(self, global_sample_index, fetch_chunks=False):
         tile_enc = self.tile_encoder
         shape = tile_enc.get_sample_shape(global_sample_index)
         tile_shape = tile_enc.get_tile_shape(global_sample_index)
         layout_shape = tile_enc.get_tile_layout_shape(global_sample_index)
         path_array: np.ndarray = (
@@ -159,18 +164,15 @@
                 Index(global_sample_index),
                 fetch_chunks,
                 is_tile=True,
             )
             .path_array
         )
 
-        sample_creds_encoded = self.creds_encoder.get_encoded_creds_key(
-            global_sample_index
-        )
-        sample_creds_key = self.link_creds.get_creds_key(sample_creds_encoded)
+        sample_creds_key = self.creds_key(global_sample_index)
         tiled_arrays = [
             read_linked_sample(path, sample_creds_key, self.link_creds, False).array
             for path in iter(path_array.flat)
         ]
         return np_list_to_sample(tiled_arrays, shape, tile_shape, layout_shape)
 
     def get_partial_tiled_sample(self, global_sample_index, index, fetch_chunks=False):
@@ -188,18 +190,15 @@
             .path_array
         )
         tiles_index, sample_index = translate_slices(
             [v.value for v in index.values[1:]], sample_shape, tile_shape  # type: ignore
         )
         required_tile_paths = ordered_tile_paths[tiles_index]
 
-        sample_creds_encoded = self.creds_encoder.get_encoded_creds_key(
-            global_sample_index
-        )
-        sample_creds_key = self.link_creds.get_creds_key(sample_creds_encoded)
+        sample_creds_key = self.creds_key(global_sample_index)
 
         tiles = np.vectorize(
             lambda path: read_linked_sample(
                 path, sample_creds_key, self.link_creds, False
             ).array,
             otypes=[object],
         )(required_tile_paths)
@@ -207,28 +206,31 @@
         sample = sample[sample_index]
         return sample
 
     def get_basic_sample(self, global_sample_index, index, fetch_chunks=False):
         sample = self.get_deeplake_read_sample(global_sample_index, fetch_chunks)
         if sample is None:
             return np.ones((0,))
-        return sample.array[tuple(entry.value for entry in index.values[1:])]
+        arr = sample.array
+        max_shape = self.tensor_meta.max_shape
+        if len(arr.shape) == 2 and max_shape and len(max_shape) == 3:
+            arr = arr.reshape(arr.shape + (1,))
+        return arr[tuple(entry.value for entry in index.values[1:])]
 
     def get_path(self, global_sample_index, fetch_chunks=False) -> str:
         return super().get_basic_sample(
             global_sample_index, Index(global_sample_index), fetch_chunks
         )[0]
 
     def get_deeplake_read_sample(self, global_sample_index, fetch_chunks=False):
         creds_encoder = self.creds_encoder
         sample_path = self.get_path(global_sample_index, fetch_chunks)
         if not sample_path:
             return None
-        sample_creds_encoded = creds_encoder.get_encoded_creds_key(global_sample_index)
-        sample_creds_key = self.link_creds.get_creds_key(sample_creds_encoded)
+        sample_creds_key = self.creds_key(global_sample_index)
         return read_linked_sample(sample_path, sample_creds_key, self.link_creds, False)
 
     @property
     def verify(self):
         return self.tensor_meta.is_link and self.tensor_meta.verify
 
     def check_each_sample(self, samples, verify=True):
@@ -257,20 +259,21 @@
             elif isinstance(sample, LinkedTiledSample):
                 verify_samples = self.verify and verify
                 sample.set_check_tile_shape(self.link_creds, verify_samples)
                 sample.set_sample_shape()
                 verified_samples.append(sample)
             else:
                 try:
+                    _verify = verify and self.verify
                     verified_samples.append(
                         read_linked_sample(
                             sample.path,
                             sample.creds_key,
                             self.link_creds,
-                            verify=verify and self.verify,
+                            verify=_verify,
                         )
                     )
                 except Exception as e:
                     raise BadLinkError(sample.path, sample.creds_key) from e
         return verified_samples
 
     def register_new_creds(self, num_samples_added, samples):
@@ -318,19 +321,17 @@
     ) -> Union[np.ndarray, Image.Image]:
         enc = self.chunk_id_encoder
         local_sample_index = enc.translate_index_relative_to_chunks(global_sample_index)
         sample_path = chunk.read_sample(
             local_sample_index, cast=cast, copy=copy, decompress=decompress
         )[0]
 
-        creds_encoder = self.creds_encoder
         if not sample_path:
             return self.get_empty_sample()
-        sample_creds_encoded = creds_encoder.get_encoded_creds_key(global_sample_index)
-        sample_creds_key = self.link_creds.get_creds_key(sample_creds_encoded)  # type: ignore
+        sample_creds_key = self.creds_key(global_sample_index)
         read_sample = read_linked_sample(
             sample_path, sample_creds_key, self.link_creds, False
         )
         if to_pil:
             return read_sample.pil
         return read_sample.array
```

### Comparing `deeplake-3.2.9/deeplake/core/linked_sample.py` & `deeplake-3.3.0/deeplake/core/linked_sample.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 from typing import Optional
+from deeplake.util.exceptions import GetDataFromLinkError
+from deeplake.util.exceptions import MissingCredsError
 from deeplake.util.path import get_path_type
 import deeplake
 import numpy as np
 
-from deeplake.util.creds import convert_creds_key
-
 
 class LinkedSample:
     """Represents a sample that is initialized using external links. See :meth:`deeplake.link`."""
 
     def __init__(self, path: str, creds_key: Optional[str] = None):
         self.path = path
-        self.creds_key = convert_creds_key(creds_key, path)
+        self.creds_key = creds_key
 
     @property
     def dtype(self) -> str:
         return np.array("").dtype.str
 
 
 def read_linked_sample(
-    sample_path: str, sample_creds_key: str, link_creds, verify: bool
+    sample_path: str, sample_creds_key: Optional[str], link_creds, verify: bool
 ):
     provider_type = get_path_type(sample_path)
-    if provider_type == "local":
-        return deeplake.read(sample_path, verify=verify)
-    elif provider_type == "http":
-        return _read_http_linked_sample(
-            link_creds, sample_creds_key, sample_path, verify
-        )
-    else:
-        return _read_cloud_linked_sample(
-            link_creds, sample_creds_key, sample_path, provider_type, verify
-        )
+    try:
+        if provider_type == "local":
+            return deeplake.read(sample_path, verify=verify)
+        elif provider_type == "http":
+            return _read_http_linked_sample(
+                link_creds, sample_creds_key, sample_path, verify
+            )
+        else:
+            return _read_cloud_linked_sample(
+                link_creds, sample_creds_key, sample_path, provider_type, verify
+            )
+    except Exception as e:
+        raise GetDataFromLinkError(sample_path) from e
 
 
 def retry_refresh_managed_creds(f):
     def wrapper(linked_creds, sample_creds_key, *args, **kwargs):
         try:
             return f(linked_creds, sample_creds_key, *args, **kwargs)
+        except MissingCredsError:
+            raise
         except Exception as e:
-            linked_creds.populate_all_managed_creds()
-            return f(linked_creds, sample_creds_key, *args, **kwargs)
+            if linked_creds.client is not None:
+                linked_creds.populate_all_managed_creds()
+                return f(linked_creds, sample_creds_key, *args, **kwargs)
+            raise e
 
     return wrapper
 
 
 @retry_refresh_managed_creds
 def _read_cloud_linked_sample(
     link_creds,
```

### Comparing `deeplake-3.2.9/deeplake/core/linked_tiled_sample.py` & `deeplake-3.3.0/deeplake/core/linked_tiled_sample.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Optional
 import numpy as np
 from deeplake.core.tensor_link import read_linked_sample
-from deeplake.util.creds import convert_creds_key
 from deeplake.util.path import get_path_type
 
 
 class LinkedTiledSample:
     """Represents a sample that is initialized using external links. See :meth:`deeplake.link_tiled`."""
 
     def __init__(
@@ -15,15 +14,15 @@
     ):
         self.path_array = path_array
         self._path = None
         # check that all paths in the array are of the same type
         path_types = {get_path_type(path) for path in path_array.flat}
         if len(path_types) > 1:
             raise ValueError("Path array contains paths in different locations.")
-        self.creds_key = convert_creds_key(creds_key, self.path)
+        self.creds_key = creds_key
         self._tile_shape = None
         self._shape = None
 
     @property
     def path(self):
         if self._path is None:
             self._path = next(iter(self.path_array.flat))
```

### Comparing `deeplake-3.2.9/deeplake/core/lock.py` & `deeplake-3.3.0/deeplake/core/lock.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import deeplake
 import time
 import uuid
 import struct
 import atexit
 import threading
-from os import urandom
+from os import urandom, getpid
 from typing import Tuple, Dict, Callable, Optional, Set
 from collections import defaultdict
 from deeplake.util.exceptions import LockedException
 from deeplake.util.keys import get_dataset_lock_key
 from deeplake.util.remove_cache import get_base_storage
 from deeplake.util.path import get_path_from_storage
 from deeplake.util.threading import terminate_thread
 from deeplake.core.storage import StorageProvider, LocalProvider, MemoryProvider
 from deeplake.constants import FIRST_COMMIT_ID
 from deeplake.client.utils import get_user_name
 
 
-def _get_lock_bytes(tag: Optional[bytes] = None) -> bytes:
-    byts = uuid.getnode().to_bytes(6, "little") + struct.pack("d", time.time())
+def _get_lock_bytes(tag: Optional[bytes] = None, duration: int = 10) -> bytes:
+    byts = uuid.getnode().to_bytes(6, "little") + struct.pack(
+        "d", time.time() + duration
+    )
     if tag:
         byts += tag
     return byts
 
 
 def _parse_lock_bytes(byts) -> Tuple[int, int, bytes]:
     assert len(byts) >= 14, len(byts)
@@ -30,79 +32,102 @@
     nodeid = int.from_bytes(byts[:6], "little")
     timestamp = struct.unpack("d", byts[6:14])[0]
     tag = byts[14:]
     return nodeid, timestamp, tag
 
 
 class Lock(object):
-    def __init__(self, storage: StorageProvider, path: str):
+    def __init__(self, storage: StorageProvider, path: str, duration: int = 10):
         self.storage = storage
         self._lock_verify_interval = (
-            0.1
+            0.01
             if isinstance(storage, (LocalProvider, MemoryProvider))
             else deeplake.constants.LOCK_VERIFY_INTERVAL
         )
         self.path = path
         username = get_user_name()
         if username == "public":
             self.username = None
         else:
             self.username = username
-        self.tag = urandom(4)
+        self.tag = int.to_bytes(getpid(), 4, "little")
+        self.duration = duration
+        self._min_sleep = (
+            0.01 if isinstance(storage, (LocalProvider, MemoryProvider)) else 1
+        )
+        self.acquired = False
 
     def _write_lock(self):
         storage = self.storage
         try:
             read_only = storage.read_only
             storage.disable_readonly()
-            storage[self.path] = _get_lock_bytes(self.tag)
+            storage[self.path] = _get_lock_bytes(self.tag, self.duration)
         finally:
             if read_only:
                 storage.enable_readonly()
 
-    def acquire(self, timeout=10, force=False):
+    def refresh_lock(self):
+        storage = self.storage
+        path = self.path
+        byts = storage.get(path)
+        if not byts:
+            raise LockedException()
+        nodeid, timestamp, tag = _parse_lock_bytes(byts)
+        if tag != self.tag or nodeid != uuid.getnode():
+            raise LockedException()
+        self._write_lock()
+
+    def acquire(self, timeout: Optional[int] = None):
         storage = self.storage
         path = self.path
+        if timeout is not None:
+            start_time = time.time()
         while True:
             try:
-                byts = storage[path]
-                if not byts:
-                    raise KeyError(path)
-                nodeid, timestamp, _ = _parse_lock_bytes(byts)
-                locked = True
-            except KeyError:
-                locked = False
-            if not locked:
-                self._write_lock()
-                time.sleep(self._lock_verify_interval)
-                byts = storage[path]
-                if not byts:
-                    continue
-                nodeid, _, tag = _parse_lock_bytes(byts)
-                if self.tag == tag and nodeid == uuid.getnode():
+                byts = storage.get(path)
+            except Exception:
+                byts = None
+            if byts:
+                nodeid, timestamp, tag = _parse_lock_bytes(byts)
+                locked = tag != self.tag or nodeid != uuid.getnode()
+                if not locked:  # Identical lock
                     return
-                else:
+            else:
+                locked = False
+
+            if locked:
+                rem = timestamp - time.time()
+                if rem > 0:
+                    if timeout is not None and time.time() - start_time > timeout:
+                        raise LockedException()
+                    time.sleep(min(rem, self._min_sleep))
                     continue
-            if time.time() - timestamp >= timeout:
-                if force:
-                    self._write_lock()
-                    time.sleep(self._lock_verify_interval)
-                    byts = storage[path]
-                    if not byts:
-                        continue
-                    nodeid, _, tag = _parse_lock_bytes(byts)
-                    if self.tag == tag and nodeid == uuid.getnode():
-                        return
-                    else:
-                        continue
-                else:
-                    raise LockedException()
-            time.sleep(0.5)
+
+            self._write_lock()
+            time.sleep(self._lock_verify_interval)
+            try:
+                byts = storage.get(path)
+            except Exception:
+                byts = None
+            if not byts:
+                continue
+            nodeid, timestamp, tag = _parse_lock_bytes(byts)
+            if self.tag == tag and nodeid == uuid.getnode():
+                self.acquired = True
+                return
+            else:
+                rem = timestamp - time.time()
+                if rem > 0:
+                    time.sleep(min(rem, self._min_sleep))
+                continue
 
     def release(self):
+        if not self.acquired:
+            return
         storage = self.storage
         try:
             read_only = storage.read_only
             storage.disable_readonly()
             del storage[self.path]
         except Exception:
             pass
@@ -147,85 +172,48 @@
     ):
         self.storage = storage
         self.path = get_dataset_lock_key() if path is None else path
         self.lock_lost_callback = lock_lost_callback
         self.acquired = False
         self._thread_lock = threading.Lock()
         self._previous_update_timestamp = None
-        username = get_user_name()
-        if username == "public":
-            self.username = None
-        else:
-            self.username = username
+        self.lock = Lock(storage, self.path, deeplake.constants.DATASET_LOCK_VALIDITY)
+        self.acquired = False
         self.acquire()
         atexit.register(self.release)
 
-    def _lock_loop(self):
-        try:
-            while True:
-                try:
-                    if (
-                        self._previous_update_timestamp is not None
-                        and time.time() - self._previous_update_timestamp
-                        >= deeplake.constants.DATASET_LOCK_VALIDITY
-                    ):
-                        # Its been too long since last update, another machine might have locked the storage
-                        lock_bytes = self.storage.get(self.path)
-                        if lock_bytes:
-                            nodeid, _, _ = _parse_lock_bytes(lock_bytes)
-                            if nodeid != uuid.getnode():
-                                if self.lock_lost_callback:
-                                    self.lock_lost_callback()
-                                self.acquired = False
-                                return
-                        elif not self._init:
-                            if self.lock_lost_callback:
-                                self.lock_lost_callback()
-                            self.acquired = False
-                            return
-                    self._previous_update_timestamp = time.time()
-                    self.storage[self.path] = _get_lock_bytes()
-                except Exception:
-                    pass
-                self._init = False
-                time.sleep(deeplake.constants.DATASET_LOCK_UPDATE_INTERVAL)
-        except Exception:  # Thread termination
-            return
-
     def acquire(self):
         if self.acquired:
             return
-        self.storage.check_readonly()
-        lock_bytes = self.storage.get(self.path)
-        if lock_bytes is not None:
-            nodeid = None
-            try:
-                nodeid, timestamp, _ = _parse_lock_bytes(lock_bytes)
-            except Exception:  # parse error from corrupt lock file, ignore
-                pass
-            if nodeid:
-                if nodeid == uuid.getnode():
-                    # Lock left by this machine from a previous run, ignore
-                    pass
-                elif time.time() - timestamp < deeplake.constants.DATASET_LOCK_VALIDITY:
-                    raise LockedException()
-
-        self._init = True
+        self.lock.acquire(timeout=0)
         self._thread = threading.Thread(target=self._lock_loop, daemon=True)
         self._thread.start()
         self.acquired = True
 
+    def _lock_loop(self):
+        try:
+            while True:
+                time.sleep(deeplake.constants.DATASET_LOCK_UPDATE_INTERVAL)
+                try:
+                    self.lock.refresh_lock(timeout=0)
+                except LockedException:
+                    if self.lock_lost_callback:
+                        self.lock_lost_callback()
+                    return
+        except Exception:  # Thread termination
+            return
+
     def release(self):
         if not self.acquired:
             return
         with self._thread_lock:
             terminate_thread(self._thread)
             self._acquired = False
         try:
-            del self.storage[self.path]
+            self.lock.release()
         except Exception:
             pass
 
 
 _LOCKS: Dict[str, Lock] = {}
 _REFS: Dict[str, Set[int]] = defaultdict(set)
```

### Comparing `deeplake-3.2.9/deeplake/core/meta/dataset_meta.py` & `deeplake-3.3.0/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.3.0/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.3.0/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.3.0/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/meta/encode/creds.py` & `deeplake-3.3.0/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/meta/encode/sequence.py` & `deeplake-3.3.0/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/meta/encode/shape.py` & `deeplake-3.3.0/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.3.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.3.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.3.0/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.3.0/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.3.0/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/meta/encode/tile.py` & `deeplake-3.3.0/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/meta/tensor_meta.py` & `deeplake-3.3.0/deeplake/core/meta/tensor_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,18 +289,15 @@
 
     defaults = HTYPE_CONFIGURATIONS[htype]
 
     for k, v in htype_overwrite.items():
         if isinstance(v, str) and v == UNSPECIFIED:
             htype_overwrite[k] = defaults[k]
 
-    if (
-        htype in ("json", "list", "text", "point_cloud_calibration_matrix")
-        and not htype_overwrite["dtype"]
-    ):
+    if htype in ("json", "list", "text", "intrinsics") and not htype_overwrite["dtype"]:
         htype_overwrite["dtype"] = HTYPE_CONFIGURATIONS[htype]["dtype"]
 
 
 def _validate_required_htype_overwrites(htype: str, htype_overwrite: dict):
     """Raises errors if `htype_overwrite` has invalid values."""
     sample_compression = htype_overwrite["sample_compression"]
     sample_compression = COMPRESSION_ALIASES.get(sample_compression, sample_compression)
@@ -338,15 +335,15 @@
 
 
 def _format_values(htype: str, htype_overwrite: dict):
     """Replaces values in `htype_overwrite` with consistent types/formats."""
 
     dtype = htype_overwrite["dtype"]
     if dtype is not None:
-        if htype in ("json", "list", "point_cloud_calibration_matrix"):
+        if htype in ("json", "list", "intrinsics"):
             if getattr(dtype, "__module__", None) == "typing":
                 htype_overwrite["dtype"] = str(dtype)
         else:
             htype_overwrite["dtype"] = np.dtype(htype_overwrite["dtype"]).name
 
     for key, value in COMPRESSION_ALIASES.items():
         if htype_overwrite.get("sample_compression") == key:
```

### Comparing `deeplake-3.2.9/deeplake/core/partial_reader.py` & `deeplake-3.3.0/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/partial_sample.py` & `deeplake-3.3.0/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/polygon.py` & `deeplake-3.3.0/deeplake/core/polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+from deeplake.util.exceptions import EmptyPolygonError
 from typing import Union, List
+
 import numpy as np
 import deeplake
 
 
 class Polygon:
     """Represents a polygon."""
 
     def __init__(self, coords: Union[np.ndarray, List[float]], dtype="float32"):
+        if coords is None or len(coords) == 0:
+            raise EmptyPolygonError(
+                "A polygons sample can be empty or None but a polygon within a sample cannot be empty or None."
+            )
         self.coords = coords
         self.dtype = dtype
 
     @property
     def ndim(self):
         """Dimension of the polygon."""
         return len(self.coords[0])
```

### Comparing `deeplake-3.2.9/deeplake/core/query/autocomplete.py` & `deeplake-3.3.0/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/query/filter.py` & `deeplake-3.3.0/deeplake/core/query/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
     if vds:
         dataset._send_query_progress(
             query_text=query_text, query_id=query_id, start=True, progress=0
         )
 
     try:
         if progressbar:
-            result = compute.map_with_progressbar(pg_filter_slice, idx, total_length=len(dataset))  # type: ignore
+            result = compute.map_with_progress_bar(pg_filter_slice, idx, total_length=len(dataset))  # type: ignore
         else:
             result = compute.map(filter_slice, idx)  # type: ignore
         index_map = [k for x in result for k in x]  # unfold the result map
         if vds:
             dataset._send_query_progress(
                 query_text=query_text,
                 query_id=query_id,
@@ -442,15 +442,15 @@
             btch = len(dataset) // num_workers
             subdatasets = [
                 QuerySlice(idx * btch, btch, dataset, query)
                 for idx in range(0, num_workers)
             ]
 
             if progressbar:
-                result = compute.map_with_progressbar(pg_subquery, subdatasets, total_length=num_samples)  # type: ignore
+                result = compute.map_with_progress_bar(pg_subquery, subdatasets, total_length=num_samples)  # type: ignore
             else:
                 result = compute.map(subquery, subdatasets)  # type: ignore
 
             index_map = []
             for ls in result:
                 index_map.extend(ls)
```

### Comparing `deeplake-3.2.9/deeplake/core/query/query.py` & `deeplake-3.3.0/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/sample.py` & `deeplake-3.3.0/deeplake/core/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,27 @@
     AUDIO_COMPRESSION,
     IMAGE_COMPRESSION,
     VIDEO_COMPRESSION,
     POINT_CLOUD_COMPRESSION,
     MESH_COMPRESSION,
     NIFTI_COMPRESSION,
 )
-from deeplake.util.exceptions import UnableToReadFromUrlError
+from deeplake.util.exceptions import SampleReadError, UnableToReadFromUrlError
 from deeplake.util.exif import getexif
 from deeplake.core.storage.provider import StorageProvider
 from deeplake.util.path import get_path_type, is_remote_path
 import numpy as np
 from typing import Optional, Tuple, Union, Dict
 
 from PIL import Image  # type: ignore
 from PIL.ExifTags import TAGS  # type: ignore
 from io import BytesIO
 
 from deeplake.core.storage.s3 import S3Provider
+from deeplake.core.storage import storage_factory
 from deeplake.core.storage.google_drive import GDriveProvider
 
 try:
     from deeplake.core.storage.gcs import GCSProvider
 except ImportError:
     GCSProvider = None  # type: ignore
 
@@ -428,24 +429,27 @@
         if self.path is not None and other.path is not None:
             return self.path == other.path
         return self.buffer == other.buffer
 
     def _read_from_path(self) -> bytes:  # type: ignore
         if self._buffer is None:
             path_type = get_path_type(self.path)
-            if path_type == "local":
-                self._buffer = self._read_from_local()
-            elif path_type == "gcs":
-                self._buffer = self._read_from_gcs()
-            elif path_type == "s3":
-                self._buffer = self._read_from_s3()
-            elif path_type == "gdrive":
-                self._buffer = self._read_from_gdrive()
-            elif path_type == "http":
-                self._buffer = self._read_from_http()
+            try:
+                if path_type == "local":
+                    self._buffer = self._read_from_local()
+                elif path_type == "gcs":
+                    self._buffer = self._read_from_gcs()
+                elif path_type == "s3":
+                    self._buffer = self._read_from_s3()
+                elif path_type == "gdrive":
+                    self._buffer = self._read_from_gdrive()
+                elif path_type == "http":
+                    self._buffer = self._read_from_http()
+            except Exception as e:
+                raise SampleReadError(self.path) from e  # type: ignore
         return self._buffer  # type: ignore
 
     def _read_from_local(self) -> bytes:
         with open(self.path, "rb") as f:  # type: ignore
             return f.read()
 
     def _get_root_and_key(self, path):
@@ -459,35 +463,37 @@
     def _read_from_s3(self) -> bytes:
         assert self.path is not None
         if self.storage is not None:
             assert isinstance(self.storage, S3Provider)
             return self.storage.get_object_from_full_url(self.path)
         path = self.path.replace("s3://", "")  # type: ignore
         root, key = self._get_root_and_key(path)
-        s3 = S3Provider(root, **self._creds)
+        s3 = storage_factory(S3Provider, root, **self._creds)
         return s3[key]
 
     def _read_from_gcs(self) -> bytes:
         assert self.path is not None
         if GCSProvider is None:
             raise Exception(
                 "GCP dependencies not installed. Install them with pip install deeplake[gcs]"
             )
         if self.storage is not None:
             assert isinstance(self.storage, GCSProvider)
             return self.storage.get_object_from_full_url(self.path)
         path = self.path.replace("gcp://", "").replace("gcs://", "")  # type: ignore
         root, key = self._get_root_and_key(path)
-        gcs = GCSProvider(root, token=self._creds)
+        gcs = storage_factory(GCSProvider, root, token=self._creds)
         return gcs[key]
 
     def _read_from_gdrive(self) -> bytes:
         assert self.path is not None
-        gdrive = GDriveProvider("gdrive://", token=self._creds, makemap=False)
-        return gdrive.get_object_from_full_url(self.path)
+        gdrive = storage_factory(
+            GDriveProvider, "gdrive://", token=self._creds, makemap=False
+        )
+        return gdrive.get_object_from_full_url(self.path)  # type: ignore
 
     def _read_from_http(self) -> bytes:
         assert self.path is not None
         if "Authorization" in self._creds:
             headers = {"Authorization": self._creds["Authorization"]}
         else:
             headers = {}
```

### Comparing `deeplake-3.2.9/deeplake/core/serialize.py` & `deeplake-3.3.0/deeplake/core/serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,14 +398,30 @@
         return version, ids, dtype
 
 
 def serialize_sequence_or_creds_encoder(version: str, enc: np.ndarray) -> bytes:
     return len(version).to_bytes(1, "little") + version.encode("ascii") + enc.tobytes()
 
 
+def serialize_pad_encoder(version: str, enc: np.ndarray) -> bytes:
+    return len(version).to_bytes(1, "little") + version.encode("ascii") + enc.tobytes()
+
+
+def deserialize_pad_encoder(byts: Union[bytes, memoryview]) -> Tuple[str, np.ndarray]:
+    byts = memoryview(byts)
+    len_version = byts[0]
+    version = str(byts[1 : 1 + len_version], "ascii")
+    enc = (
+        np.frombuffer(byts[1 + len_version :], dtype=deeplake.constants.ENCODING_DTYPE)
+        .reshape(-1)
+        .copy()
+    )
+    return version, enc
+
+
 def deserialize_sequence_or_creds_encoder(
     byts: Union[bytes, memoryview], enc_type: str
 ) -> Tuple[str, np.ndarray]:
     dim = 2 if enc_type == "creds" else 3
     byts = memoryview(byts)
     len_version = byts[0]
     version = str(byts[1 : 1 + len_version], "ascii")
```

### Comparing `deeplake-3.2.9/deeplake/core/storage/gcs.py` & `deeplake-3.3.0/deeplake/core/storage/gcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,20 +268,24 @@
             AttributeError,
             NotFound,
         )
         self._initialize_provider()
         self._presigned_urls: Dict[str, Tuple[str, float]] = {}
         self.expiration: Optional[str] = None
 
-    def subdir(self, path: str):
-        return self.__class__(
+    def subdir(self, path: str, read_only: bool = False):
+        sd = self.__class__(
             root=posixpath.join(self.root, path),
             token=self.token,
             project=self.project,
         )
+        if self.expiration:
+            sd._set_hub_creds_info(self.hub_path, self.expiration)
+        sd.read_only = read_only
+        return sd
 
     def _initialize_provider(self):
         self._set_bucket_and_path()
         if not self.token:
             self.token = None
         self.scoped_credentials = GCloudCredentials(self.token, project=self.project)
         self.retry = retry.Retry(deadline=60)
```

### Comparing `deeplake-3.2.9/deeplake/core/storage/google_drive.py` & `deeplake-3.3.0/deeplake/core/storage/google_drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,7 +363,14 @@
             if key.startswith(prefix):
                 try:
                     del self[key]
                 except:
                     pass
         if not prefix:
             self._delete_file(self.root_id)
+
+    def get_object_size(self, key: str) -> int:
+        id = self._get_id(key)
+        if not id:
+            raise KeyError(key)
+        size = int(self.drive.files().get(fileId=id, fields="size").execute()["size"])
+        return size
```

### Comparing `deeplake-3.2.9/deeplake/core/storage/local.py` & `deeplake-3.3.0/deeplake/core/storage/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,18 @@
         """
         if os.path.isfile(root):
             raise FileAtPathException(root)
         self.root = root
         self.files: Optional[Set[str]] = None
         self._all_keys()
 
-    def subdir(self, path: str):
-        return self.__class__(os.path.join(self.root, path))
+    def subdir(self, path: str, read_only: bool = False):
+        sd = self.__class__(os.path.join(self.root, path))
+        sd.read_only = read_only
+        return sd
 
     def __getitem__(self, path: str):
         """Gets the object present at the path within the given byte range.
 
         Example:
 
             >>> local_provider = LocalProvider("/home/ubuntu/Documents/")
```

### Comparing `deeplake-3.2.9/deeplake/core/storage/lru_cache.py` & `deeplake-3.3.0/deeplake/core/storage/lru_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 
 def _get_nbytes(obj: Union[bytes, memoryview, DeepLakeMemoryObject]):
     if isinstance(obj, DeepLakeMemoryObject):
         return obj.nbytes
     return len(obj)
 
 
+def obj_to_bytes(obj):
+    if isinstance(obj, DeepLakeMemoryObject):
+        obj = obj.tobytes()
+    if isinstance(obj, memoryview):
+        obj = bytes(obj)
+    return obj
+
+
 class LRUCache(StorageProvider):
     """LRU Cache that uses StorageProvider for caching"""
 
     def __init__(
         self,
         cache_storage: StorageProvider,
         next_storage: Optional[StorageProvider],
@@ -45,14 +53,21 @@
 
         self.dirty_keys: Dict[str, None] = (
             OrderedDict() if sys.version_info < (3, 7) else {}  # type: ignore
         )  # keys present in cache but not next_storage. Using a dict instead of set to preserve order.
 
         self.cache_used = 0
         self.deeplake_objects: Dict[str, DeepLakeMemoryObject] = {}
+        # TODO: BRING THIS BACK AFTER ASYNC IS FIXED
+        # self.use_async = (
+        #     next_storage.async_supported()
+        #     if next_storage
+        #     else False and sys.version_info >= (3, 7) and sys.platform != "win32"
+        # )
+        self.use_async = False
 
     def register_deeplake_object(self, path: str, obj: DeepLakeMemoryObject):
         """Registers a new object in the cache."""
         self.deeplake_objects[path] = obj
 
     def clear_deeplake_objects(self):
         """Removes all DeepLakeMemoryObjects from the cache."""
@@ -80,18 +95,26 @@
         self.autoflush = False
         for path, obj in self.deeplake_objects.items():
             if obj.is_dirty:
                 self[path] = obj
                 obj.is_dirty = False
 
         if self.dirty_keys:
-            for key in self.dirty_keys.copy():
-                self._forward(key)
-            if self.next_storage is not None:
-                self.next_storage.flush()
+            if hasattr(self.next_storage, "set_items") and self.use_async:
+                d = {
+                    key: obj_to_bytes(self.cache_storage[key])
+                    for key in self.dirty_keys
+                }
+                self.next_storage.set_items(d)
+                self.dirty_keys.clear()
+            else:
+                for key in self.dirty_keys.copy():
+                    self._forward(key)
+                if self.next_storage is not None:
+                    self.next_storage.flush()
 
         self.autoflush = initial_autoflush
 
     def get_deeplake_object(
         self,
         path: str,
         expected_class,
```

### Comparing `deeplake-3.2.9/deeplake/core/storage/memory.py` & `deeplake-3.3.0/deeplake/core/storage/memory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict
 from deeplake.core.storage.lru_cache import _get_nbytes
 from deeplake.core.storage.provider import StorageProvider
+import os
 
 
 class MemoryProvider(StorageProvider):
     """Provider class for using the memory."""
 
     def __init__(self, root: str = ""):
         self.dict: Dict[str, Any] = {}
@@ -120,7 +121,12 @@
         return self.root
 
     def __setstate__(self, state: str):
         self.__init__(root=state)  # type: ignore
 
     def get_object_size(self, key: str) -> int:
         return _get_nbytes(self[key])
+
+    def subdir(self, path: str, read_only: bool = False):
+        sd = self.__class__(os.path.join(self.root, path))
+        sd.read_only = read_only
+        return sd
```

### Comparing `deeplake-3.2.9/deeplake/core/storage/provider.py` & `deeplake-3.3.0/deeplake/core/storage/provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,31 @@
 from abc import ABC, abstractmethod
 from collections.abc import MutableMapping
-from typing import Optional, Set, Sequence
+from typing import Optional, Set, Sequence, Dict
 
 from deeplake.constants import BYTE_PADDING
 from deeplake.util.assert_byte_indexes import assert_byte_indexes
 from deeplake.util.exceptions import ReadOnlyModeError
 from deeplake.util.keys import get_dataset_lock_key
 import posixpath
+import threading
+
+_STORAGES: Dict[str, "StorageProvider"] = {}
+
+
+def storage_factory(cls, root: str = "", *args, **kwargs) -> "StorageProvider":
+    if cls.__name__ == "MemoryProvider":
+        return cls(root, *args, **kwargs)
+    thread_id = threading.get_ident()
+    try:
+        return _STORAGES[f"{thread_id}_{root}_{args}_{kwargs}"]
+    except KeyError:
+        storage = cls(root, *args, **kwargs)
+        _STORAGES[f"{thread_id}_{root}_{args}_{kwargs}"] = storage
+        return storage
 
 
 class StorageProvider(ABC, MutableMapping):
     autoflush = False
     read_only = False
     root = ""
     _is_hub_path = False
@@ -189,7 +204,10 @@
         return new_provider
 
     def get_presigned_url(self, key: str) -> str:
         return posixpath.join(self.root, key)
 
     def get_object_size(self, key: str) -> int:
         raise NotImplementedError()
+
+    def async_supported(self) -> bool:
+        return False
```

### Comparing `deeplake-3.2.9/deeplake/core/storage/s3.py` & `deeplake-3.3.0/deeplake/core/storage/s3.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,24 @@
 try:
     from botocore.exceptions import ResponseStreamingError
 
     CONNECTION_ERRORS = CONNECTION_ERRORS + (ResponseStreamingError,)  # type: ignore
 except ImportError:
     pass
 
+try:
+    import aioboto3  # type: ignore
+    import asyncio  # type: ignore
+    import nest_asyncio  # type: ignore
+
+    nest_asyncio.apply()  # needed to run asyncio in jupyter notebook
+except Exception:
+    aioboto3 = None  # type: ignore
+    asyncio = None  # type: ignore
+
 
 class S3ResetReloadCredentialsManager:
     """Tries to reload the credentials if the error is due to expired token, if error still occurs, it raises it."""
 
     def __init__(self, s3p, error_class: Type[S3Error]):
         self.error_class = error_class
         self.s3p = s3p
@@ -110,25 +120,30 @@
         self.loaded_creds_from_environment = False
         self.client_config = deeplake.config["s3"]
         self.start_time = time.time()
         self.profile_name = profile_name
         self._initialize_s3_parameters()
         self._presigned_urls: Dict[str, Tuple[str, float]] = {}
 
-    def subdir(self, path: str):
+    def async_supported(self) -> bool:
+        return asyncio is not None
+
+    def subdir(self, path: str, read_only: bool = False):
         sd = self.__class__(
             root=posixpath.join(self.root, path),
             aws_access_key_id=self.aws_access_key_id,
             aws_secret_access_key=self.aws_secret_access_key,
             aws_session_token=self.aws_session_token,
             aws_region=self.aws_region,
             endpoint_url=self.endpoint_url,
+            token=self.token,
         )
-        if sd.expiration:
+        if self.expiration:
             sd._set_hub_creds_info(self.hub_path, self.expiration)  # type: ignore
+        sd.read_only = read_only
         return sd
 
     def _set(self, path, content):
         self.client.put_object(
             Bucket=self.bucket,
             Body=content,
             Key=path,
@@ -504,25 +519,33 @@
             self.aws_secret_access_key = credentials.secret_key
             self.aws_session_token = credentials.token
             self.aws_region = session._resolve_region_name(
                 self.aws_region, self.client_config
             )
 
     def _set_s3_client_and_resource(self):
-        args = {
+        kwargs = self.s3_kwargs
+        session = boto3.session.Session(profile_name=self.profile_name)
+        self.client = session.client("s3", **kwargs)
+        self.resource = session.resource("s3", **kwargs)
+        if aioboto3 is not None:
+            self.async_session = aioboto3.session.Session(
+                profile_name=self.profile_name
+            )
+
+    @property
+    def s3_kwargs(self):
+        return {
             "aws_access_key_id": self.aws_access_key_id,
             "aws_secret_access_key": self.aws_secret_access_key,
             "aws_session_token": self.aws_session_token,
             "region_name": self.aws_region,
             "endpoint_url": self.endpoint_url,
             "config": self.client_config,
         }
-        session = boto3.session.Session(profile_name=self.profile_name)
-        self.client = session.client("s3", **args)
-        self.resource = session.resource("s3", **args)
 
     def need_to_reload_creds(self, err: botocore.exceptions.ClientError) -> bool:
         """Checks if the credentials need to be reloaded.
         This happens if the credentials were loaded from the environment and have now expired.
         """
         return (
             err.response["Error"]["Code"] == "ExpiredToken"
@@ -591,7 +614,47 @@
                     )
                     return ret
                 except Exception:
                     pass
             raise S3GetError(err) from err
         except Exception as err:
             raise S3GetError(err) from err
+
+    def _set_items(self, items: dict):
+        async def set_items_async(items):
+            async with self.async_session.client("s3", **self.s3_kwargs) as client:
+                tasks = []
+                for k, v in items.items():
+                    tasks.append(
+                        asyncio.ensure_future(
+                            client.put_object(
+                                Bucket=self.bucket, Key=self.path + k, Body=v
+                            )
+                        )
+                    )
+                await asyncio.gather(*tasks)
+
+        loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(loop)
+        loop.run_until_complete(set_items_async(items))
+
+    def set_items(self, items: dict):
+        try:
+            self._set_items(items)
+        except botocore.exceptions.ClientError as err:
+            with S3ResetReloadCredentialsManager(self, S3SetError):
+                self._set_items(items)
+        except CONNECTION_ERRORS as err:
+            tries = self.num_tries
+            for i in range(1, tries + 1):
+                always_warn(f"Encountered connection error, retry {i} out of {tries}")
+                try:
+                    self._set_items(items)
+                    always_warn(
+                        f"Connection re-established after {i} {['retries', 'retry'][i==1]}."
+                    )
+                    return
+                except Exception:
+                    pass
+            raise S3SetError(err) from err
+        except Exception as err:
+            raise S3SetError(err) from err
```

### Comparing `deeplake-3.2.9/deeplake/core/tensor.py` & `deeplake-3.3.0/deeplake/core/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -402,15 +402,14 @@
             sample (InputSample): The data to append to the tensor. :class:`~deeplake.core.sample.Sample` is generated by :func:`deeplake.read`. See the above examples.
         """
         self.extend([sample], progressbar=False)
 
     def clear(self):
         """Deletes all samples from the tensor"""
         self.chunk_engine.clear()
-        sample_id_key = get_sample_id_tensor_key(self.key)
         try:
             for t in self._all_tensor_links():
                 t.chunk_engine.clear()
         except TensorDoesNotExistError:
             pass
         self.invalidate_libdeeplake_dataset()
 
@@ -473,16 +472,18 @@
             if sample_shape_tensor
             else None
         )
         shape: Tuple[Optional[int], ...]
         shape = self.chunk_engine.shape(
             self.index, sample_shape_provider=sample_shape_provider
         )
-        if not shape and self.meta.max_shape:
-            shape = (0,) * len(self.meta.max_shape)
+
+        if len(self.index.values) == 1 and not self.index.values[0].subscriptable():
+            if np.sum(shape) == 0 and self.meta.max_shape:  # type: ignore
+                shape = (0,) * len(self.meta.max_shape)
         if self.meta.max_shape == [0, 0, 0]:
             shape = ()
         return shape
 
     @property
     def size(self) -> Optional[int]:
         s = 1
@@ -565,15 +566,15 @@
 
         Returns:
             ShapeInterval: Object containing ``lower`` and ``upper`` properties.
 
         Note:
             If you are expecting a tuple, use :attr:`shape` instead.
         """
-        return self.chunk_engine.shape_interval
+        return self.chunk_engine.shape_interval(self.index)
 
     @property
     def is_dynamic(self) -> bool:
         """Will return ``True`` if samples in this tensor have shapes that are unequal."""
         return self.shape_interval.is_dynamic
 
     @property
@@ -1035,17 +1036,47 @@
                 )
                 if val is not _NO_LINK_UPDATE:
                     if is_partial and func == update_downsample:
                         apply_partial_downsample(tensor, global_sample_index, val)
                     else:
                         val = cast_to_type(val, tensor.dtype)
                         tensor[global_sample_index] = val
-        # if self.meta.is_link and not has_shape_tensor:
-        #     func = get_link_transform("update_shape")
-        #     func(new_sample, link_creds=self.link_creds, tensor_meta=self.meta)
+
+    @invalid_view_op
+    def pop(self, index: Optional[int] = None):
+        """Removes an element at the given index."""
+
+        self.chunk_engine.pop(
+            index, link_callback=self._pop_links if self.meta.links else None
+        )
+
+        self.invalidate_libdeeplake_dataset()
+
+    def _pop_links(self, global_sample_index: int):
+        # meta.links contain tensor keys not names
+        rev_tensor_names = {v: k for k, v in self.dataset.meta.tensor_names.items()}
+
+        if self.meta.is_sequence:
+            flat_links: List[str] = []
+            links: List[str] = []
+            for link, props in self.meta.links.items():
+                (flat_links if props["flatten_sequence"] else links).append(link)
+
+            if flat_links:
+                seq_enc = self.chunk_engine.sequence_encoder
+                for link in flat_links:
+                    link_tensor = self.dataset[rev_tensor_names.get(link)]
+                    for idx in reversed(range(*seq_enc[global_sample_index])):
+                        link_tensor.pop(idx)
+        else:
+            links = list(self.meta.links.keys())
+        [
+            self.dataset[rev_tensor_names.get(link)].pop(global_sample_index)
+            for link in links
+        ]
 
     def _all_tensor_links(self):
         ds = self.dataset
         return [
             ds.version_state["full_tensors"][ds.version_state["tensor_names"][l]]
             for l in self.meta.links
         ]
@@ -1143,15 +1174,15 @@
             raise ValueError("Not supported as the tensor is not a link.")
         if self.index.values[0].subscriptable() or len(self.index.values) > 1:
             raise ValueError("_linked_sample can be used only on exatcly 1 sample.")
         return self.chunk_engine.linked_sample(self.index.values[0].value)
 
     def _get_video_stream_url(self):
         if self.is_link:
-            return self.chunk_engine.get_video_url(self.index.values[0].value)
+            return self.chunk_engine.get_video_url(self.index.values[0].value)[0]
 
         from deeplake.visualizer.video_streaming import get_video_stream_url
 
         return get_video_stream_url(self, self.index.values[0].value)
 
     def play(self):
         """Play video sample. Plays video in Jupyter notebook or plays in web browser. Video is streamed directly from storage.
@@ -1183,23 +1214,14 @@
             return video_html(
                 src=self._get_video_stream_url(),
                 alt=f"{self.key}[{self.index.values[0].value}]",
             )
         else:
             webbrowser.open(self._get_video_stream_url())
 
-    @invalid_view_op
-    def pop(self, index: Optional[int] = None):
-        """Removes an element at the given index."""
-        if index is None:
-            index = self.num_samples - 1
-        self.chunk_engine.pop(index)
-        [self.dataset[link].pop(index) for link in self.meta.links]
-        self.invalidate_libdeeplake_dataset()
-
     @property
     def timestamps(self) -> np.ndarray:
         """Returns timestamps (in seconds) for video sample as numpy array.
 
         Example:
 
             >>> # Return timestamps for all frames of first video sample
@@ -1223,15 +1245,15 @@
             if len(index.values) == 1 or index.values[1].subscriptable():
                 raise ValueError("Only supported for exactly 1 video sample.")
             sub_index = index.values[2].value if len(index.values) > 2 else None
         else:
             sub_index = index.values[1].value if len(index.values) > 1 else None
         global_sample_index = next(index.values[0].indices(self.num_samples))
         if self.is_link:
-            sample = self.chunk_engine.get_video_url(global_sample_index)  # type: ignore
+            sample = self.chunk_engine.get_video_url(global_sample_index)[0]  # type: ignore
         else:
             sample = self.chunk_engine.get_video_sample(
                 global_sample_index, index, decompress=False
             )
 
         nframes = self.shape[0]
         start, stop, step, reverse = normalize_index(sub_index, nframes)
@@ -1288,10 +1310,19 @@
     def path(self, fetch_chunks: bool = False):
         """Return path data. Only applicable for linked tensors"""
         if not self.is_link:
             raise Exception(f"Only supported for linked tensors.")
         assert isinstance(self.chunk_engine, LinkedChunkEngine)
         return self.chunk_engine.path(self.index, fetch_chunks=fetch_chunks)
 
+    def creds_key(self):
+        """Return path data. Only applicable for linked tensors"""
+        if not self.is_link:
+            raise Exception(f"Only supported for linked tensors.")
+        if self.index.values[0].subscriptable() or len(self.index.values) > 1:
+            raise ValueError("_linked_sample can be used only on exatcly 1 sample.")
+        assert isinstance(self.chunk_engine, LinkedChunkEngine)
+        return self.chunk_engine.creds_key(self.index.values[0].value)
+
     def invalidate_libdeeplake_dataset(self):
         """Invalidates the libdeeplake dataset object."""
         self.dataset.libdeeplake_dataset = None
```

### Comparing `deeplake-3.2.9/deeplake/core/tensor_link.py` & `deeplake-3.3.0/deeplake/core/tensor_link.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Callable
+import warnings
 from deeplake.core.compression import to_image
 from deeplake.core.index import Index
 from deeplake.constants import _NO_LINK_UPDATE
 import inspect
 import deeplake
 import inspect
 import numpy as np
@@ -98,30 +99,29 @@
     else:
         return extend_info.f([new_sample], link_creds)[0]
     return _NO_LINK_UPDATE
 
 
 @link
 def update_shape(new_sample, link_creds=None, tensor_meta=None):
+    if new_sample is None:
+        return np.zeros(1, dtype=np.int64)
     if isinstance(new_sample, deeplake.core.linked_sample.LinkedSample):
         new_sample = read_linked_sample(
             new_sample.path, new_sample.creds_key, link_creds, verify=False
         )
     if np.isscalar(new_sample):
         ret = np.array([1], dtype=np.int64)
     else:
         ret = np.array(
             getattr(new_sample, "shape", None) or np.array(new_sample).shape,
             dtype=np.int64,
         )
 
     if tensor_meta:
-        if tensor_meta.is_link and ret.size and np.prod(ret):
-            tensor_meta.update_shape_interval(ret.tolist())
-
         # if grayscale being appended but tensor has rgb samples, convert shape from (h, w) to (h, w, 1)
         if (
             tensor_meta.min_shape
             and (
                 tensor_meta.htype == "image"
                 or (
                     IMAGE_COMPRESSION
@@ -132,14 +132,17 @@
                 )
             )
             and ret.shape == (2,)
             and len(tensor_meta.min_shape) == 3
         ):
             ret = np.concatenate([ret, (1,)])
 
+        if tensor_meta.is_link and ret.size and np.prod(ret):
+            tensor_meta.update_shape_interval(ret.tolist())
+
     return ret
 
 
 @link
 def extend_shape(samples, link_creds=None, tensor_meta=None):
     if isinstance(samples, np.ndarray):
         if samples.dtype != object:
@@ -149,57 +152,57 @@
             return np.tile(np.array([samples_shape[1:]]), (samples_shape[0], 1))
     if samples is None:
         return np.array([], dtype=np.int64)
     shapes = [
         update_shape.f(sample, link_creds=link_creds, tensor_meta=tensor_meta)
         for sample in samples
     ]
-    mixed_ndim = False
-    try:
-        arr = np.array(shapes)
-        if arr.dtype == object:
-            mixed_ndim = True
-    except ValueError:
-        mixed_ndim = True
+
+    max_ndim = max(map(len, shapes), default=0)
+    min_ndim = min(map(len, shapes), default=0)
+    mixed_ndim = max_ndim != min_ndim
 
     if mixed_ndim:
-        ndim = max(map(len, shapes))
         for i, s in enumerate(shapes):
-            if len(s) < ndim:
+            if len(s) < max_ndim:
                 shapes[i] = np.concatenate(
-                    [s, (int(bool(np.prod(s))),) * (ndim - len(s))]
+                    [s, (int(bool(np.any(s) and np.prod(s))),) * (max_ndim - len(s))]
                 )
-        arr = np.array(shapes)
+    arr = np.array(shapes)
     return arr
 
 
 @link
 def extend_len(samples, link_creds=None):
     return [0 if sample is None else len(sample) for sample in samples]
 
 
 @link
 def update_len(new_sample, link_creds=None):
     return 0 if new_sample is None else len(new_sample)
 
 
 def convert_sample_for_downsampling(sample, link_creds=None):
-    if isinstance(sample, deeplake.core.linked_sample.LinkedSample):
-        sample = read_linked_sample(
-            sample.path, sample.creds_key, link_creds, verify=False
-        )
-    if isinstance(sample, deeplake.core.sample.Sample):
-        sample = sample.pil
-    if (
-        isinstance(sample, np.ndarray)
-        and sample.dtype != bool
-        and 0 not in sample.shape
-    ):
-        sample = to_image(sample)
-    return sample
+    try:
+        if isinstance(sample, deeplake.core.linked_sample.LinkedSample):
+            sample = read_linked_sample(
+                sample.path, sample.creds_key, link_creds, verify=False
+            )
+        if isinstance(sample, deeplake.core.sample.Sample):
+            sample = sample.pil
+        if (
+            isinstance(sample, np.ndarray)
+            and sample.dtype != bool
+            and 0 not in sample.shape
+        ):
+            sample = to_image(sample)
+        return sample
+    except Exception as e:
+        warnings.warn(f"Failed to downsample sample of type {type(sample)}")
+        return None
 
 
 @link
 def extend_downsample(samples, factor, compression, htype, link_creds=None):
     samples = [
         convert_sample_for_downsampling(sample, link_creds) for sample in samples
     ]
```

### Comparing `deeplake-3.2.9/deeplake/core/test_serialize.py` & `deeplake-3.3.0/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/tests/test_compression.py` & `deeplake-3.3.0/deeplake/core/tests/test_compression.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 )
 from deeplake.util.exceptions import CorruptedSampleError
 from PIL import Image  # type: ignore
 
 
 image_compressions = IMAGE_COMPRESSIONS[:]
 image_compressions.remove("wmf")
-image_compressions.remove("apng")
+# image_compressions.remove("apng")
 image_compressions.remove("dcm")
 image_compressions.remove("fli")
 image_compressions.remove("mpo")
 
 image_compressions = list(
     filter(lambda c: is_readonly_compression(c), image_compressions)
 )
@@ -177,36 +177,36 @@
     path = point_cloud_paths[compression]
     sample = deeplake.read(path)
     arr = np.array(sample)
     if compression == "las":
         assert len(arr[0]) == 18
 
 
-def test_apng(memory_ds):
-    ds = memory_ds
+# def test_apng(memory_ds):
+#     ds = memory_ds
 
-    arrays = {
-        "binary": [
-            np.random.randint(
-                0, 256, (25, 50, np.random.randint(100, 200)), dtype=np.uint8
-            )
-            for _ in range(10)
-        ],
-        "rgb": [
-            np.random.randint(
-                0, 256, (np.random.randint(100, 200), 32, 64, 3), dtype=np.uint8
-            )
-            for _ in range(10)
-        ],
-        "rgba": [
-            np.random.randint(
-                0, 256, (np.random.randint(100, 200), 16, 32, 4), dtype=np.uint8
-            )
-            for _ in range(10)
-        ],
-    }
-    for k, v in arrays.items():
-        with ds:
-            ds.create_tensor(k, htype="image", sample_compression="apng")
-            ds[k].extend(v)
-        for arr1, arr2 in zip(ds[k].numpy(aslist=True), v):
-            np.testing.assert_array_equal(arr1, arr2)
+#     arrays = {
+#         "binary": [
+#             np.random.randint(
+#                 0, 256, (25, 50, np.random.randint(100, 200)), dtype=np.uint8
+#             )
+#             for _ in range(10)
+#         ],
+#         "rgb": [
+#             np.random.randint(
+#                 0, 256, (np.random.randint(100, 200), 32, 64, 3), dtype=np.uint8
+#             )
+#             for _ in range(10)
+#         ],
+#         "rgba": [
+#             np.random.randint(
+#                 0, 256, (np.random.randint(100, 200), 16, 32, 4), dtype=np.uint8
+#             )
+#             for _ in range(10)
+#         ],
+#     }
+#     for k, v in arrays.items():
+#         with ds:
+#             ds.create_tensor(k, htype="image", sample_compression="apng")
+#             ds[k].extend(v)
+#         for arr1, arr2 in zip(ds[k].numpy(aslist=True), v):
+#             np.testing.assert_array_equal(arr1, arr2)
```

### Comparing `deeplake-3.2.9/deeplake/core/tests/test_compute.py` & `deeplake-3.3.0/deeplake/core/tests/test_compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 def test_compute_with_progress_bar(scheduler):
     def f(pg_callback, x):
         pg_callback(1)
         return x * 2
 
     compute = get_compute_provider(scheduler=scheduler, num_workers=2)
     try:
-        r = compute.map_with_progressbar(f, range(1000), 1000)
+        r = compute.map_with_progress_bar(f, range(1000), 1000)
 
         assert r is not None
         assert len(r) == 1000
 
     finally:
         compute.close()
```

### Comparing `deeplake-3.2.9/deeplake/core/tests/test_io.py` & `deeplake-3.3.0/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/tests/test_locking.py` & `deeplake-3.3.0/deeplake/core/tests/test_locking.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 import numpy as np
 import pytest
 import deeplake
 import uuid
 import time
 import warnings
 import json
-from deeplake.tests.dataset_fixtures import enabled_cloud_dataset_generators
+from deeplake.tests.dataset_fixtures import (
+    enabled_persistent_non_gdrive_dataset_generators,
+)
 from concurrent.futures import ThreadPoolExecutor
+import deeplake
 
 _counter = 0
 
 
 class VM(object):
     """
     Emulates a different machine
@@ -20,74 +23,69 @@
     def __init__(self):
         global _counter
         self.id = _counter
         _counter += 1
 
     def __enter__(self):
         self._getnode = uuid.getnode
-        uuid.getnode = lambda: self.id
+        uuid.getnode = lambda: self.id  # type: ignore
         self._locks = deeplake.core.lock._LOCKS.copy()
         deeplake.core.lock._LOCKS.clear()
 
     def __exit__(self, *args, **kwargs):
         uuid.getnode = self._getnode
         deeplake.core.lock._LOCKS.update(self._locks)
 
 
-@enabled_cloud_dataset_generators
+@enabled_persistent_non_gdrive_dataset_generators
 def test_dataset_locking(ds_generator):
-    ds = ds_generator()
-    ds.create_tensor("x")
-    arr = np.random.random((32, 32))
-    ds.x.append(arr)
-
-    with VM():
-        # Make sure read only warning is raised
-        with pytest.warns(UserWarning):
-            ds = ds_generator()
-            np.testing.assert_array_equal(arr, ds.x[0].numpy())
-        assert ds.read_only == True
-        with pytest.raises(LockedException):
-            ds.read_only = False
-        # Raise error if user explicitly asks for write access
-        with pytest.raises(LockedException):
-            ds = ds_generator(read_only=False)
-        # No warnings if user requests read only mode
-        with warnings.catch_warnings(record=True) as ws:
-            ds = ds_generator(read_only=True)
-            np.testing.assert_array_equal(arr, ds.x[0].numpy())
-        assert not ws
+    deeplake.constants.LOCK_LOCAL_DATASETS = True
+    try:
+        ds = ds_generator()
+        ds.create_tensor("x")
+        arr = np.random.random((32, 32))
+        ds.x.append(arr)
+
+        with VM():
+            # Make sure read only warning is raised
+            with pytest.warns(UserWarning):
+                ds = ds_generator()
+                np.testing.assert_array_equal(arr, ds.x[0].numpy())
+            assert ds.read_only == True
+            with pytest.raises(LockedException):
+                ds.read_only = False
+            # Raise error if user explicitly asks for write access
+            with pytest.raises(LockedException):
+                ds = ds_generator(read_only=False)
+            # No warnings if user requests read only mode
+            with warnings.catch_warnings(record=True) as ws:
+                ds = ds_generator(read_only=True)
+                np.testing.assert_array_equal(arr, ds.x[0].numpy())
+            assert not ws
+    finally:
+        deeplake.constants.LOCK_LOCAL_DATASETS = False
 
-        DATASET_LOCK_VALIDITY = deeplake.constants.DATASET_LOCK_VALIDITY
-        # Temporarily set validity to 1 second so we dont have to wait too long.
-        deeplake.constants.DATASET_LOCK_VALIDITY = 1
-        # Wait for lock to expire.
-        time.sleep(1.1)
 
-        try:
-            ds = ds_generator()
-            np.testing.assert_array_equal(arr, ds.x[0].numpy())
-            assert ds.read_only == False
-        finally:
-            deeplake.constants.DATASET_LOCK_VALIDITY = DATASET_LOCK_VALIDITY
-
-
-@enabled_cloud_dataset_generators
+@enabled_persistent_non_gdrive_dataset_generators
 def test_vc_locking(ds_generator):
-    ds = ds_generator()
-    ds.create_tensor("x")
-    arr = np.random.random((32, 32))
-    ds.x.append(arr)
-    ds.commit()
-    ds.checkout("branch", create=True)
-    with VM():
-        with warnings.catch_warnings(record=True) as ws:
-            ds = ds_generator()
-        np.testing.assert_array_equal(arr, ds.x[0].numpy())
-        assert not ws, str(ws[0])
+    deeplake.constants.LOCK_LOCAL_DATASETS = True
+    try:
+        ds = ds_generator()
+        ds.create_tensor("x")
+        arr = np.random.random((32, 32))
+        ds.x.append(arr)
+        ds.commit()
+        ds.checkout("branch", create=True)
+        with VM():
+            with warnings.catch_warnings(record=True) as ws:
+                ds = ds_generator()
+            np.testing.assert_array_equal(arr, ds.x[0].numpy())
+            assert not ws, str(ws[0])
+    finally:
+        deeplake.constants.LOCK_LOCAL_DATASETS = False
 
 
 def test_lock_thread_leaking(s3_ds_generator):
     locks = deeplake.core.lock._LOCKS
     refs = deeplake.core.lock._REFS
     nlocks_previous = len(locks)
```

### Comparing `deeplake-3.2.9/deeplake/core/tests/test_readonly.py` & `deeplake-3.3.0/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/tests/test_serialize.py` & `deeplake-3.3.0/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/tiling/deserialize.py` & `deeplake-3.3.0/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/tiling/optimizer.py` & `deeplake-3.3.0/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.3.0/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/tiling/serialize.py` & `deeplake-3.3.0/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.3.0/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/tiling/test_serialize.py` & `deeplake-3.3.0/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/transform/test_transform.py` & `deeplake-3.3.0/deeplake/core/transform/test_transform.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import deeplake
 import pytest
 import numpy as np
 from click.testing import CliRunner
 from deeplake.core.storage.memory import MemoryProvider
-from deeplake.core.transform.transform_tensor import TransformTensor
 from deeplake.core.version_control.test_version_control import (
     compare_dataset_diff,
     compare_tensor_diff,
     get_default_tensor_diff,
     get_default_dataset_diff,
 )
 from deeplake.util.remove_cache import remove_memory_cache
 from deeplake.util.check_installation import ray_installed
 from deeplake.util.exceptions import InvalidOutputDatasetError, TransformError
 from deeplake.tests.common import parametrize_num_workers
 from deeplake.util.transform import get_pbar_description
 import deeplake
 import gc
+import re
 from deeplake.tests.common import get_dummy_data_path
 
 
 # github actions can only support 2 workers
 TRANSFORM_TEST_NUM_WORKERS = 2
 
 all_compressions = pytest.mark.parametrize("sample_compression", [None, "png", "jpeg"])
@@ -30,16 +30,16 @@
 all_schedulers = pytest.mark.parametrize("scheduler", schedulers)
 commit_or_not = pytest.mark.parametrize("do_commit", [True, False])
 
 
 @deeplake.compute
 def fn1(sample_in, samples_out, mul=1, copy=1):
     for _ in range(copy):
-        samples_out.image.append(np.ones((337, 200)) * sample_in * mul)
-        samples_out.label.append(np.ones((1,)) * sample_in * mul)
+        samples_out.image.append(np.ones((337, 200), dtype=np.uint8) * sample_in * mul)
+        samples_out.label.append(np.ones((1,), dtype=np.uint32) * sample_in * mul)
 
 
 @deeplake.compute
 def fn2(sample_in, samples_out, mul=1, copy=1):
     for _ in range(copy):
         samples_out.image.append(sample_in.image.numpy() * mul)
         samples_out.label.append(sample_in.label.numpy() * mul)
@@ -302,22 +302,22 @@
     ds_out.create_tensor("label")
     fn2(copy=1, mul=2).eval(
         data_in, ds_out, num_workers=num_workers, progressbar=False, scheduler=scheduler
     )
     assert len(ds_out) == 99
     for index in range(1, 100):
         np.testing.assert_array_equal(
-            ds_out[index - 1].image.numpy(), 2 * index * np.ones((index, index))
+            ds_out[index - 1].image.numpy(), 2 * index * np.ones((index, index, 1))
         )
         np.testing.assert_array_equal(
             ds_out[index - 1].label.numpy(), 2 * index * np.ones((1,))
         )
 
-    assert ds_out.image.shape_interval.lower == (99, 1, 1)
-    assert ds_out.image.shape_interval.upper == (99, 99, 99)
+    assert ds_out.image.shape_interval.lower == (99, 1, 1, 1)
+    assert ds_out.image.shape_interval.upper == (99, 99, 99, 1)
     data_in.delete()
 
 
 @all_schedulers
 def test_chain_transform_list_small(local_ds, scheduler):
     ls = list(range(100))
     ds_out = local_ds
@@ -331,15 +331,16 @@
         progressbar=False,
         scheduler=scheduler,
     )
     assert len(ds_out) == 600
     for i in range(100):
         for index in range(6 * i, 6 * i + 6):
             np.testing.assert_array_equal(
-                ds_out[index].image.numpy(), 15 * i * np.ones((337, 200))
+                ds_out[index].image.numpy(),
+                np.asarray(15 * i * np.ones((337, 200)), dtype=np.uint8),
             )
             np.testing.assert_array_equal(
                 ds_out[index].label.numpy(), 15 * i * np.ones((1,))
             )
 
 
 @all_schedulers
@@ -392,15 +393,16 @@
     assert len(ds_out) == 610
     for i in range(10):
         np.testing.assert_array_equal(ds_out[i].image.numpy(), i * np.ones((10, 10)))
         np.testing.assert_array_equal(ds_out[i].label.numpy(), i * np.ones((1,)))
     for i in range(100):
         for index in range(10 + 6 * i, 10 + 6 * i + 6):
             np.testing.assert_array_equal(
-                ds_out[index].image.numpy(), 15 * i * np.ones((337, 200))
+                ds_out[index].image.numpy(),
+                np.asarray(15 * i * np.ones((337, 200)), dtype=np.uint8),
             )
             np.testing.assert_array_equal(
                 ds_out[index].label.numpy(), 15 * i * np.ones((1,))
             )
 
     expected_tensor_diff = {
         "commit_id": local_ds.pending_commit_id,
@@ -484,22 +486,22 @@
             num_workers=TRANSFORM_TEST_NUM_WORKERS,
             progressbar=False,
             scheduler=scheduler,
         )
         assert len(ds_out) == 99
         for index in range(1, 100):
             np.testing.assert_array_equal(
-                ds_out[index - 1].image.numpy(), 2 * index * np.ones((index, index))
+                ds_out[index - 1].image.numpy(), 2 * index * np.ones((index, index, 1))
             )
             np.testing.assert_array_equal(
                 ds_out[index - 1].label.numpy(), 2 * index * np.ones((1,))
             )
 
-        assert ds_out.image.shape_interval.lower == (99, 1, 1)
-        assert ds_out.image.shape_interval.upper == (99, 99, 99)
+        assert ds_out.image.shape_interval.lower == (99, 1, 1, 1)
+        assert ds_out.image.shape_interval.upper == (99, 99, 99, 1)
 
 
 def test_transform_empty(local_ds):
     local_ds.create_tensor("image")
 
     ls = list(range(10))
     filter_tr().eval(ls, local_ds, progressbar=False)
@@ -574,22 +576,22 @@
         data_in, ds_out, num_workers=num_workers, scheduler=scheduler, progressbar=False
     )
 
     def test_ds_out():
         assert len(ds_out) == 99
         for index in range(1, 100):
             np.testing.assert_array_equal(
-                ds_out[index - 1].image.numpy(), 2 * index * np.ones((index, index))
+                ds_out[index - 1].image.numpy(), 2 * index * np.ones((index, index, 1))
             )
             np.testing.assert_array_equal(
                 ds_out[index - 1].label.numpy(), 2 * index * np.ones((1,))
             )
 
-        assert ds_out.image.shape_interval.lower == (99, 1, 1)
-        assert ds_out.image.shape_interval.upper == (99, 99, 99)
+        assert ds_out.image.shape_interval.lower == (99, 1, 1, 1)
+        assert ds_out.image.shape_interval.upper == (99, 99, 99, 1)
 
     test_ds_out()
     ds_out = local_ds_generator()
     test_ds_out()
 
     data_in.delete()
 
@@ -908,28 +910,30 @@
         progressbar=False,
         scheduler="processed",
         skip_ok=True,
     )
     for i in range(100):
         for index in range(6 * i, 6 * i + 6):
             np.testing.assert_array_equal(
-                ds.image[index].numpy(), 15 * i * np.ones((337, 200))
+                ds.image[index].numpy(),
+                np.asarray(15 * i * np.ones((337, 200)), dtype=np.uint8),
             )
             np.testing.assert_array_equal(
                 ds.label[index].numpy(), 15 * i * np.ones((1,))
             )
 
     assert len(ds.unused) == 0
 
     # test persistence
     ds = local_ds_generator()
     for i in range(100):
         for index in range(6 * i, 6 * i + 6):
             np.testing.assert_array_equal(
-                ds.image[index].numpy(), 15 * i * np.ones((337, 200))
+                ds.image[index].numpy(),
+                np.asarray(15 * i * np.ones((337, 200)), dtype=np.uint8),
             )
             np.testing.assert_array_equal(
                 ds.label[index].numpy(), 15 * i * np.ones((1,))
             )
     assert len(ds.unused) == 0
 
 
@@ -1238,7 +1242,252 @@
             (327, 521, 3),
             (163, 260, 3),
         ]
         for tensor, shape in zip(tensors, expected_shapes):
             assert len(ds[tensor]) == 10
             for i in range(10):
                 assert ds[tensor][i].shape == shape
+
+
+def test_rechunk_post_transform(local_ds):
+    with local_ds as ds:
+        ds.create_tensor("image", htype="image", sample_compression="jpg")
+        ds.create_tensor("label", htype="class_label")
+
+    fn1().eval(list(range(100)), ds, num_workers=4)
+
+    label_num_chunks = ds.label.chunk_engine.num_chunks
+
+    assert label_num_chunks == 1
+
+    image_num_chunks = ds.image.chunk_engine.num_chunks
+
+    assert image_num_chunks == 4
+
+
+def test_none_rechunk_post_transform(local_ds):
+    @deeplake.compute
+    def upload(stuff, ds):
+        ds.abc.append(None)
+
+    with local_ds as ds:
+        ds.create_tensor("abc")
+
+    upload().eval(list(range(100)), ds, num_workers=2)
+
+    num_chunks = ds.abc.chunk_engine.num_chunks
+
+    assert num_chunks == 2
+
+
+@pytest.mark.parametrize("scheduler", ["serial", "threaded", "processed"])
+def test_transform_checkpointing(local_ds, scheduler):
+    @deeplake.compute
+    def upload(i, ds):
+        if i == 45:
+            raise Exception("test")
+        ds.abc.append(i)
+
+    @deeplake.compute
+    def double(data_in, ds):
+        ds.abc.append(data_in.abc * 2)
+
+    data_in = list(range(100))
+
+    with local_ds as ds:
+        ds.create_tensor("abc")
+
+    # not divisible by num_workers
+    with pytest.raises(ValueError):
+        upload().eval(
+            data_in, ds, num_workers=2, scheduler=scheduler, checkpoint_interval=51
+        )
+
+    # greater than len(data_in)
+    with pytest.raises(ValueError):
+        upload().eval(
+            data_in, ds, num_workers=2, scheduler=scheduler, checkpoint_interval=102
+        )
+
+    # less than 10% of data_in, shows warning
+    with pytest.warns(UserWarning, match="10%"):
+        with pytest.raises(TransformError):
+            upload().eval(
+                data_in, ds, num_workers=2, scheduler=scheduler, checkpoint_interval=8
+            )
+
+    assert len(ds.abc) == 40
+    assert ds.abc.numpy(aslist=True) == list(range(40))
+    with pytest.raises(ValueError):
+        double().eval(ds, num_workers=2, scheduler=scheduler, checkpoint_interval=10)
+
+    # fix input data
+    data_in[45] = 0
+
+    upload().eval(
+        data_in[40:], ds, num_workers=2, scheduler=scheduler, checkpoint_interval=10
+    )
+    assert ds.abc.numpy(aslist=True) == data_in
+
+
+def create_test_ds(path):
+    ds = deeplake.empty(path, overwrite=True)
+    ds.create_tensor("images", htype="image", sample_compression="jpg")
+    ds.create_tensor("boxes", htype="bbox")
+    ds.create_tensor("labels", htype="class_label")
+    return ds
+
+
+class BadSample:
+    # will pass shape check in transform tensor
+    shape = (250, 250, 3)
+
+
+@all_schedulers
+@pytest.mark.parametrize("method", ["ds", "multiple"])
+@pytest.mark.parametrize("error_at", ["transform", "chunk_engine"])
+def test_ds_append_errors(
+    local_path, compressed_image_paths, scheduler, method, error_at
+):
+    @deeplake.compute
+    def upload(item, ds):
+        images = (
+            deeplake.read(item["images"])
+            if isinstance(item["images"], str)
+            else item["images"]
+        )
+        if method == "ds":
+            ds.append(
+                {
+                    "labels": np.zeros(10, dtype=np.uint32),
+                    "boxes": np.ones((len(item["boxes"]), 4), dtype=np.float32),
+                    "images": images,
+                }
+            )
+        elif method == "multiple":
+            # test rolling back multiple samples
+            ds.labels.append(np.zeros(10, dtype=np.uint32))
+            ds.boxes.append(np.ones((len(item["boxes"]), 4), dtype=np.float32))
+            ds.labels.append(np.zeros(10, dtype=np.uint32))
+            ds.boxes.append(np.ones((len(item["boxes"]), 4), dtype=np.float32))
+            ds.images.append(images)
+            ds.images.append(images)
+
+    ds = create_test_ds(local_path)
+
+    images = compressed_image_paths["jpeg"][:2]
+
+    samples = []
+    for i in range(20):
+        samples.append({"images": images[i % 2], "boxes": range(i + 1)})
+
+    if error_at == "transform":
+        # errors out in transform dataset / tensor
+        bad_sample = {"images": "bad_path", "boxes": [1, 2, 3]}
+        err_msg = re.escape(
+            f"Transform failed at index 17 of the input data on the item: {bad_sample}. See traceback for more details."
+        )
+    else:
+        # errors out in chunk engine
+        bad_sample = {"images": BadSample(), "boxes": [1, 2, 3]}
+        err_msg = re.escape(
+            f"Transform failed at index 17 of the input data. See traceback for more details."
+        )
+
+    samples.insert(17, bad_sample)
+
+    with pytest.raises(TransformError, match=err_msg) as e:
+        upload().eval(
+            samples,
+            ds,
+            num_workers=TRANSFORM_TEST_NUM_WORKERS,
+            scheduler=scheduler,
+        )
+
+    ds = create_test_ds(local_path)
+
+    upload().eval(
+        samples,
+        ds,
+        num_workers=TRANSFORM_TEST_NUM_WORKERS,
+        scheduler=scheduler,
+        ignore_errors=True,
+    )
+
+    if method == "ds":
+        assert ds["images"][::2].numpy().shape == (10, *deeplake.read(images[0]).shape)
+        assert ds["images"][1::2].numpy().shape == (10, *deeplake.read(images[1]).shape)
+
+        assert len(ds["boxes"]) == 20
+        assert ds["boxes"].meta.min_shape == [1, 4]
+        assert ds["boxes"].meta.max_shape == [20, 4]
+
+        assert ds["labels"].numpy().shape == (20, 10)
+    elif method == "multiple":
+        data = ds["images"]
+
+        images_0 = np.concatenate([data[i : i + 2].numpy() for i in range(0, 40, 4)])
+        image_0_shape = deeplake.read(images[0]).shape
+        assert images_0.shape == (20, *image_0_shape)
+
+        images_1 = np.concatenate([data[i : i + 2].numpy() for i in range(2, 40, 4)])
+        image_1_shape = deeplake.read(images[1]).shape
+        assert images_1.shape == (20, *image_1_shape)
+
+        assert len(ds["boxes"]) == 40
+        assert ds["boxes"].meta.min_shape == [1, 4]
+        assert ds["boxes"].meta.max_shape == [20, 4]
+
+        assert ds["labels"].numpy().shape == (40, 10)
+
+
+def test_transform_numpy_only(local_ds):
+    @deeplake.compute
+    def upload(i, ds):
+        ds.abc.extend(i * np.ones((10, 5, 5)))
+
+    with local_ds as ds:
+        ds.create_tensor("abc")
+
+        upload().eval(list(range(100)), ds, num_workers=2)
+
+    assert len(local_ds) == 1000
+
+    for i in range(100):
+        np.testing.assert_array_equal(
+            ds.abc[i * 10 : (i + 1) * 10].numpy(), i * np.ones((10, 5, 5))
+        )
+
+
+@deeplake.compute
+def add_samples(i, ds, flower_path):
+    ds.abc.extend(i * np.ones((5, 5, 5)))
+    ds.images.extend([deeplake.read(flower_path) for _ in range(5)])
+
+
+@deeplake.compute
+def mul_by_2(sample_in, samples_out):
+    samples_out.abc.append(2 * sample_in.abc.numpy())
+    samples_out.images.append(sample_in.images.numpy() - 1)
+
+
+def test_pipeline(local_ds, flower_path):
+    pipeline = deeplake.compose([add_samples(flower_path), mul_by_2()])
+
+    flower_arr = np.array(deeplake.read(flower_path))
+
+    with local_ds as ds:
+        ds.create_tensor("abc")
+        ds.create_tensor("images", htype="image", sample_compression="png")
+
+        pipeline.eval(list(range(10)), ds, num_workers=2)
+
+    assert len(local_ds) == 50
+
+    for i in range(10):
+        np.testing.assert_array_equal(
+            ds.abc[i * 5 : (i + 1) * 5].numpy(), i * 2 * np.ones((5, 5, 5))
+        )
+        np.testing.assert_array_equal(
+            ds.images[i * 5 : (i + 1) * 5].numpy(),
+            np.tile(flower_arr - 1, (5, 1, 1, 1)),
+        )
```

### Comparing `deeplake-3.2.9/deeplake/core/transform/transform.py` & `deeplake-3.3.0/deeplake/core/transform/transform.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from uuid import uuid4
 import deeplake
 from typing import Callable, List, Optional
 from itertools import repeat
-from deeplake.core.compute.provider import ComputeProvider
+from deeplake.core.compute.provider import ComputeProvider, get_progress_bar
 from deeplake.core.storage.memory import MemoryProvider
 from deeplake.util.bugout_reporter import deeplake_reporter
 from deeplake.util.compute import get_compute_provider
-from deeplake.util.dataset import try_flushing
-from deeplake.util.remove_cache import (
-    get_base_storage,
-    get_dataset_with_zero_size_cache,
-)
+from deeplake.util.remove_cache import get_base_storage
 from deeplake.util.transform import (
     check_lengths,
     check_transform_data_in,
     check_transform_ds_out,
+    close_states,
     create_slices,
     delete_overwritten_chunks,
     get_lengths_generated,
     get_old_chunk_paths,
     get_pbar_description,
+    prepare_data_in,
     process_transform_result,
+    reload_and_rechunk,
     sanitize_workers_scheduler,
     store_data_slice,
     store_data_slice_with_pbar,
+    check_checkpoint_interval,
 )
 from deeplake.util.encoder import merge_all_meta_info
 from deeplake.util.exceptions import (
     HubComposeEmptyListError,
     HubComposeIncompatibleFunction,
     TransformError,
 )
 from deeplake.hooks import dataset_written, dataset_read
-from deeplake.util.version_control import auto_checkout, load_meta
+from deeplake.util.version_control import auto_checkout
 from deeplake.util.class_label import sync_labels
-import sys
+
+import posixpath
 
 
 class ComputeFunction:
     def __init__(self, func, args, kwargs, name: Optional[str] = None):
         """Creates a ComputeFunction object that can be evaluated using .eval or used as a part of a Pipeline."""
         self.func = func
         self.args = args
@@ -52,14 +53,17 @@
         num_workers: int = 0,
         scheduler: str = "threaded",
         progressbar: bool = True,
         skip_ok: bool = False,
         check_lengths: bool = True,
         pad_data_in: bool = False,
         read_only_ok: bool = False,
+        cache_size: int = 16,
+        checkpoint_interval: int = 0,
+        ignore_errors: bool = False,
         **kwargs,
     ):
         """Evaluates the ComputeFunction on data_in to produce an output dataset ds_out.
 
         Args:
             data_in: Input passed to the transform to generate output dataset. Should support \__getitem__ and \__len__. Can be a Deep Lake dataset.
             ds_out (Dataset, optional): The dataset object to which the transform will get written. If this is not provided, data_in will be overwritten if it is a Deep Lake dataset, otherwise error will be raised.
@@ -73,34 +77,42 @@
             skip_ok (bool): If True, skips the check for output tensors generated. This allows the user to skip certain tensors in the function definition.
                 This is especially useful for inplace transformations in which certain tensors are not modified. Defaults to False.
             check_lengths (bool): If True, checks whether ds_out has tensors of same lengths initially.
             pad_data_in (bool): NOTE: This is only applicable if data_in is a Deep Lake dataset. If True, pads tensors of data_in to match the length of the largest tensor in data_in.
                 Defaults to False.
             read_only_ok (bool): If ``True`` and output dataset is same as input dataset, the read-only check is skipped. This can be used to read data in parallel without making changes to underlying dataset.
                 Defaults to False.
+            cache_size (int): Cache size to be used by transform per worker.
+            checkpoint_interval (int): If > 0, the transform will be checkpointed with a commit every ``checkpoint_interval`` input samples to avoid restarting full transform due to intermitten failures. If the transform is interrupted, the intermediate data is deleted and the dataset is reset to the last commit.
+                If <= 0, no checkpointing is done. Checkpoint interval should be a multiple of num_workers if num_workers > 0. Defaults to 0.
+            ignore_errors (bool): If ``True``, input samples that causes transform to fail will be skipped and the errors will be ignored **if possible**.
             **kwargs: Additional arguments.
 
         Raises:
             InvalidInputDataError: If data_in passed to transform is invalid. It should support \__getitem__ and \__len__ operations. Using scheduler other than "threaded" with deeplake dataset having base storage as memory as data_in will also raise this.
             InvalidOutputDatasetError: If all the tensors of ds_out passed to transform don't have the same length. Using scheduler other than "threaded" with deeplake dataset having base storage as memory as ds_out will also raise this.
             TensorMismatchError: If one or more of the outputs generated during transform contain different tensors than the ones present in 'ds_out' provided to transform.
             UnsupportedSchedulerError: If the scheduler passed is not recognized. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
+            ValueError: If ``num_workers`` > 0 and ``checkpoint_interval`` is not a multiple of ``num_workers`` or if ``checkpoint_interval`` > 0 and ds_out is None.
         """
 
         pipeline = Pipeline([self])
         pipeline.eval(
             data_in,
             ds_out,
             num_workers,
             scheduler,
             progressbar,
             skip_ok,
             check_lengths,
             pad_data_in,
             read_only_ok,
+            cache_size,
+            checkpoint_interval,
+            ignore_errors,
             **kwargs,
         )
 
     def __call__(self, sample_in):
         return self.func(sample_in, *self.args, **self.kwargs)
 
 
@@ -119,14 +131,17 @@
         num_workers: int = 0,
         scheduler: str = "threaded",
         progressbar: bool = True,
         skip_ok: bool = False,
         check_lengths: bool = True,
         pad_data_in: bool = False,
         read_only_ok: bool = False,
+        cache_size: int = 16,
+        checkpoint_interval: int = 0,
+        ignore_errors: bool = False,
         **kwargs,
     ):
         """Evaluates the pipeline on ``data_in`` to produce an output dataset ``ds_out``.
 
         Args:
             data_in: Input passed to the transform to generate output dataset. Should support \__getitem__ and \__len__. Can be a Deep Lake dataset.
             ds_out (Dataset, optional): - The dataset object to which the transform will get written. If this is not provided, ``data_in`` will be overwritten if it is a Deep Lake dataset, otherwise error will be raised.
@@ -140,22 +155,27 @@
             skip_ok (bool): If ``True``, skips the check for output tensors generated. This allows the user to skip certain tensors in the function definition.
                 This is especially useful for inplace transformations in which certain tensors are not modified. Defaults to ``False``.
             check_lengths (bool): If ``True``, checks whether ``ds_out`` has tensors of same lengths initially.
             pad_data_in (bool): If ``True``, pads tensors of ``data_in`` to match the length of the largest tensor in ``data_in``.
                 Defaults to ``False``.
             read_only_ok (bool): If ``True`` and output dataset is same as input dataset, the read-only check is skipped.
                 Defaults to False.
+            cache_size (int): Cache size to be used by transform per worker.
+            checkpoint_interval (int): If > 0, the transform will be checkpointed with a commit every ``checkpoint_interval`` input samples to avoid restarting full transform due to intermitten failures. If the transform is interrupted, the intermediate data is deleted and the dataset is reset to the last commit.
+                If <= 0, no checkpointing is done. Checkpoint interval should be a multiple of num_workers if num_workers > 0. Defaults to 0.
+            ignore_errors (bool): If ``True``, input samples that causes transform to fail will be skipped and the errors will be ignored **if possible**.
             **kwargs: Additional arguments.
 
         Raises:
             InvalidInputDataError: If ``data_in`` passed to transform is invalid. It should support \__getitem__ and \__len__ operations. Using scheduler other than "threaded" with deeplake dataset having base storage as memory as ``data_in`` will also raise this.
             InvalidOutputDatasetError: If all the tensors of ``ds_out`` passed to transform don't have the same length. Using scheduler other than "threaded" with deeplake dataset having base storage as memory as ``ds_out`` will also raise this.
             TensorMismatchError: If one or more of the outputs generated during transform contain different tensors than the ones present in 'ds_out' provided to transform.
             UnsupportedSchedulerError: If the scheduler passed is not recognized. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
             TransformError: All other exceptions raised if there are problems while running the pipeline.
+            ValueError: If ``num_workers`` > 0 and ``checkpoint_interval`` is not a multiple of ``num_workers`` or if ``checkpoint_interval`` > 0 and ds_out is None.
 
 
         # noqa: DAR401
 
         Example::
 
             @deeplake.compute
@@ -180,24 +200,17 @@
         overwrite = ds_out is None
         deeplake_reporter.feature_report(
             feature_name="eval",
             parameters={"Num_Workers": str(num_workers), "Scheduler": scheduler},
         )
         check_transform_data_in(data_in, scheduler)
 
-        if isinstance(data_in, deeplake.Dataset):
-            try_flushing(data_in)
-            if overwrite:
-                auto_checkout(data_in)
-            original_data_in = data_in
-            data_in = get_dataset_with_zero_size_cache(data_in)
-            if pad_data_in:
-                initial_padding_state = data_in._pad_tensors
-                data_in._enable_padding()
-
+        data_in, original_data_in, initial_padding_state = prepare_data_in(
+            data_in, pad_data_in, overwrite
+        )
         target_ds = data_in if overwrite else ds_out
 
         check_transform_ds_out(
             target_ds, scheduler, check_lengths, read_only_ok and overwrite
         )
 
         # if overwrite then we've already flushed and autocheckecked out data_in which is target_ds now
@@ -207,107 +220,162 @@
 
         compute_provider = get_compute_provider(scheduler, num_workers)
         compute_id = str(uuid4().hex)
         target_ds._send_compute_progress(compute_id=compute_id, start=True, progress=0)
 
         initial_autoflush = target_ds.storage.autoflush
         target_ds.storage.autoflush = False
-        progress_end_args = {"compute_id": compute_id, "progress": 100, "end": True}
 
-        if not check_lengths:
+        if not check_lengths or read_only_ok:
             skip_ok = True
 
-        try:
-            self.run(
-                data_in,
-                target_ds,
-                compute_provider,
-                num_workers,
-                scheduler,
-                progressbar,
-                overwrite,
-                skip_ok,
-                read_only_ok and overwrite,
-                **kwargs,
+        checkpointing_enabled = checkpoint_interval > 0
+        total_samples = len(data_in)
+        if checkpointing_enabled:
+            check_checkpoint_interval(
+                data_in, checkpoint_interval, num_workers, overwrite
             )
-            target_ds._send_compute_progress(**progress_end_args, status="success")
-        except Exception as e:
-            target_ds._send_compute_progress(**progress_end_args, status="failed")
-            raise TransformError(e).with_traceback(sys.exc_info()[2])
-        finally:
-            compute_provider.close()
-            if overwrite:
-                original_data_in.storage.clear_cache_without_flush()
-                load_meta(original_data_in)
-                if pad_data_in and not initial_padding_state:
-                    original_data_in._disable_padding()
-            else:
-                load_meta(target_ds)
-                target_ds.storage.autoflush = initial_autoflush
+            datas_in = [
+                data_in[i : i + checkpoint_interval]
+                for i in range(0, len(data_in), checkpoint_interval)
+            ]
+
+        else:
+            datas_in = [data_in]
+
+        samples_processed = 0
+        desc = get_pbar_description(self.functions)
+        if progressbar:
+            pbar = get_progress_bar(len(data_in), desc)
+            pqueue = compute_provider.create_queue()
+        else:
+            pbar, pqueue = None, None
+        desc = desc.split()[1]
+        completed = False
+        progress = 0.0
+        for data_in in datas_in:
+            if checkpointing_enabled and progress > 0:
+                target_ds.commit(
+                    f"Auto-commit during deeplake.compute of {desc} after {progress}% progress"
+                )
+            progress = round(
+                (samples_processed + len(data_in)) / total_samples * 100, 2
+            )
+            end = progress == 100
+            progress_args = {"compute_id": compute_id, "progress": progress, "end": end}
+
+            try:
+                self.run(
+                    data_in,
+                    target_ds,
+                    compute_provider,
+                    num_workers,
+                    scheduler,
+                    progressbar,
+                    overwrite,
+                    skip_ok,
+                    read_only_ok and overwrite,
+                    cache_size,
+                    pbar,
+                    pqueue,
+                    ignore_errors,
+                    **kwargs,
+                )
+                target_ds._send_compute_progress(**progress_args, status="success")
+                samples_processed += len(data_in)
+                completed = end
+            except Exception as e:
+                if checkpointing_enabled:
+                    print(
+                        "Transform failed. Resetting back to last committed checkpoint."
+                    )
+                    target_ds.reset(force=True)
+                target_ds._send_compute_progress(**progress_args, status="failed")
+                close_states(compute_provider, pbar, pqueue)
+                index, sample = None, None
+                if isinstance(e, TransformError):
+                    index, sample = e.index, e.sample
+                    e = e.__cause__  # type: ignore
+                raise TransformError(
+                    index=index,
+                    sample=sample,
+                    samples_processed=samples_processed,
+                ) from e
+            finally:
+                reload_and_rechunk(
+                    overwrite,
+                    original_data_in,
+                    target_ds,
+                    initial_autoflush,
+                    pad_data_in,
+                    initial_padding_state,
+                    kwargs,
+                    completed,
+                )
+
+        close_states(compute_provider, pbar, pqueue)
 
     def run(
         self,
         data_in,
         target_ds: deeplake.Dataset,
         compute: ComputeProvider,
         num_workers: int,
         scheduler: str,
         progressbar: bool = True,
         overwrite: bool = False,
         skip_ok: bool = False,
         read_only: bool = False,
+        cache_size: int = 16,
+        pbar=None,
+        pqueue=None,
+        ignore_errors: bool = False,
         **kwargs,
     ):
         """Runs the pipeline on the input data to produce output samples and stores in the dataset.
         This receives arguments processed and sanitized by the Pipeline.eval method.
         """
         if isinstance(data_in, deeplake.Dataset):
             dataset_read(data_in)
-        slices = create_slices(data_in, num_workers)
+        slices, offsets = create_slices(data_in, num_workers)
         storage = get_base_storage(target_ds.storage)
         class_label_tensors = (
             [
                 tensor.key
                 for tensor in target_ds.tensors.values()
                 if tensor.base_htype == "class_label"
                 and not read_only
                 and not tensor.meta._disable_temp_transform
             ]
             if not kwargs.get("disable_label_sync")
             else []
         )
         label_temp_tensors = {}
-        actual_tensors = (
-            None
-            if not class_label_tensors
-            else [target_ds[t].key for t in target_ds.tensors]
-        )
+
+        visible_tensors = list(target_ds.tensors)
+        visible_tensors = [target_ds[t].key for t in visible_tensors]
 
         if not read_only:
             for tensor in class_label_tensors:
                 actual_tensor = target_ds[tensor]
-                temp_tensor = f"__temp{tensor}_{uuid4().hex[:4]}"
+                temp_tensor = f"__temp{posixpath.relpath(tensor, target_ds.group_index)}_{uuid4().hex[:4]}"
                 with target_ds:
                     temp_tensor_obj = target_ds.create_tensor(
                         temp_tensor,
                         htype="class_label",
                         dtype=actual_tensor.dtype,
                         hidden=True,
                         create_sample_info_tensor=False,
                         create_shape_tensor=False,
                         create_id_tensor=False,
                     )
                     temp_tensor_obj.meta._disable_temp_transform = True
-                    label_temp_tensors[tensor] = temp_tensor
+                    label_temp_tensors[tensor] = temp_tensor_obj.key
                 target_ds.flush()
 
-        visible_tensors = list(target_ds.tensors)
-        visible_tensors = [target_ds[t].key for t in visible_tensors]
-        visible_tensors = list(set(visible_tensors) - set(class_label_tensors))
-
         tensors = list(target_ds._tensors())
         tensors = [target_ds[t].key for t in tensors]
         tensors = list(set(tensors) - set(class_label_tensors))
 
         group_index = target_ds.group_index
         version_state = target_ds.version_state
         if isinstance(storage, MemoryProvider):
@@ -316,37 +384,40 @@
             storages = [storage.copy() for _ in slices]
         extend_only = kwargs.get("extend_only")
         args = (
             group_index,
             tensors,
             visible_tensors,
             label_temp_tensors,
-            actual_tensors,
             self,
             version_state,
             target_ds.link_creds,
             skip_ok,
             extend_only,
+            cache_size,
+            ignore_errors,
         )
-        map_inp = zip(slices, storages, repeat(args))
+        map_inp = zip(slices, offsets, storages, repeat(args))
         try:
             if progressbar:
                 desc = get_pbar_description(self.functions)
-                result = compute.map_with_progressbar(
+                result = compute.map_with_progress_bar(
                     store_data_slice_with_pbar,
                     map_inp,
                     total_length=len(data_in),
                     desc=desc,
+                    pbar=pbar,
+                    pqueue=pqueue,
                 )
             else:
                 result = compute.map(store_data_slice, map_inp)
-        except Exception as e:
+        except Exception:
             for tensor in label_temp_tensors.values():
                 target_ds.delete_tensor(tensor)
-            raise e
+            raise
 
         if read_only:
             return
 
         result = process_transform_result(result)
 
         all_num_samples, all_tensors_generated_length = get_lengths_generated(
@@ -413,14 +484,16 @@
     - ``progressbar (bool)``: Displays a progress bar if True (default).
 
     - ``skip_ok (bool)``: If True, skips the check for output tensors generated.
 
         - This allows the user to skip certain tensors in the function definition.
         - This is especially useful for inplace transformations in which certain tensors are not modified. Defaults to ``False``.
 
+    - ``ignore_errors (bool)``: If ``True``, input samples that causes transform to fail will be skipped and the errors will be ignored **if possible**.
+
     It raises the following errors:
 
     - ``InvalidInputDataError``: If data_in passed to transform is invalid. It should support ``__getitem__`` and ``__len__`` operations. Using scheduler other than "threaded" with deeplake dataset having base storage as memory as data_in will also raise this.
 
     - ``InvalidOutputDatasetError``: If all the tensors of ds_out passed to transform don't have the same length. Using scheduler other than "threaded" with deeplake dataset having base storage as memory as ds_out will also raise this.
 
     - ``TensorMismatchError``: If one or more of the outputs generated during transform contain different tensors than the ones present in 'ds_out' provided to transform.
@@ -499,14 +572,16 @@
         - This allows the user to skip certain tensors in the function definition.
         - This is especially useful for inplace transformations in which certain tensors are not modified. Defaults to ``False``.
 
     - ``check_lengths (bool)``: If ``True``, checks whether ``ds_out`` has tensors of same lengths initially.
 
     - ``pad_data_in (bool)``: If ``True``, pads tensors of ``data_in`` to match the length of the largest tensor in ``data_in``. Defaults to ``False``.
 
+    - ``ignore_errors (bool)``: If ``True``, input samples that causes transform to fail will be skipped and the errors will be ignored **if possible**.
+
     Note:
         ``pad_data_in`` is only applicable if ``data_in`` is a Deep Lake dataset.
 
     It raises the following errors:
 
     - ``InvalidInputDataError``: If ``data_in`` passed to transform is invalid. It should support ``__getitem__`` and ``__len__`` operations. Using scheduler other than "threaded" with deeplake dataset having base storage as memory as ``data_in`` will also raise this.
```

### Comparing `deeplake-3.2.9/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.3.0/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/version_control/commit_diff.py` & `deeplake-3.3.0/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/version_control/commit_node.py` & `deeplake-3.3.0/deeplake/core/version_control/commit_node.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         self.branch = branch
         self.children: List["CommitNode"] = []
         self.parent: Optional["CommitNode"] = None
         self.commit_message: Optional[str] = None
         self.commit_time: Optional[datetime] = None
         self.commit_user_name: Optional[str] = None
         self.merge_parent: Optional["CommitNode"] = None
+        self._info_updated: bool = False
 
     def add_child(self, node: "CommitNode"):
         """Adds a child to the node, used for branching."""
         node.parent = self
         self.children.append(node)
 
     def copy(self):
@@ -50,7 +51,17 @@
 
     @property
     def is_head_node(self) -> bool:
         """Returns True if the node is the head node of the branch."""
         return self.commit_time is None
 
     __str__ = __repr__
+
+    def to_json(self):
+        return {
+            "branch": self.branch,
+            "children": [node.commit_id for node in self.children],
+            "parent": self.parent.commit_id if self.parent else None,
+            "commit_message": self.commit_message,
+            "commit_time": self.commit_time.timestamp() if self.commit_time else None,
+            "commit_user_name": self.commit_user_name,
+        }
```

### Comparing `deeplake-3.2.9/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.3.0/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/core/version_control/test_merge.py` & `deeplake-3.3.0/deeplake/core/version_control/test_merge.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pytest
 import deeplake
 
-from deeplake.util.testing import assert_array_equal
+from deeplake.util.testing import assert_array_equal, compare_version_info
+from deeplake.util.version_control import rebuild_version_info
 from deeplake.util.exceptions import (
     MergeConflictError,
     MergeMismatchError,
     MergeNotSupportedError,
 )
 
 
@@ -598,7 +599,27 @@
 
     abc.extend([half_chunk, half_chunk])
 
     assert get_chunks(abc, 0, 5) == ((0, 2), None, (4, 5))
     assert get_chunks(abc, 1, 6) == ((1, 3), (1, 2), None)
     assert get_chunks(abc, 1, 5) == ((1, 2), (1, 2), (4, 5))
     assert get_chunks(abc, 0, 6) == ((0, 3), None, None)
+
+
+def test_merge_with_padding(memory_ds):
+    with memory_ds as ds:
+        ds.create_tensor("x")
+        cid = ds.commit()
+        ds.checkout("branch1", create=True)
+        ds.x[100] = 2
+        for i in range(0, 100):
+            assert ds.x.chunk_engine.pad_encoder.is_padded(i), i
+        ds.x[200] = 3
+        ds.x[300] = 4
+        ds.checkout(cid)
+        ds.checkout("branch2", create=True)
+        ds.x[150] = 10
+        ds.x[250] = 20
+        ds.x[350] = 30
+        ds.checkout("branch1")
+        ds.merge("branch2")
+        assert len(ds.x) == 304
```

### Comparing `deeplake-3.2.9/deeplake/core/version_control/test_version_control.py` & `deeplake-3.3.0/deeplake/core/version_control/test_version_control.py`

 * *Files 4% similar despite different names*

```diff
@@ -685,15 +685,15 @@
     expected_dataset_diff = [expected_dataset_diff_from_a]
 
     compare_tensor_diff(tensor_diff, expected_tensor_diff)
     compare_dataset_diff(dataset_diff, expected_dataset_diff)
     target = get_diff_helper(dataset_diff, None, tensor_diff, None)
     local_ds.diff()
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     b = local_ds.commit()
     expected_tensor_diff_from_b = {
         "commit_id": local_ds.pending_commit_id,
         "xyz": get_default_tensor_diff(),
     }
     expected_dataset_diff_from_b = get_default_dataset_diff(local_ds.pending_commit_id)
@@ -723,21 +723,21 @@
         dataset_diff[1],
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         a,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     # cover DatasetDiff.frombuffer
     ds = deeplake.load(local_ds.path)
     ds.diff(a)
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
     diff = ds.diff(a, as_dict=True)
     tensor_diff = diff["tensor"]
     dataset_diff = diff["dataset"]
     compare_tensor_diff(tensor_diff[0], expected_tensor_diff[0])
     compare_tensor_diff(tensor_diff[1], expected_tensor_diff[1])
     compare_dataset_diff(dataset_diff[0], expected_dataset_diff[0])
     compare_dataset_diff(dataset_diff[1], expected_dataset_diff[1])
@@ -772,15 +772,15 @@
     assert tensor_diff == target_tensor_diff
     compare_dataset_diff(dataset_diff, target_dataset_diff)
 
     local_ds.diff()
     target = get_diff_helper(dataset_diff, None, tensor_diff, None)
 
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     a = local_ds.commit()
     expected_tensor_diff_from_a = {
         "commit_id": local_ds.pending_commit_id,
         "abc": get_default_tensor_diff(),
     }
 
@@ -817,15 +817,15 @@
         dataset_diff[1],
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         a,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     b = local_ds.commit()
     expected_tensor_diff_from_b = {
         "commit_id": local_ds.pending_commit_id,
         "abc": get_default_tensor_diff(),
         "xyz": get_default_tensor_diff(),
     }
@@ -869,15 +869,15 @@
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         c,
         a,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
 
 def test_delete_diff(local_ds, capsys):
     local_ds.create_tensor("x/y/z")
     local_ds["x/y/z"].append([4, 5, 6])
     a = local_ds.commit()
     expected_tensor_diff_from_a = {
@@ -939,15 +939,15 @@
         dataset_diff[1],
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         a,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     d = local_ds.commit()
     expected_tensor_diff_from_d = {
         "commit_id": local_ds.pending_commit_id,
         "x/y/z": get_default_tensor_diff(),
     }
     expected_dataset_diff_from_d = get_default_dataset_diff(local_ds.pending_commit_id)
@@ -999,15 +999,15 @@
         dataset_diff[1],
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         c,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     diff = local_ds.diff(a, as_dict=True)
     tensor_diff = diff["tensor"]
     dataset_diff = diff["dataset"]
 
     expected_tensor_diff = (
         [
@@ -1041,15 +1041,15 @@
         dataset_diff[1],
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         a,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     diff = local_ds.diff(as_dict=True)
     tensor_diff = diff["tensor"]
     dataset_diff = diff["dataset"]
 
     expected_tensor_diff = [expected_tensor_diff_from_e]
     expected_dataset_diff = [expected_dataset_diff_from_e]
@@ -1090,15 +1090,15 @@
 
     compare_tensor_diff(tensor_diff, expected_tensor_diff)
     compare_dataset_diff(dataset_diff, expected_dataset_diff)
 
     local_ds.diff()
     target = get_diff_helper(dataset_diff, None, tensor_diff, None)
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     a = local_ds.commit()
     expected_tensor_diff_from_a = {
         "commit_id": local_ds.pending_commit_id,
         "efg": get_default_tensor_diff(),
         "red": get_default_tensor_diff(),
     }
@@ -1143,15 +1143,15 @@
         dataset_diff[1],
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         a,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
 
 def test_rename_diff_linear(local_ds, capsys):
     with local_ds:
         local_ds.create_tensor("abc")
         local_ds.abc.append([1, 2, 3])
         local_ds.create_tensor("xyz")
@@ -1225,15 +1225,15 @@
         dataset_diff[1],
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         a,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     c = local_ds.commit()
     expected_tensor_diff_from_c = {
         "commit_id": local_ds.pending_commit_id,
         "abc": get_default_tensor_diff(),
         "xyz": get_default_tensor_diff(),
         "blue": get_default_tensor_diff(),
@@ -1282,15 +1282,15 @@
         dataset_diff[1],
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         a,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     d = local_ds.commit()
     expected_tensor_diff_from_d = {
         "commit_id": local_ds.pending_commit_id,
         "bcd": get_default_tensor_diff(),
         "abc": get_default_tensor_diff(),
     }
@@ -1338,15 +1338,15 @@
         dataset_diff[1],
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         b,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     e = local_ds.commit()
     expected_tensor_diff_from_e = {
         "commit_id": local_ds.pending_commit_id,
         "bcd": get_default_tensor_diff(),
     }
     expected_dataset_diff_from_e = get_default_dataset_diff(local_ds.pending_commit_id)
@@ -1391,15 +1391,15 @@
         dataset_diff[1],
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         a,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
 
 def test_rename_diff_branch(local_ds, capsys):
     with local_ds:
         local_ds.create_tensor("abc")
         local_ds.abc.append([1, 2, 3])
 
@@ -1515,15 +1515,15 @@
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         b,
         e,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
 
 def test_rename_group(local_ds, capsys):
     with local_ds:
         local_ds.create_tensor("g1/g2/g3/t1")
         local_ds.create_tensor("g1/g2/t2")
         a = local_ds.commit()
@@ -1554,15 +1554,15 @@
 
     compare_tensor_diff(tensor_diff, expected_tensor_diff)
     compare_dataset_diff(dataset_diff, expected_dataset_diff)
 
     local_ds.diff()
     target = get_diff_helper(dataset_diff, None, tensor_diff, None)
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
 
 def test_diff_linear(local_ds, capsys):
     with local_ds:
         local_ds.create_tensor("xyz")
         local_ds.xyz.extend([1, 2, 3])
         local_ds.create_tensor("pqr")
@@ -1598,15 +1598,15 @@
 
     compare_tensor_diff(tensor_diff, expected_tensor_diff)
     compare_dataset_diff(dataset_diff, expected_dataset_diff)
 
     local_ds.diff()
     target = get_diff_helper(dataset_diff, None, tensor_diff, None)
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     b = local_ds.commit()
     expected_tensor_diff_from_b = {
         "commit_id": local_ds.pending_commit_id,
         "xyz": get_default_tensor_diff(),
         "pqr": get_default_tensor_diff(),
         "abc": get_default_tensor_diff(),
@@ -1621,15 +1621,15 @@
     expected_dataset_diff = [expected_dataset_diff_from_b]
     compare_tensor_diff(tensor_diff, expected_tensor_diff)
     compare_dataset_diff(dataset_diff, expected_dataset_diff)
 
     local_ds.diff()
     target = get_diff_helper(dataset_diff, None, tensor_diff, None)
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     diff = local_ds.diff(a, as_dict=True)
     tensor_diff = diff["tensor"]
     dataset_diff = diff["dataset"]
     expected_tensor_diff = [
         [expected_tensor_diff_from_b, expected_tensor_diff_from_a],
         [],
@@ -1650,15 +1650,15 @@
         dataset_diff[1],
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         a,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     diff = local_ds.diff(b, as_dict=True)
     tensor_diff = diff["tensor"]
     dataset_diff = diff["dataset"]
     expected_tensor_diff = [[expected_tensor_diff_from_b], []]
     expected_dataset_diff = [[expected_dataset_diff_from_b], []]
 
@@ -1675,15 +1675,15 @@
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         b,
     )
 
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     diff = local_ds.diff(a, b, as_dict=True)
     tensor_diff = diff["tensor"]
     dataset_diff = diff["dataset"]
     expected_tensor_diff = [[], [expected_tensor_diff_from_a]]
     expected_dataset_diff = [[], [expected_dataset_diff_from_a]]
 
@@ -1699,15 +1699,15 @@
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         a,
         b,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     diff = local_ds.diff(b, a, as_dict=True)
     tensor_diff = diff["tensor"]
     dataset_diff = diff["dataset"]
     expected_tensor_diff = [[expected_tensor_diff_from_a], []]
     expected_dataset_diff = [[expected_dataset_diff_from_a], []]
 
@@ -1723,15 +1723,15 @@
         tensor_diff[0],
         tensor_diff[1],
         local_ds.version_state,
         b,
         a,
     )
     captured = capsys.readouterr()
-    assert captured.out == target
+    assert captured.out.strip() == target.strip()
 
     local_ds.checkout(b)
     diff = local_ds.diff(as_dict=True)
     tensor_diff = diff["tensor"]
     dataset_diff = diff["dataset"]
     expected_tensor_diff = [expected_tensor_diff_from_a]
     expected_dataset_diff = [expected_dataset_diff_from_a]
@@ -2381,7 +2381,58 @@
 
 def test_reset_delete_group(local_ds):
     with local_ds as ds:
         ds.create_tensor("abc/x")
         ds.commit()
         ds.delete_group("abc")
         assert ds.has_head_changes
+
+
+def test_load_to_version(local_path):
+    with deeplake.empty(local_path, overwrite=True) as ds:
+        ds.create_tensor("abc")
+        ds.abc.append(1)
+        main_1 = ds.commit()
+        ds.create_tensor("xyz")
+        main_2 = ds.commit()
+
+        ds.checkout("alt", create=True)
+        ds.abc.append(2)
+        alt_1 = ds.commit()
+        ds.xyz.append(1)
+        ds.xyz.append(2)
+        alt_2 = ds.commit()
+
+    ds = deeplake.load(f"{local_path}@{main_1}")
+    set(ds.tensors.keys()) == {"abc"}
+    np.testing.assert_array_equal(ds.abc.numpy(), [[1]])
+
+    for address in ("main", main_2):
+        ds = deeplake.load(f"{local_path}@{address}")
+        set(ds.tensors.keys()) == {"abc", "xyz"}
+        np.testing.assert_array_equal(ds.abc.numpy(), [[1]])
+        np.testing.assert_array_equal(ds.xyz.numpy(), [])
+
+    ds = deeplake.load(f"{local_path}@{alt_1}")
+    set(ds.tensors.keys()) == {"abc", "xyz"}
+    np.testing.assert_array_equal(ds.abc.numpy(), [[1], [2]])
+    np.testing.assert_array_equal(ds.xyz.numpy(), [])
+
+    for address in ("alt", alt_2):
+        ds = deeplake.load(f"{local_path}@{address}")
+        set(ds.tensors.keys()) == {"abc", "xyz"}
+        np.testing.assert_array_equal(ds.abc.numpy(), [[1], [2]])
+        np.testing.assert_array_equal(ds.xyz.numpy(), [[1], [2]])
+
+
+def test_version_in_path(local_path):
+    with pytest.raises(ValueError):
+        deeplake.empty(f"{local_path}@main")
+
+    with pytest.raises(ValueError):
+        deeplake.delete(f"{local_path}@main")
+
+    with pytest.raises(ValueError):
+        deeplake.dataset(f"{local_path}@main")
+
+    with pytest.raises(ValueError):
+        deeplake.exists(f"{local_path}@main")
```

### Comparing `deeplake-3.2.9/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.3.0/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
             raise ValueError("Gdrive datasets are not supported for libdeeplake")
         elif path.startswith("mem://"):
             raise ValueError("In memory datasets are not supported for libdeeplake")
         elif path.startswith("hub://"):
             token = hub2_dataset._token
             provider = hub2_dataset.storage.next_storage
             if isinstance(provider, S3Provider):
+                provider._check_update_creds()
                 libdeeplake_dataset = api.dataset(
                     path,
                     origin_path=provider.root,
                     token=token,
                     aws_access_key_id=provider.aws_access_key_id,
                     aws_secret_access_key=provider.aws_secret_access_key,
                     aws_session_token=provider.aws_session_token,
```

### Comparing `deeplake-3.2.9/deeplake/enterprise/dataloader.py` & `deeplake-3.3.0/deeplake/enterprise/dataloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Callable, Dict, List, Optional, Union
-from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake  # type: ignore
+import deeplake
+from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake
+from deeplake.enterprise.dummy_dataloader import DummyDataloader  # type: ignore
 from deeplake.util.scheduling import create_fetching_schedule, find_primary_tensor
 from deeplake.enterprise.util import (
     handle_mode,
     raise_indra_installation_error,
     verify_base_storage,
     get_collate_fn,
 )
@@ -26,14 +28,27 @@
     _InfiniteConstantSampler = None  # type: ignore
     DistributedSampler = None  # type: ignore
 
 import numpy as np
 
 import math
 
+import itertools
+
+original_islice = itertools.islice
+
+
+def deeplake_islice(iterable, *args, **kwargs):
+    if isinstance(iterable, DeepLakeDataLoader):
+        return iter(iterable)
+    return original_islice(iterable, *args, **kwargs)
+
+
+itertools.islice = deeplake_islice  # type: ignore
+
 
 # Load lazy to avoid cycylic import.
 INDRA_LOADER = None
 
 
 def indra_available() -> bool:
     try:
@@ -52,15 +67,17 @@
     try:
         from indra import api  # type: ignore
         from indra.pytorch.loader import Loader  # type:ignore
 
         INDRA_LOADER = Loader
         return Loader
     except Exception as e:
-        raise_indra_installation_error(e)
+        if not deeplake.constants.RETURN_DUMMY_DATA_FOR_DATALOADER:
+            raise_indra_installation_error(e)
+        INDRA_LOADER = None
 
 
 class DeepLakeDataLoader(DataLoader):
     def __init__(
         self,
         dataset,
         _batch_size=None,
@@ -561,41 +578,75 @@
             collate_fn = self.collate_fn
             upcast = self._mode == "pytorch"  # upcast to handle unsupported dtypes
 
             primary_tensor_name = self._primary_tensor_name
             buffer_size = self._buffer_size
 
             tensors = self._tensors or map_tensor_keys(self._orig_dataset, None)
-            dataset = dataset_to_libdeeplake(self._orig_dataset)
 
-            jpeg_png_compressed_tensors = check_tensors(self._orig_dataset, tensors)
-            raw_tensors, compressed_tensors = validate_decode_method(
-                self._decode_method, tensors, jpeg_png_compressed_tensors
+            jpeg_png_compressed_tensors, json_tensors, list_tensors = check_tensors(
+                self._orig_dataset, tensors
             )
-            raw_tensors.extend(compressed_tensors)
-            self._dataloader = INDRA_LOADER(
-                dataset,
-                batch_size=self._batch_size,
-                num_threads=self._num_threads,
-                shuffle=self._shuffle,
-                num_workers=self._num_workers,
-                collate_fn=collate_fn,
-                transform_fn=self._transform,
-                distributed=self._distributed,
-                prefetch_factor=self._prefetch_factor,
-                tensors=tensors,
-                drop_last=self._drop_last,
-                upcast=upcast,
-                return_index=self._return_index,
-                primary_tensor=primary_tensor_name,
-                buffer_size=buffer_size,
-                raw_tensors=raw_tensors,
-                compressed_tensors=compressed_tensors,
-                persistent_workers=self._persistent_workers,
+            (
+                raw_tensors,
+                pil_compressed_tensors,
+                json_tensors,
+                list_tensors,
+            ) = validate_decode_method(
+                self._decode_method,
+                tensors,
+                jpeg_png_compressed_tensors,
+                json_tensors,
+                list_tensors,
             )
+            if deeplake.constants.RETURN_DUMMY_DATA_FOR_DATALOADER:
+                self._dataloader = DummyDataloader(
+                    deeplake_dataset=self._orig_dataset,
+                    batch_size=self._batch_size,
+                    shuffle=self._shuffle,
+                    num_workers=self._num_workers,
+                    collate_fn=collate_fn,
+                    transform_fn=self._transform,
+                    distributed=self._distributed,
+                    prefetch_factor=self._prefetch_factor,
+                    tensors=tensors,
+                    drop_last=self._drop_last,
+                    upcast=upcast,
+                    return_index=self._return_index,
+                    raw_tensors=raw_tensors,
+                    pil_compressed_tensors=pil_compressed_tensors,
+                    persistent_workers=self._persistent_workers,
+                )
+            else:
+                if not hasattr(self, "_indra_dataset"):
+                    indra_dataset = dataset_to_libdeeplake(self._orig_dataset)
+                else:
+                    indra_dataset = self._indra_dataset
+                self._dataloader = INDRA_LOADER(
+                    indra_dataset,
+                    batch_size=self._batch_size,
+                    num_threads=self._num_threads,
+                    shuffle=self._shuffle,
+                    num_workers=self._num_workers,
+                    collate_fn=collate_fn,
+                    transform_fn=self._transform,
+                    distributed=self._distributed,
+                    prefetch_factor=self._prefetch_factor,
+                    tensors=tensors,
+                    drop_last=self._drop_last,
+                    upcast=upcast,
+                    return_index=self._return_index,
+                    primary_tensor=primary_tensor_name,
+                    buffer_size=buffer_size,
+                    raw_tensors=raw_tensors,
+                    pil_compressed_tensors=pil_compressed_tensors,
+                    json_tensors=json_tensors,
+                    list_tensors=list_tensors,
+                    persistent_workers=self._persistent_workers,
+                )
         dataset_read(self._orig_dataset)
         return iter(self._dataloader)
 
 
 def dataloader(dataset) -> DeepLakeDataLoader:
     """Returns a :class:`~deeplake.enterprise.dataloader.DeepLakeDataLoader` object which can be transformed to either pytorch dataloader or numpy.
```

### Comparing `deeplake-3.2.9/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.3.0/deeplake/enterprise/libdeeplake_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake
 from deeplake.util.bugout_reporter import deeplake_reporter
+from deeplake.core.dataset.deeplake_query_dataset import DeepLakeQueryDataset
 from typing import Optional, Union
 
 import numpy as np
 
 
 @deeplake_reporter.record_call
 def query(dataset, query_string: str):
@@ -31,18 +32,28 @@
         >>> query_ds_train = query(ds_train, "select * where labels != 5")
 
         Query from dataset first appeard ``1000`` samples where the ``categories`` is ``car`` and ``1000`` samples where the ``categories`` is ``motorcycle``
 
         >>> ds_train = deeplake.load('hub://activeloop/coco-train')
         >>> query_ds_train = query(ds_train, "(select * where contains(categories, 'car') limit 1000) union (select * where contains(categories, 'motorcycle') limit 1000)")
     """
-    ds = dataset_to_libdeeplake(dataset)
+    if isinstance(dataset, DeepLakeQueryDataset):
+        ds = dataset.indra_ds
+    else:
+        ds = dataset_to_libdeeplake(dataset)
     dsv = ds.query(query_string)
-    indexes = dsv.indexes
-    return dataset[indexes]
+    try:
+        indexes = dsv.indexes
+        return dataset[indexes]
+    except RuntimeError:
+        view = DeepLakeQueryDataset(deeplake_ds=dataset, indra_ds=dsv)
+        view._tql_query = query_string
+        if hasattr(dataset, "is_actually_cloud"):
+            view.is_actually_cloud = dataset.is_actually_cloud
+        return view
 
 
 @deeplake_reporter.record_call
 def sample_by(
     dataset,
     weights: Union[str, list, tuple, np.ndarray],
     replace: Optional[bool] = True,
```

### Comparing `deeplake-3.2.9/deeplake/enterprise/test_pytorch.py` & `deeplake-3.3.0/deeplake/enterprise/test_pytorch.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,22 +13,29 @@
 from PIL import Image  # type: ignore
 
 try:
     from torch.utils.data._utils.collate import default_collate
 except ImportError:
     pass
 
+from unittest.mock import patch
+
+
 # ensure tests have multiple chunks without a ton of data
 PYTORCH_TESTS_MAX_CHUNK_SIZE = 5 * KB
 
 
 def double(sample):
     return sample * 2
 
 
+def identity_collate(batch):
+    return batch
+
+
 def to_tuple(sample, t1, t2):
     return sample[t1], sample[t2]
 
 
 def reorder_collate(batch):
     x = [((x["a"], x["b"]), x["c"]) for x in batch]
     return default_collate(x)
@@ -122,23 +129,22 @@
         )
         hub_cloud_ds.image2.extend(np.array([i * np.ones((12, 12)) for i in range(16)]))
 
     dl = (
         hub_cloud_ds.dataloader()
         .batch(1)
         .transform(to_tuple, t1="image", t2="image2")
-        .pytorch(num_workers=2)
+        .pytorch(num_workers=2, collate_fn=identity_collate)
     )
 
     for _ in range(2):
         for i, batch in enumerate(dl):
-            actual_image = batch[0].numpy()
-            expected_image = i * np.ones((1, i + 1, i + 1))
-            actual_image2 = batch[1].numpy()
-            expected_image2 = i * np.ones((1, 12, 12))
+            actual_image, actual_image2 = batch[0]
+            expected_image = i * np.ones((i + 1, i + 1))
+            expected_image2 = i * np.ones((12, 12))
             np.testing.assert_array_equal(actual_image, expected_image)
             np.testing.assert_array_equal(actual_image2, expected_image2)
 
 
 @requires_torch
 @requires_libdeeplake
 def test_pytorch_transform_dict(hub_cloud_ds):
@@ -254,15 +260,20 @@
     hub_cloud_ds.create_tensor("labels", max_chunk_size=PYTORCH_TESTS_MAX_CHUNK_SIZE)
     hub_cloud_ds.images.extend(np.ones((10, 12, 12)))
     hub_cloud_ds.labels.extend(np.ones(10))
 
     base_storage = get_base_storage(hub_cloud_ds.storage)
     base_storage.flush()
     base_storage.enable_readonly()
-    ds = Dataset(storage=hub_cloud_ds.storage, read_only=True, verbose=False)
+    ds = Dataset(
+        storage=hub_cloud_ds.storage,
+        token=hub_cloud_ds.token,
+        read_only=True,
+        verbose=False,
+    )
 
     ptds = ds.dataloader().pytorch(num_workers=2)
     # no need to check input, only care that readonly works
     for _ in ptds:
         pass
 
 
@@ -288,24 +299,24 @@
         hub_cloud_ds.create_tensor(
             "images/pngs/flowers", htype="image", sample_compression="png"
         )
         for _ in range(10):
             hub_cloud_ds.images.jpegs.cats.append(img1)
             hub_cloud_ds.images.pngs.flowers.append(img2)
 
-    another_ds = deeplake.dataset(hub_cloud_ds.path)
+    another_ds = deeplake.dataset(hub_cloud_ds.path, token=hub_cloud_ds.token)
     dl = another_ds.dataloader().pytorch(return_index=False)
     for i, (cat, flower) in enumerate(dl):
         assert cat[0].shape == another_ds.images.jpegs.cats[i].numpy().shape
         assert flower[0].shape == another_ds.images.pngs.flowers[i].numpy().shape
 
     dl = another_ds.images.dataloader().pytorch(return_index=False)
     for sample in dl:
-        cat = sample["jpegs/cats"]
-        flower = sample["pngs/flowers"]
+        cat = sample["images/jpegs/cats"]
+        flower = sample["images/pngs/flowers"]
         np.testing.assert_array_equal(cat[0], img1.array)
         np.testing.assert_array_equal(flower[0], img2.array)
 
 
 @requires_torch
 @requires_libdeeplake
 def test_string_tensors(hub_cloud_ds):
@@ -531,20 +542,17 @@
         .transform(index_transform)
         .pytorch(num_workers=num_workers, return_index=True)
     )
     if shuffle:
         ptds = ptds.shuffle()
 
     for batch in ptds:
-        assert len(batch) == 2
-        assert len(batch[0]) == 4
-        assert len(batch[1]) == 4
-
-        for i in range(4):
-            np.testing.assert_array_equal(batch[0][i], batch[1][i][0, 0])
+        assert len(batch) == 4
+        assert len(batch[0]) == 2
+        assert len(batch[1]) == 2
 
 
 @requires_torch
 @requires_libdeeplake
 @pytest.mark.parametrize("num_workers", [0, 2])
 def test_indexes_transform_dict(hub_cloud_ds, num_workers):
     shuffle = False
@@ -643,7 +651,121 @@
     with pytest.raises(EmptyTensorError):
         for _ in ptds:
             pass
 
     ptds = ds.dataloader().pytorch(tensors=["x"])
     for _ in ptds:
         pass
+
+
+@requires_libdeeplake
+@requires_torch
+def test_pil_decode_method(hub_cloud_ds):
+    with hub_cloud_ds as ds:
+        ds.create_tensor("x", htype="image", sample_compression="jpeg")
+        ds.x.extend(np.random.randint(0, 255, (10, 10, 10, 3), np.uint8))
+
+    ptds = ds.dataloader().pytorch(return_index=False)
+    for batch in ptds:
+        assert len(batch.keys()) == 1
+        assert "x" in batch.keys()
+        assert batch["x"].shape == (1, 10, 10, 3)
+
+    ptds = ds.dataloader().pytorch(decode_method={"x": "pil"})
+    with pytest.raises(TypeError):
+        for _ in ptds:
+            pass
+
+    def custom_transform(batch):
+        batch["x"] = np.array(batch["x"])
+        return batch
+
+    ptds = (
+        ds.dataloader()
+        .pytorch(decode_method={"x": "pil"}, return_index=False)
+        .transform(custom_transform)
+    )
+    for batch in ptds:
+        assert len(batch.keys()) == 1
+        assert "x" in batch.keys()
+        assert batch["x"].shape == (1, 10, 10, 3)
+
+
+@patch("deeplake.constants.RETURN_DUMMY_DATA_FOR_DATALOADER", True)
+@requires_torch
+@requires_libdeeplake
+def test_pytorch_dummy_data(local_ds):
+    x_data = [
+        np.random.randint(0, 255, (100, 100, 3), dtype="uint8"),
+        np.random.randint(0, 255, (120, 120, 3), dtype="uint8"),
+    ]
+    y_data = [np.random.rand(100, 100, 3), np.random.rand(120, 120, 3)]
+    z_data = ["hello", "world"]
+    with local_ds as ds:
+        ds.create_tensor("x")
+        ds.create_tensor("y")
+        ds.create_tensor("z")
+        ds.x.extend(x_data)
+        ds.y.extend(y_data)
+        ds.z.extend(z_data)
+
+    ptds = ds.dataloader()
+    for i, batch in enumerate(ptds):
+        x = x_data[i]
+        dummy_x = batch[0]["x"]
+        assert dummy_x.shape == x.shape
+        assert dummy_x.dtype == x.dtype
+
+        y = y_data[i]
+        dummy_y = batch[0]["y"]
+        assert dummy_y.shape == y.shape
+        assert dummy_y.dtype == y.dtype
+
+        dummy_z = batch[0]["z"]
+        assert dummy_z[0] == "a"
+
+
+@requires_libdeeplake
+@requires_torch
+def test_json_data_loader(hub_cloud_ds):
+    ds = hub_cloud_ds
+    with ds:
+        ds.create_tensor(
+            "json",
+            htype="json",
+            sample_compression=None,
+        )
+        d = {"x": 1, "y": 2, "z": 3}
+        for _ in range(10):
+            ds.json.append(d)
+
+    dl = ds.dataloader().batch(2)
+
+    for batch in dl:
+        sample1 = batch[0]["json"]
+        sample2 = batch[1]["json"]
+
+        assert sample1 == d
+        assert sample2 == d
+
+
+@requires_libdeeplake
+@requires_torch
+def test_list_data_loader(hub_cloud_ds):
+    ds = hub_cloud_ds
+    with ds:
+        ds.create_tensor(
+            "list",
+            htype="list",
+            sample_compression=None,
+        )
+        l = [1, 2, 3]
+        for _ in range(10):
+            ds.list.append(l)
+
+    dl = ds.dataloader().batch(2)
+
+    for batch in dl:
+        sample1 = batch[0]["list"]
+        sample2 = batch[1]["list"]
+        assert sample1.tolist() == l
+        assert sample2.tolist() == l
```

### Comparing `deeplake-3.2.9/deeplake/enterprise/test_query.py` & `deeplake-3.3.0/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.3.0/deeplake/enterprise/test_tensorflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     return sample * 2
 
 
 def to_tuple(sample, t1, t2):
     return sample[t1], sample[t2]
 
 
+def identity_collate(batch):
+    return batch
+
+
 def reorder_collate(batch):
     x = [((x["a"], x["b"]), x["c"]) for x in batch]
     return default_collate(x)
 
 
 def dict_to_list(sample):
     return [sample["a"], sample["b"], sample["c"]]
@@ -280,15 +284,20 @@
     hub_cloud_ds.create_tensor("labels", max_chunk_size=TF_TESTS_MAX_CHUNK_SIZE)
     hub_cloud_ds.images.extend(np.ones((10, 12, 12)))
     hub_cloud_ds.labels.extend(np.ones(10))
 
     base_storage = get_base_storage(hub_cloud_ds.storage)
     base_storage.flush()
     base_storage.enable_readonly()
-    ds = Dataset(storage=hub_cloud_ds.storage, read_only=True, verbose=False)
+    ds = Dataset(
+        storage=hub_cloud_ds.storage,
+        token=hub_cloud_ds.token,
+        read_only=True,
+        verbose=False,
+    )
 
     ptds = ds.dataloader().tensorflow(num_workers=2)
     # no need to check input, only care that readonly works
     for _ in ptds:
         pass
 
 
@@ -314,38 +323,41 @@
         hub_cloud_ds.create_tensor(
             "images/pngs/flowers", htype="image", sample_compression="png"
         )
         for _ in range(10):
             hub_cloud_ds.images.jpegs.cats.append(img1)
             hub_cloud_ds.images.pngs.flowers.append(img2)
 
-    another_ds = deeplake.dataset(hub_cloud_ds.path)
+    another_ds = deeplake.dataset(
+        hub_cloud_ds.path,
+        token=hub_cloud_ds.token,
+    )
     dl = another_ds.dataloader().tensorflow(return_index=False)
     for i, (cat, flower) in enumerate(dl):
         assert cat[0].shape == another_ds.images.jpegs.cats[i].numpy().shape
         assert flower[0].shape == another_ds.images.pngs.flowers[i].numpy().shape
 
     dl = another_ds.images.dataloader().tensorflow(return_index=False)
     for sample in dl:
-        cat = sample["jpegs/cats"]
-        flower = sample["pngs/flowers"]
+        cat = sample["images/jpegs/cats"]
+        flower = sample["images/pngs/flowers"]
         np.testing.assert_array_equal(cat[0], img1.array)
         np.testing.assert_array_equal(flower[0], img2.array)
 
 
 @requires_tensorflow
 @requires_libdeeplake
 def test_string_tensors(hub_cloud_ds):
     with hub_cloud_ds:
         hub_cloud_ds.create_tensor("strings", htype="text")
         hub_cloud_ds.strings.extend([f"string{idx}" for idx in range(5)])
 
-    ptds = hub_cloud_ds.dataloader().tensorflow()
+    ptds = hub_cloud_ds.dataloader().tensorflow(collate_fn=identity_collate)
     for idx, batch in enumerate(ptds):
-        np.testing.assert_array_equal(batch["strings"], f"string{idx}")
+        np.testing.assert_array_equal(batch[0]["strings"], f"string{idx}")
 
 
 @pytest.mark.xfail(raises=NotImplementedError, strict=True)
 def test_tensorflow_large():
     raise NotImplementedError
 
 
@@ -463,18 +475,20 @@
     if isinstance(
         get_base_storage(hub_cloud_ds.storage), (MemoryProvider, GCSProvider)
     ):
         with pytest.raises(ValueError):
             dl = hub_cloud_ds.dataloader()
         return
 
-    ptds = hub_cloud_ds.dataloader().tensorflow(decode_method={"image": "tobytes"})
+    ptds = hub_cloud_ds.dataloader().tensorflow(
+        collate_fn=identity_collate, decode_method={"image": "tobytes"}
+    )
 
     for i, batch in enumerate(ptds):
-        image = batch["image"][0]
+        image = batch[0]["image"]
         assert isinstance(image, bytes)
         if i < 5 and not compression:
             np.testing.assert_array_equal(
                 np.frombuffer(image, dtype=np.uint8).reshape(10, 10, 3),
                 i * np.ones((10, 10, 3), dtype=np.uint8),
             )
         elif i >= 5 and compression:
```

### Comparing `deeplake-3.2.9/deeplake/enterprise/util.py` & `deeplake-3.3.0/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/hooks.py` & `deeplake-3.3.0/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/htype.py` & `deeplake-3.3.0/deeplake/htype.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     AUDIO = "audio"
     TEXT = "text"
     JSON = "json"
     LIST = "list"
     DICOM = "dicom"
     NIFTI = "nifti"
     POINT_CLOUD = "point_cloud"
-    POINT_CLOUD_CALIBRATION_MATRIX = "point_cloud.calibration_matrix"
+    INTRINSICS = "intrinsics"
     POLYGON = "polygon"
     MESH = "mesh"
 
 
 # used for requiring the user to specify a value for htype properties. notates that the htype property has no default.
 REQUIRE_USER_SPECIFICATION = "require_user_specification"
 
@@ -43,14 +43,16 @@
 UNSPECIFIED = "unspecified"
 
 
 HTYPE_CONFIGURATIONS: Dict[str, Dict] = {
     htype.DEFAULT: {"dtype": None},
     htype.IMAGE: {
         "dtype": "uint8",
+        "intrinsics": None,
+        "_info": ["intrinsics"],
     },
     htype.IMAGE_RGB: {
         "dtype": "uint8",
     },
     htype.IMAGE_GRAY: {
         "dtype": "uint8",
     },
@@ -69,31 +71,40 @@
     },  # TODO: pack numpy arrays to store bools as 1 bit instead of 1 byte
     htype.INSTANCE_LABEL: {"dtype": "uint32"},
     htype.SEGMENT_MASK: {
         "dtype": "uint32",
         "class_names": [],
         "_info": ["class_names"],
     },
-    htype.KEYPOINTS_COCO: {"dtype": "int32"},
+    htype.KEYPOINTS_COCO: {
+        "dtype": "int32",
+        "keypoints": [],
+        "connections": [],
+        "_info": [
+            "keypoints",
+            "connections",
+        ],  # keypoints and connections should be stored in info, not meta
+    },
     htype.POINT: {"dtype": "int32"},
     htype.JSON: {
         "dtype": "Any",
     },
     htype.LIST: {"dtype": "List"},
     htype.TEXT: {"dtype": "str"},
     htype.DICOM: {"sample_compression": "dcm"},
     htype.NIFTI: {},
     htype.POINT_CLOUD: {"dtype": "float32"},
-    htype.POINT_CLOUD_CALIBRATION_MATRIX: {"dtype": "float32"},
+    htype.INTRINSICS: {"dtype": "float32"},
     htype.POLYGON: {"dtype": "float32"},
     htype.MESH: {"sample_compression": "ply"},
 }
 
 HTYPE_VERIFICATIONS: Dict[str, Dict] = {
-    htype.BBOX: {"coords": {"type": dict, "keys": ["type", "mode"]}}
+    htype.BBOX: {"coords": {"type": dict, "keys": ["type", "mode"]}},
+    htype.BBOX_3D: {"coords": {"type": dict, "keys": ["mode"]}},
 }
 
 _image_compressions = (
     IMAGE_COMPRESSIONS[:] + BYTE_COMPRESSIONS + list(COMPRESSION_ALIASES)
 )
 _image_compressions.remove("dcm")
 
@@ -140,10 +151,10 @@
     htype_verifications = HTYPE_VERIFICATIONS.get(htype, {})
     if key in htype_verifications:
         expected_type = htype_verifications[key].get("type")
         if expected_type and not isinstance(value, expected_type):
             raise TypeError(f"{key} must be of type {expected_type}, not {type(value)}")
         if expected_type == dict:
             expected_keys = set(htype_verifications[key].get("keys"))
-            present_keys = set(value.keys())
+            present_keys = set(value)
             if expected_keys and not present_keys.issubset(expected_keys):
                 raise KeyError(f"{key} must have keys belong to {expected_keys}")
```

### Comparing `deeplake-3.2.9/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.3.0/deeplake/integrations/mmdet/mmdet_.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,190 +1,191 @@
 """
 Deep Lake offers an integration with MMDetection, a popular open-source object detection toolbox based on PyTorch. 
 The integration enables users to train models while streaming Deep Lake dataset using the transformation, training, and evaluation tools built by MMDet.
 
-Learn more about MMDetection `here <https://mmsegmentation.readthedocs.io/en/latest/>`_.
+Learn more about MMDetection `here <https://mmdetection.readthedocs.io/en/latest/>`_.
 
 Integration Interface
 ~~~~~~~~~~~~~~~~~~~~~
-MMDetection works with configs. Deeplake adopted the strategy, and in order to train MMDet models, you need to create/specify your model and training/validation config. 
-Deeplake integration's logic is almost the same as MMDetection's with some minor modifications. The integrations with MMDET occurs in the deeplake.integrations.mmdet module. 
-At a high-level, Deep Lake is responsible for the pytorch dataloader that streams data to the training framework, while MMDET is used for the training, transformation, and evaluation logic. Let us take a look at the config with deeplake changes:
+MMDetection works with configs. Deeplake adopted this strategy, and in order to train MMDet models, you need to create/specify your model 
+and training/validation config. Deep Lake integration's logic is almost the same as MMDetection's with some minor modifications. The integrations 
+with MMDET occurs in the deeplake.integrations.mmdet module. At a high-level, Deep Lake is responsible for the pytorch dataloader that streams data 
+to the training framework, while MMDET is used for the training, transformation, and evaluation logic. Let us take a look at the config with deeplake changes:
 
 Deeplake integration requires the following parameters to be specified in the configuration file:
-- data: just like in the MMDetection configuration files, in data dictionary you can specify everything that you want to be applied to the data during training and validation
-    - train: is the keyword argument of data, and also a dictionary where one can specify dataset path, credentials, transformations of the training data
-    - val: is the keyword argument of data, and also a dictionary where one can specify dataset path, credentials, transformations of the validation data
-    - pipeline: list of transformations. This parameter exists for train as well as for val.
-    Example:
+
+- ``data``: Just like in the MMDetection configuration files, in data dictionary you can specify everything that you want to be applied to the data during training and validation
+    - ``train``: Keyword argument of data, a dictionary where one can specify dataset path, credentials, transformations of the training data
+    - ``val``: Keyword argument of data, a dictionary where one can specify dataset path, credentials, transformations of the validation data
+    - ``pipeline``: List of transformations. This parameter exists for train as well as for val.
+    
+        - Example:
     
->>>    pipeline =  [dict(type="Resize", img_scale=[(320, 320), (608, 608)], keep_ratio=True), dict(type="RandomFlip", flip_ratio=0.5), dict(type="PhotoMetricDistortion")]
+            >>> pipeline =  [dict(type="Resize", img_scale=[(320, 320), (608, 608)], keep_ratio=True), dict(type="RandomFlip", flip_ratio=0.5), dict(type="PhotoMetricDistortion")]
 
-    - deeplake_path: path to the deeplake dataset. This parameter exists for train as well as for val.
-    - deeplake_credentials: optional parameter. Required only when using private nonlocal datasets. See documendataion for `deeplake.load() <https://docs.deeplake.ai/en/latest/deeplake.html#deeplake.load>`_ for details. This parameter exists for train as well as for val.
-    - deeplake_commit_id: optional parameter. If specified, the dataset will checkout to the commit. This parameter exists for train as well as for val. See documentation for `Dataset.commit_id <https://deep-lake--2152.org.readthedocs.build/en/2152/deeplake.core.dataset.html#deeplake.core.dataset.Dataset.commit_id>`_
-    - deeplake_view_id: optional parameter. If specified the dataset will load saved view. This parameter exists for train as well as for val.
-    - deeplake_tensors: optional parameter. If specified maps MMDetection tensors to the associated tensors in the dataset. MMDet tensors are: "img", "gt_bboxes", "gt_labels", "gt_masks". This parameter exists for train as well as for val.
-        - "img": stands for image tensor.
-        - "gt_bboxes": stands for bounding box tensor.
-        - "gt_labels": stand for labels tensor.
-        - "gt_masks": stand for masks tensor.
-    - deeplake_dataloader: optional parameter. If specified represents the parameters of the deeplake dataloader. Deeplake dataloader parameters are: "shuffle", "batch_size", "num_workers". This parameter exists for train as well as for val.
-        - "shuffle": if True shuffles the dataset.
-        - "batch_size": size of batch. If not specified, dataloader will use samples_per_gpu.
-        - "num_workers": number of workers to use. If not specified, dataloader will use workers_per_gpu.
-- deeplake_dataloader_type: optional parameter. If specified represents the type of deeplake dataloader to use.
-- deeplake_metrics_format: optional parameter. If specified represents the format of the deeplake metrics that will be used during evaluation. Default COCO. Avaliable values are: "COCO", "PascalVOC". 
-  If COCO format is used, you can specify whether you want to evaluate on bbox only or also want to evaluate on masks. To do that you need to specify the format of the metric in metric. 
+    - ``deeplake_path``: Path to the deeplake dataset. This parameter exists for train as well as for val.
+    - ``deeplake_credentials``: Optional parameter. Required only when using private nonlocal datasets. See documendataion for `deeplake.load() <https://docs.deeplake.ai/en/latest/deeplake.html#deeplake.load>`_ for details. This parameter exists for train as well as for val.
+    - ``deeplake_commit_id``: Optional parameter. If specified, the dataset will checkout to the commit. This parameter exists for train as well as for val. See documentation for `Dataset.commit_id <https://deep-lake--2152.org.readthedocs.build/en/2152/deeplake.core.dataset.html#deeplake.core.dataset.Dataset.commit_id>`_
+    - ``deeplake_view_id``: Optional parameter. If specified the dataset will load saved view. This parameter exists for train as well as for val.
+    - ``deeplake_tensors``: Optional parameter. If specified maps MMDetection tensors to the associated tensors in the dataset. MMDet tensors are: "img", "gt_bboxes", "gt_labels", "gt_masks". This parameter exists for train as well as for val.
+        - ``"img"``: Stands for image tensor.
+        - ``"gt_bboxes"``: Stands for bounding box tensor.
+        - ``"gt_labels"``: Stands for labels tensor.
+        - ``"gt_masks"``: Stands for masks tensor.
+
+    - ``deeplake_dataloader``: Optional parameter. If specified represents the parameters of the deeplake dataloader. Deeplake dataloader parameters are: "shuffle", "batch_size", "num_workers". This parameter exists for train as well as for val.
+        - ``"shuffle"``: If ``True`` shuffles the dataset.
+        - ``"batch_size"``: Size of batch. If not specified, dataloader will use ``samples_per_gpu``.
+        - ``"num_workers"``: Number of workers to use. If not specified, dataloader will use ``workers_per_gpu``.
+
+- ``deeplake_dataloader_type``: Optional parameter. If specified, it represents the type of deeplake dataloader to use.
+- ``deeplake_metrics_format``: Optional parameter. If specified, it represents the format of the deeplake metrics that will be used during evaluation. Defaults to COCO. 
+    Avaliable values are: "COCO", "PascalVOC". If COCO format is used, you can specify whether you want to evaluate on bbox only or also want to evaluate on masks. 
+    To do that you need to specify the format of the metric in metric. 
   
-Ex:
+Example:
+
+>>> deeplake_metrics_format = "COCO"
+>>> evaluation = dict(metric=["bbox"], interval=1)
+
+- ``train_detector``: Function to train the MMDetection model.
 
->>>  deeplake_metrics_format = "COCO"
->>>  evaluation = dict(metric=["bbox"], interval=1)
+    Parameters:
 
-- train_detector: Function to train the MMDetection model. Parameters are: model, cfg: mmcv.ConfigDict, ds_train=None, ds_train_tensors=None, ds_val: Optional[dp.Dataset] = None, ds_val_tensors=None, distributed: bool = False, timestamp=None, meta=None, validate: bool = True.
-    - model: MMDetection model that is going to be used.
-    - cfg: Configuration of the model as well as of the datasets and transforms that's going to be used.
-    - ds_train: Optional parameter. If provided will overwrite deeplake_path in train, and will pass this tensor directly to the dataloader.
-    - ds_val: Optional parameter. If provided will overwrite deeplake_path in val, and will pass this tensor directly to the dataloader.
-    - ds_train_tensors: Optional parameter. If provided will overwrite deeplake_tensors in train, and will pass this tensor mapping directly to dataloader.
-    - ds_val_tensors: Optional parameter. If provided will overwrite deeplake_tensors in val, and will pass this tensor mapping directly to dataloader.
-    - distributed: Optional parameter. If provided will run the code on all available gpus. Meta data used to build runner
-    - timestamp: variable used in runner to make .log and .log.json filenames the same.'
-    - validate: bool, whether validation should be conducted, by default True
+        - ``model``: MMDetection model that is going to be used.
+        - ``cfg``: mmcv.ConfigDict, Configuration of the model as well as of the datasets and transforms that's going to be used.
+        - ``ds_train``: Optional parameter. If provided will overwrite deeplake_path in train, and will pass this tensor directly to the dataloader.
+        - ``ds_val``: Optional parameter. If provided will overwrite deeplake_path in val, and will pass this tensor directly to the dataloader.
+        - ``ds_train_tensors``: Optional parameter. If provided will overwrite deeplake_tensors in train, and will pass this tensor mapping directly to dataloader.
+        - ``ds_val_tensors``: Optional parameter. If provided will overwrite deeplake_tensors in val, and will pass this tensor mapping directly to dataloader.
+        - ``distributed``: Optional parameter. If provided will run the code on all available gpus. Meta data used to build runner.
+        - ``timestamp``: Variable used in runner to make .log and .log.json filenames the same.
+        - ``validate``: Bool, whether validation should be run, defaults to ``True``.
 
 NOTE:
-    gt_masks is optional parameter and lets say you want to train pure detecter this part is going to exclude. Other mappings are mandatory
-    if you don't specify them explicitly they are going to be searched in the dataset according to tensor htype. Better to specify them explicitly
+    ``gt_masks`` is optional parameter and lets say you want to train pure detector this part is going to exclude. Other mappings are mandatory
+    if you don't specify them explicitly they are going to be searched in the dataset according to tensor htype. Better to specify them explicitly.
 
 MMDetection Config Examples
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Below is the example of the deeplake mmdet configuration:
 
 
 >>> _base_ = "../mmdetection/configs/yolo/yolov3_d53_mstrain-416_273e_coco.py"
->>> 
 >>> # use caffe img_norm
 >>> img_norm_cfg = dict(mean=[0, 0, 0], std=[255., 255., 255.], to_rgb=True)
->>> 
 >>> train_pipeline = [
->>>     dict(type='LoadImageFromFile'),
->>>     dict(type='LoadAnnotations', with_bbox=True),
->>>     dict(
->>>         type='Expand',
->>>         mean=img_norm_cfg['mean'],
->>>         to_rgb=img_norm_cfg['to_rgb'],
->>>         ratio_range=(1, 2)),
->>>     dict(type='Resize', img_scale=[(320, 320), (416, 416)], keep_ratio=True),
->>>     dict(type='RandomFlip', flip_ratio=0.0),
->>>     dict(type='PhotoMetricDistortion'),
->>>     dict(type='Normalize', **img_norm_cfg),
->>>     dict(type='Pad', size_divisor=32),
->>>     dict(type='DefaultFormatBundle'),
->>>     dict(type='Collect', keys=['img', 'gt_bboxes', 'gt_labels'])
->>> ]
+...     dict(type='LoadImageFromFile'),
+...     dict(type='LoadAnnotations', with_bbox=True),
+...     dict(
+...         type='Expand',
+...         mean=img_norm_cfg['mean'],
+...         to_rgb=img_norm_cfg['to_rgb'],
+...         ratio_range=(1, 2)),
+...     dict(type='Resize', img_scale=[(320, 320), (416, 416)], keep_ratio=True),
+...     dict(type='RandomFlip', flip_ratio=0.0),
+...     dict(type='PhotoMetricDistortion'),
+...     dict(type='Normalize', **img_norm_cfg),
+...     dict(type='Pad', size_divisor=32),
+...     dict(type='DefaultFormatBundle'),
+...     dict(type='Collect', keys=['img', 'gt_bboxes', 'gt_labels'])
+... ]
 >>> test_pipeline = [
->>>     dict(type='LoadImageFromFile'),
->>>     dict(
->>>         type='MultiScaleFlipAug',
->>>         img_scale=(416, 416),
->>>         flip=False,
->>>         transforms=[
->>>             dict(type='Resize', keep_ratio=True),
->>>             dict(type='RandomFlip', flip_ratio=0.0),
->>>             dict(type='Normalize', **img_norm_cfg),
->>>             dict(type='Pad', size_divisor=32),
->>>             dict(type='ImageToTensor', keys=['img']),
->>>             dict(type='Collect', keys=['img'])
->>>         ])
->>> ]
+...     dict(type='LoadImageFromFile'),
+...     dict(
+...         type='MultiScaleFlipAug',
+...         img_scale=(416, 416),
+...         flip=False,
+...         transforms=[
+...             dict(type='Resize', keep_ratio=True),
+...             dict(type='RandomFlip', flip_ratio=0.0),
+...             dict(type='Normalize', **img_norm_cfg),
+...             dict(type='Pad', size_divisor=32),
+...             dict(type='ImageToTensor', keys=['img']),
+...             dict(type='Collect', keys=['img'])
+...         ])
+... ]
 >>> #--------------------------------------DEEPLAKE INPUTS------------------------------------------------------------#
->>> TOKEN = "INSERT_YOUR_DEEPLAKE_TOKEN"
-​>>> 
->>> 
+>>> TOKEN = "INSERT_YOUR_DEEPLAKE_TOKEN" 
 >>> data = dict(
->>>     # samples_per_gpu=4, # Is used instead of batch_size if deeplake_dataloader is not specified below
->>>     # workers_per_gpu=8, # Is used instead of num_workers if deeplake_dataloader is not specified below
->>>     train=dict(
->>>         pipeline=train_pipeline,
-​>>> 
->>>         # Credentials for authentication. See documendataion for deeplake.load() for details
->>>         deeplake_path="hub://activeloop/coco-train",
->>>         deeplake_credentials={
->>>             "username": None,
->>>             "password": None,
->>>             "token": TOKEN,
->>>             "creds": None,
->>>         },
->>>         #OPTIONAL - Checkout the specified commit_id before training
->>>         deeplake_commit_id="",
->>>         #OPTIONAL - Loads a dataset view for training based on view_id
->>>         deeplake_view_id="",
-​
->>>         # OPTIONAL - {"mmdet_key": "deep_lake_tensor",...} - Maps Deep Lake tensors to MMDET dictionary keys. 
->>>         # If not specified, Deep Lake will auto-infer the mapping, but it might make mistakes if datasets have many tensors
->>>         deeplake_tensors = {"img": "images", "gt_bboxes": "boxes", "gt_labels": "categories", "gt_masks": "masks},
->>>         
->>>         # OPTIONAL - Parameters to use for the Deep Lake dataloader. If unspecified, the integration uses
->>>         # the parameters in other parts of the cfg file such as samples_per_gpu, and others.
->>>         deeplake_dataloader = {"shuffle": True, "batch_size": 4, 'num_workers': 8}
->>>     ),
->>> ​
->>>     # Parameters as the same as for train
->>>     val=dict(
->>>         pipeline=test_pipeline,
->>>         deeplake_path="hub://activeloop/coco-val",
->>>         deeplake_credentials={
->>>             "username": None,
->>>             "password": None,
->>>             "token": TOKEN,
->>>             "creds": None,
->>>         },
->>>         deeplake_tensors = {"img": "images", "gt_bboxes": "boxes", "gt_labels": "categories"},
->>>         deeplake_dataloader = {"shuffle": False, "batch_size": 1, 'num_workers': 8}
->>>     ),
->>> )
-​>>> 
+...     # samples_per_gpu=4, # Is used instead of batch_size if deeplake_dataloader is not specified below
+...     # workers_per_gpu=8, # Is used instead of num_workers if deeplake_dataloader is not specified below
+...     train=dict(
+...         pipeline=train_pipeline,
+...         # Credentials for authentication. See documendataion for deeplake.load() for details
+...         deeplake_path="hub://activeloop/coco-train",
+...          deeplake_credentials={
+...             "username": None,
+...             "password": None,
+...             "token": TOKEN,
+...             "creds": None,
+...         },
+...         #OPTIONAL - Checkout the specified commit_id before training
+...         deeplake_commit_id="",
+...         #OPTIONAL - Loads a dataset view for training based on view_id
+...         deeplake_view_id="",
+...         # OPTIONAL - {"mmdet_key": "deep_lake_tensor",...} - Maps Deep Lake tensors to MMDET dictionary keys. 
+...         # If not specified, Deep Lake will auto-infer the mapping, but it might make mistakes if datasets have many tensors
+...         deeplake_tensors = {"img": "images", "gt_bboxes": "boxes", "gt_labels": "categories", "gt_masks": "masks},         
+...         # OPTIONAL - Parameters to use for the Deep Lake dataloader. If unspecified, the integration uses
+...         # the parameters in other parts of the cfg file such as samples_per_gpu, and others.
+...         deeplake_dataloader = {"shuffle": True, "batch_size": 4, 'num_workers': 8}
+...     ),
+...     # Parameters as the same as for train
+...     val=dict(
+...         pipeline=test_pipeline,
+...         deeplake_path="hub://activeloop/coco-val",
+...         deeplake_credentials={
+...             "username": None,
+...             "password": None,
+...             "token": TOKEN,
+...             "creds": None,
+...         },
+...         deeplake_tensors = {"img": "images", "gt_bboxes": "boxes", "gt_labels": "categories"},
+...         deeplake_dataloader = {"shuffle": False, "batch_size": 1, 'num_workers': 8}
+...     ),
+... )
 >>> # Which dataloader to use
 >>> deeplake_dataloader_type = "c++"  # "c++" is available to enterprise users. Otherwise use "python"
-​
 >>> # Which metrics to use for evaulation. In MMDET (without Deeplake), this is inferred from the dataset type.
 >>> # In the Deep Lake integration, since the format is standardized, a variety of metrics can be used for a given dataset.
 >>> deeplake_metrics_format = "COCO"
-​
 >>> #----------------------------------END DEEPLAKE INPUTS------------------------------------------------------------#
 
 And config for training:
 
 >>> import os
 >>> from mmcv import Config
 >>> import mmcv
 >>> from deeplake.integrations import mmdet as mmdet_deeplake
->>> 
->>> 
 >>> cfg = Config.fromfile(cfg_file)
->>> 
 >>> cfg.model.bbox_head.num_classes = num_classes
->>> 
 >>> # Build the detector
 >>> model = mmdet_deeplake.build_detector(cfg.model)
->>> 
 >>> # Create work_dir
 >>> mmcv.mkdir_or_exist(os.path.abspath(cfg.work_dir))
->>> 
 >>> # Run the training
 >>> mmdet_deeplake.train_detector(model, cfg, distributed=args.distributed, validate=args.validate)
 """
 
 
 from collections import OrderedDict
 
 from typing import Callable, Optional, List, Dict
 
-from mmdet.apis.train import auto_scale_lr  # type: ignore
+
+try:
+    from mmdet.apis.train import auto_scale_lr  # type: ignore
+except Exception:
+    import mmdet  # type: ignore
+
+    version = mmdet.__version__
+    raise Exception(
+        f"MMDet {version} version is not supported. The latest supported MMDet version with deeplake is 2.28.1."
+    )
 from mmdet.utils import (  # type: ignore
     build_dp,
     compat_cfg,
     find_latest_checkpoint,
     get_root_logger,
 )
 from mmdet.core import DistEvalHook, EvalHook  # type: ignore
@@ -225,14 +226,15 @@
 from deeplake.integrations.mmdet import mmdet_utils
 from deeplake.enterprise.dataloader import indra_available, dataloader
 from PIL import Image, ImageDraw  # type: ignore
 import os
 from mmdet.core import BitmapMasks, PolygonMasks
 import math
 import types
+from deeplake.integrations.mmdet.mmdet_runners import DeeplakeIterBasedRunner
 
 
 class Dummy:
     sampler = None
 
 
 def force_cudnn_initialization(device_id):
@@ -475,48 +477,60 @@
         self,
         *args,
         tensors_dict=None,
         mode="train",
         metrics_format="COCO",
         bbox_info=None,
         pipeline=None,
+        num_gpus=1,
+        batch_size=1,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
-        self.bbox_info = bbox_info
-        self.images = self._get_images(tensors_dict["images_tensor"])
-        self.masks = self._get_masks(tensors_dict.get("masks_tensor", None))
-        self.bboxes = self._get_bboxes(tensors_dict["boxes_tensor"])
-        bbox_format = get_bbox_format(first_non_empty(self.bboxes), bbox_info)
-        self.labels = self._get_labels(tensors_dict["labels_tensor"])
-        self.iscrowds = self._get_iscrowds(tensors_dict.get("iscrowds"))
-        self.CLASSES = self.get_classes(tensors_dict["labels_tensor"])
         self.mode = mode
-        self.metrics_format = metrics_format
-        coco_style_bbox = convert_to_coco_format(self.bboxes, bbox_format, self.images)
         self.pipeline = pipeline
-
-        if self.metrics_format == "COCO" and self.mode in ("val", "test"):
-            self.evaluator = mmdet_utils.COCODatasetEvaluater(
-                pipeline,
-                classes=self.CLASSES,
-                deeplake_dataset=self.dataset,
-                imgs=self.images,
-                masks=self.masks,
-                bboxes=coco_style_bbox,
-                labels=self.labels,
-                iscrowds=self.iscrowds,
-                bbox_format=bbox_format,
+        self.num_gpus = num_gpus
+        self.batch_size = batch_size
+        if self.mode in ("val", "test"):
+            self.bbox_info = bbox_info
+            self.images = self._get_images(tensors_dict["images_tensor"])
+            self.masks = self._get_masks(tensors_dict.get("masks_tensor", None))
+            self.bboxes = self._get_bboxes(tensors_dict["boxes_tensor"])
+            bbox_format = get_bbox_format(first_non_empty(self.bboxes), bbox_info)
+            self.labels = self._get_labels(tensors_dict["labels_tensor"])
+            self.iscrowds = self._get_iscrowds(tensors_dict.get("iscrowds"))
+            self.CLASSES = self.get_classes(tensors_dict["labels_tensor"])
+            self.metrics_format = metrics_format
+            coco_style_bbox = convert_to_coco_format(
+                self.bboxes, bbox_format, self.images
             )
-        else:
-            self.evaluator = None
+
+            if self.metrics_format == "COCO":
+                self.evaluator = mmdet_utils.COCODatasetEvaluater(
+                    pipeline,
+                    classes=self.CLASSES,
+                    deeplake_dataset=self.dataset,
+                    imgs=self.images,
+                    masks=self.masks,
+                    bboxes=coco_style_bbox,
+                    labels=self.labels,
+                    iscrowds=self.iscrowds,
+                    bbox_format=bbox_format,
+                    num_gpus=num_gpus,
+                )
+            else:
+                self.evaluator = None
 
     def __len__(self):
-        if self.mode == "eval":
-            return math.ceil(len(self.dataset) / self.batch_size)
+        if self.mode == "val":
+            per_gpu_length = math.floor(
+                len(self.dataset) / (self.batch_size * self.num_gpus)
+            )
+            total_length = per_gpu_length * self.num_gpus
+            return total_length
         return super().__len__()
 
     def _get_images(self, images_tensor):
         image_tensor = self.dataset[images_tensor]
         return image_tensor
 
     def _get_masks(self, masks_tensor):
@@ -624,14 +638,20 @@
 
         Raises:
             KeyError: if a specified metric format is not supported
 
         Returns:
             OrderedDict: Evaluation metrics dictionary
         """
+        if self.num_gpus > 1:
+            results_ordered = []
+            for i in range(self.num_gpus):
+                results_ordered += results[i :: self.num_gpus]
+            results = results_ordered
+
         if self.evaluator is None:
             if not isinstance(metric, str):
                 assert len(metric) == 1
                 metric = metric[0]
             allowed_metrics = ["mAP", "recall"]
             if metric not in allowed_metrics:
                 raise KeyError(f"metric {metric} is not supported")
@@ -667,15 +687,19 @@
                 if recalls.shape[1] > 1:
                     ar = recalls.mean(axis=1)
                     for i, num in enumerate(proposal_nums):
                         eval_results[f"AR@{num}"] = ar[i]
             return eval_results
 
         return self.evaluator.evaluate(
-            results, metric=metric, logger=logger, proposal_nums=proposal_nums, **kwargs
+            results,
+            metric=metric,
+            logger=logger,
+            proposal_nums=proposal_nums,
+            **kwargs,
         )
 
     @staticmethod
     def _coco_2_pascal(boxes):
         # Convert bounding boxes to Pascal VOC format and clip bounding boxes to make sure they have non-negative width and height
         return np.stack(
             (
@@ -975,14 +999,16 @@
             metrics_format=metrics_format,
             pipeline=pipeline,
             tensors_dict=tensors_dict,
             tensors=tensors,
             mode=mode,
             bbox_info=bbox_info,
             decode_method=decode_method,
+            num_gpus=train_loader_config["num_gpus"],
+            batch_size=batch_size,
         )
 
         loader.dataset.mmdet_dataset = mmdet_ds
         loader.dataset.pipeline = loader.dataset.mmdet_dataset.pipeline
         loader.dataset.evaluate = types.MethodType(
             mmdet_subiterable_dataset_eval, loader.dataset
         )
@@ -1007,14 +1033,16 @@
             metrics_format=metrics_format,
             pipeline=pipeline,
             tensors_dict=tensors_dict,
             tensors=tensors,
             mode=mode,
             bbox_info=bbox_info,
             decode_method=decode_method,
+            num_gpus=train_loader_config["num_gpus"],
+            batch_size=batch_size,
         )
         loader.dataset = mmdet_ds
     loader.dataset.CLASSES = classes
     return loader
 
 
 def build_pipeline(steps):
@@ -1211,17 +1239,19 @@
             train_masks_tensor = _find_tensor_with_htype(
                 ds_train, "binary_mask", "gt_masks"
             ) or _find_tensor_with_htype(ds_train, "polygon", "gt_masks")
 
     # TODO verify required tensors are not None and raise Exception.
 
     if hasattr(model, "CLASSES"):
-        warnings.warn("model already has a CLASSES attribute. Will be ignored.")
-
-    model.CLASSES = ds_train[train_labels_tensor].info.class_names
+        warnings.warn(
+            "model already has a CLASSES attribute. dataset.info.class_names will not be used."
+        )
+    elif hasattr(ds_train[train_labels_tensor].info, "class_names"):
+        model.CLASSES = ds_train[train_labels_tensor].info.class_names
 
     metrics_format = cfg.get("deeplake_metrics_format", "COCO")
 
     logger = get_root_logger(log_level=cfg.log_level)
 
     runner_type = "EpochBasedRunner" if "runner" not in cfg else cfg.runner["type"]
 
@@ -1275,14 +1305,23 @@
         implementation=dl_impl,
         **train_loader_cfg,
     )
     # build optimizer
     auto_scale_lr(cfg, distributed, logger)
     optimizer = build_optimizer(model, cfg.optimizer)
 
+    cfg.custom_imports = dict(
+        imports=["deeplake.integrations.mmdet.mmdet_runners"],
+        allow_failed_imports=False,
+    )
+    if cfg.runner.type == "IterBasedRunner":
+        cfg.runner.type = "DeeplakeIterBasedRunner"
+    elif cfg.runner.type == "EpochBasedRunner":
+        cfg.runner.type = "DeeplakeEpochBasedRunner"
+
     runner = build_runner(
         cfg.runner,
         default_args=dict(
             model=model,
             optimizer=optimizer,
             work_dir=cfg.work_dir,
             logger=logger,
@@ -1317,21 +1356,22 @@
     if distributed:
         if isinstance(runner, EpochBasedRunner):
             runner.register_hook(DistSamplerSeedHook())
 
     # register eval hooks
     if validate:
         val_dataloader_default_args = dict(
-            samples_per_gpu=1,
-            workers_per_gpu=1,
-            dist=False,
+            samples_per_gpu=batch_size,
+            workers_per_gpu=num_workers,
+            dist=distributed,
             shuffle=False,
             persistent_workers=False,
             mode="val",
             metrics_format=metrics_format,
+            num_gpus=len(cfg.gpu_ids),
         )
 
         val_dataloader_args = {
             **cfg.data.val.get("deeplake_dataloader", {}),
             **val_dataloader_default_args,
         }
 
@@ -1394,16 +1434,19 @@
             val_masks_tensor,
             val_boxes_tensor,
             val_labels_tensor,
             pipeline=cfg.get("test_pipeline", []),
             implementation=dl_impl,
             **val_dataloader_args,
         )
-        eval_cfg["by_epoch"] = cfg.runner["type"] != "IterBasedRunner"
+
+        eval_cfg["by_epoch"] = cfg.runner["type"] != "DeeplakeIterBasedRunner"
         eval_hook = EvalHook
+        if distributed:
+            eval_hook = DistEvalHook
         # In this PR (https://github.com/open-mmlab/mmcv/pull/1193), the
         # priority of IterTimerHook has been modified from 'NORMAL' to 'LOW'.
         runner.register_hook(eval_hook(val_dataloader, **eval_cfg), priority="LOW")
 
     resume_from = None
     if cfg.resume_from is None and cfg.get("auto_resume"):
         resume_from = find_latest_checkpoint(cfg.work_dir)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `deeplake-3.2.9/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.3.0/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 elif PYTHON_VERSION == 3:
     from urllib.request import urlretrieve
 from mmdet.datasets import coco as mmdet_coco  # type: ignore
 from mmdet.datasets import pipelines
 from deeplake.util.warnings import always_warn
 import json
 import mmcv  # type: ignore
+import math
+from tqdm import tqdm  # type: ignore
 
 
 def _isArrayLike(obj):
     return hasattr(obj, "__iter__") and hasattr(obj, "__len__")
 
 
 class _COCO(pycocotools_coco.COCO):
@@ -69,15 +71,19 @@
         absolute_id = 0
         all_categories = self.labels
         all_bboxes = self.bboxes
         all_masks = self.masks
         all_imgs = self.imgs_orig
         all_iscrowds = self.iscrowds
 
-        for row_index, row in enumerate(self.dataset):
+        for row_index, row in tqdm(
+            enumerate(self.dataset),
+            desc="loading annotations",
+            total=len(self.dataset),
+        ):
             if all_imgs[row_index].size == 0:
                 always_warn(
                     "found empty image, skipping it. Please verify that your dataset is not corrupted."
                 )
                 continue
             categories = all_categories[row_index]  # make referencig custom
             bboxes = all_bboxes[row_index]
@@ -361,23 +367,27 @@
         file_client_args=dict(backend="disk"),
         imgs=None,
         masks=None,
         bboxes=None,
         labels=None,
         iscrowds=None,
         bbox_format=None,
+        batch_size=1,
+        num_gpus=1,
     ):
         self.img_prefix = img_prefix
         self.seg_prefix = seg_prefix
         self.seg_suffix = seg_suffix
         self.proposal_file = proposal_file
         self.test_mode = test_mode
         self.filter_empty_gt = filter_empty_gt
         self.file_client = mmcv.FileClient(**file_client_args)
         self.CLASSES = classes
+        self.batch_size = batch_size
+        self.num_gpus = num_gpus
 
         self.data_infos = self.load_annotations(
             deeplake_dataset,
             imgs=imgs,
             labels=labels,
             masks=masks,
             bboxes=bboxes,
@@ -397,14 +407,20 @@
             self._set_group_flag()
 
         # processing pipeline
 
     def pipeline(self, x):
         return x
 
+    def __len__(self):
+        length = super().__len__()
+        per_gpu_length = math.floor(length / (self.batch_size * self.num_gpus))
+        total_length = per_gpu_length * self.num_gpus
+        return total_length
+
     def load_annotations(
         self,
         deeplake_dataset,
         imgs=None,
         labels=None,
         masks=None,
         bboxes=None,
```

### Comparing `deeplake-3.2.9/deeplake/integrations/pytorch/common.py` & `deeplake-3.3.0/deeplake/integrations/pytorch/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-from typing import Callable, Dict, List, Optional
+from typing import Callable, Dict, Optional
 import warnings
 from deeplake.util.exceptions import EmptyTensorError
 from deeplake.util.iterable_ordered_dict import IterableOrderedDict
 from deeplake.core.polygon import Polygons
 import numpy as np
 import warnings
 
 
 def collate_fn(batch):
+    import torch
     from torch.utils.data._utils.collate import default_collate
 
     elem = batch[0]
     if isinstance(elem, IterableOrderedDict):
         return IterableOrderedDict(
             (key, collate_fn([d[key] for d in batch])) for key in elem.keys()
         )
 
     if isinstance(elem, np.ndarray) and elem.size > 0 and isinstance(elem[0], str):
         batch = [it[0] for it in batch]
+    elif isinstance(elem, (tuple, list)) and len(elem) > 0 and isinstance(elem[0], str):
+        batch = [it[0] for it in batch]
     elif isinstance(elem, Polygons):
         batch = [it.numpy() for it in batch]
+    elif isinstance(elem, (tuple, list)):
+        elem_type = type(elem)
+        return [elem_type([torch.tensor(item) for item in sample]) for sample in batch]
     return default_collate(batch)
 
 
 def convert_fn(data):
     from torch.utils.data._utils.collate import default_convert
 
     if isinstance(data, IterableOrderedDict):
@@ -55,64 +61,82 @@
                 data_out[tensor] = value if fn is None else fn(value)
             data_out = IterableOrderedDict(data_out)
             return data_out
         return data_in
 
 
 def check_tensors(dataset, tensors):
-    compressed_tensors = []
-    json_list_tensors = []
-    supported_compressions = {"png", "jpeg"}
+    jpeg_png_compressed_tensors = []
+    json_tensors = []
+    list_tensors = []
+    supported_image_compressions = {"png", "jpeg"}
     for tensor_name in tensors:
         tensor = dataset._get_tensor_from_root(tensor_name)
         if len(tensor) == 0:
             raise EmptyTensorError(
                 f" the dataset has an empty tensor {tensor_name}, pytorch dataloader can't be created."
                 f" Please either populate the tensor or pass tensors argument to .pytorch that excludes this"
                 f" tensor."
             )
-        if tensor.meta.sample_compression in supported_compressions:
-            compressed_tensors.append(tensor_name)
-        if tensor.meta.htype in {"list", "json"}:
-            json_list_tensors.append(tensor_name)
+        meta = tensor.meta
+        if meta.sample_compression in supported_image_compressions:
+            jpeg_png_compressed_tensors.append(tensor_name)
+        elif meta.htype == "json":
+            json_tensors.append(tensor_name)
+        elif meta.htype == "list":
+            list_tensors.append(tensor_name)
 
-    if json_list_tensors:
+    if json_tensors or list_tensors:
+        json_list_tensors = set(json_tensors + list_tensors)
         warnings.warn(
             f"The following tensors have json or list htype: {json_list_tensors}. Collation of these tensors will fail by default. Ensure that these tensors are either transformed by specifying a transform or a custom collate_fn is specified to handle them."
         )
 
-    return compressed_tensors
+    return jpeg_png_compressed_tensors, json_tensors, list_tensors
 
 
-def validate_decode_method(decode_method, all_tensor_keys, jpeg_png_compressed_tensors):
+def validate_decode_method(
+    decode_method,
+    all_tensor_keys,
+    jpeg_png_compressed_tensors,
+    json_tensors,
+    list_tensors,
+):
     raw_tensors = []
-    compressed_tensors = []
+    pil_compressed_tensors = []
     if decode_method is None:
         if len(jpeg_png_compressed_tensors) > 0:
             warnings.warn(
                 f"Decode method for tensors {jpeg_png_compressed_tensors} is defaulting to numpy. Please consider specifying a decode_method in .pytorch() that maximizes the data preprocessing speed based on your transformation."
             )
-        return raw_tensors, compressed_tensors
+        return raw_tensors, pil_compressed_tensors, json_tensors, list_tensors
 
     jpeg_png_compressed_tensors_set = set(jpeg_png_compressed_tensors)
+    json_list_tensors_set = set(json_tensors + list_tensors)
     generic_supported_decode_methods = {"numpy", "tobytes"}
     jpeg_png_supported_decode_methods = {"numpy", "tobytes", "pil"}
+    json_list_supported_decode_methods = {"numpy"}
     for tensor_name, decode_method in decode_method.items():
         if tensor_name not in all_tensor_keys:
             raise ValueError(
                 f"decode_method tensor {tensor_name} not found in tensors."
             )
         if tensor_name in jpeg_png_compressed_tensors_set:
             if decode_method not in jpeg_png_supported_decode_methods:
                 raise ValueError(
                     f"decode_method {decode_method} not supported for tensor {tensor_name}. Supported methods for this tensor are {jpeg_png_supported_decode_methods}"
                 )
+        elif tensor_name in json_list_tensors_set:
+            if decode_method not in json_list_supported_decode_methods:
+                raise ValueError(
+                    f"decode_method {decode_method} not supported for tensor {tensor_name}. Supported methods for this tensor are {json_list_supported_decode_methods}"
+                )
         elif decode_method not in generic_supported_decode_methods:
             raise ValueError(
                 f"decode_method {decode_method} not supported for tensor {tensor_name}. Supported methods for this tensor are {generic_supported_decode_methods}"
             )
         if decode_method == "tobytes":
             raw_tensors.append(tensor_name)
         elif decode_method == "pil":
-            compressed_tensors.append(tensor_name)
+            pil_compressed_tensors.append(tensor_name)
 
-    return raw_tensors, compressed_tensors
+    return raw_tensors, pil_compressed_tensors, json_tensors, list_tensors
```

### Comparing `deeplake-3.2.9/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.3.0/deeplake/integrations/pytorch/pytorch.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .common import (
     PytorchTransformFunction,
     convert_fn as default_convert_fn,
     collate_fn as default_collate_fn,
 )
 
 
-def create_dataloader_nesteddataloader(
+def create_dataloader(
     dataset,
     tensors,
     use_local_cache,
     transform,
     num_workers,
     buffer_size,
     batch_size,
@@ -45,53 +45,14 @@
         batch_size=batch_size,
         collate_fn=collate_fn,
         pin_memory=pin_memory,
         drop_last=drop_last,
     )
 
 
-def create_dataloader_shufflingdataloader(
-    dataset,
-    tensors,
-    tobytes,
-    use_local_cache,
-    transform,
-    num_workers,
-    buffer_size,
-    batch_size,
-    collate_fn,
-    pin_memory,
-    drop_last,
-):
-    import torch
-    import torch.utils.data
-    from deeplake.integrations.pytorch.dataset import ShufflingIterableDataset
-
-    return torch.utils.data.DataLoader(
-        # this data set is more efficient also shuffles
-        # using threads race conditions as source of entropy
-        ShufflingIterableDataset(
-            dataset,
-            tensors=tensors,
-            tobytes=tobytes,
-            use_local_cache=use_local_cache,
-            transform=transform,
-            num_workers=num_workers,
-            buffer_size=buffer_size,
-        ),
-        batch_size=batch_size,
-        collate_fn=collate_fn,
-        pin_memory=pin_memory,
-        drop_last=drop_last,
-    )
-
-
-create_dataloader = create_dataloader_nesteddataloader
-
-
 def dataset_to_pytorch(
     dataset,
     num_workers: int,
     batch_size: int,
     drop_last: bool,
     *args,
     collate_fn: Optional[Callable],
@@ -161,14 +122,15 @@
                 transform=transform,
                 num_workers=num_workers,
                 shuffle=shuffle,
                 buffer_size=buffer_size,
                 return_index=return_index,
                 pad_tensors=pad_tensors,
                 decode_method=decode_method,
+                batch_size=batch_size,
             ),
             batch_size=batch_size,
             collate_fn=collate_fn,
             pin_memory=pin_memory,
             num_workers=num_workers,
             drop_last=drop_last,
         )
```

### Comparing `deeplake-3.2.9/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.3.0/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/integrations/tf/common.py` & `deeplake-3.3.0/deeplake/integrations/tf/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from deeplake.util.iterable_ordered_dict import IterableOrderedDict
 from deeplake.core.polygon import Polygons
 import numpy as np
 
 
 def collate_fn(batch):
+    from tensorflow import convert_to_tensor
+
     elem = batch[0]
     if isinstance(elem, IterableOrderedDict):
         return IterableOrderedDict(
             (key, collate_fn([d[key] for d in batch])) for key in elem.keys()
         )
 
     if isinstance(elem, np.ndarray) and elem.size > 0 and isinstance(elem[0], str):
```

### Comparing `deeplake-3.2.9/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.3.0/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import warnings
 
 from deeplake.util.exceptions import (
     ModuleNotInstalledException,
     SampleDecompressionError,
     CorruptedSampleError,
+    ReadSampleFromChunkError,
 )
 from deeplake.util.check_installation import tensorflow_installed
 
 
 def dataset_to_tensorflow(dataset, tensors, tobytes, fetch_chunks=True):
     """Converts the dataset into a tensorflow compatible format"""
     if not tensorflow_installed():
@@ -42,15 +43,15 @@
                 try:
                     value = sample[key]
                     if tobytes[key]:
                         value = [value.tobytes()]
                     else:
                         value = value.numpy(fetch_chunks=fetch_chunks)
                     out[key] = value
-                except SampleDecompressionError:
+                except ReadSampleFromChunkError:
                     warnings.warn(
                         f"Skipping corrupt {dataset[key].meta.sample_compression} sample."
                     )
                     corrupt_sample_found = True
             if not corrupt_sample_found:
                 yield out
```

### Comparing `deeplake-3.2.9/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.3.0/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/integrations/wandb/wandb.py` & `deeplake-3.3.0/deeplake/integrations/wandb/wandb.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,14 +56,24 @@
 import json
 import warnings
 import deeplake
 
 _WANDB_INSTALLED = bool(importlib.util.find_spec("wandb"))
 
 
+def ignore_exceptions(f):
+    def wrapper(*args, **kwargs):
+        try:
+            return f(*args, **kwargs)
+        except Exception:
+            pass
+
+    return wrapper
+
+
 def wandb_run():
     if not deeplake.constants.WANDB_INTEGRATION_ENABLED:
         return
     return getattr(sys.modules.get("wandb"), "run", None)
 
 
 _READ_DATASETS: Dict[str, Set[str]] = {}
@@ -179,18 +189,20 @@
     # TODO : commit and view id are not supported by visualizer. Remove below line once they are supported.
     url = "/".join(url.split("/")[:2])
     run.log(
         {f"Deep Lake Dataset - {url}": wandb.Html(_viz_html("hub://" + url))}, step=0
     )
 
 
+@ignore_exceptions
 def dataset_written(ds):
     pass
 
 
+@ignore_exceptions
 def dataset_committed(ds):
     run = wandb_run()
     key = get_ds_key(ds)
     if run:
         if run.id not in _WRITTEN_DATASETS:
             _WRITTEN_DATASETS.clear()
             _WRITTEN_DATASETS[run.id] = {}
@@ -250,14 +262,15 @@
             if not rm:
                 ret.append(dsconfig)
         else:
             ret.append(dsconfig)
     return ret
 
 
+@ignore_exceptions
 def dataset_read(ds):
     run = wandb_run()
     if not run:
         return
     feature_report_path(ds.path, "wandb_dataset_read", {})
     if run.id not in _READ_DATASETS:
         _READ_DATASETS.clear()
```

### Comparing `deeplake-3.2.9/deeplake/tests/cache_fixtures.py` & `deeplake-3.3.0/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/tests/client_fixtures.py` & `deeplake-3.3.0/deeplake/tests/client_fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,18 @@
         )
 
     username = os.getenv(ENV_HUB_DEV_USERNAME)
     password = os.getenv(ENV_HUB_DEV_PASSWORD)
 
     assert (
         username is not None
-    ), f"Hub dev username was not found in the environment variable '{ENV_HUB_DEV_USERNAME}'. This is necessary for testing deeplake cloud datasets."
+    ), f"Deep Lake dev username was not found in the environment variable '{ENV_HUB_DEV_USERNAME}'. This is necessary for testing deeplake cloud datasets."
     assert (
         password is not None
-    ), f"Hub dev password was not found in the environment variable '{ENV_HUB_DEV_PASSWORD}'. This is necessary for testing deeplake cloud datasets."
+    ), f"Deep Lake dev password was not found in the environment variable '{ENV_HUB_DEV_PASSWORD}'. This is necessary for testing deeplake cloud datasets."
 
     return username, password
 
 
 @pytest.fixture(scope="session")
 def hub_cloud_dev_token(hub_cloud_dev_credentials):
     username, password = hub_cloud_dev_credentials
```

### Comparing `deeplake-3.2.9/deeplake/tests/common.py` & `deeplake-3.3.0/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/tests/dataset_fixtures.py` & `deeplake-3.3.0/deeplake/tests/dataset_fixtures.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,24 @@
         "s3_ds_generator",
         "gcs_ds_generator",
         "gdrive_ds_generator",
     ],
     indirect=True,
 )
 
+enabled_persistent_non_gdrive_dataset_generators = pytest.mark.parametrize(
+    "ds_generator",
+    [
+        "local_ds_generator",
+        "s3_ds_generator",
+        "gcs_ds_generator",
+    ],
+    indirect=True,
+)
+
 enabled_cloud_dataset_generators = pytest.mark.parametrize(
     "ds_generator",
     [
         "s3_ds_generator",
         "gcs_ds_generator",
     ],
     indirect=True,
```

### Comparing `deeplake-3.2.9/deeplake/tests/path_fixtures.py` & `deeplake-3.3.0/deeplake/tests/path_fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,30 @@
     repo_name = posixpath.split(url)[-1]
     repo_name = repo_name.split("@", 1)[0]
     if repo_name.endswith(".git"):
         repo_name = repo_name[:-4]
     return repo_name
 
 
+def _git_clone_with_branch(branch_name, url):
+    _repo_name = _repo_name_from_git_url(url)
+    cached_dir = _GIT_CLONE_CACHE_DIR + "/" + _repo_name
+    if not os.path.isdir(cached_dir):
+        if not os.path.isdir(_GIT_CLONE_CACHE_DIR):
+            os.mkdir(_GIT_CLONE_CACHE_DIR)
+        cwd = os.getcwd()
+        os.chdir(_GIT_CLONE_CACHE_DIR)
+        try:
+            os.system(f"git clone -b {branch_name} {url}")
+        finally:
+            os.chdir(cwd)
+    assert os.path.isdir(cached_dir)
+    return cached_dir
+
+
 def _git_clone(url):
     _repo_name = _repo_name_from_git_url(url)
     cached_dir = _GIT_CLONE_CACHE_DIR + "/" + _repo_name
     if not os.path.isdir(cached_dir):
         if not os.path.isdir(_GIT_CLONE_CACHE_DIR):
             os.mkdir(_GIT_CLONE_CACHE_DIR)
         cwd = os.getcwd()
@@ -108,14 +124,24 @@
         "annotations_directory": path + "/yolo/annotations_only",
         "data_directory_missing_annotations": path + "/yolo/data_missing_annotations",
         "data_directory_unsupported_annotations": path
         + "/yolo/data_unsupported_annotations",
     }
 
 
+def _download_hub_test_dataframe_data():
+    path = _git_clone(_HUB_TEST_RESOURCES_URL)
+    return {
+        "basic_dataframe_w_sanitize_path": path + "/dataframe/text_w_sanitization.txt",
+        "dataframe_w_images_path": path + "/dataframe/csv_w_local_files.csv",
+        "dataframe_w_bad_images_path": path + "/dataframe/csv_w_local_bad_file.csv",
+        "images_basepath": path + "/dataframe/images",
+    }
+
+
 def _download_pil_test_images(ext=[".jpg", ".png"]):
     paths = {e: [] for e in ext}
     corrupt_file_keys = [
         "broken",
         "_dos",
         "truncated",
         "chunk_no_fctl",
@@ -123,15 +149,15 @@
     ]
 
     path = _git_clone(_PILLOW_URL)
     dirs = [
         path + x
         for x in [
             "/Tests/images",
-            "/Tests/images/apng",
+            # "/Tests/images/apng",
             "/Tests/images/imagedraw",
         ]
     ]
     for d in dirs:
         for f in os.listdir(d):
             brk = False
             for k in corrupt_file_keys:
@@ -371,14 +397,22 @@
     """Path to a flower image in the dummy data folder. Expected shape: (513, 464, 4)"""
 
     path = get_dummy_data_path("images")
     return os.path.join(path, "flower.png")
 
 
 @pytest.fixture
+def hopper_gray_path():
+    """Path to a grayscale hopper image in the dummy data folder. Expected shape: (512, 512)"""
+
+    path = get_dummy_data_path("images")
+    return os.path.join(path, "hopper_gray.jpg")
+
+
+@pytest.fixture
 def color_image_paths():
     base = get_dummy_data_path("images")
     paths = {
         "jpeg": os.path.join(base, "dog2.jpg"),
     }
     return paths
 
@@ -390,15 +424,15 @@
         "jpeg": os.path.join(base, "hopper_gray.jpg"),
     }
     return paths
 
 
 @pytest.fixture(scope="session")
 def mmdet_path():
-    return _git_clone(_MMDET_URL)
+    return _git_clone_with_branch("dev-2.x", _MMDET_URL)
 
 
 @pytest.fixture(scope="session")
 def compressed_image_paths():
     paths = {
         "webp": "beach.webp",
         "fli": "hopper.fli",
@@ -526,7 +560,12 @@
 def coco_ingestion_data():
     return _download_hub_test_coco_data()
 
 
 @pytest.fixture(scope="session")
 def yolo_ingestion_data():
     return _download_hub_test_yolo_data()
+
+
+@pytest.fixture(scope="session")
+def dataframe_ingestion_data():
+    return _download_hub_test_dataframe_data()
```

### Comparing `deeplake-3.2.9/deeplake/tests/storage_fixtures.py` & `deeplake-3.3.0/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/access_method.py` & `deeplake-3.3.0/deeplake/util/access_method.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     creds,
     token,
     org_id,
     verbose,
     ds_exists,
     num_workers,
     scheduler,
+    reset,
 ):
     local_path = get_local_storage_path(path, os.environ["DEEPLAKE_DOWNLOAD_PATH"])
     download = access_method == "download" or (
         access_method == "local" and not deeplake.exists(local_path)
     )
     if download:
         if not ds_exists:
@@ -87,14 +88,15 @@
         local_path,
         read_only=read_only,
         verbose=verbose,
         memory_cache_size=memory_cache_size,
         local_cache_size=local_cache_size,
         token=token,
         org_id=org_id,
+        reset=reset,
     )
     if download:
         ds.storage.next_storage[TIMESTAMP_FILENAME] = time.ctime().encode("utf-8")
     else:
         timestamp = ds.storage.next_storage[TIMESTAMP_FILENAME].decode("utf-8")
         print(f"** Loaded local copy of dataset. Downloaded on: {timestamp}")
     return ds
```

### Comparing `deeplake-3.2.9/deeplake/util/agreement.py` & `deeplake-3.3.0/deeplake/util/agreement.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from typing import List
 from deeplake.util.exceptions import AgreementNotAcceptedError
 
+import deeplake.util.spinner
+
 
 def agreement_prompt(agreements: List[str], org_id: str, ds_name: str):
+    spinner = deeplake.util.spinner.ACTIVE_SPINNER
+    if spinner:
+        spinner.hide()
     print(
         "\n\nThe owner of the dataset you are trying to access requires that you agree to the following terms first:\n"
     )
     print("-" * 16)
     print(f"Dataset Owner: {org_id}")
     print(f"Dataset Name: {ds_name}")
     print("-" * 16)
@@ -16,14 +21,16 @@
     for agreement in agreements:
         print(agreement + "\n")
 
     print("-" * 16)
     user_input = input(
         f"In order to accept, please type the dataset's name ({ds_name}) and press enter: "
     )
+    if spinner:
+        spinner.show()
     return user_input == ds_name
 
 
 def handle_dataset_agreements(client, agreements: List[str], org_id: str, ds_name: str):
     accepted = agreement_prompt(agreements, org_id, ds_name)
     if not accepted:
         raise AgreementNotAcceptedError()
```

### Comparing `deeplake-3.2.9/deeplake/util/array_list.py` & `deeplake-3.3.0/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/assert_byte_indexes.py` & `deeplake-3.3.0/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/auto.py` & `deeplake-3.3.0/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/bugout_reporter.py` & `deeplake-3.3.0/deeplake/util/bugout_reporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,23 +99,41 @@
 
 consent = HumbugConsent(consent_from_reporting_config_file)
 
 session_id = str(uuid.uuid4())
 bugout_reporting_config = get_reporting_config()
 client_id = bugout_reporting_config.get("client_id")
 
+
+def blacklist_token_parameters_fn(params: Dict[str, Any]) -> Dict[str, Any]:
+    admissible_params = {k: v for k, v in params.items() if "token" not in k.lower()}
+    return admissible_params
+
+
 deeplake_reporter = HumbugReporter(
     name="activeloopai/Hub",
     consent=consent,
     client_id=client_id,
     session_id=session_id,
     bugout_token=BUGOUT_TOKEN,
+    blacklist_fn=blacklist_token_parameters_fn,
     tags=[],
 )
 
+
+def set_username(reporter: HumbugReporter, username: str) -> None:
+    index, current_username = find_current_username(reporter)
+
+    if current_username is None:
+        reporter.tags.append(f"username:{username}")
+    else:
+        if f"username:{username}" != current_username:
+            reporter.tags[index] = f"username:{username}"
+
+
 hub_user = bugout_reporting_config.get("username")
 if hub_user is not None:
     deeplake_reporter.tags.append(f"username:{hub_user}")
 
 machine_id = bugout_reporting_config.get("machine_id")
 if machine_id is not None:
     deeplake_reporter.tags.append(f"machine_id:{machine_id}")
@@ -134,26 +152,20 @@
     if path.startswith(starts_with):
         parameters["Path"] = path
 
     if token is not None:
         client = DeepLakeBackendClient(token=token)
         username = client.get_user_profile()["name"]
 
-        index, current_username = find_current_username()
-
-        if current_username is None:
-            deeplake_reporter.tags.append(f"username:{username}")
-        else:
-            if f"username:{username}" != current_username:
-                deeplake_reporter.tags[index] = f"username:{username}"
+        set_username(deeplake_reporter, username)
 
     deeplake_reporter.feature_report(
         feature_name=feature_name,
         parameters=parameters,
     )
 
 
-def find_current_username():
-    for index, tag in enumerate(deeplake_reporter.tags):
+def find_current_username(reporter: HumbugReporter):
+    for index, tag in enumerate(reporter.tags):
         if "username" in tag:
             return index, tag
     return None, None
```

### Comparing `deeplake-3.2.9/deeplake/util/cache_chain.py` & `deeplake-3.3.0/deeplake/util/cache_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from deeplake.constants import LOCAL_CACHE_PREFIX
 from typing import List, Optional
 from uuid import uuid1
 import os
-from deeplake.core.storage import StorageProvider, MemoryProvider, LocalProvider
+from deeplake.core.storage import (
+    StorageProvider,
+    MemoryProvider,
+    LocalProvider,
+)
 from deeplake.core.storage.lru_cache import LRUCache
 from deeplake.util.exceptions import ProviderSizeListMismatch, ProviderListEmptyError
 
 
 def get_cache_chain(storage_list: List[StorageProvider], size_list: List[int]):
     """Returns a chain of storage providers as a cache
```

### Comparing `deeplake-3.2.9/deeplake/util/casting.py` & `deeplake-3.3.0/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/check_latest_version.py` & `deeplake-3.3.0/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/chunk_engine.py` & `deeplake-3.3.0/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/class_label.py` & `deeplake-3.3.0/deeplake/util/class_label.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         return idx if return_original else None
     return [convert_to_text(item, class_names) for item in inp]
 
 
 def sync_labels(
     ds, label_temp_tensors, hash_label_maps, num_workers, scheduler, verbose=True
 ):
+    ds = ds.root
     hl_maps = defaultdict(OrderedDict)
     for map in hash_label_maps:
         for tensor in map:
             hl_maps[tensor].update(map[tensor])
     hash_label_maps = hl_maps
 
     @deeplake.compute
@@ -115,16 +116,14 @@
                 target_tensor.meta._disable_temp_transform = True
                 target_tensor.meta.is_dirty = True
 
                 logger.info("Synchronizing class labels...")
                 class_label_sync(label_tensor=tensor, hash_idx_map=hash_idx_map).eval(
                     ds[temp_tensor],
                     ds,
-                    num_workers=num_workers,
-                    scheduler=scheduler,
                     progressbar=True,
                     check_lengths=False,
                     skip_ok=True,
                 )
                 target_tensor.meta._disable_temp_transform = False
             finally:
                 ds.delete_tensor(temp_tensor, large_ok=True)
```

### Comparing `deeplake-3.2.9/deeplake/util/compute.py` & `deeplake-3.3.0/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/connect_dataset.py` & `deeplake-3.3.0/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/diff.py` & `deeplake-3.3.0/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/downsample.py` & `deeplake-3.3.0/deeplake/util/downsample.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from PIL import Image  # type: ignore
 import deeplake
 from deeplake.core.partial_sample import PartialSample
 from deeplake.core.linked_tiled_sample import LinkedTiledSample
 import numpy as np
 import io
 from deeplake.core.tensor_link import read_linked_sample
+import warnings
 
 
 def validate_downsampling(downsampling):
     if downsampling is None:
         return None, None
     if len(downsampling) != 2:
         raise ValueError(
@@ -50,38 +51,46 @@
     sample: Optional[Union[Image.Image, PartialSample]],
     factor: int,
     compression: Optional[str],
     htype: str,
     partial: bool = False,
     link_creds=None,
 ):
-    if sample is None:
+    try:
+        if sample is None:
+            return None
+        elif isinstance(sample, PartialSample):
+            return sample.downsample(factor)
+        elif isinstance(sample, LinkedTiledSample):
+            return downsample_link_tiled(sample, factor, compression, htype, link_creds)
+
+        if not partial and not needs_downsampling(sample, factor):
+            arr = np.array(sample) if isinstance(sample, Image.Image) else sample
+            required_shape = tuple([0] * len(arr.shape))
+            required_dtype = arr.dtype
+            return np.ones(required_shape, dtype=required_dtype)
+
+        if isinstance(sample, np.ndarray):
+            downsampled_sample = sample[::factor, ::factor]
+            return downsampled_sample
+        size = sample.size[0] // factor, sample.size[1] // factor
+        downsampled_sample = sample.resize(size, get_filter(htype))
+        if compression is None:
+            return np.array(downsampled_sample)
+        with io.BytesIO() as f:
+            downsampled_sample.save(f, format=compression)  # type: ignore
+            image_bytes = f.getvalue()
+            return deeplake.core.sample.Sample(
+                buffer=image_bytes, compression=compression
+            )
+    except Exception as e:
+        if partial:
+            raise e
+        warnings.warn(f"Failed to downsample sample of type {type(sample)}")
         return None
-    elif isinstance(sample, PartialSample):
-        return sample.downsample(factor)
-    elif isinstance(sample, LinkedTiledSample):
-        return downsample_link_tiled(sample, factor, compression, htype, link_creds)
-
-    if not partial and not needs_downsampling(sample, factor):
-        arr = np.array(sample) if isinstance(sample, Image.Image) else sample
-        required_shape = tuple([0] * len(arr.shape))
-        required_dtype = arr.dtype
-        return np.ones(required_shape, dtype=required_dtype)
-
-    if isinstance(sample, np.ndarray):
-        downsampled_sample = sample[::factor, ::factor]
-        return downsampled_sample
-    size = sample.size[0] // factor, sample.size[1] // factor
-    downsampled_sample = sample.resize(size, get_filter(htype))
-    if compression is None:
-        return np.array(downsampled_sample)
-    with io.BytesIO() as f:
-        downsampled_sample.save(f, format=compression)  # type: ignore
-        image_bytes = f.getvalue()
-        return deeplake.core.sample.Sample(buffer=image_bytes, compression=compression)
 
 
 def downsample_link_tiled(
     sample: LinkedTiledSample, factor, compression, htype, link_creds=None
 ):
     shape = sample.shape
     tile_shape = sample.tile_shape
```

### Comparing `deeplake-3.2.9/deeplake/util/encoder.py` & `deeplake-3.3.0/deeplake/util/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 import numpy as np
 from typing import Dict, List
 from deeplake.core.meta.encode.creds import CredsEncoder
 from deeplake.core.meta.tensor_meta import TensorMeta
 from deeplake.core.meta.encode.chunk_id import ChunkIdEncoder
 from deeplake.core.meta.encode.tile import TileEncoder
 from deeplake.core.meta.encode.sequence import SequenceEncoder
+from deeplake.core.meta.encode.pad import PadEncoder
 from deeplake.core.storage.provider import StorageProvider
 from deeplake.core.version_control.commit_chunk_map import CommitChunkMap
 from deeplake.core.version_control.commit_diff import CommitDiff
 from deeplake.util.keys import (
     get_creds_encoder_key,
     get_sequence_encoder_key,
+    get_pad_encoder_key,
     get_tensor_commit_chunk_map_key,
     get_tensor_commit_diff_key,
     get_tensor_meta_key,
     get_chunk_id_encoder_key,
     get_chunk_id_encoder_key,
     get_tensor_tile_encoder_key,
 )
@@ -44,14 +46,17 @@
     )
     merge_all_creds_encoders(
         result["creds_encoders"], target_ds, storage, overwrite, generated_tensors
     )
     merge_all_sequence_encoders(
         result["sequence_encoders"], target_ds, storage, overwrite, generated_tensors
     )
+    merge_all_pad_encoders(
+        result["pad_encoders"], target_ds, storage, overwrite, generated_tensors
+    )
     if target_ds.commit_id is not None:
         merge_all_commit_chunk_maps(
             result["commit_chunk_maps"],
             target_ds,
             storage,
             overwrite,
             generated_tensors,
@@ -334,7 +339,50 @@
     """Combines the dataset's sequence_encoder with a single worker's sequence_encoder."""
     arr = worker_sequence_encoder.array
     last_index = -1
     for i in range(len(arr)):
         next_last_index = arr[i][2]
         ds_sequence_encoder.register_samples(arr[i][0], next_last_index - last_index)
         last_index = next_last_index
+
+
+def combine_pad_encoders(
+    ds_pad_encoder: PadEncoder, worker_pad_encoder: PadEncoder
+) -> PadEncoder:
+    enc = PadEncoder()
+    idx = None
+    arr1 = ds_pad_encoder.array
+    arr2 = worker_pad_encoder.array
+    if not arr1.size or not arr2.size:
+        return enc
+    for i in range(int(max(arr1.max(), arr2.max())) + 1):
+        if ds_pad_encoder.is_padded(i) and worker_pad_encoder.is_padded(i):
+            if idx is None:
+                idx = i
+        else:
+            if idx is not None:
+                enc.add_padding(idx, i - idx)
+                idx = None
+    return enc
+
+
+def merge_all_pad_encoders(
+    all_workers_pad_encoders: List[Dict[str, PadEncoder]],
+    target_ds: deeplake.Dataset,
+    storage: StorageProvider,
+    overwrite: bool,
+    tensors: List[str],
+) -> None:
+    commit_id = target_ds.version_state["commit_id"]
+    for tensor in tensors:
+        rel_path = posixpath.relpath(tensor, target_ds.group_index)
+        actual_tensor = target_ds[rel_path]
+        pad_encoder = None if overwrite else actual_tensor.chunk_engine.pad_encoder
+        for current_worker_pad_encoder in all_workers_pad_encoders:
+            current_pad_encoder = current_worker_pad_encoder[tensor]
+            if pad_encoder is None:
+                pad_encoder = current_pad_encoder
+            else:
+                pad_encoder = combine_pad_encoders(pad_encoder, current_pad_encoder)
+
+        pad_key = get_pad_encoder_key(tensor, commit_id)
+        storage[pad_key] = pad_encoder.tobytes()  # type: ignore
```

### Comparing `deeplake-3.2.9/deeplake/util/exceptions.py` & `deeplake-3.3.0/deeplake/util/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     def __init__(self, tensor_name: str):
         super().__init__(f"Tensor '{tensor_name}' does not exist.")
 
 
 class TensorAlreadyExistsError(Exception):
     def __init__(self, key: str):
         super().__init__(
-            f"Tensor '{key}' already exists. If applicable, you can use the `overwrite=True` parameter!"
+            f"Tensor '{key}' already exists. You can use the `exist_ok=True` parameter to ignore this error message."
         )
 
 
 class TensorGroupDoesNotExistError(KeyError):
     def __init__(self, group_name: str):
         super().__init__(f"Tensor group '{group_name}' does not exist.")
 
@@ -195,15 +195,24 @@
         self,
         message="Error while logging in, invalid auth token. Please try logging in again.",
     ):
         super().__init__(message)
 
 
 class UserNotLoggedInException(Exception):
-    def __init__(self, message=""):
+    def __init__(self):
+        message = (
+            "You are not logged in and an API token was not found. To complete the operation, you can\n"
+            "1. Login with your username and password using the `activeloop login` CLI command.\n"
+            "2. Create an API token at https://app.activeloop.ai and use it in any of the following ways:\n"
+            "    - Set the environment variable `ACTIVELOOP_TOKEN` to the token value.\n"
+            "    - Use the CLI command `activeloop login -t <token>`.\n"
+            "    - Pass the API token to the `token` parameter of this function.\n"
+            "Visit https://docs.activeloop.ai/getting-started/using-activeloop-storage for more information."
+        )
         super().__init__(message)
 
 
 class InvalidHubPathException(Exception):
     def __init__(self, path):
         super().__init__(
             f"The Dataset's path is an invalid Deep Lake cloud path. It should be of the form hub://username/dataset got {path}."
@@ -370,18 +379,20 @@
     ):
         super().__init__(
             f"Could not compress a sample with shape {str(sample_shape)} into '{compression_format}'. Raw error output: '{message}'.",
         )
 
 
 class SampleDecompressionError(CompressionError):
-    def __init__(self):
-        super().__init__(
-            f"Could not decompress sample buffer into an array. Either the sample's buffer is corrupted, or it is in an unsupported format. Supported compressions: {deeplake.compressions}."
-        )
+    def __init__(self, path: Optional[str] = None):
+        message = "Could not decompress sample"
+        if path:
+            message += f" at {path}"
+        message += f". Either the sample's buffer is corrupted, or it is in an unsupported format. Supported compressions: {deeplake.compressions}."
+        super().__init__(message)
 
 
 class InvalidImageDimensions(Exception):
     def __init__(self, actual_dims, expected_dims):
         super().__init__(
             f"The shape length {actual_dims} of the given array should "
             f"be greater than the number of expected dimensions {expected_dims}"
@@ -499,16 +510,96 @@
 class ReadOnlyModeError(Exception):
     def __init__(self, custom_message: Optional[str] = None):
         if custom_message is None:
             custom_message = "Modification when in read-only mode is not supported!"
         super().__init__(custom_message)
 
 
+def is_primitive(sample):
+    if isinstance(sample, (str, int, float, bool)):
+        return True
+    if isinstance(sample, dict):
+        for x, y in sample.items():
+            if not is_primitive(x) or not is_primitive(y):
+                return False
+        return True
+    if isinstance(sample, (list, tuple)):
+        for x in sample:
+            if not is_primitive(x):
+                return False
+        return True
+    return False
+
+
+def get_truncated_sample(sample, max_half_len=50):
+    if len(str(sample)) > max_half_len * 2:
+        return (
+            str(sample)[:max_half_len] + "..." + str(sample)[int(-max_half_len - 1) :]
+        )
+    return str(sample)
+
+
+def has_path(sample):
+    from deeplake.core.sample import Sample
+    from deeplake.core.linked_sample import LinkedSample
+
+    return isinstance(sample, LinkedSample) or (
+        isinstance(sample, Sample) and sample.path is not None
+    )
+
+
 class TransformError(Exception):
-    pass
+    def __init__(self, index=None, sample=None, samples_processed=0):
+        self.index = index
+        self.sample = sample
+        # multiprocessing re raises error with str
+        if isinstance(index, str):
+            super().__init__(index)
+        else:
+            print_item = print_path = False
+            if sample:
+                print_item = is_primitive(sample)
+                print_path = has_path(sample)
+
+            msg = f"Transform failed"
+            if index is not None:
+                msg += f" at index {index} of the input data"
+
+            if print_item:
+                msg += f" on the item: {get_truncated_sample(sample)}"
+            elif print_path:
+                msg += f" on the sample at path: '{sample.path}'"
+            msg += "."
+
+            if samples_processed > 0:
+                msg += f" Last checkpoint: {samples_processed} samples processed. You can slice the input to resume from this point."
+
+            msg += " See traceback for more details."
+            super().__init__(msg)
+
+
+class SampleAppendError(Exception):
+    def __init__(self, tensor, sample=None):
+        print_item = print_path = False
+        if sample:
+            print_item = is_primitive(sample)
+            print_path = has_path(sample)
+        if print_item or print_path:
+            msg = "Failed to append the sample "
+
+            if print_item:
+                msg += str(sample) + " "
+            elif print_path:
+                msg += f"at path '{sample.path}' "
+        else:
+            msg = f"Failed to append a sample "
+
+        msg += f"to the tensor '{tensor}'. See more details in the traceback."
+
+        super().__init__(msg)
 
 
 class FilterError(Exception):
     pass
 
 
 class InvalidInputDataError(TransformError):
@@ -608,16 +699,20 @@
     def __init__(self):
         super().__init__(
             "Dataset having MemoryProvider as underlying storage should not be pickled as data won't be saved."
         )
 
 
 class CorruptedSampleError(Exception):
-    def __init__(self, compression):
-        super().__init__(f"Invalid {compression} file.")
+    def __init__(self, compression, path: Optional[str] = None):
+        message = f"Unable to decompress {compression} file"
+        if path is not None:
+            message += f" at {path}"
+        message += "."
+        super().__init__(message)
 
 
 class VersionControlError(Exception):
     pass
 
 
 class MergeError(Exception):
@@ -859,8 +954,98 @@
             htype = f"For {htype} htype "
         message = f"{htype}{extension} is not supported"
 
         super().__init__(message)
 
 
 class DatasetCorruptError(Exception):
+    def __init__(self, message, action="", cause=None):
+        self.message = message
+        self.action = action
+        self.__cause__ = cause
+
+        super().__init__(self.message + (" " + self.action if self.action else ""))
+
+
+class SampleReadError(Exception):
+    def __init__(self, path: str):
+        super().__init__(f"Unable to read sample from {path}")
+
+
+class GetChunkError(Exception):
+    def __init__(
+        self,
+        chunk_key: Optional[str],
+        global_index: Optional[int] = None,
+        tensor_name: Optional[str] = None,
+    ):
+        self.chunk_key = chunk_key
+        message = "Unable to get chunk"
+        if chunk_key is not None:
+            message += f" '{chunk_key}'"
+        if global_index is not None:
+            message += f" while retrieving data at index {global_index}"
+        if tensor_name is not None:
+            message += f" in tensor {tensor_name}"
+        message += "."
+        super().__init__(message)
+
+
+class ReadSampleFromChunkError(Exception):
+    def __init__(
+        self,
+        chunk_key: Optional[str],
+        global_index: Optional[int] = None,
+        tensor_name: Optional[str] = None,
+    ):
+        self.chunk_key = chunk_key
+        message = "Unable to read sample"
+        if global_index is not None:
+            message += f" at index {global_index}"
+        message += " from chunk"
+        if chunk_key is not None:
+            message += f" '{chunk_key}'"
+        if tensor_name is not None:
+            message += f" in tensor {tensor_name}"
+        message += "."
+        super().__init__(message)
+
+
+class GetDataFromLinkError(Exception):
+    def __init__(
+        self,
+        link: str,
+        global_index: Optional[int] = None,
+        tensor_name: Optional[str] = None,
+    ):
+        self.link = link
+        message = f"Unable to get data from link {link}"
+        if global_index is not None:
+            message += f" while retrieving data at index {global_index}"
+        if tensor_name is not None:
+            message += f" in tensor {tensor_name}"
+        message += "."
+        super().__init__(message)
+
+
+class TransformFailedError(Exception):
+    def __init__(self, global_index):
+        super().__init__(
+            f"Dataloader transform failed while processing sample at index {global_index}."
+        )
+
+
+class MissingCredsError(Exception):
+    pass
+
+
+class EmptyPolygonError(Exception):
     pass
+
+
+class MissingManagedCredsError(Exception):
+    pass
+
+
+class SampleUpdateError(Exception):
+    def __init__(self, key: str):
+        super().__init__(f"Unable to update sample in tensor {key}.")
```

### Comparing `deeplake-3.2.9/deeplake/util/exif.py` & `deeplake-3.3.0/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/from_tfds.py` & `deeplake-3.3.0/deeplake/util/from_tfds.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     return from_tfds(tfds_ds=tfds_ds, ds=ds)  # type: ignore
 
 
 def from_tfds(tfds_ds: tensorflow.data.Dataset, ds: Dataset):
     """Converts a tfds dataset to Deep Lake dataset
     Args:
         tfds_ds (tensorflow.data.Dataset): A tfds_dataset object.
-        ds (Dataset) : A Hub dataset object where Tensor will be created.
+        ds (Dataset) : A Deep Lake dataset object where Tensor will be created.
     Returns:
         A Deep Lake dataset
     """
     tfds_numpy = tfds.as_numpy(tfds_ds)  # Convert `tf.data.Dataset` to Python generator
 
     for sample in tqdm(tfds_numpy):
         for col in sample:
```

### Comparing `deeplake-3.2.9/deeplake/util/htype.py` & `deeplake-3.3.0/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/image.py` & `deeplake-3.3.0/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/invalid_view_op.py` & `deeplake-3.3.0/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/iteration_warning.py` & `deeplake-3.3.0/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/json.py` & `deeplake-3.3.0/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/keys.py` & `deeplake-3.3.0/deeplake/util/keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import posixpath
 from deeplake.constants import (
     CHUNKS_FOLDER,
+    COMMIT_INFO_FILENAME,
     DATASET_DIFF_FILENAME,
     DATASET_INFO_FILENAME,
     DATASET_LOCK_FILENAME,
     ENCODED_CREDS_FOLDER,
     LINKED_CREDS_FILENAME,
     UNSHARDED_ENCODER_FILENAME,
     ENCODED_CHUNK_NAMES_FOLDER,
     ENCODED_SEQUENCE_NAMES_FOLDER,
     ENCODED_TILE_NAMES_FOLDER,
+    ENCODED_PAD_NAMES_FOLDER,
     FIRST_COMMIT_ID,
     DATASET_META_FILENAME,
     TENSOR_INFO_FILENAME,
     TENSOR_META_FILENAME,
     TENSOR_COMMIT_CHUNK_MAP_FILENAME,
     TENSOR_COMMIT_CHUNK_MAP_FILENAME,
     TENSOR_COMMIT_DIFF_FILENAME,
@@ -54,14 +56,20 @@
 
 def get_dataset_diff_key(commit_id: str) -> str:
     if commit_id == FIRST_COMMIT_ID:
         return DATASET_DIFF_FILENAME
     return "/".join(("versions", commit_id, DATASET_DIFF_FILENAME))
 
 
+def get_commit_info_key(commit_id: str) -> str:
+    if commit_id == FIRST_COMMIT_ID:
+        return COMMIT_INFO_FILENAME
+    return "/".join(("versions", commit_id, COMMIT_INFO_FILENAME))
+
+
 def get_dataset_linked_creds_key() -> str:
     return LINKED_CREDS_FILENAME
 
 
 def get_dataset_linked_creds_lock_key() -> str:
     return VERSION_CONTROL_INFO_LOCK_FILENAME
 
@@ -233,7 +241,21 @@
         factor *= current_factor
         ls = key.split("_")
         ls[-1] = str(factor)
         final_key = "_".join(ls)
     else:
         final_key = f"_{key}_downsampled_{factor}"
     return posixpath.join(group, final_key)
+
+
+def get_pad_encoder_key(key: str, commit_id: str) -> str:
+    if commit_id == FIRST_COMMIT_ID:
+        return "/".join((key, ENCODED_PAD_NAMES_FOLDER, UNSHARDED_ENCODER_FILENAME))
+    return "/".join(
+        (
+            "versions",
+            commit_id,
+            key,
+            ENCODED_PAD_NAMES_FOLDER,
+            UNSHARDED_ENCODER_FILENAME,
+        )
+    )
```

### Comparing `deeplake-3.2.9/deeplake/util/link.py` & `deeplake-3.3.0/deeplake/util/link.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,17 @@
         if key1 == key2 or i == replaced_index:
             num_common_keys += 1
         else:
             break
     new_keys = current_link_creds.creds_keys[num_common_keys:]
     current_link_creds.creds_keys = old_link_creds.creds_keys
     current_link_creds.creds_mapping = old_link_creds.creds_mapping
-    current_link_creds.managed_creds_keys = old_link_creds.managed_creds_keys
+    current_link_creds.managed_creds_keys = old_link_creds.managed_creds_keys.union(
+        current_link_creds.managed_creds_keys
+    )
     current_link_creds.used_creds_keys = old_link_creds.used_creds_keys.union(
         current_link_creds.used_creds_keys
     )
     for key in new_keys:
         if key not in current_link_creds.creds_mapping:
             managed = key in current_link_creds.managed_creds_keys
             current_link_creds.add_creds_key(key, managed)
@@ -55,15 +57,15 @@
     storage: LRUCache,
     replaced_index: Optional[int] = None,
     managed_info: Optional[Tuple] = None,
 ):
     """Saves the linked creds info to storage."""
     storage = get_base_storage(storage)
     lock = Lock(storage, get_dataset_linked_creds_lock_key())
-    lock.acquire(timeout=10, force=True)
+    lock.acquire(timeout=10)
     key = get_dataset_linked_creds_key()
     try:
         data_bytes = storage[key]
     except KeyError:
         data_bytes = None
 
     if data_bytes is not None:
```

### Comparing `deeplake-3.2.9/deeplake/util/logging.py` & `deeplake-3.3.0/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/merge.py` & `deeplake-3.3.0/deeplake/util/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from deeplake.util.exceptions import (
     MergeConflictError,
     MergeMismatchError,
     MergeNotSupportedError,
     TensorDoesNotExistError,
 )
 from deeplake.util.remove_cache import create_read_copy_dataset
-from deeplake.util.version_control import auto_checkout, auto_commit, commit
+from deeplake.util.version_control import auto_checkout, auto_commit, commit, checkout
 from deeplake.core.version_control.commit_diff import CommitDiff
 from deeplake.core.version_control.commit_chunk_map import CommitChunkMap
 from deeplake.core.index.index import Index, IndexEntry
 from deeplake.util.keys import (
     get_sample_id_tensor_key,
     get_tensor_meta_key,
     get_tensor_info_key,
@@ -30,14 +30,16 @@
     get_creds_encoder_key,
     get_tensor_commit_chunk_map_key,
     get_tensor_commit_diff_key,
     get_chunk_id_encoder_key,
     get_sequence_encoder_key,
     get_dataset_meta_key,
 )
+
+from deeplake.core.meta.encode.pad import PadEncoder
 from os.path import dirname
 import numpy as np
 
 
 def merge(
     dataset,
     target_id: str,
@@ -48,57 +50,53 @@
     """Merge works by comparing the states of the dataset at the target commit and the current commit.
     The new tensors in the target are added. The deleted tensors in the target are removed if delete_removed_tensors is True.
     For the common tensors, we compare ids of the samples. The samples with newer ids are added to the dataset.
     For samples with the same ids, we compare the changes history of the sample and resolve conflicts according to the conflict_resolution argument.
     """
     version_state = dataset.version_state
     commit_node_map = version_state["commit_node_map"]
-    auto_checkout(dataset)
+    auto_checkout(dataset, flush_version_control_info=False)
     target_commit_id = sanitize_commit(target_id, version_state)
-    target_commit_id = auto_commit_target_commit(dataset, target_commit_id)
-
+    target_commit_id = auto_commit_target_commit(
+        dataset, target_commit_id, flush_version_control_info=False
+    )
     nodes: Dict[str, CommitNode] = {}
     nodes["original"] = original_node = version_state["commit_node"]
     nodes["target"] = target_node = commit_node_map[target_commit_id]
     lca_id = get_lowest_common_ancestor(original_node, target_node)
     target_ds = create_read_copy_dataset(dataset, target_commit_id)
 
     if lca_id == target_commit_id:
         print("No merge needed, target id is an ancestor of the current commit")
         return
     nodes["lca"] = commit_node_map[lca_id]
-
     (
         new_tensors,
         common_tensors,
         deleted_tensors,
     ) = get_new_common_deleted_tensors(dataset, target_ds, lca_id, force)
-
     merge_common_tensors(common_tensors, dataset, target_ds, nodes, conflict_resolution)
     copy_new_tensors(new_tensors, dataset, target_ds)
     delete_tensors(deleted_tensors, dataset, delete_removed_tensors)
     finalize_merge(dataset, nodes)
 
 
 def get_new_common_deleted_tensors(
     dataset, target_ds, lca_id: str, force: bool
 ) -> Tuple[Set[str], Set[str], Set[str]]:
     """Gets the names of tensors, that are new, common and deleted in the target commit"""
     original_tensors: Set[str] = set(dataset.tensors)
     all_original_tensors: Set[str] = set(dataset._all_tensors_filtered())
     check_id_tensors_exist(original_tensors, all_original_tensors)
-
     target_tensors: Set[str] = set(target_ds.tensors)
     all_target_tensors: Set[str] = set(target_ds._all_tensors_filtered())
     check_id_tensors_exist(target_tensors, all_target_tensors)
-
     lca_tensors = get_lca_tensors(dataset, lca_id)
     new_tensors = target_tensors - original_tensors
     common_tensors = target_tensors & original_tensors
-
     # present in dataset at lca, but deleted or renamed in target
     target_deleted_tensors = lca_tensors - target_tensors
 
     # present in dataset at lca, but deleted or renamed in original
     original_deleted_tensors = lca_tensors - original_tensors
 
     target_changes = target_ds.diff(lca_id, as_dict=True)
@@ -116,14 +114,15 @@
         new_tensors,
         common_tensors,
         original_deleted_tensors,
         target_deleted_tensors,
         original_renamed_tensors,
         target_renamed_tensors,
     )
+
     process_deleted_tensors(new_tensors, original_deleted_tensors, target_tensor_diff)
     return new_tensors, common_tensors, target_deleted_tensors
 
 
 def process_renamed_tensors(
     dataset,
     force,
@@ -181,28 +180,34 @@
     target_id = target_node.commit_id
     commit(dataset, f"Merge {target_id} into {dataset.branch}")
 
 
 def get_lca_tensors(dataset, lca_id: str) -> Set[str]:
     """Gets the names of tensors present in the lca commit"""
     original_id = dataset.pending_commit_id
-    dataset.checkout(lca_id)
+    checkout(dataset, lca_id)
     lca_tensors: Set[str] = set(dataset.tensors.keys())
-    dataset.checkout(original_id)
+    checkout(dataset, original_id)
     return lca_tensors
 
 
-def auto_commit_target_commit(dataset, target_commit_id: str) -> str:
+def auto_commit_target_commit(
+    dataset, target_commit_id: str, flush_version_control_info: bool = True
+) -> str:
     """Automatically commits the dataset at the target id if it is the head of a branch."""
     original_id = dataset.pending_commit_id
     original_branch = dataset.branch
-    dataset.checkout(target_commit_id)
-    auto_commit(dataset, f"Auto commit before merging into {original_branch}")
+    checkout(dataset, target_commit_id)
+    auto_commit(
+        dataset,
+        f"Auto commit before merging into {original_branch}",
+        flush_version_control_info=flush_version_control_info,
+    )
     target_commit_id = dataset.pending_commit_id
-    dataset.checkout(original_id)
+    checkout(dataset, original_id)
     return target_commit_id
 
 
 def get_changes_commit_ids_for_node(
     dataset, tensor_name: str, commit_node: Optional[CommitNode], lca_node: CommitNode
 ):
     changes_commit_map = defaultdict(list)
@@ -276,25 +281,44 @@
     conflict_resolution: Optional[str] = None,
 ):
     check_common_tensor_mismatches(tensor_names, dataset, target_dataset)
     new_samples_dict: Dict[str, List[int]] = {}
     updated_samples_dict: Dict[str, List[Tuple[int, int]]] = {}
     conflict_samples_dict: Dict[str, List[Tuple[int, int]]] = {}
     conflict_tensors = set()
+    idxs = {
+        tensor_name: find_new_updated_and_conflict_indexes(
+            tensor_name, dataset, target_dataset, nodes
+        )
+        for tensor_name in tensor_names
+    }
+    all_new_idxs = set()
+    for new_idxs, _, _ in idxs.values():
+        all_new_idxs.update(new_idxs)
+    for idx in all_new_idxs:
+        non_pad_found = False
+        for tensor_name in tensor_names:
+            target_engine = target_dataset[tensor_name].chunk_engine
+            enc = target_engine.chunk_id_encoder
+            if idx <= enc.num_samples:
+                if not target_engine.pad_encoder.is_padded(idx):
+                    non_pad_found = True
+                    break
+        if not non_pad_found:
+            for new_idxs, _, _ in idxs.values():
+                try:
+                    new_idxs.remove(idx)
+                except ValueError:
+                    pass
     for tensor_name in tensor_names:
         (
             new_indexes,
             updated_indexes,
             conflict_indexes,
-        ) = find_new_updated_and_conflict_indexes(
-            tensor_name,
-            dataset,
-            target_dataset,
-            nodes,
-        )
+        ) = idxs[tensor_name]
         new_samples_dict[tensor_name] = new_indexes
         updated_samples_dict[tensor_name] = updated_indexes
         if conflict_indexes:
             conflict_samples_dict[tensor_name] = conflict_indexes
             conflict_tensors.add(tensor_name)
 
     if conflict_tensors and conflict_resolution is None:
@@ -468,15 +492,14 @@
 ):
     """Merges actual data present in 2 versions of a common tensor."""
     if conflict_resolution == "theirs" and tensor_name in conflict_samples_dict:
         updated_samples_dict[tensor_name].extend(conflict_samples_dict[tensor_name])
 
     original_tensor = dataset[tensor_name]
     target_tensor = target_dataset[tensor_name]
-    id_tensor_name = get_sample_id_tensor_key(tensor_name)
 
     new_indexes = new_samples_dict[tensor_name]
     new_indexes.sort()
     is_class_label = target_tensor.meta.htype == "class_label"
     copy_class_labels = is_class_label
     if is_class_label:
         target_class_names = target_tensor.info.class_names
@@ -794,15 +817,31 @@
         start_row,
         end_row + 1,
         start,
         end,
     )
 
 
-def _mergs_tile_encoders(
+def _merge_pad_encoders(
+    src_pad_encoder: PadEncoder, dest_pad_encoder: PadEncoder, start: int, end: int
+) -> PadEncoder:
+    enc = PadEncoder()
+    idx = None
+    for i in range(start, end):
+        if src_pad_encoder.is_padded(i) and dest_pad_encoder.is_padded(i):
+            if idx is None:
+                idx = i
+        else:
+            if idx is not None:
+                enc.add_padding(idx, i - idx)
+                idx = None
+    return enc
+
+
+def _merge_tile_encoders(
     src_tile_encoder, dest_tile_encoder, start: int, end: int
 ) -> None:
     src_entries = src_tile_encoder.entries
     dest_entries = dest_tile_encoder.entries
     for i in range(start, end):
         e = src_entries.get(i)
         if e:
@@ -870,14 +909,16 @@
         dest_meta_length = (
             len(indices) if indices else sum(end - start for start, end in ranges)
         )
         dest_chunk_map = dest_eng.commit_chunk_map
         is_link = src_meta.is_link
         src_tile_enc = src_eng.tile_encoder
         dest_tile_enc = dest_eng.tile_encoder
+        src_pad_enc = src_eng.pad_encoder
+        dest_pad_enc = dest_eng.pad_encoder
         if is_link:
             src_creds_encoder = src_eng.creds_encoder
             dest_creds_encoder = dest_eng.creds_encoder
             dest_creds_encoder.is_dirty = True
         if is_seq:
             src_seq_encoder = src_eng.sequence_encoder
             dest_seq_encoder = dest_eng.sequence_encoder
@@ -893,15 +934,16 @@
                     )
                     dest_meta_seq_length += end - start
                     flat_ranges.append((start, end))
                 if is_link:
                     _merge_creds_encoders(
                         src_creds_encoder, dest_creds_encoder, start, end
                     )
-                _mergs_tile_encoders(src_tile_enc, dest_tile_enc, start, end)
+                _merge_tile_encoders(src_tile_enc, dest_tile_enc, start, end)
+                _merge_pad_encoders(src_pad_enc, dest_pad_enc, start, end)
                 (
                     chunks_to_copy,
                     left_edge_samples,
                     right_edge_samples,
                 ) = _get_required_chunks_for_range(src_tensor, start, end)
                 if left_edge_samples:
                     s, e = left_edge_samples
```

### Comparing `deeplake-3.2.9/deeplake/util/modified.py` & `deeplake-3.3.0/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/notebook.py` & `deeplake-3.3.0/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/object_3d/mesh.py` & `deeplake-3.3.0/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.3.0/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.3.0/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.3.0/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.3.0/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.3.0/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.3.0/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.3.0/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.3.0/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.3.0/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/path.py` & `deeplake-3.3.0/deeplake/util/path.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pathlib
 import posixpath
-from typing import Optional, Union
+from typing import Optional, Union, Tuple
 from deeplake.core.storage.provider import StorageProvider
 from deeplake.util.tag import process_hub_path
 from deeplake.constants import HUB_CLOUD_DEV_USERNAME
 from deeplake.util.exceptions import InvalidDatasetNameException
 import glob
 import os
 import re
@@ -99,14 +99,21 @@
 
 def convert_pathlib_to_string_if_needed(path: Union[str, pathlib.Path]) -> str:
     if isinstance(path, pathlib.Path):
         path = str(path)
     return path
 
 
+def process_dataset_path(path: Union[str, pathlib.Path]) -> Tuple[str, Optional[str]]:
+    dataset_path, at, address = str(path).partition("@")
+    if not address:
+        address = None  # type: ignore
+    return dataset_path, address
+
+
 def get_org_id_and_ds_name(path):
     if is_hub_cloud_path(path):
         _, org_id, ds_name, subdir = process_hub_path(path)
         if subdir:
             ds_name += "/" + subdir
     else:
         org_id = HUB_CLOUD_DEV_USERNAME
```

### Comparing `deeplake-3.2.9/deeplake/util/pretty_print.py` & `deeplake-3.3.0/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/remove_cache.py` & `deeplake-3.3.0/deeplake/util/remove_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 import deeplake
-from deeplake.core.storage.provider import StorageProvider
+from deeplake.core.storage import StorageProvider
 from deeplake.core.storage.lru_cache import LRUCache
 from deeplake.core.storage import MemoryProvider
 from deeplake.core.index import Index
 from deeplake.constants import MB
 
 
 def remove_memory_cache(storage: StorageProvider):
@@ -24,14 +24,16 @@
         else:
             storage = storage.cache_storage
     return storage
 
 
 def get_dataset_with_zero_size_cache(ds):
     """Returns a dataset with same storage but cache size set to zero."""
+    if not ds._read_only:
+        ds.flush()
     ds_base_storage = get_base_storage(ds.storage)
     zero_cache_storage = LRUCache(MemoryProvider(), ds_base_storage, 0)
     commit_id = ds.pending_commit_id
     index = Index.from_json(ds.index.to_json())
     ds = deeplake.core.dataset.dataset_factory(
         path=ds.path,
         storage=zero_cache_storage,
@@ -71,12 +73,13 @@
         storage,
         group_index=dataset.group_index,
         read_only=True,
         public=dataset.public,
         token=dataset._token,
         verbose=False,
         path=dataset.path,
+        version_state=dataset.version_state,
     )
     if commit_id is not None:
         ds.checkout(commit_id)
     ds.index = index
     return ds
```

### Comparing `deeplake-3.2.9/deeplake/util/scheduling.py` & `deeplake-3.3.0/deeplake/util/scheduling.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,40 +55,44 @@
         ]
         schedule = []
         for indexes_list in nested_schedule:
             schedule.extend(indexes_list)
     return schedule
 
 
+def calculate_absolute_lengths(percent_lengths, absolute_length):
+    subset_lengths: List[int] = []
+    for i, frac in enumerate(percent_lengths):
+        if frac < 0 or frac > 1:
+            raise ValueError(f"Fraction at index {i} is not between 0 and 1")
+        n_items_in_split = int(
+            math.floor(absolute_length * frac)  # type: ignore[arg-type]
+        )
+        subset_lengths.append(n_items_in_split)
+    remainder = absolute_length - sum(subset_lengths)  # type: ignore[arg-type]
+    # add 1 to all the percent_lengths in round-robin fashion until the remainder is 0
+    for i in range(remainder):
+        idx_to_add_at = i % len(subset_lengths)
+        subset_lengths[idx_to_add_at] += 1
+    percent_lengths = subset_lengths
+    for i, length in enumerate(percent_lengths):
+        if length == 0:
+            warnings.warn(
+                f"Length of split at index {i} is 0. "
+                f"This might result in an empty dataset."
+            )
+    return percent_lengths
+
+
 def create_random_split_views(dataset, lengths):
     from deeplake.enterprise.convert_to_libdeeplake import import_indra_api
 
     import_indra_api()
     if math.isclose(sum(lengths), 1) and sum(lengths) <= 1:
-        subset_lengths: List[int] = []
-        for i, frac in enumerate(lengths):
-            if frac < 0 or frac > 1:
-                raise ValueError(f"Fraction at index {i} is not between 0 and 1")
-            n_items_in_split = int(
-                math.floor(len(dataset) * frac)  # type: ignore[arg-type]
-            )
-            subset_lengths.append(n_items_in_split)
-        remainder = len(dataset) - sum(subset_lengths)  # type: ignore[arg-type]
-        # add 1 to all the lengths in round-robin fashion until the remainder is 0
-        for i in range(remainder):
-            idx_to_add_at = i % len(subset_lengths)
-            subset_lengths[idx_to_add_at] += 1
-        lengths = subset_lengths
-        for i, length in enumerate(lengths):
-            if length == 0:
-                warnings.warn(
-                    f"Length of split at index {i} is 0. "
-                    f"This might result in an empty dataset."
-                )
-
+        lengths = calculate_absolute_lengths(lengths, len(dataset))
     if sum(lengths) != len(dataset):  # type: ignore[arg-type]
         raise ValueError(
             "Sum of input lengths does not equal the length of the input dataset!"
         )
 
     primary_tensor = find_primary_tensor(dataset)
     schedule = create_fetching_schedule(
```

### Comparing `deeplake-3.2.9/deeplake/util/shape_interval.py` & `deeplake-3.3.0/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/split.py` & `deeplake-3.3.0/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/storage.py` & `deeplake-3.3.0/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/tag.py` & `deeplake-3.3.0/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/tests/test_auto.py` & `deeplake-3.3.0/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.3.0/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.3.0/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/tests/test_read.py` & `deeplake-3.3.0/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.3.0/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/tests/test_split.py` & `deeplake-3.3.0/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/tests/test_version_control.py` & `deeplake-3.3.0/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/util/transform.py` & `deeplake-3.3.0/deeplake/util/transform.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,310 +6,329 @@
 from json.decoder import JSONDecodeError
 from deeplake.core.linked_chunk_engine import LinkedChunkEngine
 from deeplake.core.meta.tensor_meta import TensorMeta
 from deeplake.core.storage import StorageProvider, MemoryProvider, LRUCache
 from deeplake.core.chunk_engine import ChunkEngine
 from deeplake.core.transform.transform_dataset import TransformDataset
 from deeplake.core.index import Index
+from deeplake.core.tensor import Tensor
 
-from deeplake.constants import MB, TRANSFORM_PROGRESSBAR_UPDATE_INTERVAL
-from deeplake.util.remove_cache import get_base_storage
+from deeplake.constants import (
+    MB,
+    TRANSFORM_PROGRESSBAR_UPDATE_INTERVAL,
+    TRANSFORM_RECHUNK_AVG_SIZE_BOUND,
+)
+from deeplake.util.dataset import try_flushing
+from deeplake.util.remove_cache import (
+    get_base_storage,
+    get_dataset_with_zero_size_cache,
+)
 from deeplake.util.keys import get_tensor_meta_key
+from deeplake.util.version_control import auto_checkout, load_meta
 from deeplake.util.exceptions import (
     InvalidInputDataError,
     InvalidOutputDatasetError,
     InvalidTransformDataset,
     TensorMismatchError,
+    TensorDoesNotExistError,
+    TransformError,
+    SampleAppendError,
 )
 
 import posixpath
 import time
 
 try:
     import pandas as pd  # type: ignore
 except ImportError:
     pd = None
 
 
 def transform_sample(
     sample: Any,
     pipeline,
+    tensors,
 ) -> TransformDataset:
     """Calls all the functions one after the other on a single sample.
     Can return 0 or more samples.
 
     Args:
         sample: The sample on which the pipeline of functions is to be applied.
         pipeline (Pipeline): The Sequence of functions to apply on the sample.
-
-    Raises:
-        InvalidTransformDataset: If number of tensors were inconsistent between all transform datasets.
+        tensors: List of tensors in output.
 
     Returns:
         TransformDataset: A transform dataset containing all the samples that were generated.
     """
-
-    result = sample
+    out = sample
     for index in range(len(pipeline)):
         transform_fn = pipeline.functions[index]
         fn, args, kwargs = transform_fn.func, transform_fn.args, transform_fn.kwargs
 
-        if isinstance(result, TransformDataset):
-            all_samples_out = []
-            for item in result:
-                samples_out = TransformDataset()
-                fn(item, samples_out, *args, **kwargs)
-                validate_transform_dataset(samples_out)
-                all_samples_out.append(samples_out)
-            result = combine_transform_datasets(all_samples_out)
-            try:
+        if isinstance(out, TransformDataset):
+            result = TransformDataset(tensors)
+            for item in out:
+                fn(item, result, *args, **kwargs)
                 validate_transform_dataset(result)
-            except InvalidTransformDataset:
-                raise InvalidTransformDataset(
-                    "One or more of the TransformDatasets returned had different number of tensors. Always ensure that all outputs have exactly the same tensors and equal number of samples in each tensor."
-                )
+            out = result
         else:
-            samples_out = TransformDataset()
-            fn(result, samples_out, *args, **kwargs)
-            validate_transform_dataset(samples_out)
-            result = samples_out
-    return result
-
-
-def combine_transform_datasets(datasets: List[TransformDataset]):
-    """Combines multiple TransformDataset into a single transform dataset."""
-    final_ds = TransformDataset()
-    for ds in datasets:
-        for tensor in ds.tensors:
-            input_tensor = ds[tensor]
-            output_tensor = final_ds[tensor]
-            if input_tensor._numpy_only:
-                for batch in input_tensor.numpy():
-                    output_tensor.extend(batch)
-            else:
-                output_tensor.extend(input_tensor.numpy_compressed())
-    return final_ds
+            result = TransformDataset(tensors)
+            fn(out, result, *args, **kwargs)
+            validate_transform_dataset(result)
+            out = result
+    return out
 
 
 def validate_transform_dataset(dataset: TransformDataset):
     """Checks if the length of all the tensors is equal. Raises exception if not equal."""
-    lengths = [len(dataset[tensor]) for tensor in dataset.tensors]
+    data = dataset.data
+    lengths = [
+        len(data[tensor])
+        for tensor in data
+        if (not data[tensor].is_group and len(data[tensor]) > 0)
+    ]
     if any(length != lengths[0] for length in lengths):
-        raise InvalidTransformDataset
+        raise InvalidTransformDataset(
+            "The number of samples added to each tensor in transform should be the same."
+        )
 
 
 def is_empty_transform_dataset(dataset: TransformDataset):
     """Checks if there is any data in the TransformDataset. Returns True if empty, False otherwise."""
     return all(len(dataset[tensor]) == 0 for tensor in dataset.tensors)
 
 
 def store_data_slice(transform_input: Tuple) -> Dict:
     """Takes a slice of the original data and iterates through it and stores it in the actual storage.
     The tensor_meta and chunk_id_encoder are not stored to the storage to prevent overwrites/race conditions b/w workers.
     They are instead stored in memory and returned."""
     return store_data_slice_with_pbar(None, transform_input)
 
 
-def store_data_slice_with_pbar(pg_callback, transform_input: Tuple) -> Dict:
-    data_slice, output_storage, inp = transform_input
-    (
-        group_index,
-        tensors,
-        visible_tensors,
-        label_temp_tensors,
-        actual_tensors,
-        pipeline,
-        version_state,
-        link_creds,
-        skip_ok,
-        extend_only,
-    ) = inp
-    all_chunk_engines = create_worker_chunk_engines(
-        tensors, label_temp_tensors, output_storage, version_state, link_creds
+def _normalize_pg(pg_callback, num_tensors):
+    def inner(num_samples):
+        return pg_callback(num_samples / num_tensors)
+
+    return inner
+
+
+def _extend_data_slice(
+    data_slice, offset, transform_dataset, transform_fn, pg_callback
+):
+    extend_fn, args, kwargs = (
+        transform_fn.func,
+        transform_fn.args,
+        transform_fn.kwargs,
     )
+    extend_fn(data_slice, transform_dataset, *args, **kwargs)
+    data = transform_dataset.data
+    updated_tensors = set(k for k in data if not data[k].is_group and len(data[k]) > 0)
+    if pg_callback is not None:
+        pg_callback = _normalize_pg(pg_callback, len(updated_tensors))
+    transform_dataset.set_pg_callback(pg_callback)
+    transform_dataset.flush()
 
-    if isinstance(data_slice, deeplake.Dataset):
-        data_slice = add_cache_to_dataset_slice(data_slice, tensors)
 
-    if extend_only:
-        extend_data_slice(
-            data_slice,
-            pipeline,
-            all_chunk_engines,
-            group_index,
-            pg_callback,
-        )
-    else:
-        transform_data_slice_and_append(
-            data_slice,
-            pipeline,
-            visible_tensors,
-            label_temp_tensors,
-            actual_tensors,
-            all_chunk_engines,
-            group_index,
-            pg_callback,
-            skip_ok,
+def _check_pipeline(out, tensors, skip_ok):
+    data = out.data
+    result_keys = set(k for k in data if not data[k].is_group and len(data[k]) > 0)
+
+    if skip_ok:
+        if not result_keys.issubset(tensors):
+            raise TensorMismatchError(list(tensors), list(result_keys), skip_ok)
+    elif set(result_keys) != set(tensors):
+        raise TensorMismatchError(list(tensors), list(result_keys), skip_ok)
+
+
+def write_sample_to_transform_dataset(out, transform_dataset):
+    if not is_empty_transform_dataset(out):
+        for tensor in out.tensors:
+            out_tensor = out[tensor]
+            transform_tensor = transform_dataset[tensor]
+            if transform_tensor.numpy_only and out_tensor.numpy_only:
+                for item in out_tensor.items:
+                    transform_tensor.extend(item)
+            else:
+                out_tensor.non_numpy_only()
+                transform_tensor.extend(out_tensor.items)
+            out_tensor.items.clear()
+
+
+def _handle_transform_error(
+    data_slice,
+    offset,
+    transform_dataset,
+    pipeline,
+    tensors,
+    end_input_idx,
+    ignore_errors,
+):
+    start_input_idx = transform_dataset.start_input_idx
+    for i in range(start_input_idx, end_input_idx + 1):
+        sample = (
+            data_slice[i : i + 1]
+            if pd and isinstance(data_slice, pd.DataFrame)
+            else data_slice[i]
         )
+        try:
+            out = transform_sample(sample, pipeline, tensors)
 
-    # retrieve relevant objects from memory
+            write_sample_to_transform_dataset(out, transform_dataset)
+
+            transform_dataset.flush()
+        except Exception as e:
+            if isinstance(e, SampleAppendError) and ignore_errors:
+                continue
+            raise TransformError(offset + i, sample) from e
+
+
+def _transform_and_append_data_slice(
+    data_slice,
+    offset,
+    transform_dataset,
+    pipeline,
+    tensors,
+    skip_ok,
+    pg_callback,
+    ignore_errors,
+):
+    n = len(data_slice)
+
+    pipeline_checked = False
+
+    for i, sample in enumerate(
+        (data_slice[i : i + 1] for i in range(n))
+        if pd and isinstance(data_slice, pd.DataFrame)
+        else data_slice
+    ):
+        try:
+            transform_dataset.set_start_input_idx(i)
+
+            try:
+                out = transform_sample(sample, pipeline, tensors)
+            except SampleAppendError as e:
+                if ignore_errors:
+                    continue
+                raise TransformError(offset + i, sample) from e
+
+            if not pipeline_checked:
+                _check_pipeline(out, tensors, skip_ok)
+                pipeline_checked = True
+
+            write_sample_to_transform_dataset(out, transform_dataset)
+
+            if i == n - 1:
+                transform_dataset.flush()
+            else:
+                transform_dataset.check_flush()
+
+            if pg_callback is not None:
+                pg_callback(1)
+        except SampleAppendError:
+            # failure at chunk_engine
+            # retry one sample at a time
+            _handle_transform_error(
+                data_slice,
+                offset,
+                transform_dataset,
+                pipeline,
+                tensors,
+                i,
+                ignore_errors,
+            )
+            continue
+
+
+def _retrieve_memory_objects(all_chunk_engines):
     all_tensor_metas = {}
     all_chunk_id_encoders = {}
     all_tile_encoders = {}
     all_sequence_encoders = {}
+    all_pad_encoders = {}
     all_chunk_maps = {}
     all_commit_diffs = {}
     all_creds_encoders = {}
     all_hash_label_maps = {}
     for tensor, chunk_engine in all_chunk_engines.items():
         chunk_engine.cache.flush()
         chunk_engine.meta_cache.flush()
         all_tensor_metas[tensor] = chunk_engine.tensor_meta
         all_chunk_id_encoders[tensor] = chunk_engine.chunk_id_encoder
         all_tile_encoders[tensor] = chunk_engine.tile_encoder
         all_sequence_encoders[tensor] = chunk_engine.sequence_encoder
+        all_pad_encoders[tensor] = chunk_engine.pad_encoder
         all_chunk_maps[tensor] = chunk_engine.commit_chunk_map
         all_commit_diffs[tensor] = chunk_engine.commit_diff
         all_creds_encoders[tensor] = chunk_engine.creds_encoder
         if chunk_engine._is_temp_label_tensor:
             all_hash_label_maps[tensor] = chunk_engine._hash_label_map
 
     return {
         "tensor_metas": all_tensor_metas,
         "chunk_id_encoders": all_chunk_id_encoders,
         "sequence_encoders": all_sequence_encoders,
+        "pad_encoders": all_pad_encoders,
         "tile_encoders": all_tile_encoders,
         "commit_chunk_maps": all_chunk_maps,
         "commit_diffs": all_commit_diffs,
         "creds_encoders": all_creds_encoders,
         "hash_label_maps": all_hash_label_maps,
     }
 
 
-def _transform_sample_and_update_chunk_engines(
-    sample,
-    pipeline,
-    tensors: List[str],
-    label_temp_tensors: Dict[str, str],
-    actual_tensors: Optional[List[str]],
-    all_chunk_engines: Dict[str, ChunkEngine],
-    group_index: str,
-    skip_ok: bool = False,
-):
-    result = transform_sample(sample, pipeline)
-    if is_empty_transform_dataset(result):
-        return
-    result_resolved = {
-        posixpath.join(group_index, k): result[k] for k in result.tensors
-    }
-    result = result_resolved  # type: ignore
-    result_keys = set(result.keys())
-
-    # compare with actual tensors if there are temporary tensors
-    actual_tensors = actual_tensors or tensors
-    if skip_ok:
-        if not result_keys.issubset(actual_tensors):
-            raise TensorMismatchError(list(actual_tensors), list(result_keys), skip_ok)
-    elif set(result_keys) != set(actual_tensors):
-        raise TensorMismatchError(list(actual_tensors), list(result_keys), skip_ok)
-
-    for tensor, value in result.items():
-        chunk_engine = all_chunk_engines[label_temp_tensors.get(tensor) or tensor]
-        callback = chunk_engine._transform_callback
-        if value._numpy_only:
-            for batch in value.numpy_compressed():
-                chunk_engine.extend(batch, link_callback=callback)
-        else:
-            chunk_engine.extend(value.numpy_compressed(), link_callback=callback)
-        value.items.clear()
-
-
-def normalize_pg(pg_callback, num_tensors):
-    def inner(num_samples):
-        return pg_callback(num_samples / num_tensors)
-
-    return inner
-
-
-def extend_data_slice(
-    data_slice,
-    pipeline,
-    all_chunk_engines,
-    group_index: str,
-    pg_callback,
-):
-    transform_fn = pipeline.functions[0]
-    extend_fn, args, kwargs = transform_fn.func, transform_fn.args, transform_fn.kwargs
-    result = TransformDataset()
-    extend_fn(data_slice, result, *args, **kwargs)
-    result_resolved = {
-        posixpath.join(group_index, k): result[k] for k in result.tensors
-    }
-    result = result_resolved  # type: ignore
+def store_data_slice_with_pbar(pg_callback, transform_input: Tuple) -> Dict:
+    data_slice, offset, output_storage, inp = transform_input
+    (
+        group_index,
+        tensors,
+        visible_tensors,
+        label_temp_tensors,
+        pipeline,
+        version_state,
+        link_creds,
+        skip_ok,
+        extend_only,
+        cache_size,
+        ignore_errors,
+    ) = inp
+    all_chunk_engines = create_worker_chunk_engines(
+        tensors, label_temp_tensors, output_storage, version_state, link_creds
+    )
 
-    if pg_callback is not None:
-        pg_callback = normalize_pg(pg_callback, len(result))
+    if isinstance(data_slice, deeplake.Dataset):
+        data_slice = add_cache_to_dataset_slice(data_slice, tensors)
 
-    for tensor, value in result.items():
-        chunk_engine = all_chunk_engines[tensor]
-        callback = chunk_engine._transform_callback
-        if value._numpy_only:
-            for batch in value.numpy_compressed():
-                chunk_engine.extend(
-                    batch, link_callback=callback, pg_callback=pg_callback
-                )
-        else:
-            chunk_engine.extend(
-                value.numpy_compressed(),
-                link_callback=callback,
-                pg_callback=pg_callback,
-            )
-        value.items.clear()
+    rel_tensors = [posixpath.relpath(tensor, group_index) for tensor in visible_tensors]
 
+    transform_dataset = TransformDataset(
+        rel_tensors,
+        all_chunk_engines,
+        group_index,
+        label_temp_tensors,
+        cache_size=cache_size,
+    )
 
-def transform_data_slice_and_append(
-    data_slice,
-    pipeline,
-    tensors: List[str],
-    label_temp_tensors: Dict[str, str],
-    actual_tensors: Optional[List[str]],
-    all_chunk_engines: Dict[str, ChunkEngine],
-    group_index: str,
-    pg_callback=None,
-    skip_ok=False,
-) -> None:
-    """Transforms the data_slice with the pipeline and adds the resultant samples to chunk_engines."""
-    n = len(data_slice)
-    last_reported_time = time.time()
-    last_reported_num_samples = 0
-    for i, sample in enumerate(
-        (data_slice[i : i + 1] for i in range(n))
-        if pd and isinstance(data_slice, pd.DataFrame)
-        else data_slice
-    ):
-        _transform_sample_and_update_chunk_engines(
-            sample,
+    if extend_only:
+        _extend_data_slice(
+            data_slice, offset, transform_dataset, pipeline.functions[0], pg_callback
+        )
+    else:
+        _transform_and_append_data_slice(
+            data_slice,
+            offset,
+            transform_dataset,
             pipeline,
-            tensors,
-            label_temp_tensors,
-            actual_tensors,
-            all_chunk_engines,
-            group_index,
+            rel_tensors,
             skip_ok,
+            pg_callback,
+            ignore_errors,
         )
-        if pg_callback is not None:
-            curr_time = time.time()
-            if (
-                curr_time - last_reported_time > TRANSFORM_PROGRESSBAR_UPDATE_INTERVAL
-                or i == n - 1
-            ):
-                num_samples = i + 1
-                pg_callback(num_samples - last_reported_num_samples)
-                last_reported_num_samples = num_samples
-                last_reported_time = curr_time
+
+    # retrieve relevant objects from memory
+    return _retrieve_memory_objects(all_chunk_engines)
 
 
 def create_worker_chunk_engines(
     tensors: List[str],
     label_temp_tensors: Dict[str, str],
     output_storage: StorageProvider,
     version_state,
@@ -320,15 +339,19 @@
     """
     all_chunk_engines: Dict[str, ChunkEngine] = {}
     num_tries = 1000
     for tensor in tensors:
         for i in range(num_tries):
             try:
                 # TODO: replace this with simply a MemoryProvider once we get rid of cachable
-                memory_cache = LRUCache(MemoryProvider(), MemoryProvider(), 64 * MB)
+                memory_cache = LRUCache(
+                    MemoryProvider(),
+                    MemoryProvider(),
+                    64 * MB,
+                )
                 memory_cache.autoflush = False
                 storage_cache = LRUCache(MemoryProvider(), output_storage, 64 * MB)
                 storage_cache.autoflush = False
 
                 # this chunk engine is used to retrieve actual tensor meta and chunk_size
                 storage_chunk_engine = ChunkEngine(tensor, storage_cache, version_state)
                 existing_meta = storage_chunk_engine.tensor_meta
@@ -462,16 +485,32 @@
 
     names_desc = ", ".join(func_names)
     return f"Evaluating [{names_desc}]"
 
 
 def create_slices(data_in, num_workers):
     size = math.ceil(len(data_in) / num_workers)
-    ret = [data_in[i * size : (i + 1) * size] for i in range(num_workers)]
-    return ret
+
+    if isinstance(data_in, Tensor):
+        ret = [
+            Tensor(data_in.key, data_in.dataset)[i * size : (i + 1) * size]
+            for i in range(num_workers)
+        ]
+    else:
+        ret = [data_in[i * size : (i + 1) * size] for i in range(num_workers)]
+
+    if isinstance(data_in, deeplake.Dataset):
+        for ds in ret:
+            ds.version_state["full_tensors"] = {}
+            _tensors = ds.version_state["full_tensors"]
+            for tensor_key in data_in.version_state["tensor_names"].values():
+                _tensors[tensor_key] = Tensor(tensor_key, ds)
+
+    offsets = list(range(0, len(data_in), size))
+    return ret, offsets
 
 
 def get_old_chunk_paths(target_ds, generated_tensors, overwrite):
     old_chunk_paths = []
     if overwrite:
         for key in generated_tensors:
             tensor = target_ds[key]
@@ -528,7 +567,108 @@
         return result
     final = defaultdict(list)
     keys = list(result[0].keys())
     for item in result:
         for key in keys:
             final[key].append(item[key])
     return final
+
+
+def rechunk_if_necessary(ds):
+    with ds:
+        for tensor in ds.tensors:
+            try:
+                tensor = ds[tensor]
+            # temp tensors
+            except TensorDoesNotExistError:
+                continue
+            if not tensor.meta.sample_compression and not tensor.meta.chunk_compression:
+                engine = tensor.chunk_engine
+                num_chunks = engine.num_chunks
+                if num_chunks > 1:
+                    max_shape = tensor.meta.max_shape
+                    if len(max_shape) > 0:
+                        avg_chunk_size = engine.get_avg_chunk_size()
+                        if (
+                            avg_chunk_size is not None
+                            and avg_chunk_size
+                            < TRANSFORM_RECHUNK_AVG_SIZE_BOUND * engine.min_chunk_size
+                        ):
+                            enc = tensor.chunk_engine.chunk_id_encoder
+                            row = 0
+                            while row < len(enc._encoded) - 1:
+                                encoded = enc._encoded
+                                chunk_id = encoded[row, 0]
+                                chunk = engine.get_chunk_from_chunk_id(chunk_id)
+                                engine._check_rechunk(chunk, row)
+                                # np.delete will replace enc._encoded with new array
+                                # so this check works
+                                rechunked = len(encoded) != len(enc._encoded)
+                                if not rechunked:
+                                    row += 1
+
+
+def close_states(compute_provider, pbar, pqueue):
+    compute_provider.close()
+    if pbar and hasattr(pbar, "close"):
+        pbar.close()
+    if pqueue and hasattr(pqueue, "close"):
+        pqueue.close()
+
+
+def reload_and_rechunk(
+    overwrite,
+    original_data_in,
+    target_ds,
+    initial_autoflush,
+    pad_data_in,
+    initial_padding_state,
+    kwargs,
+    completed=True,
+):
+    if overwrite:
+        original_data_in.storage.clear_cache_without_flush()
+        load_meta(original_data_in)
+        if pad_data_in and not initial_padding_state:
+            original_data_in._disable_padding()
+        if completed and not kwargs.get("disable_rechunk"):
+            rechunk_if_necessary(original_data_in)
+    else:
+        load_meta(target_ds)
+        if completed:
+            target_ds.storage.autoflush = initial_autoflush
+            if not kwargs.get("disable_rechunk"):
+                rechunk_if_necessary(target_ds)
+
+
+def check_checkpoint_interval(data_in, checkpoint_interval, num_workers, overwrite):
+    if num_workers > 0 and checkpoint_interval % num_workers != 0:
+        raise ValueError(
+            "checkpoint_interval should be a multiple of num_workers if num_workers > 0"
+        )
+    if checkpoint_interval > len(data_in):
+        raise ValueError(
+            "checkpoint_interval should be less than or equal to the length of data_in"
+        )
+    if checkpoint_interval < len(data_in) / 10:
+        warnings.warn(
+            "checkpoint_interval is less than 10% of the length of data_in, this can lead to too many commits, consider increasing checkpoint_interval."
+        )
+    if overwrite:
+        raise ValueError(
+            "checkpoint_interval > 0 and ds_out is None. Cannot checkpoint during inplace transform."
+        )
+
+
+def prepare_data_in(data_in, pad_data_in, overwrite):
+    initial_padding_state = None
+    original_data_in = data_in
+    if isinstance(data_in, deeplake.Dataset):
+        try_flushing(data_in)
+        if overwrite:
+            auto_checkout(data_in)
+        original_data_in = data_in
+        data_in = get_dataset_with_zero_size_cache(data_in)
+        if pad_data_in:
+            initial_padding_state = data_in._pad_tensors
+            data_in._enable_padding()
+    return data_in, original_data_in, initial_padding_state
```

### Comparing `deeplake-3.2.9/deeplake/util/version_control.py` & `deeplake-3.3.0/deeplake/util/version_control.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random
 import time
 import hashlib
 import pickle
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, List
 import warnings
 from deeplake.client.log import logger
 from deeplake.constants import FIRST_COMMIT_ID
 from deeplake.core.fast_forwarding import ffw_dataset_meta
 from deeplake.core.meta.dataset_meta import DatasetMeta
 from deeplake.core.storage.deeplake_memory_object import DeepLakeMemoryObject
 from deeplake.core.storage.lru_cache import LRUCache
@@ -29,18 +29,22 @@
     get_tensor_commit_diff_key,
     get_tensor_info_key,
     get_tensor_meta_key,
     get_tensor_tile_encoder_key,
     get_version_control_info_key,
     get_version_control_info_key_old,
     get_version_control_info_lock_key,
+    get_commit_info_key,
 )
+from deeplake.constants import COMMIT_INFO_FILENAME
 from deeplake.util.remove_cache import get_base_storage
 from deeplake.hooks import dataset_committed
 from datetime import datetime
+
+import posixpath
 import json
 
 
 def _version_info_to_json(info):
     commit_node_map, branch_commit_map = (
         info["commit_node_map"],
         info["branch_commit_map"],
@@ -64,14 +68,17 @@
 def _version_info_from_json(info):
     commits, branch_commit_map = info["commits"], info["branches"]
     commit_node_map = {}
     stack = [FIRST_COMMIT_ID]
     while stack:
         commit_id = stack.pop()
         commit_data = commits[commit_id]
+        branch_commit_map[
+            commit_data["branch"]
+        ]  # we will rebuild version info if this fails
         node = CommitNode(commit_data["branch"], commit_id)
         node.commit_message = commit_data["commit_message"]
         commit_time = commit_data["commit_time"]
         node.commit_time = (
             None if commit_time is None else datetime.fromtimestamp(commit_time)
         )
         node.commit_user_name = commit_data["commit_user_name"]
@@ -92,87 +99,102 @@
     hsh.update(random.randrange(0, 1000000).to_bytes(4, "big"))
     return hsh.hexdigest()
 
 
 def integrity_check(dataset):
     try:
         rev_tensor_names = {v: k for k, v in dataset.meta.tensor_names.items()}
-        for k in dataset.meta.tensor_names:
-            t = dataset[k]
+        for k, t in dataset._tensors(include_disabled=False).items():
             n1 = t.meta.length
             engine = t.chunk_engine
             n2 = engine.chunk_id_encoder.num_samples
             if n1 != n2:
                 raise ValueError(
                     f"Tensor meta and chunk id encoder have different number of samples ({n1} and {n2} respectively) for tensor {k}."
                 )
             num_sequences = getattr(engine.sequence_encoder, "num_samples", None)
             for l, info in t.meta.links.items():
                 l = rev_tensor_names[l]
+                l = posixpath.relpath(l, dataset.group_index)
                 if num_sequences is not None and not info["flatten_sequence"]:
                     n2 = num_sequences
                 else:
                     n2 = n1
                 n3 = dataset[l].meta.length
                 if n2 != n3:
                     raise ValueError(
                         f"Tensor {k} and its linked tensor {l} have different number of samples ({n2} and {n3} respectively)."
                     )
             engine.tile_encoder
 
             engine.creds_encoder
     except Exception as e:
         raise DatasetCorruptError(
-            f"The HEAD node of the branch {dataset.branch} of this dataset is in a corrupted state and is likely not recoverable. Please run `ds.reset()` to revert the uncommitted changes in order to continue making updates on this branch."
+            f"The HEAD node of the branch {dataset.branch} of this dataset is in a corrupted state and is likely not recoverable.",
+            "Please run `ds.reset()` to revert the uncommitted changes in order to continue making updates on this branch.",
         ) from e
 
 
-def commit(dataset, message: Optional[str] = None, hash: Optional[str] = None) -> None:
+def commit(
+    dataset,
+    message: Optional[str] = None,
+    hash: Optional[str] = None,
+    flush_version_control_info: bool = True,
+    reload_meta: bool = True,
+) -> None:
     """Modifies the version state to reflect the commit and also copies required data to the new commit directory."""
     storage = dataset.storage
     version_state = dataset.version_state
     storage.check_readonly()
     integrity_check(dataset)
     # if not the head node, checkout to an auto branch that is newly created
-    auto_checkout(dataset)
+    auto_checkout(dataset, flush_version_control_info=False)
     stored_commit_node: CommitNode = version_state["commit_node"]
     stored_commit_id = version_state["commit_id"]
     if hash:
         if hash in version_state["commit_node_map"]:
             raise CommitError(f"Commit {hash} already exists")
-        version_state["commit_id"] = hash
     else:
-        version_state["commit_id"] = generate_hash()
-    new_node = CommitNode(version_state["branch"], version_state["commit_id"])
+        hash = generate_hash()
+    version_state["commit_id"] = hash
+    new_node = CommitNode(version_state["branch"], hash)
     version_state["commit_node"].add_successor(new_node, message)
     version_state["commit_node"] = new_node
     version_state["branch_commit_map"][version_state["branch"]] = version_state[
         "commit_id"
     ]
-    version_state["commit_node_map"][version_state["commit_id"]] = new_node
-    copy_metas(stored_commit_id, version_state["commit_id"], storage, version_state)
-    create_commit_chunk_maps(version_state["commit_id"], storage, version_state)
+    version_state["commit_node_map"][hash] = new_node
+    copy_metas(stored_commit_id, hash, storage)
+    create_commit_chunk_maps(stored_commit_id, hash, storage)
     discard_old_metas(stored_commit_id, storage, version_state["full_tensors"])
-    load_meta(dataset)
+    if reload_meta:
+        load_meta(dataset)
 
     commit_time = stored_commit_node.commit_time
     commit_message = stored_commit_node.commit_message
     author = stored_commit_node.commit_user_name
-    save_version_info(version_state, storage)
+    if flush_version_control_info:
+        save_version_info(version_state, storage)
+        save_commit_info(stored_commit_node, storage)
+        save_commit_info(new_node, storage)
+    else:
+        stored_commit_node._info_updated = True
+        new_node._info_updated = True
     dataset._send_commit_event(
         commit_message=commit_message, commit_time=commit_time, author=author
     )
     dataset_committed(dataset)
 
 
 def checkout(
     dataset,
     address: str,
     create: bool = False,
     hash: Optional[str] = None,
+    flush_version_control_info=True,
 ) -> None:
     """Modifies the version state to reflect the checkout and also copies required data to the new branch directory if a new one is being created."""
     storage = dataset.storage
     version_state = dataset.version_state
     original_commit_id = version_state["commit_id"]
 
     if address in version_state["branch_commit_map"].keys():
@@ -198,31 +220,42 @@
             storage.flush()
         version_state["commit_id"] = address
         version_state["commit_node"] = version_state["commit_node_map"][address]
         version_state["branch"] = version_state["commit_node"].branch
     elif create:
         storage.check_readonly()
         # if the original commit is head of the branch, auto commit and checkout to original commit before creating new branch
-        auto_commit(dataset, f"auto commit before checkout to {address}")
+        auto_commit(
+            dataset,
+            f"auto commit before checkout to {address}",
+            flush_version_control_info=False,
+        )
         if hash:
             if hash in version_state["commit_node_map"]:
                 raise CommitError(f"Commit {hash} already exists")
             new_commit_id = hash
         else:
             new_commit_id = generate_hash()
         new_node = CommitNode(address, new_commit_id)
-        version_state["commit_node"].add_child(new_node)
+        stored_commit_node = version_state["commit_node"]
+        stored_commit_node.add_child(new_node)
         version_state["commit_id"] = new_commit_id
         version_state["commit_node"] = new_node
         version_state["branch"] = address
         version_state["commit_node_map"][new_commit_id] = new_node
         version_state["branch_commit_map"][address] = new_commit_id
-        save_version_info(version_state, storage)
-        copy_metas(original_commit_id, new_commit_id, storage, version_state)
-        create_commit_chunk_maps(new_commit_id, storage, version_state)
+        if flush_version_control_info:
+            save_version_info(version_state, storage)
+            save_commit_info(new_node, storage)
+            save_commit_info(stored_commit_node, storage)
+        else:
+            stored_commit_node._info_updated = True
+            new_node._info_updated = True
+        copy_metas(original_commit_id, new_commit_id, storage)
+        create_commit_chunk_maps(original_commit_id, new_commit_id, storage)
         dataset._send_branch_creation_event(address)
     else:
         raise CheckoutError(
             f"Address {address} not found. If you want to create a new branch, use checkout with create=True"
         )
 
     discard_old_metas(
@@ -240,37 +273,36 @@
         ) from e
 
 
 def copy_metas(
     src_commit_id: str,
     dest_commit_id: str,
     storage: LRUCache,
-    version_state: Dict[str, Any],
 ) -> None:
     """Copies meta data from one commit to another."""
     initial_autoflush = storage.autoflush
     storage.autoflush = False
 
-    tensors = version_state["full_tensors"]
-    src_dataset_meta_key = get_dataset_meta_key(src_commit_id)
+    src_dataset_meta = _get_dataset_meta_at_commit(storage, src_commit_id)
+
     dest_dataset_meta_key = get_dataset_meta_key(dest_commit_id)
-    src_dataset_meta = storage[src_dataset_meta_key]
     dest_dataset_meta = convert_to_bytes(src_dataset_meta)
+
     storage[dest_dataset_meta_key] = dest_dataset_meta
 
     try:
         src_dataset_info_key = get_dataset_info_key(src_commit_id)
         dest_dataset_info_key = get_dataset_info_key(dest_commit_id)
         src_dataset_info = storage[src_dataset_info_key]
         dest_dataset_info = convert_to_bytes(src_dataset_info)
         storage[dest_dataset_info_key] = dest_dataset_info
     except KeyError:
         pass
 
-    tensor_list = list(tensors.keys())
+    tensor_list = src_dataset_meta.tensors
 
     for tensor in tensor_list:
         src_tensor_meta_key = get_tensor_meta_key(tensor, src_commit_id)
         dest_tensor_meta_key = get_tensor_meta_key(tensor, dest_commit_id)
         src_tensor_meta = storage[src_tensor_meta_key]
         dest_tensor_meta = convert_to_bytes(src_tensor_meta)
         storage[dest_tensor_meta_key] = dest_tensor_meta
@@ -321,20 +353,20 @@
             pass
 
     storage.autoflush = initial_autoflush
     storage.flush()
 
 
 def create_commit_chunk_maps(
+    src_commit_id: str,
     dest_commit_id: str,
     storage: LRUCache,
-    version_state: Dict[str, Any],
 ) -> None:
     """Creates commit chunk sets for all tensors in new commit."""
-    tensor_list = version_state["full_tensors"].keys()
+    tensor_list = _get_dataset_meta_at_commit(storage, src_commit_id).tensors
     for tensor in tensor_list:
         key = get_tensor_commit_chunk_map_key(tensor, dest_commit_id)
         storage[key] = CommitChunkMap()
 
 
 def discard_old_metas(
     src_commit_id: str,
@@ -371,14 +403,41 @@
             storage.cache_used -= size
         try:
             del storage.cache_storage[key]
         except KeyError:
             pass
 
 
+def reset_and_checkout(ds, address, err, verbose=True):
+    storage = ds.storage
+    version_state = ds.version_state
+
+    parent_commit_id, reset_commit_id = get_parent_and_reset_commit_ids(
+        version_state, address
+    )
+    if parent_commit_id is False:
+        # non-head node corrupted
+        raise err
+    if parent_commit_id is None:
+        # no commits in the dataset
+        storage.clear()
+        ds._populate_meta()
+        load_meta(ds)
+        return
+
+    ds.checkout(parent_commit_id)
+    new_commit_id = replace_head(storage, version_state, reset_commit_id)
+    ds.checkout(new_commit_id)
+
+    current_node = version_state["commit_node_map"][ds.commit_id]
+    if verbose:
+        logger.info(f"HEAD reset. Current version:\n{current_node}")
+    return ds.commit_id
+
+
 def _merge_commit_node_maps(map1, map2):
     merged_map = {}
 
     def _merge_node(commit_id):
         if commit_id in map1 and commit_id in map2:
             node1 = map1[commit_id]
             node2 = map2[commit_id]
@@ -415,19 +474,35 @@
     branch_commit_map.update(info2["branch_commit_map"])
     return {
         "commit_node_map": commit_node_map,
         "branch_commit_map": branch_commit_map,
     }
 
 
+def save_commit_info(commit_node: CommitNode, storage: LRUCache) -> None:
+    """Saves the commit info to the storage."""
+    storage = get_base_storage(storage)
+    key = get_commit_info_key(commit_node.commit_id)
+    storage[key] = json.dumps(commit_node.to_json()).encode("utf-8")
+    commit_node._info_updated = False
+
+
+def load_commit_info(commit_id: str, storage: LRUCache) -> Dict:
+    """Loads the commit info from the storage."""
+    storage = get_base_storage(storage)
+    key = get_commit_info_key(commit_id)
+    commit_info = json.loads(storage[key].decode("utf-8"))
+    return commit_info
+
+
 def save_version_info(version_state: Dict[str, Any], storage: LRUCache) -> None:
     """Saves the current version info to the storage."""
     storage = get_base_storage(storage)
-    lock = Lock(storage, get_version_control_info_lock_key())
-    lock.acquire(timeout=10, force=True)
+    lock = Lock(storage, get_version_control_info_lock_key(), duration=10)
+    lock.acquire()  # Blocking
     key = get_version_control_info_key()
     new_version_info = {
         "commit_node_map": version_state["commit_node_map"],
         "branch_commit_map": version_state["branch_commit_map"],
     }
     try:
         old_version_info = _version_info_from_json(
@@ -453,29 +528,182 @@
         )
     except KeyError:
         return pickle.loads(
             storage[get_version_control_info_key_old()]
         )  # backward compatiblity
 
 
-def auto_checkout(dataset) -> bool:
+def get_parent_and_reset_commit_ids(version_info, address):
+    """Returns parent commit id and commit id which will be reset. Returns (False, False) if address is a non-HEAD commit id"""
+    if address in version_info["branch_commit_map"]:
+        commit_id = version_info["branch_commit_map"][address]
+    elif address in version_info["commit_node_map"]:
+        commit_id = address
+    commit_node = version_info["commit_node_map"][commit_id]
+    if not commit_node.is_head_node:
+        return False, False
+    parent_node = commit_node.parent
+    if parent_node is None:
+        previous_commit_id = None
+    else:
+        previous_commit_id = parent_node.commit_id
+    return previous_commit_id, commit_id
+
+
+def _create_new_head(storage, version_state, branch, parent_commit_id, new_commit_id):
+    # populate new commit folder
+    copy_metas(parent_commit_id, new_commit_id, storage)
+    create_commit_chunk_maps(parent_commit_id, new_commit_id, storage)
+
+    # create new node
+    parent_node: CommitNode = version_state["commit_node_map"][parent_commit_id]
+    new_node = CommitNode(branch, new_commit_id)
+    new_node.parent = parent_node
+    version_state["branch_commit_map"][branch] = new_commit_id
+    version_state["commit_node_map"][new_commit_id] = new_node
+
+    return new_node
+
+
+def _replace_head(storage, version_state, commit_id, new_head):
+    parent_node = new_head.parent
+    del version_state["commit_node_map"][commit_id]
+    for i, child in enumerate(parent_node.children):
+        if child.commit_id == commit_id:
+            parent_node.children[i] = new_head
+            break
+
+    save_version_info(version_state, storage)
+
+
+def delete_version_from_storage(storage, commit_id):
+    deletion_folder = "/".join(("versions", commit_id))
+    storage.clear(prefix=deletion_folder)
+    storage.flush()
+
+
+def replace_head(storage, version_state, reset_commit_id):
+    """Replace HEAD of current branch with new HEAD"""
+    branch = version_state["commit_node_map"][reset_commit_id].branch
+    parent_commit_id = version_state["commit_id"]
+    new_commit_id = generate_hash()
+
+    new_node = _create_new_head(
+        storage, version_state, branch, parent_commit_id, new_commit_id
+    )
+
+    _replace_head(storage, version_state, reset_commit_id, new_node)
+
+    delete_version_from_storage(storage, reset_commit_id)
+
+    return new_node.commit_id
+
+
+def _replace_missing_with_head(missing_id, commits, branch_commit_map):
+    new_commit_id = generate_hash()
+    branch = None
+    parent_commit_id = None
+    for commit_id, commit_info in commits.items():
+        if missing_id in commit_info["children"]:
+            commit_info["children"].remove(missing_id)
+            commit_info["children"].append(new_commit_id)
+            branch = commit_info["branch"]
+            parent_commit_id = commit_id
+            break
+
+    commit_info = {
+        "branch": branch,
+        "children": [],
+        "parent": parent_commit_id,
+        "commit_message": None,
+        "commit_time": None,
+        "commit_user_name": None,
+    }
+    commits[new_commit_id] = commit_info
+    branch_commit_map[branch] = new_commit_id
+
+    return branch, parent_commit_id, new_commit_id
+
+
+def rebuild_version_info(storage):
+    """Rebuilds version info from commit info."""
+    branch_commit_map = {}
+    commits = {}
+
+    # dont do anything if first commit info is missing
+    try:
+        commit_info = load_commit_info(FIRST_COMMIT_ID, storage)
+    except Exception:
+        return
+
+    stack = [FIRST_COMMIT_ID]
+
+    new_heads = []
+
+    while stack:
+        commit_id = stack.pop()
+
+        try:
+            commit_info = load_commit_info(commit_id, storage)
+        except KeyError:
+            if commit_id != FIRST_COMMIT_ID:
+                new_head = _replace_missing_with_head(
+                    commit_id, commits, branch_commit_map
+                )
+                new_heads.append(new_head)
+                continue
+            raise
+        commits[commit_id] = commit_info
+        if commit_info["commit_time"] is None:
+            branch_commit_map[commit_info["branch"]] = commit_id
+        stack += commit_info["children"]
+
+    if not commits:
+        return
+
+    base_storage = get_base_storage(storage)
+    lock = Lock(storage, get_version_control_info_lock_key(), duration=10)
+    lock.acquire()  # Blocking
+    try:
+        del storage[get_version_control_info_key()]
+    except KeyError:
+        pass
+    key = get_version_control_info_key()
+    version_info = {"commits": commits, "branches": branch_commit_map}
+    base_storage[key] = json.dumps(version_info).encode("utf-8")
+    lock.release()
+
+    version_info = _version_info_from_json(version_info)
+
+    for new_head in new_heads:
+        _create_new_head(storage, version_info, *new_head)
+
+    return version_info
+
+
+def auto_checkout(dataset, flush_version_control_info: bool = True) -> bool:
     """Automatically checks out if current node is not the head node of the branch. This may happen either during commit/setitem/append/extend/create_tensor/delete_tensor/info updates."""
     version_state = dataset.version_state
     if not version_state["commit_node"].is_head_node:
         current_branch = version_state["branch"]
         auto_branch = f"auto_{generate_hash()}"
         logger.info(
             f"Automatically checking out to branch '{auto_branch}' as not currently at the head node of branch '{current_branch}'."
         )
-        checkout(dataset, auto_branch, True)
+        checkout(
+            dataset,
+            auto_branch,
+            True,
+            flush_version_control_info=flush_version_control_info,
+        )
         return True
     return False
 
 
-def auto_commit(dataset, message: str) -> None:
+def auto_commit(dataset, message: str, flush_version_control_info: bool = True) -> None:
     """Automatically commits to the current branch before a checkout to a newly created branch if the current node is the head node and has changes."""
     version_state = dataset.version_state
     commit_node = version_state["commit_node"]
     head = commit_node.is_head_node
     if not head:
         return
 
@@ -485,23 +713,28 @@
         return
 
     original_commit_id = version_state["commit_id"]
     branch = version_state["branch"]
     logger.info(
         f"Auto commiting to branch '{branch}' before checkout as currently at head node."
     )
-    commit(dataset, message)
-    checkout(dataset, original_commit_id, False)
+    commit(
+        dataset,
+        message,
+        flush_version_control_info=flush_version_control_info,
+        reload_meta=False,
+    )
+    checkout(dataset, original_commit_id)
 
 
 def current_commit_has_change(version_state: Dict[str, Any], storage: LRUCache) -> bool:
     return (
-        current_commit_has_data(version_state, storage)
+        version_state["commit_id"] == FIRST_COMMIT_ID
+        or current_commit_has_data(version_state, storage)
         or current_commit_has_info_modified(version_state, storage)
-        or version_state["commit_id"] == FIRST_COMMIT_ID
     )
 
 
 def current_commit_has_data(version_state: Dict[str, Any], storage: LRUCache) -> bool:
     """Checks if the current commit has any data present in it or not."""
     commit_id = version_state["commit_id"]
     try:
@@ -555,32 +788,38 @@
         key = get_tensor_commit_diff_key(tensor, commit_id)
         storage[key]
         return True
     except KeyError:
         return False
 
 
+def _get_dataset_meta_at_commit(storage, commit_id):
+    """Get dataset meta at commit."""
+    meta_key = get_dataset_meta_key(commit_id)
+    meta = storage.get_deeplake_object(meta_key, DatasetMeta)
+    if not meta.tensor_names:  # backward compatibility
+        meta.tensor_names = {key: key for key in meta.tensors}
+    storage.register_deeplake_object(meta_key, meta)
+    return meta
+
+
 def load_meta(dataset):
     """Loads the meta info for the version state."""
     from deeplake.core.tensor import Tensor
 
     version_state = dataset.version_state
     storage: LRUCache = dataset.storage
     storage.clear_deeplake_objects()
     dataset._info = None
     dataset._ds_diff = None
-    meta_key = get_dataset_meta_key(version_state["commit_id"])
-    meta = storage.get_deeplake_object(meta_key, DatasetMeta)
-    if not meta.tensor_names:  # backward compatibility
-        meta.tensor_names = {key: key for key in meta.tensors}
+    meta = _get_dataset_meta_at_commit(storage, version_state["commit_id"])
 
     ffw_dataset_meta(meta)
     version_state["meta"] = meta
 
-    storage.register_deeplake_object(meta_key, meta)
     _tensors = version_state["full_tensors"]
     _tensors.clear()
     _tensor_names = version_state["tensor_names"]
     _tensor_names.clear()
     _tensor_names.update(meta.tensor_names)
 
     for tensor_key in _tensor_names.values():
```

### Comparing `deeplake-3.2.9/deeplake/util/video.py` & `deeplake-3.3.0/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/visualizer/video_streaming.py` & `deeplake-3.3.0/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.9/deeplake/visualizer/visualizer.py` & `deeplake-3.3.0/deeplake/visualizer/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from typing import Dict, Optional, Union
 import uuid
 from flask import Flask, request, Response
 from deeplake.core.link_creds import LinkCreds  # type: ignore
-from deeplake.core.storage.provider import StorageProvider
+from deeplake.core.storage import StorageProvider
 from deeplake.core.storage.s3 import S3Provider
 from deeplake.util.threading import terminate_thread
 from deeplake.client.config import (
     USE_DEV_ENVIRONMENT,
     USE_STAGING_ENVIRONMENT,
     USE_LOCAL_HOST,
 )
@@ -167,24 +167,25 @@
 
 
 @_APP.route("/creds/<path:path>")
 def access_creds(path: str):
     paths = path.split("/", 1)
     id = paths[0]
     creds_key = paths[1]
-    if len(creds_key) == 0:
-        p = S3Provider("")
-        return {
-            "aws_access_key_id": p.aws_access_key_id,
-            "aws_secret_access_key": p.aws_secret_access_key,
-            "aws_session_token": p.aws_session_token,
-            "aws_region": p.aws_region,
-        }
     if creds_key in visualizer.get_link_creds(id).creds_keys:
-        return visualizer.get_link_creds(id).get_creds(creds_key)
+        creds = visualizer.get_link_creds(id).get_creds(creds_key)
+        if len(creds) == 0:
+            p = S3Provider("")
+            creds = {
+                "aws_access_key_id": p.aws_access_key_id,
+                "aws_secret_access_key": p.aws_secret_access_key,
+                "aws_session_token": p.aws_session_token,
+                "aws_region": p.aws_region,
+            }
+        return creds
 
     return Response("", 404)
 
 
 @_APP.route("/<path:path>")
 def access_data(path):
     try:
```

### Comparing `deeplake-3.2.9/deeplake.egg-info/PKG-INFO` & `deeplake-3.3.0/deeplake.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,408 +1,413 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.2.9
+Version: 3.3.0
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
-Description: <img src="https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82" /><p align="center">
-             <img src="https://i.postimg.cc/rsjcWc3S/deeplake-logo.png" width="400"/>
-        </h1>
-            </br>
-            <h1 align="center">Deep Lake: Data Lake for Deep Learning
-         </h1>
-        <p align="center">
-            <a href="https://github.com/activeloopai/Hub/actions/workflows/test-pr-on-label.yml"><img src="https://github.com/activeloopai/Hub/actions/workflows/test-push.yml/badge.svg" alt="PyPI version" height="18"></a>
-            <a href="https://pypi.org/project/deeplake/"><img src="https://badge.fury.io/py/deeplake.svg" alt="PyPI version" height="18"></a>
-            <a href='https://docs.deeplake.ai/en/latest/?badge=latest'>
-             <img src='https://readthedocs.org/projects/deep-lake/badge/?version=latest' alt='Documentation Status' />
-             </a>
-            <a href="https://pepy.tech/project/deeplake"><img src="https://static.pepy.tech/personalized-badge/deeplake?period=month&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="PyPI version" height="18"></a>
-             <a href="https://github.com/activeloopai/deeplake/issues">
-            <img alt="GitHub issues" src="https://img.shields.io/github/issues/activeloopai/deeplake"> </a>
-            <a href="https://codecov.io/gh/activeloopai/deeplake/branch/main"><img src="https://codecov.io/gh/activeloopai/deeplake/branch/main/graph/badge.svg" alt="codecov" height="18"></a>
-          <h3 align="center">
-           <a href="https://docs.activeloop.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Documentation</b></a> &bull;
-           <a href="https://docs.activeloop.ai/getting-started/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Getting Started</b></a> &bull;
-           <a href="https://docs.deeplake.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>API Reference</b></a> &bull;  
-           <a href="https://github.com/activeloopai/examples/"><b>Examples</b></a> &bull; 
-           <a href="https://www.activeloop.ai/resources/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Blog</b></a> &bull; 
-           <a href="https://www.deeplake.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Whitepaper</b></a> &bull;  
-          <a href="http://slack.activeloop.ai"><b>Slack Community</b></a> &bull;
-          <a href="https://twitter.com/intent/tweet?text=The%20dataset%20format%20for%20AI.%20Stream%20data%20to%20PyTorch%20and%20Tensorflow%20datasets&url=https://activeloop.ai/&via=activeloopai&hashtags=opensource,pytorch,tensorflow,data,datascience,datapipelines,activeloop,databaseforAI"><b>Twitter</b></a>
-         </h3>
-         
-        
-        *Read this in other languages: [简体中文](README.zh-cn.md)*
-        
-        ## About Deep Lake
-        
-        Deep Lake (formerly known as Activeloop Hub) is a data lake for deep learning applications. Our open-source dataset format is optimized for rapid streaming and querying of data while training models at scale, and it includes a simple API for creating, storing, and collaborating on AI datasets of any size. It can be deployed locally or in the cloud, and it enables you to store all of your data in one place, ranging from simple annotations to large videos. Deep Lake is used by Google, Waymo, Red Cross, Omdena, Yale, & Oxford. Deep Lake includes the following features:
-        
-        <details>
-          <summary><b>Storage Agnostic API</b></summary>
-        Use one API to upload, download, and stream datasets to/from AWS S3/S3-compatible storage, GCP, Activeloop cloud, or local storage.
-        </details>
-        <details>
-          <summary><b>Native Compression</b></summary>
-        Store images, audios and videos in their native compression. Deeplake automatically decompresses them to raw data only when needed, e.g., when training a model.
-        </details>
-        <details>
-          <summary><b>Lazy NumPy-like Indexing</b></summary>
-        Treat your cloud datasets as if they are a collection of NumPy arrays in your system's memory. Slice them, index them, or iterate through them. Only the bytes you ask for will be downloaded!
-        </details>
-        <details>
-          <summary><b>Dataset Version Control</b></summary>
-        Commits, branches, checkout - Concepts you are already familiar with in your code repositories can now be applied to your datasets as well!
-        </details>
-        <details>
-          <summary><b>Dataloaders for Popular Deep Learning Frameworks</b></summary>
-        Deep Lake comes with built-in dataloaders for Pytorch and Tensorflow. Train your model with a few lines of code - we even take care of dataset shuffling. :)
-        </details>
-        <details>
-          <summary><b>Distributed Transformations</b></summary>
-        Rapidly apply transformations on your datasets using multi-threading, multi-processing, or our built-in <a href="https://www.ray.io/">Ray</a> integration.</details>
-        <details>
-          <summary><b>100+ most-popular image, video, and audio datasets available in seconds</b></summary>
-        Deep Lake community has uploaded <a href="https://docs.activeloop.ai/datasets/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">100+ image, video and audio datasets</a> like <a href="https://docs.activeloop.ai/datasets/mnist/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">MNIST</a>, <a href="https://docs.activeloop.ai/datasets/coco-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">COCO</a>,  <a href="https://docs.activeloop.ai/datasets/imagenet-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">ImageNet</a>,  <a href="https://docs.activeloop.ai/datasets/cifar-10-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">CIFAR</a>,  <a href="https://docs.activeloop.ai/datasets/gtzan-genre-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">GTZAN</a> and others.
-        </details>
-        </details>
-        <details>
-          <summary><b>Instant Visualization Support in <a href="https://app.activeloop.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">Activeloop Platform</a></b></summary>
-        Deep Lake datasets are instantly visualized with bounding boxes, masks, annotations, etc. in <a href="https://app.activeloop.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">Deep Lake Visualizer</a> (see below).
-        </details>
-        
-        <div align="center">
-        <a href="https://www.youtube.com/watch?v=SxsofpSIw3k"><img src="https://www.linkpicture.com/q/ReadMe.gif" type="image"></a>
-        </div>
-        
-            
-        ## 🚀 Performance
-        
-        Deep Lake's efficient enterprise dataloaders built in C++ speeds up data streaming by >2x compared to Hub 2.x (Ofeidis et al. 2022, Hambardzumyan et al. 2023) 
-        
-        <div align="center">
-        <a href="https://arxiv.org/pdf/2209.10785.pdf"><img src="docs/source/_static/img/benchmarks.png" type="image"></a>
-        </div>
-        
-        
-        ## Getting Started with Deep Lake
-        
-        
-        ### 🚀 How to install Deep Lake
-        Deep Lake's core is efficiently built in C++ and can be quickly installed using pip.
-        
-        ```sh
-        pip3 install deeplake
-        ```
-        
-        **By default, Deep Lake does not install dependencies for audio, video, google-cloud, and other features. Details on all installation options are [available here](https://docs.deeplake.ai/en/latest/Installation.html).**
-        
-        ### 🧠 How to Train a PyTorch model on a Deep Lake dataset
-        
-        #### Load CIFAR 10, one of the readily available datasets in Deep Lake:
-        
-        ```python
-        import deeplake
-        import torch
-        from torchvision import transforms, models
-        
-        ds = deeplake.load('hub://activeloop/cifar10-train')
-        ```
-        
-        #### Inspect tensors in the dataset:
-        
-        ```python
-        ds.tensors.keys()    # dict_keys(['images', 'labels'])
-        ds.labels[0].numpy() # array([6], dtype=uint32)
-        ```
-        
-        #### Train a PyTorch model on the CIFAR 10 dataset without the need to download it
-        
-        First, define a transform for the images and use Deep Lake's built-in PyTorch one-line dataloader to connect the data to the compute:
-        
-        ```python
-        tform = transforms.Compose([
-            transforms.ToTensor(),
-            transforms.Normalize([0.5, 0.5, 0.5], [0.5, 0.5, 0.5]),
-        ])
-        
-        deeplake_loader = ds.pytorch(num_workers=0, batch_size=4, transform={
-                                'images': tform, 'labels': None}, shuffle=True)
-        ```
-        
-        Next, define the model, loss and optimizer:
-        
-        ```python
-        net = models.resnet18(pretrained=False)
-        net.fc = torch.nn.Linear(net.fc.in_features, len(ds.labels.info.class_names))
-            
-        criterion = torch.nn.CrossEntropyLoss()
-        optimizer = torch.optim.SGD(net.parameters(), lr=0.001, momentum=0.9)
-        ```
-        
-        Finally, the training loop for 2 epochs:
-        
-        ```python
-        for epoch in range(2):
-            running_loss = 0.0
-            for i, data in enumerate(deeplake_loader):
-                images, labels = data['images'], data['labels']
-                
-                # zero the parameter gradients
-                optimizer.zero_grad()
-        
-                # forward + backward + optimize
-                outputs = net(images)
-                loss = criterion(outputs, labels.reshape(-1))
-                loss.backward()
-                optimizer.step()
-                
-                # print statistics
-                running_loss += loss.item()
-                if i % 100 == 99:    # print every 100 mini-batches
-                    print('[%d, %5d] loss: %.3f' %
-                        (epoch + 1, i + 1, running_loss / 100))
-                    running_loss = 0.0
-        ```
-        
-        
-        ### 🏗️ How to create a Deep Lake Dataset
-        
-        A Deep Lake dataset can be created in various locations (Storage providers). This is how the paths for each of them would look like:
-        
-        | Storage provider        | Example path                   |
-        | ----------------------- | ------------------------------ |
-        | Activeloop cloud        | hub://user_name/dataset_name   |
-        | AWS S3 / S3 compatible  | s3://bucket_name/dataset_name  |
-        | GCP                     | gcp://bucket_name/dataset_name |
-        | Google Drive            | gdrive://path_to_dataset
-        | Local storage           | path to local directory        |
-        | In-memory               | mem://dataset_name             |
-        
-        
-        
-        Let's create a dataset in the Activeloop cloud. Activeloop cloud provides free storage up to 300 GB per user (more info [here](#-for-students-and-educators)). Create a new account with Deep Lake from the terminal using `activeloop register` or in the [Deep Lake UI](https://app.activeloop.ai/register/). You will be asked for a user name, email ID, and password.
-        
-        ```sh
-        $ activeloop register
-        Enter your details. Your password must be at least 6 characters long.
-        Username:
-        Email:
-        Password:
-        ```
-        
-        After registration, an ORGANIZATION is automatically created that shares your username. You can use it for creating and managing your datasets, or you can create a new one for your company or team.
-        
-        Initialize an empty dataset in the Activeloop Cloud:
-        
-        ```python
-        import deeplake
-        
-        ds = deeplake.empty('hub://<ORGANIZATION_NAME>/test-dataset')
-        ```
-        
-        
-        Next, create a tensor to hold images in the dataset we just initialized:
-        
-        ```python
-        images = ds.create_tensor('images', htype='image', sample_compression='jpg')
-        ```
-        
-        Assuming you have a list of image file paths, let's upload them to the dataset:
-        
-        ```python
-        image_paths = ...
-        with ds:
-            for image_path in image_paths:
-                image = deeplake.read(image_path)
-                ds.images.append(image)
-        ```
-        
-        Alternatively, you can also upload numpy arrays. Since the `images` tensor was created with `sample_compression='jpg'`, the arrays will be compressed with jpeg compression.
-        
-        
-        ```python
-        import numpy as np
-        
-        with ds:
-            for _ in range(1000):  # 1000 random images
-                random_image = np.random.randint(0, 256, (100, 100, 3), dtype=np.uint8)  # 100x100 image with 3 channels
-                ds.images.append(random_image)
-        ```
-        
-        
-        
-        ### 🚀 How to load a Deep Lake Dataset
-        
-        
-        You can load the dataset you just created with a single line of code:
-        
-        ```python
-        import deeplake
-        
-        ds = deeplake.load('hub://<ORGANIZATION_NAME>/test-dataset')
-        ```
-        
-        You can also access one of the <a href="https://docs.activeloop.ai/datasets/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">100+ image, video and audio datasets in Deep Lake format</a>, not just the ones you created. Here is how you would load the [Objectron Bikes Dataset](https://github.com/google-research-datasets/Objectron):
-        
-        ```python
-        import deeplake
-        
-        ds = deeplake.load('hub://activeloop/objectron_bike_train')
-        ```
-        
-        To get the first image in the Objectron Bikes dataset in numpy format:
-        
-        
-        ```python
-        image_arr = ds.image[0].numpy()
-        ```
-        
-        ## ⚙️ Integrations
-        Deep Lake offers integrations with other tools in order to streamline your deep learning workflows. Current integrations include:
-        
-        * **Model Training**
-          * Stream data while training thousands of pre-built models using [MMDetection](https://github.com/open-mmlab/mmdetection), a popular open-source object detection toolbox based on PyTorch. Learn more in [this tutorial](https://docs.activeloop.ai/tutorials/training-models/training-models-using-mmdetection).
-          
-        * **Experiment Tracking**
-          * Track experiments and achieve full model reproducibility using Deep Lake and [Weights & Biases](https://wandb.ai/). Our integration automatically pushes dataset-related information (uri, commit hash, view id) to your W&B runs. Further details are available [in our model-reproducibility playbook](https://docs.activeloop.ai/playbooks/training-reproducibility-with-wandb).
-        
-        ## 📚 Documentation
-        Getting started guides, examples, tutorials, API reference, and other useful information can be found on our [documentation page](http://docs.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme). 
-        
-        ## 🎓 For Students and Educators
-        Deep Lake users can access and visualize a variety of popular datasets through a free integration with Activeloop's Platform. Users can also create and store their own datasets and make them available to the public. Free storage of up to 300 GB is available for students and educators:
-        
-        | <!-- -->    | <!-- -->    |
-        | ---------------------------------------------------- | ------------- |
-        | Storage for public datasets hosted by Activeloop     | 200GB Free    |
-        | Storage for private datasets hosted by Activeloop    | 100GB Free    |
-        
-        
-        
-        ## 👩‍💻 Comparisons to Familiar Tools
-        
-        
-        <details>
-          <summary><b>Deep Lake vs DVC</b></summary>
-          
-        Deep Lake and DVC offer dataset version control similar to git for data, but their methods for storing data differ significantly. Deep Lake converts and stores data as chunked compressed arrays, which enables rapid streaming to ML models, whereas DVC operates on top of data stored in less efficient traditional file structures. The Deep Lake format makes dataset versioning significantly easier compared to traditional file structures by DVC when datasets are composed of many files (i.e., many images). An additional distinction is that DVC primarily uses a command-line interface, whereas Deep Lake is a Python package. Lastly, Deep Lake offers an API to easily connect datasets to ML frameworks and other common ML tools and enables instant dataset visualization through [Activeloop's visualization tool](http://app.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme).
-        
-        </details>
-        
-        
-        <details>
-          <summary><b>Deep Lake vs TensorFlow Datasets (TFDS)</b></summary>
-          
-        Deep Lake and TFDS seamlessly connect popular datasets to ML frameworks. Deep Lake datasets are compatible with both PyTorch and TensorFlow, whereas TFDS are only compatible with TensorFlow. A key difference between Deep Lake and TFDS is that Deep Lake datasets are designed for streaming from the cloud, whereas TFDS must be downloaded locally prior to use. As a result, with Deep Lake, one can import datasets directly from TensorFlow Datasets and stream them either to PyTorch or TensorFlow. In addition to providing access to popular publicly available datasets, Deep Lake also offers powerful tools for creating custom datasets, storing them on a variety of cloud storage providers, and collaborating with others via simple API. TFDS is primarily focused on giving the public easy access to commonly available datasets, and management of custom datasets is not the primary focus. A full comparison article can be found [here](https://www.activeloop.ai/resources/tensor-flow-tf-data-activeloop-hub-how-to-implement-your-tensor-flow-data-pipelines-with-hub/).
-        
-        </details>
-        
-        
-        
-        <details>
-          <summary><b>Deep Lake vs HuggingFace</b></summary>
-        Deep Lake and HuggingFace offer access to popular datasets, but Deep Lake primarily focuses on computer vision, whereas HuggingFace focuses on natural language processing. HuggingFace Transforms and other computational tools for NLP are not analogous to features offered by Deep Lake.
-        
-        
-        </details>
-        
-        <details>
-          <summary><b>Deep Lake vs WebDatasets</b></summary>
-        Deep Lake and WebDatasets both offer rapid data streaming across networks. They have nearly identical steaming speeds because the underlying network requests and data structures are very similar. However, Deep Lake offers superior random access and shuffling, its simple API is in python instead of command-line, and Deep Lake enables simple indexing and modification of the dataset without having to recreate it.
-        
-        
-        </details>
-        
-        <details>
-          <summary><b>Deep Lake vs Zarr</b></summary>
-        Deep Lake and Zarr both offer storage of data as chunked arrays. However, Deep Lake is primarily designed for returning data as arrays using a simple API, rather than actually storing raw arrays (even though that's also possible). Deep Lake stores data in use-case-optimized formats, such as jpeg or png for images, or mp4 for video, and the user treats the data as if it's an array, because Deep Lake handles all the data processing in between. Deep Lake offers more flexibility for storing arrays with dynamic shape (ragged tensors), and it provides several features that are not naively available in Zarr such as version control, data streaming, and connecting data to ML Frameworks.
-        
-        
-        </details>
-        
-        ## Community
-        
-        Join our [**Slack community**](https://join.slack.com/t/hubdb/shared_invite/zt-ivhsj8sz-GWv9c5FLBDVw8vn~sxRKqQ) to learn more about unstructured dataset management using Deep Lake and to get help from the Activeloop team and other users.
-        
-        We'd love your feedback by completing our 3-minute [**survey**](https://forms.gle/rLi4w33dow6CSMcm9).
-        
-        As always, thanks to our amazing contributors!    
-        
-        <a href="https://github.com/activeloopai/deeplake/graphs/contributors">
-          <img src="https://contrib.rocks/image?repo=activeloopai/hub" />
-        </a>
-        
-        Made with [contributors-img](https://contrib.rocks).
-        
-        Please read [CONTRIBUTING.md](CONTRIBUTING.md) to get started with making contributions to Deep Lake.
-        
-        
-        ## README Badge
-        
-        Using Deep Lake? Add a README badge to let everyone know: 
-        
-        
-        [![deeplake](https://img.shields.io/badge/powered%20by-Deep%20Lake%20-ff5a1f.svg)](https://github.com/activeloopai/deeplake)
-        
-        ```
-        [![deeplake](https://img.shields.io/badge/powered%20by-Deep%20Lake%20-ff5a1f.svg)](https://github.com/activeloopai/deeplake)
-        ```
-        
-        
-        
-        ## Disclaimers
-        
-        <details>
-          <summary><b> Dataset Licenses</b></summary>
-          
-        Deep Lake users may have access to a variety of publicly available datasets. We do not host or distribute these datasets, vouch for their quality or fairness, or claim that you have a license to use the datasets. It is your responsibility to determine whether you have permission to use the datasets under their license.
-        
-        If you're a dataset owner and do not want your dataset to be included in this library, please get in touch through a [GitHub issue](https://github.com/activeloopai/deeplake/issues/new). Thank you for your contribution to the ML community!
-        
-        </details>
-        
-        <details>
-          <summary><b> Usage Tracking</b></summary>
-        
-        By default, we collect usage data using Bugout (here's the [code](https://github.com/activeloopai/deeplake/blob/853456a314b4fb5623c936c825601097b0685119/deeplake/__init__.py#L24) that does it). It does not collect user data other than anonymized IP address data, and it only logs the Deep Lake library's own actions. This helps our team understand how the tool is used and how to build features that matter to you! After you register with Activeloop, data is no longer anonymous. You can always opt-out of reporting using the CLI command below, or by setting an environmental variable ```BUGGER_OFF``` to ```True```:
-        
-        ```
-        activeloop reporting --off
-        ```
-        </details>
-        
-        ## Citation
-        If you use Deep Lake in your research, please cite Activeloop using:
-        
-        ```
-        @article{deeplake,
-          title = {Deep Lake: a Lakehouse for Deep Learning},
-          author = {Hambardzumyan, Sasun and Tuli, Abhinav and Ghukasyan, Levon and Rahman, Fariz and Topchyan, Hrant and Isayan, David and Harutyunyan, Mikayel and Hakobyan, Tatevik and Stranic, Ivo and Buniatyan, Davit},
-          url = {https://www.cidrdb.org/cidr2023/papers/p69-buniatyan.pdf},
-          booktitle={Proceedings of CIDR},
-          year = {2023},
-        }
-        ```
-        
-        ## Acknowledgment
-        This technology was inspired by our research work at Princeton University. We would like to thank William Silversmith @SeungLab for his awesome [cloud-volume](https://github.com/seung-lab/cloud-volume) tool.
-        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Description-Content-Type: text/markdown
+Provides-Extra: all
 Provides-Extra: audio
-Provides-Extra: video
 Provides-Extra: av
-Provides-Extra: gcp
 Provides-Extra: dicom
-Provides-Extra: medical
-Provides-Extra: visualizer
+Provides-Extra: gcp
 Provides-Extra: gdrive
+Provides-Extra: medical
 Provides-Extra: point_cloud
-Provides-Extra: all
-Provides-Extra: enterprise
+Provides-Extra: video
+Provides-Extra: visualizer
+License-File: LICENSE
+
+<img src="https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82" /><p align="center">
+     <img src="https://i.postimg.cc/rsjcWc3S/deeplake-logo.png" width="400"/>
+</h1>
+    </br>
+    <h1 align="center">Deep Lake: Data Lake for Deep Learning
+ </h1>
+<p align="center">
+    <a href="https://github.com/activeloopai/Hub/actions/workflows/test-pr-on-label.yml"><img src="https://github.com/activeloopai/Hub/actions/workflows/test-push.yml/badge.svg" alt="PyPI version" height="18"></a>
+    <a href="https://pypi.org/project/deeplake/"><img src="https://badge.fury.io/py/deeplake.svg" alt="PyPI version" height="18"></a>
+    <a href='https://docs.deeplake.ai/en/latest/?badge=latest'>
+     <img src='https://readthedocs.org/projects/deep-lake/badge/?version=latest' alt='Documentation Status' />
+     </a>
+    <a href="https://pepy.tech/project/deeplake"><img src="https://static.pepy.tech/badge/deeplake" alt="PyPI version" height="18"></a>
+     <a href="https://github.com/activeloopai/deeplake/issues">
+    <img alt="GitHub issues" src="https://img.shields.io/github/issues/activeloopai/deeplake"> </a>
+    <a href="https://codecov.io/gh/activeloopai/deeplake/branch/main"><img src="https://codecov.io/gh/activeloopai/deeplake/branch/main/graph/badge.svg" alt="codecov" height="18"></a>
+  <h3 align="center">
+   <a href="https://docs.activeloop.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Documentation</b></a> &bull;
+   <a href="https://docs.activeloop.ai/getting-started/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Getting Started</b></a> &bull;
+   <a href="https://docs.deeplake.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>API Reference</b></a> &bull;  
+   <a href="https://github.com/activeloopai/examples/"><b>Examples</b></a> &bull; 
+   <a href="https://www.activeloop.ai/resources/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Blog</b></a> &bull; 
+   <a href="https://www.deeplake.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme"><b>Whitepaper</b></a> &bull;  
+  <a href="http://slack.activeloop.ai"><b>Slack Community</b></a> &bull;
+  <a href="https://twitter.com/intent/tweet?text=The%20dataset%20format%20for%20AI.%20Stream%20data%20to%20PyTorch%20and%20Tensorflow%20datasets&url=https://activeloop.ai/&via=activeloopai&hashtags=opensource,pytorch,tensorflow,data,datascience,datapipelines,activeloop,databaseforAI"><b>Twitter</b></a>
+ </h3>
+ 
+
+*Read this in other languages: [简体中文](README.zh-cn.md)*
+
+## About Deep Lake
+
+Deep Lake (formerly known as Activeloop Hub) is a data lake for deep learning applications. Our open-source dataset format is optimized for rapid streaming and querying of data while training models at scale, and it includes a simple API for creating, storing, and collaborating on AI datasets of any size. It can be deployed locally or in the cloud, and it enables you to store all of your data in one place, ranging from simple annotations to large videos. Deep Lake is used by Google, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep Lake includes the following features:
+
+<details>
+  <summary><b>Storage Agnostic API</b></summary>
+Use one API to upload, download, and stream datasets to/from AWS S3/S3-compatible storage, GCP, Activeloop cloud, or local storage.
+</details>
+<details>
+  <summary><b>Native Compression with Lazy NumPy-like Indexing</b></summary>
+Store images, audios and videos in their native compression. Slide, index, iterate and interact with your data like a collection of NumPy arrays in your system's memory. Deep Lake lazily loads data only when needed, e.g., when training a model.
+</details>
+<details>
+  <summary><b>Dataset Version Control</b></summary>
+Commits, branches, checkout - Concepts you are already familiar with in your code repositories can now be applied to your datasets as well!
+</details>
+<details>
+  <summary><b>Dataloaders for Popular Deep Learning Frameworks</b></summary>
+Deep Lake comes with built-in dataloaders for Pytorch and Tensorflow. Train your model with a few lines of code - we even take care of dataset shuffling. :)
+</details>
+<details>
+  <summary><b>Integrations with Popular Tools</b></summary>
+Deep Lake has integrations with <a href="https://github.com/hwchase17/langchain">Langchain</a> as a vector store for LLM apps, <a href="https://wandb.ai/">Weights & Biases</a> for data lineage during model training, and <a href="https://github.com/open-mmlab/mmdetection">MMDetection</a> for training object detection models.
+</details>
+<details>
+  <summary><b>Distributed Transformations</b></summary>
+Rapidly apply transformations on your datasets using multi-threading, multi-processing, or our built-in <a href="https://www.ray.io/">Ray</a> integration.</details>
+<details>
+  <summary><b>100+ most-popular image, video, and audio datasets available in seconds</b></summary>
+Deep Lake community has uploaded <a href="https://docs.activeloop.ai/datasets/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">100+ image, video and audio datasets</a> like <a href="https://docs.activeloop.ai/datasets/mnist/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">MNIST</a>, <a href="https://docs.activeloop.ai/datasets/coco-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">COCO</a>,  <a href="https://docs.activeloop.ai/datasets/imagenet-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">ImageNet</a>,  <a href="https://docs.activeloop.ai/datasets/cifar-10-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">CIFAR</a>,  <a href="https://docs.activeloop.ai/datasets/gtzan-genre-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">GTZAN</a> and others.
+</details>
+</details>
+<details>
+  <summary><b>Instant Visualization Support in <a href="https://app.activeloop.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">Activeloop Platform</a></b></summary>
+Deep Lake datasets are instantly visualized with bounding boxes, masks, annotations, etc. in <a href="https://app.activeloop.ai/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">Deep Lake Visualizer</a> (see below).
+</details>
+
+<div align="center">
+<a href="https://www.youtube.com/watch?v=SxsofpSIw3k"><img src="https://www.linkpicture.com/q/ReadMe.gif" type="image"></a>
+</div>
+
+    
+## 🚀 Performance
+
+Deep Lake's efficient enterprise dataloaders built in C++ speeds up data streaming by >2x compared to Hub 2.x (Ofeidis et al. 2022, Hambardzumyan et al. 2023) 
+
+<div align="center">
+<a href="https://arxiv.org/pdf/2209.10785.pdf"><img src="docs/source/_static/img/benchmarks.png" type="image"></a>
+</div>
+
+
+## Getting Started with Deep Lake
+
+
+### 🚀 How to install Deep Lake
+Deep Lake's core is efficiently built in C++ and can be quickly installed using pip.
+
+```sh
+pip3 install deeplake
+```
+
+**By default, Deep Lake does not install dependencies for audio, video, google-cloud, and other features. Details on all installation options are [available here](https://docs.deeplake.ai/en/latest/Installation.html).**
+
+### 🧠 How to Train a PyTorch model on a Deep Lake dataset
+
+#### Load CIFAR 10, one of the readily available datasets in Deep Lake:
+
+```python
+import deeplake
+import torch
+from torchvision import transforms, models
+
+ds = deeplake.load('hub://activeloop/cifar10-train')
+```
+
+#### Inspect tensors in the dataset:
+
+```python
+ds.tensors.keys()    # dict_keys(['images', 'labels'])
+ds.labels[0].numpy() # array([6], dtype=uint32)
+```
+
+#### Train a PyTorch model on the CIFAR 10 dataset without the need to download it
+
+First, define a transform for the images and use Deep Lake's built-in PyTorch one-line dataloader to connect the data to the compute:
+
+```python
+tform = transforms.Compose([
+    transforms.ToTensor(),
+    transforms.Normalize([0.5, 0.5, 0.5], [0.5, 0.5, 0.5]),
+])
+
+deeplake_loader = ds.pytorch(num_workers=0, batch_size=4, transform={
+                        'images': tform, 'labels': None}, shuffle=True)
+```
+
+Next, define the model, loss and optimizer:
+
+```python
+net = models.resnet18(pretrained=False)
+net.fc = torch.nn.Linear(net.fc.in_features, len(ds.labels.info.class_names))
+    
+criterion = torch.nn.CrossEntropyLoss()
+optimizer = torch.optim.SGD(net.parameters(), lr=0.001, momentum=0.9)
+```
+
+Finally, the training loop for 2 epochs:
+
+```python
+for epoch in range(2):
+    running_loss = 0.0
+    for i, data in enumerate(deeplake_loader):
+        images, labels = data['images'], data['labels']
+        
+        # zero the parameter gradients
+        optimizer.zero_grad()
+
+        # forward + backward + optimize
+        outputs = net(images)
+        loss = criterion(outputs, labels.reshape(-1))
+        loss.backward()
+        optimizer.step()
+        
+        # print statistics
+        running_loss += loss.item()
+        if i % 100 == 99:    # print every 100 mini-batches
+            print('[%d, %5d] loss: %.3f' %
+                (epoch + 1, i + 1, running_loss / 100))
+            running_loss = 0.0
+```
+
+
+### 🏗️ How to create a Deep Lake Dataset
+
+A Deep Lake dataset can be created in various locations (Storage providers). This is how the paths for each of them would look like:
+
+| Storage provider        | Example path                   |
+| ----------------------- | ------------------------------ |
+| Activeloop cloud        | hub://user_name/dataset_name   |
+| AWS S3 / S3 compatible  | s3://bucket_name/dataset_name  |
+| GCP                     | gcp://bucket_name/dataset_name |
+| Google Drive            | gdrive://path_to_dataset
+| Local storage           | path to local directory        |
+| In-memory               | mem://dataset_name             |
+
+
+
+Let's create a dataset in the Activeloop cloud. Activeloop cloud provides free storage up to 300 GB per user (more info [here](#-for-students-and-educators)). Create a new account with Deep Lake from the terminal using `activeloop register` or in the [Deep Lake UI](https://app.activeloop.ai/register/). You will be asked for a user name, email ID, and password.
+
+```sh
+$ activeloop register
+Enter your details. Your password must be at least 6 characters long.
+Username:
+Email:
+Password:
+```
+
+After registration, an ORGANIZATION is automatically created that shares your username. You can use it for creating and managing your datasets, or you can create a new one for your company or team.
+
+Initialize an empty dataset in the Activeloop Cloud:
+
+```python
+import deeplake
+
+ds = deeplake.empty('hub://<ORGANIZATION_NAME>/test-dataset')
+```
+
+
+Next, create a tensor to hold images in the dataset we just initialized:
+
+```python
+images = ds.create_tensor('images', htype='image', sample_compression='jpg')
+```
+
+Assuming you have a list of image file paths, let's upload them to the dataset:
+
+```python
+image_paths = ...
+with ds:
+    for image_path in image_paths:
+        image = deeplake.read(image_path)
+        ds.images.append(image)
+```
+
+Alternatively, you can also upload numpy arrays. Since the `images` tensor was created with `sample_compression='jpg'`, the arrays will be compressed with jpeg compression.
+
+
+```python
+import numpy as np
+
+with ds:
+    for _ in range(1000):  # 1000 random images
+        random_image = np.random.randint(0, 256, (100, 100, 3), dtype=np.uint8)  # 100x100 image with 3 channels
+        ds.images.append(random_image)
+```
+
+
+
+### 🚀 How to load a Deep Lake Dataset
+
+
+You can load the dataset you just created with a single line of code:
+
+```python
+import deeplake
+
+ds = deeplake.load('hub://<ORGANIZATION_NAME>/test-dataset')
+```
+
+You can also access one of the <a href="https://docs.activeloop.ai/datasets/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">100+ image, video and audio datasets in Deep Lake format</a>, not just the ones you created. Here is how you would load the [Objectron Bikes Dataset](https://github.com/google-research-datasets/Objectron):
+
+```python
+import deeplake
+
+ds = deeplake.load('hub://activeloop/objectron_bike_train')
+```
+
+To get the first image in the Objectron Bikes dataset in numpy format:
+
+
+```python
+image_arr = ds.image[0].numpy()
+```
+
+## ⚙️ Integrations
+Deep Lake offers integrations with other tools in order to streamline your deep learning workflows. Current integrations include:
+
+* **Model Training**
+  * Stream data while training thousands of pre-built models using [MMDetection](https://github.com/open-mmlab/mmdetection), a popular open-source object detection toolbox based on PyTorch. Learn more in [this tutorial](https://docs.activeloop.ai/tutorials/training-models/training-models-using-mmdetection).
+  
+* **Experiment Tracking**
+  * Track experiments and achieve full model reproducibility using Deep Lake and [Weights & Biases](https://wandb.ai/). Our integration automatically pushes dataset-related information (uri, commit hash, view id) to your W&B runs. Further details are available [in our model-reproducibility playbook](https://docs.activeloop.ai/playbooks/training-reproducibility-with-wandb).
+  
+* **LLM Apps**
+  * Use [Deep Lake as a vector store for LLM apps](https://www.activeloop.ai/resources/ultimate-guide-to-lang-chain-deep-lake-build-chat-gpt-to-answer-questions-on-your-financial-data/). Our integration combines the [Langchain](https://github.com/hwchase17/langchain) [VectorStores API](https://python.langchain.com/en/latest/reference/modules/vectorstore.html?highlight=pinecone#langchain.vectorstores.DeepLake) with Deep Lake datasets as the underlying data storage. The integration is a serverless vector store that can be deployed locally or in a cloud of your choice. 
+
+## 📚 Documentation
+Getting started guides, examples, tutorials, API reference, and other useful information can be found on our [documentation page](http://docs.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme). 
+
+## 🎓 For Students and Educators
+Deep Lake users can access and visualize a variety of popular datasets through a free integration with Activeloop's Platform. Users can also create and store their own datasets and make them available to the public. Free storage of up to 300 GB is available for students and educators:
+
+| <!-- -->    | <!-- -->    |
+| ---------------------------------------------------- | ------------- |
+| Storage for public datasets hosted by Activeloop     | 200GB Free    |
+| Storage for private datasets hosted by Activeloop    | 100GB Free    |
+
+
+
+## 👩‍💻 Comparisons to Familiar Tools
+
+
+<details>
+  <summary><b>Deep Lake vs DVC</b></summary>
+  
+Deep Lake and DVC offer dataset version control similar to git for data, but their methods for storing data differ significantly. Deep Lake converts and stores data as chunked compressed arrays, which enables rapid streaming to ML models, whereas DVC operates on top of data stored in less efficient traditional file structures. The Deep Lake format makes dataset versioning significantly easier compared to traditional file structures by DVC when datasets are composed of many files (i.e., many images). An additional distinction is that DVC primarily uses a command-line interface, whereas Deep Lake is a Python package. Lastly, Deep Lake offers an API to easily connect datasets to ML frameworks and other common ML tools and enables instant dataset visualization through [Activeloop's visualization tool](http://app.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme).
+
+</details>
+
+
+<details>
+  <summary><b>Deep Lake vs TensorFlow Datasets (TFDS)</b></summary>
+  
+Deep Lake and TFDS seamlessly connect popular datasets to ML frameworks. Deep Lake datasets are compatible with both PyTorch and TensorFlow, whereas TFDS are only compatible with TensorFlow. A key difference between Deep Lake and TFDS is that Deep Lake datasets are designed for streaming from the cloud, whereas TFDS must be downloaded locally prior to use. As a result, with Deep Lake, one can import datasets directly from TensorFlow Datasets and stream them either to PyTorch or TensorFlow. In addition to providing access to popular publicly available datasets, Deep Lake also offers powerful tools for creating custom datasets, storing them on a variety of cloud storage providers, and collaborating with others via simple API. TFDS is primarily focused on giving the public easy access to commonly available datasets, and management of custom datasets is not the primary focus. A full comparison article can be found [here](https://www.activeloop.ai/resources/tensor-flow-tf-data-activeloop-hub-how-to-implement-your-tensor-flow-data-pipelines-with-hub/).
+
+</details>
+
+
+
+<details>
+  <summary><b>Deep Lake vs HuggingFace</b></summary>
+Deep Lake and HuggingFace offer access to popular datasets, but Deep Lake primarily focuses on computer vision, whereas HuggingFace focuses on natural language processing. HuggingFace Transforms and other computational tools for NLP are not analogous to features offered by Deep Lake.
+
+
+</details>
+
+<details>
+  <summary><b>Deep Lake vs WebDatasets</b></summary>
+Deep Lake and WebDatasets both offer rapid data streaming across networks. They have nearly identical steaming speeds because the underlying network requests and data structures are very similar. However, Deep Lake offers superior random access and shuffling, its simple API is in python instead of command-line, and Deep Lake enables simple indexing and modification of the dataset without having to recreate it.
+
+
+</details>
+
+<details>
+  <summary><b>Deep Lake vs Zarr</b></summary>
+Deep Lake and Zarr both offer storage of data as chunked arrays. However, Deep Lake is primarily designed for returning data as arrays using a simple API, rather than actually storing raw arrays (even though that's also possible). Deep Lake stores data in use-case-optimized formats, such as jpeg or png for images, or mp4 for video, and the user treats the data as if it's an array, because Deep Lake handles all the data processing in between. Deep Lake offers more flexibility for storing arrays with dynamic shape (ragged tensors), and it provides several features that are not naively available in Zarr such as version control, data streaming, and connecting data to ML Frameworks.
+
+
+</details>
+
+## Community
+
+Join our [**Slack community**](https://join.slack.com/t/hubdb/shared_invite/zt-ivhsj8sz-GWv9c5FLBDVw8vn~sxRKqQ) to learn more about unstructured dataset management using Deep Lake and to get help from the Activeloop team and other users.
+
+We'd love your feedback by completing our 3-minute [**survey**](https://forms.gle/rLi4w33dow6CSMcm9).
+
+As always, thanks to our amazing contributors!    
+
+<a href="https://github.com/activeloopai/deeplake/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=activeloopai/hub" />
+</a>
+
+Made with [contributors-img](https://contrib.rocks).
+
+Please read [CONTRIBUTING.md](CONTRIBUTING.md) to get started with making contributions to Deep Lake.
+
+
+## README Badge
+
+Using Deep Lake? Add a README badge to let everyone know: 
+
+
+[![deeplake](https://img.shields.io/badge/powered%20by-Deep%20Lake%20-ff5a1f.svg)](https://github.com/activeloopai/deeplake)
+
+```
+[![deeplake](https://img.shields.io/badge/powered%20by-Deep%20Lake%20-ff5a1f.svg)](https://github.com/activeloopai/deeplake)
+```
+
+
+
+## Disclaimers
+
+<details>
+  <summary><b> Dataset Licenses</b></summary>
+  
+Deep Lake users may have access to a variety of publicly available datasets. We do not host or distribute these datasets, vouch for their quality or fairness, or claim that you have a license to use the datasets. It is your responsibility to determine whether you have permission to use the datasets under their license.
+
+If you're a dataset owner and do not want your dataset to be included in this library, please get in touch through a [GitHub issue](https://github.com/activeloopai/deeplake/issues/new). Thank you for your contribution to the ML community!
+
+</details>
+
+<details>
+  <summary><b> Usage Tracking</b></summary>
+
+By default, we collect usage data using Bugout (here's the [code](https://github.com/activeloopai/deeplake/blob/853456a314b4fb5623c936c825601097b0685119/deeplake/__init__.py#L24) that does it). It does not collect user data other than anonymized IP address data, and it only logs the Deep Lake library's own actions. This helps our team understand how the tool is used and how to build features that matter to you! After you register with Activeloop, data is no longer anonymous. You can always opt-out of reporting using the CLI command below, or by setting an environmental variable ```BUGGER_OFF``` to ```True```:
+
+```
+activeloop reporting --off
+```
+</details>
+
+## Citation
+If you use Deep Lake in your research, please cite Activeloop using:
+
+```
+@article{deeplake,
+  title = {Deep Lake: a Lakehouse for Deep Learning},
+  author = {Hambardzumyan, Sasun and Tuli, Abhinav and Ghukasyan, Levon and Rahman, Fariz and Topchyan, Hrant and Isayan, David and Harutyunyan, Mikayel and Hakobyan, Tatevik and Stranic, Ivo and Buniatyan, Davit},
+  url = {https://www.cidrdb.org/cidr2023/papers/p69-buniatyan.pdf},
+  booktitle={Proceedings of CIDR},
+  year = {2023},
+}
+```
+
+## Acknowledgment
+This technology was inspired by our research work at Princeton University. We would like to thank William Silversmith @SeungLab for his awesome [cloud-volume](https://github.com/seung-lab/cloud-volume) tool.
+
+
```

#### html2text {}

```diff
@@ -1,47 +1,53 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.2.9 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.3.0 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
-deeplake Description: [https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-
-b8ea-f711c4d35b82]
+deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
+Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
+Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
+Provides-Extra: gcp Provides-Extra: gdrive Provides-Extra: medical Provides-
+Extra: point_cloud Provides-Extra: video Provides-Extra: visualizer License-
+File: LICENSE [https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-
+f711c4d35b82]
                [https://i.postimg.cc/rsjcWc3S/deeplake-logo.png]
              ****** Deep Lake: Data Lake for Deep Learning ******
   [PyPI_version] [PyPI_version] [Documentation_Status] [PyPI_version] [GitHub
                                issues] [codecov]
    **** Documentation • Getting_Started • API_Reference • Examples • Blog •
                   Whitepaper • Slack_Community • Twitter ****
 *Read this in other languages: [ç®ä½ä¸­æ](README.zh-cn.md)* ## About Deep
 Lake Deep Lake (formerly known as Activeloop Hub) is a data lake for deep
 learning applications. Our open-source dataset format is optimized for rapid
 streaming and querying of data while training models at scale, and it includes
 a simple API for creating, storing, and collaborating on AI datasets of any
 size. It can be deployed locally or in the cloud, and it enables you to store
 all of your data in one place, ranging from simple annotations to large videos.
-Deep Lake is used by Google, Waymo, Red Cross, Omdena, Yale, & Oxford. Deep
+Deep Lake is used by Google, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep
 Lake includes the following features:  Storage Agnostic API Use one API to
 upload, download, and stream datasets to/from AWS S3/S3-compatible storage,
-GCP, Activeloop cloud, or local storage.   Native Compression Store images,
-audios and videos in their native compression. Deeplake automatically
-decompresses them to raw data only when needed, e.g., when training a model.
-Lazy NumPy-like Indexing Treat your cloud datasets as if they are a collection
-of NumPy arrays in your system's memory. Slice them, index them, or iterate
-through them. Only the bytes you ask for will be downloaded!   Dataset Version
-Control Commits, branches, checkout - Concepts you are already familiar with in
-your code repositories can now be applied to your datasets as well!
-Dataloaders for Popular Deep Learning Frameworks Deep Lake comes with built-in
-dataloaders for Pytorch and Tensorflow. Train your model with a few lines of
-code - we even take care of dataset shuffling. :)   Distributed Transformations
-Rapidly apply transformations on your datasets using multi-threading, multi-
-processing, or our built-in Ray integration.  100+ most-popular image, video,
-and audio datasets available in seconds Deep Lake community has uploaded 100+
-image,_video_and_audio_datasets like MNIST, COCO, ImageNet, CIFAR, GTZAN and
-others.    Instant Visualization Support in Activeloop_Platform Deep Lake
-datasets are instantly visualized with bounding boxes, masks, annotations, etc.
-in Deep_Lake_Visualizer (see below).
+GCP, Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-
+like Indexing Store images, audios and videos in their native compression.
+Slide, index, iterate and interact with your data like a collection of NumPy
+arrays in your system's memory. Deep Lake lazily loads data only when needed,
+e.g., when training a model.   Dataset Version Control Commits, branches,
+checkout - Concepts you are already familiar with in your code repositories can
+now be applied to your datasets as well!   Dataloaders for Popular Deep
+Learning Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
+Tensorflow. Train your model with a few lines of code - we even take care of
+dataset shuffling. :)   Integrations with Popular Tools Deep Lake has
+integrations with Langchain as a vector store for LLM apps, Weights_&_Biases
+for data lineage during model training, and MMDetection for training object
+detection models.   Distributed Transformations Rapidly apply transformations
+on your datasets using multi-threading, multi-processing, or our built-in Ray
+integration.  100+ most-popular image, video, and audio datasets available in
+seconds Deep Lake community has uploaded 100+_image,_video_and_audio_datasets
+like MNIST, COCO, ImageNet, CIFAR, GTZAN and others.    Instant Visualization
+Support in Activeloop_Platform Deep Lake datasets are instantly visualized with
+bounding boxes, masks, annotations, etc. in Deep_Lake_Visualizer (see below).
                   [https://www.linkpicture.com/q/ReadMe.gif]
 ## ð Performance Deep Lake's efficient enterprise dataloaders built in C++
 speeds up data streaming by >2x compared to Hub 2.x (Ofeidis et al. 2022,
 Hambardzumyan et al. 2023)
                    [docs/source/_static/img/benchmarks.png]
 ## Getting Started with Deep Lake ### ð How to install Deep Lake Deep Lake's
 core is efficiently built in C++ and can be quickly installed using pip. ```sh
@@ -114,15 +120,23 @@
 mmlab/mmdetection), a popular open-source object detection toolbox based on
 PyTorch. Learn more in [this tutorial](https://docs.activeloop.ai/tutorials/
 training-models/training-models-using-mmdetection). * **Experiment Tracking** *
 Track experiments and achieve full model reproducibility using Deep Lake and
 [Weights & Biases](https://wandb.ai/). Our integration automatically pushes
 dataset-related information (uri, commit hash, view id) to your W&B runs.
 Further details are available [in our model-reproducibility playbook](https://
-docs.activeloop.ai/playbooks/training-reproducibility-with-wandb). ## ð
+docs.activeloop.ai/playbooks/training-reproducibility-with-wandb). * **LLM
+Apps** * Use [Deep Lake as a vector store for LLM apps](https://
+www.activeloop.ai/resources/ultimate-guide-to-lang-chain-deep-lake-build-chat-
+gpt-to-answer-questions-on-your-financial-data/). Our integration combines the
+[Langchain](https://github.com/hwchase17/langchain) [VectorStores API](https://
+python.langchain.com/en/latest/reference/modules/
+vectorstore.html?highlight=pinecone#langchain.vectorstores.DeepLake) with Deep
+Lake datasets as the underlying data storage. The integration is a serverless
+vector store that can be deployed locally or in a cloud of your choice. ## ð
 Documentation Getting started guides, examples, tutorials, API reference, and
 other useful information can be found on our [documentation page](http://
 docs.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme). ##
 ð For Students and Educators Deep Lake users can access and visualize a
 variety of popular datasets through a free integration with Activeloop's
 Platform. Users can also create and store their own datasets and make them
 available to the public. Free storage of up to 300 GB is available for students
@@ -209,13 +223,8 @@
 Deep Learning}, author = {Hambardzumyan, Sasun and Tuli, Abhinav and Ghukasyan,
 Levon and Rahman, Fariz and Topchyan, Hrant and Isayan, David and Harutyunyan,
 Mikayel and Hakobyan, Tatevik and Stranic, Ivo and Buniatyan, Davit}, url =
 {https://www.cidrdb.org/cidr2023/papers/p69-buniatyan.pdf}, booktitle=
 {Proceedings of CIDR}, year = {2023}, } ``` ## Acknowledgment This technology
 was inspired by our research work at Princeton University. We would like to
 thank William Silversmith @SeungLab for his awesome [cloud-volume](https://
-github.com/seung-lab/cloud-volume) tool. Platform: UNKNOWN Classifier: License
-:: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0) Description-Content-
-Type: text/markdown Provides-Extra: audio Provides-Extra: video Provides-Extra:
-av Provides-Extra: gcp Provides-Extra: dicom Provides-Extra: medical Provides-
-Extra: visualizer Provides-Extra: gdrive Provides-Extra: point_cloud Provides-
-Extra: all Provides-Extra: enterprise
+github.com/seung-lab/cloud-volume) tool.
```

### Comparing `deeplake-3.2.9/deeplake.egg-info/SOURCES.txt` & `deeplake-3.3.0/deeplake.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 deeplake/__init__.py
 deeplake/compression.py
 deeplake/constants.py
@@ -48,14 +49,15 @@
 deeplake/api/tests/test_partial_upload.py
 deeplake/api/tests/test_pickle.py
 deeplake/api/tests/test_point_cloud.py
 deeplake/api/tests/test_polygons.py
 deeplake/api/tests/test_pop.py
 deeplake/api/tests/test_readonly.py
 deeplake/api/tests/test_rechunk.py
+deeplake/api/tests/test_reset.py
 deeplake/api/tests/test_sample_info.py
 deeplake/api/tests/test_text.py
 deeplake/api/tests/test_update_samples.py
 deeplake/api/tests/test_video.py
 deeplake/api/tests/test_views.py
 deeplake/auto/__init__.py
 deeplake/auto/structured/__init__.py
@@ -122,27 +124,30 @@
 deeplake/core/compute/provider.py
 deeplake/core/compute/ray.py
 deeplake/core/compute/serial.py
 deeplake/core/compute/thread.py
 deeplake/core/dataset/__init__.py
 deeplake/core/dataset/dataset.py
 deeplake/core/dataset/deeplake_cloud_dataset.py
+deeplake/core/dataset/deeplake_query_dataset.py
+deeplake/core/dataset/deeplake_query_tensor.py
 deeplake/core/dataset/invalid_view.py
 deeplake/core/dataset/view_entry.py
 deeplake/core/index/__init__.py
 deeplake/core/index/index.py
 deeplake/core/meta/__init__.py
 deeplake/core/meta/dataset_meta.py
 deeplake/core/meta/meta.py
 deeplake/core/meta/tensor_meta.py
 deeplake/core/meta/encode/__init__.py
 deeplake/core/meta/encode/base_encoder.py
 deeplake/core/meta/encode/byte_positions.py
 deeplake/core/meta/encode/chunk_id.py
 deeplake/core/meta/encode/creds.py
+deeplake/core/meta/encode/pad.py
 deeplake/core/meta/encode/sequence.py
 deeplake/core/meta/encode/shape.py
 deeplake/core/meta/encode/tile.py
 deeplake/core/meta/encode/tests/__init__.py
 deeplake/core/meta/encode/tests/common.py
 deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
 deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
@@ -161,14 +166,15 @@
 deeplake/core/storage/lru_cache.py
 deeplake/core/storage/memory.py
 deeplake/core/storage/provider.py
 deeplake/core/storage/s3.py
 deeplake/core/tests/__init__.py
 deeplake/core/tests/test_compression.py
 deeplake/core/tests/test_compute.py
+deeplake/core/tests/test_deeplake_indra_dataset.py
 deeplake/core/tests/test_io.py
 deeplake/core/tests/test_locking.py
 deeplake/core/tests/test_readonly.py
 deeplake/core/tests/test_serialize.py
 deeplake/core/tiling/__init__.py
 deeplake/core/tiling/deserialize.py
 deeplake/core/tiling/optimizer.py
@@ -187,24 +193,26 @@
 deeplake/core/version_control/commit_node.py
 deeplake/core/version_control/dataset_diff.py
 deeplake/core/version_control/test_merge.py
 deeplake/core/version_control/test_version_control.py
 deeplake/enterprise/__init__.py
 deeplake/enterprise/convert_to_libdeeplake.py
 deeplake/enterprise/dataloader.py
+deeplake/enterprise/dummy_dataloader.py
 deeplake/enterprise/libdeeplake_query.py
 deeplake/enterprise/test_pytorch.py
 deeplake/enterprise/test_query.py
 deeplake/enterprise/test_tensorflow.py
 deeplake/enterprise/util.py
 deeplake/integrations/__init__.py
 deeplake/integrations/huggingface/__init__.py
 deeplake/integrations/huggingface/huggingface.py
 deeplake/integrations/mmdet/__init__.py
 deeplake/integrations/mmdet/mmdet_.py
+deeplake/integrations/mmdet/mmdet_runners.py
 deeplake/integrations/mmdet/mmdet_utils.py
 deeplake/integrations/pytorch/__init__.py
 deeplake/integrations/pytorch/common.py
 deeplake/integrations/pytorch/dataset.py
 deeplake/integrations/pytorch/pytorch.py
 deeplake/integrations/pytorch/shuffle_buffer.py
 deeplake/integrations/tf/__init__.py
@@ -237,15 +245,14 @@
 deeplake/util/check_installation.py
 deeplake/util/check_latest_version.py
 deeplake/util/chunk_engine.py
 deeplake/util/class_label.py
 deeplake/util/compression.py
 deeplake/util/compute.py
 deeplake/util/connect_dataset.py
-deeplake/util/creds.py
 deeplake/util/dataset.py
 deeplake/util/delete_entry.py
 deeplake/util/diff.py
 deeplake/util/downsample.py
 deeplake/util/empty_sample.py
 deeplake/util/encoder.py
 deeplake/util/exceptions.py
@@ -268,14 +275,15 @@
 deeplake/util/notebook.py
 deeplake/util/path.py
 deeplake/util/pretty_print.py
 deeplake/util/remove_cache.py
 deeplake/util/scheduling.py
 deeplake/util/shape_interval.py
 deeplake/util/shuffle.py
+deeplake/util/spinner.py
 deeplake/util/split.py
 deeplake/util/storage.py
 deeplake/util/tag.py
 deeplake/util/testing.py
 deeplake/util/threading.py
 deeplake/util/token.py
 deeplake/util/transform.py
```

### Comparing `deeplake-3.2.9/deeplake.egg-info/requires.txt` & `deeplake-3.3.0/deeplake.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-numpy
-pillow
 boto3
 click
-pathos
-humbug>=0.2.6
-tqdm
+humbug>=0.3.1
 numcodecs
+numpy
+pathos
+pillow
 pyjwt
-hub>=2.8.7
+tqdm
+
+[:python_version >= "3.7" and sys_platform != "win32"]
+aioboto3>=10.4.0
+nest_asyncio
 
 [all]
-nibabel
-google-auth-oauthlib~=0.4.5
+IPython
+flask
 google-api-python-client~=2.31.0
-laspy
-google-cloud-storage~=1.42.0
+google-auth-oauthlib~=0.4.5
 google-auth~=2.0.1
+google-cloud-storage~=1.42.0
+laspy
+nibabel
 oauth2client~=4.1.3
-flask
 pydicom
-IPython
-libdeeplake==0.0.37
 
 [all:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
 [audio]
 
 [audio:python_version >= "3.7" or sys_platform != "win32"]
@@ -32,35 +34,31 @@
 
 [av]
 
 [av:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
 [dicom]
-pydicom
 nibabel
-
-[enterprise]
-libdeeplake==0.0.37
-pyjwt
+pydicom
 
 [gcp]
-google-cloud-storage~=1.42.0
-google-auth~=2.0.1
 google-auth-oauthlib~=0.4.5
+google-auth~=2.0.1
+google-cloud-storage~=1.42.0
 
 [gdrive]
 google-api-python-client~=2.31.0
-oauth2client~=4.1.3
-google-auth~=2.0.1
 google-auth-oauthlib~=0.4.5
+google-auth~=2.0.1
+oauth2client~=4.1.3
 
 [medical]
-pydicom
 nibabel
+pydicom
 
 [point_cloud]
 laspy
 
 [video]
 
 [video:python_version >= "3.7" or sys_platform != "win32"]
```

### Comparing `deeplake-3.2.9/setup.py` & `deeplake-3.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 all_extras = {r for v in extras.values() for r in v}
 install_requires = [req_map[r] for r in req_map if r not in all_extras]
 extras_require = {k: [req_map[r] for r in v] for k, v in extras.items()}
 
 extras_require["all"] = [req_map[r] for r in all_extras]
 
 if libdeeplake_availabe():
-    libdeeplake = "libdeeplake==0.0.37"
+    libdeeplake = "libdeeplake==0.0.47"
     extras_require["enterprise"] = [libdeeplake, "pyjwt"]
     extras_require["all"].append(libdeeplake)
 
 init_file = os.path.join(project_name, "__init__.py")
 
 
 def get_property(prop):
@@ -81,17 +81,14 @@
         # find variable with name `prop` in the __init__.py file
         rf'{prop}\s*=\s*[\'"]([^\'"]*)[\'"]',
         open(init_file).read(),
     )
     return result.group(1)
 
 
-install_requires.append("hub>=2.8.7")
-
-
 config = {
     "name": project_name,
     "version": get_property("__version__"),
     "description": "Activeloop Deep Lake",
     "long_description": long_description,
     "long_description_content_type": "text/markdown",
     "author": "activeloop.ai",
```

