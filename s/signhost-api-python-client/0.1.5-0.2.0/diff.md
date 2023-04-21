# Comparing `tmp/signhost_api_python_client-0.1.5.tar.gz` & `tmp/signhost_api_python_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signhost_api_python_client-0.1.5.tar", max compression
+gzip compressed data, was "signhost_api_python_client-0.2.0.tar", max compression
```

## Comparing `signhost_api_python_client-0.1.5.tar` & `signhost_api_python_client-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1071 2023-02-13 11:41:48.070822 signhost_api_python_client-0.1.5/LICENSE
--rw-r--r--   0        0        0     3469 2023-02-13 11:41:48.070822 signhost_api_python_client-0.1.5/README.md
--rw-r--r--   0        0        0     2050 2023-02-13 11:42:01.618924 signhost_api_python_client-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       34 2023-02-13 11:41:48.074823 signhost_api_python_client-0.1.5/src/signhost/__init__.py
--rw-r--r--   0        0        0     3501 2023-02-13 11:42:01.618924 signhost_api_python_client-0.1.5/src/signhost/__main__.py
--rw-r--r--   0        0        0      147 2023-02-13 11:41:48.074823 signhost_api_python_client-0.1.5/src/signhost/client/__init__.py
--rw-r--r--   0        0        0     6349 2023-02-13 11:41:48.074823 signhost_api_python_client-0.1.5/src/signhost/client/client.py
--rw-r--r--   0        0        0      449 2023-02-13 11:41:48.074823 signhost_api_python_client-0.1.5/src/signhost/client/errors.py
--rw-r--r--   0        0        0       33 2023-02-13 11:41:48.074823 signhost_api_python_client-0.1.5/src/signhost/models/__init__.py
--rw-r--r--   0        0        0     1176 2023-02-13 11:41:48.074823 signhost_api_python_client-0.1.5/src/signhost/models/enums.py
--rw-r--r--   0        0        0    17293 2023-02-13 11:41:48.074823 signhost_api_python_client-0.1.5/src/signhost/models/generated.py
--rw-r--r--   0        0        0     5373 2023-02-13 11:41:48.074823 signhost_api_python_client-0.1.5/src/signhost/models/verifications.py
--rw-r--r--   0        0        0        0 2023-02-13 11:41:48.074823 signhost_api_python_client-0.1.5/src/signhost/py.typed
--rw-r--r--   0        0        0     4556 1970-01-01 00:00:00.000000 signhost_api_python_client-0.1.5/setup.py
--rw-r--r--   0        0        0     4612 1970-01-01 00:00:00.000000 signhost_api_python_client-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 13:49:19.045572 signhost_api_python_client-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3469 2023-04-21 13:49:19.045572 signhost_api_python_client-0.2.0/README.md
+-rw-r--r--   0        0        0     2089 2023-04-21 13:49:39.525717 signhost_api_python_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-21 13:49:19.045572 signhost_api_python_client-0.2.0/src/signhost/__init__.py
+-rw-r--r--   0        0        0     3501 2023-04-21 13:49:19.045572 signhost_api_python_client-0.2.0/src/signhost/__main__.py
+-rw-r--r--   0        0        0      147 2023-04-21 13:49:19.045572 signhost_api_python_client-0.2.0/src/signhost/client/__init__.py
+-rw-r--r--   0        0        0    10688 2023-04-21 13:49:19.049572 signhost_api_python_client-0.2.0/src/signhost/client/client.py
+-rw-r--r--   0        0        0      449 2023-04-21 13:49:19.049572 signhost_api_python_client-0.2.0/src/signhost/client/errors.py
+-rw-r--r--   0        0        0       33 2023-04-21 13:49:19.049572 signhost_api_python_client-0.2.0/src/signhost/models/__init__.py
+-rw-r--r--   0        0        0     1176 2023-04-21 13:49:19.049572 signhost_api_python_client-0.2.0/src/signhost/models/enums.py
+-rw-r--r--   0        0        0    17297 2023-04-21 13:49:19.049572 signhost_api_python_client-0.2.0/src/signhost/models/generated.py
+-rw-r--r--   0        0        0     5373 2023-04-21 13:49:19.049572 signhost_api_python_client-0.2.0/src/signhost/models/verifications.py
+-rw-r--r--   0        0        0        0 2023-04-21 13:49:19.049572 signhost_api_python_client-0.2.0/src/signhost/py.typed
+-rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 signhost_api_python_client-0.2.0/PKG-INFO
```

### Comparing `signhost_api_python_client-0.1.5/LICENSE` & `signhost_api_python_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `signhost_api_python_client-0.1.5/README.md` & `signhost_api_python_client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `signhost_api_python_client-0.1.5/pyproject.toml` & `signhost_api_python_client-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "signhost-api-python-client"
-version = "0.1.5"
+version = "0.2.0"
 description = "Signhost Api Python Client"
 authors = ["Jelmer Draaijer <info@jelmert.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/foarsitter/signhost-api-python-client"
 repository = "https://github.com/foarsitter/signhost-api-python-client"
 documentation = "https://signhost-api-python-client.readthedocs.io"
@@ -19,18 +19,17 @@
 Changelog = "https://github.com/foarsitter/signhost-api-python-client/releases"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = ">=8.0.1"
 httpx = "^0.23.3"
 pydantic = "^1.10.4"
-pyupgrade = "3.3.1"
 attrs = "^22.2.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
 flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.9.2"
@@ -49,14 +48,15 @@
 sphinx-click = ">=3.0.2"
 typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 myst-parser = {version = ">=0.16.1"}
 respx = "^0.20.1"
 pygments = "^2.14.0"
 devtools = "^0.10.0"
+pytest-asyncio = "^0.21.0"
 
 [tool.poetry.scripts]
 signhost = "signhost.__main__:main"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
@@ -77,10 +77,11 @@
 [tool.mypy]
 strict = true
 warn_unreachable = true
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
+plugins = "pydantic.mypy"
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `signhost_api_python_client-0.1.5/src/signhost/__main__.py` & `signhost_api_python_client-0.2.0/src/signhost/__main__.py`

 * *Files identical despite different names*

### Comparing `signhost_api_python_client-0.1.5/src/signhost/client/client.py` & `signhost_api_python_client-0.2.0/src/signhost/client/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+import base64
+import hashlib
 import io
 from json import JSONDecodeError
+from struct import pack
 from typing import Any
+from typing import AsyncIterator
 from typing import Dict
+from typing import Mapping
 from typing import Type
 from typing import TypeVar
 
 import httpx
 
 from .. import models
 from . import errors
@@ -32,31 +37,38 @@
         app_key: str,
         base_url: str = "https://api.signhost.com/api/",
     ):
         self.api_key = api_key
         self.app_key = app_key
         self.base_url = base_url
 
+    def create_content_headers(self, data: str) -> Mapping[str, str]:
+        content_length: str = str(len(data))
+        content_type: str = "application/json"
+        headers: Mapping[str, str] = {
+            "Content-Length": content_length,
+            "Content-Type": content_type,
+        }
+        return headers
+
     def process_response(
         self, response: httpx.Response, model: Type[_T], status_code_success: int = 200
     ) -> _T:
-
         try:
             if response.status_code == status_code_success:
                 response_json = response.json()
                 return model(**response_json)
             else:
                 raise self.create_error(response)
         except JSONDecodeError as e:
             raise errors.SignhostServerError(
                 "Invalid json from server", status_code=400
             ) from e
 
     def create_error(self, response: httpx.Response) -> errors.SignhostError:
-
         try:
             response_json = response.json()
         except JSONDecodeError:
             response_json = {"message": response.text}
 
         response_json["status_code"] = response.status_code
 
@@ -70,21 +82,28 @@
     def map_exception(self, response: httpx.Response) -> Type[errors.SignhostError]:
         exception_type = self.ERROR_RESPONSE_MAPPING.get(
             response.status_code, errors.SignhostError
         )
         return exception_type
 
     def authenticate_request(self, request: httpx.Request) -> httpx.Request:
-
         request.headers["Authorization"] = f"APIKey {self.api_key}"
         request.headers["Application"] = f"APPKey {self.app_key}"
 
         return request
 
 
+def b64_digest(file_content: io.IOBase) -> str:
+    sha = hashlib.sha256(file_content.read())
+    digest = sha.digest()
+    b64_digest = base64.b64encode(pack(f"{len(digest)}s", digest)).decode("utf-8")
+    file_content.seek(0)
+    return b64_digest
+
+
 class DefaultClient(BaseClient):
     """Synchronous client"""
 
     client: httpx.Client
 
     def __init__(
         self,
@@ -144,37 +163,32 @@
 
         raise self.create_error(response)
 
     def transaction_init(self, transaction: models.Transaction) -> models.Transaction:
         """POST /api/transaction"""
 
         data = transaction.json()
-        content_length = str(len(data))
-        content_type = "application/json"
-        headers = {"Content-Length": content_length, "Content-Type": content_type}
+        headers = self.create_content_headers(data)
 
         response = self.client.post("transaction", content=data, headers=headers)
 
         return self.process_response(response, models.Transaction)
 
     def transaction_file_put(
         self, transaction_id: str, file_id: str, file_content: io.IOBase
     ) -> bool:
         """PUT /api/transaction/{transactionId}/file/{fileId}"""
-        # sha = hashlib.sha256(file_content.read())
-        # file_digest = base64.urlsafe_b64encode(sha.digest()).decode("utf-8")
-
-        file_content.seek(0)
+        digest: str = b64_digest(file_content)
 
         response = self.client.put(
             f"transaction/{transaction_id}/file/{file_id}",
             content=file_content,
             headers={
                 "Content-Type": "application/pdf",
-                # "Digest": f"SHA256={file_digest}",
+                "Digest": f"SHA256={digest}",
             },
         )
 
         if response.status_code in [
             httpx.codes.CREATED,
             httpx.codes.ACCEPTED,
             httpx.codes.NO_CONTENT,
@@ -193,7 +207,120 @@
         return True
 
 
 class AsyncClient(BaseClient):
     """Asynchronous client."""
 
     client: httpx.AsyncClient
+
+    def __init__(
+        self,
+        api_key: str,
+        app_key: str,
+        base_url: str = "https://api.signhost.com/api/",
+        **httpx_kwargs: Any,
+    ):
+        super().__init__(api_key, app_key, base_url)
+        self.client = self.create_client(base_url, **httpx_kwargs)
+
+    def create_client(self, base_url: str, **httpx_kwargs: Any) -> httpx.AsyncClient:
+        httpx_kwargs.setdefault("base_url", base_url)
+        httpx_kwargs.setdefault("auth", self.authenticate_request)
+        return httpx.AsyncClient(**httpx_kwargs)
+
+    async def transaction_get(self, transaction_id: str) -> models.Transaction:
+        """GET /api/transaction/{transactionId}"""
+        response = await self.client.get(f"transaction/{transaction_id}")
+
+        return self.process_response(response, models.Transaction)
+
+    async def transaction_cancel(
+        self, transaction_id: str, send_notifications: bool = False, reason: str = ""
+    ) -> models.Transaction:
+        """DELETE /api/transaction/{transactionId}"""
+        response = await self.client.request(
+            "DELETE",
+            f"transaction/{transaction_id}",
+            json={"SendNotifications": send_notifications, "Reason": reason},
+        )
+        return self.process_response(response, models.Transaction)
+
+    async def transaction_file_get(self, transaction_id: str, file_id: str) -> bytes:
+        """
+        GET /api/transaction/{transactionId}/file/{fileId}
+
+        Returns the contents of the (signed) document(s).
+        """
+        response = await self.client.get(f"transaction/{transaction_id}/file/{file_id}")
+
+        if response.status_code == httpx.codes.OK:
+            return response.content
+
+        raise self.create_error(response)
+
+    async def receipt_get(self, transaction_id: str) -> bytes:
+        """
+        GET /api/file/receipt/{transactionId}
+
+        Returns the contents of the receipt when the transaction is successfully signed (Status=30)
+        """
+        response = await self.client.get(f"file/receipt/{transaction_id}")
+
+        if response.status_code == httpx.codes.OK:
+            return response.content
+
+        raise self.create_error(response)
+
+    async def transaction_init(
+        self, transaction: models.Transaction
+    ) -> models.Transaction:
+        """POST /api/transaction"""
+        data: str = transaction.json()
+
+        headers = self.create_content_headers(data)
+
+        response = await self.client.post("transaction", content=data, headers=headers)
+
+        return self.process_response(response, models.Transaction)
+
+    async def transaction_file_put(
+        self, transaction_id: str, file_id: str, file_content: io.IOBase
+    ) -> bool:
+        """PUT /api/transaction/{transactionId}/file/{fileId}"""
+        digest: str = b64_digest(file_content)
+
+        response = await self.client.put(
+            f"transaction/{transaction_id}/file/{file_id}",
+            content=bytes_as_stream(file_content),
+            headers={
+                "Content-Type": "application/pdf",
+                "Digest": f"SHA256={digest}",
+            },
+        )
+
+        if response.status_code in [
+            httpx.codes.CREATED,
+            httpx.codes.ACCEPTED,
+            httpx.codes.NO_CONTENT,
+        ]:
+            return True
+
+        raise self.create_error(response)
+
+    async def transaction_start(self, transaction_id: str) -> bool:
+        """PUT /api/transaction/{transactionId}/start"""
+        response = await self.client.put(f"transaction/{transaction_id}/start")
+
+        if response.status_code != httpx.codes.NO_CONTENT:
+            raise self.create_error(response)
+
+        return True
+
+
+CHUNK_SIZE = 65_536
+
+
+async def bytes_as_stream(file_content: io.IOBase) -> AsyncIterator[bytes]:
+    chunk = file_content.read(CHUNK_SIZE)
+    while chunk:
+        yield chunk
+        chunk = file_content.read(CHUNK_SIZE)
```

### Comparing `signhost_api_python_client-0.1.5/src/signhost/models/enums.py` & `signhost_api_python_client-0.2.0/src/signhost/models/enums.py`

 * *Files identical despite different names*

### Comparing `signhost_api_python_client-0.1.5/src/signhost/models/generated.py` & `signhost_api_python_client-0.2.0/src/signhost/models/generated.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
     )
     SendSignConfirmation: Optional[bool] = Field(
         None,
         description="Send the sign confirmation to the signer his e-mail address."
         "\nDefault value is the value of `SendSignRequest`\n",
     )
     Language: Optional[Language] = Field(
-        "nl-NL",
+        Language.NL,
         description="The language of the receiving user, "
         "only de-DE, en-US, es-ES, fr-FR, it-IT, pl-PL and nl-NL are allowed.",
     )
     ScribbleName: Optional[str] = Field(
         None,
         description="The name of the signer, this will be pre filled in the scribble form.",
     )
```

### Comparing `signhost_api_python_client-0.1.5/src/signhost/models/verifications.py` & `signhost_api_python_client-0.2.0/src/signhost/models/verifications.py`

 * *Files identical despite different names*

### Comparing `signhost_api_python_client-0.1.5/setup.py` & `signhost_api_python_client-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,126 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: signhost-api-python-client
+Version: 0.2.0
+Summary: Signhost Api Python Client
+Home-page: https://github.com/foarsitter/signhost-api-python-client
+License: MIT
+Author: Jelmer Draaijer
+Author-email: info@jelmert.nl
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: attrs (>=22.2.0,<23.0.0)
+Requires-Dist: click (>=8.0.1)
+Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Project-URL: Changelog, https://github.com/foarsitter/signhost-api-python-client/releases
+Project-URL: Documentation, https://signhost-api-python-client.readthedocs.io
+Project-URL: Repository, https://github.com/foarsitter/signhost-api-python-client
+Description-Content-Type: text/markdown
+
+# Signhost Api Python Client
+
+[![PyPI](https://img.shields.io/pypi/v/signhost-api-python-client.svg)][pypi_]
+[![Status](https://img.shields.io/pypi/status/signhost-api-python-client.svg)][status]
+[![Python Version](https://img.shields.io/pypi/pyversions/signhost-api-python-client)][python version]
+[![License](https://img.shields.io/pypi/l/signhost-api-python-client)][license]
+
+[![Read the documentation at https://signhost-api-python-client.readthedocs.io/](https://img.shields.io/readthedocs/signhost-api-python-client/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Tests](https://github.com/foarsitter/signhost-api-python-client/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/foarsitter/signhost-api-python-client/branch/main/graph/badge.svg)][codecov]
+
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+
+[pypi_]: https://pypi.org/project/signhost-api-python-client/
+[status]: https://pypi.org/project/signhost-api-python-client/
+[python version]: https://pypi.org/project/signhost-api-python-client
+[read the docs]: https://signhost-api-python-client.readthedocs.io/
+[tests]: https://github.com/foarsitter/signhost-api-python-client/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/foarsitter/signhost-api-python-client
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[black]: https://github.com/psf/black
+
+## Features
+
+- 100% test coverage
+
+## Requirements
+
+- httpx
+- pydantic
+- attr
+- click
+
+## Installation
+
+You can install _Signhost Api Python Client_ via [pip] from [PyPI]:
+
+```console
+$ pip install signhost-api-python-client
+```
+
+## Usage
+
+```python
+import io
+from signhost import models
+from signhost.client import DefaultClient
+
+signhost = DefaultClient(api_key="str", app_key="str")
+transaction = models.Transaction(signers=[models.Signer(email="str")])
+
+transaction = signhost.transaction_init(transaction=transaction)
+signhost.transaction_file_put(
+    transaction.Id,
+    "file.pdf",
+    io.BytesIO(b"test"),
+)
+transaction = signhost.transaction_start(transaction.Id)
+
+print("Sign the contract over here", transaction.Signers[0].SignUrl)
+
+signhost.transaction_get(transaction.Id)
+signhost.transaction_file_get(transaction.Id, "file.pdf")
+signhost.receipt_get(transaction.Id)
+```
+
+Please see the [Command-line Reference] for details.
+
+## Contributing
+
+Contributions are very welcome.
+To learn more, see the [Contributor Guide].
+
+## License
+
+Distributed under the terms of the [MIT license][license],
+_Signhost Api Python Client_ is free and open source software.
+
+## Issues
+
+If you encounter any problems,
+please [file an issue] along with a detailed description.
+
+## Credits
+
+This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
+
+[@cjolowicz]: https://github.com/cjolowicz
+[pypi]: https://pypi.org/
+[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+[file an issue]: https://github.com/foarsitter/signhost-api-python-client/issues
+[pip]: https://pip.pypa.io/
+
+<!-- github-only -->
+
+[license]: https://github.com/foarsitter/signhost-api-python-client/blob/main/LICENSE
+[contributor guide]: https://github.com/foarsitter/signhost-api-python-client/blob/main/CONTRIBUTING.md
+[command-line reference]: https://signhost-api-python-client.readthedocs.io/en/latest/usage.html
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['signhost', 'signhost.client', 'signhost.models']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['attrs>=22.2.0,<23.0.0',
- 'click>=8.0.1',
- 'httpx>=0.23.3,<0.24.0',
- 'pydantic>=1.10.4,<2.0.0',
- 'pyupgrade==3.3.1']
-
-entry_points = \
-{'console_scripts': ['signhost = signhost.__main__:main']}
-
-setup_kwargs = {
-    'name': 'signhost-api-python-client',
-    'version': '0.1.5',
-    'description': 'Signhost Api Python Client',
-    'long_description': '# Signhost Api Python Client\n\n[![PyPI](https://img.shields.io/pypi/v/signhost-api-python-client.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/signhost-api-python-client.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/signhost-api-python-client)][python version]\n[![License](https://img.shields.io/pypi/l/signhost-api-python-client)][license]\n\n[![Read the documentation at https://signhost-api-python-client.readthedocs.io/](https://img.shields.io/readthedocs/signhost-api-python-client/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/foarsitter/signhost-api-python-client/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/foarsitter/signhost-api-python-client/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/signhost-api-python-client/\n[status]: https://pypi.org/project/signhost-api-python-client/\n[python version]: https://pypi.org/project/signhost-api-python-client\n[read the docs]: https://signhost-api-python-client.readthedocs.io/\n[tests]: https://github.com/foarsitter/signhost-api-python-client/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/foarsitter/signhost-api-python-client\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- 100% test coverage\n\n## Requirements\n\n- httpx\n- pydantic\n- attr\n- click\n\n## Installation\n\nYou can install _Signhost Api Python Client_ via [pip] from [PyPI]:\n\n```console\n$ pip install signhost-api-python-client\n```\n\n## Usage\n\n```python\nimport io\nfrom signhost import models\nfrom signhost.client import DefaultClient\n\nsignhost = DefaultClient(api_key="str", app_key="str")\ntransaction = models.Transaction(signers=[models.Signer(email="str")])\n\ntransaction = signhost.transaction_init(transaction=transaction)\nsignhost.transaction_file_put(\n    transaction.Id,\n    "file.pdf",\n    io.BytesIO(b"test"),\n)\ntransaction = signhost.transaction_start(transaction.Id)\n\nprint("Sign the contract over here", transaction.Signers[0].SignUrl)\n\nsignhost.transaction_get(transaction.Id)\nsignhost.transaction_file_get(transaction.Id, "file.pdf")\nsignhost.receipt_get(transaction.Id)\n```\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Signhost Api Python Client_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/foarsitter/signhost-api-python-client/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/foarsitter/signhost-api-python-client/blob/main/LICENSE\n[contributor guide]: https://github.com/foarsitter/signhost-api-python-client/blob/main/CONTRIBUTING.md\n[command-line reference]: https://signhost-api-python-client.readthedocs.io/en/latest/usage.html\n',
-    'author': 'Jelmer Draaijer',
-    'author_email': 'info@jelmert.nl',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/foarsitter/signhost-api-python-client',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

