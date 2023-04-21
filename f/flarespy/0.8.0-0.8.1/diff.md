# Comparing `tmp/flarespy-0.8.0.tar.gz` & `tmp/flarespy-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.8.0.tar", max compression
+gzip compressed data, was "flarespy-0.8.1.tar", max compression
```

## Comparing `flarespy-0.8.0.tar` & `flarespy-0.8.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.8.0/LICENSE
--rw-r--r--   0        0        0      428 2023-04-21 10:08:14.300704 flarespy-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.8.0/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.8.0/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.8.0/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    25272 2023-04-21 10:27:47.370450 flarespy-0.8.0/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     6907 2023-04-21 10:25:18.842486 flarespy-0.8.0/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-21 10:08:14.305876 flarespy-0.8.0/src/flarespy/version.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.8.1/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-21 10:29:38.450202 flarespy-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.8.1/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.8.1/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.8.1/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    25242 2023-04-21 10:29:01.957744 flarespy-0.8.1/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     6907 2023-04-21 10:25:18.842486 flarespy-0.8.1/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-21 10:29:38.446422 flarespy-0.8.1/src/flarespy/version.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.8.1/PKG-INFO
```

### Comparing `flarespy-0.8.0/LICENSE` & `flarespy-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.8.0/src/flarespy/Flare_model.py` & `flarespy-0.8.1/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.8.0/src/flarespy/data/model.dat` & `flarespy-0.8.1/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.8.0/src/flarespy/flarefinder.py` & `flarespy-0.8.1/src/flarespy/flarefinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,18 +314,18 @@
                     try:
                         query_result = CUSTOM_SIMBAD.query_object(f"Gaia DR3 {gaia_dr3_id}")
                     except TableParseError:
                         pass
 
         self.meta["exclude"] = False
         if query_result is None:
-            self.stellar_parameters.simbad_object_type = np.nan
+            self.stellar_parameters.obj_type = np.nan
         else:
             obj_type = query_result["OTYPE"][0]
-            self.stellar_parameters.simbad_object_type = obj_type
+            self.stellar_parameters.obj_type = obj_type
 
             if obj_type in EXCLUDED_OTYPES or "CV*" in obj_type.split("|"):
                 self.meta["exclude"] = True
 
     def detrend(self, window_length=0.3):
         """Detrend the lightcurve."""
 
@@ -594,15 +594,15 @@
                         bottom=False,
                         left=False,
                         right=False,
                     )
 
                     period = "{:.2f}d".format(self.period) if self.period > 0 else "/"
                     title = (
-                        f"{self.label}, Sector {self.sector}, {self.stellar_parameters.simbad_object_type}, P={period}"
+                        f"{self.label}, Sector {self.sector}, {self.stellar_parameters.obj_type}, P={period}"
                     )
 
                     plt.suptitle(title, y=0.94, fontsize=15)
                     plt.subplots_adjust(hspace=0.05, wspace=0.012)
 
                     figure_path = figure_subfolder / "{}-S{}-{}.png".format(
                         self.label.replace(" ", ""), self.sector, round(row.t_peak, 7)
```

### Comparing `flarespy-0.8.0/src/flarespy/utils.py` & `flarespy-0.8.1/src/flarespy/utils.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.8.0/PKG-INFO` & `flarespy-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.8.0
+Version: 0.8.1
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

