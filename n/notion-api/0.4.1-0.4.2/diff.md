# Comparing `tmp/notion_api-0.4.1.tar.gz` & `tmp/notion_api-0.4.2.tar.gz`

## Comparing `notion_api-0.4.1.tar` & `notion_api-0.4.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11253 2020-02-02 00:00:00.000000 notion_api-0.4.1/README.md
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/py.typed
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/__init__.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/_about.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/_pkgv.py
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/blockmixin.py
--rw-r--r--   0        0        0    20946 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/blocktypefactory.py
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/client.py
--rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/notionblock.py
--rw-r--r--   0        0        0    26159 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/notiondatabase.py
--rw-r--r--   0        0        0    20435 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/notionpage.py
--rw-r--r--   0        0        0    15457 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/api/notionworkspace.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/exceptions/__init__.py
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/exceptions/errors.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/exceptions/validate.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/__init__.py
--rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/blocktypes.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/build.py
--rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/common.py
--rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/files.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/options.py
--rw-r--r--   0        0        0    14699 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/propertyobjects.py
--rw-r--r--   0        0        0    15442 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/propertyvalues.py
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/properties/richtext.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/propertyitems/__init__.py
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/propertyitems/base.py
--rw-r--r--   0        0        0     8508 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/propertyitems/call.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/query/__init__.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/query/compound.py
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/query/conditions.py
--rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/query/propfilter.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/query/sort.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 notion_api-0.4.1/notion/query/timestamp.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 notion_api-0.4.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 notion_api-0.4.1/LICENSE
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 notion_api-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    12717 2020-02-02 00:00:00.000000 notion_api-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11253 2020-02-02 00:00:00.000000 notion_api-0.4.2/README.md
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/py.typed
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/__init__.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/_about.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/_pkgv.py
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/blockmixin.py
+-rw-r--r--   0        0        0    20946 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/blocktypefactory.py
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/client.py
+-rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/notionblock.py
+-rw-r--r--   0        0        0    26159 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/notiondatabase.py
+-rw-r--r--   0        0        0    20211 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/notionpage.py
+-rw-r--r--   0        0        0    15457 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/notionworkspace.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/exceptions/__init__.py
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/exceptions/errors.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/exceptions/validate.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/__init__.py
+-rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/blocktypes.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/build.py
+-rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/common.py
+-rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/files.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/options.py
+-rw-r--r--   0        0        0    14699 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/propertyobjects.py
+-rw-r--r--   0        0        0    15442 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/propertyvalues.py
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/richtext.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/propertyitems/__init__.py
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/propertyitems/base.py
+-rw-r--r--   0        0        0     8508 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/propertyitems/call.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/query/__init__.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/query/compound.py
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/query/conditions.py
+-rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/query/propfilter.py
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/query/sort.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/query/timestamp.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 notion_api-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 notion_api-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 notion_api-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    12717 2020-02-02 00:00:00.000000 notion_api-0.4.2/PKG-INFO
```

### Comparing `notion_api-0.4.1/README.md` & `notion_api-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/__init__.py` & `notion_api-0.4.2/notion/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/api/__init__.py` & `notion_api-0.4.2/notion/api/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/api/_about.py` & `notion_api-0.4.2/notion/api/_about.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "__package_url__",
     "__package_json__",
 )
 
 __notion_version__: Final[str] = "2022-06-28"
 __content_type__: Final[str] = "application/json"
 __base_url__: Final[str] = "https://api.notion.com/v1/"
-__version__: Final[str] = "0.4.1"
+__version__: Final[str] = "0.4.2"
 __package_url__: Final[str] = "https://pypi.org/pypi/notion-api/"
 __package_json__: Final[str] = "https://pypi.org/pypi/notion-api/json"
 
 
 # Notion API Changlog
 # https://developers.notion.com/page/changelog
```

### Comparing `notion_api-0.4.1/notion/api/_pkgv.py` & `notion_api-0.4.2/notion/api/_pkgv.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/api/blockmixin.py` & `notion_api-0.4.2/notion/api/blockmixin.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/api/blocktypefactory.py` & `notion_api-0.4.2/notion/api/blocktypefactory.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/api/client.py` & `notion_api-0.4.2/notion/api/client.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/api/notionblock.py` & `notion_api-0.4.2/notion/api/notionblock.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/api/notiondatabase.py` & `notion_api-0.4.2/notion/api/notiondatabase.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/api/notionpage.py` & `notion_api-0.4.2/notion/api/notionpage.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,24 +20,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
 from datetime import datetime
 from functools import cached_property
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Iterator,
-    MutableMapping,
-    Optional,
-    Sequence,
-    Union,
-    cast,
-)
+from typing import TYPE_CHECKING, Any, MutableMapping, Optional, Sequence, Union, cast
 
 from notion.api.blockmixin import _TokenBlockMixin
 from notion.api.client import _NLOG
 from notion.api.notionblock import Block
 from notion.api.notiondatabase import Database
 from notion.properties.build import build_payload
 from notion.properties.common import Parent, UserObject, _NotionUUID
@@ -159,30 +150,24 @@
 
         return cls_
 
     def __getattr__(self, attr: str) -> PropertyItem:
         def lower_alnum(s: str) -> str:
             return "".join([c if c.isalnum() else "_" for c in s]).lower()
 
-        for property in self:
+        for property in self.properties:
             if lower_alnum(attr) == lower_alnum(property):
                 return PropertyItem(
                     map=self.retrieve_property_item(property), source_page=self.id
                 )
 
         raise AttributeError(f"{attr} not found in page property values.")
 
-    def __contains__(self, property_name: str) -> bool:
-        return property_name in self.properties
-
-    def __iter__(self) -> Iterator[str]:
-        return iter(self.properties)
-
     def __getitem__(self, property_name: str) -> MutableMapping[str, Any]:
-        if property_name in self:
+        if property_name in self.properties:
             return cast(MutableMapping[str, Any], self.properties[property_name])
         raise KeyError(f"{property_name} not found in page property values.")
 
     @cached_property
     def properties(self) -> MutableMapping[str, Any]:
         return cast(MutableMapping[str, Any], self.retrieve()["properties"])
```

### Comparing `notion_api-0.4.1/notion/api/notionworkspace.py` & `notion_api-0.4.2/notion/api/notionworkspace.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/exceptions/__init__.py` & `notion_api-0.4.2/notion/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/exceptions/errors.py` & `notion_api-0.4.2/notion/exceptions/errors.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/exceptions/validate.py` & `notion_api-0.4.2/notion/exceptions/validate.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/properties/__init__.py` & `notion_api-0.4.2/notion/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/properties/blocktypes.py` & `notion_api-0.4.2/notion/properties/blocktypes.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/properties/build.py` & `notion_api-0.4.2/notion/properties/build.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/properties/common.py` & `notion_api-0.4.2/notion/properties/common.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/properties/files.py` & `notion_api-0.4.2/notion/properties/files.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/properties/options.py` & `notion_api-0.4.2/notion/properties/options.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/properties/propertyobjects.py` & `notion_api-0.4.2/notion/properties/propertyobjects.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/properties/propertyvalues.py` & `notion_api-0.4.2/notion/properties/propertyvalues.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/properties/richtext.py` & `notion_api-0.4.2/notion/properties/richtext.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/propertyitems/__init__.py` & `notion_api-0.4.2/notion/propertyitems/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/propertyitems/base.py` & `notion_api-0.4.2/notion/propertyitems/base.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/propertyitems/call.py` & `notion_api-0.4.2/notion/propertyitems/call.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/query/__init__.py` & `notion_api-0.4.2/notion/query/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/query/compound.py` & `notion_api-0.4.2/notion/query/compound.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/query/conditions.py` & `notion_api-0.4.2/notion/query/conditions.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/query/propfilter.py` & `notion_api-0.4.2/notion/query/propfilter.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/query/sort.py` & `notion_api-0.4.2/notion/query/sort.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/notion/query/timestamp.py` & `notion_api-0.4.2/notion/query/timestamp.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/.gitignore` & `notion_api-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/LICENSE` & `notion_api-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/pyproject.toml` & `notion_api-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.1/PKG-INFO` & `notion_api-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-api
-Version: 0.4.1
+Version: 0.4.2
 Summary: An unofficial wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion.
 Project-URL: Homepage, https://github.com/ayvi-0001/notion-api
 Project-URL: Source Code, https://github.com/ayvi-0001/notion-api
 Author-email: Alan Vickers <alan.k.vickers@gmail.com>
 License-File: LICENSE
 Keywords: notion-api,notion-version-2022-06-28,wrapper
 Classifier: Development Status :: 3 - Alpha
```

