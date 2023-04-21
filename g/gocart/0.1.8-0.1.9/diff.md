# Comparing `tmp/gocart-0.1.8.tar.gz` & `tmp/gocart-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocart-0.1.8.tar", last modified: Thu Apr  6 16:57:24 2023, max compression
+gzip compressed data, was "gocart-0.1.9.tar", last modified: Wed Apr 19 15:03:34 2023, max compression
```

## Comparing `gocart-0.1.8.tar` & `gocart-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-06 16:57:24.471863 gocart-0.1.8/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      899 2023-04-06 16:52:44.000000 gocart-0.1.8/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-04-06 16:52:44.000000 gocart-0.1.8/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-04-06 16:52:44.000000 gocart-0.1.8/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5996 2023-04-06 16:57:24.467863 gocart-0.1.8/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5430 2023-04-06 16:52:44.000000 gocart-0.1.8/README.md
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-06 16:57:24.467863 gocart-0.1.8/gocart/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7204 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-06 16:57:24.467863 gocart-0.1.8/gocart/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1920 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/commonutils/flatten_healpix_map.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2956 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/commonutils/generate_skymap_stats.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/commonutils/getpackagepath.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-06 16:57:24.467863 gocart-0.1.8/gocart/convert/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/convert/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11081 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/convert/aitoff.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3293 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/convert/ascii.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/convert/healpix2cart.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2236 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/default_settings.yaml
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-06 16:57:24.467863 gocart-0.1.8/gocart/parsers/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/parsers/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6496 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/parsers/lvk.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2003 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/test_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-04-06 16:52:44.000000 gocart-0.1.8/gocart/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-06 16:57:24.467863 gocart-0.1.8/gocart.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5996 2023-04-06 16:57:24.000000 gocart-0.1.8/gocart.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      718 2023-04-06 16:57:24.000000 gocart-0.1.8/gocart.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-06 16:57:24.000000 gocart-0.1.8/gocart.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-04-06 16:57:24.000000 gocart-0.1.8/gocart.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-06 16:56:24.000000 gocart-0.1.8/gocart.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      113 2023-04-06 16:57:24.000000 gocart-0.1.8/gocart.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-04-06 16:57:24.000000 gocart-0.1.8/gocart.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-04-06 16:57:24.471863 gocart-0.1.8/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1934 2023-04-06 16:52:44.000000 gocart-0.1.8/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-19 15:03:34.625041 gocart-0.1.9/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      990 2023-04-19 14:58:37.000000 gocart-0.1.9/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-04-19 14:58:37.000000 gocart-0.1.9/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-04-19 14:58:37.000000 gocart-0.1.9/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5996 2023-04-19 15:03:34.625041 gocart-0.1.9/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5430 2023-04-19 14:58:37.000000 gocart-0.1.9/README.md
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-19 15:03:34.613040 gocart-0.1.9/gocart/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7204 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-19 15:03:34.621040 gocart-0.1.9/gocart/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1920 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/commonutils/flatten_healpix_map.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2956 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/commonutils/generate_skymap_stats.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/commonutils/getpackagepath.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-19 15:03:34.625041 gocart-0.1.9/gocart/convert/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/convert/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12117 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/convert/aitoff.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3293 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/convert/ascii.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/convert/healpix2cart.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2303 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/default_settings.yaml
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-19 15:03:34.625041 gocart-0.1.9/gocart/parsers/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/parsers/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6509 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/parsers/lvk.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2069 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/test_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-19 15:03:34.617040 gocart-0.1.9/gocart.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5996 2023-04-19 15:03:34.000000 gocart-0.1.9/gocart.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      718 2023-04-19 15:03:34.000000 gocart-0.1.9/gocart.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-19 15:03:34.000000 gocart-0.1.9/gocart.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-04-19 15:03:34.000000 gocart-0.1.9/gocart.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-19 15:02:25.000000 gocart-0.1.9/gocart.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      113 2023-04-19 15:03:34.000000 gocart-0.1.9/gocart.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-04-19 15:03:34.000000 gocart-0.1.9/gocart.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-04-19 15:03:34.625041 gocart-0.1.9/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1934 2023-04-19 14:58:37.000000 gocart-0.1.9/setup.py
```

### Comparing `gocart-0.1.8/CHANGES.md` & `gocart-0.1.9/CHANGES.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 
 ## Release Notes
 
 <!-- **vx.x.x - xxdatexx** -->
 
+**v0.1.9 - April 19, 2023**
+
+- **REFACTOR** -- sun and moon footprints replace terminator
+
 **v0.1.8 - April 6, 2023**
 
 - **FIXED** -- echo command now parses message to the end of the partition queue
 - **FIXED** -- listen command remembers where it left off
 - **FIXED** -- sun & moon coordinates ... they were not geocentric!
 
 **v0.1.7 - April 4, 2023**
```

### Comparing `gocart-0.1.8/LICENSE` & `gocart-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gocart-0.1.8/PKG-INFO` & `gocart-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.1.8
+Version: 0.1.9
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.1.8.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.1.9.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gocart-0.1.8/README.md` & `gocart-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gocart-0.1.8/gocart/cl_utils.py` & `gocart-0.1.9/gocart/cl_utils.py`

 * *Files identical despite different names*

### Comparing `gocart-0.1.8/gocart/commonutils/flatten_healpix_map.py` & `gocart-0.1.9/gocart/commonutils/flatten_healpix_map.py`

 * *Files identical despite different names*

### Comparing `gocart-0.1.8/gocart/commonutils/generate_skymap_stats.py` & `gocart-0.1.9/gocart/commonutils/generate_skymap_stats.py`

 * *Files identical despite different names*

### Comparing `gocart-0.1.8/gocart/convert/aitoff.py` & `gocart-0.1.9/gocart/convert/aitoff.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,27 +59,28 @@
         self.outputFolder = outputFolder
         self.meta = meta
         # xt-self-arg-tmpx
 
         return None
 
     def convert(
-            self,
-            contours=True,
-            galacticPlane=True,
-            daynight=True,
-            sunmoon=True):
+        self,
+        contours=True,
+        galacticPlane=True,
+        sunmoon=True,
+        sunmoonContour=True
+    ):
         """
         *convert the healpix map to an aitoff plot*
 
         **Key Arguments:**
             - ``contours`` -- plot 50 and 90% contours. Default *True*
             - ``galacticPlane`` -- plot galactic plane contours. Default *True*
-            - ``daynight`` -- show sun-position and day/night terminator. Default *True*
             - ``sunmoon`` -- plot sun and moon. Default *True*
+            - ``sunmoonContour`` -- show contours within 33 deg of sun and 20 deg from moon
 
         **Return:**
             - ``plotPath`` -- path to the printed plot
         """
         self.log.debug('starting the ``convert`` method')
 
         import matplotlib.pyplot as plt
@@ -132,72 +133,98 @@
 
         # AITOFF DOES NOT PLAY WELL WITH ADDING LABELS - USE HAMMER PROJECTION INSTEAD
         ax = fig.add_subplot(111, projection='hammer')
 
         # RASTERIZED MAKES THE MAP BITMAP WHILE THE LABELS REMAIN VECTORIAL
         std = data.std()
         mean = data.mean()
-        #image = ax.pcolormesh(long, lat, data, rasterized=False, cmap=cmap, vmin=mean, vmax=mean + 5 * std)
+        # image = ax.pcolormesh(long, lat, data, rasterized=False, cmap=cmap, vmin=mean, vmax=mean + 5 * std)
 
         # GRATICULE
         ax.set_longitude_grid(30)
         ax.set_latitude_grid(15)
         ax.xaxis.set_major_formatter(ThetaFormatterShiftPi(30))
         ax.set_longitude_grid_ends(90)
 
-        if daynight:
+        if sunmoonContour:
             t = Time(header['DATE-OBS'], scale='utc')
 
             # FIND SUN AND PLACE ON CORRECT PLOT COORDINATE
             sun = get_sun(t)
             sun.ra.degree = -sun.ra.degree + 180
             if sun.ra.degree > 180.:
                 sun.ra.degree -= 360
             sun.ra.radian = np.deg2rad(sun.ra.degree)
 
             # COMPUTE LONS AND LATS OF DAY/NIGHT TERMINATOR.
             nlons = 1441
             nlats = ((nlons - 1) / 2) + 1
-            lons, lats = terminator(sun.ra.radian, sun.dec.radian, nlons)
 
-            # for i, l in zip(lons, lats):
-            #     print(np.rad2deg(i), np.rad2deg(l))
+            # COLOR IN THE SUN
+            lons2 = np.linspace(-np.pi, np.pi, nlons)
+            lats2 = np.linspace(-np.pi / 2, np.pi / 2, int(nlats))
+            lons2, lats2 = np.meshgrid(lons2, lats2)
+            sunlight = np.ones(lons2.shape)
+            raSep = sun.ra.radian - lons2
+            raSep[raSep > np.pi] = 2 * np.pi - raSep[raSep > np.pi]
+            separation = ((raSep * np.cos((sun.dec.radian + lats2) / 2))**2 + (sun.dec.radian - lats2)**2)**0.5
+            sunlight[separation < np.radians(33)] = 0
+            sunyellow = matplotlib.colors.colorConverter.to_rgba('#b58900', alpha=0.2)
+            ax.contourf(lons2, lats2, sunlight, 1, colors=[sunyellow, (0.0, 0.0, 0.0, 0.0)], zorder=3)
+
+            # PLOT THE MOON
+            moon = get_moon(t)
+            moon.ra.degree = -moon.ra.degree + 180
+            if moon.ra.degree > 180.:
+                moon.ra.degree -= 360
+            moon.ra.radian = np.deg2rad(moon.ra.degree)
 
-            # DRAW THIN TERMINATOR LINE
-            ax.plot(lons, lats, '#002b36', linewidth=0.3)
+            # COMPUTE LONS AND LATS OF DAY/NIGHT TERMINATOR.
+            nlons = 1441
+            nlats = ((nlons - 1) / 2) + 1
 
-            # COLOR IN THE NIGHT
+            # COLOR IN THE SUN
             lons2 = np.linspace(-np.pi, np.pi, nlons)
             lats2 = np.linspace(-np.pi / 2, np.pi / 2, int(nlats))
             lons2, lats2 = np.meshgrid(lons2, lats2)
-            daynight = np.ones(lons2.shape)
-            for nlon in range(nlons):
-                daynight[:, nlon] = np.where(lats2[:, nlon] < lats[nlon], 0, daynight[:, nlon])
-            ax.contourf(lons2, lats2, daynight, 1, colors=[(0.0, 0.0, 0.0, 0.2), (0.0, 0.0, 0.0, 0.0)], zorder=3)
+            moonlight = np.ones(lons2.shape)
+            raSep = moon.ra.radian - lons2
+            raSep[raSep > np.pi] = 2 * np.pi - raSep[raSep > np.pi]
+            separation = ((raSep * np.cos((moon.dec.radian + lats2) / 2))**2 + (moon.dec.radian - lats2)**2)**0.5
+            moonlight[separation < np.radians(20)] = 0
+            moonblue = matplotlib.colors.colorConverter.to_rgba('#268bd2', alpha=0.2)
+            ax.contourf(lons2, lats2, moonlight, 1, colors=[moonblue, (0.0, 0.0, 0.0, 0.0)], zorder=3)
 
         # PLOT THE SUN
         if sunmoon:
             t = Time(header['DATE-OBS'], scale='utc')
 
             # FIND SUN AND PLACE ON CORRECT PLOT COORDINATE
             sun = get_sun(t)
             sun.ra.degree = -sun.ra.degree + 180
             if sun.ra.degree > 180.:
                 sun.ra.degree -= 360
             sun.ra.radian = np.deg2rad(sun.ra.degree)
 
-            ax.scatter(sun.ra.radian, sun.dec.radian, color="#b58900", alpha=0.8, s=20, marker="o", edgecolors="#cb4b16", linewidths=0.5, label="Sun", zorder=30)
+            label = "Sun"
+            if sunmoonContour:
+                label += " (within $33^o$)"
+            ax.scatter(sun.ra.radian, sun.dec.radian, color="#b58900", alpha=0.8, s=20, marker="o", edgecolors="#cb4b16", linewidths=0.5, label=label, zorder=30)
 
             # PLOT THE MOON
             moon = get_moon(t)
             moon.ra.degree = -moon.ra.degree + 180
             if moon.ra.degree > 180.:
                 moon.ra.degree -= 360
             moon.ra.radian = np.deg2rad(moon.ra.degree)
-            ax.scatter(moon.ra.radian, moon.dec.radian, color="#268bd2", alpha=0.8, s=20, marker="o", edgecolors="#1e6ea7", linewidths=0.5, label="Moon", zorder=29)
+
+            label = "Moon"
+            if sunmoonContour:
+                label += " (within $20^o$)"
+            ax.scatter(moon.ra.radian, moon.dec.radian, color="#268bd2", alpha=0.8, s=20, marker="o", edgecolors="#1e6ea7", linewidths=0.5, label=label, zorder=29)
 
         handles, labels = plt.gca().get_legend_handles_labels()
         if galacticPlane:
             # LON:LAT is lon 0-360 at lat=0
             lon_array = np.arange(0, 360, 0.5)
             lat_arry = np.full_like(lon_array, 0)
             galc = SkyCoord(l=lon_array, b=lat_arry, frame=Galactic, unit=u.deg)
@@ -285,15 +312,7 @@
 
         plt.savefig(self.outputFolder + "/skymap.png", bbox_inches='tight', dpi=300)
 
         plt.close()
 
         self.log.debug('completed the ``convert`` method')
         return None
-
-
-def terminator(ra, dec, nlons):
-    import numpy as np
-    lons = np.linspace(-np.pi, np.pi, nlons)
-    longitude = lons + ra
-    lats = np.arctan(-np.cos(longitude) / np.tan(dec))
-    return lons, lats
```

### Comparing `gocart-0.1.8/gocart/convert/ascii.py` & `gocart-0.1.9/gocart/convert/ascii.py`

 * *Files identical despite different names*

### Comparing `gocart-0.1.8/gocart/convert/healpix2cart.py` & `gocart-0.1.9/gocart/convert/healpix2cart.py`

 * *Files identical despite different names*

### Comparing `gocart-0.1.8/gocart/default_settings.yaml` & `gocart-0.1.9/gocart/default_settings.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,17 @@
     # DOWNLOAD PRODUCTION EVENT ALERTS?
     parse_real_events: False
     # LOCATION TO DOWNLOAD EVENT ALERT AND MAPS TO
     download_dir: ~/lvk_events
     # CONVERT MAPS TO AITOFF PLOTS?
     aitoff:
         convert: True
-        day_night: True
         sun_moon: True
+        # PLOT CONTOUR 33 DEG FROM SUN AND 20 DEG FROM MOON
+        sun_moon_contour: True
         galactic_plane: True
     # CONVERT MAP TO ASCII FILE - ONE ROW PER HEALPIX PIXEL
     ascii_map:
         convert: True
         # THE SIZE OF HEALPIX PIXELS TO RESOLVE SKY TO. NSIDE = 64 IS ~0.84 deg2 PER PIXEL.
         nside: 64
```

### Comparing `gocart-0.1.8/gocart/parsers/lvk.py` & `gocart-0.1.9/gocart/parsers/lvk.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,12 +168,12 @@
                     mapPath=fitsPath,
                     outputFolder=alertDir,
                     settings=self.settings,
                     meta=meta
                 )
                 c.convert(
                     galacticPlane=self.settings["lvk"]["aitoff"]["galactic_plane"],
-                    daynight=self.settings["lvk"]["aitoff"]["day_night"],
+                    sunmoonContour=self.settings["lvk"]["aitoff"]["sun_moon_contour"],
                     sunmoon=self.settings["lvk"]["aitoff"]["sun_moon"])
 
         self.log.debug('completed the ``parse`` method')
         return lvk
```

### Comparing `gocart-0.1.8/gocart/setup.cfg` & `gocart-0.1.9/gocart/setup.cfg`

 * *Files identical despite different names*

### Comparing `gocart-0.1.8/gocart/test_settings.yaml` & `gocart-0.1.9/gocart/test_settings.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 lvk:
     parse_mock_events: True
     parse_real_events: False
     download_dir: ~/lvk_events
     # CONVERT MAPS TO AITOFF PLOTS?
     aitoff:
         convert: True
-        day_night: False
+        # PLOT CONTOUR 33 DEG FROM SUN AND 20 DEG FROM MOON
+        sun_moon_contour: True
         sun_moon: False
         galactic_plane: True
     # CONVERT MAP TO ASCII FILE - ONE ROW PER HEALPIX PIXEL
     ascii_map:
         convert: True
         # THE SIZE OF HEALPIX PIXELS TO RESOLVE SKY TO. NSIDE = 64 IS ~0.84 deg2 PER PIXEL.
         nside: 16
```

### Comparing `gocart-0.1.8/gocart/utKit.py` & `gocart-0.1.9/gocart/utKit.py`

 * *Files identical despite different names*

### Comparing `gocart-0.1.8/gocart.egg-info/PKG-INFO` & `gocart-0.1.9/gocart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.1.8
+Version: 0.1.9
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.1.8.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.1.9.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gocart-0.1.8/gocart.egg-info/SOURCES.txt` & `gocart-0.1.9/gocart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gocart-0.1.8/setup.py` & `gocart-0.1.9/setup.py`

 * *Files identical despite different names*

