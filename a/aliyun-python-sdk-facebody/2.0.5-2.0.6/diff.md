# Comparing `tmp/aliyun-python-sdk-facebody-2.0.5.tar.gz` & `tmp/aliyun-python-sdk-facebody-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-facebody-2.0.5.tar", last modified: Fri Jan  6 06:45:40 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-facebody-2.0.6.tar", last modified: Fri Feb  3 05:50:03 2023, max compression
```

## Comparing `aliyun-python-sdk-facebody-2.0.5.tar` & `aliyun-python-sdk-facebody-2.0.6.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 06:45:40.000000 aliyun-python-sdk-facebody-2.0.5/
--rw-r--r--   0 root         (0) root         (0)      575 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1562 2023-01-06 06:45:40.000000 aliyun-python-sdk-facebody-2.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      537 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 06:45:40.000000 aliyun-python-sdk-facebody-2.0.5/aliyun_python_sdk_facebody.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1562 2023-01-06 06:45:40.000000 aliyun-python-sdk-facebody-2.0.5/aliyun_python_sdk_facebody.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3822 2023-01-06 06:45:40.000000 aliyun-python-sdk-facebody-2.0.5/aliyun_python_sdk_facebody.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-06 06:45:40.000000 aliyun-python-sdk-facebody-2.0.5/aliyun_python_sdk_facebody.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-01-06 06:45:40.000000 aliyun-python-sdk-facebody-2.0.5/aliyun_python_sdk_facebody.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-01-06 06:45:40.000000 aliyun-python-sdk-facebody-2.0.5/aliyun_python_sdk_facebody.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 06:45:40.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 06:45:40.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 06:45:40.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/
--rw-r--r--   0 root         (0) root         (0)     1793 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/AddFaceEntityRequest.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/AddFaceImageTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/AddFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2733 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/BatchAddFacesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3683 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/BeautifyBodyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/BlurFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/BodyPostureRequest.py
--rw-r--r--   0 root         (0) root         (0)     2281 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/CompareFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1623 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/CountCrowdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1435 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/CreateFaceDbRequest.py
--rw-r--r--   0 root         (0) root         (0)     1435 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DeleteFaceDbRequest.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DeleteFaceEntityRequest.py
--rw-r--r--   0 root         (0) root         (0)     1493 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DeleteFaceImageTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1609 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DeleteFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectBodyCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectCelebrityRequest.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectChefCapRequest.py
--rw-r--r--   0 root         (0) root         (0)     2169 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectIPCPedestrianRequest.py
--rw-r--r--   0 root         (0) root         (0)     1756 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectLivingFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectPedestrianIntrusionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1467 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectPedestrianRequest.py
--rw-r--r--   0 root         (0) root         (0)     1477 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectVideoLivingFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/EnhanceFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1655 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/ExtractFingerPrintRequest.py
--rw-r--r--   0 root         (0) root         (0)     1859 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/ExtractPedestrianFeatureAttrRequest.py
--rw-r--r--   0 root         (0) root         (0)     1935 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/FaceBeautyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/FaceFilterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2023 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/FaceMakeupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/FaceTidyupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1947 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/GenRealPersonVerificationTokenRequest.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/GenerateHumanAnimeStyleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/GenerateHumanSketchStyleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1627 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/GetFaceEntityRequest.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/GetRealPersonVerificationResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/HandPostureRequest.py
--rw-r--r--   0 root         (0) root         (0)     1645 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/LiquifyFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1597 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/ListFaceDbsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2485 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/ListFaceEntitiesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/MergeImageFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/MonitorExaminationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/PedestrianDetectAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1491 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/QueryFaceImageTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2279 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/RecognizeActionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1473 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/RecognizeExpressionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2985 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/RecognizeFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/RecognizeHandGestureRequest.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/RecognizePublicFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/RetouchBodyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/RetouchSkinRequest.py
--rw-r--r--   0 root         (0) root         (0)     2395 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/SearchFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/SwapFacialFeaturesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/UpdateFaceEntityRequest.py
--rw-r--r--   0 root         (0) root         (0)     1985 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/VerifyFaceMaskRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-01-06 06:45:40.000000 aliyun-python-sdk-facebody-2.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2477 2023-01-06 06:45:39.000000 aliyun-python-sdk-facebody-2.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      537 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyun_python_sdk_facebody.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyun_python_sdk_facebody.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3959 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyun_python_sdk_facebody.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyun_python_sdk_facebody.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyun_python_sdk_facebody.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyun_python_sdk_facebody.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/
+-rw-r--r--   0 root         (0) root         (0)     1793 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/AddFaceEntityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/AddFaceImageTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/AddFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/BatchAddFacesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3683 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/BeautifyBodyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/BlurFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/BodyPostureRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/CompareFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/CompareFaceWithMaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1623 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/CountCrowdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/CreateFaceDbRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DeleteFaceDbRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DeleteFaceEntityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DeleteFaceImageTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1609 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DeleteFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectBodyCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectCelebrityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectChefCapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectIPCPedestrianRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectInfraredLivingFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectLivingFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectPedestrianIntrusionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectPedestrianRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectVideoLivingFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/EnhanceFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/ExtractFingerPrintRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/ExtractPedestrianFeatureAttrRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/FaceBeautyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/FaceFilterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/FaceMakeupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/FaceTidyupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/GenRealPersonVerificationTokenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/GenerateHumanAnimeStyleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/GenerateHumanSketchStyleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/GetFaceEntityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/GetRealPersonVerificationResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/HandPostureRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/LiquifyFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/ListFaceDbsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/ListFaceEntitiesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/MergeImageFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/MonitorExaminationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/PedestrianDetectAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/QueryFaceImageTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/RecognizeActionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/RecognizeExpressionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/RecognizeFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/RecognizeHandGestureRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/RecognizePublicFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/RetouchBodyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/RetouchSkinRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/SearchFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/SwapFacialFeaturesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/UpdateFaceEntityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/VerifyFaceMaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-02-03 05:50:03.000000 aliyun-python-sdk-facebody-2.0.6/setup.py
```

### Comparing `aliyun-python-sdk-facebody-2.0.5/LICENSE` & `aliyun-python-sdk-facebody-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/PKG-INFO` & `aliyun-python-sdk-facebody-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-facebody
-Version: 2.0.5
+Version: 2.0.6
 Summary: The facebody module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-facebody
```

### Comparing `aliyun-python-sdk-facebody-2.0.5/README.rst` & `aliyun-python-sdk-facebody-2.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyun_python_sdk_facebody.egg-info/PKG-INFO` & `aliyun-python-sdk-facebody-2.0.6/aliyun_python_sdk_facebody.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-facebody
-Version: 2.0.5
+Version: 2.0.6
 Summary: The facebody module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-facebody
```

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyun_python_sdk_facebody.egg-info/SOURCES.txt` & `aliyun-python-sdk-facebody-2.0.6/aliyun_python_sdk_facebody.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,27 @@
 aliyunsdkfacebody/request/v20191230/AddFaceImageTemplateRequest.py
 aliyunsdkfacebody/request/v20191230/AddFaceRequest.py
 aliyunsdkfacebody/request/v20191230/BatchAddFacesRequest.py
 aliyunsdkfacebody/request/v20191230/BeautifyBodyRequest.py
 aliyunsdkfacebody/request/v20191230/BlurFaceRequest.py
 aliyunsdkfacebody/request/v20191230/BodyPostureRequest.py
 aliyunsdkfacebody/request/v20191230/CompareFaceRequest.py
+aliyunsdkfacebody/request/v20191230/CompareFaceWithMaskRequest.py
 aliyunsdkfacebody/request/v20191230/CountCrowdRequest.py
 aliyunsdkfacebody/request/v20191230/CreateFaceDbRequest.py
 aliyunsdkfacebody/request/v20191230/DeleteFaceDbRequest.py
 aliyunsdkfacebody/request/v20191230/DeleteFaceEntityRequest.py
 aliyunsdkfacebody/request/v20191230/DeleteFaceImageTemplateRequest.py
 aliyunsdkfacebody/request/v20191230/DeleteFaceRequest.py
 aliyunsdkfacebody/request/v20191230/DetectBodyCountRequest.py
 aliyunsdkfacebody/request/v20191230/DetectCelebrityRequest.py
 aliyunsdkfacebody/request/v20191230/DetectChefCapRequest.py
 aliyunsdkfacebody/request/v20191230/DetectFaceRequest.py
 aliyunsdkfacebody/request/v20191230/DetectIPCPedestrianRequest.py
+aliyunsdkfacebody/request/v20191230/DetectInfraredLivingFaceRequest.py
 aliyunsdkfacebody/request/v20191230/DetectLivingFaceRequest.py
 aliyunsdkfacebody/request/v20191230/DetectPedestrianIntrusionRequest.py
 aliyunsdkfacebody/request/v20191230/DetectPedestrianRequest.py
 aliyunsdkfacebody/request/v20191230/DetectVideoLivingFaceRequest.py
 aliyunsdkfacebody/request/v20191230/EnhanceFaceRequest.py
 aliyunsdkfacebody/request/v20191230/ExtractFingerPrintRequest.py
 aliyunsdkfacebody/request/v20191230/ExtractPedestrianFeatureAttrRequest.py
```

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/endpoint.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/AddFaceEntityRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/AddFaceEntityRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/AddFaceImageTemplateRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/AddFaceImageTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/AddFaceRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/AddFaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/BatchAddFacesRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/BatchAddFacesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/BeautifyBodyRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/BeautifyBodyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/BlurFaceRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/BlurFaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/BodyPostureRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/BodyPostureRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/CompareFaceRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/CompareFaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/CountCrowdRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/CountCrowdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/CreateFaceDbRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/CreateFaceDbRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DeleteFaceDbRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DeleteFaceDbRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DeleteFaceEntityRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DeleteFaceEntityRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DeleteFaceImageTemplateRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DeleteFaceImageTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DeleteFaceRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DeleteFaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectBodyCountRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectBodyCountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectCelebrityRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectCelebrityRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectChefCapRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectChefCapRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectFaceRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectFaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectIPCPedestrianRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectIPCPedestrianRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectLivingFaceRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectLivingFaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectPedestrianIntrusionRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectPedestrianIntrusionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectPedestrianRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectPedestrianRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/DetectVideoLivingFaceRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/DetectVideoLivingFaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/EnhanceFaceRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/EnhanceFaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/ExtractFingerPrintRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/ExtractFingerPrintRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/ExtractPedestrianFeatureAttrRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/ExtractPedestrianFeatureAttrRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/FaceBeautyRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/FaceBeautyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/FaceFilterRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/FaceFilterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/FaceMakeupRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/FaceMakeupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/FaceTidyupRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/FaceTidyupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/GenRealPersonVerificationTokenRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/GenRealPersonVerificationTokenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/GenerateHumanAnimeStyleRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/GenerateHumanAnimeStyleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/GenerateHumanSketchStyleRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/GenerateHumanSketchStyleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/GetFaceEntityRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/GetFaceEntityRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/GetRealPersonVerificationResultRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/GetRealPersonVerificationResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/HandPostureRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/HandPostureRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/LiquifyFaceRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/LiquifyFaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/ListFaceDbsRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/ListFaceDbsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/ListFaceEntitiesRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/ListFaceEntitiesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/MergeImageFaceRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/MergeImageFaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/MonitorExaminationRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/MonitorExaminationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/PedestrianDetectAttributeRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/PedestrianDetectAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/QueryFaceImageTemplateRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/QueryFaceImageTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/RecognizeActionRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/RecognizeActionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/RecognizeExpressionRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/RecognizeExpressionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/RecognizeFaceRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/RecognizeFaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/RecognizeHandGestureRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/RecognizeHandGestureRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/RecognizePublicFaceRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/RecognizePublicFaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/RetouchBodyRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/RetouchBodyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/RetouchSkinRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/RetouchSkinRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/SearchFaceRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/SearchFaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/SwapFacialFeaturesRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/SwapFacialFeaturesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/UpdateFaceEntityRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/UpdateFaceEntityRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/aliyunsdkfacebody/request/v20191230/VerifyFaceMaskRequest.py` & `aliyun-python-sdk-facebody-2.0.6/aliyunsdkfacebody/request/v20191230/VerifyFaceMaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-facebody-2.0.5/setup.py` & `aliyun-python-sdk-facebody-2.0.6/setup.py`

 * *Files identical despite different names*

