# Comparing `tmp/ethereal-0.1.4.tar.gz` & `tmp/ethereal-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethereal-0.1.4.tar", max compression
+gzip compressed data, was "ethereal-0.1.5.tar", max compression
```

## Comparing `ethereal-0.1.4.tar` & `ethereal-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-04-02 19:03:02.167776 ethereal-0.1.4/LICENSE
--rw-r--r--   0        0        0     1541 2023-04-17 18:19:20.949560 ethereal-0.1.4/README.md
--rw-r--r--   0        0        0     1308 2023-04-16 07:11:11.928618 ethereal-0.1.4/ethereal/__init__.py
--rw-r--r--   0        0        0     1402 2023-04-14 14:08:02.175740 ethereal-0.1.4/ethereal/app.py
--rw-r--r--   0        0        0      288 2023-04-14 18:53:08.549415 ethereal-0.1.4/ethereal/base.py
--rw-r--r--   0        0        0     6978 2023-04-16 06:36:31.316428 ethereal-0.1.4/ethereal/cache.py
--rw-r--r--   0        0        0      782 2023-04-14 18:44:54.261252 ethereal-0.1.4/ethereal/config.yml
--rw-r--r--   0        0        0      968 2023-04-18 06:13:03.668120 ethereal-0.1.4/ethereal/containers.py
--rw-r--r--   0        0        0     8806 2023-04-17 07:14:39.659777 ethereal-0.1.4/ethereal/contracts.py
--rw-r--r--   0        0        0     4652 2023-04-14 18:47:51.186401 ethereal-0.1.4/ethereal/etherscan.py
--rw-r--r--   0        0        0     3175 2023-04-14 14:31:35.858070 ethereal-0.1.4/ethereal/facade.py
--rw-r--r--   0        0        0     1439 2023-04-14 18:59:17.941096 ethereal-0.1.4/ethereal/networks.py
--rw-r--r--   0        0        0      586 2023-04-18 06:13:30.793162 ethereal-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2318 2023-04-18 06:13:33.442368 ethereal-0.1.4/setup.py
--rw-r--r--   0        0        0     2136 2023-04-18 06:13:33.442552 ethereal-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-02 19:03:02.167776 ethereal-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1758 2023-04-19 16:04:17.948471 ethereal-0.1.5/README.md
+-rw-r--r--   0        0        0       37 2023-04-08 22:51:50.151953 ethereal-0.1.5/ethereal/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      194 2023-04-08 22:51:50.152033 ethereal-0.1.5/ethereal/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      295 2023-04-08 22:51:50.151889 ethereal-0.1.5/ethereal/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2023-04-08 22:52:21.459375 ethereal-0.1.5/ethereal/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-04-08 22:52:21.459512 ethereal-0.1.5/ethereal/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     1308 2023-04-16 07:11:11.928618 ethereal-0.1.5/ethereal/__init__.py
+-rw-r--r--   0        0        0      866 2023-04-21 08:44:32.823284 ethereal-0.1.5/ethereal/accounts.py
+-rw-r--r--   0        0        0     1402 2023-04-14 14:08:02.175740 ethereal-0.1.5/ethereal/app.py
+-rw-r--r--   0        0        0      288 2023-04-14 18:53:08.549415 ethereal-0.1.5/ethereal/base.py
+-rw-r--r--   0        0        0     6978 2023-04-16 06:36:31.316428 ethereal-0.1.5/ethereal/cache.py
+-rw-r--r--   0        0        0      782 2023-04-14 18:44:54.261252 ethereal-0.1.5/ethereal/config.yml
+-rw-r--r--   0        0        0     1061 2023-04-20 20:19:54.363594 ethereal-0.1.5/ethereal/containers.py
+-rw-r--r--   0        0        0     8806 2023-04-17 07:14:39.659777 ethereal-0.1.5/ethereal/contracts.py
+-rw-r--r--   0        0        0     4652 2023-04-14 18:47:51.186401 ethereal-0.1.5/ethereal/etherscan.py
+-rw-r--r--   0        0        0     3737 2023-04-21 08:44:32.827546 ethereal-0.1.5/ethereal/facade.py
+-rw-r--r--   0        0        0     1439 2023-04-14 18:59:17.941096 ethereal-0.1.5/ethereal/networks.py
+-rw-r--r--   0        0        0      606 2023-04-21 08:44:56.705997 ethereal-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2639 2023-04-21 08:45:06.847479 ethereal-0.1.5/setup.py
+-rw-r--r--   0        0        0     2394 2023-04-21 08:45:06.847682 ethereal-0.1.5/PKG-INFO
```

### Comparing `ethereal-0.1.4/LICENSE` & `ethereal-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.4/README.md` & `ethereal-0.1.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 accessible under the `e` property.
 
 For example, you can call `w3.e.get_abi("0x...")` or
 `w3.e.list_events("0x...", "Mint", "2023-01-01", "2023-02-14")`.
 
 For more available methods, please refer to the [EtherealFacade](https://ethereal.readthedocs.io/en/latest/?badge=latest#ethereal.facade.EtherealFacade) class.
 
+### Demo
+
+![Ethereal demo](./docs/images/demo.gif)
+
 ### Example
 
 ```python
 from web3.auto import w3
 from ethereal import Ethereal
 from ethereal import load_provider_from_uri
 
@@ -38,7 +42,20 @@
 ```
 
 ### Install
 
 ```
 pip install ethereal
 ```
+
+### Supported networks
+
+- Ethereum
+- Polygon
+- Avalanche
+- Fantom
+- Arbitrum
+- Optimism
+
+### Contributing
+
+Feel free to create feature requests or pull requests :D
```

### Comparing `ethereal-0.1.4/ethereal/__init__.py` & `ethereal-0.1.5/ethereal/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.4/ethereal/app.py` & `ethereal-0.1.5/ethereal/app.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.4/ethereal/cache.py` & `ethereal-0.1.5/ethereal/cache.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.4/ethereal/config.yml` & `ethereal-0.1.5/ethereal/config.yml`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.4/ethereal/containers.py` & `ethereal-0.1.5/ethereal/containers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import logging.config
 from dependency_injector import containers, providers
+from .accounts import Accounts
 from .etherscan import Etherscan
 from .facade import EtherealFacade
 from .cache import MemoryCache, DbCache, Cache
 
 current_folder = os.path.realpath(os.path.dirname(__file__))
 
 
@@ -17,10 +18,11 @@
         yaml_files=[os.path.abspath(f"{current_folder}/config.yml")]
     )
     logging = providers.Resource(logging.config.dictConfig, config=config.logging)
     memory_cache = providers.Factory(MemoryCache)
     db_cache = providers.Singleton(DbCache, config=config.cache)
     cache = providers.Factory(Cache, memory_cache=memory_cache, db_cache=db_cache)
     etherscan = providers.Factory(Etherscan, config=config.etherscan, cache=cache)
+    accounts = providers.Factory(Accounts)
     ethereal_facade = providers.Factory(
-        EtherealFacade, etherscan=etherscan, cache=cache
+        EtherealFacade, etherscan=etherscan, accounts=accounts, cache=cache
     )
```

### Comparing `ethereal-0.1.4/ethereal/contracts.py` & `ethereal-0.1.5/ethereal/contracts.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.4/ethereal/etherscan.py` & `ethereal-0.1.5/ethereal/etherscan.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.4/ethereal/facade.py` & `ethereal-0.1.5/ethereal/facade.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 from typing import Any, Dict, List
 from datetime import datetime
 from web3 import Web3
 from web3.contract import Contract
+from .accounts import Accounts, Account
 from .etherscan import Etherscan
 from .contracts import Contracts
 from .cache import Cache
 
 
 class EtherealFacade:
     """
     The main class containing Ethereal's functionality.
     """
 
     _etherscan: Etherscan
     _web3: Web3
+    _accounts: Accounts
     _cache: Cache
 
-    def __init__(self, etherscan: Etherscan, web3: Web3, cache: Cache, *args, **kwargs):
+    def __init__(
+        self,
+        etherscan: Etherscan,
+        web3: Web3,
+        accounts: Accounts,
+        cache: Cache,
+        *args,
+        **kwargs
+    ):
         super().__init__(*args, **kwargs)
         self._etherscan = etherscan
         self._web3 = web3
+        self._accounts = accounts
         self._cache = cache
 
     def get_block_by_timestamp(self, timestamp: int = True) -> int:
         """
         Get the block number for a given timestamp.
 
         :param timestamp: The timestamp to look up.
@@ -55,14 +66,25 @@
 
         :param address: The address to look up.
         :param resolve_proxy: Whether to resolve proxies. If true, the ABI for the
                               implementation contract will be used.
         """
         return self._contracts().get_contract(address, resolve_proxy)
 
+    def derive_account(self, seed_phrase: str, index: int) -> Account:
+        """
+        Derive public and a private key from a seed phrase (Metamask or other bip 44)
+
+        :param seed_phrase: The seed phrase to use
+        :param index: The index to use
+
+        :return: The pubic and private key
+        """
+        return self._accounts.derive_account(seed_phrase, index)
+
     def get_events(
         self,
         address: str,
         event: str,
         from_time: int | str | datetime,
         to_time: int | str | datetime,
         argument_filters: Dict[str, Any] | None = None,
```

### Comparing `ethereal-0.1.4/ethereal/networks.py` & `ethereal-0.1.5/ethereal/networks.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.4/pyproject.toml` & `ethereal-0.1.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "ethereal"
-version = "0.1.4"
+version = "0.1.5"
 description = "Ergonomic python tooling for web3"
 authors = ["Alex Euler <0xalexeuler@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 web3 = "^6.1.0"
 dependency-injector = "^4.41.0"
 click = "^8.1.3"
 PyYAML = "^6.0"
 python-dateutil = "^2.8.2"
+hdwallet = "^2.2.1"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 pytest = "^7.3.0"
 jupyterlab = "^3.6.3"
 pylint = "^2.17.2"
 Sphinx = "^6.1.3"
```

### Comparing `ethereal-0.1.4/setup.py` & `ethereal-0.1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['ethereal']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'ethereal': ['.pytest_cache/*', '.pytest_cache/v/cache/*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'click>=8.1.3,<9.0.0',
  'dependency-injector>=4.41.0,<5.0.0',
+ 'hdwallet>=2.2.1,<3.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'web3>=6.1.0,<7.0.0']
 
 setup_kwargs = {
     'name': 'ethereal',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Ergonomic python tooling for web3',
-    'long_description': '![Ethereal logo](./docs/images/ethereal_cat.png)\n\n## Ethereal\n\n[![docs](https://readthedocs.org/projects/ethereal/badge/?version=latest)](https://ethereal.readthedocs.io/en/latest/?badge=latest)\n\nEthereal is a lightweight wrapper around the [Web3](https://web3py.readthedocs.io/en/stable/web3.main.html#web3.Web3) class that simplifies\nworking with Ethereum smart contracts.\n\nTo use it, simply create a regular [Web3](https://web3py.readthedocs.io/en/stable/web3.main.html#web3.Web3) instance and write `w3 = Ethereal(w3)`.\nThen, you can use w3 as usual, but with additional methods\naccessible under the `e` property.\n\nFor example, you can call `w3.e.get_abi("0x...")` or\n`w3.e.list_events("0x...", "Mint", "2023-01-01", "2023-02-14")`.\n\nFor more available methods, please refer to the [EtherealFacade](https://ethereal.readthedocs.io/en/latest/?badge=latest#ethereal.facade.EtherealFacade) class.\n\n### Example\n\n```python\nfrom web3.auto import w3\nfrom ethereal import Ethereal\nfrom ethereal import load_provider_from_uri\n\n# If WEB3_PROVIDER_URI env is not set, uncomment the lines below\n# w3 = Web3(load_provider_from_uri("https://alchemy.com/..."))\n\nw3 = Ethereal(w3)\n\nADDRESS = "0xB0B195aEFA3650A6908f15CdaC7D92F8a5791B0B"\nprint(w3.e.list_events(ADDRESS))\n# Lists event signatures for the contract at ADDRESS\n\nevents = w3.e.get_events(ADDRESS, "Transfer", "2023-01-01", "2023-02-14")\n# Gets all Transfer events for the contract at ADDRESS between 2023-01-01 and 2023-02-14\nprint(events[:10])\n```\n\n### Install\n\n```\npip install ethereal\n```\n',
+    'long_description': '![Ethereal logo](./docs/images/ethereal_cat.png)\n\n## Ethereal\n\n[![docs](https://readthedocs.org/projects/ethereal/badge/?version=latest)](https://ethereal.readthedocs.io/en/latest/?badge=latest)\n\nEthereal is a lightweight wrapper around the [Web3](https://web3py.readthedocs.io/en/stable/web3.main.html#web3.Web3) class that simplifies\nworking with Ethereum smart contracts.\n\nTo use it, simply create a regular [Web3](https://web3py.readthedocs.io/en/stable/web3.main.html#web3.Web3) instance and write `w3 = Ethereal(w3)`.\nThen, you can use w3 as usual, but with additional methods\naccessible under the `e` property.\n\nFor example, you can call `w3.e.get_abi("0x...")` or\n`w3.e.list_events("0x...", "Mint", "2023-01-01", "2023-02-14")`.\n\nFor more available methods, please refer to the [EtherealFacade](https://ethereal.readthedocs.io/en/latest/?badge=latest#ethereal.facade.EtherealFacade) class.\n\n### Demo\n\n![Ethereal demo](./docs/images/demo.gif)\n\n### Example\n\n```python\nfrom web3.auto import w3\nfrom ethereal import Ethereal\nfrom ethereal import load_provider_from_uri\n\n# If WEB3_PROVIDER_URI env is not set, uncomment the lines below\n# w3 = Web3(load_provider_from_uri("https://alchemy.com/..."))\n\nw3 = Ethereal(w3)\n\nADDRESS = "0xB0B195aEFA3650A6908f15CdaC7D92F8a5791B0B"\nprint(w3.e.list_events(ADDRESS))\n# Lists event signatures for the contract at ADDRESS\n\nevents = w3.e.get_events(ADDRESS, "Transfer", "2023-01-01", "2023-02-14")\n# Gets all Transfer events for the contract at ADDRESS between 2023-01-01 and 2023-02-14\nprint(events[:10])\n```\n\n### Install\n\n```\npip install ethereal\n```\n\n### Supported networks\n\n- Ethereum\n- Polygon\n- Avalanche\n- Fantom\n- Arbitrum\n- Optimism\n\n### Contributing\n\nFeel free to create feature requests or pull requests :D\n',
     'author': 'Alex Euler',
     'author_email': '0xalexeuler@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ethereal-0.1.4/PKG-INFO` & `ethereal-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ethereal
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ergonomic python tooling for web3
 License: MIT
 Author: Alex Euler
 Author-email: 0xalexeuler@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dependency-injector (>=4.41.0,<5.0.0)
+Requires-Dist: hdwallet (>=2.2.1,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: web3 (>=6.1.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 ![Ethereal logo](./docs/images/ethereal_cat.png)
 
 ## Ethereal
@@ -30,14 +31,18 @@
 accessible under the `e` property.
 
 For example, you can call `w3.e.get_abi("0x...")` or
 `w3.e.list_events("0x...", "Mint", "2023-01-01", "2023-02-14")`.
 
 For more available methods, please refer to the [EtherealFacade](https://ethereal.readthedocs.io/en/latest/?badge=latest#ethereal.facade.EtherealFacade) class.
 
+### Demo
+
+![Ethereal demo](./docs/images/demo.gif)
+
 ### Example
 
 ```python
 from web3.auto import w3
 from ethereal import Ethereal
 from ethereal import load_provider_from_uri
 
@@ -57,7 +62,20 @@
 
 ### Install
 
 ```
 pip install ethereal
 ```
 
+### Supported networks
+
+- Ethereum
+- Polygon
+- Avalanche
+- Fantom
+- Arbitrum
+- Optimism
+
+### Contributing
+
+Feel free to create feature requests or pull requests :D
+
```

