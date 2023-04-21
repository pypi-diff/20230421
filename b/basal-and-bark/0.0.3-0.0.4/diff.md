# Comparing `tmp/basal_and_bark-0.0.3.tar.gz` & `tmp/basal_and_bark-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basal_and_bark-0.0.3.tar", last modified: Wed Apr 12 16:41:41 2023, max compression
+gzip compressed data, was "basal_and_bark-0.0.4.tar", last modified: Fri Apr 21 19:24:09 2023, max compression
```

## Comparing `basal_and_bark-0.0.3.tar` & `basal_and_bark-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:41:41.125162 basal_and_bark-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 16:41:30.000000 basal_and_bark-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-12 16:41:30.000000 basal_and_bark-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-12 16:41:41.125162 basal_and_bark-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-12 16:41:30.000000 basal_and_bark-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:41:41.121163 basal_and_bark-0.0.3/basal_and_bark/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-12 16:41:30.000000 basal_and_bark-0.0.3/basal_and_bark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-04-12 16:41:30.000000 basal_and_bark-0.0.3/basal_and_bark/basal_and_bark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:41:41.125162 basal_and_bark-0.0.3/basal_and_bark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-12 16:41:41.000000 basal_and_bark-0.0.3/basal_and_bark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-12 16:41:41.000000 basal_and_bark-0.0.3/basal_and_bark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 16:41:41.000000 basal_and_bark-0.0.3/basal_and_bark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:41:41.000000 basal_and_bark-0.0.3/basal_and_bark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 16:41:41.000000 basal_and_bark-0.0.3/basal_and_bark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 16:41:41.000000 basal_and_bark-0.0.3/basal_and_bark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 16:41:30.000000 basal_and_bark-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-12 16:41:41.125162 basal_and_bark-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-12 16:41:30.000000 basal_and_bark-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:24:09.280096 basal_and_bark-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-21 19:23:56.000000 basal_and_bark-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-21 19:23:56.000000 basal_and_bark-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-21 19:24:09.280096 basal_and_bark-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-21 19:23:56.000000 basal_and_bark-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:24:09.280096 basal_and_bark-0.0.4/basal_and_bark/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-21 19:23:56.000000 basal_and_bark-0.0.4/basal_and_bark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-04-21 19:23:56.000000 basal_and_bark-0.0.4/basal_and_bark/basal_and_bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-21 19:23:56.000000 basal_and_bark-0.0.4/basal_and_bark/basal_and_bark_folium.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:24:09.280096 basal_and_bark-0.0.4/basal_and_bark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-21 19:24:09.000000 basal_and_bark-0.0.4/basal_and_bark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-21 19:24:09.000000 basal_and_bark-0.0.4/basal_and_bark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-21 19:24:09.000000 basal_and_bark-0.0.4/basal_and_bark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:24:09.000000 basal_and_bark-0.0.4/basal_and_bark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-21 19:24:09.000000 basal_and_bark-0.0.4/basal_and_bark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 19:24:09.000000 basal_and_bark-0.0.4/basal_and_bark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 19:23:57.000000 basal_and_bark-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-21 19:24:09.280096 basal_and_bark-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-21 19:23:57.000000 basal_and_bark-0.0.4/setup.py
```

### Comparing `basal_and_bark-0.0.3/LICENSE` & `basal_and_bark-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.3/PKG-INFO` & `basal_and_bark-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basal_and_bark
-Version: 0.0.3
+Version: 0.0.4
 Summary: Welcome to Basal and Bark, a spatial python package for working with forest data.
 Home-page: https://github.com/ZachDorm/basal_and_bark
 Author: Zach Dorminey
 Author-email: zach.dorminey@gmail.com
 License: MIT license
 Keywords: basal_and_bark
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `basal_and_bark-0.0.3/README.md` & `basal_and_bark-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.3/basal_and_bark/basal_and_bark.py` & `basal_and_bark-0.0.4/basal_and_bark/basal_and_bark.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Main module."""
 
 import string
 import random
 import ipyleaflet
 from ipyleaflet import GeoData, LayersControl, GeoJSON
-import folium
-from folium import TileLayer
+# import folium
+# from folium import TileLayer
 import xyzservices.providers as xyz
 
 import geopandas
 from geopandas import GeoDataFrame, GeoSeries
 
 def generate_random_string(length):
     """Generates a random string
@@ -125,23 +125,23 @@
     Args:
         map (basal_and_bark map): This will be the map that is being worked on
         data (any file type that is accepted by GeoData): Originally intended for vector files
 
     Returns:
         basal_and_bark map: basal_and_bark map with provided data added to it
     """    
-        try:
+        # try:
             #m = Map(center = [40,-100], zoom = 4, test = "test", scroll_wheel_zoom = True)
-            f = geopandas.read_file(data)
-            geo = GeoData(geo_dataframe=f, name="TN Counties")
-            self.add_layer(geo)
-            return self
+        f = geopandas.read_file(data)
+        geo = GeoData(geo_dataframe=f, name="TN Counties")
+        self.add_layer(geo)
+        return self
     
-        except:
-            return None
+        # except:
+        #     return None
         
 
     def add_geojson(self, data, **kwargs):
         try:
             #m = Map(center = [40,-100], zoom = 4, test = "test", scroll_wheel_zoom = True)
             self.add_shp(data)
             # f = geopandas.read_file(data)
@@ -157,44 +157,36 @@
 
         Args:
             data (vector data): Geopandas supported vector format.
 
         Returns:
             basal_and_bark map: basal_and_bark map with the vector data added.
         """     
-        count = 0
 
         try:
             self.add_shp(data)
         except:
-            count = count +1
-        try:
-            geo = GeoData(geo_dataframe=data, name="New Data")
-            self.add_layer(geo)
-        except:
-            count = count +1
 
-        try:
-            geo = GeoSeries(data=data, name="New Data")
-            self.add_layer(geo)
-        except:
-            count = count +1
+            try:
+                geo = GeoData(geo_dataframe=data, name="New Data")
+                self.add_layer(geo)
+            except:
+
+                try:
+                    geo = GeoSeries(data=data, name="New Data")
+                    self.add_layer(geo)
+                except:
         
-        try:
-            geo = GeoDataFrame(data=data, name="New Data")
-            self.add_layer(geo)
-        except:
-            count = count +1
+                    try:
+                        geo = GeoDataFrame(data=data, name="New Data")
+                        self.add_layer(geo)
+                    except:
 
-        if(count==3):
-            return "Not a supported file type"
-        else:
-            pass
-            #raise ValueError(f"Not found.")
-        #return self
+                        return "Not a supported file type"
+                    
 
     def add_basemap(self, url = xyz.Esri.WorldImagery.build_url(), basemap="Esri.WorldImagery", **kwargs):
         """Add a basemap from xyz.services
 
         Args:
             url (string, optional: URL to xyz.services map. Defaults to xyz.Esri.WorldImagery.build_url().
             basemap (str, optional): Name of the basemap on xyz.services. Defaults to "Esri.WorldImagery".
@@ -227,165 +219,55 @@
             name=name,
             attribution=attribution,
             **kwargs
         )
         self.add_layer(tile_layer)
 
 
-
-
-class Map_Folium(folium.Map):
-    """create the Map_Folium class of basal_and_bark
-
-    Args:
-        folium (Map): This is a folium Map instance upon which basal_and_bark's functionality is built on
-    """    
-    def __init__(self, location, tiles, zoom_start, **kwargs):
-        super().__init__(location=location, tiles=tiles, zoom_start=zoom_start, **kwargs)
-
-    def add_tile_layer_folium(self, url = xyz.Esri.WorldImagery.build_url(), name="", attribution="Esri.WorldImagery", **kwargs):
-        """Adds a tile layer to the map.
-        Args:
-            url (str): The URL of the tile layer.
-            name (str): The name of the tile layer.
-            attribution (str, optional): The attribution of the tile layer. Defaults to "".
-        """
-        tile_layer = folium.TileLayer(
-            tiles=url,
-            attr=attribution,
-            name=name,
-            **kwargs
-        )
-        tile_layer.add_to(self)
-
-    def add_basemap(self, url = xyz.Esri.WorldImagery.build_url(), basemap="Esri.WorldImagery", **kwargs):
-        """Add a basemap from xyz.services
-
-        Args:
-            url (string, optional: URL to xyz.services map. Defaults to xyz.Esri.WorldImagery.build_url().
-            basemap (str, optional): Name of the basemap on xyz.services. Defaults to "Esri.WorldImagery".
-
-        Raises:
-            ValueError: If basemap does not exist.
-
-        Returns:
-            basal_and_bark map_folium: basal_and_bark map_folium with new basemap
-        """        
-        try:
-            basemap = eval(f"xyz.{basemap}")
-            url = basemap.build_url()
-            attribution = basemap.attribution
-            b = self.add_tile_layer_folium(url, name = basemap.name, attribution=attribution, **kwargs)
-            return b
-
-        except:
-            raise ValueError(f"Basemap '{basemap}' not found.")
-
-
     def add_raster(self, url, name="raster", fit_bound = True, **kwargs):
-        """Adds a raster to the basal_and_bark map_folium
+        """Adds a raster to the basal_and_bark map
 
         Args:
             url (string): URL to raster you want to use.
             name (str, optional): Name of the raster. Defaults to "raster".
             fit_bound (bool, optional): Whether the bound of the map should be fit to the raster. Defaults to True.
         """        
         import httpx
         titiler_endpoint = "https://titiler.xyz"  # Developmentseed Demo endpoint. Please be kind
 
-        r = httpx.get(f"{titiler_endpoint}/cog/tilejson.json", params = {"url": url,}).json()
+        r = httpx.get(f"{titiler_endpoint}/cog/info", params = {"url": url,}).json()
         bounds = r["bounds"]
 
-        r = httpx.get(f"{titiler_endpoint}/cog/info", params = {"url": url,}).json()
+        r = httpx.get(f"{titiler_endpoint}/cog/tilejson.json", params = {"url": url,}).json()
         tile = r["tiles"][0]
+
+        bbox = [[bounds[1], bounds[0]], [bounds[3], bounds[2]]]
+        self.fit_bounds(bbox)
         self.add_tile_layer(url=tile, name=name, **kwargs)
 
-    def add_geojson_folium(self, data, **kwargs):
-        """Add GeoJSON to a map_folium
+    def add_image(self, url, **kwargs):
+        """Add a static image to the bottom right corner of a basal_and_bark map.
 
         Args:
-            data (GeoJSON file): GeoJSON
-
-        Returns:
-            basal_and_bark map_folium: basal_and_bark map_folium with provided data added to it
+            url (String): The url where the image to add is located.
         """        
-        try:
-            f = geopandas.read_file(data)
-            geo = folium.GeoJson(data=data, name="TN Counties")
-            m = geo.add_to(self)
-            return m
-    
-        except:
-            return None
-        
-
-    def add_shp_folium(self, data, **kwargs):
-        """Add a shapefile to a map_folium
-
-    Args:
-        map_folium (basal_and_bark map_folium): This will be the map that is being worked on
-        data (any file type that is accepted by GeoData): Originally intended for vector files
+        import ipywidgets as widgets
+        from ipyleaflet import WidgetControl
 
-    Returns:
-        basal_and_bark map_folium: basal_and_bark map_folium with provided data added to it
-    """  
-        data=data 
-        try:
-            f = geopandas.read_file(data)
-            geo = f["geometry"].simplify(tolerance=0.001)
-            json = geo.to_json()
-            geo_j = folium.GeoJson(data=json)
-            geo_j.add_to(self)
-        
-        #     for _, r in f.iterrows():
-        # # Without simplifying the representation of each borough,
-        # # the map might not be displayed
-        #      sim_geo = geopandas.GeoSeries(r['geometry'])#.simplify(tolerance=0.001)
-        #     geo_j = sim_geo.to_json()
-        #     geo_j = folium.GeoJson(data=geo_j)
-        #     geo_j.add_to(self)
-        # # geo = GeoData(geo_dataframe=f, name="TN Counties")
-        # # m = map.add_layer(geo)
-            self
-    
-        except:
-            None
-
-
-    def add_vector_folium(self, data, **kwargs):
-        """Accepts a file. Checks if it is a geopandas supported format. If not, then except silently.
-
-        Args:
-            data (vector data): Geopandas supported vector format.
+        output_widget = widgets.Output(layout={'border': '1px solid black'})
+        output_widget.clear_output()
+        output_control = WidgetControl(widget=output_widget, position='bottomright')
+        self.add_control(output_control)
+        logo = widgets.HTML(
+            value='<img src="https://wvstateparks.com/wp-content/uploads/2017/03/Ascend-WV-Brand-Photo-Coopers-Rock-State-Forest-Morgantown-scaled.jpg" width="200" height="200">'
+            )
+        with output_widget:
+            display(logo)
 
-        Returns:
-            basal_and_bark map_folium: basal_and_bark map_folium with the vector data added.
-        """        
-        count = 0
-
-        try:
-            self.add_shp_folium(data)
-        except:
-            count = count +1
-        try:
-            self.add_geojson_folium(data)
-        except:
-            count = count +1
-        
-        try:
-            json = data.to_json()
-            geo_j = folium.GeoJson(data=json)
-            geo_j.add_to(self)
-        except:
-            count = count +1
 
-        if(count==3):
-            return "Not a supported file type"
-        else:
-            pass
```

### Comparing `basal_and_bark-0.0.3/basal_and_bark.egg-info/PKG-INFO` & `basal_and_bark-0.0.4/basal_and_bark.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basal-and-bark
-Version: 0.0.3
+Version: 0.0.4
 Summary: Welcome to Basal and Bark, a spatial python package for working with forest data.
 Home-page: https://github.com/ZachDorm/basal_and_bark
 Author: Zach Dorminey
 Author-email: zach.dorminey@gmail.com
 License: MIT license
 Keywords: basal_and_bark
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `basal_and_bark-0.0.3/setup.py` & `basal_and_bark-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='basal_and_bark',
     name='basal_and_bark',
     packages=find_packages(include=['basal_and_bark', 'basal_and_bark.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ZachDorm/basal_and_bark',
-    version='0.0.3',
+    version='0.0.4',
     zip_safe=False,
 )
```

