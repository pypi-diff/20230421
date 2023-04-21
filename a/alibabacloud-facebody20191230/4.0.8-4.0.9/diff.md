# Comparing `tmp/alibabacloud_facebody20191230-4.0.8.tar.gz` & `tmp/alibabacloud_facebody20191230-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_facebody20191230-4.0.8.tar", last modified: Wed Feb  8 02:50:16 2023, max compression
+gzip compressed data, was "dist/alibabacloud_facebody20191230-4.0.9.tar", last modified: Fri Apr 21 02:52:11 2023, max compression
```

## Comparing `alibabacloud_facebody20191230-4.0.8.tar` & `alibabacloud_facebody20191230-4.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/
--rw-r--r--   0 root         (0) root         (0)     2723 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/alibabacloud_facebody20191230/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/alibabacloud_facebody20191230/__init__.py
--rw-r--r--   0 root         (0) root         (0)   502075 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/alibabacloud_facebody20191230/client.py
--rw-r--r--   0 root         (0) root         (0)   431200 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/alibabacloud_facebody20191230/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/alibabacloud_facebody20191230.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/alibabacloud_facebody20191230.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/alibabacloud_facebody20191230.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/alibabacloud_facebody20191230.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      359 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/alibabacloud_facebody20191230.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/alibabacloud_facebody20191230.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2878 2023-02-08 02:50:16.000000 alibabacloud_facebody20191230-4.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/
+-rw-r--r--   0 root         (0) root         (0)     2794 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/alibabacloud_facebody20191230/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/alibabacloud_facebody20191230/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   502759 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/alibabacloud_facebody20191230/client.py
+-rw-r--r--   0 root         (0) root         (0)   441421 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/alibabacloud_facebody20191230/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/alibabacloud_facebody20191230.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/alibabacloud_facebody20191230.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/alibabacloud_facebody20191230.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/alibabacloud_facebody20191230.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      359 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/alibabacloud_facebody20191230.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/alibabacloud_facebody20191230.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2878 2023-04-21 02:52:11.000000 alibabacloud_facebody20191230-4.0.9/setup.py
```

### Comparing `alibabacloud_facebody20191230-4.0.8/ChangeLog.md` & `alibabacloud_facebody20191230-4.0.9/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-02-08 Version: 4.0.8
+- Generated python 2019-12-30 for facebody.
+
 2023-02-03 Version: 4.0.7
 - Release CompareFaceWithMask DetectInfraredLivingFace.
 
 2023-01-11 Version: 4.0.6
 - Update sdk.
 
 2023-01-11 Version: 4.0.5
```

### Comparing `alibabacloud_facebody20191230-4.0.8/LICENSE` & `alibabacloud_facebody20191230-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_facebody20191230-4.0.8/PKG-INFO` & `alibabacloud_facebody20191230-4.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_facebody20191230
-Version: 4.0.8
+Version: 4.0.9
 Summary: Alibaba Cloud facebody (20191230) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_facebody20191230-4.0.8/README-CN.md` & `alibabacloud_facebody20191230-4.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_facebody20191230-4.0.8/README.md` & `alibabacloud_facebody20191230-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_facebody20191230-4.0.8/alibabacloud_facebody20191230/client.py` & `alibabacloud_facebody20191230-4.0.9/alibabacloud_facebody20191230/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -7615,16 +7615,22 @@
     def merge_image_face_with_options(
         self,
         request: facebody_20191230_models.MergeImageFaceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> facebody_20191230_models.MergeImageFaceResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.add_watermark):
+            body['AddWatermark'] = request.add_watermark
         if not UtilClient.is_unset(request.image_url):
             body['ImageURL'] = request.image_url
+        if not UtilClient.is_unset(request.merge_infos):
+            body['MergeInfos'] = request.merge_infos
+        if not UtilClient.is_unset(request.model_version):
+            body['ModelVersion'] = request.model_version
         if not UtilClient.is_unset(request.template_id):
             body['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='MergeImageFace',
@@ -7645,16 +7651,22 @@
     async def merge_image_face_with_options_async(
         self,
         request: facebody_20191230_models.MergeImageFaceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> facebody_20191230_models.MergeImageFaceResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.add_watermark):
+            body['AddWatermark'] = request.add_watermark
         if not UtilClient.is_unset(request.image_url):
             body['ImageURL'] = request.image_url
+        if not UtilClient.is_unset(request.merge_infos):
+            body['MergeInfos'] = request.merge_infos
+        if not UtilClient.is_unset(request.model_version):
+            body['ModelVersion'] = request.model_version
         if not UtilClient.is_unset(request.template_id):
             body['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='MergeImageFace',
```

### Comparing `alibabacloud_facebody20191230-4.0.8/alibabacloud_facebody20191230/models.py` & `alibabacloud_facebody20191230-4.0.9/alibabacloud_facebody20191230/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,36 +402,130 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ImageURL') is not None:
             self.image_urlobject = m.get('ImageURL')
         return self
 
 
+class AddFaceImageTemplateResponseBodyDataFaceInfosFaceRect(TeaModel):
+    def __init__(
+        self,
+        height: str = None,
+        width: str = None,
+        x: str = None,
+        y: str = None,
+    ):
+        self.height = height
+        self.width = width
+        self.x = x
+        self.y = y
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.height is not None:
+            result['Height'] = self.height
+        if self.width is not None:
+            result['Width'] = self.width
+        if self.x is not None:
+            result['X'] = self.x
+        if self.y is not None:
+            result['Y'] = self.y
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Height') is not None:
+            self.height = m.get('Height')
+        if m.get('Width') is not None:
+            self.width = m.get('Width')
+        if m.get('X') is not None:
+            self.x = m.get('X')
+        if m.get('Y') is not None:
+            self.y = m.get('Y')
+        return self
+
+
+class AddFaceImageTemplateResponseBodyDataFaceInfos(TeaModel):
+    def __init__(
+        self,
+        face_rect: AddFaceImageTemplateResponseBodyDataFaceInfosFaceRect = None,
+        template_face_id: str = None,
+    ):
+        self.face_rect = face_rect
+        self.template_face_id = template_face_id
+
+    def validate(self):
+        if self.face_rect:
+            self.face_rect.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.face_rect is not None:
+            result['FaceRect'] = self.face_rect.to_map()
+        if self.template_face_id is not None:
+            result['TemplateFaceID'] = self.template_face_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('FaceRect') is not None:
+            temp_model = AddFaceImageTemplateResponseBodyDataFaceInfosFaceRect()
+            self.face_rect = temp_model.from_map(m['FaceRect'])
+        if m.get('TemplateFaceID') is not None:
+            self.template_face_id = m.get('TemplateFaceID')
+        return self
+
+
 class AddFaceImageTemplateResponseBodyData(TeaModel):
     def __init__(
         self,
+        face_infos: List[AddFaceImageTemplateResponseBodyDataFaceInfos] = None,
         template_id: str = None,
     ):
+        self.face_infos = face_infos
         self.template_id = template_id
 
     def validate(self):
-        pass
+        if self.face_infos:
+            for k in self.face_infos:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        result['FaceInfos'] = []
+        if self.face_infos is not None:
+            for k in self.face_infos:
+                result['FaceInfos'].append(k.to_map() if k else None)
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        self.face_infos = []
+        if m.get('FaceInfos') is not None:
+            for k in m.get('FaceInfos'):
+                temp_model = AddFaceImageTemplateResponseBodyDataFaceInfos()
+                self.face_infos.append(temp_model.from_map(k))
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
         return self
 
 
 class AddFaceImageTemplateResponseBody(TeaModel):
     def __init__(
@@ -9937,75 +10031,193 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListFaceEntitiesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class MergeImageFaceRequestMergeInfos(TeaModel):
+    def __init__(
+        self,
+        image_url: str = None,
+        template_face_id: str = None,
+    ):
+        self.image_url = image_url
+        self.template_face_id = template_face_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.image_url is not None:
+            result['ImageURL'] = self.image_url
+        if self.template_face_id is not None:
+            result['TemplateFaceID'] = self.template_face_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ImageURL') is not None:
+            self.image_url = m.get('ImageURL')
+        if m.get('TemplateFaceID') is not None:
+            self.template_face_id = m.get('TemplateFaceID')
+        return self
+
+
 class MergeImageFaceRequest(TeaModel):
     def __init__(
         self,
+        add_watermark: bool = None,
         image_url: str = None,
+        merge_infos: List[MergeImageFaceRequestMergeInfos] = None,
+        model_version: str = None,
         template_id: str = None,
     ):
+        self.add_watermark = add_watermark
         self.image_url = image_url
+        self.merge_infos = merge_infos
+        self.model_version = model_version
         self.template_id = template_id
 
     def validate(self):
-        pass
+        if self.merge_infos:
+            for k in self.merge_infos:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.add_watermark is not None:
+            result['AddWatermark'] = self.add_watermark
         if self.image_url is not None:
             result['ImageURL'] = self.image_url
+        result['MergeInfos'] = []
+        if self.merge_infos is not None:
+            for k in self.merge_infos:
+                result['MergeInfos'].append(k.to_map() if k else None)
+        if self.model_version is not None:
+            result['ModelVersion'] = self.model_version
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AddWatermark') is not None:
+            self.add_watermark = m.get('AddWatermark')
         if m.get('ImageURL') is not None:
             self.image_url = m.get('ImageURL')
+        self.merge_infos = []
+        if m.get('MergeInfos') is not None:
+            for k in m.get('MergeInfos'):
+                temp_model = MergeImageFaceRequestMergeInfos()
+                self.merge_infos.append(temp_model.from_map(k))
+        if m.get('ModelVersion') is not None:
+            self.model_version = m.get('ModelVersion')
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
         return self
 
 
+class MergeImageFaceAdvanceRequestMergeInfos(TeaModel):
+    def __init__(
+        self,
+        image_url: str = None,
+        template_face_id: str = None,
+    ):
+        self.image_url = image_url
+        self.template_face_id = template_face_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.image_url is not None:
+            result['ImageURL'] = self.image_url
+        if self.template_face_id is not None:
+            result['TemplateFaceID'] = self.template_face_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ImageURL') is not None:
+            self.image_url = m.get('ImageURL')
+        if m.get('TemplateFaceID') is not None:
+            self.template_face_id = m.get('TemplateFaceID')
+        return self
+
+
 class MergeImageFaceAdvanceRequest(TeaModel):
     def __init__(
         self,
+        add_watermark: bool = None,
         image_urlobject: BinaryIO = None,
+        merge_infos: List[MergeImageFaceAdvanceRequestMergeInfos] = None,
+        model_version: str = None,
         template_id: str = None,
     ):
+        self.add_watermark = add_watermark
         self.image_urlobject = image_urlobject
+        self.merge_infos = merge_infos
+        self.model_version = model_version
         self.template_id = template_id
 
     def validate(self):
-        pass
+        if self.merge_infos:
+            for k in self.merge_infos:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.add_watermark is not None:
+            result['AddWatermark'] = self.add_watermark
         if self.image_urlobject is not None:
             result['ImageURL'] = self.image_urlobject
+        result['MergeInfos'] = []
+        if self.merge_infos is not None:
+            for k in self.merge_infos:
+                result['MergeInfos'].append(k.to_map() if k else None)
+        if self.model_version is not None:
+            result['ModelVersion'] = self.model_version
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AddWatermark') is not None:
+            self.add_watermark = m.get('AddWatermark')
         if m.get('ImageURL') is not None:
             self.image_urlobject = m.get('ImageURL')
+        self.merge_infos = []
+        if m.get('MergeInfos') is not None:
+            for k in m.get('MergeInfos'):
+                temp_model = MergeImageFaceAdvanceRequestMergeInfos()
+                self.merge_infos.append(temp_model.from_map(k))
+        if m.get('ModelVersion') is not None:
+            self.model_version = m.get('ModelVersion')
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
         return self
 
 
 class MergeImageFaceResponseBodyData(TeaModel):
     def __init__(
@@ -11297,54 +11509,148 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
         return self
 
 
+class QueryFaceImageTemplateResponseBodyDataElementsFaceInfosFaceRect(TeaModel):
+    def __init__(
+        self,
+        height: str = None,
+        width: str = None,
+        x: str = None,
+        y: str = None,
+    ):
+        self.height = height
+        self.width = width
+        self.x = x
+        self.y = y
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.height is not None:
+            result['Height'] = self.height
+        if self.width is not None:
+            result['Width'] = self.width
+        if self.x is not None:
+            result['X'] = self.x
+        if self.y is not None:
+            result['Y'] = self.y
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Height') is not None:
+            self.height = m.get('Height')
+        if m.get('Width') is not None:
+            self.width = m.get('Width')
+        if m.get('X') is not None:
+            self.x = m.get('X')
+        if m.get('Y') is not None:
+            self.y = m.get('Y')
+        return self
+
+
+class QueryFaceImageTemplateResponseBodyDataElementsFaceInfos(TeaModel):
+    def __init__(
+        self,
+        face_rect: QueryFaceImageTemplateResponseBodyDataElementsFaceInfosFaceRect = None,
+        template_face_id: str = None,
+    ):
+        self.face_rect = face_rect
+        self.template_face_id = template_face_id
+
+    def validate(self):
+        if self.face_rect:
+            self.face_rect.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.face_rect is not None:
+            result['FaceRect'] = self.face_rect.to_map()
+        if self.template_face_id is not None:
+            result['TemplateFaceID'] = self.template_face_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('FaceRect') is not None:
+            temp_model = QueryFaceImageTemplateResponseBodyDataElementsFaceInfosFaceRect()
+            self.face_rect = temp_model.from_map(m['FaceRect'])
+        if m.get('TemplateFaceID') is not None:
+            self.template_face_id = m.get('TemplateFaceID')
+        return self
+
+
 class QueryFaceImageTemplateResponseBodyDataElements(TeaModel):
     def __init__(
         self,
         create_time: str = None,
+        face_infos: List[QueryFaceImageTemplateResponseBodyDataElementsFaceInfos] = None,
         template_id: str = None,
         template_url: str = None,
         update_time: str = None,
         user_id: str = None,
     ):
         self.create_time = create_time
+        self.face_infos = face_infos
         self.template_id = template_id
         self.template_url = template_url
         self.update_time = update_time
         self.user_id = user_id
 
     def validate(self):
-        pass
+        if self.face_infos:
+            for k in self.face_infos:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
+        result['FaceInfos'] = []
+        if self.face_infos is not None:
+            for k in self.face_infos:
+                result['FaceInfos'].append(k.to_map() if k else None)
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
         if self.template_url is not None:
             result['TemplateURL'] = self.template_url
         if self.update_time is not None:
             result['UpdateTime'] = self.update_time
         if self.user_id is not None:
             result['UserId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
+        self.face_infos = []
+        if m.get('FaceInfos') is not None:
+            for k in m.get('FaceInfos'):
+                temp_model = QueryFaceImageTemplateResponseBodyDataElementsFaceInfos()
+                self.face_infos.append(temp_model.from_map(k))
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
         if m.get('TemplateURL') is not None:
             self.template_url = m.get('TemplateURL')
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         if m.get('UserId') is not None:
```

### Comparing `alibabacloud_facebody20191230-4.0.8/alibabacloud_facebody20191230.egg-info/PKG-INFO` & `alibabacloud_facebody20191230-4.0.9/alibabacloud_facebody20191230.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-facebody20191230
-Version: 4.0.8
+Version: 4.0.9
 Summary: Alibaba Cloud facebody (20191230) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_facebody20191230-4.0.8/setup.py` & `alibabacloud_facebody20191230-4.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_facebody20191230.
 
-Created on 08/02/2023
+Created on 21/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_facebody20191230"
 NAME = "alibabacloud_facebody20191230" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud facebody (20191230) SDK Library for Python"
@@ -39,15 +39,15 @@
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_oss_sdk>=0.1.0, <1.0.0",
     "alibabacloud_openplatform20191219>=2.0.0, <3.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
     "alibabacloud_tea_fileform>=0.0.3, <1.0.0",
     "alibabacloud_darabonba_number>=0.0.4, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.7, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

