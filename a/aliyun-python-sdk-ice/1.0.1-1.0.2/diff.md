# Comparing `tmp/aliyun-python-sdk-ice-1.0.1.tar.gz` & `tmp/aliyun-python-sdk-ice-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-ice-1.0.1.tar", last modified: Wed Mar  1 07:30:45 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-ice-1.0.2.tar", last modified: Fri Apr 21 17:16:00 2023, max compression
```

## Comparing `aliyun-python-sdk-ice-1.0.1.tar` & `aliyun-python-sdk-ice-1.0.2.tar`

### file list

```diff
@@ -1,186 +1,192 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      575 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyun_python_sdk_ice.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyun_python_sdk_ice.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10621 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyun_python_sdk_ice.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyun_python_sdk_ice.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyun_python_sdk_ice.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyun_python_sdk_ice.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3511 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/
--rw-r--r--   0 root         (0) root         (0)     1773 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/AddCategoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/AddEditingProjectMaterialsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/AddFavoritePublicMediaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/AddMediaMarksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/AddTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/BatchGetMediaInfosRequest.py
--rw-r--r--   0 root         (0) root         (0)     2267 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CancelDNAJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CancelFavoritePublicMediaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateAuditRequest.py
--rw-r--r--   0 root         (0) root         (0)     1984 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateCustomTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateDNADBRequest.py
--rw-r--r--   0 root         (0) root         (0)     2995 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateEditingProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateLiveRecordTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2134 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateLiveSnapshotTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1845 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateLiveTranscodeTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreatePipelineRequest.py
--rw-r--r--   0 root         (0) root         (0)     2655 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateUploadMediaRequest.py
--rw-r--r--   0 root         (0) root         (0)     2203 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateUploadStreamRequest.py
--rw-r--r--   0 root         (0) root         (0)     1433 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteCategoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1473 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteCustomTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2259 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteDNADBRequest.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteDNAFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1885 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteEditingProjectMaterialsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteEditingProjectsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteLiveRecordFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1481 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteLiveRecordTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteLiveSnapshotFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1484 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteLiveSnapshotTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteLiveTranscodeJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteLiveTranscodeTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1885 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteMediaInfosRequest.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteMediaMarksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeletePipelineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeletePlayInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1431 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteSmartJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1439 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeFilterConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1960 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterIceEditUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1984 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterIceLiveMediaConvertUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterIceMediaConvertUHDUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1976 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterIceMediaConvertUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1962 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterIceMpsAiUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1960 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsEditUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1968 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsLiveEditUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1984 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsLiveMediaConvertUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsLiveRecordUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1976 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsLiveSnapshotUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsMediaConvertUHDUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1976 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsMediaConvertUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1962 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsMpsAiUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1781 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsSummaryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1630 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribePlayDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1986 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribePlayEventListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribePlayFirstFrameDurationMetricDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2847 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribePlayListRequest.py
--rw-r--r--   0 root         (0) root         (0)     3295 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribePlayMetricDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     3625 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribePlayQoeListRequest.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribePlayQosListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeQueryConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetCategoriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetCustomTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1292 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetDefaultStorageLocationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1439 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetDynamicImageJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetEditingProjectMaterialsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetEditingProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetEventCallbackRequest.py
--rw-r--r--   0 root         (0) root         (0)     2028 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveEditingIndexFileRequest.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveEditingJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1434 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveRecordJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveRecordTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveSnapshotJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1478 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveSnapshotTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveTranscodeJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1481 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveTranscodeTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1433 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetMediaInfoJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1809 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetMediaInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetMediaMarksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetMediaProducingJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1429 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetPackageJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1455 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetPipelineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1616 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetPlayInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetPublicMediaInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetSmartHandleJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1431 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetSnapshotJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2149 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetSnapshotUrlsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1467 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetSystemTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetTemplateMaterialsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetTemplateParamsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1469 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetTranscodeJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetUrlUploadInfosRequest.py
--rw-r--r--   0 root         (0) root         (0)     1439 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetWorkflowTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListAllPublicMediaTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2501 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListCustomTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2261 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListDNADBRequest.py
--rw-r--r--   0 root         (0) root         (0)     2651 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListDNAFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2627 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListDynamicImageJobsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2586 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveRecordFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveRecordJobsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2397 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveRecordTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveSnapshotFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2532 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveSnapshotJobsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveSnapshotTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2485 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveTranscodeJobsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveTranscodeTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3331 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListMediaBasicInfosRequest.py
--rw-r--r--   0 root         (0) root         (0)     2621 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListMediaInfoJobsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListMediaMarksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListPackageJobsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1429 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListPipelinesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListPublicMediaBasicInfosRequest.py
--rw-r--r--   0 root         (0) root         (0)     2496 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListSmartJobsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2619 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListSnapshotJobsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2495 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListSystemTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2657 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListTranscodeJobsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2279 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/QueryDNAJobListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1638 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/QueryIProductionJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/QueryMediaCensorJobDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     3635 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/QueryMediaCensorJobListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/QuerySmarttagJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/RefreshUploadMediaRequest.py
--rw-r--r--   0 root         (0) root         (0)     3894 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/RegisterMediaInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/RegisterMediaStreamRequest.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SearchEditingProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SearchMediaRequest.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SearchPublicMediaInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SendLiveSnapshotJobCommandRequest.py
--rw-r--r--   0 root         (0) root         (0)     1630 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SendLiveTranscodeJobCommandRequest.py
--rw-r--r--   0 root         (0) root         (0)     1481 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SetDefaultCustomTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SetDefaultStorageLocationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SetEventCallbackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1823 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/StartWorkflowRequest.py
--rw-r--r--   0 root         (0) root         (0)     2352 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitASRJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitAudioProduceJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     3365 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitDNAJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     3665 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitDynamicChartJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2436 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitDynamicImageJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2786 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitIProductionJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2739 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitLiveEditingJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitLiveRecordJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitLiveSnapshotJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2482 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitLiveTranscodeJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     3150 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitMediaCensorJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2024 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitMediaInfoJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     3515 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitMediaProducingJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2203 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitPackageJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     3138 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitSmarttagJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitSnapshotJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitSubtitleProduceJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitSyncMediaInfoJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2259 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitTranscodeJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1612 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateCategoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateCustomTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2780 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateEditingProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1858 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateLiveRecordTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateLiveSnapshotTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2265 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateLiveTranscodeJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateLiveTranscodeTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     3460 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateMediaInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1638 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateMediaMarksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdatePipelineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1610 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateSmartJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     2720 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2665 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UploadMediaByURLRequest.py
--rw-r--r--   0 root         (0) root         (0)     2386 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UploadStreamByURLRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2023-03-01 07:30:45.000000 aliyun-python-sdk-ice-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 17:16:00.000000 aliyun-python-sdk-ice-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-04-21 17:16:00.000000 aliyun-python-sdk-ice-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 17:16:00.000000 aliyun-python-sdk-ice-1.0.2/aliyun_python_sdk_ice.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyun_python_sdk_ice.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11001 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyun_python_sdk_ice.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyun_python_sdk_ice.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyun_python_sdk_ice.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyun_python_sdk_ice.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 17:16:00.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3511 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 17:16:00.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 17:16:00.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/AddCategoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/AddEditingProjectMaterialsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/AddFavoritePublicMediaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/AddMediaMarksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/AddTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/BatchGetMediaInfosRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CancelDNAJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CancelFavoritePublicMediaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateAuditRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateCustomTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateDNADBRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateEditingProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateLiveRecordTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2134 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateLiveSnapshotTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateLiveTranscodeTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreatePipelineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateUploadMediaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateUploadStreamRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1433 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteCategoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteCustomTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteDNADBRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteDNAFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteEditingProjectMaterialsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteEditingProjectsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteLiveRecordFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteLiveRecordTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteLiveSnapshotFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteLiveSnapshotTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteLiveTranscodeJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteLiveTranscodeTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteMediaInfosRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteMediaMarksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeletePipelineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeletePlayInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1431 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteSmartJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeFilterConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterIceEditUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterIceLiveMediaConvertUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterIceMediaConvertUHDUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterIceMediaConvertUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1962 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterIceMpsAiUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsEditUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1968 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsLiveEditUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsLiveMediaConvertUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsLiveRecordUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsLiveSnapshotUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsMediaConvertUHDUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsMediaConvertUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1962 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsMpsAiUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsSummaryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribePlayDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribePlayEventListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribePlayFirstFrameDurationMetricDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribePlayListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3295 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribePlayMetricDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3625 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribePlayQoeListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribePlayQosListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeQueryConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetCategoriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1288 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetContentAnalyzeConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetCustomTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetDefaultStorageLocationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetDynamicImageJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetEditingProjectMaterialsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetEditingProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetEventCallbackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2028 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveEditingIndexFileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveEditingJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveRecordJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveRecordTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveSnapshotJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveSnapshotTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveTranscodeJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveTranscodeTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1433 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetMediaInfoJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetMediaInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetMediaMarksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetMediaProducingJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetPackageJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetPipelineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetPlayInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetPublicMediaInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetSmartHandleJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1431 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetSnapshotJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetSnapshotUrlsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetSystemTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetTemplateMaterialsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetTemplateParamsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetTranscodeJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetUrlUploadInfosRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetWorkflowTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListAllPublicMediaTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListCustomTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListDNADBRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListDNAFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListDynamicImageJobsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveRecordFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveRecordJobsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveRecordTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveSnapshotFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveSnapshotJobsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveSnapshotTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveTranscodeJobsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveTranscodeTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3331 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListMediaBasicInfosRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2621 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListMediaInfoJobsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListMediaMarksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListPackageJobsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListPipelinesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListPublicMediaBasicInfosRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListSmartJobsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListSmartSysAvatarModelsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListSnapshotJobsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListSystemTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListTranscodeJobsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/QueryDNAJobListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/QueryIProductionJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/QueryMediaCensorJobDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3635 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/QueryMediaCensorJobListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/QuerySmarttagJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/RefreshUploadMediaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3894 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/RegisterMediaInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/RegisterMediaStreamRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SearchEditingProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SearchMediaByFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SearchMediaClipByFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SearchMediaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SearchPublicMediaInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SendLiveSnapshotJobCommandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SendLiveTranscodeJobCommandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SetContentAnalyzeConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SetDefaultCustomTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SetDefaultStorageLocationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SetEventCallbackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/StartWorkflowRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitASRJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitAudioProduceJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitAvatarVideoJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3365 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitDNAJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3665 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitDynamicChartJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitDynamicImageJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitIProductionJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitLiveEditingJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitLiveRecordJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitLiveSnapshotJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitLiveTranscodeJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitMediaCensorJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitMediaInfoJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3515 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitMediaProducingJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitPackageJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitSmarttagJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitSnapshotJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitSubtitleProduceJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitSyncMediaInfoJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitTranscodeJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateCategoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateCustomTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateEditingProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateLiveRecordTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateLiveSnapshotTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateLiveTranscodeJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateLiveTranscodeTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3460 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateMediaInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateMediaMarksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdatePipelineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateSmartJobRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UploadMediaByURLRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UploadStreamByURLRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-21 17:16:00.000000 aliyun-python-sdk-ice-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-04-21 17:15:59.000000 aliyun-python-sdk-ice-1.0.2/setup.py
```

### Comparing `aliyun-python-sdk-ice-1.0.1/LICENSE` & `aliyun-python-sdk-ice-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/PKG-INFO` & `aliyun-python-sdk-ice-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ice
-Version: 1.0.1
+Version: 1.0.2
 Summary: The ice module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-ice
```

### Comparing `aliyun-python-sdk-ice-1.0.1/README.rst` & `aliyun-python-sdk-ice-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyun_python_sdk_ice.egg-info/PKG-INFO` & `aliyun-python-sdk-ice-1.0.2/aliyun_python_sdk_ice.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ice
-Version: 1.0.1
+Version: 1.0.2
 Summary: The ice module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-ice
```

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyun_python_sdk_ice.egg-info/SOURCES.txt` & `aliyun-python-sdk-ice-1.0.2/aliyun_python_sdk_ice.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 aliyunsdkice/request/v20201109/DescribePlayFirstFrameDurationMetricDataRequest.py
 aliyunsdkice/request/v20201109/DescribePlayListRequest.py
 aliyunsdkice/request/v20201109/DescribePlayMetricDataRequest.py
 aliyunsdkice/request/v20201109/DescribePlayQoeListRequest.py
 aliyunsdkice/request/v20201109/DescribePlayQosListRequest.py
 aliyunsdkice/request/v20201109/DescribeQueryConfigsRequest.py
 aliyunsdkice/request/v20201109/GetCategoriesRequest.py
+aliyunsdkice/request/v20201109/GetContentAnalyzeConfigRequest.py
 aliyunsdkice/request/v20201109/GetCustomTemplateRequest.py
 aliyunsdkice/request/v20201109/GetDefaultStorageLocationRequest.py
 aliyunsdkice/request/v20201109/GetDynamicImageJobRequest.py
 aliyunsdkice/request/v20201109/GetEditingProjectMaterialsRequest.py
 aliyunsdkice/request/v20201109/GetEditingProjectRequest.py
 aliyunsdkice/request/v20201109/GetEventCallbackRequest.py
 aliyunsdkice/request/v20201109/GetLiveEditingIndexFileRequest.py
@@ -119,37 +120,42 @@
 aliyunsdkice/request/v20201109/ListMediaBasicInfosRequest.py
 aliyunsdkice/request/v20201109/ListMediaInfoJobsRequest.py
 aliyunsdkice/request/v20201109/ListMediaMarksRequest.py
 aliyunsdkice/request/v20201109/ListPackageJobsRequest.py
 aliyunsdkice/request/v20201109/ListPipelinesRequest.py
 aliyunsdkice/request/v20201109/ListPublicMediaBasicInfosRequest.py
 aliyunsdkice/request/v20201109/ListSmartJobsRequest.py
+aliyunsdkice/request/v20201109/ListSmartSysAvatarModelsRequest.py
 aliyunsdkice/request/v20201109/ListSnapshotJobsRequest.py
 aliyunsdkice/request/v20201109/ListSystemTemplatesRequest.py
 aliyunsdkice/request/v20201109/ListTemplatesRequest.py
 aliyunsdkice/request/v20201109/ListTranscodeJobsRequest.py
 aliyunsdkice/request/v20201109/QueryDNAJobListRequest.py
 aliyunsdkice/request/v20201109/QueryIProductionJobRequest.py
 aliyunsdkice/request/v20201109/QueryMediaCensorJobDetailRequest.py
 aliyunsdkice/request/v20201109/QueryMediaCensorJobListRequest.py
 aliyunsdkice/request/v20201109/QuerySmarttagJobRequest.py
 aliyunsdkice/request/v20201109/RefreshUploadMediaRequest.py
 aliyunsdkice/request/v20201109/RegisterMediaInfoRequest.py
 aliyunsdkice/request/v20201109/RegisterMediaStreamRequest.py
 aliyunsdkice/request/v20201109/SearchEditingProjectRequest.py
+aliyunsdkice/request/v20201109/SearchMediaByFaceRequest.py
+aliyunsdkice/request/v20201109/SearchMediaClipByFaceRequest.py
 aliyunsdkice/request/v20201109/SearchMediaRequest.py
 aliyunsdkice/request/v20201109/SearchPublicMediaInfoRequest.py
 aliyunsdkice/request/v20201109/SendLiveSnapshotJobCommandRequest.py
 aliyunsdkice/request/v20201109/SendLiveTranscodeJobCommandRequest.py
+aliyunsdkice/request/v20201109/SetContentAnalyzeConfigRequest.py
 aliyunsdkice/request/v20201109/SetDefaultCustomTemplateRequest.py
 aliyunsdkice/request/v20201109/SetDefaultStorageLocationRequest.py
 aliyunsdkice/request/v20201109/SetEventCallbackRequest.py
 aliyunsdkice/request/v20201109/StartWorkflowRequest.py
 aliyunsdkice/request/v20201109/SubmitASRJobRequest.py
 aliyunsdkice/request/v20201109/SubmitAudioProduceJobRequest.py
+aliyunsdkice/request/v20201109/SubmitAvatarVideoJobRequest.py
 aliyunsdkice/request/v20201109/SubmitDNAJobRequest.py
 aliyunsdkice/request/v20201109/SubmitDynamicChartJobRequest.py
 aliyunsdkice/request/v20201109/SubmitDynamicImageJobRequest.py
 aliyunsdkice/request/v20201109/SubmitIProductionJobRequest.py
 aliyunsdkice/request/v20201109/SubmitLiveEditingJobRequest.py
 aliyunsdkice/request/v20201109/SubmitLiveRecordJobRequest.py
 aliyunsdkice/request/v20201109/SubmitLiveSnapshotJobRequest.py
```

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/endpoint.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/AddCategoryRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/AddCategoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/AddEditingProjectMaterialsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/AddEditingProjectMaterialsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/AddFavoritePublicMediaRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/AddFavoritePublicMediaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/AddMediaMarksRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/AddMediaMarksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/AddTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/AddTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/BatchGetMediaInfosRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/BatchGetMediaInfosRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CancelDNAJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CancelDNAJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CancelFavoritePublicMediaRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CancelFavoritePublicMediaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateAuditRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateAuditRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateCustomTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateCustomTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateDNADBRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateDNADBRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateEditingProjectRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateEditingProjectRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 	def set_MaterialMaps(self, MaterialMaps):  # String
 		self.add_query_param('MaterialMaps', MaterialMaps)
 	def get_CoverURL(self): # String
 		return self.get_query_params().get('CoverURL')
 
 	def set_CoverURL(self, CoverURL):  # String
 		self.add_query_param('CoverURL', CoverURL)
+	def get_TemplateType(self): # String
+		return self.get_query_params().get('TemplateType')
+
+	def set_TemplateType(self, TemplateType):  # String
+		self.add_query_param('TemplateType', TemplateType)
 	def get_ProjectType(self): # String
 		return self.get_query_params().get('ProjectType')
 
 	def set_ProjectType(self, ProjectType):  # String
 		self.add_query_param('ProjectType', ProjectType)
 	def get_TemplateId(self): # String
 		return self.get_query_params().get('TemplateId')
```

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateLiveRecordTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateLiveRecordTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateLiveSnapshotTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateLiveSnapshotTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateLiveTranscodeTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateLiveTranscodeTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreatePipelineRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreatePipelineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateUploadMediaRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateUploadMediaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/CreateUploadStreamRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/CreateUploadStreamRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteCategoryRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteCategoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteCustomTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteCustomTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteDNADBRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteDNADBRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteDNAFilesRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteDNAFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteEditingProjectMaterialsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteEditingProjectMaterialsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteEditingProjectsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteEditingProjectsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteLiveRecordFilesRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteLiveRecordFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteLiveRecordTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteLiveRecordTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteLiveSnapshotFilesRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteLiveSnapshotFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteLiveSnapshotTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteLiveSnapshotTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteLiveTranscodeJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteLiveTranscodeJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteLiveTranscodeTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteLiveTranscodeTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteMediaInfosRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteMediaInfosRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteMediaMarksRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteMediaMarksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeletePipelineRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeletePipelineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeletePlayInfoRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeletePlayInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteSmartJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteSmartJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DeleteTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DeleteTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeFilterConfigsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeFilterConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterIceEditUsageRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterIceEditUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterIceLiveMediaConvertUsageRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterIceLiveMediaConvertUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterIceMediaConvertUHDUsageRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterIceMediaConvertUHDUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterIceMediaConvertUsageRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterIceMediaConvertUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterIceMpsAiUsageRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterIceMpsAiUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsEditUsageRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsEditUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsLiveEditUsageRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsLiveEditUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsLiveMediaConvertUsageRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsLiveMediaConvertUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsLiveRecordUsageRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsLiveRecordUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsLiveSnapshotUsageRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsLiveSnapshotUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsMediaConvertUHDUsageRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsMediaConvertUHDUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsMediaConvertUsageRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsMediaConvertUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsMpsAiUsageRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsMpsAiUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeMeterImsSummaryRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeMeterImsSummaryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribePlayDetailRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribePlayDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribePlayEventListRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribePlayEventListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribePlayFirstFrameDurationMetricDataRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribePlayFirstFrameDurationMetricDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribePlayListRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribePlayListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribePlayMetricDataRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribePlayMetricDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribePlayQoeListRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribePlayQoeListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribePlayQosListRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribePlayQosListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/DescribeQueryConfigsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/DescribeQueryConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetCategoriesRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetCategoriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetCustomTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetCustomTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetDefaultStorageLocationRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetDefaultStorageLocationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetDynamicImageJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetDynamicImageJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetEditingProjectMaterialsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetEditingProjectMaterialsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetEditingProjectRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetEditingProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetEventCallbackRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetEventCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveEditingIndexFileRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveEditingIndexFileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveEditingJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveEditingJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveRecordJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveRecordJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveRecordTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveRecordTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveSnapshotJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveSnapshotJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveSnapshotTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveSnapshotTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveTranscodeJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveTranscodeJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetLiveTranscodeTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetLiveTranscodeTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetMediaInfoJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetMediaInfoJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetMediaInfoRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetMediaInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetMediaMarksRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetMediaMarksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetMediaProducingJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetMediaProducingJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetPackageJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetPackageJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetPipelineRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetPipelineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetPlayInfoRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetPlayInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetPublicMediaInfoRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetPublicMediaInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetSmartHandleJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetSmartHandleJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetSnapshotJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetSnapshotJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetSnapshotUrlsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetSnapshotUrlsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetSystemTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetSystemTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetTemplateMaterialsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetTemplateMaterialsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetTemplateParamsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetTemplateParamsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetTranscodeJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetTranscodeJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetUrlUploadInfosRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetUrlUploadInfosRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/GetWorkflowTaskRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/GetWorkflowTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListAllPublicMediaTagsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListAllPublicMediaTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListCustomTemplatesRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListCustomTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListDNADBRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListDNADBRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListDNAFilesRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListDNAFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListDynamicImageJobsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListDynamicImageJobsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveRecordFilesRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveRecordFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveRecordJobsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveRecordJobsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveRecordTemplatesRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveRecordTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveSnapshotFilesRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveSnapshotFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveSnapshotJobsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveSnapshotJobsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveSnapshotTemplatesRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveSnapshotTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveTranscodeJobsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveTranscodeJobsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListLiveTranscodeTemplatesRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListLiveTranscodeTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListMediaBasicInfosRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListMediaBasicInfosRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListMediaInfoJobsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListMediaInfoJobsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListMediaMarksRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListMediaMarksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListPackageJobsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListPackageJobsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListPipelinesRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListPipelinesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListPublicMediaBasicInfosRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListPublicMediaBasicInfosRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListSmartJobsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListSmartJobsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListSnapshotJobsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListSnapshotJobsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListSystemTemplatesRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListSystemTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListTemplatesRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/ListTranscodeJobsRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/ListTranscodeJobsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/QueryDNAJobListRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/QueryDNAJobListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/QueryIProductionJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/QueryIProductionJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/QueryMediaCensorJobDetailRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/QueryMediaCensorJobDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/QueryMediaCensorJobListRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/QueryMediaCensorJobListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/QuerySmarttagJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/QuerySmarttagJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/RefreshUploadMediaRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/RefreshUploadMediaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/RegisterMediaInfoRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/RegisterMediaInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/RegisterMediaStreamRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/RegisterMediaStreamRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SearchEditingProjectRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SearchEditingProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SearchMediaRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SearchMediaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SearchPublicMediaInfoRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SearchPublicMediaInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SendLiveSnapshotJobCommandRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SendLiveSnapshotJobCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SendLiveTranscodeJobCommandRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SendLiveTranscodeJobCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SetDefaultCustomTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SetDefaultCustomTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SetDefaultStorageLocationRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SetDefaultStorageLocationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SetEventCallbackRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SetEventCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/StartWorkflowRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/StartWorkflowRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitASRJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitASRJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitAudioProduceJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitAudioProduceJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitDNAJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitDNAJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitDynamicChartJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitDynamicChartJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitDynamicImageJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitDynamicImageJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitIProductionJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitIProductionJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitLiveEditingJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitLiveEditingJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitLiveRecordJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitLiveRecordJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitLiveSnapshotJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitLiveSnapshotJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitLiveTranscodeJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitLiveTranscodeJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitMediaCensorJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitMediaCensorJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitMediaInfoJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitMediaInfoJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitMediaProducingJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitMediaProducingJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitPackageJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitPackageJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitSmarttagJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitSmarttagJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitSnapshotJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitSnapshotJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitSubtitleProduceJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitSubtitleProduceJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitSyncMediaInfoJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitSyncMediaInfoJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/SubmitTranscodeJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/SubmitTranscodeJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateCategoryRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateCategoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateCustomTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateCustomTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateEditingProjectRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateEditingProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateLiveRecordTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateLiveRecordTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateLiveSnapshotTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateLiveSnapshotTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateLiveTranscodeJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateLiveTranscodeJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateLiveTranscodeTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateLiveTranscodeTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateMediaInfoRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateMediaInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateMediaMarksRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateMediaMarksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdatePipelineRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdatePipelineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateSmartJobRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateSmartJobRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UpdateTemplateRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UpdateTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UploadMediaByURLRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UploadMediaByURLRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/aliyunsdkice/request/v20201109/UploadStreamByURLRequest.py` & `aliyun-python-sdk-ice-1.0.2/aliyunsdkice/request/v20201109/UploadStreamByURLRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ice-1.0.1/setup.py` & `aliyun-python-sdk-ice-1.0.2/setup.py`

 * *Files identical despite different names*

