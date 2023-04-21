# Comparing `tmp/flarespy-0.7.3.tar.gz` & `tmp/flarespy-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.7.3.tar", max compression
+gzip compressed data, was "flarespy-0.7.4.tar", max compression
```

## Comparing `flarespy-0.7.3.tar` & `flarespy-0.7.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.7.3/LICENSE
--rw-r--r--   0        0        0      428 2023-04-20 02:34:27.679255 flarespy-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.7.3/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.7.3/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.7.3/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    26176 2023-04-20 02:13:28.425091 flarespy-0.7.3/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     4572 2023-04-16 09:27:59.194030 flarespy-0.7.3/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-20 02:34:27.680752 flarespy-0.7.3/src/flarespy/version.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.7.4/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-20 15:39:33.014974 flarespy-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.7.4/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.7.4/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.7.4/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    26286 2023-04-20 15:38:58.402467 flarespy-0.7.4/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     4590 2023-04-20 15:30:12.090637 flarespy-0.7.4/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-20 15:39:33.020573 flarespy-0.7.4/src/flarespy/version.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.7.4/PKG-INFO
```

### Comparing `flarespy-0.7.3/LICENSE` & `flarespy-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.7.3/src/flarespy/Flare_model.py` & `flarespy-0.7.4/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.7.3/src/flarespy/data/model.dat` & `flarespy-0.7.4/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.7.3/src/flarespy/flarefinder.py` & `flarespy-0.7.4/src/flarespy/flarefinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,20 +337,21 @@
                 plx = r["parallax"].data.data[target_index]
                 if plx > 0:
                     self.stellar_parameters.parallax = np.round(plx, 4)
                 self.stellar_parameters.phot_g_mean_mag = np.round(r["phot_g_mean_mag"].data.data[target_index], 4)
                 self.stellar_parameters.phot_bp_mean_mag = np.round(r["phot_bp_mean_mag"].data.data[target_index], 4)
                 self.stellar_parameters.phot_rp_mean_mag = np.round(r["phot_rp_mean_mag"].data.data[target_index], 4)
 
-        # Query TESS mag from TIC
+        # Query TESS mag and contamination ratio from TIC
         tic_data = Catalogs.query_object(self.label, radius=0.02, catalog="TIC")
         tic_data.add_index("ID")
         try:
             target_row = tic_data.loc[str(self.ticid)]
             self.stellar_parameters.tess_mag = target_row["Tmag"]
+            self.stellar_parameters.cont_ratio = np.round(target_row["contratio"], 4)
         except KeyError:
             pass
 
     def detrend(self, window_length=0.3):
         """Detrend the lightcurve."""
 
         self._query_object_type_from_simbad()
```

### Comparing `flarespy-0.7.3/src/flarespy/utils.py` & `flarespy-0.7.4/src/flarespy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 STELLAR_PARAMETER_COLUMNS = [
     "gaia3_source_id",
     "parallax",
     "phot_g_mean_mag",
     "phot_bp_mean_mag",
     "phot_rp_mean_mag",
     "tess_mag",
+    "cont_ratio",
     "obs_duration",
 ]
 
 
 def extract_features(x):
     abs_energy = np.dot(x, x)
     first_location_of_maximum = np.argmax(x) / len(x)
```

### Comparing `flarespy-0.7.3/PKG-INFO` & `flarespy-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.7.3
+Version: 0.7.4
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

