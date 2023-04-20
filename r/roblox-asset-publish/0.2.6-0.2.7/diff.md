# Comparing `tmp/roblox-asset-publish-0.2.6.tar.gz` & `tmp/roblox-asset-publish-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-asset-publish-0.2.6.tar", last modified: Wed Apr 19 12:42:00 2023, max compression
+gzip compressed data, was "roblox-asset-publish-0.2.7.tar", last modified: Thu Apr 20 23:11:56 2023, max compression
```

## Comparing `roblox-asset-publish-0.2.6.tar` & `roblox-asset-publish-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:42:00.047176 roblox-asset-publish-0.2.6/
--rw-rw-rw-   0        0        0    11558 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      454 2023-04-19 12:42:00.047176 roblox-asset-publish-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.6/README.md
--rw-rw-rw-   0        0        0      560 2023-04-19 12:41:10.000000 roblox-asset-publish-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 12:42:00.048174 roblox-asset-publish-0.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 12:42:00.006400 roblox-asset-publish-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 12:42:00.043188 roblox-asset-publish-0.2.6/src/roblox_asset_publish.egg-info/
--rw-rw-rw-   0        0        0      454 2023-04-19 12:41:59.000000 roblox-asset-publish-0.2.6/src/roblox_asset_publish.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-19 12:41:59.000000 roblox-asset-publish-0.2.6/src/roblox_asset_publish.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:41:59.000000 roblox-asset-publish-0.2.6/src/roblox_asset_publish.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-19 12:41:59.000000 roblox-asset-publish-0.2.6/src/roblox_asset_publish.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-19 12:41:59.000000 roblox-asset-publish-0.2.6/src/roblox_asset_publish.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 12:42:00.045182 roblox-asset-publish-0.2.6/src/ropublisher/
--rw-rw-rw-   0        0        0    10935 2023-04-19 12:41:05.000000 roblox-asset-publish-0.2.6/src/ropublisher/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 23:11:56.021487 roblox-asset-publish-0.2.7/
+-rw-rw-rw-   0        0        0    11558 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      454 2023-04-20 23:11:56.020478 roblox-asset-publish-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.7/README.md
+-rw-rw-rw-   0        0        0      560 2023-04-20 23:11:15.000000 roblox-asset-publish-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 23:11:56.021487 roblox-asset-publish-0.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 23:11:55.961077 roblox-asset-publish-0.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 23:11:56.013499 roblox-asset-publish-0.2.7/src/roblox_asset_publish.egg-info/
+-rw-rw-rw-   0        0        0      454 2023-04-20 23:11:55.000000 roblox-asset-publish-0.2.7/src/roblox_asset_publish.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-20 23:11:55.000000 roblox-asset-publish-0.2.7/src/roblox_asset_publish.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 23:11:55.000000 roblox-asset-publish-0.2.7/src/roblox_asset_publish.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-20 23:11:55.000000 roblox-asset-publish-0.2.7/src/roblox_asset_publish.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 23:11:55.000000 roblox-asset-publish-0.2.7/src/roblox_asset_publish.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 23:11:56.016492 roblox-asset-publish-0.2.7/src/ropublisher/
+-rw-rw-rw-   0        0        0    10934 2023-04-20 23:10:31.000000 roblox-asset-publish-0.2.7/src/ropublisher/__init__.py
```

### Comparing `roblox-asset-publish-0.2.6/LICENSE` & `roblox-asset-publish-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-asset-publish-0.2.6/pyproject.toml` & `roblox-asset-publish-0.2.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "roblox-asset-publish"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"requests==2.28.2", 
 	"mutagen==1.46.0", 
 ]
```

### Comparing `roblox-asset-publish-0.2.6/src/ropublisher/__init__.py` & `roblox-asset-publish-0.2.7/src/ropublisher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 from typing import TypedDict, Literal, Any, Union
 from requests import Session, Response
 from mutagen.wave import WAVE
 from mutagen.mp3 import MP3
 from mutagen.oggvorbis import OggVorbis
 
 OpenCloudAssetTypeName = Literal["Audio", "Decal", "Model"]
-OpenCloudAssetTypeValue = Literal[1,2,3]
+# OpenCloudAssetTypeValue = Literal[1,2,3]
 HttpMethod = Literal["POST", "GET", "PATCH", "DELETE"]
 
 LEGACY_AUDIO_URL = "https://publish.roblox.com/v1/audio"
 LEGACY_IMAGE_URL = "https://data.roblox.com/data/upload/json?assetTypeId=13"
 LEGACY_MODEL_URL = "https://data.roblox.com/data/upload/json?assetTypeId=10"
 LEGACY_PACKAGE_URL = "https://data.roblox.com/data/upload/json?assetTypeId=28"
 LEGACY_ANIMATION_URL = "https://data.roblox.com/data/upload/json?assetTypeId=20"
 LEGACY_MESH_URL = "https://data.roblox.com/data/upload/json?assetTypeId=35"
 LEGACY_MESH_URL = "https://data.roblox.com/data/upload/json?assetTypeId=35"
 ASSET_URL = "https://apis.roblox.com/assets/v1/assets"
 
-ASSET_TYPE: dict[OpenCloudAssetTypeName, OpenCloudAssetTypeValue] = {
-	"Audio": 1,
-	"Decal": 2,
-	"Model": 3,
-}
+# ASSET_TYPE: dict[OpenCloudAssetTypeName, OpenCloudAssetTypeValue] = {
+# 	"Audio": 1,
+# 	"Decal": 2,
+# 	"Model": 3,
+# }
 
 LIMITS = {
 	"Audio": {
 		"duration": 60*7,
 		"uploads_per_month": 100,
 		"is_updatable": False,
 	},
@@ -80,15 +80,15 @@
 	path: str | None
 	revisionId: str | None
 	revisionCreateTime: str | None
 
 class OpenCloudCreationAsset(OpenCloudAssetInfo):
 	description: str
 	displayName: str
-	assetType: OpenCloudAssetTypeValue
+	assetType: OpenCloudAssetTypeName
 	creationContext: OpenCloudCreationContext
 
 class OpenCloudUpdateAsset(OpenCloudAssetInfo):
 	assetId: int
 	description: str | None
 	displayName: str | None
 
@@ -182,15 +182,15 @@
 			if file_ext in type_registry:
 				asset_type = type_category
 				file_type = type_registry[file_ext]
 
 		assert file_type and asset_type, f"bad file type for {file_path}"
 
 		request_payload : OpenCloudCreationAsset = {
-			"assetType": ASSET_TYPE[asset_type],
+			"assetType": asset_type,
 			"displayName": name,
 			"description": description,
 			"creationContext": {},
 		}
 
 		if publish_to_group:
 			request_payload ["creationContext"]["creator"] = {
```

