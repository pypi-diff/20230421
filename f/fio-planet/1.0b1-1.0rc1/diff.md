# Comparing `tmp/fio_planet-1.0b1.tar.gz` & `tmp/fio_planet-1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fio_planet-1.0b1.tar", last modified: Thu Apr 13 20:04:26 2023, max compression
+gzip compressed data, was "fio_planet-1.0rc1.tar", last modified: Wed Apr 19 02:00:51 2023, max compression
```

## Comparing `fio_planet-1.0b1.tar` & `fio_planet-1.0rc1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      164 2023-03-30 20:10:41.857799 fio_planet-1.0b1/.readthedocs.yml
--rw-r--r--   0        0        0      809 2023-04-13 19:55:49.739453 fio_planet-1.0b1/CHANGES
--rw-r--r--   0        0        0     1986 2023-03-30 20:10:41.857799 fio_planet-1.0b1/CODE_OF_CONDUCT
--rw-r--r--   0        0        0    11357 2023-03-30 20:10:41.857799 fio_planet-1.0b1/LICENSE
--rw-r--r--   0        0        0     4507 2023-04-13 19:52:55.913276 fio_planet-1.0b1/README.md
--rw-r--r--   0        0        0     1428 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/commands.md
--rw-r--r--   0        0        0     1379 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/custom_theme/main.html
--rw-r--r--   0        0        0     4827 2023-04-13 19:52:55.913276 fio_planet-1.0b1/docs/expressions.md
--rw-r--r--   0        0        0     7116 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/images/Planet_primarymark_RGB_White.png
--rw-r--r--   0        0        0    36552 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/images/SatelliteOrbits-main100Dove4RapidEye6Skysat-100mm01-pulsing.svg
--rw-r--r--   0        0        0      655 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/images/logo.svg
--rw-r--r--   0        0        0     3955 2023-04-13 19:53:16.401533 fio_planet-1.0b1/docs/index.md
--rw-r--r--   0        0        0      169 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/requirements.txt
--rw-r--r--   0        0        0     2091 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/stylesheets/extra.css
--rw-r--r--   0        0        0       72 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/topics/index.md
--rw-r--r--   0        0        0     4010 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/topics/simplification.md
--rw-r--r--   0        0        0     1795 2023-04-13 19:52:55.913276 fio_planet-1.0b1/mkdocs.yml
--rw-r--r--   0        0        0     1107 2023-04-13 19:52:55.913276 fio_planet-1.0b1/pyproject.toml
--rw-r--r--   0        0        0      722 2023-04-13 19:53:56.058030 fio_planet-1.0b1/src/fio_planet/__init__.py
--rw-r--r--   0        0        0     7860 2023-04-12 20:23:10.271883 fio_planet-1.0b1/src/fio_planet/cli.py
--rw-r--r--   0        0        0      215 2023-03-30 20:10:41.857799 fio_planet-1.0b1/src/fio_planet/errors.py
--rw-r--r--   0        0        0     9132 2023-04-12 20:23:10.271883 fio_planet-1.0b1/src/fio_planet/features.py
--rw-r--r--   0        0        0     8341 2023-03-30 20:10:41.857799 fio_planet-1.0b1/src/fio_planet/snuggs.py
--rw-r--r--   0        0        0    12885 2023-03-30 20:10:41.857799 fio_planet-1.0b1/tests/data/rmnp.geojson
--rw-r--r--   0        0        0     1555 2023-03-30 20:10:41.857799 fio_planet-1.0b1/tests/data/trio.geojson
--rw-r--r--   0        0        0      805 2023-03-30 20:10:41.857799 fio_planet-1.0b1/tests/data/trio.seq
--rw-r--r--   0        0        0     3370 2023-03-30 20:10:41.857799 fio_planet-1.0b1/tests/test_cli.py
--rw-r--r--   0        0        0    10638 2023-03-30 20:10:41.857799 fio_planet-1.0b1/tests/test_mod.py
--rw-r--r--   0        0        0      436 2023-03-30 20:10:41.857799 fio_planet-1.0b1/tox.ini
--rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 fio_planet-1.0b1/PKG-INFO
+-rw-r--r--   0        0        0      164 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/.readthedocs.yml
+-rw-r--r--   0        0        0      972 2023-04-19 01:46:14.819848 fio_planet-1.0rc1/CHANGES
+-rw-r--r--   0        0        0     1986 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/CODE_OF_CONDUCT
+-rw-r--r--   0        0        0    11357 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/LICENSE
+-rw-r--r--   0        0        0     4507 2023-04-18 20:16:26.730938 fio_planet-1.0rc1/README.md
+-rw-r--r--   0        0        0     1428 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/docs/commands.md
+-rw-r--r--   0        0        0     1379 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/docs/custom_theme/main.html
+-rw-r--r--   0        0        0     4831 2023-04-18 20:16:26.730938 fio_planet-1.0rc1/docs/expressions.md
+-rw-r--r--   0        0        0     7116 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/docs/images/Planet_primarymark_RGB_White.png
+-rw-r--r--   0        0        0    36552 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/docs/images/SatelliteOrbits-main100Dove4RapidEye6Skysat-100mm01-pulsing.svg
+-rw-r--r--   0        0        0      655 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/docs/images/logo.svg
+-rw-r--r--   0        0        0     3955 2023-04-13 19:53:16.401533 fio_planet-1.0rc1/docs/index.md
+-rw-r--r--   0        0        0      169 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/docs/requirements.txt
+-rw-r--r--   0        0        0     2091 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0       72 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/docs/topics/index.md
+-rw-r--r--   0        0        0     4010 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/docs/topics/simplification.md
+-rw-r--r--   0        0        0     1795 2023-04-18 20:16:26.730938 fio_planet-1.0rc1/mkdocs.yml
+-rw-r--r--   0        0        0     1107 2023-04-18 20:16:26.730938 fio_planet-1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      723 2023-04-19 01:47:11.404388 fio_planet-1.0rc1/src/fio_planet/__init__.py
+-rw-r--r--   0        0        0     7860 2023-04-18 20:16:26.730938 fio_planet-1.0rc1/src/fio_planet/cli.py
+-rw-r--r--   0        0        0      215 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/src/fio_planet/errors.py
+-rw-r--r--   0        0        0     9162 2023-04-18 23:18:25.822402 fio_planet-1.0rc1/src/fio_planet/features.py
+-rw-r--r--   0        0        0     8402 2023-04-19 01:46:41.008097 fio_planet-1.0rc1/src/fio_planet/snuggs.py
+-rw-r--r--   0        0        0    12885 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/tests/data/rmnp.geojson
+-rw-r--r--   0        0        0     1555 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/tests/data/trio.geojson
+-rw-r--r--   0        0        0      805 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/tests/data/trio.seq
+-rw-r--r--   0        0        0     3370 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/tests/test_cli.py
+-rw-r--r--   0        0        0    10638 2023-03-30 20:10:41.857799 fio_planet-1.0rc1/tests/test_mod.py
+-rw-r--r--   0        0        0     1165 2023-04-19 01:51:49.679167 fio_planet-1.0rc1/tests/test_snuggs.py
+-rw-r--r--   0        0        0      436 2023-04-19 01:14:06.650769 fio_planet-1.0rc1/tox.ini
+-rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 fio_planet-1.0rc1/PKG-INFO
```

### Comparing `fio_planet-1.0b1/CHANGES` & `fio_planet-1.0rc1/CHANGES`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changes
 =======
 
-1.0b1 (2023-04-18)
+1.0rc1 (2023-04-18)
+------------------
+
+- The truth, is, and not functions from operators have been added to
+  the mapping of functions available in expressions.
+
+1.0b1 (2023-04-13)
 ------------------
 
 - Require pyparsing >= 3.0 (#29).
 - Added a documentation site hosted on Read the Docs (#26, #28, #32).
 
 1.0a3 (2023-03-24)
 ------------------
```

### Comparing `fio_planet-1.0b1/CODE_OF_CONDUCT` & `fio_planet-1.0rc1/CODE_OF_CONDUCT`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/LICENSE` & `fio_planet-1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/README.md` & `fio_planet-1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/docs/commands.md` & `fio_planet-1.0rc1/docs/commands.md`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/docs/custom_theme/main.html` & `fio_planet-1.0rc1/docs/custom_theme/main.html`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/docs/expressions.md` & `fio_planet-1.0rc1/docs/expressions.md`

 * *Files 5% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 ```python
 >>> snuggs.eval('(distance (Point 0 0) (Point 0.1 0.1))')
 15995.164946207413
 ```
 
 A geometry can be simplified to a tolerance value in meters using `simplify`.
 There are more examples of this function under
-[topics:simplication](topcs/simplification).
+[topics:simplification](topics/simplification/).
 
 ```python
 >>> snuggs.eval('(simplify (buffer (Point 0 0) :distance 100) :tolerance 100)')
 <POLYGON ((0.001 0, 0 -0.001, -0.001 0, 0 0.001, 0.001 0))>
 ```
 
 The `set_precision` function snaps a geometry to a fixed precision grid with a
```

### Comparing `fio_planet-1.0b1/docs/images/Planet_primarymark_RGB_White.png` & `fio_planet-1.0rc1/docs/images/Planet_primarymark_RGB_White.png`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/docs/images/SatelliteOrbits-main100Dove4RapidEye6Skysat-100mm01-pulsing.svg` & `fio_planet-1.0rc1/docs/images/SatelliteOrbits-main100Dove4RapidEye6Skysat-100mm01-pulsing.svg`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/docs/images/logo.svg` & `fio_planet-1.0rc1/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/docs/index.md` & `fio_planet-1.0rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/docs/stylesheets/extra.css` & `fio_planet-1.0rc1/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/docs/topics/simplification.md` & `fio_planet-1.0rc1/docs/topics/simplification.md`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/mkdocs.yml` & `fio_planet-1.0rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/pyproject.toml` & `fio_planet-1.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/src/fio_planet/__init__.py` & `fio_planet-1.0rc1/src/fio_planet/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """fio_planet: Fiona CLI plugins from Planet Labs."""
 
-__version__ = "1.0b1"
+__version__ = "1.0rc1"
```

### Comparing `fio_planet-1.0b1/src/fio_planet/cli.py` & `fio_planet-1.0rc1/src/fio_planet/cli.py`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/src/fio_planet/features.py` & `fio_planet-1.0rc1/src/fio_planet/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,17 @@
         if key in self.data:
             return self.data[key]
         elif key in __builtins__ and not key.startswith("__"):
             return __builtins__[key]
         elif key in dir(shapely):
             return lambda g, *args, **kwargs: getattr(shapely, key)(g, *args, **kwargs)
         elif key in dir(shapely.ops):
-            return lambda g, *args, **kwargs: getattr(shapely.ops, key)(g, *args, **kwargs)
+            return lambda g, *args, **kwargs: getattr(shapely.ops, key)(
+                g, *args, **kwargs
+            )
         else:
             return (
                 lambda g, *args, **kwargs: getattr(g, key)(*args, **kwargs)
                 if callable(getattr(g, key))
                 else getattr(g, key)
             )
```

### Comparing `fio_planet-1.0b1/src/fio_planet/snuggs.py` & `fio_planet-1.0rc1/src/fio_planet/snuggs.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     Group,
     OneOrMore,
     ParseResults,
     Regex,
     ZeroOrMore,
     alphanums,
     pyparsing_common,
+    replace_with,
 )
 
 __all__ = ["eval"]
 __version__ = "1.4.7"
 
 
 class Context(object):
@@ -121,14 +122,17 @@
     "|": lambda *args: functools.reduce(lambda x, y: operator.or_(x, y), args),
     "<": operator.lt,
     "<=": operator.le,
     "==": operator.eq,
     "!=": operator.ne,
     ">=": operator.ge,
     ">": operator.gt,
+    "truth": operator.truth,
+    "is": operator.is_,
+    "not": operator.not_,
 }
 
 
 def compose(f, g):
     """Compose two functions.
 
     compose(f, g)(x) = f(g(x)).
@@ -145,17 +149,17 @@
     "partial": functools.partial,
     "reduce": functools.reduce,
     "attrgetter": operator.attrgetter,
     "methodcaller": operator.methodcaller,
     "itemgetter": operator.itemgetter,
 }
 
-nil = Keyword("null").set_parse_action(lambda source, loc, toks: None)
-true = Keyword("true").set_parse_action(lambda source, loc, toks: True)
-false = Keyword("false").set_parse_action(lambda source, loc, toks: False)
+nil = Keyword("null").set_parse_action(replace_with(None))
+true = Keyword("true").set_parse_action(replace_with(True))
+false = Keyword("false").set_parse_action(replace_with(False))
 
 
 def resolve_var(source, loc, toks):
     try:
         return _ctx.get(toks[0])
     except KeyError:
         err = ExpressionError("name '{}' is not defined".format(toks[0]))
```

### Comparing `fio_planet-1.0b1/tests/data/rmnp.geojson` & `fio_planet-1.0rc1/tests/data/rmnp.geojson`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/tests/data/trio.geojson` & `fio_planet-1.0rc1/tests/data/trio.geojson`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/tests/data/trio.seq` & `fio_planet-1.0rc1/tests/data/trio.seq`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/tests/test_cli.py` & `fio_planet-1.0rc1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/tests/test_mod.py` & `fio_planet-1.0rc1/tests/test_mod.py`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0b1/PKG-INFO` & `fio_planet-1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fio_planet
-Version: 1.0b1
+Version: 1.0rc1
 Summary: fio_planet: Fiona CLI plugins from Planet Labs.
 Keywords: GeoJSON,GIS,CLI
 Author: Sean Gillies
 Maintainer-email: Planet Developer Relations <developers@planet.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
```

