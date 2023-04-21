# Comparing `tmp/pokelance-0.0.9a0.tar.gz` & `tmp/pokelance-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokelance-0.0.9a0.tar", max compression
+gzip compressed data, was "pokelance-0.1.0.tar", max compression
```

## Comparing `pokelance-0.0.9a0.tar` & `pokelance-0.1.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1089 2022-12-10 11:13:03.511548 pokelance-0.0.9a0/LICENSE
--rw-r--r--   0        0        0      113 2023-01-15 15:29:42.503617 pokelance-0.0.9a0/pokelance/__init__.py
--rw-r--r--   0        0        0      440 2022-12-11 17:08:17.590957 pokelance-0.0.9a0/pokelance/cache/__init__.py
--rw-r--r--   0        0        0    11402 2022-12-20 18:48:39.115038 pokelance-0.0.9a0/pokelance/cache/cache.py
--rw-r--r--   0        0        0    13281 2022-12-11 17:08:17.582941 pokelance-0.0.9a0/pokelance/cache/cache_manager.py
--rw-r--r--   0        0        0     7220 2022-12-20 12:38:38.895456 pokelance-0.0.9a0/pokelance/client.py
--rw-r--r--   0        0        0     4029 2023-01-15 15:29:04.733511 pokelance-0.0.9a0/pokelance/exceptions.py
--rw-r--r--   0        0        0      557 2022-12-11 13:38:48.112513 pokelance-0.0.9a0/pokelance/ext/__init__.py
--rw-r--r--   0        0        0     2752 2022-12-16 15:19:02.709295 pokelance-0.0.9a0/pokelance/ext/_base.py
--rw-r--r--   0        0        0     8283 2022-12-12 08:19:49.122292 pokelance-0.0.9a0/pokelance/ext/berry.py
--rw-r--r--   0        0        0     8305 2022-12-12 08:50:00.325832 pokelance-0.0.9a0/pokelance/ext/contest.py
--rw-r--r--   0        0        0     8518 2022-12-12 08:19:49.153538 pokelance-0.0.9a0/pokelance/ext/encounter.py
--rw-r--r--   0        0        0     5848 2022-12-12 09:36:06.045977 pokelance-0.0.9a0/pokelance/ext/evolution.py
--rw-r--r--   0        0        0     9663 2022-12-12 08:19:49.122292 pokelance-0.0.9a0/pokelance/ext/game.py
--rw-r--r--   0        0        0    12868 2022-12-12 08:19:49.137914 pokelance-0.0.9a0/pokelance/ext/item.py
--rw-r--r--   0        0        0    10380 2022-12-12 08:19:49.106655 pokelance-0.0.9a0/pokelance/ext/location.py
--rw-r--r--   0        0        0     3218 2022-12-12 08:19:49.137914 pokelance-0.0.9a0/pokelance/ext/machine.py
--rw-r--r--   0        0        0    17794 2022-12-12 08:19:49.153538 pokelance-0.0.9a0/pokelance/ext/move.py
--rw-r--r--   0        0        0    37654 2022-12-16 15:22:25.618475 pokelance-0.0.9a0/pokelance/ext/pokemon.py
--rw-r--r--   0        0        0     4915 2023-01-15 15:14:32.904490 pokelance-0.0.9a0/pokelance/http/__init__.py
--rw-r--r--   0        0        0    20788 2023-01-15 14:53:37.103076 pokelance-0.0.9a0/pokelance/http/endpoints.py
--rw-r--r--   0        0        0     8879 2023-01-12 15:18:29.781435 pokelance-0.0.9a0/pokelance/languages.py
--rw-r--r--   0        0        0     3705 2022-12-20 18:51:58.101341 pokelance-0.0.9a0/pokelance/logger.py
--rw-r--r--   0        0        0     2026 2023-01-11 15:01:47.770702 pokelance-0.0.9a0/pokelance/models/__init__.py
--rw-r--r--   0        0        0      553 2022-12-11 20:07:41.544812 pokelance-0.0.9a0/pokelance/models/_base.py
--rw-r--r--   0        0        0     1953 2022-12-14 07:51:07.459692 pokelance-0.0.9a0/pokelance/models/abstract/__init__.py
--rw-r--r--   0        0        0     5673 2022-12-12 10:01:29.037738 pokelance-0.0.9a0/pokelance/models/abstract/berry.py
--rw-r--r--   0        0        0     4198 2022-12-12 10:01:29.005834 pokelance-0.0.9a0/pokelance/models/abstract/contest.py
--rw-r--r--   0        0        0     3612 2022-12-12 10:01:29.045625 pokelance-0.0.9a0/pokelance/models/abstract/encounter.py
--rw-r--r--   0        0        0     2477 2022-12-12 09:29:14.458132 pokelance-0.0.9a0/pokelance/models/abstract/evolution.py
--rw-r--r--   0        0        0     7819 2022-12-12 10:01:29.030788 pokelance-0.0.9a0/pokelance/models/abstract/game.py
--rw-r--r--   0        0        0     9018 2022-12-12 10:07:49.062544 pokelance-0.0.9a0/pokelance/models/abstract/item.py
--rw-r--r--   0        0        0     6884 2022-12-12 10:01:29.017252 pokelance-0.0.9a0/pokelance/models/abstract/location.py
--rw-r--r--   0        0        0     1261 2022-12-12 10:02:12.153337 pokelance-0.0.9a0/pokelance/models/abstract/machine.py
--rw-r--r--   0        0        0    13071 2022-12-12 10:07:49.076966 pokelance-0.0.9a0/pokelance/models/abstract/move.py
--rw-r--r--   0        0        0    36150 2023-01-12 15:16:55.376161 pokelance-0.0.9a0/pokelance/models/abstract/pokemon.py
--rw-r--r--   0        0        0    20518 2022-12-14 07:45:21.884450 pokelance-0.0.9a0/pokelance/models/abstract/showdown.py
--rw-r--r--   0        0        0     2601 2022-12-11 11:50:28.534022 pokelance-0.0.9a0/pokelance/models/abstract/utils/__init__.py
--rw-r--r--   0        0        0     1539 2022-12-11 18:59:05.329462 pokelance-0.0.9a0/pokelance/models/abstract/utils/berries.py
--rw-r--r--   0        0        0      978 2022-12-12 10:07:49.053540 pokelance-0.0.9a0/pokelance/models/abstract/utils/contests.py
--rw-r--r--   0        0        0     6291 2022-12-15 17:00:51.853687 pokelance-0.0.9a0/pokelance/models/abstract/utils/evolutions.py
--rw-r--r--   0        0        0      921 2022-12-12 10:07:49.024480 pokelance-0.0.9a0/pokelance/models/abstract/utils/games.py
--rw-r--r--   0        0        0     2362 2022-12-12 10:07:49.068442 pokelance-0.0.9a0/pokelance/models/abstract/utils/items.py
--rw-r--r--   0        0        0     3655 2022-12-12 10:07:49.084482 pokelance-0.0.9a0/pokelance/models/abstract/utils/locations.py
--rw-r--r--   0        0        0     7275 2022-12-12 10:07:49.031476 pokelance-0.0.9a0/pokelance/models/abstract/utils/moves.py
--rw-r--r--   0        0        0    43239 2023-01-12 15:16:55.402704 pokelance-0.0.9a0/pokelance/models/abstract/utils/pokemons.py
--rw-r--r--   0        0        0      684 2023-01-11 15:01:47.945064 pokelance-0.0.9a0/pokelance/models/common/__init__.py
--rw-r--r--   0        0        0    11207 2023-01-11 15:09:24.211629 pokelance-0.0.9a0/pokelance/models/common/models.py
--rw-r--r--   0        0        0     1112 2022-12-11 18:59:05.425975 pokelance-0.0.9a0/pokelance/models/common/resources.py
--rw-r--r--   0        0        0        0 2022-12-10 11:13:00.835196 pokelance-0.0.9a0/pokelance/py.typed
--rw-r--r--   0        0        0     1169 2023-01-15 15:29:42.494758 pokelance-0.0.9a0/pyproject.toml
--rw-r--r--   0        0        0     3762 2023-01-15 15:14:39.817070 pokelance-0.0.9a0/README.md
--rw-r--r--   0        0        0     4693 1970-01-01 00:00:00.000000 pokelance-0.0.9a0/setup.py
--rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 pokelance-0.0.9a0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-21 15:29:11.374173 pokelance-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3658 2023-04-21 15:29:11.374173 pokelance-0.1.0/README.md
+-rw-r--r--   0        0        0      106 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/__init__.py
+-rw-r--r--   0        0        0      431 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/cache/__init__.py
+-rw-r--r--   0        0        0    14534 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/cache/cache.py
+-rw-r--r--   0        0        0    13942 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/cache/cache_manager.py
+-rw-r--r--   0        0        0     8907 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/client.py
+-rw-r--r--   0        0        0     3725 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/constants.py
+-rw-r--r--   0        0        0     3868 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/exceptions.py
+-rw-r--r--   0        0        0      530 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/__init__.py
+-rw-r--r--   0        0        0     3163 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/_base.py
+-rw-r--r--   0        0        0     7196 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/berry.py
+-rw-r--r--   0        0        0     7189 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/contest.py
+-rw-r--r--   0        0        0     7747 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/encounter.py
+-rw-r--r--   0        0        0     4990 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/evolution.py
+-rw-r--r--   0        0        0     8348 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/game.py
+-rw-r--r--   0        0        0    11273 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/item.py
+-rw-r--r--   0        0        0     9049 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/location.py
+-rw-r--r--   0        0        0     2625 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/machine.py
+-rw-r--r--   0        0        0    15682 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/move.py
+-rw-r--r--   0        0        0    33460 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/pokemon.py
+-rw-r--r--   0        0        0     4724 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/http/__init__.py
+-rw-r--r--   0        0        0    20467 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/http/endpoints.py
+-rw-r--r--   0        0        0     8683 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/languages.py
+-rw-r--r--   0        0        0     3588 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/logger.py
+-rw-r--r--   0        0        0     1919 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/__init__.py
+-rw-r--r--   0        0        0      529 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/_base.py
+-rw-r--r--   0        0        0     1873 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/__init__.py
+-rw-r--r--   0        0        0     5528 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/berry.py
+-rw-r--r--   0        0        0     4083 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/contest.py
+-rw-r--r--   0        0        0     3507 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/encounter.py
+-rw-r--r--   0        0        0     2410 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/evolution.py
+-rw-r--r--   0        0        0     7628 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/game.py
+-rw-r--r--   0        0        0     8794 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/item.py
+-rw-r--r--   0        0        0     6706 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/location.py
+-rw-r--r--   0        0        0     1222 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/machine.py
+-rw-r--r--   0        0        0    12765 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/move.py
+-rw-r--r--   0        0        0    35329 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/pokemon.py
+-rw-r--r--   0        0        0     1351 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/showdown.py
+-rw-r--r--   0        0        0     2506 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/__init__.py
+-rw-r--r--   0        0        0     1494 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/berries.py
+-rw-r--r--   0        0        0      943 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/contests.py
+-rw-r--r--   0        0        0     6255 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/evolutions.py
+-rw-r--r--   0        0        0      890 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/games.py
+-rw-r--r--   0        0        0     2284 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/items.py
+-rw-r--r--   0        0        0     3546 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/locations.py
+-rw-r--r--   0        0        0     7112 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/moves.py
+-rw-r--r--   0        0        0    42172 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/pokemons.py
+-rw-r--r--   0        0        0      650 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/common/__init__.py
+-rw-r--r--   0        0        0    10868 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/common/models.py
+-rw-r--r--   0        0        0     1063 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/common/resources.py
+-rw-r--r--   0        0        0        0 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/py.typed
+-rw-r--r--   0        0        0     1114 2023-04-21 15:29:11.382173 pokelance-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4404 1970-01-01 00:00:00.000000 pokelance-0.1.0/PKG-INFO
```

### Comparing `pokelance-0.0.9a0/LICENSE` & `pokelance-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 FallenDeity
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 FallenDeity
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pokelance-0.0.9a0/pokelance/ext/__init__.py` & `pokelance-0.1.0/pokelance/ext/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import typing as t
-
-from ._base import BaseExtension
-from .berry import Berry
-from .contest import Contest
-from .encounter import Encounter
-from .evolution import Evolution
-from .game import Game
-from .item import Item
-from .location import Location
-from .machine import Machine
-from .move import Move
-from .pokemon import Pokemon
-
-__all__: t.Tuple[str, ...] = (
-    "BaseExtension",
-    "Berry",
-    "Contest",
-    "Encounter",
-    "Evolution",
-    "Game",
-    "Item",
-    "Location",
-    "Machine",
-    "Move",
-    "Pokemon",
-)
+import typing as t
+
+from ._base import BaseExtension
+from .berry import Berry
+from .contest import Contest
+from .encounter import Encounter
+from .evolution import Evolution
+from .game import Game
+from .item import Item
+from .location import Location
+from .machine import Machine
+from .move import Move
+from .pokemon import Pokemon
+
+__all__: t.Tuple[str, ...] = (
+    "BaseExtension",
+    "Berry",
+    "Contest",
+    "Encounter",
+    "Evolution",
+    "Game",
+    "Item",
+    "Location",
+    "Machine",
+    "Move",
+    "Pokemon",
+)
```

### Comparing `pokelance-0.0.9a0/pokelance/ext/_base.py` & `pokelance-0.1.0/pokelance/ext/_base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,102 @@
-import typing as t
-from difflib import get_close_matches
-
-from pokelance.exceptions import ResourceNotFound
-
-if t.TYPE_CHECKING:
-    from pokelance.cache import BaseCache, Cache
-    from pokelance.http import HttpClient, Route
-
-
-__all__: t.Tuple[str, ...] = ("BaseExtension",)
-_KT = t.TypeVar("_KT", bound="Route")
-_VT = t.TypeVar("_VT")
-
-
-class BaseExtension:
-    """The base extension class.
-
-    Parameters
-    ----------
-    client: pokelance.http.HttpClient
-        The client to use for requests.
-
-    Attributes
-    ----------
-    _client: pokelance.http.HttpClient
-        The client to use for requests.
-    _cache: pokelance.cache.Cache
-        The cache to use for requests.
-    """
-
-    _cache: "Cache"
-
-    def __init__(self, client: "HttpClient") -> None:
-        """Initializes the extension.
-
-        Parameters
-        ----------
-        client: pokelance.http.HttpClient
-            The client to use for requests.
-
-        Returns
-        -------
-        pokelance.ext.BaseExtension
-            The extension.
-        """
-        self._client = client
-        self._cache = self._client.cache
-
-    def _validate_resource(self, cache: "BaseCache[_KT, _VT]", resource: t.Union[str, int], route: "Route") -> None:
-        """Validates a resource.
-
-        Parameters
-        ----------
-        cache: pokelance.cache.BaseCache[typing.Any, typing.Any]
-            The cache to use for the validation.
-        resource: typing.Union[str, int]
-            The resource to validate.
-        route: pokelance.http.Route
-            The route to use for the validation.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The resource was not found in the cache.
-        """
-        data: t.Set[str] = set(list(map(str, cache.endpoints.values())) + list(cache.endpoints.keys()))
-        if data and str(resource) not in data:
-            raise ResourceNotFound(self.get_message(str(resource), data), route)
-
-    @staticmethod
-    def get_message(case: str, data: t.Set[str]) -> str:
-        """Gets the error message for a resource not found error.
-
-        Parameters
-        ----------
-        case: str
-            The case to use for the error message.
-        data: typing.Set[str]
-            The data to use for the error message.
-
-        Returns
-        -------
-        str
-            The error message.
-        """
-        matches = get_close_matches(case, data, n=10, cutoff=0.5)
-        if matches:
-            return f"Resource not found. Did you mean {', '.join(matches)}?"
-        return "Resource not found."
-
-    async def setup(self) -> None:
-        """Sets up the extension."""
-        ...
+import typing as t
+from difflib import get_close_matches
+
+from pokelance.exceptions import ResourceNotFound
+from pokelance.http import Endpoint
+
+if t.TYPE_CHECKING:
+    from pokelance.cache import BaseCache, Cache
+    from pokelance.http import HttpClient, Route
+    from pokelance.models import BaseModel
+
+
+__all__: t.Tuple[str, ...] = ("BaseExtension",)
+_KT = t.TypeVar("_KT", bound="Route")
+_VT = t.TypeVar("_VT", bound="BaseModel")
+
+
+class BaseExtension:
+    """The base extension class.
+
+    Parameters
+    ----------
+    client: pokelance.http.HttpClient
+        The client to use for requests.
+
+    Attributes
+    ----------
+    _client: pokelance.http.HttpClient
+        The client to use for requests.
+    _cache: pokelance.cache.Cache
+        The cache to use for requests.
+    """
+
+    _cache: "Cache"
+
+    def __init__(self, client: "HttpClient") -> None:
+        """Initializes the extension.
+
+        Parameters
+        ----------
+        client: pokelance.http.HttpClient
+            The client to use for requests.
+
+        Returns
+        -------
+        pokelance.ext.BaseExtension
+            The extension.
+        """
+        self._client = client
+        self._cache = self._client.cache
+        self.cache = getattr(self._cache, self.__class__.__name__.lower())
+
+    def _validate_resource(self, cache: "BaseCache[_KT, _VT]", resource: t.Union[str, int], route: "Route") -> None:
+        """Validates a resource.
+
+        Parameters
+        ----------
+        cache: pokelance.cache.BaseCache[typing.Any, typing.Any]
+            The cache to use for the validation.
+        resource: typing.Union[str, int]
+            The resource to validate.
+        route: pokelance.http.Route
+            The route to use for the validation.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The resource was not found in the cache.
+        """
+        data: t.Set[str] = set(list(map(str, cache.endpoints.values())) + list(cache.endpoints.keys()))
+        if data and str(resource) not in data:
+            raise ResourceNotFound(self.get_message(str(resource), data), route)
+
+    @staticmethod
+    def get_message(case: str, data: t.Set[str]) -> str:
+        """Gets the error message for a resource not found error.
+
+        Parameters
+        ----------
+        case: str
+            The case to use for the error message.
+        data: typing.Set[str]
+            The data to use for the error message.
+
+        Returns
+        -------
+        str
+            The error message.
+        """
+        matches = get_close_matches(case, data, n=10, cutoff=0.5)
+        if matches:
+            return f"Resource not found. Did you mean {', '.join(matches)}?"
+        return "Resource not found."
+
+    async def setup(self) -> None:
+        """Sets up the extension."""
+        for item in dir(self):
+            if item.startswith("fetch_"):
+                data = await self._client.request(
+                    t.cast(t.Callable[[], "Route"], getattr(Endpoint, f"get_{item[6:]}_endpoints"))()
+                )
+                self._cache.load_documents(str(self.__class__.__name__), item[6:], data["results"])
```

### Comparing `pokelance-0.0.9a0/pokelance/ext/berry.py` & `pokelance-0.1.0/pokelance/ext/berry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,249 +1,232 @@
-import typing as t
-
-from pokelance.http import Endpoint
-from pokelance.models import Berry as BerryModel
-from pokelance.models import BerryFirmness, BerryFlavor
-
-from ._base import BaseExtension
-
-if t.TYPE_CHECKING:
-    from pokelance import PokeLance
-    from pokelance.http import HttpClient
-
-
-__all__: t.Tuple[str, ...] = (
-    "setup",
-    "Berry",
-)
-
-
-class Berry(BaseExtension):
-    """Extension for berry related endpoints.
-
-    Parameters
-    ----------
-    client: pokelance.http.HttpClient
-        The client to use for requests.
-
-    Attributes
-    ----------
-    cache: pokelance.cache.Berry
-        The cache for this extension.
-
-    """
-
-    def __init__(self, client: "HttpClient") -> None:
-        """Initializes the extension."""
-        super().__init__(client)
-        self.cache = self._cache.berry
-
-    async def setup(self) -> None:
-        """Sets up the extension."""
-        data = await self._client.request(Endpoint.get_berry_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "berry", data["results"])
-        data = await self._client.request(Endpoint.get_berry_flavor_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "berry_flavor", data["results"])
-        data = await self._client.request(Endpoint.get_berry_firmness_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "berry_firmness", data["results"])
-
-    def get_berry(self, name: t.Union[str, int]) -> t.Optional[BerryModel]:
-        """Gets a berry from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the berry.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.Berry]
-            The berry if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the berry is invalid.
-
-        Examples
-        -------
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> berry = client.berry.get_berry("cheri")  # None if not cached
-        >>> berry.name
-        'cheri'
-        """
-        route = Endpoint.get_berry(name)
-        self._validate_resource(self.cache.berry, name, route)
-        return self.cache.berry.get(route, None)
-
-    async def fetch_berry(self, name: t.Union[str, int]) -> t.Optional[BerryModel]:
-        """Fetches a berry from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the berry.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.Berry]
-            The berry if it exists in the API, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the berry is invalid.
-
-        Examples
-        -------
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     berry = await client.berry.fetch_berry("cheri")
-        ...     print(berry.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        cheri
-        """
-        route = Endpoint.get_berry(name)
-        self._validate_resource(self.cache.berry, name, route)
-        data = await self._client.request(route)
-        return self.cache.berry.setdefault(route, BerryModel.from_payload(data))
-
-    def get_berry_flavor(self, name: t.Union[str, int]) -> t.Optional[BerryFlavor]:
-        """Gets a berry flavor from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the berry flavor.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.BerryFlavor]
-            The berry flavor if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the berry flavor is invalid.
-
-        Examples
-        -------
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> berry_flavor = client.berry.get_berry_flavor("spicy")  # None if not cached
-        >>> berry_flavor.name
-        'spicy'
-        """
-        route = Endpoint.get_berry_flavor(name)
-        self._validate_resource(self.cache.berry_flavor, name, route)
-        return self.cache.berry_flavor.get(route, None)
-
-    async def fetch_berry_flavor(self, name: t.Union[str, int]) -> t.Optional[BerryFlavor]:
-        """Fetches a berry flavor from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the berry flavor.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.BerryFlavor]
-            The berry flavor if it exists in the API, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the berry flavor is invalid.
-
-        Examples
-        -------
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     berry_flavor = await client.berry.fetch_berry_flavor("spicy")
-        ...     print(berry_flavor.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        spicy
-        """
-        route = Endpoint.get_berry_flavor(name)
-        self._validate_resource(self.cache.berry_flavor, name, route)
-        data = await self._client.request(route)
-        self.cache.berry_flavor[route] = BerryFlavor.from_payload(data)
-        return self.cache.berry_flavor[route]
-
-    def get_berry_firmness(self, name: t.Union[str, int]) -> t.Optional[BerryFirmness]:
-        """Gets a berry firmness from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the berry firmness.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.BerryFirmness]
-            The berry firmness if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the berry firmness is invalid.
-
-        Examples
-        -------
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> berry_firmness = client.berry.get_berry_firmness("very-soft")  # None if not cached
-        >>> berry_firmness.name
-        'very-soft'
-        """
-        route = Endpoint.get_berry_firmness(name)
-        self._validate_resource(self.cache.berry_firmness, name, route)
-        return self.cache.berry_firmness.get(route, None)
-
-    async def fetch_berry_firmness(self, name: t.Union[str, int]) -> t.Optional[BerryFirmness]:
-        """Fetches a berry firmness from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the berry firmness.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.BerryFirmness]
-            The berry firmness if it exists in the API, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the berry firmness is invalid.
-
-        Examples
-        -------
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     berry_firmness = await client.berry.fetch_berry_firmness("very-soft")
-        ...     print(berry_firmness.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        very-soft
-        """
-        route = Endpoint.get_berry_firmness(name)
-        self._validate_resource(self.cache.berry_firmness, name, route)
-        data = await self._client.request(route)
-        self.cache.berry_firmness[route] = BerryFirmness.from_payload(data)
-        return self.cache.berry_firmness[route]
-
-
-def setup(lance: "PokeLance") -> None:
-    """Sets up the berry cog."""
-    lance.add_extension("berry", Berry(lance.http))
+import typing as t
+
+from pokelance.http import Endpoint
+from pokelance.models import Berry as BerryModel
+from pokelance.models import BerryFirmness, BerryFlavor
+
+from ._base import BaseExtension
+
+if t.TYPE_CHECKING:
+    from pokelance import PokeLance
+    from pokelance.cache import Berry as BerryCache
+
+
+__all__: t.Tuple[str, ...] = (
+    "setup",
+    "Berry",
+)
+
+
+class Berry(BaseExtension):
+    """
+    Extension for berry related endpoints.
+
+    Attributes
+    ----------
+    cache: pokelance.cache.Berry
+        The cache for this extension.
+    """
+
+    cache: "BerryCache"
+
+    def get_berry(self, name: t.Union[str, int]) -> t.Optional[BerryModel]:
+        """Gets a berry from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the berry.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.Berry]
+            The berry if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the berry is invalid.
+
+        Examples
+        -------
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> berry = client.berry.get_berry("cheri")  # None if not cached
+        >>> berry.name
+        'cheri'
+        """
+        route = Endpoint.get_berry(name)
+        self._validate_resource(self.cache.berry, name, route)
+        return self.cache.berry.get(route, None)
+
+    async def fetch_berry(self, name: t.Union[str, int]) -> t.Optional[BerryModel]:
+        """Fetches a berry from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the berry.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.Berry]
+            The berry if it exists in the API, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the berry is invalid.
+
+        Examples
+        -------
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     berry = await client.berry.fetch_berry("cheri")
+        ...     print(berry.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        cheri
+        """
+        route = Endpoint.get_berry(name)
+        self._validate_resource(self.cache.berry, name, route)
+        data = await self._client.request(route)
+        return self.cache.berry.setdefault(route, BerryModel.from_payload(data))
+
+    def get_berry_flavor(self, name: t.Union[str, int]) -> t.Optional[BerryFlavor]:
+        """Gets a berry flavor from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the berry flavor.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.BerryFlavor]
+            The berry flavor if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the berry flavor is invalid.
+
+        Examples
+        -------
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> berry_flavor = client.berry.get_berry_flavor("spicy")  # None if not cached
+        >>> berry_flavor.name
+        'spicy'
+        """
+        route = Endpoint.get_berry_flavor(name)
+        self._validate_resource(self.cache.berry_flavor, name, route)
+        return self.cache.berry_flavor.get(route, None)
+
+    async def fetch_berry_flavor(self, name: t.Union[str, int]) -> t.Optional[BerryFlavor]:
+        """Fetches a berry flavor from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the berry flavor.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.BerryFlavor]
+            The berry flavor if it exists in the API, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the berry flavor is invalid.
+
+        Examples
+        -------
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     berry_flavor = await client.berry.fetch_berry_flavor("spicy")
+        ...     print(berry_flavor.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        spicy
+        """
+        route = Endpoint.get_berry_flavor(name)
+        self._validate_resource(self.cache.berry_flavor, name, route)
+        data = await self._client.request(route)
+        self.cache.berry_flavor[route] = BerryFlavor.from_payload(data)
+        return self.cache.berry_flavor[route]
+
+    def get_berry_firmness(self, name: t.Union[str, int]) -> t.Optional[BerryFirmness]:
+        """Gets a berry firmness from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the berry firmness.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.BerryFirmness]
+            The berry firmness if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the berry firmness is invalid.
+
+        Examples
+        -------
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> berry_firmness = client.berry.get_berry_firmness("very-soft")  # None if not cached
+        >>> berry_firmness.name
+        'very-soft'
+        """
+        route = Endpoint.get_berry_firmness(name)
+        self._validate_resource(self.cache.berry_firmness, name, route)
+        return self.cache.berry_firmness.get(route, None)
+
+    async def fetch_berry_firmness(self, name: t.Union[str, int]) -> t.Optional[BerryFirmness]:
+        """Fetches a berry firmness from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the berry firmness.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.BerryFirmness]
+            The berry firmness if it exists in the API, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the berry firmness is invalid.
+
+        Examples
+        -------
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     berry_firmness = await client.berry.fetch_berry_firmness("very-soft")
+        ...     print(berry_firmness.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        very-soft
+        """
+        route = Endpoint.get_berry_firmness(name)
+        self._validate_resource(self.cache.berry_firmness, name, route)
+        data = await self._client.request(route)
+        self.cache.berry_firmness[route] = BerryFirmness.from_payload(data)
+        return self.cache.berry_firmness[route]
+
+
+def setup(lance: "PokeLance") -> None:
+    """Sets up the berry cog."""
+    lance.add_extension("berry", Berry(lance.http))
```

### Comparing `pokelance-0.0.9a0/pokelance/ext/encounter.py` & `pokelance-0.1.0/pokelance/ext/encounter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,236 +1,235 @@
-import typing as t
-
-from pokelance.http import Endpoint
-from pokelance.models import EncounterCondition, EncounterConditionValue, EncounterMethod
-
-from ._base import BaseExtension
-
-if t.TYPE_CHECKING:
-    from pokelance import PokeLance
-    from pokelance.http import HttpClient
-
-
-__all__: t.Tuple[str, ...] = (
-    "setup",
-    "Encounter",
-)
-
-
-class Encounter(BaseExtension):
-    def __init__(self, client: "HttpClient") -> None:
-        super().__init__(client)
-        self.cache = self._cache.encounter
-
-    async def setup(self) -> None:
-        data = await self._client.request(Endpoint.get_encounter_condition_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "encounter_condition", data["results"])
-        data = await self._client.request(Endpoint.get_encounter_method_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "encounter_method", data["results"])
-        data = await self._client.request(Endpoint.get_encounter_condition_value_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "encounter_condition_value", data["results"])
-
-    def get_encounter_condition(self, name: t.Union[str, int]) -> t.Optional[EncounterCondition]:
-        """Gets an encounter condition from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the encounter condition.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.EncounterCondition]
-            The encounter condition if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the encounter condition is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> condition = client.encounter.get_encounter_condition("swarm")
-        >>> condition.name
-        'swarm'
-        """
-        route = Endpoint.get_encounter_condition(name)
-        self._validate_resource(self.cache.encounter_condition, name, route)
-        return self.cache.encounter_condition.get(route, None)
-
-    async def fetch_encounter_condition(self, name: t.Union[str, int]) -> t.Optional[EncounterCondition]:
-        """Fetches an encounter condition from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the encounter condition.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.EncounterCondition]
-            The encounter condition if it exists in the API, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the encounter condition is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     condition = await client.encounter.fetch_encounter_condition("swarm")
-        ...     print(condition.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        swarm
-        """
-        route = Endpoint.get_encounter_condition(name)
-        self._validate_resource(self.cache.encounter_condition, name, route)
-        data = await self._client.request(route)
-        return self.cache.encounter_condition.setdefault(route, EncounterCondition.from_payload(data))
-
-    def get_encounter_condition_value(self, name: t.Union[str, int]) -> t.Optional[EncounterConditionValue]:
-        """Gets an encounter condition value from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the encounter condition value.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.EncounterConditionValue]
-            The encounter condition value if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the encounter condition value is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> condition = client.encounter.get_encounter_condition_value("swarm-yes")
-        >>> condition.name
-        'swarm-yes'
-        """
-        route = Endpoint.get_encounter_condition_value(name)
-        self._validate_resource(self.cache.encounter_condition_value, name, route)
-        return self.cache.encounter_condition_value.get(route, None)
-
-    async def fetch_encounter_condition_value(self, name: t.Union[str, int]) -> t.Optional[EncounterConditionValue]:
-        """Fetches an encounter condition value from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the encounter condition value.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.EncounterConditionValue]
-            The encounter condition value if it exists in the API, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the encounter condition value is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     condition = await client.encounter.fetch_encounter_condition_value("swarm-yes")
-        ...     print(condition.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        swarm-yes
-        """
-        route = Endpoint.get_encounter_condition_value(name)
-        self._validate_resource(self.cache.encounter_condition_value, name, route)
-        data = await self._client.request(route)
-        return self.cache.encounter_condition_value.setdefault(route, EncounterConditionValue.from_payload(data))
-
-    def get_encounter_method(self, name: t.Union[str, int]) -> t.Optional[EncounterMethod]:
-        """Gets an encounter method from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the encounter method.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.EncounterMethod]
-            The encounter method if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the encounter method is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> method = client.encounter.get_encounter_method("walk")
-        >>> method.name
-        'walk'
-        """
-        route = Endpoint.get_encounter_method(name)
-        self._validate_resource(self.cache.encounter_method, name, route)
-        return self.cache.encounter_method.get(route, None)
-
-    async def fetch_encounter_method(self, name: t.Union[str, int]) -> t.Optional[EncounterMethod]:
-        """Fetches an encounter method from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the encounter method.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.EncounterMethod]
-            The encounter method if it exists in the API, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the encounter method is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     method = await client.encounter.fetch_encounter_method("walk")
-        ...     print(method.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        walk
-        """
-        route = Endpoint.get_encounter_method(name)
-        self._validate_resource(self.cache.encounter_method, name, route)
-        data = await self._client.request(route)
-        return self.cache.encounter_method.setdefault(route, EncounterMethod.from_payload(data))
-
-
-def setup(lance: "PokeLance") -> None:
-    """Sets up the encounter cog."""
-    lance.add_extension("encounter", Encounter(lance.http))
+import typing as t
+
+from pokelance.http import Endpoint
+from pokelance.models import EncounterCondition, EncounterConditionValue, EncounterMethod
+
+from ._base import BaseExtension
+
+if t.TYPE_CHECKING:
+    from pokelance import PokeLance
+    from pokelance.cache import Encounter as EncounterCache
+
+
+__all__: t.Tuple[str, ...] = (
+    "setup",
+    "Encounter",
+)
+
+
+class Encounter(BaseExtension):
+    """
+    Extension for encounter related endpoints.
+
+    Attributes
+    ----------
+    cache: pokelance.cache.Encounter
+        The cache for this extension.
+    """
+
+    cache: "EncounterCache"
+
+    def get_encounter_condition(self, name: t.Union[str, int]) -> t.Optional[EncounterCondition]:
+        """Gets an encounter condition from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the encounter condition.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.EncounterCondition]
+            The encounter condition if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the encounter condition is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> condition = client.encounter.get_encounter_condition("swarm")
+        >>> condition.name
+        'swarm'
+        """
+        route = Endpoint.get_encounter_condition(name)
+        self._validate_resource(self.cache.encounter_condition, name, route)
+        return self.cache.encounter_condition.get(route, None)
+
+    async def fetch_encounter_condition(self, name: t.Union[str, int]) -> t.Optional[EncounterCondition]:
+        """Fetches an encounter condition from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the encounter condition.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.EncounterCondition]
+            The encounter condition if it exists in the API, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the encounter condition is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     condition = await client.encounter.fetch_encounter_condition("swarm")
+        ...     print(condition.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        swarm
+        """
+        route = Endpoint.get_encounter_condition(name)
+        self._validate_resource(self.cache.encounter_condition, name, route)
+        data = await self._client.request(route)
+        return self.cache.encounter_condition.setdefault(route, EncounterCondition.from_payload(data))
+
+    def get_encounter_condition_value(self, name: t.Union[str, int]) -> t.Optional[EncounterConditionValue]:
+        """Gets an encounter condition value from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the encounter condition value.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.EncounterConditionValue]
+            The encounter condition value if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the encounter condition value is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> condition = client.encounter.get_encounter_condition_value("swarm-yes")
+        >>> condition.name
+        'swarm-yes'
+        """
+        route = Endpoint.get_encounter_condition_value(name)
+        self._validate_resource(self.cache.encounter_condition_value, name, route)
+        return self.cache.encounter_condition_value.get(route, None)
+
+    async def fetch_encounter_condition_value(self, name: t.Union[str, int]) -> t.Optional[EncounterConditionValue]:
+        """Fetches an encounter condition value from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the encounter condition value.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.EncounterConditionValue]
+            The encounter condition value if it exists in the API, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the encounter condition value is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     condition = await client.encounter.fetch_encounter_condition_value("swarm-yes")
+        ...     print(condition.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        swarm-yes
+        """
+        route = Endpoint.get_encounter_condition_value(name)
+        self._validate_resource(self.cache.encounter_condition_value, name, route)
+        data = await self._client.request(route)
+        return self.cache.encounter_condition_value.setdefault(route, EncounterConditionValue.from_payload(data))
+
+    def get_encounter_method(self, name: t.Union[str, int]) -> t.Optional[EncounterMethod]:
+        """Gets an encounter method from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the encounter method.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.EncounterMethod]
+            The encounter method if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the encounter method is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> method = client.encounter.get_encounter_method("walk")
+        >>> method.name
+        'walk'
+        """
+        route = Endpoint.get_encounter_method(name)
+        self._validate_resource(self.cache.encounter_method, name, route)
+        return self.cache.encounter_method.get(route, None)
+
+    async def fetch_encounter_method(self, name: t.Union[str, int]) -> t.Optional[EncounterMethod]:
+        """Fetches an encounter method from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the encounter method.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.EncounterMethod]
+            The encounter method if it exists in the API, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the encounter method is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     method = await client.encounter.fetch_encounter_method("walk")
+        ...     print(method.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        walk
+        """
+        route = Endpoint.get_encounter_method(name)
+        self._validate_resource(self.cache.encounter_method, name, route)
+        data = await self._client.request(route)
+        return self.cache.encounter_method.setdefault(route, EncounterMethod.from_payload(data))
+
+
+def setup(lance: "PokeLance") -> None:
+    """Sets up the encounter cog."""
+    lance.add_extension("encounter", Encounter(lance.http))
```

### Comparing `pokelance-0.0.9a0/pokelance/ext/evolution.py` & `pokelance-0.1.0/pokelance/ext/evolution.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,182 +1,168 @@
-import typing as t
-
-from pokelance.http import Endpoint
-from pokelance.models import EvolutionChain, EvolutionTrigger
-
-from ._base import BaseExtension
-
-if t.TYPE_CHECKING:
-    from pokelance import PokeLance
-    from pokelance.http import HttpClient
-
-
-__all__: t.Tuple[str, ...] = (
-    "setup",
-    "Evolution",
-)
-
-
-class Evolution(BaseExtension):
-    """Extension for evolution related endpoints.
-
-    Parameters
-    ----------
-    client: pokelance.http.HttpClient
-        The client to use for requests.
-
-    Attributes
-    ----------
-    cache: pokelance.cache.Evolution
-        The cache for this extension.
-    """
-
-    def __init__(self, client: "HttpClient") -> None:
-        """Initializes the extension."""
-        super().__init__(client)
-        self.cache = self._cache.evolution
-
-    async def setup(self) -> None:
-        """Sets up the extension."""
-        data = await self._client.request(Endpoint.get_evolution_chain_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "evolution_chain", data["results"])
-        data = await self._client.request(Endpoint.get_evolution_trigger_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "evolution_trigger", data["results"])
-
-    def get_evolution_chain(self, id_: int) -> t.Optional[EvolutionChain]:
-        """Gets an evolution chain from the cache.
-
-        Parameters
-        ----------
-        id_: int
-            The name or id of the encounter method.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.EvolutionChain]
-            The evolution chain if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the evolution chain is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> chain = client.evolution.get_evolution_chain(1)
-        >>> chain.id
-        1
-        """
-        route = Endpoint.get_evolution_chain(id_)
-        self._validate_resource(self.cache.evolution_chain, id_, route)
-        return self.cache.evolution_chain.get(route, None)
-
-    async def fetch_evolution_chain(self, id_: int) -> t.Optional[EvolutionChain]:
-        """Fetches an evolution chain from the API.
-
-        Parameters
-        ----------
-        id_: int
-            The name or id of the encounter method.
-
-        Returns
-        -------
-        t.Optional[pokelance.models.EvolutionChain]
-            The evolution chain.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the evolution chain is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     chain = await client.evolution.fetch_evolution_chain(1)
-        ...     print(chain.id)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        1
-        """
-        route = Endpoint.get_evolution_chain(id_)
-        self._validate_resource(self.cache.evolution_chain, id_, route)
-        data = await self._client.request(route)
-        return self.cache.evolution_chain.setdefault(route, EvolutionChain.from_payload(data))
-
-    def get_evolution_trigger(self, name: t.Union[str, int]) -> t.Optional[EvolutionTrigger]:
-        """Gets an evolution trigger from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the encounter method.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.EvolutionTrigger]
-            The evolution trigger if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the evolution trigger is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> trigger = client.evolution.get_evolution_trigger(1)
-        >>> trigger.name
-        'level-up'
-        """
-        route = Endpoint.get_evolution_trigger(name)
-        self._validate_resource(self.cache.evolution_trigger, name, route)
-        return self.cache.evolution_trigger.get(route, None)
-
-    async def fetch_evolution_trigger(self, name: t.Union[str, int]) -> t.Optional[EvolutionTrigger]:
-        """Fetches an evolution trigger from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the encounter method.
-
-        Returns
-        -------
-        t.Optional[pokelance.models.EvolutionTrigger]
-            The evolution trigger.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the evolution trigger is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     trigger = await client.evolution.fetch_evolution_trigger(1)
-        ...     print(trigger.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        level-up
-        """
-        route = Endpoint.get_evolution_trigger(name)
-        self._validate_resource(self.cache.evolution_trigger, name, route)
-        data = await self._client.request(route)
-        return self.cache.evolution_trigger.setdefault(route, EvolutionTrigger.from_payload(data))
-
-
-def setup(lance: "PokeLance") -> None:
-    """Sets up the evolution cog."""
-    lance.add_extension("evolution", Evolution(lance.http))
+import typing as t
+
+from pokelance.http import Endpoint
+from pokelance.models import EvolutionChain, EvolutionTrigger
+
+from ._base import BaseExtension
+
+if t.TYPE_CHECKING:
+    from pokelance import PokeLance
+    from pokelance.cache import Evolution as EvolutionCache
+
+
+__all__: t.Tuple[str, ...] = (
+    "setup",
+    "Evolution",
+)
+
+
+class Evolution(BaseExtension):
+    """
+    Extension for evolution related endpoints.
+
+    Attributes
+    ----------
+    cache: pokelance.cache.Evolution
+        The cache for this extension.
+    """
+
+    cache: "EvolutionCache"
+
+    def get_evolution_chain(self, id_: int) -> t.Optional[EvolutionChain]:
+        """Gets an evolution chain from the cache.
+
+        Parameters
+        ----------
+        id_: int
+            The name or id of the encounter method.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.EvolutionChain]
+            The evolution chain if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the evolution chain is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> chain = client.evolution.get_evolution_chain(1)
+        >>> chain.id
+        1
+        """
+        route = Endpoint.get_evolution_chain(id_)
+        self._validate_resource(self.cache.evolution_chain, id_, route)
+        return self.cache.evolution_chain.get(route, None)
+
+    async def fetch_evolution_chain(self, id_: int) -> t.Optional[EvolutionChain]:
+        """Fetches an evolution chain from the API.
+
+        Parameters
+        ----------
+        id_: int
+            The name or id of the encounter method.
+
+        Returns
+        -------
+        t.Optional[pokelance.models.EvolutionChain]
+            The evolution chain.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the evolution chain is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     chain = await client.evolution.fetch_evolution_chain(1)
+        ...     print(chain.id)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        1
+        """
+        route = Endpoint.get_evolution_chain(id_)
+        self._validate_resource(self.cache.evolution_chain, id_, route)
+        data = await self._client.request(route)
+        return self.cache.evolution_chain.setdefault(route, EvolutionChain.from_payload(data))
+
+    def get_evolution_trigger(self, name: t.Union[str, int]) -> t.Optional[EvolutionTrigger]:
+        """Gets an evolution trigger from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the encounter method.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.EvolutionTrigger]
+            The evolution trigger if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the evolution trigger is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> trigger = client.evolution.get_evolution_trigger(1)
+        >>> trigger.name
+        'level-up'
+        """
+        route = Endpoint.get_evolution_trigger(name)
+        self._validate_resource(self.cache.evolution_trigger, name, route)
+        return self.cache.evolution_trigger.get(route, None)
+
+    async def fetch_evolution_trigger(self, name: t.Union[str, int]) -> t.Optional[EvolutionTrigger]:
+        """Fetches an evolution trigger from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the encounter method.
+
+        Returns
+        -------
+        t.Optional[pokelance.models.EvolutionTrigger]
+            The evolution trigger.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the evolution trigger is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     trigger = await client.evolution.fetch_evolution_trigger(1)
+        ...     print(trigger.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        level-up
+        """
+        route = Endpoint.get_evolution_trigger(name)
+        self._validate_resource(self.cache.evolution_trigger, name, route)
+        data = await self._client.request(route)
+        return self.cache.evolution_trigger.setdefault(route, EvolutionTrigger.from_payload(data))
+
+
+def setup(lance: "PokeLance") -> None:
+    """Sets up the evolution cog."""
+    lance.add_extension("evolution", Evolution(lance.http))
```

### Comparing `pokelance-0.0.9a0/pokelance/ext/game.py` & `pokelance-0.1.0/pokelance/ext/game.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,300 +1,283 @@
-import typing as t
-
-from pokelance.http import Endpoint
-from pokelance.models import Generation, Pokedex, Version, VersionGroup
-
-from ._base import BaseExtension
-
-if t.TYPE_CHECKING:
-    from pokelance import PokeLance
-    from pokelance.http import HttpClient
-
-
-__all__: t.Tuple[str, ...] = (
-    "setup",
-    "Game",
-)
-
-
-class Game(BaseExtension):
-    """Extension for game related endpoints.
-
-    Parameters
-    ----------
-    client: pokelance.http.HttpClient
-        The client to use for requests.
-
-    Attributes
-    ----------
-    cache: pokelance.cache.Game
-        The cache to use for caching resources.
-    """
-
-    def __init__(self, client: "HttpClient") -> None:
-        """Initializes the game extension."""
-        super().__init__(client)
-        self.cache = self._cache.game
-
-    async def setup(self) -> None:
-        """Sets up the game extension."""
-        data = await self._client.request(Endpoint.get_generation_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "generation", data["results"])
-        data = await self._client.request(Endpoint.get_pokedex_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "pokedex", data["results"])
-        data = await self._client.request(Endpoint.get_version_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "version", data["results"])
-        data = await self._client.request(Endpoint.get_version_group_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "version_group", data["results"])
-
-    def get_generation(self, name: t.Union[str, int]) -> t.Optional[Generation]:
-        """Gets a generation from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the generation.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.Generation]
-            The generation if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the generation is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> generation = client.game.get_generation(1)
-        >>> generation.id
-        1
-        """
-        route = Endpoint.get_generation(name)
-        self._validate_resource(self.cache.generation, name, route)
-        return self.cache.generation.get(route, None)
-
-    async def fetch_generation(self, name: t.Union[str, int]) -> t.Optional[Generation]:
-        """Fetches a generation from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the generation.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the generation is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     generation = await client.game.fetch_generation(1)
-        ...     print(generation.id)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        1
-        """
-        route = Endpoint.get_generation(name)
-        self._validate_resource(self.cache.generation, name, route)
-        data = await self._client.request(route)
-        return self.cache.generation.setdefault(route, Generation.from_payload(data))
-
-    def get_pokedex(self, name: t.Union[str, int]) -> t.Optional[Pokedex]:
-        """Gets a pokedex from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the pokedex.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.Pokedex]
-            The pokedex if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the pokedex is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> pokedex = client.game.get_pokedex(1)
-        >>> pokedex.region
-        None
-        """
-        route = Endpoint.get_pokedex(name)
-        self._validate_resource(self.cache.pokedex, name, route)
-        return self.cache.pokedex.get(route, None)
-
-    async def fetch_pokedex(self, name: t.Union[str, int]) -> t.Optional[Pokedex]:
-        """Fetches a pokedex from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the pokedex.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the pokedex is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     pokedex = await client.game.fetch_pokedex(1)
-        ...     print(pokedex.region)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        None
-        """
-        route = Endpoint.get_pokedex(name)
-        self._validate_resource(self.cache.pokedex, name, route)
-        data = await self._client.request(route)
-        return self.cache.pokedex.setdefault(route, Pokedex.from_payload(data))
-
-    def get_version(self, name: t.Union[str, int]) -> t.Optional[Version]:
-        """Gets a version from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the version.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.Version]
-            The version if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the version is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> version = client.game.get_version(1)
-        >>> version.name
-        'red'
-        """
-        route = Endpoint.get_version(name)
-        self._validate_resource(self.cache.version, name, route)
-        return self.cache.version.get(route, None)
-
-    async def fetch_version(self, name: t.Union[str, int]) -> t.Optional[Version]:
-        """Fetches a version from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the version.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the version is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     version = await client.game.fetch_version(1)
-        ...     print(version.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        red
-        """
-        route = Endpoint.get_version(name)
-        self._validate_resource(self.cache.version, name, route)
-        data = await self._client.request(route)
-        return self.cache.version.setdefault(route, Version.from_payload(data))
-
-    def get_version_group(self, name: t.Union[str, int]) -> t.Optional[VersionGroup]:
-        """Gets a version group from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the version group.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.VersionGroup]
-            The version group if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the version group is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> version_group = client.game.get_version_group(1)
-        >>> version_group.id
-        1
-        """
-        route = Endpoint.get_version_group(name)
-        self._validate_resource(self.cache.version_group, name, route)
-        return self.cache.version_group.get(route, None)
-
-    async def fetch_version_group(self, name: t.Union[str, int]) -> t.Optional[VersionGroup]:
-        """Fetches a version group from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the version group.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the version group is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     version_group = await client.game.fetch_version_group(1)
-        ...     print(version_group.id)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        1
-        """
-        route = Endpoint.get_version_group(name)
-        self._validate_resource(self.cache.version_group, name, route)
-        data = await self._client.request(route)
-        return self.cache.version_group.setdefault(route, VersionGroup.from_payload(data))
-
-
-def setup(lance: "PokeLance") -> None:
-    """Sets up the game cog."""
-    lance.add_extension("game", Game(lance.http))
+import typing as t
+
+from pokelance.http import Endpoint
+from pokelance.models import Generation, Pokedex, Version, VersionGroup
+
+from ._base import BaseExtension
+
+if t.TYPE_CHECKING:
+    from pokelance import PokeLance
+    from pokelance.cache import Game as GameCache
+
+
+__all__: t.Tuple[str, ...] = (
+    "setup",
+    "Game",
+)
+
+
+class Game(BaseExtension):
+    """
+    Extension for game related endpoints.
+
+    Attributes
+    ----------
+    cache: pokelance.cache.Game
+        The cache to use for caching resources.
+
+    """
+
+    cache: "GameCache"
+
+    def get_generation(self, name: t.Union[str, int]) -> t.Optional[Generation]:
+        """Gets a generation from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the generation.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.Generation]
+            The generation if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the generation is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> generation = client.game.get_generation(1)
+        >>> generation.id
+        1
+        """
+        route = Endpoint.get_generation(name)
+        self._validate_resource(self.cache.generation, name, route)
+        return self.cache.generation.get(route, None)
+
+    async def fetch_generation(self, name: t.Union[str, int]) -> t.Optional[Generation]:
+        """Fetches a generation from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the generation.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the generation is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     generation = await client.game.fetch_generation(1)
+        ...     print(generation.id)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        1
+        """
+        route = Endpoint.get_generation(name)
+        self._validate_resource(self.cache.generation, name, route)
+        data = await self._client.request(route)
+        return self.cache.generation.setdefault(route, Generation.from_payload(data))
+
+    def get_pokedex(self, name: t.Union[str, int]) -> t.Optional[Pokedex]:
+        """Gets a pokedex from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the pokedex.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.Pokedex]
+            The pokedex if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the pokedex is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> pokedex = client.game.get_pokedex(1)
+        >>> pokedex.region
+        None
+        """
+        route = Endpoint.get_pokedex(name)
+        self._validate_resource(self.cache.pokedex, name, route)
+        return self.cache.pokedex.get(route, None)
+
+    async def fetch_pokedex(self, name: t.Union[str, int]) -> t.Optional[Pokedex]:
+        """Fetches a pokedex from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the pokedex.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the pokedex is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     pokedex = await client.game.fetch_pokedex(1)
+        ...     print(pokedex.region)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        None
+        """
+        route = Endpoint.get_pokedex(name)
+        self._validate_resource(self.cache.pokedex, name, route)
+        data = await self._client.request(route)
+        return self.cache.pokedex.setdefault(route, Pokedex.from_payload(data))
+
+    def get_version(self, name: t.Union[str, int]) -> t.Optional[Version]:
+        """Gets a version from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the version.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.Version]
+            The version if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the version is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> version = client.game.get_version(1)
+        >>> version.name
+        'red'
+        """
+        route = Endpoint.get_version(name)
+        self._validate_resource(self.cache.version, name, route)
+        return self.cache.version.get(route, None)
+
+    async def fetch_version(self, name: t.Union[str, int]) -> t.Optional[Version]:
+        """Fetches a version from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the version.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the version is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     version = await client.game.fetch_version(1)
+        ...     print(version.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        red
+        """
+        route = Endpoint.get_version(name)
+        self._validate_resource(self.cache.version, name, route)
+        data = await self._client.request(route)
+        return self.cache.version.setdefault(route, Version.from_payload(data))
+
+    def get_version_group(self, name: t.Union[str, int]) -> t.Optional[VersionGroup]:
+        """Gets a version group from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the version group.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.VersionGroup]
+            The version group if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the version group is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> version_group = client.game.get_version_group(1)
+        >>> version_group.id
+        1
+        """
+        route = Endpoint.get_version_group(name)
+        self._validate_resource(self.cache.version_group, name, route)
+        return self.cache.version_group.get(route, None)
+
+    async def fetch_version_group(self, name: t.Union[str, int]) -> t.Optional[VersionGroup]:
+        """Fetches a version group from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the version group.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the version group is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     version_group = await client.game.fetch_version_group(1)
+        ...     print(version_group.id)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        1
+        """
+        route = Endpoint.get_version_group(name)
+        self._validate_resource(self.cache.version_group, name, route)
+        data = await self._client.request(route)
+        return self.cache.version_group.setdefault(route, VersionGroup.from_payload(data))
+
+
+def setup(lance: "PokeLance") -> None:
+    """Sets up the game cog."""
+    lance.add_extension("game", Game(lance.http))
```

### Comparing `pokelance-0.0.9a0/pokelance/ext/item.py` & `pokelance-0.1.0/pokelance/ext/item.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,390 +1,370 @@
-import typing as t
-
-from pokelance.http import Endpoint
-from pokelance.models import Item as ItemModel
-from pokelance.models import ItemAttribute, ItemCategory, ItemFlingEffect, ItemPocket
-
-from ._base import BaseExtension
-
-if t.TYPE_CHECKING:
-    from pokelance import PokeLance
-    from pokelance.http import HttpClient
-
-
-__all__: t.Tuple[str, ...] = (
-    "setup",
-    "Item",
-)
-
-
-class Item(BaseExtension):
-    """Extension for item related endpoints.
-
-    Parameters
-    ----------
-    client: pokelance.http.HttpClient
-        The client to use for requests.
-
-    Attributes
-    ----------
-    cache: pokelance.cache.Item
-        The cache for this extension.
-    """
-
-    def __init__(self, client: "HttpClient") -> None:
-        """Initializes the extension."""
-        super().__init__(client)
-        self.cache = self._cache.item
-
-    async def setup(self) -> None:
-        """Sets up the extension."""
-        data = await self._client.request(Endpoint.get_item_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "item", data["results"])
-        data = await self._client.request(Endpoint.get_item_attribute_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "item_attribute", data["results"])
-        data = await self._client.request(Endpoint.get_item_category_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "item_category", data["results"])
-        data = await self._client.request(Endpoint.get_item_fling_effect_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "item_fling_effect", data["results"])
-        data = await self._client.request(Endpoint.get_item_pocket_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "item_pocket", data["results"])
-
-    def get_item(self, name: t.Union[str, int]) -> t.Optional[ItemModel]:
-        """Gets an item from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the item.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.Item]
-            The item if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the item is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> item = client.item.get_item("potion")
-        >>> item.id
-        17
-        """
-        route = Endpoint.get_item(name)
-        self._validate_resource(self.cache.item, name, route)
-        return self.cache.item.get(route, None)
-
-    async def fetch_item(self, name: t.Union[str, int]) -> t.Optional[ItemModel]:
-        """Fetches an item from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the item.
-
-        Returns
-        -------
-        t.Optional[pokelance.models.Item]
-            The item.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the item is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     item = await client.item.fetch_item("potion")
-        ...     print(item.id)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        17
-        """
-        route = Endpoint.get_item(name)
-        self._validate_resource(self.cache.item, name, route)
-        data = await self._client.request(route)
-        return self.cache.item.setdefault(route, ItemModel.from_payload(data))
-
-    def get_item_attribute(self, name: t.Union[str, int]) -> t.Optional[ItemAttribute]:
-        """Gets an item attribute from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the item attribute.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.ItemAttribute]
-            The item attribute if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the item attribute is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> item_attribute = client.item.get_item_attribute("holdable")
-        >>> item_attribute.id
-        5
-        """
-        route = Endpoint.get_item_attribute(name)
-        self._validate_resource(self.cache.item_attribute, name, route)
-        return self.cache.item_attribute.get(route, None)
-
-    async def fetch_item_attribute(self, name: t.Union[str, int]) -> t.Optional[ItemAttribute]:
-        """Fetches an item attribute from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the item attribute.
-
-        Returns
-        -------
-        t.Optional[pokelance.models.ItemAttribute]
-            The item attribute.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the item attribute is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     item_attribute = await client.item.fetch_item_attribute("holdable")
-        ...     print(item_attribute.id)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        5
-        """
-        route = Endpoint.get_item_attribute(name)
-        self._validate_resource(self.cache.item_attribute, name, route)
-        data = await self._client.request(route)
-        return self.cache.item_attribute.setdefault(route, ItemAttribute.from_payload(data))
-
-    def get_item_category(self, name: t.Union[str, int]) -> t.Optional[ItemCategory]:
-        """Gets an item category from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the item category.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.ItemCategory]
-            The item category if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the item category is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> item_category = client.item.get_item_category(1)
-        >>> item_category.name
-        'stat-boosts'
-        """
-        route = Endpoint.get_item_category(name)
-        self._validate_resource(self.cache.item_category, name, route)
-        return self.cache.item_category.get(route, None)
-
-    async def fetch_item_category(self, name: t.Union[str, int]) -> t.Optional[ItemCategory]:
-        """Fetches an item category from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the item category.
-
-        Returns
-        -------
-        t.Optional[pokelance.models.ItemCategory]
-            The item category.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the item category is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     item_category = await client.item.fetch_item_category(1)
-        ...     print(item_category.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        stat-boosts
-        """
-        route = Endpoint.get_item_category(name)
-        self._validate_resource(self.cache.item_category, name, route)
-        data = await self._client.request(route)
-        return self.cache.item_category.setdefault(route, ItemCategory.from_payload(data))
-
-    def get_item_fling_effect(self, name: t.Union[str, int]) -> t.Optional[ItemFlingEffect]:
-        """Gets an item fling effect from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the item fling effect.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.ItemFlingEffect]
-            The item fling effect if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the item fling effect is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> item_fling_effect = client.item.get_item_fling_effect(1)
-        >>> item_fling_effect.name
-        'badly-poison'
-        """
-        route = Endpoint.get_item_fling_effect(name)
-        self._validate_resource(self.cache.item_fling_effect, name, route)
-        return self.cache.item_fling_effect.get(route, None)
-
-    async def fetch_item_fling_effect(self, name: t.Union[str, int]) -> t.Optional[ItemFlingEffect]:
-        """Fetches an item fling effect from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the item fling effect.
-
-        Returns
-        -------
-        t.Optional[pokelance.models.ItemFlingEffect]
-            The item fling effect.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the item fling effect is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     item_fling_effect = await client.item.fetch_item_fling_effect(1)
-        ...     print(item_fling_effect.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        badly-poison
-        """
-        route = Endpoint.get_item_fling_effect(name)
-        self._validate_resource(self.cache.item_fling_effect, name, route)
-        data = await self._client.request(route)
-        return self.cache.item_fling_effect.setdefault(route, ItemFlingEffect.from_payload(data))
-
-    def get_item_pocket(self, name: t.Union[str, int]) -> t.Optional[ItemPocket]:
-        """Gets an item pocket from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the item pocket.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.ItemPocket]
-            The item pocket if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the item pocket is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> item_pocket = client.item.get_item_pocket(1)
-        >>> item_pocket.name
-        'misc'
-        """
-        route = Endpoint.get_item_pocket(name)
-        self._validate_resource(self.cache.item_pocket, name, route)
-        return self.cache.item_pocket.get(route, None)
-
-    async def fetch_item_pocket(self, name: t.Union[str, int]) -> t.Optional[ItemPocket]:
-        """Fetches an item pocket from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the item pocket.
-
-        Returns
-        -------
-        t.Optional[pokelance.models.ItemPocket]
-            The item pocket.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the item pocket is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     item_pocket = await client.item.fetch_item_pocket(1)
-        ...     print(item_pocket.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        misc
-        """
-        route = Endpoint.get_item_pocket(name)
-        self._validate_resource(self.cache.item_pocket, name, route)
-        data = await self._client.request(route)
-        return self.cache.item_pocket.setdefault(route, ItemPocket.from_payload(data))
-
-
-def setup(lance: "PokeLance") -> None:
-    """Sets up the item cog."""
-    lance.add_extension("item", Item(lance.http))
+import typing as t
+
+from pokelance.http import Endpoint
+from pokelance.models import Item as ItemModel
+from pokelance.models import ItemAttribute, ItemCategory, ItemFlingEffect, ItemPocket
+
+from ._base import BaseExtension
+
+if t.TYPE_CHECKING:
+    from pokelance import PokeLance
+    from pokelance.cache import Item as ItemCache
+
+
+__all__: t.Tuple[str, ...] = (
+    "setup",
+    "Item",
+)
+
+
+class Item(BaseExtension):
+    """
+    Extension for item related endpoints.
+
+    Attributes
+    ----------
+    cache: pokelance.cache.Item
+        The cache for this extension.
+    """
+
+    cache: "ItemCache"
+
+    def get_item(self, name: t.Union[str, int]) -> t.Optional[ItemModel]:
+        """Gets an item from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the item.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.Item]
+            The item if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the item is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> item = client.item.get_item("potion")
+        >>> item.id
+        17
+        """
+        route = Endpoint.get_item(name)
+        self._validate_resource(self.cache.item, name, route)
+        return self.cache.item.get(route, None)
+
+    async def fetch_item(self, name: t.Union[str, int]) -> t.Optional[ItemModel]:
+        """Fetches an item from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the item.
+
+        Returns
+        -------
+        t.Optional[pokelance.models.Item]
+            The item.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the item is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     item = await client.item.fetch_item("potion")
+        ...     print(item.id)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        17
+        """
+        route = Endpoint.get_item(name)
+        self._validate_resource(self.cache.item, name, route)
+        data = await self._client.request(route)
+        return self.cache.item.setdefault(route, ItemModel.from_payload(data))
+
+    def get_item_attribute(self, name: t.Union[str, int]) -> t.Optional[ItemAttribute]:
+        """Gets an item attribute from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the item attribute.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.ItemAttribute]
+            The item attribute if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the item attribute is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> item_attribute = client.item.get_item_attribute("holdable")
+        >>> item_attribute.id
+        5
+        """
+        route = Endpoint.get_item_attribute(name)
+        self._validate_resource(self.cache.item_attribute, name, route)
+        return self.cache.item_attribute.get(route, None)
+
+    async def fetch_item_attribute(self, name: t.Union[str, int]) -> t.Optional[ItemAttribute]:
+        """Fetches an item attribute from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the item attribute.
+
+        Returns
+        -------
+        t.Optional[pokelance.models.ItemAttribute]
+            The item attribute.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the item attribute is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     item_attribute = await client.item.fetch_item_attribute("holdable")
+        ...     print(item_attribute.id)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        5
+        """
+        route = Endpoint.get_item_attribute(name)
+        self._validate_resource(self.cache.item_attribute, name, route)
+        data = await self._client.request(route)
+        return self.cache.item_attribute.setdefault(route, ItemAttribute.from_payload(data))
+
+    def get_item_category(self, name: t.Union[str, int]) -> t.Optional[ItemCategory]:
+        """Gets an item category from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the item category.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.ItemCategory]
+            The item category if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the item category is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> item_category = client.item.get_item_category(1)
+        >>> item_category.name
+        'stat-boosts'
+        """
+        route = Endpoint.get_item_category(name)
+        self._validate_resource(self.cache.item_category, name, route)
+        return self.cache.item_category.get(route, None)
+
+    async def fetch_item_category(self, name: t.Union[str, int]) -> t.Optional[ItemCategory]:
+        """Fetches an item category from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the item category.
+
+        Returns
+        -------
+        t.Optional[pokelance.models.ItemCategory]
+            The item category.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the item category is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     item_category = await client.item.fetch_item_category(1)
+        ...     print(item_category.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        stat-boosts
+        """
+        route = Endpoint.get_item_category(name)
+        self._validate_resource(self.cache.item_category, name, route)
+        data = await self._client.request(route)
+        return self.cache.item_category.setdefault(route, ItemCategory.from_payload(data))
+
+    def get_item_fling_effect(self, name: t.Union[str, int]) -> t.Optional[ItemFlingEffect]:
+        """Gets an item fling effect from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the item fling effect.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.ItemFlingEffect]
+            The item fling effect if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the item fling effect is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> item_fling_effect = client.item.get_item_fling_effect(1)
+        >>> item_fling_effect.name
+        'badly-poison'
+        """
+        route = Endpoint.get_item_fling_effect(name)
+        self._validate_resource(self.cache.item_fling_effect, name, route)
+        return self.cache.item_fling_effect.get(route, None)
+
+    async def fetch_item_fling_effect(self, name: t.Union[str, int]) -> t.Optional[ItemFlingEffect]:
+        """Fetches an item fling effect from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the item fling effect.
+
+        Returns
+        -------
+        t.Optional[pokelance.models.ItemFlingEffect]
+            The item fling effect.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the item fling effect is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     item_fling_effect = await client.item.fetch_item_fling_effect(1)
+        ...     print(item_fling_effect.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        badly-poison
+        """
+        route = Endpoint.get_item_fling_effect(name)
+        self._validate_resource(self.cache.item_fling_effect, name, route)
+        data = await self._client.request(route)
+        return self.cache.item_fling_effect.setdefault(route, ItemFlingEffect.from_payload(data))
+
+    def get_item_pocket(self, name: t.Union[str, int]) -> t.Optional[ItemPocket]:
+        """Gets an item pocket from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the item pocket.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.ItemPocket]
+            The item pocket if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the item pocket is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> item_pocket = client.item.get_item_pocket(1)
+        >>> item_pocket.name
+        'misc'
+        """
+        route = Endpoint.get_item_pocket(name)
+        self._validate_resource(self.cache.item_pocket, name, route)
+        return self.cache.item_pocket.get(route, None)
+
+    async def fetch_item_pocket(self, name: t.Union[str, int]) -> t.Optional[ItemPocket]:
+        """Fetches an item pocket from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the item pocket.
+
+        Returns
+        -------
+        t.Optional[pokelance.models.ItemPocket]
+            The item pocket.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the item pocket is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     item_pocket = await client.item.fetch_item_pocket(1)
+        ...     print(item_pocket.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        misc
+        """
+        route = Endpoint.get_item_pocket(name)
+        self._validate_resource(self.cache.item_pocket, name, route)
+        data = await self._client.request(route)
+        return self.cache.item_pocket.setdefault(route, ItemPocket.from_payload(data))
+
+
+def setup(lance: "PokeLance") -> None:
+    """Sets up the item cog."""
+    lance.add_extension("item", Item(lance.http))
```

### Comparing `pokelance-0.0.9a0/pokelance/ext/location.py` & `pokelance-0.1.0/pokelance/ext/location.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,322 +1,303 @@
-import typing as t
-
-from pokelance.http import Endpoint
-from pokelance.models import Location as LocationModel
-from pokelance.models import LocationArea, PalParkArea, Region
-
-from ._base import BaseExtension
-
-if t.TYPE_CHECKING:
-    from pokelance import PokeLance
-    from pokelance.http import HttpClient
-
-
-__all__: t.Tuple[str, ...] = (
-    "setup",
-    "Location",
-)
-
-
-class Location(BaseExtension):
-    """
-    Extension for location related endpoints.
-
-    Parameters
-    ----------
-    client: pokelance.http.HttpClient
-        The client to use for requests.
-
-    Attributes
-    ----------
-    cache: pokelance.cache.Location
-        The cache for this extension.
-    """
-
-    def __init__(self, client: "HttpClient") -> None:
-        """Initializes the extension."""
-        super().__init__(client)
-        self.cache = self._cache.location
-
-    async def setup(self) -> None:
-        """Sets up the extension."""
-        data = await self._client.request(Endpoint.get_location_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "location", data["results"])
-        data = await self._client.request(Endpoint.get_location_area_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "location_area", data["results"])
-        data = await self._client.request(Endpoint.get_pal_park_area_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "pal_park_area", data["results"])
-        data = await self._client.request(Endpoint.get_region_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "region", data["results"])
-
-    def get_location(self, name: t.Union[str, int]) -> t.Optional[LocationModel]:
-        """Gets a location from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the location.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.Location]
-            The location if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the item pocket is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> location = client.location.get_location(1)
-        >>> location.name
-        'canalave-city'
-        """
-        route = Endpoint.get_location(name)
-        self._validate_resource(self.cache.location, name, route)
-        return self.cache.location.get(route, None)
-
-    async def fetch_location(self, name: t.Union[str, int]) -> t.Optional[LocationModel]:
-        """Fetches a location from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the location.
-
-        Returns
-        -------
-        t.Optional[pokelance.models.Location]
-            The location.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the location is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     location = await client.location.fetch_location(1)
-        ...     print(location.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        canalave-city
-        """
-        route = Endpoint.get_location(name)
-        self._validate_resource(self.cache.location, name, route)
-        data = await self._client.request(route)
-        return self.cache.location.setdefault(route, LocationModel.from_payload(data))
-
-    def get_location_area(self, name: t.Union[str, int]) -> t.Optional[LocationArea]:
-        """Gets a location area from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the location area.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.LocationArea]
-            The location area if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the location area is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> location_area = client.location.get_location_area(1)
-        >>> location_area.name
-        'canalave-city-area'
-        """
-        route = Endpoint.get_location_area(name)
-        self._validate_resource(self.cache.location_area, name, route)
-        return self.cache.location_area.get(route, None)
-
-    async def fetch_location_area(self, name: t.Union[str, int]) -> t.Optional[LocationArea]:
-        """Fetches a location area from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the location area.
-
-        Returns
-        -------
-        t.Optional[pokelance.models.LocationArea]
-            The location area.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the location area is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     location_area = await client.location.fetch_location_area(1)
-        ...     print(location_area.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        canalave-city-area
-        """
-        route = Endpoint.get_location_area(name)
-        self._validate_resource(self.cache.location_area, name, route)
-        data = await self._client.request(route)
-        return self.cache.location_area.setdefault(route, LocationArea.from_payload(data))
-
-    def get_pal_park_area(self, name: t.Union[str, int]) -> t.Optional[PalParkArea]:
-        """Gets a pal park area from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the pal park area.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.PalParkArea]
-            The pal park area if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the pal park area is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> pal_park_area = client.location.get_pal_park_area(1)
-        >>> pal_park_area.name
-        'forest'
-        """
-        route = Endpoint.get_pal_park_area(name)
-        self._validate_resource(self.cache.pal_park_area, name, route)
-        return self.cache.pal_park_area.get(route, None)
-
-    async def fetch_pal_park_area(self, name: t.Union[str, int]) -> t.Optional[PalParkArea]:
-        """Fetches a pal park area from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the pal park area.
-
-        Returns
-        -------
-        t.Optional[pokelance.models.PalParkArea]
-            The pal park area.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the pal park area is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     pal_park_area = await client.location.fetch_pal_park_area(1)
-        ...     print(pal_park_area.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        forest
-        """
-        route = Endpoint.get_pal_park_area(name)
-        self._validate_resource(self.cache.pal_park_area, name, route)
-        data = await self._client.request(route)
-        return self.cache.pal_park_area.setdefault(route, PalParkArea.from_payload(data))
-
-    def get_region(self, name: t.Union[str, int]) -> t.Optional[Region]:
-        """Gets a region from the cache.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the region.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.Region]
-            The region if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the region is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> region = client.location.get_region(1)
-        >>> region.name
-        'kanto'
-        """
-        route = Endpoint.get_region(name)
-        self._validate_resource(self.cache.region, name, route)
-        return self.cache.region.get(route, None)
-
-    async def fetch_region(self, name: t.Union[str, int]) -> t.Optional[Region]:
-        """Fetches a region from the API.
-
-        Parameters
-        ----------
-        name: typing.Union[str, int]
-            The name or id of the region.
-
-        Returns
-        -------
-        t.Optional[pokelance.models.Region]
-            The region.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            The name or id of the region is invalid.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     region = await client.location.fetch_region(1)
-        ...     print(region.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        kanto
-        """
-        route = Endpoint.get_region(name)
-        self._validate_resource(self.cache.region, name, route)
-        data = await self._client.request(route)
-        return self.cache.region.setdefault(route, Region.from_payload(data))
-
-
-def setup(lance: "PokeLance") -> None:
-    """Sets up the location cog."""
-    lance.add_extension("location", Location(lance.http))
+import typing as t
+
+from pokelance.http import Endpoint
+from pokelance.models import Location as LocationModel
+from pokelance.models import LocationArea, PalParkArea, Region
+
+from ._base import BaseExtension
+
+if t.TYPE_CHECKING:
+    from pokelance import PokeLance
+    from pokelance.cache import Location as LocationCache
+
+
+__all__: t.Tuple[str, ...] = (
+    "setup",
+    "Location",
+)
+
+
+class Location(BaseExtension):
+    """
+    Extension for location related endpoints.
+
+    Attributes
+    ----------
+    cache: pokelance.cache.Location
+        The cache for this extension.
+    """
+
+    cache: "LocationCache"
+
+    def get_location(self, name: t.Union[str, int]) -> t.Optional[LocationModel]:
+        """Gets a location from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the location.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.Location]
+            The location if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the item pocket is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> location = client.location.get_location(1)
+        >>> location.name
+        'canalave-city'
+        """
+        route = Endpoint.get_location(name)
+        self._validate_resource(self.cache.location, name, route)
+        return self.cache.location.get(route, None)
+
+    async def fetch_location(self, name: t.Union[str, int]) -> t.Optional[LocationModel]:
+        """Fetches a location from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the location.
+
+        Returns
+        -------
+        t.Optional[pokelance.models.Location]
+            The location.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the location is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     location = await client.location.fetch_location(1)
+        ...     print(location.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        canalave-city
+        """
+        route = Endpoint.get_location(name)
+        self._validate_resource(self.cache.location, name, route)
+        data = await self._client.request(route)
+        return self.cache.location.setdefault(route, LocationModel.from_payload(data))
+
+    def get_location_area(self, name: t.Union[str, int]) -> t.Optional[LocationArea]:
+        """Gets a location area from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the location area.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.LocationArea]
+            The location area if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the location area is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> location_area = client.location.get_location_area(1)
+        >>> location_area.name
+        'canalave-city-area'
+        """
+        route = Endpoint.get_location_area(name)
+        self._validate_resource(self.cache.location_area, name, route)
+        return self.cache.location_area.get(route, None)
+
+    async def fetch_location_area(self, name: t.Union[str, int]) -> t.Optional[LocationArea]:
+        """Fetches a location area from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the location area.
+
+        Returns
+        -------
+        t.Optional[pokelance.models.LocationArea]
+            The location area.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the location area is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     location_area = await client.location.fetch_location_area(1)
+        ...     print(location_area.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        canalave-city-area
+        """
+        route = Endpoint.get_location_area(name)
+        self._validate_resource(self.cache.location_area, name, route)
+        data = await self._client.request(route)
+        return self.cache.location_area.setdefault(route, LocationArea.from_payload(data))
+
+    def get_pal_park_area(self, name: t.Union[str, int]) -> t.Optional[PalParkArea]:
+        """Gets a pal park area from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the pal park area.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.PalParkArea]
+            The pal park area if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the pal park area is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> pal_park_area = client.location.get_pal_park_area(1)
+        >>> pal_park_area.name
+        'forest'
+        """
+        route = Endpoint.get_pal_park_area(name)
+        self._validate_resource(self.cache.pal_park_area, name, route)
+        return self.cache.pal_park_area.get(route, None)
+
+    async def fetch_pal_park_area(self, name: t.Union[str, int]) -> t.Optional[PalParkArea]:
+        """Fetches a pal park area from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the pal park area.
+
+        Returns
+        -------
+        t.Optional[pokelance.models.PalParkArea]
+            The pal park area.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the pal park area is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     pal_park_area = await client.location.fetch_pal_park_area(1)
+        ...     print(pal_park_area.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        forest
+        """
+        route = Endpoint.get_pal_park_area(name)
+        self._validate_resource(self.cache.pal_park_area, name, route)
+        data = await self._client.request(route)
+        return self.cache.pal_park_area.setdefault(route, PalParkArea.from_payload(data))
+
+    def get_region(self, name: t.Union[str, int]) -> t.Optional[Region]:
+        """Gets a region from the cache.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the region.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.Region]
+            The region if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the region is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> region = client.location.get_region(1)
+        >>> region.name
+        'kanto'
+        """
+        route = Endpoint.get_region(name)
+        self._validate_resource(self.cache.region, name, route)
+        return self.cache.region.get(route, None)
+
+    async def fetch_region(self, name: t.Union[str, int]) -> t.Optional[Region]:
+        """Fetches a region from the API.
+
+        Parameters
+        ----------
+        name: typing.Union[str, int]
+            The name or id of the region.
+
+        Returns
+        -------
+        t.Optional[pokelance.models.Region]
+            The region.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            The name or id of the region is invalid.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     region = await client.location.fetch_region(1)
+        ...     print(region.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        kanto
+        """
+        route = Endpoint.get_region(name)
+        self._validate_resource(self.cache.region, name, route)
+        data = await self._client.request(route)
+        return self.cache.region.setdefault(route, Region.from_payload(data))
+
+
+def setup(lance: "PokeLance") -> None:
+    """Sets up the location cog."""
+    lance.add_extension("location", Location(lance.http))
```

### Comparing `pokelance-0.0.9a0/pokelance/ext/machine.py` & `pokelance-0.1.0/pokelance/ext/machine.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,113 +1,100 @@
-import typing as t
-
-from pokelance.http import Endpoint
-from pokelance.models import Machine as MachineModel
-
-from ._base import BaseExtension
-
-if t.TYPE_CHECKING:
-    from pokelance import PokeLance
-    from pokelance.http import HttpClient
-
-
-__all__: t.Tuple[str, ...] = (
-    "setup",
-    "Machine",
-)
-
-
-class Machine(BaseExtension):
-    """Extension for machine related endpoints.
-
-    Parameters
-    ----------
-    client: pokelance.http.HttpClient
-        The client to use for requests.
-
-    Attributes
-    ----------
-    cache: pokelance.cache.Machine
-        The cache for this extension.
-    """
-
-    def __init__(self, client: "HttpClient") -> None:
-        """Initializes the extension."""
-        super().__init__(client)
-        self.cache = self._cache.machine
-
-    async def setup(self) -> None:
-        """Sets up the extension."""
-        data = await self._client.request(Endpoint.get_machine_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "machine", data["results"])
-
-    def get_machine(self, id_: int) -> t.Optional[MachineModel]:
-        """Gets a machine from the cache.
-
-        Parameters
-        ----------
-        id_: int
-            The id of the machine.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.Machine]
-            The machine if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the machine does not exist in the cache.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> machine = client.machine.get_machine(1)
-        >>> machine.item.name
-        'tm00'
-        """
-        route = Endpoint.get_machine(id_)
-        self._validate_resource(self.cache.machine, id_, route)
-        return self.cache.machine.get(route, None)
-
-    async def fetch_machine(self, id_: int) -> t.Optional[MachineModel]:
-        """Fetches a machine from the API.
-
-        Parameters
-        ----------
-        id_: int
-            The id of the machine.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.Machine]
-            The machine if it exists in the API, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the machine does not exist in the API.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     machine = await client.machine.fetch_machine(1)
-        ...     print(machine.item.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        tm00
-        """
-        route = Endpoint.get_machine(id_)
-        self._validate_resource(self.cache.machine, id_, route)
-        data = await self._client.request(route)
-        return self.cache.machine.setdefault(route, MachineModel.from_payload(data))
-
-
-def setup(lance: "PokeLance") -> None:
-    """Sets up the machine cog."""
-    lance.add_extension("machine", Machine(lance.http))
+import typing as t
+
+from pokelance.http import Endpoint
+from pokelance.models import Machine as MachineModel
+
+from ._base import BaseExtension
+
+if t.TYPE_CHECKING:
+    from pokelance import PokeLance
+    from pokelance.cache import Machine as MachineCache
+
+
+__all__: t.Tuple[str, ...] = (
+    "setup",
+    "Machine",
+)
+
+
+class Machine(BaseExtension):
+    """Extension for machine related endpoints.
+
+    Attributes
+    ----------
+    cache: pokelance.cache.Machine
+        The cache for this extension.
+    """
+
+    cache: "MachineCache"
+
+    def get_machine(self, id_: int) -> t.Optional[MachineModel]:
+        """Gets a machine from the cache.
+
+        Parameters
+        ----------
+        id_: int
+            The id of the machine.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.Machine]
+            The machine if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the machine does not exist in the cache.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> machine = client.machine.get_machine(1)
+        >>> machine.item.name
+        'tm00'
+        """
+        route = Endpoint.get_machine(id_)
+        self._validate_resource(self.cache.machine, id_, route)
+        return self.cache.machine.get(route, None)
+
+    async def fetch_machine(self, id_: int) -> t.Optional[MachineModel]:
+        """Fetches a machine from the API.
+
+        Parameters
+        ----------
+        id_: int
+            The id of the machine.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.Machine]
+            The machine if it exists in the API, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the machine does not exist in the API.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     machine = await client.machine.fetch_machine(1)
+        ...     print(machine.item.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        tm00
+        """
+        route = Endpoint.get_machine(id_)
+        self._validate_resource(self.cache.machine, id_, route)
+        data = await self._client.request(route)
+        return self.cache.machine.setdefault(route, MachineModel.from_payload(data))
+
+
+def setup(lance: "PokeLance") -> None:
+    """Sets up the machine cog."""
+    lance.add_extension("machine", Machine(lance.http))
```

### Comparing `pokelance-0.0.9a0/pokelance/ext/move.py` & `pokelance-0.1.0/pokelance/ext/move.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,528 +1,503 @@
-import typing as t
-
-from pokelance.http import Endpoint
-from pokelance.models import Move as MoveModel
-from pokelance.models import MoveAilment, MoveBattleStyle, MoveCategory, MoveDamageClass, MoveLearnMethod, MoveTarget
-
-from ._base import BaseExtension
-
-if t.TYPE_CHECKING:
-    from pokelance import PokeLance
-    from pokelance.http import HttpClient
-
-
-__all__: t.Tuple[str, ...] = (
-    "setup",
-    "Move",
-)
-
-
-class Move(BaseExtension):
-    """Extension for move related endpoints.
-
-    Parameters
-    ----------
-    client: pokelance.http.HttpClient
-        The client to use for requests.
-
-    Attributes
-    ----------
-    cache: pokelance.cache.Move
-        The cache for this extension.
-    """
-
-    def __init__(self, client: "HttpClient") -> None:
-        """Initializes the extension."""
-        super().__init__(client)
-        self.cache = self._cache.move
-
-    async def setup(self) -> None:
-        """Sets up the extension."""
-        data = await self._client.request(Endpoint.get_move_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "move", data["results"])
-        data = await self._client.request(Endpoint.get_move_ailment_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "move_ailment", data["results"])
-        data = await self._client.request(Endpoint.get_move_battle_style_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "move_battle_style", data["results"])
-        data = await self._client.request(Endpoint.get_move_category_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "move_category", data["results"])
-        data = await self._client.request(Endpoint.get_move_damage_class_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "move_damage_class", data["results"])
-        data = await self._client.request(Endpoint.get_move_learn_method_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "move_learn_method", data["results"])
-        data = await self._client.request(Endpoint.get_move_target_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "move_target", data["results"])
-
-    def get_move(self, name: t.Union[str, int]) -> t.Optional[MoveModel]:
-        """Gets a move from the cache.
-
-        Parameters
-        ----------
-        name: t.Union[str, int]
-            The id of the move.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.Move]
-            The move if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the move does not exist in the cache.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> move = client.move.get_move(1)
-        >>> move.name
-        'pound'
-        """
-        route = Endpoint.get_move(name)
-        self._validate_resource(self.cache.move, name, route)
-        return self.cache.move.get(route, None)
-
-    async def fetch_move(self, name: t.Union[str, int]) -> t.Optional[MoveModel]:
-        """Fetches a move from the API.
-
-        Parameters
-        ----------
-        name: t.Union[str, int]
-            The id of the move.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.Move]
-            The move if it exists in the API, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the move does not exist in the API.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     move = await client.move.fetch_move(1)
-        ...     print(move.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        pound
-        """
-        route = Endpoint.get_move(name)
-        self._validate_resource(self.cache.move, name, route)
-        data = await self._client.request(route)
-        return self.cache.move.setdefault(route, MoveModel.from_payload(data))
-
-    def get_move_ailment(self, name: t.Union[str, int]) -> t.Optional[MoveAilment]:
-        """Gets a move ailment from the cache.
-
-        Parameters
-        ----------
-        name: t.Union[str, int]
-            The id of the move ailment.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.MoveAilment]
-            The move ailment if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the move ailment does not exist in the cache.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> ailment = client.move.get_move_ailment(1)
-        >>> ailment.name
-        'paralysis'
-        """
-        route = Endpoint.get_move_ailment(name)
-        self._validate_resource(self.cache.move_ailment, name, route)
-        return self.cache.move_ailment.get(route, None)
-
-    async def fetch_move_ailment(self, name: t.Union[str, int]) -> t.Optional[MoveAilment]:
-        """Fetches a move ailment from the API.
-
-        Parameters
-        ----------
-        name: t.Union[str, int]
-            The id of the move ailment.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.MoveAilment]
-            The move ailment if it exists in the API, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the move ailment does not exist in the API.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     ailment = await client.move.fetch_move_ailment(1)
-        ...     print(ailment.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        paralysis
-        """
-        route = Endpoint.get_move_ailment(name)
-        self._validate_resource(self.cache.move_ailment, name, route)
-        data = await self._client.request(route)
-        return self.cache.move_ailment.setdefault(route, MoveAilment.from_payload(data))
-
-    def get_move_battle_style(self, name: t.Union[str, int]) -> t.Optional[MoveBattleStyle]:
-        """Gets a move battle style from the cache.
-
-        Parameters
-        ----------
-        name: t.Union[str, int]
-            The id of the move battle style.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.MoveBattleStyle]
-            The move battle style if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the move battle style does not exist in the cache.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> style = client.move.get_move_battle_style(1)
-        >>> style.name
-        'attack'
-        """
-        route = Endpoint.get_move_battle_style(name)
-        self._validate_resource(self.cache.move_battle_style, name, route)
-        return self.cache.move_battle_style.get(route, None)
-
-    async def fetch_move_battle_style(self, name: t.Union[str, int]) -> t.Optional[MoveBattleStyle]:
-        """Fetches a move battle style from the API.
-
-        Parameters
-        ----------
-        name: t.Union[str, int]
-            The id of the move battle style.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.MoveBattleStyle]
-            The move battle style if it exists in the API, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the move battle style does not exist in the API.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     style = await client.move.fetch_move_battle_style(1)
-        ...     print(style.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        attack
-        """
-        route = Endpoint.get_move_battle_style(name)
-        self._validate_resource(self.cache.move_battle_style, name, route)
-        data = await self._client.request(route)
-        return self.cache.move_battle_style.setdefault(route, MoveBattleStyle.from_payload(data))
-
-    def get_move_category(self, name: t.Union[str, int]) -> t.Optional[MoveCategory]:
-        """Gets a move category from the cache.
-
-        Parameters
-        ----------
-        name: t.Union[str, int]
-            The id of the move category.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.MoveCategory]
-            The move category if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the move category does not exist in the cache.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> category = client.move.get_move_category(1)
-        >>> category.name
-        'ailment'
-        """
-        route = Endpoint.get_move_category(name)
-        self._validate_resource(self.cache.move_category, name, route)
-        return self.cache.move_category.get(route, None)
-
-    async def fetch_move_category(self, name: t.Union[str, int]) -> t.Optional[MoveCategory]:
-        """Fetches a move category from the API.
-
-        Parameters
-        ----------
-        name: t.Union[str, int]
-            The id of the move category.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.MoveCategory]
-            The move category if it exists in the API, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the move category does not exist in the API.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     category = await client.move.fetch_move_category(1)
-        ...     print(category.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        ailment
-        """
-        route = Endpoint.get_move_category(name)
-        self._validate_resource(self.cache.move_category, name, route)
-        data = await self._client.request(route)
-        return self.cache.move_category.setdefault(route, MoveCategory.from_payload(data))
-
-    def get_move_damage_class(self, name: t.Union[str, int]) -> t.Optional[MoveDamageClass]:
-        """Gets a move damage class from the cache.
-
-        Parameters
-        ----------
-        name: t.Union[str, int]
-            The id of the move damage class.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.MoveDamageClass]
-            The move damage class if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the move damage class does not exist in the cache.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> damage_class = client.move.get_move_damage_class(1)
-        >>> damage_class.name
-        'status'
-        """
-        route = Endpoint.get_move_damage_class(name)
-        self._validate_resource(self.cache.move_damage_class, name, route)
-        return self.cache.move_damage_class.get(route, None)
-
-    async def fetch_move_damage_class(self, name: t.Union[str, int]) -> t.Optional[MoveDamageClass]:
-        """Fetches a move damage class from the API.
-
-        Parameters
-        ----------
-        name: t.Union[str, int]
-            The id of the move damage class.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.MoveDamageClass]
-            The move damage class if it exists in the API, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the move damage class does not exist in the API.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     damage_class = await client.move.fetch_move_damage_class(1)
-        ...     print(damage_class.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        status
-        """
-        route = Endpoint.get_move_damage_class(name)
-        self._validate_resource(self.cache.move_damage_class, name, route)
-        data = await self._client.request(route)
-        return self.cache.move_damage_class.setdefault(route, MoveDamageClass.from_payload(data))
-
-    def get_move_learn_method(self, name: t.Union[str, int]) -> t.Optional[MoveLearnMethod]:
-        """Gets a move learn method from the cache.
-
-        Parameters
-        ----------
-        name: t.Union[str, int]
-            The id of the move learn method.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.MoveLearnMethod]
-            The move learn method if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the move learn method does not exist in the cache.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> learn_method = client.move.get_move_learn_method(1)
-        >>> learn_method.name
-        'level-up'
-        """
-        route = Endpoint.get_move_learn_method(name)
-        self._validate_resource(self.cache.move_learn_method, name, route)
-        return self.cache.move_learn_method.get(route, None)
-
-    async def fetch_move_learn_method(self, name: t.Union[str, int]) -> t.Optional[MoveLearnMethod]:
-        """Fetches a move learn method from the API.
-
-        Parameters
-        ----------
-        name: t.Union[str, int]
-            The id of the move learn method.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.MoveLearnMethod]
-            The move learn method if it exists in the API, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the move learn method does not exist in the API.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     learn_method = await client.move.fetch_move_learn_method(1)
-        ...     print(learn_method.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        level-up
-        """
-        route = Endpoint.get_move_learn_method(name)
-        self._validate_resource(self.cache.move_learn_method, name, route)
-        data = await self._client.request(route)
-        return self.cache.move_learn_method.setdefault(route, MoveLearnMethod.from_payload(data))
-
-    def get_move_target(self, name: t.Union[str, int]) -> t.Optional[MoveTarget]:
-        """Gets a move target from the cache.
-
-        Parameters
-        ----------
-        name: t.Union[str, int]
-            The id of the move target.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.MoveTarget]
-            The move target if it exists in the cache, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the move target does not exist in the cache.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> target = client.move.get_move_target(1)
-        >>> target.name
-        'specific-pokemon'
-        """
-        route = Endpoint.get_move_target(name)
-        self._validate_resource(self.cache.move_target, name, route)
-        return self.cache.move_target.get(route, None)
-
-    async def fetch_move_target(self, name: t.Union[str, int]) -> t.Optional[MoveTarget]:
-        """Fetches a move target from the API.
-
-        Parameters
-        ----------
-        name: t.Union[str, int]
-            The id of the move target.
-
-        Returns
-        -------
-        typing.Optional[pokelance.models.MoveTarget]
-            The move target if it exists in the API, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the move target does not exist in the API.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     target = await client.move.fetch_move_target(1)
-        ...     print(target.name)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        specific-pokemon
-        """
-        route = Endpoint.get_move_target(name)
-        self._validate_resource(self.cache.move_target, name, route)
-        data = await self._client.request(route)
-        return self.cache.move_target.setdefault(route, MoveTarget.from_payload(data))
-
-
-def setup(lance: "PokeLance") -> None:
-    """Sets up the move cog."""
-    lance.add_extension("move", Move(lance.http))
+import typing as t
+
+from pokelance.http import Endpoint
+from pokelance.models import Move as MoveModel
+from pokelance.models import MoveAilment, MoveBattleStyle, MoveCategory, MoveDamageClass, MoveLearnMethod, MoveTarget
+
+from ._base import BaseExtension
+
+if t.TYPE_CHECKING:
+    from pokelance import PokeLance
+    from pokelance.cache import Move as MoveCache
+
+
+__all__: t.Tuple[str, ...] = (
+    "setup",
+    "Move",
+)
+
+
+class Move(BaseExtension):
+    """Extension for move related endpoints.
+
+    Attributes
+    ----------
+    cache: pokelance.cache.Move
+        The cache for this extension.
+    """
+
+    cache: "MoveCache"
+
+    def get_move(self, name: t.Union[str, int]) -> t.Optional[MoveModel]:
+        """Gets a move from the cache.
+
+        Parameters
+        ----------
+        name: t.Union[str, int]
+            The id of the move.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.Move]
+            The move if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the move does not exist in the cache.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> move = client.move.get_move(1)
+        >>> move.name
+        'pound'
+        """
+        route = Endpoint.get_move(name)
+        self._validate_resource(self.cache.move, name, route)
+        return self.cache.move.get(route, None)
+
+    async def fetch_move(self, name: t.Union[str, int]) -> t.Optional[MoveModel]:
+        """Fetches a move from the API.
+
+        Parameters
+        ----------
+        name: t.Union[str, int]
+            The id of the move.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.Move]
+            The move if it exists in the API, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the move does not exist in the API.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     move = await client.move.fetch_move(1)
+        ...     print(move.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        pound
+        """
+        route = Endpoint.get_move(name)
+        self._validate_resource(self.cache.move, name, route)
+        data = await self._client.request(route)
+        return self.cache.move.setdefault(route, MoveModel.from_payload(data))
+
+    def get_move_ailment(self, name: t.Union[str, int]) -> t.Optional[MoveAilment]:
+        """Gets a move ailment from the cache.
+
+        Parameters
+        ----------
+        name: t.Union[str, int]
+            The id of the move ailment.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.MoveAilment]
+            The move ailment if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the move ailment does not exist in the cache.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> ailment = client.move.get_move_ailment(1)
+        >>> ailment.name
+        'paralysis'
+        """
+        route = Endpoint.get_move_ailment(name)
+        self._validate_resource(self.cache.move_ailment, name, route)
+        return self.cache.move_ailment.get(route, None)
+
+    async def fetch_move_ailment(self, name: t.Union[str, int]) -> t.Optional[MoveAilment]:
+        """Fetches a move ailment from the API.
+
+        Parameters
+        ----------
+        name: t.Union[str, int]
+            The id of the move ailment.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.MoveAilment]
+            The move ailment if it exists in the API, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the move ailment does not exist in the API.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     ailment = await client.move.fetch_move_ailment(1)
+        ...     print(ailment.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        paralysis
+        """
+        route = Endpoint.get_move_ailment(name)
+        self._validate_resource(self.cache.move_ailment, name, route)
+        data = await self._client.request(route)
+        return self.cache.move_ailment.setdefault(route, MoveAilment.from_payload(data))
+
+    def get_move_battle_style(self, name: t.Union[str, int]) -> t.Optional[MoveBattleStyle]:
+        """Gets a move battle style from the cache.
+
+        Parameters
+        ----------
+        name: t.Union[str, int]
+            The id of the move battle style.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.MoveBattleStyle]
+            The move battle style if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the move battle style does not exist in the cache.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> style = client.move.get_move_battle_style(1)
+        >>> style.name
+        'attack'
+        """
+        route = Endpoint.get_move_battle_style(name)
+        self._validate_resource(self.cache.move_battle_style, name, route)
+        return self.cache.move_battle_style.get(route, None)
+
+    async def fetch_move_battle_style(self, name: t.Union[str, int]) -> t.Optional[MoveBattleStyle]:
+        """Fetches a move battle style from the API.
+
+        Parameters
+        ----------
+        name: t.Union[str, int]
+            The id of the move battle style.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.MoveBattleStyle]
+            The move battle style if it exists in the API, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the move battle style does not exist in the API.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     style = await client.move.fetch_move_battle_style(1)
+        ...     print(style.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        attack
+        """
+        route = Endpoint.get_move_battle_style(name)
+        self._validate_resource(self.cache.move_battle_style, name, route)
+        data = await self._client.request(route)
+        return self.cache.move_battle_style.setdefault(route, MoveBattleStyle.from_payload(data))
+
+    def get_move_category(self, name: t.Union[str, int]) -> t.Optional[MoveCategory]:
+        """Gets a move category from the cache.
+
+        Parameters
+        ----------
+        name: t.Union[str, int]
+            The id of the move category.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.MoveCategory]
+            The move category if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the move category does not exist in the cache.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> category = client.move.get_move_category(1)
+        >>> category.name
+        'ailment'
+        """
+        route = Endpoint.get_move_category(name)
+        self._validate_resource(self.cache.move_category, name, route)
+        return self.cache.move_category.get(route, None)
+
+    async def fetch_move_category(self, name: t.Union[str, int]) -> t.Optional[MoveCategory]:
+        """Fetches a move category from the API.
+
+        Parameters
+        ----------
+        name: t.Union[str, int]
+            The id of the move category.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.MoveCategory]
+            The move category if it exists in the API, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the move category does not exist in the API.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     category = await client.move.fetch_move_category(1)
+        ...     print(category.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        ailment
+        """
+        route = Endpoint.get_move_category(name)
+        self._validate_resource(self.cache.move_category, name, route)
+        data = await self._client.request(route)
+        return self.cache.move_category.setdefault(route, MoveCategory.from_payload(data))
+
+    def get_move_damage_class(self, name: t.Union[str, int]) -> t.Optional[MoveDamageClass]:
+        """Gets a move damage class from the cache.
+
+        Parameters
+        ----------
+        name: t.Union[str, int]
+            The id of the move damage class.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.MoveDamageClass]
+            The move damage class if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the move damage class does not exist in the cache.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> damage_class = client.move.get_move_damage_class(1)
+        >>> damage_class.name
+        'status'
+        """
+        route = Endpoint.get_move_damage_class(name)
+        self._validate_resource(self.cache.move_damage_class, name, route)
+        return self.cache.move_damage_class.get(route, None)
+
+    async def fetch_move_damage_class(self, name: t.Union[str, int]) -> t.Optional[MoveDamageClass]:
+        """Fetches a move damage class from the API.
+
+        Parameters
+        ----------
+        name: t.Union[str, int]
+            The id of the move damage class.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.MoveDamageClass]
+            The move damage class if it exists in the API, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the move damage class does not exist in the API.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     damage_class = await client.move.fetch_move_damage_class(1)
+        ...     print(damage_class.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        status
+        """
+        route = Endpoint.get_move_damage_class(name)
+        self._validate_resource(self.cache.move_damage_class, name, route)
+        data = await self._client.request(route)
+        return self.cache.move_damage_class.setdefault(route, MoveDamageClass.from_payload(data))
+
+    def get_move_learn_method(self, name: t.Union[str, int]) -> t.Optional[MoveLearnMethod]:
+        """Gets a move learn method from the cache.
+
+        Parameters
+        ----------
+        name: t.Union[str, int]
+            The id of the move learn method.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.MoveLearnMethod]
+            The move learn method if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the move learn method does not exist in the cache.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> learn_method = client.move.get_move_learn_method(1)
+        >>> learn_method.name
+        'level-up'
+        """
+        route = Endpoint.get_move_learn_method(name)
+        self._validate_resource(self.cache.move_learn_method, name, route)
+        return self.cache.move_learn_method.get(route, None)
+
+    async def fetch_move_learn_method(self, name: t.Union[str, int]) -> t.Optional[MoveLearnMethod]:
+        """Fetches a move learn method from the API.
+
+        Parameters
+        ----------
+        name: t.Union[str, int]
+            The id of the move learn method.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.MoveLearnMethod]
+            The move learn method if it exists in the API, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the move learn method does not exist in the API.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     learn_method = await client.move.fetch_move_learn_method(1)
+        ...     print(learn_method.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        level-up
+        """
+        route = Endpoint.get_move_learn_method(name)
+        self._validate_resource(self.cache.move_learn_method, name, route)
+        data = await self._client.request(route)
+        return self.cache.move_learn_method.setdefault(route, MoveLearnMethod.from_payload(data))
+
+    def get_move_target(self, name: t.Union[str, int]) -> t.Optional[MoveTarget]:
+        """Gets a move target from the cache.
+
+        Parameters
+        ----------
+        name: t.Union[str, int]
+            The id of the move target.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.MoveTarget]
+            The move target if it exists in the cache, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the move target does not exist in the cache.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> target = client.move.get_move_target(1)
+        >>> target.name
+        'specific-pokemon'
+        """
+        route = Endpoint.get_move_target(name)
+        self._validate_resource(self.cache.move_target, name, route)
+        return self.cache.move_target.get(route, None)
+
+    async def fetch_move_target(self, name: t.Union[str, int]) -> t.Optional[MoveTarget]:
+        """Fetches a move target from the API.
+
+        Parameters
+        ----------
+        name: t.Union[str, int]
+            The id of the move target.
+
+        Returns
+        -------
+        typing.Optional[pokelance.models.MoveTarget]
+            The move target if it exists in the API, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the move target does not exist in the API.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     target = await client.move.fetch_move_target(1)
+        ...     print(target.name)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        specific-pokemon
+        """
+        route = Endpoint.get_move_target(name)
+        self._validate_resource(self.cache.move_target, name, route)
+        data = await self._client.request(route)
+        return self.cache.move_target.setdefault(route, MoveTarget.from_payload(data))
+
+
+def setup(lance: "PokeLance") -> None:
+    """Sets up the move cog."""
+    lance.add_extension("move", Move(lance.http))
```

### Comparing `pokelance-0.0.9a0/pokelance/ext/pokemon.py` & `pokelance-0.1.0/pokelance/ext/pokemon.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,1198 +1,1156 @@
-import typing as t
-
-from pokelance.http import Endpoint
-from pokelance.models import (
-    Ability,
-    Characteristic,
-    EggGroup,
-    Gender,
-    GrowthRate,
-    LocationAreaEncounter,
-    Nature,
-    PokeathlonStat,
-)
-from pokelance.models import Pokemon as PokemonModel
-from pokelance.models import PokemonColor, PokemonForm, PokemonHabitats, PokemonShape, PokemonSpecies, Stat, Type
-
-from ._base import BaseExtension
-
-if t.TYPE_CHECKING:
-    from pokelance import PokeLance
-    from pokelance.http import HttpClient
-
-
-__all__: t.Tuple[str, ...] = (
-    "setup",
-    "Pokemon",
-)
-
-
-class Pokemon(BaseExtension):
-    """Extension for pokemon related endpoints.
-
-    Parameters
-    ----------
-    client: pokelance.http.HttpClient
-        The client to use for requests.
-
-    Attributes
-    ----------
-    cache: pokelance.cache.Pokemon
-        The cache for this extension.
-    """
-
-    def __init__(self, client: "HttpClient") -> None:
-        """Initialize the extension."""
-        super().__init__(client)
-        self.cache = self._cache.pokemon
-
-    async def setup(self) -> None:
-        """Sets up the extension."""
-        data = await self._client.request(Endpoint.get_ability_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "ability", data["results"])
-        data = await self._client.request(Endpoint.get_characteristic_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "characteristic", data["results"])
-        data = await self._client.request(Endpoint.get_egg_group_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "egg_group", data["results"])
-        data = await self._client.request(Endpoint.get_gender_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "gender", data["results"])
-        data = await self._client.request(Endpoint.get_growth_rate_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "growth_rate", data["results"])
-        data = await self._client.request(Endpoint.get_nature_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "nature", data["results"])
-        data = await self._client.request(Endpoint.get_pokeathlon_stat_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "pokeathlon_stat", data["results"])
-        data = await self._client.request(Endpoint.get_pokemon_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "pokemon", data["results"])
-        self._cache.load_documents(str(self.__class__.__name__), "location_area", data["results"])
-        data = await self._client.request(Endpoint.get_pokemon_color_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "pokemon_color", data["results"])
-        data = await self._client.request(Endpoint.get_pokemon_form_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "pokemon_form", data["results"])
-        data = await self._client.request(Endpoint.get_pokemon_habitat_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "pokemon_habitat", data["results"])
-        data = await self._client.request(Endpoint.get_pokemon_shape_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "pokemon_shape", data["results"])
-        data = await self._client.request(Endpoint.get_pokemon_species_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "pokemon_species", data["results"])
-        data = await self._client.request(Endpoint.get_stat_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "stat", data["results"])
-        data = await self._client.request(Endpoint.get_type_endpoints())
-        self._cache.load_documents(str(self.__class__.__name__), "type", data["results"])
-
-    def get_ability(self, name: t.Union[str, int]) -> t.Optional[Ability]:
-        """Get an ability by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the ability.
-
-        Returns
-        -------
-        Optional[Ability]
-            The ability if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the ability was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> ability = client.pokemon.get_ability("stench")
-        >>> ability.id
-        1
-        """
-        route = Endpoint.get_ability(name)
-        self._validate_resource(self.cache.ability, name, route)
-        return self.cache.ability.get(route, None)
-
-    async def fetch_ability(self, name: t.Union[str, int]) -> t.Optional[Ability]:
-        """Fetch an ability by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the ability.
-
-        Returns
-        -------
-        Optional[Ability]
-            The ability if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the ability was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     ability = await client.pokemon.fetch_ability("stench")
-        ...     print(ability.id)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        1
-        """
-        route = Endpoint.get_ability(name)
-        self._validate_resource(self.cache.ability, name, route)
-        data = await self._client.request(route)
-        return self.cache.ability.setdefault(route, Ability.from_payload(data))
-
-    def get_characteristic(self, id_: int) -> t.Optional[Characteristic]:
-        """Get a characteristic by id.
-
-        Parameters
-        ----------
-        id_: int
-            The id of the characteristic.
-
-        Returns
-        -------
-        Optional[Characteristic]
-            The characteristic if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the characteristic was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> characteristic = client.pokemon.get_characteristic(1)
-        >>> characteristic.gene_modulo
-        0
-        """
-        route = Endpoint.get_characteristic(id_)
-        self._validate_resource(self.cache.characteristic, id_, route)
-        return self.cache.characteristic.get(route, None)
-
-    async def fetch_characteristic(self, id_: int) -> t.Optional[Characteristic]:
-        """Fetch a characteristic by id.
-
-        Parameters
-        ----------
-        id_: int
-            The id of the characteristic.
-
-        Returns
-        -------
-        Optional[Characteristic]
-            The characteristic if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the characteristic was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     characteristic = await client.pokemon.fetch_characteristic(1)
-        ...     print(characteristic.gene_modulo)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        0
-        """
-        route = Endpoint.get_characteristic(id_)
-        self._validate_resource(self.cache.characteristic, id_, route)
-        data = await self._client.request(route)
-        return self.cache.characteristic.setdefault(route, Characteristic.from_payload(data))
-
-    def get_egg_group(self, name: t.Union[str, int]) -> t.Optional[EggGroup]:
-        """Get an egg group by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the egg group.
-
-        Returns
-        -------
-        Optional[EggGroup]
-            The egg group if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the egg group was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> egg_group = client.pokemon.get_egg_group("monster")
-        >>> egg_group.id
-        1
-        """
-        route = Endpoint.get_egg_group(name)
-        self._validate_resource(self.cache.egg_group, name, route)
-        return self.cache.egg_group.get(route, None)
-
-    async def fetch_egg_group(self, name: t.Union[str, int]) -> t.Optional[EggGroup]:
-        """Fetch an egg group by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the egg group.
-
-        Returns
-        -------
-        Optional[EggGroup]
-            The egg group if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            If the egg group was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...     egg_group = await client.pokemon.fetch_egg_group("monster")
-        ...     print(egg_group.id)
-        ...     await client.close()
-        >>> asyncio.run(main())
-        1
-        """
-        route = Endpoint.get_egg_group(name)
-        self._validate_resource(self.cache.egg_group, name, route)
-        data = await self._client.request(route)
-        return self.cache.egg_group.setdefault(route, EggGroup.from_payload(data))
-
-    def get_gender(self, name: t.Union[str, int]) -> t.Optional[Gender]:
-        """
-        Get gender from cache.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the gender.
-
-        Returns
-        -------
-        t.Optional[Gender]
-            Gender model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if gender was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> gender = client.pokemon.get_gender(1)
-        >>> gender.name
-        'female'
-        """
-        route = Endpoint.get_gender(name)
-        self._validate_resource(self.cache.gender, name, route)
-        return self.cache.gender.get(route, None)
-
-    async def fetch_gender(self, name: t.Union[str, int]) -> t.Optional[Gender]:
-        """
-        Fetches a gender model by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the
-
-        Returns
-        -------
-        t.Optional[Gender]
-            Gender model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if gender was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...    gender = await client.pokemon.fetch_gender(1)
-        ...    print(gender.name)
-        ...    await client.close()
-        >>> asyncio.run(main())
-        female
-        """
-        route = Endpoint.get_gender(name)
-        self._validate_resource(self.cache.gender, name, route)
-        data = await self._client.request(route)
-        return self.cache.gender.setdefault(route, Gender.from_payload(data))
-
-    def get_growth_rate(self, name: t.Union[str, int]) -> t.Optional[GrowthRate]:
-        """
-        Get growth rate from cache.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the growth rate.
-
-        Returns
-        -------
-        t.Optional[GrowthRate]
-            Growth rate model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if growth rate was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> growth_rate = client.pokemon.get_growth_rate(1)
-        >>> growth_rate.name
-        'slow'
-        """
-        route = Endpoint.get_growth_rate(name)
-        self._validate_resource(self.cache.growth_rate, name, route)
-        return self.cache.growth_rate.get(route, None)
-
-    async def fetch_growth_rate(self, name: t.Union[str, int]) -> t.Optional[GrowthRate]:
-        """
-        Fetches a growth rate model by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the
-
-        Returns
-        -------
-        t.Optional[GrowthRate]
-            Growth rate model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if growth rate was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...    growth_rate = await client.pokemon.fetch_growth_rate(1)
-        ...    print(growth_rate.name)
-        ...    await client.close()
-        >>> asyncio.run(main())
-        slow
-        """
-        route = Endpoint.get_growth_rate(name)
-        self._validate_resource(self.cache.growth_rate, name, route)
-        data = await self._client.request(route)
-        return self.cache.growth_rate.setdefault(route, GrowthRate.from_payload(data))
-
-    def get_nature(self, name: t.Union[str, int]) -> t.Optional[Nature]:
-        """
-        Get nature from cache.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the nature.
-
-        Returns
-        -------
-        t.Optional[Nature]
-            Nature model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if nature was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> nature = client.pokemon.get_nature(1)
-        >>> nature.name
-        'hardy'
-        """
-        route = Endpoint.get_nature(name)
-        self._validate_resource(self.cache.nature, name, route)
-        return self.cache.nature.get(route, None)
-
-    async def fetch_nature(self, name: t.Union[str, int]) -> t.Optional[Nature]:
-        """
-        Fetches a nature model by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the
-
-        Returns
-        -------
-        t.Optional[Nature]
-            Nature model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if nature was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...    nature = await client.pokemon.fetch_nature(1)
-        ...    print(nature.name)
-        ...    await client.close()
-        >>> asyncio.run(main())
-        hardy
-        """
-        route = Endpoint.get_nature(name)
-        self._validate_resource(self.cache.nature, name, route)
-        data = await self._client.request(route)
-        return self.cache.nature.setdefault(route, Nature.from_payload(data))
-
-    def get_pokeathlon_stat(self, name: t.Union[str, int]) -> t.Optional[PokeathlonStat]:
-        """
-        Get pokeathlon stat from cache.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the pokeathlon stat.
-
-        Returns
-        -------
-        t.Optional[PokeathlonStat]
-            Pokeathlon stat model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if pokeathlon stat was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> pokeathlon_stat = client.pokemon.get_pokeathlon_stat(1)
-        >>> pokeathlon_stat.name
-        'speed'
-        """
-        route = Endpoint.get_pokeathlon_stat(name)
-        self._validate_resource(self.cache.pokeathlon_stat, name, route)
-        return self.cache.pokeathlon_stat.get(route, None)
-
-    async def fetch_pokeathlon_stat(self, name: t.Union[str, int]) -> t.Optional[PokeathlonStat]:
-        """
-        Fetches a pokeathlon stat model by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the
-
-        Returns
-        -------
-        t.Optional[PokeathlonStat]
-            Pokeathlon stat model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if pokeathlon stat was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...    pokeathlon_stat = await client.pokemon.fetch_pokeathlon_stat(1)
-        ...    print(pokeathlon_stat.name)
-        ...    await client.close()
-        >>> asyncio.run(main())
-        speed
-        """
-        route = Endpoint.get_pokeathlon_stat(name)
-        self._validate_resource(self.cache.pokeathlon_stat, name, route)
-        data = await self._client.request(route)
-        return self.cache.pokeathlon_stat.setdefault(route, PokeathlonStat.from_payload(data))
-
-    def get_location_area_encounter(self, name: t.Union[str, int]) -> t.Optional[LocationAreaEncounter]:
-        """
-        Get location area encounter from cache.
-        It gets areas where a pokemon can be found.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the location area encounter.
-
-        Returns
-        -------
-        t.Optional[LocationAreaEncounter]
-            Location area encounter model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if location area encounter was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> location_area_encounter = client.pokemon.get_location_area_encounter(1)
-        >>> location_area_encounter.location_area.name
-        'cerulean-city-area'
-        """
-        route = Endpoint.get_location_area_encounter(name)
-        self._validate_resource(self.cache.location_area, name, route)
-        return self.cache.location_area.get(route, None)
-
-    async def fetch_location_area_encounter(self, name: t.Union[str, int]) -> t.Optional[LocationAreaEncounter]:
-        """
-        Fetches a location area encounter model by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the
-
-        Returns
-        -------
-        t.Optional[LocationAreaEncounter]
-            Location area encounter model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if location area encounter was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...    location_area_encounter = await client.pokemon.fetch_location_area_encounter(1)
-        ...    print(location_area_encounter.location_area.name)
-        ...    await client.close()
-        >>> asyncio.run(main())
-        cerulean-city-area
-        """
-        route = Endpoint.get_location_area_encounter(name)
-        self._validate_resource(self.cache.location_area, name, route)
-        data = await self._client.request(route)
-        return self.cache.location_area.setdefault(route, LocationAreaEncounter.from_payload(data[0]))
-
-    def get_pokemon(self, name: t.Union[str, int]) -> t.Optional[PokemonModel]:
-        """
-        Get pokemon from cache.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the pokemon.
-
-        Returns
-        -------
-        t.Optional[PokemonModel]
-            Pokemon model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if pokemon was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> pokemon = client.pokemon.get_pokemon(1)
-        >>> pokemon.name
-        'bulbasaur'
-        """
-        route = Endpoint.get_pokemon(name)
-        self._validate_resource(self.cache.pokemon, name, route)
-        return self.cache.pokemon.get(route, None)
-
-    async def fetch_pokemon(self, name: t.Union[str, int]) -> t.Optional[PokemonModel]:
-        """
-        Fetches a pokemon model by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the
-
-        Returns
-        -------
-        t.Optional[PokemonModel]
-            Pokemon model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if pokemon was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...    pokemon = await client.pokemon.fetch_pokemon(1)
-        ...    print(pokemon.name)
-        ...    await client.close()
-        >>> asyncio.run(main())
-        bulbasaur
-        """
-        route = Endpoint.get_pokemon(name)
-        self._validate_resource(self.cache.pokemon, name, route)
-        data = await self._client.request(route)
-        return self.cache.pokemon.setdefault(route, PokemonModel.from_payload(data))
-
-    def get_pokemon_color(self, name: t.Union[str, int]) -> t.Optional[PokemonColor]:
-        """
-        Get pokemon color from cache.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the pokemon color.
-
-        Returns
-        -------
-        t.Optional[PokemonColor]
-            Pokemon color model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if pokemon color was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> pokemon_color = client.pokemon.get_pokemon_color(1)
-        >>> pokemon_color.name
-        'black'
-        """
-        route = Endpoint.get_pokemon_color(name)
-        self._validate_resource(self.cache.pokemon_color, name, route)
-        return self.cache.pokemon_color.get(route, None)
-
-    async def fetch_pokemon_color(self, name: t.Union[str, int]) -> t.Optional[PokemonColor]:
-        """
-        Fetches a pokemon color model by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the
-
-        Returns
-        -------
-        t.Optional[PokemonColor]
-            Pokemon color model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if pokemon color was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...    pokemon_color = await client.pokemon.fetch_pokemon_color(1)
-        ...    print(pokemon_color.name)
-        ...    await client.close()
-        >>> asyncio.run(main())
-        black
-        """
-        route = Endpoint.get_pokemon_color(name)
-        self._validate_resource(self.cache.pokemon_color, name, route)
-        data = await self._client.request(route)
-        return self.cache.pokemon_color.setdefault(route, PokemonColor.from_payload(data))
-
-    def get_pokemon_form(self, name: t.Union[str, int]) -> t.Optional[PokemonForm]:
-        """
-        Get pokemon form from cache.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the pokemon form.
-
-        Returns
-        -------
-        t.Optional[PokemonForm]
-            Pokemon form model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if pokemon form was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> pokemon_form = client.pokemon.get_pokemon_form(1)
-        >>> pokemon_form.name
-        'bulbasaur'
-        """
-        route = Endpoint.get_pokemon_form(name)
-        self._validate_resource(self.cache.pokemon_form, name, route)
-        return self.cache.pokemon_form.get(route, None)
-
-    async def fetch_pokemon_form(self, name: t.Union[str, int]) -> t.Optional[PokemonForm]:
-        """
-        Fetches a pokemon form model by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the
-
-        Returns
-        -------
-        t.Optional[PokemonForm]
-            Pokemon form model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if pokemon form was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...    pokemon_form = await client.pokemon.fetch_pokemon_form(1)
-        ...    print(pokemon_form.name)
-        ...    await client.close()
-        >>> asyncio.run(main())
-        bulbasaur
-        """
-        route = Endpoint.get_pokemon_form(name)
-        self._validate_resource(self.cache.pokemon_form, name, route)
-        data = await self._client.request(route)
-        return self.cache.pokemon_form.setdefault(route, PokemonForm.from_payload(data))
-
-    def get_pokemon_habitat(self, name: t.Union[str, int]) -> t.Optional[PokemonHabitats]:
-        """
-        Get pokemon habitat from cache.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the pokemon habitat.
-
-        Returns
-        -------
-        t.Optional[PokemonHabitats]
-            Pokemon habitat model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if pokemon habitat was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> pokemon_habitat = client.pokemon.get_pokemon_habitat(1)
-        >>> pokemon_habitat.name
-        'cave'
-        """
-        route = Endpoint.get_pokemon_habitat(name)
-        self._validate_resource(self.cache.pokemon_habitat, name, route)
-        return self.cache.pokemon_habitat.get(route, None)
-
-    async def fetch_pokemon_habitat(self, name: t.Union[str, int]) -> t.Optional[PokemonHabitats]:
-        """
-        Fetches a pokemon habitat model by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the
-
-        Returns
-        -------
-        t.Optional[PokemonHabitats]
-            Pokemon habitat model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if pokemon habitat was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...    pokemon_habitat = await client.pokemon.fetch_pokemon_habitat(1)
-        ...    print(pokemon_habitat.name)
-        ...    await client.close()
-        >>> asyncio.run(main())
-        cave
-        """
-        route = Endpoint.get_pokemon_habitat(name)
-        self._validate_resource(self.cache.pokemon_habitat, name, route)
-        data = await self._client.request(route)
-        return self.cache.pokemon_habitat.setdefault(route, PokemonHabitats.from_payload(data))
-
-    def get_pokemon_shape(self, name: t.Union[str, int]) -> t.Optional[PokemonShape]:
-        """
-        Get pokemon shape from cache.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the pokemon shape.
-
-        Returns
-        -------
-        t.Optional[PokemonShape]
-            Pokemon shape model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if pokemon shape was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> pokemon_shape = client.pokemon.get_pokemon_shape(1)
-        >>> pokemon_shape.name
-        'ball'
-        """
-        route = Endpoint.get_pokemon_shape(name)
-        self._validate_resource(self.cache.pokemon_shape, name, route)
-        return self.cache.pokemon_shape.get(route, None)
-
-    async def fetch_pokemon_shape(self, name: t.Union[str, int]) -> t.Optional[PokemonShape]:
-        """
-        Fetches a pokemon shape model by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the
-
-        Returns
-        -------
-        t.Optional[PokemonShape]
-            Pokemon shape model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if pokemon shape was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...    pokemon_shape = await client.pokemon.fetch_pokemon_shape(1)
-        ...    print(pokemon_shape.name)
-        ...    await client.close()
-        >>> asyncio.run(main())
-        ball
-        """
-        route = Endpoint.get_pokemon_shape(name)
-        self._validate_resource(self.cache.pokemon_shape, name, route)
-        data = await self._client.request(route)
-        return self.cache.pokemon_shape.setdefault(route, PokemonShape.from_payload(data))
-
-    def get_pokemon_species(self, name: t.Union[str, int]) -> t.Optional[PokemonSpecies]:
-        """
-        Get pokemon species from cache.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the pokemon species.
-
-        Returns
-        -------
-        t.Optional[PokemonSpecies]
-            Pokemon species model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if pokemon species was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> pokemon_species = client.pokemon.get_pokemon_species(1)
-        >>> pokemon_species.name
-        'bulbasaur'
-        """
-        route = Endpoint.get_pokemon_species(name)
-        self._validate_resource(self.cache.pokemon_species, name, route)
-        return self.cache.pokemon_species.get(route, None)
-
-    async def fetch_pokemon_species(self, name: t.Union[str, int]) -> t.Optional[PokemonSpecies]:
-        """
-        Fetches a pokemon species model by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the
-
-        Returns
-        -------
-        t.Optional[PokemonSpecies]
-            Pokemon species model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if pokemon species was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...    pokemon_species = await client.pokemon.fetch_pokemon_species(1)
-        ...    print(pokemon_species.name)
-        ...    await client.close()
-        >>> asyncio.run(main())
-        bulbasaur
-        """
-        route = Endpoint.get_pokemon_species(name)
-        self._validate_resource(self.cache.pokemon_species, name, route)
-        data = await self._client.request(route)
-        return self.cache.pokemon_species.setdefault(route, PokemonSpecies.from_payload(data))
-
-    def get_stat(self, name: t.Union[str, int]) -> t.Optional[Stat]:
-        """
-        Get stat from cache.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the stat.
-
-        Returns
-        -------
-        t.Optional[Stat]
-            Stat model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if stat was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> stat = client.pokemon.get_stat(1)
-        >>> stat.name
-        'hp'
-        """
-        route = Endpoint.get_stat(name)
-        self._validate_resource(self.cache.stat, name, route)
-        return self.cache.stat.get(route, None)
-
-    async def fetch_stat(self, name: t.Union[str, int]) -> t.Optional[Stat]:
-        """
-        Fetches a stat model by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the
-
-        Returns
-        -------
-        t.Optional[Stat]
-            Stat model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if stat was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...    stat = await client.pokemon.fetch_stat(1)
-        ...    print(stat.name)
-        ...    await client.close()
-        >>> asyncio.run(main())
-        hp
-        """
-        route = Endpoint.get_stat(name)
-        self._validate_resource(self.cache.stat, name, route)
-        data = await self._client.request(route)
-        return self.cache.stat.setdefault(route, Stat.from_payload(data))
-
-    def get_type(self, name: t.Union[str, int]) -> t.Optional[Type]:
-        """
-        Get type from cache.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the type.
-
-        Returns
-        -------
-        t.Optional[Type]
-            Type model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if type was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> client = PokeLance()
-        >>> type_ = client.pokemon.get_type(1)
-        >>> type_.name
-        'normal'
-        """
-        route = Endpoint.get_type(name)
-        self._validate_resource(self.cache.type, name, route)
-        return self.cache.type.get(route, None)
-
-    async def fetch_type(self, name: t.Union[str, int]) -> t.Optional[Type]:
-        """
-        Fetches a type model by name or id.
-
-        Parameters
-        ----------
-        name: Union[str, int]
-            The name or id of the
-
-        Returns
-        -------
-        t.Optional[Type]
-            Type model if found, else None.
-
-        Raises
-        ------
-        pokelance.exceptions.ResourceNotFound
-            if type was not found.
-
-        Examples
-        --------
-
-        >>> from pokelance import PokeLance
-        >>> import asyncio
-        >>> client = PokeLance()
-        >>> async def main() -> None:
-        ...    type_ = await client.pokemon.fetch_type(1)
-        ...    print(type_.name)
-        ...    await client.close()
-        >>> asyncio.run(main())
-        normal
-        """
-        route = Endpoint.get_type(name)
-        self._validate_resource(self.cache.type, name, route)
-        data = await self._client.request(route)
-        return self.cache.type.setdefault(route, Type.from_payload(data))
-
-    @property
-    def all_pokemons(self) -> t.Optional[t.List[str]]:
-        """
-        Returns a list of all pokemon names.
-
-        Returns
-        -------
-        t.Optional[t.List[str]]
-            List of all pokemon names. None if not cached yet.
-        """
-        data = list(self.cache.pokemon.endpoints.keys())
-        return data if data else None
-
-
-def setup(lance: "PokeLance") -> None:
-    """Setup the pokemon cog."""
-    lance.add_extension("pokemon", Pokemon(lance.http))
+import typing as t
+
+from pokelance.http import Endpoint
+from pokelance.models import (
+    Ability,
+    Characteristic,
+    EggGroup,
+    Gender,
+    GrowthRate,
+    LocationAreaEncounter,
+    Nature,
+    PokeathlonStat,
+)
+from pokelance.models import Pokemon as PokemonModel
+from pokelance.models import PokemonColor, PokemonForm, PokemonHabitats, PokemonShape, PokemonSpecies, Stat, Type
+
+from ._base import BaseExtension
+
+if t.TYPE_CHECKING:
+    from pokelance import PokeLance
+    from pokelance.cache import Pokemon as PokemonCache
+
+
+__all__: t.Tuple[str, ...] = (
+    "setup",
+    "Pokemon",
+)
+
+
+class Pokemon(BaseExtension):
+    """Extension for pokemon related endpoints.
+
+    Attributes
+    ----------
+    cache: pokelance.cache.Pokemon
+        The cache for this extension.
+    """
+
+    cache: "PokemonCache"
+
+    def get_ability(self, name: t.Union[str, int]) -> t.Optional[Ability]:
+        """Get an ability by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the ability.
+
+        Returns
+        -------
+        Optional[Ability]
+            The ability if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the ability was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> ability = client.pokemon.get_ability("stench")
+        >>> ability.id
+        1
+        """
+        route = Endpoint.get_ability(name)
+        self._validate_resource(self.cache.ability, name, route)
+        return self.cache.ability.get(route, None)
+
+    async def fetch_ability(self, name: t.Union[str, int]) -> t.Optional[Ability]:
+        """Fetch an ability by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the ability.
+
+        Returns
+        -------
+        Optional[Ability]
+            The ability if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the ability was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     ability = await client.pokemon.fetch_ability("stench")
+        ...     print(ability.id)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        1
+        """
+        route = Endpoint.get_ability(name)
+        self._validate_resource(self.cache.ability, name, route)
+        data = await self._client.request(route)
+        return self.cache.ability.setdefault(route, Ability.from_payload(data))
+
+    def get_characteristic(self, id_: int) -> t.Optional[Characteristic]:
+        """Get a characteristic by id.
+
+        Parameters
+        ----------
+        id_: int
+            The id of the characteristic.
+
+        Returns
+        -------
+        Optional[Characteristic]
+            The characteristic if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the characteristic was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> characteristic = client.pokemon.get_characteristic(1)
+        >>> characteristic.gene_modulo
+        0
+        """
+        route = Endpoint.get_characteristic(id_)
+        self._validate_resource(self.cache.characteristic, id_, route)
+        return self.cache.characteristic.get(route, None)
+
+    async def fetch_characteristic(self, id_: int) -> t.Optional[Characteristic]:
+        """Fetch a characteristic by id.
+
+        Parameters
+        ----------
+        id_: int
+            The id of the characteristic.
+
+        Returns
+        -------
+        Optional[Characteristic]
+            The characteristic if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the characteristic was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     characteristic = await client.pokemon.fetch_characteristic(1)
+        ...     print(characteristic.gene_modulo)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        0
+        """
+        route = Endpoint.get_characteristic(id_)
+        self._validate_resource(self.cache.characteristic, id_, route)
+        data = await self._client.request(route)
+        return self.cache.characteristic.setdefault(route, Characteristic.from_payload(data))
+
+    def get_egg_group(self, name: t.Union[str, int]) -> t.Optional[EggGroup]:
+        """Get an egg group by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the egg group.
+
+        Returns
+        -------
+        Optional[EggGroup]
+            The egg group if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the egg group was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> egg_group = client.pokemon.get_egg_group("monster")
+        >>> egg_group.id
+        1
+        """
+        route = Endpoint.get_egg_group(name)
+        self._validate_resource(self.cache.egg_group, name, route)
+        return self.cache.egg_group.get(route, None)
+
+    async def fetch_egg_group(self, name: t.Union[str, int]) -> t.Optional[EggGroup]:
+        """Fetch an egg group by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the egg group.
+
+        Returns
+        -------
+        Optional[EggGroup]
+            The egg group if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            If the egg group was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...     egg_group = await client.pokemon.fetch_egg_group("monster")
+        ...     print(egg_group.id)
+        ...     await client.close()
+        >>> asyncio.run(main())
+        1
+        """
+        route = Endpoint.get_egg_group(name)
+        self._validate_resource(self.cache.egg_group, name, route)
+        data = await self._client.request(route)
+        return self.cache.egg_group.setdefault(route, EggGroup.from_payload(data))
+
+    def get_gender(self, name: t.Union[str, int]) -> t.Optional[Gender]:
+        """
+        Get gender from cache.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the gender.
+
+        Returns
+        -------
+        t.Optional[Gender]
+            Gender model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if gender was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> gender = client.pokemon.get_gender(1)
+        >>> gender.name
+        'female'
+        """
+        route = Endpoint.get_gender(name)
+        self._validate_resource(self.cache.gender, name, route)
+        return self.cache.gender.get(route, None)
+
+    async def fetch_gender(self, name: t.Union[str, int]) -> t.Optional[Gender]:
+        """
+        Fetches a gender model by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the
+
+        Returns
+        -------
+        t.Optional[Gender]
+            Gender model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if gender was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...    gender = await client.pokemon.fetch_gender(1)
+        ...    print(gender.name)
+        ...    await client.close()
+        >>> asyncio.run(main())
+        female
+        """
+        route = Endpoint.get_gender(name)
+        self._validate_resource(self.cache.gender, name, route)
+        data = await self._client.request(route)
+        return self.cache.gender.setdefault(route, Gender.from_payload(data))
+
+    def get_growth_rate(self, name: t.Union[str, int]) -> t.Optional[GrowthRate]:
+        """
+        Get growth rate from cache.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the growth rate.
+
+        Returns
+        -------
+        t.Optional[GrowthRate]
+            Growth rate model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if growth rate was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> growth_rate = client.pokemon.get_growth_rate(1)
+        >>> growth_rate.name
+        'slow'
+        """
+        route = Endpoint.get_growth_rate(name)
+        self._validate_resource(self.cache.growth_rate, name, route)
+        return self.cache.growth_rate.get(route, None)
+
+    async def fetch_growth_rate(self, name: t.Union[str, int]) -> t.Optional[GrowthRate]:
+        """
+        Fetches a growth rate model by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the
+
+        Returns
+        -------
+        t.Optional[GrowthRate]
+            Growth rate model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if growth rate was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...    growth_rate = await client.pokemon.fetch_growth_rate(1)
+        ...    print(growth_rate.name)
+        ...    await client.close()
+        >>> asyncio.run(main())
+        slow
+        """
+        route = Endpoint.get_growth_rate(name)
+        self._validate_resource(self.cache.growth_rate, name, route)
+        data = await self._client.request(route)
+        return self.cache.growth_rate.setdefault(route, GrowthRate.from_payload(data))
+
+    def get_nature(self, name: t.Union[str, int]) -> t.Optional[Nature]:
+        """
+        Get nature from cache.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the nature.
+
+        Returns
+        -------
+        t.Optional[Nature]
+            Nature model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if nature was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> nature = client.pokemon.get_nature(1)
+        >>> nature.name
+        'hardy'
+        """
+        route = Endpoint.get_nature(name)
+        self._validate_resource(self.cache.nature, name, route)
+        return self.cache.nature.get(route, None)
+
+    async def fetch_nature(self, name: t.Union[str, int]) -> t.Optional[Nature]:
+        """
+        Fetches a nature model by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the
+
+        Returns
+        -------
+        t.Optional[Nature]
+            Nature model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if nature was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...    nature = await client.pokemon.fetch_nature(1)
+        ...    print(nature.name)
+        ...    await client.close()
+        >>> asyncio.run(main())
+        hardy
+        """
+        route = Endpoint.get_nature(name)
+        self._validate_resource(self.cache.nature, name, route)
+        data = await self._client.request(route)
+        return self.cache.nature.setdefault(route, Nature.from_payload(data))
+
+    def get_pokeathlon_stat(self, name: t.Union[str, int]) -> t.Optional[PokeathlonStat]:
+        """
+        Get pokeathlon stat from cache.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the pokeathlon stat.
+
+        Returns
+        -------
+        t.Optional[PokeathlonStat]
+            Pokeathlon stat model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if pokeathlon stat was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> pokeathlon_stat = client.pokemon.get_pokeathlon_stat(1)
+        >>> pokeathlon_stat.name
+        'speed'
+        """
+        route = Endpoint.get_pokeathlon_stat(name)
+        self._validate_resource(self.cache.pokeathlon_stat, name, route)
+        return self.cache.pokeathlon_stat.get(route, None)
+
+    async def fetch_pokeathlon_stat(self, name: t.Union[str, int]) -> t.Optional[PokeathlonStat]:
+        """
+        Fetches a pokeathlon stat model by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the
+
+        Returns
+        -------
+        t.Optional[PokeathlonStat]
+            Pokeathlon stat model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if pokeathlon stat was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...    pokeathlon_stat = await client.pokemon.fetch_pokeathlon_stat(1)
+        ...    print(pokeathlon_stat.name)
+        ...    await client.close()
+        >>> asyncio.run(main())
+        speed
+        """
+        route = Endpoint.get_pokeathlon_stat(name)
+        self._validate_resource(self.cache.pokeathlon_stat, name, route)
+        data = await self._client.request(route)
+        return self.cache.pokeathlon_stat.setdefault(route, PokeathlonStat.from_payload(data))
+
+    def get_location_area_encounter(self, name: t.Union[str, int]) -> t.Optional[LocationAreaEncounter]:
+        """
+        Get location area encounter from cache.
+        It gets areas where a pokemon can be found.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the location area encounter.
+
+        Returns
+        -------
+        t.Optional[LocationAreaEncounter]
+            Location area encounter model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if location area encounter was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> location_area_encounter = client.pokemon.get_location_area_encounter(1)
+        >>> location_area_encounter.location_area.name
+        'cerulean-city-area'
+        """
+        route = Endpoint.get_location_area_encounter(name)
+        self._validate_resource(self.cache.location_area_encounter, name, route)
+        return self.cache.location_area_encounter.get(route, None)
+
+    async def fetch_location_area_encounter(self, name: t.Union[str, int]) -> t.Optional[LocationAreaEncounter]:
+        """
+        Fetches a location area encounter model by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the
+
+        Returns
+        -------
+        t.Optional[LocationAreaEncounter]
+            Location area encounter model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if location area encounter was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...    location_area_encounter = await client.pokemon.fetch_location_area_encounter(1)
+        ...    print(location_area_encounter.location_area.name)
+        ...    await client.close()
+        >>> asyncio.run(main())
+        cerulean-city-area
+        """
+        route = Endpoint.get_location_area_encounter(name)
+        self._validate_resource(self.cache.location_area_encounter, name, route)
+        data = await self._client.request(route)
+        return self.cache.location_area_encounter.setdefault(route, LocationAreaEncounter.from_payload(data[0]))
+
+    def get_pokemon(self, name: t.Union[str, int]) -> t.Optional[PokemonModel]:
+        """
+        Get pokemon from cache.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the pokemon.
+
+        Returns
+        -------
+        t.Optional[PokemonModel]
+            Pokemon model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if pokemon was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> pokemon = client.pokemon.get_pokemon(1)
+        >>> pokemon.name
+        'bulbasaur'
+        """
+        route = Endpoint.get_pokemon(name)
+        self._validate_resource(self.cache.pokemon, name, route)
+        return self.cache.pokemon.get(route, None)
+
+    async def fetch_pokemon(self, name: t.Union[str, int]) -> t.Optional[PokemonModel]:
+        """
+        Fetches a pokemon model by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the
+
+        Returns
+        -------
+        t.Optional[PokemonModel]
+            Pokemon model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if pokemon was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...    pokemon = await client.pokemon.fetch_pokemon(1)
+        ...    print(pokemon.name)
+        ...    await client.close()
+        >>> asyncio.run(main())
+        bulbasaur
+        """
+        route = Endpoint.get_pokemon(name)
+        self._validate_resource(self.cache.pokemon, name, route)
+        data = await self._client.request(route)
+        return self.cache.pokemon.setdefault(route, PokemonModel.from_payload(data))
+
+    def get_pokemon_color(self, name: t.Union[str, int]) -> t.Optional[PokemonColor]:
+        """
+        Get pokemon color from cache.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the pokemon color.
+
+        Returns
+        -------
+        t.Optional[PokemonColor]
+            Pokemon color model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if pokemon color was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> pokemon_color = client.pokemon.get_pokemon_color(1)
+        >>> pokemon_color.name
+        'black'
+        """
+        route = Endpoint.get_pokemon_color(name)
+        self._validate_resource(self.cache.pokemon_color, name, route)
+        return self.cache.pokemon_color.get(route, None)
+
+    async def fetch_pokemon_color(self, name: t.Union[str, int]) -> t.Optional[PokemonColor]:
+        """
+        Fetches a pokemon color model by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the
+
+        Returns
+        -------
+        t.Optional[PokemonColor]
+            Pokemon color model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if pokemon color was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...    pokemon_color = await client.pokemon.fetch_pokemon_color(1)
+        ...    print(pokemon_color.name)
+        ...    await client.close()
+        >>> asyncio.run(main())
+        black
+        """
+        route = Endpoint.get_pokemon_color(name)
+        self._validate_resource(self.cache.pokemon_color, name, route)
+        data = await self._client.request(route)
+        return self.cache.pokemon_color.setdefault(route, PokemonColor.from_payload(data))
+
+    def get_pokemon_form(self, name: t.Union[str, int]) -> t.Optional[PokemonForm]:
+        """
+        Get pokemon form from cache.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the pokemon form.
+
+        Returns
+        -------
+        t.Optional[PokemonForm]
+            Pokemon form model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if pokemon form was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> pokemon_form = client.pokemon.get_pokemon_form(1)
+        >>> pokemon_form.name
+        'bulbasaur'
+        """
+        route = Endpoint.get_pokemon_form(name)
+        self._validate_resource(self.cache.pokemon_form, name, route)
+        return self.cache.pokemon_form.get(route, None)
+
+    async def fetch_pokemon_form(self, name: t.Union[str, int]) -> t.Optional[PokemonForm]:
+        """
+        Fetches a pokemon form model by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the
+
+        Returns
+        -------
+        t.Optional[PokemonForm]
+            Pokemon form model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if pokemon form was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...    pokemon_form = await client.pokemon.fetch_pokemon_form(1)
+        ...    print(pokemon_form.name)
+        ...    await client.close()
+        >>> asyncio.run(main())
+        bulbasaur
+        """
+        route = Endpoint.get_pokemon_form(name)
+        self._validate_resource(self.cache.pokemon_form, name, route)
+        data = await self._client.request(route)
+        return self.cache.pokemon_form.setdefault(route, PokemonForm.from_payload(data))
+
+    def get_pokemon_habitat(self, name: t.Union[str, int]) -> t.Optional[PokemonHabitats]:
+        """
+        Get pokemon habitat from cache.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the pokemon habitat.
+
+        Returns
+        -------
+        t.Optional[PokemonHabitats]
+            Pokemon habitat model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if pokemon habitat was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> pokemon_habitat = client.pokemon.get_pokemon_habitat(1)
+        >>> pokemon_habitat.name
+        'cave'
+        """
+        route = Endpoint.get_pokemon_habitat(name)
+        self._validate_resource(self.cache.pokemon_habitat, name, route)
+        return self.cache.pokemon_habitat.get(route, None)
+
+    async def fetch_pokemon_habitat(self, name: t.Union[str, int]) -> t.Optional[PokemonHabitats]:
+        """
+        Fetches a pokemon habitat model by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the
+
+        Returns
+        -------
+        t.Optional[PokemonHabitats]
+            Pokemon habitat model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if pokemon habitat was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...    pokemon_habitat = await client.pokemon.fetch_pokemon_habitat(1)
+        ...    print(pokemon_habitat.name)
+        ...    await client.close()
+        >>> asyncio.run(main())
+        cave
+        """
+        route = Endpoint.get_pokemon_habitat(name)
+        self._validate_resource(self.cache.pokemon_habitat, name, route)
+        data = await self._client.request(route)
+        return self.cache.pokemon_habitat.setdefault(route, PokemonHabitats.from_payload(data))
+
+    def get_pokemon_shape(self, name: t.Union[str, int]) -> t.Optional[PokemonShape]:
+        """
+        Get pokemon shape from cache.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the pokemon shape.
+
+        Returns
+        -------
+        t.Optional[PokemonShape]
+            Pokemon shape model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if pokemon shape was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> pokemon_shape = client.pokemon.get_pokemon_shape(1)
+        >>> pokemon_shape.name
+        'ball'
+        """
+        route = Endpoint.get_pokemon_shape(name)
+        self._validate_resource(self.cache.pokemon_shape, name, route)
+        return self.cache.pokemon_shape.get(route, None)
+
+    async def fetch_pokemon_shape(self, name: t.Union[str, int]) -> t.Optional[PokemonShape]:
+        """
+        Fetches a pokemon shape model by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the
+
+        Returns
+        -------
+        t.Optional[PokemonShape]
+            Pokemon shape model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if pokemon shape was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...    pokemon_shape = await client.pokemon.fetch_pokemon_shape(1)
+        ...    print(pokemon_shape.name)
+        ...    await client.close()
+        >>> asyncio.run(main())
+        ball
+        """
+        route = Endpoint.get_pokemon_shape(name)
+        self._validate_resource(self.cache.pokemon_shape, name, route)
+        data = await self._client.request(route)
+        return self.cache.pokemon_shape.setdefault(route, PokemonShape.from_payload(data))
+
+    def get_pokemon_species(self, name: t.Union[str, int]) -> t.Optional[PokemonSpecies]:
+        """
+        Get pokemon species from cache.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the pokemon species.
+
+        Returns
+        -------
+        t.Optional[PokemonSpecies]
+            Pokemon species model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if pokemon species was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> pokemon_species = client.pokemon.get_pokemon_species(1)
+        >>> pokemon_species.name
+        'bulbasaur'
+        """
+        route = Endpoint.get_pokemon_species(name)
+        self._validate_resource(self.cache.pokemon_species, name, route)
+        return self.cache.pokemon_species.get(route, None)
+
+    async def fetch_pokemon_species(self, name: t.Union[str, int]) -> t.Optional[PokemonSpecies]:
+        """
+        Fetches a pokemon species model by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the
+
+        Returns
+        -------
+        t.Optional[PokemonSpecies]
+            Pokemon species model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if pokemon species was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...    pokemon_species = await client.pokemon.fetch_pokemon_species(1)
+        ...    print(pokemon_species.name)
+        ...    await client.close()
+        >>> asyncio.run(main())
+        bulbasaur
+        """
+        route = Endpoint.get_pokemon_species(name)
+        self._validate_resource(self.cache.pokemon_species, name, route)
+        data = await self._client.request(route)
+        return self.cache.pokemon_species.setdefault(route, PokemonSpecies.from_payload(data))
+
+    def get_stat(self, name: t.Union[str, int]) -> t.Optional[Stat]:
+        """
+        Get stat from cache.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the stat.
+
+        Returns
+        -------
+        t.Optional[Stat]
+            Stat model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if stat was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> stat = client.pokemon.get_stat(1)
+        >>> stat.name
+        'hp'
+        """
+        route = Endpoint.get_stat(name)
+        self._validate_resource(self.cache.stat, name, route)
+        return self.cache.stat.get(route, None)
+
+    async def fetch_stat(self, name: t.Union[str, int]) -> t.Optional[Stat]:
+        """
+        Fetches a stat model by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the
+
+        Returns
+        -------
+        t.Optional[Stat]
+            Stat model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if stat was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...    stat = await client.pokemon.fetch_stat(1)
+        ...    print(stat.name)
+        ...    await client.close()
+        >>> asyncio.run(main())
+        hp
+        """
+        route = Endpoint.get_stat(name)
+        self._validate_resource(self.cache.stat, name, route)
+        data = await self._client.request(route)
+        return self.cache.stat.setdefault(route, Stat.from_payload(data))
+
+    def get_type(self, name: t.Union[str, int]) -> t.Optional[Type]:
+        """
+        Get type from cache.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the type.
+
+        Returns
+        -------
+        t.Optional[Type]
+            Type model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if type was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> client = PokeLance()
+        >>> type_ = client.pokemon.get_type(1)
+        >>> type_.name
+        'normal'
+        """
+        route = Endpoint.get_type(name)
+        self._validate_resource(self.cache.type, name, route)
+        return self.cache.type.get(route, None)
+
+    async def fetch_type(self, name: t.Union[str, int]) -> t.Optional[Type]:
+        """
+        Fetches a type model by name or id.
+
+        Parameters
+        ----------
+        name: Union[str, int]
+            The name or id of the
+
+        Returns
+        -------
+        t.Optional[Type]
+            Type model if found, else None.
+
+        Raises
+        ------
+        pokelance.exceptions.ResourceNotFound
+            if type was not found.
+
+        Examples
+        --------
+
+        >>> from pokelance import PokeLance
+        >>> import asyncio
+        >>> client = PokeLance()
+        >>> async def main() -> None:
+        ...    type_ = await client.pokemon.fetch_type(1)
+        ...    print(type_.name)
+        ...    await client.close()
+        >>> asyncio.run(main())
+        normal
+        """
+        route = Endpoint.get_type(name)
+        self._validate_resource(self.cache.type, name, route)
+        data = await self._client.request(route)
+        return self.cache.type.setdefault(route, Type.from_payload(data))
+
+    @property
+    def all_pokemons(self) -> t.Optional[t.List[str]]:
+        """
+        Returns a list of all pokemon names.
+
+        Returns
+        -------
+        t.Optional[t.List[str]]
+            List of all pokemon names. None if not cached yet.
+        """
+        data = list(self.cache.pokemon.endpoints.keys())
+        return data if data else None
+
+
+def setup(lance: "PokeLance") -> None:
+    """Setup the pokemon cog."""
+    lance.add_extension("pokemon", Pokemon(lance.http))
```

### Comparing `pokelance-0.0.9a0/pokelance/http/__init__.py` & `pokelance-0.1.0/pokelance/http/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,171 +1,170 @@
-import asyncio
-import time
-import typing as t
-
-import aiohttp
-
-from pokelance.cache import Cache
-from pokelance.exceptions import HTTPException, ImageNotFound
-
-from .endpoints import Endpoint, Route
-
-if t.TYPE_CHECKING:
-    from pokelance import PokeLance
-
-
-__all__: t.Tuple[str, ...] = (
-    "HttpClient",
-    "Route",
-    "Endpoint",
-)
-
-
-@t.final
-class HttpClient:
-    """The HTTP client for PokeLance.
-
-    Parameters
-    ----------
-    client: pokelance.PokeLance
-        The client that this HTTP client is for.
-    cache_size: int
-        The size of the cache.
-    session: aiohttp.ClientSession
-        The session to use for the HTTP client.
-
-    Attributes
-    ----------
-    session: aiohttp.ClientSession
-        The session to use for the HTTP client.
-    _is_ready: bool
-        Whether the HTTP client is ready.
-    _cache: pokelance.cache.Cache
-        The cache to use for the HTTP client.
-    _client: pokelance.PokeLance
-        The client that this HTTP client is for.
-    """
-
-    __slots__: t.Tuple[str, ...] = (
-        "_client",
-        "session",
-        "_cache",
-        "_is_ready",
-    )
-
-    def __init__(
-        self, *, cache_size: int, client: "PokeLance", session: t.Optional[aiohttp.ClientSession] = None
-    ) -> None:
-        """Initializes the HTTP client.
-
-        Parameters
-        ----------
-        cache_size: int
-            The size of the cache.
-        client: pokelance.PokeLance
-            The client that this HTTP client is for.
-        session: aiohttp.ClientSession
-            The session to use for the HTTP client.
-
-        Returns
-        -------
-        pokelance.http.HttpClient
-            The HTTP client.
-        """
-        self._client = client
-        self.session = session
-        self._is_ready = False
-        self._cache = Cache(max_size=cache_size)
-
-    def _load_endpoints(self) -> None:
-        """Loads the endpoints for the HTTP client."""
-        for num, (coro, name) in enumerate(self._client.loaders):
-            task = asyncio.create_task(coro)
-            task.add_done_callback(
-                lambda _: self._client.logger.info(f"Loaded {self._client.loaders.pop(0)[1]} endpoints.")
-            )
-        self._is_ready = True
-
-    async def connect(self) -> None:
-        """Connects the HTTP client."""
-        if not self._is_ready:
-            if self.session is None:
-                self.session = aiohttp.ClientSession()
-                self._load_endpoints()
-
-    async def request(self, route: Route) -> t.Any:
-        """Makes a request to the PokeAPI.
-
-        Parameters
-        ----------
-        route: pokelance.http.Route
-            The route to use for the request.
-
-        Returns
-        -------
-        t.Any
-            The response from the PokeAPI.
-
-        Raises
-        ------
-        pokelance.exceptions.HTTPException
-            An error occurred while making the request.
-        """
-        if self.session is None:
-            await self.connect()
-        if not self._is_ready and self._client.loaders:
-            self._load_endpoints()
-        if self.session is not None:
-            async with self.session.request(route.method, route.url, params=route.payload) as response:
-                if 300 > response.status >= 200:
-                    return await response.json()
-                else:
-                    raise HTTPException(str(response.reason), route, response.status).create()
-        else:
-            raise HTTPException("No session was provided.", route, 0).create()
-
-    async def load_image(self, url: str) -> bytes:
-        """Loads an image from the url.
-
-        Parameters
-        ----------
-        url: str
-            The URL to load the image from.
-
-        Returns
-        -------
-        bytes
-            The image.
-        """
-        if self.session is None:
-            await self.connect()
-        if self.session is not None:
-            async with self.session.get(url) as response:
-                if 300 > response.status >= 200:
-                    data: bytes = await response.read()
-                    return data
-                else:
-                    raise ImageNotFound(str(response.reason), Route(), response.status).create()
-        return b""
-
-    async def ping(self) -> float:
-        """Pings the PokeAPI and returns the latency.
-
-        Returns
-        -------
-        float
-            The latency of the PokeAPI.
-        """
-        start = time.perf_counter()
-        await self.request(Route())
-        return time.perf_counter() - start
-
-    @property
-    def cache(self) -> Cache:
-        """The cache to use for the HTTP client.
-
-        Returns
-        -------
-        pokelance.cache.Cache
-            The cache.
-        """
-        return self._cache
+import asyncio
+import time
+import typing as t
+
+import aiohttp
+
+from pokelance.cache import Cache
+from pokelance.exceptions import HTTPException, ImageNotFound
+
+from .endpoints import Endpoint, Route
+
+if t.TYPE_CHECKING:
+    from pokelance import PokeLance
+
+
+__all__: t.Tuple[str, ...] = (
+    "HttpClient",
+    "Route",
+    "Endpoint",
+)
+
+
+@t.final
+class HttpClient:
+    """The HTTP client for PokeLance.
+
+    Parameters
+    ----------
+    client: pokelance.PokeLance
+        The client that this HTTP client is for.
+    cache_size: int
+        The size of the cache.
+    session: aiohttp.ClientSession
+        The session to use for the HTTP client.
+
+    Attributes
+    ----------
+    session: aiohttp.ClientSession
+        The session to use for the HTTP client.
+    _is_ready: bool
+        Whether the HTTP client is ready.
+    _cache: pokelance.cache.Cache
+        The cache to use for the HTTP client.
+    _client: pokelance.PokeLance
+        The client that this HTTP client is for.
+    """
+
+    __slots__: t.Tuple[str, ...] = (
+        "_client",
+        "session",
+        "_cache",
+        "_is_ready",
+    )
+
+    def __init__(
+        self, *, cache_size: int, client: "PokeLance", session: t.Optional[aiohttp.ClientSession] = None
+    ) -> None:
+        """Initializes the HTTP client.
+
+        Parameters
+        ----------
+        cache_size: int
+            The size of the cache.
+        client: pokelance.PokeLance
+            The client that this HTTP client is for.
+        session: aiohttp.ClientSession
+            The session to use for the HTTP client.
+
+        Returns
+        -------
+        pokelance.http.HttpClient
+            The HTTP client.
+        """
+        self._client = client
+        self.session = session
+        self._is_ready = False
+        self._cache = Cache(max_size=cache_size)
+
+    def _load_endpoints(self) -> None:
+        """Loads the endpoints for the HTTP client."""
+        for num, (coro, name) in enumerate(self._client.loaders):
+            task = asyncio.create_task(coro)
+            task.add_done_callback(
+                lambda _: self._client.logger.info(f"Loaded {self._client.loaders.pop(0)[1]} endpoints.")
+            )
+        self._is_ready = True
+
+    async def connect(self) -> None:
+        """Connects the HTTP client."""
+        if not self._is_ready and self.session is None:
+            self.session = aiohttp.ClientSession()
+            self._load_endpoints()
+
+    async def request(self, route: Route) -> t.Any:
+        """Makes a request to the PokeAPI.
+
+        Parameters
+        ----------
+        route: pokelance.http.Route
+            The route to use for the request.
+
+        Returns
+        -------
+        t.Any
+            The response from the PokeAPI.
+
+        Raises
+        ------
+        pokelance.exceptions.HTTPException
+            An error occurred while making the request.
+        """
+        if self.session is None:
+            await self.connect()
+        if not self._is_ready and self._client.loaders:
+            self._load_endpoints()
+        if self.session is not None:
+            async with self.session.request(route.method, route.url, params=route.payload) as response:
+                if 300 > response.status >= 200:
+                    return await response.json()
+                else:
+                    raise HTTPException(str(response.reason), route, response.status).create()
+        else:
+            raise HTTPException("No session was provided.", route, 0).create()
+
+    async def load_image(self, url: str) -> bytes:
+        """Loads an image from the url.
+
+        Parameters
+        ----------
+        url: str
+            The URL to load the image from.
+
+        Returns
+        -------
+        bytes
+            The image.
+        """
+        if self.session is None:
+            await self.connect()
+        if self.session is not None:
+            async with self.session.get(url) as response:
+                if 300 > response.status >= 200:
+                    data: bytes = await response.read()
+                    return data
+                else:
+                    raise ImageNotFound(str(response.reason), Route(), response.status).create()
+        return b""
+
+    async def ping(self) -> float:
+        """Pings the PokeAPI and returns the latency.
+
+        Returns
+        -------
+        float
+            The latency of the PokeAPI.
+        """
+        start = time.perf_counter()
+        await self.request(Route())
+        return time.perf_counter() - start
+
+    @property
+    def cache(self) -> Cache:
+        """The cache to use for the HTTP client.
+
+        Returns
+        -------
+        pokelance.cache.Cache
+            The cache.
+        """
+        return self._cache
```

### Comparing `pokelance-0.0.9a0/pokelance/http/endpoints.py` & `pokelance-0.1.0/pokelance/http/endpoints.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,531 +1,536 @@
-import typing as t
-
-import attrs
-
-__all__: t.Tuple[str, ...] = ("Endpoint", "Route")
-
-
-@attrs.define(repr=True, slots=True, kw_only=True, hash=True)
-class Route:
-    """Represents a route for an endpoint.
-
-    Attributes
-    ----------
-    endpoint: str
-        The endpoint name.
-    _url: str
-        The URL for the route.
-    _api_version: int
-        The API version for the route.
-    method: str
-        The HTTP method for the route.
-    payload: t.Optional[t.Dict[str, t.Any]]
-        The payload for the route.
-
-    Examples
-    --------
-    >>> pokemon = "pikachu"
-    >>> route = Route(endpoint=f"/pokemon/{pokemon}", method="GET")
-    """
-
-    endpoint: str = attrs.field(factory=str)
-    _url: str = "https://pokeapi.co/api/v2{endpoint}"
-    _api_version: int = 2
-    method: str = "GET"
-    payload: t.Optional[t.Dict[str, t.Any]] = None
-
-    def __str__(self) -> str:
-        return f"<Route endpoint={self.endpoint} method={self.method}>"
-
-    @property
-    def url(self) -> str:
-        return self._url.format(endpoint=self.endpoint)
-
-
-class Endpoint:
-    """Represents an endpoint for the API."""
-
-    @classmethod
-    def get_language_endpoints(cls) -> Route:
-        """Gets the language endpoints."""
-        return Route(endpoint="/language", payload={"limit": 10000})
-
-    @classmethod
-    def get_language(cls, language: t.Union[str, int]) -> Route:
-        """Gets a language."""
-        return Route(endpoint=f"/language/{language}")
-
-    @classmethod
-    def get_berry_endpoints(cls) -> Route:
-        """Get a list of berry endpoints."""
-        return Route(endpoint="/berry", payload={"limit": 10000})
-
-    @classmethod
-    def get_berry(cls, berry: t.Union[int, str]) -> Route:
-        """Get a berry by its ID or name."""
-        return Route(endpoint=f"/berry/{berry}")
-
-    @classmethod
-    def get_berry_firmness_endpoints(cls) -> Route:
-        """Get a list of berry firmness endpoints."""
-        return Route(endpoint="/berry-firmness", payload={"limit": 10000})
-
-    @classmethod
-    def get_berry_firmness(cls, berry_firmness: t.Union[int, str]) -> Route:
-        """Get a berry firmness by its ID or name."""
-        return Route(endpoint=f"/berry-firmness/{berry_firmness}")
-
-    @classmethod
-    def get_berry_flavor_endpoints(cls) -> Route:
-        """Get a list of berry flavor endpoints."""
-        return Route(endpoint="/berry-flavor", payload={"limit": 10000})
-
-    @classmethod
-    def get_berry_flavor(cls, berry_flavor: t.Union[int, str]) -> Route:
-        """Get a berry flavor by its ID or name."""
-        return Route(endpoint=f"/berry-flavor/{berry_flavor}")
-
-    @classmethod
-    def get_contest_type_endpoints(cls) -> Route:
-        """Get a list of contest type endpoints."""
-        return Route(endpoint="/contest-type", payload={"limit": 10000})
-
-    @classmethod
-    def get_contest_type(cls, contest_type: t.Union[int, str]) -> Route:
-        """Get a contest type by its ID or name."""
-        return Route(endpoint=f"/contest-type/{contest_type}")
-
-    @classmethod
-    def get_contest_effect_endpoints(cls) -> Route:
-        """Get a list of contest effect endpoints."""
-        return Route(endpoint="/contest-effect", payload={"limit": 10000})
-
-    @classmethod
-    def get_contest_effect(cls, contest_effect: int) -> Route:
-        """Get a contest effect by its ID."""
-        return Route(endpoint=f"/contest-effect/{contest_effect}")
-
-    @classmethod
-    def get_super_contest_effect_endpoints(cls) -> Route:
-        """Get a list of super contest effect endpoints."""
-        return Route(endpoint="/super-contest-effect", payload={"limit": 10000})
-
-    @classmethod
-    def get_super_contest_effect(cls, super_contest_effect: int) -> Route:
-        """Get a super contest effect by its ID."""
-        return Route(endpoint=f"/super-contest-effect/{super_contest_effect}")
-
-    @classmethod
-    def get_encounter_method_endpoints(cls) -> Route:
-        """Get a list of encounter method endpoints."""
-        return Route(endpoint="/encounter-method", payload={"limit": 10000})
-
-    @classmethod
-    def get_encounter_method(cls, encounter_method: t.Union[int, str]) -> Route:
-        """Get an encounter method by its ID or name."""
-        return Route(endpoint=f"/encounter-method/{encounter_method}")
-
-    @classmethod
-    def get_encounter_condition_endpoints(cls) -> Route:
-        """Get a list of encounter condition endpoints."""
-        return Route(endpoint="/encounter-condition", payload={"limit": 10000})
-
-    @classmethod
-    def get_encounter_condition(cls, encounter_condition: t.Union[int, str]) -> Route:
-        """Get an encounter condition by its ID or name."""
-        return Route(endpoint=f"/encounter-condition/{encounter_condition}")
-
-    @classmethod
-    def get_encounter_condition_value_endpoints(cls) -> Route:
-        """Get a list of encounter condition value endpoints."""
-        return Route(endpoint="/encounter-condition-value", payload={"limit": 10000})
-
-    @classmethod
-    def get_encounter_condition_value(cls, encounter_condition_value: t.Union[int, str]) -> Route:
-        """Get an encounter condition value by its ID or name."""
-        return Route(endpoint=f"/encounter-condition-value/{encounter_condition_value}")
-
-    @classmethod
-    def get_evolution_chain_endpoints(cls) -> Route:
-        """Get a list of evolution chain endpoints."""
-        return Route(endpoint="/evolution-chain", payload={"limit": 10000})
-
-    @classmethod
-    def get_evolution_chain(cls, evolution_chain: int) -> Route:
-        """Get an evolution chain by its ID."""
-        return Route(endpoint=f"/evolution-chain/{evolution_chain}")
-
-    @classmethod
-    def get_evolution_trigger_endpoints(cls) -> Route:
-        """Get a list of evolution trigger endpoints."""
-        return Route(endpoint="/evolution-trigger", payload={"limit": 10000})
-
-    @classmethod
-    def get_evolution_trigger(cls, evolution_trigger: t.Union[int, str]) -> Route:
-        """Get an evolution trigger by its ID or name."""
-        return Route(endpoint=f"/evolution-trigger/{evolution_trigger}")
-
-    @classmethod
-    def get_generation_endpoints(cls) -> Route:
-        """Get a list of generation endpoints."""
-        return Route(endpoint="/generation", payload={"limit": 10000})
-
-    @classmethod
-    def get_generation(cls, generation: t.Union[int, str]) -> Route:
-        """Get a generation by its ID or name."""
-        return Route(endpoint=f"/generation/{generation}")
-
-    @classmethod
-    def get_pokedex_endpoints(cls) -> Route:
-        """Get a list of pokedex endpoints."""
-        return Route(endpoint="/pokedex", payload={"limit": 10000})
-
-    @classmethod
-    def get_pokedex(cls, pokedex: t.Union[int, str]) -> Route:
-        """Get a pokedex by its ID or name."""
-        return Route(endpoint=f"/pokedex/{pokedex}")
-
-    @classmethod
-    def get_version_endpoints(cls) -> Route:
-        """Get a list of version endpoints."""
-        return Route(endpoint="/version", payload={"limit": 10000})
-
-    @classmethod
-    def get_version(cls, version: t.Union[int, str]) -> Route:
-        """Get a version by its ID or name."""
-        return Route(endpoint=f"/version/{version}")
-
-    @classmethod
-    def get_version_group_endpoints(cls) -> Route:
-        """Get a list of version group endpoints."""
-        return Route(endpoint="/version-group", payload={"limit": 10000})
-
-    @classmethod
-    def get_version_group(cls, version_group: t.Union[int, str]) -> Route:
-        """Get a version group by its ID or name."""
-        return Route(endpoint=f"/version-group/{version_group}")
-
-    @classmethod
-    def get_item_endpoints(cls) -> Route:
-        """Get a list of item endpoints."""
-        return Route(endpoint="/item", payload={"limit": 10000})
-
-    @classmethod
-    def get_item(cls, item: t.Union[int, str]) -> Route:
-        """Get an item by its ID or name."""
-        return Route(endpoint=f"/item/{item}")
-
-    @classmethod
-    def get_item_attribute_endpoints(cls) -> Route:
-        """Get a list of item attribute endpoints."""
-        return Route(endpoint="/item-attribute", payload={"limit": 10000})
-
-    @classmethod
-    def get_item_attribute(cls, item_attribute: t.Union[int, str]) -> Route:
-        """Get an item attribute by its ID or name."""
-        return Route(endpoint=f"/item-attribute/{item_attribute}")
-
-    @classmethod
-    def get_item_category_endpoints(cls) -> Route:
-        """Get a list of item category endpoints."""
-        return Route(endpoint="/item-category", payload={"limit": 10000})
-
-    @classmethod
-    def get_item_category(cls, item_category: t.Union[int, str]) -> Route:
-        """Get an item category by its ID or name."""
-        return Route(endpoint=f"/item-category/{item_category}")
-
-    @classmethod
-    def get_item_fling_effect_endpoints(cls) -> Route:
-        """Get a list of item fling effect endpoints."""
-        return Route(endpoint="/item-fling-effect", payload={"limit": 10000})
-
-    @classmethod
-    def get_item_fling_effect(cls, item_fling_effect: t.Union[int, str]) -> Route:
-        """Get an item fling effect by its ID or name."""
-        return Route(endpoint=f"/item-fling-effect/{item_fling_effect}")
-
-    @classmethod
-    def get_item_pocket_endpoints(cls) -> Route:
-        """Get a list of item pocket endpoints."""
-        return Route(endpoint="/item-pocket", payload={"limit": 10000})
-
-    @classmethod
-    def get_item_pocket(cls, item_pocket: t.Union[int, str]) -> Route:
-        """Get an item pocket by its ID or name."""
-        return Route(endpoint=f"/item-pocket/{item_pocket}")
-
-    @classmethod
-    def get_location_endpoints(cls) -> Route:
-        """Get a list of location endpoints."""
-        return Route(endpoint="/location", payload={"limit": 10000})
-
-    @classmethod
-    def get_location(cls, location: t.Union[int, str]) -> Route:
-        """Get a location by its ID or name."""
-        return Route(endpoint=f"/location/{location}")
-
-    @classmethod
-    def get_location_area_endpoints(cls) -> Route:
-        """Get a list of location area endpoints."""
-        return Route(endpoint="/location-area", payload={"limit": 10000})
-
-    @classmethod
-    def get_location_area(cls, location_area: t.Union[int, str]) -> Route:
-        """Get a location area by its ID or name."""
-        return Route(endpoint=f"/location-area/{location_area}")
-
-    @classmethod
-    def get_pal_park_area_endpoints(cls) -> Route:
-        """Get a list of pal park area endpoints."""
-        return Route(endpoint="/pal-park-area", payload={"limit": 10000})
-
-    @classmethod
-    def get_pal_park_area(cls, pal_park_area: t.Union[int, str]) -> Route:
-        """Get a pal park area by its ID or name."""
-        return Route(endpoint=f"/pal-park-area/{pal_park_area}")
-
-    @classmethod
-    def get_region_endpoints(cls) -> Route:
-        """Get a list of region endpoints."""
-        return Route(endpoint="/region", payload={"limit": 10000})
-
-    @classmethod
-    def get_region(cls, region: t.Union[int, str]) -> Route:
-        """Get a region by its ID or name."""
-        return Route(endpoint=f"/region/{region}")
-
-    @classmethod
-    def get_machine_endpoints(cls) -> Route:
-        """Get a list of machine endpoints."""
-        return Route(endpoint="/machine", payload={"limit": 10000})
-
-    @classmethod
-    def get_machine(cls, machine: int) -> Route:
-        """Get a machine by its ID."""
-        return Route(endpoint=f"/machine/{machine}")
-
-    @classmethod
-    def get_move_endpoints(cls) -> Route:
-        """Get a list of move endpoints."""
-        return Route(endpoint="/move", payload={"limit": 10000})
-
-    @classmethod
-    def get_move(cls, move: t.Union[int, str]) -> Route:
-        """Get a move by its ID or name."""
-        return Route(endpoint=f"/move/{move}")
-
-    @classmethod
-    def get_move_ailment_endpoints(cls) -> Route:
-        """Get a list of move ailment endpoints."""
-        return Route(endpoint="/move-ailment", payload={"limit": 10000})
-
-    @classmethod
-    def get_move_ailment(cls, move_ailment: t.Union[int, str]) -> Route:
-        """Get a move ailment by its ID or name."""
-        return Route(endpoint=f"/move-ailment/{move_ailment}")
-
-    @classmethod
-    def get_move_battle_style_endpoints(cls) -> Route:
-        """Get a list of move battle style endpoints."""
-        return Route(endpoint="/move-battle-style", payload={"limit": 10000})
-
-    @classmethod
-    def get_move_battle_style(cls, move_battle_style: t.Union[int, str]) -> Route:
-        """Get a move battle style by its ID or name."""
-        return Route(endpoint=f"/move-battle-style/{move_battle_style}")
-
-    @classmethod
-    def get_move_category_endpoints(cls) -> Route:
-        """Get a list of move category endpoints."""
-        return Route(endpoint="/move-category", payload={"limit": 10000})
-
-    @classmethod
-    def get_move_category(cls, move_category: t.Union[int, str]) -> Route:
-        """Get a move category by its ID or name."""
-        return Route(endpoint=f"/move-category/{move_category}")
-
-    @classmethod
-    def get_move_damage_class_endpoints(cls) -> Route:
-        """Get a list of move damage class endpoints."""
-        return Route(endpoint="/move-damage-class", payload={"limit": 10000})
-
-    @classmethod
-    def get_move_damage_class(cls, move_damage_class: t.Union[int, str]) -> Route:
-        """Get a move damage class by its ID or name."""
-        return Route(endpoint=f"/move-damage-class/{move_damage_class}")
-
-    @classmethod
-    def get_move_learn_method_endpoints(cls) -> Route:
-        """Get a list of move learn method endpoints."""
-        return Route(endpoint="/move-learn-method", payload={"limit": 10000})
-
-    @classmethod
-    def get_move_learn_method(cls, move_learn_method: t.Union[int, str]) -> Route:
-        """Get a move learn method by its ID or name."""
-        return Route(endpoint=f"/move-learn-method/{move_learn_method}")
-
-    @classmethod
-    def get_move_target_endpoints(cls) -> Route:
-        """Get a list of move target endpoints."""
-        return Route(endpoint="/move-target", payload={"limit": 10000})
-
-    @classmethod
-    def get_move_target(cls, move_target: t.Union[int, str]) -> Route:
-        """Get a move target by its ID or name."""
-        return Route(endpoint=f"/move-target/{move_target}")
-
-    @classmethod
-    def get_ability_endpoints(cls) -> Route:
-        """Get a list of ability endpoints."""
-        return Route(endpoint="/ability", payload={"limit": 10000})
-
-    @classmethod
-    def get_ability(cls, ability: t.Union[int, str]) -> Route:
-        """Get an ability by its ID or name."""
-        return Route(endpoint=f"/ability/{ability}")
-
-    @classmethod
-    def get_characteristic_endpoints(cls) -> Route:
-        """Get a list of characteristic endpoints."""
-        return Route(endpoint="/characteristic", payload={"limit": 10000})
-
-    @classmethod
-    def get_characteristic(cls, characteristic: int) -> Route:
-        """Get a characteristic by its ID."""
-        return Route(endpoint=f"/characteristic/{characteristic}")
-
-    @classmethod
-    def get_egg_group_endpoints(cls) -> Route:
-        """Get a list of egg group endpoints."""
-        return Route(endpoint="/egg-group", payload={"limit": 10000})
-
-    @classmethod
-    def get_egg_group(cls, egg_group: t.Union[int, str]) -> Route:
-        """Get an egg group by its ID or name."""
-        return Route(endpoint=f"/egg-group/{egg_group}")
-
-    @classmethod
-    def get_gender_endpoints(cls) -> Route:
-        """Get a list of gender endpoints."""
-        return Route(endpoint="/gender", payload={"limit": 10000})
-
-    @classmethod
-    def get_gender(cls, gender: t.Union[int, str]) -> Route:
-        """Get a gender by its ID or name."""
-        return Route(endpoint=f"/gender/{gender}")
-
-    @classmethod
-    def get_growth_rate_endpoints(cls) -> Route:
-        """Get a list of growth rate endpoints."""
-        return Route(endpoint="/growth-rate", payload={"limit": 10000})
-
-    @classmethod
-    def get_growth_rate(cls, growth_rate: t.Union[int, str]) -> Route:
-        """Get a growth rate by its ID or name."""
-        return Route(endpoint=f"/growth-rate/{growth_rate}")
-
-    @classmethod
-    def get_nature_endpoints(cls) -> Route:
-        """Get a list of nature endpoints."""
-        return Route(endpoint="/nature", payload={"limit": 10000})
-
-    @classmethod
-    def get_nature(cls, nature: t.Union[int, str]) -> Route:
-        """Get a nature by its ID or name."""
-        return Route(endpoint=f"/nature/{nature}")
-
-    @classmethod
-    def get_location_area_encounter(cls, name: t.Union[int, str]) -> Route:
-        """Get a location area encounter by its ID or name."""
-        return Route(endpoint=f"/pokemon/{name}/encounters")
-
-    @classmethod
-    def get_pokeathlon_stat_endpoints(cls) -> Route:
-        """Get a list of pokeathlon stat endpoints."""
-        return Route(endpoint="/pokeathlon-stat", payload={"limit": 10000})
-
-    @classmethod
-    def get_pokeathlon_stat(cls, pokeathlon_stat: t.Union[int, str]) -> Route:
-        """Get a pokeathlon stat by its ID or name."""
-        return Route(endpoint=f"/pokeathlon-stat/{pokeathlon_stat}")
-
-    @classmethod
-    def get_pokemon_endpoints(cls) -> Route:
-        """Get a list of pokemon endpoints."""
-        return Route(endpoint="/pokemon", payload={"limit": 10000})
-
-    @classmethod
-    def get_pokemon(cls, pokemon: t.Union[int, str]) -> Route:
-        """Get a pokemon by its ID or name."""
-        return Route(endpoint=f"/pokemon/{pokemon}")
-
-    @classmethod
-    def get_pokemon_color_endpoints(cls) -> Route:
-        """Get a list of pokemon color endpoints."""
-        return Route(endpoint="/pokemon-color", payload={"limit": 10000})
-
-    @classmethod
-    def get_pokemon_color(cls, pokemon_color: t.Union[int, str]) -> Route:
-        """Get a pokemon color by its ID or name."""
-        return Route(endpoint=f"/pokemon-color/{pokemon_color}")
-
-    @classmethod
-    def get_pokemon_form_endpoints(cls) -> Route:
-        """Get a list of pokemon form endpoints."""
-        return Route(endpoint="/pokemon-form", payload={"limit": 10000})
-
-    @classmethod
-    def get_pokemon_form(cls, pokemon_form: t.Union[int, str]) -> Route:
-        """Get a pokemon form by its ID or name."""
-        return Route(endpoint=f"/pokemon-form/{pokemon_form}")
-
-    @classmethod
-    def get_pokemon_habitat_endpoints(cls) -> Route:
-        """Get a list of pokemon habitat endpoints."""
-        return Route(endpoint="/pokemon-habitat", payload={"limit": 10000})
-
-    @classmethod
-    def get_pokemon_habitat(cls, pokemon_habitat: t.Union[int, str]) -> Route:
-        """Get a pokemon habitat by its ID or name."""
-        return Route(endpoint=f"/pokemon-habitat/{pokemon_habitat}")
-
-    @classmethod
-    def get_pokemon_shape_endpoints(cls) -> Route:
-        """Get a list of pokemon shape endpoints."""
-        return Route(endpoint="/pokemon-shape", payload={"limit": 10000})
-
-    @classmethod
-    def get_pokemon_shape(cls, pokemon_shape: t.Union[int, str]) -> Route:
-        """Get a pokemon shape by its ID or name."""
-        return Route(endpoint=f"/pokemon-shape/{pokemon_shape}")
-
-    @classmethod
-    def get_pokemon_species_endpoints(cls) -> Route:
-        """Get a list of pokemon species endpoints."""
-        return Route(endpoint="/pokemon-species", payload={"limit": 10000})
-
-    @classmethod
-    def get_pokemon_species(cls, pokemon_species: t.Union[int, str]) -> Route:
-        """Get a pokemon species by its ID or name."""
-        return Route(endpoint=f"/pokemon-species/{pokemon_species}")
-
-    @classmethod
-    def get_stat_endpoints(cls) -> Route:
-        """Get a list of stat endpoints."""
-        return Route(endpoint="/stat", payload={"limit": 10000})
-
-    @classmethod
-    def get_stat(cls, stat: t.Union[int, str]) -> Route:
-        """Get a stat by its ID or name."""
-        return Route(endpoint=f"/stat/{stat}")
-
-    @classmethod
-    def get_type_endpoints(cls) -> Route:
-        """Get a list of type endpoints."""
-        return Route(endpoint="/type", payload={"limit": 10000})
-
-    @classmethod
-    def get_type(cls, type_: t.Union[int, str]) -> Route:
-        """Get a type by its ID or name."""
-        return Route(endpoint=f"/type/{type_}")
+import typing as t
+
+import attrs
+
+__all__: t.Tuple[str, ...] = ("Endpoint", "Route")
+
+
+@attrs.define(repr=True, slots=True, kw_only=True, hash=True)
+class Route:
+    """Represents a route for an endpoint.
+
+    Attributes
+    ----------
+    endpoint: str
+        The endpoint name.
+    _url: str
+        The URL for the route.
+    _api_version: int
+        The API version for the route.
+    method: str
+        The HTTP method for the route.
+    payload: t.Optional[t.Dict[str, t.Any]]
+        The payload for the route.
+
+    Examples
+    --------
+    >>> pokemon = "pikachu"
+    >>> route = Route(endpoint=f"/pokemon/{pokemon}", method="GET")
+    """
+
+    endpoint: str = attrs.field(factory=str)
+    _url: str = "https://pokeapi.co/api/v2{endpoint}"
+    _api_version: int = 2
+    method: str = "GET"
+    payload: t.Optional[t.Dict[str, t.Any]] = None
+
+    def __str__(self) -> str:
+        return f"<Route endpoint={self.endpoint} method={self.method}>"
+
+    @property
+    def url(self) -> str:
+        return self._url.format(endpoint=self.endpoint)
+
+
+class Endpoint:
+    """Represents an endpoint for the API."""
+
+    @classmethod
+    def get_language_endpoints(cls) -> Route:
+        """Gets the language endpoints."""
+        return Route(endpoint="/language", payload={"limit": 10000})
+
+    @classmethod
+    def get_language(cls, language: t.Union[str, int]) -> Route:
+        """Gets a language."""
+        return Route(endpoint=f"/language/{language}")
+
+    @classmethod
+    def get_berry_endpoints(cls) -> Route:
+        """Get a list of berry endpoints."""
+        return Route(endpoint="/berry", payload={"limit": 10000})
+
+    @classmethod
+    def get_berry(cls, berry: t.Union[int, str]) -> Route:
+        """Get a berry by its ID or name."""
+        return Route(endpoint=f"/berry/{berry}")
+
+    @classmethod
+    def get_berry_firmness_endpoints(cls) -> Route:
+        """Get a list of berry firmness endpoints."""
+        return Route(endpoint="/berry-firmness", payload={"limit": 10000})
+
+    @classmethod
+    def get_berry_firmness(cls, berry_firmness: t.Union[int, str]) -> Route:
+        """Get a berry firmness by its ID or name."""
+        return Route(endpoint=f"/berry-firmness/{berry_firmness}")
+
+    @classmethod
+    def get_berry_flavor_endpoints(cls) -> Route:
+        """Get a list of berry flavor endpoints."""
+        return Route(endpoint="/berry-flavor", payload={"limit": 10000})
+
+    @classmethod
+    def get_berry_flavor(cls, berry_flavor: t.Union[int, str]) -> Route:
+        """Get a berry flavor by its ID or name."""
+        return Route(endpoint=f"/berry-flavor/{berry_flavor}")
+
+    @classmethod
+    def get_contest_type_endpoints(cls) -> Route:
+        """Get a list of contest type endpoints."""
+        return Route(endpoint="/contest-type", payload={"limit": 10000})
+
+    @classmethod
+    def get_contest_type(cls, contest_type: t.Union[int, str]) -> Route:
+        """Get a contest type by its ID or name."""
+        return Route(endpoint=f"/contest-type/{contest_type}")
+
+    @classmethod
+    def get_contest_effect_endpoints(cls) -> Route:
+        """Get a list of contest effect endpoints."""
+        return Route(endpoint="/contest-effect", payload={"limit": 10000})
+
+    @classmethod
+    def get_contest_effect(cls, contest_effect: int) -> Route:
+        """Get a contest effect by its ID."""
+        return Route(endpoint=f"/contest-effect/{contest_effect}")
+
+    @classmethod
+    def get_super_contest_effect_endpoints(cls) -> Route:
+        """Get a list of super contest effect endpoints."""
+        return Route(endpoint="/super-contest-effect", payload={"limit": 10000})
+
+    @classmethod
+    def get_super_contest_effect(cls, super_contest_effect: int) -> Route:
+        """Get a super contest effect by its ID."""
+        return Route(endpoint=f"/super-contest-effect/{super_contest_effect}")
+
+    @classmethod
+    def get_encounter_method_endpoints(cls) -> Route:
+        """Get a list of encounter method endpoints."""
+        return Route(endpoint="/encounter-method", payload={"limit": 10000})
+
+    @classmethod
+    def get_encounter_method(cls, encounter_method: t.Union[int, str]) -> Route:
+        """Get an encounter method by its ID or name."""
+        return Route(endpoint=f"/encounter-method/{encounter_method}")
+
+    @classmethod
+    def get_encounter_condition_endpoints(cls) -> Route:
+        """Get a list of encounter condition endpoints."""
+        return Route(endpoint="/encounter-condition", payload={"limit": 10000})
+
+    @classmethod
+    def get_encounter_condition(cls, encounter_condition: t.Union[int, str]) -> Route:
+        """Get an encounter condition by its ID or name."""
+        return Route(endpoint=f"/encounter-condition/{encounter_condition}")
+
+    @classmethod
+    def get_encounter_condition_value_endpoints(cls) -> Route:
+        """Get a list of encounter condition value endpoints."""
+        return Route(endpoint="/encounter-condition-value", payload={"limit": 10000})
+
+    @classmethod
+    def get_encounter_condition_value(cls, encounter_condition_value: t.Union[int, str]) -> Route:
+        """Get an encounter condition value by its ID or name."""
+        return Route(endpoint=f"/encounter-condition-value/{encounter_condition_value}")
+
+    @classmethod
+    def get_evolution_chain_endpoints(cls) -> Route:
+        """Get a list of evolution chain endpoints."""
+        return Route(endpoint="/evolution-chain", payload={"limit": 10000})
+
+    @classmethod
+    def get_evolution_chain(cls, evolution_chain: int) -> Route:
+        """Get an evolution chain by its ID."""
+        return Route(endpoint=f"/evolution-chain/{evolution_chain}")
+
+    @classmethod
+    def get_evolution_trigger_endpoints(cls) -> Route:
+        """Get a list of evolution trigger endpoints."""
+        return Route(endpoint="/evolution-trigger", payload={"limit": 10000})
+
+    @classmethod
+    def get_evolution_trigger(cls, evolution_trigger: t.Union[int, str]) -> Route:
+        """Get an evolution trigger by its ID or name."""
+        return Route(endpoint=f"/evolution-trigger/{evolution_trigger}")
+
+    @classmethod
+    def get_generation_endpoints(cls) -> Route:
+        """Get a list of generation endpoints."""
+        return Route(endpoint="/generation", payload={"limit": 10000})
+
+    @classmethod
+    def get_generation(cls, generation: t.Union[int, str]) -> Route:
+        """Get a generation by its ID or name."""
+        return Route(endpoint=f"/generation/{generation}")
+
+    @classmethod
+    def get_pokedex_endpoints(cls) -> Route:
+        """Get a list of pokedex endpoints."""
+        return Route(endpoint="/pokedex", payload={"limit": 10000})
+
+    @classmethod
+    def get_pokedex(cls, pokedex: t.Union[int, str]) -> Route:
+        """Get a pokedex by its ID or name."""
+        return Route(endpoint=f"/pokedex/{pokedex}")
+
+    @classmethod
+    def get_version_endpoints(cls) -> Route:
+        """Get a list of version endpoints."""
+        return Route(endpoint="/version", payload={"limit": 10000})
+
+    @classmethod
+    def get_version(cls, version: t.Union[int, str]) -> Route:
+        """Get a version by its ID or name."""
+        return Route(endpoint=f"/version/{version}")
+
+    @classmethod
+    def get_version_group_endpoints(cls) -> Route:
+        """Get a list of version group endpoints."""
+        return Route(endpoint="/version-group", payload={"limit": 10000})
+
+    @classmethod
+    def get_version_group(cls, version_group: t.Union[int, str]) -> Route:
+        """Get a version group by its ID or name."""
+        return Route(endpoint=f"/version-group/{version_group}")
+
+    @classmethod
+    def get_item_endpoints(cls) -> Route:
+        """Get a list of item endpoints."""
+        return Route(endpoint="/item", payload={"limit": 10000})
+
+    @classmethod
+    def get_item(cls, item: t.Union[int, str]) -> Route:
+        """Get an item by its ID or name."""
+        return Route(endpoint=f"/item/{item}")
+
+    @classmethod
+    def get_item_attribute_endpoints(cls) -> Route:
+        """Get a list of item attribute endpoints."""
+        return Route(endpoint="/item-attribute", payload={"limit": 10000})
+
+    @classmethod
+    def get_item_attribute(cls, item_attribute: t.Union[int, str]) -> Route:
+        """Get an item attribute by its ID or name."""
+        return Route(endpoint=f"/item-attribute/{item_attribute}")
+
+    @classmethod
+    def get_item_category_endpoints(cls) -> Route:
+        """Get a list of item category endpoints."""
+        return Route(endpoint="/item-category", payload={"limit": 10000})
+
+    @classmethod
+    def get_item_category(cls, item_category: t.Union[int, str]) -> Route:
+        """Get an item category by its ID or name."""
+        return Route(endpoint=f"/item-category/{item_category}")
+
+    @classmethod
+    def get_item_fling_effect_endpoints(cls) -> Route:
+        """Get a list of item fling effect endpoints."""
+        return Route(endpoint="/item-fling-effect", payload={"limit": 10000})
+
+    @classmethod
+    def get_item_fling_effect(cls, item_fling_effect: t.Union[int, str]) -> Route:
+        """Get an item fling effect by its ID or name."""
+        return Route(endpoint=f"/item-fling-effect/{item_fling_effect}")
+
+    @classmethod
+    def get_item_pocket_endpoints(cls) -> Route:
+        """Get a list of item pocket endpoints."""
+        return Route(endpoint="/item-pocket", payload={"limit": 10000})
+
+    @classmethod
+    def get_item_pocket(cls, item_pocket: t.Union[int, str]) -> Route:
+        """Get an item pocket by its ID or name."""
+        return Route(endpoint=f"/item-pocket/{item_pocket}")
+
+    @classmethod
+    def get_location_endpoints(cls) -> Route:
+        """Get a list of location endpoints."""
+        return Route(endpoint="/location", payload={"limit": 10000})
+
+    @classmethod
+    def get_location(cls, location: t.Union[int, str]) -> Route:
+        """Get a location by its ID or name."""
+        return Route(endpoint=f"/location/{location}")
+
+    @classmethod
+    def get_location_area_endpoints(cls) -> Route:
+        """Get a list of location area endpoints."""
+        return Route(endpoint="/location-area", payload={"limit": 10000})
+
+    @classmethod
+    def get_location_area(cls, location_area: t.Union[int, str]) -> Route:
+        """Get a location area by its ID or name."""
+        return Route(endpoint=f"/location-area/{location_area}")
+
+    @classmethod
+    def get_pal_park_area_endpoints(cls) -> Route:
+        """Get a list of pal park area endpoints."""
+        return Route(endpoint="/pal-park-area", payload={"limit": 10000})
+
+    @classmethod
+    def get_pal_park_area(cls, pal_park_area: t.Union[int, str]) -> Route:
+        """Get a pal park area by its ID or name."""
+        return Route(endpoint=f"/pal-park-area/{pal_park_area}")
+
+    @classmethod
+    def get_region_endpoints(cls) -> Route:
+        """Get a list of region endpoints."""
+        return Route(endpoint="/region", payload={"limit": 10000})
+
+    @classmethod
+    def get_region(cls, region: t.Union[int, str]) -> Route:
+        """Get a region by its ID or name."""
+        return Route(endpoint=f"/region/{region}")
+
+    @classmethod
+    def get_machine_endpoints(cls) -> Route:
+        """Get a list of machine endpoints."""
+        return Route(endpoint="/machine", payload={"limit": 10000})
+
+    @classmethod
+    def get_machine(cls, machine: int) -> Route:
+        """Get a machine by its ID."""
+        return Route(endpoint=f"/machine/{machine}")
+
+    @classmethod
+    def get_move_endpoints(cls) -> Route:
+        """Get a list of move endpoints."""
+        return Route(endpoint="/move", payload={"limit": 10000})
+
+    @classmethod
+    def get_move(cls, move: t.Union[int, str]) -> Route:
+        """Get a move by its ID or name."""
+        return Route(endpoint=f"/move/{move}")
+
+    @classmethod
+    def get_move_ailment_endpoints(cls) -> Route:
+        """Get a list of move ailment endpoints."""
+        return Route(endpoint="/move-ailment", payload={"limit": 10000})
+
+    @classmethod
+    def get_move_ailment(cls, move_ailment: t.Union[int, str]) -> Route:
+        """Get a move ailment by its ID or name."""
+        return Route(endpoint=f"/move-ailment/{move_ailment}")
+
+    @classmethod
+    def get_move_battle_style_endpoints(cls) -> Route:
+        """Get a list of move battle style endpoints."""
+        return Route(endpoint="/move-battle-style", payload={"limit": 10000})
+
+    @classmethod
+    def get_move_battle_style(cls, move_battle_style: t.Union[int, str]) -> Route:
+        """Get a move battle style by its ID or name."""
+        return Route(endpoint=f"/move-battle-style/{move_battle_style}")
+
+    @classmethod
+    def get_move_category_endpoints(cls) -> Route:
+        """Get a list of move category endpoints."""
+        return Route(endpoint="/move-category", payload={"limit": 10000})
+
+    @classmethod
+    def get_move_category(cls, move_category: t.Union[int, str]) -> Route:
+        """Get a move category by its ID or name."""
+        return Route(endpoint=f"/move-category/{move_category}")
+
+    @classmethod
+    def get_move_damage_class_endpoints(cls) -> Route:
+        """Get a list of move damage class endpoints."""
+        return Route(endpoint="/move-damage-class", payload={"limit": 10000})
+
+    @classmethod
+    def get_move_damage_class(cls, move_damage_class: t.Union[int, str]) -> Route:
+        """Get a move damage class by its ID or name."""
+        return Route(endpoint=f"/move-damage-class/{move_damage_class}")
+
+    @classmethod
+    def get_move_learn_method_endpoints(cls) -> Route:
+        """Get a list of move learn method endpoints."""
+        return Route(endpoint="/move-learn-method", payload={"limit": 10000})
+
+    @classmethod
+    def get_move_learn_method(cls, move_learn_method: t.Union[int, str]) -> Route:
+        """Get a move learn method by its ID or name."""
+        return Route(endpoint=f"/move-learn-method/{move_learn_method}")
+
+    @classmethod
+    def get_move_target_endpoints(cls) -> Route:
+        """Get a list of move target endpoints."""
+        return Route(endpoint="/move-target", payload={"limit": 10000})
+
+    @classmethod
+    def get_move_target(cls, move_target: t.Union[int, str]) -> Route:
+        """Get a move target by its ID or name."""
+        return Route(endpoint=f"/move-target/{move_target}")
+
+    @classmethod
+    def get_ability_endpoints(cls) -> Route:
+        """Get a list of ability endpoints."""
+        return Route(endpoint="/ability", payload={"limit": 10000})
+
+    @classmethod
+    def get_ability(cls, ability: t.Union[int, str]) -> Route:
+        """Get an ability by its ID or name."""
+        return Route(endpoint=f"/ability/{ability}")
+
+    @classmethod
+    def get_characteristic_endpoints(cls) -> Route:
+        """Get a list of characteristic endpoints."""
+        return Route(endpoint="/characteristic", payload={"limit": 10000})
+
+    @classmethod
+    def get_characteristic(cls, characteristic: int) -> Route:
+        """Get a characteristic by its ID."""
+        return Route(endpoint=f"/characteristic/{characteristic}")
+
+    @classmethod
+    def get_egg_group_endpoints(cls) -> Route:
+        """Get a list of egg group endpoints."""
+        return Route(endpoint="/egg-group", payload={"limit": 10000})
+
+    @classmethod
+    def get_egg_group(cls, egg_group: t.Union[int, str]) -> Route:
+        """Get an egg group by its ID or name."""
+        return Route(endpoint=f"/egg-group/{egg_group}")
+
+    @classmethod
+    def get_gender_endpoints(cls) -> Route:
+        """Get a list of gender endpoints."""
+        return Route(endpoint="/gender", payload={"limit": 10000})
+
+    @classmethod
+    def get_gender(cls, gender: t.Union[int, str]) -> Route:
+        """Get a gender by its ID or name."""
+        return Route(endpoint=f"/gender/{gender}")
+
+    @classmethod
+    def get_growth_rate_endpoints(cls) -> Route:
+        """Get a list of growth rate endpoints."""
+        return Route(endpoint="/growth-rate", payload={"limit": 10000})
+
+    @classmethod
+    def get_growth_rate(cls, growth_rate: t.Union[int, str]) -> Route:
+        """Get a growth rate by its ID or name."""
+        return Route(endpoint=f"/growth-rate/{growth_rate}")
+
+    @classmethod
+    def get_nature_endpoints(cls) -> Route:
+        """Get a list of nature endpoints."""
+        return Route(endpoint="/nature", payload={"limit": 10000})
+
+    @classmethod
+    def get_nature(cls, nature: t.Union[int, str]) -> Route:
+        """Get a nature by its ID or name."""
+        return Route(endpoint=f"/nature/{nature}")
+
+    @classmethod
+    def get_location_area_encounter_endpoints(cls) -> Route:
+        """Get a list of location area encounter endpoints."""
+        return Route(endpoint="/pokemon", payload={"limit": 10000})
+
+    @classmethod
+    def get_location_area_encounter(cls, name: t.Union[int, str]) -> Route:
+        """Get a location area encounter by its ID or name."""
+        return Route(endpoint=f"/pokemon/{name}/encounters")
+
+    @classmethod
+    def get_pokeathlon_stat_endpoints(cls) -> Route:
+        """Get a list of pokeathlon stat endpoints."""
+        return Route(endpoint="/pokeathlon-stat", payload={"limit": 10000})
+
+    @classmethod
+    def get_pokeathlon_stat(cls, pokeathlon_stat: t.Union[int, str]) -> Route:
+        """Get a pokeathlon stat by its ID or name."""
+        return Route(endpoint=f"/pokeathlon-stat/{pokeathlon_stat}")
+
+    @classmethod
+    def get_pokemon_endpoints(cls) -> Route:
+        """Get a list of pokemon endpoints."""
+        return Route(endpoint="/pokemon", payload={"limit": 10000})
+
+    @classmethod
+    def get_pokemon(cls, pokemon: t.Union[int, str]) -> Route:
+        """Get a pokemon by its ID or name."""
+        return Route(endpoint=f"/pokemon/{pokemon}")
+
+    @classmethod
+    def get_pokemon_color_endpoints(cls) -> Route:
+        """Get a list of pokemon color endpoints."""
+        return Route(endpoint="/pokemon-color", payload={"limit": 10000})
+
+    @classmethod
+    def get_pokemon_color(cls, pokemon_color: t.Union[int, str]) -> Route:
+        """Get a pokemon color by its ID or name."""
+        return Route(endpoint=f"/pokemon-color/{pokemon_color}")
+
+    @classmethod
+    def get_pokemon_form_endpoints(cls) -> Route:
+        """Get a list of pokemon form endpoints."""
+        return Route(endpoint="/pokemon-form", payload={"limit": 10000})
+
+    @classmethod
+    def get_pokemon_form(cls, pokemon_form: t.Union[int, str]) -> Route:
+        """Get a pokemon form by its ID or name."""
+        return Route(endpoint=f"/pokemon-form/{pokemon_form}")
+
+    @classmethod
+    def get_pokemon_habitat_endpoints(cls) -> Route:
+        """Get a list of pokemon habitat endpoints."""
+        return Route(endpoint="/pokemon-habitat", payload={"limit": 10000})
+
+    @classmethod
+    def get_pokemon_habitat(cls, pokemon_habitat: t.Union[int, str]) -> Route:
+        """Get a pokemon habitat by its ID or name."""
+        return Route(endpoint=f"/pokemon-habitat/{pokemon_habitat}")
+
+    @classmethod
+    def get_pokemon_shape_endpoints(cls) -> Route:
+        """Get a list of pokemon shape endpoints."""
+        return Route(endpoint="/pokemon-shape", payload={"limit": 10000})
+
+    @classmethod
+    def get_pokemon_shape(cls, pokemon_shape: t.Union[int, str]) -> Route:
+        """Get a pokemon shape by its ID or name."""
+        return Route(endpoint=f"/pokemon-shape/{pokemon_shape}")
+
+    @classmethod
+    def get_pokemon_species_endpoints(cls) -> Route:
+        """Get a list of pokemon species endpoints."""
+        return Route(endpoint="/pokemon-species", payload={"limit": 10000})
+
+    @classmethod
+    def get_pokemon_species(cls, pokemon_species: t.Union[int, str]) -> Route:
+        """Get a pokemon species by its ID or name."""
+        return Route(endpoint=f"/pokemon-species/{pokemon_species}")
+
+    @classmethod
+    def get_stat_endpoints(cls) -> Route:
+        """Get a list of stat endpoints."""
+        return Route(endpoint="/stat", payload={"limit": 10000})
+
+    @classmethod
+    def get_stat(cls, stat: t.Union[int, str]) -> Route:
+        """Get a stat by its ID or name."""
+        return Route(endpoint=f"/stat/{stat}")
+
+    @classmethod
+    def get_type_endpoints(cls) -> Route:
+        """Get a list of type endpoints."""
+        return Route(endpoint="/type", payload={"limit": 10000})
+
+    @classmethod
+    def get_type(cls, type_: t.Union[int, str]) -> Route:
+        """Get a type by its ID or name."""
+        return Route(endpoint=f"/type/{type_}")
```

### Comparing `pokelance-0.0.9a0/pokelance/languages.py` & `pokelance-0.1.0/pokelance/languages.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-import enum
-import typing as t
-
-from pokelance.http import Endpoint
-from pokelance.models import Language
-
-__all__: t.Tuple[str, ...] = ("Languages",)
-LANGUAGE = Endpoint.get_language_endpoints().url
-
-
-class Languages(enum.Enum):
-    JAPANESE = Language.from_payload(
-        {
-            "id": 1,
-            "iso3166": "jp",
-            "iso639": "ja",
-            "name": "ja-Hrkt",
-            "names": [
-                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "日本語"},
-                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "일본어"},
-                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Japonais"},
-                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Japanisch"},
-                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Japonés"},
-                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "Japanese"},
-            ],
-            "official": True,
-        }
-    )
-    ROOMAJI = Language.from_payload(
-        {
-            "id": 2,
-            "iso3166": "jp",
-            "iso639": "ja",
-            "name": "roomaji",
-            "names": [
-                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "正式ローマジ"},
-                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "정식 로마자"},
-                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Romaji"},
-                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Rōmaji"},
-                {
-                    "language": {"name": "en", "url": f"{LANGUAGE}/9/"},
-                    "name": "Official roomaji",
-                },
-            ],
-            "official": True,
-        }
-    )
-    KOREAN = Language.from_payload(
-        {
-            "id": 3,
-            "iso3166": "kr",
-            "iso639": "ko",
-            "name": "ko",
-            "names": [
-                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "韓国語"},
-                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "한국어"},
-                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Coréen"},
-                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Koreanisch"},
-                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Coreano"},
-                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "Korean"},
-            ],
-            "official": True,
-        }
-    )
-    CHINESE = Language.from_payload(
-        {
-            "id": 4,
-            "iso3166": "cn",
-            "iso639": "zh",
-            "name": "zh-Hant",
-            "names": [
-                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "中国語"},
-                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "중국어"},
-                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Chinois"},
-                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Chinesisch"},
-                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Chino"},
-                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "Chinese"},
-            ],
-            "official": True,
-        }
-    )
-    FRENCH = Language.from_payload(
-        {
-            "id": 5,
-            "iso3166": "fr",
-            "iso639": "fr",
-            "name": "fr",
-            "names": [
-                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "フランス語"},
-                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "프랑스어"},
-                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Français"},
-                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Französisch"},
-                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Francés"},
-                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "French"},
-            ],
-            "official": True,
-        }
-    )
-    GERMAN = Language.from_payload(
-        {
-            "id": 6,
-            "iso3166": "de",
-            "iso639": "de",
-            "name": "de",
-            "names": [
-                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "ドイツ語"},
-                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "도이치어"},
-                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Allemand"},
-                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Deutsch"},
-                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Alemán"},
-                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "German"},
-            ],
-            "official": True,
-        }
-    )
-    SPANISH = Language.from_payload(
-        {
-            "id": 7,
-            "iso3166": "es",
-            "iso639": "es",
-            "name": "es",
-            "names": [
-                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "西語"},
-                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "스페인어"},
-                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Espagnol"},
-                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Spanisch"},
-                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Español"},
-                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "Spanish"},
-            ],
-            "official": True,
-        }
-    )
-    ITALIAN = Language.from_payload(
-        {
-            "id": 8,
-            "iso3166": "it",
-            "iso639": "it",
-            "name": "it",
-            "names": [
-                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "伊語"},
-                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "이탈리아어"},
-                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Italien"},
-                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Italienisch"},
-                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Italiano"},
-                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "Italian"},
-            ],
-            "official": True,
-        }
-    )
-    ENGLISH = Language.from_payload(
-        {
-            "id": 9,
-            "iso3166": "us",
-            "iso639": "en",
-            "name": "en",
-            "names": [
-                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "英語"},
-                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "영어"},
-                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Anglais"},
-                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Englisch"},
-                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Inglés"},
-                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "English"},
-            ],
-            "official": True,
-        }
-    )
-    CZECH = Language.from_payload(
-        {
-            "id": 10,
-            "iso3166": "cz",
-            "iso639": "cs",
-            "name": "cs",
-            "names": [
-                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "チェコ語"},
-                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "체코어"},
-                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Tchèque"},
-                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Tschechisch"},
-                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Checo"},
-                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "Czech"},
-            ],
-            "official": False,
-        }
-    )
-    JA = Language.from_payload({"id": 11, "iso3166": "jp", "iso639": "ja", "name": "ja", "names": [], "official": True})
-    CHINESE_SIMPLIFIED = Language.from_payload(
-        {"id": 12, "iso3166": "cn", "iso639": "zh", "name": "zh-Hans", "names": [], "official": True}
-    )
-    PORTUGAL_BRAZILIAN = Language.from_payload(
-        {"id": 13, "iso3166": "br", "iso639": "pt-BR", "name": "pt-BR", "names": [], "official": False}
-    )
-
-    def __str__(self) -> str:
-        return str(self.value.name)
-
-    def __int__(self) -> int:
-        return int(self.value.id)
+import enum
+import typing as t
+
+from pokelance.http import Endpoint
+from pokelance.models import Language
+
+__all__: t.Tuple[str, ...] = ("Languages",)
+LANGUAGE = Endpoint.get_language_endpoints().url
+
+
+class Languages(enum.Enum):
+    JAPANESE = Language.from_payload(
+        {
+            "id": 1,
+            "iso3166": "jp",
+            "iso639": "ja",
+            "name": "ja-Hrkt",
+            "names": [
+                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "日本語"},
+                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "일본어"},
+                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Japonais"},
+                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Japanisch"},
+                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Japonés"},
+                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "Japanese"},
+            ],
+            "official": True,
+        }
+    )
+    ROOMAJI = Language.from_payload(
+        {
+            "id": 2,
+            "iso3166": "jp",
+            "iso639": "ja",
+            "name": "roomaji",
+            "names": [
+                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "正式ローマジ"},
+                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "정식 로마자"},
+                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Romaji"},
+                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Rōmaji"},
+                {
+                    "language": {"name": "en", "url": f"{LANGUAGE}/9/"},
+                    "name": "Official roomaji",
+                },
+            ],
+            "official": True,
+        }
+    )
+    KOREAN = Language.from_payload(
+        {
+            "id": 3,
+            "iso3166": "kr",
+            "iso639": "ko",
+            "name": "ko",
+            "names": [
+                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "韓国語"},
+                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "한국어"},
+                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Coréen"},
+                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Koreanisch"},
+                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Coreano"},
+                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "Korean"},
+            ],
+            "official": True,
+        }
+    )
+    CHINESE = Language.from_payload(
+        {
+            "id": 4,
+            "iso3166": "cn",
+            "iso639": "zh",
+            "name": "zh-Hant",
+            "names": [
+                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "中国語"},
+                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "중국어"},
+                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Chinois"},
+                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Chinesisch"},
+                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Chino"},
+                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "Chinese"},
+            ],
+            "official": True,
+        }
+    )
+    FRENCH = Language.from_payload(
+        {
+            "id": 5,
+            "iso3166": "fr",
+            "iso639": "fr",
+            "name": "fr",
+            "names": [
+                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "フランス語"},
+                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "프랑스어"},
+                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Français"},
+                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Französisch"},
+                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Francés"},
+                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "French"},
+            ],
+            "official": True,
+        }
+    )
+    GERMAN = Language.from_payload(
+        {
+            "id": 6,
+            "iso3166": "de",
+            "iso639": "de",
+            "name": "de",
+            "names": [
+                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "ドイツ語"},
+                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "도이치어"},
+                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Allemand"},
+                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Deutsch"},
+                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Alemán"},
+                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "German"},
+            ],
+            "official": True,
+        }
+    )
+    SPANISH = Language.from_payload(
+        {
+            "id": 7,
+            "iso3166": "es",
+            "iso639": "es",
+            "name": "es",
+            "names": [
+                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "西語"},
+                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "스페인어"},
+                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Espagnol"},
+                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Spanisch"},
+                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Español"},
+                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "Spanish"},
+            ],
+            "official": True,
+        }
+    )
+    ITALIAN = Language.from_payload(
+        {
+            "id": 8,
+            "iso3166": "it",
+            "iso639": "it",
+            "name": "it",
+            "names": [
+                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "伊語"},
+                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "이탈리아어"},
+                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Italien"},
+                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Italienisch"},
+                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Italiano"},
+                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "Italian"},
+            ],
+            "official": True,
+        }
+    )
+    ENGLISH = Language.from_payload(
+        {
+            "id": 9,
+            "iso3166": "us",
+            "iso639": "en",
+            "name": "en",
+            "names": [
+                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "英語"},
+                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "영어"},
+                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Anglais"},
+                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Englisch"},
+                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Inglés"},
+                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "English"},
+            ],
+            "official": True,
+        }
+    )
+    CZECH = Language.from_payload(
+        {
+            "id": 10,
+            "iso3166": "cz",
+            "iso639": "cs",
+            "name": "cs",
+            "names": [
+                {"language": {"name": "ja-Hrkt", "url": f"{LANGUAGE}/1/"}, "name": "チェコ語"},
+                {"language": {"name": "ko", "url": f"{LANGUAGE}/3/"}, "name": "체코어"},
+                {"language": {"name": "fr", "url": f"{LANGUAGE}/5/"}, "name": "Tchèque"},
+                {"language": {"name": "de", "url": f"{LANGUAGE}/6/"}, "name": "Tschechisch"},
+                {"language": {"name": "es", "url": f"{LANGUAGE}/7/"}, "name": "Checo"},
+                {"language": {"name": "en", "url": f"{LANGUAGE}/9/"}, "name": "Czech"},
+            ],
+            "official": False,
+        }
+    )
+    JA = Language.from_payload({"id": 11, "iso3166": "jp", "iso639": "ja", "name": "ja", "names": [], "official": True})
+    CHINESE_SIMPLIFIED = Language.from_payload(
+        {"id": 12, "iso3166": "cn", "iso639": "zh", "name": "zh-Hans", "names": [], "official": True}
+    )
+    PORTUGAL_BRAZILIAN = Language.from_payload(
+        {"id": 13, "iso3166": "br", "iso639": "pt-BR", "name": "pt-BR", "names": [], "official": False}
+    )
+
+    def __str__(self) -> str:
+        return str(self.value.name)
+
+    def __int__(self) -> int:
+        return int(self.value.id)
```

### Comparing `pokelance-0.0.9a0/pokelance/logger.py` & `pokelance-0.1.0/pokelance/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,123 @@
-import datetime
-import enum
-import logging
-import pathlib
-import typing as t
-
-__all__: t.Tuple[str, ...] = (
-    "Logger",
-    "FileHandler",
-    "Formatter",
-)
-FLAIR: int = 95
-
-
-class LogLevelColors(enum.Enum):
-    """Colors for the log levels."""
-
-    DEBUG = "\033[96m"
-    INFO = "\033[92m"
-    WARNING = "\033[93m"
-    ERROR = "\033[33m"
-    CRITICAL = "\033[91m"
-    ENDC = "\033[0m"
-    FLAIR = "\033[95m"
-
-
-class Formatter(logging.Formatter):
-    """Format the log record."""
-
-    def __init__(self) -> None:
-        super().__init__(
-            "[%(asctime)s] | %(pathname)s:%(lineno)d | %(levelname)s | %(message)s",
-            style="%",
-        )
-
-    def format(self, record: logging.LogRecord) -> str:
-        """Format the log record."""
-        return f"{LogLevelColors[record.levelname].value}{super().format(record)}{LogLevelColors.ENDC.value}"
-
-
-class FileHandler(logging.FileHandler):
-    """Emit a log record.
-
-    Parameters
-    ----------
-    ext : str
-        The file extension.
-    folder : pathlib.Path | str
-        The folder to save the logs in. Defaults to "logs".
-    """
-
-    _last_entry: datetime.datetime = datetime.datetime.today()
-
-    def __init__(self, *, ext: str, folder: t.Union[pathlib.Path, str] = "logs") -> None:
-        """Create a new file handler."""
-        self.folder = pathlib.Path(folder)
-        self.ext = ext
-        self.folder.mkdir(exist_ok=True)
-        super().__init__(
-            self.folder / f"{datetime.datetime.today().strftime('%Y-%m-%d')}-{ext}.log",
-            encoding="utf-8",
-        )
-        self.setFormatter(Formatter())
-
-    def emit(self, record: logging.LogRecord) -> None:
-        """Emit a log record."""
-        if self._last_entry.date() != datetime.datetime.today().date():
-            self._last_entry = datetime.datetime.today()
-            self.close()
-            self.baseFilename = (self.folder / f"{self._last_entry.strftime('%Y-%m-%d')}-{self.ext}.log").as_posix()
-            self.stream = self._open()
-        super().emit(record)
-
-
-class Logger(logging.Logger):
-    """The logger used to log information about the client.
-
-    Parameters
-    ----------
-    name : str
-        The name of the logger.
-    level : int
-        The level of the logger.
-    file_logging : bool
-        Whether or not to log to a file.
-
-    Attributes
-    ----------
-    _handler : logging.StreamHandler
-        The stream handler used to log to the console.
-    _file_handler : t.Optional[logging.FileHandler]
-        The file handler used to log to a file.
-
-    Examples
-    --------
-
-    >>> logs = Logger(name="pokelance")
-    >>> logs.info("Hello, world!")
-    [2021-08-29 17:05:32,000] | pokelance\logger.py:95 | INFO | Hello, world!
-
-    """
-
-    file_handler: t.Optional[FileHandler] = None
-
-    def __init__(self, *, name: str, level: int = logging.INFO, file_logging: bool = False) -> None:
-        super().__init__(name, level)
-        self._handler = logging.StreamHandler()
-        self._handler.setFormatter(Formatter())
-        self.addHandler(self._handler)
-        if file_logging:
-            self._file_handler = FileHandler(ext=name)
-            self.addHandler(self._file_handler)
-        logging.addLevelName(FLAIR, "FLAIR")
-
-    def set_formatter(self, formatter: logging.Formatter) -> None:
-        """Set the formatter."""
-        self._handler.setFormatter(formatter)
-        self._file_handler.setFormatter(formatter)
-
-    def flair(self, message: str, *args: t.Any, **kwargs: t.Any) -> None:
-        """Record a flair log."""
-        self.log(FLAIR, message, *args, **kwargs)
+import datetime
+import enum
+import logging
+import pathlib
+import typing as t
+
+__all__: t.Tuple[str, ...] = (
+    "Logger",
+    "FileHandler",
+    "Formatter",
+)
+FLAIR: int = 95
+
+
+class LogLevelColors(enum.Enum):
+    """Colors for the log levels."""
+
+    DEBUG = "\033[96m"
+    INFO = "\033[92m"
+    WARNING = "\033[93m"
+    ERROR = "\033[33m"
+    CRITICAL = "\033[91m"
+    ENDC = "\033[0m"
+    FLAIR = "\033[95m"
+
+
+class Formatter(logging.Formatter):
+    """Format the log record."""
+
+    def __init__(self) -> None:
+        super().__init__(
+            "[%(asctime)s] | %(pathname)s:%(lineno)d | %(levelname)s | %(message)s",
+            style="%",
+        )
+
+    def format(self, record: logging.LogRecord) -> str:
+        """Format the log record."""
+        return f"{LogLevelColors[record.levelname].value}{super().format(record)}{LogLevelColors.ENDC.value}"
+
+
+class FileHandler(logging.FileHandler):
+    """Emit a log record.
+
+    Parameters
+    ----------
+    ext : str
+        The file extension.
+    folder : pathlib.Path | str
+        The folder to save the logs in. Defaults to "logs".
+    """
+
+    _last_entry: datetime.datetime = datetime.datetime.today()
+
+    def __init__(self, *, ext: str, folder: t.Union[pathlib.Path, str] = "logs") -> None:
+        """Create a new file handler."""
+        self.folder = pathlib.Path(folder)
+        self.ext = ext
+        self.folder.mkdir(exist_ok=True)
+        super().__init__(
+            self.folder / f"{datetime.datetime.today().strftime('%Y-%m-%d')}-{ext}.log",
+            encoding="utf-8",
+        )
+        self.setFormatter(Formatter())
+
+    def emit(self, record: logging.LogRecord) -> None:
+        """Emit a log record."""
+        if self._last_entry.date() != datetime.datetime.today().date():
+            self._last_entry = datetime.datetime.today()
+            self.close()
+            self.baseFilename = (self.folder / f"{self._last_entry.strftime('%Y-%m-%d')}-{self.ext}.log").as_posix()
+            self.stream = self._open()
+        super().emit(record)
+
+
+class Logger(logging.Logger):
+    """
+    The logger used to log information about the client.
+
+    Parameters
+    ----------
+    name : str
+        The name of the logger.
+    level : int
+        The level of the logger.
+    file_logging : bool
+        Whether or not to log to a file.
+
+    Attributes
+    ----------
+    _handler : logging.StreamHandler
+        The stream handler used to log to the console.
+    _file_handler : t.Optional[logging.FileHandler]
+        The file handler used to log to a file.
+
+    Examples
+    --------
+
+    >>> logs = Logger(name="pokelance")
+    >>> logs.info("Hello, world!")
+    [2021-08-29 17:05:32,000] | pokelance\logger.py:95 | INFO | Hello, world!
+
+    """
+
+    file_handler: t.Optional[FileHandler] = None
+
+    def __init__(self, *, name: str, level: int = logging.INFO, file_logging: bool = False) -> None:
+        super().__init__(name, level)
+        self._handler = logging.StreamHandler()
+        self._handler.setFormatter(Formatter())
+        self.addHandler(self._handler)
+        if file_logging:
+            self._file_handler = FileHandler(ext=name)
+            self.addHandler(self._file_handler)
+        logging.addLevelName(FLAIR, "FLAIR")
+
+    def set_formatter(self, formatter: logging.Formatter) -> None:
+        """Set the formatter."""
+        self._handler.setFormatter(formatter)
+        self._file_handler.setFormatter(formatter)
+
+    def flair(self, message: str, *args: t.Any, **kwargs: t.Any) -> None:
+        """Record a flair log."""
+        self.log(FLAIR, message, *args, **kwargs)
```

### Comparing `pokelance-0.0.9a0/pokelance/models/__init__.py` & `pokelance-0.1.0/pokelance/models/abstract/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,107 +1,80 @@
-import typing as t
-
-from ._base import BaseModel
-from .abstract import (
-    Ability,
-    Berry,
-    BerryFirmness,
-    BerryFlavor,
-    Characteristic,
-    ContestEffect,
-    ContestType,
-    EggGroup,
-    EncounterCondition,
-    EncounterConditionValue,
-    EncounterMethod,
-    EvolutionChain,
-    EvolutionTrigger,
-    Gender,
-    Generation,
-    GrowthRate,
-    Item,
-    ItemAttribute,
-    ItemCategory,
-    ItemFlingEffect,
-    ItemPocket,
-    Location,
-    LocationArea,
-    LocationAreaEncounter,
-    Machine,
-    Move,
-    MoveAilment,
-    MoveBattleStyle,
-    MoveCategory,
-    MoveDamageClass,
-    MoveLearnMethod,
-    MoveTarget,
-    Nature,
-    PalParkArea,
-    PokeathlonStat,
-    Pokedex,
-    Pokemon,
-    PokemonColor,
-    PokemonForm,
-    PokemonHabitats,
-    PokemonShape,
-    PokemonSpecies,
-    Region,
-    Stat,
-    SuperContestEffect,
-    Type,
-    Version,
-    VersionGroup,
-)
-from .common import Language
-
-__all__: t.Tuple[str, ...] = (
-    "BaseModel",
-    "Berry",
-    "BerryFirmness",
-    "BerryFlavor",
-    "ContestEffect",
-    "ContestType",
-    "SuperContestEffect",
-    "EncounterCondition",
-    "EncounterConditionValue",
-    "EncounterMethod",
-    "EvolutionChain",
-    "EvolutionTrigger",
-    "Generation",
-    "Pokedex",
-    "Version",
-    "VersionGroup",
-    "Item",
-    "ItemAttribute",
-    "ItemCategory",
-    "ItemFlingEffect",
-    "ItemPocket",
-    "Location",
-    "LocationArea",
-    "PalParkArea",
-    "Region",
-    "Machine",
-    "Move",
-    "MoveAilment",
-    "MoveBattleStyle",
-    "MoveCategory",
-    "MoveDamageClass",
-    "MoveLearnMethod",
-    "MoveTarget",
-    "Ability",
-    "Characteristic",
-    "Pokemon",
-    "PokemonSpecies",
-    "PokemonForm",
-    "Nature",
-    "Type",
-    "Gender",
-    "GrowthRate",
-    "EggGroup",
-    "LocationAreaEncounter",
-    "PokemonColor",
-    "PokeathlonStat",
-    "PokemonHabitats",
-    "PokemonShape",
-    "Stat",
-    "Language",
-)
+import typing as t
+
+from .berry import Berry, BerryFirmness, BerryFlavor
+from .contest import ContestEffect, ContestType, SuperContestEffect
+from .encounter import EncounterCondition, EncounterConditionValue, EncounterMethod
+from .evolution import EvolutionChain, EvolutionTrigger
+from .game import Generation, Pokedex, Version, VersionGroup
+from .item import Item, ItemAttribute, ItemCategory, ItemFlingEffect, ItemPocket
+from .location import Location, LocationArea, PalParkArea, Region
+from .machine import Machine
+from .move import Move, MoveAilment, MoveBattleStyle, MoveCategory, MoveDamageClass, MoveLearnMethod, MoveTarget
+from .pokemon import (
+    Ability,
+    Characteristic,
+    EggGroup,
+    Gender,
+    GrowthRate,
+    LocationAreaEncounter,
+    Nature,
+    PokeathlonStat,
+    Pokemon,
+    PokemonColor,
+    PokemonForm,
+    PokemonHabitats,
+    PokemonShape,
+    PokemonSpecies,
+    Stat,
+    Type,
+)
+
+__all__: t.Tuple[str, ...] = (
+    "Berry",
+    "BerryFirmness",
+    "BerryFlavor",
+    "ContestEffect",
+    "ContestType",
+    "SuperContestEffect",
+    "EncounterCondition",
+    "EncounterConditionValue",
+    "EncounterMethod",
+    "EvolutionChain",
+    "EvolutionTrigger",
+    "Generation",
+    "Pokedex",
+    "Version",
+    "VersionGroup",
+    "Item",
+    "ItemAttribute",
+    "ItemCategory",
+    "ItemFlingEffect",
+    "ItemPocket",
+    "Location",
+    "LocationArea",
+    "PalParkArea",
+    "Region",
+    "Machine",
+    "Move",
+    "MoveAilment",
+    "MoveBattleStyle",
+    "MoveCategory",
+    "MoveDamageClass",
+    "MoveLearnMethod",
+    "MoveTarget",
+    "Ability",
+    "Characteristic",
+    "Pokemon",
+    "PokemonSpecies",
+    "PokemonForm",
+    "Nature",
+    "Type",
+    "Gender",
+    "GrowthRate",
+    "EggGroup",
+    "LocationAreaEncounter",
+    "PokemonColor",
+    "PokeathlonStat",
+    "PokemonHabitats",
+    "PokemonShape",
+    "Stat",
+)
```

### Comparing `pokelance-0.0.9a0/pokelance/models/_base.py` & `pokelance-0.1.0/pokelance/models/_base.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import typing as t
-
-import attrs
-
-
-@attrs.define(hash=True, slots=True, kw_only=True)
-class BaseModel:
-    """Base model for all models"""
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "BaseModel":
-        """Create a model from a payload
-
-        Parameters
-        ----------
-        payload: typing.Dict[str, Any]
-            The payload to create the model from.
-
-        Returns
-        -------
-        BaseModel
-            The model created from the payload.
-        """
-        return cls()
+import typing as t
+
+import attrs
+
+
+@attrs.define(hash=True, slots=True, kw_only=True)
+class BaseModel:
+    """Base model for all models"""
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "BaseModel":
+        """Create a model from a payload
+
+        Parameters
+        ----------
+        payload: typing.Dict[str, Any]
+            The payload to create the model from.
+
+        Returns
+        -------
+        BaseModel
+            The model created from the payload.
+        """
+        return cls()
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/__init__.py` & `pokelance-0.1.0/pokelance/models/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,107 @@
-import typing as t
-
-from .berry import Berry, BerryFirmness, BerryFlavor
-from .contest import ContestEffect, ContestType, SuperContestEffect
-from .encounter import EncounterCondition, EncounterConditionValue, EncounterMethod
-from .evolution import EvolutionChain, EvolutionTrigger
-from .game import Generation, Pokedex, Version, VersionGroup
-from .item import Item, ItemAttribute, ItemCategory, ItemFlingEffect, ItemPocket
-from .location import Location, LocationArea, PalParkArea, Region
-from .machine import Machine
-from .move import Move, MoveAilment, MoveBattleStyle, MoveCategory, MoveDamageClass, MoveLearnMethod, MoveTarget
-from .pokemon import (
-    Ability,
-    Characteristic,
-    EggGroup,
-    Gender,
-    GrowthRate,
-    LocationAreaEncounter,
-    Nature,
-    PokeathlonStat,
-    Pokemon,
-    PokemonColor,
-    PokemonForm,
-    PokemonHabitats,
-    PokemonShape,
-    PokemonSpecies,
-    Stat,
-    Type,
-)
-
-__all__: t.Tuple[str, ...] = (
-    "Berry",
-    "BerryFirmness",
-    "BerryFlavor",
-    "ContestEffect",
-    "ContestType",
-    "SuperContestEffect",
-    "EncounterCondition",
-    "EncounterConditionValue",
-    "EncounterMethod",
-    "EvolutionChain",
-    "EvolutionTrigger",
-    "Generation",
-    "Pokedex",
-    "Version",
-    "VersionGroup",
-    "Item",
-    "ItemAttribute",
-    "ItemCategory",
-    "ItemFlingEffect",
-    "ItemPocket",
-    "Location",
-    "LocationArea",
-    "PalParkArea",
-    "Region",
-    "Machine",
-    "Move",
-    "MoveAilment",
-    "MoveBattleStyle",
-    "MoveCategory",
-    "MoveDamageClass",
-    "MoveLearnMethod",
-    "MoveTarget",
-    "Ability",
-    "Characteristic",
-    "Pokemon",
-    "PokemonSpecies",
-    "PokemonForm",
-    "Nature",
-    "Type",
-    "Gender",
-    "GrowthRate",
-    "EggGroup",
-    "LocationAreaEncounter",
-    "PokemonColor",
-    "PokeathlonStat",
-    "PokemonHabitats",
-    "PokemonShape",
-    "Stat",
-)
+import typing as t
+
+from ._base import BaseModel
+from .abstract import (
+    Ability,
+    Berry,
+    BerryFirmness,
+    BerryFlavor,
+    Characteristic,
+    ContestEffect,
+    ContestType,
+    EggGroup,
+    EncounterCondition,
+    EncounterConditionValue,
+    EncounterMethod,
+    EvolutionChain,
+    EvolutionTrigger,
+    Gender,
+    Generation,
+    GrowthRate,
+    Item,
+    ItemAttribute,
+    ItemCategory,
+    ItemFlingEffect,
+    ItemPocket,
+    Location,
+    LocationArea,
+    LocationAreaEncounter,
+    Machine,
+    Move,
+    MoveAilment,
+    MoveBattleStyle,
+    MoveCategory,
+    MoveDamageClass,
+    MoveLearnMethod,
+    MoveTarget,
+    Nature,
+    PalParkArea,
+    PokeathlonStat,
+    Pokedex,
+    Pokemon,
+    PokemonColor,
+    PokemonForm,
+    PokemonHabitats,
+    PokemonShape,
+    PokemonSpecies,
+    Region,
+    Stat,
+    SuperContestEffect,
+    Type,
+    Version,
+    VersionGroup,
+)
+from .common import Language
+
+__all__: t.Tuple[str, ...] = (
+    "BaseModel",
+    "Berry",
+    "BerryFirmness",
+    "BerryFlavor",
+    "ContestEffect",
+    "ContestType",
+    "SuperContestEffect",
+    "EncounterCondition",
+    "EncounterConditionValue",
+    "EncounterMethod",
+    "EvolutionChain",
+    "EvolutionTrigger",
+    "Generation",
+    "Pokedex",
+    "Version",
+    "VersionGroup",
+    "Item",
+    "ItemAttribute",
+    "ItemCategory",
+    "ItemFlingEffect",
+    "ItemPocket",
+    "Location",
+    "LocationArea",
+    "PalParkArea",
+    "Region",
+    "Machine",
+    "Move",
+    "MoveAilment",
+    "MoveBattleStyle",
+    "MoveCategory",
+    "MoveDamageClass",
+    "MoveLearnMethod",
+    "MoveTarget",
+    "Ability",
+    "Characteristic",
+    "Pokemon",
+    "PokemonSpecies",
+    "PokemonForm",
+    "Nature",
+    "Type",
+    "Gender",
+    "GrowthRate",
+    "EggGroup",
+    "LocationAreaEncounter",
+    "PokemonColor",
+    "PokeathlonStat",
+    "PokemonHabitats",
+    "PokemonShape",
+    "Stat",
+    "Language",
+)
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/berry.py` & `pokelance-0.1.0/pokelance/models/abstract/berry.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import Name, NamedResource
-
-from .utils import BerryFlavorMap, FlavorBerryMap
-
-__all__: t.Tuple[str, ...] = (
-    "Berry",
-    "BerryFirmness",
-    "BerryFlavor",
-)
-
-
-@attrs.define(slots=True, kw_only=True)
-class Berry(BaseModel):
-    """A berry resource.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this berry resource.
-    name: str
-        The name for this berry resource.
-    growth_time: int
-        Time it takes the tree to grow one stage, in hours. Berry trees go through
-        four of these growth stages before they can be picked.
-    max_harvest: int
-        The maximum number of these berries that can grow on one tree in Generation
-        IV.
-    natural_gift_power: int
-        The power of the move "Natural Gift" when used with this Berry.
-    size: int
-        Berries are actually items. This is the number of those items.
-    smoothness: int
-        The speed at which this Berry dries out the soil as it grows. A higher
-        rate means the soil dries more quickly.
-    soil_dryness: int
-        The firmness of this berry, used in making Pokéblocks or Poffins.
-    flavors: typing.List[BerryFlavorMap]
-        A list of references to each flavor a berry can have and the potency of
-        each of those flavors in regard to this berry.
-    item: pokelance.models.common.NamedResource
-        The item that corresponds to this berry.
-    natural_gift_type: pokelance.models.common.NamedResource
-        The type inherited by "Natural Gift" when used with this Berry.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    growth_time: int = attrs.field(factory=int)
-    max_harvest: int = attrs.field(factory=int)
-    natural_gift_power: int = attrs.field(factory=int)
-    size: int = attrs.field(factory=int)
-    smoothness: int = attrs.field(factory=int)
-    soil_dryness: int = attrs.field(factory=int)
-    firmness: NamedResource = attrs.field(factory=NamedResource)
-    flavors: t.List[BerryFlavorMap] = attrs.field(factory=list)
-    item: NamedResource = attrs.field(factory=NamedResource)
-    natural_gift_type: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, data: t.Dict[str, t.Any]) -> "Berry":
-        return cls(
-            id=data.get("id", 0),
-            name=data.get("name", ""),
-            growth_time=data.get("growth_time", 0),
-            max_harvest=data.get("max_harvest", 0),
-            natural_gift_power=data.get("natural_gift_power", 0),
-            size=data.get("size", 0),
-            smoothness=data.get("smoothness", 0),
-            soil_dryness=data.get("soil_dryness", 0),
-            firmness=NamedResource.from_payload(data.get("firmness", {}) or {}),
-            flavors=[BerryFlavorMap.from_payload(flavor) for flavor in data.get("flavors", [])],
-            item=NamedResource.from_payload(data.get("item", {}) or {}),
-            natural_gift_type=NamedResource.from_payload(data.get("natural_gift_type", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class BerryFirmness(BaseModel):
-    """A berry firmness resource.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this berry firmness resource.
-    name: str
-        The name for this berry firmness resource.
-    berries: typing.List[pokelance.models.common.NamedResource]
-        A list of the berries with this firmness.
-    names: typing.List[pokelance.models.common.Name]
-        A list of the name of this berry firmness listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    berries: t.List[NamedResource] = attrs.field(factory=list)
-    names: t.List[Name] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, data: t.Dict[str, t.Any]) -> "BerryFirmness":
-        return cls(
-            id=data.get("id", 0),
-            name=data.get("name", ""),
-            berries=[NamedResource.from_payload(berry) for berry in data.get("berries", [])],
-            names=[Name.from_payload(name) for name in data.get("names", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class BerryFlavor(BaseModel):
-    """A berry flavor resource.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this berry flavor resource.
-    name: str
-        The name for this berry flavor resource.
-    berries: typing.List[FlavorBerryMap]
-        A list of the berries with this flavor.
-    contest_type: pokelance.models.common.NamedResource
-        The contest type that correlates with this berry flavor.
-    names: typing.List[pokelance.models.common.Name]
-        The name of this berry flavor listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    berries: t.List[FlavorBerryMap] = attrs.field(factory=list)
-    contest_type: NamedResource = attrs.field(factory=NamedResource)
-    names: t.List[Name] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, data: t.Dict[str, t.Any]) -> "BerryFlavor":
-        return cls(
-            id=data.get("id", 0),
-            name=data.get("name", ""),
-            berries=[FlavorBerryMap.from_payload(berry) for berry in data.get("berries", [])],
-            contest_type=NamedResource.from_payload(data.get("contest_type", {}) or {}),
-            names=[Name.from_payload(name) for name in data.get("names", [])],
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import Name, NamedResource
+
+from .utils import BerryFlavorMap, FlavorBerryMap
+
+__all__: t.Tuple[str, ...] = (
+    "Berry",
+    "BerryFirmness",
+    "BerryFlavor",
+)
+
+
+@attrs.define(slots=True, kw_only=True)
+class Berry(BaseModel):
+    """A berry resource.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this berry resource.
+    name: str
+        The name for this berry resource.
+    growth_time: int
+        Time it takes the tree to grow one stage, in hours. Berry trees go through
+        four of these growth stages before they can be picked.
+    max_harvest: int
+        The maximum number of these berries that can grow on one tree in Generation
+        IV.
+    natural_gift_power: int
+        The power of the move "Natural Gift" when used with this Berry.
+    size: int
+        Berries are actually items. This is the number of those items.
+    smoothness: int
+        The speed at which this Berry dries out the soil as it grows. A higher
+        rate means the soil dries more quickly.
+    soil_dryness: int
+        The firmness of this berry, used in making Pokéblocks or Poffins.
+    flavors: typing.List[BerryFlavorMap]
+        A list of references to each flavor a berry can have and the potency of
+        each of those flavors in regard to this berry.
+    item: pokelance.models.common.NamedResource
+        The item that corresponds to this berry.
+    natural_gift_type: pokelance.models.common.NamedResource
+        The type inherited by "Natural Gift" when used with this Berry.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    growth_time: int = attrs.field(factory=int)
+    max_harvest: int = attrs.field(factory=int)
+    natural_gift_power: int = attrs.field(factory=int)
+    size: int = attrs.field(factory=int)
+    smoothness: int = attrs.field(factory=int)
+    soil_dryness: int = attrs.field(factory=int)
+    firmness: NamedResource = attrs.field(factory=NamedResource)
+    flavors: t.List[BerryFlavorMap] = attrs.field(factory=list)
+    item: NamedResource = attrs.field(factory=NamedResource)
+    natural_gift_type: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, data: t.Dict[str, t.Any]) -> "Berry":
+        return cls(
+            id=data.get("id", 0),
+            name=data.get("name", ""),
+            growth_time=data.get("growth_time", 0),
+            max_harvest=data.get("max_harvest", 0),
+            natural_gift_power=data.get("natural_gift_power", 0),
+            size=data.get("size", 0),
+            smoothness=data.get("smoothness", 0),
+            soil_dryness=data.get("soil_dryness", 0),
+            firmness=NamedResource.from_payload(data.get("firmness", {}) or {}),
+            flavors=[BerryFlavorMap.from_payload(flavor) for flavor in data.get("flavors", [])],
+            item=NamedResource.from_payload(data.get("item", {}) or {}),
+            natural_gift_type=NamedResource.from_payload(data.get("natural_gift_type", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class BerryFirmness(BaseModel):
+    """A berry firmness resource.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this berry firmness resource.
+    name: str
+        The name for this berry firmness resource.
+    berries: typing.List[pokelance.models.common.NamedResource]
+        A list of the berries with this firmness.
+    names: typing.List[pokelance.models.common.Name]
+        A list of the name of this berry firmness listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    berries: t.List[NamedResource] = attrs.field(factory=list)
+    names: t.List[Name] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, data: t.Dict[str, t.Any]) -> "BerryFirmness":
+        return cls(
+            id=data.get("id", 0),
+            name=data.get("name", ""),
+            berries=[NamedResource.from_payload(berry) for berry in data.get("berries", [])],
+            names=[Name.from_payload(name) for name in data.get("names", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class BerryFlavor(BaseModel):
+    """A berry flavor resource.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this berry flavor resource.
+    name: str
+        The name for this berry flavor resource.
+    berries: typing.List[FlavorBerryMap]
+        A list of the berries with this flavor.
+    contest_type: pokelance.models.common.NamedResource
+        The contest type that correlates with this berry flavor.
+    names: typing.List[pokelance.models.common.Name]
+        The name of this berry flavor listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    berries: t.List[FlavorBerryMap] = attrs.field(factory=list)
+    contest_type: NamedResource = attrs.field(factory=NamedResource)
+    names: t.List[Name] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, data: t.Dict[str, t.Any]) -> "BerryFlavor":
+        return cls(
+            id=data.get("id", 0),
+            name=data.get("name", ""),
+            berries=[FlavorBerryMap.from_payload(berry) for berry in data.get("berries", [])],
+            contest_type=NamedResource.from_payload(data.get("contest_type", {}) or {}),
+            names=[Name.from_payload(name) for name in data.get("names", [])],
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/contest.py` & `pokelance-0.1.0/pokelance/models/abstract/contest.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import Effect, FlavorText, NamedResource
-
-from .utils import ContestName
-
-__all__: t.Tuple[str, ...] = (
-    "ContestType",
-    "ContestEffect",
-    "SuperContestEffect",
-)
-
-
-@attrs.define(slots=True, kw_only=True)
-class ContestType(BaseModel):
-    """A contest type resource.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this contest type resource.
-    name: str
-        The name for this contest type resource.
-    berry_flavor: pokelance.models.common.NamedResource
-        The berry flavor that correlates with this contest type.
-    names: typing.List[pokelance.models.common.Name]
-        The name of this contest type listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    berry_flavor: NamedResource = attrs.field(factory=NamedResource)
-    names: t.List[ContestName] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ContestType":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            berry_flavor=NamedResource.from_payload(payload.get("berry_flavor", {}) or {}),
-            names=[ContestName.from_payload(name) for name in payload.get("names", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class ContestEffect(BaseModel):
-    """A contest effect resource.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this contest effect resource.
-    appeal: int
-        The base number of hearts the user of this move gets.
-    jam: int
-        The base number of hearts the user's opponent loses.
-    effect_entries: typing.List[pokelance.models.common.Effect]
-        The result of this contest effect listed in different languages.
-    flavor_text_entries: typing.List[pokelance.models.common.FlavorText]
-        The flavor text of this contest effect listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    appeal: int = attrs.field(factory=int)
-    jam: int = attrs.field(factory=int)
-    effect_entries: t.List[Effect] = attrs.field(factory=list)
-    flavor_text_entries: t.List[FlavorText] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ContestEffect":
-        return cls(
-            id=payload.get("id", 0),
-            appeal=payload.get("appeal", 0),
-            jam=payload.get("jam", 0),
-            effect_entries=[Effect.from_payload(effect) for effect in payload.get("effect_entries", [])],
-            flavor_text_entries=[
-                FlavorText.from_payload(flavor_text) for flavor_text in payload.get("flavor_text_entries", [])
-            ],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class SuperContestEffect(BaseModel):
-    """A super contest effect resource.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this super contest effect resource.
-    appeal: int
-        The level of appeal this super contest effect has.
-    flavor_text_entries: typing.List[pokelance.models.common.FlavorText]
-        The flavor text of this super contest effect listed in different languages.
-    moves: typing.List[pokelance.models.common.NamedResource]
-        A list of moves that have the effect when used in super contests.
-    """
-
-    id: int = attrs.field(factory=int)
-    appeal: int = attrs.field(factory=int)
-    flavor_text_entries: t.List[FlavorText] = attrs.field(factory=list)
-    moves: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "SuperContestEffect":
-        return cls(
-            id=payload.get("id", 0),
-            appeal=payload.get("appeal", 0),
-            flavor_text_entries=[
-                FlavorText.from_payload(flavor_text) for flavor_text in payload.get("flavor_text_entries", [])
-            ],
-            moves=[NamedResource.from_payload(move) for move in payload.get("moves", [])],
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import Effect, FlavorText, NamedResource
+
+from .utils import ContestName
+
+__all__: t.Tuple[str, ...] = (
+    "ContestType",
+    "ContestEffect",
+    "SuperContestEffect",
+)
+
+
+@attrs.define(slots=True, kw_only=True)
+class ContestType(BaseModel):
+    """A contest type resource.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this contest type resource.
+    name: str
+        The name for this contest type resource.
+    berry_flavor: pokelance.models.common.NamedResource
+        The berry flavor that correlates with this contest type.
+    names: typing.List[pokelance.models.common.Name]
+        The name of this contest type listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    berry_flavor: NamedResource = attrs.field(factory=NamedResource)
+    names: t.List[ContestName] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ContestType":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            berry_flavor=NamedResource.from_payload(payload.get("berry_flavor", {}) or {}),
+            names=[ContestName.from_payload(name) for name in payload.get("names", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class ContestEffect(BaseModel):
+    """A contest effect resource.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this contest effect resource.
+    appeal: int
+        The base number of hearts the user of this move gets.
+    jam: int
+        The base number of hearts the user's opponent loses.
+    effect_entries: typing.List[pokelance.models.common.Effect]
+        The result of this contest effect listed in different languages.
+    flavor_text_entries: typing.List[pokelance.models.common.FlavorText]
+        The flavor text of this contest effect listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    appeal: int = attrs.field(factory=int)
+    jam: int = attrs.field(factory=int)
+    effect_entries: t.List[Effect] = attrs.field(factory=list)
+    flavor_text_entries: t.List[FlavorText] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ContestEffect":
+        return cls(
+            id=payload.get("id", 0),
+            appeal=payload.get("appeal", 0),
+            jam=payload.get("jam", 0),
+            effect_entries=[Effect.from_payload(effect) for effect in payload.get("effect_entries", [])],
+            flavor_text_entries=[
+                FlavorText.from_payload(flavor_text) for flavor_text in payload.get("flavor_text_entries", [])
+            ],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class SuperContestEffect(BaseModel):
+    """A super contest effect resource.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this super contest effect resource.
+    appeal: int
+        The level of appeal this super contest effect has.
+    flavor_text_entries: typing.List[pokelance.models.common.FlavorText]
+        The flavor text of this super contest effect listed in different languages.
+    moves: typing.List[pokelance.models.common.NamedResource]
+        A list of moves that have the effect when used in super contests.
+    """
+
+    id: int = attrs.field(factory=int)
+    appeal: int = attrs.field(factory=int)
+    flavor_text_entries: t.List[FlavorText] = attrs.field(factory=list)
+    moves: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "SuperContestEffect":
+        return cls(
+            id=payload.get("id", 0),
+            appeal=payload.get("appeal", 0),
+            flavor_text_entries=[
+                FlavorText.from_payload(flavor_text) for flavor_text in payload.get("flavor_text_entries", [])
+            ],
+            moves=[NamedResource.from_payload(move) for move in payload.get("moves", [])],
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/encounter.py` & `pokelance-0.1.0/pokelance/models/abstract/encounter.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import Name, NamedResource
-
-__all__: t.Tuple[str, ...] = (
-    "EncounterMethod",
-    "EncounterCondition",
-    "EncounterConditionValue",
-)
-
-
-@attrs.define(slots=True, kw_only=True)
-class EncounterMethod(BaseModel):
-    """An encounter method resource.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this encounter method resource.
-    name: str
-        The name for this encounter method resource.
-    order: int
-        A good value for sorting.
-    names: typing.List[pokelance.models.common.Name]
-        The name of this encounter method listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    order: int = attrs.field(factory=int)
-    names: t.List[Name] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EncounterMethod":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            order=payload.get("order", 0),
-            names=[Name.from_payload(name) for name in payload.get("names", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class EncounterCondition(BaseModel):
-    """An encounter condition resource.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this encounter condition resource.
-    name: str
-        The name for this encounter condition resource.
-    names: typing.List[pokelance.models.common.Name]
-        The name of this encounter condition listed in different languages.
-    values: typing.List[pokelance.models.common.NamedResource]
-        A list of possible values for this encounter condition.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    names: t.List[Name] = attrs.field(factory=list)
-    values: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EncounterCondition":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            names=[Name.from_payload(name) for name in payload.get("names", [])],
-            values=[NamedResource.from_payload(value) for value in payload.get("values", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class EncounterConditionValue(BaseModel):
-    """An encounter condition value resource.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this encounter condition value resource.
-    name: str
-        The name for this encounter condition value resource.
-    condition: pokelance.models.common.NamedResource
-        The condition this encounter condition value pertains to.
-    names: typing.List[pokelance.models.common.Name]
-        The name of this encounter condition value listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    condition: NamedResource = attrs.field(factory=NamedResource)
-    names: t.List[Name] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EncounterConditionValue":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            condition=NamedResource.from_payload(payload.get("condition", {}) or {}),
-            names=[Name.from_payload(name) for name in payload.get("names", [])],
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import Name, NamedResource
+
+__all__: t.Tuple[str, ...] = (
+    "EncounterMethod",
+    "EncounterCondition",
+    "EncounterConditionValue",
+)
+
+
+@attrs.define(slots=True, kw_only=True)
+class EncounterMethod(BaseModel):
+    """An encounter method resource.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this encounter method resource.
+    name: str
+        The name for this encounter method resource.
+    order: int
+        A good value for sorting.
+    names: typing.List[pokelance.models.common.Name]
+        The name of this encounter method listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    order: int = attrs.field(factory=int)
+    names: t.List[Name] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EncounterMethod":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            order=payload.get("order", 0),
+            names=[Name.from_payload(name) for name in payload.get("names", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class EncounterCondition(BaseModel):
+    """An encounter condition resource.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this encounter condition resource.
+    name: str
+        The name for this encounter condition resource.
+    names: typing.List[pokelance.models.common.Name]
+        The name of this encounter condition listed in different languages.
+    values: typing.List[pokelance.models.common.NamedResource]
+        A list of possible values for this encounter condition.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    names: t.List[Name] = attrs.field(factory=list)
+    values: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EncounterCondition":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            names=[Name.from_payload(name) for name in payload.get("names", [])],
+            values=[NamedResource.from_payload(value) for value in payload.get("values", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class EncounterConditionValue(BaseModel):
+    """An encounter condition value resource.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this encounter condition value resource.
+    name: str
+        The name for this encounter condition value resource.
+    condition: pokelance.models.common.NamedResource
+        The condition this encounter condition value pertains to.
+    names: typing.List[pokelance.models.common.Name]
+        The name of this encounter condition value listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    condition: NamedResource = attrs.field(factory=NamedResource)
+    names: t.List[Name] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EncounterConditionValue":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            condition=NamedResource.from_payload(payload.get("condition", {}) or {}),
+            names=[Name.from_payload(name) for name in payload.get("names", [])],
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/evolution.py` & `pokelance-0.1.0/pokelance/models/abstract/evolution.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import Name, NamedResource
-
-from .utils import ChainLink
-
-__all__: t.Tuple[str, ...] = (
-    "EvolutionChain",
-    "EvolutionTrigger",
-)
-
-
-@attrs.define(slots=True, kw_only=True)
-class EvolutionChain(BaseModel):
-    """Evolution chain model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    baby_trigger_item: t.Optional[NamedResource]
-        The item that a Pokémon would be holding when mating that would trigger the egg hatching a baby
-         Pokémon rather than a basic Pokémon.
-    chain: ChainLink
-        The base chain link object. Each link contains evolution details for a Pokémon in the chain.
-         Each link references the next Pokémon in the natural evolution order.
-    """
-
-    id: int = attrs.field(factory=int)
-    baby_trigger_item: NamedResource = attrs.field(factory=NamedResource)
-    chain: ChainLink = attrs.field(factory=ChainLink)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EvolutionChain":
-        return cls(
-            id=payload.get("id", 0),
-            baby_trigger_item=NamedResource.from_payload(payload.get("baby_trigger_item", {}) or {}),
-            chain=ChainLink.from_payload(payload.get("chain", {})),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class EvolutionTrigger(BaseModel):
-    """Evolution trigger model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    names: t.List[Name]
-        A list of name and language pairs for this resource.
-    pokemon_species: t.List[NamedResource]
-        A list of pokemon species that result from this evolution trigger.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    names: t.List[Name] = attrs.field(factory=list)
-    pokemon_species: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EvolutionTrigger":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            names=[Name.from_payload(name) for name in payload.get("names", [])],
-            pokemon_species=[NamedResource.from_payload(species) for species in payload.get("pokemon_species", [])],
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import Name, NamedResource
+
+from .utils import ChainLink
+
+__all__: t.Tuple[str, ...] = (
+    "EvolutionChain",
+    "EvolutionTrigger",
+)
+
+
+@attrs.define(slots=True, kw_only=True)
+class EvolutionChain(BaseModel):
+    """Evolution chain model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    baby_trigger_item: t.Optional[NamedResource]
+        The item that a Pokémon would be holding when mating that would trigger the egg hatching a baby
+         Pokémon rather than a basic Pokémon.
+    chain: ChainLink
+        The base chain link object. Each link contains evolution details for a Pokémon in the chain.
+         Each link references the next Pokémon in the natural evolution order.
+    """
+
+    id: int = attrs.field(factory=int)
+    baby_trigger_item: NamedResource = attrs.field(factory=NamedResource)
+    chain: ChainLink = attrs.field(factory=ChainLink)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EvolutionChain":
+        return cls(
+            id=payload.get("id", 0),
+            baby_trigger_item=NamedResource.from_payload(payload.get("baby_trigger_item", {}) or {}),
+            chain=ChainLink.from_payload(payload.get("chain", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class EvolutionTrigger(BaseModel):
+    """Evolution trigger model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    names: t.List[Name]
+        A list of name and language pairs for this resource.
+    pokemon_species: t.List[NamedResource]
+        A list of pokemon species that result from this evolution trigger.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    names: t.List[Name] = attrs.field(factory=list)
+    pokemon_species: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EvolutionTrigger":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            names=[Name.from_payload(name) for name in payload.get("names", [])],
+            pokemon_species=[NamedResource.from_payload(species) for species in payload.get("pokemon_species", [])],
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/game.py` & `pokelance-0.1.0/pokelance/models/abstract/game.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import Description, Name, NamedResource
-
-from .utils import PokemonEntry
-
-__all__: t.Tuple[str, ...] = (
-    "Generation",
-    "Pokedex",
-    "Version",
-    "VersionGroup",
-)
-
-
-@attrs.define(slots=True, kw_only=True)
-class Generation(BaseModel):
-    """Generation model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    abilities: t.List[NamedResource]
-        A list of abilities that were introduced in this generation.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    main_region: NamedResource
-        The main region travelled in this generation.
-    moves: t.List[NamedResource]
-        A list of moves that were introduced in this generation.
-    pokemon_species: t.List[NamedResource]
-        A list of Pokémon species that were introduced in this generation.
-    types: t.List[NamedResource]
-        A list of types that were introduced in this generation.
-    version_groups: t.List[NamedResource]
-        A list of version groups that were introduced in this generation.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    abilities: t.List[NamedResource] = attrs.field(factory=list)
-    names: t.List[Name] = attrs.field(factory=list)
-    main_region: NamedResource = attrs.field(factory=NamedResource)
-    moves: t.List[NamedResource] = attrs.field(factory=list)
-    pokemon_species: t.List[NamedResource] = attrs.field(factory=list)
-    types: t.List[NamedResource] = attrs.field(factory=list)
-    version_groups: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Generation":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            abilities=[NamedResource.from_payload(i) for i in payload.get("abilities", [])],
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            main_region=NamedResource.from_payload(payload.get("main_region", {}) or {}),
-            moves=[NamedResource.from_payload(i) for i in payload.get("moves", [])],
-            pokemon_species=[NamedResource.from_payload(i) for i in payload.get("pokemon_species", [])],
-            types=[NamedResource.from_payload(i) for i in payload.get("types", [])],
-            version_groups=[NamedResource.from_payload(i) for i in payload.get("version_groups", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Pokedex(BaseModel):
-    """Pokedex model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    is_main_series: bool
-        Whether or not this Pokédex originated in the main series of the video games.
-    descriptions: t.List[Description]
-        The description of this resource listed in different languages.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    pokemon_entries: t.List[PokemonEntry]
-        A list of Pokémon catalogued in this Pokédex and their indexes.
-    region: NamedResource
-        The region this Pokédex catalogues Pokémon for.
-    version_groups: t.List[NamedResource]
-        A list of version groups this Pokédex is relevant to.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    is_main_series: bool = attrs.field(factory=bool)
-    descriptions: t.List[Description] = attrs.field(factory=list)
-    names: t.List[Name] = attrs.field(factory=list)
-    pokemon_entries: t.List[PokemonEntry] = attrs.field(factory=list)
-    region: NamedResource = attrs.field(factory=NamedResource)
-    version_groups: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Pokedex":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            is_main_series=payload.get("is_main_series", False),
-            descriptions=[Description.from_payload(i) for i in payload.get("descriptions", [])],
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            pokemon_entries=[PokemonEntry.from_payload(i) for i in payload.get("pokemon_entries", [])],
-            region=NamedResource.from_payload(payload.get("region", {}) or {}),
-            version_groups=[NamedResource.from_payload(i) for i in payload.get("version_groups", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Version(BaseModel):
-    """Version model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    version_group: NamedResource
-        The version group this version belongs to.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    names: t.List[Name] = attrs.field(factory=list)
-    version_group: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Version":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class VersionGroup(BaseModel):
-    """VersionGroup model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    order: int
-        Order for sorting. Almost by date of release, except similar versions are grouped together.
-    generation: NamedResource
-        The generation this version was introduced in.
-    move_learn_methods: t.List[NamedResource]
-        A list of methods in which Pokémon can learn moves in this version group.
-    pokedexes: t.List[NamedResource]
-        A list of Pokédexes introduces in this version group.
-    regions: t.List[NamedResource]
-        A list of regions that can be visited in this version group.
-    versions: t.List[NamedResource]
-        A list of versions this version group owns.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    order: int = attrs.field(factory=int)
-    generation: NamedResource = attrs.field(factory=NamedResource)
-    move_learn_methods: t.List[NamedResource] = attrs.field(factory=list)
-    pokedexes: t.List[NamedResource] = attrs.field(factory=list)
-    regions: t.List[NamedResource] = attrs.field(factory=list)
-    versions: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "VersionGroup":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            order=payload.get("order", 0),
-            generation=NamedResource.from_payload(payload.get("generation", {}) or {}),
-            move_learn_methods=[NamedResource.from_payload(i) for i in payload.get("move_learn_methods", [])],
-            pokedexes=[NamedResource.from_payload(i) for i in payload.get("pokedexes", [])],
-            regions=[NamedResource.from_payload(i) for i in payload.get("regions", [])],
-            versions=[NamedResource.from_payload(i) for i in payload.get("versions", [])],
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import Description, Name, NamedResource
+
+from .utils import PokemonEntry
+
+__all__: t.Tuple[str, ...] = (
+    "Generation",
+    "Pokedex",
+    "Version",
+    "VersionGroup",
+)
+
+
+@attrs.define(slots=True, kw_only=True)
+class Generation(BaseModel):
+    """Generation model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    abilities: t.List[NamedResource]
+        A list of abilities that were introduced in this generation.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    main_region: NamedResource
+        The main region travelled in this generation.
+    moves: t.List[NamedResource]
+        A list of moves that were introduced in this generation.
+    pokemon_species: t.List[NamedResource]
+        A list of Pokémon species that were introduced in this generation.
+    types: t.List[NamedResource]
+        A list of types that were introduced in this generation.
+    version_groups: t.List[NamedResource]
+        A list of version groups that were introduced in this generation.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    abilities: t.List[NamedResource] = attrs.field(factory=list)
+    names: t.List[Name] = attrs.field(factory=list)
+    main_region: NamedResource = attrs.field(factory=NamedResource)
+    moves: t.List[NamedResource] = attrs.field(factory=list)
+    pokemon_species: t.List[NamedResource] = attrs.field(factory=list)
+    types: t.List[NamedResource] = attrs.field(factory=list)
+    version_groups: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Generation":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            abilities=[NamedResource.from_payload(i) for i in payload.get("abilities", [])],
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            main_region=NamedResource.from_payload(payload.get("main_region", {}) or {}),
+            moves=[NamedResource.from_payload(i) for i in payload.get("moves", [])],
+            pokemon_species=[NamedResource.from_payload(i) for i in payload.get("pokemon_species", [])],
+            types=[NamedResource.from_payload(i) for i in payload.get("types", [])],
+            version_groups=[NamedResource.from_payload(i) for i in payload.get("version_groups", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Pokedex(BaseModel):
+    """Pokedex model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    is_main_series: bool
+        Whether or not this Pokédex originated in the main series of the video games.
+    descriptions: t.List[Description]
+        The description of this resource listed in different languages.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    pokemon_entries: t.List[PokemonEntry]
+        A list of Pokémon catalogued in this Pokédex and their indexes.
+    region: NamedResource
+        The region this Pokédex catalogues Pokémon for.
+    version_groups: t.List[NamedResource]
+        A list of version groups this Pokédex is relevant to.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    is_main_series: bool = attrs.field(factory=bool)
+    descriptions: t.List[Description] = attrs.field(factory=list)
+    names: t.List[Name] = attrs.field(factory=list)
+    pokemon_entries: t.List[PokemonEntry] = attrs.field(factory=list)
+    region: NamedResource = attrs.field(factory=NamedResource)
+    version_groups: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Pokedex":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            is_main_series=payload.get("is_main_series", False),
+            descriptions=[Description.from_payload(i) for i in payload.get("descriptions", [])],
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            pokemon_entries=[PokemonEntry.from_payload(i) for i in payload.get("pokemon_entries", [])],
+            region=NamedResource.from_payload(payload.get("region", {}) or {}),
+            version_groups=[NamedResource.from_payload(i) for i in payload.get("version_groups", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Version(BaseModel):
+    """Version model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    version_group: NamedResource
+        The version group this version belongs to.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    names: t.List[Name] = attrs.field(factory=list)
+    version_group: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Version":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class VersionGroup(BaseModel):
+    """VersionGroup model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    order: int
+        Order for sorting. Almost by date of release, except similar versions are grouped together.
+    generation: NamedResource
+        The generation this version was introduced in.
+    move_learn_methods: t.List[NamedResource]
+        A list of methods in which Pokémon can learn moves in this version group.
+    pokedexes: t.List[NamedResource]
+        A list of Pokédexes introduces in this version group.
+    regions: t.List[NamedResource]
+        A list of regions that can be visited in this version group.
+    versions: t.List[NamedResource]
+        A list of versions this version group owns.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    order: int = attrs.field(factory=int)
+    generation: NamedResource = attrs.field(factory=NamedResource)
+    move_learn_methods: t.List[NamedResource] = attrs.field(factory=list)
+    pokedexes: t.List[NamedResource] = attrs.field(factory=list)
+    regions: t.List[NamedResource] = attrs.field(factory=list)
+    versions: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "VersionGroup":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            order=payload.get("order", 0),
+            generation=NamedResource.from_payload(payload.get("generation", {}) or {}),
+            move_learn_methods=[NamedResource.from_payload(i) for i in payload.get("move_learn_methods", [])],
+            pokedexes=[NamedResource.from_payload(i) for i in payload.get("pokedexes", [])],
+            regions=[NamedResource.from_payload(i) for i in payload.get("regions", [])],
+            versions=[NamedResource.from_payload(i) for i in payload.get("versions", [])],
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/item.py` & `pokelance-0.1.0/pokelance/models/abstract/item.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import (
-    Description,
-    Effect,
-    GenerationGameIndex,
-    MachineVersionDetail,
-    Name,
-    NamedResource,
-    VerboseEffect,
-    VersionGroupFlavorText,
-)
-
-from .utils import ItemHolderPokemon, ItemSprites
-
-__all__: t.Tuple[str, ...] = ("Item", "ItemAttribute", "ItemCategory", "ItemFlingEffect", "ItemPocket")
-
-
-@attrs.define(slots=True, kw_only=True)
-class Item(BaseModel):
-    """Item model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    cost: int
-        The price of this item in stores.
-    fling_power: int
-        The power of the move Fling when used with this item.
-    fling_effect: NamedResource
-        The effect of the move Fling when used with this item.
-    attributes: t.List[NamedResource]
-        A list of attributes this item has.
-    category: NamedResource
-        The category of items this item falls into.
-    effect_entries: t.List[Effect]
-        The effect of this ability listed in different languages.
-    flavor_text_entries: t.List[VersionGroupFlavorText]
-        The flavor text of this ability listed in different languages.
-    game_indices: t.List[GenerationGameIndex]
-        A list of game indices relevent to this item by generation.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    sprites: ItemSprites
-        A set of sprites used to depict this item in the game.
-    held_by_pokemon: t.List[ItemHolderPokemon]
-        A list of Pokémon that might be found in the wild holding this item.
-    baby_trigger_for: NamedResource
-        An evolution chain this item requires to produce a bay during mating.
-    machines: t.List[MachineVersionDetail]
-        A list of the machines related to this item.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    cost: int = attrs.field(factory=int)
-    fling_power: int = attrs.field(factory=int)
-    fling_effect: NamedResource = attrs.field(factory=NamedResource)
-    attributes: t.List[NamedResource] = attrs.field(factory=list)
-    category: NamedResource = attrs.field(factory=NamedResource)
-    effect_entries: t.List[VerboseEffect] = attrs.field(factory=list)
-    flavor_text_entries: t.List[VersionGroupFlavorText] = attrs.field(factory=list)
-    game_indices: t.List[GenerationGameIndex] = attrs.field(factory=list)
-    names: t.List[Name] = attrs.field(factory=list)
-    sprites: ItemSprites = attrs.field(factory=ItemSprites)
-    held_by_pokemon: t.List[ItemHolderPokemon] = attrs.field(factory=list)
-    baby_trigger_for: NamedResource = attrs.field(factory=NamedResource)
-    machines: t.List[MachineVersionDetail] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Item":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            cost=payload.get("cost", 0),
-            fling_power=payload.get("fling_power", 0),
-            fling_effect=NamedResource.from_payload(payload.get("fling_effect", {}) or {}),
-            attributes=[NamedResource.from_payload(attribute) for attribute in payload.get("attributes", [])],
-            category=NamedResource.from_payload(payload.get("category", {}) or {}),
-            effect_entries=[VerboseEffect.from_payload(effect) for effect in payload.get("effect_entries", [])],
-            flavor_text_entries=[
-                VersionGroupFlavorText.from_payload(flavor_text)
-                for flavor_text in payload.get("flavor_text_entries", [])
-            ],
-            game_indices=[
-                GenerationGameIndex.from_payload(game_index) for game_index in payload.get("game_indices", [])
-            ],
-            names=[Name.from_payload(name) for name in payload.get("names", [])],
-            sprites=ItemSprites.from_payload(payload.get("sprites", {})),
-            held_by_pokemon=[
-                ItemHolderPokemon.from_payload(held_by_pokemon)
-                for held_by_pokemon in payload.get("held_by_pokemon", [])
-            ],
-            baby_trigger_for=NamedResource.from_payload(payload.get("baby_trigger_for", {}) or {}),
-            machines=[MachineVersionDetail.from_payload(machine) for machine in payload.get("machines", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class ItemAttribute(BaseModel):
-    """ItemAttribute model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    items: t.List[NamedResource]
-        A list of items that have this attribute.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    items: t.List[NamedResource] = attrs.field(factory=list)
-    names: t.List[Name] = attrs.field(factory=list)
-    descriptions: t.List[Description] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ItemAttribute":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            items=[NamedResource.from_payload(item) for item in payload.get("items", [])],
-            names=[Name.from_payload(name) for name in payload.get("names", [])],
-            descriptions=[Description.from_payload(description) for description in payload.get("descriptions", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class ItemCategory(BaseModel):
-    """ItemCategory model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    items: t.List[NamedResource]
-        A list of items that are a part of this category.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    items: t.List[NamedResource] = attrs.field(factory=list)
-    names: t.List[Name] = attrs.field(factory=list)
-    pocket: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ItemCategory":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            items=[NamedResource.from_payload(item) for item in payload.get("items", [])],
-            names=[Name.from_payload(name) for name in payload.get("names", [])],
-            pocket=NamedResource.from_payload(payload.get("pocket", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class ItemFlingEffect(BaseModel):
-    """ItemFlingEffect model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    effect_entries: t.List[Effect]
-        The result of this fling effect listed in different languages.
-    items: t.List[NamedResource]
-        A list of items that have this fling effect.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    effect_entries: t.List[Effect] = attrs.field(factory=list)
-    items: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ItemFlingEffect":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            effect_entries=[Effect.from_payload(effect) for effect in payload.get("effect_entries", [])],
-            items=[NamedResource.from_payload(item) for item in payload.get("items", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class ItemPocket(BaseModel):
-    """ItemPocket model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    categories: t.List[NamedResource]
-        A list of item categories that are relevant to this item pocket.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    categories: t.List[NamedResource] = attrs.field(factory=list)
-    names: t.List[Name] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ItemPocket":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            categories=[NamedResource.from_payload(category) for category in payload.get("categories", [])],
-            names=[Name.from_payload(name) for name in payload.get("names", [])],
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import (
+    Description,
+    Effect,
+    GenerationGameIndex,
+    MachineVersionDetail,
+    Name,
+    NamedResource,
+    VerboseEffect,
+    VersionGroupFlavorText,
+)
+
+from .utils import ItemHolderPokemon, ItemSprites
+
+__all__: t.Tuple[str, ...] = ("Item", "ItemAttribute", "ItemCategory", "ItemFlingEffect", "ItemPocket")
+
+
+@attrs.define(slots=True, kw_only=True)
+class Item(BaseModel):
+    """Item model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    cost: int
+        The price of this item in stores.
+    fling_power: int
+        The power of the move Fling when used with this item.
+    fling_effect: NamedResource
+        The effect of the move Fling when used with this item.
+    attributes: t.List[NamedResource]
+        A list of attributes this item has.
+    category: NamedResource
+        The category of items this item falls into.
+    effect_entries: t.List[Effect]
+        The effect of this ability listed in different languages.
+    flavor_text_entries: t.List[VersionGroupFlavorText]
+        The flavor text of this ability listed in different languages.
+    game_indices: t.List[GenerationGameIndex]
+        A list of game indices relevent to this item by generation.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    sprites: ItemSprites
+        A set of sprites used to depict this item in the game.
+    held_by_pokemon: t.List[ItemHolderPokemon]
+        A list of Pokémon that might be found in the wild holding this item.
+    baby_trigger_for: NamedResource
+        An evolution chain this item requires to produce a bay during mating.
+    machines: t.List[MachineVersionDetail]
+        A list of the machines related to this item.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    cost: int = attrs.field(factory=int)
+    fling_power: int = attrs.field(factory=int)
+    fling_effect: NamedResource = attrs.field(factory=NamedResource)
+    attributes: t.List[NamedResource] = attrs.field(factory=list)
+    category: NamedResource = attrs.field(factory=NamedResource)
+    effect_entries: t.List[VerboseEffect] = attrs.field(factory=list)
+    flavor_text_entries: t.List[VersionGroupFlavorText] = attrs.field(factory=list)
+    game_indices: t.List[GenerationGameIndex] = attrs.field(factory=list)
+    names: t.List[Name] = attrs.field(factory=list)
+    sprites: ItemSprites = attrs.field(factory=ItemSprites)
+    held_by_pokemon: t.List[ItemHolderPokemon] = attrs.field(factory=list)
+    baby_trigger_for: NamedResource = attrs.field(factory=NamedResource)
+    machines: t.List[MachineVersionDetail] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Item":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            cost=payload.get("cost", 0),
+            fling_power=payload.get("fling_power", 0),
+            fling_effect=NamedResource.from_payload(payload.get("fling_effect", {}) or {}),
+            attributes=[NamedResource.from_payload(attribute) for attribute in payload.get("attributes", [])],
+            category=NamedResource.from_payload(payload.get("category", {}) or {}),
+            effect_entries=[VerboseEffect.from_payload(effect) for effect in payload.get("effect_entries", [])],
+            flavor_text_entries=[
+                VersionGroupFlavorText.from_payload(flavor_text)
+                for flavor_text in payload.get("flavor_text_entries", [])
+            ],
+            game_indices=[
+                GenerationGameIndex.from_payload(game_index) for game_index in payload.get("game_indices", [])
+            ],
+            names=[Name.from_payload(name) for name in payload.get("names", [])],
+            sprites=ItemSprites.from_payload(payload.get("sprites", {}) or {}),
+            held_by_pokemon=[
+                ItemHolderPokemon.from_payload(held_by_pokemon)
+                for held_by_pokemon in payload.get("held_by_pokemon", [])
+            ],
+            baby_trigger_for=NamedResource.from_payload(payload.get("baby_trigger_for", {}) or {}),
+            machines=[MachineVersionDetail.from_payload(machine) for machine in payload.get("machines", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class ItemAttribute(BaseModel):
+    """ItemAttribute model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    items: t.List[NamedResource]
+        A list of items that have this attribute.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    items: t.List[NamedResource] = attrs.field(factory=list)
+    names: t.List[Name] = attrs.field(factory=list)
+    descriptions: t.List[Description] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ItemAttribute":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            items=[NamedResource.from_payload(item) for item in payload.get("items", [])],
+            names=[Name.from_payload(name) for name in payload.get("names", [])],
+            descriptions=[Description.from_payload(description) for description in payload.get("descriptions", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class ItemCategory(BaseModel):
+    """ItemCategory model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    items: t.List[NamedResource]
+        A list of items that are a part of this category.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    items: t.List[NamedResource] = attrs.field(factory=list)
+    names: t.List[Name] = attrs.field(factory=list)
+    pocket: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ItemCategory":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            items=[NamedResource.from_payload(item) for item in payload.get("items", [])],
+            names=[Name.from_payload(name) for name in payload.get("names", [])],
+            pocket=NamedResource.from_payload(payload.get("pocket", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class ItemFlingEffect(BaseModel):
+    """ItemFlingEffect model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    effect_entries: t.List[Effect]
+        The result of this fling effect listed in different languages.
+    items: t.List[NamedResource]
+        A list of items that have this fling effect.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    effect_entries: t.List[Effect] = attrs.field(factory=list)
+    items: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ItemFlingEffect":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            effect_entries=[Effect.from_payload(effect) for effect in payload.get("effect_entries", [])],
+            items=[NamedResource.from_payload(item) for item in payload.get("items", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class ItemPocket(BaseModel):
+    """ItemPocket model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    categories: t.List[NamedResource]
+        A list of item categories that are relevant to this item pocket.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    categories: t.List[NamedResource] = attrs.field(factory=list)
+    names: t.List[Name] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ItemPocket":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            categories=[NamedResource.from_payload(category) for category in payload.get("categories", [])],
+            names=[Name.from_payload(name) for name in payload.get("names", [])],
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/location.py` & `pokelance-0.1.0/pokelance/models/abstract/location.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import GenerationGameIndex, Name, NamedResource
-
-from .utils import EncounterMethodRate, PalParkEncounterSpecies, PokemonEncounter
-
-__all__: t.Tuple[str, ...] = (
-    "Location",
-    "LocationArea",
-    "PalParkArea",
-    "Region",
-)
-
-
-@attrs.define(slots=True, kw_only=True)
-class Location(BaseModel):
-    """Location model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    region: NamedResource
-        The region this location can be found in.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    game_indices: t.List[GenerationGameIndex]
-        A list of game indices relevent to this location by generation.
-    areas: t.List[NamedResource]
-        A list of methods in which Pokémon may be encountered in this
-        location.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    region: NamedResource = attrs.field(factory=NamedResource)
-    names: t.List[Name] = attrs.field(factory=list)
-    game_indices: t.List[GenerationGameIndex] = attrs.field(factory=list)
-    areas: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Location":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            region=NamedResource.from_payload(payload.get("region", {}) or {}),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            game_indices=[GenerationGameIndex.from_payload(i) for i in payload.get("game_indices", [])],
-            areas=[NamedResource.from_payload(i) for i in payload.get("areas", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class LocationArea(BaseModel):
-    """LocationArea model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    game_index: int
-        The internal id of an API resource within game data.
-    encounter_method_rates: t.List[EncounterMethodRate]
-        A list of methods in which Pokémon may be encountered in this
-        area and how likely the method will occur depending on the
-        version of the game.
-    location: NamedResource
-        The region this location can be found in.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    pokemon_encounters: t.List[PokemonEncounter]
-        A list of Pokémon that can be encountered in this area along
-        with version specific details about the encounter.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    game_index: int = attrs.field(factory=int)
-    names: t.List[Name] = attrs.field(factory=list)
-    location: NamedResource = attrs.field(factory=NamedResource)
-    encounter_method_rates: t.List[EncounterMethodRate] = attrs.field(factory=list)
-    pokemon_encounters: t.List[PokemonEncounter] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "LocationArea":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            game_index=payload.get("game_index", 0),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            location=NamedResource.from_payload(payload.get("location", {}) or {}),
-            encounter_method_rates=[
-                EncounterMethodRate.from_payload(i) for i in payload.get("encounter_method_rates", [])
-            ],
-            pokemon_encounters=[PokemonEncounter.from_payload(i) for i in payload.get("pokemon_encounters", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PalParkArea(BaseModel):
-    """PalParkArea model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    pokemon_encounters: t.List[PalParkEncounterSpecies]
-        A list of Pokémon encountered in this pal park area along with
-        details.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    names: t.List[Name] = attrs.field(factory=list)
-    pokemon_encounters: t.List[PalParkEncounterSpecies] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PalParkArea":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            pokemon_encounters=[PalParkEncounterSpecies.from_payload(i) for i in payload.get("pokemon_encounters", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Region(BaseModel):
-    """Region model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    locations: t.List[NamedResource]
-        A list of locations that can be found in this region.
-    main_generation: NamedResource
-        The generation this region was introduced in.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    pokedexes: t.List[NamedResource]
-        A list of pokédexes that catalogue Pokémon in this region.
-    version_groups: t.List[NamedResource]
-        A list of version groups where this region can be visited.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    locations: t.List[NamedResource] = attrs.field(factory=list)
-    main_generation: NamedResource = attrs.field(factory=NamedResource)
-    names: t.List[Name] = attrs.field(factory=list)
-    pokedexes: t.List[NamedResource] = attrs.field(factory=list)
-    version_groups: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Region":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            locations=[NamedResource.from_payload(i) for i in payload.get("locations", [])],
-            main_generation=NamedResource.from_payload(payload.get("main_generation", {}) or {}),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            pokedexes=[NamedResource.from_payload(i) for i in payload.get("pokedexes", [])],
-            version_groups=[NamedResource.from_payload(i) for i in payload.get("version_groups", [])],
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import GenerationGameIndex, Name, NamedResource
+
+from .utils import EncounterMethodRate, PalParkEncounterSpecies, PokemonEncounter
+
+__all__: t.Tuple[str, ...] = (
+    "Location",
+    "LocationArea",
+    "PalParkArea",
+    "Region",
+)
+
+
+@attrs.define(slots=True, kw_only=True)
+class Location(BaseModel):
+    """Location model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    region: NamedResource
+        The region this location can be found in.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    game_indices: t.List[GenerationGameIndex]
+        A list of game indices relevent to this location by generation.
+    areas: t.List[NamedResource]
+        A list of methods in which Pokémon may be encountered in this
+        location.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    region: NamedResource = attrs.field(factory=NamedResource)
+    names: t.List[Name] = attrs.field(factory=list)
+    game_indices: t.List[GenerationGameIndex] = attrs.field(factory=list)
+    areas: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Location":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            region=NamedResource.from_payload(payload.get("region", {}) or {}),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            game_indices=[GenerationGameIndex.from_payload(i) for i in payload.get("game_indices", [])],
+            areas=[NamedResource.from_payload(i) for i in payload.get("areas", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class LocationArea(BaseModel):
+    """LocationArea model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    game_index: int
+        The internal id of an API resource within game data.
+    encounter_method_rates: t.List[EncounterMethodRate]
+        A list of methods in which Pokémon may be encountered in this
+        area and how likely the method will occur depending on the
+        version of the game.
+    location: NamedResource
+        The region this location can be found in.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    pokemon_encounters: t.List[PokemonEncounter]
+        A list of Pokémon that can be encountered in this area along
+        with version specific details about the encounter.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    game_index: int = attrs.field(factory=int)
+    names: t.List[Name] = attrs.field(factory=list)
+    location: NamedResource = attrs.field(factory=NamedResource)
+    encounter_method_rates: t.List[EncounterMethodRate] = attrs.field(factory=list)
+    pokemon_encounters: t.List[PokemonEncounter] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "LocationArea":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            game_index=payload.get("game_index", 0),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            location=NamedResource.from_payload(payload.get("location", {}) or {}),
+            encounter_method_rates=[
+                EncounterMethodRate.from_payload(i) for i in payload.get("encounter_method_rates", [])
+            ],
+            pokemon_encounters=[PokemonEncounter.from_payload(i) for i in payload.get("pokemon_encounters", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PalParkArea(BaseModel):
+    """PalParkArea model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    pokemon_encounters: t.List[PalParkEncounterSpecies]
+        A list of Pokémon encountered in this pal park area along with
+        details.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    names: t.List[Name] = attrs.field(factory=list)
+    pokemon_encounters: t.List[PalParkEncounterSpecies] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PalParkArea":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            pokemon_encounters=[PalParkEncounterSpecies.from_payload(i) for i in payload.get("pokemon_encounters", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Region(BaseModel):
+    """Region model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    locations: t.List[NamedResource]
+        A list of locations that can be found in this region.
+    main_generation: NamedResource
+        The generation this region was introduced in.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    pokedexes: t.List[NamedResource]
+        A list of pokédexes that catalogue Pokémon in this region.
+    version_groups: t.List[NamedResource]
+        A list of version groups where this region can be visited.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    locations: t.List[NamedResource] = attrs.field(factory=list)
+    main_generation: NamedResource = attrs.field(factory=NamedResource)
+    names: t.List[Name] = attrs.field(factory=list)
+    pokedexes: t.List[NamedResource] = attrs.field(factory=list)
+    version_groups: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Region":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            locations=[NamedResource.from_payload(i) for i in payload.get("locations", [])],
+            main_generation=NamedResource.from_payload(payload.get("main_generation", {}) or {}),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            pokedexes=[NamedResource.from_payload(i) for i in payload.get("pokedexes", [])],
+            version_groups=[NamedResource.from_payload(i) for i in payload.get("version_groups", [])],
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/move.py` & `pokelance-0.1.0/pokelance/models/abstract/move.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,318 +1,318 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import Description, MachineVersionDetail, Name, NamedResource, Resource, VerboseEffect
-
-from .utils import (
-    AbilityEffectChange,
-    ContestComboSet,
-    MoveFlavorText,
-    MoveMetaData,
-    MoveStatChange,
-    PastMoveStatValues,
-)
-
-__all__: t.Tuple[str, ...] = (
-    "Move",
-    "MoveAilment",
-    "MoveBattleStyle",
-    "MoveCategory",
-    "MoveDamageClass",
-    "MoveLearnMethod",
-    "MoveTarget",
-)
-
-
-@attrs.define(slots=True, kw_only=True)
-class Move(BaseModel):
-    """Move model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    accuracy: int
-        The percent value of how likely this move is to be successful.
-    effect_chance: int
-        The percent value of how likely it is this moves effect will take effect.
-    pp: int
-        Power points. The number of times this move can be used.
-    priority: int
-        A value between -8 and 8. Sets the order in which moves
-        are executed during battle. See Bulbapedia for greater detail.
-    power: int
-        The base power of this move with a value of 0 if it does not have a base power.
-    contest_combos: ContestComboSet
-        A detail of normal and super contest combos that require this move.
-    contest_type: NamedResource
-        The type of appeal this move gives a Pokémon when used in a contest.
-    contest_effect: Resource
-        The effect the move has when used in a contest.
-    damage_class: NamedResource
-        The type of damage the move inflicts on the target, e.g. physical.
-    effect_entries: t.List[VerboseEffect]
-        The effect of this move listed in different languages.
-    effect_changes: t.List[AbilityEffectChange]
-        The list of previous effects this move has had across version groups of the games.
-    flavor_text_entries: t.List[MoveFlavorText]
-        The flavor text of this move listed in different languages.
-    generation: NamedResource
-        The generation in which this move was introduced.
-    machines: t.List[MachineVersionDetail]
-        A list of the machines that teach this move.
-    meta: MoveMetaData
-        Metadata about this move.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    past_values: t.List[PastMoveStatValues]
-        A list of move resource value changes across version groups of the games.
-    stat_changes: t.List[MoveStatChange]
-        A list of stats this moves effects and how much it effects them.
-    super_contest_effect: Resource
-        The effect the move has when used in a super contest.
-    target: NamedResource
-        The type of target that will receive the effects of the attack.
-    type: NamedResource
-        The elemental type of this move.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    accuracy: int = attrs.field(factory=int)
-    effect_chance: int = attrs.field(factory=int)
-    pp: int = attrs.field(factory=int)
-    priority: int = attrs.field(factory=int)
-    power: int = attrs.field(factory=int)
-    contest_combos: ContestComboSet = attrs.field(factory=ContestComboSet)
-    contest_type: NamedResource = attrs.field(factory=NamedResource)
-    contest_effect: Resource = attrs.field(factory=Resource)
-    damage_class: NamedResource = attrs.field(factory=NamedResource)
-    effect_entries: t.List[VerboseEffect] = attrs.field(factory=list)
-    effect_changes: t.List[AbilityEffectChange] = attrs.field(factory=list)
-    learned_by_pokemon: t.List[NamedResource] = attrs.field(factory=list)
-    flavor_text_entries: t.List[MoveFlavorText] = attrs.field(factory=list)
-    generation: NamedResource = attrs.field(factory=NamedResource)
-    machines: t.List[MachineVersionDetail] = attrs.field(factory=list)
-    meta: MoveMetaData = attrs.field(factory=MoveMetaData)
-    names: t.List[Name] = attrs.field(factory=list)
-    past_values: t.List[PastMoveStatValues] = attrs.field(factory=list)
-    stat_changes: t.List[MoveStatChange] = attrs.field(factory=list)
-    super_contest_effect: Resource = attrs.field(factory=Resource)
-    target: NamedResource = attrs.field(factory=NamedResource)
-    type: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Move":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            accuracy=payload.get("accuracy", 0),
-            effect_chance=payload.get("effect_chance", 0),
-            pp=payload.get("pp", 0),
-            priority=payload.get("priority", 0),
-            power=payload.get("power", 0),
-            contest_combos=ContestComboSet.from_payload(payload.get("contest_combos", {})),
-            contest_type=NamedResource.from_payload(payload.get("contest_type", {}) or {}),
-            contest_effect=Resource.from_payload(payload.get("contest_effect", {}) or {}),
-            damage_class=NamedResource.from_payload(payload.get("damage_class", {}) or {}),
-            effect_entries=[VerboseEffect.from_payload(i) for i in payload.get("effect_entries", [])],
-            effect_changes=[AbilityEffectChange.from_payload(i) for i in payload.get("effect_changes", [])],
-            learned_by_pokemon=[NamedResource.from_payload(i) for i in payload.get("learned_by_pokemon", [])],
-            flavor_text_entries=[MoveFlavorText.from_payload(i) for i in payload.get("flavor_text_entries", [])],
-            generation=NamedResource.from_payload(payload.get("generation", {}) or {}),
-            machines=[MachineVersionDetail.from_payload(i) for i in payload.get("machines", [])],
-            meta=MoveMetaData.from_payload(payload.get("meta", {})),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            past_values=[PastMoveStatValues.from_payload(i) for i in payload.get("past_values", [])],
-            stat_changes=[MoveStatChange.from_payload(i) for i in payload.get("stat_changes", [])],
-            super_contest_effect=Resource.from_payload(payload.get("super_contest_effect", {}) or {}),
-            target=NamedResource.from_payload(payload.get("target", {}) or {}),
-            type=NamedResource.from_payload(payload.get("type", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class MoveAilment(BaseModel):
-    """
-    MoveAilment models the data returned by the API for a move ailment.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    moves: t.List[NamedResource]
-        A list of moves that cause this ailment.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    moves: t.List[NamedResource] = attrs.field(factory=list)
-    names: t.List[Name] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveAilment":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            moves=[NamedResource.from_payload(i) for i in payload.get("moves", [])],
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class MoveBattleStyle(BaseModel):
-    """
-    MoveBattleStyle models the data returned by the API for a move battle style.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    names: t.List[Name] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveBattleStyle":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class MoveCategory(BaseModel):
-    """
-    MoveCategory models the data returned by the API for a move category.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    moves: t.List[NamedResource]
-        A list of moves that fall into this category.
-    descriptions: t.List[Description]
-        The description of this resource listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    moves: t.List[NamedResource] = attrs.field(factory=list)
-    descriptions: t.List[Description] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveCategory":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            moves=[NamedResource.from_payload(i) for i in payload.get("moves", [])],
-            descriptions=[Description.from_payload(i) for i in payload.get("descriptions", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class MoveDamageClass(BaseModel):
-    """
-    MoveDamageClass models the data returned by the API for a move damage class.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    descriptions: t.List[Description]
-        The description of this resource listed in different languages.
-    moves: t.List[NamedResource]
-        A list of moves that fall into this damage class.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    descriptions: t.List[Description] = attrs.field(factory=list)
-    moves: t.List[NamedResource] = attrs.field(factory=list)
-    names: t.List[Name] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveDamageClass":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            descriptions=[Description.from_payload(i) for i in payload.get("descriptions", [])],
-            moves=[NamedResource.from_payload(i) for i in payload.get("moves", [])],
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class MoveLearnMethod(BaseModel):
-    """
-    MoveLearnMethod models the data returned by the API for a move learn method.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    descriptions: t.List[Description]
-        The description of this resource listed in different languages.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    version_groups: t.List[NamedResource]
-        A list of version groups where moves can be learned through this method.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    descriptions: t.List[Description] = attrs.field(factory=list)
-    names: t.List[Name] = attrs.field(factory=list)
-    version_groups: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveLearnMethod":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            descriptions=[Description.from_payload(i) for i in payload.get("descriptions", [])],
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            version_groups=[NamedResource.from_payload(i) for i in payload.get("version_groups", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class MoveTarget(BaseModel):
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    descriptions: t.List[Description] = attrs.field(factory=list)
-    moves: t.List[NamedResource] = attrs.field(factory=list)
-    names: t.List[Name] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveTarget":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            descriptions=[Description.from_payload(i) for i in payload.get("descriptions", [])],
-            moves=[NamedResource.from_payload(i) for i in payload.get("moves", [])],
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import Description, MachineVersionDetail, Name, NamedResource, Resource, VerboseEffect
+
+from .utils import (
+    AbilityEffectChange,
+    ContestComboSet,
+    MoveFlavorText,
+    MoveMetaData,
+    MoveStatChange,
+    PastMoveStatValues,
+)
+
+__all__: t.Tuple[str, ...] = (
+    "Move",
+    "MoveAilment",
+    "MoveBattleStyle",
+    "MoveCategory",
+    "MoveDamageClass",
+    "MoveLearnMethod",
+    "MoveTarget",
+)
+
+
+@attrs.define(slots=True, kw_only=True)
+class Move(BaseModel):
+    """Move model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    accuracy: int
+        The percent value of how likely this move is to be successful.
+    effect_chance: int
+        The percent value of how likely it is this moves effect will take effect.
+    pp: int
+        Power points. The number of times this move can be used.
+    priority: int
+        A value between -8 and 8. Sets the order in which moves
+        are executed during battle. See Bulbapedia for greater detail.
+    power: int
+        The base power of this move with a value of 0 if it does not have a base power.
+    contest_combos: ContestComboSet
+        A detail of normal and super contest combos that require this move.
+    contest_type: NamedResource
+        The type of appeal this move gives a Pokémon when used in a contest.
+    contest_effect: Resource
+        The effect the move has when used in a contest.
+    damage_class: NamedResource
+        The type of damage the move inflicts on the target, e.g. physical.
+    effect_entries: t.List[VerboseEffect]
+        The effect of this move listed in different languages.
+    effect_changes: t.List[AbilityEffectChange]
+        The list of previous effects this move has had across version groups of the games.
+    flavor_text_entries: t.List[MoveFlavorText]
+        The flavor text of this move listed in different languages.
+    generation: NamedResource
+        The generation in which this move was introduced.
+    machines: t.List[MachineVersionDetail]
+        A list of the machines that teach this move.
+    meta: MoveMetaData
+        Metadata about this move.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    past_values: t.List[PastMoveStatValues]
+        A list of move resource value changes across version groups of the games.
+    stat_changes: t.List[MoveStatChange]
+        A list of stats this moves effects and how much it effects them.
+    super_contest_effect: Resource
+        The effect the move has when used in a super contest.
+    target: NamedResource
+        The type of target that will receive the effects of the attack.
+    type: NamedResource
+        The elemental type of this move.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    accuracy: int = attrs.field(factory=int)
+    effect_chance: int = attrs.field(factory=int)
+    pp: int = attrs.field(factory=int)
+    priority: int = attrs.field(factory=int)
+    power: int = attrs.field(factory=int)
+    contest_combos: ContestComboSet = attrs.field(factory=ContestComboSet)
+    contest_type: NamedResource = attrs.field(factory=NamedResource)
+    contest_effect: Resource = attrs.field(factory=Resource)
+    damage_class: NamedResource = attrs.field(factory=NamedResource)
+    effect_entries: t.List[VerboseEffect] = attrs.field(factory=list)
+    effect_changes: t.List[AbilityEffectChange] = attrs.field(factory=list)
+    learned_by_pokemon: t.List[NamedResource] = attrs.field(factory=list)
+    flavor_text_entries: t.List[MoveFlavorText] = attrs.field(factory=list)
+    generation: NamedResource = attrs.field(factory=NamedResource)
+    machines: t.List[MachineVersionDetail] = attrs.field(factory=list)
+    meta: MoveMetaData = attrs.field(factory=MoveMetaData)
+    names: t.List[Name] = attrs.field(factory=list)
+    past_values: t.List[PastMoveStatValues] = attrs.field(factory=list)
+    stat_changes: t.List[MoveStatChange] = attrs.field(factory=list)
+    super_contest_effect: Resource = attrs.field(factory=Resource)
+    target: NamedResource = attrs.field(factory=NamedResource)
+    type: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Move":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            accuracy=payload.get("accuracy", 0),
+            effect_chance=payload.get("effect_chance", 0),
+            pp=payload.get("pp", 0),
+            priority=payload.get("priority", 0),
+            power=payload.get("power", 0),
+            contest_combos=ContestComboSet.from_payload(payload.get("contest_combos", {}) or {}),
+            contest_type=NamedResource.from_payload(payload.get("contest_type", {}) or {}),
+            contest_effect=Resource.from_payload(payload.get("contest_effect", {}) or {}),
+            damage_class=NamedResource.from_payload(payload.get("damage_class", {}) or {}),
+            effect_entries=[VerboseEffect.from_payload(i) for i in payload.get("effect_entries", [])],
+            effect_changes=[AbilityEffectChange.from_payload(i) for i in payload.get("effect_changes", [])],
+            learned_by_pokemon=[NamedResource.from_payload(i) for i in payload.get("learned_by_pokemon", [])],
+            flavor_text_entries=[MoveFlavorText.from_payload(i) for i in payload.get("flavor_text_entries", [])],
+            generation=NamedResource.from_payload(payload.get("generation", {}) or {}),
+            machines=[MachineVersionDetail.from_payload(i) for i in payload.get("machines", [])],
+            meta=MoveMetaData.from_payload(payload.get("meta", {}) or {}),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            past_values=[PastMoveStatValues.from_payload(i) for i in payload.get("past_values", [])],
+            stat_changes=[MoveStatChange.from_payload(i) for i in payload.get("stat_changes", [])],
+            super_contest_effect=Resource.from_payload(payload.get("super_contest_effect", {}) or {}),
+            target=NamedResource.from_payload(payload.get("target", {}) or {}),
+            type=NamedResource.from_payload(payload.get("type", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class MoveAilment(BaseModel):
+    """
+    MoveAilment models the data returned by the API for a move ailment.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    moves: t.List[NamedResource]
+        A list of moves that cause this ailment.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    moves: t.List[NamedResource] = attrs.field(factory=list)
+    names: t.List[Name] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveAilment":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            moves=[NamedResource.from_payload(i) for i in payload.get("moves", [])],
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class MoveBattleStyle(BaseModel):
+    """
+    MoveBattleStyle models the data returned by the API for a move battle style.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    names: t.List[Name] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveBattleStyle":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class MoveCategory(BaseModel):
+    """
+    MoveCategory models the data returned by the API for a move category.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    moves: t.List[NamedResource]
+        A list of moves that fall into this category.
+    descriptions: t.List[Description]
+        The description of this resource listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    moves: t.List[NamedResource] = attrs.field(factory=list)
+    descriptions: t.List[Description] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveCategory":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            moves=[NamedResource.from_payload(i) for i in payload.get("moves", [])],
+            descriptions=[Description.from_payload(i) for i in payload.get("descriptions", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class MoveDamageClass(BaseModel):
+    """
+    MoveDamageClass models the data returned by the API for a move damage class.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    descriptions: t.List[Description]
+        The description of this resource listed in different languages.
+    moves: t.List[NamedResource]
+        A list of moves that fall into this damage class.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    descriptions: t.List[Description] = attrs.field(factory=list)
+    moves: t.List[NamedResource] = attrs.field(factory=list)
+    names: t.List[Name] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveDamageClass":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            descriptions=[Description.from_payload(i) for i in payload.get("descriptions", [])],
+            moves=[NamedResource.from_payload(i) for i in payload.get("moves", [])],
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class MoveLearnMethod(BaseModel):
+    """
+    MoveLearnMethod models the data returned by the API for a move learn method.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    descriptions: t.List[Description]
+        The description of this resource listed in different languages.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    version_groups: t.List[NamedResource]
+        A list of version groups where moves can be learned through this method.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    descriptions: t.List[Description] = attrs.field(factory=list)
+    names: t.List[Name] = attrs.field(factory=list)
+    version_groups: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveLearnMethod":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            descriptions=[Description.from_payload(i) for i in payload.get("descriptions", [])],
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            version_groups=[NamedResource.from_payload(i) for i in payload.get("version_groups", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class MoveTarget(BaseModel):
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    descriptions: t.List[Description] = attrs.field(factory=list)
+    moves: t.List[NamedResource] = attrs.field(factory=list)
+    names: t.List[Name] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveTarget":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            descriptions=[Description.from_payload(i) for i in payload.get("descriptions", [])],
+            moves=[NamedResource.from_payload(i) for i in payload.get("moves", [])],
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/pokemon.py` & `pokelance-0.1.0/pokelance/models/abstract/pokemon.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,840 +1,840 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import (
-    Description,
-    FlavorText,
-    GenerationGameIndex,
-    Name,
-    NamedResource,
-    Resource,
-    VerboseEffect,
-    VersionEncounterDetail,
-    VersionGameIndex,
-)
-
-from .showdown import ShowdownSprites
-from .utils import (
-    AbilityEffectChange,
-    AbilityFlavorText,
-    AbilityPokemon,
-    AwesomeName,
-    Genus,
-    GrowthRateExperienceLevel,
-    MoveBattleStylePreference,
-    MoveStatAffectSets,
-    NaturePokeathlonStatAffectSet,
-    NatureStatAffectSets,
-    NatureStatChange,
-    PalParkEncounterArea,
-    PokemonAbility,
-    PokemonFormSprites,
-    PokemonHeldItem,
-    PokemonMove,
-    PokemonSpeciesDexEntry,
-    PokemonSpeciesGender,
-    PokemonSpeciesVariety,
-    PokemonSprite,
-    PokemonStat,
-    PokemonType,
-    PokemonTypePast,
-    TypePokemon,
-    TypeRelations,
-)
-
-__all__: t.Tuple[str, ...] = (
-    "Ability",
-    "Characteristic",
-    "Pokemon",
-    "PokemonSpecies",
-    "PokemonForm",
-    "Nature",
-    "Type",
-    "Gender",
-    "GrowthRate",
-    "EggGroup",
-    "LocationAreaEncounter",
-    "PokemonColor",
-    "PokeathlonStat",
-    "PokemonHabitats",
-    "PokemonShape",
-    "Stat",
-)
-
-
-@attrs.define(slots=True, kw_only=True)
-class Ability(BaseModel):
-    """Ability model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this ability resource.
-    name: str
-        The name for this ability resource.
-    is_main_series: bool
-        Whether or not this ability originated in the main series of the video games.
-    generation: NamedResource
-        The generation this ability originated in.
-    names: t.List[Name]
-        The name of this ability listed in different languages.
-    effect_entries: t.List[VerboseEffect]
-        The effect of this ability listed in different languages.
-    effect_changes: t.List[AbilityEffectChange]
-        The list of previous effects this ability has had across version groups of the games.
-    flavor_text_entries: t.List[AbilityFlavorText]
-        The flavor text of this ability listed in different languages.
-    pokemon: t.List[AbilityPokemon]
-        A list of Pokémon that could potentially have this ability.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    is_main_series: bool = attrs.field(factory=bool)
-    generation: NamedResource = attrs.field(factory=NamedResource)
-    names: t.List[Name] = attrs.field(factory=list)
-    effect_entries: t.List[VerboseEffect] = attrs.field(factory=list)
-    effect_changes: t.List[AbilityEffectChange] = attrs.field(factory=list)
-    flavor_text_entries: t.List[AbilityFlavorText] = attrs.field(factory=list)
-    pokemon: t.List[AbilityPokemon] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Ability":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            is_main_series=payload.get("is_main_series", False),
-            generation=NamedResource.from_payload(payload.get("generation", {}) or {}),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            effect_entries=[VerboseEffect.from_payload(i) for i in payload.get("effect_entries", [])],
-            effect_changes=[AbilityEffectChange.from_payload(i) for i in payload.get("effect_changes", [])],
-            flavor_text_entries=[AbilityFlavorText.from_payload(i) for i in payload.get("flavor_text_entries", [])],
-            pokemon=[AbilityPokemon.from_payload(i) for i in payload.get("pokemon", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Characteristic(BaseModel):
-    """Characteristic model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this characteristic resource.
-    gene_modulo: int
-        The remainder of the highest stat/IV divided by 5.
-    possible_values: t.List[int]
-        The possible values of the highest stat that would result in a Pokémon
-         recieving this characteristic when divided by 5.
-
-    """
-
-    id: int = attrs.field(factory=int)
-    gene_modulo: int = attrs.field(factory=int)
-    possible_values: t.List[int] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Characteristic":
-        return cls(
-            id=payload.get("id", 0),
-            gene_modulo=payload.get("gene_modulo", 0),
-            possible_values=payload.get("possible_values", []),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class EggGroup(BaseModel):
-    """EggGroup model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this egg group resource.
-    name: str
-        The name for this egg group resource.
-    names: t.List[Name]
-        The name of this egg group listed in different languages.
-    pokemon_species: t.List[NamedResource]
-        A list of all Pokémon species that are members of this egg group.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    names: t.List[Name] = attrs.field(factory=list)
-    pokemon_species: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EggGroup":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            pokemon_species=[NamedResource.from_payload(i) for i in payload.get("pokemon_species", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Gender(BaseModel):
-    """Gender model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for gender resource.
-    name: str
-        The name for this gender resource.
-    pokemon_species_details: t.List[PokemonSpeciesGender]
-        A list of Pokémon species that belong to this gender.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    pokemon_species_details: t.List[PokemonSpeciesGender] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Gender":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            pokemon_species_details=[
-                PokemonSpeciesGender.from_payload(i) for i in payload.get("pokemon_species_details", [])
-            ],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class GrowthRate(BaseModel):
-    """GrowthRate model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this growth rate resource.
-    name: str
-        The name for this growth rate resource.
-    formula: str
-        The formula used to calculate the rate at which the Pokémon species gains level.
-    descriptions: t.List[Description]
-        The descriptions of this characteristic listed in different languages.
-    levels: t.List[GrowthRateExperienceLevel]
-        A list of levels and the amount of experienced needed to atain them based on this growth rate.
-    pokemon_species: t.List[NamedResource]
-        A list of Pokémon species that gain levels at this growth rate.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    formula: str = attrs.field(factory=str)
-    descriptions: t.List[Description] = attrs.field(factory=list)
-    levels: t.List[GrowthRateExperienceLevel] = attrs.field(factory=list)
-    pokemon_species: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GrowthRate":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            formula=payload.get("formula", ""),
-            descriptions=[Description.from_payload(i) for i in payload.get("descriptions", [])],
-            levels=[GrowthRateExperienceLevel.from_payload(i) for i in payload.get("levels", [])],
-            pokemon_species=[NamedResource.from_payload(i) for i in payload.get("pokemon_species", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Nature(BaseModel):
-    """Nature model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this nature resource.
-    name: str
-        The name for this nature resource.
-    decreased_stat: NamedAPIResource
-        The stat decreased by 10% in Pokémon with this nature.
-    increased_stat: NamedAPIResource
-        The stat increased by 10% in Pokémon with this nature.
-    hates_flavor: NamedAPIResource
-        The flavor hated by Pokémon with this nature.
-    likes_flavor: NamedAPIResource
-        The flavor liked by Pokémon with this nature.
-    pokeathlon_stat_changes: t.List[NatureStatChange]
-        A list of Pokéathlon stats this nature effects and how much it effects them.
-    move_battle_style_preferences: t.List[MoveBattleStylePreference]
-        A list of battle styles and how likely a Pokémon with this nature
-        is to use them in the Battle Palace or Battle Tent.
-    names: t.List[Name]
-        The name of this nature listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    decreased_stat: NamedResource = attrs.field(factory=NamedResource)
-    increased_stat: NamedResource = attrs.field(factory=NamedResource)
-    hates_flavor: NamedResource = attrs.field(factory=NamedResource)
-    likes_flavor: NamedResource = attrs.field(factory=NamedResource)
-    pokeathlon_stat_changes: t.List[NatureStatChange] = attrs.field(factory=list)
-    move_battle_style_preferences: t.List[MoveBattleStylePreference] = attrs.field(factory=list)
-    names: t.List[Name] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Nature":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            decreased_stat=NamedResource.from_payload(payload.get("decreased_stat", {}) or {}),
-            increased_stat=NamedResource.from_payload(payload.get("increased_stat", {}) or {}),
-            hates_flavor=NamedResource.from_payload(payload.get("hates_flavor", {}) or {}),
-            likes_flavor=NamedResource.from_payload(payload.get("likes_flavor", {}) or {}),
-            pokeathlon_stat_changes=[
-                NatureStatChange.from_payload(i) for i in payload.get("pokeathlon_stat_changes", [])
-            ],
-            move_battle_style_preferences=[
-                MoveBattleStylePreference.from_payload(i) for i in payload.get("move_battle_style_preferences", [])
-            ],
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokeathlonStat(BaseModel):
-    """PokeathlonStat model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    names: t.List[Name]
-        A list of natures which affect this Pokéathlon stat positively or negatively.
-    affecting_natures: NaturePokeathlonStatAffectSets
-        A detail of natures which affect this Pokéathlon stat positively or negatively.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    names: t.List[Name] = attrs.field(factory=list)
-    affecting_natures: NaturePokeathlonStatAffectSet = attrs.field(factory=NaturePokeathlonStatAffectSet)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokeathlonStat":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            affecting_natures=NaturePokeathlonStatAffectSet.from_payload(payload.get("affecting_natures", {})),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Pokemon(BaseModel):
-    """Pokemon model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this Pokémon resource.
-    name: str
-        The name for this Pokémon resource.
-    base_experience: int
-        The base experience gained for defeating this Pokémon.
-    height: int
-        The height of this Pokémon in decimetres.
-    is_default: bool
-        Set for exactly one Pokémon used as the default for each species.
-    order: int
-        Order for sorting. Almost national order, except families are grouped together.
-    weight: int
-        The weight of this Pokémon in hectograms.
-    abilities: t.List[PokemonAbility]
-        A list of abilities this Pokémon could potentially have.
-    forms: t.List[NamedAPIResource]
-        A list of forms this Pokémon can take on.
-    game_indices: t.List[VersionGameIndex]
-        A list of game indices relevent to Pokémon item by generation.
-    held_items: t.List[PokemonHeldItem]
-        A list of items this Pokémon may be holding when encountered.
-    location_area_encounters: str
-        Location area encounter details for different versions.
-    moves: t.List[PokemonMove]
-        A list of details showing types this Pokémon has.
-    species: NamedAPIResource
-        The species this Pokémon belongs to.
-    sprites: PokemonSprites
-        A set of sprites used to depict this Pokémon in the game.
-    stats: t.List[PokemonStat]
-        A list of details showing all the stats this Pokémon has.
-    types: t.List[PokemonType]
-        A list of details showing types this Pokémon has.
-    showdown: ShowdownSprites
-        A set of sprites used to depict this Pokémon in the Showdown client.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    base_experience: int = attrs.field(factory=int)
-    height: int = attrs.field(factory=int)
-    is_default: bool = attrs.field(factory=bool)
-    order: int = attrs.field(factory=int)
-    weight: int = attrs.field(factory=int)
-    abilities: t.List[PokemonAbility] = attrs.field(factory=list)
-    forms: t.List[NamedResource] = attrs.field(factory=list)
-    game_indices: t.List[VersionGameIndex] = attrs.field(factory=list)
-    held_items: t.List[PokemonHeldItem] = attrs.field(factory=list)
-    location_area_encounters: str = attrs.field(factory=str)
-    moves: t.List[PokemonMove] = attrs.field(factory=list)
-    past_types: t.List[PokemonTypePast] = attrs.field(factory=list)
-    sprites: PokemonSprite = attrs.field(factory=PokemonSprite)
-    species: NamedResource = attrs.field(factory=NamedResource)
-    stats: t.List[PokemonStat] = attrs.field(factory=list)
-    types: t.List[PokemonType] = attrs.field(factory=list)
-    showdown: ShowdownSprites = attrs.field(factory=ShowdownSprites)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Pokemon":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            base_experience=payload.get("base_experience", 0),
-            height=payload.get("height", 0),
-            is_default=payload.get("is_default", False),
-            order=payload.get("order", 0),
-            weight=payload.get("weight", 0),
-            abilities=[PokemonAbility.from_payload(i) for i in payload.get("abilities", [])],
-            forms=[NamedResource.from_payload(i) for i in payload.get("forms", [])],
-            game_indices=[VersionGameIndex.from_payload(i) for i in payload.get("game_indices", [])],
-            held_items=[PokemonHeldItem.from_payload(i) for i in payload.get("held_items", [])],
-            location_area_encounters=payload.get("location_area_encounters", ""),
-            moves=[PokemonMove.from_payload(i) for i in payload.get("moves", [])],
-            past_types=[PokemonTypePast.from_payload(i) for i in payload.get("past_types", [])],
-            sprites=PokemonSprite.from_payload(payload.get("sprites", {}) or {}),
-            species=NamedResource.from_payload(payload.get("species", {}) or {}),
-            stats=[PokemonStat.from_payload(i) for i in payload.get("stats", [])],
-            types=[PokemonType.from_payload(i) for i in payload.get("types", [])],
-            showdown=ShowdownSprites.from_name(payload.get("name", "")),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class LocationAreaEncounter(BaseModel):
-    """LocationAreaEncounter model.
-
-    Attributes
-    ----------
-    location_area: NamedAPIResource
-        The location area the referenced Pokémon can be encountered in.
-    version_details: t.List[VersionEncounterDetail]
-        A list of versions and encounters with the referenced Pokémon that might happen.
-    """
-
-    location_area: NamedResource = attrs.field(factory=NamedResource)
-    version_details: t.List[VersionEncounterDetail] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "LocationAreaEncounter":
-        return cls(
-            location_area=NamedResource.from_payload(payload.get("location_area", {}) or {}),
-            version_details=[VersionEncounterDetail.from_payload(i) for i in payload.get("version_details", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonColor(BaseModel):
-    """PokemonColor model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this Pokémon color resource.
-    name: str
-        The name for this Pokémon color resource.
-    names: t.List[Name]
-        The name of this Pokémon color listed in different languages.
-    pokemon_species: t.List[NamedAPIResource]
-        A list of the Pokémon species that have this color.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    names: t.List[Name] = attrs.field(factory=list)
-    pokemon_species: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonColor":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            pokemon_species=[NamedResource.from_payload(i) for i in payload.get("pokemon_species", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonForm(BaseModel):
-    """PokemonForm model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this Pokémon form resource.
-    name: str
-        The name for this Pokémon form resource.
-    order: int
-        The order in which forms should be sorted within all forms. Multiple forms may have equal order,
-        in which case they should fall back on sorting by name.
-    form_order: int
-        The order in which forms should be sorted within a species' forms.
-    is_default: bool
-        True for exactly one form used as the default for each Pokémon.
-    is_battle_only: bool
-        Whether or not this form can only happen during battle.
-    is_mega: bool
-        Whether or not this form requires mega evolution.
-    form_name: str
-        The name of this form.
-    pokemon: NamedAPIResource
-        The Pokémon that can take on this form.
-    sprites: PokemonFormSprites
-        A set of sprites used to depict this Pokémon form in the game.
-    version_group: NamedAPIResource
-        The version group this Pokémon form was introduced in.
-    names: t.List[Name]
-        The form specific full name of this Pokémon form, or empty if the form does not have a specific name.
-    form_names: t.List[Name]
-        The form specific form name of this Pokémon form, or empty if the form does not have a specific name.
-    pokemon_species: NamedAPIResource
-        The Pokémon species that this form belongs to.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    order: int = attrs.field(factory=int)
-    form_order: int = attrs.field(factory=int)
-    is_default: bool = attrs.field(factory=bool)
-    is_battle_only: bool = attrs.field(factory=bool)
-    is_mega: bool = attrs.field(factory=bool)
-    form_name: str = attrs.field(factory=str)
-    pokemon: NamedResource = attrs.field(factory=NamedResource)
-    sprites: PokemonFormSprites = attrs.field(factory=PokemonFormSprites)
-    version_group: NamedResource = attrs.field(factory=NamedResource)
-    names: t.List[Name] = attrs.field(factory=list)
-    form_names: t.List[Name] = attrs.field(factory=list)
-    pokemon_species: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonForm":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            order=payload.get("order", 0),
-            form_order=payload.get("form_order", 0),
-            is_default=payload.get("is_default", False),
-            is_battle_only=payload.get("is_battle_only", False),
-            is_mega=payload.get("is_mega", False),
-            form_name=payload.get("form_name", ""),
-            pokemon=NamedResource.from_payload(payload.get("pokemon", {}) or {}),
-            sprites=PokemonFormSprites.from_payload(payload.get("sprites", {}) or {}),
-            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            form_names=[Name.from_payload(i) for i in payload.get("form_names", [])],
-            pokemon_species=NamedResource.from_payload(payload.get("pokemon_species", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonHabitats(BaseModel):
-    """PokemonHabitats model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this Pokémon habitat resource.
-    name: str
-        The name for this Pokémon habitat resource.
-    names: t.List[Name]
-        The name of this Pokémon habitat listed in different languages.
-    pokemon_species: t.List[NamedAPIResource]
-        A list of the Pokémon species that can be found in this habitat.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    names: t.List[Name] = attrs.field(factory=list)
-    pokemon_species: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonHabitats":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            pokemon_species=[NamedResource.from_payload(i) for i in payload.get("pokemon_species", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonShape(BaseModel):
-    """PokemonShape model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this Pokémon shape resource.
-    name: str
-        The name for this Pokémon shape resource.
-    awesome_names: t.List[AwesomeName]
-        The "scientific" name of this Pokémon shape listed in different languages.
-    names: t.List[Name]
-        The name of this Pokémon shape listed in different languages.
-    pokemon_species: t.List[NamedAPIResource]
-        A list of the Pokémon species that have this shape.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    awesome_names: t.List[AwesomeName] = attrs.field(factory=list)
-    names: t.List[Name] = attrs.field(factory=list)
-    pokemon_species: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonShape":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            awesome_names=[AwesomeName.from_payload(i) for i in payload.get("awesome_names", [])],
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            pokemon_species=[NamedResource.from_payload(i) for i in payload.get("pokemon_species", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonSpecies(BaseModel):
-    """PokemonSpecies model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this Pokémon species resource.
-    name: str
-        The name for this Pokémon species resource.
-    order: int
-        The order in which species should be sorted. Based on National Dex order,
-        except families are grouped together and sorted by stage.
-    gender_rate: int
-        The chance of this Pokémon being of a particular gender. Ratio is male to female. -1 for genderless.
-    capture_rate: int
-        The base capture rate; up to 255. The higher the number, the easier the catch.
-    base_happiness: int
-        The happiness when caught by a normal Pokéball; up to 255. The higher the number, the happier the Pokémon.
-    is_baby: bool
-        Whether or not this is a baby Pokémon.
-    is_legendary: bool
-        Whether or not this is a legendary Pokémon.
-    is_mythical: bool
-        Whether or not this is a mythical Pokémon.
-    hatch_counter: int
-        Initial hatch counter: one must walk 255 × (hatch_counter + 1) steps before this
-        Pokémon's egg hatches, unless utilizing bonuses like Flame Body's.
-    has_gender_differences: bool
-        Whether or not this Pokémon has visual differences due to gender.
-    forms_switchable: bool
-        Whether or not this Pokémon has multiple forms and can switch between them.
-    growth_rate: NamedAPIResource
-        The rate at which this Pokémon species gains levels.
-    pokedex_numbers: t.List[PokemonSpeciesDexEntry]
-        A list of Pokedexes and the indexes reserved within them for this Pokémon species.
-    egg_groups: t.List[NamedAPIResource]
-        A list of egg groups this Pokémon species is a member of.
-    color: NamedAPIResource
-        The color of this Pokémon for Pokédex search.
-    shape: NamedAPIResource
-        The shape of this Pokémon for Pokédex search.
-    evolves_from_species: NamedAPIResource
-        The Pokémon species that evolves into this Pokemon_species.
-    evolution_chain: APIResource
-        The evolution chain this Pokémon species is a member of.
-    habitat: NamedAPIResource
-        The habitat this Pokémon species can be encountered in.
-    generation: NamedAPIResource
-        The generation this Pokémon species was introduced in.
-    names: t.List[Name]
-        The name of this Pokémon species listed in different languages.
-    pal_park_encounters: t.List[PalParkEncounterArea]
-        A list of encounters that can be had with this Pokémon species in pal park.
-    flavor_text_entries: t.List[FlavorText]
-        A list of flavor text entries for this Pokémon species.
-    form_descriptions: t.List[Description]
-        A list of form description for this Pokémon species.
-    genera: t.List[Genus]
-        A list of the genus of this Pokémon species listed in multiple languages.
-    varieties: t.List[PokemonSpeciesVariety]
-        A list of the Pokémon that exist within this Pokémon species.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    order: int = attrs.field(factory=int)
-    gender_rate: int = attrs.field(factory=int)
-    capture_rate: int = attrs.field(factory=int)
-    base_happiness: int = attrs.field(factory=int)
-    is_baby: bool = attrs.field(factory=bool)
-    is_legendary: bool = attrs.field(factory=bool)
-    is_mythical: bool = attrs.field(factory=bool)
-    hatch_counter: int = attrs.field(factory=int)
-    has_gender_differences: bool = attrs.field(factory=bool)
-    forms_switchable: bool = attrs.field(factory=bool)
-    growth_rate: NamedResource = attrs.field(factory=NamedResource)
-    pokedex_numbers: t.List[PokemonSpeciesDexEntry] = attrs.field(factory=list)
-    egg_groups: t.List[NamedResource] = attrs.field(factory=list)
-    color: NamedResource = attrs.field(factory=NamedResource)
-    shape: NamedResource = attrs.field(factory=NamedResource)
-    evolves_from_species: NamedResource = attrs.field(factory=NamedResource)
-    evolution_chain: Resource = attrs.field(factory=Resource)
-    habitat: NamedResource = attrs.field(factory=NamedResource)
-    generation: NamedResource = attrs.field(factory=NamedResource)
-    names: t.List[Name] = attrs.field(factory=list)
-    pal_park_encounters: t.List[PalParkEncounterArea] = attrs.field(factory=list)
-    flavor_text_entries: t.List[FlavorText] = attrs.field(factory=list)
-    form_descriptions: t.List[Description] = attrs.field(factory=list)
-    genera: t.List[Genus] = attrs.field(factory=list)
-    varieties: t.List[PokemonSpeciesVariety] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonSpecies":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            order=payload.get("order", 0),
-            gender_rate=payload.get("gender_rate", 0),
-            capture_rate=payload.get("capture_rate", 0),
-            base_happiness=payload.get("base_happiness", 0),
-            is_baby=payload.get("is_baby", False),
-            is_legendary=payload.get("is_legendary", False),
-            is_mythical=payload.get("is_mythical", False),
-            hatch_counter=payload.get("hatch_counter", 0),
-            has_gender_differences=payload.get("has_gender_differences", False),
-            forms_switchable=payload.get("forms_switchable", False),
-            growth_rate=NamedResource.from_payload(payload.get("growth_rate", {}) or {}),
-            pokedex_numbers=[PokemonSpeciesDexEntry.from_payload(i) for i in payload.get("pokedex_numbers", [])],
-            egg_groups=[NamedResource.from_payload(i) for i in payload.get("egg_groups", [])],
-            color=NamedResource.from_payload(payload.get("color", {}) or {}),
-            shape=NamedResource.from_payload(payload.get("shape", {}) or {}),
-            evolves_from_species=NamedResource.from_payload(payload.get("evolves_from_species", {}) or {}),
-            evolution_chain=Resource.from_payload(payload.get("evolution_chain", {}) or {}),
-            habitat=NamedResource.from_payload(payload.get("habitat", {}) or {}),
-            generation=NamedResource.from_payload(payload.get("generation", {}) or {}),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            pal_park_encounters=[PalParkEncounterArea.from_payload(i) for i in payload.get("pal_park_encounters", [])],
-            flavor_text_entries=[FlavorText.from_payload(i) for i in payload.get("flavor_text_entries", [])],
-            form_descriptions=[Description.from_payload(i) for i in payload.get("form_descriptions", [])],
-            genera=[Genus.from_payload(i) for i in payload.get("genera", [])],
-            varieties=[PokemonSpeciesVariety.from_payload(i) for i in payload.get("varieties", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Stat(BaseModel):
-    """
-    A Pokémon stat model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    game_index: int
-        The stat order in which effects of this stat take place during battle.
-    is_battle_only: bool
-        Whether this stat only exists within a battle.
-    affecting_moves: MoveStatAffectSets
-        A detail of moves which affect this stat positively or negatively.
-    affecting_natures: NatureStatAffectSets
-        A detail of natures which affect this stat positively or negatively.
-    characteristics: t.List[Resource]
-        A list of characteristics that are set on a Pokémon when its highest base stat is this stat.
-    move_damage_class: NamedResource
-        The class of damage this stat is directly related to.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    game_index: int = attrs.field(factory=int)
-    is_battle_only: bool = attrs.field(factory=bool)
-    affecting_moves: MoveStatAffectSets = attrs.field(factory=MoveStatAffectSets)
-    affecting_natures: NatureStatAffectSets = attrs.field(factory=NatureStatAffectSets)
-    characteristics: t.List[Resource] = attrs.field(factory=list)
-    move_damage_class: NamedResource = attrs.field(factory=NamedResource)
-    names: t.List[Name] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Stat":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            game_index=payload.get("game_index", 0),
-            is_battle_only=payload.get("is_battle_only", False),
-            affecting_moves=MoveStatAffectSets.from_payload(payload.get("affecting_moves", {})),
-            affecting_natures=NatureStatAffectSets.from_payload(payload.get("affecting_natures", {})),
-            characteristics=[Resource.from_payload(i) for i in payload.get("characteristics", [])],
-            move_damage_class=NamedResource.from_payload(payload.get("move_damage_class", {}) or {}),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Type(BaseModel):
-    """
-    A Pokémon type model.
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    damage_relations: TypeRelations
-        A detail of how effective this type is toward others and vice versa.
-    game_indices: t.List[GenerationGameIndex]
-        A list of game indices relevent to this item by generation.
-    generation: NamedResource
-        The generation this type was introduced in.
-    move_damage_class: NamedResource
-        The class of damage inflicted by this type.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    pokemon: t.List[TypePokemon]
-        A list of details of Pokémon that have this type.
-    moves: t.List[NamedResource]
-        A list of moves that have this type.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    damage_relations: TypeRelations = attrs.field(factory=TypeRelations)
-    game_indices: t.List[GenerationGameIndex] = attrs.field(factory=list)
-    generation: NamedResource = attrs.field(factory=NamedResource)
-    move_damage_class: NamedResource = attrs.field(factory=NamedResource)
-    names: t.List[Name] = attrs.field(factory=list)
-    pokemon: t.List[TypePokemon] = attrs.field(factory=list)
-    moves: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Type":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            damage_relations=TypeRelations.from_payload(payload.get("damage_relations", {})),
-            game_indices=[GenerationGameIndex.from_payload(i) for i in payload.get("game_indices", [])],
-            generation=NamedResource.from_payload(payload.get("generation", {}) or {}),
-            move_damage_class=NamedResource.from_payload(payload.get("move_damage_class", {}) or {}),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-            pokemon=[TypePokemon.from_payload(i) for i in payload.get("pokemon", [])],
-            moves=[NamedResource.from_payload(i) for i in payload.get("moves", [])],
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import (
+    Description,
+    FlavorText,
+    GenerationGameIndex,
+    Name,
+    NamedResource,
+    Resource,
+    VerboseEffect,
+    VersionEncounterDetail,
+    VersionGameIndex,
+)
+
+from .showdown import ShowdownSprites
+from .utils import (
+    AbilityEffectChange,
+    AbilityFlavorText,
+    AbilityPokemon,
+    AwesomeName,
+    Genus,
+    GrowthRateExperienceLevel,
+    MoveBattleStylePreference,
+    MoveStatAffectSets,
+    NaturePokeathlonStatAffectSet,
+    NatureStatAffectSets,
+    NatureStatChange,
+    PalParkEncounterArea,
+    PokemonAbility,
+    PokemonFormSprites,
+    PokemonHeldItem,
+    PokemonMove,
+    PokemonSpeciesDexEntry,
+    PokemonSpeciesGender,
+    PokemonSpeciesVariety,
+    PokemonSprite,
+    PokemonStat,
+    PokemonType,
+    PokemonTypePast,
+    TypePokemon,
+    TypeRelations,
+)
+
+__all__: t.Tuple[str, ...] = (
+    "Ability",
+    "Characteristic",
+    "Pokemon",
+    "PokemonSpecies",
+    "PokemonForm",
+    "Nature",
+    "Type",
+    "Gender",
+    "GrowthRate",
+    "EggGroup",
+    "LocationAreaEncounter",
+    "PokemonColor",
+    "PokeathlonStat",
+    "PokemonHabitats",
+    "PokemonShape",
+    "Stat",
+)
+
+
+@attrs.define(slots=True, kw_only=True)
+class Ability(BaseModel):
+    """Ability model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this ability resource.
+    name: str
+        The name for this ability resource.
+    is_main_series: bool
+        Whether or not this ability originated in the main series of the video games.
+    generation: NamedResource
+        The generation this ability originated in.
+    names: t.List[Name]
+        The name of this ability listed in different languages.
+    effect_entries: t.List[VerboseEffect]
+        The effect of this ability listed in different languages.
+    effect_changes: t.List[AbilityEffectChange]
+        The list of previous effects this ability has had across version groups of the games.
+    flavor_text_entries: t.List[AbilityFlavorText]
+        The flavor text of this ability listed in different languages.
+    pokemon: t.List[AbilityPokemon]
+        A list of Pokémon that could potentially have this ability.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    is_main_series: bool = attrs.field(factory=bool)
+    generation: NamedResource = attrs.field(factory=NamedResource)
+    names: t.List[Name] = attrs.field(factory=list)
+    effect_entries: t.List[VerboseEffect] = attrs.field(factory=list)
+    effect_changes: t.List[AbilityEffectChange] = attrs.field(factory=list)
+    flavor_text_entries: t.List[AbilityFlavorText] = attrs.field(factory=list)
+    pokemon: t.List[AbilityPokemon] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Ability":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            is_main_series=payload.get("is_main_series", False),
+            generation=NamedResource.from_payload(payload.get("generation", {}) or {}),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            effect_entries=[VerboseEffect.from_payload(i) for i in payload.get("effect_entries", [])],
+            effect_changes=[AbilityEffectChange.from_payload(i) for i in payload.get("effect_changes", [])],
+            flavor_text_entries=[AbilityFlavorText.from_payload(i) for i in payload.get("flavor_text_entries", [])],
+            pokemon=[AbilityPokemon.from_payload(i) for i in payload.get("pokemon", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Characteristic(BaseModel):
+    """Characteristic model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this characteristic resource.
+    gene_modulo: int
+        The remainder of the highest stat/IV divided by 5.
+    possible_values: t.List[int]
+        The possible values of the highest stat that would result in a Pokémon
+         recieving this characteristic when divided by 5.
+
+    """
+
+    id: int = attrs.field(factory=int)
+    gene_modulo: int = attrs.field(factory=int)
+    possible_values: t.List[int] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Characteristic":
+        return cls(
+            id=payload.get("id", 0),
+            gene_modulo=payload.get("gene_modulo", 0),
+            possible_values=payload.get("possible_values", []),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class EggGroup(BaseModel):
+    """EggGroup model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this egg group resource.
+    name: str
+        The name for this egg group resource.
+    names: t.List[Name]
+        The name of this egg group listed in different languages.
+    pokemon_species: t.List[NamedResource]
+        A list of all Pokémon species that are members of this egg group.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    names: t.List[Name] = attrs.field(factory=list)
+    pokemon_species: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EggGroup":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            pokemon_species=[NamedResource.from_payload(i) for i in payload.get("pokemon_species", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Gender(BaseModel):
+    """Gender model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for gender resource.
+    name: str
+        The name for this gender resource.
+    pokemon_species_details: t.List[PokemonSpeciesGender]
+        A list of Pokémon species that belong to this gender.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    pokemon_species_details: t.List[PokemonSpeciesGender] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Gender":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            pokemon_species_details=[
+                PokemonSpeciesGender.from_payload(i) for i in payload.get("pokemon_species_details", [])
+            ],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class GrowthRate(BaseModel):
+    """GrowthRate model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this growth rate resource.
+    name: str
+        The name for this growth rate resource.
+    formula: str
+        The formula used to calculate the rate at which the Pokémon species gains level.
+    descriptions: t.List[Description]
+        The descriptions of this characteristic listed in different languages.
+    levels: t.List[GrowthRateExperienceLevel]
+        A list of levels and the amount of experienced needed to atain them based on this growth rate.
+    pokemon_species: t.List[NamedResource]
+        A list of Pokémon species that gain levels at this growth rate.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    formula: str = attrs.field(factory=str)
+    descriptions: t.List[Description] = attrs.field(factory=list)
+    levels: t.List[GrowthRateExperienceLevel] = attrs.field(factory=list)
+    pokemon_species: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GrowthRate":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            formula=payload.get("formula", ""),
+            descriptions=[Description.from_payload(i) for i in payload.get("descriptions", [])],
+            levels=[GrowthRateExperienceLevel.from_payload(i) for i in payload.get("levels", [])],
+            pokemon_species=[NamedResource.from_payload(i) for i in payload.get("pokemon_species", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Nature(BaseModel):
+    """Nature model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this nature resource.
+    name: str
+        The name for this nature resource.
+    decreased_stat: NamedAPIResource
+        The stat decreased by 10% in Pokémon with this nature.
+    increased_stat: NamedAPIResource
+        The stat increased by 10% in Pokémon with this nature.
+    hates_flavor: NamedAPIResource
+        The flavor hated by Pokémon with this nature.
+    likes_flavor: NamedAPIResource
+        The flavor liked by Pokémon with this nature.
+    pokeathlon_stat_changes: t.List[NatureStatChange]
+        A list of Pokéathlon stats this nature effects and how much it effects them.
+    move_battle_style_preferences: t.List[MoveBattleStylePreference]
+        A list of battle styles and how likely a Pokémon with this nature
+        is to use them in the Battle Palace or Battle Tent.
+    names: t.List[Name]
+        The name of this nature listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    decreased_stat: NamedResource = attrs.field(factory=NamedResource)
+    increased_stat: NamedResource = attrs.field(factory=NamedResource)
+    hates_flavor: NamedResource = attrs.field(factory=NamedResource)
+    likes_flavor: NamedResource = attrs.field(factory=NamedResource)
+    pokeathlon_stat_changes: t.List[NatureStatChange] = attrs.field(factory=list)
+    move_battle_style_preferences: t.List[MoveBattleStylePreference] = attrs.field(factory=list)
+    names: t.List[Name] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Nature":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            decreased_stat=NamedResource.from_payload(payload.get("decreased_stat", {}) or {}),
+            increased_stat=NamedResource.from_payload(payload.get("increased_stat", {}) or {}),
+            hates_flavor=NamedResource.from_payload(payload.get("hates_flavor", {}) or {}),
+            likes_flavor=NamedResource.from_payload(payload.get("likes_flavor", {}) or {}),
+            pokeathlon_stat_changes=[
+                NatureStatChange.from_payload(i) for i in payload.get("pokeathlon_stat_changes", [])
+            ],
+            move_battle_style_preferences=[
+                MoveBattleStylePreference.from_payload(i) for i in payload.get("move_battle_style_preferences", [])
+            ],
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokeathlonStat(BaseModel):
+    """PokeathlonStat model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    names: t.List[Name]
+        A list of natures which affect this Pokéathlon stat positively or negatively.
+    affecting_natures: NaturePokeathlonStatAffectSets
+        A detail of natures which affect this Pokéathlon stat positively or negatively.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    names: t.List[Name] = attrs.field(factory=list)
+    affecting_natures: NaturePokeathlonStatAffectSet = attrs.field(factory=NaturePokeathlonStatAffectSet)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokeathlonStat":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            affecting_natures=NaturePokeathlonStatAffectSet.from_payload(payload.get("affecting_natures", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Pokemon(BaseModel):
+    """Pokemon model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this Pokémon resource.
+    name: str
+        The name for this Pokémon resource.
+    base_experience: int
+        The base experience gained for defeating this Pokémon.
+    height: int
+        The height of this Pokémon in decimetres.
+    is_default: bool
+        Set for exactly one Pokémon used as the default for each species.
+    order: int
+        Order for sorting. Almost national order, except families are grouped together.
+    weight: int
+        The weight of this Pokémon in hectograms.
+    abilities: t.List[PokemonAbility]
+        A list of abilities this Pokémon could potentially have.
+    forms: t.List[NamedAPIResource]
+        A list of forms this Pokémon can take on.
+    game_indices: t.List[VersionGameIndex]
+        A list of game indices relevent to Pokémon item by generation.
+    held_items: t.List[PokemonHeldItem]
+        A list of items this Pokémon may be holding when encountered.
+    location_area_encounters: str
+        Location area encounter details for different versions.
+    moves: t.List[PokemonMove]
+        A list of details showing types this Pokémon has.
+    species: NamedAPIResource
+        The species this Pokémon belongs to.
+    sprites: PokemonSprites
+        A set of sprites used to depict this Pokémon in the game.
+    stats: t.List[PokemonStat]
+        A list of details showing all the stats this Pokémon has.
+    types: t.List[PokemonType]
+        A list of details showing types this Pokémon has.
+    showdown: ShowdownSprites
+        A set of sprites used to depict this Pokémon in the Showdown client.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    base_experience: int = attrs.field(factory=int)
+    height: int = attrs.field(factory=int)
+    is_default: bool = attrs.field(factory=bool)
+    order: int = attrs.field(factory=int)
+    weight: int = attrs.field(factory=int)
+    abilities: t.List[PokemonAbility] = attrs.field(factory=list)
+    forms: t.List[NamedResource] = attrs.field(factory=list)
+    game_indices: t.List[VersionGameIndex] = attrs.field(factory=list)
+    held_items: t.List[PokemonHeldItem] = attrs.field(factory=list)
+    location_area_encounters: str = attrs.field(factory=str)
+    moves: t.List[PokemonMove] = attrs.field(factory=list)
+    past_types: t.List[PokemonTypePast] = attrs.field(factory=list)
+    sprites: PokemonSprite = attrs.field(factory=PokemonSprite)
+    species: NamedResource = attrs.field(factory=NamedResource)
+    stats: t.List[PokemonStat] = attrs.field(factory=list)
+    types: t.List[PokemonType] = attrs.field(factory=list)
+    showdown: ShowdownSprites = attrs.field(factory=ShowdownSprites)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Pokemon":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            base_experience=payload.get("base_experience", 0),
+            height=payload.get("height", 0),
+            is_default=payload.get("is_default", False),
+            order=payload.get("order", 0),
+            weight=payload.get("weight", 0),
+            abilities=[PokemonAbility.from_payload(i) for i in payload.get("abilities", [])],
+            forms=[NamedResource.from_payload(i) for i in payload.get("forms", [])],
+            game_indices=[VersionGameIndex.from_payload(i) for i in payload.get("game_indices", [])],
+            held_items=[PokemonHeldItem.from_payload(i) for i in payload.get("held_items", [])],
+            location_area_encounters=payload.get("location_area_encounters", ""),
+            moves=[PokemonMove.from_payload(i) for i in payload.get("moves", [])],
+            past_types=[PokemonTypePast.from_payload(i) for i in payload.get("past_types", [])],
+            sprites=PokemonSprite.from_payload(payload.get("sprites", {}) or {}),
+            species=NamedResource.from_payload(payload.get("species", {}) or {}),
+            stats=[PokemonStat.from_payload(i) for i in payload.get("stats", [])],
+            types=[PokemonType.from_payload(i) for i in payload.get("types", [])],
+            showdown=ShowdownSprites.from_id(payload.get("id", 0)),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class LocationAreaEncounter(BaseModel):
+    """LocationAreaEncounter model.
+
+    Attributes
+    ----------
+    location_area: NamedAPIResource
+        The location area the referenced Pokémon can be encountered in.
+    version_details: t.List[VersionEncounterDetail]
+        A list of versions and encounters with the referenced Pokémon that might happen.
+    """
+
+    location_area: NamedResource = attrs.field(factory=NamedResource)
+    version_details: t.List[VersionEncounterDetail] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "LocationAreaEncounter":
+        return cls(
+            location_area=NamedResource.from_payload(payload.get("location_area", {}) or {}),
+            version_details=[VersionEncounterDetail.from_payload(i) for i in payload.get("version_details", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonColor(BaseModel):
+    """PokemonColor model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this Pokémon color resource.
+    name: str
+        The name for this Pokémon color resource.
+    names: t.List[Name]
+        The name of this Pokémon color listed in different languages.
+    pokemon_species: t.List[NamedAPIResource]
+        A list of the Pokémon species that have this color.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    names: t.List[Name] = attrs.field(factory=list)
+    pokemon_species: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonColor":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            pokemon_species=[NamedResource.from_payload(i) for i in payload.get("pokemon_species", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonForm(BaseModel):
+    """PokemonForm model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this Pokémon form resource.
+    name: str
+        The name for this Pokémon form resource.
+    order: int
+        The order in which forms should be sorted within all forms. Multiple forms may have equal order,
+        in which case they should fall back on sorting by name.
+    form_order: int
+        The order in which forms should be sorted within a species' forms.
+    is_default: bool
+        True for exactly one form used as the default for each Pokémon.
+    is_battle_only: bool
+        Whether or not this form can only happen during battle.
+    is_mega: bool
+        Whether or not this form requires mega evolution.
+    form_name: str
+        The name of this form.
+    pokemon: NamedAPIResource
+        The Pokémon that can take on this form.
+    sprites: PokemonFormSprites
+        A set of sprites used to depict this Pokémon form in the game.
+    version_group: NamedAPIResource
+        The version group this Pokémon form was introduced in.
+    names: t.List[Name]
+        The form specific full name of this Pokémon form, or empty if the form does not have a specific name.
+    form_names: t.List[Name]
+        The form specific form name of this Pokémon form, or empty if the form does not have a specific name.
+    pokemon_species: NamedAPIResource
+        The Pokémon species that this form belongs to.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    order: int = attrs.field(factory=int)
+    form_order: int = attrs.field(factory=int)
+    is_default: bool = attrs.field(factory=bool)
+    is_battle_only: bool = attrs.field(factory=bool)
+    is_mega: bool = attrs.field(factory=bool)
+    form_name: str = attrs.field(factory=str)
+    pokemon: NamedResource = attrs.field(factory=NamedResource)
+    sprites: PokemonFormSprites = attrs.field(factory=PokemonFormSprites)
+    version_group: NamedResource = attrs.field(factory=NamedResource)
+    names: t.List[Name] = attrs.field(factory=list)
+    form_names: t.List[Name] = attrs.field(factory=list)
+    pokemon_species: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonForm":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            order=payload.get("order", 0),
+            form_order=payload.get("form_order", 0),
+            is_default=payload.get("is_default", False),
+            is_battle_only=payload.get("is_battle_only", False),
+            is_mega=payload.get("is_mega", False),
+            form_name=payload.get("form_name", ""),
+            pokemon=NamedResource.from_payload(payload.get("pokemon", {}) or {}),
+            sprites=PokemonFormSprites.from_payload(payload.get("sprites", {}) or {}),
+            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            form_names=[Name.from_payload(i) for i in payload.get("form_names", [])],
+            pokemon_species=NamedResource.from_payload(payload.get("pokemon_species", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonHabitats(BaseModel):
+    """PokemonHabitats model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this Pokémon habitat resource.
+    name: str
+        The name for this Pokémon habitat resource.
+    names: t.List[Name]
+        The name of this Pokémon habitat listed in different languages.
+    pokemon_species: t.List[NamedAPIResource]
+        A list of the Pokémon species that can be found in this habitat.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    names: t.List[Name] = attrs.field(factory=list)
+    pokemon_species: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonHabitats":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            pokemon_species=[NamedResource.from_payload(i) for i in payload.get("pokemon_species", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonShape(BaseModel):
+    """PokemonShape model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this Pokémon shape resource.
+    name: str
+        The name for this Pokémon shape resource.
+    awesome_names: t.List[AwesomeName]
+        The "scientific" name of this Pokémon shape listed in different languages.
+    names: t.List[Name]
+        The name of this Pokémon shape listed in different languages.
+    pokemon_species: t.List[NamedAPIResource]
+        A list of the Pokémon species that have this shape.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    awesome_names: t.List[AwesomeName] = attrs.field(factory=list)
+    names: t.List[Name] = attrs.field(factory=list)
+    pokemon_species: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonShape":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            awesome_names=[AwesomeName.from_payload(i) for i in payload.get("awesome_names", [])],
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            pokemon_species=[NamedResource.from_payload(i) for i in payload.get("pokemon_species", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonSpecies(BaseModel):
+    """PokemonSpecies model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this Pokémon species resource.
+    name: str
+        The name for this Pokémon species resource.
+    order: int
+        The order in which species should be sorted. Based on National Dex order,
+        except families are grouped together and sorted by stage.
+    gender_rate: int
+        The chance of this Pokémon being of a particular gender. Ratio is male to female. -1 for genderless.
+    capture_rate: int
+        The base capture rate; up to 255. The higher the number, the easier the catch.
+    base_happiness: int
+        The happiness when caught by a normal Pokéball; up to 255. The higher the number, the happier the Pokémon.
+    is_baby: bool
+        Whether or not this is a baby Pokémon.
+    is_legendary: bool
+        Whether or not this is a legendary Pokémon.
+    is_mythical: bool
+        Whether or not this is a mythical Pokémon.
+    hatch_counter: int
+        Initial hatch counter: one must walk 255 × (hatch_counter + 1) steps before this
+        Pokémon's egg hatches, unless utilizing bonuses like Flame Body's.
+    has_gender_differences: bool
+        Whether or not this Pokémon has visual differences due to gender.
+    forms_switchable: bool
+        Whether or not this Pokémon has multiple forms and can switch between them.
+    growth_rate: NamedAPIResource
+        The rate at which this Pokémon species gains levels.
+    pokedex_numbers: t.List[PokemonSpeciesDexEntry]
+        A list of Pokedexes and the indexes reserved within them for this Pokémon species.
+    egg_groups: t.List[NamedAPIResource]
+        A list of egg groups this Pokémon species is a member of.
+    color: NamedAPIResource
+        The color of this Pokémon for Pokédex search.
+    shape: NamedAPIResource
+        The shape of this Pokémon for Pokédex search.
+    evolves_from_species: NamedAPIResource
+        The Pokémon species that evolves into this Pokemon_species.
+    evolution_chain: APIResource
+        The evolution chain this Pokémon species is a member of.
+    habitat: NamedAPIResource
+        The habitat this Pokémon species can be encountered in.
+    generation: NamedAPIResource
+        The generation this Pokémon species was introduced in.
+    names: t.List[Name]
+        The name of this Pokémon species listed in different languages.
+    pal_park_encounters: t.List[PalParkEncounterArea]
+        A list of encounters that can be had with this Pokémon species in pal park.
+    flavor_text_entries: t.List[FlavorText]
+        A list of flavor text entries for this Pokémon species.
+    form_descriptions: t.List[Description]
+        A list of form description for this Pokémon species.
+    genera: t.List[Genus]
+        A list of the genus of this Pokémon species listed in multiple languages.
+    varieties: t.List[PokemonSpeciesVariety]
+        A list of the Pokémon that exist within this Pokémon species.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    order: int = attrs.field(factory=int)
+    gender_rate: int = attrs.field(factory=int)
+    capture_rate: int = attrs.field(factory=int)
+    base_happiness: int = attrs.field(factory=int)
+    is_baby: bool = attrs.field(factory=bool)
+    is_legendary: bool = attrs.field(factory=bool)
+    is_mythical: bool = attrs.field(factory=bool)
+    hatch_counter: int = attrs.field(factory=int)
+    has_gender_differences: bool = attrs.field(factory=bool)
+    forms_switchable: bool = attrs.field(factory=bool)
+    growth_rate: NamedResource = attrs.field(factory=NamedResource)
+    pokedex_numbers: t.List[PokemonSpeciesDexEntry] = attrs.field(factory=list)
+    egg_groups: t.List[NamedResource] = attrs.field(factory=list)
+    color: NamedResource = attrs.field(factory=NamedResource)
+    shape: NamedResource = attrs.field(factory=NamedResource)
+    evolves_from_species: NamedResource = attrs.field(factory=NamedResource)
+    evolution_chain: Resource = attrs.field(factory=Resource)
+    habitat: NamedResource = attrs.field(factory=NamedResource)
+    generation: NamedResource = attrs.field(factory=NamedResource)
+    names: t.List[Name] = attrs.field(factory=list)
+    pal_park_encounters: t.List[PalParkEncounterArea] = attrs.field(factory=list)
+    flavor_text_entries: t.List[FlavorText] = attrs.field(factory=list)
+    form_descriptions: t.List[Description] = attrs.field(factory=list)
+    genera: t.List[Genus] = attrs.field(factory=list)
+    varieties: t.List[PokemonSpeciesVariety] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonSpecies":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            order=payload.get("order", 0),
+            gender_rate=payload.get("gender_rate", 0),
+            capture_rate=payload.get("capture_rate", 0),
+            base_happiness=payload.get("base_happiness", 0),
+            is_baby=payload.get("is_baby", False),
+            is_legendary=payload.get("is_legendary", False),
+            is_mythical=payload.get("is_mythical", False),
+            hatch_counter=payload.get("hatch_counter", 0),
+            has_gender_differences=payload.get("has_gender_differences", False),
+            forms_switchable=payload.get("forms_switchable", False),
+            growth_rate=NamedResource.from_payload(payload.get("growth_rate", {}) or {}),
+            pokedex_numbers=[PokemonSpeciesDexEntry.from_payload(i) for i in payload.get("pokedex_numbers", [])],
+            egg_groups=[NamedResource.from_payload(i) for i in payload.get("egg_groups", [])],
+            color=NamedResource.from_payload(payload.get("color", {}) or {}),
+            shape=NamedResource.from_payload(payload.get("shape", {}) or {}),
+            evolves_from_species=NamedResource.from_payload(payload.get("evolves_from_species", {}) or {}),
+            evolution_chain=Resource.from_payload(payload.get("evolution_chain", {}) or {}),
+            habitat=NamedResource.from_payload(payload.get("habitat", {}) or {}),
+            generation=NamedResource.from_payload(payload.get("generation", {}) or {}),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            pal_park_encounters=[PalParkEncounterArea.from_payload(i) for i in payload.get("pal_park_encounters", [])],
+            flavor_text_entries=[FlavorText.from_payload(i) for i in payload.get("flavor_text_entries", [])],
+            form_descriptions=[Description.from_payload(i) for i in payload.get("form_descriptions", [])],
+            genera=[Genus.from_payload(i) for i in payload.get("genera", [])],
+            varieties=[PokemonSpeciesVariety.from_payload(i) for i in payload.get("varieties", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Stat(BaseModel):
+    """
+    A Pokémon stat model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    game_index: int
+        The stat order in which effects of this stat take place during battle.
+    is_battle_only: bool
+        Whether this stat only exists within a battle.
+    affecting_moves: MoveStatAffectSets
+        A detail of moves which affect this stat positively or negatively.
+    affecting_natures: NatureStatAffectSets
+        A detail of natures which affect this stat positively or negatively.
+    characteristics: t.List[Resource]
+        A list of characteristics that are set on a Pokémon when its highest base stat is this stat.
+    move_damage_class: NamedResource
+        The class of damage this stat is directly related to.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    game_index: int = attrs.field(factory=int)
+    is_battle_only: bool = attrs.field(factory=bool)
+    affecting_moves: MoveStatAffectSets = attrs.field(factory=MoveStatAffectSets)
+    affecting_natures: NatureStatAffectSets = attrs.field(factory=NatureStatAffectSets)
+    characteristics: t.List[Resource] = attrs.field(factory=list)
+    move_damage_class: NamedResource = attrs.field(factory=NamedResource)
+    names: t.List[Name] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Stat":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            game_index=payload.get("game_index", 0),
+            is_battle_only=payload.get("is_battle_only", False),
+            affecting_moves=MoveStatAffectSets.from_payload(payload.get("affecting_moves", {}) or {}),
+            affecting_natures=NatureStatAffectSets.from_payload(payload.get("affecting_natures", {}) or {}),
+            characteristics=[Resource.from_payload(i) for i in payload.get("characteristics", [])],
+            move_damage_class=NamedResource.from_payload(payload.get("move_damage_class", {}) or {}),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Type(BaseModel):
+    """
+    A Pokémon type model.
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    damage_relations: TypeRelations
+        A detail of how effective this type is toward others and vice versa.
+    game_indices: t.List[GenerationGameIndex]
+        A list of game indices relevent to this item by generation.
+    generation: NamedResource
+        The generation this type was introduced in.
+    move_damage_class: NamedResource
+        The class of damage inflicted by this type.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    pokemon: t.List[TypePokemon]
+        A list of details of Pokémon that have this type.
+    moves: t.List[NamedResource]
+        A list of moves that have this type.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    damage_relations: TypeRelations = attrs.field(factory=TypeRelations)
+    game_indices: t.List[GenerationGameIndex] = attrs.field(factory=list)
+    generation: NamedResource = attrs.field(factory=NamedResource)
+    move_damage_class: NamedResource = attrs.field(factory=NamedResource)
+    names: t.List[Name] = attrs.field(factory=list)
+    pokemon: t.List[TypePokemon] = attrs.field(factory=list)
+    moves: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Type":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            damage_relations=TypeRelations.from_payload(payload.get("damage_relations", {}) or {}),
+            game_indices=[GenerationGameIndex.from_payload(i) for i in payload.get("game_indices", [])],
+            generation=NamedResource.from_payload(payload.get("generation", {}) or {}),
+            move_damage_class=NamedResource.from_payload(payload.get("move_damage_class", {}) or {}),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+            pokemon=[TypePokemon.from_payload(i) for i in payload.get("pokemon", [])],
+            moves=[NamedResource.from_payload(i) for i in payload.get("moves", [])],
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/utils/contests.py` & `pokelance-0.1.0/pokelance/models/abstract/utils/contests.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import NamedResource
-
-__all__: t.Tuple[str, ...] = ("ContestName",)
-
-
-@attrs.define(slots=True, kw_only=True)
-class ContestName(BaseModel):
-    """A contest name resource.
-
-    Attributes
-    ----------
-    name: str
-        The name for this contest.
-    color: str
-        The color associated with this contest's name.
-    language: NamedResource
-        The language that this name is in.
-    """
-
-    name: str = attrs.field(factory=str)
-    color: str = attrs.field(factory=str)
-    language: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ContestName":
-        return cls(
-            name=payload.get("name", ""),
-            color=payload.get("color", ""),
-            language=NamedResource.from_payload(payload.get("language", {}) or {}),
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import NamedResource
+
+__all__: t.Tuple[str, ...] = ("ContestName",)
+
+
+@attrs.define(slots=True, kw_only=True)
+class ContestName(BaseModel):
+    """A contest name resource.
+
+    Attributes
+    ----------
+    name: str
+        The name for this contest.
+    color: str
+        The color associated with this contest's name.
+    language: NamedResource
+        The language that this name is in.
+    """
+
+    name: str = attrs.field(factory=str)
+    color: str = attrs.field(factory=str)
+    language: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ContestName":
+        return cls(
+            name=payload.get("name", ""),
+            color=payload.get("color", ""),
+            language=NamedResource.from_payload(payload.get("language", {}) or {}),
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/utils/evolutions.py` & `pokelance-0.1.0/pokelance/models/abstract/utils/evolutions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,129 +1,130 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import NamedResource
-
-__all__: t.Tuple[str, ...] = (
-    "ChainLink",
-    "EvolutionDetail",
-)
-
-
-@attrs.define(slots=True, kw_only=True)
-class EvolutionDetail(BaseModel):
-    """An evolution detail resource.
-
-    Attributes
-    ----------
-    item: NamedResource
-        The item required to cause evolution this into Pokémon species.
-    trigger: NamedResource
-        The type of event that triggers evolution into this Pokémon species.
-    gender: int
-        Gender of the evolving Pokémon species must be in order to evolve.
-    held_item: NamedResource
-        The item the evolving Pokémon species must be holding during the evolution trigger event.
-    known_move: NamedResource
-        The move that must be known by the evolving Pokémon species during the evolution trigger event.
-    known_move_type: NamedResource
-        The evolving Pokémon species must know a move with this type during the evolution trigger event.
-    location: NamedResource
-        The location the evolution must be triggered at.
-    min_affection: int
-        The minimum required level of affection the evolving Pokémon species must have.
-    min_beauty: int
-        The minimum required level of beauty the evolving Pokémon species must have.
-    min_happiness: int
-        The minimum required level of happiness the evolving Pokémon species must have.
-    min_level: int
-        The minimum required level of the evolving Pokémon species.
-    needs_overworld_rain: bool
-        Whether or not it must be raining in the overworld to cause evolution this Pokémon species.
-    party_species: NamedResource
-        The specific Pokémon species that must be in the players party in order for the evolution to occur.
-    party_type: NamedResource
-        The player must have a Pokémon of this type in their party during the evolution trigger event.
-    relative_physical_stats: int
-        The required relation between the Pokémon's Attack and Defense stats.
-    time_of_day: str
-        The time of day the evolution must be triggered at.
-    trade_species: NamedResource
-        The specific Pokémon species that must be traded with the evolving Pokémon species.
-    turn_upside_down: bool
-        Whether or not the 3DS needs to be turned upside-down as this Pokémon levels up.
-    """
-
-    item: NamedResource = attrs.field(factory=NamedResource)
-    trigger: NamedResource = attrs.field(factory=NamedResource)
-    gender: int = attrs.field(factory=int)
-    held_item: NamedResource = attrs.field(factory=NamedResource)
-    known_move: NamedResource = attrs.field(factory=NamedResource)
-    known_move_type: NamedResource = attrs.field(factory=NamedResource)
-    location: NamedResource = attrs.field(factory=NamedResource)
-    min_level: int = attrs.field(factory=int)
-    min_happiness: int = attrs.field(factory=int)
-    min_beauty: int = attrs.field(factory=int)
-    min_affection: int = attrs.field(factory=int)
-    needs_overworld_rain: bool = attrs.field(factory=bool)
-    party_species: NamedResource = attrs.field(factory=NamedResource)
-    party_type: NamedResource = attrs.field(factory=NamedResource)
-    relative_physical_stats: int = attrs.field(factory=int)
-    time_of_day: str = attrs.field(factory=str)
-    trade_species: NamedResource = attrs.field(factory=NamedResource)
-    turn_upside_down: bool = attrs.field(factory=bool)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EvolutionDetail":
-        return cls(
-            item=NamedResource.from_payload(payload.get("item", {}) or {}),
-            trigger=NamedResource.from_payload(payload.get("trigger", {}) or {}),
-            gender=payload.get("gender", 0),
-            held_item=NamedResource.from_payload(payload.get("held_item", {}) or {}),
-            known_move=NamedResource.from_payload(payload.get("known_move", {}) or {}),
-            known_move_type=NamedResource.from_payload(payload.get("known_move_type", {}) or {}),
-            location=NamedResource.from_payload(payload.get("location", {}) or {}),
-            min_level=payload.get("min_level", 0),
-            min_happiness=payload.get("min_happiness", 0),
-            min_beauty=payload.get("min_beauty", 0),
-            min_affection=payload.get("min_affection", 0),
-            needs_overworld_rain=payload.get("needs_overworld_rain", False),
-            party_species=NamedResource.from_payload(payload.get("party_species", {}) or {}),
-            party_type=NamedResource.from_payload(payload.get("party_type", {}) or {}),
-            relative_physical_stats=payload.get("relative_physical_stats", 0),
-            time_of_day=payload.get("time_of_day", ""),
-            trade_species=NamedResource.from_payload(payload.get("trade_species", {}) or {}),
-            turn_upside_down=payload.get("turn_upside_down", False),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class ChainLink(BaseModel):
-    """A chain link resource.
-
-    Attributes
-    ----------
-    is_baby: bool
-        Whether or not this link is for a baby Pokémon.
-    species: NamedResource
-        The Pokémon species at this point in the evolution chain.
-    evolution_details: t.List[EvolutionDetail]
-        A list of details regarding the specific details of the referenced Pokémon species evolution.
-    evolves_to: t.List[ChainLink]
-        A list of chain links.
-    """
-
-    is_baby: bool = attrs.field(factory=bool)
-    species: NamedResource = attrs.field(factory=NamedResource)
-    evolution_details: t.List[EvolutionDetail] = attrs.field(factory=list)
-    evolves_to: t.List["ChainLink"] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ChainLink":
-        return cls(
-            is_baby=payload.get("is_baby", False),
-            species=NamedResource.from_payload(payload.get("species", {}) or {}),
-            evolution_details=[EvolutionDetail.from_payload(detail) for detail in payload.get("evolution_details", [])],
-            evolves_to=[ChainLink.from_payload(link) for link in payload.get("evolves_to", [])],
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import NamedResource
+
+__all__: t.Tuple[str, ...] = (
+    "ChainLink",
+    "EvolutionDetail",
+)
+GENDER_MAP: t.Dict[int, str] = {1: "Female", 2: "Male", 3: "Genderless"}
+
+
+@attrs.define(slots=True, kw_only=True)
+class EvolutionDetail(BaseModel):
+    """An evolution detail resource.
+
+    Attributes
+    ----------
+    item: NamedResource
+        The item required to cause evolution this into Pokémon species.
+    trigger: NamedResource
+        The type of event that triggers evolution into this Pokémon species.
+    gender: str
+        Gender of the evolving Pokémon species must be in order to evolve.
+    held_item: NamedResource
+        The item the evolving Pokémon species must be holding during the evolution trigger event.
+    known_move: NamedResource
+        The move that must be known by the evolving Pokémon species during the evolution trigger event.
+    known_move_type: NamedResource
+        The evolving Pokémon species must know a move with this type during the evolution trigger event.
+    location: NamedResource
+        The location the evolution must be triggered at.
+    min_affection: int
+        The minimum required level of affection the evolving Pokémon species must have.
+    min_beauty: int
+        The minimum required level of beauty the evolving Pokémon species must have.
+    min_happiness: int
+        The minimum required level of happiness the evolving Pokémon species must have.
+    min_level: int
+        The minimum required level of the evolving Pokémon species.
+    needs_overworld_rain: bool
+        Whether or not it must be raining in the overworld to cause evolution this Pokémon species.
+    party_species: NamedResource
+        The specific Pokémon species that must be in the players party in order for the evolution to occur.
+    party_type: NamedResource
+        The player must have a Pokémon of this type in their party during the evolution trigger event.
+    relative_physical_stats: int
+        The required relation between the Pokémon's Attack and Defense stats.
+    time_of_day: str
+        The time of day the evolution must be triggered at.
+    trade_species: NamedResource
+        The specific Pokémon species that must be traded with the evolving Pokémon species.
+    turn_upside_down: bool
+        Whether or not the 3DS needs to be turned upside-down as this Pokémon levels up.
+    """
+
+    item: NamedResource = attrs.field(factory=NamedResource)
+    trigger: NamedResource = attrs.field(factory=NamedResource)
+    gender: str = attrs.field(factory=str)
+    held_item: NamedResource = attrs.field(factory=NamedResource)
+    known_move: NamedResource = attrs.field(factory=NamedResource)
+    known_move_type: NamedResource = attrs.field(factory=NamedResource)
+    location: NamedResource = attrs.field(factory=NamedResource)
+    min_level: int = attrs.field(factory=int)
+    min_happiness: int = attrs.field(factory=int)
+    min_beauty: int = attrs.field(factory=int)
+    min_affection: int = attrs.field(factory=int)
+    needs_overworld_rain: bool = attrs.field(factory=bool)
+    party_species: NamedResource = attrs.field(factory=NamedResource)
+    party_type: NamedResource = attrs.field(factory=NamedResource)
+    relative_physical_stats: int = attrs.field(factory=int)
+    time_of_day: str = attrs.field(factory=str)
+    trade_species: NamedResource = attrs.field(factory=NamedResource)
+    turn_upside_down: bool = attrs.field(factory=bool)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EvolutionDetail":
+        return cls(
+            item=NamedResource.from_payload(payload.get("item", {}) or {}),
+            trigger=NamedResource.from_payload(payload.get("trigger", {}) or {}),
+            gender=GENDER_MAP.get(payload.get("gender", 0), ""),
+            held_item=NamedResource.from_payload(payload.get("held_item", {}) or {}),
+            known_move=NamedResource.from_payload(payload.get("known_move", {}) or {}),
+            known_move_type=NamedResource.from_payload(payload.get("known_move_type", {}) or {}),
+            location=NamedResource.from_payload(payload.get("location", {}) or {}),
+            min_level=payload.get("min_level", 0),
+            min_happiness=payload.get("min_happiness", 0),
+            min_beauty=payload.get("min_beauty", 0),
+            min_affection=payload.get("min_affection", 0),
+            needs_overworld_rain=payload.get("needs_overworld_rain", False),
+            party_species=NamedResource.from_payload(payload.get("party_species", {}) or {}),
+            party_type=NamedResource.from_payload(payload.get("party_type", {}) or {}),
+            relative_physical_stats=payload.get("relative_physical_stats", 0),
+            time_of_day=payload.get("time_of_day", ""),
+            trade_species=NamedResource.from_payload(payload.get("trade_species", {}) or {}),
+            turn_upside_down=payload.get("turn_upside_down", False),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class ChainLink(BaseModel):
+    """A chain link resource.
+
+    Attributes
+    ----------
+    is_baby: bool
+        Whether or not this link is for a baby Pokémon.
+    species: NamedResource
+        The Pokémon species at this point in the evolution chain.
+    evolution_details: t.List[EvolutionDetail]
+        A list of details regarding the specific details of the referenced Pokémon species evolution.
+    evolves_to: t.List[ChainLink]
+        A list of chain links.
+    """
+
+    is_baby: bool = attrs.field(factory=bool)
+    species: NamedResource = attrs.field(factory=NamedResource)
+    evolution_details: t.List[EvolutionDetail] = attrs.field(factory=list)
+    evolves_to: t.List["ChainLink"] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ChainLink":
+        return cls(
+            is_baby=payload.get("is_baby", False),
+            species=NamedResource.from_payload(payload.get("species", {}) or {}),
+            evolution_details=[EvolutionDetail.from_payload(detail) for detail in payload.get("evolution_details", [])],
+            evolves_to=[ChainLink.from_payload(link) for link in payload.get("evolves_to", [])],
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/utils/games.py` & `pokelance-0.1.0/pokelance/models/abstract/utils/games.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import NamedResource
-
-__all__: t.Tuple[str, ...] = ("PokemonEntry",)
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonEntry(BaseModel):
-    """A pokemon entry resource.
-
-    Attributes
-    ----------
-    entry_number: int
-        The index of this Pokémon species entry within the Pokédex.
-    pokemon_species: NamedResource
-        The Pokémon species being encountered.
-    """
-
-    entry_number: int = attrs.field(factory=int)
-    pokemon_species: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonEntry":
-        return cls(
-            entry_number=payload.get("entry_number", 0),
-            pokemon_species=NamedResource.from_payload(payload.get("pokemon_species", {}) or {}),
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import NamedResource
+
+__all__: t.Tuple[str, ...] = ("PokemonEntry",)
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonEntry(BaseModel):
+    """A pokemon entry resource.
+
+    Attributes
+    ----------
+    entry_number: int
+        The index of this Pokémon species entry within the Pokédex.
+    pokemon_species: NamedResource
+        The Pokémon species being encountered.
+    """
+
+    entry_number: int = attrs.field(factory=int)
+    pokemon_species: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonEntry":
+        return cls(
+            entry_number=payload.get("entry_number", 0),
+            pokemon_species=NamedResource.from_payload(payload.get("pokemon_species", {}) or {}),
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/utils/items.py` & `pokelance-0.1.0/pokelance/models/abstract/utils/items.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import NamedResource
-
-__all__: t.Tuple[str, ...] = (
-    "ItemSprites",
-    "ItemHolderPokemon",
-    "ItemHolderPokemonVersionDetail",
-)
-
-
-@attrs.define(slots=True, kw_only=True)
-class ItemSprites(BaseModel):
-    """An item sprites resource.
-
-    Attributes
-    ----------
-    default: str
-        The default depiction of this item.
-    """
-
-    default: str = attrs.field(factory=str)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, str]) -> "ItemSprites":
-        return cls(default=payload.get("default", ""))
-
-
-@attrs.define(slots=True, kw_only=True)
-class ItemHolderPokemonVersionDetail(BaseModel):
-    """An item holder pokemon version detail resource.
-
-    Attributes
-    ----------
-    rarity: int
-        The chance of this Pokémon holding this item in this version.
-    version: NamedResource
-        The version that this item is held in by the Pokémon.
-    """
-
-    rarity: int = attrs.field(factory=int)
-    version: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ItemHolderPokemonVersionDetail":
-        return cls(
-            rarity=payload.get("rarity", 0),
-            version=NamedResource.from_payload(payload.get("version", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class ItemHolderPokemon(BaseModel):
-    """An item holder pokemon resource.
-
-    Attributes
-    ----------
-    pokemon: str
-        The Pokémon that holds this item.
-    version_details: t.List[ItemHolderPokemonVersionDetail]
-        The details for the version that this item is held in by the Pokémon.
-    """
-
-    pokemon: NamedResource = attrs.field(factory=NamedResource)
-    version_details: t.List["ItemHolderPokemonVersionDetail"] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ItemHolderPokemon":
-        return cls(
-            pokemon=NamedResource.from_payload(payload.get("pokemon", {}) or {}),
-            version_details=[
-                ItemHolderPokemonVersionDetail.from_payload(version_detail)
-                for version_detail in payload.get("version_details", [])
-            ],
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import NamedResource
+
+__all__: t.Tuple[str, ...] = (
+    "ItemSprites",
+    "ItemHolderPokemon",
+    "ItemHolderPokemonVersionDetail",
+)
+
+
+@attrs.define(slots=True, kw_only=True)
+class ItemSprites(BaseModel):
+    """An item sprites resource.
+
+    Attributes
+    ----------
+    default: str
+        The default depiction of this item.
+    """
+
+    default: str = attrs.field(factory=str)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, str]) -> "ItemSprites":
+        return cls(default=payload.get("default", ""))
+
+
+@attrs.define(slots=True, kw_only=True)
+class ItemHolderPokemonVersionDetail(BaseModel):
+    """An item holder pokemon version detail resource.
+
+    Attributes
+    ----------
+    rarity: int
+        The chance of this Pokémon holding this item in this version.
+    version: NamedResource
+        The version that this item is held in by the Pokémon.
+    """
+
+    rarity: int = attrs.field(factory=int)
+    version: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ItemHolderPokemonVersionDetail":
+        return cls(
+            rarity=payload.get("rarity", 0),
+            version=NamedResource.from_payload(payload.get("version", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class ItemHolderPokemon(BaseModel):
+    """An item holder pokemon resource.
+
+    Attributes
+    ----------
+    pokemon: str
+        The Pokémon that holds this item.
+    version_details: t.List[ItemHolderPokemonVersionDetail]
+        The details for the version that this item is held in by the Pokémon.
+    """
+
+    pokemon: NamedResource = attrs.field(factory=NamedResource)
+    version_details: t.List["ItemHolderPokemonVersionDetail"] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ItemHolderPokemon":
+        return cls(
+            pokemon=NamedResource.from_payload(payload.get("pokemon", {}) or {}),
+            version_details=[
+                ItemHolderPokemonVersionDetail.from_payload(version_detail)
+                for version_detail in payload.get("version_details", [])
+            ],
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/utils/locations.py` & `pokelance-0.1.0/pokelance/models/abstract/utils/locations.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import NamedResource
-
-__all__: t.Tuple[str, ...] = (
-    "EncounterVersionDetails",
-    "EncounterMethodRate",
-    "PokemonEncounter",
-    "PalParkEncounterSpecies",
-)
-
-
-@attrs.define(slots=True, kw_only=True)
-class EncounterVersionDetails(BaseModel):
-    """An encounter version details resource.
-
-    Attributes
-    ----------
-    rate: int
-        The chance of an encounter to occur.
-    version: NamedResource
-        The version of this encounter.
-    """
-
-    rate: int = attrs.field(factory=int)
-    version: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EncounterVersionDetails":
-        return cls(
-            rate=payload.get("rate", 0),
-            version=NamedResource.from_payload(payload.get("version", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class EncounterMethodRate(BaseModel):
-    """An encounter method rate resource.
-
-    Attributes
-    ----------
-    encounter_method: NamedResource
-        The method in which Pokémon may be encountered in an area.
-    version_details: t.List[EncounterVersionDetails]
-        A list of version details for the encounter.
-    """
-
-    encounter_method: NamedResource = attrs.field(factory=NamedResource)
-    version_details: t.List[EncounterVersionDetails] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EncounterMethodRate":
-        return cls(
-            encounter_method=NamedResource.from_payload(payload.get("encounter_method", {}) or {}),
-            version_details=[EncounterVersionDetails.from_payload(i) for i in payload.get("version_details", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonEncounter(BaseModel):
-    """A pokemon encounter resource.
-
-    Attributes
-    ----------
-    pokemon: NamedResource
-        The Pokémon being encountered.
-    version_details: t.List[EncounterVersionDetails]
-        A list of versions and encounters with Pokémon that might happen.
-    """
-
-    pokemon: NamedResource = attrs.field(factory=NamedResource)
-    version_details: t.List[EncounterVersionDetails] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonEncounter":
-        return cls(
-            pokemon=NamedResource.from_payload(payload.get("pokemon", {}) or {}),
-            version_details=[EncounterVersionDetails.from_payload(i) for i in payload.get("version_details", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PalParkEncounterSpecies(BaseModel):
-    """A pal park encounter species resource.
-
-    Attributes
-    ----------
-    base_score: int
-        The base score given to the player when this Pokémon is caught during a pal park run.
-    rate: int
-        The base rate for encountering this Pokémon in pal park.
-    pokemon_species: NamedResource
-        The Pokémon species being encountered.
-    """
-
-    base_score: int = attrs.field(factory=int)
-    rate: int = attrs.field(factory=int)
-    pokemon_species: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PalParkEncounterSpecies":
-        return cls(
-            base_score=payload.get("base_score", 0),
-            rate=payload.get("rate", 0),
-            pokemon_species=NamedResource.from_payload(payload.get("pokemon_species", {}) or {}),
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import NamedResource
+
+__all__: t.Tuple[str, ...] = (
+    "EncounterVersionDetails",
+    "EncounterMethodRate",
+    "PokemonEncounter",
+    "PalParkEncounterSpecies",
+)
+
+
+@attrs.define(slots=True, kw_only=True)
+class EncounterVersionDetails(BaseModel):
+    """An encounter version details resource.
+
+    Attributes
+    ----------
+    rate: int
+        The chance of an encounter to occur.
+    version: NamedResource
+        The version of this encounter.
+    """
+
+    rate: int = attrs.field(factory=int)
+    version: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EncounterVersionDetails":
+        return cls(
+            rate=payload.get("rate", 0),
+            version=NamedResource.from_payload(payload.get("version", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class EncounterMethodRate(BaseModel):
+    """An encounter method rate resource.
+
+    Attributes
+    ----------
+    encounter_method: NamedResource
+        The method in which Pokémon may be encountered in an area.
+    version_details: t.List[EncounterVersionDetails]
+        A list of version details for the encounter.
+    """
+
+    encounter_method: NamedResource = attrs.field(factory=NamedResource)
+    version_details: t.List[EncounterVersionDetails] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "EncounterMethodRate":
+        return cls(
+            encounter_method=NamedResource.from_payload(payload.get("encounter_method", {}) or {}),
+            version_details=[EncounterVersionDetails.from_payload(i) for i in payload.get("version_details", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonEncounter(BaseModel):
+    """A pokemon encounter resource.
+
+    Attributes
+    ----------
+    pokemon: NamedResource
+        The Pokémon being encountered.
+    version_details: t.List[EncounterVersionDetails]
+        A list of versions and encounters with Pokémon that might happen.
+    """
+
+    pokemon: NamedResource = attrs.field(factory=NamedResource)
+    version_details: t.List[EncounterVersionDetails] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonEncounter":
+        return cls(
+            pokemon=NamedResource.from_payload(payload.get("pokemon", {}) or {}),
+            version_details=[EncounterVersionDetails.from_payload(i) for i in payload.get("version_details", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PalParkEncounterSpecies(BaseModel):
+    """A pal park encounter species resource.
+
+    Attributes
+    ----------
+    base_score: int
+        The base score given to the player when this Pokémon is caught during a pal park run.
+    rate: int
+        The base rate for encountering this Pokémon in pal park.
+    pokemon_species: NamedResource
+        The Pokémon species being encountered.
+    """
+
+    base_score: int = attrs.field(factory=int)
+    rate: int = attrs.field(factory=int)
+    pokemon_species: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PalParkEncounterSpecies":
+        return cls(
+            base_score=payload.get("base_score", 0),
+            rate=payload.get("rate", 0),
+            pokemon_species=NamedResource.from_payload(payload.get("pokemon_species", {}) or {}),
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/utils/moves.py` & `pokelance-0.1.0/pokelance/models/abstract/utils/moves.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import NamedResource
-
-__all__: t.Tuple[str, ...] = (
-    "ContestComboSet",
-    "ContestComboDetail",
-    "MoveFlavorText",
-    "MoveMetaData",
-    "MoveStatChange",
-    "PastMoveStatValues",
-)
-
-
-@attrs.define(slots=True, kw_only=True)
-class ContestComboDetail(BaseModel):
-    """A contest combo detail resource.
-
-    Attributes
-    ----------
-    use_before: NamedResource
-        A detail of moves this move can be used before, i.e. leading into this move.
-    use_after: NamedResource
-        A detail of moves this move can be used after, i.e. result in this move being used.
-    """
-
-    use_before: t.List[NamedResource] = attrs.field(factory=list)
-    use_after: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ContestComboDetail":
-        return cls(
-            use_before=[NamedResource.from_payload(i or {}) for i in (payload.get("use_before", []) or [])],
-            use_after=[NamedResource.from_payload(i or {}) for i in (payload.get("use_after", []) or [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class ContestComboSet(BaseModel):
-    """A contest combo set resource.
-
-    Attributes
-    ----------
-    normal: ContestComboDetail
-        A detail of normal moves in a contest combo.
-    super_: ContestComboDetail
-        A detail of super moves in a contest combo.
-    """
-
-    normal: ContestComboDetail = attrs.field(factory=ContestComboDetail)
-    super_: ContestComboDetail = attrs.field(factory=ContestComboDetail)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ContestComboSet":
-        return cls(
-            normal=ContestComboDetail.from_payload(payload.get("normal", {})),
-            super_=ContestComboDetail.from_payload(payload.get("super", {})),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class MoveFlavorText(BaseModel):
-    """A move flavor text resource.
-
-    Attributes
-    ----------
-    flavor_text: str
-        The localized flavor text for an api resource in a specific language.
-    language: NamedResource
-        The language this name is in.
-    version_group: NamedResource
-        The version group that uses this flavor text.
-    """
-
-    flavor_text: str = attrs.field(factory=str)
-    language: NamedResource = attrs.field(factory=NamedResource)
-    version_group: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveFlavorText":
-        return cls(
-            flavor_text=payload.get("flavor_text", ""),
-            language=NamedResource.from_payload(payload.get("language", {}) or {}),
-            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class MoveMetaData(BaseModel):
-    """A move meta data resource.
-
-    Attributes
-    ----------
-    ailment: NamedResource
-        The status ailment this move inflicts on its target.
-    category: NamedResource
-        The category of move this move falls under, e.g. damage or ailment.
-    min_hits: int
-        The minimum number of times this move hits. Null if it always only hits once.
-    max_hits: int
-        The maximum number of times this move hits. Null if it always only hits once.
-    min_turns: int
-        The minimum number of turns this move continues to take effect. Null if it always only lasts one turn.
-    max_turns: int
-        The maximum number of turns this move continues to take effect. Null if it always only lasts one turn.
-    drain: int
-        HP drain (if positive) or Recoil damage (if negative), in percent of damage done.
-    healing: int
-        The amount of hp gained by the attacking Pokemon, in percent of it's maximum HP.
-    crit_rate: int
-        Critical hit rate bonus.
-    ailment_chance: int
-        The likelihood this attack will cause an ailment.
-    flinch_chance: int
-        The likelihood this attack will cause the target Pokémon to flinch.
-    stat_chance: int
-        The likelihood this attack will cause a stat change in the target Pokémon.
-    """
-
-    ailment: NamedResource = attrs.field(factory=NamedResource)
-    category: NamedResource = attrs.field(factory=NamedResource)
-    min_hits: int = attrs.field(factory=int)
-    max_hits: int = attrs.field(factory=int)
-    min_turns: int = attrs.field(factory=int)
-    max_turns: int = attrs.field(factory=int)
-    drain: int = attrs.field(factory=int)
-    healing: int = attrs.field(factory=int)
-    crit_rate: int = attrs.field(factory=int)
-    ailment_chance: int = attrs.field(factory=int)
-    flinch_chance: int = attrs.field(factory=int)
-    stat_chance: int = attrs.field(factory=int)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveMetaData":
-        return cls(
-            ailment=NamedResource.from_payload(payload.get("ailment", {}) or {}),
-            category=NamedResource.from_payload(payload.get("category", {}) or {}),
-            min_hits=payload.get("min_hits", 0) or 1,
-            max_hits=payload.get("max_hits", 0) or 1,
-            min_turns=payload.get("min_turns", 0) or 1,
-            max_turns=payload.get("max_turns", 0) or 1,
-            drain=payload.get("drain", 0),
-            healing=payload.get("healing", 0),
-            crit_rate=payload.get("crit_rate", 0),
-            ailment_chance=payload.get("ailment_chance", 0),
-            flinch_chance=payload.get("flinch_chance", 0),
-            stat_chance=payload.get("stat_chance", 0),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class MoveStatChange(BaseModel):
-    change: int = attrs.field(factory=int)
-    stat: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveStatChange":
-        return cls(
-            change=payload.get("change", 0),
-            stat=NamedResource.from_payload(payload.get("stat", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PastMoveStatValues(BaseModel):
-    accuracy: int = attrs.field(factory=int)
-    effect_chance: int = attrs.field(factory=int)
-    power: int = attrs.field(factory=int)
-    pp: int = attrs.field(factory=int)
-    effect_entries: t.List[NamedResource] = attrs.field(factory=list)
-    type: NamedResource = attrs.field(factory=NamedResource)
-    version_group: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PastMoveStatValues":
-        return cls(
-            accuracy=payload.get("accuracy", 0),
-            effect_chance=payload.get("effect_chance", 0),
-            power=payload.get("power", 0),
-            pp=payload.get("pp", 0),
-            effect_entries=[NamedResource.from_payload(i) for i in payload.get("effect_entries", [])],
-            type=NamedResource.from_payload(payload.get("type", {})),
-            version_group=NamedResource.from_payload(payload.get("version_group", {})),
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import NamedResource
+
+__all__: t.Tuple[str, ...] = (
+    "ContestComboSet",
+    "ContestComboDetail",
+    "MoveFlavorText",
+    "MoveMetaData",
+    "MoveStatChange",
+    "PastMoveStatValues",
+)
+
+
+@attrs.define(slots=True, kw_only=True)
+class ContestComboDetail(BaseModel):
+    """A contest combo detail resource.
+
+    Attributes
+    ----------
+    use_before: NamedResource
+        A detail of moves this move can be used before, i.e. leading into this move.
+    use_after: NamedResource
+        A detail of moves this move can be used after, i.e. result in this move being used.
+    """
+
+    use_before: t.List[NamedResource] = attrs.field(factory=list)
+    use_after: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ContestComboDetail":
+        return cls(
+            use_before=[NamedResource.from_payload(i or {}) for i in (payload.get("use_before", []) or [])],
+            use_after=[NamedResource.from_payload(i or {}) for i in (payload.get("use_after", []) or [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class ContestComboSet(BaseModel):
+    """A contest combo set resource.
+
+    Attributes
+    ----------
+    normal: ContestComboDetail
+        A detail of normal moves in a contest combo.
+    super_: ContestComboDetail
+        A detail of super moves in a contest combo.
+    """
+
+    normal: ContestComboDetail = attrs.field(factory=ContestComboDetail)
+    super_: ContestComboDetail = attrs.field(factory=ContestComboDetail)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "ContestComboSet":
+        return cls(
+            normal=ContestComboDetail.from_payload(payload.get("normal", {}) or {}),
+            super_=ContestComboDetail.from_payload(payload.get("super", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class MoveFlavorText(BaseModel):
+    """A move flavor text resource.
+
+    Attributes
+    ----------
+    flavor_text: str
+        The localized flavor text for an api resource in a specific language.
+    language: NamedResource
+        The language this name is in.
+    version_group: NamedResource
+        The version group that uses this flavor text.
+    """
+
+    flavor_text: str = attrs.field(factory=str)
+    language: NamedResource = attrs.field(factory=NamedResource)
+    version_group: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveFlavorText":
+        return cls(
+            flavor_text=payload.get("flavor_text", ""),
+            language=NamedResource.from_payload(payload.get("language", {}) or {}),
+            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class MoveMetaData(BaseModel):
+    """A move meta data resource.
+
+    Attributes
+    ----------
+    ailment: NamedResource
+        The status ailment this move inflicts on its target.
+    category: NamedResource
+        The category of move this move falls under, e.g. damage or ailment.
+    min_hits: int
+        The minimum number of times this move hits. Null if it always only hits once.
+    max_hits: int
+        The maximum number of times this move hits. Null if it always only hits once.
+    min_turns: int
+        The minimum number of turns this move continues to take effect. Null if it always only lasts one turn.
+    max_turns: int
+        The maximum number of turns this move continues to take effect. Null if it always only lasts one turn.
+    drain: int
+        HP drain (if positive) or Recoil damage (if negative), in percent of damage done.
+    healing: int
+        The amount of hp gained by the attacking Pokemon, in percent of it's maximum HP.
+    crit_rate: int
+        Critical hit rate bonus.
+    ailment_chance: int
+        The likelihood this attack will cause an ailment.
+    flinch_chance: int
+        The likelihood this attack will cause the target Pokémon to flinch.
+    stat_chance: int
+        The likelihood this attack will cause a stat change in the target Pokémon.
+    """
+
+    ailment: NamedResource = attrs.field(factory=NamedResource)
+    category: NamedResource = attrs.field(factory=NamedResource)
+    min_hits: int = attrs.field(factory=int)
+    max_hits: int = attrs.field(factory=int)
+    min_turns: int = attrs.field(factory=int)
+    max_turns: int = attrs.field(factory=int)
+    drain: int = attrs.field(factory=int)
+    healing: int = attrs.field(factory=int)
+    crit_rate: int = attrs.field(factory=int)
+    ailment_chance: int = attrs.field(factory=int)
+    flinch_chance: int = attrs.field(factory=int)
+    stat_chance: int = attrs.field(factory=int)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveMetaData":
+        return cls(
+            ailment=NamedResource.from_payload(payload.get("ailment", {}) or {}),
+            category=NamedResource.from_payload(payload.get("category", {}) or {}),
+            min_hits=payload.get("min_hits", 0) or 1,
+            max_hits=payload.get("max_hits", 0) or 1,
+            min_turns=payload.get("min_turns", 0) or 1,
+            max_turns=payload.get("max_turns", 0) or 1,
+            drain=payload.get("drain", 0),
+            healing=payload.get("healing", 0),
+            crit_rate=payload.get("crit_rate", 0),
+            ailment_chance=payload.get("ailment_chance", 0),
+            flinch_chance=payload.get("flinch_chance", 0),
+            stat_chance=payload.get("stat_chance", 0),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class MoveStatChange(BaseModel):
+    change: int = attrs.field(factory=int)
+    stat: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveStatChange":
+        return cls(
+            change=payload.get("change", 0),
+            stat=NamedResource.from_payload(payload.get("stat", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PastMoveStatValues(BaseModel):
+    accuracy: int = attrs.field(factory=int)
+    effect_chance: int = attrs.field(factory=int)
+    power: int = attrs.field(factory=int)
+    pp: int = attrs.field(factory=int)
+    effect_entries: t.List[NamedResource] = attrs.field(factory=list)
+    type: NamedResource = attrs.field(factory=NamedResource)
+    version_group: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PastMoveStatValues":
+        return cls(
+            accuracy=payload.get("accuracy", 0),
+            effect_chance=payload.get("effect_chance", 0),
+            power=payload.get("power", 0),
+            pp=payload.get("pp", 0),
+            effect_entries=[NamedResource.from_payload(i) for i in payload.get("effect_entries", [])],
+            type=NamedResource.from_payload(payload.get("type", {}) or {}),
+            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
+        )
```

### Comparing `pokelance-0.0.9a0/pokelance/models/abstract/utils/pokemons.py` & `pokelance-0.1.0/pokelance/models/abstract/utils/pokemons.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1253 +1,1253 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-from pokelance.models.common import Effect, NamedResource
-
-__all__: t.Tuple[str, ...] = (
-    "AbilityEffectChange",
-    "AbilityFlavorText",
-    "AbilityPokemon",
-    "PokemonSpeciesGender",
-    "GrowthRateExperienceLevel",
-    "NatureStatChange",
-    "MoveBattleStylePreference",
-    "NaturePokeathlonStatAffect",
-    "NaturePokeathlonStatAffectSet",
-    "PokemonMoveVersion",
-    "PokemonStat",
-    "PokemonType",
-    "PokemonHeldItemVersion",
-    "PokemonHeldItem",
-    "PokemonSprite",
-    "PokemonAbility",
-    "PokemonMove",
-    "PokemonTypePast",
-    "PokemonFormType",
-    "PokemonFormSprites",
-    "AwesomeName",
-    "PokemonSpeciesVariety",
-    "PokemonSpeciesDexEntry",
-    "PalParkEncounterArea",
-    "Genus",
-    "MoveStatAffectSets",
-    "NatureStatAffectSets",
-    "MoveStatEffect",
-    "TypeRelations",
-    "TypePokemon",
-    "TypeRelationsPast",
-)
-
-
-@attrs.define(kw_only=True, slots=True)
-class BaseSprite(BaseModel):
-    """A pokemon sprite resource.
-
-    Attributes
-    ----------
-    front_default: str
-        The default depiction of this pokemon from the front in battle.
-    front_shiny: str
-        The shiny depiction of this pokemon from the front in battle.
-    front_female: str
-        The default depiction of female gender of this pokemon from the front in battle.
-    front_shiny_female: str
-        The shiny depiction of female gender of this pokemon from the front in battle.
-    back_default: str
-        The default depiction of this pokemon from the back in battle.
-    back_shiny: str
-        The shiny depiction of this pokemon from the back in battle.
-    back_female: str
-        The default depiction of female gender of this pokemon from the back in battle.
-    back_shiny_female: str
-        The shiny depiction of female gender of this pokemon from the back in battle.
-    """
-
-    back_default: str = attrs.field(factory=str)
-    back_shiny: str = attrs.field(factory=str)
-    back_female: str = attrs.field(factory=str)
-    back_shiny_female: str = attrs.field(factory=str)
-    front_default: str = attrs.field(factory=str)
-    front_shiny: str = attrs.field(factory=str)
-    front_female: str = attrs.field(factory=str)
-    front_shiny_female: str = attrs.field(factory=str)
-
-
-@attrs.define(kw_only=True, slots=True)
-class Generation(BaseModel):
-    """A generation resource."""
-
-    ...
-
-
-@attrs.define(kw_only=True, slots=True)
-class Animated(BaseSprite):
-    """A pokemon animated sprite resource."""
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Animated":
-        return cls(
-            back_default=payload.get("back_default", ""),
-            back_shiny=payload.get("back_shiny", ""),
-            back_female=payload.get("back_female", ""),
-            back_shiny_female=payload.get("back_shiny_female", ""),
-            front_default=payload.get("front_default", ""),
-            front_shiny=payload.get("front_shiny", ""),
-            front_female=payload.get("front_female", ""),
-            front_shiny_female=payload.get("front_shiny_female", ""),
-        )
-
-
-@attrs.define(kw_only=True, slots=True)
-class VersionSprite(BaseSprite):
-    """A pokemon version sprite resource.
-
-    Attributes
-    ----------
-    back_gray: str
-        The gray depiction of this pokemon from the back in battle.
-    front_gray: str
-        The gray depiction of this pokemon from the front in battle.
-    back_transperent: str
-        The transparent depiction of this pokemon from the back in battle.
-    front_transperent: str
-        The transparent depiction of this pokemon from the front in battle.
-    animated: Animated
-        The animated depiction of this pokemon.
-    """
-
-    back_gray: str = attrs.field(factory=str)
-    back_transperent: str = attrs.field(factory=str)
-    back_shiny_transperent: str = attrs.field(factory=str)
-    front_gray: str = attrs.field(factory=str)
-    front_transperent: str = attrs.field(factory=str)
-    front_shiny_transperent: str = attrs.field(factory=str)
-    animated: Animated = attrs.field(factory=Animated)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "VersionSprite":
-        return cls(
-            back_default=payload.get("back_default", ""),
-            back_gray=payload.get("back_gray", ""),
-            back_shiny=payload.get("back_shiny", ""),
-            back_transperent=payload.get("back_transperent", ""),
-            back_shiny_transperent=payload.get("back_shiny_transperent", ""),
-            back_female=payload.get("back_female", ""),
-            back_shiny_female=payload.get("back_shiny_female", ""),
-            front_default=payload.get("front_default", ""),
-            front_shiny=payload.get("front_shiny", ""),
-            front_shiny_transperent=payload.get("front_shiny_transperent", ""),
-            front_female=payload.get("front_female", ""),
-            front_shiny_female=payload.get("front_shiny_female", ""),
-            front_gray=payload.get("front_gray", ""),
-            front_transperent=payload.get("front_transperent", ""),
-            animated=Animated.from_payload(payload.get("animated", {})),
-        )
-
-
-@attrs.define(kw_only=True, slots=True)
-class GenerationI(Generation):
-    """A generation I resource.
-
-    Attributes
-    ----------
-    red_blue: VersionSprite
-        The red-blue depiction of this pokemon.
-    yellow: VersionSprite
-        The yellow depiction of this pokemon.
-    """
-
-    red_blue: VersionSprite = attrs.field(factory=VersionSprite)
-    yellow: VersionSprite = attrs.field(factory=VersionSprite)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationI":
-        return cls(
-            red_blue=VersionSprite.from_payload(payload.get("red-blue", {})),
-            yellow=VersionSprite.from_payload(payload.get("yellow", {})),
-        )
-
-
-@attrs.define(kw_only=True, slots=True)
-class GenerationII(Generation):
-    """A generation II resource.
-
-    Attributes
-    ----------
-    crystal: VersionSprite
-        The crystal depiction of this pokemon.
-    gold: VersionSprite
-        The gold depiction of this pokemon.
-    silver: VersionSprite
-        The silver depiction of this pokemon.
-    """
-
-    crystal: VersionSprite = attrs.field(factory=VersionSprite)
-    gold: VersionSprite = attrs.field(factory=VersionSprite)
-    silver: VersionSprite = attrs.field(factory=VersionSprite)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationII":
-        return cls(
-            crystal=VersionSprite.from_payload(payload.get("crystal", {})),
-            gold=VersionSprite.from_payload(payload.get("gold", {})),
-            silver=VersionSprite.from_payload(payload.get("silver", {})),
-        )
-
-
-@attrs.define(kw_only=True, slots=True)
-class GenerationIII(Generation):
-    """A generation III resource.
-
-    Attributes
-    ----------
-    emerald: VersionSprite
-        The emerald depiction of this pokemon.
-    firered_leafgreen: VersionSprite
-        The firered-leafgreen depiction of this pokemon.
-    ruby_sapphire: VersionSprite
-        The ruby-sapphire depiction of this pokemon.
-    """
-
-    emerald: VersionSprite = attrs.field(factory=VersionSprite)
-    firered_leafgreen: VersionSprite = attrs.field(factory=VersionSprite)
-    ruby_sapphire: VersionSprite = attrs.field(factory=VersionSprite)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationIII":
-        return cls(
-            emerald=VersionSprite.from_payload(payload.get("emerald", {})),
-            firered_leafgreen=VersionSprite.from_payload(payload.get("firered-leafgreen", {})),
-            ruby_sapphire=VersionSprite.from_payload(payload.get("ruby-sapphire", {})),
-        )
-
-
-@attrs.define(kw_only=True, slots=True)
-class GenerationIV(Generation):
-    """A generation IV resource.
-
-    Attributes
-    ----------
-    diamond_pearl: VersionSprite
-        The diamond-pearl depiction of this pokemon.
-    heartgold_soulsilver: VersionSprite
-        The heartgold-soulsilver depiction of this pokemon.
-    platinum: VersionSprite
-        The platinum depiction of this pokemon.
-    """
-
-    diamond_pearl: VersionSprite = attrs.field(factory=VersionSprite)
-    heartgold_soulsilver: VersionSprite = attrs.field(factory=VersionSprite)
-    platinum: VersionSprite = attrs.field(factory=VersionSprite)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationIV":
-        return cls(
-            diamond_pearl=VersionSprite.from_payload(payload.get("diamond-pearl", {})),
-            heartgold_soulsilver=VersionSprite.from_payload(payload.get("heartgold-soulsilver", {})),
-            platinum=VersionSprite.from_payload(payload.get("platinum", {})),
-        )
-
-
-@attrs.define(kw_only=True, slots=True)
-class GenerationV(Generation):
-    """A generation V resource.
-
-    Attributes
-    ----------
-    black_white: VersionSprite
-        The black-white depiction of this pokemon.
-    """
-
-    black_white: VersionSprite = attrs.field(factory=VersionSprite)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationV":
-        return cls(
-            black_white=VersionSprite.from_payload(payload.get("black-white", {})),
-        )
-
-
-@attrs.define(kw_only=True, slots=True)
-class GenerationVI(Generation):
-    """A generation VI resource.
-
-    Attributes
-    ----------
-    omegaruby_alphasapphire: VersionSprite
-        The omegaruby-alphasapphire depiction of this pokemon.
-    x_y: VersionSprite
-        The x-y depiction of this pokemon.
-    """
-
-    omegaruby_alphasapphire: VersionSprite = attrs.field(factory=VersionSprite)
-    x_y: VersionSprite = attrs.field(factory=VersionSprite)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationVI":
-        return cls(
-            omegaruby_alphasapphire=VersionSprite.from_payload(payload.get("omegaruby-alphasapphire", {})),
-            x_y=VersionSprite.from_payload(payload.get("x-y", {})),
-        )
-
-
-@attrs.define(kw_only=True, slots=True)
-class GenerationVII(Generation):
-    """A generation VII resource.
-
-    Attributes
-    ----------
-    icons: VersionSprite
-        The icons depiction of this pokemon.
-    ultra_sun_ultra_moon: VersionSprite
-        The ultra-sun-ultra-moon depiction of this pokemon.
-    """
-
-    icons: VersionSprite = attrs.field(factory=VersionSprite)
-    ultra_sun_ultra_moon: VersionSprite = attrs.field(factory=VersionSprite)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationVII":
-        return cls(
-            icons=VersionSprite.from_payload(payload.get("icons", {})),
-            ultra_sun_ultra_moon=VersionSprite.from_payload(payload.get("ultra-sun-ultra-moon", {})),
-        )
-
-
-@attrs.define(kw_only=True, slots=True)
-class GenerationVIII(Generation):
-    """A generation VIII resource.
-
-    Attributes
-    ----------
-    icons: VersionSprite
-        The icons depiction of this pokemon.
-    """
-
-    icons: VersionSprite = attrs.field(factory=VersionSprite)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationVIII":
-        return cls(
-            icons=VersionSprite.from_payload(payload.get("icons", {})),
-        )
-
-
-@attrs.define(kw_only=True, slots=True)
-class Versions(BaseModel):
-    """A sprite resource for all generations.
-
-    Attributes
-    ----------
-    generation_i: GenerationI
-        The generation I depiction of this pokemon.
-    generation_ii: GenerationII
-        The generation II depiction of this pokemon.
-    generation_iii: GenerationIII
-        The generation III depiction of this pokemon.
-    generation_iv: GenerationIV
-        The generation IV depiction of this pokemon.
-    generation_v: GenerationV
-        The generation V depiction of this pokemon.
-    generation_vi: GenerationVI
-        The generation VI depiction of this pokemon.
-    generation_vii: GenerationVII
-        The generation VII depiction of this pokemon.
-    generation_viii: GenerationVIII
-        The generation VIII depiction of this pokemon.
-    """
-
-    generation_i: GenerationI = attrs.field(factory=GenerationI)
-    generation_ii: GenerationII = attrs.field(factory=GenerationII)
-    generation_iii: GenerationIII = attrs.field(factory=GenerationIII)
-    generation_iv: GenerationIV = attrs.field(factory=GenerationIV)
-    generation_v: GenerationV = attrs.field(factory=GenerationV)
-    generation_vi: GenerationVI = attrs.field(factory=GenerationVI)
-    generation_vii: GenerationVII = attrs.field(factory=GenerationVII)
-    generation_viii: GenerationVIII = attrs.field(factory=GenerationVIII)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Versions":
-        return cls(
-            generation_i=GenerationI.from_payload(payload.get("generation-i", {})),
-            generation_ii=GenerationII.from_payload(payload.get("generation-ii", {})),
-            generation_iii=GenerationIII.from_payload(payload.get("generation-iii", {})),
-            generation_iv=GenerationIV.from_payload(payload.get("generation-iv", {})),
-            generation_v=GenerationV.from_payload(payload.get("generation-v", {})),
-            generation_vi=GenerationVI.from_payload(payload.get("generation-vi", {})),
-            generation_vii=GenerationVII.from_payload(payload.get("generation-vii", {})),
-            generation_viii=GenerationVIII.from_payload(payload.get("generation-viii", {})),
-        )
-
-
-@attrs.define(kw_only=True, slots=True)
-class DreamWorld(BaseModel):
-    """A dream world resource.
-
-    Attributes
-    ----------
-    front_default: str
-        The default depiction of this pokemon.
-    front_female: str
-        The female depiction of this pokemon.
-    """
-
-    front_default: str = attrs.field(factory=str)
-    front_female: str = attrs.field(factory=str)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "DreamWorld":
-        return cls(
-            front_default=payload.get("front_default", ""),
-            front_female=payload.get("front_female", ""),
-        )
-
-
-@attrs.define(kw_only=True, slots=True)
-class Home(BaseModel):
-    """A home resource.
-
-    Attributes
-    ----------
-    front_default: str
-        The default depiction of this pokemon.
-    front_female: str
-        The female depiction of this pokemon.
-    front_shiny: str
-        The shiny depiction of this pokemon.
-    front_shiny_female: str
-        The shiny female depiction of this pokemon.
-    """
-
-    front_default: str = attrs.field(factory=str)
-    front_female: str = attrs.field(factory=str)
-    front_shiny: str = attrs.field(factory=str)
-    front_shiny_female: str = attrs.field(factory=str)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Home":
-        return cls(
-            front_default=payload.get("front_default", ""),
-            front_female=payload.get("front_female", ""),
-            front_shiny=payload.get("front_shiny", ""),
-            front_shiny_female=payload.get("front_shiny_female", ""),
-        )
-
-
-@attrs.define(kw_only=True, slots=True)
-class OfficialArtwork(BaseModel):
-    """Official artwork for this Pokémon from Nintendo.
-
-    Attributes
-    ----------
-    front_default: str
-        The default depiction of this Pokémon from the official artwork.
-    front_shiny: str
-        The shiny depiction of this Pokémon from the official artwork.
-    """
-
-    front_default: str = attrs.field(factory=str)
-    front_shiny: str = attrs.field(factory=str)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "OfficialArtwork":
-        return cls(
-            front_default=payload.get("front_default", ""),
-            front_shiny=payload.get("front_shiny", ""),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Other(BaseModel):
-    """Other sprites for this pokemon
-
-    Attributes
-    ----------
-    dream_world: DreamWorld
-        The dream world sprites for this pokemon
-    home: Home
-        The home sprites for this pokemon
-    official_artwork: OfficialArtwork
-        The official artwork sprites for this pokemon
-    """
-
-    dream_world: DreamWorld = attrs.field(factory=DreamWorld)
-    home: Home = attrs.field(factory=Home)
-    official_artwork: OfficialArtwork = attrs.field(factory=OfficialArtwork)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Other":
-        return cls(
-            dream_world=DreamWorld.from_payload(payload.get("dream_world", {})),
-            home=Home.from_payload(payload.get("home", {})),
-            official_artwork=OfficialArtwork.from_payload(payload.get("official-artwork", {})),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class AbilityEffectChange(BaseModel):
-    """An ability effect change resource.
-
-    Attributes
-    ----------
-    effect_entries: t.List[Effect]
-        The previous effect of this ability listed in different languages.
-    version_group: NamedResource
-        The version group in which the previous effect of this ability originated.
-    """
-
-    effect_entries: t.List[Effect] = attrs.field(factory=list)
-    version_group: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "AbilityEffectChange":
-        return cls(
-            effect_entries=[Effect.from_payload(i) for i in payload.get("effect_entries", [])],
-            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class AbilityFlavorText(BaseModel):
-    """An ability flavor text resource.
-
-    Attributes
-    ----------
-    flavor_text: str
-        The localized flavor text for an api resource in a specific language.
-    language: NamedResource
-        The language this name is in.
-    version_group: NamedResource
-        The version group that uses this flavor text.
-    """
-
-    flavor_text: str = attrs.field(factory=str)
-    language: NamedResource = attrs.field(factory=NamedResource)
-    version_group: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "AbilityFlavorText":
-        return cls(
-            flavor_text=payload.get("flavor_text", ""),
-            language=NamedResource.from_payload(payload.get("language", {}) or {}),
-            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class AbilityPokemon(BaseModel):
-    """An ability pokemon resource.
-
-    Attributes
-    ----------
-    is_hidden: bool
-        Whether or not this a hidden ability for the referenced pokemon.
-    slot: int
-        The slot this ability occupies in this pokemon species.
-    pokemon: NamedResource
-        The pokemon this ability could belong to.
-    """
-
-    is_hidden: bool = attrs.field(factory=bool)
-    slot: int = attrs.field(factory=int)
-    pokemon: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "AbilityPokemon":
-        return cls(
-            is_hidden=payload.get("is_hidden", False),
-            slot=payload.get("slot", 0),
-            pokemon=NamedResource.from_payload(payload.get("pokemon", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonSpeciesGender(BaseModel):
-    """A pokemon species gender resource.
-
-    Attributes
-    ----------
-    rate: int
-        The chance of a particular gender in this pokemon species.
-    pokemon_species: NamedResource
-        The pokemon species here.
-    """
-
-    rate: int = attrs.field(factory=int)
-    pokemon_species: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonSpeciesGender":
-        return cls(
-            rate=payload.get("rate", 0),
-            pokemon_species=NamedResource.from_payload(payload.get("pokemon_species", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class GrowthRateExperienceLevel(BaseModel):
-    """A growth rate experience level resource.
-
-    Attributes
-    ----------
-    level: int
-        The level gained.
-    experience: int
-        The amount of experience required to reach the referenced level.
-    """
-
-    level: int = attrs.field(factory=int)
-    experience: int = attrs.field(factory=int)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GrowthRateExperienceLevel":
-        return cls(
-            level=payload.get("level", 0),
-            experience=payload.get("experience", 0),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class NatureStatChange(BaseModel):
-    """A nature stat change resource.
-
-    Attributes
-    ----------
-    max_change: int
-        The maximum amount of change to the referenced stat.
-    pokeathlon_stat: NamedResource
-        The stat being affected.
-    """
-
-    max_change: int = attrs.field(factory=int)
-    pokeathlon_stat: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "NatureStatChange":
-        return cls(
-            max_change=payload.get("max_change", 0),
-            pokeathlon_stat=NamedResource.from_payload(payload.get("pokeathlon_stat", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class MoveBattleStylePreference(BaseModel):
-    """A move battle style preference resource.
-
-    Attributes
-    ----------
-    low_hp_preference: int
-        Chance of using the move, in percent, if HP is under one half.
-    high_hp_preference: int
-        Chance of using the move, in percent, if HP is over one half.
-    move_battle_style: NamedResource
-        The move battle style.
-    """
-
-    low_hp_preference: int = attrs.field(factory=int)
-    high_hp_preference: int = attrs.field(factory=int)
-    move_battle_style: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveBattleStylePreference":
-        return cls(
-            low_hp_preference=payload.get("low_hp_preference", 0),
-            high_hp_preference=payload.get("high_hp_preference", 0),
-            move_battle_style=NamedResource.from_payload(payload.get("battle_style", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class NaturePokeathlonStatAffect(BaseModel):
-    """A nature pokeathlon stat affect resource.
-
-    Attributes
-    ----------
-    max_change: int
-        The maximum amount of change to the referenced stat.
-    nature: NamedResource
-        The nature causing the change.
-    """
-
-    max_change: int = attrs.field(factory=int)
-    nature: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "NaturePokeathlonStatAffect":
-        return cls(
-            max_change=payload.get("max_change", 0),
-            nature=NamedResource.from_payload(payload.get("nature", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class NaturePokeathlonStatAffectSet(BaseModel):
-    """A nature pokeathlon stat affect set resource.
-
-    Attributes
-    ----------
-    increase: t.List[NaturePokeathlonStatAffect]
-        A list of natures and how they change the referenced pokeathlon stat.
-    decrease: t.List[NaturePokeathlonStatAffect]
-        A list of natures and how they change the referenced pokeathlon stat.
-    """
-
-    increase: t.List[NaturePokeathlonStatAffect] = attrs.field(factory=list)
-    decrease: t.List[NaturePokeathlonStatAffect] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "NaturePokeathlonStatAffectSet":
-        return cls(
-            increase=[NaturePokeathlonStatAffect.from_payload(i) for i in payload.get("increase", [])],
-            decrease=[NaturePokeathlonStatAffect.from_payload(i) for i in payload.get("decrease", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonAbility(BaseModel):
-    """A pokemon ability resource.
-
-    Attributes
-    ----------
-    is_hidden: bool
-        Whether or not this is a hidden ability.
-    slot: int
-        The slot this ability occupies in this pokemon species.
-    ability: NamedResource
-        The ability the pokemon may have.
-    """
-
-    is_hidden: bool = attrs.field(factory=bool)
-    slot: int = attrs.field(factory=int)
-    ability: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonAbility":
-        return cls(
-            is_hidden=payload.get("is_hidden", False),
-            slot=payload.get("slot", 0),
-            ability=NamedResource.from_payload(payload.get("ability", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonType(BaseModel):
-    """A pokemon type resource.
-
-    Attributes
-    ----------
-    slot: int
-        The order the types are listed in.
-    type: NamedResource
-        The type the referenced pokemon has.
-    """
-
-    slot: int = attrs.field(factory=int)
-    type: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonType":
-        return cls(
-            slot=payload.get("slot", 0),
-            type=NamedResource.from_payload(payload.get("type", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonFormType(BaseModel):
-    """A pokemon form type resource.
-
-    Attributes
-    ----------
-    slot: int
-        The order the types are listed in.
-    type: NamedResource
-        The type the referenced pokemon has.
-    """
-
-    slot: int = attrs.field(factory=int)
-    type: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonFormType":
-        return cls(
-            slot=payload.get("slot", 0),
-            type=NamedResource.from_payload(payload.get("type", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonTypePast(BaseModel):
-    """A pokemon type past resource.
-
-    Attributes
-    ----------
-    generation: NamedResource
-        The generation this type was introduced in.
-    types: t.List[NamedResource]
-        The name of the type.
-    """
-
-    generation: NamedResource = attrs.field(factory=NamedResource)
-    types: t.List[PokemonType] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonTypePast":
-        return cls(
-            generation=NamedResource.from_payload(payload.get("generation", {}) or {}),
-            types=[PokemonType.from_payload(i) for i in payload.get("types", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonHeldItemVersion(BaseModel):
-    """A pokemon held item version resource.
-
-    Attributes
-    ----------
-    rarity: int
-        How often this item is held.
-    version: NamedResource
-        The version this item is held in by the pokemon.
-    """
-
-    version: NamedResource = attrs.field(factory=NamedResource)
-    rarity: int = attrs.field(factory=int)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonHeldItemVersion":
-        return cls(
-            version=NamedResource.from_payload(payload.get("version", {}) or {}),
-            rarity=payload.get("rarity", 0),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonHeldItem(BaseModel):
-    """A pokemon held item resource.
-
-    Attributes
-    ----------
-    item: NamedResource
-        The item the referenced pokemon holds.
-    version_details: t.List[PokemonHeldItemVersion]
-        The details for the version that this item is held in by the pokemon.
-    """
-
-    item: NamedResource = attrs.field(factory=NamedResource)
-    version_details: t.List[PokemonHeldItemVersion] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonHeldItem":
-        return cls(
-            item=NamedResource.from_payload(payload.get("item", {}) or {}),
-            version_details=[PokemonHeldItemVersion.from_payload(i) for i in payload.get("version_details", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonMoveVersion(BaseModel):
-    """A pokemon move version resource.
-
-    Attributes
-    ----------
-    move_learn_method: NamedResource
-        The method by which the move is learned.
-    version_group: NamedResource
-        The version group in which the move is learned.
-    level_learned_at: int
-        The minimum level to learn the move.
-    """
-
-    move_learn_method: NamedResource = attrs.field(factory=NamedResource)
-    version_group: NamedResource = attrs.field(factory=NamedResource)
-    level_learned_at: int = attrs.field(factory=int)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonMoveVersion":
-        return cls(
-            move_learn_method=NamedResource.from_payload(payload.get("move_learn_method", {}) or {}),
-            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
-            level_learned_at=payload.get("level_learned_at", 0),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonMove(BaseModel):
-    """A pokemon move resource.
-
-    Attributes
-    ----------
-    move: NamedResource
-        The move the referenced pokemon can learn.
-    version_group_details: t.List[PokemonMoveVersion]
-        The details for the version group that this move can be learned in.
-    """
-
-    move: NamedResource = attrs.field(factory=NamedResource)
-    version_group_details: t.List[PokemonMoveVersion] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonMove":
-        return cls(
-            move=NamedResource.from_payload(payload.get("move", {}) or {}),
-            version_group_details=[
-                PokemonMoveVersion.from_payload(i) for i in payload.get("version_group_details", [])
-            ],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonStat(BaseModel):
-    """A pokemon stat resource.
-
-    Attributes
-    ----------
-    stat: NamedResource
-        The stat the referenced pokemon has.
-    effort: int
-        The effort points (EV) the referenced pokemon has in the stat.
-    base_stat: int
-        The base value of the stat.
-    """
-
-    stat: NamedResource = attrs.field(factory=NamedResource)
-    effort: int = attrs.field(factory=int)
-    base_stat: int = attrs.field(factory=int)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonStat":
-        return cls(
-            stat=NamedResource.from_payload(payload.get("stat", {}) or {}),
-            effort=payload.get("effort", 0),
-            base_stat=payload.get("base_stat", 0),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonSprite(BaseSprite):
-    """A pokemon sprite resource.
-
-    Attributes
-    ----------
-    other: Other
-        A set of sprites used tin official artwork, home.
-    versions: Versions
-        A set of sprites used to depict this Pokémon in the game.
-    """
-
-    other: Other = attrs.field(factory=Other)
-    versions: Versions = attrs.field(factory=Versions)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonSprite":
-        return cls(
-            front_default=payload.get("front_default", ""),
-            front_shiny=payload.get("front_shiny", ""),
-            front_female=payload.get("front_female", ""),
-            front_shiny_female=payload.get("front_shiny_female", ""),
-            back_default=payload.get("back_default", ""),
-            back_shiny=payload.get("back_shiny", ""),
-            back_female=payload.get("back_female", ""),
-            back_shiny_female=payload.get("back_shiny_female", ""),
-            other=Other.from_payload(payload.get("other", {})),
-            versions=Versions.from_payload(payload.get("versions", {})),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonFormSprites(BaseModel):
-    """A pokemon form sprites resource.
-
-    Attributes
-    ----------
-    front_default: str
-        The default depiction of this pokemon form from the front in battle.
-    front_shiny: str
-        The shiny depiction of this pokemon form from the front in battle.
-    back_default: str
-        The default depiction of this pokemon form from the back in battle.
-    back_shiny: str
-        The shiny depiction of this pokemon form from the back in battle.
-    """
-
-    front_default: str = attrs.field(factory=str)
-    front_shiny: str = attrs.field(factory=str)
-    back_default: str = attrs.field(factory=str)
-    back_shiny: str = attrs.field(factory=str)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonFormSprites":
-        return cls(
-            front_default=payload.get("front_default", ""),
-            front_shiny=payload.get("front_shiny", ""),
-            back_default=payload.get("back_default", ""),
-            back_shiny=payload.get("back_shiny", ""),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class AwesomeName(BaseModel):
-    """An awesome name resource.
-
-    Attributes
-    ----------
-    awesome_name: str
-        The localized "scientific" name for an API resource in a specific language.
-    language: NamedResource
-        The language this "scientific" name is in.
-    """
-
-    awesome_name: str = attrs.field(factory=str)
-    language: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "AwesomeName":
-        return cls(
-            awesome_name=payload.get("awesome_name", ""),
-            language=NamedResource.from_payload(payload.get("language", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Genus(BaseModel):
-    """A genus resource.
-
-    Attributes
-    ----------
-    genus: str
-        The localized genus for the referenced type in the specified language.
-    language: NamedResource
-        The language this genus is in.
-    """
-
-    genus: str = attrs.field(factory=str)
-    language: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Genus":
-        return cls(
-            genus=payload.get("genus", ""),
-            language=NamedResource.from_payload(payload.get("language", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonSpeciesDexEntry(BaseModel):
-    """A pokemon species dex entry resource.
-
-    Attributes
-    ----------
-    entry_number: int
-        The index number within the Pokédex.
-    pokedex: NamedResource
-        The Pokédex the referenced Pokémon species can be found in.
-    """
-
-    entry_number: int = attrs.field(factory=int)
-    pokedex: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonSpeciesDexEntry":
-        return cls(
-            entry_number=payload.get("entry_number", 0),
-            pokedex=NamedResource.from_payload(payload.get("pokedex", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PalParkEncounterArea(BaseModel):
-    """A pal park encounter area resource.
-
-    Attributes
-    ----------
-    base_score: int
-        The base score given to the player when the referenced Pokémon is caught during a pal park run.
-    rate: int
-        The base rate for encountering the referenced Pokémon in this pal park area.
-    area: NamedResource
-        The pal park area where this encounter happens.
-    """
-
-    base_score: int = attrs.field(factory=int)
-    rate: int = attrs.field(factory=int)
-    area: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PalParkEncounterArea":
-        return cls(
-            base_score=payload.get("base_score", 0),
-            rate=payload.get("rate", 0),
-            area=NamedResource.from_payload(payload.get("area", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class PokemonSpeciesVariety(BaseModel):
-    """A pokemon species variety resource.
-
-    Attributes
-    ----------
-    is_default: bool
-        Whether this variety is the default variety.
-    pokemon: NamedResource
-        The Pokémon variety.
-    """
-
-    is_default: bool = attrs.field(factory=bool)
-    pokemon: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonSpeciesVariety":
-        return cls(
-            is_default=payload.get("is_default", False),
-            pokemon=NamedResource.from_payload(payload.get("pokemon", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class MoveStatEffect(BaseModel):
-    """A move stat effect resource.
-
-    Attributes
-    ----------
-    change: int
-        The maximum amount of change to the referenced stat.
-    stat: NamedResource
-        The stat being affected.
-    """
-
-    change: int = attrs.field(factory=int)
-    stat: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveStatEffect":
-        return cls(
-            change=payload.get("change", 0),
-            stat=NamedResource.from_payload(payload.get("stat", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class MoveStatAffectSets(BaseModel):
-    """A move stat affect sets resource.
-
-    Attributes
-    ----------
-    increase: typing.List[MoveStatAffect]
-        A list of move stat affects.
-    decrease: typing.List[MoveStatAffect]
-        A list of move stat affects.
-    """
-
-    increase: t.List[MoveStatEffect] = attrs.field(factory=list)
-    decrease: t.List[MoveStatEffect] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveStatAffectSets":
-        return cls(
-            increase=[MoveStatEffect.from_payload(i) for i in payload.get("increase", [])],
-            decrease=[MoveStatEffect.from_payload(i) for i in payload.get("decrease", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class NatureStatAffectSets(BaseModel):
-    """A nature stat affect sets resource.
-
-    Attributes
-    ----------
-    increase: typing.List[NatureStatAffect]
-        A list of nature stat affects.
-    decrease: typing.List[NatureStatAffect]
-        A list of nature stat affects.
-    """
-
-    increase: t.List[NamedResource] = attrs.field(factory=list)
-    decrease: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "NatureStatAffectSets":
-        return cls(
-            increase=[NamedResource.from_payload(i) for i in payload.get("increase", [])],
-            decrease=[NamedResource.from_payload(i) for i in payload.get("decrease", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class TypePokemon(BaseModel):
-    """A type pokemon resource.
-
-    Attributes
-    ----------
-    slot: int
-        The order the Pokémon's types are listed in.
-    pokemon: NamedResource
-        The Pokémon that has the referenced type.
-    """
-
-    slot: int = attrs.field(factory=int)
-    pokemon: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "TypePokemon":
-        return cls(
-            slot=payload.get("slot", 0),
-            pokemon=NamedResource.from_payload(payload.get("pokemon", {} or {})),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class TypeRelations(BaseModel):
-    """A type relations resource.
-
-    Attributes
-    ----------
-    no_damage_to: typing.List[NamedResource]
-        A list of types this type has no damage to.
-    half_damage_to: typing.List[NamedResource]
-        A list of types this type is half damage to.
-    double_damage_to: typing.List[NamedResource]
-        A list of types this type is double damage to.
-    no_damage_from: typing.List[NamedResource]
-        A list of types that have no damage to this type.
-    half_damage_from: typing.List[NamedResource]
-        A list of types that have half damage to this type.
-    double_damage_from: typing.List[NamedResource]
-        A list of types that have double damage to this type.
-    """
-
-    no_damage_to: t.List[NamedResource] = attrs.field(factory=list)
-    half_damage_to: t.List[NamedResource] = attrs.field(factory=list)
-    double_damage_to: t.List[NamedResource] = attrs.field(factory=list)
-    no_damage_from: t.List[NamedResource] = attrs.field(factory=list)
-    half_damage_from: t.List[NamedResource] = attrs.field(factory=list)
-    double_damage_from: t.List[NamedResource] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "TypeRelations":
-        return cls(
-            no_damage_to=[NamedResource.from_payload(i) for i in payload.get("no_damage_to", [])],
-            half_damage_to=[NamedResource.from_payload(i) for i in payload.get("half_damage_to", [])],
-            double_damage_to=[NamedResource.from_payload(i) for i in payload.get("double_damage_to", [])],
-            no_damage_from=[NamedResource.from_payload(i) for i in payload.get("no_damage_from", [])],
-            half_damage_from=[NamedResource.from_payload(i) for i in payload.get("half_damage_from", [])],
-            double_damage_from=[NamedResource.from_payload(i) for i in payload.get("double_damage_from", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class TypeRelationsPast(BaseModel):
-    """A type relations past resource.
-
-    Attributes
-    ----------
-    generation: NamedResource
-        The generation of this type relation.
-    damage_relations: TypeRelations
-        The type relations for this generation.
-    """
-
-    generation: NamedResource = attrs.field(factory=NamedResource)
-    damage_relations: TypeRelations = attrs.field(factory=TypeRelations)
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+from pokelance.models.common import Effect, NamedResource
+
+__all__: t.Tuple[str, ...] = (
+    "AbilityEffectChange",
+    "AbilityFlavorText",
+    "AbilityPokemon",
+    "PokemonSpeciesGender",
+    "GrowthRateExperienceLevel",
+    "NatureStatChange",
+    "MoveBattleStylePreference",
+    "NaturePokeathlonStatAffect",
+    "NaturePokeathlonStatAffectSet",
+    "PokemonMoveVersion",
+    "PokemonStat",
+    "PokemonType",
+    "PokemonHeldItemVersion",
+    "PokemonHeldItem",
+    "PokemonSprite",
+    "PokemonAbility",
+    "PokemonMove",
+    "PokemonTypePast",
+    "PokemonFormType",
+    "PokemonFormSprites",
+    "AwesomeName",
+    "PokemonSpeciesVariety",
+    "PokemonSpeciesDexEntry",
+    "PalParkEncounterArea",
+    "Genus",
+    "MoveStatAffectSets",
+    "NatureStatAffectSets",
+    "MoveStatEffect",
+    "TypeRelations",
+    "TypePokemon",
+    "TypeRelationsPast",
+)
+
+
+@attrs.define(kw_only=True, slots=True)
+class BaseSprite(BaseModel):
+    """A pokemon sprite resource.
+
+    Attributes
+    ----------
+    front_default: str
+        The default depiction of this pokemon from the front in battle.
+    front_shiny: str
+        The shiny depiction of this pokemon from the front in battle.
+    front_female: str
+        The default depiction of female gender of this pokemon from the front in battle.
+    front_shiny_female: str
+        The shiny depiction of female gender of this pokemon from the front in battle.
+    back_default: str
+        The default depiction of this pokemon from the back in battle.
+    back_shiny: str
+        The shiny depiction of this pokemon from the back in battle.
+    back_female: str
+        The default depiction of female gender of this pokemon from the back in battle.
+    back_shiny_female: str
+        The shiny depiction of female gender of this pokemon from the back in battle.
+    """
+
+    back_default: str = attrs.field(factory=str)
+    back_shiny: str = attrs.field(factory=str)
+    back_female: str = attrs.field(factory=str)
+    back_shiny_female: str = attrs.field(factory=str)
+    front_default: str = attrs.field(factory=str)
+    front_shiny: str = attrs.field(factory=str)
+    front_female: str = attrs.field(factory=str)
+    front_shiny_female: str = attrs.field(factory=str)
+
+
+@attrs.define(kw_only=True, slots=True)
+class Generation(BaseModel):
+    """A generation resource."""
+
+    ...
+
+
+@attrs.define(kw_only=True, slots=True)
+class Animated(BaseSprite):
+    """A pokemon animated sprite resource."""
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Animated":
+        return cls(
+            back_default=payload.get("back_default", ""),
+            back_shiny=payload.get("back_shiny", ""),
+            back_female=payload.get("back_female", ""),
+            back_shiny_female=payload.get("back_shiny_female", ""),
+            front_default=payload.get("front_default", ""),
+            front_shiny=payload.get("front_shiny", ""),
+            front_female=payload.get("front_female", ""),
+            front_shiny_female=payload.get("front_shiny_female", ""),
+        )
+
+
+@attrs.define(kw_only=True, slots=True)
+class VersionSprite(BaseSprite):
+    """A pokemon version sprite resource.
+
+    Attributes
+    ----------
+    back_gray: str
+        The gray depiction of this pokemon from the back in battle.
+    front_gray: str
+        The gray depiction of this pokemon from the front in battle.
+    back_transperent: str
+        The transparent depiction of this pokemon from the back in battle.
+    front_transperent: str
+        The transparent depiction of this pokemon from the front in battle.
+    animated: Animated
+        The animated depiction of this pokemon.
+    """
+
+    back_gray: str = attrs.field(factory=str)
+    back_transperent: str = attrs.field(factory=str)
+    back_shiny_transperent: str = attrs.field(factory=str)
+    front_gray: str = attrs.field(factory=str)
+    front_transperent: str = attrs.field(factory=str)
+    front_shiny_transperent: str = attrs.field(factory=str)
+    animated: Animated = attrs.field(factory=Animated)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "VersionSprite":
+        return cls(
+            back_default=payload.get("back_default", ""),
+            back_gray=payload.get("back_gray", ""),
+            back_shiny=payload.get("back_shiny", ""),
+            back_transperent=payload.get("back_transperent", ""),
+            back_shiny_transperent=payload.get("back_shiny_transperent", ""),
+            back_female=payload.get("back_female", ""),
+            back_shiny_female=payload.get("back_shiny_female", ""),
+            front_default=payload.get("front_default", ""),
+            front_shiny=payload.get("front_shiny", ""),
+            front_shiny_transperent=payload.get("front_shiny_transperent", ""),
+            front_female=payload.get("front_female", ""),
+            front_shiny_female=payload.get("front_shiny_female", ""),
+            front_gray=payload.get("front_gray", ""),
+            front_transperent=payload.get("front_transperent", ""),
+            animated=Animated.from_payload(payload.get("animated", {}) or {}),
+        )
+
+
+@attrs.define(kw_only=True, slots=True)
+class GenerationI(Generation):
+    """A generation I resource.
+
+    Attributes
+    ----------
+    red_blue: VersionSprite
+        The red-blue depiction of this pokemon.
+    yellow: VersionSprite
+        The yellow depiction of this pokemon.
+    """
+
+    red_blue: VersionSprite = attrs.field(factory=VersionSprite)
+    yellow: VersionSprite = attrs.field(factory=VersionSprite)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationI":
+        return cls(
+            red_blue=VersionSprite.from_payload(payload.get("red-blue", {}) or {}),
+            yellow=VersionSprite.from_payload(payload.get("yellow", {}) or {}),
+        )
+
+
+@attrs.define(kw_only=True, slots=True)
+class GenerationII(Generation):
+    """A generation II resource.
+
+    Attributes
+    ----------
+    crystal: VersionSprite
+        The crystal depiction of this pokemon.
+    gold: VersionSprite
+        The gold depiction of this pokemon.
+    silver: VersionSprite
+        The silver depiction of this pokemon.
+    """
+
+    crystal: VersionSprite = attrs.field(factory=VersionSprite)
+    gold: VersionSprite = attrs.field(factory=VersionSprite)
+    silver: VersionSprite = attrs.field(factory=VersionSprite)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationII":
+        return cls(
+            crystal=VersionSprite.from_payload(payload.get("crystal", {}) or {}),
+            gold=VersionSprite.from_payload(payload.get("gold", {}) or {}),
+            silver=VersionSprite.from_payload(payload.get("silver", {}) or {}),
+        )
+
+
+@attrs.define(kw_only=True, slots=True)
+class GenerationIII(Generation):
+    """A generation III resource.
+
+    Attributes
+    ----------
+    emerald: VersionSprite
+        The emerald depiction of this pokemon.
+    firered_leafgreen: VersionSprite
+        The firered-leafgreen depiction of this pokemon.
+    ruby_sapphire: VersionSprite
+        The ruby-sapphire depiction of this pokemon.
+    """
+
+    emerald: VersionSprite = attrs.field(factory=VersionSprite)
+    firered_leafgreen: VersionSprite = attrs.field(factory=VersionSprite)
+    ruby_sapphire: VersionSprite = attrs.field(factory=VersionSprite)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationIII":
+        return cls(
+            emerald=VersionSprite.from_payload(payload.get("emerald", {}) or {}),
+            firered_leafgreen=VersionSprite.from_payload(payload.get("firered-leafgreen", {}) or {}),
+            ruby_sapphire=VersionSprite.from_payload(payload.get("ruby-sapphire", {}) or {}),
+        )
+
+
+@attrs.define(kw_only=True, slots=True)
+class GenerationIV(Generation):
+    """A generation IV resource.
+
+    Attributes
+    ----------
+    diamond_pearl: VersionSprite
+        The diamond-pearl depiction of this pokemon.
+    heartgold_soulsilver: VersionSprite
+        The heartgold-soulsilver depiction of this pokemon.
+    platinum: VersionSprite
+        The platinum depiction of this pokemon.
+    """
+
+    diamond_pearl: VersionSprite = attrs.field(factory=VersionSprite)
+    heartgold_soulsilver: VersionSprite = attrs.field(factory=VersionSprite)
+    platinum: VersionSprite = attrs.field(factory=VersionSprite)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationIV":
+        return cls(
+            diamond_pearl=VersionSprite.from_payload(payload.get("diamond-pearl", {}) or {}),
+            heartgold_soulsilver=VersionSprite.from_payload(payload.get("heartgold-soulsilver", {}) or {}),
+            platinum=VersionSprite.from_payload(payload.get("platinum", {}) or {}),
+        )
+
+
+@attrs.define(kw_only=True, slots=True)
+class GenerationV(Generation):
+    """A generation V resource.
+
+    Attributes
+    ----------
+    black_white: VersionSprite
+        The black-white depiction of this pokemon.
+    """
+
+    black_white: VersionSprite = attrs.field(factory=VersionSprite)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationV":
+        return cls(
+            black_white=VersionSprite.from_payload(payload.get("black-white", {}) or {}),
+        )
+
+
+@attrs.define(kw_only=True, slots=True)
+class GenerationVI(Generation):
+    """A generation VI resource.
+
+    Attributes
+    ----------
+    omegaruby_alphasapphire: VersionSprite
+        The omegaruby-alphasapphire depiction of this pokemon.
+    x_y: VersionSprite
+        The x-y depiction of this pokemon.
+    """
+
+    omegaruby_alphasapphire: VersionSprite = attrs.field(factory=VersionSprite)
+    x_y: VersionSprite = attrs.field(factory=VersionSprite)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationVI":
+        return cls(
+            omegaruby_alphasapphire=VersionSprite.from_payload(payload.get("omegaruby-alphasapphire", {}) or {}),
+            x_y=VersionSprite.from_payload(payload.get("x-y", {}) or {}),
+        )
+
+
+@attrs.define(kw_only=True, slots=True)
+class GenerationVII(Generation):
+    """A generation VII resource.
+
+    Attributes
+    ----------
+    icons: VersionSprite
+        The icons depiction of this pokemon.
+    ultra_sun_ultra_moon: VersionSprite
+        The ultra-sun-ultra-moon depiction of this pokemon.
+    """
+
+    icons: VersionSprite = attrs.field(factory=VersionSprite)
+    ultra_sun_ultra_moon: VersionSprite = attrs.field(factory=VersionSprite)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationVII":
+        return cls(
+            icons=VersionSprite.from_payload(payload.get("icons", {}) or {}),
+            ultra_sun_ultra_moon=VersionSprite.from_payload(payload.get("ultra-sun-ultra-moon", {}) or {}),
+        )
+
+
+@attrs.define(kw_only=True, slots=True)
+class GenerationVIII(Generation):
+    """A generation VIII resource.
+
+    Attributes
+    ----------
+    icons: VersionSprite
+        The icons depiction of this pokemon.
+    """
+
+    icons: VersionSprite = attrs.field(factory=VersionSprite)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationVIII":
+        return cls(
+            icons=VersionSprite.from_payload(payload.get("icons", {}) or {}),
+        )
+
+
+@attrs.define(kw_only=True, slots=True)
+class Versions(BaseModel):
+    """A sprite resource for all generations.
+
+    Attributes
+    ----------
+    generation_i: GenerationI
+        The generation I depiction of this pokemon.
+    generation_ii: GenerationII
+        The generation II depiction of this pokemon.
+    generation_iii: GenerationIII
+        The generation III depiction of this pokemon.
+    generation_iv: GenerationIV
+        The generation IV depiction of this pokemon.
+    generation_v: GenerationV
+        The generation V depiction of this pokemon.
+    generation_vi: GenerationVI
+        The generation VI depiction of this pokemon.
+    generation_vii: GenerationVII
+        The generation VII depiction of this pokemon.
+    generation_viii: GenerationVIII
+        The generation VIII depiction of this pokemon.
+    """
+
+    generation_i: GenerationI = attrs.field(factory=GenerationI)
+    generation_ii: GenerationII = attrs.field(factory=GenerationII)
+    generation_iii: GenerationIII = attrs.field(factory=GenerationIII)
+    generation_iv: GenerationIV = attrs.field(factory=GenerationIV)
+    generation_v: GenerationV = attrs.field(factory=GenerationV)
+    generation_vi: GenerationVI = attrs.field(factory=GenerationVI)
+    generation_vii: GenerationVII = attrs.field(factory=GenerationVII)
+    generation_viii: GenerationVIII = attrs.field(factory=GenerationVIII)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Versions":
+        return cls(
+            generation_i=GenerationI.from_payload(payload.get("generation-i", {}) or {}),
+            generation_ii=GenerationII.from_payload(payload.get("generation-ii", {}) or {}),
+            generation_iii=GenerationIII.from_payload(payload.get("generation-iii", {}) or {}),
+            generation_iv=GenerationIV.from_payload(payload.get("generation-iv", {}) or {}),
+            generation_v=GenerationV.from_payload(payload.get("generation-v", {}) or {}),
+            generation_vi=GenerationVI.from_payload(payload.get("generation-vi", {}) or {}),
+            generation_vii=GenerationVII.from_payload(payload.get("generation-vii", {}) or {}),
+            generation_viii=GenerationVIII.from_payload(payload.get("generation-viii", {}) or {}),
+        )
+
+
+@attrs.define(kw_only=True, slots=True)
+class DreamWorld(BaseModel):
+    """A dream world resource.
+
+    Attributes
+    ----------
+    front_default: str
+        The default depiction of this pokemon.
+    front_female: str
+        The female depiction of this pokemon.
+    """
+
+    front_default: str = attrs.field(factory=str)
+    front_female: str = attrs.field(factory=str)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "DreamWorld":
+        return cls(
+            front_default=payload.get("front_default", ""),
+            front_female=payload.get("front_female", ""),
+        )
+
+
+@attrs.define(kw_only=True, slots=True)
+class Home(BaseModel):
+    """A home resource.
+
+    Attributes
+    ----------
+    front_default: str
+        The default depiction of this pokemon.
+    front_female: str
+        The female depiction of this pokemon.
+    front_shiny: str
+        The shiny depiction of this pokemon.
+    front_shiny_female: str
+        The shiny female depiction of this pokemon.
+    """
+
+    front_default: str = attrs.field(factory=str)
+    front_female: str = attrs.field(factory=str)
+    front_shiny: str = attrs.field(factory=str)
+    front_shiny_female: str = attrs.field(factory=str)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Home":
+        return cls(
+            front_default=payload.get("front_default", ""),
+            front_female=payload.get("front_female", ""),
+            front_shiny=payload.get("front_shiny", ""),
+            front_shiny_female=payload.get("front_shiny_female", ""),
+        )
+
+
+@attrs.define(kw_only=True, slots=True)
+class OfficialArtwork(BaseModel):
+    """Official artwork for this Pokémon from Nintendo.
+
+    Attributes
+    ----------
+    front_default: str
+        The default depiction of this Pokémon from the official artwork.
+    front_shiny: str
+        The shiny depiction of this Pokémon from the official artwork.
+    """
+
+    front_default: str = attrs.field(factory=str)
+    front_shiny: str = attrs.field(factory=str)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "OfficialArtwork":
+        return cls(
+            front_default=payload.get("front_default", ""),
+            front_shiny=payload.get("front_shiny", ""),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Other(BaseModel):
+    """Other sprites for this pokemon
+
+    Attributes
+    ----------
+    dream_world: DreamWorld
+        The dream world sprites for this pokemon
+    home: Home
+        The home sprites for this pokemon
+    official_artwork: OfficialArtwork
+        The official artwork sprites for this pokemon
+    """
+
+    dream_world: DreamWorld = attrs.field(factory=DreamWorld)
+    home: Home = attrs.field(factory=Home)
+    official_artwork: OfficialArtwork = attrs.field(factory=OfficialArtwork)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Other":
+        return cls(
+            dream_world=DreamWorld.from_payload(payload.get("dream_world", {}) or {}),
+            home=Home.from_payload(payload.get("home", {}) or {}),
+            official_artwork=OfficialArtwork.from_payload(payload.get("official-artwork", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class AbilityEffectChange(BaseModel):
+    """An ability effect change resource.
+
+    Attributes
+    ----------
+    effect_entries: t.List[Effect]
+        The previous effect of this ability listed in different languages.
+    version_group: NamedResource
+        The version group in which the previous effect of this ability originated.
+    """
+
+    effect_entries: t.List[Effect] = attrs.field(factory=list)
+    version_group: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "AbilityEffectChange":
+        return cls(
+            effect_entries=[Effect.from_payload(i) for i in payload.get("effect_entries", [])],
+            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class AbilityFlavorText(BaseModel):
+    """An ability flavor text resource.
+
+    Attributes
+    ----------
+    flavor_text: str
+        The localized flavor text for an api resource in a specific language.
+    language: NamedResource
+        The language this name is in.
+    version_group: NamedResource
+        The version group that uses this flavor text.
+    """
+
+    flavor_text: str = attrs.field(factory=str)
+    language: NamedResource = attrs.field(factory=NamedResource)
+    version_group: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "AbilityFlavorText":
+        return cls(
+            flavor_text=payload.get("flavor_text", ""),
+            language=NamedResource.from_payload(payload.get("language", {}) or {}),
+            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class AbilityPokemon(BaseModel):
+    """An ability pokemon resource.
+
+    Attributes
+    ----------
+    is_hidden: bool
+        Whether or not this a hidden ability for the referenced pokemon.
+    slot: int
+        The slot this ability occupies in this pokemon species.
+    pokemon: NamedResource
+        The pokemon this ability could belong to.
+    """
+
+    is_hidden: bool = attrs.field(factory=bool)
+    slot: int = attrs.field(factory=int)
+    pokemon: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "AbilityPokemon":
+        return cls(
+            is_hidden=payload.get("is_hidden", False),
+            slot=payload.get("slot", 0),
+            pokemon=NamedResource.from_payload(payload.get("pokemon", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonSpeciesGender(BaseModel):
+    """A pokemon species gender resource.
+
+    Attributes
+    ----------
+    rate: int
+        The chance of a particular gender in this pokemon species.
+    pokemon_species: NamedResource
+        The pokemon species here.
+    """
+
+    rate: int = attrs.field(factory=int)
+    pokemon_species: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonSpeciesGender":
+        return cls(
+            rate=payload.get("rate", 0),
+            pokemon_species=NamedResource.from_payload(payload.get("pokemon_species", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class GrowthRateExperienceLevel(BaseModel):
+    """A growth rate experience level resource.
+
+    Attributes
+    ----------
+    level: int
+        The level gained.
+    experience: int
+        The amount of experience required to reach the referenced level.
+    """
+
+    level: int = attrs.field(factory=int)
+    experience: int = attrs.field(factory=int)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GrowthRateExperienceLevel":
+        return cls(
+            level=payload.get("level", 0),
+            experience=payload.get("experience", 0),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class NatureStatChange(BaseModel):
+    """A nature stat change resource.
+
+    Attributes
+    ----------
+    max_change: int
+        The maximum amount of change to the referenced stat.
+    pokeathlon_stat: NamedResource
+        The stat being affected.
+    """
+
+    max_change: int = attrs.field(factory=int)
+    pokeathlon_stat: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "NatureStatChange":
+        return cls(
+            max_change=payload.get("max_change", 0),
+            pokeathlon_stat=NamedResource.from_payload(payload.get("pokeathlon_stat", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class MoveBattleStylePreference(BaseModel):
+    """A move battle style preference resource.
+
+    Attributes
+    ----------
+    low_hp_preference: int
+        Chance of using the move, in percent, if HP is under one half.
+    high_hp_preference: int
+        Chance of using the move, in percent, if HP is over one half.
+    move_battle_style: NamedResource
+        The move battle style.
+    """
+
+    low_hp_preference: int = attrs.field(factory=int)
+    high_hp_preference: int = attrs.field(factory=int)
+    move_battle_style: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveBattleStylePreference":
+        return cls(
+            low_hp_preference=payload.get("low_hp_preference", 0),
+            high_hp_preference=payload.get("high_hp_preference", 0),
+            move_battle_style=NamedResource.from_payload(payload.get("battle_style", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class NaturePokeathlonStatAffect(BaseModel):
+    """A nature pokeathlon stat affect resource.
+
+    Attributes
+    ----------
+    max_change: int
+        The maximum amount of change to the referenced stat.
+    nature: NamedResource
+        The nature causing the change.
+    """
+
+    max_change: int = attrs.field(factory=int)
+    nature: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "NaturePokeathlonStatAffect":
+        return cls(
+            max_change=payload.get("max_change", 0),
+            nature=NamedResource.from_payload(payload.get("nature", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class NaturePokeathlonStatAffectSet(BaseModel):
+    """A nature pokeathlon stat affect set resource.
+
+    Attributes
+    ----------
+    increase: t.List[NaturePokeathlonStatAffect]
+        A list of natures and how they change the referenced pokeathlon stat.
+    decrease: t.List[NaturePokeathlonStatAffect]
+        A list of natures and how they change the referenced pokeathlon stat.
+    """
+
+    increase: t.List[NaturePokeathlonStatAffect] = attrs.field(factory=list)
+    decrease: t.List[NaturePokeathlonStatAffect] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "NaturePokeathlonStatAffectSet":
+        return cls(
+            increase=[NaturePokeathlonStatAffect.from_payload(i) for i in payload.get("increase", [])],
+            decrease=[NaturePokeathlonStatAffect.from_payload(i) for i in payload.get("decrease", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonAbility(BaseModel):
+    """A pokemon ability resource.
+
+    Attributes
+    ----------
+    is_hidden: bool
+        Whether or not this is a hidden ability.
+    slot: int
+        The slot this ability occupies in this pokemon species.
+    ability: NamedResource
+        The ability the pokemon may have.
+    """
+
+    is_hidden: bool = attrs.field(factory=bool)
+    slot: int = attrs.field(factory=int)
+    ability: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonAbility":
+        return cls(
+            is_hidden=payload.get("is_hidden", False),
+            slot=payload.get("slot", 0),
+            ability=NamedResource.from_payload(payload.get("ability", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonType(BaseModel):
+    """A pokemon type resource.
+
+    Attributes
+    ----------
+    slot: int
+        The order the types are listed in.
+    type: NamedResource
+        The type the referenced pokemon has.
+    """
+
+    slot: int = attrs.field(factory=int)
+    type: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonType":
+        return cls(
+            slot=payload.get("slot", 0),
+            type=NamedResource.from_payload(payload.get("type", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonFormType(BaseModel):
+    """A pokemon form type resource.
+
+    Attributes
+    ----------
+    slot: int
+        The order the types are listed in.
+    type: NamedResource
+        The type the referenced pokemon has.
+    """
+
+    slot: int = attrs.field(factory=int)
+    type: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonFormType":
+        return cls(
+            slot=payload.get("slot", 0),
+            type=NamedResource.from_payload(payload.get("type", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonTypePast(BaseModel):
+    """A pokemon type past resource.
+
+    Attributes
+    ----------
+    generation: NamedResource
+        The generation this type was introduced in.
+    types: t.List[NamedResource]
+        The name of the type.
+    """
+
+    generation: NamedResource = attrs.field(factory=NamedResource)
+    types: t.List[PokemonType] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonTypePast":
+        return cls(
+            generation=NamedResource.from_payload(payload.get("generation", {}) or {}),
+            types=[PokemonType.from_payload(i) for i in payload.get("types", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonHeldItemVersion(BaseModel):
+    """A pokemon held item version resource.
+
+    Attributes
+    ----------
+    rarity: int
+        How often this item is held.
+    version: NamedResource
+        The version this item is held in by the pokemon.
+    """
+
+    version: NamedResource = attrs.field(factory=NamedResource)
+    rarity: int = attrs.field(factory=int)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonHeldItemVersion":
+        return cls(
+            version=NamedResource.from_payload(payload.get("version", {}) or {}),
+            rarity=payload.get("rarity", 0),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonHeldItem(BaseModel):
+    """A pokemon held item resource.
+
+    Attributes
+    ----------
+    item: NamedResource
+        The item the referenced pokemon holds.
+    version_details: t.List[PokemonHeldItemVersion]
+        The details for the version that this item is held in by the pokemon.
+    """
+
+    item: NamedResource = attrs.field(factory=NamedResource)
+    version_details: t.List[PokemonHeldItemVersion] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonHeldItem":
+        return cls(
+            item=NamedResource.from_payload(payload.get("item", {}) or {}),
+            version_details=[PokemonHeldItemVersion.from_payload(i) for i in payload.get("version_details", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonMoveVersion(BaseModel):
+    """A pokemon move version resource.
+
+    Attributes
+    ----------
+    move_learn_method: NamedResource
+        The method by which the move is learned.
+    version_group: NamedResource
+        The version group in which the move is learned.
+    level_learned_at: int
+        The minimum level to learn the move.
+    """
+
+    move_learn_method: NamedResource = attrs.field(factory=NamedResource)
+    version_group: NamedResource = attrs.field(factory=NamedResource)
+    level_learned_at: int = attrs.field(factory=int)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonMoveVersion":
+        return cls(
+            move_learn_method=NamedResource.from_payload(payload.get("move_learn_method", {}) or {}),
+            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
+            level_learned_at=payload.get("level_learned_at", 0),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonMove(BaseModel):
+    """A pokemon move resource.
+
+    Attributes
+    ----------
+    move: NamedResource
+        The move the referenced pokemon can learn.
+    version_group_details: t.List[PokemonMoveVersion]
+        The details for the version group that this move can be learned in.
+    """
+
+    move: NamedResource = attrs.field(factory=NamedResource)
+    version_group_details: t.List[PokemonMoveVersion] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonMove":
+        return cls(
+            move=NamedResource.from_payload(payload.get("move", {}) or {}),
+            version_group_details=[
+                PokemonMoveVersion.from_payload(i) for i in payload.get("version_group_details", [])
+            ],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonStat(BaseModel):
+    """A pokemon stat resource.
+
+    Attributes
+    ----------
+    stat: NamedResource
+        The stat the referenced pokemon has.
+    effort: int
+        The effort points (EV) the referenced pokemon has in the stat.
+    base_stat: int
+        The base value of the stat.
+    """
+
+    stat: NamedResource = attrs.field(factory=NamedResource)
+    effort: int = attrs.field(factory=int)
+    base_stat: int = attrs.field(factory=int)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonStat":
+        return cls(
+            stat=NamedResource.from_payload(payload.get("stat", {}) or {}),
+            effort=payload.get("effort", 0),
+            base_stat=payload.get("base_stat", 0),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonSprite(BaseSprite):
+    """A pokemon sprite resource.
+
+    Attributes
+    ----------
+    other: Other
+        A set of sprites used tin official artwork, home.
+    versions: Versions
+        A set of sprites used to depict this Pokémon in the game.
+    """
+
+    other: Other = attrs.field(factory=Other)
+    versions: Versions = attrs.field(factory=Versions)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonSprite":
+        return cls(
+            front_default=payload.get("front_default", ""),
+            front_shiny=payload.get("front_shiny", ""),
+            front_female=payload.get("front_female", ""),
+            front_shiny_female=payload.get("front_shiny_female", ""),
+            back_default=payload.get("back_default", ""),
+            back_shiny=payload.get("back_shiny", ""),
+            back_female=payload.get("back_female", ""),
+            back_shiny_female=payload.get("back_shiny_female", ""),
+            other=Other.from_payload(payload.get("other", {}) or {}),
+            versions=Versions.from_payload(payload.get("versions", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonFormSprites(BaseModel):
+    """A pokemon form sprites resource.
+
+    Attributes
+    ----------
+    front_default: str
+        The default depiction of this pokemon form from the front in battle.
+    front_shiny: str
+        The shiny depiction of this pokemon form from the front in battle.
+    back_default: str
+        The default depiction of this pokemon form from the back in battle.
+    back_shiny: str
+        The shiny depiction of this pokemon form from the back in battle.
+    """
+
+    front_default: str = attrs.field(factory=str)
+    front_shiny: str = attrs.field(factory=str)
+    back_default: str = attrs.field(factory=str)
+    back_shiny: str = attrs.field(factory=str)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonFormSprites":
+        return cls(
+            front_default=payload.get("front_default", ""),
+            front_shiny=payload.get("front_shiny", ""),
+            back_default=payload.get("back_default", ""),
+            back_shiny=payload.get("back_shiny", ""),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class AwesomeName(BaseModel):
+    """An awesome name resource.
+
+    Attributes
+    ----------
+    awesome_name: str
+        The localized "scientific" name for an API resource in a specific language.
+    language: NamedResource
+        The language this "scientific" name is in.
+    """
+
+    awesome_name: str = attrs.field(factory=str)
+    language: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "AwesomeName":
+        return cls(
+            awesome_name=payload.get("awesome_name", ""),
+            language=NamedResource.from_payload(payload.get("language", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Genus(BaseModel):
+    """A genus resource.
+
+    Attributes
+    ----------
+    genus: str
+        The localized genus for the referenced type in the specified language.
+    language: NamedResource
+        The language this genus is in.
+    """
+
+    genus: str = attrs.field(factory=str)
+    language: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Genus":
+        return cls(
+            genus=payload.get("genus", ""),
+            language=NamedResource.from_payload(payload.get("language", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonSpeciesDexEntry(BaseModel):
+    """A pokemon species dex entry resource.
+
+    Attributes
+    ----------
+    entry_number: int
+        The index number within the Pokédex.
+    pokedex: NamedResource
+        The Pokédex the referenced Pokémon species can be found in.
+    """
+
+    entry_number: int = attrs.field(factory=int)
+    pokedex: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonSpeciesDexEntry":
+        return cls(
+            entry_number=payload.get("entry_number", 0),
+            pokedex=NamedResource.from_payload(payload.get("pokedex", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PalParkEncounterArea(BaseModel):
+    """A pal park encounter area resource.
+
+    Attributes
+    ----------
+    base_score: int
+        The base score given to the player when the referenced Pokémon is caught during a pal park run.
+    rate: int
+        The base rate for encountering the referenced Pokémon in this pal park area.
+    area: NamedResource
+        The pal park area where this encounter happens.
+    """
+
+    base_score: int = attrs.field(factory=int)
+    rate: int = attrs.field(factory=int)
+    area: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PalParkEncounterArea":
+        return cls(
+            base_score=payload.get("base_score", 0),
+            rate=payload.get("rate", 0),
+            area=NamedResource.from_payload(payload.get("area", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class PokemonSpeciesVariety(BaseModel):
+    """A pokemon species variety resource.
+
+    Attributes
+    ----------
+    is_default: bool
+        Whether this variety is the default variety.
+    pokemon: NamedResource
+        The Pokémon variety.
+    """
+
+    is_default: bool = attrs.field(factory=bool)
+    pokemon: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "PokemonSpeciesVariety":
+        return cls(
+            is_default=payload.get("is_default", False),
+            pokemon=NamedResource.from_payload(payload.get("pokemon", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class MoveStatEffect(BaseModel):
+    """A move stat effect resource.
+
+    Attributes
+    ----------
+    change: int
+        The maximum amount of change to the referenced stat.
+    stat: NamedResource
+        The stat being affected.
+    """
+
+    change: int = attrs.field(factory=int)
+    stat: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveStatEffect":
+        return cls(
+            change=payload.get("change", 0),
+            stat=NamedResource.from_payload(payload.get("stat", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class MoveStatAffectSets(BaseModel):
+    """A move stat affect sets resource.
+
+    Attributes
+    ----------
+    increase: typing.List[MoveStatAffect]
+        A list of move stat affects.
+    decrease: typing.List[MoveStatAffect]
+        A list of move stat affects.
+    """
+
+    increase: t.List[MoveStatEffect] = attrs.field(factory=list)
+    decrease: t.List[MoveStatEffect] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveStatAffectSets":
+        return cls(
+            increase=[MoveStatEffect.from_payload(i) for i in payload.get("increase", [])],
+            decrease=[MoveStatEffect.from_payload(i) for i in payload.get("decrease", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class NatureStatAffectSets(BaseModel):
+    """A nature stat affect sets resource.
+
+    Attributes
+    ----------
+    increase: typing.List[NatureStatAffect]
+        A list of nature stat affects.
+    decrease: typing.List[NatureStatAffect]
+        A list of nature stat affects.
+    """
+
+    increase: t.List[NamedResource] = attrs.field(factory=list)
+    decrease: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "NatureStatAffectSets":
+        return cls(
+            increase=[NamedResource.from_payload(i) for i in payload.get("increase", [])],
+            decrease=[NamedResource.from_payload(i) for i in payload.get("decrease", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class TypePokemon(BaseModel):
+    """A type pokemon resource.
+
+    Attributes
+    ----------
+    slot: int
+        The order the Pokémon's types are listed in.
+    pokemon: NamedResource
+        The Pokémon that has the referenced type.
+    """
+
+    slot: int = attrs.field(factory=int)
+    pokemon: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "TypePokemon":
+        return cls(
+            slot=payload.get("slot", 0),
+            pokemon=NamedResource.from_payload(payload.get("pokemon", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class TypeRelations(BaseModel):
+    """A type relations resource.
+
+    Attributes
+    ----------
+    no_damage_to: typing.List[NamedResource]
+        A list of types this type has no damage to.
+    half_damage_to: typing.List[NamedResource]
+        A list of types this type is half damage to.
+    double_damage_to: typing.List[NamedResource]
+        A list of types this type is double damage to.
+    no_damage_from: typing.List[NamedResource]
+        A list of types that have no damage to this type.
+    half_damage_from: typing.List[NamedResource]
+        A list of types that have half damage to this type.
+    double_damage_from: typing.List[NamedResource]
+        A list of types that have double damage to this type.
+    """
+
+    no_damage_to: t.List[NamedResource] = attrs.field(factory=list)
+    half_damage_to: t.List[NamedResource] = attrs.field(factory=list)
+    double_damage_to: t.List[NamedResource] = attrs.field(factory=list)
+    no_damage_from: t.List[NamedResource] = attrs.field(factory=list)
+    half_damage_from: t.List[NamedResource] = attrs.field(factory=list)
+    double_damage_from: t.List[NamedResource] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "TypeRelations":
+        return cls(
+            no_damage_to=[NamedResource.from_payload(i) for i in payload.get("no_damage_to", [])],
+            half_damage_to=[NamedResource.from_payload(i) for i in payload.get("half_damage_to", [])],
+            double_damage_to=[NamedResource.from_payload(i) for i in payload.get("double_damage_to", [])],
+            no_damage_from=[NamedResource.from_payload(i) for i in payload.get("no_damage_from", [])],
+            half_damage_from=[NamedResource.from_payload(i) for i in payload.get("half_damage_from", [])],
+            double_damage_from=[NamedResource.from_payload(i) for i in payload.get("double_damage_from", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class TypeRelationsPast(BaseModel):
+    """A type relations past resource.
+
+    Attributes
+    ----------
+    generation: NamedResource
+        The generation of this type relation.
+    damage_relations: TypeRelations
+        The type relations for this generation.
+    """
+
+    generation: NamedResource = attrs.field(factory=NamedResource)
+    damage_relations: TypeRelations = attrs.field(factory=TypeRelations)
```

### Comparing `pokelance-0.0.9a0/pokelance/models/common/__init__.py` & `pokelance-0.1.0/pokelance/models/common/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import typing as t
-
-from .models import (
-    Description,
-    Effect,
-    Encounter,
-    FlavorText,
-    GenerationGameIndex,
-    Language,
-    MachineVersionDetail,
-    Name,
-    VerboseEffect,
-    VersionEncounterDetail,
-    VersionGameIndex,
-    VersionGroupFlavorText,
-)
-from .resources import NamedResource, Resource
-
-__all__: t.Tuple[str, ...] = (
-    "Description",
-    "Effect",
-    "Encounter",
-    "FlavorText",
-    "GenerationGameIndex",
-    "MachineVersionDetail",
-    "Name",
-    "VerboseEffect",
-    "VersionEncounterDetail",
-    "VersionGameIndex",
-    "VersionGroupFlavorText",
-    "Resource",
-    "NamedResource",
-    "Language",
-)
+import typing as t
+
+from .models import (
+    Description,
+    Effect,
+    Encounter,
+    FlavorText,
+    GenerationGameIndex,
+    Language,
+    MachineVersionDetail,
+    Name,
+    VerboseEffect,
+    VersionEncounterDetail,
+    VersionGameIndex,
+    VersionGroupFlavorText,
+)
+from .resources import NamedResource, Resource
+
+__all__: t.Tuple[str, ...] = (
+    "Description",
+    "Effect",
+    "Encounter",
+    "FlavorText",
+    "GenerationGameIndex",
+    "MachineVersionDetail",
+    "Name",
+    "VerboseEffect",
+    "VersionEncounterDetail",
+    "VersionGameIndex",
+    "VersionGroupFlavorText",
+    "Resource",
+    "NamedResource",
+    "Language",
+)
```

### Comparing `pokelance-0.0.9a0/pokelance/models/common/models.py` & `pokelance-0.1.0/pokelance/models/common/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,339 +1,339 @@
-import typing as t
-
-import attrs
-
-from pokelance.models import BaseModel
-
-from .resources import NamedResource, Resource
-
-__all__: t.Tuple[str, ...] = (
-    "Description",
-    "Effect",
-    "Encounter",
-    "FlavorText",
-    "GenerationGameIndex",
-    "MachineVersionDetail",
-    "Name",
-    "VerboseEffect",
-    "VersionEncounterDetail",
-    "VersionGameIndex",
-    "VersionGroupFlavorText",
-    "Language",
-)
-
-
-@attrs.define(slots=True, kw_only=True)
-class Description(BaseModel):
-    """Model for a description object
-
-    Attributes
-    ----------
-    description: str
-        The localized description for an API resource in a specific language.
-    language: NamedResource
-        The language this name is in.
-    """
-
-    description: str = attrs.field(factory=str)
-    language: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Description":
-        return cls(
-            description=payload.get("description", ""),
-            language=NamedResource.from_payload(payload.get("language", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Effect(BaseModel):
-    """Model for an effect object
-
-    Attributes
-    ----------
-    effect: str
-        The localized effect text for an API resource in a specific language.
-    language: NamedResource
-        The language this effect is in.
-    """
-
-    effect: str = attrs.field(factory=str)
-    language: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Effect":
-        return cls(
-            effect=payload.get("effect", ""),
-            language=NamedResource.from_payload(payload.get("language", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Encounter(BaseModel):
-    """Model for an encounter object
-
-    Attributes
-    ----------
-    min_level: int
-        The lowest level the Pokémon could be encountered at.
-    max_level: int
-        The highest level the Pokémon could be encountered at.
-    condition_values: t.List[NamedResource]
-        A list of condition values that must be in effect for this encounter to occur.
-    chance: int
-        The chance of the encounter to occur on a version of the game.
-    method: NamedResource
-        The method by which this encounter happens.
-    """
-
-    min_level: int = attrs.field(factory=int)
-    max_level: int = attrs.field(factory=int)
-    condition_values: t.List[Resource] = attrs.field(factory=list)
-    chance: int = attrs.field(factory=int)
-    method: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Encounter":
-        return cls(
-            min_level=payload.get("min_level", 0),
-            max_level=payload.get("max_level", 0),
-            condition_values=[Resource.from_payload(i) for i in payload.get("condition_values", [])],
-            chance=payload.get("chance", 0),
-            method=NamedResource.from_payload(payload.get("method", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class FlavorText(BaseModel):
-    """Model for a flavor text object
-
-    Attributes
-    ----------
-    flavor_text: str
-        The localized flavor text for an API resource in a specific language.
-    language: NamedResource
-        The language this name is in.
-    version: NamedResource
-        The version that this flavor text is extracted from.
-    """
-
-    flavor_text: str = attrs.field(factory=str)
-    language: NamedResource = attrs.field(factory=NamedResource)
-    version: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "FlavorText":
-        return cls(
-            flavor_text=payload.get("flavor_text", ""),
-            language=NamedResource.from_payload(payload.get("language", {}) or {}),
-            version=NamedResource.from_payload(payload.get("version", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class GenerationGameIndex(BaseModel):
-    """Model for a generation game index object
-
-    Attributes
-    ----------
-    game_index: int
-        The internal id of an API resource within game data.
-    generation: NamedResource
-        The generation relevent to this game index.
-    """
-
-    game_index: int = attrs.field(factory=int)
-    generation: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationGameIndex":
-        return cls(
-            game_index=payload.get("game_index", 0),
-            generation=NamedResource.from_payload(payload.get("generation", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class MachineVersionDetail(BaseModel):
-    """Model for a machine version detail object
-
-    Attributes
-    ----------
-    machine: Resource
-        The machine that teaches a move from an item.
-    version_group: NamedResource
-        The version group of this specific machine.
-    """
-
-    machine: Resource = attrs.field(factory=Resource)
-    version_group: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MachineVersionDetail":
-        return cls(
-            machine=Resource.from_payload(payload.get("machine", {}) or {}),
-            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Name(BaseModel):
-    """Model for a name object
-
-    Attributes
-    ----------
-    name: str
-        The localized name for an API resource in a specific language.
-    language: NamedResource
-        The language this name is in.
-    """
-
-    name: str = attrs.field(factory=str)
-    language: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Name":
-        return cls(name=payload.get("name", ""), language=NamedResource.from_payload(payload.get("language", {}) or {}))
-
-
-@attrs.define(slots=True, kw_only=True)
-class VerboseEffect(BaseModel):
-    """Model for a verbose effect object
-
-    Attributes
-    ----------
-    effect: str
-        The localized effect text for an API resource in a specific language.
-    short_effect: str
-        The localized short effect text for an API resource in a specific language.
-    language: NamedResource
-        The language this effect is in.
-    """
-
-    effect: str = attrs.field(factory=str)
-    short_effect: str = attrs.field(factory=str)
-    language: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "VerboseEffect":
-        return cls(
-            effect=payload.get("effect", ""),
-            short_effect=payload.get("short_effect", ""),
-            language=NamedResource.from_payload(payload.get("language", {} or {})),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class VersionEncounterDetail(BaseModel):
-    """Model for a version encounter detail object
-
-    Attributes
-    ----------
-    max_chance: int
-        The chance of an encounter to occur.
-    encounter_details: t.List[Encounter]
-        A list of encounters and their specifics.
-    version: NamedResource
-        The game version this encounter happens in.
-    """
-
-    version: NamedResource = attrs.field(factory=NamedResource)
-    max_chance: int = attrs.field(factory=int)
-    encounter_details: t.List[Encounter] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "VersionEncounterDetail":
-        return cls(
-            version=NamedResource.from_payload(payload.get("version", {}) or {}),
-            max_chance=payload.get("max_chance", 0),
-            encounter_details=[Encounter.from_payload(i) for i in payload.get("encounter_details", [])],
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class VersionGameIndex(BaseModel):
-    """Model for a version game index object
-
-    Attributes
-    ----------
-    game_index: int
-        The internal id of an API resource within game data.
-    version: NamedResource
-        The version relevent to this game index.
-    """
-
-    game_index: int = attrs.field(factory=int)
-    version: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "VersionGameIndex":
-        return cls(
-            game_index=payload.get("game_index", 0),
-            version=NamedResource.from_payload(payload.get("version", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class VersionGroupFlavorText(BaseModel):
-    """Model for a version group flavor text object
-
-    Attributes
-    ----------
-    text: str
-        The localized name for an API resource in a specific language.
-    language: NamedResource
-        The language this name is in.
-    version_group: NamedResource
-        The version group which uses this flavor text.
-    """
-
-    text: str = attrs.field(factory=str)
-    language: NamedResource = attrs.field(factory=NamedResource)
-    version_group: NamedResource = attrs.field(factory=NamedResource)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "VersionGroupFlavorText":
-        return cls(
-            text=payload.get("text", ""),
-            language=NamedResource.from_payload(payload.get("language", {}) or {}),
-            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
-        )
-
-
-@attrs.define(slots=True, kw_only=True)
-class Language(BaseModel):
-    """Model for a language object
-
-    Attributes
-    ----------
-    id: int
-        The identifier for this resource.
-    name: str
-        The name for this resource.
-    official: bool
-        Whether or not the games are published in this language.
-    iso639: str
-        The two-letter code of the country where this language is spoken. Note that it is not unique.
-    iso3166: str
-        The two-letter code of the language. Note that it is not unique.
-    names: t.List[Name]
-        The name of this resource listed in different languages.
-    """
-
-    id: int = attrs.field(factory=int)
-    name: str = attrs.field(factory=str)
-    official: bool = attrs.field(factory=bool)
-    iso639: str = attrs.field(factory=str)
-    iso3166: str = attrs.field(factory=str)
-    names: t.List[Name] = attrs.field(factory=list)
-
-    @classmethod
-    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Language":
-        return cls(
-            id=payload.get("id", 0),
-            name=payload.get("name", ""),
-            official=payload.get("official", False),
-            iso639=payload.get("iso639", ""),
-            iso3166=payload.get("iso3166", ""),
-            names=[Name.from_payload(i) for i in payload.get("names", [])],
-        )
+import typing as t
+
+import attrs
+
+from pokelance.models import BaseModel
+
+from .resources import NamedResource, Resource
+
+__all__: t.Tuple[str, ...] = (
+    "Description",
+    "Effect",
+    "Encounter",
+    "FlavorText",
+    "GenerationGameIndex",
+    "MachineVersionDetail",
+    "Name",
+    "VerboseEffect",
+    "VersionEncounterDetail",
+    "VersionGameIndex",
+    "VersionGroupFlavorText",
+    "Language",
+)
+
+
+@attrs.define(slots=True, kw_only=True)
+class Description(BaseModel):
+    """Model for a description object
+
+    Attributes
+    ----------
+    description: str
+        The localized description for an API resource in a specific language.
+    language: NamedResource
+        The language this name is in.
+    """
+
+    description: str = attrs.field(factory=str)
+    language: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Description":
+        return cls(
+            description=payload.get("description", ""),
+            language=NamedResource.from_payload(payload.get("language", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Effect(BaseModel):
+    """Model for an effect object
+
+    Attributes
+    ----------
+    effect: str
+        The localized effect text for an API resource in a specific language.
+    language: NamedResource
+        The language this effect is in.
+    """
+
+    effect: str = attrs.field(factory=str)
+    language: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Effect":
+        return cls(
+            effect=payload.get("effect", ""),
+            language=NamedResource.from_payload(payload.get("language", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Encounter(BaseModel):
+    """Model for an encounter object
+
+    Attributes
+    ----------
+    min_level: int
+        The lowest level the Pokémon could be encountered at.
+    max_level: int
+        The highest level the Pokémon could be encountered at.
+    condition_values: t.List[NamedResource]
+        A list of condition values that must be in effect for this encounter to occur.
+    chance: int
+        The chance of the encounter to occur on a version of the game.
+    method: NamedResource
+        The method by which this encounter happens.
+    """
+
+    min_level: int = attrs.field(factory=int)
+    max_level: int = attrs.field(factory=int)
+    condition_values: t.List[Resource] = attrs.field(factory=list)
+    chance: int = attrs.field(factory=int)
+    method: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Encounter":
+        return cls(
+            min_level=payload.get("min_level", 0),
+            max_level=payload.get("max_level", 0),
+            condition_values=[Resource.from_payload(i) for i in payload.get("condition_values", [])],
+            chance=payload.get("chance", 0),
+            method=NamedResource.from_payload(payload.get("method", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class FlavorText(BaseModel):
+    """Model for a flavor text object
+
+    Attributes
+    ----------
+    flavor_text: str
+        The localized flavor text for an API resource in a specific language.
+    language: NamedResource
+        The language this name is in.
+    version: NamedResource
+        The version that this flavor text is extracted from.
+    """
+
+    flavor_text: str = attrs.field(factory=str)
+    language: NamedResource = attrs.field(factory=NamedResource)
+    version: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "FlavorText":
+        return cls(
+            flavor_text=payload.get("flavor_text", ""),
+            language=NamedResource.from_payload(payload.get("language", {}) or {}),
+            version=NamedResource.from_payload(payload.get("version", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class GenerationGameIndex(BaseModel):
+    """Model for a generation game index object
+
+    Attributes
+    ----------
+    game_index: int
+        The internal id of an API resource within game data.
+    generation: NamedResource
+        The generation relevent to this game index.
+    """
+
+    game_index: int = attrs.field(factory=int)
+    generation: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "GenerationGameIndex":
+        return cls(
+            game_index=payload.get("game_index", 0),
+            generation=NamedResource.from_payload(payload.get("generation", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class MachineVersionDetail(BaseModel):
+    """Model for a machine version detail object
+
+    Attributes
+    ----------
+    machine: Resource
+        The machine that teaches a move from an item.
+    version_group: NamedResource
+        The version group of this specific machine.
+    """
+
+    machine: Resource = attrs.field(factory=Resource)
+    version_group: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MachineVersionDetail":
+        return cls(
+            machine=Resource.from_payload(payload.get("machine", {}) or {}),
+            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Name(BaseModel):
+    """Model for a name object
+
+    Attributes
+    ----------
+    name: str
+        The localized name for an API resource in a specific language.
+    language: NamedResource
+        The language this name is in.
+    """
+
+    name: str = attrs.field(factory=str)
+    language: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Name":
+        return cls(name=payload.get("name", ""), language=NamedResource.from_payload(payload.get("language", {}) or {}))
+
+
+@attrs.define(slots=True, kw_only=True)
+class VerboseEffect(BaseModel):
+    """Model for a verbose effect object
+
+    Attributes
+    ----------
+    effect: str
+        The localized effect text for an API resource in a specific language.
+    short_effect: str
+        The localized short effect text for an API resource in a specific language.
+    language: NamedResource
+        The language this effect is in.
+    """
+
+    effect: str = attrs.field(factory=str)
+    short_effect: str = attrs.field(factory=str)
+    language: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "VerboseEffect":
+        return cls(
+            effect=payload.get("effect", ""),
+            short_effect=payload.get("short_effect", ""),
+            language=NamedResource.from_payload(payload.get("language", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class VersionEncounterDetail(BaseModel):
+    """Model for a version encounter detail object
+
+    Attributes
+    ----------
+    max_chance: int
+        The chance of an encounter to occur.
+    encounter_details: t.List[Encounter]
+        A list of encounters and their specifics.
+    version: NamedResource
+        The game version this encounter happens in.
+    """
+
+    version: NamedResource = attrs.field(factory=NamedResource)
+    max_chance: int = attrs.field(factory=int)
+    encounter_details: t.List[Encounter] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "VersionEncounterDetail":
+        return cls(
+            version=NamedResource.from_payload(payload.get("version", {}) or {}),
+            max_chance=payload.get("max_chance", 0),
+            encounter_details=[Encounter.from_payload(i) for i in payload.get("encounter_details", [])],
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class VersionGameIndex(BaseModel):
+    """Model for a version game index object
+
+    Attributes
+    ----------
+    game_index: int
+        The internal id of an API resource within game data.
+    version: NamedResource
+        The version relevent to this game index.
+    """
+
+    game_index: int = attrs.field(factory=int)
+    version: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "VersionGameIndex":
+        return cls(
+            game_index=payload.get("game_index", 0),
+            version=NamedResource.from_payload(payload.get("version", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class VersionGroupFlavorText(BaseModel):
+    """Model for a version group flavor text object
+
+    Attributes
+    ----------
+    text: str
+        The localized name for an API resource in a specific language.
+    language: NamedResource
+        The language this name is in.
+    version_group: NamedResource
+        The version group which uses this flavor text.
+    """
+
+    text: str = attrs.field(factory=str)
+    language: NamedResource = attrs.field(factory=NamedResource)
+    version_group: NamedResource = attrs.field(factory=NamedResource)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "VersionGroupFlavorText":
+        return cls(
+            text=payload.get("text", ""),
+            language=NamedResource.from_payload(payload.get("language", {}) or {}),
+            version_group=NamedResource.from_payload(payload.get("version_group", {}) or {}),
+        )
+
+
+@attrs.define(slots=True, kw_only=True)
+class Language(BaseModel):
+    """Model for a language object
+
+    Attributes
+    ----------
+    id: int
+        The identifier for this resource.
+    name: str
+        The name for this resource.
+    official: bool
+        Whether or not the games are published in this language.
+    iso639: str
+        The two-letter code of the country where this language is spoken. Note that it is not unique.
+    iso3166: str
+        The two-letter code of the language. Note that it is not unique.
+    names: t.List[Name]
+        The name of this resource listed in different languages.
+    """
+
+    id: int = attrs.field(factory=int)
+    name: str = attrs.field(factory=str)
+    official: bool = attrs.field(factory=bool)
+    iso639: str = attrs.field(factory=str)
+    iso3166: str = attrs.field(factory=str)
+    names: t.List[Name] = attrs.field(factory=list)
+
+    @classmethod
+    def from_payload(cls, payload: t.Dict[str, t.Any]) -> "Language":
+        return cls(
+            id=payload.get("id", 0),
+            name=payload.get("name", ""),
+            official=payload.get("official", False),
+            iso639=payload.get("iso639", ""),
+            iso3166=payload.get("iso3166", ""),
+            names=[Name.from_payload(i) for i in payload.get("names", [])],
+        )
```

### Comparing `pokelance-0.0.9a0/README.md` & `pokelance-0.1.0/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-<h1 align="center"><b>PokeLance</b></h1>
-<p align="center">
-<img src="https://raw.githubusercontent.com/FallenDeity/PokeLance/master/docs/assets/pokelance.png" width=450 alt="logo"><br><br>
-<img src="https://img.shields.io/github/license/FallenDeity/PokeLance?style=flat-square" alt="license">
-<img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">
-<img src="https://img.shields.io/badge/%20type_checker-mypy-%231674b1?style=flat-square" alt="mypy">
-<img src="https://img.shields.io/badge/%20linter-ruff-%231674b1?style=flat-square" alt="ruff">
-<img src="https://img.shields.io/github/stars/FallenDeity/PokeLance?style=flat-square" alt="stars">
-<img src="https://img.shields.io/github/last-commit/FallenDeity/PokeLance?style=flat-square" alt="commits">
-<img src="https://img.shields.io/pypi/pyversions/PokeLance?style=flat-square" alt="py">
-<img src="https://img.shields.io/pypi/v/PokeLance?style=flat-square" alt="versions">
-<br><br>
-A flexible, statically typed and easy to use pokeapi wrapper for python 🚀
-</p>
-
----
-
-
-Features:
-- Modern and pythonic API asynchronously built on top of aiohttp
-- Flexible and easy to use
-- Statically typed with mypy
-- Linted with ruff
-- Well documented
-- Optimized for speed and performance
-- Automatically caches data for faster access
-- Caches endpoints for user convenience
-
----
-
-## Installation
-
-```bash
-$ python -m pip install PokeLance
-```
-
----
-
-## Usage
-
-```python
-import asyncio
-
-from pokelance import PokeLance
-
-client = PokeLance()  # Create a client instance
-
-
-async def main() -> None:
-    print(await client.ping())  # Ping the pokeapi
-    print(await client.berry.fetch_berry("cheri"))  # Fetch a berry from the pokeapi
-    print(await client.berry.fetch_berry_flavor("spicy"))
-    print(await client.berry.fetch_berry_firmness("very-soft"))
-    print(client.berry.get_berry("cheri"))  # Get a cached berry it will return None if it doesn't exist
-    print(client.berry.get_berry_flavor("spicy"))
-    print(client.berry.get_berry_firmness("very-soft"))
-    await client.close()  # Close the client
-    return None
-
-
-asyncio.run(main())
-```
-
-## With Async Context Manager
-
-```python
-import asyncio
-
-import aiohttp
-from pokelance import PokeLance
-
-
-async def main() -> None:
-    # Use an async context manager to create a client instance
-    async with aiohttp.ClientSession() as session, PokeLance(session=session) as client:
-        print(await client.ping())  # Ping the pokeapi
-        print(await client.berry.fetch_berry("cheri"))  # Fetch a berry from the pokeapi
-        print(await client.berry.fetch_berry_flavor("spicy"))
-        print(await client.berry.fetch_berry_firmness("very-soft"))
-        print(client.berry.get_berry("cheri"))  # Get a cached berry it will return None if it doesn't exist
-        print(client.berry.get_berry_flavor("spicy"))
-        print(client.berry.get_berry_firmness("very-soft"))
-        # The client will be closed automatically when the async context manager exits
-    return None
-
-asyncio.run(main())
-```
-
-## Important Links
-
-
-- [PokeAPI](https://pokeapi.co/)
-- [PokeAPI Documentation](https://pokeapi.co/docs/v2)
-- [PokeLance Documentation](https://FallenDeity.github.io/PokeLance/)
-- [PokeLance ReadTheDocs](https://pokelance.readthedocs.io/en/latest/)
-- [PokeLance GitHub](https://github.com/FallenDeity/PokeLance)
-- [PokeLance PyPI](https://pypi.org/project/PokeLance/)
-- [PokeLance Discord](https://discord.gg/yeyEvT5V2J)
-
----
-
-!!! note "Note"
-    This is a work in progress. If you find any bugs or have any suggestions, please open an issue [here](https://github.com/FallenDeity/PokeLance/issues/new).
-
+<h1 align="center"><b>PokeLance</b></h1>
+<p align="center">
+<img src="https://raw.githubusercontent.com/FallenDeity/PokeLance/master/docs/assets/pokelance.png" width=450 alt="logo"><br><br>
+<img src="https://img.shields.io/github/license/FallenDeity/PokeLance?style=flat-square" alt="license">
+<img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">
+<img src="https://img.shields.io/badge/%20type_checker-mypy-%231674b1?style=flat-square" alt="mypy">
+<img src="https://img.shields.io/badge/%20linter-ruff-%231674b1?style=flat-square" alt="ruff">
+<img src="https://img.shields.io/github/stars/FallenDeity/PokeLance?style=flat-square" alt="stars">
+<img src="https://img.shields.io/github/last-commit/FallenDeity/PokeLance?style=flat-square" alt="commits">
+<img src="https://img.shields.io/pypi/pyversions/PokeLance?style=flat-square" alt="py">
+<img src="https://img.shields.io/pypi/v/PokeLance?style=flat-square" alt="versions">
+<br><br>
+A flexible, statically typed and easy to use pokeapi wrapper for python 🚀
+</p>
+
+---
+
+
+Features:
+- Modern and pythonic API asynchronously built on top of aiohttp
+- Flexible and easy to use
+- Statically typed with mypy
+- Linted with ruff
+- Well documented
+- Optimized for speed and performance
+- Automatically caches data for faster access
+- Caches endpoints for user convenience
+
+---
+
+## Installation
+
+```bash
+$ python -m pip install PokeLance
+```
+
+---
+
+## Usage
+
+```python
+import asyncio
+
+from pokelance import PokeLance
+
+client = PokeLance()  # Create a client instance
+
+
+async def main() -> None:
+    print(await client.ping())  # Ping the pokeapi
+    print(await client.berry.fetch_berry("cheri"))  # Fetch a berry from the pokeapi
+    print(await client.berry.fetch_berry_flavor("spicy"))
+    print(await client.berry.fetch_berry_firmness("very-soft"))
+    print(client.berry.get_berry("cheri"))  # Get a cached berry it will return None if it doesn't exist
+    print(client.berry.get_berry_flavor("spicy"))
+    print(client.berry.get_berry_firmness("very-soft"))
+    await client.close()  # Close the client
+    return None
+
+
+asyncio.run(main())
+```
+
+## With Async Context Manager
+
+```python
+import asyncio
+
+import aiohttp
+from pokelance import PokeLance
+
+
+async def main() -> None:
+    # Use an async context manager to create a client instance
+    async with aiohttp.ClientSession() as session, PokeLance(session=session) as client:
+        print(await client.ping())  # Ping the pokeapi
+        print(await client.berry.fetch_berry("cheri"))  # Fetch a berry from the pokeapi
+        print(await client.berry.fetch_berry_flavor("spicy"))
+        print(await client.berry.fetch_berry_firmness("very-soft"))
+        print(client.berry.get_berry("cheri"))  # Get a cached berry it will return None if it doesn't exist
+        print(client.berry.get_berry_flavor("spicy"))
+        print(client.berry.get_berry_firmness("very-soft"))
+        # The client will be closed automatically when the async context manager exits
+    return None
+
+asyncio.run(main())
+```
+
+## Important Links
+
+
+- [PokeAPI](https://pokeapi.co/)
+- [PokeAPI Documentation](https://pokeapi.co/docs/v2)
+- [PokeLance Documentation](https://FallenDeity.github.io/PokeLance/)
+- [PokeLance ReadTheDocs](https://pokelance.readthedocs.io/en/latest/)
+- [PokeLance GitHub](https://github.com/FallenDeity/PokeLance)
+- [PokeLance PyPI](https://pypi.org/project/PokeLance/)
+- [PokeLance Discord](https://discord.gg/yeyEvT5V2J)
+
+---
+
+!!! note "Note"
+    This is a work in progress. If you find any bugs or have any suggestions, please open an issue [here](https://github.com/FallenDeity/PokeLance/issues/new).
+
 ---
```

### Comparing `pokelance-0.0.9a0/setup.py` & `pokelance-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,126 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pokelance
+Version: 0.1.0
+Summary: A flexible and easy to use pokemon library.
+License: MIT
+Author: FallenDeity
+Author-email: 61227305+FallenDeity@users.noreply.github.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
+Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Requires-Dist: attrs (>=22.1.0,<23.0.0)
+Requires-Dist: types-aiofiles (>=23.1.0.1,<24.0.0.0)
+Description-Content-Type: text/markdown
+
+<h1 align="center"><b>PokeLance</b></h1>
+<p align="center">
+<img src="https://raw.githubusercontent.com/FallenDeity/PokeLance/master/docs/assets/pokelance.png" width=450 alt="logo"><br><br>
+<img src="https://img.shields.io/github/license/FallenDeity/PokeLance?style=flat-square" alt="license">
+<img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">
+<img src="https://img.shields.io/badge/%20type_checker-mypy-%231674b1?style=flat-square" alt="mypy">
+<img src="https://img.shields.io/badge/%20linter-ruff-%231674b1?style=flat-square" alt="ruff">
+<img src="https://img.shields.io/github/stars/FallenDeity/PokeLance?style=flat-square" alt="stars">
+<img src="https://img.shields.io/github/last-commit/FallenDeity/PokeLance?style=flat-square" alt="commits">
+<img src="https://img.shields.io/pypi/pyversions/PokeLance?style=flat-square" alt="py">
+<img src="https://img.shields.io/pypi/v/PokeLance?style=flat-square" alt="versions">
+<br><br>
+A flexible, statically typed and easy to use pokeapi wrapper for python 🚀
+</p>
+
+---
+
+
+Features:
+- Modern and pythonic API asynchronously built on top of aiohttp
+- Flexible and easy to use
+- Statically typed with mypy
+- Linted with ruff
+- Well documented
+- Optimized for speed and performance
+- Automatically caches data for faster access
+- Caches endpoints for user convenience
+
+---
+
+## Installation
+
+```bash
+$ python -m pip install PokeLance
+```
+
+---
+
+## Usage
+
+```python
+import asyncio
+
+from pokelance import PokeLance
+
+client = PokeLance()  # Create a client instance
+
+
+async def main() -> None:
+    print(await client.ping())  # Ping the pokeapi
+    print(await client.berry.fetch_berry("cheri"))  # Fetch a berry from the pokeapi
+    print(await client.berry.fetch_berry_flavor("spicy"))
+    print(await client.berry.fetch_berry_firmness("very-soft"))
+    print(client.berry.get_berry("cheri"))  # Get a cached berry it will return None if it doesn't exist
+    print(client.berry.get_berry_flavor("spicy"))
+    print(client.berry.get_berry_firmness("very-soft"))
+    await client.close()  # Close the client
+    return None
+
+
+asyncio.run(main())
+```
+
+## With Async Context Manager
+
+```python
+import asyncio
+
+import aiohttp
+from pokelance import PokeLance
+
+
+async def main() -> None:
+    # Use an async context manager to create a client instance
+    async with aiohttp.ClientSession() as session, PokeLance(session=session) as client:
+        print(await client.ping())  # Ping the pokeapi
+        print(await client.berry.fetch_berry("cheri"))  # Fetch a berry from the pokeapi
+        print(await client.berry.fetch_berry_flavor("spicy"))
+        print(await client.berry.fetch_berry_firmness("very-soft"))
+        print(client.berry.get_berry("cheri"))  # Get a cached berry it will return None if it doesn't exist
+        print(client.berry.get_berry_flavor("spicy"))
+        print(client.berry.get_berry_firmness("very-soft"))
+        # The client will be closed automatically when the async context manager exits
+    return None
+
+asyncio.run(main())
+```
+
+## Important Links
+
+
+- [PokeAPI](https://pokeapi.co/)
+- [PokeAPI Documentation](https://pokeapi.co/docs/v2)
+- [PokeLance Documentation](https://FallenDeity.github.io/PokeLance/)
+- [PokeLance ReadTheDocs](https://pokelance.readthedocs.io/en/latest/)
+- [PokeLance GitHub](https://github.com/FallenDeity/PokeLance)
+- [PokeLance PyPI](https://pypi.org/project/PokeLance/)
+- [PokeLance Discord](https://discord.gg/yeyEvT5V2J)
 
-packages = \
-['pokelance',
- 'pokelance.cache',
- 'pokelance.ext',
- 'pokelance.http',
- 'pokelance.models',
- 'pokelance.models.abstract',
- 'pokelance.models.abstract.utils',
- 'pokelance.models.common']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiofiles>=22.1.0,<23.0.0',
- 'aiohttp>=3.8.3,<4.0.0',
- 'attrs>=22.1.0,<23.0.0',
- 'types-aiofiles>=22.1.0.4,<23.0.0.0']
-
-setup_kwargs = {
-    'name': 'pokelance',
-    'version': '0.0.9a0',
-    'description': 'A flexible and easy to use pokemon library.',
-    'long_description': '<h1 align="center"><b>PokeLance</b></h1>\n<p align="center">\n<img src="https://raw.githubusercontent.com/FallenDeity/PokeLance/master/docs/assets/pokelance.png" width=450 alt="logo"><br><br>\n<img src="https://img.shields.io/github/license/FallenDeity/PokeLance?style=flat-square" alt="license">\n<img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n<img src="https://img.shields.io/badge/%20type_checker-mypy-%231674b1?style=flat-square" alt="mypy">\n<img src="https://img.shields.io/badge/%20linter-ruff-%231674b1?style=flat-square" alt="ruff">\n<img src="https://img.shields.io/github/stars/FallenDeity/PokeLance?style=flat-square" alt="stars">\n<img src="https://img.shields.io/github/last-commit/FallenDeity/PokeLance?style=flat-square" alt="commits">\n<img src="https://img.shields.io/pypi/pyversions/PokeLance?style=flat-square" alt="py">\n<img src="https://img.shields.io/pypi/v/PokeLance?style=flat-square" alt="versions">\n<br><br>\nA flexible, statically typed and easy to use pokeapi wrapper for python 🚀\n</p>\n\n---\n\n\nFeatures:\n- Modern and pythonic API asynchronously built on top of aiohttp\n- Flexible and easy to use\n- Statically typed with mypy\n- Linted with ruff\n- Well documented\n- Optimized for speed and performance\n- Automatically caches data for faster access\n- Caches endpoints for user convenience\n\n---\n\n## Installation\n\n```bash\n$ python -m pip install PokeLance\n```\n\n---\n\n## Usage\n\n```python\nimport asyncio\n\nfrom pokelance import PokeLance\n\nclient = PokeLance()  # Create a client instance\n\n\nasync def main() -> None:\n    print(await client.ping())  # Ping the pokeapi\n    print(await client.berry.fetch_berry("cheri"))  # Fetch a berry from the pokeapi\n    print(await client.berry.fetch_berry_flavor("spicy"))\n    print(await client.berry.fetch_berry_firmness("very-soft"))\n    print(client.berry.get_berry("cheri"))  # Get a cached berry it will return None if it doesn\'t exist\n    print(client.berry.get_berry_flavor("spicy"))\n    print(client.berry.get_berry_firmness("very-soft"))\n    await client.close()  # Close the client\n    return None\n\n\nasyncio.run(main())\n```\n\n## With Async Context Manager\n\n```python\nimport asyncio\n\nimport aiohttp\nfrom pokelance import PokeLance\n\n\nasync def main() -> None:\n    # Use an async context manager to create a client instance\n    async with aiohttp.ClientSession() as session, PokeLance(session=session) as client:\n        print(await client.ping())  # Ping the pokeapi\n        print(await client.berry.fetch_berry("cheri"))  # Fetch a berry from the pokeapi\n        print(await client.berry.fetch_berry_flavor("spicy"))\n        print(await client.berry.fetch_berry_firmness("very-soft"))\n        print(client.berry.get_berry("cheri"))  # Get a cached berry it will return None if it doesn\'t exist\n        print(client.berry.get_berry_flavor("spicy"))\n        print(client.berry.get_berry_firmness("very-soft"))\n        # The client will be closed automatically when the async context manager exits\n    return None\n\nasyncio.run(main())\n```\n\n## Important Links\n\n\n- [PokeAPI](https://pokeapi.co/)\n- [PokeAPI Documentation](https://pokeapi.co/docs/v2)\n- [PokeLance Documentation](https://FallenDeity.github.io/PokeLance/)\n- [PokeLance ReadTheDocs](https://pokelance.readthedocs.io/en/latest/)\n- [PokeLance GitHub](https://github.com/FallenDeity/PokeLance)\n- [PokeLance PyPI](https://pypi.org/project/PokeLance/)\n- [PokeLance Discord](https://discord.gg/yeyEvT5V2J)\n\n---\n\n!!! note "Note"\n    This is a work in progress. If you find any bugs or have any suggestions, please open an issue [here](https://github.com/FallenDeity/PokeLance/issues/new).\n\n---\n',
-    'author': 'FallenDeity',
-    'author_email': '61227305+FallenDeity@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+---
 
+!!! note "Note"
+    This is a work in progress. If you find any bugs or have any suggestions, please open an issue [here](https://github.com/FallenDeity/PokeLance/issues/new).
+
+---
 
-setup(**setup_kwargs)
```

