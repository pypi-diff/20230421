# Comparing `tmp/voronoi-diagram-for-polygons-0.1.3.tar.gz` & `tmp/voronoi-diagram-for-polygons-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voronoi-diagram-for-polygons-0.1.3.tar", last modified: Thu Nov 17 03:37:40 2022, max compression
+gzip compressed data, was "voronoi-diagram-for-polygons-0.1.6.tar", last modified: Fri Apr 21 07:18:25 2023, max compression
```

## Comparing `voronoi-diagram-for-polygons-0.1.3.tar` & `voronoi-diagram-for-polygons-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 bruce     (1000) bruce     (1000)        0 2022-11-17 03:37:40.057662 voronoi-diagram-for-polygons-0.1.3/
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)     1091 2020-07-31 21:47:37.000000 voronoi-diagram-for-polygons-0.1.3/LICENSE
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)     7157 2022-11-17 03:37:40.057662 voronoi-diagram-for-polygons-0.1.3/PKG-INFO
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)     6780 2022-11-17 03:34:11.000000 voronoi-diagram-for-polygons-0.1.3/README.md
-drwxrwxrwx   0 bruce     (1000) bruce     (1000)        0 2022-11-17 03:37:39.988653 voronoi-diagram-for-polygons-0.1.3/longsgis/
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)      152 2022-11-17 02:22:59.000000 voronoi-diagram-for-polygons-0.1.3/longsgis/__init__.py
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)     6049 2022-11-17 03:28:31.000000 voronoi-diagram-for-polygons-0.1.3/longsgis/longsgis.py
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)       38 2022-11-17 03:37:40.057662 voronoi-diagram-for-polygons-0.1.3/setup.cfg
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)      828 2022-11-17 02:23:36.000000 voronoi-diagram-for-polygons-0.1.3/setup.py
-drwxrwxrwx   0 bruce     (1000) bruce     (1000)        0 2022-11-17 03:37:40.035532 voronoi-diagram-for-polygons-0.1.3/voronoi_diagram_for_polygons.egg-info/
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)     7157 2022-11-17 03:37:39.000000 voronoi-diagram-for-polygons-0.1.3/voronoi_diagram_for_polygons.egg-info/PKG-INFO
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)      327 2022-11-17 03:37:39.000000 voronoi-diagram-for-polygons-0.1.3/voronoi_diagram_for_polygons.egg-info/SOURCES.txt
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)        1 2022-11-17 03:37:39.000000 voronoi-diagram-for-polygons-0.1.3/voronoi_diagram_for_polygons.egg-info/dependency_links.txt
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)       34 2022-11-17 03:37:39.000000 voronoi-diagram-for-polygons-0.1.3/voronoi_diagram_for_polygons.egg-info/requires.txt
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)        9 2022-11-17 03:37:39.000000 voronoi-diagram-for-polygons-0.1.3/voronoi_diagram_for_polygons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:18:25.059480 voronoi-diagram-for-polygons-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 07:18:13.000000 voronoi-diagram-for-polygons-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-21 07:18:25.059480 voronoi-diagram-for-polygons-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-04-21 07:18:13.000000 voronoi-diagram-for-polygons-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:18:25.059480 voronoi-diagram-for-polygons-0.1.6/longsgis/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-21 07:18:13.000000 voronoi-diagram-for-polygons-0.1.6/longsgis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-21 07:18:13.000000 voronoi-diagram-for-polygons-0.1.6/longsgis/longsgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 07:18:25.059480 voronoi-diagram-for-polygons-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-21 07:18:13.000000 voronoi-diagram-for-polygons-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:18:25.059480 voronoi-diagram-for-polygons-0.1.6/voronoi_diagram_for_polygons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-21 07:18:25.000000 voronoi-diagram-for-polygons-0.1.6/voronoi_diagram_for_polygons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-21 07:18:25.000000 voronoi-diagram-for-polygons-0.1.6/voronoi_diagram_for_polygons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 07:18:25.000000 voronoi-diagram-for-polygons-0.1.6/voronoi_diagram_for_polygons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 07:18:25.000000 voronoi-diagram-for-polygons-0.1.6/voronoi_diagram_for_polygons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 07:18:25.000000 voronoi-diagram-for-polygons-0.1.6/voronoi_diagram_for_polygons.egg-info/top_level.txt
```

### Comparing `voronoi-diagram-for-polygons-0.1.3/LICENSE` & `voronoi-diagram-for-polygons-0.1.6/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 longavailable
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 longavailable
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `voronoi-diagram-for-polygons-0.1.3/PKG-INFO` & `voronoi-diagram-for-polygons-0.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voronoi-diagram-for-polygons
-Version: 0.1.3
+Version: 0.1.6
 Summary: A tool to create Voronoi diagram for polygons.
 Home-page: https://github.com/longavailable/voronoi-diagram-for-polygons
 Author: Xiaolong "Bruce" Liu, Meixiu Yu
 Author-email: liuxiaolong125@gmail.com, meixiuyu@hhu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,27 +19,28 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/voronoi-diagram-for-polygons)
 [![Downloads](https://pepy.tech/badge/voronoi-diagram-for-polygons)](https://pepy.tech/project/voronoi-diagram-for-polygons)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3960407.svg)](https://doi.org/10.5281/zenodo.3960407)
 
 [Voronoi diagram for polygons] is a tool to create a [Voronoi diagram] also known as [Thiessen polygons] for **polygons**. It's based on [Shapely] and [GeoPandas]. There are lots of tools to create a [Voronoi diagram] for points, for example [Create Thiessen Polygons (Analysis)] in [ArcGIS Pro] or [ArcGIS Desktop], [Voronoi Polygons] in [QGIS], or [voronoi_diagram] in [Shapely]. All of them are really cool. How about a [Voronoi diagram] for polygons? That's what this tool does.
 
 <p float="left">
-<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/inputs.png"/>
-<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/outputs.png"/>
+<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/inputs.png"/>
+<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/outputs.png"/>
 </p>
 
 [***Important!***](#dependencies) You have to install or upgrade to the latest developing version of [Shapely] before install [Voronoi diagram for polygons]
 
 ## Table of contents
 - [Installation, update and uninstallation](#installation--update-and-uninstallation)
 	* [Dependencies](#dependencies)
   * [To install](#to-install)
   * [To update](#to-update)
   * [To uninstall](#to-uninstall)
 - [Usage](#usage)
+- [FAQ](#faq)
 - [Known shortages](#known-shortages)
 - [How to cite?](#how-to-cite)
 - [Changelog](#changelog)
 
 ## Installation, update and uninstallation
 
 ### Dependencies
@@ -87,25 +88,37 @@
 
 builtup = gpd.read_file('input.geojson'); builtup.crs = 32650
 boundary = gpd.read_file('boundary.geojson'); boundary.crs = 32650
 vd = voronoiDiagram4plg(builtup, boundary)
 vd.to_file('output.geojson', driver='GeoJSON')
 ```
 
+## FAQ
+
+- I/O support.
+
+	It was noticed someone were struggled with the input/output files with a format of `.geojson` (https://github.com/longavailable/voronoi-diagram-for-polygons/issues/3, https://github.com/longavailable/voronoi-diagram-for-polygons/issues/5). Actually, that's not a question related to this package. I will explain more here about it. This package is totally based on [GeoPandas]. In other words, any format that can be converted to `geopandas.GeoDataFrame` object is supported. As the [official documentation](https://geopandas.org/en/stable/docs/user_guide/io.html#reading-spatial-data) said:
+
+	> geopandas can read almost any vector-based spatial data format including ESRI shapefile, GeoJSON files and more using the command: `geopandas.read_file()`
+	
+	That means, you can put your `.shp` files as inputs and output as well. Any format you'd like. I used a few geojson-s (`input.geojson`, `boundary.geojson`, and `output.geojson`) in my example because the geojson format is very open. However, it's NOT necessary.
+	
+	For more, I upload the [input.geojson] and [boundary.geojson] files. Hope they helps. For the sake of caution, I declare here that they are only a test file, any actual geographical data, similar or not, I have no guarantee to the accuracy and authenticity for them.
+
 ## Known shortages
 
 - It may produce multipolygons (consisted by some unconnected polygons) around the boundary.
 
-	<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/bug001.png"/>
+	<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/bug001.png"/>
 
 - Special input may cause overlap. See the following:
 
 	<p float="left">
-	<img width="300" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/bug002_input.png"/>
-	<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/bug002_output.png"/>
+	<img width="300" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/bug002_input.png"/>
+	<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/bug002_output.png"/>
 	</p>
 	
 	*To avoid this, I recommend reasonable preprocessing of the input, but use a buffer operation with high-resolution carefully.* A buffer operation with high-resolution will result in circular arcs, which will generate too many vertices in a local area. This may trigger other bugs. In my practices, the following code snippet worked well.
 	
 ```python
 def bufferDissolve(gdf, distance, join_style=3):	
 	'''Create buffer and dissolve thoese intersects.
@@ -150,21 +163,28 @@
 - Fix a [FutureWarning](https://pandas.pydata.org/docs/whatsnew/v1.4.0.html#whatsnew-140-deprecations-frame-series-append).
 
 ### v0.1.3
 
 - Make it more robust for the less-vertice-geometry inputs. [#4](https://github.com/longavailable/voronoi-diagram-for-polygons/issues/4#issue-1378217062).
 - Fix a few ***FutureWarnings***.
 
+### v0.1.6 (Merged)
+
+- Change as [Shapely] goes. `MultiPolygon` is not iterable any more from [Shapely] 2.0.
+- Upload a few test data.
+
 [Voronoi diagram for polygons]: https://github.com/longavailable/voronoi-diagram-for-polygons
 [Voronoi diagram]: https://en.wikipedia.org/wiki/Voronoi_diagram
 [Thiessen polygons]: https://en.wikipedia.org/wiki/Voronoi_diagram
 [Shapely]: https://shapely.readthedocs.io/en/latest/
 [GeoPandas]: https://geopandas.org/index.html
 [Create Thiessen Polygons (Analysis)]: https://pro.arcgis.com/en/pro-app/tool-reference/analysis/create-thiessen-polygons.htm
 [ArcGIS Pro]: https://www.esri.com/en-us/arcgis/products/arcgis-pro/overview
 [ArcGIS Desktop]: https://desktop.arcgis.com/en/
 [Voronoi polygons]: https://docs.qgis.org/3.10/en/docs/user_manual/processing_algs/qgis/vectorgeometry.html#voronoi-polygons
 [QGIS]: https://qgis.org/en/site/
 [voronoi_diagram]: https://shapely.readthedocs.io/en/latest/manual.html?#voronoi-diagram
-[longsgis/longsgis.py]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/longsgis/longsgis.py
-[tests/01voronoiDiagram4plg.py]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/tests/01voronoiDiagram4plg.py
+[longsgis/longsgis.py]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/longsgis/longsgis.py
+[tests/01voronoiDiagram4plg.py]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/tests/01voronoiDiagram4plg.py
+[input.geojson]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/tests/input.geojson
+[boundary.geojson]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/tests/boundary.geojson
```

### Comparing `voronoi-diagram-for-polygons-0.1.3/README.md` & `voronoi-diagram-for-polygons-0.1.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,156 +1,176 @@
-                             
-# Voronoi diagram for polygons
-
-[![PyPI version](https://badge.fury.io/py/voronoi-diagram-for-polygons.svg)](https://badge.fury.io/py/voronoi-diagram-for-polygons)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/voronoi-diagram-for-polygons)
-[![Downloads](https://pepy.tech/badge/voronoi-diagram-for-polygons)](https://pepy.tech/project/voronoi-diagram-for-polygons)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3960407.svg)](https://doi.org/10.5281/zenodo.3960407)
-
-[Voronoi diagram for polygons] is a tool to create a [Voronoi diagram] also known as [Thiessen polygons] for **polygons**. It's based on [Shapely] and [GeoPandas]. There are lots of tools to create a [Voronoi diagram] for points, for example [Create Thiessen Polygons (Analysis)] in [ArcGIS Pro] or [ArcGIS Desktop], [Voronoi Polygons] in [QGIS], or [voronoi_diagram] in [Shapely]. All of them are really cool. How about a [Voronoi diagram] for polygons? That's what this tool does.
-
-<p float="left">
-<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/inputs.png"/>
-<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/outputs.png"/>
-</p>
-
-[***Important!***](#dependencies) You have to install or upgrade to the latest developing version of [Shapely] before install [Voronoi diagram for polygons]
-
-## Table of contents
-- [Installation, update and uninstallation](#installation--update-and-uninstallation)
-	* [Dependencies](#dependencies)
-  * [To install](#to-install)
-  * [To update](#to-update)
-  * [To uninstall](#to-uninstall)
-- [Usage](#usage)
-- [Known shortages](#known-shortages)
-- [How to cite?](#how-to-cite)
-- [Changelog](#changelog)
-
-## Installation, update and uninstallation
-
-### Dependencies
-
-***Important!*** It's based on `voronoi_diagram` from [Shapely] which is new in version 1.8.dev0. As of today, it is still a developing version. *(2020-07-26)* You have to install or upgrade to the latest developing version from source firstly:
-
-```bash
-pip install git+https://github.com/Toblerity/Shapely
-```
-
-```bash
-pip install --upgrade git+https://github.com/Toblerity/Shapely
-```
-
-### To install
-
-Quick installation with `pip`:
-```bash
-pip install voronoi-diagram-for-polygons
-```
-Or from github:
-```bash
-pip install git+https://github.com/longavailable/voronoi-diagram-for-polygons
-```
-Also, you can just copy related functions from *[longsgis/longsgis.py]* to your work.
-
-### To update
-
-```bash
-pip install --upgrade voronoi-diagram-for-polygons
-```
-
-### To uninstall
-
-```bash
-pip uninstall voronoi-diagram-for-polygons
-```
-
-## Usage
-
-See *[tests/01voronoiDiagram4plg.py]*.
-```python
-import geopandas as gpd
-from longsgis import voronoiDiagram4plg
-
-builtup = gpd.read_file('input.geojson'); builtup.crs = 32650
-boundary = gpd.read_file('boundary.geojson'); boundary.crs = 32650
-vd = voronoiDiagram4plg(builtup, boundary)
-vd.to_file('output.geojson', driver='GeoJSON')
-```
-
-## Known shortages
-
-- It may produce multipolygons (consisted by some unconnected polygons) around the boundary.
-
-	<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/bug001.png"/>
-
-- Special input may cause overlap. See the following:
-
-	<p float="left">
-	<img width="300" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/bug002_input.png"/>
-	<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/bug002_output.png"/>
-	</p>
-	
-	*To avoid this, I recommend reasonable preprocessing of the input, but use a buffer operation with high-resolution carefully.* A buffer operation with high-resolution will result in circular arcs, which will generate too many vertices in a local area. This may trigger other bugs. In my practices, the following code snippet worked well.
-	
-```python
-def bufferDissolve(gdf, distance, join_style=3):	
-	'''Create buffer and dissolve thoese intersects.
-	
-	Parameters:
-		gdf: 
-			Type: geopandas.GeoDataFrame
-		distance: radius of the buffer
-			Type: float
-	Returns:
-		gdf_bf: buffered and dissolved GeoDataFrame
-			Type: geopandas.GeoDataFrame
-	'''
-	#create buffer and dissolve by invoking `unary_union`
-	smp = gdf.buffer(distance, join_style).unary_union
-	#convert to GeoSeries and explode to single polygons
-	gs = gpd.GeoSeries([smp]).explode()
-	#convert to GeoDataFrame
-	gdf_bf = gpd.GeoDataFrame(geometry=gs, crs=gdf.crs).reset_index(drop=True)
-	return gdf_bf
-```
-
-## How to cite
-
-If this tool is useful to your research, 
-<a class="github-button" href="https://github.com/longavailable/voronoi-diagram-for-polygons" aria-label="Star longavailable/voronoi-diagram-for-polygons on GitHub">star</a> and cite it as below:
-```
-Xiaolong Liu, & Meixiu Yu. (2020, July 26). longavailable/voronoi-diagram-for-polygons. Zenodo. 
-http://doi.org/10.5281/zenodo.3960407
-```
-Easily, you can import it to 
-<a href="https://www.mendeley.com/import/?url=https://zenodo.org/record/3960407"><i class="fa fa-external-link"></i> Mendeley</a>.
-
-## Changelog
-
-### v0.1.1
-
-- First release.
-
-### v0.1.2
-
-- Fix a [FutureWarning](https://pandas.pydata.org/docs/whatsnew/v1.4.0.html#whatsnew-140-deprecations-frame-series-append).
-
-### v0.1.3
-
-- Make it more robust for the less-vertice-geometry inputs. [#4](https://github.com/longavailable/voronoi-diagram-for-polygons/issues/4#issue-1378217062).
-- Fix a few ***FutureWarnings***.
-
-[Voronoi diagram for polygons]: https://github.com/longavailable/voronoi-diagram-for-polygons
-[Voronoi diagram]: https://en.wikipedia.org/wiki/Voronoi_diagram
-[Thiessen polygons]: https://en.wikipedia.org/wiki/Voronoi_diagram
-[Shapely]: https://shapely.readthedocs.io/en/latest/
-[GeoPandas]: https://geopandas.org/index.html
-[Create Thiessen Polygons (Analysis)]: https://pro.arcgis.com/en/pro-app/tool-reference/analysis/create-thiessen-polygons.htm
-[ArcGIS Pro]: https://www.esri.com/en-us/arcgis/products/arcgis-pro/overview
-[ArcGIS Desktop]: https://desktop.arcgis.com/en/
-[Voronoi polygons]: https://docs.qgis.org/3.10/en/docs/user_manual/processing_algs/qgis/vectorgeometry.html#voronoi-polygons
-[QGIS]: https://qgis.org/en/site/
-[voronoi_diagram]: https://shapely.readthedocs.io/en/latest/manual.html?#voronoi-diagram
-[longsgis/longsgis.py]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/longsgis/longsgis.py
-[tests/01voronoiDiagram4plg.py]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/tests/01voronoiDiagram4plg.py
-
+                             
+# Voronoi diagram for polygons
+
+[![PyPI version](https://badge.fury.io/py/voronoi-diagram-for-polygons.svg)](https://badge.fury.io/py/voronoi-diagram-for-polygons)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/voronoi-diagram-for-polygons)
+[![Downloads](https://pepy.tech/badge/voronoi-diagram-for-polygons)](https://pepy.tech/project/voronoi-diagram-for-polygons)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3960407.svg)](https://doi.org/10.5281/zenodo.3960407)
+
+[Voronoi diagram for polygons] is a tool to create a [Voronoi diagram] also known as [Thiessen polygons] for **polygons**. It's based on [Shapely] and [GeoPandas]. There are lots of tools to create a [Voronoi diagram] for points, for example [Create Thiessen Polygons (Analysis)] in [ArcGIS Pro] or [ArcGIS Desktop], [Voronoi Polygons] in [QGIS], or [voronoi_diagram] in [Shapely]. All of them are really cool. How about a [Voronoi diagram] for polygons? That's what this tool does.
+
+<p float="left">
+<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/inputs.png"/>
+<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/outputs.png"/>
+</p>
+
+[***Important!***](#dependencies) You have to install or upgrade to the latest developing version of [Shapely] before install [Voronoi diagram for polygons]
+
+## Table of contents
+- [Installation, update and uninstallation](#installation--update-and-uninstallation)
+	* [Dependencies](#dependencies)
+  * [To install](#to-install)
+  * [To update](#to-update)
+  * [To uninstall](#to-uninstall)
+- [Usage](#usage)
+- [FAQ](#faq)
+- [Known shortages](#known-shortages)
+- [How to cite?](#how-to-cite)
+- [Changelog](#changelog)
+
+## Installation, update and uninstallation
+
+### Dependencies
+
+***Important!*** It's based on `voronoi_diagram` from [Shapely] which is new in version 1.8.dev0. As of today, it is still a developing version. *(2020-07-26)* You have to install or upgrade to the latest developing version from source firstly:
+
+```bash
+pip install git+https://github.com/Toblerity/Shapely
+```
+
+```bash
+pip install --upgrade git+https://github.com/Toblerity/Shapely
+```
+
+### To install
+
+Quick installation with `pip`:
+```bash
+pip install voronoi-diagram-for-polygons
+```
+Or from github:
+```bash
+pip install git+https://github.com/longavailable/voronoi-diagram-for-polygons
+```
+Also, you can just copy related functions from *[longsgis/longsgis.py]* to your work.
+
+### To update
+
+```bash
+pip install --upgrade voronoi-diagram-for-polygons
+```
+
+### To uninstall
+
+```bash
+pip uninstall voronoi-diagram-for-polygons
+```
+
+## Usage
+
+See *[tests/01voronoiDiagram4plg.py]*.
+```python
+import geopandas as gpd
+from longsgis import voronoiDiagram4plg
+
+builtup = gpd.read_file('input.geojson'); builtup.crs = 32650
+boundary = gpd.read_file('boundary.geojson'); boundary.crs = 32650
+vd = voronoiDiagram4plg(builtup, boundary)
+vd.to_file('output.geojson', driver='GeoJSON')
+```
+
+## FAQ
+
+- I/O support.
+
+	It was noticed someone were struggled with the input/output files with a format of `.geojson` (https://github.com/longavailable/voronoi-diagram-for-polygons/issues/3, https://github.com/longavailable/voronoi-diagram-for-polygons/issues/5). Actually, that's not a question related to this package. I will explain more here about it. This package is totally based on [GeoPandas]. In other words, any format that can be converted to `geopandas.GeoDataFrame` object is supported. As the [official documentation](https://geopandas.org/en/stable/docs/user_guide/io.html#reading-spatial-data) said:
+
+	> geopandas can read almost any vector-based spatial data format including ESRI shapefile, GeoJSON files and more using the command: `geopandas.read_file()`
+	
+	That means, you can put your `.shp` files as inputs and output as well. Any format you'd like. I used a few geojson-s (`input.geojson`, `boundary.geojson`, and `output.geojson`) in my example because the geojson format is very open. However, it's NOT necessary.
+	
+	For more, I upload the [input.geojson] and [boundary.geojson] files. Hope they helps. For the sake of caution, I declare here that they are only a test file, any actual geographical data, similar or not, I have no guarantee to the accuracy and authenticity for them.
+
+## Known shortages
+
+- It may produce multipolygons (consisted by some unconnected polygons) around the boundary.
+
+	<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/bug001.png"/>
+
+- Special input may cause overlap. See the following:
+
+	<p float="left">
+	<img width="300" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/bug002_input.png"/>
+	<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/bug002_output.png"/>
+	</p>
+	
+	*To avoid this, I recommend reasonable preprocessing of the input, but use a buffer operation with high-resolution carefully.* A buffer operation with high-resolution will result in circular arcs, which will generate too many vertices in a local area. This may trigger other bugs. In my practices, the following code snippet worked well.
+	
+```python
+def bufferDissolve(gdf, distance, join_style=3):	
+	'''Create buffer and dissolve thoese intersects.
+	
+	Parameters:
+		gdf: 
+			Type: geopandas.GeoDataFrame
+		distance: radius of the buffer
+			Type: float
+	Returns:
+		gdf_bf: buffered and dissolved GeoDataFrame
+			Type: geopandas.GeoDataFrame
+	'''
+	#create buffer and dissolve by invoking `unary_union`
+	smp = gdf.buffer(distance, join_style).unary_union
+	#convert to GeoSeries and explode to single polygons
+	gs = gpd.GeoSeries([smp]).explode()
+	#convert to GeoDataFrame
+	gdf_bf = gpd.GeoDataFrame(geometry=gs, crs=gdf.crs).reset_index(drop=True)
+	return gdf_bf
+```
+
+## How to cite
+
+If this tool is useful to your research, 
+<a class="github-button" href="https://github.com/longavailable/voronoi-diagram-for-polygons" aria-label="Star longavailable/voronoi-diagram-for-polygons on GitHub">star</a> and cite it as below:
+```
+Xiaolong Liu, & Meixiu Yu. (2020, July 26). longavailable/voronoi-diagram-for-polygons. Zenodo. 
+http://doi.org/10.5281/zenodo.3960407
+```
+Easily, you can import it to 
+<a href="https://www.mendeley.com/import/?url=https://zenodo.org/record/3960407"><i class="fa fa-external-link"></i> Mendeley</a>.
+
+## Changelog
+
+### v0.1.1
+
+- First release.
+
+### v0.1.2
+
+- Fix a [FutureWarning](https://pandas.pydata.org/docs/whatsnew/v1.4.0.html#whatsnew-140-deprecations-frame-series-append).
+
+### v0.1.3
+
+- Make it more robust for the less-vertice-geometry inputs. [#4](https://github.com/longavailable/voronoi-diagram-for-polygons/issues/4#issue-1378217062).
+- Fix a few ***FutureWarnings***.
+
+### v0.1.6 (Merged)
+
+- Change as [Shapely] goes. `MultiPolygon` is not iterable any more from [Shapely] 2.0.
+- Upload a few test data.
+
+[Voronoi diagram for polygons]: https://github.com/longavailable/voronoi-diagram-for-polygons
+[Voronoi diagram]: https://en.wikipedia.org/wiki/Voronoi_diagram
+[Thiessen polygons]: https://en.wikipedia.org/wiki/Voronoi_diagram
+[Shapely]: https://shapely.readthedocs.io/en/latest/
+[GeoPandas]: https://geopandas.org/index.html
+[Create Thiessen Polygons (Analysis)]: https://pro.arcgis.com/en/pro-app/tool-reference/analysis/create-thiessen-polygons.htm
+[ArcGIS Pro]: https://www.esri.com/en-us/arcgis/products/arcgis-pro/overview
+[ArcGIS Desktop]: https://desktop.arcgis.com/en/
+[Voronoi polygons]: https://docs.qgis.org/3.10/en/docs/user_manual/processing_algs/qgis/vectorgeometry.html#voronoi-polygons
+[QGIS]: https://qgis.org/en/site/
+[voronoi_diagram]: https://shapely.readthedocs.io/en/latest/manual.html?#voronoi-diagram
+[longsgis/longsgis.py]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/longsgis/longsgis.py
+[tests/01voronoiDiagram4plg.py]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/tests/01voronoiDiagram4plg.py
+[input.geojson]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/tests/input.geojson
+[boundary.geojson]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/tests/boundary.geojson
+
```

### Comparing `voronoi-diagram-for-polygons-0.1.3/longsgis/longsgis.py` & `voronoi-diagram-for-polygons-0.1.6/longsgis/longsgis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,162 +1,166 @@
-# -*- coding: utf-8 -*-
-"""
-* Updated on 2022/11/17
-* python3
-**
-* Geoprocessing in Python
-"""
-import pandas as pd
-import geopandas as gpd
-import numpy as np
-from shapely.ops import voronoi_diagram as svd
-from shapely.geometry import Polygon, MultiPolygon
-import itertools, math
-
-def minimum_distance(gdf):
-	'''Calculate the minimum distance of all vertices of input geometries.
-	
-	Parameters:
-		gdf: polygons to be used
-			Type: geopandas.GeoDataFrame
-	Returns:
-		A float for the minimum distance.
-	'''
-	smp = gdf.unary_union	# convert to shapely.geometry.MultiPolygon
-	vertices = []
-	for g in smp.geoms:
-		coords = np.dstack(g.exterior.coords.xy).tolist()[0]	# vertices of each geometry
-		vertices = vertices + coords
-	potentials = list(itertools.combinations(vertices,2))	# pairs of vertices
-	all_distance = [math.sqrt((pp[0][0]-pp[1][0])**2+(pp[0][1]-pp[1][1])**2) for pp in potentials]	# calculate distance for each pair of vertices
-	nonzero_distance = [d for d in all_distance if d>0.0]	# drop zeros
-	return min(nonzero_distance)
-	
-def _pnts_on_line_(a, spacing=1, is_percent=False):  # densify by distance
-	"""Add points, at a fixed spacing, to an array representing a line.
-	Sourced from https://stackoverflow.com/a/65008592/12371819
-
-	**See**  `densify_by_distance` for documentation.
-
-	Parameters
-	----------
-	a : array
-		A sequence of `points`, x,y pairs, representing the bounds of a polygon
-		or polyline object.
-	spacing : number
-		Spacing between the points to be added to the line.
-	is_percent : boolean
-		Express the densification as a percent of the total length.
-
-	Notes
-	-----
-	Called by `pnt_on_poly`.
-	"""
-	N = len(a) - 1                                    # segments
-	dxdy = a[1:, :] - a[:-1, :]                       # coordinate differences
-	leng = np.sqrt(np.einsum('ij,ij->i', dxdy, dxdy))  # segment lengths
-	if is_percent:                                    # as percentage
-		spacing = abs(spacing)
-		spacing = min(spacing / 100, 1.)
-		steps = (sum(leng) * spacing) / leng          # step distance
-	else:
-		steps = leng / spacing                        # step distance
-	deltas = dxdy / (steps.reshape(-1, 1))            # coordinate steps
-	pnts = np.empty((N,), dtype='O')                  # construct an `O` array
-	for i in range(N):              # cycle through the segments and make
-		num = np.arange(steps[i])   # the new points
-		pnts[i] = np.array((num, num)).T * deltas[i] + a[i]
-	a0 = a[-1].reshape(1, -1)       # add the final point and concatenate
-	return np.concatenate((*pnts, a0), axis=0)
-
-def densify_polygon(gdf, spacing='auto'):
-	'''Densify the vertex along the edge of polygon(s).
-	
-	Parameters:
-		gdf: polygons to be used
-			Type: geopandas.GeoDataFrame
-		spacing: type or distance to be used
-			Type: string, int, or float
-	Returns:
-		A set of new polygon(s) with more vertices.
-		Type: geopandas.GeoDataFrame
-	'''
-	if isinstance(spacing, (str, float, int)):
-		if isinstance(spacing, str) and spacing.upper() == 'AUTO':
-			spacing = int(0.25 * minimum_distance(gdf))	# less than 0.5? The less, the better?
-		smp = gdf.unary_union	# convert to shapely.geometry.MultiPolygon
-		all_coords = []
-		for g in smp.geoms:
-			coords=np.dstack(g.exterior.coords.xy).tolist()	# vertices of each geometry
-			all_coords.append(*coords)
-			
-		polygons = []
-		for i, p in enumerate(all_coords):
-			new_polygon = Polygon(_pnts_on_line_(np.array(p),spacing=spacing))	# densify each polygon
-			polygons.append(new_polygon)
-		return gpd.GeoDataFrame({'geometry': polygons}, crs=gdf.crs)
-
-def voronoiDiagram4plg(gdf, mask, densify=False, spacing='auto'):
-	'''Create Voronoi diagram / Thiessen polygons based on polygons.
-	
-	Parameters:
-		gdf: polygons to be used to create Voronoi diagram
-			Type: geopandas.GeoDataFrame
-		mask: polygon vector used to clip the created Voronoi diagram
-			Type: GeoDataFrame, GeoSeries, (Multi)Polygon
-	Returns:
-		gdf_vd: Thiessen polygons
-			Type: geopandas.geodataframe.GeoDataFrame
-	'''
-	if densify: gdf = densify_polygon(gdf, spacing=spacing)
-	gdf.reset_index(drop=True)
-	#convert to shapely.geometry.MultiPolygon
-	smp = gdf.unary_union
-	#create primary voronoi diagram by invoking shapely.ops.voronoi_diagram (new in Shapely 1.8.dev0)
-	smp_vd = svd(smp)
-	#convert to GeoSeries and explode to single polygons
-	#note that it is NOT supported to GeoDataFrame directly
-	gs = gpd.GeoSeries([smp_vd]).explode(index_parts=True)
-	#convert to GeoDataFrame
-	#note that if gdf was shapely.geometry.MultiPolygon, it has no attribute 'crs'
-	gdf_vd_primary = gpd.geodataframe.GeoDataFrame(geometry=gs, crs=gdf.crs)
-	
-	#reset index
-	gdf_vd_primary.reset_index(drop=True)	#append(gdf)
-	#spatial join by intersecting and dissolve by `index_right`
-	gdf_temp = ( gpd.sjoin(gdf_vd_primary, gdf, how='inner', predicate='intersects')
-		.dissolve(by='index_right').reset_index(drop=True) )
-	gdf_vd = gpd.clip(gdf_temp, mask)
-	gdf_vd = dropHoles(gdf_vd)
-	return gdf_vd
-
-def dropHolesBase(plg):
-	'''Basic function to remove / drop / fill the holes.
-	
-	Parameters:
-		plg: plg who has holes / empties
-			Type: shapely.geometry.MultiPolygon or shapely.geometry.Polygon
-	Returns:
-		a shapely.geometry.MultiPolygon or shapely.geometry.Polygon object
-	'''
-	if isinstance(plg, MultiPolygon):
-		return MultiPolygon(Polygon(p.exterior) for p in plg)
-	elif isinstance(plg, Polygon):
-		return Polygon(plg.exterior)
-
-def dropHoles(gdf):
-	'''Remove / drop / fill the holes / empties for iterms in GeoDataFrame.
-	
-	Parameters:
-		gdf:
-			Type: geopandas.GeoDataFrame
-	Returns:
-		gdf_nohole: GeoDataFrame without holes
-			Type: geopandas.GeoDataFrame
-	'''
-	gdf_nohole = gpd.GeoDataFrame()
-	for g in gdf['geometry']:
-		geo = gpd.GeoDataFrame(geometry=gpd.GeoSeries(dropHolesBase(g)))
-		gdf_nohole=pd.concat([gdf_nohole, geo], ignore_index=True)
-	gdf_nohole.rename(columns={gdf_nohole.columns[0]:'geometry'}, inplace=True)
-	gdf_nohole.crs = gdf.crs
+# -*- coding: utf-8 -*-
+"""
+* Updated on 2023/04/17
+* python3
+**
+* Geoprocessing in Python
+"""
+import pandas as pd
+import geopandas as gpd
+import numpy as np
+import shapely
+from shapely.ops import voronoi_diagram as svd
+from shapely.geometry import Polygon, MultiPolygon
+import itertools, math
+
+def minimum_distance(gdf):
+	'''Calculate the minimum distance of all vertices of input geometries.
+	
+	Parameters:
+		gdf: polygons to be used
+			Type: geopandas.GeoDataFrame
+	Returns:
+		A float for the minimum distance.
+	'''
+	smp = gdf.unary_union	# convert to shapely.geometry.MultiPolygon
+	vertices = []
+	for g in smp.geoms:
+		coords = np.dstack(g.exterior.coords.xy).tolist()[0]	# vertices of each geometry
+		vertices = vertices + coords
+	potentials = list(itertools.combinations(vertices,2))	# pairs of vertices
+	all_distance = [math.sqrt((pp[0][0]-pp[1][0])**2+(pp[0][1]-pp[1][1])**2) for pp in potentials]	# calculate distance for each pair of vertices
+	nonzero_distance = [d for d in all_distance if d>0.0]	# drop zeros
+	return min(nonzero_distance)
+	
+def _pnts_on_line_(a, spacing=1, is_percent=False):  # densify by distance
+	"""Add points, at a fixed spacing, to an array representing a line.
+	Sourced from https://stackoverflow.com/a/65008592/12371819
+
+	**See**  `densify_by_distance` for documentation.
+
+	Parameters
+	----------
+	a : array
+		A sequence of `points`, x,y pairs, representing the bounds of a polygon
+		or polyline object.
+	spacing : number
+		Spacing between the points to be added to the line.
+	is_percent : boolean
+		Express the densification as a percent of the total length.
+
+	Notes
+	-----
+	Called by `pnt_on_poly`.
+	"""
+	N = len(a) - 1                                    # segments
+	dxdy = a[1:, :] - a[:-1, :]                       # coordinate differences
+	leng = np.sqrt(np.einsum('ij,ij->i', dxdy, dxdy))  # segment lengths
+	if is_percent:                                    # as percentage
+		spacing = abs(spacing)
+		spacing = min(spacing / 100, 1.)
+		steps = (sum(leng) * spacing) / leng          # step distance
+	else:
+		steps = leng / spacing                        # step distance
+	deltas = dxdy / (steps.reshape(-1, 1))            # coordinate steps
+	pnts = np.empty((N,), dtype='O')                  # construct an `O` array
+	for i in range(N):              # cycle through the segments and make
+		num = np.arange(steps[i])   # the new points
+		pnts[i] = np.array((num, num)).T * deltas[i] + a[i]
+	a0 = a[-1].reshape(1, -1)       # add the final point and concatenate
+	return np.concatenate((*pnts, a0), axis=0)
+
+def densify_polygon(gdf, spacing='auto'):
+	'''Densify the vertex along the edge of polygon(s).
+	
+	Parameters:
+		gdf: polygons to be used
+			Type: geopandas.GeoDataFrame
+		spacing: type or distance to be used
+			Type: string, int, or float
+	Returns:
+		A set of new polygon(s) with more vertices.
+		Type: geopandas.GeoDataFrame
+	'''
+	if isinstance(spacing, (str, float, int)):
+		if isinstance(spacing, str) and spacing.upper() == 'AUTO':
+			spacing = int(0.25 * minimum_distance(gdf))	# less than 0.5? The less, the better?
+		smp = gdf.unary_union	# convert to shapely.geometry.MultiPolygon
+		all_coords = []
+		for g in smp.geoms:
+			coords=np.dstack(g.exterior.coords.xy).tolist()	# vertices of each geometry
+			all_coords.append(*coords)
+			
+		polygons = []
+		for i, p in enumerate(all_coords):
+			new_polygon = Polygon(_pnts_on_line_(np.array(p),spacing=spacing))	# densify each polygon
+			polygons.append(new_polygon)
+		return gpd.GeoDataFrame({'geometry': polygons}, crs=gdf.crs)
+
+def voronoiDiagram4plg(gdf, mask, densify=False, spacing='auto'):
+	'''Create Voronoi diagram / Thiessen polygons based on polygons.
+	
+	Parameters:
+		gdf: polygons to be used to create Voronoi diagram
+			Type: geopandas.GeoDataFrame
+		mask: polygon vector used to clip the created Voronoi diagram
+			Type: GeoDataFrame, GeoSeries, (Multi)Polygon
+	Returns:
+		gdf_vd: Thiessen polygons
+			Type: geopandas.geodataframe.GeoDataFrame
+	'''
+	if densify: gdf = densify_polygon(gdf, spacing=spacing)
+	gdf.reset_index(drop=True)
+	#convert to shapely.geometry.MultiPolygon
+	smp = gdf.unary_union
+	#create primary voronoi diagram by invoking shapely.ops.voronoi_diagram (new in Shapely 1.8.dev0)
+	smp_vd = svd(smp)
+	#convert to GeoSeries and explode to single polygons
+	#note that it is NOT supported to GeoDataFrame directly
+	gs = gpd.GeoSeries([smp_vd]).explode(index_parts=True)
+	#convert to GeoDataFrame
+	#note that if gdf was shapely.geometry.MultiPolygon, it has no attribute 'crs'
+	gdf_vd_primary = gpd.geodataframe.GeoDataFrame(geometry=gs, crs=gdf.crs)
+	
+	#reset index
+	gdf_vd_primary.reset_index(drop=True)	#append(gdf)
+	#spatial join by intersecting and dissolve by `index_right`
+	gdf_temp = ( gpd.sjoin(gdf_vd_primary, gdf, how='inner', predicate='intersects')
+		.dissolve(by='index_right').reset_index(drop=True) )
+	gdf_vd = gpd.clip(gdf_temp, mask)
+	gdf_vd = dropHoles(gdf_vd)
+	return gdf_vd
+
+def dropHolesBase(plg):
+	'''Basic function to remove / drop / fill the holes.
+	
+	Parameters:
+		plg: plg who has holes / empties
+			Type: shapely.geometry.MultiPolygon or shapely.geometry.Polygon
+	Returns:
+		a shapely.geometry.MultiPolygon or shapely.geometry.Polygon object
+	'''
+	if isinstance(plg, MultiPolygon):
+		if shapely.__version__ < '2.0':
+			return MultiPolygon(Polygon(p.exterior) for p in plg)
+		else:
+			return MultiPolygon(Polygon(p.exterior) for p in plg.geoms)
+	elif isinstance(plg, Polygon):
+		return Polygon(plg.exterior)
+
+def dropHoles(gdf):
+	'''Remove / drop / fill the holes / empties for iterms in GeoDataFrame.
+	
+	Parameters:
+		gdf:
+			Type: geopandas.GeoDataFrame
+	Returns:
+		gdf_nohole: GeoDataFrame without holes
+			Type: geopandas.GeoDataFrame
+	'''
+	gdf_nohole = gpd.GeoDataFrame()
+	for g in gdf['geometry']:
+		geo = gpd.GeoDataFrame(geometry=gpd.GeoSeries(dropHolesBase(g)))
+		gdf_nohole=pd.concat([gdf_nohole, geo], ignore_index=True)
+	gdf_nohole.rename(columns={gdf_nohole.columns[0]:'geometry'}, inplace=True)
+	gdf_nohole.crs = gdf.crs
 	return gdf_nohole
```

### Comparing `voronoi-diagram-for-polygons-0.1.3/voronoi_diagram_for_polygons.egg-info/PKG-INFO` & `voronoi-diagram-for-polygons-0.1.6/voronoi_diagram_for_polygons.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voronoi-diagram-for-polygons
-Version: 0.1.3
+Version: 0.1.6
 Summary: A tool to create Voronoi diagram for polygons.
 Home-page: https://github.com/longavailable/voronoi-diagram-for-polygons
 Author: Xiaolong "Bruce" Liu, Meixiu Yu
 Author-email: liuxiaolong125@gmail.com, meixiuyu@hhu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,27 +19,28 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/voronoi-diagram-for-polygons)
 [![Downloads](https://pepy.tech/badge/voronoi-diagram-for-polygons)](https://pepy.tech/project/voronoi-diagram-for-polygons)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3960407.svg)](https://doi.org/10.5281/zenodo.3960407)
 
 [Voronoi diagram for polygons] is a tool to create a [Voronoi diagram] also known as [Thiessen polygons] for **polygons**. It's based on [Shapely] and [GeoPandas]. There are lots of tools to create a [Voronoi diagram] for points, for example [Create Thiessen Polygons (Analysis)] in [ArcGIS Pro] or [ArcGIS Desktop], [Voronoi Polygons] in [QGIS], or [voronoi_diagram] in [Shapely]. All of them are really cool. How about a [Voronoi diagram] for polygons? That's what this tool does.
 
 <p float="left">
-<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/inputs.png"/>
-<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/outputs.png"/>
+<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/inputs.png"/>
+<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/outputs.png"/>
 </p>
 
 [***Important!***](#dependencies) You have to install or upgrade to the latest developing version of [Shapely] before install [Voronoi diagram for polygons]
 
 ## Table of contents
 - [Installation, update and uninstallation](#installation--update-and-uninstallation)
 	* [Dependencies](#dependencies)
   * [To install](#to-install)
   * [To update](#to-update)
   * [To uninstall](#to-uninstall)
 - [Usage](#usage)
+- [FAQ](#faq)
 - [Known shortages](#known-shortages)
 - [How to cite?](#how-to-cite)
 - [Changelog](#changelog)
 
 ## Installation, update and uninstallation
 
 ### Dependencies
@@ -87,25 +88,37 @@
 
 builtup = gpd.read_file('input.geojson'); builtup.crs = 32650
 boundary = gpd.read_file('boundary.geojson'); boundary.crs = 32650
 vd = voronoiDiagram4plg(builtup, boundary)
 vd.to_file('output.geojson', driver='GeoJSON')
 ```
 
+## FAQ
+
+- I/O support.
+
+	It was noticed someone were struggled with the input/output files with a format of `.geojson` (https://github.com/longavailable/voronoi-diagram-for-polygons/issues/3, https://github.com/longavailable/voronoi-diagram-for-polygons/issues/5). Actually, that's not a question related to this package. I will explain more here about it. This package is totally based on [GeoPandas]. In other words, any format that can be converted to `geopandas.GeoDataFrame` object is supported. As the [official documentation](https://geopandas.org/en/stable/docs/user_guide/io.html#reading-spatial-data) said:
+
+	> geopandas can read almost any vector-based spatial data format including ESRI shapefile, GeoJSON files and more using the command: `geopandas.read_file()`
+	
+	That means, you can put your `.shp` files as inputs and output as well. Any format you'd like. I used a few geojson-s (`input.geojson`, `boundary.geojson`, and `output.geojson`) in my example because the geojson format is very open. However, it's NOT necessary.
+	
+	For more, I upload the [input.geojson] and [boundary.geojson] files. Hope they helps. For the sake of caution, I declare here that they are only a test file, any actual geographical data, similar or not, I have no guarantee to the accuracy and authenticity for them.
+
 ## Known shortages
 
 - It may produce multipolygons (consisted by some unconnected polygons) around the boundary.
 
-	<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/bug001.png"/>
+	<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/bug001.png"/>
 
 - Special input may cause overlap. See the following:
 
 	<p float="left">
-	<img width="300" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/bug002_input.png"/>
-	<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/docs/pics/bug002_output.png"/>
+	<img width="300" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/bug002_input.png"/>
+	<img width="150" height="150" src="https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/docs/pics/bug002_output.png"/>
 	</p>
 	
 	*To avoid this, I recommend reasonable preprocessing of the input, but use a buffer operation with high-resolution carefully.* A buffer operation with high-resolution will result in circular arcs, which will generate too many vertices in a local area. This may trigger other bugs. In my practices, the following code snippet worked well.
 	
 ```python
 def bufferDissolve(gdf, distance, join_style=3):	
 	'''Create buffer and dissolve thoese intersects.
@@ -150,21 +163,28 @@
 - Fix a [FutureWarning](https://pandas.pydata.org/docs/whatsnew/v1.4.0.html#whatsnew-140-deprecations-frame-series-append).
 
 ### v0.1.3
 
 - Make it more robust for the less-vertice-geometry inputs. [#4](https://github.com/longavailable/voronoi-diagram-for-polygons/issues/4#issue-1378217062).
 - Fix a few ***FutureWarnings***.
 
+### v0.1.6 (Merged)
+
+- Change as [Shapely] goes. `MultiPolygon` is not iterable any more from [Shapely] 2.0.
+- Upload a few test data.
+
 [Voronoi diagram for polygons]: https://github.com/longavailable/voronoi-diagram-for-polygons
 [Voronoi diagram]: https://en.wikipedia.org/wiki/Voronoi_diagram
 [Thiessen polygons]: https://en.wikipedia.org/wiki/Voronoi_diagram
 [Shapely]: https://shapely.readthedocs.io/en/latest/
 [GeoPandas]: https://geopandas.org/index.html
 [Create Thiessen Polygons (Analysis)]: https://pro.arcgis.com/en/pro-app/tool-reference/analysis/create-thiessen-polygons.htm
 [ArcGIS Pro]: https://www.esri.com/en-us/arcgis/products/arcgis-pro/overview
 [ArcGIS Desktop]: https://desktop.arcgis.com/en/
 [Voronoi polygons]: https://docs.qgis.org/3.10/en/docs/user_manual/processing_algs/qgis/vectorgeometry.html#voronoi-polygons
 [QGIS]: https://qgis.org/en/site/
 [voronoi_diagram]: https://shapely.readthedocs.io/en/latest/manual.html?#voronoi-diagram
-[longsgis/longsgis.py]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/longsgis/longsgis.py
-[tests/01voronoiDiagram4plg.py]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/master/tests/01voronoiDiagram4plg.py
+[longsgis/longsgis.py]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/longsgis/longsgis.py
+[tests/01voronoiDiagram4plg.py]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/tests/01voronoiDiagram4plg.py
+[input.geojson]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/tests/input.geojson
+[boundary.geojson]: https://github.com/longavailable/voronoi-diagram-for-polygons/raw/main/tests/boundary.geojson
```

