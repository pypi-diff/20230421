# Comparing `tmp/cancelchain-1.2.0.tar.gz` & `tmp/cancelchain-1.3.0.tar.gz`

## Comparing `cancelchain-1.2.0.tar` & `cancelchain-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/__init__.py
--rw-r--r--   0        0        0    17826 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/api.py
--rw-r--r--   0        0        0     7318 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/api_client.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/application.py
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/block.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/browser.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/cache.py
--rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/chain.py
--rw-r--r--   0        0        0    29735 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/command.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/config.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/console.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/database.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/exceptions.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/miller.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/milling.py
--rw-r--r--   0        0        0    20782 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/models.py
--rw-r--r--   0        0        0     9440 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/node.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/payload.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/schema.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/signals.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/tasks.py
--rw-r--r--   0        0        0    10109 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/transaction.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/util.py
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/wallet.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/templates/base.html
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/templates/block.html
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/templates/chains.html
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/templates/index.html
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 cancelchain-1.2.0/src/cancelchain/templates/transaction.html
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 cancelchain-1.2.0/.gitignore
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 cancelchain-1.2.0/LICENSE
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 cancelchain-1.2.0/README.rst
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 cancelchain-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 cancelchain-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/__init__.py
+-rw-r--r--   0        0        0    17826 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/api.py
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/api_client.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/application.py
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/block.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/browser.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/cache.py
+-rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/chain.py
+-rw-r--r--   0        0        0    29702 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/command.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/config.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/console.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/database.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/exceptions.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/miller.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/milling.py
+-rw-r--r--   0        0        0    20782 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/models.py
+-rw-r--r--   0        0        0     9440 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/node.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/payload.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/schema.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/signals.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/tasks.py
+-rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/transaction.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/util.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/wallet.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/templates/base.html
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/templates/block.html
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/templates/chains.html
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/templates/index.html
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 cancelchain-1.3.0/src/cancelchain/templates/transaction.html
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 cancelchain-1.3.0/.gitignore
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 cancelchain-1.3.0/LICENSE
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 cancelchain-1.3.0/README.rst
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 cancelchain-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 cancelchain-1.3.0/PKG-INFO
```

### Comparing `cancelchain-1.2.0/src/cancelchain/__init__.py` & `cancelchain-1.3.0/src/cancelchain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import click
 from flask import Flask
 from flask.cli import FlaskGroup
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 
 def create_app(app=None, register_browser=True, test_config=None):
     from .application import init_app
     from .cache import cache
     from .config import EnvAppSettings
     from .database import db
```

### Comparing `cancelchain-1.2.0/src/cancelchain/api.py` & `cancelchain-1.3.0/src/cancelchain/api.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/api_client.py` & `cancelchain-1.3.0/src/cancelchain/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import requests
 
 from cancelchain.util import dt_2_ciso, host_address
 
 OK = requests.codes.ok
 UNAUTHORIZED = requests.codes.unauthorized
 PEER_HOST_HEADER = 'Peer-Hosts'
-ADDRESS_MISSMATCH_MSG = 'Address/wallet mismatch'
+ADDRESS_MISMATCH_MSG = 'Address/wallet mismatch'
 
 
 def json_header(headers=None):
     headers = headers or {}
     headers['Content-Type'] = 'application/json'
     return headers
 
@@ -24,15 +24,15 @@
     return headers
 
 
 class ApiClient():
     def __init__(self, host, wallet, timeout=None):
         host, address = host_address(host)
         if address and address != wallet.address:
-            raise Exception(ADDRESS_MISSMATCH_MSG)
+            raise Exception(ADDRESS_MISMATCH_MSG)
         self.host = host
         self.wallet = wallet
         self.token = None
         self.timeout = timeout if timeout is not None else 10
 
     def request_token(self, rfs=True):
         r = requests.get(
```

### Comparing `cancelchain-1.2.0/src/cancelchain/application.py` & `cancelchain-1.3.0/src/cancelchain/application.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/block.py` & `cancelchain-1.3.0/src/cancelchain/block.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/browser.py` & `cancelchain-1.3.0/src/cancelchain/browser.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/chain.py` & `cancelchain-1.3.0/src/cancelchain/chain.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/command.py` & `cancelchain-1.3.0/src/cancelchain/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,14 @@
             f.seek(0)
         return f.readline().decode()
 
 
 class ProgressBar():
     def __init__(self, title, console=None, total=None, completed=0):
         self.progress = Progress(
-            # TextColumn(title),
             BarColumn(),
             TextColumn('{task.completed}/{task.total}'),
             TaskProgressColumn(),
             TimeRemainingColumn(),
             TextColumn('['),
             TimeElapsedColumn(),
             TextColumn(']'),
```

### Comparing `cancelchain-1.2.0/src/cancelchain/exceptions.py` & `cancelchain-1.3.0/src/cancelchain/exceptions.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/miller.py` & `cancelchain-1.3.0/src/cancelchain/miller.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/milling.py` & `cancelchain-1.3.0/src/cancelchain/milling.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/models.py` & `cancelchain-1.3.0/src/cancelchain/models.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/node.py` & `cancelchain-1.3.0/src/cancelchain/node.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/payload.py` & `cancelchain-1.3.0/src/cancelchain/payload.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/schema.py` & `cancelchain-1.3.0/src/cancelchain/schema.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/tasks.py` & `cancelchain-1.3.0/src/cancelchain/tasks.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/transaction.py` & `cancelchain-1.3.0/src/cancelchain/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     validate_address,
     validate_signature,
 )
 from cancelchain.util import dt_2_iso, iso_2_dt, now_iso
 
 VERSION_1 = '1'
 MAX_FLOWS = 50
-ADDRESS_MISSMATCH_MSG = 'Address/public key mismatch'
+ADDRESS_MISMATCH_MSG = 'Address/public key mismatch'
 
 
 class TransactionSchema(SansNoneSchema):
     timestamp = Timestamp(required=True)
     txid = MillHash(required=True)
     address = Address(required=True)
     public_key = PublicKey(required=True)
@@ -61,15 +61,15 @@
         validate=validate.Length(min=1, max=MAX_FLOWS)
     )
     version = fields.String(required=True, validate=validate.Equal(VERSION_1))
 
     @validates_schema
     def validate_pk_address(self, data, **kwargs):
         if not validate_address(data.get('public_key'), data.get('address')):
-            raise ValidationError(ADDRESS_MISSMATCH_MSG)
+            raise ValidationError(ADDRESS_MISMATCH_MSG)
 
     @post_load
     def make_transaction(self, data, **kwargs):
         return Transaction(**data)
 
 
 class RegularTransactionSchema(TransactionSchema):
```

### Comparing `cancelchain-1.2.0/src/cancelchain/util.py` & `cancelchain-1.3.0/src/cancelchain/util.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/wallet.py` & `cancelchain-1.3.0/src/cancelchain/wallet.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/templates/base.html` & `cancelchain-1.3.0/src/cancelchain/templates/base.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/templates/block.html` & `cancelchain-1.3.0/src/cancelchain/templates/block.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/templates/chains.html` & `cancelchain-1.3.0/src/cancelchain/templates/chains.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/templates/index.html` & `cancelchain-1.3.0/src/cancelchain/templates/index.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/src/cancelchain/templates/transaction.html` & `cancelchain-1.3.0/src/cancelchain/templates/transaction.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/.gitignore` & `cancelchain-1.3.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -138,7 +138,10 @@
 *.jsonl
 
 # sphinx
 _build/
 
 # ruff
 .ruff_cache/
+
+# vscode
+.vscode/
```

### Comparing `cancelchain-1.2.0/LICENSE` & `cancelchain-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cancelchain-1.2.0/pyproject.toml` & `cancelchain-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   "passlib[argon2]>=1.7",
   "pg8000>=1.29",
   "pycryptodome>=3.17",
   "pyjwt>=2.6",
   "pymerkle>=4.0",
   "python-dotenv>=1.0",
   "requests>=2.28",
-  "rich>=13.3.3",
+  "rich>=13.3",
   "sqlalchemy<2.0",
 ]
 
 [project.scripts]
 cancelchain = "cancelchain:cli"
 
 [project.urls]
@@ -70,20 +70,20 @@
 exclude = [
   "/.github",
 ]
 
 [tool.hatch.envs.test]
 dependencies = [
   "coverage[toml]>=7.2",
-  "pytest>=7.2",
+  "pytest>=7.3",
   "pytest-cov>=4.0",
   "pytest-dotenv>=0.5",
   "requests-mock>=1.10",
   "time-machine>=2.9",
-  "ruff>=0.0.260",
+  "ruff>=0.0.261",
 ]
 
 [tool.hatch.envs.test.scripts]
 run-coverage = "pytest --cov-config=pyproject.toml --cov=cancelchain"
 run = "run-coverage --no-cov"
 
 # RUFF
@@ -135,20 +135,22 @@
 ]
 
 # PYTEST
 [tool.pytest.ini_options]
 testpaths = [
   "tests",
 ]
-env_files = [
-  "tests/.test.env",
-]
 filterwarnings = [
   "ignore:.*SelectableGroups dict interface is deprecated.*"
 ]
+# PYTEST-DOTENV
+env_files = [
+  "tests/.test.env",
+]
+env_override_existing_values = 1
 
 # COVERAGE
 [tool.coverage.html]
 directory = "coverage_html_report"
 
 [tool.coverage.report]
 exclude_lines = [
```

