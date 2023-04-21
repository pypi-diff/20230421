# Comparing `tmp/processpiper-0.2.0.tar.gz` & `tmp/processpiper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processpiper-0.2.0.tar", last modified: Mon Apr 17 09:22:21 2023, max compression
+gzip compressed data, was "processpiper-0.3.0.tar", last modified: Fri Apr 21 09:16:03 2023, max compression
```

## Comparing `processpiper-0.2.0.tar` & `processpiper-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 09:22:21.723548 processpiper-0.2.0/
--rw-rw-rw-   0        0        0     1084 2023-01-11 04:26:51.000000 processpiper-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     6655 2023-04-17 09:22:21.722547 processpiper-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6100 2023-04-17 09:21:44.000000 processpiper-0.2.0/README.md
--rw-rw-rw-   0        0        0     1014 2023-04-09 04:12:22.000000 processpiper-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 09:22:21.723548 processpiper-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 09:22:21.684538 processpiper-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 09:22:21.704543 processpiper-0.2.0/src/processpiper/
--rw-rw-rw-   0        0        0      188 2023-04-09 10:02:01.000000 processpiper-0.2.0/src/processpiper/__init__.py
--rw-rw-rw-   0        0        0     2090 2023-04-09 09:57:23.000000 processpiper-0.2.0/src/processpiper/activity.py
--rw-rw-rw-   0        0        0    11673 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/processpiper/colourtheme.py
--rw-rw-rw-   0        0        0     1752 2023-04-10 02:30:30.000000 processpiper-0.2.0/src/processpiper/constants.py
--rw-rw-rw-   0        0        0     4978 2023-04-16 00:55:33.000000 processpiper-0.2.0/src/processpiper/event.py
--rw-rw-rw-   0        0        0     2339 2023-04-09 09:10:37.000000 processpiper-0.2.0/src/processpiper/footer.py
--rw-rw-rw-   0        0        0     2800 2023-04-09 09:10:50.000000 processpiper-0.2.0/src/processpiper/gateway.py
--rw-rw-rw-   0        0        0     1658 2023-04-10 03:27:48.000000 processpiper-0.2.0/src/processpiper/helper.py
--rw-rw-rw-   0        0        0    10507 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/processpiper/lane.py
--rw-rw-rw-   0        0        0    35774 2023-04-16 00:46:46.000000 processpiper-0.2.0/src/processpiper/painter.py
--rw-rw-rw-   0        0        0     5043 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/processpiper/pool.py
--rw-rw-rw-   0        0        0    17603 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/processpiper/processmap.py
--rw-rw-rw-   0        0        0    18609 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/processpiper/shape.py
--rw-rw-rw-   0        0        0     6829 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/processpiper/text2diagram.py
--rw-rw-rw-   0        0        0     2267 2023-04-09 09:14:12.000000 processpiper-0.2.0/src/processpiper/title.py
--rw-rw-rw-   0        0        0     1189 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/processpiper/version.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:22:21.719547 processpiper-0.2.0/src/processpiper.egg-info/
--rw-rw-rw-   0        0        0     6655 2023-04-17 09:22:21.000000 processpiper-0.2.0/src/processpiper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-04-17 09:22:21.000000 processpiper-0.2.0/src/processpiper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 09:22:21.000000 processpiper-0.2.0/src/processpiper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-17 09:22:21.000000 processpiper-0.2.0/src/processpiper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-17 09:22:21.000000 processpiper-0.2.0/src/processpiper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 09:22:21.720547 processpiper-0.2.0/src/tests/
--rw-rw-rw-   0        0        0        0 2023-04-09 04:19:21.000000 processpiper-0.2.0/src/tests/__init__.py
--rw-rw-rw-   0        0        0     2170 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/tests/github_action_test.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:16:03.038380 processpiper-0.3.0/
+-rw-rw-rw-   0        0        0     1084 2023-01-11 04:26:51.000000 processpiper-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     6245 2023-04-21 09:16:03.037380 processpiper-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5690 2023-04-21 09:15:30.000000 processpiper-0.3.0/README.md
+-rw-rw-rw-   0        0        0     1014 2023-04-09 04:12:22.000000 processpiper-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 09:16:03.038380 processpiper-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 09:16:03.007374 processpiper-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 09:16:03.022377 processpiper-0.3.0/src/processpiper/
+-rw-rw-rw-   0        0        0      188 2023-04-09 10:02:01.000000 processpiper-0.3.0/src/processpiper/__init__.py
+-rw-rw-rw-   0        0        0     2090 2023-04-09 09:57:23.000000 processpiper-0.3.0/src/processpiper/activity.py
+-rw-rw-rw-   0        0        0    11673 2023-04-17 09:21:44.000000 processpiper-0.3.0/src/processpiper/colourtheme.py
+-rw-rw-rw-   0        0        0     1753 2023-04-21 08:48:40.000000 processpiper-0.3.0/src/processpiper/constants.py
+-rw-rw-rw-   0        0        0     4978 2023-04-16 00:55:33.000000 processpiper-0.3.0/src/processpiper/event.py
+-rw-rw-rw-   0        0        0     2339 2023-04-09 09:10:37.000000 processpiper-0.3.0/src/processpiper/footer.py
+-rw-rw-rw-   0        0        0     2800 2023-04-09 09:10:50.000000 processpiper-0.3.0/src/processpiper/gateway.py
+-rw-rw-rw-   0        0        0     1658 2023-04-10 03:27:48.000000 processpiper-0.3.0/src/processpiper/helper.py
+-rw-rw-rw-   0        0        0    10689 2023-04-21 08:45:10.000000 processpiper-0.3.0/src/processpiper/lane.py
+-rw-rw-rw-   0        0        0    35665 2023-04-21 04:25:43.000000 processpiper-0.3.0/src/processpiper/painter.py
+-rw-rw-rw-   0        0        0     5043 2023-04-17 09:21:44.000000 processpiper-0.3.0/src/processpiper/pool.py
+-rw-rw-rw-   0        0        0    18855 2023-04-21 08:59:35.000000 processpiper-0.3.0/src/processpiper/processmap.py
+-rw-rw-rw-   0        0        0    19242 2023-04-21 08:51:52.000000 processpiper-0.3.0/src/processpiper/shape.py
+-rw-rw-rw-   0        0        0     9016 2023-04-21 09:05:31.000000 processpiper-0.3.0/src/processpiper/text2diagram.py
+-rw-rw-rw-   0        0        0     2267 2023-04-09 09:14:12.000000 processpiper-0.3.0/src/processpiper/title.py
+-rw-rw-rw-   0        0        0     1189 2023-04-21 06:29:34.000000 processpiper-0.3.0/src/processpiper/version.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:16:03.035380 processpiper-0.3.0/src/processpiper.egg-info/
+-rw-rw-rw-   0        0        0     6245 2023-04-21 09:16:02.000000 processpiper-0.3.0/src/processpiper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-04-21 09:16:03.000000 processpiper-0.3.0/src/processpiper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:16:02.000000 processpiper-0.3.0/src/processpiper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-21 09:16:02.000000 processpiper-0.3.0/src/processpiper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-21 09:16:02.000000 processpiper-0.3.0/src/processpiper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 09:16:03.036380 processpiper-0.3.0/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-09 04:19:21.000000 processpiper-0.3.0/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     2170 2023-04-17 09:21:44.000000 processpiper-0.3.0/src/tests/github_action_test.py
```

### Comparing `processpiper-0.2.0/LICENSE` & `processpiper-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `processpiper-0.2.0/PKG-INFO` & `processpiper-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: processpiper
-Version: 0.2.0
+Version: 0.3.0
 Summary: Processpiper. An open source python library to generate business process diagram using code.
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/processpiper
 Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![release](https://img.shields.io/pypi/v/processpiper?style=plastic)
 ![Wheel](https://img.shields.io/pypi/wheel/processpiper?style=plastic)
+![Downloads](https://img.shields.io/pypi/dm/processpiper?style=plastic)
 ![Platforms](https://img.shields.io/badge/Platform%3A-win%20%7C%20ubuntu%20%7C%20osx-brightgreen?style=plastic)
 [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=plastic)](https://en.wikipedia.org/wiki/MIT_License)
 [![CodeFactor](https://www.codefactor.io/repository/github/csgoh/processpiper/badge?style=plastic)](https://www.codefactor.io/repository/github/csgoh/processpiper)
 ![code size](https://img.shields.io/github/languages/code-size/csgoh/processmapper?style=plastic)
 ![python version](https://img.shields.io/pypi/pyversions/processpiper?style=plastic)
 ![stars](https://img.shields.io/github/stars/csgoh/processpiper?style=plastic)
 [![Twitter Follow](https://img.shields.io/twitter/follow/CSGohNZ?style=social)](https://twitter.com/CSGohNZ)
@@ -141,23 +142,18 @@
 ```
 
 The generated diagram is as follows:
 ![Process Map](https://github.com/csgoh/processpiper/blob/main/images/test/test_auto_case1.png)
 
 
 ## Development Status
-First version 0.1.0 is released. This release would only cover the following basic business process elements. Other element types will be introduced in subsequence releases.
+Initial first release would only cover the following basic business process elements. Other element types will be introduced in subsequence releases.
 
 * Event: Start, End, Timer, Intermediate
 * Activity: Task, Subprocess
 * Gateway: Inclusive, Exclusive, Parallel
 
 Any ideas or suggestions, please send it to me via [GitHub Discussions](https://github.com/csgoh/processmapper/discussions).
 
 
-Thank you for checking out my project. If you have found ProcessPiper useful and would like to show your appreciation, consider buying me a coffee or flat white :coffee: and keep me going. To buy me a coffee, simply follow this link: 
-
-<a href="https://www.buymeacoffee.com/csgoh" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
-
-
```

### Comparing `processpiper-0.2.0/README.md` & `processpiper-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ![release](https://img.shields.io/pypi/v/processpiper?style=plastic)
 ![Wheel](https://img.shields.io/pypi/wheel/processpiper?style=plastic)
+![Downloads](https://img.shields.io/pypi/dm/processpiper?style=plastic)
 ![Platforms](https://img.shields.io/badge/Platform%3A-win%20%7C%20ubuntu%20%7C%20osx-brightgreen?style=plastic)
 [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=plastic)](https://en.wikipedia.org/wiki/MIT_License)
 [![CodeFactor](https://www.codefactor.io/repository/github/csgoh/processpiper/badge?style=plastic)](https://www.codefactor.io/repository/github/csgoh/processpiper)
 ![code size](https://img.shields.io/github/languages/code-size/csgoh/processmapper?style=plastic)
 ![python version](https://img.shields.io/pypi/pyversions/processpiper?style=plastic)
 ![stars](https://img.shields.io/github/stars/csgoh/processpiper?style=plastic)
 [![Twitter Follow](https://img.shields.io/twitter/follow/CSGohNZ?style=social)](https://twitter.com/CSGohNZ)
@@ -127,23 +128,18 @@
 ```
 
 The generated diagram is as follows:
 ![Process Map](https://github.com/csgoh/processpiper/blob/main/images/test/test_auto_case1.png)
 
 
 ## Development Status
-First version 0.1.0 is released. This release would only cover the following basic business process elements. Other element types will be introduced in subsequence releases.
+Initial first release would only cover the following basic business process elements. Other element types will be introduced in subsequence releases.
 
 * Event: Start, End, Timer, Intermediate
 * Activity: Task, Subprocess
 * Gateway: Inclusive, Exclusive, Parallel
 
 Any ideas or suggestions, please send it to me via [GitHub Discussions](https://github.com/csgoh/processmapper/discussions).
 
 
-Thank you for checking out my project. If you have found ProcessPiper useful and would like to show your appreciation, consider buying me a coffee or flat white :coffee: and keep me going. To buy me a coffee, simply follow this link: 
-
-<a href="https://www.buymeacoffee.com/csgoh" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
-
-
```

### Comparing `processpiper-0.2.0/pyproject.toml` & `processpiper-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `processpiper-0.2.0/src/processpiper/activity.py` & `processpiper-0.3.0/src/processpiper/activity.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.2.0/src/processpiper/colourtheme.py` & `processpiper-0.3.0/src/processpiper/colourtheme.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.2.0/src/processpiper/constants.py` & `processpiper-0.3.0/src/processpiper/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 
     POOL_TEXT_WIDTH = 50
 
     LANE_TEXT_WIDTH = 50
 
     LANE_SHAPE_TOP_MARGIN = 50
     LANE_SHAPE_BOTTOM_MARGIN = 50
-    LANE_SHAPE_LEFT_MARGIN = 30
+    LANE_SHAPE_LEFT_MARGIN = 50
     LANE_SHAPE_RIGHT_MARGIN = 30
 
-    HSPACE_BETWEEN_SHAPES = 70
-    VSPACE_BETWEEN_SHAPES = 50
+    HSPACE_BETWEEN_SHAPES = 50
+    VSPACE_BETWEEN_SHAPES = 100
 
     VSPACE_BETWEEN_POOLS = 10
     VSPACE_BETWEEN_LANES = 2
 
     HSPACE_BETWEEN_POOL_AND_LANE = 2
```

### Comparing `processpiper-0.2.0/src/processpiper/event.py` & `processpiper-0.3.0/src/processpiper/event.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.2.0/src/processpiper/footer.py` & `processpiper-0.3.0/src/processpiper/footer.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.2.0/src/processpiper/gateway.py` & `processpiper-0.3.0/src/processpiper/gateway.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.2.0/src/processpiper/helper.py` & `processpiper-0.3.0/src/processpiper/helper.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.2.0/src/processpiper/lane.py` & `processpiper-0.3.0/src/processpiper/lane.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 from itertools import count
 from .shape import Shape
 from .painter import Painter
 from .event import Event, Start, End, Timer, Intermediate
 from .activity import Activity, Task, Subprocess
 from .gateway import Gateway, Exclusive, Parallel, Inclusive
 from .constants import Configs
-#from .helper import Helper
+from .helper import Helper
+
+# from .helper import Helper
 
 
 class EventType:
     """Event types"""
 
     START = "Start"
     END = "End"
@@ -194,20 +196,23 @@
             self.y + self.height,
             "white",
             0.5,
             5,
             "solid",
         )
         ### Uncomment the following line to see the grid. Useful for debugging
-        ####self.painter.draw_grid()
+        ###self.painter.draw_grid()
 
     def draw_shape(self) -> None:
         """Draw the shapes in the lane"""
         if self.shapes:
             for shape in self.shapes:
+                Helper.printc(
+                    f"Drawing shape: {shape.name}, x={shape.x}, y={shape.y}, w={shape.width}, h={shape.height}"
+                )
                 shape.draw(self.painter)
 
     def draw_connection(self) -> None:
         """Draw the connections in the lane"""
         if self.shapes:
             for shape in self.shapes:
                 shape.draw_connection(self.painter)
@@ -251,15 +256,15 @@
         ### Set own shape position
         if shape.lane_name == self.name:
             shape_x, shape_y, shape_w, shape_h = shape.set_draw_position(
                 x,
                 (y + Configs.LANE_SHAPE_TOP_MARGIN),
                 painter,
             )
-            
+
             #### Mark for removal
             # shape.draw_position_set = True
 
             shape.x_pos_traversed = True
 
             ### Set next elements' position
             for index, next_shape in enumerate(shape.connection_to.target):
```

### Comparing `processpiper-0.2.0/src/processpiper/painter.py` & `processpiper-0.3.0/src/processpiper/painter.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,27 +559,26 @@
         connector_line_width,
         connector_line_colour,
     ):
         """Draw a horizontal dashed line"""
         gap_size = 10
         x1 = int(x1)
         x2 = int(x2)
-        print(f"horizontal dashed line: {x1}, {y1}, {x2}, {y2}")
+
         if x1 > x2:
             x1 += 10
             for i in range(x2, x1, gap_size):
                 # print(f">> {i}, {y1}, {x2}, {y2}")
                 if i - 5 < x2:
                     new_x = x2
                 else:
                     new_x = i - 5
                 # print(f"x1 > x2    {i}, {y1}, {new_x}, {y2}")
                 self.__cr.line((i, y1, new_x, y2), fill="black", width=1)
         else:
-
             for i in range(x1, x2, gap_size):
                 if i + 5 > x2:
                     new_x = x2
                 else:
                     new_x = i + 5
                 # print(f"x2 < x1    {i}, {y1}, {new_x}, {y2}")
                 self.__cr.line((i, y1, new_x, y2), fill="black", width=1)
@@ -717,15 +716,14 @@
                 right_angle_point = (x2, y1 - elbow_height)
             else:
                 Helper.printc(
                     f"   D-else: right_angle_line: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}"
                 )
                 # if so, then the line should be drawn from the bottom side of the box
                 points = [(x1, y1), (x1, y2), (x2, y2)]
-                print(f"points {points}")
                 right_angle_point = (x1, y2)
             # for point in points:
             #     self.draw_circle(point[0], point[1], 4, "yellow")
 
         if x1 > x2:
             if y1 <= y2:
                 if abs(y1 - y2) == 10:
```

### Comparing `processpiper-0.2.0/src/processpiper/pool.py` & `processpiper-0.3.0/src/processpiper/pool.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.2.0/src/processpiper/processmap.py` & `processpiper-0.3.0/src/processpiper/processmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,27 @@
 from .pool import Pool
 from .painter import Painter
 from .shape import Shape
 from .title import Title
 from .footer import Footer
 from .constants import Configs
 from .helper import Helper
-
+from PIL import Image
 import time
 import logging
 
 
 class UnconnectedElementException(Exception):
     pass
 
 
+class EmptyProcessMapException(Exception):
+    pass
+
+
 @dataclass
 class ProcessMap:
     """Process Map Class"""
 
     title: str = field(init=True, default="<Process Map Title>")
     width: int = field(init=True, default=3200)
     height: int = field(init=True, default=3200)
@@ -168,26 +172,28 @@
                 + Configs.HSPACE_BETWEEN_POOL_AND_LANE
                 + Configs.LANE_TEXT_WIDTH
                 + Configs.LANE_SHAPE_LEFT_MARGIN
             )
 
         return self.next_shape_x
 
-    def get_next_x_position(self) -> int:
+    def get_next_x_position(self, previous_shape_width: str) -> int:
         """Get the next x position for the next shape to be added"""
         if self.next_shape_x == 0:
             self.next_shape_x = (
                 Configs.SURFACE_LEFT_MARGIN
                 + Configs.POOL_TEXT_WIDTH
                 + Configs.HSPACE_BETWEEN_POOL_AND_LANE
                 + Configs.LANE_TEXT_WIDTH
                 + Configs.LANE_SHAPE_LEFT_MARGIN
             )
+            Helper.printc(f"            [0]get_next_x_position: {self.next_shape_x}")
         else:
-            self.next_shape_x += 100 + Configs.HSPACE_BETWEEN_SHAPES
+            self.next_shape_x += previous_shape_width + Configs.VSPACE_BETWEEN_SHAPES
+            Helper.printc(f"            [1]get_next_x_position: {self.next_shape_x}")
         return self.next_shape_x
 
     def find_start_shape(self) -> Shape:
         """Find the start shape in the process map"""
         for pool in self._pools:
             for lane in pool._lanes:
                 for shape in lane.shapes:
@@ -221,28 +227,28 @@
     ):
         """Set the x position for the shape"""
         current_lane = self.get_lane_by_id(current_shape.lane_id)
         Helper.printc(
             f"set_shape_x_position: {current_lane.name}, {current_shape.name}", "34"
         )
         if index == 0:
-            
+
             if previous_shape is not None:
                 if previous_shape.pool_name == current_shape.pool_name:
                     if previous_shape.lane_id == current_shape.lane_id:
-                        current_shape.x = self.get_next_x_position()
+                        current_shape.x = self.get_next_x_position(previous_shape.width)
                         Helper.printc(f"          same pool same lane")
                     else:
-                        current_shape.x = self.get_next_x_position()
+                        current_shape.x = self.get_next_x_position(previous_shape.width)
                         Helper.printc(f"          same pool diff lane")
                 else:
-                    current_shape.x = self.get_next_x_position()
+                    current_shape.x = self.get_next_x_position(previous_shape.width)
                     Helper.printc(f"          diff pool")
             else:
-                current_shape.x = self.get_next_x_position()
+                current_shape.x = self.get_next_x_position(0)
                 Helper.printc(f"          previous = none")
         else:
             ### If previous shape is connecting to multiple shapes,
             ### the x position of the shape is the same as the previous shape
             current_shape.x = x_pos
         current_lane.width = max(current_lane.width, current_shape.x + 100)
         Helper.printc(
@@ -411,14 +417,34 @@
                     ):
                         orphan_elements.append(shape.name)
 
         return orphan_elements
 
     def draw(self) -> None:
         """Draw the process map"""
+
+        ### Ensure title is defined
+        if (len(self.title) == 0) and (self._title == None):
+            raise ValueError("The process map must contain a title")
+
+        ### Ensure at least a pool is defined
+        if len(self._pools) == 0:
+            raise EmptyProcessMapException(
+                "The process map must contain at least one pool or lane"
+            )
+
+        ### Ensure at least one shape is defined
+        for pool in self._pools:
+            if len(pool._lanes) > 0:
+                if len(pool._lanes[0].shapes) == 0:
+                    raise EmptyProcessMapException(
+                        "The process map must contain at least one shape"
+                    )
+
+        ### Ensure connections are defined
         orphan_elements = self.get_orphan_elements()
         if len(orphan_elements) > 0:
             raise UnconnectedElementException(
                 f"The following element(s) are defined but not connected to other element(s): \n{orphan_elements}"
             )
 
         self.set_draw_position(self.__painter)
@@ -457,14 +483,18 @@
     def save(self, filename: str) -> None:
         """This method saves the process map to a file"""
         self.__painter.save_surface(filename)
 
         elapsed_time = (time.time() - self.start_time) * 1000
         Helper.info_log(f"Took [{elapsed_time:.2f}ms] to generate '{filename}' diagram")
 
+    # def get_image(self) -> Image:
+    #     """This method returns the process map image"""
+    #     return self.__painter.get_image()
+
     def __enter__(self):
         """This method is called when the 'with' statement is used"""
         return self
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         """This method is called when the 'with' statement is used"""
         pass
```

### Comparing `processpiper-0.2.0/src/processpiper/shape.py` & `processpiper-0.3.0/src/processpiper/shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,32 +318,37 @@
                     painter.connector_line_width,
                     painter.connector_line_colour,
                     painter.connector_arrow_colour,
                     painter.connector_arrow_size,
                 )
 
 
+@dataclass
 class Box(Shape):
     """Box shape"""
 
+    def __post_init__(self):
+        self.width = BOX_WIDTH
+        self.height = BOX_HEIGHT
+
     def set_draw_position(self, painter: Painter) -> tuple:
         """Set draw position of box
 
         Args:
             x (int): x position
             y (int): y position
             painter (Painter): Painter object
 
         Returns:
             tuple: x, y position
         """
         # self.x = x
         # self.y = y
-        self.width = BOX_WIDTH
-        self.height = BOX_HEIGHT
+        # self.width = BOX_WIDTH
+        # self.height = BOX_HEIGHT
         self.points = {
             ### Uncomment the following if we need more connection points
             # "top_left": (self.x, self.y),
             # "top_right": (self.x + self.width, self.y),
             # "bottom_left": (self.x, self.y + self.height),
             # "bottom_right": (self.x + self.width, self.y + self.height),
             "left_middle": (self.x, self.y + self.height / 2),
@@ -379,27 +384,34 @@
             text_font_size=self.font_size,
             text_font_colour=self.font_colour,
         )
 
         super().draw(painter)
 
 
+@dataclass
 class Circle(Shape):
     """Circle shape"""
 
     text_x: int = field(init=False)
     text_y: int = field(init=False)
     text_width: int = field(init=False)
     text_height: int = field(init=False)
 
+    def __post_init__(self):
+        self.radius = CIRCLE_RADIUS
+
     def set_draw_position(self, painter: Painter) -> tuple:
         """Set draw position of circle"""
         ### Circle x position starts from the circle centre, so add radius to x.
         ### But we want to cater for cases when circle and box aligned vertically.
-        self.x = int(self.x + CIRCLE_RADIUS + (BOX_WIDTH / 2) - (CIRCLE_RADIUS))
+        # self.x = int(self.x + CIRCLE_RADIUS + (BOX_WIDTH / 2) - (CIRCLE_RADIUS))
+        # self.x = int(self.x + CIRCLE_RADIUS)
+        # self.x = int(self.x + (BOX_WIDTH / 2) - (CIRCLE_RADIUS))
+        # self.x = int(self.x - (CIRCLE_RADIUS))
         self.y = int(self.y + (BOX_HEIGHT / 2))
         self.radius = CIRCLE_RADIUS
         self.points = {
             "right": (
                 self.x + self.radius * math.cos(math.radians(0)),
                 self.y + self.radius * math.sin(math.radians(0)),
             ),
@@ -432,31 +444,40 @@
             self.text_y,
             self.name,
             self.font,
             self.font_size,
             self.font_colour,
         )
         super().draw(painter)
-        # painter.draw_circle(self.points["top"][0], self.points["top"][1], 4, "red")
+        # painter.draw_circle(self.points["left"][0], self.points["left"][1], 2, "red")
+        # painter.draw_circle(self.points["right"][0], self.points["right"][1], 2, "red")
 
 
+@dataclass
 class Diamond(Shape):
     """Diamond shape"""
 
     text_x: int = field(init=False)
     text_y: int = field(init=False)
     text_width: int = field(init=False)
     text_height: int = field(init=False)
 
+    def __post_init__(self):
+        self.width = DIAMOND_WIDTH
+        self.height = DIAMOND_HEIGHT
+
     def set_draw_position(self, painter: Painter) -> tuple:
         """Set draw position of diamond"""
-        self.x = self.x + (BOX_WIDTH / 2) - (DIAMOND_WIDTH / 2)
+
+        # self.x = self.x + (BOX_WIDTH / 2) - (DIAMOND_WIDTH / 2)
+        # self.x = self.x - (DIAMOND_WIDTH / 2)
         self.y = self.y + (BOX_HEIGHT / 2) - (DIAMOND_HEIGHT / 2)
-        self.width = DIAMOND_WIDTH
-        self.height = DIAMOND_HEIGHT
+
+        # self.width = DIAMOND_WIDTH
+        # self.height = DIAMOND_HEIGHT
         self.points = {
             "top_middle": (self.x + self.width / 2, self.y),
             "right_middle": (self.x + self.width, self.y + self.height / 2),
             "bottom_middle": (self.x + self.width / 2, self.y + self.height),
             "left_middle": (self.x, self.y + self.height / 2),
         }
         self.text_width, self.text_height = painter.get_text_dimension(
```

### Comparing `processpiper-0.2.0/src/processpiper/text2diagram.py` & `processpiper-0.3.0/src/processpiper/text2diagram.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,26 @@
+import datetime
 import re
+from processpiper.helper import Helper
+from PIL import Image
+
 
 def parse_and_generate_code(input_str, png_output_file):
-    """Parse input string and generate code to create a diagram"""
+    """
+    Parse input string and generate code to create a diagram
+    """
 
     lines = input_str.strip().split("\n")
     process_map_title = parse_title(lines)
 
+    if len(lines) == 0:
+        raise ValueError(
+            "No business process definition found. Please add pool(s), lane(s) and element(s)."
+        )
+
     colour_theme = parse_colour_theme(lines)
 
     code_lines = [
         "from processpiper import ProcessMap, EventType, ActivityType, GatewayType",
         f'with ProcessMap("{process_map_title}") as my_process_map:'
         if colour_theme is None
         else f'with ProcessMap("{process_map_title}", colour_theme="{colour_theme}") as my_process_map:',
@@ -36,101 +47,135 @@
         code_lines.append(f'{indent}my_process_map.set_footer("{footer[1]}")')
 
     code_lines.append(f"{indent}my_process_map.draw()")
     code_lines.append(f'{indent}my_process_map.save("{png_output_file}")')
 
     return "\n".join(code_lines)
 
+
 def parse_element(lines, code_lines, indent, lane_id):
+    """
+    This function parses an element from a list of lines and adds it to a code block with the
+    appropriate indentation.
+    """
     while (
-                lines
-                and not lines[0].strip().startswith("lane:")
-                and not lines[0].strip().startswith("pool:")
-                and not lines[0].strip().startswith("footer:")
-                and not lines[0].strip() == ""
-            ):
+        lines
+        and not lines[0].strip().startswith("lane:")
+        and not lines[0].strip().startswith("pool:")
+        and not lines[0].strip().startswith("footer:")
+        and lines[0].strip() != ""
+    ):
         lane_element = lines.pop(0).strip()
-        element_type, element_name, element_var = parse_lane_element(
-                    lane_element
-                )
+        # check if lane_element contained '->' characters
+        if lane_element.find("->") > 0:
+            # push lane_element back to lines
+            lines.insert(0, lane_element)
+            break
+        element_type, element_name, element_var = parse_lane_element(lane_element)
         code_lines.append(
-                    f'{indent}{element_var} = lane{lane_id}.add_element("{element_name}", {element_type})'
-                )
+            f'{indent}{element_var} = lane{lane_id}.add_element("{element_name}", {element_type})'
+        )
+
 
 def parse_lane(code_lines, pool_id, lane_id, pool_found, line):
+    """
+    The function parses a lane from a code line and adds it to a process map.
+    """
     lane_name = line.split(":")[1].strip()
     lane_id += 1
     if pool_found:
         indent = " " * 8
         code_lines.append(
-                    f'{indent}with pool{pool_id - 1}.add_lane("{lane_name}") as lane{lane_id}:'
-                )
+            f'{indent}with pool{pool_id - 1}.add_lane("{lane_name}") as lane{lane_id}:'
+        )
     else:
         indent = " " * 4
         code_lines.append(
-                    f'{indent}with my_process_map.add_lane("{lane_name}") as lane{lane_id}:'
-                )
-    
+            f'{indent}with my_process_map.add_lane("{lane_name}") as lane{lane_id}:'
+        )
 
     indent += " " * 4
     return indent, lane_id
 
+
 def parse_pool(code_lines, pool_id, line):
+    """
+    This function parses a line of code to extract a pool name and adds it to a list of code lines with
+    a specific format.
+    """
     pool_name = line.split(":")[1].strip()
     indent = " " * 4
     code_lines.append(
-                f'{indent}with my_process_map.add_pool("{pool_name}") as pool{pool_id}:'
-            )
+        f'{indent}with my_process_map.add_pool("{pool_name}") as pool{pool_id}:'
+    )
     pool_id += 1
     pool_found = True
     return pool_found, pool_id
 
+
 def parse_connection(input_str, code_lines):
+    """
+    The function parses a string input containing connection information and generates code lines to
+    establish those connections in Python.
+    """
     connections_list = [
         line.split("->") for line in input_str.strip().split("\n") if "->" in line
     ]
 
     for connection in connections_list:
-        
-        print (f"connection {connection}")
-        
         for i in range(len(connection) - 1):
-            print (f"   [{connection[i]}]")
-            element_name, label = get_element_name_and_label(connection[i])
-            target_element_name, target_label = get_element_name_and_label(connection[i + 1])
+            element_name, label = get_element_name_and_label(connection[i].strip())
+            target_element_name, target_label = get_element_name_and_label(
+                connection[i + 1].strip()
+            )
             if label:
-                print (f"       {element_name}, label {label}")
-                code_lines.append(f'        {element_name}.connect({target_element_name}, "{label}")')
+                code_lines.append(
+                    f'        {element_name}.connect({target_element_name}, "{label}")'
+                )
             else:
-                code_lines.append(f"        {element_name}.connect({target_element_name})")
+                code_lines.append(
+                    f"        {element_name}.connect({target_element_name})"
+                )
+
 
 def get_element_name_and_label(connection: str):
-    #pattern = r'(\w+)-\|(.*?)\|'
-    pattern = r'(\w+)-\"(.*?)\"'
-    result = re.search(pattern, connection)
-    if result:
-        return result.group(1), result.group(2)
+    """
+    The function extracts the element name and label from a given connection string using regular
+    expressions.
+    """
+    pattern = r"(\w+)-\"(.*?)\""
+    if result := re.search(pattern, connection):
+        return result[1], result[2]
     else:
         return connection, None
 
+
 def parse_colour_theme(lines):
-    colour_theme = None
-    if "colourtheme" in lines[0]:
-        colour_theme = lines.pop(0).split(":")[1].strip()
-    return colour_theme
+    """
+    The function extracts the color theme from a list of lines if it exists.
+    """
+    return lines.pop(0).split(":")[1].strip() if "colourtheme" in lines[0] else None
+
 
 def parse_title(lines):
+    """
+    The function extracts the title from a list of lines if the first line contains the word "title".
+    """
     if "title" in lines[0]:
         process_map_title = lines.pop(0).split(":")[1].strip()
     else:
         raise ValueError("The first line must contain the word 'title'.")
     return process_map_title
 
 
 def parse_lane_element(element_str):
+    """
+    The function parses a string representing a BPMN element and returns its type, name, and variable
+    name.
+    """
     """Detect element type"""
     ### EventType
     if element_str.startswith("(start)"):
         element_type = "EventType.START"
         element_name = element_str[1 : element_str.index(")")].strip()
     elif element_str.startswith("(end)"):
         element_type = "EventType.END"
@@ -168,12 +213,41 @@
         raise ValueError(f"Invalid element string: {element_str}")
 
     element_var = element_str.split(" as ")[1].strip()
 
     return element_type, element_name, element_var
 
 
-def render(text: str, png_output_file: str = "diagram.png"):
+def show_code_with_line_number(code: str):
+    """
+    The function takes a string of code and prints it with line numbers.
+    """
+    print("Generated code: ")
+    for i, line in enumerate(code.split("\n")):
+        print(f"{i+1:3} {line}")
+
+
+def validate_generated_code(code: str):
+    if "add_lane" not in code:
+        raise ValueError("There is no lane defined. Please add lanes to process map.")
+
+    ### If a multiline code does not contain add_element, raise error
+    if "add_element" not in code:
+        raise ValueError("There is no element defined. Please add elements to lane.")
+
+
+def render(text: str, png_output_file: str = ""):
     """Render text to diagram"""
+    if png_output_file.strip() == "":
+        # add datetime to the file name
+        png_output_file = (
+            f"piper_{datetime.datetime.now().strftime('%Y%m%d_%H%M%S')}.png"
+        )
+
     generated_code = parse_and_generate_code(text, png_output_file)
-    print(generated_code)
+    validate_generated_code(generated_code)
+    # show_code_with_line_number(generated_code)
+    # print(generated_code)
     exec(generated_code)
+    generated_image = Image.open(png_output_file)
+
+    return generated_code, generated_image
```

### Comparing `processpiper-0.2.0/src/processpiper/title.py` & `processpiper-0.3.0/src/processpiper/title.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.2.0/src/processpiper/version.py` & `processpiper-0.3.0/src/processpiper/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Version information for processpiper."""
-__version__ = "v0.2.0"
+__version__ = "v0.3.0"
```

### Comparing `processpiper-0.2.0/src/processpiper.egg-info/PKG-INFO` & `processpiper-0.3.0/src/processpiper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: processpiper
-Version: 0.2.0
+Version: 0.3.0
 Summary: Processpiper. An open source python library to generate business process diagram using code.
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/processpiper
 Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![release](https://img.shields.io/pypi/v/processpiper?style=plastic)
 ![Wheel](https://img.shields.io/pypi/wheel/processpiper?style=plastic)
+![Downloads](https://img.shields.io/pypi/dm/processpiper?style=plastic)
 ![Platforms](https://img.shields.io/badge/Platform%3A-win%20%7C%20ubuntu%20%7C%20osx-brightgreen?style=plastic)
 [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=plastic)](https://en.wikipedia.org/wiki/MIT_License)
 [![CodeFactor](https://www.codefactor.io/repository/github/csgoh/processpiper/badge?style=plastic)](https://www.codefactor.io/repository/github/csgoh/processpiper)
 ![code size](https://img.shields.io/github/languages/code-size/csgoh/processmapper?style=plastic)
 ![python version](https://img.shields.io/pypi/pyversions/processpiper?style=plastic)
 ![stars](https://img.shields.io/github/stars/csgoh/processpiper?style=plastic)
 [![Twitter Follow](https://img.shields.io/twitter/follow/CSGohNZ?style=social)](https://twitter.com/CSGohNZ)
@@ -141,23 +142,18 @@
 ```
 
 The generated diagram is as follows:
 ![Process Map](https://github.com/csgoh/processpiper/blob/main/images/test/test_auto_case1.png)
 
 
 ## Development Status
-First version 0.1.0 is released. This release would only cover the following basic business process elements. Other element types will be introduced in subsequence releases.
+Initial first release would only cover the following basic business process elements. Other element types will be introduced in subsequence releases.
 
 * Event: Start, End, Timer, Intermediate
 * Activity: Task, Subprocess
 * Gateway: Inclusive, Exclusive, Parallel
 
 Any ideas or suggestions, please send it to me via [GitHub Discussions](https://github.com/csgoh/processmapper/discussions).
 
 
-Thank you for checking out my project. If you have found ProcessPiper useful and would like to show your appreciation, consider buying me a coffee or flat white :coffee: and keep me going. To buy me a coffee, simply follow this link: 
-
-<a href="https://www.buymeacoffee.com/csgoh" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
-
-
```

### Comparing `processpiper-0.2.0/src/processpiper.egg-info/SOURCES.txt` & `processpiper-0.3.0/src/processpiper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processpiper-0.2.0/src/tests/github_action_test.py` & `processpiper-0.3.0/src/tests/github_action_test.py`

 * *Files identical despite different names*

