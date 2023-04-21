# Comparing `tmp/tank_wars_iit-1.0.1.tar.gz` & `tmp/tank_wars_iit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tank_wars_iit-1.0.1.tar", last modified: Fri Apr 21 18:21:35 2023, max compression
+gzip compressed data, was "tank_wars_iit-1.0.2.tar", last modified: Fri Apr 21 18:28:28 2023, max compression
```

## Comparing `tank_wars_iit-1.0.1.tar` & `tank_wars_iit-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 18:21:35.644621 tank_wars_iit-1.0.1/
--rw-rw-rw-   0        0        0     1154 2023-04-21 12:24:12.000000 tank_wars_iit-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     5404 2023-04-21 18:21:35.644621 tank_wars_iit-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4713 2023-04-16 01:02:19.000000 tank_wars_iit-1.0.1/README.md
--rw-rw-rw-   0        0        0      833 2023-04-21 18:21:13.000000 tank_wars_iit-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      229 2023-04-21 18:21:35.645622 tank_wars_iit-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 18:21:35.593621 tank_wars_iit-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 18:21:35.605619 tank_wars_iit-1.0.1/src/tank_wars_iit/
--rw-rw-rw-   0        0        0      282 2023-04-21 17:47:12.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:21:35.623624 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/
--rw-rw-rw-   0        0        0      242 2023-04-21 17:47:00.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/__init__.py
--rw-rw-rw-   0        0        0    30197 2023-04-21 17:47:40.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/arena.py
--rw-rw-rw-   0        0        0    11336 2023-04-21 17:23:12.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/control.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:21:35.630620 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/entity/
--rw-rw-rw-   0        0        0      418 2023-04-21 17:47:03.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/entity/__init__.py
--rw-rw-rw-   0        0        0     3963 2023-04-21 17:46:07.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/entity/bullet.py
--rw-rw-rw-   0        0        0     2141 2023-04-21 17:46:09.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/entity/coin.py
--rw-rw-rw-   0        0        0     6797 2023-04-21 17:46:06.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/entity/entity.py
--rw-rw-rw-   0        0        0    24829 2023-04-21 17:46:36.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/entity/robot.py
--rw-rw-rw-   0        0        0     2824 2023-04-21 17:46:41.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/entity/wall.py
--rw-rw-rw-   0        0        0     1699 2023-04-21 14:15:33.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/map.py
--rw-rw-rw-   0        0        0    10237 2023-04-21 17:46:46.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/pathfinding.py
--rw-rw-rw-   0        0        0    18973 2023-04-21 12:24:12.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/quadtree.py
--rw-rw-rw-   0        0        0     9857 2023-04-21 17:46:52.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/robotlist.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:21:35.634620 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/util/
--rw-rw-rw-   0        0        0      804 2023-04-21 17:47:06.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/util/__init__.py
--rw-rw-rw-   0        0        0     2383 2023-04-04 07:12:58.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/util/draw.py
--rw-rw-rw-   0        0        0     6639 2023-04-21 17:46:04.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/util/geometry.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:21:35.636620 tank_wars_iit-1.0.1/src/tank_wars_iit/examples/
--rw-rw-rw-   0        0        0      447 2023-04-21 17:28:05.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/examples/__init__.py
--rw-rw-rw-   0        0        0     3205 2023-04-21 17:46:13.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/examples/controllers.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:21:35.642618 tank_wars_iit-1.0.1/src/tank_wars_iit/scenario/
--rw-rw-rw-   0        0        0      238 2023-04-21 17:21:01.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/scenario/__init__.py
--rw-rw-rw-   0        0        0     2335 2023-04-21 17:46:16.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/scenario/battleroyale.py
--rw-rw-rw-   0        0        0     1894 2023-04-21 17:46:27.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/scenario/onevsone.py
--rw-rw-rw-   0        0        0    19532 2023-04-21 17:46:31.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/scenario/tournament.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:21:35.643620 tank_wars_iit-1.0.1/src/tank_wars_iit/util/
--rw-rw-rw-   0        0        0      221 2023-04-21 17:47:15.000000 tank_wars_iit-1.0.1/src/tank_wars_iit/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:21:35.612621 tank_wars_iit-1.0.1/src/tank_wars_iit.egg-info/
--rw-rw-rw-   0        0        0     5404 2023-04-21 18:21:35.000000 tank_wars_iit-1.0.1/src/tank_wars_iit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1195 2023-04-21 18:21:35.000000 tank_wars_iit-1.0.1/src/tank_wars_iit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 18:21:35.000000 tank_wars_iit-1.0.1/src/tank_wars_iit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-21 18:21:35.000000 tank_wars_iit-1.0.1/src/tank_wars_iit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-21 18:21:35.000000 tank_wars_iit-1.0.1/src/tank_wars_iit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 18:28:28.691629 tank_wars_iit-1.0.2/
+-rw-rw-rw-   0        0        0     1154 2023-04-21 12:24:12.000000 tank_wars_iit-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       47 2023-04-21 18:26:56.000000 tank_wars_iit-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5404 2023-04-21 18:28:28.692631 tank_wars_iit-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4713 2023-04-16 01:02:19.000000 tank_wars_iit-1.0.2/README.md
+-rw-rw-rw-   0        0        0      833 2023-04-21 18:28:01.000000 tank_wars_iit-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      192 2023-04-21 18:28:28.693626 tank_wars_iit-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 18:28:28.632650 tank_wars_iit-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 18:28:28.645633 tank_wars_iit-1.0.2/src/tank_wars_iit/
+-rw-rw-rw-   0        0        0      282 2023-04-21 17:47:12.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:28:28.662633 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/
+-rw-rw-rw-   0        0        0      242 2023-04-21 17:47:00.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/__init__.py
+-rw-rw-rw-   0        0        0    30197 2023-04-21 17:47:40.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/arena.py
+-rw-rw-rw-   0        0        0    11336 2023-04-21 17:23:12.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/control.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:28:28.669629 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/entity/
+-rw-rw-rw-   0        0        0      418 2023-04-21 17:47:03.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/entity/__init__.py
+-rw-rw-rw-   0        0        0     3963 2023-04-21 17:46:07.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/entity/bullet.py
+-rw-rw-rw-   0        0        0     2141 2023-04-21 17:46:09.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/entity/coin.py
+-rw-rw-rw-   0        0        0     6797 2023-04-21 17:46:06.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/entity/entity.py
+-rw-rw-rw-   0        0        0    24829 2023-04-21 17:46:36.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/entity/robot.py
+-rw-rw-rw-   0        0        0     2824 2023-04-21 17:46:41.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/entity/wall.py
+-rw-rw-rw-   0        0        0     1699 2023-04-21 14:15:33.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/map.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:28:28.677629 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/maps/
+-rw-rw-rw-   0        0        0     1488 2023-04-21 14:15:33.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/maps/basic.json
+-rw-rw-rw-   0        0        0     9781 2023-04-21 17:51:42.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/maps/circles.json
+-rw-rw-rw-   0        0        0    10876 2023-04-21 17:52:18.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/maps/circles_large.json
+-rw-rw-rw-   0        0        0    24632 2023-04-21 17:52:22.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/maps/lock.json
+-rw-rw-rw-   0        0        0     6565 2023-04-21 17:52:25.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/maps/maze.json
+-rw-rw-rw-   0        0        0     4836 2023-04-21 17:52:29.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/maps/stress_test.json
+-rw-rw-rw-   0        0        0    10237 2023-04-21 17:46:46.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/pathfinding.py
+-rw-rw-rw-   0        0        0    18973 2023-04-21 12:24:12.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/quadtree.py
+-rw-rw-rw-   0        0        0     9857 2023-04-21 17:46:52.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/robotlist.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:28:28.681631 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/util/
+-rw-rw-rw-   0        0        0      804 2023-04-21 17:47:06.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/util/__init__.py
+-rw-rw-rw-   0        0        0     2383 2023-04-04 07:12:58.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/util/draw.py
+-rw-rw-rw-   0        0        0     6639 2023-04-21 17:46:04.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/util/geometry.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:28:28.683631 tank_wars_iit-1.0.2/src/tank_wars_iit/examples/
+-rw-rw-rw-   0        0        0      447 2023-04-21 17:28:05.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/examples/__init__.py
+-rw-rw-rw-   0        0        0     3205 2023-04-21 17:46:13.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/examples/controllers.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:28:28.689630 tank_wars_iit-1.0.2/src/tank_wars_iit/scenario/
+-rw-rw-rw-   0        0        0      238 2023-04-21 17:21:01.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/scenario/__init__.py
+-rw-rw-rw-   0        0        0     2335 2023-04-21 17:46:16.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/scenario/battleroyale.py
+-rw-rw-rw-   0        0        0     1894 2023-04-21 17:46:27.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/scenario/onevsone.py
+-rw-rw-rw-   0        0        0    19532 2023-04-21 17:46:31.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/scenario/tournament.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:28:28.690633 tank_wars_iit-1.0.2/src/tank_wars_iit/util/
+-rw-rw-rw-   0        0        0      221 2023-04-21 17:47:15.000000 tank_wars_iit-1.0.2/src/tank_wars_iit/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:28:28.653627 tank_wars_iit-1.0.2/src/tank_wars_iit.egg-info/
+-rw-rw-rw-   0        0        0     5404 2023-04-21 18:28:28.000000 tank_wars_iit-1.0.2/src/tank_wars_iit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1473 2023-04-21 18:28:28.000000 tank_wars_iit-1.0.2/src/tank_wars_iit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 18:28:28.000000 tank_wars_iit-1.0.2/src/tank_wars_iit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-21 18:28:28.000000 tank_wars_iit-1.0.2/src/tank_wars_iit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-21 18:28:28.000000 tank_wars_iit-1.0.2/src/tank_wars_iit.egg-info/top_level.txt
```

### Comparing `tank_wars_iit-1.0.1/LICENSE` & `tank_wars_iit-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/PKG-INFO` & `tank_wars_iit-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tank_wars_iit
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tank Wars framework for Scarlet HackNiite
 Author-email: Association for Computing Machinery at the Illinois Institute of Technology <acm@iit.edu>, Tommy Vadakumchery <t.vadakumchery1@gmail.com>
 Project-URL: Homepage, https://github.com/acm-iit/robot-wars
 Project-URL: Bug Tracker, https://github.com/acm-iit/robot-wars/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tank_wars_iit-1.0.1/README.md` & `tank_wars_iit-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/pyproject.toml` & `tank_wars_iit-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tank_wars_iit"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Association for Computing Machinery at the Illinois Institute of Technology", email="acm@iit.edu" },
   { name="Tommy Vadakumchery", email="t.vadakumchery1@gmail.com" },
 ]
 description = "Tank Wars framework for Scarlet HackNiite"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/arena.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/arena.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/control.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/control.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/entity/bullet.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/entity/bullet.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/entity/coin.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/entity/coin.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/entity/entity.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/entity/entity.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/entity/robot.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/entity/robot.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/entity/wall.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/entity/wall.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/map.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/map.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/pathfinding.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/pathfinding.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/quadtree.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/quadtree.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/robotlist.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/robotlist.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/util/__init__.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/util/draw.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/util/draw.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/_engine/util/geometry.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/_engine/util/geometry.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/examples/controllers.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/examples/controllers.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/scenario/battleroyale.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/scenario/battleroyale.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/scenario/onevsone.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/scenario/onevsone.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit/scenario/tournament.py` & `tank_wars_iit-1.0.2/src/tank_wars_iit/scenario/tournament.py`

 * *Files identical despite different names*

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit.egg-info/PKG-INFO` & `tank_wars_iit-1.0.2/src/tank_wars_iit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tank-wars-iit
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tank Wars framework for Scarlet HackNiite
 Author-email: Association for Computing Machinery at the Illinois Institute of Technology <acm@iit.edu>, Tommy Vadakumchery <t.vadakumchery1@gmail.com>
 Project-URL: Homepage, https://github.com/acm-iit/robot-wars
 Project-URL: Bug Tracker, https://github.com/acm-iit/robot-wars/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tank_wars_iit-1.0.1/src/tank_wars_iit.egg-info/SOURCES.txt` & `tank_wars_iit-1.0.2/src/tank_wars_iit.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 src/tank_wars_iit/__init__.py
 src/tank_wars_iit.egg-info/PKG-INFO
 src/tank_wars_iit.egg-info/SOURCES.txt
 src/tank_wars_iit.egg-info/dependency_links.txt
@@ -17,14 +18,20 @@
 src/tank_wars_iit/_engine/robotlist.py
 src/tank_wars_iit/_engine/entity/__init__.py
 src/tank_wars_iit/_engine/entity/bullet.py
 src/tank_wars_iit/_engine/entity/coin.py
 src/tank_wars_iit/_engine/entity/entity.py
 src/tank_wars_iit/_engine/entity/robot.py
 src/tank_wars_iit/_engine/entity/wall.py
+src/tank_wars_iit/_engine/maps/basic.json
+src/tank_wars_iit/_engine/maps/circles.json
+src/tank_wars_iit/_engine/maps/circles_large.json
+src/tank_wars_iit/_engine/maps/lock.json
+src/tank_wars_iit/_engine/maps/maze.json
+src/tank_wars_iit/_engine/maps/stress_test.json
 src/tank_wars_iit/_engine/util/__init__.py
 src/tank_wars_iit/_engine/util/draw.py
 src/tank_wars_iit/_engine/util/geometry.py
 src/tank_wars_iit/examples/__init__.py
 src/tank_wars_iit/examples/controllers.py
 src/tank_wars_iit/scenario/__init__.py
 src/tank_wars_iit/scenario/battleroyale.py
```

