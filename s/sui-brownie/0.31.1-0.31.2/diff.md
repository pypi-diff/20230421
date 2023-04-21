# Comparing `tmp/sui_brownie-0.31.1-py3-none-any.whl.zip` & `tmp/sui_brownie-0.31.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 27336 bytes, number of entries: 16
+Zip file size: 27601 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       10 b- defN 22-Dec-02 09:41 sui_brownie/MANIFEST.in
 -rw-r--r--  2.0 unx      878 b- defN 23-Apr-01 13:03 sui_brownie/README.md
 -rw-r--r--  2.0 unx       38 b- defN 23-Apr-11 02:45 sui_brownie/__init__.py
 -rw-r--r--  2.0 unx     2514 b- defN 23-Apr-01 12:52 sui_brownie/account.py
 -rw-r--r--  2.0 unx    12144 b- defN 23-Apr-01 10:43 sui_brownie/bcs.py
 -rw-r--r--  2.0 unx     4326 b- defN 23-Apr-01 12:53 sui_brownie/ed25519.py
 -rw-r--r--  2.0 unx    10047 b- defN 22-Dec-02 09:41 sui_brownie/parallelism.py
--rw-r--r--  2.0 unx    86180 b- defN 23-Apr-18 07:14 sui_brownie/sui_brownie.py
--rw-r--r--  2.0 unx    32439 b- defN 23-Apr-11 02:45 sui_brownie/sui_client.py
+-rw-r--r--  2.0 unx    91104 b- defN 23-Apr-21 07:49 sui_brownie/sui_brownie.py
+-rw-r--r--  2.0 unx    32439 b- defN 23-Apr-19 08:03 sui_brownie/sui_client.py
 -rw-r--r--  2.0 unx      140 b- defN 22-Dec-02 09:41 sui_brownie/sui_config.template.yaml
 -rw-r--r--  2.0 unx       19 b- defN 22-Dec-02 09:41 sui_brownie/sui_keystore.template.keystore
 -rw-r--r--  2.0 unx      866 b- defN 23-Apr-11 02:45 sui_brownie/utils.py
--rw-r--r--  2.0 unx      983 b- defN 23-Apr-18 07:23 sui_brownie-0.31.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 07:23 sui_brownie-0.31.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-18 07:23 sui_brownie-0.31.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1300 b- defN 23-Apr-18 07:23 sui_brownie-0.31.1.dist-info/RECORD
-16 files, 151988 bytes uncompressed, 25194 bytes compressed:  83.4%
+-rw-r--r--  2.0 unx      983 b- defN 23-Apr-21 07:51 sui_brownie-0.31.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 07:51 sui_brownie-0.31.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-21 07:51 sui_brownie-0.31.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1300 b- defN 23-Apr-21 07:51 sui_brownie-0.31.2.dist-info/RECORD
+16 files, 156912 bytes uncompressed, 25459 bytes compressed:  83.8%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sui_brownie/sui_keystore.template.keystore
 Comment: 
 
 Filename: sui_brownie/utils.py
 Comment: 
 
-Filename: sui_brownie-0.31.1.dist-info/METADATA
+Filename: sui_brownie-0.31.2.dist-info/METADATA
 Comment: 
 
-Filename: sui_brownie-0.31.1.dist-info/WHEEL
+Filename: sui_brownie-0.31.2.dist-info/WHEEL
 Comment: 
 
-Filename: sui_brownie-0.31.1.dist-info/top_level.txt
+Filename: sui_brownie-0.31.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sui_brownie-0.31.1.dist-info/RECORD
+Filename: sui_brownie-0.31.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sui_brownie/sui_brownie.py

```diff
@@ -1295,18 +1295,20 @@
         if isinstance(data, dict):
             self.format_dict(data)
         return data
 
     @retry(stop_max_attempt_number=3, wait_random_min=500, wait_random_max=1000)
     def publish_package(
             self,
-            gas_budget=100000000,
+            gas_budget=None,
             replace_address: dict = None,
             skip_dependency_verification=True
     ):
+        if gas_budget is None:
+            gas_budget = self.project.gas_budget
         replace_tomls = self.replace_addresses(replace_address=replace_address, output=dict())
         view = f"Publish {self.package_name}"
         print("\n" + "-" * 50 + view + "-" * 50)
         try:
             with self.project.cli_config as cof:
                 skip_flag = " --skip-dependency-verification" if skip_dependency_verification else ""
                 cmd = f"sui client --client.config {cof.file.absolute()} publish " \
@@ -1339,17 +1341,21 @@
             traceback.print_exc()
             raise
         return result
 
     def program_publish_package(
             self,
             replace_address: dict = None,
-            gas_price=1000,
-            gas_budget=100000000,
+            gas_price=None,
+            gas_budget=None,
     ):
+        if gas_budget is None:
+            gas_budget = self.project.gas_budget
+        if gas_price is None:
+            gas_price = self.project.estimate_gas_price()
         replace_tomls = self.replace_addresses(replace_address=replace_address, output=dict())
         try:
             cmd = f"sui move build --dump-bytecode-as-base64 --path {self.package_path.absolute()}"
             with os.popen(cmd) as f:
                 result = f.read()
             try:
                 result = json.loads(result[result.find("{"):])
@@ -1384,17 +1390,21 @@
         return result
 
     def program_upgrade_package(
             self,
             upgrade_capability: str,
             upgrade_policy: int,
             replace_address: dict = None,
-            gas_price=1000,
-            gas_budget=100000000,
+            gas_price=None,
+            gas_budget=None,
     ):
+        if gas_budget is None:
+            gas_budget = self.project.gas_budget
+        if gas_price is None:
+            gas_price = self.project.estimate_gas_price()
         replace_tomls = self.replace_addresses(replace_address=replace_address, output=dict())
         try:
             cmd = f"sui move build --dump-bytecode-as-base64 --dump-package-digest " \
                   f"--path {self.package_path.absolute()}"
             with os.popen(cmd) as f:
                 result = f.read()
             try:
@@ -1453,17 +1463,21 @@
     def program_dola_upgrade_package(
             self,
             proposal_package_id,
             governance_info: str,
             governance_contracts: str,
             proposal: str,
             replace_address: dict = None,
-            gas_price=1000,
-            gas_budget=100000000,
+            gas_price=None,
+            gas_budget=None,
     ):
+        if gas_budget is None:
+            gas_budget = self.project.gas_budget
+        if gas_price is None:
+            gas_price = self.project.estimate_gas_price()
         replace_tomls = self.replace_addresses(replace_address=replace_address, output=dict())
         try:
             cmd = f"sui move build --dump-bytecode-as-base64 --dump-package-digest " \
                   f"--path {self.package_path.absolute()}"
             with os.popen(cmd) as f:
                 result = f.read()
             try:
@@ -1512,14 +1526,15 @@
     def __init__(
             self,
             project_path: Union[Path, str] = Path.cwd(),
             network: str = "sui-testnet"
     ):
         self.project_path = project_path
         self.network = network
+        self.gas_budget = 500000000
 
         self.config = {}
         self.network_config = {}
         self.client: SuiClient = None
         self.accounts: Dict[str, Account] = {}
         self.__active_account = None
         self.packages: Dict[str, List[SuiPackage]] = DefaultDict([])
@@ -1533,14 +1548,18 @@
         self.cli_config: SuiCliConfig = None
 
         self.load_config()
         self.reload_cache()
 
         _load_project.append(self)
 
+    def set_gas_budget(self, gas_budget):
+        """Set global gas budget"""
+        self.gas_budget = gas_budget
+
     def read_item_from_cache(self, item: Union[str, SuiObject]):
         if item in self.cache_objects:
             if self.account.account_address in self.cache_objects[item]:
                 return self.cache_objects[item][self.account.account_address]
             elif "Shared" in self.cache_objects[item]:
                 return self.cache_objects[item]["Shared"]
             else:
@@ -1746,25 +1765,27 @@
 
     def unsafe(
             self,
             package_id,
             abi: dict,
             *arguments,
             type_arguments: List[str] = None,
-            gas_budget=100000000,
+            gas_budget=None,
     ):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
         result = self.construct_transaction(
             package_id=package_id,
             abi=abi,
             arguments=arguments,
             type_arguments=type_arguments,
             gas_budget=gas_budget)
-        # Simulate before execute
+
         tx_bytes = result["txBytes"]
-        self.client.sui_dryRunTransactionBlock(tx_bytes)
+        self.simulate_fail_abort(tx_bytes)
 
         # sig
         msg = bytes([IntentScope.TransactionData[1], IntentVersion.V0[1], AppId.Sui[1]]
                     + list(base64.b64decode(tx_bytes)))
         serialized_sig_base64 = self.generate_signature(msg)
 
         # Execute
@@ -1775,30 +1796,33 @@
 
     def execute(
             self,
             package_id,
             abi: dict,
             *arguments,
             type_arguments: List[str] = None,
-            gas_price=1000,
-            gas_budget=100000000,
+            gas_price=None,
+            gas_budget=None,
     ):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
         # Construct
         msg = TransactionBuild.move_call(
             self.account.account_address,
             package_id,
             abi,
             type_arguments,
             arguments,
             gas_price=gas_price,
             gas_budget=gas_budget
         )
-        # simulate
         tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
-        self.client.sui_dryRunTransactionBlock(tx_bytes)
+        self.simulate_fail_abort(tx_bytes)
 
         # Sig
         serialized_sig_base64 = self.generate_signature(msg.encode)
 
         # Execute
         print(f'\nExecute transaction {abi["module_name"]}::{abi["func_name"]}, waiting...')
         return self._execute(tx_bytes, [serialized_sig_base64], module=abi["module_name"], function=abi["func_name"])
@@ -1874,16 +1898,18 @@
 
     def construct_transaction(
             self,
             package_id,
             abi: dict,
             arguments: list,
             type_arguments: List[str] = None,
-            gas_budget=100000000,
+            gas_budget=None,
     ):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
         arguments, type_arguments = TransactionBuild.check_args(abi, arguments, type_arguments)
 
         for k in range(len(arguments)):
             # Process U64, U128, U256
             if abi["parameters"][k] in ["U64", "U128", "U256"]:
                 arguments[k] = str(arguments[k])
 
@@ -1904,38 +1930,51 @@
 
     def simulate(
             self,
             package_id,
             abi: dict,
             *arguments,
             type_arguments: List[str] = None,
-            gas_price=1000,
-            gas_budget=100000000,
+            gas_price=None,
+            gas_budget=None,
     ):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
         msg = TransactionBuild.move_call(
             self.account.account_address,
             package_id,
             abi,
             type_arguments,
             arguments,
             gas_price=gas_price,
             gas_budget=gas_budget
         )
         tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
         return self.client.sui_dryRunTransactionBlock(tx_bytes)
 
+    def simulate_fail_abort(self, tx_bytes):
+        result = self.client.sui_dryRunTransactionBlock(tx_bytes)
+        assert result["effects"]["status"]["status"] == "success", result
+        return result
+
     def inspect(
             self,
             package_id,
             abi: dict,
             *arguments,
             type_arguments: List[str] = None,
-            gas_price=1000,
-            gas_budget=100000000,
+            gas_price=None,
+            gas_budget=None,
     ):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
         msg = TransactionBuild.move_call(
             self.account.account_address,
             package_id,
             abi,
             type_arguments,
             arguments,
             gas_price=gas_price,
@@ -1945,191 +1984,215 @@
         return self.client.sui_devInspectTransactionBlock(
             self.account.account_address,
             tx_bytes,
             None,
             None
         )
 
-    def unsafe_pay_all_sui(self, input_coins=None, recipient=None, gas_budget=100000000):
+    def unsafe_pay_all_sui(self, input_coins=None, recipient=None, gas_budget=None):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
         if recipient is None:
             recipient = self.account.account_address
         if input_coins is None:
             input_coins = list(self.get_account_sui().keys())
         result = self.client.unsafe_payAllSui(self.account.account_address, input_coins, recipient, str(gas_budget))
 
-        # Simulate before execute
         tx_bytes = result["txBytes"]
-        self.client.sui_dryRunTransactionBlock(tx_bytes)
+        self.simulate_fail_abort(tx_bytes)
 
         # sig
         msg = bytes([IntentScope.TransactionData[1], IntentVersion.V0[1], AppId.Sui[1]]
                     + list(base64.b64decode(tx_bytes)))
         serialized_sig_base64 = self.generate_signature(msg)
 
         # Execute
         print(f'\nExecute transaction unsafe::pay_all_sui, waiting...')
         return self._execute(tx_bytes,
                              signatures=[serialized_sig_base64],
                              module="unsafe",
                              function="pay_all_sui"
                              )
 
-    def pay_all_sui(self, input_coins=None, recipient=None, gas_price=1000, gas_budget=100000000):
+    def pay_all_sui(self, input_coins=None, recipient=None, gas_price=None, gas_budget=None):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
         if recipient is None:
             recipient = self.account.account_address
         if input_coins is None:
             input_coins = self.get_account_sui()
         msg = TransactionBuild.pay_all_sui(
             self.account.account_address,
             input_coins=input_coins,
             recipient=recipient,
             gas_price=gas_price,
             gas_budget=gas_budget
         )
         # simulate
         tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
-        self.client.sui_dryRunTransactionBlock(tx_bytes)
+        self.simulate_fail_abort(tx_bytes)
 
         # Sig
         serialized_sig_base64 = self.generate_signature(msg.encode)
 
         # Execute
         print(f'\nExecute transaction unsafe::pay_all_sui, waiting...')
         return self._execute(tx_bytes,
                              signatures=[serialized_sig_base64],
                              module="unsafe",
                              function="pay_all_sui"
                              )
 
-    def unsafe_pay_sui(self, amounts, input_coins=None, recipients=None, gas_budget=100000000):
+    def unsafe_pay_sui(self, amounts, input_coins=None, recipients=None, gas_budget=None):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
         if recipients is None:
             recipients = [self.account.account_address] * len(amounts)
         if input_coins is None:
             input_coins = list(self.get_account_sui().keys())
         amounts = [str(v) for v in amounts]
         result = self.client.unsafe_paySui(
             self.account.account_address,
             input_coins,
             recipients,
             amounts,
             gas_budget=gas_budget
         )
-        # simulate
+
         tx_bytes = result["txBytes"]
-        self.client.sui_dryRunTransactionBlock(tx_bytes)
+        self.simulate_fail_abort(tx_bytes)
 
         # Sig
         msg = bytes([IntentScope.TransactionData[1], IntentVersion.V0[1], AppId.Sui[1]]
                     + list(base64.b64decode(tx_bytes)))
         serialized_sig_base64 = self.generate_signature(msg)
 
         # Execute
         print(f'\nExecute transaction unsafe_transfer::transfer_object, waiting...')
         return self._execute(tx_bytes, [serialized_sig_base64], module="unsafe_transfer", function="transfer_object")
 
-    def pay_sui(self, amounts, input_coins=None, recipients=None, gas_price=1000, gas_budget=100000000):
+    def pay_sui(self, amounts, input_coins=None, recipients=None, gas_price=None, gas_budget=None):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
         if recipients is None:
             recipients = [self.account.account_address] * len(amounts)
         if input_coins is None:
             input_coins = self.get_account_sui()
         msg = TransactionBuild.pay_sui(
             self.account.account_address,
             input_coins,
             recipients,
             amounts,
             gas_price=gas_price,
             gas_budget=gas_budget
         )
-        # simulate
+
         tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
-        self.client.sui_dryRunTransactionBlock(tx_bytes)
+        self.simulate_fail_abort(tx_bytes)
 
         # Sig
         serialized_sig_base64 = self.generate_signature(msg.encode)
 
         # Execute
         print(f'\nExecute transaction unsafe_transfer::transfer_object, waiting...')
         return self._execute(tx_bytes, [serialized_sig_base64], module="unsafe_transfer", function="transfer_object")
 
-    def unsafe_transfer_object(self, object_id, recipient, gas_price=1000, gas_budget=100000000):
+    def unsafe_transfer_object(self, object_id, recipient, gas_price=None, gas_budget=None):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
         result = self.client.unsafe_transferObject(
             self.account.account_address,
             object_id,
             gas=None,
             gas_budget=gas_budget,
             recipient=recipient)
-        # simulate
+
         tx_bytes = result["txBytes"]
-        self.client.sui_dryRunTransactionBlock(tx_bytes)
+        self.simulate_fail_abort(tx_bytes)
 
         # Sig
         msg = bytes([IntentScope.TransactionData[1], IntentVersion.V0[1], AppId.Sui[1]]
                     + list(base64.b64decode(tx_bytes)))
         serialized_sig_base64 = self.generate_signature(msg)
 
         # Execute
         print(f'\nExecute transaction unsafe_transfer::transfer_object, waiting...')
         return self._execute(tx_bytes, [serialized_sig_base64], module="unsafe_transfer", function="transfer_object")
 
-    def transfer_object(self, object_id, recipient, gas_price=1000, gas_budget=100000000):
+    def transfer_object(self, object_id, recipient, gas_price=None, gas_budget=None):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
         msg = TransactionBuild.transfer_object(
             self.account.account_address,
             object_id,
             recipient,
             gas_price=gas_price,
             gas_budget=gas_budget)
 
-        # simulate
         tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
-        self.client.sui_dryRunTransactionBlock(tx_bytes)
+        self.simulate_fail_abort(tx_bytes)
 
         # Sig
         serialized_sig_base64 = self.generate_signature(msg.encode)
 
         # Execute
         print(f'\nExecute transaction transfer::transfer_object, waiting...')
         return self._execute(tx_bytes, [serialized_sig_base64], module="transfer", function="transfer_object")
 
-    def pay(self, input_coins: list, amounts, recipients=None, gas_price=1000, gas_budget=100000000):
+    def pay(self, input_coins: list, amounts, recipients=None, gas_price=None, gas_budget=None):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
         msg = TransactionBuild.pay(
             self.account.account_address,
             input_coins,
             recipients,
             amounts,
             gas_price=gas_price,
             gas_budget=gas_budget)
 
-        # simulate
         tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
-        self.client.sui_dryRunTransactionBlock(tx_bytes)
+        self.simulate_fail_abort(tx_bytes)
 
         # Sig
         serialized_sig_base64 = self.generate_signature(msg.encode)
 
         # Execute
         print(f'\nExecute transaction pay::pay, waiting...')
         return self._execute(tx_bytes, [serialized_sig_base64], module="pay", function="pay")
 
     def publish(
             self,
             compiled_modules,
             dep_ids,
-            gas_price=1000,
-            gas_budget=100000000
+            gas_price=None,
+            gas_budget=None
     ):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
         msg = TransactionBuild.publish(
             self.account.account_address,
             compiled_modules,
             dep_ids,
             gas_price=gas_price,
             gas_budget=gas_budget)
 
-        # simulate
         tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
-        self.client.sui_dryRunTransactionBlock(tx_bytes)
+        self.simulate_fail_abort(tx_bytes)
 
         # Sig
         serialized_sig_base64 = self.generate_signature(msg.encode)
 
         # Execute
         print(f'\nExecute transaction publish::package, waiting...')
         return self._execute(tx_bytes, [serialized_sig_base64], module="publish", function="package")
@@ -2138,31 +2201,34 @@
             self,
             package_id,
             compiled_modules,
             dep_ids,
             upgrade_capability: str,
             upgrade_policy: int,
             digest: Union[str, list],
-            gas_price=1000,
-            gas_budget=100000000
+            gas_price=None,
+            gas_budget=None
     ):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
         msg = TransactionBuild.upgrade(
             package_id=package_id,
             sender=self.account.account_address,
             compiled_modules=compiled_modules,
             dep_ids=dep_ids,
             upgrade_capability=upgrade_capability,
             upgrade_policy=upgrade_policy,
             digest=digest,
             gas_price=gas_price,
             gas_budget=gas_budget)
 
-        # simulate
         tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
-        self.client.sui_dryRunTransactionBlock(tx_bytes)
+        self.simulate_fail_abort(tx_bytes)
 
         # Sig
         serialized_sig_base64 = self.generate_signature(msg.encode)
 
         # Execute
         print(f'\nExecute transaction publish::package, waiting...')
         return self._execute(tx_bytes, [serialized_sig_base64], module="publish", function="package")
@@ -2172,92 +2238,166 @@
             package_id,
             proposal_package_id,
             compiled_modules,
             dep_ids,
             governance_info: str,
             governance_contracts: str,
             proposal: str,
-            gas_price=1000,
-            gas_budget=100000000
+            gas_price=None,
+            gas_budget=None
     ):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
         msg = TransactionBuild.dola_upgrade(
             package_id=package_id,
             proposal_package_id=proposal_package_id,
             sender=self.account.account_address,
             compiled_modules=compiled_modules,
             dep_ids=dep_ids,
             governance_info=governance_info,
             governance_contracts=governance_contracts,
             proposal=proposal,
             gas_price=gas_price,
             gas_budget=gas_budget)
 
-        # simulate
         tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
-        self.client.sui_dryRunTransactionBlock(tx_bytes)
+        self.simulate_fail_abort(tx_bytes)
 
         # Sig
         serialized_sig_base64 = self.generate_signature(msg.encode)
 
         # Execute
         print(f'\nExecute transaction dola_upgrade::upgrade, waiting...')
         return self._execute(tx_bytes, [serialized_sig_base64], module="dola_upgrade", function="upgrade")
 
     def batch_transaction(
             self,
             actual_params,
             transactions,
-            gas_price=1000,
-            gas_budget=100000000
+            gas_price=None,
+            gas_budget=None
     ):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
         inputs = []
         for module_function, arguments, type_arguments in transactions:
             package_id = module_function.package.package_id
             abi = module_function.abi
             inputs.append([package_id, abi, type_arguments, arguments])
         msg = TransactionBuild.batch_transaction(
             sender=self.account.account_address,
             actual_params=actual_params,
             transactions=inputs,
             gas_price=gas_price,
             gas_budget=gas_budget)
 
-        # simulate
         tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
-        self.client.sui_dryRunTransactionBlock(tx_bytes)
+        self.simulate_fail_abort(tx_bytes)
 
         # Sig
         serialized_sig_base64 = self.generate_signature(msg.encode)
 
         # Execute
         print(f'\nExecute transaction batch::transactions, waiting...')
         return self._execute(tx_bytes, [serialized_sig_base64], module="batch", function="transactions")
 
+    def batch_transaction_simulate(
+            self,
+            actual_params,
+            transactions,
+            gas_price=None,
+            gas_budget=None
+    ):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
+        inputs = []
+        for module_function, arguments, type_arguments in transactions:
+            package_id = module_function.package.package_id
+            abi = module_function.abi
+            inputs.append([package_id, abi, type_arguments, arguments])
+        msg = TransactionBuild.batch_transaction(
+            sender=self.account.account_address,
+            actual_params=actual_params,
+            transactions=inputs,
+            gas_price=gas_price,
+            gas_budget=gas_budget)
+
+        tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
+        return self.client.sui_dryRunTransactionBlock(tx_bytes)
+
+    def batch_transaction_inspect(
+            self,
+            actual_params,
+            transactions,
+            gas_price=None,
+            gas_budget=None
+    ):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
+        inputs = []
+        for module_function, arguments, type_arguments in transactions:
+            package_id = module_function.package.package_id
+            abi = module_function.abi
+            inputs.append([package_id, abi, type_arguments, arguments])
+        msg = TransactionBuild.batch_transaction(
+            sender=self.account.account_address,
+            actual_params=actual_params,
+            transactions=inputs,
+            gas_price=gas_price,
+            gas_budget=gas_budget)
+
+        tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
+        return self.client.sui_devInspectTransactionBlock(
+            self.account.account_address,
+            tx_bytes,
+            None,
+            None
+        )
+
     def with_gas_coin(
             self,
             package_id,
             abi: dict,
             *arguments,
             type_arguments: List[str] = None,
-            gas_price=1000,
-            gas_budget=100000000,
+            gas_price=None,
+            gas_budget=None,
     ):
+        if gas_budget is None:
+            gas_budget = self.gas_budget
+        if gas_price is None:
+            gas_price = self.estimate_gas_price()
         # Construct
         msg = TransactionBuild.move_call_with_gas_coin(
             self.account.account_address,
             package_id,
             abi,
             type_arguments,
             arguments,
             gas_price=gas_price,
             gas_budget=gas_budget
         )
-        # simulate
         tx_bytes = base64.b64encode(msg.value.encode).decode("ascii")
-        self.client.sui_dryRunTransactionBlock(tx_bytes)
+        self.simulate_fail_abort(tx_bytes)
 
         # Sig
         serialized_sig_base64 = self.generate_signature(msg.encode)
 
         # Execute
         print(f'\nExecute transaction {abi["module_name"]}::{abi["func_name"]}, waiting...')
         return self._execute(tx_bytes, [serialized_sig_base64], module=abi["module_name"], function=abi["func_name"])
+
+    def estimate_gas_price(self):
+        try:
+            result = self.client.suix_getReferenceGasPrice()
+            return int(result)
+        except Exception as e:
+            print(f"Estimate gas price fail:{e}, using default 1000")
+            return 1000
```

## Comparing `sui_brownie-0.31.1.dist-info/METADATA` & `sui_brownie-0.31.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sui-brownie
-Version: 0.31.1
+Version: 0.31.2
 Summary: Sui Package Tool
 Home-page: https://github.com/OmniBTC/DolaProtocol/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `sui_brownie-0.31.1.dist-info/RECORD` & `sui_brownie-0.31.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 sui_brownie/MANIFEST.in,sha256=BzExY9sw9x0Pqk6SYHuMRRvYS-cm75AxBOBjsYGFfU4,10
 sui_brownie/README.md,sha256=-7DxT6cGHbWLr_VufOEwIzl4Vtojp5dZc_r89lwnK3o,878
 sui_brownie/__init__.py,sha256=ROrbn7qi0haZjB8FG5JqXpD5mQ6qQPDNOwe0-rPnKeM,38
 sui_brownie/account.py,sha256=suZRI__kDNhyuoCZ9_q4mIV673lJDz0jgj0HyEj_hsQ,2514
 sui_brownie/bcs.py,sha256=8LwJihqmjLGwtzq87XKAQhE7ZgxiRDUsUYRbK6yRy7s,12144
 sui_brownie/ed25519.py,sha256=8hLHtC21og60B3MzXi4JmdQoOCbUutExyQIJhypJ9dg,4326
 sui_brownie/parallelism.py,sha256=Thh7TUrRU1fn47lNTF30RrcL5lBPBeMT2DX9A_swXDg,10047
-sui_brownie/sui_brownie.py,sha256=W7QyQeSfhtIGpG6PJxyIVBBJq1RPGp4VfscqhAS4oTk,86180
+sui_brownie/sui_brownie.py,sha256=KkLB2Yl2xUM2UvpmeGBkOUZa7Iy15PbXQABb7ESrWsQ,91104
 sui_brownie/sui_client.py,sha256=Epyu5pXAI6jl_L-lzBg4gnNLYQVjdQTZ8kR4YrJfnqk,32439
 sui_brownie/sui_config.template.yaml,sha256=Qa6n48nf4qeLDhZnpVNjZJIYDm8jYFs7dVLCyLjxMTs,140
 sui_brownie/sui_keystore.template.keystore,sha256=dIQsJL_H6FdnGlET9u5NYXSmjTc1-8dk8wZWKrzcLOM,19
 sui_brownie/utils.py,sha256=bttovGstKoozRoMvzYFOFs_z73aled7UFbNBDPxX9Uo,866
-sui_brownie-0.31.1.dist-info/METADATA,sha256=Wkgs6mfdT7fzhH8qktX72BJUbgZ-q1yWkIlT4y0i8zw,983
-sui_brownie-0.31.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sui_brownie-0.31.1.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
-sui_brownie-0.31.1.dist-info/RECORD,,
+sui_brownie-0.31.2.dist-info/METADATA,sha256=yhvBCi-TvE4018O4YS3IwjpiWK4TspacVBrMMIhiOnU,983
+sui_brownie-0.31.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sui_brownie-0.31.2.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
+sui_brownie-0.31.2.dist-info/RECORD,,
```

