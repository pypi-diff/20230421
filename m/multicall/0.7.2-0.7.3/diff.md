# Comparing `tmp/multicall-0.7.2.tar.gz` & `tmp/multicall-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicall-0.7.2.tar", max compression
+gzip compressed data, was "multicall-0.7.3.tar", max compression
```

## Comparing `multicall-0.7.2.tar` & `multicall-0.7.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      116 2022-09-24 21:37:51.678438 multicall-0.7.2/multicall/__init__.py
--rw-r--r--   0        0        0     4884 2023-04-21 00:47:13.189773 multicall-0.7.2/multicall/call.py
--rw-r--r--   0        0        0    21026 2023-04-21 00:45:46.699989 multicall-0.7.2/multicall/constants.py
--rw-r--r--   0        0        0       54 2022-09-24 21:37:51.678438 multicall-0.7.2/multicall/exceptions.py
--rw-r--r--   0        0        0      267 2022-09-24 21:37:51.678438 multicall-0.7.2/multicall/loggers.py
--rw-r--r--   0        0        0     8331 2023-04-21 00:44:24.830234 multicall-0.7.2/multicall/multicall.py
--rw-r--r--   0        0        0     2490 2023-04-20 23:29:57.988779 multicall-0.7.2/multicall/signature.py
--rw-r--r--   0        0        0     3116 2023-02-03 17:57:14.581595 multicall-0.7.2/multicall/utils.py
--rw-r--r--   0        0        0      624 2023-04-21 01:19:37.740641 multicall-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 multicall-0.7.2/setup.py
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 multicall-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      116 2022-09-24 21:37:51.678438 multicall-0.7.3/multicall/__init__.py
+-rw-r--r--   0        0        0     4884 2023-04-21 01:32:54.180157 multicall-0.7.3/multicall/call.py
+-rw-r--r--   0        0        0    21026 2023-04-21 01:26:37.041976 multicall-0.7.3/multicall/constants.py
+-rw-r--r--   0        0        0       54 2022-09-24 21:37:51.678438 multicall-0.7.3/multicall/exceptions.py
+-rw-r--r--   0        0        0      267 2022-09-24 21:37:51.678438 multicall-0.7.3/multicall/loggers.py
+-rw-r--r--   0        0        0     8331 2023-04-21 01:33:04.472591 multicall-0.7.3/multicall/multicall.py
+-rw-r--r--   0        0        0     2490 2023-04-21 01:26:37.041976 multicall-0.7.3/multicall/signature.py
+-rw-r--r--   0        0        0     3116 2023-02-03 17:57:14.581595 multicall-0.7.3/multicall/utils.py
+-rw-r--r--   0        0        0      624 2023-04-21 01:33:56.926764 multicall-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 multicall-0.7.3/setup.py
+-rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 multicall-0.7.3/PKG-INFO
```

### Comparing `multicall-0.7.2/multicall/call.py` & `multicall-0.7.3/multicall/call.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,16 @@
         )
         return Call.decode_output(
             _w3.eth.call(*args),
             self.signature,
             self.returns,
         )
     
-    async def __await__(self) -> Any:
-        return await self.coroutine()
+    def __await__(self) -> Any:
+        return self.coroutine().__await__()
 
     @eth_retry.auto_retry
     async def coroutine(self, args: Optional[Any] = None, _w3: Optional[Web3] = None) -> Any:
         _w3 = self.w3 or _w3 or w3
 
         if self.state_override_code and not state_override_supported(_w3):
             raise StateOverrideNotSupported(f'State override is not supported on {Network(chain_id(_w3)).__repr__()[1:-1]}.')
```

### Comparing `multicall-0.7.2/multicall/constants.py` & `multicall-0.7.3/multicall/constants.py`

 * *Files identical despite different names*

### Comparing `multicall-0.7.2/multicall/multicall.py` & `multicall-0.7.3/multicall/multicall.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 
     def __call__(self) -> Dict[str,Any]:
         start = time()
         response = await_awaitable(self)
         logger.debug(f"Multicall took {time() - start}s")
         return response
      
-    async def __await__(self) -> Dict[str,Any]:
-        return await self.coroutine()
+    def __await__(self) -> Dict[str,Any]:
+        return self.coroutine().__await__()
 
     async def coroutine(self) -> Dict[str,Any]:
         batches = await gather([
             self.fetch_outputs(batch, id=str(i)) 
             for i,batch in enumerate(batcher.batch_calls(self.calls,batcher.step))
         ])
         outputs = await run_in_subprocess(unpack_batch_results, batches)
```

### Comparing `multicall-0.7.2/multicall/signature.py` & `multicall-0.7.3/multicall/signature.py`

 * *Files identical despite different names*

### Comparing `multicall-0.7.2/multicall/utils.py` & `multicall-0.7.3/multicall/utils.py`

 * *Files identical despite different names*

### Comparing `multicall-0.7.2/pyproject.toml` & `multicall-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multicall"
-version = "0.7.2"
+version = "0.7.3"
 description = "aggregate results from multiple ethereum contract calls"
 authors = ["banteg"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 # These web3.py versions have a busted async provider and cannot be used in any multithreaded applications
 web3 = "^5.27,!=5.29.*,!=5.30.*,!=5.31.0,!=5.31.1,!=5.31.2"
```

### Comparing `multicall-0.7.2/setup.py` & `multicall-0.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 install_requires = \
 ['eth_retry>=0.1.8,<0.2.0',
  'web3>=5.27,<6.0,!=5.29.*,!=5.30.*,!=5.31.0,!=5.31.1,!=5.31.2']
 
 setup_kwargs = {
     'name': 'multicall',
-    'version': '0.7.2',
+    'version': '0.7.3',
     'description': 'aggregate results from multiple ethereum contract calls',
     'long_description': 'None',
     'author': 'banteg',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

