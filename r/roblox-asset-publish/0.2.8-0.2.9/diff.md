# Comparing `tmp/roblox-asset-publish-0.2.8.tar.gz` & `tmp/roblox-asset-publish-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-asset-publish-0.2.8.tar", last modified: Thu Apr 20 23:15:14 2023, max compression
+gzip compressed data, was "roblox-asset-publish-0.2.9.tar", last modified: Thu Apr 20 23:24:32 2023, max compression
```

## Comparing `roblox-asset-publish-0.2.8.tar` & `roblox-asset-publish-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 23:15:14.994816 roblox-asset-publish-0.2.8/
--rw-rw-rw-   0        0        0    11558 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.8/LICENSE
--rw-rw-rw-   0        0        0      454 2023-04-20 23:15:14.993820 roblox-asset-publish-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.8/README.md
--rw-rw-rw-   0        0        0      560 2023-04-20 23:14:50.000000 roblox-asset-publish-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 23:15:14.994816 roblox-asset-publish-0.2.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-20 23:15:14.958925 roblox-asset-publish-0.2.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-20 23:15:14.990851 roblox-asset-publish-0.2.8/src/roblox_asset_publish.egg-info/
--rw-rw-rw-   0        0        0      454 2023-04-20 23:15:14.000000 roblox-asset-publish-0.2.8/src/roblox_asset_publish.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-20 23:15:14.000000 roblox-asset-publish-0.2.8/src/roblox_asset_publish.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 23:15:14.000000 roblox-asset-publish-0.2.8/src/roblox_asset_publish.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-20 23:15:14.000000 roblox-asset-publish-0.2.8/src/roblox_asset_publish.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-20 23:15:14.000000 roblox-asset-publish-0.2.8/src/roblox_asset_publish.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 23:15:14.991825 roblox-asset-publish-0.2.8/src/ropublisher/
--rw-rw-rw-   0        0        0    10946 2023-04-20 23:14:50.000000 roblox-asset-publish-0.2.8/src/ropublisher/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 23:24:32.945654 roblox-asset-publish-0.2.9/
+-rw-rw-rw-   0        0        0    11558 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      454 2023-04-20 23:24:32.944657 roblox-asset-publish-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-04-19 07:49:48.000000 roblox-asset-publish-0.2.9/README.md
+-rw-rw-rw-   0        0        0      560 2023-04-20 23:24:13.000000 roblox-asset-publish-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 23:24:32.945654 roblox-asset-publish-0.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 23:24:32.905837 roblox-asset-publish-0.2.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 23:24:32.939670 roblox-asset-publish-0.2.9/src/roblox_asset_publish.egg-info/
+-rw-rw-rw-   0        0        0      454 2023-04-20 23:24:32.000000 roblox-asset-publish-0.2.9/src/roblox_asset_publish.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-20 23:24:32.000000 roblox-asset-publish-0.2.9/src/roblox_asset_publish.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 23:24:32.000000 roblox-asset-publish-0.2.9/src/roblox_asset_publish.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-20 23:24:32.000000 roblox-asset-publish-0.2.9/src/roblox_asset_publish.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 23:24:32.000000 roblox-asset-publish-0.2.9/src/roblox_asset_publish.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 23:24:32.942663 roblox-asset-publish-0.2.9/src/ropublisher/
+-rw-rw-rw-   0        0        0    11036 2023-04-20 23:23:54.000000 roblox-asset-publish-0.2.9/src/ropublisher/__init__.py
```

### Comparing `roblox-asset-publish-0.2.8/LICENSE` & `roblox-asset-publish-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-asset-publish-0.2.8/pyproject.toml` & `roblox-asset-publish-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "roblox-asset-publish"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"requests==2.28.2", 
 	"mutagen==1.46.0", 
 ]
```

### Comparing `roblox-asset-publish-0.2.8/src/ropublisher/__init__.py` & `roblox-asset-publish-0.2.9/src/ropublisher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,16 +218,18 @@
 			},
 			data=data,
 		)
 
 		# print(response)
 		# print(response.text)
 		content_data = json.loads(response.text)
-		return content_data["path"].replace("operations/", "")
-
+		if "path" in content_data:
+			return content_data["path"].replace("operations/", "")
+		else
+			raise ValueError(f"bad response {content_data}")
 	def _token_authorized_request(self, method: HttpMethod, url: str, **kwargs) -> Response | None:
 
 		response = self.session.request(method, url, **kwargs)
 
 		method = method.lower()
 		if method in ["post", "put", "patch", "delete"]:
 			if "x-csrf-token" in response.headers:
```

