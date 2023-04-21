# Comparing `tmp/vectordb-orm-0.1.0.tar.gz` & `tmp/vectordb_orm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectordb-orm-0.1.0.tar", max compression
+gzip compressed data, was "vectordb_orm-0.2.0.tar", max compression
```

## Comparing `vectordb-orm-0.1.0.tar` & `vectordb_orm-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,30 @@
--rw-r--r--   0        0        0     1071 2023-04-17 15:02:33.589258 vectordb-orm-0.1.0/LICENSE
--rw-r--r--   0        0        0     4988 2023-04-18 18:56:20.181298 vectordb-orm-0.1.0/README.md
--rw-r--r--   0        0        0      427 2023-04-18 19:21:01.425925 vectordb-orm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      236 2023-04-18 18:54:24.854024 vectordb-orm-0.1.0/vectordb_orm/__init__.py
--rw-r--r--   0        0        0     1753 2023-04-18 18:54:24.854254 vectordb-orm-0.1.0/vectordb_orm/attributes.py
--rw-r--r--   0        0        0    10102 2023-04-18 18:54:24.854378 vectordb-orm-0.1.0/vectordb_orm/base.py
--rw-r--r--   0        0        0     1160 2023-04-18 18:54:24.854914 vectordb-orm-0.1.0/vectordb_orm/fields.py
--rw-r--r--   0        0        0      765 2023-04-18 18:54:24.855104 vectordb-orm-0.1.0/vectordb_orm/indexes.py
--rw-r--r--   0        0        0     5813 2023-04-18 18:54:24.855197 vectordb-orm-0.1.0/vectordb_orm/query.py
--rw-r--r--   0        0        0      336 2023-04-18 18:54:24.855338 vectordb-orm-0.1.0/vectordb_orm/results.py
--rw-r--r--   0        0        0      372 2023-04-18 18:54:24.855414 vectordb-orm-0.1.0/vectordb_orm/session.py
--rw-r--r--   0        0        0      117 2023-04-18 18:54:24.855594 vectordb-orm-0.1.0/vectordb_orm/similarity.py
--rw-r--r--   0        0        0        0 2023-04-18 18:54:24.855626 vectordb-orm-0.1.0/vectordb_orm/tests/__init__.py
--rw-r--r--   0        0        0      633 2023-04-18 18:54:24.855737 vectordb-orm-0.1.0/vectordb_orm/tests/conftest.py
--rw-r--r--   0        0        0      408 2023-04-18 18:54:24.855825 vectordb-orm-0.1.0/vectordb_orm/tests/models.py
--rw-r--r--   0        0        0     1556 2023-04-18 18:54:24.855904 vectordb-orm-0.1.0/vectordb_orm/tests/test_base.py
--rw-r--r--   0        0        0     2476 2023-04-18 18:54:24.855992 vectordb-orm-0.1.0/vectordb_orm/tests/test_query.py
--rw-r--r--   0        0        0     5736 1970-01-01 00:00:00.000000 vectordb-orm-0.1.0/setup.py
--rw-r--r--   0        0        0     5401 1970-01-01 00:00:00.000000 vectordb-orm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7130 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/README.md
+-rw-r--r--   0        0        0      497 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      906 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/__init__.py
+-rw-r--r--   0        0        0     1582 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/attributes.py
+-rw-r--r--   0        0        0        0 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/__init__.py
+-rw-r--r--   0        0        0     2033 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/base.py
+-rw-r--r--   0        0        0      155 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/milvus/__init__.py
+-rw-r--r--   0        0        0    10264 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/milvus/indexes.py
+-rw-r--r--   0        0        0    13202 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/milvus/milvus.py
+-rw-r--r--   0        0        0      746 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/milvus/similarity.py
+-rw-r--r--   0        0        0      107 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/pinecone/__init__.py
+-rw-r--r--   0        0        0      884 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/pinecone/indexes.py
+-rw-r--r--   0        0        0     9671 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/pinecone/pinecone.py
+-rw-r--r--   0        0        0     3594 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/base.py
+-rw-r--r--   0        0        0      473 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/enums.py
+-rw-r--r--   0        0        0      984 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/fields.py
+-rw-r--r--   0        0        0       26 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/index.py
+-rw-r--r--   0        0        0     4342 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/query.py
+-rw-r--r--   0        0        0      364 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/results.py
+-rw-r--r--   0        0        0     1435 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/session.py
+-rw-r--r--   0        0        0        0 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/__init__.py
+-rw-r--r--   0        0        0     1609 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/milvus/__init__.py
+-rw-r--r--   0        0        0     3603 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/milvus/test_indexes.py
+-rw-r--r--   0        0        0     1194 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/milvus/test_milvus.py
+-rw-r--r--   0        0        0     1114 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/models.py
+-rw-r--r--   0        0        0     2537 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/test_base.py
+-rw-r--r--   0        0        0     2756 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/test_query.py
+-rw-r--r--   0        0        0     7642 1970-01-01 00:00:00.000000 vectordb_orm-0.2.0/PKG-INFO
```

### Comparing `vectordb-orm-0.1.0/LICENSE` & `vectordb_orm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vectordb-orm-0.1.0/vectordb_orm/attributes.py` & `vectordb_orm-0.2.0/vectordb_orm/attributes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from enum import Enum
-from typing import Any, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from vectordb_orm.base import MilvusBase
 
 
 class OperationType(Enum):
     """
-    Values of the operation type should correspond to the operators used in the Milvus query language
+    Types fo comparison supported by our querying language
 
     """
-    EQUALS = '=='
-    GREATER_THAN = '>'
-    LESS_THAN = '<'
-    LESS_THAN_EQUAL = '<='
-    GREATER_THAN_EQUAL = '>='
-    NOT_EQUAL = '!='
+    EQUALS = 'EQUALS'
+    GREATER_THAN = 'GREATER_THAN'
+    LESS_THAN = 'LESS_THAN'
+    LESS_THAN_EQUAL = 'LESS_THAN_EQUAL'
+    GREATER_THAN_EQUAL = 'GREATER_THAN_EQUAL'
+    NOT_EQUAL = 'NOT_EQUAL'
 
 
 class AttributeCompare:
     """
     Attributes accessed on the class level are used for query construction like filtering or retrieval. This
     class allows for Python-native comparison definition like `MyObj.text == "value"`. The operation type is
     used to construct the query expression at execution time.
@@ -41,14 +41,7 @@
         return AttributeCompare(self.base_cls, self.attr, other, OperationType.LESS_THAN)
 
     def __le__(self, other):
         return AttributeCompare(self.base_cls, self.attr, other, OperationType.LESS_THAN_EQUAL)
 
     def __ge__(self, other):
         return AttributeCompare(self.base_cls, self.attr, other, OperationType.GREATER_THAN_EQUAL)
-
-    def to_expression(self):
-        value = self.value
-        if isinstance(value, str):
-            value = f"\"{self.value}\""
-
-        return f"{self.attr} {self.op.value} {value}"
```

### Comparing `vectordb-orm-0.1.0/setup.py` & `vectordb_orm-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,139 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# vectordb-orm
 
-packages = \
-['vectordb_orm', 'vectordb_orm.tests']
+`vectordb-orm` is an Object-Relational Mapping (ORM) library designed to work with vector databases. This project aims to provide a consistent and convenient interface for working with vector data, allowing you to interact with vector databases using familiar ORM concepts and syntax. Right now [Milvus](https://milvus.io/) and [Pinecone](https://www.pinecone.io/) are supported with more backend engines planned for the future.
 
-package_data = \
-{'': ['*']}
+## Getting Started
 
-install_requires = \
-['numpy>=1.24.2,<2.0.0', 'protobuf>=4.22.3,<5.0.0', 'pymilvus>=2.2.6,<3.0.0']
-
-setup_kwargs = {
-    'name': 'vectordb-orm',
-    'version': '0.1.0',
-    'description': '',
-    'long_description': "# vectordb-orm\n\n`vectordb-orm` is an Object-Relational Mapping (ORM) library designed to work with vector databases, such as Milvus. The project aims to provide a consistent and convenient interface for working with vector data, allowing you to interact with vector databases using familiar ORM concepts and syntax.\n\n## Getting Started\n\nHere are some example code snippets demonstrating common behavior with vectordb-orm. vectordb-orm is designed around python typehints. You create a class definition by subclassing `MilvusBase` and providing typehints for the keys of your model, similar to pydantic. These fields also support custom initialization behavior if you want (or need) to modify their configuration options.\n\n| Field Type      | Description                                                                                                                                                                                                                                |\n|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|\n| BaseField       | The `BaseField` provides the ability to add a default value for a given field. This should be used in cases where the more specific field types aren't relevant.                                                                           |\n| PrimaryKeyField | The `PrimaryKeyField` is used to specify the primary key of your model, and one is required per class.                                                                                                                                     |\n| VarCharField    | The `VarCharField` is used to specify a string field, and the `EmbeddingField` is used to specify a vector field.                                                                                                                          |\n| EmbeddingField  | The `EmbeddingField` also supports specifying an index type, which is used to specify the index type for the field. The `EmbeddingField` also supports specifying a dimension, which is used to specify the dimension of the vector field. |\n\n### Object Definition\n\n```python\nfrom vectordb_orm import MilvusBase, EmbeddingField, VarCharField, PrimaryKeyField\nfrom pymilvus import Milvus\nfrom vectordb_orm.indexes import IVF_FLAT\nimport numpy as np\n\nclass MyObject(MilvusBase):\n    __collection_name__ = 'my_object_collection'\n\n    id: int = PrimaryKeyField()\n    text: str = VarCharField(max_length=128)\n    embedding: np.ndarray = EmbeddingField(dim=128, index=IVF_FLAT(cluster_units=128))\n```\n\n## Querying Syntax\n\n```python\nfrom vectordb_orm import MilvusSession\n\n# Instantiate a MilvusSession\nsession = MilvusSession()\n\n# Perform a simple boolean query\nresults = session.query(MyObject).filter(MyObject.text == 'bar').limit(2).all()\n\n# Rank results by their similarity to a given reference vector\nquery_vector = np.array([8.0]*128)\nresults = session.query(MyObject).filter(MyObject.text == 'bar').order_by_similarity(MyObject.embedding, query_vector).limit(2).all()\n```\n\n## Installation\n\nTo get started with vectordb-orm, simply install the package and its dependencies, then import the necessary modules:\n\n```bash\npip install vectordb-orm\n```\n\nWe use poetry for local development work:\n\n```bash\npoetry install\npoetry run pytest\n```\n\n## Why use an ORM?\n\nMost vector databases use a JSON-like querying syntax where schemas and objects are specified as dictionary blobs. This makes it difficult to use IDE features like autocomplete or typehinting, and also can lead to error prone code while translating between Python logic and querying syntax.\n\nAn ORM provides a high-level, abstracted interface to work with databases. This abstraction makes it easier to write, read, and maintain code, as well as to switch between different database backends with minimal changes. Furthermore, an ORM allows developers to work with databases in a more Pythonic way, using Python objects and classes instead of raw SQL queries or low-level API calls.\n\n## Comparison to SQLAlchemy\n\nWhile vectordb-orm is inspired by the widely-used SQLAlchemy ORM, it is specifically designed for vector databases, such as Milvus. This means that vectordb-orm offers unique features tailored to the needs of working with vector data, such as similarity search, index management, and efficient data storage. Although the two ORMs share some similarities in terms of syntax and structure, vectordb-orm focuses on providing a seamless experience for working with vector databases.\n\n## WIP\n\nPlease note that vectordb-orm is still a (somewhat large) work in progress. The current implementation focuses on Milvus integration, the goal is to eventually expand support to other vector databases. Contributions and feedback are welcome as we work to improve and expand the capabilities of vectordb-orm.\n",
-    'author': 'Pierce Freeman',
-    'author_email': 'pierce@freeman.vc',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+Here are some simple examples demonstrating common behavior with vectordb-orm. First a note on structure. vectordb-orm is designed around the idea of a `Schema`, which is logically equivalent to a table in classic relational databases. This schema is marked up with python typehints that define the type of vector and metadata that will be stored alongisde the objects.
 
+You create a class definition by subclassing `VectorSchemaBase` and providing typehints for the keys of your model, similar to pydantic. These fields also support custom initialization behavior if you want (or need) to modify their configuration options.
 
-setup(**setup_kwargs)
+Make sure to have a vector database running on your system before connecting. We provide an archive of the [official](https://milvus.io/docs/install_standalone-docker.md) docker-compose that's mainly used for testing Milvus. Pinecone requires your API key and environment parameters.
+
+```bash
+git clone https://github.com/piercefreeman/vectordb-orm.git
+cd vectordb-orm
+docker-compose up -d
+```
+
+| Field Type      | Description                                                                                                                                                                                                                                |
+|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| BaseField       | The `BaseField` provides the ability to add a default value for a given field. This should be used in cases where the more specific field types aren't relevant.                                                                           |
+| PrimaryKeyField | The `PrimaryKeyField` is used to specify the primary key of your model, and one is required per class.                                                                                                                                     |
+| VarCharField    | The `VarCharField` is used to specify a string field, and the `EmbeddingField` is used to specify a vector field.                                                                                                                          |
+| EmbeddingField  | The `EmbeddingField` also supports specifying an index type, which is used to specify the index type for the field. The `EmbeddingField` also supports specifying a dimension, which is used to specify the dimension of the vector field. |
+
+### Object Definition
+
+Defining a schema is almost entirely the same between backends but there are some small differences when it comes to index creation.
+
+Milvus:
+
+```python
+from vectordb_orm import VectorSchemaBase, EmbeddingField, VarCharField, PrimaryKeyField, Milvus_IVF_FLAT
+import numpy as np
+
+class MyObject(VectorSchemaBase):
+    __collection_name__ = 'my_object_collection'
+
+    id: int = PrimaryKeyField()
+    text: str = VarCharField(max_length=128)
+    embedding: np.ndarray = EmbeddingField(dim=128, index=Milvus_IVF_FLAT(cluster_units=128))
+```
+
+Pinecone:
+
+```python
+from vectordb_orm import VectorSchemaBase, EmbeddingField, VarCharField, PrimaryKeyField, PineconeIndex, PineconeSimilarityMetric
+import numpy as np
+
+class MyObject(VectorSchemaBase):
+    __collection_name__ = 'my_object_collection'
+
+    id: int = PrimaryKeyField()
+    text: str = VarCharField(max_length=128)
+    embedding: np.ndarray = EmbeddingField(dim=128, index=PineconeIndex(metric_type=PineconeSimilarityMetric.COSINE))
+```
+
+## Embedding Types
+
+We currently support two different types of embeddings: floating point and binary. We distinguish these based on the type signatures of the embedding array.
+
+For binary:
+
+```python
+embedding: np.ndarray[np.bool_] = EmbeddingField(
+    dim=128,
+    index=FLAT()
+)
+```
+
+For floating point:
+
+```python
+embedding: np.ndarray = EmbeddingField(
+    dim=128,
+    index=BIN_FLAT()
+)
+```
+
+## Querying Syntax
+
+```python
+from pymilvus import Milvus, connections
+from vectordb_orm import MilvusBackend, VectorSession
+
+# Instantiate a Milvus session
+session = VectorSession(MilvusBackend(Milvus()))
+connections.connect("default", host="localhost", port="19530")
+```
+
+```python
+from vectordb_orm import PineconeBackend, VectorSession
+
+# Instantiate a Pinecone session
+session = VectorSession(
+    PineconeBackend(
+        api_key=getenv("PINECONE_API_KEY"),
+        environment=getenv("PINECONE_ENVIRONMENT"),
+    )
+)
+```
+
+```python
+# Perform a simple boolean query
+results = session.query(MyObject).filter(MyObject.text == 'bar').limit(2).all()
+
+# Rank results by their similarity to a given reference vector
+query_vector = np.array([8.0]*128)
+results = session.query(MyObject).filter(MyObject.text == 'bar').order_by_similarity(MyObject.embedding, query_vector).limit(2).all()
+```
+
+## Installation
+
+To get started with vectordb-orm, simply install the package and its dependencies, then import the necessary modules:
+
+```bash
+pip install vectordb-orm
+```
+
+We use poetry for local development work:
+
+```bash
+poetry install
+poetry run pytest
+```
+
+## Why use an ORM?
+
+Most vector databases use a JSON-like querying syntax where schemas and objects are specified as dictionary blobs. This makes it difficult to use IDE features like autocomplete or typehinting, and also can lead to error prone code while translating between Python logic and querying syntax.
+
+An ORM provides a high-level, abstracted interface to work with databases. This abstraction makes it easier to write, read, and maintain code, as well as to switch between different database backends with minimal changes. Furthermore, an ORM allows developers to work with databases in a more Pythonic way, using Python objects and classes instead of raw SQL queries or low-level API calls.
+
+## Comparison to SQLAlchemy
+
+While vectordb-orm is inspired by the widely-used SQLAlchemy ORM, it is specifically designed for vector databases, such as Milvus. This means that vectordb-orm offers unique features tailored to the needs of working with vector data, such as similarity search, index management, and efficient data storage. Although the two ORMs share some similarities in terms of syntax and structure, vectordb-orm focuses on providing a seamless experience for working with vector databases.
+
+## WIP
+
+Please note that vectordb-orm is still a (somewhat large) work in progress. The current implementation focuses on Milvus integration; the goal is to eventually expand support to other vector databases. Contributions and feedback are welcome as we work to improve and expand the capabilities of vectordb-orm.
```

### Comparing `vectordb-orm-0.1.0/PKG-INFO` & `vectordb_orm-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,126 @@
 Metadata-Version: 2.1
 Name: vectordb-orm
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: pinecone-client (>=2.2.1,<3.0.0)
 Requires-Dist: protobuf (>=4.22.3,<5.0.0)
 Requires-Dist: pymilvus (>=2.2.6,<3.0.0)
 Description-Content-Type: text/markdown
 
 # vectordb-orm
 
-`vectordb-orm` is an Object-Relational Mapping (ORM) library designed to work with vector databases, such as Milvus. The project aims to provide a consistent and convenient interface for working with vector data, allowing you to interact with vector databases using familiar ORM concepts and syntax.
+`vectordb-orm` is an Object-Relational Mapping (ORM) library designed to work with vector databases. This project aims to provide a consistent and convenient interface for working with vector data, allowing you to interact with vector databases using familiar ORM concepts and syntax. Right now [Milvus](https://milvus.io/) and [Pinecone](https://www.pinecone.io/) are supported with more backend engines planned for the future.
 
 ## Getting Started
 
-Here are some example code snippets demonstrating common behavior with vectordb-orm. vectordb-orm is designed around python typehints. You create a class definition by subclassing `MilvusBase` and providing typehints for the keys of your model, similar to pydantic. These fields also support custom initialization behavior if you want (or need) to modify their configuration options.
+Here are some simple examples demonstrating common behavior with vectordb-orm. First a note on structure. vectordb-orm is designed around the idea of a `Schema`, which is logically equivalent to a table in classic relational databases. This schema is marked up with python typehints that define the type of vector and metadata that will be stored alongisde the objects.
+
+You create a class definition by subclassing `VectorSchemaBase` and providing typehints for the keys of your model, similar to pydantic. These fields also support custom initialization behavior if you want (or need) to modify their configuration options.
+
+Make sure to have a vector database running on your system before connecting. We provide an archive of the [official](https://milvus.io/docs/install_standalone-docker.md) docker-compose that's mainly used for testing Milvus. Pinecone requires your API key and environment parameters.
+
+```bash
+git clone https://github.com/piercefreeman/vectordb-orm.git
+cd vectordb-orm
+docker-compose up -d
+```
 
 | Field Type      | Description                                                                                                                                                                                                                                |
 |-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | BaseField       | The `BaseField` provides the ability to add a default value for a given field. This should be used in cases where the more specific field types aren't relevant.                                                                           |
 | PrimaryKeyField | The `PrimaryKeyField` is used to specify the primary key of your model, and one is required per class.                                                                                                                                     |
 | VarCharField    | The `VarCharField` is used to specify a string field, and the `EmbeddingField` is used to specify a vector field.                                                                                                                          |
 | EmbeddingField  | The `EmbeddingField` also supports specifying an index type, which is used to specify the index type for the field. The `EmbeddingField` also supports specifying a dimension, which is used to specify the dimension of the vector field. |
 
 ### Object Definition
 
+Defining a schema is almost entirely the same between backends but there are some small differences when it comes to index creation.
+
+Milvus:
+
+```python
+from vectordb_orm import VectorSchemaBase, EmbeddingField, VarCharField, PrimaryKeyField, Milvus_IVF_FLAT
+import numpy as np
+
+class MyObject(VectorSchemaBase):
+    __collection_name__ = 'my_object_collection'
+
+    id: int = PrimaryKeyField()
+    text: str = VarCharField(max_length=128)
+    embedding: np.ndarray = EmbeddingField(dim=128, index=Milvus_IVF_FLAT(cluster_units=128))
+```
+
+Pinecone:
+
 ```python
-from vectordb_orm import MilvusBase, EmbeddingField, VarCharField, PrimaryKeyField
-from pymilvus import Milvus
-from vectordb_orm.indexes import IVF_FLAT
+from vectordb_orm import VectorSchemaBase, EmbeddingField, VarCharField, PrimaryKeyField, PineconeIndex, PineconeSimilarityMetric
 import numpy as np
 
-class MyObject(MilvusBase):
+class MyObject(VectorSchemaBase):
     __collection_name__ = 'my_object_collection'
 
     id: int = PrimaryKeyField()
     text: str = VarCharField(max_length=128)
-    embedding: np.ndarray = EmbeddingField(dim=128, index=IVF_FLAT(cluster_units=128))
+    embedding: np.ndarray = EmbeddingField(dim=128, index=PineconeIndex(metric_type=PineconeSimilarityMetric.COSINE))
+```
+
+## Embedding Types
+
+We currently support two different types of embeddings: floating point and binary. We distinguish these based on the type signatures of the embedding array.
+
+For binary:
+
+```python
+embedding: np.ndarray[np.bool_] = EmbeddingField(
+    dim=128,
+    index=FLAT()
+)
+```
+
+For floating point:
+
+```python
+embedding: np.ndarray = EmbeddingField(
+    dim=128,
+    index=BIN_FLAT()
+)
 ```
 
 ## Querying Syntax
 
 ```python
-from vectordb_orm import MilvusSession
+from pymilvus import Milvus, connections
+from vectordb_orm import MilvusBackend, VectorSession
+
+# Instantiate a Milvus session
+session = VectorSession(MilvusBackend(Milvus()))
+connections.connect("default", host="localhost", port="19530")
+```
+
+```python
+from vectordb_orm import PineconeBackend, VectorSession
 
-# Instantiate a MilvusSession
-session = MilvusSession()
+# Instantiate a Pinecone session
+session = VectorSession(
+    PineconeBackend(
+        api_key=getenv("PINECONE_API_KEY"),
+        environment=getenv("PINECONE_ENVIRONMENT"),
+    )
+)
+```
 
+```python
 # Perform a simple boolean query
 results = session.query(MyObject).filter(MyObject.text == 'bar').limit(2).all()
 
 # Rank results by their similarity to a given reference vector
 query_vector = np.array([8.0]*128)
 results = session.query(MyObject).filter(MyObject.text == 'bar').order_by_similarity(MyObject.embedding, query_vector).limit(2).all()
 ```
@@ -82,9 +148,9 @@
 
 ## Comparison to SQLAlchemy
 
 While vectordb-orm is inspired by the widely-used SQLAlchemy ORM, it is specifically designed for vector databases, such as Milvus. This means that vectordb-orm offers unique features tailored to the needs of working with vector data, such as similarity search, index management, and efficient data storage. Although the two ORMs share some similarities in terms of syntax and structure, vectordb-orm focuses on providing a seamless experience for working with vector databases.
 
 ## WIP
 
-Please note that vectordb-orm is still a (somewhat large) work in progress. The current implementation focuses on Milvus integration, the goal is to eventually expand support to other vector databases. Contributions and feedback are welcome as we work to improve and expand the capabilities of vectordb-orm.
+Please note that vectordb-orm is still a (somewhat large) work in progress. The current implementation focuses on Milvus integration; the goal is to eventually expand support to other vector databases. Contributions and feedback are welcome as we work to improve and expand the capabilities of vectordb-orm.
```

