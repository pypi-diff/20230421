# Comparing `tmp/satip-2.9.8.tar.gz` & `tmp/satip-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satip-2.9.8.tar", last modified: Tue Jun 21 21:53:40 2022, max compression
+gzip compressed data, was "satip-2.9.9.tar", last modified: Tue Jun 21 22:01:35 2022, max compression
```

## Comparing `satip-2.9.8.tar` & `satip-2.9.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 21:53:40.601348 satip-2.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-06-21 21:53:09.000000 satip-2.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-06-21 21:53:09.000000 satip-2.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7079 2022-06-21 21:53:40.601348 satip-2.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6813 2022-06-21 21:53:09.000000 satip-2.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-06-21 21:53:10.000000 satip-2.9.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 21:53:40.601348 satip-2.9.8/satip/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-06-21 21:53:10.000000 satip-2.9.8/satip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4727 2022-06-21 21:53:10.000000 satip-2.9.8/satip/app.py
--rw-r--r--   0 runner    (1001) docker     (121)    15491 2022-06-21 21:53:10.000000 satip-2.9.8/satip/download.py
--rw-r--r--   0 runner    (1001) docker     (121)    18902 2022-06-21 21:53:10.000000 satip-2.9.8/satip/eumetsat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-06-21 21:53:10.000000 satip-2.9.8/satip/geospatial.py
--rw-r--r--   0 runner    (1001) docker     (121)    14186 2022-06-21 21:53:10.000000 satip-2.9.8/satip/intermediate.py
--rw-r--r--   0 runner    (1001) docker     (121)     8034 2022-06-21 21:53:10.000000 satip-2.9.8/satip/jpeg_xl_float_with_nans.py
--rw-r--r--   0 runner    (1001) docker     (121)     5266 2022-06-21 21:53:10.000000 satip-2.9.8/satip/scale_to_zero_to_one.py
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-06-21 21:53:10.000000 satip-2.9.8/satip/serialize.py
--rw-r--r--   0 runner    (1001) docker     (121)    32930 2022-06-21 21:53:10.000000 satip-2.9.8/satip/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 21:53:40.601348 satip-2.9.8/satip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7079 2022-06-21 21:53:40.000000 satip-2.9.8/satip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-06-21 21:53:40.000000 satip-2.9.8/satip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-21 21:53:40.000000 satip-2.9.8/satip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-06-21 21:53:40.000000 satip-2.9.8/satip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-21 21:53:40.000000 satip-2.9.8/satip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-21 21:53:40.601348 satip-2.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-06-21 21:53:24.000000 satip-2.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 22:01:35.256207 satip-2.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-06-21 22:01:03.000000 satip-2.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-06-21 22:01:03.000000 satip-2.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7079 2022-06-21 22:01:35.256207 satip-2.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6813 2022-06-21 22:01:03.000000 satip-2.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-06-21 22:01:03.000000 satip-2.9.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 22:01:35.252207 satip-2.9.9/satip/
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-06-21 22:01:03.000000 satip-2.9.9/satip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4727 2022-06-21 22:01:03.000000 satip-2.9.9/satip/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15491 2022-06-21 22:01:03.000000 satip-2.9.9/satip/download.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18902 2022-06-21 22:01:03.000000 satip-2.9.9/satip/eumetsat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-06-21 22:01:03.000000 satip-2.9.9/satip/geospatial.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14186 2022-06-21 22:01:03.000000 satip-2.9.9/satip/intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8034 2022-06-21 22:01:03.000000 satip-2.9.9/satip/jpeg_xl_float_with_nans.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5266 2022-06-21 22:01:03.000000 satip-2.9.9/satip/scale_to_zero_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-06-21 22:01:03.000000 satip-2.9.9/satip/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32918 2022-06-21 22:01:03.000000 satip-2.9.9/satip/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 22:01:35.252207 satip-2.9.9/satip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7079 2022-06-21 22:01:34.000000 satip-2.9.9/satip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-06-21 22:01:35.000000 satip-2.9.9/satip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-21 22:01:34.000000 satip-2.9.9/satip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-06-21 22:01:35.000000 satip-2.9.9/satip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-21 22:01:35.000000 satip-2.9.9/satip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-21 22:01:35.256207 satip-2.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-06-21 22:01:21.000000 satip-2.9.9/setup.py
```

### Comparing `satip-2.9.8/LICENSE` & `satip-2.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `satip-2.9.8/PKG-INFO` & `satip-2.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satip
-Version: 2.9.8
+Version: 2.9.9
 Summary: Satip provides the functionality necessary for
 Author: Jacob Bieker, Ayrton Bourn, Jack Kelly
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `satip-2.9.8/README.md` & `satip-2.9.9/README.md`

 * *Files identical despite different names*

### Comparing `satip-2.9.8/satip/app.py` & `satip-2.9.9/satip/app.py`

 * *Files identical despite different names*

### Comparing `satip-2.9.8/satip/download.py` & `satip-2.9.9/satip/download.py`

 * *Files identical despite different names*

### Comparing `satip-2.9.8/satip/eumetsat.py` & `satip-2.9.9/satip/eumetsat.py`

 * *Files identical despite different names*

### Comparing `satip-2.9.8/satip/geospatial.py` & `satip-2.9.9/satip/geospatial.py`

 * *Files identical despite different names*

### Comparing `satip-2.9.8/satip/intermediate.py` & `satip-2.9.9/satip/intermediate.py`

 * *Files identical despite different names*

### Comparing `satip-2.9.8/satip/jpeg_xl_float_with_nans.py` & `satip-2.9.9/satip/jpeg_xl_float_with_nans.py`

 * *Files identical despite different names*

### Comparing `satip-2.9.8/satip/scale_to_zero_to_one.py` & `satip-2.9.9/satip/scale_to_zero_to_one.py`

 * *Files identical despite different names*

### Comparing `satip-2.9.8/satip/serialize.py` & `satip-2.9.9/satip/serialize.py`

 * *Files identical despite different names*

### Comparing `satip-2.9.8/satip/utils.py` & `satip-2.9.9/satip/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,15 +322,15 @@
 
     Returns:
         Xarray DataArray
     """
     dataarray = dataarray.reindex({"variable": variable_order}).transpose(
         "time", "y_geostationary", "x_geostationary", "variable"
     )
-    upper_bound = (2**10) - 1
+    upper_bound = (2 ** 10) - 1
     new_max = maxs - mins
 
     dataarray -= mins
     dataarray /= new_max
     dataarray *= upper_bound
     dataarray = dataarray.round().clip(min=0, max=upper_bound).astype(np.int16)
     return dataarray
@@ -443,15 +443,15 @@
                     variable_order=["HRV"],
                     maxs=np.array([103.90016]),
                     mins=np.array([-1.2278595]),
                 )
             hrv_dataarray = hrv_dataarray.transpose(
                 "time", "y_geostationary", "x_geostationary", "variable"
             )
-            hrv_dataarray = hrv_dataarray.chunk((1,512,512,1))
+            hrv_dataarray = hrv_dataarray.chunk((1, 512, 512, 1))
             hrv_dataset = hrv_dataarray.to_dataset(name="data")
             del hrv_dataarray
             hrv_dataset.attrs.update(attrs)
             now_time = pd.Timestamp(hrv_dataset["time"].values[0]).strftime("%Y%m%d%H%M")
             save_file = os.path.join(
                 save_dir, f"{'15_' if using_backup else ''}hrv_{now_time}.zarr.zip"
             )
@@ -526,15 +526,15 @@
                     "VIS006",
                     "VIS008",
                     "WV_062",
                     "WV_073",
                 ],
             )
         dataarray = dataarray.transpose("time", "y_geostationary", "x_geostationary", "variable")
-        dataarray = dataarray.chunk((1,256,256,1))
+        dataarray = dataarray.chunk((1, 256, 256, 1))
         dataset = dataarray.to_dataset(name="data")
         del dataarray
         dataset.attrs.update(attrs)
         now_time = pd.Timestamp(dataset["time"].values[0]).strftime("%Y%m%d%H%M")
         save_file = os.path.join(save_dir, f"{'15_' if using_backup else ''}{now_time}.zarr.zip")
         logger.info(f"Saving non-HRV netcdf in {save_file}")
         save_to_zarr_to_s3(dataset, save_file)
@@ -684,24 +684,23 @@
     2. upload to s3
     :param dataset: The Xarray Dataset to be save
     :param filename: The s3 filename
     """
 
     gc.collect()
     logger.info(f"Saving file to {filename}")
-    logger.info(f'nbytes in MB:  {dataset.nbytes / (1024 * 1024)}')
+    logger.info(f"nbytes in MB:  {dataset.nbytes / (1024 * 1024)}")
 
     with tempfile.TemporaryDirectory() as dir:
         # save locally
         path = f"{dir}/temp.zarr.zip"
         with zarr.ZipStore(path) as store:
             dataset.to_zarr(store, compute=True, mode="w")
 
-        logger.debug(f'Saved to temporary file {path}, '
-                     f'now pushing to {filename}')
+        logger.debug(f"Saved to temporary file {path}, " f"now pushing to {filename}")
 
         # save to s3
         filesystem = fsspec.open(filename).fs
         filesystem.put(path, filename)
 
 
 def filter_dataset_ids_on_current_files(datasets: list, save_dir: str) -> list:
@@ -721,22 +720,22 @@
         The filtered list of new datasets ids to download
     """
     from satip.eumetsat import eumetsat_filename_to_datetime
 
     ids = [dataset["id"] for dataset in datasets]
     filesystem = fsspec.open(save_dir).fs
     finished_files_not_latest = list(filesystem.glob(f"{save_dir}/*.zarr.zip"))
-    logger.info(f'Found {len(finished_files_not_latest)} already downloaded in data folder')
+    logger.info(f"Found {len(finished_files_not_latest)} already downloaded in data folder")
 
-    filesystem_latest = fsspec.open(save_dir + '/latest').fs
+    filesystem_latest = fsspec.open(save_dir + "/latest").fs
     finished_files_latest = list(filesystem_latest.glob(f"{save_dir}/latest/*.zarr.zip"))
-    logger.info(f'Found {len(finished_files_latest)} already downloaded in latest folder')
+    logger.info(f"Found {len(finished_files_latest)} already downloaded in latest folder")
 
-    finished_files = finished_files_not_latest+ finished_files_latest
-    logger.info(f'Found {len(finished_files)} already downloaded')
+    finished_files = finished_files_not_latest + finished_files_latest
+    logger.info(f"Found {len(finished_files)} already downloaded")
 
     datetimes = [pd.Timestamp(eumetsat_filename_to_datetime(idx)).round("5 min") for idx in ids]
     if not datetimes:  # Empty list
         logger.debug("No datetimes to download")
         return []
     logger.debug(f"The latest datetime that we want to downloaded is {max(datetimes)}")
 
@@ -759,17 +758,17 @@
         logger.debug("There are no files already downloaded")
 
     # find which indexes to remove, if file is already there
     idx_to_remove = []
     for idx, date in enumerate(datetimes):
         if date in finished_datetimes:
             idx_to_remove.append(idx)
-            logger.debug(f'Will not be downloading file with {date=} as already downloaded')
+            logger.debug(f"Will not be downloading file with {date=} as already downloaded")
         else:
-            logger.debug(f'Will be downloading file with {date=}')
+            logger.debug(f"Will be downloading file with {date=}")
     logger.debug(
         f"Will be not be downloading {len(idx_to_remove)} files "
         f"as they have already been downloaded"
     )
 
     # remove index
     indices = sorted(idx_to_remove, reverse=True)
@@ -794,15 +793,15 @@
     finished_files = filesystem.glob(f"{save_dir}/*.zarr.zip")
 
     logger.info(f"Checking {save_dir}/ for moving newer files into {save_dir}/latest/")
 
     # get datetimes of the finished files
 
     for date in finished_files:
-        logger.debug(f'Looking at file {date}')
+        logger.debug(f"Looking at file {date}")
         if "latest.zarr" in date or "tmp" in date:
             continue
         if "hrv" in date:
             file_time = pd.to_datetime(
                 date.replace("15_", "").split(".zarr.zip")[0].split("/")[-1].split("_")[-1],
                 format="%Y%m%d%H%M",
                 errors="ignore",
@@ -812,27 +811,27 @@
             file_time = pd.to_datetime(
                 date.replace("15_", "").split(".zarr.zip")[0].split("/")[-1],
                 format="%Y%m%d%H%M",
                 errors="ignore",
                 utc=True,
             )
         if file_time > history_time:
-            logger.debug('Moving file out of latest folder')
+            logger.debug("Moving file out of latest folder")
             # Move HRV and non-HRV to new place
             filesystem.move(date, f"{save_dir}/latest/{date.split('/')[-1]}")
         elif file_time < (history_time - pd.Timedelta("2 days")):
             # Delete files over 2 days old
-            logger.debug('Removing file over 2 days over')
+            logger.debug("Removing file over 2 days over")
             filesystem.rm(date)
 
     finished_files = filesystem.glob(f"{save_dir}/latest/*.zarr.zip")
     logger.info(f"Checking {save_dir}/latest/ for older files")
     # get datetimes of the finished files
     for date in finished_files:
-        logger.debug(f'Looking at file {date}')
+        logger.debug(f"Looking at file {date}")
         if "latest" in date or "tmp" in date:
             continue
         if "hrv" in date:
             file_time = pd.to_datetime(
                 date.replace("15_", "").split(".zarr.zip")[0].split("/")[-1].split("_")[-1],
                 format="%Y%m%d%H%M",
                 errors="ignore",
@@ -842,15 +841,15 @@
             file_time = pd.to_datetime(
                 date.replace("15_", "").split(".zarr.zip")[0].split("/")[-1],
                 format="%Y%m%d%H%M",
                 errors="ignore",
                 utc=True,
             )
         if file_time < history_time:
-            logger.debug('Moving file out of latest folder')
+            logger.debug("Moving file out of latest folder")
             # Move HRV and non-HRV to new place
             filesystem.move(date, f"{save_dir}/{date.split('/')[-1]}")
 
 
 def collate_files_into_latest(save_dir: str, using_backup: bool = False):
     """
     Convert individual files into single latest file for HRV and non-HRV
```

### Comparing `satip-2.9.8/satip.egg-info/PKG-INFO` & `satip-2.9.9/satip.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satip
-Version: 2.9.8
+Version: 2.9.9
 Summary: Satip provides the functionality necessary for
 Author: Jacob Bieker, Ayrton Bourn, Jack Kelly
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `satip-2.9.8/setup.py` & `satip-2.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
 
 setup(
     name="satip",
-    version="2.9.8",
+    version="2.9.9",
     license="MIT",
     description="""Satip provides the functionality necessary for
                    retrieving, and storing EUMETSAT data""",
     author="Jacob Bieker, Ayrton Bourn, Jack Kelly",
     author_email="info@openclimatefix.org",
     company="Open Climate Fix Ltd",
     install_requires=install_requires,
```

