# Comparing `tmp/hepai-1.0.6.tar.gz` & `tmp/hepai-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hepai-1.0.6.tar", last modified: Wed Oct 19 20:49:15 2022, max compression
+gzip compressed data, was "dist/hepai-1.0.7.tar", last modified: Fri Apr 21 12:16:27 2023, max compression
```

## Comparing `hepai-1.0.6.tar` & `hepai-1.0.7.tar`

### file list

```diff
@@ -1,173 +1,179 @@
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      118 2022-10-19 07:27:29.000000 hepai-1.0.6/MANIFEST.in
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3289 2022-10-19 20:49:15.000000 hepai-1.0.6/PKG-INFO
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2636 2022-10-18 14:32:48.000000 hepai-1.0.6/README.md
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1256 2022-10-19 11:15:06.000000 hepai-1.0.6/hai/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/apis/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1891 2022-10-18 05:48:01.000000 hepai-1.0.6/hai/apis/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/apis/basic/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-30 09:36:57.000000 hepai-1.0.6/hai/apis/basic/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       55 2022-09-27 11:58:39.000000 hepai-1.0.6/hai/apis/basic/argparse.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      458 2022-08-24 16:43:32.000000 hepai-1.0.6/hai/apis/basic/base.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       54 2022-09-02 03:07:47.000000 hepai-1.0.6/hai/apis/basic/grpc.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      122 2022-09-22 05:50:52.000000 hepai-1.0.6/hai/apis/basic/registry.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      141 2022-09-27 11:58:39.000000 hepai-1.0.6/hai/apis/basic/utils.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/apis/hub/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-04 00:48:55.000000 hepai-1.0.6/hai/apis/hub/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      803 2022-10-08 09:52:47.000000 hepai-1.0.6/hai/apis/hub/hubs.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/apis/modules/
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/apis/modules/ResNet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1057 2022-08-23 09:57:15.000000 hepai-1.0.6/hai/apis/modules/ResNet/ResNet.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      415 2022-08-31 12:42:53.000000 hepai-1.0.6/hai/apis/modules/ResNet/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/apis/modules/UNet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      637 2022-09-02 00:38:16.000000 hepai-1.0.6/hai/apis/modules/UNet/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2478 2022-09-22 09:20:00.000000 hepai-1.0.6/hai/apis/modules/UNet/argparse_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-09-02 00:21:08.000000 hepai-1.0.6/hai/apis/modules/UNet/evaluate_api.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4730 2022-09-03 22:56:22.000000 hepai-1.0.6/hai/apis/modules/UNet/predict_api.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     9139 2022-09-22 08:22:39.000000 hepai-1.0.6/hai/apis/modules/UNet/train_api.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3099 2022-09-22 04:07:35.000000 hepai-1.0.6/hai/apis/modules/UNet/unet_api.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/apis/modules/YOLOv5/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      434 2022-10-18 11:12:44.000000 hepai-1.0.6/hai/apis/modules/YOLOv5/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:54:43.000000 hepai-1.0.6/hai/apis/modules/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/configs/
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/configs/Base/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:19:48.000000 hepai-1.0.6/hai/configs/Base/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      421 2022-10-19 18:47:53.000000 hepai-1.0.6/hai/configs/Base/hai_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/configs/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      285 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/configs/uaii_deepsort_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2706 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/configs/uaii_seyolov5_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1476 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/configs/uaii_stream_config.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/configs/urls/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1752 2022-10-19 18:44:14.000000 hepai-1.0.6/hai/configs/urls/datasets.json
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      960 2022-10-19 20:40:27.000000 hepai-1.0.6/hai/configs/urls/hub_models.json
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      534 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/configs/visible_loader_config.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/modules/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:42:32.000000 hepai-1.0.6/hai/modules/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/modules/detection/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:41:52.000000 hepai-1.0.6/hai/modules/detection/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/modules/exporter/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:29.000000 hepai-1.0.6/hai/modules/exporter/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/modules/exporter/images_exporter/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5282 2022-10-08 08:46:30.000000 hepai-1.0.6/hai/modules/exporter/images_exporter/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/modules/loader/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:28.000000 hepai-1.0.6/hai/modules/loader/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/modules/loader/images_loader/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1618 2022-10-08 08:46:26.000000 hepai-1.0.6/hai/modules/loader/images_loader/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3320 2022-10-18 10:46:42.000000 hepai-1.0.6/hai/modules/loader/images_loader/dataloader.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    14091 2022-10-18 10:33:57.000000 hepai-1.0.6/hai/modules/loader/images_loader/dataset_torch.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    26952 2022-10-18 11:10:17.000000 hepai-1.0.6/hai/modules/loader/images_loader/datasets.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1446 2022-10-18 17:35:03.000000 hepai-1.0.6/hai/modules/model_hub.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/modules/segmentation/
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:56:25.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1573 2022-08-31 21:12:48.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/evaluate.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      842 2022-08-30 18:18:45.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/hubconf.py
--rwxrwxr-x   0 zzd       (1000) zzd       (1000)     3997 2022-08-30 18:18:45.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/predict.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     8621 2022-08-31 21:12:32.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/train.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/unet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       29 2022-08-30 18:18:45.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/unet/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1130 2022-08-30 18:18:45.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2602 2022-08-30 18:18:45.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/utils/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-30 18:18:45.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/utils/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2991 2022-10-08 08:56:24.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-30 18:18:45.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      533 2022-09-30 09:30:48.000000 hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/utils/utils.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:55:50.000000 hepai-1.0.6/hai/modules/segmentation/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/testor/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      164 2022-09-27 09:48:37.000000 hepai-1.0.6/hai/testor/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      189 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/testor/test.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2685 2022-10-08 08:24:56.000000 hepai-1.0.6/hai/testor/test_module.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      404 2022-10-08 08:39:37.000000 hepai-1.0.6/hai/testor/testor.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       46 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/cli/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:00:08.000000 hepai-1.0.6/hai/uaii/cli/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1954 2022-10-19 18:57:10.000000 hepai-1.0.6/hai/uaii/cli/cli_functions.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     8911 2022-10-19 19:47:07.000000 hepai-1.0.6/hai/uaii/cli/cli_main.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/datasets/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       28 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/datasets/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3223 2022-10-18 16:32:02.000000 hepai-1.0.6/hai/uaii/datasets/dataloader.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     8485 2022-10-18 11:06:03.000000 hepai-1.0.6/hai/uaii/datasets/dataset_utils.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    40434 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/datasets/datasets.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4673 2022-10-19 18:52:31.000000 hepai-1.0.6/hai/uaii/datasets/datasets_hub.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4020 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/datasets/uaii_loaders.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/registry/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      374 2022-09-22 05:57:37.000000 hepai-1.0.6/hai/uaii/registry/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5671 2022-10-08 08:57:37.000000 hepai-1.0.6/hai/uaii/registry/init_register.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    11103 2022-09-22 03:26:47.000000 hepai-1.0.6/hai/uaii/registry/registy.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       81 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/registry/testor.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/registry/utils/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/registry/utils/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/registry/utils/general.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/server/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/server/grpc/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/grpc/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/server/grpc/example/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/grpc/example/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      517 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/grpc/example/grpc-client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1353 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/grpc/example/grpc-test.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3163 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/grpc/example/hello_pb2.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2242 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/grpc/example/hello_pb2_grpc.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     6022 2022-09-02 03:06:02.000000 hepai-1.0.6/hai/uaii/server/grpc/grpc_pb2.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3707 2022-10-18 10:41:24.000000 hepai-1.0.6/hai/uaii/server/grpc/grpc_pb2_grpc.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5517 2022-09-02 04:56:59.000000 hepai-1.0.6/hai/uaii/server/grpc/grpc_secure_client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    10437 2022-10-18 10:42:22.000000 hepai-1.0.6/hai/uaii/server/grpc/grpc_secure_server.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     6172 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/grpc/grpc_xai_client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5648 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/grpc/grpc_xai_server.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/server/nacos/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/nacos/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/server/nacos/nacos/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      184 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/nacos/nacos/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    47889 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/nacos/nacos/client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      752 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/nacos/nacos/commons.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/nacos/nacos/exception.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1645 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/nacos/nacos/files.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2403 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/nacos/nacos/listener.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      624 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/nacos/nacos/params.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4363 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/nacos/nacos/timer.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1555 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/nacos/nacos-test.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2388 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/nacos/request_test.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/server/socket/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/socket/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/server/socket/example/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/socket/example/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/socket/example/client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      674 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/socket/example/server.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2131 2022-09-02 03:01:13.000000 hepai-1.0.6/hai/uaii/server/socket/server.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/socket/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/socket/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/socket/example/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/socket/example/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/socket/example/client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      672 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/socket/example/server.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2153 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/socket/server.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/stream/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/stream/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1411 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/stream/base_input.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     7745 2022-10-18 09:58:17.000000 hepai-1.0.6/hai/uaii/stream/base_module.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2575 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/stream/base_output.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      354 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/stream/base_queue.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        4 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/stream/rabbit_qm.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    15802 2022-09-27 10:17:02.000000 hepai-1.0.6/hai/uaii/stream/stream.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4094 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/stream/streams.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    12294 2022-08-24 17:25:48.000000 hepai-1.0.6/hai/uaii/uaii_main.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hai/uaii/utils/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.6/hai/uaii/utils/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      921 2022-09-22 07:46:07.000000 hepai-1.0.6/hai/uaii/utils/arbitrary_import.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    17029 2022-10-19 18:44:45.000000 hepai-1.0.6/hai/uaii/utils/base_uaii.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    15333 2022-10-18 05:49:47.000000 hepai-1.0.6/hai/uaii/utils/config_loader.py
--rw-r--r--   0 zzd       (1000) zzd       (1000)     4472 2022-09-30 05:15:38.000000 hepai-1.0.6/hai/uaii/utils/fake_argparse.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3729 2022-09-29 09:48:36.000000 hepai-1.0.6/hai/uaii/utils/general.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      339 2022-10-19 20:48:54.000000 hepai-1.0.6/hai/version.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2022-10-19 20:49:15.000000 hepai-1.0.6/hepai.egg-info/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3289 2022-10-19 20:49:15.000000 hepai-1.0.6/hepai.egg-info/PKG-INFO
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4456 2022-10-19 20:49:15.000000 hepai-1.0.6/hepai.egg-info/SOURCES.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2022-10-19 20:49:15.000000 hepai-1.0.6/hepai.egg-info/dependency_links.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       50 2022-10-19 20:49:15.000000 hepai-1.0.6/hepai.egg-info/entry_points.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       15 2022-10-19 20:49:15.000000 hepai-1.0.6/hepai.egg-info/requires.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        4 2022-10-19 20:49:15.000000 hepai-1.0.6/hepai.egg-info/top_level.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       38 2022-10-19 20:49:15.000000 hepai-1.0.6/setup.cfg
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4651 2022-10-19 14:41:29.000000 hepai-1.0.6/setup.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      118 2022-10-28 08:51:38.000000 hepai-1.0.7/MANIFEST.in
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4030 2023-04-21 12:16:27.000000 hepai-1.0.7/PKG-INFO
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3247 2023-04-21 12:15:37.000000 hepai-1.0.7/README.md
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1293 2023-04-21 07:42:34.000000 hepai-1.0.7/hai/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/apis/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1938 2023-04-21 07:42:31.000000 hepai-1.0.7/hai/apis/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/apis/basic/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-30 09:36:57.000000 hepai-1.0.7/hai/apis/basic/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       55 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/apis/basic/argparse.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      458 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/apis/basic/base.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       54 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/apis/basic/grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      122 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/apis/basic/registry.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      141 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/apis/basic/utils.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/apis/hub/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-04 00:48:55.000000 hepai-1.0.7/hai/apis/hub/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      803 2022-10-08 09:52:47.000000 hepai-1.0.7/hai/apis/hub/hubs.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/apis/modules/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/apis/modules/ResNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1057 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/apis/modules/ResNet/ResNet.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      415 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/apis/modules/ResNet/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/apis/modules/UNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      637 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/apis/modules/UNet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2478 2022-09-22 09:20:00.000000 hepai-1.0.7/hai/apis/modules/UNet/argparse_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-09-02 00:21:08.000000 hepai-1.0.7/hai/apis/modules/UNet/evaluate_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4730 2022-09-03 22:56:22.000000 hepai-1.0.7/hai/apis/modules/UNet/predict_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     9139 2022-09-22 08:22:39.000000 hepai-1.0.7/hai/apis/modules/UNet/train_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3099 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/apis/modules/UNet/unet_api.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/apis/modules/YOLOv5/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      434 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/apis/modules/YOLOv5/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:54:43.000000 hepai-1.0.7/hai/apis/modules/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/apis/workers_api/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:36:18.000000 hepai-1.0.7/hai/apis/workers_api/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      403 2023-04-21 07:47:44.000000 hepai-1.0.7/hai/apis/workers_api/model.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/configs/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/configs/Base/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:19:48.000000 hepai-1.0.7/hai/configs/Base/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      407 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/configs/Base/hai_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/configs/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      285 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/configs/uaii_deepsort_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2706 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/configs/uaii_seyolov5_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1476 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/configs/uaii_stream_config.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/configs/urls/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1752 2022-10-19 18:44:14.000000 hepai-1.0.7/hai/configs/urls/datasets.json
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      960 2022-10-19 20:40:27.000000 hepai-1.0.7/hai/configs/urls/hub_models.json
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      534 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/configs/visible_loader_config.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/modules/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:42:32.000000 hepai-1.0.7/hai/modules/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/modules/detection/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:41:52.000000 hepai-1.0.7/hai/modules/detection/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/modules/exporter/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:29.000000 hepai-1.0.7/hai/modules/exporter/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/modules/exporter/images_exporter/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5282 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/modules/exporter/images_exporter/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/modules/loader/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:28.000000 hepai-1.0.7/hai/modules/loader/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/modules/loader/images_loader/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1618 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/modules/loader/images_loader/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3346 2023-04-21 12:08:18.000000 hepai-1.0.7/hai/modules/loader/images_loader/dataloader.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    14091 2022-10-18 10:33:57.000000 hepai-1.0.7/hai/modules/loader/images_loader/dataset_torch.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    26952 2022-10-18 11:10:17.000000 hepai-1.0.7/hai/modules/loader/images_loader/datasets.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1446 2022-10-18 17:35:03.000000 hepai-1.0.7/hai/modules/model_hub.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/modules/segmentation/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:56:25.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1573 2022-08-31 21:12:48.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/evaluate.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      842 2022-08-30 18:18:45.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/hubconf.py
+-rwxrwxr-x   0 zzd       (1000) zzd       (1000)     3997 2022-08-30 18:18:45.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/predict.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     8621 2022-08-31 21:12:32.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/train.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/unet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       29 2022-08-30 18:18:45.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/unet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1130 2022-08-30 18:18:45.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2602 2022-08-30 18:18:45.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-30 18:18:45.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2991 2022-10-08 08:56:24.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-30 18:18:45.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      533 2022-09-30 09:30:48.000000 hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/utils/utils.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:55:50.000000 hepai-1.0.7/hai/modules/segmentation/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/testor/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      166 2023-04-21 07:26:13.000000 hepai-1.0.7/hai/testor/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      189 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/testor/test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      281 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/testor/test_module.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      406 2023-04-21 07:26:41.000000 hepai-1.0.7/hai/testor/testor.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       46 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/actuator/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       71 2022-12-07 09:16:51.000000 hepai-1.0.7/hai/uaii/actuator/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      430 2022-12-07 09:20:22.000000 hepai-1.0.7/hai/uaii/actuator/trainer.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/cli/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:00:08.000000 hepai-1.0.7/hai/uaii/cli/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3692 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/uaii/cli/cli_functions.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     9276 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/uaii/cli/cli_main.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/datasets/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       28 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/datasets/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3240 2023-04-21 12:05:26.000000 hepai-1.0.7/hai/uaii/datasets/dataloader.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     8489 2023-04-21 12:07:18.000000 hepai-1.0.7/hai/uaii/datasets/dataset_utils.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    40434 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/datasets/datasets.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4673 2022-10-19 18:52:31.000000 hepai-1.0.7/hai/uaii/datasets/datasets_hub.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4046 2023-04-21 12:05:05.000000 hepai-1.0.7/hai/uaii/datasets/uaii_loaders.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/registry/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      374 2022-09-22 05:57:37.000000 hepai-1.0.7/hai/uaii/registry/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5669 2023-04-04 04:04:35.000000 hepai-1.0.7/hai/uaii/registry/init_register.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    11103 2022-09-22 03:26:47.000000 hepai-1.0.7/hai/uaii/registry/registy.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       81 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/registry/testor.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/registry/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/registry/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/registry/utils/general.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/server/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1893 2022-12-02 17:03:40.000000 hepai-1.0.7/hai/uaii/server/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/server/grpc/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/grpc/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/server/grpc/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/grpc/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      517 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/grpc/example/grpc-client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1353 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/grpc/example/grpc-test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3163 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/grpc/example/hello_pb2.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2242 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/grpc/example/hello_pb2_grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     6022 2022-09-02 03:06:02.000000 hepai-1.0.7/hai/uaii/server/grpc/grpc_pb2.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3707 2022-10-18 10:41:24.000000 hepai-1.0.7/hai/uaii/server/grpc/grpc_pb2_grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5517 2022-09-02 04:56:59.000000 hepai-1.0.7/hai/uaii/server/grpc/grpc_secure_client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    10437 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/uaii/server/grpc/grpc_secure_server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     6172 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/grpc/grpc_xai_client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5648 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/grpc/grpc_xai_server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/server/nacos/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/nacos/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/server/nacos/nacos/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      184 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/nacos/nacos/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    47889 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/nacos/nacos/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      752 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/nacos/nacos/commons.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/nacos/nacos/exception.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1645 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/nacos/nacos/files.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2403 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/nacos/nacos/listener.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      624 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/nacos/nacos/params.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4363 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/nacos/nacos/timer.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1555 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/nacos/nacos-test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2388 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/nacos/request_test.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/server/socket/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/socket/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/server/socket/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/socket/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/socket/example/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      674 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/socket/example/server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2131 2022-09-02 03:01:13.000000 hepai-1.0.7/hai/uaii/server/socket/server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/socket/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/socket/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/socket/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/socket/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/socket/example/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      672 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/socket/example/server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2153 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/socket/server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/stream/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/stream/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1411 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/stream/base_input.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     7745 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/uaii/stream/base_module.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2575 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/stream/base_output.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      354 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/stream/base_queue.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        4 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/stream/rabbit_qm.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    15802 2022-09-27 10:17:02.000000 hepai-1.0.7/hai/uaii/stream/stream.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4094 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/stream/streams.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    12294 2022-08-24 17:25:48.000000 hepai-1.0.7/hai/uaii/uaii_main.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hai/uaii/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.7/hai/uaii/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      921 2022-09-22 07:46:07.000000 hepai-1.0.7/hai/uaii/utils/arbitrary_import.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    17055 2023-04-21 12:06:51.000000 hepai-1.0.7/hai/uaii/utils/base_uaii.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    15272 2023-04-21 07:34:39.000000 hepai-1.0.7/hai/uaii/utils/config_loader.py
+-rw-r--r--   0 zzd       (1000) zzd       (1000)     4472 2022-09-30 05:15:38.000000 hepai-1.0.7/hai/uaii/utils/fake_argparse.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3729 2022-09-29 09:48:36.000000 hepai-1.0.7/hai/uaii/utils/general.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      339 2023-04-21 12:02:49.000000 hepai-1.0.7/hai/version.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 12:16:27.000000 hepai-1.0.7/hepai.egg-info/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4030 2023-04-21 12:16:27.000000 hepai-1.0.7/hepai.egg-info/PKG-INFO
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4578 2023-04-21 12:16:27.000000 hepai-1.0.7/hepai.egg-info/SOURCES.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2023-04-21 12:16:27.000000 hepai-1.0.7/hepai.egg-info/dependency_links.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       50 2023-04-21 12:16:27.000000 hepai-1.0.7/hepai.egg-info/entry_points.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       43 2023-04-21 12:16:27.000000 hepai-1.0.7/hepai.egg-info/requires.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        4 2023-04-21 12:16:27.000000 hepai-1.0.7/hepai.egg-info/top_level.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       38 2023-04-21 12:16:27.000000 hepai-1.0.7/setup.cfg
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4815 2023-04-21 12:07:47.000000 hepai-1.0.7/setup.py
```

### Comparing `hepai-1.0.6/PKG-INFO` & `hepai-1.0.7/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,58 @@
-Metadata-Version: 2.1
-Name: hepai
-Version: 1.0.6
-Summary: High energy phscis Artificial Intelligence plateform, HAI.
-Home-page: https://github.com/zhangzhengde0225/hai
-Author: Zhengde Zhang
-Author-email: zdzhang@163.com
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
+# [HAI](https://code.ihep.ac.cn/zdzhang/hai)
+白泽AI平台(Hakutaku AI)分为算法框架、模型库、数据集、算力资源四个部分。其中，HAI算法框架集成高能物理领域经典和SOTA的人工智能算法，提供统一、简单、易用的复现和应用接口。
 
+<details open>
+<summary><b>News</b></summary>
 
-# HAI
-高能物理AI平台(HAI)分为算法框架、模型库、数据集、算力资源四个部分。其中，HAI算法框架集成高能物理领域经典和SOTA的人工智能算法，提供统一、简单、易用的复现和应用接口。
++ [2023.04.21] 通过hepai使用GPT-3.5，[hepai_api.md](docs/hepai_api.md).
++ [2023.02.09] 基于ChatGPT的**HaiChatGPT**已上线，使用简单，无需梯子！详情查看：[HaiChatGPT](https://code.ihep.ac.cn/zdzhang/haichatgpt).
++ [2023.01.16] 华为NPU服务器上架，如有算法国产化需求，请查阅[NPU文档](docs/computing_power/npu_power_doc.md)。
++ [2022.10.20] HAI v1.0.6-Beta 第一个测试版本发布，4个算法和3个数据集
 
++ [2022.08.23] HAI v1.0.0
+</details>
 
 <details open>
 <summary><b>Tutorials</b></summary>
 
 [在计算集群上使用HAI的快速入门](docs/quickstart_hpc.md)
 
-更多教程[TODO]
+[使用PointNet对JUNO实验的大气中微子进行重建和鉴别](https://code.ihep.ac.cn/zhangyiyu/pointnet)
 
 </details>
 
 <details open>
-<summary><b>Model Zoo</b></summary>
-    <a href="https://code.ihep.ac.cn/zdzhang/hai/-/blob/main/docs/model_zoo.md">
-    <img src="https://img.shields.io/static/v1?style=social&label=图像相关&message=2 online, 5 TODO">
-    <br>
-    <img src="https://img.shields.io/static/v1?style=social&label=分类算法&message=3 TODO">
-    <br>
+<summary><b>Algorithm Zoo</b></summary>
+<a href="https://code.ihep.ac.cn/zdzhang/hai/-/blob/main/docs/model_zoo.md">
+    <ul>
+    <li>
     <img src="https://img.shields.io/static/v1?style=social&label=粒子物理&message=4 online, 3 TODO">
-    <br>
+    <li>
     <img src="https://img.shields.io/static/v1?style=social&label=天体物理&message=1 TODO">
-    <br>
-    <img src="https://img.shields.io/static/v1?style=social&label=射线科学&message=3 TODO">
-    <br>
-    <img src="https://img.shields.io/static/v1?style=social&label=机器学习&message=TODO">
+    <li>
+    <img src="https://img.shields.io/static/v1?style=social&label=同步辐射&message=2 TODO">
+    <li>
+    <img src="https://img.shields.io/static/v1?style=social&label=中子物理&message=0">
+    <li>
+    <img src="https://img.shields.io/static/v1?style=social&label=通用神经网络&message=2 online, 5 TODO">
+    <li>
+    <img src="https://img.shields.io/static/v1?style=social&label=经典机器学习&message=TODO">
+    </ul>
     </a>
     
 </details>
 
 <details open>
-<summary><b>Datasets</b></summary>
-    <a href="https://code.ihep.ac.cn/zdzhang/hai/-/blob/main/docs/datasets.md">
+<summary><b>Dataset Zoo</b></summary>
+<a href="https://code.ihep.ac.cn/zdzhang/hai/-/blob/main/docs/datasets.md">
+<ul>
+<li>
     <img src="https://img.shields.io/static/v1?style=social&label=粒子物理&message=3 available, 10+ TODO">
-    <br>
+    <li>
     <img src="https://img.shields.io/static/v1?style=social&label=CV&message=1 available">
     </a>
 </details>
 
 
 ### Quick start
 ```
@@ -98,22 +94,11 @@
     ```bash
     pip install hai-client
     ```
     ```python
     import hai_client
     hai = hai_client.HAI()
     ```
-    或其他支持gRPC的语言，详见[deploy](docs/deploy.md)（TODO）
-
-
-### TODO
-+ Visualize the dataset
-  +  .parquet file
-    + images
-
-+ Display in the docker container
-
-
-
+    或其他支持gRPC的语言，详见[deploy](docs/deploy.md)
```

#### html2text {}

```diff
@@ -1,39 +1,41 @@
-Metadata-Version: 2.1 Name: hepai Version: 1.0.6 Summary: High energy phscis
-Artificial Intelligence plateform, HAI. Home-page: https://github.com/
-zhangzhengde0225/hai Author: Zhengde Zhang Author-email: zdzhang@163.com
-License: MIT Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
-Python: >=3.6.0 Description-Content-Type: text/markdown # HAI
-é«è½ç©çAIå¹³å°
-(HAI)åä¸ºç®æ³æ¡æ¶ãæ¨¡ååºãæ°æ®éãç®åèµæºåä¸ªé¨åãå¶ä¸­ï¼HAIç®æ³æ¡æ¶éæé«è½ç©çé¢åç»å¸åSOTAçäººå·¥æºè½ç®æ³ï¼æä¾ç»ä¸ãç®åãæç¨çå¤ç°ååºç¨æ¥å£ã
-Tutorials [å¨è®¡ç®éç¾¤ä¸ä½¿ç¨HAIçå¿«éå¥é¨](docs/quickstart_hpc.md)
-æ´å¤æç¨[TODO]   Model Zoo [https://img.shields.io/static/
-v1?style=social&label=å¾åç¸å³&message=2_online,_5_TODO]_
-[https://img.shields.io/static/v1?style=social&label=åç±»ç®æ³&message=3
-TODO]_
-[https://img.shields.io/static/v1?style=social&label=ç²å­ç©ç&message=4
-online,_3_TODO]_
-[https://img.shields.io/static/v1?style=social&label=å¤©ä½ç©ç&message=1
-TODO]_
-[https://img.shields.io/static/v1?style=social&label=å°çº¿ç§å­¦&message=3
-TODO]_
-[https://img.shields.io/static/v1?style=social&label=æºå¨å­¦ä¹ &message=TODO]
-Datasets [https://img.shields.io/static/
-v1?style=social&label=ç²å­ç©ç&message=3_available,_10+_TODO]_
-[https://img.shields.io/static/v1?style=social&label=CV&message=1_available]
-### Quick start ``` pip install hepai hai -V # æ¥ççæ¬ ``` 1.
+# [HAI](https://code.ihep.ac.cn/zdzhang/hai) ç½æ³½AIå¹³å°(Hakutaku
+AI)åä¸ºç®æ³æ¡æ¶ãæ¨¡ååºãæ°æ®éãç®åèµæºåä¸ªé¨åãå¶ä¸­ï¼HAIç®æ³æ¡æ¶éæé«è½ç©çé¢åç»å¸åSOTAçäººå·¥æºè½ç®æ³ï¼æä¾ç»ä¸ãç®åãæç¨çå¤ç°ååºç¨æ¥å£ã
+News + [2023.04.21] éè¿hepaiä½¿ç¨GPT-3.5ï¼[hepai_api.md](docs/
+hepai_api.md). + [2023.02.09]
+åºäºChatGPTç**HaiChatGPT**å·²ä¸çº¿ï¼ä½¿ç¨ç®åï¼æ éæ¢¯å­ï¼è¯¦ææ¥çï¼
+[HaiChatGPT](https://code.ihep.ac.cn/zdzhang/haichatgpt). + [2023.01.16]
+åä¸ºNPUæå¡å¨ä¸æ¶ï¼å¦æç®æ³å½äº§åéæ±ï¼è¯·æ¥é[NPUææ¡£]
+(docs/computing_power/npu_power_doc.md)ã + [2022.10.20] HAI v1.0.6-Beta
+ç¬¬ä¸ä¸ªæµè¯çæ¬åå¸ï¼4ä¸ªç®æ³å3ä¸ªæ°æ®é + [2022.08.23] HAI
+v1.0.0   Tutorials [å¨è®¡ç®éç¾¤ä¸ä½¿ç¨HAIçå¿«éå¥é¨](docs/
+quickstart_hpc.md)
+[ä½¿ç¨PointNetå¯¹JUNOå®éªçå¤§æ°ä¸­å¾®å­è¿è¡éå»ºåé´å«](https://
+code.ihep.ac.cn/zhangyiyu/pointnet)   Algorithm Zoo
+    *_[https://img.shields.io/static/
+      v1?style=social&label=ç²å­ç©ç&message=4_online,_3_TODO]
+    *_[https://img.shields.io/static/
+      v1?style=social&label=å¤©ä½ç©ç&message=1_TODO]
+    *_[https://img.shields.io/static/
+      v1?style=social&label=åæ­¥è¾å°&message=2_TODO]
+    *_[https://img.shields.io/static/
+      v1?style=social&label=ä¸­å­ç©ç&message=0]
+    *_[https://img.shields.io/static/
+      v1?style=social&label=éç¨ç¥ç»ç½ç»&message=2_online,_5_TODO]
+    *_[https://img.shields.io/static/
+      v1?style=social&label=ç»å¸æºå¨å­¦ä¹ &message=TODO]
+   Dataset Zoo
+    *_[https://img.shields.io/static/
+      v1?style=social&label=ç²å­ç©ç&message=3_available,_10+_TODO]
+    *_[https://img.shields.io/static/v1?style=social&label=CV&message=1
+      available]
+  ### Quick start ``` pip install hepai hai -V # æ¥ççæ¬ ``` 1.
 å½ä»¤è¡ä½¿ç¨ ```bash hai train  # è®­ç»æ¨¡å, ä¾å¦: hai train
 particle_transformer hai eval  ``` 2. pythonåºä½¿ç¨ pythonåºç»ä¸æ¥å£ï¼
 ```python import hai model = hai.hub.load('') # å è½½æ¨¡å config =
 model.config # è·åæ¨¡åéç½® config.batch_size = 32 # ä¿®æ¹éç½®
 model.trian() # è®­ç»æ¨¡å model.eval() # è¯ä¼°æ¨¡å model.infer('') #
 æ¨¡åæ¨ç hai.train('particle_transformer') ``` 3. é¨ç½²åè¿ç¨è°ç¨
 è·¨è¯­è¨ãè·¨å¹³å°çæ¨¡åé¨ç½²åè¿ç¨è°ç¨ æå¡ç«¯ï¼ ```bash hai
 start server # å¯å¨æå¡ ``` å®¢æ·ç«¯ ```bash pip install hai-client ```
 ```python import hai_client hai = hai_client.HAI() ```
-æå¶ä»æ¯ægRPCçè¯­è¨ï¼è¯¦è§[deploy](docs/deploy.md)ï¼TODOï¼ ###
-TODO + Visualize the dataset + .parquet file + images + Display in the docker
-container
+æå¶ä»æ¯ægRPCçè¯­è¨ï¼è¯¦è§[deploy](docs/deploy.md)
```

### Comparing `hepai-1.0.6/hai/__init__.py` & `hepai-1.0.7/hai/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import os
 
+from .apis import __version__, __author__, __appname__, __email__, __affiliation__, __version_suffix__
+from .version import __url__
 from .apis import AbstractInput, AbstractModule, AbstractOutput, AbstractQue
 from .apis import MODULES, SCRIPTS, IOS, init_register
 from .apis import Config
 from .apis import UAII, uaii, cli
 from .apis import hub
 from .apis import hai_config as config  # inclue hai root_path, weights_root and other configs
 from .apis import grpc_secure_server
 from .apis import Testor
 from .apis import argparse
 from .apis import general
-from .apis import __version__, __author__, __appname__, __email__, __affiliation__, __version_suffix__
-from .version import __url__
+
+# LLM
+from .apis import LLM, Model
+
 # from xsensing_ai.modules import *  # 加载项目的模块
 # from xsensing_ai.uaii.server.grpc.grpc_xai_client import XAIGrpcClient
 
 # from . import nn
 
 # """
 # 导入内部模块和外部模块
```

### Comparing `hepai-1.0.6/hai/apis/__init__.py` & `hepai-1.0.7/hai/apis/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 try:
     import damei
 except:
     sys.path.append(f'{__pydir__.parent.parent.parent}/damei')
     import damei
 
 logger = damei.getLogger('hai')
-logger.info(f'HAI version: {__version__}')
+# logger.info(f'HAI version: {__version__}')
 
 
 if __backend__ == 'local':
     from .basic.base import AbstractModule, AbstractInput, AbstractOutput, AbstractQue
     from .basic.registry import MODULES, SCRIPTS, IOS, InitRegister
     from .basic.utils import Config
     from .basic.grpc import grpc_secure_server
@@ -39,14 +39,18 @@
     from damei.nn.api.registry import MODULES, SCRIPTS, IOS
     from damei.nn.api.utils import Config
     from damei.nn.api.utils import Config as PyConfigLoader
     from damei.nn.api import UAII as UAII
 else:
     raise NotImplementedError(f'{__backend__} backend is not supported, only local and damei, please check')
 
+from .workers_api.llm.llm import HaiLLM as LLM
+from .workers_api.model import HaiModel as Model
+
+
 hai_config = Config(f'{__pydir__.parent}/configs/Base/hai_config.py')
 # from ..configs.Base.hai_config import root_path, weights_root
 # root_path = f'{Path(__pydir__).parent.parent}'
-# weights_root = f'{os.environ["HOME"]}/.hai/weights'
+
 init_register = InitRegister(internal_dir=hai_config.root_path)
 uaii = UAII()
 cli = CommandLineInterface(uaii=uaii, config=hai_config)
```

### Comparing `hepai-1.0.6/hai/apis/hub/hubs.py` & `hepai-1.0.7/hai/apis/hub/hubs.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/apis/modules/ResNet/ResNet.py` & `hepai-1.0.7/hai/apis/modules/ResNet/ResNet.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/apis/modules/UNet/__init__.py` & `hepai-1.0.7/hai/apis/modules/UNet/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/apis/modules/UNet/argparse_config.py` & `hepai-1.0.7/hai/apis/modules/UNet/argparse_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/apis/modules/UNet/evaluate_api.py` & `hepai-1.0.7/hai/apis/modules/UNet/evaluate_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/apis/modules/UNet/predict_api.py` & `hepai-1.0.7/hai/apis/modules/UNet/predict_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/apis/modules/UNet/train_api.py` & `hepai-1.0.7/hai/apis/modules/UNet/train_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/apis/modules/UNet/unet_api.py` & `hepai-1.0.7/hai/apis/modules/UNet/unet_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/configs/uaii_seyolov5_config.py` & `hepai-1.0.7/hai/configs/uaii_seyolov5_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/configs/uaii_stream_config.py` & `hepai-1.0.7/hai/configs/uaii_stream_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/configs/urls/datasets.json` & `hepai-1.0.7/hai/configs/urls/datasets.json`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/configs/urls/hub_models.json` & `hepai-1.0.7/hai/configs/urls/hub_models.json`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/configs/visible_loader_config.py` & `hepai-1.0.7/hai/configs/visible_loader_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/modules/exporter/images_exporter/__init__.py` & `hepai-1.0.7/hai/modules/exporter/images_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/modules/loader/images_loader/__init__.py` & `hepai-1.0.7/hai/modules/loader/images_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/modules/loader/images_loader/dataloader.py` & `hepai-1.0.7/hai/modules/loader/images_loader/dataloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import os
-import cv2
+try:
+    import cv2
+except:
+    pass
 from pathlib import Path
 import numpy as np
 import damei as dm
 from copy import deepcopy
 
 from .datasets import LoadStreams, LoadImages
```

### Comparing `hepai-1.0.6/hai/modules/loader/images_loader/dataset_torch.py` & `hepai-1.0.7/hai/modules/loader/images_loader/dataset_torch.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/modules/loader/images_loader/datasets.py` & `hepai-1.0.7/hai/modules/loader/images_loader/datasets.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/modules/model_hub.py` & `hepai-1.0.7/hai/modules/model_hub.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/evaluate.py` & `hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/evaluate.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/hubconf.py` & `hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/hubconf.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/predict.py` & `hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/predict.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/train.py` & `hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/train.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py` & `hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py` & `hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py` & `hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py` & `hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/modules/segmentation/Pytorch_UNet/utils/utils.py` & `hepai-1.0.7/hai/modules/segmentation/Pytorch_UNet/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/cli/cli_main.py` & `hepai-1.0.7/hai/uaii/cli/cli_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     cli = CommandLineInterface()
     cli(opt) 
 
 
 class CommandLineInterface(CLIFunctions):
     def __init__(self, uaii=None, config=None):
         self.uaii = uaii if uaii is not None else hai.UAII()
-        self.config = config  # this is the hai config
+        self.config = config if config else hai.config # this is the hai config
         self.default_model = None  # if run hai command in a folder containing a model, then set the model as default model
         self.opt = None
         self.testor = Testor()
     
     def _init_opt(self, opt):
         # is cwd not in sys.path, then add it
         cwd = os.getcwd()
@@ -67,14 +67,16 @@
             self._deal_datasets_mode(opt)
         elif mode == 'test':
             self._deal_test_mode(opt)
         elif mode == 'train':
             self._deal_train_mode(opt)
         elif mode == 'version' or opt.version:
             self._show_version()
+        elif mode == 'start':
+            self._deal_with_start(**kwargs)
         elif mode is None:
             self._show_version()
             print(f'Please use "{hai.__appname__} -h" to see help.')
         else:
             exists_model_names = self.uaii.module_names
             if mode in exists_model_names:
                 self._deal_exists_model(opt)
@@ -180,18 +182,23 @@
         else:                                                                                                                                                                                                                                                                                                                                                                                           
             os.mkdir(api_fold_name)
 
         cwd = os.getcwd()
         project_name = os.path.basename(cwd).lower()
 
         # Copy template files to api_fold
-        shutil.copy(f'{root_path}/hai/apis/templates/README_template.md', f'{api_fold_name}/README.md')
-        os.system(f'echo "\nfrom .{project_name}_api import *" > {api_fold_name}/__init__.py')
+        shutil.copy(f'{root_path}/hai/apis/templates/README_template.md', 
+                    f'{api_fold_name}/README.md')
+        shutil.copy(f'{root_path}/hai/apis/templates/register_module_template.py', 
+                    f'{api_fold_name}/{project_name}_api.py')
+        shutil.copy(f'{root_path}/hai/apis/templates/init_template.py', 
+                    f'{api_fold_name}/__init__.py')
+        os.system(f'echo "\nfrom .{project_name}_api import *" >> {api_fold_name}/__init__.py')
+        logger.info(f'Create API folder and files successfully: "{os.getcwd()}/{api_fold_name}"')
 
-        shutil.copy(f'{root_path}/hai/apis/templates/register_module_template.py', f'{api_fold_name}/{project_name}_api.py')
 
     def _show_version(self):
         data = dict()
         ver = hai.__version__ + '-' + hai.__version_suffix__
         data[f'{hai.__appname__.upper()} Version'] = ver
         # data['Author'] = hai.__author__
         data['URL'] = hai.__url__
```

### Comparing `hepai-1.0.6/hai/uaii/datasets/dataloader.py` & `hepai-1.0.7/hai/uaii/datasets/dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
-import cv2
+# import cv2
 from pathlib import Path
 import numpy as np
 import damei as dm
 from copy import deepcopy
 
 try:
     import torch.backends.cudnn as cudnn
     from .datasets import LoadStreams, LoadImages
+    import cv2
 except ImportError as e:
     pass
     # dm.EXCEPTION(ImportError, e, info='You may need to install "torch" for full functionality', mute=True)
 
 
 class Dataloader(object):
     def __init__(self, source=None, imgsz=None):
```

### Comparing `hepai-1.0.6/hai/uaii/datasets/dataset_utils.py` & `hepai-1.0.7/hai/uaii/datasets/dataset_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import imp
 import os
 import shutil
 import zipfile
 import tarfile
 import urllib
 # import requests
-from tqdm import tqdm
 
 
 def _download(url, fname, chunk_size=1024):
+    from tqdm import tqdm
     import requests
     '''https://gist.github.com/yanqd0/c13ed29e29432e3cf3e7c38467f42f51'''
     resp = requests.get(url, stream=True)
     total = int(resp.headers.get('content-length', 0))
     with open(fname, 'wb') as file, tqdm(
         desc=fname,
         total=total,
```

### Comparing `hepai-1.0.6/hai/uaii/datasets/datasets.py` & `hepai-1.0.7/hai/uaii/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/datasets/datasets_hub.py` & `hepai-1.0.7/hai/uaii/datasets/datasets_hub.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/datasets/uaii_loaders.py` & `hepai-1.0.7/hai/uaii/datasets/uaii_loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import os, sys
 import time
 import damei as dm
-import cv2
+try:
+    import cv2
+except:
+    pass
 import shutil
 
 from ..utils.config_loader import PyConfigLoader
 from ..registry import MODULES, SCRIPTS, IOS
 from .dataloader import Dataloader
 
 logger = dm.getLogger('uaii loaders')
```

### Comparing `hepai-1.0.6/hai/uaii/registry/init_register.py` & `hepai-1.0.7/hai/uaii/registry/init_register.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     def import_external_module(self, external_module_path):
         """
         导入外部模块
         :param external_module_path: external module path, e.g.: repos/xxx/hai_api
         """
         emp = external_module_path
         if emp.startswith('~'):
-            emp = emp.replace('~', os.environ['HOME'])
+            emp = emp.replace('~', str(Path.home()))
         emp = os.path.abspath(emp) 
         if not os.path.exists(os.path.join(emp, self.api_fold_name)):
             if self.show_logger:
                 logger.warn(f'External module path "{emp}" not exists, and will be ignored.')
             return
 
         emp = os.path.join(emp, self.api_fold_name)
```

### Comparing `hepai-1.0.6/hai/uaii/registry/registy.py` & `hepai-1.0.7/hai/uaii/registry/registy.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/registry/utils/general.py` & `hepai-1.0.7/hai/uaii/registry/utils/general.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/grpc/example/grpc-client.py` & `hepai-1.0.7/hai/uaii/server/grpc/example/grpc-client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/grpc/example/grpc-test.py` & `hepai-1.0.7/hai/uaii/server/grpc/example/grpc-test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/grpc/example/hello_pb2.py` & `hepai-1.0.7/hai/uaii/server/grpc/example/hello_pb2.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/grpc/example/hello_pb2_grpc.py` & `hepai-1.0.7/hai/uaii/server/grpc/example/hello_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/grpc/grpc_pb2.py` & `hepai-1.0.7/hai/uaii/server/grpc/grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/grpc/grpc_pb2_grpc.py` & `hepai-1.0.7/hai/uaii/server/grpc/grpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/grpc/grpc_secure_client.py` & `hepai-1.0.7/hai/uaii/server/grpc/grpc_secure_client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/grpc/grpc_secure_server.py` & `hepai-1.0.7/hai/uaii/server/grpc/grpc_secure_server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/grpc/grpc_xai_client.py` & `hepai-1.0.7/hai/uaii/server/grpc/grpc_xai_client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/grpc/grpc_xai_server.py` & `hepai-1.0.7/hai/uaii/server/grpc/grpc_xai_server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/nacos/nacos/client.py` & `hepai-1.0.7/hai/uaii/server/nacos/nacos/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/nacos/nacos/commons.py` & `hepai-1.0.7/hai/uaii/server/nacos/nacos/commons.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/nacos/nacos/files.py` & `hepai-1.0.7/hai/uaii/server/nacos/nacos/files.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/nacos/nacos/listener.py` & `hepai-1.0.7/hai/uaii/server/nacos/nacos/listener.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/nacos/nacos/params.py` & `hepai-1.0.7/hai/uaii/server/nacos/nacos/params.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/nacos/nacos/timer.py` & `hepai-1.0.7/hai/uaii/server/nacos/nacos/timer.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/nacos/nacos-test.py` & `hepai-1.0.7/hai/uaii/server/nacos/nacos-test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/nacos/request_test.py` & `hepai-1.0.7/hai/uaii/server/nacos/request_test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/socket/example/client.py` & `hepai-1.0.7/hai/uaii/server/socket/example/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/socket/example/server.py` & `hepai-1.0.7/hai/uaii/server/socket/example/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/server/socket/server.py` & `hepai-1.0.7/hai/uaii/server/socket/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/socket/example/client.py` & `hepai-1.0.7/hai/uaii/socket/example/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/socket/example/server.py` & `hepai-1.0.7/hai/uaii/socket/example/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/socket/server.py` & `hepai-1.0.7/hai/uaii/socket/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/stream/base_input.py` & `hepai-1.0.7/hai/uaii/stream/base_input.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/stream/base_module.py` & `hepai-1.0.7/hai/uaii/stream/base_module.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/stream/base_output.py` & `hepai-1.0.7/hai/uaii/stream/base_output.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/stream/stream.py` & `hepai-1.0.7/hai/uaii/stream/stream.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/stream/streams.py` & `hepai-1.0.7/hai/uaii/stream/streams.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/uaii_main.py` & `hepai-1.0.7/hai/uaii/uaii_main.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/utils/arbitrary_import.py` & `hepai-1.0.7/hai/uaii/utils/arbitrary_import.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/utils/base_uaii.py` & `hepai-1.0.7/hai/uaii/utils/base_uaii.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import collections
 import os, sys
 from statistics import mode
 from select import select
 import numpy as np
 import copy
 import damei as dm
-import cv2
+# import cv2
 import json
 from hai.configs.Base.hai_config import WEIGHTS_ROOT, DATASETS_ROOT
 from ..datasets.datasets_hub import DatasetsHub
 from ...modules.model_hub import ModelHub
 
 logger = dm.getLogger('base_uaii')
 from . import general
@@ -140,15 +140,15 @@
         """根据模块名和类别获取模块，是未初始化的"""
         # print(args, kwargs, cls)
         ps = self.ps(**kwargs)
         # 输入的名字也可以是ID
         exist_names = [x.split()[2] for x in ps.split('\n')[1::]]
         is_exist = [idx for idx, x in enumerate(exist_names) if x.lower() == name.lower()]
         if is_exist:
-            assert len(is_exist) == 1, f'存在多个同名的模块: {name}'
+            assert len(is_exist) == 1, f'存在多个同名的模块: {name}，请在注册时修改'
             name = exist_names[is_exist[0]]
 
         if name not in exist_names:
             exist_ids = [x.split()[0] for x in ps.split('\n')[1::]]
             assert len(exist_ids) == len(exist_names)
             if name in exist_ids:
                 name = exist_names[exist_ids.index(name)]
```

### Comparing `hepai-1.0.6/hai/uaii/utils/config_loader.py` & `hepai-1.0.7/hai/uaii/utils/config_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
     def __init__(self, cfg_file=None, name=None, root_path=None, cfg_dict=None, **kwargs):
         super(PyConfigLoader, self).__init__()
         # super().__init__()
         work_dir = os.getcwd()
         self.root_path = root_path if root_path else f'{work_dir}'  # 默认当前工作目录
         self._name = name if name else f'{cfg_file}'  # 其实是path
-        # self._replace_rule = {'~': os.environ['HOME'], }
 
         self._items = dict()
         self._load_items(cfg_file, cfg_dict, **kwargs)  # 从配置文件或配置字典初始化配置，配置添加到_items和对应的属性里
         self.check_items()  # TODO
 
     def _load_items(self, cfg_file=None, cfg_dict=None, **kwargs):
         if cfg_file is None and cfg_dict is None:
@@ -278,15 +277,15 @@
             setattr(self, k, EasyDict(new_v)) if isinstance(new_v, dict) else setattr(self, k, new_v)
 
     def recursive_func(self, value):
         """递归函数,如果v类型是str,判断替换，如果循环完了，结束，如果v的类型是dict，继续循环"""
         if value is None:
             return None
         elif isinstance(value, str):
-            return value.replace('~', os.environ['HOME'])
+            return value.replace('~', str(Path.home()))
         elif isinstance(value, int):
             return value
         elif isinstance(value, float):
             return value
         elif isinstance(value, bool):
             return value
         elif isinstance(value, list):
```

### Comparing `hepai-1.0.6/hai/uaii/utils/fake_argparse.py` & `hepai-1.0.7/hai/uaii/utils/fake_argparse.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hai/uaii/utils/general.py` & `hepai-1.0.7/hai/uaii/utils/general.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.6/hepai.egg-info/SOURCES.txt` & `hepai-1.0.7/hepai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 hai/apis/modules/UNet/__init__.py
 hai/apis/modules/UNet/argparse_config.py
 hai/apis/modules/UNet/evaluate_api.py
 hai/apis/modules/UNet/predict_api.py
 hai/apis/modules/UNet/train_api.py
 hai/apis/modules/UNet/unet_api.py
 hai/apis/modules/YOLOv5/__init__.py
+hai/apis/workers_api/__init__.py
+hai/apis/workers_api/model.py
 hai/configs/__init__.py
 hai/configs/uaii_deepsort_config.py
 hai/configs/uaii_seyolov5_config.py
 hai/configs/uaii_stream_config.py
 hai/configs/visible_loader_config.py
 hai/configs/Base/__init__.py
 hai/configs/Base/hai_config.py
@@ -56,14 +58,16 @@
 hai/modules/segmentation/Pytorch_UNet/utils/utils.py
 hai/testor/__init__.py
 hai/testor/test.py
 hai/testor/test_module.py
 hai/testor/testor.py
 hai/uaii/__init__.py
 hai/uaii/uaii_main.py
+hai/uaii/actuator/__init__.py
+hai/uaii/actuator/trainer.py
 hai/uaii/cli/__init__.py
 hai/uaii/cli/cli_functions.py
 hai/uaii/cli/cli_main.py
 hai/uaii/datasets/__init__.py
 hai/uaii/datasets/dataloader.py
 hai/uaii/datasets/dataset_utils.py
 hai/uaii/datasets/datasets.py
```

### Comparing `hepai-1.0.6/setup.py` & `hepai-1.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os
 import sys
 from shutil import rmtree
 from unicodedata import name
 
 from setuptools import find_packages, setup, Command
 
-# Package meta-demo_for_dm.data.
+
 NAME = 'hepai'
 DESCRIPTION = 'High energy phscis Artificial Intelligence plateform, HAI.'
 URL = 'https://github.com/zhangzhengde0225/hai'
 EMAIL = 'zdzhang@163.com'
 AUTHOR = 'Zhengde Zhang'
 REQUIRES_PYTHON = '>=3.6.0'
 
@@ -36,16 +36,19 @@
         return f.read().splitlines()
 
 
 # REQUIRED = read_requirements()
 # REQUIRED = []
 REQUIRED = [
 	"damei",
-# 	"opencv-python",
+    "numpy",
+	# "opencv-python",
 	"easydict",
+    "grpcio-tools",
+    "requests"
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'rsa': ['rsa'],
     # 'fancy feature': ['django'],
 }
@@ -98,15 +101,15 @@
             rmtree(os.path.join(here, 'dist'))
         except OSError:
             pass
 
         self.status('Building Source and Wheel (universal) distribution…')
         os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
 
-        self.status('Uploading the package to PyPI via Twine…')
+        self.status('Uploading the package to PyPI via Twine …')
         try:
             import twine  # 需要用twine上传，但twine不一定安装，如果没装报错
         except:
             raise NameError(
                 f'You need twine to upload the package to pypi.\n'
                 f'           Install twine with "pip install twine" or switch a environment with twine.')
         os.system('twine upload dist/*')
@@ -145,14 +148,17 @@
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
```

