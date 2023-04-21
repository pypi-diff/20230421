# Comparing `tmp/flow_pilot-0.1.3.tar.gz` & `tmp/flow_pilot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow_pilot-0.1.3.tar", last modified: Fri Apr 21 14:31:36 2023, max compression
+gzip compressed data, was "flow_pilot-0.1.4.tar", last modified: Fri Apr 21 14:41:46 2023, max compression
```

## Comparing `flow_pilot-0.1.3.tar` & `flow_pilot-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:31:36.951546 flow_pilot-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-04-21 14:31:36.937477 flow_pilot-0.1.3/FlowPilot/
--rw-rw-rw-   0        0        0       34 2023-04-21 10:55:09.000000 flow_pilot-0.1.3/FlowPilot/__init__.py
--rw-rw-rw-   0        0        0     5936 2023-04-21 14:31:02.000000 flow_pilot-0.1.3/FlowPilot/flow_pilot.py
--rw-rw-rw-   0        0        0      127 2023-04-21 14:31:06.000000 flow_pilot-0.1.3/FlowPilot/setup.py
--rw-rw-rw-   0        0        0     1087 2023-04-21 09:45:08.000000 flow_pilot-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       80 2023-04-21 14:31:36.950545 flow_pilot-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3487 2023-04-21 14:07:55.000000 flow_pilot-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 14:31:36.949545 flow_pilot-0.1.3/flow_pilot.egg-info/
-drwxrwxrwx   0        0        0        0 2023-04-21 14:31:36.949545 flow_pilot-0.1.3/flow_pilot.egg-info/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0      162 2023-04-21 09:51:44.000000 flow_pilot-0.1.3/flow_pilot.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-rw-rw-   0        0        0       80 2023-04-21 14:31:36.000000 flow_pilot-0.1.3/flow_pilot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-21 14:31:36.000000 flow_pilot-0.1.3/flow_pilot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:31:36.000000 flow_pilot-0.1.3/flow_pilot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 14:31:36.000000 flow_pilot-0.1.3/flow_pilot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 14:31:36.951546 flow_pilot-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 14:31:36.950545 flow_pilot-0.1.3/tests/
--rw-rw-rw-   0        0        0     3010 2023-04-21 14:07:39.000000 flow_pilot-0.1.3/tests/test_flowpilot.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:41:46.681075 flow_pilot-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-04-21 14:41:46.665488 flow_pilot-0.1.4/FlowPilot/
+-rw-rw-rw-   0        0        0       24 2023-04-21 14:41:00.000000 flow_pilot-0.1.4/FlowPilot/__init__.py
+-rw-rw-rw-   0        0        0     5936 2023-04-21 14:39:44.000000 flow_pilot-0.1.4/FlowPilot/flow_pilot.py
+-rw-rw-rw-   0        0        0     1087 2023-04-21 09:45:08.000000 flow_pilot-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       80 2023-04-21 14:41:46.665488 flow_pilot-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3487 2023-04-21 14:07:55.000000 flow_pilot-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 14:41:46.665488 flow_pilot-0.1.4/flow_pilot.egg-info/
+-rw-rw-rw-   0        0        0       80 2023-04-21 14:41:46.000000 flow_pilot-0.1.4/flow_pilot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-04-21 14:41:46.000000 flow_pilot-0.1.4/flow_pilot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:41:46.000000 flow_pilot-0.1.4/flow_pilot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 14:41:46.000000 flow_pilot-0.1.4/flow_pilot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:41:46.681075 flow_pilot-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      127 2023-04-21 14:39:38.000000 flow_pilot-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:41:46.665488 flow_pilot-0.1.4/tests/
+-rw-rw-rw-   0        0        0     3010 2023-04-21 14:39:53.000000 flow_pilot-0.1.4/tests/test_flowpilot.py
```

### Comparing `flow_pilot-0.1.3/FlowPilot/flow_pilot.py` & `flow_pilot-0.1.4/FlowPilot/flow_pilot.py`

 * *Files identical despite different names*

### Comparing `flow_pilot-0.1.3/LICENSE` & `flow_pilot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flow_pilot-0.1.3/README.md` & `flow_pilot-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `flow_pilot-0.1.3/tests/test_flowpilot.py` & `flow_pilot-0.1.4/tests/test_flowpilot.py`

 * *Files identical despite different names*

