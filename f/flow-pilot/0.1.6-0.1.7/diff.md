# Comparing `tmp/flow_pilot-0.1.6.tar.gz` & `tmp/flow_pilot-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow_pilot-0.1.6.tar", last modified: Fri Apr 21 14:49:03 2023, max compression
+gzip compressed data, was "flow_pilot-0.1.7.tar", last modified: Fri Apr 21 14:54:04 2023, max compression
```

## Comparing `flow_pilot-0.1.6.tar` & `flow_pilot-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:49:03.551280 flow_pilot-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-04-21 14:49:03.535637 flow_pilot-0.1.6/FlowPilot/
--rw-rw-rw-   0        0        0       34 2023-04-21 14:48:47.000000 flow_pilot-0.1.6/FlowPilot/__init__.py
--rw-rw-rw-   0        0        0     5889 2023-04-21 14:46:24.000000 flow_pilot-0.1.6/FlowPilot/flow_pilot.py
--rw-rw-rw-   0        0        0     1087 2023-04-21 09:45:08.000000 flow_pilot-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       80 2023-04-21 14:49:03.551280 flow_pilot-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3487 2023-04-21 14:07:55.000000 flow_pilot-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 14:49:03.551280 flow_pilot-0.1.6/flow_pilot.egg-info/
--rw-rw-rw-   0        0        0       80 2023-04-21 14:49:03.000000 flow_pilot-0.1.6/flow_pilot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-04-21 14:49:03.000000 flow_pilot-0.1.6/flow_pilot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:49:03.000000 flow_pilot-0.1.6/flow_pilot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 14:49:03.000000 flow_pilot-0.1.6/flow_pilot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 14:49:03.551280 flow_pilot-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      127 2023-04-21 14:49:00.000000 flow_pilot-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:49:03.551280 flow_pilot-0.1.6/tests/
--rw-rw-rw-   0        0        0     3010 2023-04-21 14:39:53.000000 flow_pilot-0.1.6/tests/test_flowpilot.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:54:04.981632 flow_pilot-0.1.7/
+drwxrwxrwx   0        0        0        0 2023-04-21 14:54:04.948063 flow_pilot-0.1.7/FlowPilot/
+-rw-rw-rw-   0        0        0       24 2023-04-21 14:53:12.000000 flow_pilot-0.1.7/FlowPilot/__init__.py
+-rw-rw-rw-   0        0        0     5889 2023-04-21 14:46:24.000000 flow_pilot-0.1.7/FlowPilot/flow_pilot.py
+-rw-rw-rw-   0        0        0     1087 2023-04-21 09:45:08.000000 flow_pilot-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       80 2023-04-21 14:54:04.981632 flow_pilot-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3487 2023-04-21 14:07:55.000000 flow_pilot-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 14:54:04.963832 flow_pilot-0.1.7/flow_pilot.egg-info/
+-rw-rw-rw-   0        0        0       80 2023-04-21 14:54:04.000000 flow_pilot-0.1.7/flow_pilot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-04-21 14:54:04.000000 flow_pilot-0.1.7/flow_pilot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:54:04.000000 flow_pilot-0.1.7/flow_pilot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 14:54:04.000000 flow_pilot-0.1.7/flow_pilot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:54:04.981632 flow_pilot-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      127 2023-04-21 14:53:42.000000 flow_pilot-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:54:04.963832 flow_pilot-0.1.7/tests/
+-rw-rw-rw-   0        0        0     3010 2023-04-21 14:39:53.000000 flow_pilot-0.1.7/tests/test_flowpilot.py
```

### Comparing `flow_pilot-0.1.6/FlowPilot/flow_pilot.py` & `flow_pilot-0.1.7/FlowPilot/flow_pilot.py`

 * *Files identical despite different names*

### Comparing `flow_pilot-0.1.6/LICENSE` & `flow_pilot-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flow_pilot-0.1.6/README.md` & `flow_pilot-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `flow_pilot-0.1.6/tests/test_flowpilot.py` & `flow_pilot-0.1.7/tests/test_flowpilot.py`

 * *Files identical despite different names*

