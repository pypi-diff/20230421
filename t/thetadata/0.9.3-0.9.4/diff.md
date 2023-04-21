# Comparing `tmp/thetadata-0.9.3.tar.gz` & `tmp/thetadata-0.9.4.tar.gz`

## Comparing `thetadata-0.9.3.tar` & `thetadata-0.9.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 thetadata-0.9.3/mkdocs.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 thetadata-0.9.3/setup.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 thetadata-0.9.3/.github/workflows/main.yml
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thetadata-0.9.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/__init__.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/connection_msgs.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/explanation.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/how-to-guides.md
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/index.md
--rw-r--r--   0        0        0    51619 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/logo.png
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/manipulate_df.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/manipulate_series.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/reference.md
--rw-r--r--   0        0        0    27736 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/tutorials.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/options/__init__.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/options/cancel_streams.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/options/eod.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/options/get_last.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/options/list_roots.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/options/open_interest_streaming.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/options/quote_1min.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/options/quote_tick.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/options/trade_streaming.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/options/trade_streaming_full.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/stocks/__init__.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/stocks/eod.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/stocks/get_last.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/stocks/list_roots.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/stocks/quote_1min.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 thetadata-0.9.3/docs/stocks/quote_tick.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 thetadata-0.9.3/tests/__init__.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 thetadata-0.9.3/tests/test_client.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 thetadata-0.9.3/tests/test_docs.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 thetadata-0.9.3/thetadata/__init__.py
--rw-r--r--   0        0        0    58526 2020-02-02 00:00:00.000000 thetadata-0.9.3/thetadata/client.py
--rw-r--r--   0        0        0    20277 2020-02-02 00:00:00.000000 thetadata-0.9.3/thetadata/enums.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 thetadata-0.9.3/thetadata/exceptions.py
--rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 thetadata-0.9.3/thetadata/parsing.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thetadata-0.9.3/thetadata/py.typed
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 thetadata-0.9.3/thetadata/terminal.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 thetadata-0.9.3/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 thetadata-0.9.3/LICENSE
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 thetadata-0.9.3/README.md
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 thetadata-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 thetadata-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 thetadata-0.9.4/mkdocs.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 thetadata-0.9.4/setup.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 thetadata-0.9.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thetadata-0.9.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/__init__.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/connection_msgs.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/explanation.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/how-to-guides.md
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/index.md
+-rw-r--r--   0        0        0    51619 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/logo.png
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/manipulate_df.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/manipulate_series.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/reference.md
+-rw-r--r--   0        0        0    27736 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/tutorials.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/options/__init__.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/options/cancel_streams.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/options/eod.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/options/get_last.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/options/list_roots.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/options/open_interest_streaming.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/options/quote_1min.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/options/quote_tick.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/options/trade_streaming.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/options/trade_streaming_full.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/stocks/__init__.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/stocks/eod.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/stocks/get_last.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/stocks/list_roots.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/stocks/quote_1min.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 thetadata-0.9.4/docs/stocks/quote_tick.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 thetadata-0.9.4/tests/__init__.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 thetadata-0.9.4/tests/test_client.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 thetadata-0.9.4/tests/test_docs.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 thetadata-0.9.4/thetadata/__init__.py
+-rw-r--r--   0        0        0    58526 2020-02-02 00:00:00.000000 thetadata-0.9.4/thetadata/client.py
+-rw-r--r--   0        0        0    20277 2020-02-02 00:00:00.000000 thetadata-0.9.4/thetadata/enums.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 thetadata-0.9.4/thetadata/exceptions.py
+-rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 thetadata-0.9.4/thetadata/parsing.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thetadata-0.9.4/thetadata/py.typed
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 thetadata-0.9.4/thetadata/terminal.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 thetadata-0.9.4/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 thetadata-0.9.4/LICENSE
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 thetadata-0.9.4/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 thetadata-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 thetadata-0.9.4/PKG-INFO
```

### Comparing `thetadata-0.9.3/mkdocs.yml` & `thetadata-0.9.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/.github/workflows/main.yml` & `thetadata-0.9.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/.github/workflows/python-publish.yml` & `thetadata-0.9.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/connection_msgs.py` & `thetadata-0.9.4/docs/connection_msgs.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/explanation.md` & `thetadata-0.9.4/docs/explanation.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/how-to-guides.md` & `thetadata-0.9.4/docs/how-to-guides.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/index.md` & `thetadata-0.9.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/logo.png` & `thetadata-0.9.4/docs/logo.png`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/manipulate_series.py` & `thetadata-0.9.4/docs/manipulate_series.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/tutorials.md` & `thetadata-0.9.4/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/options/cancel_streams.py` & `thetadata-0.9.4/docs/options/cancel_streams.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/options/eod.py` & `thetadata-0.9.4/docs/options/eod.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/options/get_last.py` & `thetadata-0.9.4/docs/options/get_last.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/options/open_interest_streaming.py` & `thetadata-0.9.4/docs/options/open_interest_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/options/quote_1min.py` & `thetadata-0.9.4/docs/options/quote_1min.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/options/quote_tick.py` & `thetadata-0.9.4/docs/options/quote_tick.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/options/trade_streaming.py` & `thetadata-0.9.4/docs/options/trade_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/options/trade_streaming_full.py` & `thetadata-0.9.4/docs/options/trade_streaming_full.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/stocks/eod.py` & `thetadata-0.9.4/docs/stocks/eod.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/stocks/get_last.py` & `thetadata-0.9.4/docs/stocks/get_last.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/stocks/quote_1min.py` & `thetadata-0.9.4/docs/stocks/quote_1min.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/docs/stocks/quote_tick.py` & `thetadata-0.9.4/docs/stocks/quote_tick.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/tests/test_client.py` & `thetadata-0.9.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/tests/test_docs.py` & `thetadata-0.9.4/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/thetadata/client.py` & `thetadata-0.9.4/thetadata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     TickBody,
     ListBody,
     parse_list_REST, parse_flexible_REST, parse_hist_REST, parse_hist_REST_stream, parse_hist_REST_stream_ijson,
 )
 from .terminal import check_download, launch_terminal
 
 _NOT_CONNECTED_MSG = "You must establish a connection first."
-_VERSION = '0.9.3'
+_VERSION = '0.9.4'
 URL_BASE = "http://127.0.0.1:25510/"
 
 
 def _format_strike(strike: float) -> int:
     """Round USD to the nearest tenth of a cent, acceptable by the terminal."""
     return round(strike * 1000)
```

### Comparing `thetadata-0.9.3/thetadata/enums.py` & `thetadata-0.9.4/thetadata/enums.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/thetadata/exceptions.py` & `thetadata-0.9.4/thetadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/thetadata/parsing.py` & `thetadata-0.9.4/thetadata/parsing.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/thetadata/terminal.py` & `thetadata-0.9.4/thetadata/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                                        stdout=subprocess.PIPE, shell=True, cwd=cwd)
     for line in process.stdout:
         print(line.decode('utf-8').rstrip("\n"))
 
 
 def check_download(auto_update: bool, stable: bool) -> bool:
     if stable:
-        link = 'https://download-latest.thetadata.us'
+        link = 'https://download-stable.thetadata.us'
     else:
         link = 'https://download-unstable.thetadata.us'
     try:
         if not os.path.exists('ThetaTerminal.jar') or auto_update:
             jar = urllib.request.urlopen(link)
             with open('ThetaTerminal.jar', 'wb') as output:
                 output.write(jar.read())
```

### Comparing `thetadata-0.9.3/LICENSE` & `thetadata-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/README.md` & `thetadata-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.3/pyproject.toml` & `thetadata-0.9.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thetadata"
-version = "0.9.3"
+version = "0.9.4"
 authors = [
   { name="Bailey Danseglio", email="bailey@thetadata.net" },
   { name="Adler Weber", email="redacted@thetadata.net" },
 ]
 description = "Python API for Thetadata"
 readme = "README.md"
 license = { file="LICENSE" }
@@ -20,14 +20,15 @@
 ]
 dependencies = [
   "tqdm",
   "pandas",
   "wget",
   "psutil",
   "ijson",
+  "requests",
 ]
 
 [project.optional-dependencies]
 tests = [
   "coverage>=5.0.3",
   "pytest",
   "pytest-benchmark[histogram]>=3.2.1",
```

### Comparing `thetadata-0.9.3/PKG-INFO` & `thetadata-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thetadata
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python API for Thetadata
 Project-URL: Homepage, https://thetadata.net
 Project-URL: Source, https://thetadata-api.github.io/thetadata-python/reference/
 Project-URL: Bug Tracker, https://github.com/ThetaData-API/thetadata-python/issues
 Project-URL: Documentation, https://thetadata-api.github.io/thetadata-python/
 Author-email: Bailey Danseglio <bailey@thetadata.net>, Adler Weber <redacted@thetadata.net>
 License: MIT License
@@ -32,14 +32,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: ijson
 Requires-Dist: pandas
 Requires-Dist: psutil
+Requires-Dist: requests
 Requires-Dist: tqdm
 Requires-Dist: wget
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings[python]; extra == 'docs'
 Provides-Extra: tests
```

