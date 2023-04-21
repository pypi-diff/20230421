# Comparing `tmp/npp_materialslab_tools-0.0.3.tar.gz` & `tmp/npp_materialslab_tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npp_materialslab_tools-0.0.3.tar", last modified: Mon Mar 20 14:09:17 2023, max compression
+gzip compressed data, was "npp_materialslab_tools-0.0.4.tar", last modified: Fri Apr 21 14:26:08 2023, max compression
```

## Comparing `npp_materialslab_tools-0.0.3.tar` & `npp_materialslab_tools-0.0.4.tar`

### file list

```diff
@@ -1,47 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 14:09:17.059206 npp_materialslab_tools-0.0.3/
--rw-rw-rw-   0        0        0     2529 2023-03-20 14:09:17.058205 npp_materialslab_tools-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2129 2023-03-20 14:05:40.000000 npp_materialslab_tools-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 14:09:16.994657 npp_materialslab_tools-0.0.3/npp_materialslab_tools/
--rw-rw-rw-   0        0        0      134 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-20 14:09:17.012206 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dic/
--rw-rw-rw-   0        0        0        0 2023-03-06 12:01:34.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dic/__init__.py
--rw-rw-rw-   0        0        0     4655 2023-03-14 10:00:38.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dic/misc.py
--rw-rw-rw-   0        0        0    19359 2023-03-11 20:46:35.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dic/pydic.py
--rw-rw-rw-   0        0        0    20887 2023-03-11 20:46:35.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dic/pydicGrid.py
-drwxrwxrwx   0        0        0        0 2023-03-20 14:09:17.014211 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/
--rw-rw-rw-   0        0        0        0 2023-03-11 20:46:35.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-20 14:09:17.026204 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/tektronix_DMM4020/
--rw-rw-rw-   0        0        0      168 2023-03-20 14:05:40.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/tektronix_DMM4020/__init__.py
--rw-rw-rw-   0        0        0     2960 2023-03-20 14:05:40.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/tektronix_DMM4020/_basic_recording.py
--rw-rw-rw-   0        0        0     4189 2023-03-20 14:05:40.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/tektronix_DMM4020/_misc.py
--rw-rw-rw-   0        0        0     8626 2023-03-20 14:05:40.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/tektronix_DMM4020/monitorMeasurementClass.py
--rw-rw-rw-   0        0        0     8858 2023-03-20 14:05:40.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/tektronix_DMM4020/monitorMeasurementClassDummy.py
--rw-rw-rw-   0        0        0     6697 2023-03-20 14:05:40.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/tektronix_DMM4020/plot_util.py
--rw-rw-rw-   0        0        0      164 2023-03-20 14:05:40.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/tektronix_DMM4020/tekDMM4020.py
-drwxrwxrwx   0        0        0        0 2023-03-20 14:09:17.032206 npp_materialslab_tools-0.0.3/npp_materialslab_tools/plottools/
--rw-rw-rw-   0        0        0      285 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/plottools/__init__.py
--rw-rw-rw-   0        0        0     1042 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/plottools/cursor_crosshairs.py
--rw-rw-rw-   0        0        0     3836 2023-02-07 06:43:07.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/plottools/point_selector.py
--rw-rw-rw-   0        0        0     2708 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/plottools/point_selector2.py
-drwxrwxrwx   0        0        0        0 2023-03-20 14:09:17.049204 npp_materialslab_tools-0.0.3/npp_materialslab_tools/testing_machine/
--rw-rw-rw-   0        0        0      233 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/testing_machine/__init__.py
--rw-rw-rw-   0        0        0    11521 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/testing_machine/app_ElasticModGUI_v1.py
--rw-rw-rw-   0        0        0     8220 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/testing_machine/app_ElasticModGUI_v2.py
-drwxrwxrwx   0        0        0        0 2023-03-20 14:09:17.052205 npp_materialslab_tools-0.0.3/npp_materialslab_tools/testing_machine/imada/
--rw-rw-rw-   0        0        0        0 2023-03-11 20:46:35.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/testing_machine/imada/__init__.py
--rw-rw-rw-   0        0        0     1123 2023-03-11 20:46:35.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/testing_machine/imada/imada_tools.py
--rw-rw-rw-   0        0        0      475 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/testing_machine/specimen_classes.py
--rw-rw-rw-   0        0        0     2646 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/testing_machine/tensile_data.py
--rw-rw-rw-   0        0        0      349 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/testing_machine/test_appElasticityModulus.py
-drwxrwxrwx   0        0        0        0 2023-03-20 14:09:17.057205 npp_materialslab_tools-0.0.3/npp_materialslab_tools/tktools/
--rw-rw-rw-   0        0        0      103 2023-02-03 16:56:34.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/tktools/__init__.py
--rw-rw-rw-   0        0        0     4192 2023-02-03 16:15:33.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/tktools/tl_ImageProjection.py
--rw-rw-rw-   0        0        0     3780 2023-02-03 16:35:10.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools/tktools/tl_matplotlib_graph.py
-drwxrwxrwx   0        0        0        0 2023-03-20 14:09:17.006205 npp_materialslab_tools-0.0.3/npp_materialslab_tools.egg-info/
--rw-rw-rw-   0        0        0     2529 2023-03-20 14:09:16.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1741 2023-03-20 14:09:16.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 14:09:16.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-03-20 14:09:16.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-03-20 14:09:16.000000 npp_materialslab_tools-0.0.3/npp_materialslab_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-20 14:09:17.059206 npp_materialslab_tools-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1026 2023-03-20 14:08:18.000000 npp_materialslab_tools-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:26:08.520082 npp_materialslab_tools-0.0.4/
+-rw-rw-rw-   0        0        0     2529 2023-04-21 14:26:08.519084 npp_materialslab_tools-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2129 2023-03-21 07:17:12.000000 npp_materialslab_tools-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 14:26:08.450105 npp_materialslab_tools-0.0.4/npp_materialslab_tools/
+-rw-rw-rw-   0        0        0      134 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:26:08.476083 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dic/
+-rw-rw-rw-   0        0        0       97 2023-04-08 07:48:47.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dic/__init__.py
+-rw-rw-rw-   0        0        0     5718 2023-04-10 09:09:38.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dic/_pydic_support.py
+-rw-rw-rw-   0        0        0     9951 2023-04-10 09:09:38.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dic/dic_processor.py
+-rw-rw-rw-   0        0        0     6112 2023-04-13 12:02:54.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dic/misc.py
+-rw-rw-rw-   0        0        0     4394 2023-04-08 07:48:47.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dic/offset_selector.py
+-rw-rw-rw-   0        0        0    15940 2023-04-10 09:09:38.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dic/pydic.py
+-rw-rw-rw-   0        0        0    20887 2023-03-11 20:46:35.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dic/pydicGrid.py
+-rw-rw-rw-   0        0        0    16904 2023-04-21 13:08:28.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dic/pydic_processor.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:26:08.477082 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/
+-rw-rw-rw-   0        0        0        0 2023-03-11 20:46:35.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:26:08.488079 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/tektronix_DMM4020/
+-rw-rw-rw-   0        0        0      168 2023-03-21 07:18:39.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/tektronix_DMM4020/__init__.py
+-rw-rw-rw-   0        0        0     2960 2023-03-21 07:18:39.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/tektronix_DMM4020/_basic_recording.py
+-rw-rw-rw-   0        0        0     4189 2023-03-21 07:18:39.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/tektronix_DMM4020/_misc.py
+-rw-rw-rw-   0        0        0     8626 2023-03-21 07:18:39.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/tektronix_DMM4020/monitorMeasurementClass.py
+-rw-rw-rw-   0        0        0     8858 2023-03-21 07:18:39.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/tektronix_DMM4020/monitorMeasurementClassDummy.py
+-rw-rw-rw-   0        0        0     6697 2023-03-21 07:18:39.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/tektronix_DMM4020/plot_util.py
+-rw-rw-rw-   0        0        0      164 2023-03-21 07:18:39.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/tektronix_DMM4020/tekDMM4020.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:26:08.495082 npp_materialslab_tools-0.0.4/npp_materialslab_tools/plottools/
+-rw-rw-rw-   0        0        0      285 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/plottools/__init__.py
+-rw-rw-rw-   0        0        0     1042 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/plottools/cursor_crosshairs.py
+-rw-rw-rw-   0        0        0     3836 2023-02-07 06:43:07.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/plottools/point_selector.py
+-rw-rw-rw-   0        0        0     2708 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/plottools/point_selector2.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:26:08.504082 npp_materialslab_tools-0.0.4/npp_materialslab_tools/testing_machine/
+-rw-rw-rw-   0        0        0      233 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/testing_machine/__init__.py
+-rw-rw-rw-   0        0        0    11521 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/testing_machine/app_ElasticModGUI_v1.py
+-rw-rw-rw-   0        0        0     8220 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/testing_machine/app_ElasticModGUI_v2.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:26:08.507081 npp_materialslab_tools-0.0.4/npp_materialslab_tools/testing_machine/imada/
+-rw-rw-rw-   0        0        0        0 2023-03-11 20:46:35.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/testing_machine/imada/__init__.py
+-rw-rw-rw-   0        0        0     1123 2023-03-11 20:46:35.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/testing_machine/imada/imada_tools.py
+-rw-rw-rw-   0        0        0      475 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/testing_machine/specimen_classes.py
+-rw-rw-rw-   0        0        0     2646 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/testing_machine/tensile_data.py
+-rw-rw-rw-   0        0        0      349 2023-02-13 09:36:13.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/testing_machine/test_appElasticityModulus.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:26:08.512081 npp_materialslab_tools-0.0.4/npp_materialslab_tools/tktools/
+-rw-rw-rw-   0        0        0      103 2023-02-03 16:56:34.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/tktools/__init__.py
+-rw-rw-rw-   0        0        0     4192 2023-02-03 16:15:33.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/tktools/tl_ImageProjection.py
+-rw-rw-rw-   0        0        0     3780 2023-02-03 16:35:10.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools/tktools/tl_matplotlib_graph.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:26:08.463086 npp_materialslab_tools-0.0.4/npp_materialslab_tools.egg-info/
+-rw-rw-rw-   0        0        0     2529 2023-04-21 14:26:07.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2041 2023-04-21 14:26:07.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:26:07.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-21 14:26:07.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-21 14:26:07.000000 npp_materialslab_tools-0.0.4/npp_materialslab_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:26:08.520082 npp_materialslab_tools-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2023-04-21 14:22:52.000000 npp_materialslab_tools-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:26:08.513083 npp_materialslab_tools-0.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:58:34.000000 npp_materialslab_tools-0.0.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:26:08.518083 npp_materialslab_tools-0.0.4/tests/dic/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:58:34.000000 npp_materialslab_tools-0.0.4/tests/dic/__init__.py
+-rw-rw-rw-   0        0        0     5599 2023-04-10 09:09:38.000000 npp_materialslab_tools-0.0.4/tests/dic/test_dic_processor.py
+-rw-rw-rw-   0        0        0     7490 2023-04-21 13:42:18.000000 npp_materialslab_tools-0.0.4/tests/dic/test_image_displacement_processor.py
```

### Comparing `npp_materialslab_tools-0.0.3/PKG-INFO` & `npp_materialslab_tools-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npp_materialslab_tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for the material lab tools
 Home-page: 
 Author: N. Papadakis
 Author-email: npapnet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `npp_materialslab_tools-0.0.3/README.md` & `npp_materialslab_tools-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/dic/pydic.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/dic/pydic.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
 import cv2
 import numpy as np
 from matplotlib import pyplot as plt
 from matplotlib.widgets import Button, RadioButtons, Slider
 
 from .pydicGrid import grid, draw_opencv
+from ._pydic_support import compute_disp_and_remove_rigid_transform, compute_displacement, AreaSelector, remove_point_outside
 
 
 # logging.basicConfig(level=logging.DEBUG)
 
 
       
 def build_grid(area, num_point, *args, **kwargs):
@@ -87,17 +88,34 @@
          points (_type_): _description_
      """     
      result_file.write(image + '\t')
      for p in points:
           result_file.write(str(p[0]) + ',' + str(p[1]) + '\t')
      result_file.write('\n')
     
+
+# def remove_point_outside(points, area,  *args, **kwargs):
+#      shape = 'box' if not 'shape' in kwargs else kwargs['shape']
+#      # what is shape doing here?
+#      xmin = area[0][0]
+#      xmax = area[1][0]
+#      ymin = area[0][1]
+#      ymax = area[1][1]
+#      res = []
+#      for p in points:
+#           x = p[0]; y = p[1]
+#           if ((x >= xmin) and (x <= xmax) and (y >= ymin) and (y <= ymax)):
+#                res.append(p)
+#      return np.array(res)
+
+
+
 def init(image_pattern, win_size_px, grid_size_px, result_file, area_of_interest=None, *args, **kwargs):
      """the init function is a simple wrapper function that allows to parse a 
-sequence of images. The displacements are computed and a result file is written
+          sequence of images. The displacements are computed and a result file is written
 
      Args:
          image_pattern (str): the path and pattern describing where your image are located 
          win_size_px (list):  the size in pixel of your correlation windows.Given as a (dx, dy) tuple
          grid_size_px (list): the size of your correlation grid. Given as a (dx, dy) tuple
          result_file (str): the name of the result file
          area_of_interest (list of two tuples, optional): gives the area of interset in 
@@ -105,25 +123,25 @@
                  Defaults to None.
                          if you don't give this argument, a windows with the first image is displayed. 
                          You can pick in this picture manually your area of interest.
 
      Parsed kwargs:
           unstructured_grid=(val1,val2) : to let the 'goodFeaturesToTrack' opencv2 algorithm. Note that you can't use the 'spline' or the 'raw' interpolation method.
      """
-
-     
      img_list = sorted(glob.glob(image_pattern))
      assert len(img_list) > 1, "there is not image in " + str(image_pattern)
      img_ref = cv2.imread(img_list[0], 0)
      
      # choose area of interset 
      if (area_of_interest is None):
           print("please pick your area of interest on the picture")
           print("Press 'c' to proceed")
-          area_of_interest = pick_area_of_interest(img_ref)
+          # area_of_interest = pick_area_of_interest(img_ref)
+          areaSelector = AreaSelector(img_ref)
+          area_of_interest = areaSelector.pick_area_of_interest()
 
      # init correlation grid
      area     = area_of_interest
 
      points   = []
      points_x = np.float64(np.arange(area[0][0], area[1][0], grid_size_px[0]))
      points_y = np.float64(np.arange(area[0][1], area[1][1], grid_size_px[1]))
@@ -242,15 +260,16 @@
      scale_disp   = 4. if not 'scale_disp' in kwargs else float(kwargs['scale_disp'])
      scale_grid   = 25. if not 'scale_grid' in kwargs else float(kwargs['scale_grid'])
      strain_type  = 'cauchy' if not 'strain_type' in kwargs else kwargs['strain_type']
      rm_rigid_body_transform = True if not 'rm_rigid_body_transform' in kwargs else kwargs['rm_rigid_body_transform']
      
      # read meta info file
      meta_info = {}
-     if 'meta_info_file' in kwargs:
+     # if 'meta_info_file' in kwargs:
+     if  kwargs.get('meta_info_file', None) is not None:
           print('read meta info file', kwargs['meta_info_file'], '...')
           with open(kwargs['meta_info_file']) as f:
                lines = f.readlines()
                header = lines[0]
                field = header.split()
                for l in lines[1:-1]:
                     val = l.split()
@@ -318,159 +337,25 @@
           if (save_image):
                mygrid.draw_marker_img()
                mygrid.draw_disp_img(scale_disp)
                mygrid.draw_grid_img(scale_grid)
                if win_size_x == 1 and win_size_y == 1 : 
                     mygrid.draw_disp_hsv_img()
 
-          # write result file
-          mygrid.write_result()
+          if not kwargs.get("unit_test_mode", False):
+               # write result file
+               mygrid.write_result()
 
           # add meta info to grid if it exists
           if (len(meta_info) > 0):
                img = os.path.basename(mygrid.image)
                #if not meta_info.has_key(img):
                if img not in meta_info.keys():
                     print("warning, can't affect meta deta for image", img)
                else:
                     mygrid.add_meta_info(meta_info.get(img))
                     print('add meta info', meta_info.get(img))
      return grid_list
                     
           
 
-def compute_displacement(point, pointf):
-    """To compute a displacement between two point arrays"""
-    assert len(point)==len(pointf)
-    values = []
-    for i, pt0 in enumerate(point):
-        pt1 = pointf[i]
-        values.append((pt1[0]-pt0[0], pt1[1]-pt0[1]))
-    return values
-
-# TODO: Move those two into the pick_area_of_interest
-# this should remove the need for 
-area = []
-cropping = False # I don't see much use in the cropping flag. 
-
-def pick_area_of_interest(PreliminaryImage):
-     """used by init. Picks area of interest from an image
-     if data are not selected
-
-
-     Args:
-         PreliminaryImage (_type_): _description_
-
-     Returns:
-         _type_: _description_
-     """    
-     global area, cropping
-     image = cv2.putText(PreliminaryImage, "Pick the area of interest (left click + move mouse) and press 'c' button to continue", (50,50), cv2.FONT_HERSHEY_SIMPLEX, 1,(255,255,255),4)
-          
-     def click_and_crop(event, x, y, flags, param):
-          global area, cropping
-          if event == cv2.EVENT_LBUTTONDOWN:
-               area = [(x, y)]
-               cropping = True
-
-          elif event == cv2.EVENT_LBUTTONUP:
-               area.append((x, y))
-               cropping = False
-
-               # draw a rectangle around the region of interest
-               Newimage = cv2.rectangle(image, area[0], area[1], (0, 255, 0), 2)
-               cv2.imshow('image', Newimage)
-               
-     clone = image.copy()
-     cv2.namedWindow('image', cv2.WINDOW_NORMAL)
-     cv2.resizeWindow('image', image.shape[1], image.shape[0])
-     cv2.setMouseCallback("image", click_and_crop)
-
-     # keep looping until the 'c' key is pressed
-     while True:
-          # display the image and wait for a keypress
-          cv2.imshow("image", image)
-          key = cv2.waitKey(1) & 0xFF
-
-          # if the 'r' key is pressed, reset the cropping region
-          if key == ord("r"):
-               image = clone.copy()
-
-               # if the 'c' key is pressed, break from the loop
-          elif key == ord("c"):
-               print(f'The area of interest is {area}')
-               break
-     return area
-
-def remove_point_outside(points, area,  *args, **kwargs):
-     shape = 'box' if not 'shape' in kwargs else kwargs['shape']
-     # what is shape doing here?
-     xmin = area[0][0]; xmax = area[1][0]
-     ymin = area[0][1]; ymax = area[1][1]
-     res = []
-     for p in points:
-          x = p[0]; y = p[1]
-          if ((x >= xmin) and (x <= xmax) and (y >= ymin) and (y <= ymax)):
-               res.append(p)
-     return np.array(res)
-
-
-def compute_disp_and_remove_rigid_transform(p1, p2):
-     """_summary_
-
-     Args:
-         p1 (_type_): _description_
-         p2 (_type_): _description_
-
-     Returns:
-         _type_: _description_
-     """     
-     A = []
-     B = []
-     removed_indices = []
-     for i in range(len(p1)):
-          if np.isnan(p1[i][0]):
-               assert np.isnan(p1[i][0]) and np.isnan(p1[i][1]) and np.isnan(p2[i][0]) and np.isnan(p2[i][1])
-               removed_indices.append(i)
-          else:
-               A.append(p1[i])
-               B.append(p2[i])
-          
-     A = np.matrix(A)
-     B =  np.matrix(B)
-     assert len(A) == len(B)
-     N = A.shape[0]; # total points
-     
-     centroid_A = np.mean(A, axis=0)
-     centroid_B = np.mean(B, axis=0)
-    
-     # centre the points
-     AA = np.matrix(A - np.tile(centroid_A, (N, 1)))
-     BB = np.matrix(B - np.tile(centroid_B, (N, 1)))
-
-     # dot is matrix multiplication for array
-     H = np.transpose(AA) * BB
-     U, S, Vt = np.linalg.svd(H)
-     R = Vt.T * U.T
-
-     # special reflection case
-     if np.linalg.det(R) < 0:
-          print("Reflection detected")
-          Vt[2,:] *= -1
-          R = Vt.T * U.T
-
-     n = len(A)
-     T = -R*centroid_A.T + centroid_B.T
-     A2 = (R*A.T) + np.tile(T, (1, n))
-     A2 = np.array(A2.T)
-     out = []
-     j = 0
-     for i in range(len(p1)):
-          if np.isnan(p1[i][0]):
-               out.append(p1[i])
-          else:
-               out.append(A2[j])
-               j = j + 1
-     out = np.array(out)
-     return compute_displacement(p2, out)
-
```

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/dic/pydicGrid.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/dic/pydicGrid.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/tektronix_DMM4020/_basic_recording.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/tektronix_DMM4020/_basic_recording.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/tektronix_DMM4020/_misc.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/tektronix_DMM4020/_misc.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/tektronix_DMM4020/monitorMeasurementClass.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/tektronix_DMM4020/monitorMeasurementClass.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/tektronix_DMM4020/monitorMeasurementClassDummy.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/tektronix_DMM4020/monitorMeasurementClassDummy.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/dmm/tektronix_DMM4020/plot_util.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/dmm/tektronix_DMM4020/plot_util.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/plottools/cursor_crosshairs.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/plottools/cursor_crosshairs.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/plottools/point_selector.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/plottools/point_selector.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/plottools/point_selector2.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/plottools/point_selector2.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/testing_machine/app_ElasticModGUI_v1.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/testing_machine/app_ElasticModGUI_v1.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/testing_machine/app_ElasticModGUI_v2.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/testing_machine/app_ElasticModGUI_v2.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/testing_machine/imada/imada_tools.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/testing_machine/imada/imada_tools.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/testing_machine/tensile_data.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/testing_machine/tensile_data.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/tktools/tl_ImageProjection.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/tktools/tl_ImageProjection.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools/tktools/tl_matplotlib_graph.py` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools/tktools/tl_matplotlib_graph.py`

 * *Files identical despite different names*

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools.egg-info/PKG-INFO` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npp-materialslab-tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for the material lab tools
 Home-page: 
 Author: N. Papadakis
 Author-email: npapnet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `npp_materialslab_tools-0.0.3/npp_materialslab_tools.egg-info/SOURCES.txt` & `npp_materialslab_tools-0.0.4/npp_materialslab_tools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,21 @@
 npp_materialslab_tools/__init__.py
 npp_materialslab_tools.egg-info/PKG-INFO
 npp_materialslab_tools.egg-info/SOURCES.txt
 npp_materialslab_tools.egg-info/dependency_links.txt
 npp_materialslab_tools.egg-info/requires.txt
 npp_materialslab_tools.egg-info/top_level.txt
 npp_materialslab_tools/dic/__init__.py
+npp_materialslab_tools/dic/_pydic_support.py
+npp_materialslab_tools/dic/dic_processor.py
 npp_materialslab_tools/dic/misc.py
+npp_materialslab_tools/dic/offset_selector.py
 npp_materialslab_tools/dic/pydic.py
 npp_materialslab_tools/dic/pydicGrid.py
+npp_materialslab_tools/dic/pydic_processor.py
 npp_materialslab_tools/dmm/__init__.py
 npp_materialslab_tools/dmm/tektronix_DMM4020/__init__.py
 npp_materialslab_tools/dmm/tektronix_DMM4020/_basic_recording.py
 npp_materialslab_tools/dmm/tektronix_DMM4020/_misc.py
 npp_materialslab_tools/dmm/tektronix_DMM4020/monitorMeasurementClass.py
 npp_materialslab_tools/dmm/tektronix_DMM4020/monitorMeasurementClassDummy.py
 npp_materialslab_tools/dmm/tektronix_DMM4020/plot_util.py
@@ -28,8 +32,12 @@
 npp_materialslab_tools/testing_machine/specimen_classes.py
 npp_materialslab_tools/testing_machine/tensile_data.py
 npp_materialslab_tools/testing_machine/test_appElasticityModulus.py
 npp_materialslab_tools/testing_machine/imada/__init__.py
 npp_materialslab_tools/testing_machine/imada/imada_tools.py
 npp_materialslab_tools/tktools/__init__.py
 npp_materialslab_tools/tktools/tl_ImageProjection.py
-npp_materialslab_tools/tktools/tl_matplotlib_graph.py
+npp_materialslab_tools/tktools/tl_matplotlib_graph.py
+tests/__init__.py
+tests/dic/__init__.py
+tests/dic/test_dic_processor.py
+tests/dic/test_image_displacement_processor.py
```

### Comparing `npp_materialslab_tools-0.0.3/setup.py` & `npp_materialslab_tools-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     # 'pytest-pep8',
     # 'pytest-cov',
 ]
 
 
 setuptools.setup(
     name="npp_materialslab_tools", # Replace with your own username
-    version="0.0.3",
+    version="0.0.4",
     author="N. Papadakis",
     author_email="npapnet@gmail.com",
     description="A package for the material lab tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

