# Comparing `tmp/TonTools-2.0.6.tar.gz` & `tmp/TonTools-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TonTools-2.0.6.tar", last modified: Sat Apr  8 15:11:37 2023, max compression
+gzip compressed data, was "dist/TonTools-2.0.8.tar", last modified: Fri Apr 21 13:26:28 2023, max compression
```

## Comparing `TonTools-2.0.6.tar` & `TonTools-2.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-08 15:11:37.909478 TonTools-2.0.6/
--rw-r--r--   0 maxankurb   (501) staff       (20)     1071 2023-03-09 07:49:38.000000 TonTools-2.0.6/LICENSE
--rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-04-08 15:11:37.909086 TonTools-2.0.6/PKG-INFO
--rw-r--r--   0 maxankurb   (501) staff       (20)    10004 2023-04-01 17:07:53.000000 TonTools-2.0.6/README.md
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-08 15:11:37.892682 TonTools-2.0.6/TonTools/
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-08 15:11:37.903860 TonTools-2.0.6/TonTools/Contracts/
--rw-r--r--   0 maxankurb   (501) staff       (20)     4820 2023-04-01 15:06:10.000000 TonTools-2.0.6/TonTools/Contracts/Contract.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     3905 2023-04-08 15:09:01.000000 TonTools-2.0.6/TonTools/Contracts/Jetton.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     5661 2023-03-01 07:15:23.000000 TonTools-2.0.6/TonTools/Contracts/NFT.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     6091 2023-03-29 17:48:14.000000 TonTools-2.0.6/TonTools/Contracts/Wallet.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      782 2023-04-01 15:38:26.000000 TonTools-2.0.6/TonTools/Contracts/utils.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-08 15:11:37.908400 TonTools-2.0.6/TonTools/Providers/
--rw-r--r--   0 maxankurb   (501) staff       (20)    15041 2023-03-01 08:22:28.000000 TonTools-2.0.6/TonTools/Providers/LsClient.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    10543 2023-03-01 06:55:03.000000 TonTools-2.0.6/TonTools/Providers/TonApiClient.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    15489 2023-03-29 17:49:00.000000 TonTools-2.0.6/TonTools/Providers/TonCenterClient.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     2375 2023-04-08 15:09:01.000000 TonTools-2.0.6/TonTools/Providers/utils.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      288 2023-04-01 17:11:58.000000 TonTools-2.0.6/TonTools/__init__.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-08 15:11:37.896170 TonTools-2.0.6/TonTools.egg-info/
--rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-04-08 15:11:37.000000 TonTools-2.0.6/TonTools.egg-info/PKG-INFO
--rw-r--r--   0 maxankurb   (501) staff       (20)      481 2023-04-08 15:11:37.000000 TonTools-2.0.6/TonTools.egg-info/SOURCES.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)        1 2023-04-08 15:11:37.000000 TonTools-2.0.6/TonTools.egg-info/dependency_links.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)       93 2023-04-08 15:11:37.000000 TonTools-2.0.6/TonTools.egg-info/requires.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)       47 2023-04-08 15:11:37.000000 TonTools-2.0.6/TonTools.egg-info/top_level.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)       38 2023-04-08 15:11:37.909590 TonTools-2.0.6/setup.cfg
--rw-r--r--   0 maxankurb   (501) staff       (20)      489 2023-04-08 15:09:54.000000 TonTools-2.0.6/setup.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-21 13:26:28.861388 TonTools-2.0.8/
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1071 2023-03-09 07:49:38.000000 TonTools-2.0.8/LICENSE
+-rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-04-21 13:26:28.860121 TonTools-2.0.8/PKG-INFO
+-rw-r--r--   0 maxankurb   (501) staff       (20)    10004 2023-04-01 17:07:53.000000 TonTools-2.0.8/README.md
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-21 13:26:28.834508 TonTools-2.0.8/TonTools/
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-21 13:26:28.849301 TonTools-2.0.8/TonTools/Contracts/
+-rw-r--r--   0 maxankurb   (501) staff       (20)     4820 2023-04-01 15:06:10.000000 TonTools-2.0.8/TonTools/Contracts/Contract.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     3905 2023-04-08 15:09:01.000000 TonTools-2.0.8/TonTools/Contracts/Jetton.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5661 2023-03-01 07:15:23.000000 TonTools-2.0.8/TonTools/Contracts/NFT.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     6091 2023-03-29 17:48:14.000000 TonTools-2.0.8/TonTools/Contracts/Wallet.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      782 2023-04-01 15:38:26.000000 TonTools-2.0.8/TonTools/Contracts/utils.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-21 13:26:28.857698 TonTools-2.0.8/TonTools/Providers/
+-rw-r--r--   0 maxankurb   (501) staff       (20)    15041 2023-03-01 08:22:28.000000 TonTools-2.0.8/TonTools/Providers/LsClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    10553 2023-04-21 13:25:55.000000 TonTools-2.0.8/TonTools/Providers/TonApiClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    15489 2023-03-29 17:49:00.000000 TonTools-2.0.8/TonTools/Providers/TonCenterClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     2375 2023-04-08 15:09:01.000000 TonTools-2.0.8/TonTools/Providers/utils.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      288 2023-04-01 17:11:58.000000 TonTools-2.0.8/TonTools/__init__.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-04-21 13:26:28.839300 TonTools-2.0.8/TonTools.egg-info/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-04-21 13:26:28.000000 TonTools-2.0.8/TonTools.egg-info/PKG-INFO
+-rw-r--r--   0 maxankurb   (501) staff       (20)      481 2023-04-21 13:26:28.000000 TonTools-2.0.8/TonTools.egg-info/SOURCES.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)        1 2023-04-21 13:26:28.000000 TonTools-2.0.8/TonTools.egg-info/dependency_links.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)       93 2023-04-21 13:26:28.000000 TonTools-2.0.8/TonTools.egg-info/requires.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)       47 2023-04-21 13:26:28.000000 TonTools-2.0.8/TonTools.egg-info/top_level.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)       38 2023-04-21 13:26:28.861575 TonTools-2.0.8/setup.cfg
+-rw-r--r--   0 maxankurb   (501) staff       (20)      489 2023-04-21 13:26:24.000000 TonTools-2.0.8/setup.py
```

### Comparing `TonTools-2.0.6/LICENSE` & `TonTools-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `TonTools-2.0.6/README.md` & `TonTools-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `TonTools-2.0.6/TonTools/Contracts/Contract.py` & `TonTools-2.0.8/TonTools/Contracts/Contract.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.0.6/TonTools/Contracts/Jetton.py` & `TonTools-2.0.8/TonTools/Contracts/Jetton.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.0.6/TonTools/Contracts/NFT.py` & `TonTools-2.0.8/TonTools/Contracts/NFT.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.0.6/TonTools/Contracts/Wallet.py` & `TonTools-2.0.8/TonTools/Contracts/Wallet.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.0.6/TonTools/Contracts/utils.py` & `TonTools-2.0.8/TonTools/Contracts/utils.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.0.6/TonTools/Providers/LsClient.py` & `TonTools-2.0.8/TonTools/Providers/LsClient.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.0.6/TonTools/Providers/TonApiClient.py` & `TonTools-2.0.8/TonTools/Providers/TonApiClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             return Wallet(self, self._process_address(item['owner']['address']))
 
     async def get_nft_items(self, nft_addresses: list):
         result = []
         async with aiohttp.ClientSession() as session:
             url = self.base_url + 'nft/getItems'
             params = {
-                'addresses': nft_addresses
+                'addresses': ','.join(nft_addresses)
             }
             response = await session.get(url=url, params=params, headers=self.headers)
             response = await process_response(response)
             for item in response['nft_items']:
                 temp = {
                     'address': self._process_address(item['address']),
                     'collection': {
```

### Comparing `TonTools-2.0.6/TonTools/Providers/TonCenterClient.py` & `TonTools-2.0.8/TonTools/Providers/TonCenterClient.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.0.6/TonTools/Providers/utils.py` & `TonTools-2.0.8/TonTools/Providers/utils.py`

 * *Files identical despite different names*

