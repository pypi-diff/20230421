# Comparing `tmp/poseidon-python-1.1.4.tar.gz` & `tmp/poseidon-python-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poseidon-python-1.1.4.tar", last modified: Wed Mar 29 13:08:06 2023, max compression
+gzip compressed data, was "poseidon-python-1.1.5.tar", last modified: Fri Apr 21 02:57:26 2023, max compression
```

## Comparing `poseidon-python-1.1.4.tar` & `poseidon-python-1.1.5.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:08:06.194533 poseidon-python-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-29 13:07:49.000000 poseidon-python-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41187 2023-03-29 13:08:06.194533 poseidon-python-1.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:08:06.194533 poseidon-python-1.1.4/Poseidon/
--rw-r--r--   0 runner    (1001) docker     (123)    59751 2023-03-29 13:07:49.000000 poseidon-python-1.1.4/Poseidon/Blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)    30980 2023-03-29 13:07:49.000000 poseidon-python-1.1.4/Poseidon/Cryptography.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-03-29 13:07:49.000000 poseidon-python-1.1.4/Poseidon/PoW.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-29 13:07:49.000000 poseidon-python-1.1.4/Poseidon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40667 2023-03-29 13:07:49.000000 poseidon-python-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:08:06.194533 poseidon-python-1.1.4/poseidon_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41187 2023-03-29 13:08:06.000000 poseidon-python-1.1.4/poseidon_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-29 13:08:06.000000 poseidon-python-1.1.4/poseidon_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 13:08:06.000000 poseidon-python-1.1.4/poseidon_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 13:08:06.000000 poseidon-python-1.1.4/poseidon_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-29 13:08:06.000000 poseidon-python-1.1.4/poseidon_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-29 13:08:06.000000 poseidon-python-1.1.4/poseidon_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 13:08:06.194533 poseidon-python-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-29 13:07:49.000000 poseidon-python-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:57:26.806919 poseidon-python-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 02:57:11.000000 poseidon-python-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42109 2023-04-21 02:57:26.806919 poseidon-python-1.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:57:26.806919 poseidon-python-1.1.5/Poseidon/
+-rw-r--r--   0 runner    (1001) docker     (123)    64777 2023-04-21 02:57:11.000000 poseidon-python-1.1.5/Poseidon/Blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30980 2023-04-21 02:57:11.000000 poseidon-python-1.1.5/Poseidon/Cryptography.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-04-21 02:57:11.000000 poseidon-python-1.1.5/Poseidon/PoW.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-21 02:57:11.000000 poseidon-python-1.1.5/Poseidon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41585 2023-04-21 02:57:11.000000 poseidon-python-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:57:26.806919 poseidon-python-1.1.5/poseidon_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42109 2023-04-21 02:57:26.000000 poseidon-python-1.1.5/poseidon_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-21 02:57:26.000000 poseidon-python-1.1.5/poseidon_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 02:57:26.000000 poseidon-python-1.1.5/poseidon_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 02:57:26.000000 poseidon-python-1.1.5/poseidon_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-21 02:57:26.000000 poseidon-python-1.1.5/poseidon_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 02:57:26.000000 poseidon-python-1.1.5/poseidon_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 02:57:26.806919 poseidon-python-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-21 02:57:11.000000 poseidon-python-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:57:26.806919 poseidon-python-1.1.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-21 02:57:11.000000 poseidon-python-1.1.5/test/test.py
```

### Comparing `poseidon-python-1.1.4/LICENSE` & `poseidon-python-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `poseidon-python-1.1.4/PKG-INFO` & `poseidon-python-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: poseidon-python
-Version: 1.1.4
-Summary: 海神波塞冬工具对常用的链上交互操作进行了封装，使得开发者能够便捷地与任何以太坊同构链交互，主要用于在CTF比赛中攻克Blockchain方向的题目。
+Version: 1.1.5
+Summary: 海神波塞冬工具对常用的链上交互操作进行了封装，使得开发者能够便捷地与任何以太坊同构链交互，主要用于在 CTF 比赛中攻克 Blockchain 方向的题目。
 Home-page: https://github.com/B1ue1nWh1te/Poseidon
 Author: B1ue1nWh1te
 Author-email: b1ue1nwh1te@skiff.com
 License: GPL-3.0
 Keywords: POSEIDON,BLOCKCHAIN,EVM,CRYPTO,CTF
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
 # Poseidon
 
-![data](https://socialify.git.ci/B1ue1nWh1te/Poseidon/image?font=Rokkitt&forks=1&issues=1&language=1&logo=https%3A%2F%2Fimg.seaeye.cn%2Fimg%2Fseaeye%2Flogo.png&owner=1&pattern=Circuit%20Board&stargazers=1&theme=Light)
+![data](https://socialify.git.ci/B1ue1nWh1te/Poseidon/image?font=Rokkitt&forks=1&issues=1&language=1&logo=https%3A%2F%2Fimg.seaeye.cn%2Fimg%2Fseaverse%2Flogo.png&owner=1&pattern=Circuit%20Board&stargazers=1&theme=Light)
 
 **海神波塞冬 Poseidon** 工具对常用的链上交互操作进行了封装，使得开发者能够便捷地
 
 与任何以太坊同构链交互，主要用于在 CTF 比赛中攻克 Blockchain 方向的题目。
 
 [![Lisence](https://img.shields.io/github/license/B1ue1nWh1te/Poseidon)](https://github.com/B1ue1nWh1te/Poseidon/blob/main/LICENSE)
-[![Python Version](https://img.shields.io/badge/python-3.8+-blue)](https://www.python.org/)
+[![Python](https://img.shields.io/badge/python-3.9+-blue)](https://www.python.org/)
 [![Release](https://img.shields.io/github/v/release/B1ue1nWh1te/Poseidon?include_prereleases)](https://github.com/B1ue1nWh1te/Poseidon/releases/)
 [![Visitors](https://visitor-badge.glitch.me/badge?page_id=B1ue1nWh1te-Poseidon&left_color=gray&right_color=orange)](https://github.com/B1ue1nWh1te/Poseidon)
-![Downloads](https://img.shields.io/pypi/dm/poseidon-python)
+![Downloads](https://img.shields.io/pypi/dd/poseidon-python)
 
 </div>
 
 # 注意事项
 
 1. **本工具原则上仅可用于 CTF 比赛解题或测试链开发。但开源工具无法约束使用场景，若执意要在具有经济价值的公链中使用，所产生的影响将由你自行承担。**
 
 2. 在使用 `Blockchain` 模块时，你始终应该使用全新生成的账户，而不是导入常用的具有实际价值的账户，以确保你的账户安全。
 
-3. `Blockchain` 模块的所有功能在 `Goerli` 测试网络中均正常通过检验。
+3. `Blockchain` 模块的所有功能在 `Goerli, Sepolia` 测试网络中均正常通过检验。
 
 4. 如果你在使用过程中遇到了其他问题，或者有任何好的想法和建议，欢迎提[issue](https://github.com/B1ue1nWh1te/Poseidon/issues)进行反馈。
 
 # 安装
 
 ```bash
 pip install -U poseidon-python
@@ -66,52 +66,55 @@
 ### Chain 类
 
 Chain 是区块链实例，后续的所有链上交互的操作都将经由该指定节点处理。
 
 `Chain(RPCUrl: str, RequestParams: Optional[dict] = None)`：
 
 ```
-初始化。根据给定的节点 RPC 地址进行连接，可通过代理访问。当连接节点失败时会抛出异常。
+初始化。根据给定的节点 RPC 地址以 HTTP/HTTPS 方式进行连接，可通过代理访问。当连接节点失败时会抛出异常。
 
 参数：
 	RPCUrl (str): 节点 RPC 地址
 	RequestParams (可选)(Optional[dict]): 连接时使用的 request 参数，默认为 None。
 	例如当需要使用代理进行访问时，则传入 RequestParams={"proxies": {"http": "http://localhost:<ProxyPort>","https": "http://localhost:<ProxyPort>"}}
 
 成员变量：
 	ChainId (int): 链 ID
 	Node (Web3.HTTPProvider): web3.py 原生的 HTTP 交互器实例
 	Eth (Web3.HTTPProvider.eth): HTTP 交互器实例中的 eth 模块
 ```
 
 <br>
 
-`Chain.GetBasicInformation() -> dict`：
+`Chain.GetBasicInformation(ShowTimeslot: bool = True) -> dict`：
 
 ```
-获取区块链基本信息。包括链 ID 、区块高度、 GasPrice 、出块间隔、当前节点的客户端软件版本号。
+获取区块链基本信息。包括 ChainId 、BlockNumber 、GasPrice 、(Timeslot)、ClientVersion 。
+
+参数：
+	ShowTimeslot (bool): 是否获取并显示 Timeslot 。该操作比较耗时，在主动调用时默认为 True , 在 Chain 实例初始化时默认为 False 。
 
 返回值：
 	BasicInformation (dict): 区块链基本信息构成的字典。
-	{"ChainId"|"BlockNumber"|"GasPrice"|"Timeslot"|"ClientVersion"}
+	{"ChainId"|"BlockNumber"|"GasPrice"|("Timeslot")|"ClientVersion"}
 ```
 
 <br>
 
 `Chain.GetTransactionInformationByHash(TransactionHash: str) -> dict`：
 
 ```
 根据交易哈希查询该交易的详细回执信息。包括交易哈希、所在区块号、交易索引号、交易状态、交易类型、交易行为、发送者、接收者、(部署的合约地址)、(GasPrice 或 (MaxFeePerGas 和 MaxPriorityFeePerGas))、GasLimit、GasUsed、Nonce、Value、R、S、V、Logs、InputData。
 
 参数：
 	TransactionHash (str): 要查询的交易的哈希
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典。当出现异常时返回 None 。
-	{"TransactionHash"|"BlockNumber"|"TransactionIndex"|"Status"|"Type"|"Action"|"From"|"To"|("ContractAddress")|<"GasPrice"|"MaxPriorityFeePerGas")>|"GasLimit"|"GasUsed"|"Nonce"|"Value"|"R"|"S"|"V"|"RawTransaction"|"Logs"|"InputData"}
+	{"TransactionHash"|"BlockNumber"|"TransactionIndex"|"Status"|"Type"|"Action"|"From"|"To"|("ContractAddress")|<"GasPrice"|("MaxFeePerGas"&"MaxPriorityFeePerGas")>|"GasLimit"|"GasUsed"|"Nonce"|"Value"|"R"|"S"|"V"|"Logs"|"InputData"}
 ```
 
 <br>
 
 `Chain.GetTransactionInformationByBlockIdAndIndex(BlockID: Union[str,int], TransactionIndex: int) -> dict`：
 
 ```
@@ -148,59 +151,59 @@
 ```
 根据账户地址获取其网络原生代币余额。
 
 参数：
 	Address (str): 账户地址
 
 返回值：
-	Balance (int): 账户网络原生代币余额。单位为 wei ，当出现异常时返回 None 。
+	Balance (int): 账户网络原生代币余额，单位为 wei 。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Chain.GetCode(Address: str) -> str`：
 
 ```
 根据合约地址获取其已部署字节码。
 
 参数：
 	Address (str): 合约地址
 
 返回值：
-	Code (str): 合约已部署字节码。含 0x 前缀的十六进制形式，当出现异常时返回 None 。
+	Code (str): 合约已部署字节码。当出现异常时返回 None 。
 ```
 
 <br>
 
-`Chain.GetStorage(Address: str, Index: int) -> str`：
+`Chain.GetStorage(Address: str, SlotIndex: int) -> str`：
 
 ```
 根据合约地址和存储插槽索引获取存储值。
 
 参数：
 	Address (str): 合约地址
 	SlotIndex (int): 存储插槽索引
 
 返回值：
-	Data (str): 存储值。含 0x 前缀的十六进制形式，当出现异常时返回 None 。
+	Data (str): 存储值。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Chain.DumpStorage(Address: str, Count: int) -> list`：
 
 ```
 根据合约地址和指定插槽数量值，从插槽 0 开始批量遍历存储插槽并获取值。
 
 参数：
 	Address (str): 合约地址
 	Count (int): 指定插槽数量值
 
 返回值：
-	Data (List[str]): 存储值列表。含 0x 前缀的十六进制形式，当出现异常时返回 None 。
+	Data (List[str]): 存储值列表。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Chain.GetPublicKeyByTransactionHash(TransactionHash: str) -> tuple`：
 
 ```
@@ -222,55 +225,55 @@
 `Account(Chain: Chain, PrivateKey: str)`：
 
 ```
 初始化。通过私钥导入账户并与 Chain 实例绑定，后续的交易将经由该指定账户发送至链上。当导入账户失败时将会抛出异常。
 
 参数：
 	Chain (Poseidon.Blockchain.Chain): 区块链实例
-	PrivateKey (str): 账户私钥。不含 0x 前缀的十六进制形式。
+	PrivateKey (str): 账户私钥。
 
 成员变量：
 	EthAccount (eth_account.Account): eth_account 的原生 Account 对象实例
 ```
 
 <br>
 
 `Account.RequestAuthorizationBeforeSendTransaction(Open: bool = True)`：
 
 ```
-设置在通过该账户发送每一笔交易之前是否请求授权。开启后会在每笔交易即将发送前暂停流程，在终端询问是否发送该笔交易。在实例化 Account 对象时默认设置为 False 。
+设置在通过该账户发送每一笔交易之前是否请求授权。开启后会在每笔交易即将发送前暂停流程，在终端询问是否发送该笔交易。
 
 参数：
-	Open (bool): 请求授权开关。函数定义的默认值为 True ，但在实例化 Account 对象时默认设置为 False 。
+	Open (bool): 请求授权开关。主动调用时默认值为 True ，但在 Account 实例初始化时默认设置为 False 。
 ```
 
 <br>
 
 `Account.GetSelfBalance() -> int`：
 
 ```
 获取自身账户的网络原生代币余额。
 
 返回值：
-	Balance (int): 自身账户网络原生代币余额。单位为 wei ，当出现异常时返回 None 。
+	Balance (int): 自身账户网络原生代币余额，单位为 wei 。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Account.Transfer(To: str, Value: int, Data: str = "0x", GasPrice: Optional[int] = None, GasLimit: int = 100000) -> dict`：
 
 ```
 向指定账户转账指定数量的网络原生代币，可附带信息。若 120 秒内交易未确认则作超时处理。
 
 参数：
 	To (str): 接收方地址
-	Value (int): 发送的网络原生代币数量。单位为 wei 。
-	Data (可选)(str): 交易数据。含 0x 前缀的十六进制形式，默认值为 "0x" 。
-	GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 100000 wei 。
+	Value (int): 发送的网络原生代币数量，单位为 wei 。
+	Data (可选)(str): 交易数据。含 0x 前缀的十六进制形式。默认值为 "0x" 。
+	GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 100000 wei 。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
 <br>
 
@@ -278,17 +281,17 @@
 
 ```
 以传统方式发送一笔自定义交易。若 120 秒内交易未确认则作超时处理。
 
 参数：
 	To (str): 接收方地址
 	Data (str): 交易数据。含 0x 前缀的十六进制形式。
-	Value (可选)(int): 随交易发送的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-	GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 1000000 wei 。
+	Value (可选)(int): 随交易发送的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+	GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 1000000 wei 。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
 <br>
 
@@ -296,54 +299,54 @@
 
 ```
 以 EIP-1559 方式发送一笔自定义交易。若 120 秒内交易未确认则作超时处理。
 
 参数：
 	To (str): 接收方地址
 	Data (str): 交易数据。含 0x 前缀的十六进制形式。
-	Value (可选)(int): 随交易发送的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-	BaseFee (可选)(Optional[int]): BaseFee 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	MaxPriorityFee (可选)(Optional[int]): MaxPriorityFee 价格。单位为 wei ，默认使用 RPC 建议的 max_priority_fee 。
-	GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 1000000 wei 。
+	Value (可选)(int): 随交易发送的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+	BaseFee (可选)(Optional[int]): BaseFee 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	MaxPriorityFee (可选)(Optional[int]): MaxPriorityFee 价格，单位为 wei ，默认使用 RPC 建议的 max_priority_fee 。
+	GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 1000000 wei 。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Account.DeployContract(ABI: dict, Bytecode: str, Value: int = 0, GasPrice: Optional[int] = None, *Arguments: Optional[Any]) -> dict`：
 
 ```
 部署合约。若 120 秒内交易未确认则作超时处理。
 
 参数：
 	ABI (dict): 合约 ABI
-	Bytecode (str): 合约部署字节码。含 0x 前缀的十六进制形式。
-	Value (可选)(int): 随交易发送给合约的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-	GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	Bytecode (str): 合约部署字节码。
+	Value (可选)(int): 随交易发送给合约的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+	GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
 	*Arguments (可选)(Optional[Any]): 传给合约构造函数的参数，默认为空。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
-	当合约部署成功时，字典中会额外添加"Contract"字段，该变量是已实例化的 Contract 对象，失败时为 None。
+	当合约部署成功时，字典中会额外添加"Contract"字段，该变量是已实例化的 Contract 对象，若失败则为 None。
 ```
 
 <br>
 
 `Account.DeployContractWithoutABI(Bytecode: str, Value: int = 0, GasPrice: Optional[int] = None, GasLimit: int = 5000000) -> dict`：
 
 ```
 在没有 ABI 的情况下，仅使用字节码来部署合约。若 120 秒内交易未确认则作超时处理。
 
 参数：
-	Bytecode (str): 合约部署字节码。含 0x 前缀的十六进制形式。
-	Value (可选)(int): 随交易发送给合约的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-	GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 5000000 wei 。
+	Bytecode (str): 合约部署字节码。
+	Value (可选)(int): 随交易发送给合约的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+	GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 5000000 wei 。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
 <br>
 
@@ -415,17 +418,17 @@
 
 `Contract.CallFunctionWithParameters(Value: int, GasPrice: Optional[int], GasLimit: int, FunctionName: str, *FunctionArguments: Optional[Any]) -> dict`：
 
 ```
 通过传入函数名及参数来调用该合约内的函数。支持自定义 Value 和 GasLimit 。
 
 参数：
-	Value (int): 随交易发送的网络原生代币数量。单位为 wei 。
-	GasPrice (Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	GasLimit (int): Gas 最大使用量。单位为 wei 。
+	Value (int): 随交易发送的网络原生代币数量，单位为 wei 。
+	GasPrice (Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	GasLimit (int): Gas 最大使用量，单位为 wei 。
 	FunctionName (str): 函数名称
 	*FunctionArguments (Optional[Any]): 函数参数，默认为空。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
@@ -457,14 +460,28 @@
 
 返回值：
 	CallData (str): 调用数据编码。含 0x 前缀的十六进制形式。当出现异常时返回 None 。
 ```
 
 <br>
 
+`Contract.DecodeFunctionInputData(InputData: str) -> tuple`：
+
+```
+解码对当前合约执行调用的 InputData ，得出所调用的函数及其参数值。
+
+参数：
+	InputData (str): 对当前合约执行调用的 InputData
+
+返回值：
+	Result (tuple): 函数及其参数值
+```
+
+<br>
+
 ### BlockchainUtils 类
 
 通用工具集，整合了常用的链下操作。静态类，无需实例化。
 
 `BlockchainUtils.SwitchSolidityVersion(SolidityVersion: str)`：
 
 ```
@@ -580,19 +597,19 @@
 
 ```
 将 R S V 合并成签名。
 
 参数：
 	R (str): 签名 r 值。含 0x 前缀的十六进制形式。
 	S (str): 签名 s 值。含 0x 前缀的十六进制形式。
-	V (int): 签名 v 值。十进制数字。
+	V (int): 签名 v 值。含 0x 前缀的十六进制形式。
 
 返回值：
 	Result (dict): 合并结果。当出现异常时返回 None 。
-	{"R"|"S"|"V"|"Signature"}
+	{"Signature"|"R"|"S"|"V"}
 ```
 
 <br>
 
 `BlockchainUtils.GetFunctionSelector(FunctionName: str, FunctionParameters: Optional[List[str]] = None) -> str`：
 
 ```
@@ -664,14 +681,45 @@
 
 返回值：
 	ToGenerateFunction (str): 碰撞出的函数的名称与参数完整表示。当出现异常时返回 None 。
 ```
 
 <br>
 
+`BlockchainUtils.GetContractAddressByCREATE(Deployer: str, Nonce: int) -> str`：
+
+```
+获取某账户以 CREATE 方式部署的合约的地址。
+
+参数：
+	Deployer (str): 部署者地址
+	Nonce (int): 部署者发送合约部署交易的 nonce 值
+
+返回值：
+	Address (str): 计算出的合约地址
+```
+
+<br>
+
+`BlockchainUtils.GetContractAddressByCREATE2(Deployer: str, Salt: str, CreationCode: str) -> str`：
+
+```
+获取某合约账户以 CREATE2 方式部署的另一个合约的地址。
+
+参数：
+	Deployer (str): 部署者地址
+	Salt (str): 盐值
+	CreationCode (str): 合约的创建时字节码
+
+返回值：
+	Address (str): 计算出的合约地址
+```
+
+<br>
+
 ## Cryptography 模块
 
 本模块用于解决常见的密码学问题。
 
 ```python
 from Poseidon.Cryptography import ModernCryptoUtils, ClassicalCryptoUtils, MiscUtils
 ```
```

### Comparing `poseidon-python-1.1.4/Poseidon/Blockchain.py` & `poseidon-python-1.1.5/Poseidon/Blockchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """
 本模块可用于与任何以太坊同构链（即通常所说的 EVM 链）进行交互，支持常用的链上交互操作。
 """
 
-from web3 import Web3
+import os
+import pkg_resources
+from web3 import Web3, utils
 from eth_account import Account as EthAccount
 from loguru import logger
 from typing import Optional, Union, List, Any
 from traceback import format_exc
 from json import dump, dumps
-import os
 
 LogPath = os.path.join("logs", "Poseidon_{time}.log")
+Version = pkg_resources.get_distribution("poseidon-python").version
 logger.add(LogPath)
+logger.success(f"\n[Poseidon]Current Poseidon Version [{Version}]\n{'-'*80}")
 
 
 class Chain():
     """
     Chain 是区块链实例，后续的所有链上交互的操作都将经由该指定节点处理。
     """
 
     def __init__(self, RPCUrl: str, RequestParams: Optional[dict] = None):
         """
-        初始化。根据给定的节点 RPC 地址进行连接，可通过代理访问。当连接节点失败时会抛出异常。
+        初始化。根据给定的节点 RPC 地址以 HTTP/HTTPS 方式进行连接，可通过代理访问。当连接节点失败时会抛出异常。
 
         参数：
             RPCUrl (str): 节点 RPC 地址
             RequestParams (可选)(Optional[dict]): 连接时使用的 request 参数，默认为 None。
             例如当需要使用代理进行访问时，则传入 RequestParams={"proxies": {"http": "http://localhost:<ProxyPort>","https": "http://localhost:<ProxyPort>"}}
 
         成员变量：
@@ -42,34 +45,47 @@
         self.Node = Web3(HTTPProvider(RPCUrl, request_kwargs=RequestParams))
         if self.Node.is_connected():
             FinishTime = time()
             Delay = round((FinishTime - StartTime) * 1000)
             logger.success(f"\n[Chain][Initialize]Connected to [{RPCUrl}] [{Delay} ms]\n{RequestParamsPrint}{'-'*80}")
             self.Node.middleware_onion.inject(geth_poa_middleware, layer=0)
             self.Eth = self.Node.eth
-            self.GetBasicInformation()
+            self.GetBasicInformation(False)
         else:
             logger.error(f"\n[Chain][Initialize]Failed to connect to [{RPCUrl}]\n{RequestParamsPrint}{'-'*80}")
             raise Exception("Failed to connect to chain.")
 
-    def GetBasicInformation(self) -> dict:
+    def GetBasicInformation(self, ShowTimeslot: bool = True) -> dict:
         """
-        获取区块链基本信息。包括链 ID 、区块高度、 GasPrice 、出块间隔、当前节点的客户端软件版本号。
+        获取区块链基本信息。包括 ChainId 、BlockNumber 、GasPrice 、(Timeslot)、ClientVersion 。
+
+        参数：
+            ShowTimeslot (bool): 是否获取并显示 Timeslot 。该操作比较耗时，在主动调用时默认为 True , 在 Chain 实例初始化时默认为 False 。
 
         返回值：
             BasicInformation (dict): 区块链基本信息构成的字典。
-            {"ChainId"|"BlockNumber"|"GasPrice"|"Timeslot"|"ClientVersion"}
+            {"ChainId"|"BlockNumber"|"GasPrice"|("Timeslot")|"ClientVersion"}
         """
 
         self.ChainId, BlockNumber, GasPrice, ClientVersion = self.Eth.chain_id, self.Eth.block_number, self.Eth.gas_price, self.Node.client_version
-        Timeslot = self.Eth.get_block(BlockNumber).timestamp - self.Eth.get_block(BlockNumber - 1).timestamp
+        TimeslotPrint = ""
+        if ShowTimeslot:
+            Timeslot = self.Eth.get_block(BlockNumber).timestamp - self.Eth.get_block(BlockNumber - 1).timestamp
+            TimeslotPrint = f"[Timeslot]{Timeslot}s\n"
         logger.success(
-            f"\n[Chain][GetBasicInformation]\n[ChainId]{self.ChainId}\n[BlockNumber]{BlockNumber}\n[GasPrice]{Web3.from_wei(GasPrice, 'gwei')} Gwei\n[Timeslot]{Timeslot}s\n[ClientVersion]{ClientVersion}\n{'-'*80}"
+            f"\n[Chain][GetBasicInformation]\n[ChainId]{self.ChainId}\n[BlockNumber]{BlockNumber}\n[GasPrice]{Web3.from_wei(GasPrice, 'gwei')} Gwei\n{TimeslotPrint}[ClientVersion]{ClientVersion}\n{'-'*80}"
         )
-        return {"ChainId": self.ChainId, "BlockNumber": BlockNumber, "GasPrice": GasPrice, "Timeslot": Timeslot, "ClientVersion": ClientVersion}
+        BasicInformation = {
+            "ChainId": self.ChainId,
+            "BlockNumber": BlockNumber,
+            "GasPrice": GasPrice,
+            "Timeslot": Timeslot if ShowTimeslot else None,
+            "ClientVersion": ClientVersion
+        }
+        return BasicInformation
 
     def GetTransactionInformationByHash(self, TransactionHash: str) -> dict:
         """
         根据交易哈希查询该交易的详细回执信息。包括交易哈希、所在区块号、交易索引号、交易状态、交易类型、交易行为、发送者、接收者、(部署的合约地址)、(GasPrice 或 (MaxFeePerGas 和 MaxPriorityFeePerGas))、GasLimit、GasUsed、Nonce、Value、R、S、V、Logs、InputData。
 
         参数：
             TransactionHash (str): 要查询的交易的哈希
@@ -83,21 +99,44 @@
             Info = self.Eth.wait_for_transaction_receipt(TransactionHash, timeout=120)
             BlockNumber, TransactionIndex, Status, From, To, ContractAddress, GasUsed, Logs = Info.blockNumber, Info.transactionIndex, Info.status, Info["from"], Info.to, Info.contractAddress, Info.gasUsed, Web3.to_json(Info.logs)
             Info = self.Eth.get_transaction(TransactionHash)
             TransactionHash, GasPrice, MaxFeePerGas, MaxPriorityFeePerGas, GasLimit, Nonce, Value, R, S, V, InputData = Info.hash.hex(), Info.gasPrice, Info.get("maxFeePerGas", None), Info.get("maxPriorityFeePerGas", None), Info.gas, Info.nonce, Info.value, Info.r.hex(), Info.s.hex(), Info.v, Info.input
             Type = "EIP-1559" if MaxFeePerGas or MaxPriorityFeePerGas else "Traditional"
             Action = "Deploy Contract" if To == None else "Call Contract" if self.Eth.get_code(Web3.to_checksum_address(To)).hex() != "0x" else "Normal Transfer"
             ContractPrint = f"[ContractAddress]{ContractAddress}\n" if ContractAddress else ""
-            GasPricePrint = f"[GasPrice]{Web3.from_wei(GasPrice, 'gwei')} Gwei" if Type == "Traditional" else f"[MaxFeePerGas]{Web3.from_wei(MaxFeePerGas, 'gwei')} Gwei\n[MaxPriorityFeePerGas]{Web3.from_wei(MaxPriorityFeePerGas, 'gwei')} Gwei"
+            GasPricePrint = f"[MaxFeePerGas]{Web3.from_wei(MaxFeePerGas, 'gwei')} Gwei\n[MaxPriorityFeePerGas]{Web3.from_wei(MaxPriorityFeePerGas, 'gwei')} Gwei" if Type == "EIP-1559" else f"[GasPrice]{Web3.from_wei(GasPrice, 'gwei')} Gwei"
             GeneralPrint = f"\n[Chain][GetTransactionInformationByHash]\n[TransactionHash]{TransactionHash}\n[BlockNumber]{BlockNumber}\n[TransactionIndex]{TransactionIndex}\n[Status]{'Success' if Status else 'Fail'}\n[Type]{Type}\n[Action]{Action}\n[From]{From}\n[To]{To}\n{ContractPrint}{GasPricePrint}\n[GasLimit]{GasLimit} [GasUsed]{GasUsed}\n[Nonce]{Nonce} [Value]{Value}\n[R]{R}\n[S]{S}\n[V]{V}\n[Logs]{Logs}\n[InputData]{InputData}\n{'-'*80}"
             if Status:
                 logger.success(GeneralPrint)
             else:
                 logger.error(GeneralPrint)
-            return {"TransactionHash": TransactionHash, "BlockNumber": BlockNumber, "TransactionIndex": TransactionIndex, "Status": Status, "Type": Type, "Action": Action, "From": From, "To": To, "ContractAddress": ContractAddress, "GasPrice": GasPrice, "MaxFeePerGas": MaxFeePerGas, "MaxPriorityFeePerGas": MaxPriorityFeePerGas, "GasLimit": GasLimit, "GasUsed": GasUsed, "Nonce": Nonce, "Value": Value, "R": R, "S": S, "V": V, "Logs": Logs, "InputData": InputData}
+            TransactionInformation = {
+                "TransactionHash": TransactionHash,
+                "BlockNumber": BlockNumber,
+                "TransactionIndex": TransactionIndex,
+                "Status": Status,
+                "Type": Type,
+                "Action": Action,
+                "From": From,
+                "To": To,
+                "ContractAddress": ContractAddress,
+                "GasPrice": GasPrice,
+                "MaxFeePerGas": MaxFeePerGas,
+                "MaxPriorityFeePerGas": MaxPriorityFeePerGas,
+                "GasLimit": GasLimit,
+                "GasUsed": GasUsed,
+                "Nonce": Nonce,
+                "Value": Value,
+                "R": R,
+                "S": S,
+                "V": V,
+                "Logs": Logs,
+                "InputData": InputData
+            }
+            return TransactionInformation
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(
                 f"\n[Chain][GetTransactionInformationByHash]Failed\n[TransactionHash]{TransactionHash}\n[ExceptionInformation]{ExceptionInformation}{'-'*80}"
             )
             return None
 
@@ -118,21 +157,44 @@
             Info = self.Eth.get_transaction_by_block(BlockID, TransactionIndex)
             TransactionHash, BlockNumber, TransactionIndex, From, To, GasPrice, MaxFeePerGas, MaxPriorityFeePerGas, GasLimit, Nonce, Value, R, S, V, InputData = Info.hash.hex(), Info.blockNumber, Info.transactionIndex, Info["from"], Info.to, Info.gasPrice, Info.get("maxFeePerGas", None), Info.get("maxPriorityFeePerGas", None), Info.gas, Info.nonce, Info.value, Info.r.hex(), Info.s.hex(), Info.v, Info.input
             Info = self.Eth.wait_for_transaction_receipt(TransactionHash, timeout=120)
             Status, GasUsed, ContractAddress, Logs = Info.status, Info.gasUsed, Info.contractAddress, Info.logs
             Type = "EIP-1559" if MaxFeePerGas else "Traditional"
             Action = "Deploy Contract" if To == None else "Call Contract" if self.Eth.get_code(Web3.toChecksumAddress(To)).hex() != "0x" else "Normal Transfer"
             ContractPrint = f"[ContractAddress]{ContractAddress}\n" if ContractAddress else ""
-            GasPricePrint = f"[GasPrice]{Web3.from_wei(GasPrice, 'gwei')} Gwei" if Type == "Traditional" else f"[MaxFeePerGas]{Web3.from_wei(MaxFeePerGas, 'gwei')} Gwei\n[MaxPriorityFeePerGas]{Web3.from_wei(MaxPriorityFeePerGas, 'gwei')} Gwei"
+            GasPricePrint = f"[MaxFeePerGas]{Web3.from_wei(MaxFeePerGas, 'gwei')} Gwei\n[MaxPriorityFeePerGas]{Web3.from_wei(MaxPriorityFeePerGas, 'gwei')} Gwei" if Type == "EIP-1559" else f"[GasPrice]{Web3.from_wei(GasPrice, 'gwei')} Gwei"
             GeneralPrint = f"\n[Chain][GetTransactionInformationByBlockIdAndIndex]\n[TransactionHash]{TransactionHash}\n[BlockNumber]{BlockNumber}\n[TransactionIndex]{TransactionIndex}\n[Status]{'Success' if Status else 'Fail'}\n[Type]{Type}\n[Action]{Action}\n[From]{From}\n[To]{To}\n{ContractPrint}{GasPricePrint}\n[GasLimit]{GasLimit} [GasUsed]{GasUsed}\n[Nonce]{Nonce} [Value]{Value}\n[R]{R}\n[S]{S}\n[V]{V}\n[Logs]{Logs}\n[InputData]{InputData}\n{'-'*80}"
             if Status:
                 logger.success(GeneralPrint)
             else:
                 logger.error(GeneralPrint)
-            return {"TransactionHash": TransactionHash, "BlockNumber": BlockNumber, "TransactionIndex": TransactionIndex, "Status": Status, "Type": Type, "Action": Action, "From": From, "To": To, "ContractAddress": ContractAddress, "GasPrice": GasPrice, "MaxFeePerGas": MaxFeePerGas, "MaxPriorityFeePerGas": MaxPriorityFeePerGas, "GasLimit": GasLimit, "GasUsed": GasUsed, "Nonce": Nonce, "Value": Value, "R": R, "S": S, "V": V, "Logs": Logs, "InputData": InputData}
+            TransactionInformation = {
+                "TransactionHash": TransactionHash,
+                "BlockNumber": BlockNumber,
+                "TransactionIndex": TransactionIndex,
+                "Status": Status,
+                "Type": Type,
+                "Action": Action,
+                "From": From,
+                "To": To,
+                "ContractAddress": ContractAddress,
+                "GasPrice": GasPrice,
+                "MaxFeePerGas": MaxFeePerGas,
+                "MaxPriorityFeePerGas": MaxPriorityFeePerGas,
+                "GasLimit": GasLimit,
+                "GasUsed": GasUsed,
+                "Nonce": Nonce,
+                "Value": Value,
+                "R": R,
+                "S": S,
+                "V": V,
+                "Logs": Logs,
+                "InputData": InputData
+            }
+            return TransactionInformation
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(
                 f"\n[Chain][GetTransactionInformationByBlockIdAndIndex]Failed\n[BlockID]{BlockID}\n[TransactionIndex]{TransactionIndex}\n[ExceptionInformation]{ExceptionInformation}{'-'*80}"
             )
             return None
 
@@ -150,15 +212,24 @@
 
         try:
             Info = self.Eth.get_block(BlockID)
             BlockNumber, BlockHash, Miner, TimeStamp, GasLimit, GasUsed, Transactions = Info.number, Info.hash.hex(), Info.miner, Info.timestamp, Info.gasLimit, Info.gasUsed, Web3.to_json(Info.transactions)
             logger.success(
                 f"\n[Chain][GetBlockInformation]\n[BlockNumber]{BlockNumber}\n[BlockHash]{BlockHash}\n[Miner]{Miner}\n[TimeStamp]{TimeStamp}\n[GasLimit]{GasLimit}\n[GasUsed]{GasUsed}\n[Transactions]{Transactions}"
             )
-            return {"BlockNumber": BlockNumber, "BlockHash": BlockHash, "Miner": Miner, "TimeStamp": TimeStamp, "GasLimit": GasLimit, "GasUsed": GasUsed, "Transactions": Transactions}
+            BlockInformation = {
+                "BlockNumber": BlockNumber,
+                "BlockHash": BlockHash,
+                "Miner": Miner,
+                "TimeStamp": TimeStamp,
+                "GasLimit": GasLimit,
+                "GasUsed": GasUsed,
+                "Transactions": Transactions
+            }
+            return BlockInformation
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(
                 f"\n[Chain][GetBlockInformation]Failed\n[BlockID]{BlockID}\n[ExceptionInformation]{ExceptionInformation}{'-'*80}"
             )
             return None
 
@@ -166,15 +237,15 @@
         """
         根据账户地址获取其网络原生代币余额。
 
         参数：
             Address (str): 账户地址
 
         返回值：
-            Balance (int): 账户网络原生代币余额。单位为 wei ，当出现异常时返回 None 。
+            Balance (int): 账户网络原生代币余额，单位为 wei 。当出现异常时返回 None 。
         """
 
         try:
             Address = Web3.to_checksum_address(Address)
             Balance = self.Eth.get_balance(Address)
             logger.success(
                 f"\n[Chain][GetBalance]\n[Address]{Address}\n[Balance][{Balance} Wei]<=>[{Web3.from_wei(Balance,'ether')} Ether]\n{'-'*80}"
@@ -189,15 +260,15 @@
         """
         根据合约地址获取其已部署字节码。
 
         参数：
             Address (str): 合约地址
 
         返回值：
-            Code (str): 合约已部署字节码。含 0x 前缀的十六进制形式，当出现异常时返回 None 。
+            Code (str): 合约已部署字节码。当出现异常时返回 None 。
         """
 
         try:
             Address = Web3.to_checksum_address(Address)
             Code = self.Eth.get_code(Address).hex()
             logger.success(f"\n[Chain][GetCode]\n[Address]{Address}\n[Code]{Code}\n{'-'*80}")
             return Code
@@ -211,15 +282,15 @@
         根据合约地址和存储插槽索引获取存储值。
 
         参数：
             Address (str): 合约地址
             SlotIndex (int): 存储插槽索引
 
         返回值：
-            Data (str): 存储值。含 0x 前缀的十六进制形式，当出现异常时返回 None 。
+            Data (str): 存储值。当出现异常时返回 None 。
         """
 
         try:
             Address = Web3.to_checksum_address(Address)
             Data = self.Eth.get_storage_at(Address, SlotIndex).hex()
             logger.success(
                 f"\n[Chain][GetStorage]\n[Address]{Address}\n[SlotIndex]{SlotIndex}\n[Value][Hex][{Data}]<=>[Dec][{int(Data,16)}]\n{'-'*80}"
@@ -237,15 +308,15 @@
         根据合约地址和指定插槽数量值，从插槽 0 开始批量遍历存储插槽并获取值。
 
         参数：
             Address (str): 合约地址
             Count (int): 指定插槽数量值
 
         返回值：
-            Data (List[str]): 存储值列表。含 0x 前缀的十六进制形式，当出现异常时返回 None 。
+            Data (List[str]): 存储值列表。当出现异常时返回 None 。
         """
 
         try:
             Address = Web3.to_checksum_address(Address)
             Data = [self.Eth.get_storage_at(Address, i).hex() for i in range(Count)]
             Temp = '\n'.join([f"[Slot {i}]{Data[i]}" for i in range(len(Data))])
             logger.success(f"\n[Chain][DumpStorage]\n[Address]{Address}\n{Temp}\n{'-'*80}")
@@ -268,16 +339,15 @@
             (Address, PublicKey) (tuple): 由账户地址和账户公钥组成的元组。当出现异常时返回 None 。
         """
 
         try:
             from eth_account._utils.signing import to_standard_v, extract_chain_id, serializable_unsigned_transaction_from_dict
             Transaction = self.Eth.get_transaction(TransactionHash)
             Signature = self.Eth.account._keys.Signature(vrs=(to_standard_v(extract_chain_id(Transaction.v)[1]), Web3.to_int(Transaction.r), Web3.to_int(Transaction.s)))
-            UnsignedTransactionDict = {i: Transaction[i] for i in ['chainId', 'nonce', 'gasPrice' if int(
-                Transaction.type, 0) != 2 else '', 'gas', 'to', 'value', 'accessList', 'maxFeePerGas', 'maxPriorityFeePerGas'] if i in Transaction}
+            UnsignedTransactionDict = {i: Transaction[i] for i in ['chainId', 'nonce', 'gasPrice' if Transaction.type != 2 else '', 'gas', 'to', 'value', 'accessList', 'maxFeePerGas', 'maxPriorityFeePerGas'] if i in Transaction}
             UnsignedTransactionDict['data'] = Transaction['input']
             UnsignedTransaction = serializable_unsigned_transaction_from_dict(UnsignedTransactionDict)
             Temp = Signature.recover_public_key_from_msg_hash(UnsignedTransaction.hash())
             PublicKey = str(Temp).replace('0x', '0x04')  # 比特币未压缩公钥格式
             Address = Temp.to_checksum_address()
             logger.success(
                 f"\n[Chain][GetPublicKeyByTransactionHash]\n[TransactionHash]{TransactionHash}\n[Address]{Address}\n[PublicKey]{PublicKey}\n{'-'*80}"
@@ -298,15 +368,15 @@
 
     def __init__(self, Chain: Chain, PrivateKey: str):
         """
         初始化。通过私钥导入账户并与 Chain 实例绑定，后续的交易将经由该指定账户发送至链上。当导入账户失败时将会抛出异常。
 
         参数：
             Chain (Poseidon.Blockchain.Chain): 区块链实例
-            PrivateKey (str): 账户私钥。不含 0x 前缀的十六进制形式。
+            PrivateKey (str): 账户私钥。
 
         成员变量：
             EthAccount (eth_account.Account): eth_account 的原生 Account 对象实例
         """
 
         try:
             self.EthAccount, self._Chain, self._Eth = EthAccount.from_key(PrivateKey), Chain, Chain.Eth
@@ -317,49 +387,49 @@
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(f"\n[Account][Initialize]Failed to import account\n[ExceptionInformation]{ExceptionInformation}{'-'*80}")
             raise Exception("Failed to import account.")
 
     def RequestAuthorizationBeforeSendTransaction(self, Open: bool = True):
         """
-        设置在通过该账户发送每一笔交易之前是否请求授权。开启后会在每笔交易即将发送前暂停流程，在终端询问是否发送该笔交易。在实例化 Account 对象时默认设置为 False 。
+        设置在通过该账户发送每一笔交易之前是否请求授权。开启后会在每笔交易即将发送前暂停流程，在终端询问是否发送该笔交易。
 
         参数：
-            Open (bool): 请求授权开关。函数定义的默认值为 True ，但在实例化 Account 对象时默认设置为 False 。
+            Open (bool): 请求授权开关。主动调用时默认值为 True ，但在 Account 实例初始化时默认设置为 False 。
         """
 
         self._Request = Open
         if self._Request:
-            logger.success(f"\n[Account][RequestAuthorizationBeforeSendTransaction]Status: True\n{'-'*80}")
+            logger.success(f"\n[Account][RequestAuthorizationBeforeSendTransaction]Open: True\n{'-'*80}")
         else:
-            logger.warning(f"\n[Account][RequestAuthorizationBeforeSendTransaction]Status: False\n{'-'*80}")
+            logger.warning(f"\n[Account][RequestAuthorizationBeforeSendTransaction]Open: False\n{'-'*80}")
 
     def GetSelfBalance(self) -> int:
         """
         获取自身账户的网络原生代币余额。
 
         返回值：
-            Balance (int): 自身账户网络原生代币余额。单位为 wei ，当出现异常时返回 None 。
+            Balance (int): 自身账户网络原生代币余额，单位为 wei 。当出现异常时返回 None 。
         """
 
         Balance = self._Chain.GetBalance(self.EthAccount.address)
         if Balance == 0:
             logger.warning(f"\n[Account][GetSelfBalance]\n[Warning]This account's balance is insufficient to send transactions\n{'-'*80}")
         return Balance
 
     def Transfer(self, To: str, Value: int, Data: str = "0x", GasPrice: Optional[int] = None, GasLimit: int = 100000) -> dict:
         """
         向指定账户转账指定数量的网络原生代币，可附带信息。若 120 秒内交易未确认则作超时处理。
 
         参数：
             To (str): 接收方地址
-            Value (int): 发送的网络原生代币数量。单位为 wei 。
-            Data (可选)(str): 交易数据。含 0x 前缀的十六进制形式，默认值为 "0x" 。
-            GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-            GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 100000 wei 。
+            Value (int): 发送的网络原生代币数量，单位为 wei 。
+            Data (可选)(str): 交易数据。含 0x 前缀的十六进制形式。默认值为 "0x" 。
+            GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+            GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 100000 wei 。
 
         返回值：
             TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
         """
 
         try:
             From = self.EthAccount.address
@@ -396,17 +466,17 @@
     def SendTransaction(self, To: str, Data: str, Value: int = 0, GasPrice: Optional[int] = None, GasLimit: int = 1000000) -> dict:
         """
         以传统方式发送一笔自定义交易。若 120 秒内交易未确认则作超时处理。
 
         参数：
             To (str): 接收方地址
             Data (str): 交易数据。含 0x 前缀的十六进制形式。
-            Value (可选)(int): 随交易发送的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-            GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-            GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 1000000 wei 。
+            Value (可选)(int): 随交易发送的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+            GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+            GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 1000000 wei 。
 
         返回值：
             TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
         """
 
         try:
             From = self.EthAccount.address
@@ -443,18 +513,18 @@
     def SendTransactionByEIP1559(self, To: str, Data: str, Value: int = 0, BaseFee: Optional[int] = None, MaxPriorityFee: Optional[int] = None, GasLimit: int = 1000000) -> dict:
         """
         以 EIP-1559 方式发送一笔自定义交易。若 120 秒内交易未确认则作超时处理。
 
         参数：
             To (str): 接收方地址
             Data (str): 交易数据。含 0x 前缀的十六进制形式。
-            Value (可选)(int): 随交易发送的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-            BaseFee (可选)(Optional[int]): BaseFee 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-            MaxPriorityFee (可选)(Optional[int]): MaxPriorityFee 价格。单位为 wei ，默认使用 RPC 建议的 max_priority_fee 。
-            GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 1000000 wei 。
+            Value (可选)(int): 随交易发送的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+            BaseFee (可选)(Optional[int]): BaseFee 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+            MaxPriorityFee (可选)(Optional[int]): MaxPriorityFee 价格，单位为 wei ，默认使用 RPC 建议的 max_priority_fee 。
+            GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 1000000 wei 。
 
         返回值：
             TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
         """
 
         try:
             From = self.EthAccount.address
@@ -493,28 +563,28 @@
             return None
 
     def DeployContract(self, ABI: dict, Bytecode: str, Value: int = 0, GasPrice: Optional[int] = None, *Arguments: Optional[Any]) -> dict:
         """
         部署合约。若 120 秒内交易未确认则作超时处理。
 
         参数：
-            ABI (dict): 合约 ABI
-            Bytecode (str): 合约部署字节码。含 0x 前缀的十六进制形式。
-            Value (可选)(int): 随交易发送给合约的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-            GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
+            ABI (dict): 合约 ABI 
+            Bytecode (str): 合约部署字节码。
+            Value (可选)(int): 随交易发送给合约的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+            GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
             *Arguments (可选)(Optional[Any]): 传给合约构造函数的参数，默认为空。
 
         返回值：
             TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
-            当合约部署成功时，字典中会额外添加"Contract"字段，该变量是已实例化的 Contract 对象，失败时为 None。
+            当合约部署成功时，字典中会额外添加"Contract"字段，该变量是已实例化的 Contract 对象，若失败则为 None。
         """
 
         try:
             DeployingContract = self._Eth.contract(abi=ABI, bytecode=Bytecode)
-            TransactionData = DeployingContract.constructor(*Arguments).buildTransaction({"value": Value, "gasPrice": GasPrice if GasPrice else self._Eth.gas_price})
+            TransactionData = DeployingContract.constructor(*Arguments).build_transaction({"value": Value, "gasPrice": GasPrice if GasPrice else self._Eth.gas_price})
             Txn = {
                 "chainId": self._Chain.ChainId,
                 "from": self.EthAccount.address,
                 "value": TransactionData["value"],
                 "gas": TransactionData["gas"],
                 "gasPrice": TransactionData["gasPrice"],
                 "nonce": self._Eth.get_transaction_count(self.EthAccount.address),
@@ -546,31 +616,31 @@
             return None
 
     def DeployContractWithoutABI(self, Bytecode: str, Value: int = 0, GasPrice: Optional[int] = None, GasLimit: int = 5000000) -> dict:
         """
         在没有 ABI 的情况下，仅使用字节码来部署合约。若 120 秒内交易未确认则作超时处理。
 
         参数：
-            Bytecode (str): 合约部署字节码。含 0x 前缀的十六进制形式。
-            Value (可选)(int): 随交易发送给合约的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-            GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-            GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 5000000 wei 。
+            Bytecode (str): 合约部署字节码。
+            Value (可选)(int): 随交易发送给合约的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+            GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+            GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 5000000 wei 。
 
         返回值：
             TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
         """
 
         try:
             Txn = {
                 "chainId": self._Chain.ChainId,
                 "from": self.EthAccount.address,
                 "value": Value,
                 "gas": GasLimit,
-                "gasPrice": self._Eth.gas_price,
-                "nonce": GasPrice if GasPrice else self._Eth.get_transaction_count(self.EthAccount.address),
+                "gasPrice": GasPrice if GasPrice else self._Eth.gas_price,
+                "nonce": self._Eth.get_transaction_count(self.EthAccount.address),
                 "data": Bytecode,
             }
             SignedTxn = self.EthAccount.sign_transaction(Txn)
             Txn["gasPrice"] = f'{Web3.from_wei(Txn["gasPrice"],"gwei")} Gwei'
             logger.info(f"\n[Account][DeployContractWithoutABI]\n[Txn]{dumps(Txn, indent=2)}\n{'-'*80}")
             if self._Request:
                 logger.warning(f"\n[Account][RequestAuthorizationBeforeSendTransaction][True]\nDo you confirm sending this transaction?")
@@ -599,19 +669,28 @@
             SignatureData (str): 签名数据构成的字典。当出现异常时返回 None 。
             {"Address"|"Message"|"MessageHash"|"Signature"|"R"|"S"|"V"}
         """
 
         try:
             from eth_account.messages import encode_defunct
             SignedMessage = self.EthAccount.sign_message(encode_defunct(text=Message))
-            MessageHash, Signature, R, S, V = SignedMessage.messageHash.hex(), SignedMessage.signature.hex(), hex(SignedMessage.r), hex(SignedMessage.s), SignedMessage.v
+            MessageHash, Signature, R, S, V = SignedMessage.messageHash.hex(), SignedMessage.signature.hex(), f"0x{int(hex(SignedMessage.r), 16):02x}", f"0x{int(hex(SignedMessage.s), 16):02x}", SignedMessage.v
             logger.success(
                 f"\n[Account][SignMessage]\n[Address]{self.EthAccount.address}\n[Message]{Message}\n[MessageHash]{MessageHash}\n[Signature]{Signature}\n[R]{R}\n[S]{S}\n[V]{V}\n{'-'*80}"
             )
-            return {"Address": self.EthAccount.address, "Message": Message, "MessageHash": MessageHash, "Signature": Signature, "R": R, "S": S, "V": V}
+            SignatureData = {
+                "Address": self.EthAccount.address,
+                "Message": Message,
+                "MessageHash": MessageHash,
+                "Signature": Signature,
+                "R": R,
+                "S": S,
+                "V": V
+            }
+            return SignatureData
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(
                 f"\n[Account][SignMessage]Failed to sign message\n[Address]{self.EthAccount.address}\n[Message]{Message}\n[ExceptionInformation]{ExceptionInformation}{'-'*80}"
             )
             return None
 
@@ -625,19 +704,27 @@
         返回值：
             SignatureData (str): 签名数据构成的字典。当出现异常时返回 None 。
             {"Address"|"MessageHash"|"Signature"|"R"|"S"|"V"}
         """
 
         try:
             SignedMessage = self.EthAccount.signHash(MessageHash)
-            Signature, R, S, V = SignedMessage.signature.hex(), hex(SignedMessage.r), hex(SignedMessage.s), SignedMessage.v
+            Signature, R, S, V = SignedMessage.signature.hex(), f"0x{int(hex(SignedMessage.r), 16):02x}", f"0x{int(hex(SignedMessage.s), 16):02x}", SignedMessage.v
             logger.success(
                 f"\n[Account][SignMessageHash]\n[Address]{self.EthAccount.address}\n[MessageHash]{MessageHash}\n[Signature]{Signature}\n[R]{R}\n[S]{S}\n[V]{V}\n{'-'*80}"
             )
-            return {"Address": self.EthAccount.address, "MessageHash": MessageHash, "Signature": Signature, "R": R, "S": S, "V": V}
+            SignatureData = {
+                "Address": self.EthAccount.address,
+                "MessageHash": MessageHash,
+                "Signature": Signature,
+                "R": R,
+                "S": S,
+                "V": V
+            }
+            return SignatureData
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(
                 f"\n[Account][SignMessageHash]Failed\n[Address]{self.EthAccount.address}\n[MessageHash]{MessageHash}\n[ExceptionInformation]{ExceptionInformation}{'-'*80}"
             )
             return None
 
@@ -680,35 +767,35 @@
             FunctionName (str): 函数名称
             *FunctionArguments (可选)(Optional[Any]): 函数参数，默认为空。
 
         返回值：
             TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
         """
 
-        TransactionData = self.Instance.functions[FunctionName](*FunctionArguments).buildTransaction({"gasPrice": self._Eth.gas_price})
+        TransactionData = self.Instance.functions[FunctionName](*FunctionArguments).build_transaction({"gasPrice": self._Eth.gas_price})
         logger.info(f"\n[Contract][CallFunction]\n[ContractAddress]{self.Address}\n[Function]{FunctionName}{FunctionArguments}\n{'-'*80}")
         TransactionInformation = self._Account.SendTransaction(self.Address, TransactionData["data"], TransactionData["value"], TransactionData['gasPrice'], TransactionData["gas"])
         return TransactionInformation
 
     def CallFunctionWithParameters(self, Value: int, GasPrice: Optional[int], GasLimit: int, FunctionName: str, *FunctionArguments: Optional[Any]) -> dict:
         """
         通过传入函数名及参数来调用该合约内的函数。支持自定义 Value 和 GasLimit 。
 
         参数：
-            Value (int): 随交易发送的网络原生代币数量。单位为 wei 。
-            GasPrice (Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-            GasLimit (int): Gas 最大使用量。单位为 wei 。
+            Value (int): 随交易发送的网络原生代币数量，单位为 wei 。
+            GasPrice (Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+            GasLimit (int): Gas 最大使用量，单位为 wei 。
             FunctionName (str): 函数名称
             *FunctionArguments (Optional[Any]): 函数参数，默认为空。
 
         返回值：
             TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
         """
 
-        TransactionData = self.Instance.functions[FunctionName](*FunctionArguments).buildTransaction({"value": Value, "gasPrice": GasPrice if GasPrice else self._Eth.gas_price, "gas": GasLimit})
+        TransactionData = self.Instance.functions[FunctionName](*FunctionArguments).build_transaction({"value": Value, "gasPrice": GasPrice if GasPrice else self._Eth.gas_price, "gas": GasLimit})
         logger.info(
             f"\n[Contract][CallFunctionWithValueAndGasLimit]\n[ContractAddress]{self.Address}\n[Function]{FunctionName}{FunctionArguments}\n[Value]{TransactionData['value']}\n[GasPrice]{TransactionData['gasPrice']}\n[GasLimit]{TransactionData['gas']}\n{'-'*80}"
         )
         TransactionInformation = self._Account.SendTransaction(self.Address, TransactionData["data"], TransactionData["value"], TransactionData['gasPrice'], TransactionData["gas"])
         return TransactionInformation
 
     def ReadOnlyCallFunction(self, FunctionName: str, *FunctionArguments: Optional[Any]) -> Any:
@@ -757,14 +844,38 @@
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(
                 f"\n[Contract][EncodeABI]Failed\n[ContractAddress]{self.Address}\n[Function]{FunctionName}{FunctionArguments}\n[ExceptionInformation]{ExceptionInformation}{'-'*80}"
             )
             return None
 
+    def DecodeFunctionInputData(self, InputData: str) -> tuple:
+        """
+        解码对当前合约执行调用的 InputData ，得出所调用的函数及其参数值。
+
+        参数：
+            InputData (str): 对当前合约执行调用的 InputData 
+
+        返回值：
+            Result (tuple): 函数及其参数值
+        """
+
+        try:
+            Result = self.Instance.decode_function_input(InputData)
+            logger.success(
+                f"\n[Contract][DecodeFunctionInputData]\n[InputData]{InputData}\n[Function]{Result[0]}\n[Parameters]{Result[1]}\n{'-'*80}"
+            )
+            return Result
+        except Exception:
+            ExceptionInformation = format_exc()
+            logger.error(
+                f"\n[Contract][DecodeFunctionInputData]Failed\n[InputData]{InputData}\n[ExceptionInformation]{ExceptionInformation}{'-'*80}"
+            )
+            return None
+
 
 class BlockchainUtils():
     """
     通用工具集，整合了常用的链下操作。静态类，无需实例化。
     """
 
     @staticmethod
@@ -773,17 +884,18 @@
         设置当前使用的 Solidity 版本，若该版本未安装则会自动安装。
 
         参数：
             SolidityVersion (str): Solidity 版本号
         """
 
         try:
-            from solcx import install_solc, set_solc_version
+            from solcx import install_solc, set_solc_version, get_solc_version
             install_solc(SolidityVersion)
             set_solc_version(SolidityVersion)
+            SolidityVersion = get_solc_version(True)
             logger.success(f"\n[BlockchainUtils][SwitchSolidityVersion]Current Solidity Version [{SolidityVersion}]\n{'-'*80}")
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(
                 f"\n[BlockchainUtils][SwitchSolidityVersion]Failed to switch to version [{SolidityVersion}]\n[ExceptionInformation]{ExceptionInformation}{'-'*80}"
             )
 
@@ -828,15 +940,15 @@
         创建新账户。
 
         返回值：
             (Address, PrivateKey) (tuple): 由账户地址和私钥组成的元组
         """
 
         Temp = EthAccount.create()
-        Address, PrivateKey = Web3.to_checksum_address(Temp.address), Temp.privateKey.hex()
+        Address, PrivateKey = Web3.to_checksum_address(Temp.address), Temp.key.hex()
         logger.success(f"\n[BlockchainUtils][CreateNewAccount]\n[Address]{Address}\n[PrivateKey]{PrivateKey}\n{'-'*80}")
         return (Address, PrivateKey)
 
     @staticmethod
     def MnemonicToAddressAndPrivateKey(Mnemonic: str) -> tuple:
         """
         将助记词转换为账户地址与私钥。参考 BIP-39 标准。
@@ -847,15 +959,15 @@
         返回值：
             (Address, PrivateKey) (tuple): 由账户地址和私钥组成的元组。当出现异常时返回 None 。
         """
 
         try:
             EthAccount.enable_unaudited_hdwallet_features()
             Temp = EthAccount.from_mnemonic(Mnemonic)
-            Address, PrivateKey = Web3.to_checksum_address(Temp.address), Temp.privateKey.hex()
+            Address, PrivateKey = Web3.to_checksum_address(Temp.address), Temp.key.hex()
             logger.success(
                 f"\n[BlockchainUtils][MnemonicToAddressAndPrivateKey]\n[Mnemonic]{Mnemonic}\n[Address]{Address}\n[PrivateKey]{PrivateKey}\n{'-'*80}"
             )
             return (Address, PrivateKey)
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(
@@ -870,14 +982,15 @@
 
         参数：
             Value (Union[int,float]): 假设以 Gwei 为单位的待转换值。
 
         返回值：
             Result (int): 已转换为以 wei 为单位的值。当出现异常时返回 None 。
         """
+
         try:
             assert(Value > 0)
             return int(Value * 10**9)
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(
                 f"\n[BlockchainUtils][GweiToWei]Failed\n[Value]{Value}\n[ExceptionInformation]{ExceptionInformation}{'-'*80}"
@@ -946,15 +1059,21 @@
         """
 
         try:
             Signature = hex(int(Signature, 16))
             assert (len(Signature) == 130 + 2)
             R, S, V = '0x' + Signature[2:66], '0x' + Signature[66:-2], int('0x' + Signature[-2:], 16)
             logger.success(f"\n[BlockchainUtils][SignatureToRSV]\n[Signature]{Signature}\n[R]{R}\n[S]{S}\n[V]{V}\n{'-'*80}")
-            return {"Signature": Signature, "R": R, "S": S, "V": V}
+            Result = {
+                "Signature": Signature,
+                "R": R,
+                "S": S,
+                "V": V
+            }
+            return Result
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(
                 f"\n[BlockchainUtils][SignatureToRSV]Failed\n[Signature]{Signature}\n[ExceptionInformation]{ExceptionInformation}{'-'*80}"
             )
             return None
 
@@ -966,23 +1085,29 @@
         参数：
             R (str): 签名 r 值。含 0x 前缀的十六进制形式。
             S (str): 签名 s 值。含 0x 前缀的十六进制形式。
             V (int): 签名 v 值。含 0x 前缀的十六进制形式。
 
         返回值：
             Result (dict): 合并结果。当出现异常时返回 None 。
-            {"R"|"S"|"V"|"Signature"}
+            {"Signature"|"R"|"S"|"V"}
         """
 
         try:
             R, S, V = hex(int(R, 16)), hex(int(S, 16)), hex(int(V, 16))
             assert (len(R) == 64 + 2 and len(S) == 64 + 2 and len(V) == 2 + 2)
             Signature = '0x' + R[2:] + S[2:] + V[2:]
             logger.success(f"\n[BlockchainUtils][RSVToSignature]\n[R]{R}\n[S]{S}\n[V]{V}\n[Signature]{Signature}\n{'-'*80}")
-            return {"R": R, "S": S, "V": V, "Signature": Signature}
+            Result = {
+                "Signature": Signature,
+                "R": R,
+                "S": S,
+                "V": V
+            }
+            return Result
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(
                 f"\n[BlockchainUtils][RSVToSignature]Failed\n[R]{R}\n[S]{S}\n[V]{V}\n[ExceptionInformation]{ExceptionInformation}{'-'*80}"
             )
             return None
 
@@ -994,14 +1119,15 @@
         参数：
             FunctionName (str): 函数名称。
             FunctionParameters (可选)(Optional[List[str]]): 函数参数列表。默认为空。
 
         返回值：
             Result (str): 四字节函数选择器。含 0x 前缀的十六进制形式
         """
+
         try:
             FunctionSelector = Web3.keccak(f"{FunctionName}({','.join(FunctionParameters)})".encode())[:4].hex()
             logger.success(f"\n[BlockchainUtils][GetFunctionSelector]\n[FunctionName]{FunctionName}\n[FunctionParameters]{FunctionParameters}\n[FunctionSelector]{FunctionSelector}\n{'-'*80}")
             return FunctionSelector
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(
@@ -1044,15 +1170,15 @@
             Signature (str): 签名
 
         返回值：
             Signer (str): 签署者的账户地址。当出现异常时返回 None 。
         """
 
         try:
-            Signer = EthAccount.recoverHash(MessageHash, signature=Signature)
+            Signer = EthAccount._recover_hash(MessageHash, signature=Signature)
             logger.success(
                 f"\n[BlockchainUtils][RecoverMessageByHash]\n[MessageHash]{MessageHash}\n[Signature]{Signature}\n[Signer]{Signer}\n{'-'*80}"
             )
             return Signer
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(
@@ -1118,7 +1244,60 @@
             return ToGenerateFunction
         except Exception:
             ExceptionInformation = format_exc()
             logger.error(
                 f"\n[BlockchainUtils][CrackSelector]Failed\n[SourceFunction]{SourceFunctionName}({','.join(SourceFunctionParameters)})\n[ToGenerateFunction]{f'function_?({Temp})'}\n[ExceptionInformation]{ExceptionInformation}{'-'*80}"
             )
             return None
+
+    @staticmethod
+    def GetContractAddressByCREATE(Deployer: str, Nonce: int) -> str:
+        """
+        获取某账户以 CREATE 方式部署的合约的地址。
+
+        参数：
+            Deployer (str): 部署者地址
+            Nonce (int): 部署者发送合约部署交易的 nonce 值
+
+        返回值：
+            Address (str): 计算出的合约地址
+        """
+
+        try:
+            Address = utils.address.get_create_address(Deployer, Nonce)
+            logger.success(
+                f"\n[BlockchainUtils][GetContractAddressByCREATE]\n[Deployer]{Deployer}\n[Nonce]{Nonce}\n[ContractAddress]{Address}\n{'-'*80}"
+            )
+            return Address
+        except Exception:
+            ExceptionInformation = format_exc()
+            logger.error(
+                f"\n[BlockchainUtils][GetContractAddressByCREATE]Failed\n[Deployer]{Deployer}\n[Nonce]{Nonce}\n[ExceptionInformation]{ExceptionInformation}{'-'*80}"
+            )
+            return None
+
+    @staticmethod
+    def GetContractAddressByCREATE2(Deployer: str, Salt: str, CreationCode: str) -> str:
+        """
+        获取某合约账户以 CREATE2 方式部署的另一个合约的地址。
+
+        参数：
+            Deployer (str): 部署者地址
+            Salt (str): 盐值
+            CreationCode (str): 合约的创建时字节码
+
+        返回值：
+            Address (str): 计算出的合约地址
+        """
+
+        try:
+            Address = utils.address.get_create2_address(Deployer, Salt, CreationCode)
+            logger.success(
+                f"\n[BlockchainUtils][GetContractAddressByCREATE2]\n[Deployer]{Deployer}\n[Salt]{Salt}\n[CreationCode]{CreationCode}\n[ContractAddress]{Address}\n{'-'*80}"
+            )
+            return Address
+        except Exception:
+            ExceptionInformation = format_exc()
+            logger.error(
+                f"\n[BlockchainUtils][GetContractAddressByCREATE2]Failed\n[Deployer]{Deployer}\n[Salt]{Salt}\n[CreationCode]{CreationCode}\n[ExceptionInformation]{ExceptionInformation}{'-'*80}"
+            )
+            return None
```

### Comparing `poseidon-python-1.1.4/Poseidon/Cryptography.py` & `poseidon-python-1.1.5/Poseidon/Cryptography.py`

 * *Files identical despite different names*

### Comparing `poseidon-python-1.1.4/Poseidon/PoW.py` & `poseidon-python-1.1.5/Poseidon/PoW.py`

 * *Files identical despite different names*

### Comparing `poseidon-python-1.1.4/README.md` & `poseidon-python-1.1.5/poseidon_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,45 @@
+Metadata-Version: 2.1
+Name: poseidon-python
+Version: 1.1.5
+Summary: 海神波塞冬工具对常用的链上交互操作进行了封装，使得开发者能够便捷地与任何以太坊同构链交互，主要用于在 CTF 比赛中攻克 Blockchain 方向的题目。
+Home-page: https://github.com/B1ue1nWh1te/Poseidon
+Author: B1ue1nWh1te
+Author-email: b1ue1nwh1te@skiff.com
+License: GPL-3.0
+Keywords: POSEIDON,BLOCKCHAIN,EVM,CRYPTO,CTF
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 
 # Poseidon
 
-![data](https://socialify.git.ci/B1ue1nWh1te/Poseidon/image?font=Rokkitt&forks=1&issues=1&language=1&logo=https%3A%2F%2Fimg.seaeye.cn%2Fimg%2Fseaeye%2Flogo.png&owner=1&pattern=Circuit%20Board&stargazers=1&theme=Light)
+![data](https://socialify.git.ci/B1ue1nWh1te/Poseidon/image?font=Rokkitt&forks=1&issues=1&language=1&logo=https%3A%2F%2Fimg.seaeye.cn%2Fimg%2Fseaverse%2Flogo.png&owner=1&pattern=Circuit%20Board&stargazers=1&theme=Light)
 
 **海神波塞冬 Poseidon** 工具对常用的链上交互操作进行了封装，使得开发者能够便捷地
 
 与任何以太坊同构链交互，主要用于在 CTF 比赛中攻克 Blockchain 方向的题目。
 
 [![Lisence](https://img.shields.io/github/license/B1ue1nWh1te/Poseidon)](https://github.com/B1ue1nWh1te/Poseidon/blob/main/LICENSE)
-[![Python Version](https://img.shields.io/badge/python-3.8+-blue)](https://www.python.org/)
+[![Python](https://img.shields.io/badge/python-3.9+-blue)](https://www.python.org/)
 [![Release](https://img.shields.io/github/v/release/B1ue1nWh1te/Poseidon?include_prereleases)](https://github.com/B1ue1nWh1te/Poseidon/releases/)
 [![Visitors](https://visitor-badge.glitch.me/badge?page_id=B1ue1nWh1te-Poseidon&left_color=gray&right_color=orange)](https://github.com/B1ue1nWh1te/Poseidon)
-![Downloads](https://img.shields.io/pypi/dm/poseidon-python)
+![Downloads](https://img.shields.io/pypi/dd/poseidon-python)
 
 </div>
 
 # 注意事项
 
 1. **本工具原则上仅可用于 CTF 比赛解题或测试链开发。但开源工具无法约束使用场景，若执意要在具有经济价值的公链中使用，所产生的影响将由你自行承担。**
 
 2. 在使用 `Blockchain` 模块时，你始终应该使用全新生成的账户，而不是导入常用的具有实际价值的账户，以确保你的账户安全。
 
-3. `Blockchain` 模块的所有功能在 `Goerli` 测试网络中均正常通过检验。
+3. `Blockchain` 模块的所有功能在 `Goerli, Sepolia` 测试网络中均正常通过检验。
 
 4. 如果你在使用过程中遇到了其他问题，或者有任何好的想法和建议，欢迎提[issue](https://github.com/B1ue1nWh1te/Poseidon/issues)进行反馈。
 
 # 安装
 
 ```bash
 pip install -U poseidon-python
@@ -53,52 +66,55 @@
 ### Chain 类
 
 Chain 是区块链实例，后续的所有链上交互的操作都将经由该指定节点处理。
 
 `Chain(RPCUrl: str, RequestParams: Optional[dict] = None)`：
 
 ```
-初始化。根据给定的节点 RPC 地址进行连接，可通过代理访问。当连接节点失败时会抛出异常。
+初始化。根据给定的节点 RPC 地址以 HTTP/HTTPS 方式进行连接，可通过代理访问。当连接节点失败时会抛出异常。
 
 参数：
 	RPCUrl (str): 节点 RPC 地址
 	RequestParams (可选)(Optional[dict]): 连接时使用的 request 参数，默认为 None。
 	例如当需要使用代理进行访问时，则传入 RequestParams={"proxies": {"http": "http://localhost:<ProxyPort>","https": "http://localhost:<ProxyPort>"}}
 
 成员变量：
 	ChainId (int): 链 ID
 	Node (Web3.HTTPProvider): web3.py 原生的 HTTP 交互器实例
 	Eth (Web3.HTTPProvider.eth): HTTP 交互器实例中的 eth 模块
 ```
 
 <br>
 
-`Chain.GetBasicInformation() -> dict`：
+`Chain.GetBasicInformation(ShowTimeslot: bool = True) -> dict`：
 
 ```
-获取区块链基本信息。包括链 ID 、区块高度、 GasPrice 、出块间隔、当前节点的客户端软件版本号。
+获取区块链基本信息。包括 ChainId 、BlockNumber 、GasPrice 、(Timeslot)、ClientVersion 。
+
+参数：
+	ShowTimeslot (bool): 是否获取并显示 Timeslot 。该操作比较耗时，在主动调用时默认为 True , 在 Chain 实例初始化时默认为 False 。
 
 返回值：
 	BasicInformation (dict): 区块链基本信息构成的字典。
-	{"ChainId"|"BlockNumber"|"GasPrice"|"Timeslot"|"ClientVersion"}
+	{"ChainId"|"BlockNumber"|"GasPrice"|("Timeslot")|"ClientVersion"}
 ```
 
 <br>
 
 `Chain.GetTransactionInformationByHash(TransactionHash: str) -> dict`：
 
 ```
 根据交易哈希查询该交易的详细回执信息。包括交易哈希、所在区块号、交易索引号、交易状态、交易类型、交易行为、发送者、接收者、(部署的合约地址)、(GasPrice 或 (MaxFeePerGas 和 MaxPriorityFeePerGas))、GasLimit、GasUsed、Nonce、Value、R、S、V、Logs、InputData。
 
 参数：
 	TransactionHash (str): 要查询的交易的哈希
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典。当出现异常时返回 None 。
-	{"TransactionHash"|"BlockNumber"|"TransactionIndex"|"Status"|"Type"|"Action"|"From"|"To"|("ContractAddress")|<"GasPrice"|"MaxPriorityFeePerGas")>|"GasLimit"|"GasUsed"|"Nonce"|"Value"|"R"|"S"|"V"|"RawTransaction"|"Logs"|"InputData"}
+	{"TransactionHash"|"BlockNumber"|"TransactionIndex"|"Status"|"Type"|"Action"|"From"|"To"|("ContractAddress")|<"GasPrice"|("MaxFeePerGas"&"MaxPriorityFeePerGas")>|"GasLimit"|"GasUsed"|"Nonce"|"Value"|"R"|"S"|"V"|"Logs"|"InputData"}
 ```
 
 <br>
 
 `Chain.GetTransactionInformationByBlockIdAndIndex(BlockID: Union[str,int], TransactionIndex: int) -> dict`：
 
 ```
@@ -135,59 +151,59 @@
 ```
 根据账户地址获取其网络原生代币余额。
 
 参数：
 	Address (str): 账户地址
 
 返回值：
-	Balance (int): 账户网络原生代币余额。单位为 wei ，当出现异常时返回 None 。
+	Balance (int): 账户网络原生代币余额，单位为 wei 。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Chain.GetCode(Address: str) -> str`：
 
 ```
 根据合约地址获取其已部署字节码。
 
 参数：
 	Address (str): 合约地址
 
 返回值：
-	Code (str): 合约已部署字节码。含 0x 前缀的十六进制形式，当出现异常时返回 None 。
+	Code (str): 合约已部署字节码。当出现异常时返回 None 。
 ```
 
 <br>
 
-`Chain.GetStorage(Address: str, Index: int) -> str`：
+`Chain.GetStorage(Address: str, SlotIndex: int) -> str`：
 
 ```
 根据合约地址和存储插槽索引获取存储值。
 
 参数：
 	Address (str): 合约地址
 	SlotIndex (int): 存储插槽索引
 
 返回值：
-	Data (str): 存储值。含 0x 前缀的十六进制形式，当出现异常时返回 None 。
+	Data (str): 存储值。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Chain.DumpStorage(Address: str, Count: int) -> list`：
 
 ```
 根据合约地址和指定插槽数量值，从插槽 0 开始批量遍历存储插槽并获取值。
 
 参数：
 	Address (str): 合约地址
 	Count (int): 指定插槽数量值
 
 返回值：
-	Data (List[str]): 存储值列表。含 0x 前缀的十六进制形式，当出现异常时返回 None 。
+	Data (List[str]): 存储值列表。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Chain.GetPublicKeyByTransactionHash(TransactionHash: str) -> tuple`：
 
 ```
@@ -209,55 +225,55 @@
 `Account(Chain: Chain, PrivateKey: str)`：
 
 ```
 初始化。通过私钥导入账户并与 Chain 实例绑定，后续的交易将经由该指定账户发送至链上。当导入账户失败时将会抛出异常。
 
 参数：
 	Chain (Poseidon.Blockchain.Chain): 区块链实例
-	PrivateKey (str): 账户私钥。不含 0x 前缀的十六进制形式。
+	PrivateKey (str): 账户私钥。
 
 成员变量：
 	EthAccount (eth_account.Account): eth_account 的原生 Account 对象实例
 ```
 
 <br>
 
 `Account.RequestAuthorizationBeforeSendTransaction(Open: bool = True)`：
 
 ```
-设置在通过该账户发送每一笔交易之前是否请求授权。开启后会在每笔交易即将发送前暂停流程，在终端询问是否发送该笔交易。在实例化 Account 对象时默认设置为 False 。
+设置在通过该账户发送每一笔交易之前是否请求授权。开启后会在每笔交易即将发送前暂停流程，在终端询问是否发送该笔交易。
 
 参数：
-	Open (bool): 请求授权开关。函数定义的默认值为 True ，但在实例化 Account 对象时默认设置为 False 。
+	Open (bool): 请求授权开关。主动调用时默认值为 True ，但在 Account 实例初始化时默认设置为 False 。
 ```
 
 <br>
 
 `Account.GetSelfBalance() -> int`：
 
 ```
 获取自身账户的网络原生代币余额。
 
 返回值：
-	Balance (int): 自身账户网络原生代币余额。单位为 wei ，当出现异常时返回 None 。
+	Balance (int): 自身账户网络原生代币余额，单位为 wei 。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Account.Transfer(To: str, Value: int, Data: str = "0x", GasPrice: Optional[int] = None, GasLimit: int = 100000) -> dict`：
 
 ```
 向指定账户转账指定数量的网络原生代币，可附带信息。若 120 秒内交易未确认则作超时处理。
 
 参数：
 	To (str): 接收方地址
-	Value (int): 发送的网络原生代币数量。单位为 wei 。
-	Data (可选)(str): 交易数据。含 0x 前缀的十六进制形式，默认值为 "0x" 。
-	GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 100000 wei 。
+	Value (int): 发送的网络原生代币数量，单位为 wei 。
+	Data (可选)(str): 交易数据。含 0x 前缀的十六进制形式。默认值为 "0x" 。
+	GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 100000 wei 。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
 <br>
 
@@ -265,17 +281,17 @@
 
 ```
 以传统方式发送一笔自定义交易。若 120 秒内交易未确认则作超时处理。
 
 参数：
 	To (str): 接收方地址
 	Data (str): 交易数据。含 0x 前缀的十六进制形式。
-	Value (可选)(int): 随交易发送的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-	GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 1000000 wei 。
+	Value (可选)(int): 随交易发送的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+	GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 1000000 wei 。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
 <br>
 
@@ -283,54 +299,54 @@
 
 ```
 以 EIP-1559 方式发送一笔自定义交易。若 120 秒内交易未确认则作超时处理。
 
 参数：
 	To (str): 接收方地址
 	Data (str): 交易数据。含 0x 前缀的十六进制形式。
-	Value (可选)(int): 随交易发送的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-	BaseFee (可选)(Optional[int]): BaseFee 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	MaxPriorityFee (可选)(Optional[int]): MaxPriorityFee 价格。单位为 wei ，默认使用 RPC 建议的 max_priority_fee 。
-	GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 1000000 wei 。
+	Value (可选)(int): 随交易发送的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+	BaseFee (可选)(Optional[int]): BaseFee 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	MaxPriorityFee (可选)(Optional[int]): MaxPriorityFee 价格，单位为 wei ，默认使用 RPC 建议的 max_priority_fee 。
+	GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 1000000 wei 。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Account.DeployContract(ABI: dict, Bytecode: str, Value: int = 0, GasPrice: Optional[int] = None, *Arguments: Optional[Any]) -> dict`：
 
 ```
 部署合约。若 120 秒内交易未确认则作超时处理。
 
 参数：
 	ABI (dict): 合约 ABI
-	Bytecode (str): 合约部署字节码。含 0x 前缀的十六进制形式。
-	Value (可选)(int): 随交易发送给合约的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-	GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	Bytecode (str): 合约部署字节码。
+	Value (可选)(int): 随交易发送给合约的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+	GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
 	*Arguments (可选)(Optional[Any]): 传给合约构造函数的参数，默认为空。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
-	当合约部署成功时，字典中会额外添加"Contract"字段，该变量是已实例化的 Contract 对象，失败时为 None。
+	当合约部署成功时，字典中会额外添加"Contract"字段，该变量是已实例化的 Contract 对象，若失败则为 None。
 ```
 
 <br>
 
 `Account.DeployContractWithoutABI(Bytecode: str, Value: int = 0, GasPrice: Optional[int] = None, GasLimit: int = 5000000) -> dict`：
 
 ```
 在没有 ABI 的情况下，仅使用字节码来部署合约。若 120 秒内交易未确认则作超时处理。
 
 参数：
-	Bytecode (str): 合约部署字节码。含 0x 前缀的十六进制形式。
-	Value (可选)(int): 随交易发送给合约的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-	GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 5000000 wei 。
+	Bytecode (str): 合约部署字节码。
+	Value (可选)(int): 随交易发送给合约的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+	GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 5000000 wei 。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
 <br>
 
@@ -402,17 +418,17 @@
 
 `Contract.CallFunctionWithParameters(Value: int, GasPrice: Optional[int], GasLimit: int, FunctionName: str, *FunctionArguments: Optional[Any]) -> dict`：
 
 ```
 通过传入函数名及参数来调用该合约内的函数。支持自定义 Value 和 GasLimit 。
 
 参数：
-	Value (int): 随交易发送的网络原生代币数量。单位为 wei 。
-	GasPrice (Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	GasLimit (int): Gas 最大使用量。单位为 wei 。
+	Value (int): 随交易发送的网络原生代币数量，单位为 wei 。
+	GasPrice (Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	GasLimit (int): Gas 最大使用量，单位为 wei 。
 	FunctionName (str): 函数名称
 	*FunctionArguments (Optional[Any]): 函数参数，默认为空。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
@@ -444,14 +460,28 @@
 
 返回值：
 	CallData (str): 调用数据编码。含 0x 前缀的十六进制形式。当出现异常时返回 None 。
 ```
 
 <br>
 
+`Contract.DecodeFunctionInputData(InputData: str) -> tuple`：
+
+```
+解码对当前合约执行调用的 InputData ，得出所调用的函数及其参数值。
+
+参数：
+	InputData (str): 对当前合约执行调用的 InputData
+
+返回值：
+	Result (tuple): 函数及其参数值
+```
+
+<br>
+
 ### BlockchainUtils 类
 
 通用工具集，整合了常用的链下操作。静态类，无需实例化。
 
 `BlockchainUtils.SwitchSolidityVersion(SolidityVersion: str)`：
 
 ```
@@ -567,19 +597,19 @@
 
 ```
 将 R S V 合并成签名。
 
 参数：
 	R (str): 签名 r 值。含 0x 前缀的十六进制形式。
 	S (str): 签名 s 值。含 0x 前缀的十六进制形式。
-	V (int): 签名 v 值。十进制数字。
+	V (int): 签名 v 值。含 0x 前缀的十六进制形式。
 
 返回值：
 	Result (dict): 合并结果。当出现异常时返回 None 。
-	{"R"|"S"|"V"|"Signature"}
+	{"Signature"|"R"|"S"|"V"}
 ```
 
 <br>
 
 `BlockchainUtils.GetFunctionSelector(FunctionName: str, FunctionParameters: Optional[List[str]] = None) -> str`：
 
 ```
@@ -651,14 +681,45 @@
 
 返回值：
 	ToGenerateFunction (str): 碰撞出的函数的名称与参数完整表示。当出现异常时返回 None 。
 ```
 
 <br>
 
+`BlockchainUtils.GetContractAddressByCREATE(Deployer: str, Nonce: int) -> str`：
+
+```
+获取某账户以 CREATE 方式部署的合约的地址。
+
+参数：
+	Deployer (str): 部署者地址
+	Nonce (int): 部署者发送合约部署交易的 nonce 值
+
+返回值：
+	Address (str): 计算出的合约地址
+```
+
+<br>
+
+`BlockchainUtils.GetContractAddressByCREATE2(Deployer: str, Salt: str, CreationCode: str) -> str`：
+
+```
+获取某合约账户以 CREATE2 方式部署的另一个合约的地址。
+
+参数：
+	Deployer (str): 部署者地址
+	Salt (str): 盐值
+	CreationCode (str): 合约的创建时字节码
+
+返回值：
+	Address (str): 计算出的合约地址
+```
+
+<br>
+
 ## Cryptography 模块
 
 本模块用于解决常见的密码学问题。
 
 ```python
 from Poseidon.Cryptography import ModernCryptoUtils, ClassicalCryptoUtils, MiscUtils
 ```
```

### Comparing `poseidon-python-1.1.4/poseidon_python.egg-info/PKG-INFO` & `poseidon-python-1.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,32 @@
-Metadata-Version: 2.1
-Name: poseidon-python
-Version: 1.1.4
-Summary: 海神波塞冬工具对常用的链上交互操作进行了封装，使得开发者能够便捷地与任何以太坊同构链交互，主要用于在CTF比赛中攻克Blockchain方向的题目。
-Home-page: https://github.com/B1ue1nWh1te/Poseidon
-Author: B1ue1nWh1te
-Author-email: b1ue1nwh1te@skiff.com
-License: GPL-3.0
-Keywords: POSEIDON,BLOCKCHAIN,EVM,CRYPTO,CTF
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 
 # Poseidon
 
-![data](https://socialify.git.ci/B1ue1nWh1te/Poseidon/image?font=Rokkitt&forks=1&issues=1&language=1&logo=https%3A%2F%2Fimg.seaeye.cn%2Fimg%2Fseaeye%2Flogo.png&owner=1&pattern=Circuit%20Board&stargazers=1&theme=Light)
+![data](https://socialify.git.ci/B1ue1nWh1te/Poseidon/image?font=Rokkitt&forks=1&issues=1&language=1&logo=https%3A%2F%2Fimg.seaeye.cn%2Fimg%2Fseaverse%2Flogo.png&owner=1&pattern=Circuit%20Board&stargazers=1&theme=Light)
 
 **海神波塞冬 Poseidon** 工具对常用的链上交互操作进行了封装，使得开发者能够便捷地
 
 与任何以太坊同构链交互，主要用于在 CTF 比赛中攻克 Blockchain 方向的题目。
 
 [![Lisence](https://img.shields.io/github/license/B1ue1nWh1te/Poseidon)](https://github.com/B1ue1nWh1te/Poseidon/blob/main/LICENSE)
-[![Python Version](https://img.shields.io/badge/python-3.8+-blue)](https://www.python.org/)
+[![Python](https://img.shields.io/badge/python-3.9+-blue)](https://www.python.org/)
 [![Release](https://img.shields.io/github/v/release/B1ue1nWh1te/Poseidon?include_prereleases)](https://github.com/B1ue1nWh1te/Poseidon/releases/)
 [![Visitors](https://visitor-badge.glitch.me/badge?page_id=B1ue1nWh1te-Poseidon&left_color=gray&right_color=orange)](https://github.com/B1ue1nWh1te/Poseidon)
-![Downloads](https://img.shields.io/pypi/dm/poseidon-python)
+![Downloads](https://img.shields.io/pypi/dd/poseidon-python)
 
 </div>
 
 # 注意事项
 
 1. **本工具原则上仅可用于 CTF 比赛解题或测试链开发。但开源工具无法约束使用场景，若执意要在具有经济价值的公链中使用，所产生的影响将由你自行承担。**
 
 2. 在使用 `Blockchain` 模块时，你始终应该使用全新生成的账户，而不是导入常用的具有实际价值的账户，以确保你的账户安全。
 
-3. `Blockchain` 模块的所有功能在 `Goerli` 测试网络中均正常通过检验。
+3. `Blockchain` 模块的所有功能在 `Goerli, Sepolia` 测试网络中均正常通过检验。
 
 4. 如果你在使用过程中遇到了其他问题，或者有任何好的想法和建议，欢迎提[issue](https://github.com/B1ue1nWh1te/Poseidon/issues)进行反馈。
 
 # 安装
 
 ```bash
 pip install -U poseidon-python
@@ -66,52 +53,55 @@
 ### Chain 类
 
 Chain 是区块链实例，后续的所有链上交互的操作都将经由该指定节点处理。
 
 `Chain(RPCUrl: str, RequestParams: Optional[dict] = None)`：
 
 ```
-初始化。根据给定的节点 RPC 地址进行连接，可通过代理访问。当连接节点失败时会抛出异常。
+初始化。根据给定的节点 RPC 地址以 HTTP/HTTPS 方式进行连接，可通过代理访问。当连接节点失败时会抛出异常。
 
 参数：
 	RPCUrl (str): 节点 RPC 地址
 	RequestParams (可选)(Optional[dict]): 连接时使用的 request 参数，默认为 None。
 	例如当需要使用代理进行访问时，则传入 RequestParams={"proxies": {"http": "http://localhost:<ProxyPort>","https": "http://localhost:<ProxyPort>"}}
 
 成员变量：
 	ChainId (int): 链 ID
 	Node (Web3.HTTPProvider): web3.py 原生的 HTTP 交互器实例
 	Eth (Web3.HTTPProvider.eth): HTTP 交互器实例中的 eth 模块
 ```
 
 <br>
 
-`Chain.GetBasicInformation() -> dict`：
+`Chain.GetBasicInformation(ShowTimeslot: bool = True) -> dict`：
 
 ```
-获取区块链基本信息。包括链 ID 、区块高度、 GasPrice 、出块间隔、当前节点的客户端软件版本号。
+获取区块链基本信息。包括 ChainId 、BlockNumber 、GasPrice 、(Timeslot)、ClientVersion 。
+
+参数：
+	ShowTimeslot (bool): 是否获取并显示 Timeslot 。该操作比较耗时，在主动调用时默认为 True , 在 Chain 实例初始化时默认为 False 。
 
 返回值：
 	BasicInformation (dict): 区块链基本信息构成的字典。
-	{"ChainId"|"BlockNumber"|"GasPrice"|"Timeslot"|"ClientVersion"}
+	{"ChainId"|"BlockNumber"|"GasPrice"|("Timeslot")|"ClientVersion"}
 ```
 
 <br>
 
 `Chain.GetTransactionInformationByHash(TransactionHash: str) -> dict`：
 
 ```
 根据交易哈希查询该交易的详细回执信息。包括交易哈希、所在区块号、交易索引号、交易状态、交易类型、交易行为、发送者、接收者、(部署的合约地址)、(GasPrice 或 (MaxFeePerGas 和 MaxPriorityFeePerGas))、GasLimit、GasUsed、Nonce、Value、R、S、V、Logs、InputData。
 
 参数：
 	TransactionHash (str): 要查询的交易的哈希
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典。当出现异常时返回 None 。
-	{"TransactionHash"|"BlockNumber"|"TransactionIndex"|"Status"|"Type"|"Action"|"From"|"To"|("ContractAddress")|<"GasPrice"|"MaxPriorityFeePerGas")>|"GasLimit"|"GasUsed"|"Nonce"|"Value"|"R"|"S"|"V"|"RawTransaction"|"Logs"|"InputData"}
+	{"TransactionHash"|"BlockNumber"|"TransactionIndex"|"Status"|"Type"|"Action"|"From"|"To"|("ContractAddress")|<"GasPrice"|("MaxFeePerGas"&"MaxPriorityFeePerGas")>|"GasLimit"|"GasUsed"|"Nonce"|"Value"|"R"|"S"|"V"|"Logs"|"InputData"}
 ```
 
 <br>
 
 `Chain.GetTransactionInformationByBlockIdAndIndex(BlockID: Union[str,int], TransactionIndex: int) -> dict`：
 
 ```
@@ -148,59 +138,59 @@
 ```
 根据账户地址获取其网络原生代币余额。
 
 参数：
 	Address (str): 账户地址
 
 返回值：
-	Balance (int): 账户网络原生代币余额。单位为 wei ，当出现异常时返回 None 。
+	Balance (int): 账户网络原生代币余额，单位为 wei 。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Chain.GetCode(Address: str) -> str`：
 
 ```
 根据合约地址获取其已部署字节码。
 
 参数：
 	Address (str): 合约地址
 
 返回值：
-	Code (str): 合约已部署字节码。含 0x 前缀的十六进制形式，当出现异常时返回 None 。
+	Code (str): 合约已部署字节码。当出现异常时返回 None 。
 ```
 
 <br>
 
-`Chain.GetStorage(Address: str, Index: int) -> str`：
+`Chain.GetStorage(Address: str, SlotIndex: int) -> str`：
 
 ```
 根据合约地址和存储插槽索引获取存储值。
 
 参数：
 	Address (str): 合约地址
 	SlotIndex (int): 存储插槽索引
 
 返回值：
-	Data (str): 存储值。含 0x 前缀的十六进制形式，当出现异常时返回 None 。
+	Data (str): 存储值。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Chain.DumpStorage(Address: str, Count: int) -> list`：
 
 ```
 根据合约地址和指定插槽数量值，从插槽 0 开始批量遍历存储插槽并获取值。
 
 参数：
 	Address (str): 合约地址
 	Count (int): 指定插槽数量值
 
 返回值：
-	Data (List[str]): 存储值列表。含 0x 前缀的十六进制形式，当出现异常时返回 None 。
+	Data (List[str]): 存储值列表。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Chain.GetPublicKeyByTransactionHash(TransactionHash: str) -> tuple`：
 
 ```
@@ -222,55 +212,55 @@
 `Account(Chain: Chain, PrivateKey: str)`：
 
 ```
 初始化。通过私钥导入账户并与 Chain 实例绑定，后续的交易将经由该指定账户发送至链上。当导入账户失败时将会抛出异常。
 
 参数：
 	Chain (Poseidon.Blockchain.Chain): 区块链实例
-	PrivateKey (str): 账户私钥。不含 0x 前缀的十六进制形式。
+	PrivateKey (str): 账户私钥。
 
 成员变量：
 	EthAccount (eth_account.Account): eth_account 的原生 Account 对象实例
 ```
 
 <br>
 
 `Account.RequestAuthorizationBeforeSendTransaction(Open: bool = True)`：
 
 ```
-设置在通过该账户发送每一笔交易之前是否请求授权。开启后会在每笔交易即将发送前暂停流程，在终端询问是否发送该笔交易。在实例化 Account 对象时默认设置为 False 。
+设置在通过该账户发送每一笔交易之前是否请求授权。开启后会在每笔交易即将发送前暂停流程，在终端询问是否发送该笔交易。
 
 参数：
-	Open (bool): 请求授权开关。函数定义的默认值为 True ，但在实例化 Account 对象时默认设置为 False 。
+	Open (bool): 请求授权开关。主动调用时默认值为 True ，但在 Account 实例初始化时默认设置为 False 。
 ```
 
 <br>
 
 `Account.GetSelfBalance() -> int`：
 
 ```
 获取自身账户的网络原生代币余额。
 
 返回值：
-	Balance (int): 自身账户网络原生代币余额。单位为 wei ，当出现异常时返回 None 。
+	Balance (int): 自身账户网络原生代币余额，单位为 wei 。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Account.Transfer(To: str, Value: int, Data: str = "0x", GasPrice: Optional[int] = None, GasLimit: int = 100000) -> dict`：
 
 ```
 向指定账户转账指定数量的网络原生代币，可附带信息。若 120 秒内交易未确认则作超时处理。
 
 参数：
 	To (str): 接收方地址
-	Value (int): 发送的网络原生代币数量。单位为 wei 。
-	Data (可选)(str): 交易数据。含 0x 前缀的十六进制形式，默认值为 "0x" 。
-	GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 100000 wei 。
+	Value (int): 发送的网络原生代币数量，单位为 wei 。
+	Data (可选)(str): 交易数据。含 0x 前缀的十六进制形式。默认值为 "0x" 。
+	GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 100000 wei 。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
 <br>
 
@@ -278,17 +268,17 @@
 
 ```
 以传统方式发送一笔自定义交易。若 120 秒内交易未确认则作超时处理。
 
 参数：
 	To (str): 接收方地址
 	Data (str): 交易数据。含 0x 前缀的十六进制形式。
-	Value (可选)(int): 随交易发送的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-	GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 1000000 wei 。
+	Value (可选)(int): 随交易发送的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+	GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 1000000 wei 。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
 <br>
 
@@ -296,54 +286,54 @@
 
 ```
 以 EIP-1559 方式发送一笔自定义交易。若 120 秒内交易未确认则作超时处理。
 
 参数：
 	To (str): 接收方地址
 	Data (str): 交易数据。含 0x 前缀的十六进制形式。
-	Value (可选)(int): 随交易发送的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-	BaseFee (可选)(Optional[int]): BaseFee 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	MaxPriorityFee (可选)(Optional[int]): MaxPriorityFee 价格。单位为 wei ，默认使用 RPC 建议的 max_priority_fee 。
-	GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 1000000 wei 。
+	Value (可选)(int): 随交易发送的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+	BaseFee (可选)(Optional[int]): BaseFee 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	MaxPriorityFee (可选)(Optional[int]): MaxPriorityFee 价格，单位为 wei ，默认使用 RPC 建议的 max_priority_fee 。
+	GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 1000000 wei 。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
 <br>
 
 `Account.DeployContract(ABI: dict, Bytecode: str, Value: int = 0, GasPrice: Optional[int] = None, *Arguments: Optional[Any]) -> dict`：
 
 ```
 部署合约。若 120 秒内交易未确认则作超时处理。
 
 参数：
 	ABI (dict): 合约 ABI
-	Bytecode (str): 合约部署字节码。含 0x 前缀的十六进制形式。
-	Value (可选)(int): 随交易发送给合约的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-	GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	Bytecode (str): 合约部署字节码。
+	Value (可选)(int): 随交易发送给合约的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+	GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
 	*Arguments (可选)(Optional[Any]): 传给合约构造函数的参数，默认为空。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
-	当合约部署成功时，字典中会额外添加"Contract"字段，该变量是已实例化的 Contract 对象，失败时为 None。
+	当合约部署成功时，字典中会额外添加"Contract"字段，该变量是已实例化的 Contract 对象，若失败则为 None。
 ```
 
 <br>
 
 `Account.DeployContractWithoutABI(Bytecode: str, Value: int = 0, GasPrice: Optional[int] = None, GasLimit: int = 5000000) -> dict`：
 
 ```
 在没有 ABI 的情况下，仅使用字节码来部署合约。若 120 秒内交易未确认则作超时处理。
 
 参数：
-	Bytecode (str): 合约部署字节码。含 0x 前缀的十六进制形式。
-	Value (可选)(int): 随交易发送给合约的网络原生代币数量。单位为 wei ，默认为 0 wei 。
-	GasPrice (可选)(Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	GasLimit (可选)(int): Gas 最大使用量。单位为 wei ，默认为 5000000 wei 。
+	Bytecode (str): 合约部署字节码。
+	Value (可选)(int): 随交易发送给合约的网络原生代币数量，单位为 wei ，默认为 0 wei 。
+	GasPrice (可选)(Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	GasLimit (可选)(int): Gas 最大使用量，单位为 wei ，默认为 5000000 wei 。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
 <br>
 
@@ -415,17 +405,17 @@
 
 `Contract.CallFunctionWithParameters(Value: int, GasPrice: Optional[int], GasLimit: int, FunctionName: str, *FunctionArguments: Optional[Any]) -> dict`：
 
 ```
 通过传入函数名及参数来调用该合约内的函数。支持自定义 Value 和 GasLimit 。
 
 参数：
-	Value (int): 随交易发送的网络原生代币数量。单位为 wei 。
-	GasPrice (Optional[int]): Gas 价格。单位为 wei ，默认使用 RPC 建议的 gas_price 。
-	GasLimit (int): Gas 最大使用量。单位为 wei 。
+	Value (int): 随交易发送的网络原生代币数量，单位为 wei 。
+	GasPrice (Optional[int]): Gas 价格，单位为 wei ，默认使用 RPC 建议的 gas_price 。
+	GasLimit (int): Gas 最大使用量，单位为 wei 。
 	FunctionName (str): 函数名称
 	*FunctionArguments (Optional[Any]): 函数参数，默认为空。
 
 返回值：
 	TransactionInformation (dict): 交易信息构成的字典，通过 Chain.GetTransactionInformationByHash 获取。当出现异常时返回 None 。
 ```
 
@@ -457,14 +447,28 @@
 
 返回值：
 	CallData (str): 调用数据编码。含 0x 前缀的十六进制形式。当出现异常时返回 None 。
 ```
 
 <br>
 
+`Contract.DecodeFunctionInputData(InputData: str) -> tuple`：
+
+```
+解码对当前合约执行调用的 InputData ，得出所调用的函数及其参数值。
+
+参数：
+	InputData (str): 对当前合约执行调用的 InputData
+
+返回值：
+	Result (tuple): 函数及其参数值
+```
+
+<br>
+
 ### BlockchainUtils 类
 
 通用工具集，整合了常用的链下操作。静态类，无需实例化。
 
 `BlockchainUtils.SwitchSolidityVersion(SolidityVersion: str)`：
 
 ```
@@ -580,19 +584,19 @@
 
 ```
 将 R S V 合并成签名。
 
 参数：
 	R (str): 签名 r 值。含 0x 前缀的十六进制形式。
 	S (str): 签名 s 值。含 0x 前缀的十六进制形式。
-	V (int): 签名 v 值。十进制数字。
+	V (int): 签名 v 值。含 0x 前缀的十六进制形式。
 
 返回值：
 	Result (dict): 合并结果。当出现异常时返回 None 。
-	{"R"|"S"|"V"|"Signature"}
+	{"Signature"|"R"|"S"|"V"}
 ```
 
 <br>
 
 `BlockchainUtils.GetFunctionSelector(FunctionName: str, FunctionParameters: Optional[List[str]] = None) -> str`：
 
 ```
@@ -664,14 +668,45 @@
 
 返回值：
 	ToGenerateFunction (str): 碰撞出的函数的名称与参数完整表示。当出现异常时返回 None 。
 ```
 
 <br>
 
+`BlockchainUtils.GetContractAddressByCREATE(Deployer: str, Nonce: int) -> str`：
+
+```
+获取某账户以 CREATE 方式部署的合约的地址。
+
+参数：
+	Deployer (str): 部署者地址
+	Nonce (int): 部署者发送合约部署交易的 nonce 值
+
+返回值：
+	Address (str): 计算出的合约地址
+```
+
+<br>
+
+`BlockchainUtils.GetContractAddressByCREATE2(Deployer: str, Salt: str, CreationCode: str) -> str`：
+
+```
+获取某合约账户以 CREATE2 方式部署的另一个合约的地址。
+
+参数：
+	Deployer (str): 部署者地址
+	Salt (str): 盐值
+	CreationCode (str): 合约的创建时字节码
+
+返回值：
+	Address (str): 计算出的合约地址
+```
+
+<br>
+
 ## Cryptography 模块
 
 本模块用于解决常见的密码学问题。
 
 ```python
 from Poseidon.Cryptography import ModernCryptoUtils, ClassicalCryptoUtils, MiscUtils
 ```
```

### Comparing `poseidon-python-1.1.4/setup.py` & `poseidon-python-1.1.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 def long_description():
     with open(os.path.join(os.path.dirname(os.path.realpath(__file__)), 'README.md'), encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name="poseidon-python",
-    version="1.1.4",
+    version="1.1.5",
     author="B1ue1nWh1te",
     author_email="b1ue1nwh1te@skiff.com",
-    description="海神波塞冬工具对常用的链上交互操作进行了封装，使得开发者能够便捷地与任何以太坊同构链交互，主要用于在CTF比赛中攻克Blockchain方向的题目。",
+    description="海神波塞冬工具对常用的链上交互操作进行了封装，使得开发者能够便捷地与任何以太坊同构链交互，主要用于在 CTF 比赛中攻克 Blockchain 方向的题目。",
     keywords=['POSEIDON', 'BLOCKCHAIN', 'EVM', 'CRYPTO', 'CTF'],
     long_description=long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/B1ue1nWh1te/Poseidon",
     license="GPL-3.0",
     packages=["Poseidon"],
     python_requires='>=3.9',
-    install_requires=["web3", "py-solc-x", "pyevmasm", "loguru", "pycryptodome", "gmpy2", "pwntools"],
+    install_requires=["web3>=6.2.0", "py-solc-x>=1.1.1", "pyevmasm>=0.2.3", "loguru>=0.7.0", "pycryptodome>=3.17", "gmpy2>=2.1.5", "pwntools>=4.9.0"],
     zip_safe=False
 )
```

