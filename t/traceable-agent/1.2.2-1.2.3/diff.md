# Comparing `tmp/traceable-agent-1.2.2.tar.gz` & `tmp/traceable-agent-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceable-agent-1.2.2.tar", last modified: Wed Jan 18 16:17:50 2023, max compression
+gzip compressed data, was "traceable-agent-1.2.3.tar", last modified: Fri Apr 21 19:04:25 2023, max compression
```

## Comparing `traceable-agent-1.2.2.tar` & `traceable-agent-1.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 16:17:50.078950 traceable-agent-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-01-18 16:17:50.078950 traceable-agent-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2570 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-01-18 16:17:50.078950 traceable-agent-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1223 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 16:17:50.078950 traceable-agent-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 16:17:50.078950 traceable-agent-1.2.2/src/traceable_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-01-18 16:17:50.000000 traceable-agent-1.2.2/src/traceable_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-01-18 16:17:50.000000 traceable-agent-1.2.2/src/traceable_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-18 16:17:50.000000 traceable-agent-1.2.2/src/traceable_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-01-18 16:17:50.000000 traceable-agent-1.2.2/src/traceable_agent.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-01-18 16:17:50.000000 traceable-agent-1.2.2/src/traceable_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-18 16:17:50.000000 traceable-agent-1.2.2/src/traceable_agent.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 16:17:50.078950 traceable-agent-1.2.2/src/traceableai/
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/src/traceableai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3248 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/src/traceableai/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 16:17:50.078950 traceable-agent-1.2.2/src/traceableai/autoinstrumentation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/src/traceableai/autoinstrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/src/traceableai/autoinstrumentation/sitecustomize.py
--rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/src/traceableai/autoinstrumentation/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 16:17:50.078950 traceable-agent-1.2.2/src/traceableai/config/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/src/traceableai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/src/traceableai/config/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      570 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/src/traceableai/config/default.py
--rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/src/traceableai/config/environment.py
--rw-r--r--   0 runner    (1001) docker     (122)    18027 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/src/traceableai/config/traceable_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     7515 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/src/traceableai/config_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-18 16:17:50.078950 traceable-agent-1.2.2/src/traceableai/filter/
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/src/traceableai/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9643 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/src/traceableai/filter/traceable.py
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-01-18 16:09:49.000000 traceable-agent-1.2.2/src/traceableai/hypertrace_env_override.py
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-01-18 16:09:50.000000 traceable-agent-1.2.2/src/traceableai/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 19:04:25.914281 traceable-agent-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-04-21 19:04:25.914281 traceable-agent-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2570 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-04-21 19:04:25.914281 traceable-agent-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1223 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 19:04:25.906281 traceable-agent-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 19:04:25.910282 traceable-agent-1.2.3/src/traceable_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-04-21 19:04:25.000000 traceable-agent-1.2.3/src/traceable_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-04-21 19:04:25.000000 traceable-agent-1.2.3/src/traceable_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 19:04:25.000000 traceable-agent-1.2.3/src/traceable_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-04-21 19:04:25.000000 traceable-agent-1.2.3/src/traceable_agent.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-04-21 19:04:25.000000 traceable-agent-1.2.3/src/traceable_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-21 19:04:25.000000 traceable-agent-1.2.3/src/traceable_agent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 19:04:25.910282 traceable-agent-1.2.3/src/traceableai/
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/src/traceableai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3248 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/src/traceableai/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 19:04:25.910282 traceable-agent-1.2.3/src/traceableai/autoinstrumentation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/src/traceableai/autoinstrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/src/traceableai/autoinstrumentation/sitecustomize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/src/traceableai/autoinstrumentation/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 19:04:25.910282 traceable-agent-1.2.3/src/traceableai/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/src/traceableai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/src/traceableai/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/src/traceableai/config/default.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/src/traceableai/config/environment.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18027 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/src/traceableai/config/traceable_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7515 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/src/traceableai/config_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 19:04:25.914281 traceable-agent-1.2.3/src/traceableai/filter/
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/src/traceableai/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9643 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/src/traceableai/filter/traceable.py
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-04-21 18:54:23.000000 traceable-agent-1.2.3/src/traceableai/hypertrace_env_override.py
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-21 18:54:24.000000 traceable-agent-1.2.3/src/traceableai/version.py
```

### Comparing `traceable-agent-1.2.2/PKG-INFO` & `traceable-agent-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceable-agent
-Version: 1.2.2
+Version: 1.2.3
 Summary: Traceable.ai Python Agent
 Home-page: https://traceable.ai
 Author: Traceable.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `traceable-agent-1.2.2/README.md` & `traceable-agent-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `traceable-agent-1.2.2/setup.py` & `traceable-agent-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         Extension(
             name='traceableai.filter._libtraceable',
             sources=[],
             optional=os.environ.get('CIBUILDWHEEL', '0') != '1'
         )
     ],
     install_requires=[
-        "hypertrace-agent==0.14.0",
+        "hypertrace-agent==0.14.1",
         "psutil",
         "distro==1.6.0",
         "cffi",
     ],
     entry_points={
         'console_scripts': [
             'traceableai-instrument = traceableai.autoinstrumentation.wrapper:run',
```

### Comparing `traceable-agent-1.2.2/src/traceable_agent.egg-info/PKG-INFO` & `traceable-agent-1.2.3/src/traceable_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceable-agent
-Version: 1.2.2
+Version: 1.2.3
 Summary: Traceable.ai Python Agent
 Home-page: https://traceable.ai
 Author: Traceable.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `traceable-agent-1.2.2/src/traceable_agent.egg-info/SOURCES.txt` & `traceable-agent-1.2.3/src/traceable_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `traceable-agent-1.2.2/src/traceableai/agent.py` & `traceable-agent-1.2.3/src/traceableai/agent.py`

 * *Files identical despite different names*

### Comparing `traceable-agent-1.2.2/src/traceableai/autoinstrumentation/sitecustomize.py` & `traceable-agent-1.2.3/src/traceableai/autoinstrumentation/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `traceable-agent-1.2.2/src/traceableai/autoinstrumentation/wrapper.py` & `traceable-agent-1.2.3/src/traceableai/autoinstrumentation/wrapper.py`

 * *Files identical despite different names*

### Comparing `traceable-agent-1.2.2/src/traceableai/config/config.py` & `traceable-agent-1.2.3/src/traceableai/config/config.py`

 * *Files identical despite different names*

### Comparing `traceable-agent-1.2.2/src/traceableai/config/default.py` & `traceable-agent-1.2.3/src/traceableai/config/default.py`

 * *Files identical despite different names*

### Comparing `traceable-agent-1.2.2/src/traceableai/config/environment.py` & `traceable-agent-1.2.3/src/traceableai/config/environment.py`

 * *Files identical despite different names*

### Comparing `traceable-agent-1.2.2/src/traceableai/config/traceable_config_pb2.py` & `traceable-agent-1.2.3/src/traceableai/config/traceable_config_pb2.py`

 * *Files identical despite different names*

### Comparing `traceable-agent-1.2.2/src/traceableai/config_wrapper.py` & `traceable-agent-1.2.3/src/traceableai/config_wrapper.py`

 * *Files identical despite different names*

### Comparing `traceable-agent-1.2.2/src/traceableai/filter/__init__.py` & `traceable-agent-1.2.3/src/traceableai/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `traceable-agent-1.2.2/src/traceableai/filter/traceable.py` & `traceable-agent-1.2.3/src/traceableai/filter/traceable.py`

 * *Files identical despite different names*

### Comparing `traceable-agent-1.2.2/src/traceableai/hypertrace_env_override.py` & `traceable-agent-1.2.3/src/traceableai/hypertrace_env_override.py`

 * *Files identical despite different names*

