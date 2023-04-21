# Comparing `tmp/multicall-0.7.1.tar.gz` & `tmp/multicall-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicall-0.7.1.tar", max compression
+gzip compressed data, was "multicall-0.7.2.tar", max compression
```

## Comparing `multicall-0.7.1.tar` & `multicall-0.7.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      116 2022-09-24 21:37:51.678438 multicall-0.7.1/multicall/__init__.py
--rw-r--r--   0        0        0     4673 2022-09-24 21:37:51.678438 multicall-0.7.1/multicall/call.py
--rw-r--r--   0        0        0    20653 2023-02-03 17:57:14.581595 multicall-0.7.1/multicall/constants.py
--rw-r--r--   0        0        0       54 2022-09-24 21:37:51.678438 multicall-0.7.1/multicall/exceptions.py
--rw-r--r--   0        0        0      267 2022-09-24 21:37:51.678438 multicall-0.7.1/multicall/loggers.py
--rw-r--r--   0        0        0     8126 2023-01-18 04:20:15.348143 multicall-0.7.1/multicall/multicall.py
--rw-r--r--   0        0        0     2349 2022-10-19 20:16:40.545472 multicall-0.7.1/multicall/signature.py
--rw-r--r--   0        0        0     3116 2023-02-03 17:57:14.581595 multicall-0.7.1/multicall/utils.py
--rw-r--r--   0        0        0      624 2023-02-03 18:07:53.082769 multicall-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 multicall-0.7.1/setup.py
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 multicall-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      116 2022-09-24 21:37:51.678438 multicall-0.7.2/multicall/__init__.py
+-rw-r--r--   0        0        0     4884 2023-04-21 00:47:13.189773 multicall-0.7.2/multicall/call.py
+-rw-r--r--   0        0        0    21026 2023-04-21 00:45:46.699989 multicall-0.7.2/multicall/constants.py
+-rw-r--r--   0        0        0       54 2022-09-24 21:37:51.678438 multicall-0.7.2/multicall/exceptions.py
+-rw-r--r--   0        0        0      267 2022-09-24 21:37:51.678438 multicall-0.7.2/multicall/loggers.py
+-rw-r--r--   0        0        0     8331 2023-04-21 00:44:24.830234 multicall-0.7.2/multicall/multicall.py
+-rw-r--r--   0        0        0     2490 2023-04-20 23:29:57.988779 multicall-0.7.2/multicall/signature.py
+-rw-r--r--   0        0        0     3116 2023-02-03 17:57:14.581595 multicall-0.7.2/multicall/utils.py
+-rw-r--r--   0        0        0      624 2023-04-21 01:19:37.740641 multicall-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 multicall-0.7.2/setup.py
+-rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 multicall-0.7.2/PKG-INFO
```

### Comparing `multicall-0.7.1/multicall/call.py` & `multicall-0.7.2/multicall/call.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import eth_retry
 from eth_typing import Address, ChecksumAddress, HexAddress
 from eth_typing.abi import Decodable
 from eth_utils import to_checksum_address
 from web3 import Web3
 
 from multicall import Signature
-from multicall.constants import Network, w3
+from multicall.constants import Network, w3, ASYNC_SEMAPHORE
 from multicall.exceptions import StateOverrideNotSupported
 from multicall.loggers import setup_logger
 from multicall.utils import (chain_id, get_async_w3, run_in_subprocess,
                              state_override_supported)
 
 logger = setup_logger(__name__)
 
@@ -96,33 +96,37 @@
             self.state_override_code,
         )
         return Call.decode_output(
             _w3.eth.call(*args),
             self.signature,
             self.returns,
         )
+    
+    async def __await__(self) -> Any:
+        return await self.coroutine()
 
     @eth_retry.auto_retry
     async def coroutine(self, args: Optional[Any] = None, _w3: Optional[Web3] = None) -> Any:
         _w3 = self.w3 or _w3 or w3
 
         if self.state_override_code and not state_override_supported(_w3):
             raise StateOverrideNotSupported(f'State override is not supported on {Network(chain_id(_w3)).__repr__()[1:-1]}.')
         
-        args = await run_in_subprocess(
-            prep_args,
-            self.target,
-            self.signature,
-            args or self.args,
-            self.block_id,
-            self.gas_limit,
-            self.state_override_code,
-        )
-
-        output = await get_async_w3(_w3).eth.call(*args)
+        async with ASYNC_SEMAPHORE:
+            output = await get_async_w3(_w3).eth.call(
+                *await run_in_subprocess(
+                    prep_args,
+                    self.target,
+                    self.signature,
+                    args or self.args,
+                    self.block_id,
+                    self.gas_limit,
+                    self.state_override_code,
+                )
+            )
 
         return await run_in_subprocess(Call.decode_output, output, self.signature, self.returns)
     
 def prep_args(
     target: str, 
     signature: Signature, 
     args: Optional[Any],
```

### Comparing `multicall-0.7.1/multicall/constants.py` & `multicall-0.7.2/multicall/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import os
 from enum import IntEnum
 from typing import Dict
 
 from aiohttp import ClientTimeout
 
 # If brownie is installed and connected, we will use brownie's Web3
@@ -52,14 +53,15 @@
     Metis = 1088
     Moonbeam = 1284
     Moonriver = 1285
     MoonbaseAlphaTestnet = 1287
     Milkomeda = 2001
     Kava = 2222
     FantomTestnet = 4002
+    Canto = 7700
     Klaytn = 8217
     EvmosTestnet = 9000
     Evmos = 9001
     Arbitrum = 42161
     Celo = 42220
     Oasis = 42262
     AvalancheFuji = 43113
@@ -142,14 +144,15 @@
     Network.Astar: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Metis: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Moonbeam: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Moonriver: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.MoonbaseAlphaTestnet: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Milkomeda: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.FantomTestnet: '0xcA11bde05977b3631167028862bE2a173976CA11',
+    Network.Canto: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Klaytn: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.EvmosTestnet: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Evmos: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Arbitrum: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Celo: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.Oasis: '0xcA11bde05977b3631167028862bE2a173976CA11',
     Network.AvalancheFuji: '0xcA11bde05977b3631167028862bE2a173976CA11',
@@ -170,7 +173,11 @@
 
 # Parallelism
 user_choice = max(1, int(os.environ.get("MULTICALL_PROCESSES", 1)))
 parallelism_capacity = max(1, os.cpu_count() - 1)
 NUM_PROCESSES = min(user_choice, parallelism_capacity)
 
 NO_STATE_OVERRIDE = [ Network.Gnosis, Network.Harmony, Network.Moonbeam, Network.Moonriver, Network.Kovan, Network.Fuse ]
+
+# NOTE: If we run too many async calls at once, we'll have memory issues.
+#       Feel free to increase this with the "MULTICALL_CALL_SEMAPHORE" env var if you know what you're doing.
+ASYNC_SEMAPHORE = asyncio.Semaphore(int(os.environ.get("MULTICALL_CALL_SEMAPHORE", 1000)))
```

### Comparing `multicall-0.7.1/multicall/multicall.py` & `multicall-0.7.2/multicall/multicall.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import aiohttp
 import requests
 from web3 import Web3
 
 from multicall import Call
-from multicall.constants import (GAS_LIMIT, MULTICALL2_ADDRESSES, MULTICALL2_BYTECODE,
-                                 MULTICALL3_BYTECODE, MULTICALL3_ADDRESSES, w3)
+from multicall.constants import (ASYNC_SEMAPHORE, GAS_LIMIT,
+                                 MULTICALL2_ADDRESSES, MULTICALL3_ADDRESSES,
+                                 MULTICALL3_BYTECODE, w3)
 from multicall.loggers import setup_logger
 from multicall.utils import (await_awaitable, chain_id, gather,
                              run_in_subprocess, state_override_supported)
 
 logger = setup_logger(__name__)
 
 CallResponse = Tuple[Union[None,bool],bytes]
@@ -50,17 +51,20 @@
         else:
             multicall_map = MULTICALL3_ADDRESSES if self.chainid in MULTICALL3_ADDRESSES else MULTICALL2_ADDRESSES
             self.multicall_sig = 'tryBlockAndAggregate(bool,(address,bytes)[])(uint256,uint256,(bool,bytes)[])'
         self.multicall_address = multicall_map[self.chainid]
 
     def __call__(self) -> Dict[str,Any]:
         start = time()
-        response = await_awaitable(self.coroutine())
+        response = await_awaitable(self)
         logger.debug(f"Multicall took {time() - start}s")
         return response
+     
+    async def __await__(self) -> Dict[str,Any]:
+        return await self.coroutine()
 
     async def coroutine(self) -> Dict[str,Any]:
         batches = await gather([
             self.fetch_outputs(batch, id=str(i)) 
             for i,batch in enumerate(batcher.batch_calls(self.calls,batcher.step))
         ])
         outputs = await run_in_subprocess(unpack_batch_results, batches)
@@ -73,29 +77,30 @@
 
     async def fetch_outputs(self, calls: List[Call], ConnErr_retries: int = 0, id: str = '') -> List[CallResponse]:
         logger.debug(f"coroutine {id} started")
 
         if calls is None:
             calls = self.calls
         
-        try:
-            args = await run_in_subprocess(get_args, calls, self.require_success)
-            if self.require_success is True:
-                _, outputs = await self.aggregate.coroutine(args)
-                outputs = await run_in_subprocess(unpack_aggregate_outputs, outputs)
-            else:
-                _, _, outputs = await self.aggregate.coroutine(args)
-            outputs = await gather([
-                run_in_subprocess(Call.decode_output, output, call.signature, call.returns, success)
-                for call, (success, output) in zip(calls, outputs)
-            ])
-            logger.debug(f"coroutine {id} finished")
-            return outputs
-        except Exception as e:
-            _raise_or_proceed(e, len(calls), ConnErr_retries=ConnErr_retries)
+        async with ASYNC_SEMAPHORE:
+            try:
+                args = await run_in_subprocess(get_args, calls, self.require_success)
+                if self.require_success is True:
+                    _, outputs = await self.aggregate.coroutine(args)
+                    outputs = await run_in_subprocess(unpack_aggregate_outputs, outputs)
+                else:
+                    _, _, outputs = await self.aggregate.coroutine(args)
+                outputs = await gather([
+                    run_in_subprocess(Call.decode_output, output, call.signature, call.returns, success)
+                    for call, (success, output) in zip(calls, outputs)
+                ])
+                logger.debug(f"coroutine {id} finished")
+                return outputs
+            except Exception as e:
+                _raise_or_proceed(e, len(calls), ConnErr_retries=ConnErr_retries)
         
         # Failed, we need to rebatch the calls and try again.
         batch_results = await gather([
             self.fetch_outputs(chunk, ConnErr_retries+1, f"{id}_{i}")
             for i, chunk in enumerate(await batcher.rebatch(calls))
         ])
```

### Comparing `multicall-0.7.1/multicall/signature.py` & `multicall-0.7.2/multicall/signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+from functools import lru_cache
 from typing import Any, List, Optional, Tuple
 
 # For eth_abi versions < 2.2.0, `decode` and `encode` have not yet been added.
 # As we require web3 ^5.27, we require eth_abi compatability with eth_abi v2.0.0b6 and greater.
 try:
     from eth_abi import decode, encode
 except ImportError: 
     from eth_abi import encode_abi as encode, decode_abi as decode
 
 from eth_typing.abi import Decodable, TypeStr
 from eth_utils import function_signature_to_4byte_selector
 
 
+get_4byte_selector = lru_cache(maxsize=None)(function_signature_to_4byte_selector)
+
 def parse_signature(signature: str) -> Tuple[str, List[TypeStr], List[TypeStr]]:
     """
     Breaks 'func(address)(uint256)' into ['func', ['address'], ['uint256']]
     """
     parts: List[str] = []
     stack: List[str] = []
     start: int = 0
@@ -54,14 +57,17 @@
     return parts
 
 
 class Signature:
     def __init__(self, signature: str) -> None:
         self.signature = signature
         self.function, self.input_types, self.output_types = parse_signature(signature)
-        self.fourbyte = function_signature_to_4byte_selector(self.function)
+    
+    @property
+    def fourbyte(self) -> bytes:
+        return get_4byte_selector(self.function)
 
     def encode_data(self, args: Optional[Any] = None) -> bytes:
         return self.fourbyte + encode(self.input_types, args) if args else self.fourbyte
 
     def decode_data(self, output: Decodable) -> Any:
         return decode(self.output_types, output)
```

### Comparing `multicall-0.7.1/multicall/utils.py` & `multicall-0.7.2/multicall/utils.py`

 * *Files identical despite different names*

### Comparing `multicall-0.7.1/pyproject.toml` & `multicall-0.7.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multicall"
-version = "0.7.1"
+version = "0.7.2"
 description = "aggregate results from multiple ethereum contract calls"
 authors = ["banteg"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 # These web3.py versions have a busted async provider and cannot be used in any multithreaded applications
 web3 = "^5.27,!=5.29.*,!=5.30.*,!=5.31.0,!=5.31.1,!=5.31.2"
```

### Comparing `multicall-0.7.1/setup.py` & `multicall-0.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 install_requires = \
 ['eth_retry>=0.1.8,<0.2.0',
  'web3>=5.27,<6.0,!=5.29.*,!=5.30.*,!=5.31.0,!=5.31.1,!=5.31.2']
 
 setup_kwargs = {
     'name': 'multicall',
-    'version': '0.7.1',
+    'version': '0.7.2',
     'description': 'aggregate results from multiple ethereum contract calls',
     'long_description': 'None',
     'author': 'banteg',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

