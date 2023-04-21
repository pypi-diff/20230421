# Comparing `tmp/pokelance-0.1.0.tar.gz` & `tmp/pokelance-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokelance-0.1.0.tar", max compression
+gzip compressed data, was "pokelance-0.1.1.tar", max compression
```

## Comparing `pokelance-0.1.0.tar` & `pokelance-0.1.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1068 2023-04-21 15:29:11.374173 pokelance-0.1.0/LICENSE
--rw-r--r--   0        0        0     3658 2023-04-21 15:29:11.374173 pokelance-0.1.0/README.md
--rw-r--r--   0        0        0      106 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/__init__.py
--rw-r--r--   0        0        0      431 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/cache/__init__.py
--rw-r--r--   0        0        0    14534 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/cache/cache.py
--rw-r--r--   0        0        0    13942 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/cache/cache_manager.py
--rw-r--r--   0        0        0     8907 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/client.py
--rw-r--r--   0        0        0     3725 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/constants.py
--rw-r--r--   0        0        0     3868 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/exceptions.py
--rw-r--r--   0        0        0      530 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/__init__.py
--rw-r--r--   0        0        0     3163 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/_base.py
--rw-r--r--   0        0        0     7196 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/berry.py
--rw-r--r--   0        0        0     7189 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/contest.py
--rw-r--r--   0        0        0     7747 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/encounter.py
--rw-r--r--   0        0        0     4990 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/evolution.py
--rw-r--r--   0        0        0     8348 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/game.py
--rw-r--r--   0        0        0    11273 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/item.py
--rw-r--r--   0        0        0     9049 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/location.py
--rw-r--r--   0        0        0     2625 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/machine.py
--rw-r--r--   0        0        0    15682 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/move.py
--rw-r--r--   0        0        0    33460 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/ext/pokemon.py
--rw-r--r--   0        0        0     4724 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/http/__init__.py
--rw-r--r--   0        0        0    20467 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/http/endpoints.py
--rw-r--r--   0        0        0     8683 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/languages.py
--rw-r--r--   0        0        0     3588 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/logger.py
--rw-r--r--   0        0        0     1919 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/__init__.py
--rw-r--r--   0        0        0      529 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/_base.py
--rw-r--r--   0        0        0     1873 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/__init__.py
--rw-r--r--   0        0        0     5528 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/berry.py
--rw-r--r--   0        0        0     4083 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/contest.py
--rw-r--r--   0        0        0     3507 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/encounter.py
--rw-r--r--   0        0        0     2410 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/evolution.py
--rw-r--r--   0        0        0     7628 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/game.py
--rw-r--r--   0        0        0     8794 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/item.py
--rw-r--r--   0        0        0     6706 2023-04-21 15:29:11.378173 pokelance-0.1.0/pokelance/models/abstract/location.py
--rw-r--r--   0        0        0     1222 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/machine.py
--rw-r--r--   0        0        0    12765 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/move.py
--rw-r--r--   0        0        0    35329 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/pokemon.py
--rw-r--r--   0        0        0     1351 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/showdown.py
--rw-r--r--   0        0        0     2506 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/__init__.py
--rw-r--r--   0        0        0     1494 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/berries.py
--rw-r--r--   0        0        0      943 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/contests.py
--rw-r--r--   0        0        0     6255 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/evolutions.py
--rw-r--r--   0        0        0      890 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/games.py
--rw-r--r--   0        0        0     2284 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/items.py
--rw-r--r--   0        0        0     3546 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/locations.py
--rw-r--r--   0        0        0     7112 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/moves.py
--rw-r--r--   0        0        0    42172 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/abstract/utils/pokemons.py
--rw-r--r--   0        0        0      650 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/common/__init__.py
--rw-r--r--   0        0        0    10868 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/common/models.py
--rw-r--r--   0        0        0     1063 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/models/common/resources.py
--rw-r--r--   0        0        0        0 2023-04-21 15:29:11.382173 pokelance-0.1.0/pokelance/py.typed
--rw-r--r--   0        0        0     1114 2023-04-21 15:29:11.382173 pokelance-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4404 1970-01-01 00:00:00.000000 pokelance-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-21 19:23:59.329383 pokelance-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3658 2023-04-21 19:23:59.329383 pokelance-0.1.1/README.md
+-rw-r--r--   0        0        0      106 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/__init__.py
+-rw-r--r--   0        0        0      431 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/cache/__init__.py
+-rw-r--r--   0        0        0    14534 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/cache/cache.py
+-rw-r--r--   0        0        0    13942 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/cache/cache_manager.py
+-rw-r--r--   0        0        0     9015 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/client.py
+-rw-r--r--   0        0        0     5886 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/constants.py
+-rw-r--r--   0        0        0     3868 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/exceptions.py
+-rw-r--r--   0        0        0      530 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/ext/__init__.py
+-rw-r--r--   0        0        0     3163 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/ext/_base.py
+-rw-r--r--   0        0        0     7196 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/ext/berry.py
+-rw-r--r--   0        0        0     7189 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/ext/contest.py
+-rw-r--r--   0        0        0     7747 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/ext/encounter.py
+-rw-r--r--   0        0        0     4990 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/ext/evolution.py
+-rw-r--r--   0        0        0     8348 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/ext/game.py
+-rw-r--r--   0        0        0    11273 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/ext/item.py
+-rw-r--r--   0        0        0     9049 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/ext/location.py
+-rw-r--r--   0        0        0     2625 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/ext/machine.py
+-rw-r--r--   0        0        0    15682 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/ext/move.py
+-rw-r--r--   0        0        0    33460 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/ext/pokemon.py
+-rw-r--r--   0        0        0     4724 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/http/__init__.py
+-rw-r--r--   0        0        0    20467 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/http/endpoints.py
+-rw-r--r--   0        0        0     9677 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/languages.py
+-rw-r--r--   0        0        0     3588 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/logger.py
+-rw-r--r--   0        0        0     1919 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/models/__init__.py
+-rw-r--r--   0        0        0      529 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/models/_base.py
+-rw-r--r--   0        0        0     1873 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/models/abstract/__init__.py
+-rw-r--r--   0        0        0     5528 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/models/abstract/berry.py
+-rw-r--r--   0        0        0     4083 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/models/abstract/contest.py
+-rw-r--r--   0        0        0     3507 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/models/abstract/encounter.py
+-rw-r--r--   0        0        0     2410 2023-04-21 19:23:59.333383 pokelance-0.1.1/pokelance/models/abstract/evolution.py
+-rw-r--r--   0        0        0     7628 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/game.py
+-rw-r--r--   0        0        0     8794 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/item.py
+-rw-r--r--   0        0        0     6706 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/location.py
+-rw-r--r--   0        0        0     1222 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/machine.py
+-rw-r--r--   0        0        0    12765 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/move.py
+-rw-r--r--   0        0        0    35329 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/pokemon.py
+-rw-r--r--   0        0        0     1351 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/showdown.py
+-rw-r--r--   0        0        0     2506 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/utils/__init__.py
+-rw-r--r--   0        0        0     1494 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/utils/berries.py
+-rw-r--r--   0        0        0      943 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/utils/contests.py
+-rw-r--r--   0        0        0     6255 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/utils/evolutions.py
+-rw-r--r--   0        0        0      890 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/utils/games.py
+-rw-r--r--   0        0        0     2284 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/utils/items.py
+-rw-r--r--   0        0        0     3546 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/utils/locations.py
+-rw-r--r--   0        0        0     7112 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/utils/moves.py
+-rw-r--r--   0        0        0    42172 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/abstract/utils/pokemons.py
+-rw-r--r--   0        0        0      650 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/common/__init__.py
+-rw-r--r--   0        0        0    10868 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/common/models.py
+-rw-r--r--   0        0        0     1063 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/models/common/resources.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:23:59.337383 pokelance-0.1.1/pokelance/py.typed
+-rw-r--r--   0        0        0     1114 2023-04-21 19:23:59.337383 pokelance-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4404 1970-01-01 00:00:00.000000 pokelance-0.1.1/PKG-INFO
```

### Comparing `pokelance-0.1.0/LICENSE` & `pokelance-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/README.md` & `pokelance-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/cache/cache.py` & `pokelance-0.1.1/pokelance/cache/cache.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/cache/cache_manager.py` & `pokelance-0.1.1/pokelance/cache/cache_manager.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/client.py` & `pokelance-0.1.1/pokelance/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,22 +174,22 @@
         Not needed if the client is used in a context manager.
         """
         self._logger.info("Closing session")
         if self._http.session is not None:
             await self._http.session.close()
 
     async def getch_data(
-        self, ext: t.Union[ExtensionEnum, ExtensionsL], category: str, id_: t.Union[int, str]
+        self, ext: t.Union[ExtensionEnum, ExtensionsL, str], category: str, id_: t.Union[int, str]
     ) -> BaseType:
         """
         A getch method that looks up the cache for the data first then gets it from the API if it is not found.
 
         Parameters
         ----------
-        ext : Union[ExtensionEnum, ExtensionsL]
+        ext : Union[ExtensionEnum, ExtensionsL, str]
             The extension to get the data from.
         category : str
             The category to get the data from.
         id_ : Union[int, str]
             The ID of the data to get.
 
         Returns
@@ -204,29 +204,30 @@
         HTTPException
             If the data is not found.
 
         Examples
         --------
         >>> import pokelance
         >>> import asyncio
+        >>> from pokelance.constants import ExtensionEnum
         >>> from pokelance.models import Pokemon
         >>> client = pokelance.PokeLance()
         >>> async def main() -> None:
-        ...     pokemon: Pokemon = await client.getch_data("pokemon", "pokemon", 1)
+        ...     pokemon: Pokemon = await client.getch_data(ExtensionEnum.Pokemon, "pokemon", 1)
         ...     print(pokemon.name)
         ...     await client.close()
         >>> asyncio.run(main())
         bulbasaur
         """
-        if isinstance(ext, str) and ext.lower() not in ExtensionEnum.__members__:
+        if isinstance(ext, str) and (ext := str(ext).title()) not in ExtensionEnum.__members__:
             raise ValueError(f"Invalid extension: {ext}")
         categories = ExtensionEnum.get_categories(ext) if isinstance(ext, str) else ext.categories  # type: ignore
-        if category not in categories:
+        if (category := category.lower()) not in categories:
             raise ValueError(f"Invalid category: {category}")
-        ext_ = getattr(self, ext.lower()) if isinstance(ext, str) else getattr(self, ext.name.lower())
+        ext_ = getattr(self, ext) if isinstance(ext, str) else getattr(self, ext.name.lower())
         get_, fetch_ = getattr(ext_, f"get_{category}"), getattr(ext_, f"fetch_{category}")
         return t.cast(BaseType, get_(id_) or await fetch_(id_))
 
     async def get_image_async(self, url: str) -> bytes:
         """
         Gets an image from the url asynchronously.
```

### Comparing `pokelance-0.1.0/pokelance/exceptions.py` & `pokelance-0.1.1/pokelance/exceptions.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/ext/__init__.py` & `pokelance-0.1.1/pokelance/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/ext/_base.py` & `pokelance-0.1.1/pokelance/ext/_base.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/ext/berry.py` & `pokelance-0.1.1/pokelance/ext/berry.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/ext/contest.py` & `pokelance-0.1.1/pokelance/ext/contest.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/ext/encounter.py` & `pokelance-0.1.1/pokelance/ext/encounter.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/ext/evolution.py` & `pokelance-0.1.1/pokelance/ext/evolution.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/ext/game.py` & `pokelance-0.1.1/pokelance/ext/game.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/ext/item.py` & `pokelance-0.1.1/pokelance/ext/item.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/ext/location.py` & `pokelance-0.1.1/pokelance/ext/location.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/ext/machine.py` & `pokelance-0.1.1/pokelance/ext/machine.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/ext/move.py` & `pokelance-0.1.1/pokelance/ext/move.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/ext/pokemon.py` & `pokelance-0.1.1/pokelance/ext/pokemon.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/http/__init__.py` & `pokelance-0.1.1/pokelance/http/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/http/endpoints.py` & `pokelance-0.1.1/pokelance/http/endpoints.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/languages.py` & `pokelance-0.1.1/pokelance/languages.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,47 @@
 from pokelance.models import Language
 
 __all__: t.Tuple[str, ...] = ("Languages",)
 LANGUAGE = Endpoint.get_language_endpoints().url
 
 
 class Languages(enum.Enum):
+    """
+    Languages that are available on Pokeapi.
+
+    Attributes
+    ----------
+    JAPANESE: Language
+        The Japanese language.
+    ROOMAJI: Language
+        The Japanese language written in roomaji.
+    KOREAN: Language
+        The Korean language.
+    CHINESE: Language
+        The Chinese language.
+    FRENCH: Language
+        The French language.
+    GERMAN: Language
+        The German language.
+    SPANISH: Language
+        The Spanish language.
+    ITALIAN: Language
+        The Italian language.
+    CZECH: Language
+        The Czech language.
+    ENGLISH: Language
+        The English language.
+    JA: Language
+        The Japanese language.
+    CHINESE_SIMPLIFIED: Language
+        The Chinese language written in simplified Chinese.
+    PORTUGAL_BRAZILIAN: Language
+        The Portuguese language written in Brazilian Portuguese.
+    """
+
     JAPANESE = Language.from_payload(
         {
             "id": 1,
             "iso3166": "jp",
             "iso639": "ja",
             "name": "ja-Hrkt",
             "names": [
@@ -186,11 +219,17 @@
         {"id": 12, "iso3166": "cn", "iso639": "zh", "name": "zh-Hans", "names": [], "official": True}
     )
     PORTUGAL_BRAZILIAN = Language.from_payload(
         {"id": 13, "iso3166": "br", "iso639": "pt-BR", "name": "pt-BR", "names": [], "official": False}
     )
 
     def __str__(self) -> str:
+        """
+        Returns the name of the language.
+        """
         return str(self.value.name)
 
     def __int__(self) -> int:
+        """
+        Returns the id of the language.
+        """
         return int(self.value.id)
```

### Comparing `pokelance-0.1.0/pokelance/logger.py` & `pokelance-0.1.1/pokelance/logger.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/__init__.py` & `pokelance-0.1.1/pokelance/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/_base.py` & `pokelance-0.1.1/pokelance/models/_base.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/__init__.py` & `pokelance-0.1.1/pokelance/models/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/berry.py` & `pokelance-0.1.1/pokelance/models/abstract/berry.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/contest.py` & `pokelance-0.1.1/pokelance/models/abstract/contest.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/encounter.py` & `pokelance-0.1.1/pokelance/models/abstract/encounter.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/evolution.py` & `pokelance-0.1.1/pokelance/models/abstract/evolution.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/game.py` & `pokelance-0.1.1/pokelance/models/abstract/game.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/item.py` & `pokelance-0.1.1/pokelance/models/abstract/item.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/location.py` & `pokelance-0.1.1/pokelance/models/abstract/location.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/machine.py` & `pokelance-0.1.1/pokelance/models/abstract/machine.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/move.py` & `pokelance-0.1.1/pokelance/models/abstract/move.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/pokemon.py` & `pokelance-0.1.1/pokelance/models/abstract/pokemon.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/showdown.py` & `pokelance-0.1.1/pokelance/models/abstract/showdown.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/utils/__init__.py` & `pokelance-0.1.1/pokelance/models/abstract/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/utils/berries.py` & `pokelance-0.1.1/pokelance/models/abstract/utils/berries.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/utils/contests.py` & `pokelance-0.1.1/pokelance/models/abstract/utils/contests.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/utils/evolutions.py` & `pokelance-0.1.1/pokelance/models/abstract/utils/evolutions.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/utils/games.py` & `pokelance-0.1.1/pokelance/models/abstract/utils/games.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/utils/items.py` & `pokelance-0.1.1/pokelance/models/abstract/utils/items.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/utils/locations.py` & `pokelance-0.1.1/pokelance/models/abstract/utils/locations.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/utils/moves.py` & `pokelance-0.1.1/pokelance/models/abstract/utils/moves.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/abstract/utils/pokemons.py` & `pokelance-0.1.1/pokelance/models/abstract/utils/pokemons.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/common/__init__.py` & `pokelance-0.1.1/pokelance/models/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/common/models.py` & `pokelance-0.1.1/pokelance/models/common/models.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pokelance/models/common/resources.py` & `pokelance-0.1.1/pokelance/models/common/resources.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.0/pyproject.toml` & `pokelance-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pokelance"
-version = "0.1.0"
+version = "0.1.1"
 description = "A flexible and easy to use pokemon library."
 authors = ["FallenDeity <61227305+FallenDeity@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pokelance-0.1.0/PKG-INFO` & `pokelance-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokelance
-Version: 0.1.0
+Version: 0.1.1
 Summary: A flexible and easy to use pokemon library.
 License: MIT
 Author: FallenDeity
 Author-email: 61227305+FallenDeity@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

