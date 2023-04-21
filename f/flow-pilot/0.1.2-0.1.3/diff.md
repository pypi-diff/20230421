# Comparing `tmp/flow_pilot-0.1.2.tar.gz` & `tmp/flow_pilot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow_pilot-0.1.2.tar", last modified: Fri Apr 21 14:26:38 2023, max compression
+gzip compressed data, was "flow_pilot-0.1.3.tar", last modified: Fri Apr 21 14:31:36 2023, max compression
```

## Comparing `flow_pilot-0.1.2.tar` & `flow_pilot-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:26:38.367793 flow_pilot-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-04-21 14:26:38.358794 flow_pilot-0.1.2/FlowPilot/
--rw-rw-rw-   0        0        0       34 2023-04-21 10:55:09.000000 flow_pilot-0.1.2/FlowPilot/__init__.py
--rw-rw-rw-   0        0        0     5684 2023-04-21 14:25:05.000000 flow_pilot-0.1.2/FlowPilot/flow_pilot.py
--rw-rw-rw-   0        0        0      127 2023-04-21 14:26:23.000000 flow_pilot-0.1.2/FlowPilot/setup.py
--rw-rw-rw-   0        0        0     1087 2023-04-21 09:45:08.000000 flow_pilot-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       80 2023-04-21 14:26:38.367793 flow_pilot-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3487 2023-04-21 14:07:55.000000 flow_pilot-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 14:26:38.365813 flow_pilot-0.1.2/flow_pilot.egg-info/
-drwxrwxrwx   0        0        0        0 2023-04-21 14:26:38.366824 flow_pilot-0.1.2/flow_pilot.egg-info/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0      162 2023-04-21 09:51:44.000000 flow_pilot-0.1.2/flow_pilot.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-rw-rw-   0        0        0       80 2023-04-21 14:26:38.000000 flow_pilot-0.1.2/flow_pilot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-21 14:26:38.000000 flow_pilot-0.1.2/flow_pilot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:26:38.000000 flow_pilot-0.1.2/flow_pilot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 14:26:38.000000 flow_pilot-0.1.2/flow_pilot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 14:26:38.367793 flow_pilot-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 14:26:38.366824 flow_pilot-0.1.2/tests/
--rw-rw-rw-   0        0        0     3010 2023-04-21 14:07:39.000000 flow_pilot-0.1.2/tests/test_flowpilot.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:31:36.951546 flow_pilot-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-04-21 14:31:36.937477 flow_pilot-0.1.3/FlowPilot/
+-rw-rw-rw-   0        0        0       34 2023-04-21 10:55:09.000000 flow_pilot-0.1.3/FlowPilot/__init__.py
+-rw-rw-rw-   0        0        0     5936 2023-04-21 14:31:02.000000 flow_pilot-0.1.3/FlowPilot/flow_pilot.py
+-rw-rw-rw-   0        0        0      127 2023-04-21 14:31:06.000000 flow_pilot-0.1.3/FlowPilot/setup.py
+-rw-rw-rw-   0        0        0     1087 2023-04-21 09:45:08.000000 flow_pilot-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       80 2023-04-21 14:31:36.950545 flow_pilot-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3487 2023-04-21 14:07:55.000000 flow_pilot-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 14:31:36.949545 flow_pilot-0.1.3/flow_pilot.egg-info/
+drwxrwxrwx   0        0        0        0 2023-04-21 14:31:36.949545 flow_pilot-0.1.3/flow_pilot.egg-info/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0      162 2023-04-21 09:51:44.000000 flow_pilot-0.1.3/flow_pilot.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-rw-rw-   0        0        0       80 2023-04-21 14:31:36.000000 flow_pilot-0.1.3/flow_pilot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-21 14:31:36.000000 flow_pilot-0.1.3/flow_pilot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:31:36.000000 flow_pilot-0.1.3/flow_pilot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 14:31:36.000000 flow_pilot-0.1.3/flow_pilot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:31:36.951546 flow_pilot-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 14:31:36.950545 flow_pilot-0.1.3/tests/
+-rw-rw-rw-   0        0        0     3010 2023-04-21 14:07:39.000000 flow_pilot-0.1.3/tests/test_flowpilot.py
```

### Comparing `flow_pilot-0.1.2/FlowPilot/flow_pilot.py` & `flow_pilot-0.1.3/FlowPilot/flow_pilot.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,19 @@
 
         return wrapper
 
     def data_loader(self, func: Callable) -> Callable[..., Any]:
         """Tag a function as a data loader and save it in the 'data_loader' directory."""
         dir_path: str = 'data_loader'
         return self._file_writer(func, dir_path)
+    
+    def data_writer(self, func: Callable) -> Callable[..., Any]:
+        """Tag a function as a data writer and save it in the 'data_writer' directory."""
+        dir_path: str = 'data_writer'
+        return self._file_writer(func, dir_path)
 
     def preprocessor(self, func: Callable) -> Callable[..., Any]:
         """Tag a function as a preprocessor and save it in the 'preprocessor' directory."""
         dir_path: str = 'preprocessor'
         return self._file_writer(func, dir_path)
 
     def model_training(self, func: Callable) -> Callable[..., Any]:
```

### Comparing `flow_pilot-0.1.2/LICENSE` & `flow_pilot-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flow_pilot-0.1.2/README.md` & `flow_pilot-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `flow_pilot-0.1.2/tests/test_flowpilot.py` & `flow_pilot-0.1.3/tests/test_flowpilot.py`

 * *Files identical despite different names*

