# Comparing `tmp/pygismeteo_base-4.1.0.tar.gz` & `tmp/pygismeteo_base-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygismeteo_base-4.1.0.tar", max compression
+gzip compressed data, was "pygismeteo_base-4.2.0.tar", max compression
```

## Comparing `pygismeteo_base-4.1.0.tar` & `pygismeteo_base-4.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1065 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/LICENSE
--rw-r--r--   0        0        0      553 2023-04-19 13:39:46.260706 pygismeteo_base-4.1.0/README.md
--rw-r--r--   0        0        0       86 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/__init__.py
--rw-r--r--   0        0        0       92 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/constants.py
--rw-r--r--   0        0        0      755 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/current.py
--rw-r--r--   0        0        0      392 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/endpoint.py
--rw-r--r--   0        0        0      812 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/http.py
--rw-r--r--   0        0        0      309 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/__init__.py
--rw-r--r--   0        0        0     1812 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/current.py
--rw-r--r--   0        0        0      759 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/search_by_coordinates.py
--rw-r--r--   0        0        0      673 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/search_by_ip.py
--rw-r--r--   0        0        0      783 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/search_by_query.py
--rw-r--r--   0        0        0     2908 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/step24.py
--rw-r--r--   0        0        0     1786 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/step3.py
--rw-r--r--   0        0        0     1803 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/models/step6.py
--rw-r--r--   0        0        0        0 2023-04-16 13:33:22.269443 pygismeteo_base-4.1.0/pygismeteo_base/py.typed
--rw-r--r--   0        0        0      955 2023-04-16 13:33:22.279443 pygismeteo_base-4.1.0/pygismeteo_base/search.py
--rw-r--r--   0        0        0        0 2023-04-16 13:33:22.279443 pygismeteo_base-4.1.0/pygismeteo_base/step_n/__init__.py
--rw-r--r--   0        0        0     1246 2023-04-16 13:33:22.279443 pygismeteo_base-4.1.0/pygismeteo_base/step_n/abc.py
--rw-r--r--   0        0        0     1604 2023-04-16 13:33:22.279443 pygismeteo_base-4.1.0/pygismeteo_base/step_n/mixins.py
--rw-r--r--   0        0        0     1453 2023-04-16 14:30:28.989419 pygismeteo_base-4.1.0/pygismeteo_base/types.py
--rw-r--r--   0        0        0     1017 2023-04-16 13:33:22.279443 pygismeteo_base-4.1.0/pygismeteo_base/validators.py
--rw-r--r--   0        0        0     2706 2023-04-19 13:23:14.550693 pygismeteo_base-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 pygismeteo_base-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/LICENSE
+-rw-r--r--   0        0        0      553 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/README.md
+-rw-r--r--   0        0        0       86 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/__init__.py
+-rw-r--r--   0        0        0       92 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/constants.py
+-rw-r--r--   0        0        0      925 2023-04-21 19:11:10.073668 pygismeteo_base-4.2.0/pygismeteo_base/current.py
+-rw-r--r--   0        0        0      392 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/endpoint.py
+-rw-r--r--   0        0        0      901 2023-04-21 19:29:03.763651 pygismeteo_base-4.2.0/pygismeteo_base/http.py
+-rw-r--r--   0        0        0      309 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/__init__.py
+-rw-r--r--   0        0        0     1812 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/current.py
+-rw-r--r--   0        0        0      759 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/search_by_coordinates.py
+-rw-r--r--   0        0        0      673 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/search_by_ip.py
+-rw-r--r--   0        0        0      783 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/search_by_query.py
+-rw-r--r--   0        0        0     2908 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/step24.py
+-rw-r--r--   0        0        0     1786 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/step3.py
+-rw-r--r--   0        0        0     1803 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/step6.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/py.typed
+-rw-r--r--   0        0        0     1149 2023-04-21 19:25:53.063683 pygismeteo_base-4.2.0/pygismeteo_base/search.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/step_n/__init__.py
+-rw-r--r--   0        0        0     1433 2023-04-21 19:08:58.453658 pygismeteo_base-4.2.0/pygismeteo_base/step_n/abc.py
+-rw-r--r--   0        0        0     1604 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/step_n/mixins.py
+-rw-r--r--   0        0        0     1217 2023-04-21 19:39:40.203642 pygismeteo_base-4.2.0/pygismeteo_base/types.py
+-rw-r--r--   0        0        0      400 2023-04-21 18:50:04.713658 pygismeteo_base-4.2.0/pygismeteo_base/typing_compat.py
+-rw-r--r--   0        0        0      815 2023-04-21 18:44:17.243666 pygismeteo_base-4.2.0/pygismeteo_base/validators.py
+-rw-r--r--   0        0        0     2706 2023-04-21 19:43:49.973683 pygismeteo_base-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 pygismeteo_base-4.2.0/PKG-INFO
```

### Comparing `pygismeteo_base-4.1.0/LICENSE` & `pygismeteo_base-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.1.0/README.md` & `pygismeteo_base-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.1.0/pygismeteo_base/http.py` & `pygismeteo_base-4.2.0/pygismeteo_base/http.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,19 @@
     def __init__(self, session: Optional[T], settings: validators.Settings) -> None:
         self.session = session
         self.settings = settings
 
     def _get_params_and_headers(
         self, params: types.Params
     ) -> Tuple[types.Params, types.Headers]:
-        lang_dict = {"lang": self.settings.lang} if self.settings.lang else {}
-        params_dict = params or {}
+        if self.settings.lang:
+            params = (
+                {"lang": self.settings.lang, **params}
+                if params
+                else {"lang": self.settings.lang}
+            )
         token = self.settings.token or constants.DEFAULT_TOKEN
-        return {**lang_dict, **params_dict}, {"X-Gismeteo-Token": token}
+        headers = {"X-Gismeteo-Token": token}
+        return params, headers
 
 
 THttpClient = TypeVar("THttpClient", bound=BaseHttpClient[Any])
```

### Comparing `pygismeteo_base-4.1.0/pygismeteo_base/models/current.py` & `pygismeteo_base-4.2.0/pygismeteo_base/models/current.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.1.0/pygismeteo_base/models/search_by_coordinates.py` & `pygismeteo_base-4.2.0/pygismeteo_base/models/search_by_coordinates.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.1.0/pygismeteo_base/models/search_by_ip.py` & `pygismeteo_base-4.2.0/pygismeteo_base/models/search_by_ip.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.1.0/pygismeteo_base/models/search_by_query.py` & `pygismeteo_base-4.2.0/pygismeteo_base/models/search_by_query.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.1.0/pygismeteo_base/models/step24.py` & `pygismeteo_base-4.2.0/pygismeteo_base/models/step24.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.1.0/pygismeteo_base/models/step3.py` & `pygismeteo_base-4.2.0/pygismeteo_base/models/step3.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.1.0/pygismeteo_base/models/step6.py` & `pygismeteo_base-4.2.0/pygismeteo_base/models/step6.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.1.0/pygismeteo_base/search.py` & `pygismeteo_base-4.2.0/pygismeteo_base/current.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from __future__ import annotations
 
+from typing import Tuple
+
 from . import http, types, validators
 from .endpoint import EndpointABC
 
 
-class SearchBase(EndpointABC[http.THttpClient]):
+class CurrentBase(EndpointABC[http.THttpClient]):
     __slots__ = ()
 
     @property
     def _endpoint(self) -> str:
-        return "search/cities"
+        return "weather/current"
 
-    @staticmethod
     def _get_params_by_coordinates(
-        latitude: float, longitude: float, *, limit: types.SearchLimit
-    ) -> types.Params:
-        coordinates = validators.Coordinates(latitude=latitude, longitude=longitude)
-        params = coordinates.dict()
-        lim = validators.SearchLimit.parse_obj(limit).__root__
-        return dict(params, limit=lim)
-
-    @staticmethod
-    def _get_params_by_ip(ip: str) -> types.Params:
-        ip = str(validators.IPAddress.parse_obj(ip).__root__)
-        return {"ip": ip}
-
-    @staticmethod
-    def _get_params_by_query(query: str) -> types.Params:
-        query = validators.Query.parse_obj(query).__root__
-        return {"query": query}
+        self, latitude: float, longitude: float
+    ) -> Tuple[str, types.Params]:
+        coords_validator = validators.Coordinates(
+            latitude=latitude, longitude=longitude
+        )
+        params = {
+            "latitude": str(coords_validator.latitude),
+            "longitude": str(coords_validator.longitude),
+        }
+        return self._endpoint, params
+
+    def _get_params_by_id(self, id: int) -> Tuple[str, types.Params]:  # noqa: A002
+        id_validator = validators.LocalityID.parse_obj(id)
+        url = f"{self._endpoint}/{id_validator.__root__}"
+        return url, None
```

### Comparing `pygismeteo_base-4.1.0/pygismeteo_base/step_n/abc.py` & `pygismeteo_base-4.2.0/pygismeteo_base/search.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 from __future__ import annotations
 
-from abc import abstractmethod
-from typing import Tuple, Type, Union
+from ipaddress import IPv4Address
+from typing import Union
 
-from .. import http, types, validators
-from ..endpoint import EndpointABC
+from . import http, types, validators
+from .endpoint import EndpointABC
 
 
-class StepNABC(EndpointABC[http.THttpClient]):
+class SearchBase(EndpointABC[http.THttpClient]):
     __slots__ = ()
 
     @property
-    @abstractmethod
-    def _model(self) -> types.StepNModel:
-        pass
-
-    @property
-    @abstractmethod
-    def _days_validator(
-        self,
-    ) -> Type[Union[validators.Step3Days, validators.Step6or24Days]]:
-        pass
+    def _endpoint(self) -> str:
+        return "search/cities"
 
+    @staticmethod
     def _get_params_by_coordinates(
-        self, latitude: float, longitude: float, *, days: Union[str, int]
-    ) -> Tuple[str, types.Params]:
-        coords = validators.Coordinates(latitude=latitude, longitude=longitude)
-        days_model = self._days_validator.parse_obj(days)
-        params = dict(coords.dict(), days=days_model.__root__)
-        return self._endpoint, params
-
-    def _get_params_by_id(
-        self, id: int, *, days: Union[str, int]  # noqa: A002
-    ) -> Tuple[str, types.Params]:
-        id_model = validators.LocalityID.parse_obj(id)
-        url = f"{self._endpoint}/{id_model.__root__}"
-        days_model = self._days_validator.parse_obj(days)
-        params = {"days": days_model.__root__}
-        return url, params
+        latitude: float, longitude: float, *, limit: types.SearchLimit
+    ) -> types.Params:
+        coords_validator = validators.Coordinates(
+            latitude=latitude, longitude=longitude
+        )
+        limit_validator = validators.SearchLimit.parse_obj(limit)
+        return {
+            "latitude": str(coords_validator.latitude),
+            "longitude": str(coords_validator.longitude),
+            "limit": str(limit_validator.__root__),
+        }
+
+    @staticmethod
+    def _get_params_by_ip(ip: Union[IPv4Address, str]) -> types.Params:
+        ip_validator = validators.IPAddress.parse_obj(ip)
+        return {"ip": str(ip_validator.__root__)}
+
+    @staticmethod
+    def _get_params_by_query(query: str) -> types.Params:
+        return {"query": str(query)}
```

### Comparing `pygismeteo_base-4.1.0/pygismeteo_base/step_n/mixins.py` & `pygismeteo_base-4.2.0/pygismeteo_base/step_n/mixins.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.1.0/pygismeteo_base/types.py` & `pygismeteo_base-4.2.0/pygismeteo_base/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 from __future__ import annotations
 
-import sys
 from typing import Mapping, Optional, Type, TypeVar, Union
 
 from . import models
-
-if sys.version_info < (3, 10):  # pragma: <3.10 cover
-    from typing_extensions import TypeAlias
-else:  # pragma: >=3.10 cover
-    from typing import TypeAlias
-
-if sys.version_info < (3, 8):  # pragma: <3.8 cover
-    from typing_extensions import Literal
-else:  # pragma: >=3.8 cover
-    from typing import Literal
+from .typing_compat import Literal, TypeAlias
 
 Lang: TypeAlias = Literal["ru", "en", "ua", "lt", "lv", "pl", "ro"]
 Step3Days: TypeAlias = Literal[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
 Step6or24Days: TypeAlias = Literal[3, 4, 5, 6, 7, 8, 9, 10]
-Params: TypeAlias = Optional[Mapping[str, Union[str, int, float]]]
-Headers: TypeAlias = Mapping[str, str]
+StepNDays: TypeAlias = Union[Step3Days, Step6or24Days]
+Params: TypeAlias = Optional[Mapping[str, str]]
+Headers: TypeAlias = Optional[Mapping[str, str]]
 SearchLimit: TypeAlias = Literal[
     1,
     2,
     3,
     4,
     5,
     6,
```

### Comparing `pygismeteo_base-4.1.0/pygismeteo_base/validators.py` & `pygismeteo_base-4.2.0/pygismeteo_base/validators.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,40 +13,30 @@
     token: Optional[str] = Field(...)
 
     class Config:
         anystr_strip_whitespace = True
         validate_assignment = True
 
 
-class ImmutableModel(BaseModel):
-    class Config:
-        allow_mutation = False
-        anystr_strip_whitespace = True
-
-
-class Coordinates(ImmutableModel):
+class Coordinates(BaseModel):
     latitude: float = Field(ge=-90, le=90)
     longitude: float = Field(ge=-180, le=180)
 
 
-class SearchLimit(ImmutableModel):
+class SearchLimit(BaseModel):
     __root__: int = Field(ge=1, le=36)
 
 
-class IPAddress(ImmutableModel):
+class IPAddress(BaseModel):
     __root__: IPv4Address
 
 
-class Query(ImmutableModel):
-    __root__: str
-
-
-class LocalityID(ImmutableModel):
+class LocalityID(BaseModel):
     __root__: int = Field(ge=1)
 
 
-class Step3Days(ImmutableModel):
+class Step3Days(BaseModel):
     __root__: int = Field(ge=1, le=10)
 
 
-class Step6or24Days(ImmutableModel):
+class Step6or24Days(BaseModel):
     __root__: int = Field(ge=3, le=10)
```

### Comparing `pygismeteo_base-4.1.0/pyproject.toml` & `pygismeteo_base-4.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygismeteo-base"
-version = "4.1.0"
+version = "4.2.0"
 description = "Base for pygismeteo and aiopygismeteo"
 authors = ["monosans <hsyqixco@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/monosans/pygismeteo-base"
 classifiers = [
     "Environment :: Web Environment",
@@ -29,15 +29,15 @@
 pydantic = "^1.9"
 typing-extensions = { version = ">=3.7.4.3,<5", python = "<3.10" }
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 mypy = "1.2.0"
 pre-commit = "2.21.0"
-ruff = "0.0.261"
+ruff = "0.0.262"
 
 [tool.black]
 target-version = ["py37"]
 skip-magic-trailing-comma = true
 preview = true
 
 [tool.mypy]
```

### Comparing `pygismeteo_base-4.1.0/PKG-INFO` & `pygismeteo_base-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygismeteo-base
-Version: 4.1.0
+Version: 4.2.0
 Summary: Base for pygismeteo and aiopygismeteo
 Home-page: https://github.com/monosans/pygismeteo-base
 License: MIT
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
```

