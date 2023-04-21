# Comparing `tmp/pymafia-0.1.9.tar.gz` & `tmp/pymafia-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymafia-0.1.9.tar", max compression
+gzip compressed data, was "pymafia-0.2.0.tar", max compression
```

## Comparing `pymafia-0.1.9.tar` & `pymafia-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,49 @@
--rw-r--r--   0        0        0     1068 2023-03-09 20:00:06.534800 pymafia-0.1.9/LICENSE
--rw-r--r--   0        0        0     1896 2023-03-09 20:00:06.534800 pymafia-0.1.9/README.md
--rw-r--r--   0        0        0      855 2023-03-09 20:00:42.843985 pymafia-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      371 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/__init__.py
--rw-r--r--   0        0        0     4125 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/ash.py
--rw-r--r--   0        0        0     1431 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/combat.py
--rw-r--r--   0        0        0     1085 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/__init__.py
--rw-r--r--   0        0        0     2483 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/bounty.py
--rw-r--r--   0        0        0     1819 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/class_.py
--rw-r--r--   0        0        0     2363 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/coinmaster.py
--rw-r--r--   0        0        0     2641 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/effect.py
--rw-r--r--   0        0        0     2215 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/element.py
--rw-r--r--   0        0        0     6764 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/familiar.py
--rw-r--r--   0        0        0    11459 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/item.py
--rw-r--r--   0        0        0     4568 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/location.py
--rw-r--r--   0        0        0     5882 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/monster.py
--rw-r--r--   0        0        0     2064 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/path.py
--rw-r--r--   0        0        0     1595 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/phylum.py
--rw-r--r--   0        0        0     2508 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/servant.py
--rw-r--r--   0        0        0     3256 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/skill.py
--rw-r--r--   0        0        0     1289 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/slot.py
--rw-r--r--   0        0        0     1352 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/stat.py
--rw-r--r--   0        0        0     2416 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/thrall.py
--rw-r--r--   0        0        0     2190 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/vykea.py
--rw-r--r--   0        0        0     1223 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/datatypes/zodiac.py
--rw-r--r--   0        0        0      254 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/__init__.py
--rw-r--r--   0        0        0      583 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/barrel_god.py
--rw-r--r--   0        0        0      890 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/boxing_daycare.py
--rw-r--r--   0        0        0     1350 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/cartography.py
--rw-r--r--   0        0        0     1030 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/cosplay_saber.py
--rw-r--r--   0        0        0     1784 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/crimbo_shrub.py
--rw-r--r--   0        0        0     1286 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/god_lobster.py
--rw-r--r--   0        0        0     1569 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/love_tunnel.py
--rw-r--r--   0        0        0     1054 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/mumming_trunk.py
--rw-r--r--   0        0        0     3518 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/pantogram.py
--rw-r--r--   0        0        0     1597 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/protonic_pack.py
--rw-r--r--   0        0        0     1139 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/snojo.py
--rw-r--r--   0        0        0     1299 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/songboom.py
--rw-r--r--   0        0        0      670 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/stomping_boots.py
--rw-r--r--   0        0        0     1408 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/iotms/witchess.py
--rw-r--r--   0        0        0     2150 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/kolmafia.py
--rw-r--r--   0        0        0     1689 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/player.py
--rw-r--r--   0        0        0     1148 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/preference.py
--rw-r--r--   0        0        0     1283 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/utils.py
--rw-r--r--   0        0        0     1350 2023-03-09 20:00:06.534800 pymafia-0.1.9/src/pymafia/wanderer.py
--rw-r--r--   0        0        0     2531 1970-01-01 00:00:00.000000 pymafia-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-21 15:26:57.097055 pymafia-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1896 2023-04-21 15:26:57.097055 pymafia-0.2.0/README.md
+-rw-r--r--   0        0        0     1265 2023-04-21 15:27:38.661594 pymafia-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      384 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/__init__.py
+-rw-r--r--   0        0        0      247 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/ash/__init__.py
+-rw-r--r--   0        0        0     3193 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/ash/conversion.py
+-rw-r--r--   0        0        0     1421 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/ash/library.py
+-rw-r--r--   0        0        0     1431 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/combat.py
+-rw-r--r--   0        0        0     1449 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/__init__.py
+-rw-r--r--   0        0        0     2379 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/bounty.py
+-rw-r--r--   0        0        0     1776 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/class_.py
+-rw-r--r--   0        0        0     2389 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/coinmaster.py
+-rw-r--r--   0        0        0     2445 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/effect.py
+-rw-r--r--   0        0        0     1995 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/element.py
+-rw-r--r--   0        0        0     6757 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/familiar.py
+-rw-r--r--   0        0        0    11438 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/item.py
+-rw-r--r--   0        0        0     5269 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/location.py
+-rw-r--r--   0        0        0     6646 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/monster.py
+-rw-r--r--   0        0        0     1914 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/path.py
+-rw-r--r--   0        0        0     1359 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/phylum.py
+-rw-r--r--   0        0        0     2699 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/servant.py
+-rw-r--r--   0        0        0     3100 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/skill.py
+-rw-r--r--   0        0        0      990 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/slot.py
+-rw-r--r--   0        0        0     1059 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/stat.py
+-rw-r--r--   0        0        0     2547 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/thrall.py
+-rw-r--r--   0        0        0     2829 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/datatypes/vykea.py
+-rw-r--r--   0        0        0      545 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/__init__.py
+-rw-r--r--   0        0        0      583 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/barrel_god.py
+-rw-r--r--   0        0        0      890 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/boxing_daycare.py
+-rw-r--r--   0        0        0     1350 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/cartography.py
+-rw-r--r--   0        0        0     1030 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/cosplay_saber.py
+-rw-r--r--   0        0        0     1784 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/crimbo_shrub.py
+-rw-r--r--   0        0        0     1286 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/god_lobster.py
+-rw-r--r--   0        0        0     1569 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/love_tunnel.py
+-rw-r--r--   0        0        0     1044 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/mumming_trunk.py
+-rw-r--r--   0        0        0     3518 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/pantogram.py
+-rw-r--r--   0        0        0     1597 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/protonic_pack.py
+-rw-r--r--   0        0        0     1139 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/snojo.py
+-rw-r--r--   0        0        0     1299 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/songboom.py
+-rw-r--r--   0        0        0      670 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/stomping_boots.py
+-rw-r--r--   0        0        0     1408 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/iotms/witchess.py
+-rw-r--r--   0        0        0      125 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/kolmafia/__init__.py
+-rw-r--r--   0        0        0     1471 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/kolmafia/kolmafia.py
+-rw-r--r--   0        0        0     1572 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/kolmafia/patch.py
+-rw-r--r--   0        0        0     1689 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/player.py
+-rw-r--r--   0        0        0     1148 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/preference.py
+-rw-r--r--   0        0        0     1277 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/utils.py
+-rw-r--r--   0        0        0     1350 2023-04-21 15:26:57.097055 pymafia-0.2.0/src/pymafia/wanderer.py
+-rw-r--r--   0        0        0     2568 1970-01-01 00:00:00.000000 pymafia-0.2.0/PKG-INFO
```

### Comparing `pymafia-0.1.9/LICENSE` & `pymafia-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/README.md` & `pymafia-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/pyproject.toml` & `pymafia-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,60 @@
 [tool.poetry]
 name = "pymafia"
-version = "0.1.9"  # This is the standard placeholder for poetry-dynamic-versioning
-description = "A Python module and bridge for reflecting KoLmafia's Java environment."
+version = "0.2.0"  # This is the standard placeholder for poetry-dynamic-versioning
+description = "A Python module and bridge for reflecting KoLmafia's Java environment"
 license = "MIT"
 authors = ["MrFizzyBubbs <MrFizzyBubbs@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MrFizzyBubbs/pymafia"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pyjnius = "^1.4.2"
+JPype1 = "^1.4.1"
+wrapt = "^1.15.0"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.15.1"
-black = "^22.6.0"
+black = "^23.3.0"
 isort = "^5.10.1"
 docformatter = "^1.5.0"
 mypy = "^0.971"
+pytest = "^7.2.2"
+pytest-cov = "^4.0.0"
+pre-commit = "^3.2.2"
+yamlfix = "^1.9.0"
 
 [tool.isort]
 profile = "black"
 
+[tool.ruff]
+ignore = [
+  "E501",  # Line too long, handled by black
+]
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = [
+  "F401",  # Unused import
+  "F403",  # Wildcard import
+]
+"tests/__init__.py" = [
+  "E722",  # Bare except
+]
+
 [tool.mypy]
 ignore_missing_imports = true
 
+[tool.yamlfix]
+explicit_start = false
+
 [tool.poetry-dynamic-versioning]
 enable = false
 format = "{base}"
 style = "pep440"
 strict = true
 
+[tool.pytest.ini_options]
+pythonpath = "src"
+
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `pymafia-0.1.9/src/pymafia/combat.py` & `pymafia-0.2.0/src/pymafia/combat.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/datatypes/bounty.py` & `pymafia-0.2.0/src/pymafia/datatypes/thrall.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,91 @@
 from __future__ import annotations
 
-from functools import total_ordering
+from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
-    from .location import Location
-    from .monster import Monster
+    from pymafia.datatypes.skill import Skill
 
 
-@total_ordering
-class Bounty:
-    name: str = "none"
-
-    def __init__(self, key: str | None = None):
-        if key.casefold() == self.name.casefold() or key is None:
+@dataclass(frozen=True, order=True)
+class Thrall:
+    data: Any = field(default=km.DataTypes.THRALL_INIT.content, compare=False)
+    id: int = km.DataTypes.THRALL_INIT.contentLong
+    type: str = km.DataTypes.THRALL_INIT.contentString
+
+    def __init__(self, key: int | str | None = None):
+        if (isinstance(key, str) and key.casefold() == self.type.casefold()) or key in (
+            self.id,
+            None,
+        ):
             return
 
-        bounties = km.BountyDatabase.getMatchingNames(key)
-        if len(bounties) != 1:
+        data = (
+            km.PastaThrallData.typeToData(key)
+            if isinstance(key, str)
+            else km.PastaThrallData.idToData(key)
+        )
+        if data is None:
             raise ValueError(f"{type(self).__name__} {key!r} not found")
 
-        canonical = bounties[0]
-        self.name = km.BountyDatabase.canonicalToName(canonical)
+        object.__setattr__(self, "data", data)
+        object.__setattr__(self, "id", km.PastaThrallData.dataToId(data))
+        object.__setattr__(self, "type", km.PastaThrallData.dataToType(data))
 
     def __str__(self) -> str:
-        return self.name
+        return self.type
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({str(self)!r})"
 
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.name == other.name
-        return NotImplemented
-
-    def __lt__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.name < other.name
-        return NotImplemented
-
     def __bool__(self) -> bool:
-        return self.name != type(self).name
+        return self != type(self)()
 
     @classmethod
-    def all(cls) -> list[Bounty]:
-        from pymafia import ash
+    def all(cls) -> list[Thrall]:
+        from pymafia.ash import from_java
 
-        values = km.DataTypes.BOUNTY_TYPE.allValues()
-        return sorted(ash.to_python(values))
+        values = km.DataTypes.THRALL_TYPE.allValues()
+        return sorted(from_java(values))
 
     @property
-    def plural(self) -> str:
-        return km.BountyDatabase.getPlural(self.name) or ""
+    def thrall(self) -> Any:
+        return km.KoLCharacter.findPastaThrall(self.type)
 
     @property
-    def type_(self) -> str:
-        return km.BountyDatabase.getType(self.name) or ""
+    def name(self) -> str:
+        return self.thrall.getName() if self.thrall else ""
 
     @property
-    def kol_internal_type(self) -> str | None:
-        match self.type_:
-            case "easy":
-                return "low"
-            case "hard":
-                return "high"
-            case "special":
-                return "special"
-            case _:
-                return None
+    def level(self) -> int:
+        return self.thrall.getLevel() if self.thrall else 0
 
     @property
-    def number(self) -> int:
-        return km.BountyDatabase.getNumber(self.name)
+    def image(self) -> str:
+        return (
+            km.PastaThrallData.dataToImage(self.data) if self.data is not None else ""
+        )
 
     @property
-    def image(self) -> str:
-        return km.BountyDatabase.getImage(self.name) or ""
+    def tinyimage(self) -> str:
+        return (
+            km.PastaThrallData.dataToTinyImage(self.data)
+            if self.data is not None
+            else ""
+        )
 
     @property
-    def monster(self) -> Monster:
-        from .monster import Monster
+    def skill(self) -> Skill:
+        from pymafia.datatypes.skill import Skill
 
-        return Monster(km.BountyDatabase.getMonster(self.name))
+        return Skill(
+            km.PastaThrallData.dataToSkillId(self.data)
+            if self.data is not None
+            else None
+        )
 
     @property
-    def location(self) -> Location:
-        from .location import Location
-
-        return Location(km.BountyDatabase.getLocation(self.name))
+    def current_modifiers(self) -> str:
+        return self.thrall.getCurrentModifiers() if self.thrall else ""
```

### Comparing `pymafia-0.1.9/src/pymafia/datatypes/class_.py` & `pymafia-0.2.0/src/pymafia/datatypes/class_.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,57 @@
 from __future__ import annotations
 
-from functools import total_ordering
+from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
-    from .stat import Stat
+    from pymafia.datatypes.stat import Stat
 
 
-@total_ordering
+@dataclass(frozen=True, order=True)
 class Class:
-    id: int = -1
-    name: str = "none"
-    ascension_class: Any = None
+    ascension_class: Any = field(default=km.DataTypes.CLASS_INIT.content, compare=False)
+    id: int = km.DataTypes.CLASS_INIT.contentLong
+    name: str = km.DataTypes.CLASS_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
-        if key.casefold() == self.name.casefold() or key in (self.id, None):
+        if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
+            self.id,
+            None,
+        ):
             return
 
         ascension_class = km.AscensionClass.find(key)
         if ascension_class is None or ascension_class.getId() < 0:
             raise ValueError(f"{type(self).__name__} {key!r} not found")
 
-        self.id = ascension_class.getId()
-        self.name = ascension_class.getName()
-        self.ascension_class = ascension_class
+        object.__setattr__(self, "ascension_class", ascension_class)
+        object.__setattr__(self, "id", ascension_class.getId())
+        object.__setattr__(self, "name", ascension_class.getName())
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({str(self)!r})"
 
-    def __hash__(self) -> int:
-        return hash(self.id)
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.id == other.id
-        return NotImplemented
-
-    def __lt__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.id < other.id
-        return NotImplemented
-
     def __bool__(self) -> bool:
-        return self.id != type(self).id
+        return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Class]:
-        from pymafia import ash
+        from pymafia.ash import from_java
 
         values = km.DataTypes.CLASS_TYPE.allValues()
-        return sorted(ash.to_python(values))
+        return sorted(from_java(values))
 
     @property
     def primestat(self) -> Stat:
-        from .stat import Stat
+        from pymafia.datatypes.stat import Stat
 
-        if not self:
-            return Stat(None)
+        if self.ascension_class is None:
+            return Stat()
         prime_index = self.ascension_class.getPrimeStatIndex()
         name = km.AdventureResult.STAT_NAMES[prime_index]
         return Stat(name)
```

### Comparing `pymafia-0.1.9/src/pymafia/datatypes/coinmaster.py` & `pymafia-0.2.0/src/pymafia/datatypes/coinmaster.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,81 @@
 from __future__ import annotations
 
-from functools import total_ordering
+from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
-    from .item import Item
+    from pymafia.datatypes.item import Item
 
 
-@total_ordering
+@dataclass(frozen=True, order=True)
 class Coinmaster:
-    name: str = "none"
-    coinmaster: Any = None
+    coinmaster: Any = field(default=km.DataTypes.COINMASTER_INIT.content, compare=False)
+    name: str = km.DataTypes.COINMASTER_INIT.contentString
 
     def __init__(self, key: str | None = None):
-        if key.casefold() == self.name.casefold() or key is None:
+        if (
+            isinstance(key, str) and key.casefold() == self.name.casefold()
+        ) or key is None:
             return
 
         coinmaster = km.CoinmasterRegistry.findCoinmaster(key)
         if coinmaster is None:
             raise ValueError(f"{type(self).__name__} {key!r} not found")
 
-        self.name = coinmaster.getMaster()
-        self.coinmaster = coinmaster
+        object.__setattr__(self, "coinmaster", coinmaster)
+        object.__setattr__(self, "name", coinmaster.getMaster())
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({str(self)!r})"
 
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.name == other.name
-        return NotImplemented
-
-    def __lt__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.name < other.name
-        return NotImplemented
-
     def __bool__(self) -> bool:
-        return self.name != type(self).name
+        return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Coinmaster]:
-        from pymafia import ash
+        from pymafia.ash import from_java
 
         values = km.DataTypes.COINMASTER_TYPE.allValues()
-        return sorted(ash.to_python(values))
+        return from_java(values)
 
     @property
     def token(self) -> str:
-        return self.coinmaster.getToken() if self else ""
+        return self.coinmaster.getToken() if self.coinmaster else ""
 
     @property
     def item(self) -> Item:
-        from .item import Item
+        from pymafia.datatypes.item import Item
 
-        if not self:
-            return Item(None)
+        if self.coinmaster is None:
+            return Item()
         item = self.coinmaster.getItem()
-        return Item(None) if item is None else Item(item.getItemId())
+        return Item(item.getItemId()) if item is not None else Item()
 
     @property
     def preference(self) -> str:
-        return self.coinmaster.getProperty() if self else ""
+        return self.coinmaster.getProperty() if self.coinmaster is not None else ""
 
     @property
     def available_tokens(self) -> int:
-        return self.coinmaster.availableTokens() if self else 0
+        return self.coinmaster.availableTokens() if self.coinmaster is not None else 0
 
     @property
     def buys(self) -> bool:
-        return self.coinmaster.getSellAction() is not None if self else False
+        return (
+            self.coinmaster is not None and self.coinmaster.getSellAction() is not None
+        )
 
     @property
     def sells(self) -> bool:
-        return self.coinmaster.getBuyAction() is not None if self else False
+        return (
+            self.coinmaster is not None and self.coinmaster.getBuyAction() is not None
+        )
 
     @property
     def nickname(self) -> str:
-        return self.coinmaster.getNickname() if self else ""
+        return self.coinmaster.getNickname() if self.coinmaster is not None else ""
```

### Comparing `pymafia-0.1.9/src/pymafia/datatypes/effect.py` & `pymafia-0.2.0/src/pymafia/datatypes/effect.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,58 @@
 from __future__ import annotations
 
+from dataclasses import dataclass
 from enum import IntEnum
-from functools import total_ordering
-from typing import Any
 
 from pymafia.kolmafia import km
 
 
 class EffectQuality(IntEnum):
     NONE = -1
     GOOD = 0
     NEUTRAL = 1
     BAD = 2
 
 
-@total_ordering
+@dataclass(frozen=True, order=True)
 class Effect:
-    id: int = -1
-    name: str = "none"
+    id: int = km.DataTypes.EFFECT_INIT.contentLong
+    name: str = km.DataTypes.EFFECT_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
-        if key.casefold() == self.name.casefold() or key in (self.id, None):
+        if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
+            self.id,
+            None,
+        ):
             return
 
         id = km.EffectDatabase.getEffectId(key) if isinstance(key, str) else key
         name = km.EffectDatabase.getEffectName(id)
         if name is None:
             raise ValueError(f"{type(self).__name__} {key!r} not found")
 
-        self.id = id
-        self.name = name
+        object.__setattr__(self, "id", id)
+        object.__setattr__(self, "name", name)
 
     def __str__(self) -> str:
         ids = km.EffectDatabase.getEffectIds(self.name, False)
         return f"[{self.id}]{self.name}" if len(ids) > 1 else self.name
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({str(self)!r})"
 
-    def __hash__(self) -> int:
-        return hash(self.id)
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.id == other.id
-        return NotImplemented
-
-    def __lt__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.id < other.id
-        return NotImplemented
-
     def __bool__(self) -> bool:
-        return self.id != type(self).id
+        return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Effect]:
-        from pymafia import ash
+        from pymafia.ash import from_java
 
         values = km.DataTypes.EFFECT_TYPE.allValues()
-        return sorted(ash.to_python(values))
+        return sorted(from_java(values))
 
     @property
     def default(self) -> str:
         return km.EffectDatabase.getDefaultAction(self.id) or ""
 
     @property
     def actions(self) -> list[str]:
@@ -72,15 +61,15 @@
     @property
     def quality(self) -> EffectQuality:
         return EffectQuality(km.EffectDatabase.getQuality(self.id))
 
     @property
     def attributes(self) -> list[str]:
         attrs = km.EffectDatabase.getEffectAttributes(self.id)
-        return [] if attrs is None else list(attrs)
+        return list(attrs) if attrs is not None else []
 
     @property
     def note(self) -> str:
         return km.EffectDatabase.getActionNote(self.id) or ""
 
     @property
     def image(self) -> str:
```

### Comparing `pymafia-0.1.9/src/pymafia/datatypes/element.py` & `pymafia-0.2.0/src/pymafia/datatypes/element.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,62 @@
 from __future__ import annotations
 
-from functools import total_ordering
+from dataclasses import dataclass, field
 from typing import Any
 
 from pymafia.kolmafia import km
 
-MonsterDatabaseElement = getattr(km, "persistence.MonsterDatabase$Element")
 
-
-@total_ordering
+@dataclass(frozen=True, order=True)
 class Element:
-    name: str = "none"
-    element: Any = None
+    element: Any = field(default=km.DataTypes.ELEMENT_INIT.content, compare=False)
+    name: str = km.DataTypes.ELEMENT_INIT.contentString
 
     def __init__(self, key: str | None = None):
-        if key.casefold() == self.name.casefold() or key is None:
+        if (
+            isinstance(key, str) and key.casefold() == self.name.casefold()
+        ) or key is None:
             return
 
         element = km.MonsterDatabase.stringToElement(key)
-        if element == MonsterDatabaseElement.NONE:
+        if element == km.MonsterDatabase.Element.NONE:
             raise ValueError(f"{type(self).__name__} {key!r} not found")
 
-        self.name = element.toString()
-        self.element = element
+        object.__setattr__(self, "element", element)
+        object.__setattr__(self, "name", element.toString())
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({str(self)!r})"
 
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.name == other.name
-        return NotImplemented
-
-    def __lt__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.name < other.name
-        return NotImplemented
-
     def __bool__(self) -> bool:
-        return self.name != type(self).name
+        return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Element]:
-        from pymafia import ash
+        from pymafia.ash import from_java
 
         values = km.DataTypes.ELEMENT_TYPE.allValues()
-        return sorted(ash.to_python(values))
+        return from_java(values)
 
     @property
     def image(self) -> str:
         # No image for Slime or Supercold in Manuel
         if self.element in [
-            MonsterDatabaseElement.NONE,
-            MonsterDatabaseElement.SLIME,
-            MonsterDatabaseElement.SUPERCOLD,
+            km.MonsterDatabase.Element.NONE,
+            km.MonsterDatabase.Element.SLIME,
+            km.MonsterDatabase.Element.SUPERCOLD,
         ]:
             return "circle.gif"
-        if self.element == MonsterDatabaseElement.COLD:
+        if self.element == km.MonsterDatabase.Element.COLD:
             return "snowflake.gif"
-        if self.element == MonsterDatabaseElement.HOT:
+        if self.element == km.MonsterDatabase.Element.HOT:
             return "fire.gif"
-        if self.element == MonsterDatabaseElement.SLEAZE:
+        if self.element == km.MonsterDatabase.Element.SLEAZE:
             return "wink.gif"
-        if self.element == MonsterDatabaseElement.SPOOKY:
+        if self.element == km.MonsterDatabase.Element.SPOOKY:
             return "skull.gif"
-        if self.element == MonsterDatabaseElement.STENCH:
+        if self.element == km.MonsterDatabase.Element.STENCH:
             return "stench.gif"
         return ""
```

### Comparing `pymafia-0.1.9/src/pymafia/datatypes/familiar.py` & `pymafia-0.2.0/src/pymafia/datatypes/familiar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,69 +1,62 @@
 from __future__ import annotations
 
-from functools import total_ordering
-from typing import TYPE_CHECKING, Any
+from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
-    from .item import Item
+    from pymafia.datatypes.item import Item
 
 
-@total_ordering
+@dataclass(frozen=True, order=True)
 class Familiar:
-    id: int = -1
-    name: str = "none"
+    id: int = km.DataTypes.FAMILIAR_INIT.contentLong
+    name: str = km.DataTypes.FAMILIAR_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
-        if key.casefold() == self.name.casefold() or key in (self.id, None):
+        if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
+            self.id,
+            None,
+        ):
             return
 
         id = km.FamiliarDatabase.getFamiliarId(key) if isinstance(key, str) else key
         name = km.FamiliarDatabase.getFamiliarName(id)
         if name is None:
             raise ValueError(f"{type(self).__name__} {key!r} not found")
 
-        self.id = id
-        self.name = name
+        object.__setattr__(self, "id", id)
+        object.__setattr__(self, "name", name)
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({str(self)!r})"
 
-    def __hash__(self) -> int:
-        return hash(self.id)
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.id == other.id
-        return NotImplemented
-
-    def __lt__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.id < other.id
-        return NotImplemented
-
     def __bool__(self) -> bool:
-        return self.id != type(self).id
+        return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Familiar]:
-        from pymafia import ash
+        from pymafia.ash import from_java
 
         values = km.DataTypes.FAMILIAR_TYPE.allValues()
-        return sorted(ash.to_python(values))
+        return sorted(from_java(values))
 
     @property
     def hatchling(self) -> Item:
-        from .item import Item
+        from pymafia.datatypes.item import Item
 
-        return Item(km.FamiliarDatabase.getFamiliarLarva(self.id))
+        try:
+            return Item(km.FamiliarDatabase.getFamiliarLarva(self.id))
+        except ValueError:
+            return Item()
 
     @property
     def image(self) -> str:
         return km.FamiliarDatabase.getFamiliarImageLocation(self.id)
 
     @property
     def nickname(self) -> str:
@@ -92,18 +85,18 @@
 
     @property
     def drop_name(self) -> str:
         return km.FamiliarData.dropName(self.id) or ""
 
     @property
     def drop_item(self) -> Item:
-        from .item import Item
+        from pymafia.datatypes.item import Item
 
         item = km.FamiliarData.dropItem(self.id)
-        return Item(item.getItemId() if item is not None else None)
+        return Item(item.getItemId()) if item is not None else Item()
 
     @property
     def drops_today(self) -> int:
         return km.FamiliarData.dropsToday(self.id)
 
     @property
     def drops_limit(self) -> int:
@@ -172,63 +165,63 @@
     @property
     def variable(self) -> bool:
         return km.FamiliarDatabase.isVariableType(self.id)
 
     @property
     def attributes(self) -> list[str]:
         attrs = km.FamiliarDatabase.getFamiliarAttributes(self.id)
-        return [] if attrs is None else list(attrs)
+        return list(attrs) if attrs is not None else []
 
     @property
     def poke_level(self) -> int:
         fam = km.KoLCharacter.usableFamiliar(self.id)
-        return 0 if fam is None else fam.getPokeLevel()
+        return fam.getPokeLevel() if fam is not None else 0
 
     @property
     def poke_level_2_power(self) -> int:
         data = km.FamiliarDatabase.getPokeDataById(self.id)
-        return 0 if data is None else data.getPower2()
+        return data.getPower2() if data is not None else 0
 
     @property
     def poke_level_2_hp(self) -> int:
         data = km.FamiliarDatabase.getPokeDataById(self.id)
-        return 0 if data is None else data.getHP2()
+        return data.getHP2() if data is not None else 0
 
     @property
     def poke_level_3_power(self) -> int:
         data = km.FamiliarDatabase.getPokeDataById(self.id)
-        return 0 if data is None else data.getPower3()
+        return data.getPower3() if data is not None else 0
 
     @property
     def poke_level_3_hp(self) -> int:
         data = km.FamiliarDatabase.getPokeDataById(self.id)
-        return 0 if data is None else data.getHP3()
+        return data.getHP3() if data is not None else 0
 
     @property
     def poke_level_4_power(self) -> int:
         data = km.FamiliarDatabase.getPokeDataById(self.id)
-        return 0 if data is None else data.getPower4()
+        return data.getPower4() if data is not None else 0
 
     @property
     def poke_level_4_hp(self) -> int:
         data = km.FamiliarDatabase.getPokeDataById(self.id)
-        return 0 if data is None else data.getHP4()
+        return data.getHP4() if data is not None else 0
 
     @property
     def poke_move_1(self) -> str:
         data = km.FamiliarDatabase.getPokeDataById(self.id)
-        return "" if data is None else data.getMove1()
+        return data.getMove1() if data is not None else ""
 
     @property
     def poke_move_2(self) -> str:
         data = km.FamiliarDatabase.getPokeDataById(self.id)
-        return "" if data is None else data.getMove2()
+        return data.getMove2() if data is not None else ""
 
     @property
     def poke_move_3(self) -> str:
         data = km.FamiliarDatabase.getPokeDataById(self.id)
-        return "" if data is None else data.getMove3()
+        return data.getMove3() if data is not None else ""
 
     @property
     def poke_attribute(self) -> str:
         data = km.FamiliarDatabase.getPokeDataById(self.id)
-        return "" if data is None else data.getAttribute()
+        return data.getAttribute() if data is not None else ""
```

### Comparing `pymafia-0.1.9/src/pymafia/datatypes/item.py` & `pymafia-0.2.0/src/pymafia/datatypes/item.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,67 @@
 from __future__ import annotations
 
+from dataclasses import dataclass
 from enum import Enum
-from functools import total_ordering
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING
+
+from jpype import JClass
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
-    from .coinmaster import Coinmaster
-    from .skill import Skill
-
+    from pymafia.datatypes.coinmaster import Coinmaster
+    from pymafia.datatypes.skill import Skill
 
-class ConsumableQuality(Enum):
-    NONE = ""
-    CRAPPY = "crappy"
-    DECENT = "decent"
-    GOOD = "good"
-    AWESOME = "awesome"
-    EPIC = "EPIC"
-    QUEST = "quest"
-    CHANGING = "???"
-    DRIPPY = "drippy"
-    SUSHI = "sushi"
+EnumSet = JClass("java.util.EnumSet")
 
 
 class CandyType(Enum):
-    NONE = "none"
-    UNSPADED = "unspaded"
-    SIMPLE = "simple"
-    COMPLEX = "complex"
+    NONE = km.CandyDatabase.CandyType.NONE
+    UNSPADED = km.CandyDatabase.CandyType.UNSPADED
+    SIMPLE = km.CandyDatabase.CandyType.SIMPLE
+    COMPLEX = km.CandyDatabase.CandyType.COMPLEX
 
 
-@total_ordering
+@dataclass(frozen=True, order=True)
 class Item:
-    id: int = -1
-    name: str = "none"
+    id: int = km.DataTypes.ITEM_INIT.contentLong
+    name: str = km.DataTypes.ITEM_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
-        if key.casefold() == self.name.casefold() or key in (self.id, None):
+        if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
+            self.id,
+            None,
+        ):
             return
 
         id = km.ItemDatabase.getItemId(key) if isinstance(key, str) else key
         name = km.ItemDatabase.getItemDataName(id)
         if name is None:
             raise ValueError(f"{type(self).__name__} {key!r} not found")
 
-        self.id = id
-        self.name = name
+        object.__setattr__(self, "id", id)
+        object.__setattr__(self, "name", name)
 
     def __str__(self) -> str:
         ids = km.ItemDatabase.getItemIds(self.name, 1, False)
         return f"[{self.id}]{self.name}" if len(ids) > 1 else self.name
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({str(self)!r})"
 
-    def __hash__(self) -> int:
-        return hash(self.id)
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.id == other.id
-        return NotImplemented
-
-    def __lt__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.id < other.id
-        return NotImplemented
-
     def __bool__(self) -> bool:
-        return self.id != type(self).id
+        return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Item]:
-        from pymafia import ash
+        from pymafia.ash import from_java
 
         values = km.DataTypes.ITEM_TYPE.allValues()
-        return sorted(ash.to_python(values))
+        return sorted(from_java(values))
 
     @property
     def tcrs_name(self) -> str:
         """Return the name of the Item as it appears in your current Two Crazy Random Summer run. If you are not in a TCRS run, the regular Item name is returned."""
         return km.TCRSDatabase.getTCRSName(self.id) or ""
 
     @property
@@ -108,37 +89,37 @@
 
     @property
     def levelreq(self) -> int:
         """Return the level requirement for consuming or equipping the Item."""
         return km.ConsumablesDatabase.getLevelReqByName(self.name) or 0
 
     @property
-    def quality(self) -> ConsumableQuality:
+    def quality(self) -> str:
         """Return the quality of the Item if it is a consumable."""
-        return ConsumableQuality(km.ConsumablesDatabase.getQuality(self.name).getName())
+        return km.ConsumablesDatabase.getQuality(self.name).getName()
 
     @property
     def adventures(self) -> str:
         """Return the range of adventures gained from consuming the Item. The string will either contain the adventures for invariant gains, or a hyphen-separated minimum and maximum for variant gains."""
-        return km.ConsumablesDatabase.getAdvRangeByName(self.name)
+        return km.ConsumablesDatabase.getBaseAdventureRange(self.name)
 
     @property
     def muscle(self) -> str:
         """Return the range of muscle substats gained from consuming the Item. The string will either contain the substats for invariant gains, or a hyphen-separated minimum and maximum for variant gains. Note that substat gains can be negative."""
-        return km.ConsumablesDatabase.getMuscleByName(self.name)
+        return km.ConsumablesDatabase.getBaseMuscleByName(self.name)
 
     @property
     def mysticality(self) -> str:
         """Return the range of mysticality substats gained from consuming the Item. The string will either contain the substats for invariant gains, or a hyphen-separated minimum and maximum for variant gains. Note that substat gains can be negative."""
-        return km.ConsumablesDatabase.getMysticalityByName(self.name)
+        return km.ConsumablesDatabase.getBaseMysticalityByName(self.name)
 
     @property
     def moxie(self) -> str:
         """Return the range of moxie substats gained from consuming the Item. The string will either contain the substats for invariant gains, or a hyphen-separated minimum and maximum for variant gains. Note that substat gains can be negative."""
-        return km.ConsumablesDatabase.getMoxieByName(self.name)
+        return km.ConsumablesDatabase.getBaseMoxieByName(self.name)
 
     @property
     def fullness(self) -> int:
         """Return the stomach size of Item. If the Item is not edible, return 0."""
         return km.ConsumablesDatabase.getFullness(self.name)
 
     @property
@@ -206,37 +187,39 @@
     def discardable(self) -> bool:
         """Return True if the Item is discardable, else False."""
         return km.ItemDatabase.isDiscardable(self.id)
 
     @property
     def combat(self) -> bool:
         """Return True if the Item is usable in combat, else False. This returns True whether the Item is consumed by being used or not."""
-        return km.ItemDatabase.getAttribute(
-            self.id, km.ItemDatabase.ATTR_COMBAT | km.ItemDatabase.ATTR_COMBAT_REUSABLE
+        mask = EnumSet.of(
+            km.ItemDatabase.Attribute.COMBAT,
+            km.ItemDatabase.Attribute.COMBAT_REUSABLE,
         )
+        return km.ItemDatabase.getAttribute(self.id, mask)
 
     @property
     def combat_reusable(self) -> bool:
         """Return True if the Item is usable in combat and is not consumed when doing so, else False."""
         return km.ItemDatabase.getAttribute(
-            self.id, km.ItemDatabase.ATTR_COMBAT_REUSABLE
+            self.id, km.ItemDatabase.Attribute.COMBAT_REUSABLE
         )
 
     @property
     def usable(self) -> bool:
         """Return True if the Item is usable, else False. This returns True whether the Item is consumed by being used or not."""
         return km.ItemDatabase.isUsable(self.id)
 
     @property
     def reusable(self) -> bool:
         """Return True if the Item is usable and is not consumed when doing so, else False."""
         return km.ItemDatabase.getConsumptionType(
             self.id
-        ) == km.KoLConstants.INFINITE_USES or km.ItemDatabase.getAttribute(
-            self.id, km.ItemDatabase.ATTR_REUSABLE
+        ) == km.KoLConstants.ConsumptionType.USE_INFINITE or km.ItemDatabase.getAttribute(
+            self.id, km.ItemDatabase.Attribute.REUSABLE
         )
 
     @property
     def multi(self) -> bool:
         """Return True if the Item is multiusable, else False."""
         return km.ItemDatabase.isMultiUsable(self.id)
 
@@ -284,31 +267,34 @@
     def potion(self) -> bool:
         """Return True if the Item is a potion, else False."""
         return km.ItemDatabase.isPotion(self.id)
 
     @property
     def seller(self) -> Coinmaster:
         """Return which Coinmaster sells this Item, if any."""
-        from .coinmaster import Coinmaster
+        from pymafia.datatypes.coinmaster import Coinmaster
 
         data = km.CoinmasterRegistry.findSeller(self.id)
-        return Coinmaster(data.getMaster() if data is not None else None)
+        return Coinmaster(data.getMaster()) if data is not None else Coinmaster()
 
     @property
     def buyer(self) -> Coinmaster:
         """Return which Coinmaster buys this Item, if any."""
-        from .coinmaster import Coinmaster
+        from pymafia.datatypes.coinmaster import Coinmaster
 
         data = km.CoinmasterRegistry.findBuyer(self.id)
-        return Coinmaster(data.getMaster() if data is not None else None)
+        return Coinmaster(data.getMaster()) if data is not None else Coinmaster()
 
     @property
     def name_length(self) -> int:
         """Return the length of the Item's display name."""
         return km.ItemDatabase.getNameLength(self.id)
 
     @property
     def noob_skill(self) -> Skill:
         """Return the noob Skill granted by absorbing this Item."""
-        from .skill import Skill
+        from pymafia.datatypes.skill import Skill
 
-        return Skill(km.ItemDatabase.getNoobSkillId(self.id))
+        try:
+            return Skill(km.ItemDatabase.getNoobSkillId(self.id))
+        except ValueError:
+            return Skill()
```

### Comparing `pymafia-0.1.9/src/pymafia/datatypes/monster.py` & `pymafia-0.2.0/src/pymafia/datatypes/monster.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,217 +1,217 @@
 from __future__ import annotations
 
-from functools import total_ordering
+from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any
 
+from jpype import JClass
+
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
-    from .effect import Effect
-    from .element import Element
-    from .phylum import Phylum
+    from pymafia.datatypes.effect import Effect
+    from pymafia.datatypes.element import Element
+    from pymafia.datatypes.phylum import Phylum
 
 
-Integer = km.autoclass("java.lang.Integer")
+Integer = JClass("java.lang.Integer")
 
 
-@total_ordering
+@dataclass(frozen=True, order=True)
 class Monster:
-    id: int = 0
-    name: str = "none"
-    monster: Any = None
+    monster: Any = field(default=km.DataTypes.MONSTER_INIT.content, compare=False)
+    id: int = km.DataTypes.MONSTER_INIT.contentLong
+    name: str = km.DataTypes.MONSTER_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
-        if key.casefold() == self.name.casefold() or key in (self.id, None):
+        if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
+            self.id,
+            None,
+        ):
             return
 
         monster = (
             km.MonsterDatabase.findMonster(key, True)
             if isinstance(key, str)
             else km.MonsterDatabase.findMonsterById(key)
         )
         if monster is None:
             raise ValueError(f"{type(self).__name__} {key!r} not found")
 
-        self.id = monster.getId()
-        self.name = monster.getName()
-        self.monster = monster
+        object.__setattr__(self, "monster", monster)
+        object.__setattr__(self, "id", monster.getId())
+        object.__setattr__(self, "name", monster.getName())
 
     def __str__(self) -> str:
         ids = km.MonsterDatabase.getMonsterIds(self.name, False)
         return f"[{self.id}]{self.name}" if len(ids) > 1 else self.name
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({str(self)!r})"
 
-    def __hash__(self) -> int:
-        return hash(self.id)
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.id == other.id
-        return NotImplemented
-
-    def __lt__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.id < other.id
-        return NotImplemented
-
     def __bool__(self) -> bool:
-        return self.id != type(self).id
+        return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Monster]:
-        from pymafia import ash
+        from pymafia.ash import from_java
 
         values = km.DataTypes.MONSTER_TYPE.allValues()
-        return sorted(ash.to_python(values))
+        return sorted(from_java(values))
 
     @property
     def article(self) -> str:
-        return self.monster.getArticle() if self else ""
+        return self.monster.getArticle() if self.monster is not None else ""
 
     @property
     def base_hp(self) -> int:
-        return self.monster.getHP() if self else 0
+        return self.monster.getHP() if self.monster is not None else 0
 
     @property
     def base_attack(self) -> int:
-        return self.monster.getAttack() if self else 0
+        return self.monster.getAttack() if self.monster is not None else 0
 
     @property
     def raw_hp(self) -> int:
-        return self.monster.getRawHP() if self else 0
+        return self.monster.getRawHP() if self.monster is not None else 0
 
     @property
     def raw_attack(self) -> int:
-        return self.monster.getRawAttack() if self else 0
+        return self.monster.getRawAttack() if self.monster is not None else 0
 
     @property
     def raw_defense(self) -> int:
-        return self.monster.getRawDefense() if self else 0
+        return self.monster.getRawDefense() if self.monster is not None else 0
 
     @property
     def base_defense(self) -> int:
-        return self.monster.getDefense() if self else 0
+        return self.monster.getDefense() if self.monster is not None else 0
 
     @property
     def base_initiative(self) -> int:
-        return self.monster.getInitiative() if self else 0
+        return self.monster.getInitiative() if self.monster is not None else 0
 
     @property
     def raw_initiative(self) -> int:
-        return self.monster.getRawInitiative() if self else 0
+        return self.monster.getRawInitiative() if self.monster is not None else 0
 
     @property
     def attack_element(self) -> Element:
-        from .element import Element
+        from pymafia.datatypes.element import Element
 
         return (
             Element(self.monster.getAttackElement().toString())
-            if self
-            else Element(None)
+            if self.monster is not None
+            else Element()
         )
 
     @property
     def attack_elements(self) -> list[Element]:
-        if not self:
+        from pymafia.datatypes.element import Element
+
+        if self.monster is None:
             return []
         return [Element(x.toString()) for x in self.monster.getAttackElements()]
 
     @property
     def defense_element(self) -> Element:
-        from .element import Element
+        from pymafia.datatypes.element import Element
 
         return (
             Element(self.monster.getDefenseElement().toString())
-            if self
-            else Element(None)
+            if self.monster is not None
+            else Element()
         )
 
     @property
     def physical_resistance(self) -> int:
-        return self.monster.getPhysicalResistance() if self else 0
+        return self.monster.getPhysicalResistance() if self.monster is not None else 0
 
     @property
     def elemental_resistance(self) -> int:
-        return self.monster.getElementalResistance() if self else 0
+        return self.monster.getElementalResistance() if self.monster is not None else 0
 
     @property
     def min_meat(self) -> int:
-        return self.monster.getMinMeat() if self else 0
+        return self.monster.getMinMeat() if self.monster is not None else 0
 
     @property
     def max_meat(self) -> int:
-        return self.monster.getMaxMeat() if self else 0
+        return self.monster.getMaxMeat() if self.monster is not None else 0
 
     @property
     def min_sprinkles(self) -> int:
-        return self.monster.getMinSprinkles() if self else 0
+        return self.monster.getMinSprinkles() if self.monster is not None else 0
 
     @property
     def max_sprinkles(self) -> int:
-        return self.monster.getMaxSprinkles() if self else 0
+        return self.monster.getMaxSprinkles() if self.monster is not None else 0
 
     @property
     def base_mainstat_exp(self) -> float:
-        return self.monster.getExperience() if self else 0
+        return self.monster.getExperience() if self.monster is not None else 0
 
     @property
     def group(self) -> int:
-        return self.monster.getGroup() if self else 0
+        return self.monster.getGroup() if self.monster is not None else 0
 
     @property
     def phylum(self) -> Phylum:
-        from .phylum import Phylum
+        from pymafia.datatypes.phylum import Phylum
 
-        return Phylum(self.monster.getPhylum().toString()) if self else Phylum(None)
+        return (
+            Phylum(self.monster.getPhylum().toString())
+            if self.monster is not None
+            else Phylum()
+        )
 
     @property
     def poison(self) -> Effect:
-        from .effect import Effect
+        from pymafia.datatypes.effect import Effect
 
-        if not self:
-            return Effect(None)
+        if self.monster is None:
+            return Effect()
         poison_level = self.monster.getPoison()
         if poison_level == Integer.MAX_VALUE:
-            return Effect(None)
+            return Effect()
         poison_name = km.EffectDatabase.getEffectName(
             km.EffectDatabase.POISON_ID[poison_level]
         )
         return Effect(poison_name)
 
     @property
     def boss(self) -> bool:
-        return self.monster.isBoss() if self else False
+        return self.monster.isBoss() if self.monster is not None else False
 
     @property
     def copyable(self) -> bool:
-        return self.monster.isNoCopy() if self else False
+        return self.monster.isNoCopy() if self.monster is not None else False
 
     @property
     def image(self) -> str:
-        return self.monster.getImage() if self else ""
+        return self.monster.getImage() if self.monster is not None else ""
 
     @property
     def images(self) -> list[str]:
-        return list(self.monster.getImages()) if self else []
+        return list(self.monster.getImages()) if self.monster is not None else []
 
     @property
     def random_modifiers(self) -> list[str]:
-        return list(self.monster.getRandomModifiers()) if self else []
+        return (
+            list(self.monster.getRandomModifiers()) if self.monster is not None else []
+        )
 
     @property
     def sub_types(self) -> list[str]:
-        return list(self.monster.getSubTypes()) if self else []
+        return list(self.monster.getSubTypes()) if self.monster is not None else []
 
     @property
     def manuel_name(self) -> str:
-        return self.monster.getManuelName() if self else ""
+        return self.monster.getManuelName() if self.monster is not None else ""
 
     @property
     def wiki_name(self) -> str:
-        return self.monster.getWikiName() if self else ""
+        return self.monster.getWikiName() if self.monster is not None else ""
 
     @property
     def attributes(self) -> str:
-        return self.monster.getAttributes() if self else ""
+        return self.monster.getAttributes() if self.monster is not None else ""
```

### Comparing `pymafia-0.1.9/src/pymafia/datatypes/servant.py` & `pymafia-0.2.0/src/pymafia/datatypes/servant.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,96 @@
 from __future__ import annotations
 
-from functools import total_ordering
+from dataclasses import dataclass, field
 from typing import Any
 
 from pymafia.kolmafia import km
 
 
-@total_ordering
+@dataclass(frozen=True, order=True)
 class Servant:
-    id: int = 0
-    name: str = "none"
-    data: Any = None
+    data: Any = field(default=km.DataTypes.SERVANT_INIT.content, compare=False)
+    id: int = km.DataTypes.SERVANT_INIT.contentLong
+    name: str = km.DataTypes.SERVANT_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
-        if key.casefold() == self.name.casefold() or key in (self.id, None):
+        if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
+            self.id,
+            None,
+        ):
             return
 
         data = (
             km.EdServantData.typeToData(key)
             if isinstance(key, str)
             else km.EdServantData.idToData(key)
         )
         if data is None:
             raise ValueError(f"{type(self).__name__} {key!r} not found")
 
-        self.id = km.EdServantData.dataToId(data)
-        self.name = km.EdServantData.dataToType(data)
-        self.data = data
+        object.__setattr__(self, "data", data)
+        object.__setattr__(self, "id", km.EdServantData.dataToId(data))
+        object.__setattr__(self, "name", km.EdServantData.dataToType(data))
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({str(self)!r})"
 
-    def __hash__(self) -> int:
-        return hash(self.id)
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.id == other.id
-        return NotImplemented
-
-    def __lt__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.id < other.id
-        return NotImplemented
-
     def __bool__(self) -> bool:
-        return self.id != type(self).id
+        return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Servant]:
-        from pymafia import ash
+        from pymafia.ash import from_java
 
         values = km.DataTypes.SERVANT_TYPE.allValues()
-        return sorted(ash.to_python(values))
+        return from_java(values)
 
     @property
     def servant(self) -> Any:
         return km.EdServantData.findEdServant(self.name)
 
     @property
     def level(self) -> int:
-        return 0 if self.servant is None else self.servant.getLevel()
+        return self.servant.getLevel() if self.servant is not None else 0
 
     @property
     def experience(self) -> int:
-        return 0 if self.servant is None else self.servant.getExperience()
+        return self.servant.getExperience() if self.servant is not None else 0
 
     @property
     def image(self) -> str:
-        return km.EdServantData.dataToImage(self.data) if self else ""
+        return km.EdServantData.dataToImage(self.data) if self.data is not None else ""
 
     @property
     def level1_ability(self) -> str:
-        return km.EdServantData.dataToLevel1Ability(self.data) if self else ""
+        return (
+            km.EdServantData.dataToLevel1Ability(self.data)
+            if self.data is not None
+            else ""
+        )
 
     @property
     def level7_ability(self) -> str:
-        return km.EdServantData.dataToLevel7Ability(self.data) if self else ""
+        return (
+            km.EdServantData.dataToLevel7Ability(self.data)
+            if self.data is not None
+            else ""
+        )
 
     @property
     def level14_ability(self) -> str:
-        return km.EdServantData.dataToLevel14Ability(self.data) if self else ""
+        return (
+            km.EdServantData.dataToLevel14Ability(self.data)
+            if self.data is not None
+            else ""
+        )
 
     @property
     def level21_ability(self) -> str:
-        return km.EdServantData.dataToLevel21Ability(self.data) if self else ""
+        return (
+            km.EdServantData.dataToLevel21Ability(self.data)
+            if self.data is not None
+            else ""
+        )
```

### Comparing `pymafia-0.1.9/src/pymafia/datatypes/skill.py` & `pymafia-0.2.0/src/pymafia/datatypes/skill.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,57 @@
 from __future__ import annotations
 
-from functools import total_ordering
-from typing import TYPE_CHECKING, Any
+from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
-    from .class_ import Class
+    from pymafia.datatypes.class_ import Class
 
 
-@total_ordering
+@dataclass(frozen=True, order=True)
 class Skill:
-    id: int = -1
-    name: str = "none"
+    id: int = km.DataTypes.SKILL_INIT.contentLong
+    name: str = km.DataTypes.SKILL_INIT.contentString
 
     def __init__(self, key: int | str | None = None):
-        if key.casefold() == self.name.casefold() or key in (self.id, None):
+        if (isinstance(key, str) and key.casefold() == self.name.casefold()) or key in (
+            self.id,
+            None,
+        ):
             return
 
-        # Deviate from the behavior of mafia's DataTypes.parseSkillValue
         id = km.SkillDatabase.getSkillId(key) if isinstance(key, str) else key
         name = km.SkillDatabase.getSkillName(id)
         if name is None:
             raise ValueError(f"{type(self).__name__} {key!r} not found")
 
-        self.id = id
-        self.name = name
+        object.__setattr__(self, "id", id)
+        object.__setattr__(self, "name", name)
 
     def __str__(self) -> str:
         ids = km.SkillDatabase.getSkillIds(self.name, False)
         return f"[{self.id}]{self.name}" if len(ids) > 1 else self.name
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({str(self)!r})"
 
-    def __hash__(self) -> int:
-        return hash(self.id)
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.id == other.id
-        return NotImplemented
-
-    def __lt__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.id < other.id
-        return NotImplemented
-
     def __bool__(self) -> bool:
-        return self.id != type(self).id
+        return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Skill]:
-        from pymafia import ash
+        from pymafia.ash import from_java
 
         values = km.DataTypes.SKILL_TYPE.allValues()
-        return sorted(ash.to_python(values))
+        return sorted(from_java(values))
 
     @property
-    def type_(self) -> str:
+    def type(self) -> str:
         return km.SkillDatabase.getSkillTypeName(self.id)
 
     @property
     def level(self) -> int:
         return km.SkillDatabase.getSkillLevel(self.id)
 
     @property
@@ -71,17 +60,20 @@
 
     @property
     def traincost(self) -> int:
         return km.SkillDatabase.getSkillPurchaseCost(self.id)
 
     @property
     def class_(self) -> Class:
-        from .class_ import Class
+        from pymafia.datatypes.class_ import Class
 
-        return Class(km.SkillDatabase.getSkillCategory(self.id) or None)
+        try:
+            return Class(km.SkillDatabase.getSkillCategory(self.id).name)
+        except ValueError:
+            return Class()
 
     @property
     def libram(self) -> bool:
         return km.SkillDatabase.isLibramSkill(self.id)
 
     @property
     def passive(self) -> bool:
```

### Comparing `pymafia-0.1.9/src/pymafia/datatypes/slot.py` & `pymafia-0.2.0/src/pymafia/datatypes/stat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,40 @@
 from __future__ import annotations
 
-from functools import total_ordering
-from typing import Any
+from dataclasses import dataclass
 
 from pymafia.kolmafia import km
 
 
-@total_ordering
-class Slot:
-    name: str = "none"
+@dataclass(frozen=True, order=True)
+class Stat:
+    name: str = km.DataTypes.STAT_INIT.contentString
 
     def __init__(self, key: str | None = None):
-        if key.casefold() == self.name.casefold() or key is None:
+        if (
+            isinstance(key, str) and key.casefold() == self.name.casefold()
+        ) or key is None:
             return
 
-        slot = km.EquipmentRequest.slotNumber(key)
-        if slot == km.Slot.NONE:
-            raise ValueError(f"{type(self).__name__} {key!r} not found")
+        for stat in km.DataTypes.STAT_VALUES:
+            name = stat.toString()
+            if name.casefold() == key.casefold():
+                object.__setattr__(self, "name", name)
+                return
 
-        self.name = slot.toString()
+        raise ValueError(f"{type(self).__name__} {key!r} not found")
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({str(self)!r})"
 
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.name == other.name
-        return NotImplemented
-
-    def __lt__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.name < other.name
-        return NotImplemented
-
     def __bool__(self) -> bool:
-        return self.name != type(self).name
+        return self != type(self)()
 
     @classmethod
-    def all(cls) -> list[Slot]:
-        from pymafia import ash
+    def all(cls) -> list[Stat]:
+        from pymafia.ash import from_java
 
-        values = km.DataTypes.SLOT_TYPE.allValues()
-        return sorted(ash.to_python(values))
+        values = km.DataTypes.STAT_TYPE.allValues()
+        return from_java(values)
```

### Comparing `pymafia-0.1.9/src/pymafia/datatypes/stat.py` & `pymafia-0.2.0/src/pymafia/ash/library.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,46 @@
-from __future__ import annotations
-
-from functools import total_ordering
 from typing import Any
 
-from pymafia.kolmafia import km
+from jpype import JClass
 
+from pymafia.ash.conversion import from_java, to_java
+from pymafia.kolmafia import km
 
-@total_ordering
-class Stat:
-    name: str = "none"
-
-    def __init__(self, key: str | None = None):
-        if key.casefold() == self.name.casefold() or key is None:
-            return
-
-        for stat in km.DataTypes.STAT_VALUES:
-            name = stat.toString()
-            if name.casefold() == key.casefold():
-                self.name = name
-                return
+String = JClass("java.lang.String")
+ByteArrayInputStream = JClass("java.io.ByteArrayInputStream")
 
-        raise ValueError(f"{type(self).__name__} {key!r} not found")
 
-    def __str__(self) -> str:
-        return self.name
+class LibraryFunction:
+    def __init__(self, name: str):
+        self.name = name
+        self.func = getattr(km.RuntimeLibrary, self.name)
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}({str(self)!r})"
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.name == other.name
-        return NotImplemented
-
-    def __lt__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return self.name < other.name
-        return NotImplemented
-
-    def __bool__(self) -> bool:
-        return self.name != type(self).name
-
-    @classmethod
-    def all(cls) -> list[Stat]:
-        from pymafia import ash
+        return f"{type(self).__name__}({self.name!r})"
 
-        values = km.DataTypes.STAT_TYPE.allValues()
-        return sorted(ash.to_python(values))
+    def __call__(self, *args, raw=False) -> Any:
+        interpreter = km.AshRuntime()
+        jargs = [to_java(arg) for arg in args]
+        value = self.func(interpreter, *jargs)
+        return value if raw else from_java(value)
+
+    @property
+    def signatures(self) -> list[str]:
+        functions = km.RuntimeLibrary.getFunctions().findFunctions(self.name)
+        return [f"{f.getType().toString()} {f.getSignature()}" for f in functions]
+
+
+def script(lines: str, raw=False) -> Any:
+    stream = ByteArrayInputStream(String(lines).getBytes())
+    interpreter = km.AshRuntime()
+    interpreter.validate(None, stream)
+    value = interpreter.execute("main", None)
+    return value if raw else from_java(value)
+
+
+def ashref(command="") -> list[str]:
+    names = set()
+    for func in km.RuntimeLibrary.getFunctions():
+        name = func.getName()
+        if command.casefold() in name.casefold():
+            names.add(name)
+    return sorted(names)
```

### Comparing `pymafia-0.1.9/src/pymafia/datatypes/vykea.py` & `pymafia-0.2.0/src/pymafia/datatypes/bounty.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,91 @@
 from __future__ import annotations
 
+from dataclasses import dataclass
 from enum import Enum
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING
 
 from pymafia.kolmafia import km
 
 if TYPE_CHECKING:
-    from .element import Element
-    from .item import Item
+    from pymafia.datatypes.location import Location
+    from pymafia.datatypes.monster import Monster
 
 
-class Vykea:
-    companion: Any = km.VYKEACompanionData.NO_COMPANION
+class BountyType(Enum):
+    NONE = None
+    EASY = "easy"
+    HARD = "hard"
+    SPECIAL = "special"
+
+
+class KoLInternalBountyType(Enum):
+    NONE = BountyType.NONE
+    LOW = BountyType.EASY
+    HIGH = BountyType.HARD
+    SPECIAL = BountyType.SPECIAL
+
+
+@dataclass(frozen=True, order=True)
+class Bounty:
+    name: str = km.DataTypes.BOUNTY_INIT.contentString
 
     def __init__(self, key: str | None = None):
-        if key.casefold() == "none".casefold() or key is None:
+        if (
+            isinstance(key, str) and key.casefold() == self.name.casefold()
+        ) or key is None:
             return
 
-        companion = km.VYKEACompanionData.fromString(key)
-        if companion is None:
+        bounties = km.BountyDatabase.getMatchingNames(key)
+        if len(bounties) != 1:
             raise ValueError(f"{type(self).__name__} {key!r} not found")
 
-        self.companion = companion
+        canonical = bounties[0]
+        object.__setattr__(self, "name", km.BountyDatabase.canonicalToName(canonical))
 
     def __str__(self) -> str:
-        return self.companion.toString()
+        return self.name
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({str(self)!r})"
 
-    def __hash__(self) -> int:
-        return hash((self.type_, self.rune, self.level))
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, type(self)):
-            return (
-                self.type_,
-                self.rune,
-                self.level,
-            ) == (other.type_, other.rune, other.level)
-        return NotImplemented
-
-    def __lt__(self, other: Any) -> bool:
-        raise NotImplementedError
-
     def __bool__(self) -> bool:
-        return self.companion != type(self).companion
+        return self != type(self)()
 
     @classmethod
-    def all(cls) -> list[Vykea]:
-        from pymafia import ash
+    def all(cls) -> list[Bounty]:
+        from pymafia.ash import from_java
 
-        values = km.DataTypes.VYKEA_TYPE.allValues()
-        return ash.to_python(values)
+        values = km.DataTypes.BOUNTY_TYPE.allValues()
+        return from_java(values)
 
     @property
-    def name(self) -> str:
-        return self.companion.getName()
+    def plural(self) -> str:
+        return km.BountyDatabase.getPlural(self.name) or ""
 
     @property
-    def type_(self) -> str:
-        return self.companion.getType()
+    def type(self) -> BountyType:
+        return BountyType(km.BountyDatabase.getType(self.name))
 
     @property
-    def rune(self) -> Item:
-        from .item import Item
-
-        return Item(self.companion.getRune().getItemId())
+    def kol_internal_type(self) -> KoLInternalBountyType:
+        return KoLInternalBountyType(self.type)
 
     @property
-    def level(self) -> int:
-        return self.companion.getLevel()
+    def number(self) -> int:
+        return km.BountyDatabase.getNumber(self.name)
 
     @property
     def image(self) -> str:
-        return self.companion.getImage()
+        return km.BountyDatabase.getImage(self.name) or ""
 
     @property
-    def modifiers(self) -> str:
-        return self.companion.getModifiers()
+    def monster(self) -> Monster:
+        from pymafia.datatypes.monster import Monster
+
+        return Monster(km.BountyDatabase.getMonster(self.name))
 
     @property
-    def attack_element(self) -> Element:
-        from .element import Element
+    def location(self) -> Location:
+        from pymafia.datatypes.location import Location
 
-        return Element(self.companion.getAttackElement().toString())
+        return Location(km.BountyDatabase.getLocation(self.name))
```

### Comparing `pymafia-0.1.9/src/pymafia/iotms/barrel_god.py` & `pymafia-0.2.0/src/pymafia/iotms/barrel_god.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/iotms/boxing_daycare.py` & `pymafia-0.2.0/src/pymafia/iotms/boxing_daycare.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/iotms/cartography.py` & `pymafia-0.2.0/src/pymafia/iotms/cartography.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/iotms/cosplay_saber.py` & `pymafia-0.2.0/src/pymafia/iotms/cosplay_saber.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/iotms/crimbo_shrub.py` & `pymafia-0.2.0/src/pymafia/iotms/crimbo_shrub.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/iotms/god_lobster.py` & `pymafia-0.2.0/src/pymafia/iotms/god_lobster.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/iotms/love_tunnel.py` & `pymafia-0.2.0/src/pymafia/iotms/love_tunnel.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/iotms/mumming_trunk.py` & `pymafia-0.2.0/src/pymafia/iotms/mumming_trunk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import re
 from enum import IntEnum
 from typing import List
 
 from pymafia import ash, player
 from pymafia.datatypes import Familiar, Item
 from pymafia.preference import get_property
```

### Comparing `pymafia-0.1.9/src/pymafia/iotms/pantogram.py` & `pymafia-0.2.0/src/pymafia/iotms/pantogram.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/iotms/protonic_pack.py` & `pymafia-0.2.0/src/pymafia/iotms/protonic_pack.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/iotms/snojo.py` & `pymafia-0.2.0/src/pymafia/iotms/snojo.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/iotms/songboom.py` & `pymafia-0.2.0/src/pymafia/iotms/songboom.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/iotms/stomping_boots.py` & `pymafia-0.2.0/src/pymafia/iotms/stomping_boots.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/iotms/witchess.py` & `pymafia-0.2.0/src/pymafia/iotms/witchess.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/player.py` & `pymafia-0.2.0/src/pymafia/player.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/preference.py` & `pymafia-0.2.0/src/pymafia/preference.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/src/pymafia/utils.py` & `pymafia-0.2.0/src/pymafia/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from html import escape
 
+from jpype import JClass
+
 from pymafia.kolmafia import km
 
+ByteArrayOutputStream = JClass("java.io.ByteArrayOutputStream")
+PrintStream = JClass("java.io.PrintStream")
+OutputStream = JClass("java.io.OutputStream")
+
 
 def launch_gui():
     """Launch the KoLmafia GUI."""
     km.KoLmafia.main(["--GUI"])
 
 
 def login(username: str, password: str | None = None) -> bool:
@@ -16,30 +22,26 @@
     request = km.LoginRequest(username, password)
     request.run()
     return request
 
 
 def abort(message: str = ""):
     """Immediately halt KoLmafia."""
-    MafiaState = getattr(km, "KoLConstants$MafiaState")
-    km.KoLmafia.updateDisplay(MafiaState.ABORT, message)
+    km.KoLmafia.updateDisplay(km.KoLConstants.MafiaState.ABORT, message)
 
 
 def log(message: str, html: bool = False):
     """Log a message in the KoLmafia CLI."""
     message = str(message)
     if not html:
         message = escape(message)
 
     km.RequestLogger.printLine(message)
 
 
 def execute(command: str) -> str:
     """Execute a command in the KoLmafia CLI and return the output."""
-    ByteArrayOutputStream = km.autoclass("java.io.ByteArrayOutputStream")
-    PrintStream = km.autoclass("java.io.PrintStream")
-
-    ostream = km.cast("java.io.OutputStream", ByteArrayOutputStream())
+    ostream = OutputStream @ ByteArrayOutputStream()
     out = PrintStream(ostream)
     km.RequestLogger.openCustom(out)
     km.KoLmafiaCLI.DEFAULT_SHELL.executeLine(command)
     return ostream.toString()
```

### Comparing `pymafia-0.1.9/src/pymafia/wanderer.py` & `pymafia-0.2.0/src/pymafia/wanderer.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.1.9/PKG-INFO` & `pymafia-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pymafia
-Version: 0.1.9
-Summary: A Python module and bridge for reflecting KoLmafia's Java environment.
+Version: 0.2.0
+Summary: A Python module and bridge for reflecting KoLmafia's Java environment
 Home-page: https://github.com/MrFizzyBubbs/pymafia
 License: MIT
 Author: MrFizzyBubbs
 Author-email: MrFizzyBubbs@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pyjnius (>=1.4.2,<2.0.0)
+Requires-Dist: JPype1 (>=1.4.1,<2.0.0)
+Requires-Dist: wrapt (>=1.15.0,<2.0.0)
 Project-URL: Repository, https://github.com/MrFizzyBubbs/pymafia
 Description-Content-Type: text/markdown
 
 # pymafia
 
 A Python module and bridge for reflecting KoLmafia's Java environment.
```

