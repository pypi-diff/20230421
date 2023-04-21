# Comparing `tmp/openpolicedata-0.5.1.tar.gz` & `tmp/openpolicedata-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpolicedata-0.5.1.tar", last modified: Fri Feb 10 00:26:51 2023, max compression
+gzip compressed data, was "openpolicedata-0.5.2.tar", last modified: Fri Apr 21 12:22:15 2023, max compression
```

## Comparing `openpolicedata-0.5.1.tar` & `openpolicedata-0.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-02-10 00:26:51.254398 openpolicedata-0.5.1/
--rw-rw-rw-   0        0        0     1542 2022-02-12 00:47:00.000000 openpolicedata-0.5.1/LICENSE
--rw-rw-rw-   0        0        0    12089 2023-02-10 00:26:51.255398 openpolicedata-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    11024 2023-02-10 00:25:24.000000 openpolicedata-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-10 00:26:51.205053 openpolicedata-0.5.1/openpolicedata/
--rw-rw-rw-   0        0        0      569 2022-09-24 21:27:15.000000 openpolicedata-0.5.1/openpolicedata/__init__.py
--rw-rw-rw-   0        0        0       21 2023-02-08 22:54:45.000000 openpolicedata-0.5.1/openpolicedata/_version.py
--rw-rw-rw-   0        0        0    30603 2023-02-09 23:24:28.000000 openpolicedata-0.5.1/openpolicedata/data.py
--rw-rw-rw-   0        0        0    72208 2023-02-10 00:11:57.000000 openpolicedata-0.5.1/openpolicedata/data_loaders.py
--rw-rw-rw-   0        0        0    10387 2023-02-08 22:54:38.000000 openpolicedata-0.5.1/openpolicedata/datasets.py
--rw-rw-rw-   0        0        0     8334 2023-01-25 12:45:44.000000 openpolicedata-0.5.1/openpolicedata/defs.py
--rw-rw-rw-   0        0        0     1601 2022-09-24 20:54:13.000000 openpolicedata-0.5.1/openpolicedata/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-02-10 00:26:51.242396 openpolicedata-0.5.1/openpolicedata.egg-info/
--rw-rw-rw-   0        0        0    12089 2023-02-10 00:26:51.000000 openpolicedata-0.5.1/openpolicedata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2023-02-10 00:26:51.000000 openpolicedata-0.5.1/openpolicedata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-10 00:26:51.000000 openpolicedata-0.5.1/openpolicedata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-02-10 00:26:51.000000 openpolicedata-0.5.1/openpolicedata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-02-10 00:26:51.000000 openpolicedata-0.5.1/openpolicedata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      426 2023-01-03 00:17:47.000000 openpolicedata-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0     1278 2023-02-10 00:26:51.256397 openpolicedata-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      425 2023-01-02 22:32:48.000000 openpolicedata-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-10 00:26:51.251399 openpolicedata-0.5.1/tests/
--rw-rw-rw-   0        0        0    20094 2023-02-09 12:40:56.000000 openpolicedata-0.5.1/tests/test_data_loaders.py
--rw-rw-rw-   0        0        0     8977 2023-02-09 00:29:49.000000 openpolicedata-0.5.1/tests/test_datasets.py
--rw-rw-rw-   0        0        0    11017 2023-02-10 00:17:26.000000 openpolicedata-0.5.1/tests/test_opd_data1.py
--rw-rw-rw-   0        0        0     7776 2023-02-09 01:12:12.000000 openpolicedata-0.5.1/tests/test_opd_data2.py
--rw-rw-rw-   0        0        0    10996 2023-01-08 17:35:42.000000 openpolicedata-0.5.1/tests/test_opd_data3.py
+drwxrwxrwx   0        0        0        0 2023-04-21 12:22:15.306262 openpolicedata-0.5.2/
+-rw-rw-rw-   0        0        0     1542 2022-02-12 00:47:00.000000 openpolicedata-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0    12140 2023-04-21 12:22:15.307252 openpolicedata-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11024 2023-02-11 13:57:45.000000 openpolicedata-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 12:22:15.283528 openpolicedata-0.5.2/openpolicedata/
+-rw-rw-rw-   0        0        0      569 2022-09-24 21:27:15.000000 openpolicedata-0.5.2/openpolicedata/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-04-17 23:24:30.000000 openpolicedata-0.5.2/openpolicedata/_version.py
+-rw-rw-rw-   0        0        0    30772 2023-04-20 11:21:06.000000 openpolicedata-0.5.2/openpolicedata/data.py
+-rw-rw-rw-   0        0        0    72813 2023-04-21 11:39:12.000000 openpolicedata-0.5.2/openpolicedata/data_loaders.py
+-rw-rw-rw-   0        0        0    10387 2023-02-14 01:01:36.000000 openpolicedata-0.5.2/openpolicedata/datasets.py
+-rw-rw-rw-   0        0        0     8616 2023-04-17 11:23:17.000000 openpolicedata-0.5.2/openpolicedata/defs.py
+-rw-rw-rw-   0        0        0     1601 2022-09-24 20:54:13.000000 openpolicedata-0.5.2/openpolicedata/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-21 12:22:15.292920 openpolicedata-0.5.2/openpolicedata.egg-info/
+-rw-rw-rw-   0        0        0    12140 2023-04-21 12:22:15.000000 openpolicedata-0.5.2/openpolicedata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2023-04-21 12:22:15.000000 openpolicedata-0.5.2/openpolicedata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 12:22:15.000000 openpolicedata-0.5.2/openpolicedata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-21 12:22:15.000000 openpolicedata-0.5.2/openpolicedata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-21 12:22:15.000000 openpolicedata-0.5.2/openpolicedata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      426 2023-02-11 00:12:22.000000 openpolicedata-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1318 2023-04-21 12:22:15.309253 openpolicedata-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      425 2023-01-02 22:32:48.000000 openpolicedata-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 12:22:15.304252 openpolicedata-0.5.2/tests/
+-rw-rw-rw-   0        0        0    20542 2023-04-17 23:25:34.000000 openpolicedata-0.5.2/tests/test_data_loaders.py
+-rw-rw-rw-   0        0        0     9035 2023-04-17 11:23:01.000000 openpolicedata-0.5.2/tests/test_datasets.py
+-rw-rw-rw-   0        0        0    11163 2023-04-19 23:02:19.000000 openpolicedata-0.5.2/tests/test_opd_data1.py
+-rw-rw-rw-   0        0        0     7811 2023-04-18 23:05:43.000000 openpolicedata-0.5.2/tests/test_opd_data2.py
+-rw-rw-rw-   0        0        0    11428 2023-04-21 12:15:02.000000 openpolicedata-0.5.2/tests/test_opd_data3.py
```

### Comparing `openpolicedata-0.5.1/LICENSE` & `openpolicedata-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.1/PKG-INFO` & `openpolicedata-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: openpolicedata
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Python library providing easy access to 276+ incident-level open datasets released by police departments including traffic stops, use of force, officer-involved shootings, and complaints data
 Home-page: https://github.com/openpolicedata/openpolicedata
 Author: Matt Sowd
 Author-email: openpolicedata@gmail.com
 Project-URL: Bug Tracker, https://github.com/openpolicedata/openpolicedata/issues
 Keywords: police data,use of force,traffic,stops,complaints,officer-involved,shootings,pandas,arcgis,socrata,police transparency,police accountability
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `openpolicedata-0.5.1/README.md` & `openpolicedata-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.1/openpolicedata/__init__.py` & `openpolicedata-0.5.2/openpolicedata/__init__.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.1/openpolicedata/data.py` & `openpolicedata-0.5.2/openpolicedata/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -619,20 +619,22 @@
         return loader
 
 def _check_date(table, date_field):
     if date_field != None and table is not None and len(table)>0:
         dts = table[date_field]
         dts = dts[dts.notnull()]
         if len(dts) > 0:
-            one_date = dts.iloc[0]            
-            if type(one_date) == str:
+            one_date = dts.iloc[0]  
+            if type(one_date) == pd._libs.tslibs.timestamps.Timestamp:
+                table[date_field] = pd.to_datetime(table[date_field], errors='ignore')
+            elif type(one_date) == str:
                 p = re.compile(r'^Unknown string format: \d{4}-(\d{2}|__)-(\d{2}|__) present at position \d+$')
                 def to_datetime(x):
                     try:
-                        return pd.to_datetime(x)
+                        return pd.to_datetime(x, errors='ignore')
                     except ParserError as e:
                         if len(e.args)>0 and p.match(e.args[0]) != None:
                             return pd.NaT
                         else:
                             raise
                     except:
                         raise
```

### Comparing `openpolicedata-0.5.1/openpolicedata/data_loaders.py` & `openpolicedata-0.5.2/openpolicedata/data_loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,15 +315,16 @@
             raise ValueError("Extracting the years of a CSV file requires reading the whole file in. In most cases, "+
                 "running load() with no arguments to load in the whole CSV file and manually finding the years will be more "
                 "efficient. If running get_years is still desired, set force=True")
         else:
             if self.date_field==None:
                 raise ValueError("No date field provided to access year information")
             df = self.load()
-            years = list(df[self.date_field].dt.year.dropna().unique())
+            date_col = pd.to_datetime(df[self.date_field])
+            years = list(date_col.dt.year.dropna().unique())
             years.sort()
             return [int(x) for x in years]
 
 
 class Excel(Data_Loader):
     """
     A class for accessing data from Excel download URLs
@@ -365,15 +366,15 @@
         self.url = url
         self.date_field = date_field
         self.agency_field = agency_field
         
         try:
             self.excel_file = pd.ExcelFile(url)
         except urllib.error.HTTPError as e:
-            if str(e) == "HTTP Error 406: Not Acceptable":
+            if str(e) in ["HTTP Error 406: Not Acceptable", 'HTTP Error 403: Forbidden']:
                 # 406 error: https://stackoverflow.com/questions/34832970/http-error-406-not-acceptable-python-urllib2
                 # File-like input for URL: https://stackoverflow.com/questions/57815780/how-can-i-directly-handle-excel-file-link-python/57815864#57815864
                 headers = {'User-agent' : 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.75.14 (KHTML, like Gecko) Version/7.0.3 Safari/7046A194A'}
                 r = requests.get(url, stream=True, headers=headers)
                 r.raise_for_status()
                 file_like = BytesIO(r.content)
                 self.excel_file = pd.ExcelFile(file_like)
@@ -575,14 +576,24 @@
 
         if offset>0:
             rows_limit = nrows_read if nrows_read is not None and nrows_read<len(table) else len(table)
             table = table.iloc[offset:rows_limit].reset_index(drop=True)
         if nrows is not None and len(table)>nrows:
             table = table.head(nrows)
 
+        # Check for empty rows at the bottom
+        num_empty = table.isnull().sum(axis=1)
+        empty_rows = num_empty==len(table.columns)
+        if empty_rows.any():
+            # Check if all rows after first empty row are empty or almost empty
+            empty_rows = empty_rows[empty_rows]
+            num_empty = num_empty.loc[empty_rows.index[0]:]
+            if ((num_empty / len(table.columns)) > 0.75).all():
+                table = table.head(empty_rows.index[0])
+
         # Clean up column names
         table.columns = [x.strip() if isinstance(x, str) else x for x in table.columns]
 
         table = filter_dataframe(table, date_field=self.date_field, year_filter=year, 
             agency_field=self.agency_field, agency=agency)
 
         return table
@@ -629,15 +640,15 @@
         year_dict, has_year_sheets = self.__get_sheets()
 
         if has_year_sheets:
             years = list(year_dict.keys())
             years.sort()
             return list(year_dict.keys())
         if not force:
-            raise ValueError("Extracting the years of a CSV file requires reading the whole file in. In most cases, "+
+            raise ValueError("Extracting the years of a Excel file requires reading the whole file in. In most cases, "+
                 "running load() with no arguments to load in the whole CSV file and manually finding the years will be more "
                 "efficient. If running get_years is still desired, set force=True")
         else:
             if self.date_field==None:
                 raise ValueError("No date field provided to access year information")
             df = self.load()
             years = list(df[self.date_field].dt.year.dropna().unique())
@@ -883,15 +894,15 @@
         if self._date_format in [0,1] or self._date_format==None:
             start_date, stop_date = _process_date(year)
             
             for k in range(0,2):
                 if k==0:
                     where_query = f"{self.date_field} >= '{start_date}' AND  {self.date_field} < '{stop_date}'"
                 else:
-                    break
+                    # break
                     # Dataset (San Jose crash data) that required this does not function well so removing its functionality for now to speed up this function.
                     # This is the recommended way but it has been found to not work sometimes. One dataset was found that requires this.
                     # https://gis.stackexchange.com/questions/451107/arcgis-rest-api-unable-to-complete-operation-on-esrifieldtypedate-in-query
                     stop_date_tmp = stop_date.replace("T"," ")
                     where_query = f"{self.date_field} >= TIMESTAMP '{start_date}' AND  {self.date_field} < TIMESTAMP '{stop_date_tmp}'"
             
                 try:
@@ -1115,16 +1126,14 @@
                     except Exception as e:
                         raise e
                 else:
                     geometry = [feat["geometry"] if "geometry" in feat else None for feat in features]
 
                     if "geolocation" not in df:
                         df["geolocation"] = geometry
-                    else:
-                        raise KeyError("geolocation already exists in DataFrame")
 
             return df
         else:
             return None
 
 
 class Carto(Data_Loader):
@@ -1330,15 +1339,15 @@
                     use_gpd = _use_gpd_force
                 else:
                     use_gpd = _has_gpd
 
                 if use_gpd:
                     geometry = []
                     for feat in features:
-                        if "geometry" not in feat or feat["geometry"]==None:
+                        if "geometry" not in feat or feat["geometry"]==None or len(feat["geometry"]["coordinates"])<2:
                             geometry.append(None)
                         else:
                             geometry.append(Point(feat["geometry"]["coordinates"][0], feat["geometry"]["coordinates"][1]))
 
                     df = gpd.GeoDataFrame(df, crs=4326, geometry=geometry)
                 else:
                     geometry = [feat["geometry"] if "geometry" in feat else None for feat in features]
@@ -1436,16 +1445,26 @@
         -------
         int
             Record count or number of rows in data request
         '''
 
         if where==None:
             where = self.__construct_where(year, opt_filter)
+
+        try:
+            results = self.client.get(self.data_set, where=where, select="count(*)")
+        except requests.HTTPError as e:
+            raise OPD_SocrataHTTPError(self.url, self.data_set, *e.args, _url_error_msg.format(self.url))
+        except Exception as e: 
+            if len(e.args)>0 and (e.args[0]=='Unknown response format: text/html' or \
+                "Read timed out" in e.args[0]):
+                raise OPD_SocrataHTTPError(self.url, self.data_set, *e.args, _url_error_msg.format(self.url))
+            else:
+                raise e  
             
-        results = self.client.get(self.data_set, where=where, select="count(*)")
         try:
             num_rows = float(results[0]["count"])
         except:
             num_rows = float(results[0]["count_1"]) # Value used in VT Shootings data
 
         return int(num_rows)
 
@@ -1648,21 +1667,23 @@
 
     if date_field != None and not hasattr(df[date_field], "dt"):
         with warnings.catch_warnings():
             # Ignore future warning about how this operation will be attempted to be done inplace:
             # In a future version, `df.iloc[:, i] = newvals` will attempt to set the values inplace instead of always setting a new array. 
             # To retain the old behavior, use either `df[df.columns[i]] = newvals` or, if columns are non-unique, `df.isetitem(i, newvals)`
             warnings.simplefilter("ignore", category=FutureWarning)
-            df.loc[:, date_field] = pd.to_datetime(df[date_field])
+            if date_field.lower()!="year":
+                df.loc[:, date_field] = pd.to_datetime(df[date_field])
     
     if year_filter != None and date_field != None:
         if isinstance(year_filter, list):
             df = df[(df[date_field].dt.year >= year_filter[0]) & (df[date_field].dt.year <= year_filter[1])]
         else:
-            df = df[df[date_field].dt.year == year_filter]
+            date_col = pd.to_datetime(df[date_field])
+            df = df[date_col.dt.year == year_filter]
 
     if agency != None and agency_field != None:
         df = df.query(agency_field + " = '" + agency + "'")
 
     return df
 
 
@@ -1706,20 +1727,8 @@
                 # Number of rows read is greater than user-requested limit
                 return ""
             self.rows_read += 1
             return next(self.reader)
         except StopIteration:
             if self.pbar:
                 self.bar.update(self.bar.total - self.bar.n)
-            return ""
-
-
-if __name__ == "__main__":
-    import time
-    _default_limit = 10000
-    start_time = time.time()
-    url = "https://gis.charlottenc.gov/arcgis/rest/services/CMPD/CMPD/MapServer/13/"
-    # url = 'https://services1.arcgis.com/zdB7qR0BtYrg0Xpl/arcgis/rest/services/ODC_CRIME_STOPS_P/FeatureServer/32'
-    date_field = 'YR'
-    years = _get_years("ArcGIS", url, date_field)
-    load_arcgis(url, date_field, [2020,2021])
-    print(f"Completed in {time.time()-start_time} seconds")
+            return ""
```

### Comparing `openpolicedata-0.5.1/openpolicedata/datasets.py` & `openpolicedata-0.5.2/openpolicedata/datasets.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.1/openpolicedata/defs.py` & `openpolicedata-0.5.2/openpolicedata/defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,17 @@
     CRASHES = ("CRASHES", "Traffic crashes")
     CRASHES_CIVILIANS = ("CRASHES - CIVILIANS",
         "Crash data may be split into several tables due to the possibility that multiple "+
         "civilians and vehicles may be involved in an incident. This table contains data on civilians.")
     CRASHES_INCIDENTS = ("CRASHES - INCIDENTS",
         "Crash data may be split into several tables due to the possibility that multiple "+
         "civilians and vehicles may be involved in an incident. This table contains data on the incident.")
+    CRASH_NONMOTORIST = ("CRASHES - NONMOTORIST",
+        "Crash data may be split into several tables due to the possibility that multiple "+
+        "civilians and vehicles may be involved in an incident. This table contains information on non-motorists involved in a crash.")
     CRASHES_VEHICLES = ("CRASHES - VEHICLES",
         "Crash data may be split into several tables due to the possibility that multiple "+
         "civilians and vehicles may be involved in an incident. This table contains data on vehicles    .")
     EMPLOYEE = ("EMPLOYEE","Demographic data of the police workforce")
     FIELD_CONTACTS = ("FIELD CONTACTS", "Consensual contacts between officers and the community.")
     INCIDENTS = ("INCIDENTS", "Crime incident reports")
     PEDESTRIAN = ("PEDESTRIAN STOPS","Stops of pedestrians based on 'reasonable suspicion'. May lead to a frisk.")
```

### Comparing `openpolicedata-0.5.1/openpolicedata/exceptions.py` & `openpolicedata-0.5.2/openpolicedata/exceptions.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.1/openpolicedata.egg-info/PKG-INFO` & `openpolicedata-0.5.2/openpolicedata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: openpolicedata
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Python library providing easy access to 276+ incident-level open datasets released by police departments including traffic stops, use of force, officer-involved shootings, and complaints data
 Home-page: https://github.com/openpolicedata/openpolicedata
 Author: Matt Sowd
 Author-email: openpolicedata@gmail.com
 Project-URL: Bug Tracker, https://github.com/openpolicedata/openpolicedata/issues
 Keywords: police data,use of force,traffic,stops,complaints,officer-involved,shootings,pandas,arcgis,socrata,police transparency,police accountability
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `openpolicedata-0.5.1/openpolicedata.egg-info/SOURCES.txt` & `openpolicedata-0.5.2/openpolicedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.1/setup.cfg` & `openpolicedata-0.5.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -37,44 +37,47 @@
 00000240: 2042 5344 204c 6963 656e 7365 0d0a 094f   BSD License...O
 00000250: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
 00000260: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
 00000270: 740d 0a09 5072 6f67 7261 6d6d 696e 6720  t...Programming 
 00000280: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
 00000290: 6f6e 203a 3a20 330d 0a09 5072 6f67 7261  on :: 3...Progra
 000002a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002b0: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
+000002b0: 3a20 5079 7468 6f6e 203a 3a20 332e 370d  : Python :: 3.7.
 000002c0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
 000002d0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002e0: 203a 3a20 332e 390d 0a09 5072 6f67 7261   :: 3.9...Progra
+000002e0: 203a 3a20 332e 380d 0a09 5072 6f67 7261   :: 3.8...Progra
 000002f0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000300: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-00000310: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000320: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000330: 6e20 3a3a 2033 2e31 310d 0a6b 6579 776f  n :: 3.11..keywo
-00000340: 7264 7320 3d20 0d0a 0970 6f6c 6963 6520  rds = ...police 
-00000350: 6461 7461 0d0a 0975 7365 206f 6620 666f  data...use of fo
-00000360: 7263 650d 0a09 7472 6166 6669 630d 0a09  rce...traffic...
-00000370: 7374 6f70 730d 0a09 636f 6d70 6c61 696e  stops...complain
-00000380: 7473 0d0a 096f 6666 6963 6572 2d69 6e76  ts...officer-inv
-00000390: 6f6c 7665 640d 0a09 7368 6f6f 7469 6e67  olved...shooting
-000003a0: 730d 0a09 7061 6e64 6173 0d0a 0961 7263  s...pandas...arc
-000003b0: 6769 730d 0a09 736f 6372 6174 610d 0a09  gis...socrata...
-000003c0: 706f 6c69 6365 2074 7261 6e73 7061 7265  police transpare
-000003d0: 6e63 790d 0a09 706f 6c69 6365 2061 6363  ncy...police acc
-000003e0: 6f75 6e74 6162 696c 6974 790d 0a0d 0a5b  ountability....[
-000003f0: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
-00000400: 655f 6469 7220 3d20 0d0a 093d 202e 0d0a  e_dir = ...= ...
-00000410: 7061 636b 6167 6573 203d 206f 7065 6e70  packages = openp
-00000420: 6f6c 6963 6564 6174 610d 0a70 7974 686f  olicedata..pytho
-00000430: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000440: 2e37 0d0a 696e 7374 616c 6c5f 7265 7175  .7..install_requ
-00000450: 6972 6573 203d 200d 0a09 6f70 656e 7079  ires = ...openpy
-00000460: 786c 0d0a 096e 756d 7079 0d0a 0970 616e  xl...numpy...pan
-00000470: 6461 730d 0a09 7079 7072 6f6a 0d0a 0972  das...pyproj...r
-00000480: 6170 6964 6675 7a7a 0d0a 0972 6571 7565  apidfuzz...reque
-00000490: 7374 730d 0a09 736f 6461 7079 0d0a 0974  sts...sodapy...t
-000004a0: 7164 6d0d 0a09 786c 7264 0d0a 0d0a 5b6f  qdm...xlrd....[o
-000004b0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-000004c0: 6669 6e64 5d0d 0a77 6865 7265 203d 202e  find]..where = .
-000004d0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000004e0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-000004f0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000300: 3a20 5079 7468 6f6e 203a 3a20 332e 390d  : Python :: 3.9.
+00000310: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000320: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000330: 203a 3a20 332e 3130 0d0a 0950 726f 6772   :: 3.10...Progr
+00000340: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000350: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000360: 310d 0a6b 6579 776f 7264 7320 3d20 0d0a  1..keywords = ..
+00000370: 0970 6f6c 6963 6520 6461 7461 0d0a 0975  .police data...u
+00000380: 7365 206f 6620 666f 7263 650d 0a09 7472  se of force...tr
+00000390: 6166 6669 630d 0a09 7374 6f70 730d 0a09  affic...stops...
+000003a0: 636f 6d70 6c61 696e 7473 0d0a 096f 6666  complaints...off
+000003b0: 6963 6572 2d69 6e76 6f6c 7665 640d 0a09  icer-involved...
+000003c0: 7368 6f6f 7469 6e67 730d 0a09 7061 6e64  shootings...pand
+000003d0: 6173 0d0a 0961 7263 6769 730d 0a09 736f  as...arcgis...so
+000003e0: 6372 6174 610d 0a09 706f 6c69 6365 2074  crata...police t
+000003f0: 7261 6e73 7061 7265 6e63 790d 0a09 706f  ransparency...po
+00000400: 6c69 6365 2061 6363 6f75 6e74 6162 696c  lice accountabil
+00000410: 6974 790d 0a0d 0a5b 6f70 7469 6f6e 735d  ity....[options]
+00000420: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
+00000430: 0d0a 093d 202e 0d0a 7061 636b 6167 6573  ...= ...packages
+00000440: 203d 206f 7065 6e70 6f6c 6963 6564 6174   = openpolicedat
+00000450: 610d 0a70 7974 686f 6e5f 7265 7175 6972  a..python_requir
+00000460: 6573 203d 203e 3d33 2e37 0d0a 696e 7374  es = >=3.7..inst
+00000470: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
+00000480: 0a09 6f70 656e 7079 786c 0d0a 096e 756d  ..openpyxl...num
+00000490: 7079 0d0a 0970 616e 6461 730d 0a09 7079  py...pandas...py
+000004a0: 7072 6f6a 0d0a 0972 6170 6964 6675 7a7a  proj...rapidfuzz
+000004b0: 0d0a 0972 6571 7565 7374 730d 0a09 736f  ...requests...so
+000004c0: 6461 7079 0d0a 0974 7164 6d0d 0a09 786c  dapy...tqdm...xl
+000004d0: 7264 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  rd....[options.p
+000004e0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+000004f0: 6865 7265 203d 202e 0d0a 0d0a 5b65 6767  here = .....[egg
+00000500: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000510: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000520: 2030 0d0a 0d0a                            0....
```

### Comparing `openpolicedata-0.5.1/tests/test_data_loaders.py` & `openpolicedata-0.5.2/tests/test_data_loaders.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,36 +46,36 @@
         year = 2019
         count = loader.get_count(year=year)
 
         r = requests.get(f"https://phl.carto.com/api/v2/sql?q=SELECT count(*) FROM {dataset} WHERE {date_field} >= '{year}-01-01' AND {date_field} < '{year+1}-01-01'")
         r.raise_for_status()
         assert count==r.json()["rows"][0]["count"]
 
-        df = loader.load(year=year)
+        df = loader.load(year=year, pbar=False)
 
         offset = 1
         nrows = count - 2
-        df_offset = loader.load(year=year, nrows=nrows, offset=1)
+        df_offset = loader.load(year=year, nrows=nrows, offset=1, pbar=False)
 
         assert df_offset.equals(df.iloc[offset:offset+nrows].reset_index(drop=True))
 
-        df_offset = loader.load(year=year, offset=1)
+        df_offset = loader.load(year=year, offset=1, pbar=False)
         assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
 
         r = requests.get(f"https://phl.carto.com/api/v2/sql?format=GeoJSON&q=SELECT * FROM {dataset} WHERE {date_field} >= '{year}-01-01' AND {date_field} < '{year+1}-01-01'")
         features = r.json()["features"]
         df_comp= pd.DataFrame.from_records([x["properties"] for x in features])
         df_comp[date_field] = pd.to_datetime(df_comp[date_field])
         
         try:
             import geopandas as gpd
             from shapely.geometry import Point
             geometry = []
             for feat in features:
-                if "geometry" not in feat or feat["geometry"]==None:
+                if "geometry" not in feat or feat["geometry"]==None or len(feat["geometry"]["coordinates"])<2:
                     geometry.append(None)
                 else:
                     geometry.append(Point(feat["geometry"]["coordinates"][0], feat["geometry"]["coordinates"][1]))
 
             df_comp = gpd.GeoDataFrame(df_comp, crs=4326, geometry=geometry)
         except:
             geometry = [feat["geometry"] if "geometry" in feat else None for feat in features]
@@ -84,15 +84,15 @@
         assert df.equals(df_comp)
 
         data_loaders._default_limit = lim
 
         if data_loaders._has_gpd:
             assert type(df) == gpd.GeoDataFrame
             data_loaders._has_gpd = False
-            df = loader.load(year=year, nrows=nrows)
+            df = loader.load(year=year, nrows=nrows, pbar=False)
             data_loaders._has_gpd = True
             assert isinstance(df, pd.DataFrame)
 
         url2 = "https://phl.carto.com/api/v2/sql?"
         loader2 = data_loaders.Carto(url2, dataset, date_field)
         assert loader.url==loader2.url
 
@@ -183,23 +183,24 @@
         assert set(df.columns) == set(layer_query_result.columns)
         assert len(layer_query_result) == count
         df = df[layer_query_result.columns]
 
         assert layer_query_result.equals(df)
 
 
-    def test_arcgis_legacy_server(self, csvfile, source, last, skip, loghtml):
-        url = "https://opendata.baltimorecity.gov/egis/rest/services/Hosted/911_Calls_For_Service_2017_csv/FeatureServer/0" 
-
-        gis = data_loaders.Arcgis(url)
-        gis.load(nrows=1)
-
-        url = "https://xmaps.indy.gov/arcgis/rest/services/OpenData/OpenData_NonSpatial/MapServer/5/" 
-        gis = data_loaders.Arcgis(url)
-        gis.load(nrows=1)
+    # No datasets currently trigger usage of the legacy server code
+    # def test_arcgis_legacy_server(self, csvfile, source, last, skip, loghtml):
+    #     url = "https://egis.baltimorecity.gov/egis/rest/services/GeoSpatialized_Tables/Arrest/FeatureServer/0/" 
+
+    #     gis = data_loaders.Arcgis(url)
+    #     gis.load(nrows=1)
+
+    #     url = "https://xmaps.indy.gov/arcgis/rest/services/OpenData/OpenData_NonSpatial/MapServer/5/" 
+    #     gis = data_loaders.Arcgis(url)
+    #     gis.load(nrows=1)
 
 
     def test_arcgis_geopandas(self, csvfile, source, last, skip, loghtml):
         if _has_gpd:
             url = "https://services1.arcgis.com/zdB7qR0BtYrg0Xpl/arcgis/rest/services/ODC_CRIME_STOPS_P/FeatureServer/32/"
             date_field = "TIME_PHONEPICKUP"
             year_filter = 2020
@@ -240,40 +241,40 @@
     def test_socrata_pandas(self, csvfile, source, last, skip, loghtml):
         data_loaders._use_gpd_force = False
         url = "data.montgomerycountymd.gov"
         data_set = "usip-62e2"
         date_field = "created_dt"
         year = 2020
         loader = data_loaders.Socrata(url=url, data_set=data_set, date_field=date_field)
-        df = loader.load(year=year)
+        df = loader.load(year=year, pbar=False)
         count = loader.get_count(year=year)
 
         # Reset
         data_loaders._use_gpd_force = None
 
         assert type(df) == pd.DataFrame
         assert len(df) == count
 
     def test_socrata(self, csvfile, source, last, skip, loghtml):
         lim = data_loaders._default_limit
         data_loaders._default_limit = 500
         url = "data.austintexas.gov"
         data_set = "sc8s-w4ka"
         loader = data_loaders.Socrata(url, data_set)
-        df =loader.load()
+        df =loader.load(pbar=False)
         count = loader.get_count()
 
         offset = 1
         nrows = len(df)-offset-1
-        df_offset = loader.load(offset=offset,nrows=nrows)
+        df_offset = loader.load(offset=offset,nrows=nrows, pbar=False)
         assert set(df.columns)==set(df_offset.columns)
         df_offset = df_offset[df.columns]
         assert df_offset.equals(df.iloc[offset:nrows+offset].reset_index(drop=True))
 
-        df_offset = loader.load(offset=offset)
+        df_offset = loader.load(offset=offset, pbar=False)
         assert set(df.columns)==set(df_offset.columns)
         df_offset = df_offset[df.columns]
         assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
         
         data_loaders._default_limit = lim
 
         client = data_loaders.SocrataClient(url, data_loaders.default_sodapy_key, timeout=60)
@@ -283,26 +284,27 @@
         assert len(df) == count
         assert rows.equals(df)
 
     def test_csv(self, csvfile, source, last, skip, loghtml):
         url = "https://www.denvergov.org/media/gis/DataCatalog/denver_police_officer_involved_shootings/csv/denver_police_officer_involved_shootings.csv"
         date_field = "INCIDENT_DATE"
         loader = data_loaders.Csv(url, date_field=date_field)
-        df = loader.load()
+        df = loader.load(pbar=False)
 
         offset = 1
         nrows = len(df)-offset-1
-        df_offset = loader.load(offset=offset,nrows=nrows)
+        df_offset = loader.load(offset=offset,nrows=nrows, pbar=False)
         assert df_offset.equals(df.iloc[offset:nrows+offset].reset_index(drop=True))
         
-        df_offset = loader.load(offset=offset)
+        df_offset = loader.load(offset=offset, pbar=False)
         assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
 
         df_comp = pd.read_csv(url)
         df_comp = df_comp.astype({date_field: 'datetime64[ns]'})
+        df = df.astype({date_field: 'datetime64[ns]'})
 
         count = loader.get_count()
         assert len(df_comp) == count
 
         assert df_comp.equals(df)
 
         with pytest.raises(ValueError):
@@ -320,34 +322,34 @@
         assert df_comp.equals(df)
 
 
     def test_csv_year_filter(self, csvfile, source, last, skip, loghtml):
         url = "https://www.denvergov.org/media/gis/DataCatalog/denver_police_officer_involved_shootings/csv/denver_police_officer_involved_shootings.csv"
         loader = data_loaders.Csv(url, date_field="INCIDENT_DATE")
         year = 2020
-        df = loader.load(year=year)
+        df = loader.load(year=year, pbar=False)
         with pytest.raises(ValueError):
             count = loader.get_count(year=year)
 
         count = loader.get_count(year=year, force=True)
         assert len(df) == count
 
 
     def test_excel(self, csvfile, source, last, skip, loghtml):
         url = "https://www.norristown.org/DocumentCenter/View/1789/2017-2018-Use-of-Force"
         date_field = "Date"
         loader = data_loaders.Excel(url, date_field=date_field)
-        df = loader.load()
+        df = loader.load(pbar=False)
 
         offset = 1
         nrows = len(df)-offset-1
-        df_offset = loader.load(offset=offset,nrows=nrows)
+        df_offset = loader.load(offset=offset,nrows=nrows, pbar=False)
         assert df_offset.equals(df.iloc[offset:nrows+offset].reset_index(drop=True))
 
-        df_offset = loader.load(offset=offset)
+        df_offset = loader.load(offset=offset, pbar=False)
         assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
 
         df_comp = pd.read_excel(url)
         df_comp = df_comp.convert_dtypes()
         df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
 
         with pytest.raises(ValueError):
@@ -362,15 +364,15 @@
 
         years = loader.get_years(force=True)
 
         df = df.astype({date_field: 'datetime64[ns]'})
         assert list(df[date_field].dt.year.sort_values(ascending=True).dropna().unique()) == years
 
         nrows = 7
-        df = loader.load(nrows=nrows)        
+        df = loader.load(nrows=nrows, pbar=False)        
         df_comp = pd.read_excel(url, nrows=nrows)
         df_comp = df_comp.convert_dtypes()
         df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
         assert df_comp.equals(df)
 
 
     def test_excel_year_sheets(self, csvfile, source, last, skip, loghtml):
@@ -385,57 +387,58 @@
         df_comp.drop(index=df_comp.index[0], inplace=True)
         df_comp.reset_index(drop=True, inplace=True)
         df_comp = df_comp.convert_dtypes()
         df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
         df_comp = df_comp.iloc[:, 1:]
 
         # Load all years
-        df_2014 = loader.load(year=2014)
+        df_2014 = loader.load(year=2014, pbar=False)
 
         assert df_comp.equals(df_2014)
 
         df_comp = pd.read_excel(url, sheet_name="2015")
         df_comp.columns= [x for x in df_comp.iloc[0]]
         df_comp.drop(index=df_comp.index[0], inplace=True)
         df_comp.reset_index(drop=True, inplace=True)
         df_comp = df_comp.convert_dtypes()
         df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
         df_comp = df_comp.iloc[:, 1:]
 
         # Load all years
-        df_2015 = loader.load(year=2015)
+        df_2015 = loader.load(year=2015, pbar=False)
 
         assert df_comp.equals(df_2015)
 
         # Note: There is no 2013 data
-        df_multi = loader.load(year=[2013,2015])
+        df_multi = loader.load(year=[2013,2015], pbar=False)
 
         assert df_multi.equals(pd.concat([df_2014, df_2015], ignore_index=True))
 
-        df = loader.load()
-        df_last = loader.load(year=years[-1])
+        df = loader.load(pbar=False)
+        df_last = loader.load(year=years[-1], pbar=False)
 
         assert df.head(len(df_multi)).equals(df_multi)
         assert df.tail(len(df_last)).reset_index(drop=True).equals(df_last.reset_index(drop=True))
 
         # Test loading to ensure that channel name changes are handled
         data_loaders.Excel("https://northamptonpd.com/images/ODP%20Spreadsheets/NPD_Use_of_Force_2014-2020_incident_level_data.xlsx").load()
 
     def test_excel_header(self, csvfile, source, last, skip, loghtml):
         url = "https://cms7files1.revize.com/sparksnv/Document_Center/Sparks%20Police/IA%20Data/2000-2022-SPD-OIS-Incidents%20(3).xlsx"
 
         loader = data_loaders.Excel(url)
-        df = loader.load()
+        df = loader.load(pbar=False)
 
         df_comp = pd.read_excel(url)
         df_comp.columns= [x for x in df_comp.iloc[3]]
         df_comp.drop(index=df_comp.index[0:4], inplace=True)
         df_comp.reset_index(drop=True, inplace=True)
         df_comp = df_comp.convert_dtypes()
         df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
+        df_comp = df_comp.dropna(thresh=10)
 
         assert(df_comp.equals(df))
 
 
     def test_excel_xls(self, csvfile, source, last, skip, loghtml):
         url = "http://gouda.beloitwi.gov/WebLink/0/edoc/66423/3Use%20of%20Force%202017%20-%20last%20updated%201-12-18.xls"
 
@@ -479,34 +482,33 @@
 
         df_comp = pd.read_excel(open(file_path_decrypted, 'rb'))
 
         os.remove(file_path)
         os.remove(file_path_decrypted)
 
         loader = data_loaders.Excel(url)
-        df = loader.load()
+        df = loader.load(pbar=False)
 
         df_comp = df_comp.convert_dtypes()
         df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
         assert df_comp.equals(df)
 
 if __name__ == "__main__":
     tp = TestProduct()
 
-    tp.test_arcgis_legacy_server(None,None,None,None,None)
-    tp.test_carto(None,None,None,None,None)
-    tp.test_arcgis(None,None,None,None,None)
-    tp.test_arcgis_geopandas(None,None,None,None,None)
-    tp.test_arcgis_pandas(None,None,None,None,None)
-    tp.test_csv(None,None,None,None,None)
-    tp.test_csv_year_filter(None,None,None,None,None)
-    tp.test_process_date_input_empty(None,None,None,None,None)
-    tp.test_process_date_too_many(None,None,None,None,None)
-    tp.test_process_dates_year_input_wrong_order(None,None,None,None,None)
-    tp.test_socrata(None,None,None,None,None)
-    tp.test_socrata_geopandas(None,None,None,None,None)
-    tp.test_socrata_pandas(None,None,None,None,None)
-    tp.test_excel(None,None,None,None,None)
-    tp.test_excel_year_sheets(None,None,None,None,None)
-    tp.test_excel_header(None,None,None,None,None)
+    # tp.test_carto(None,None,None,None,None)
+    # tp.test_arcgis(None,None,None,None,None)
+    # tp.test_arcgis_geopandas(None,None,None,None,None)
+    # tp.test_arcgis_pandas(None,None,None,None,None)
+    # tp.test_csv(None,None,None,None,None)
+    # tp.test_csv_year_filter(None,None,None,None,None)
+    # tp.test_process_date_input_empty(None,None,None,None,None)
+    # tp.test_process_date_too_many(None,None,None,None,None)
+    # tp.test_process_dates_year_input_wrong_order(None,None,None,None,None)
+    # tp.test_socrata(None,None,None,None,None)
+    # tp.test_socrata_geopandas(None,None,None,None,None)
+    # tp.test_socrata_pandas(None,None,None,None,None)
+    # tp.test_excel(None,None,None,None,None)
+    # tp.test_excel_year_sheets(None,None,None,None,None)
+    # tp.test_excel_header(None,None,None,None,None)
     tp.test_excel_xls(None,None,None,None,None)
     tp.test_excel_xls_protected(None,None,None,None,None)
```

### Comparing `openpolicedata-0.5.1/tests/test_datasets.py` & `openpolicedata-0.5.2/tests/test_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         for col in datasets.columns:
             if not col in can_have_nulls:
                 assert pd.isnull(datasets[col]).sum() == 0
 
     
     def test_check_state_names(self, csvfile, source, last, skip, loghtml):
         all_states = [
-            'Alabama', 'Alaska', 'American Samoa', 'Arizona', 'Arkansas', 'California', 'Colorado', 'Connecticut', 'Delaware', 'District Of Columbia',
+            'Alabama', 'Alaska', 'American Samoa', 'Arizona', 'Arkansas', 'California', 'Colorado', 'Connecticut', 'Delaware', 'District of Columbia',
             'Florida', 'Georgia', 'Guam', 'Hawaii', 'Idaho', 'Illinois', 'Indiana', 'Iowa', 'Kansas', 'Kentucky', 'Louisiana', 'Maine',
             'Maryland', 'Massachusetts', 'Michigan', 'Minnesota', 'Mississippi', 'Missouri', 'Montana', 'Nebraska', 'Nevada', 'New Hampshire',
             'New Jersey', 'New Mexico', 'New York', 'North Carolina', 'North Dakota', 'Northern Mariana Islands', 'Ohio', 'Oklahoma', 'Oregon',
             'Pennsylvania', 'Puerto Rico', 'Rhode Island', 'South Carolina', 'South Dakota', 'Tennessee', 'Texas', 'Utah', 'Vermont', 'Virgin Islands',
             'Virginia', 'Washington', 'West Virginia', 'Wisconsin', 'Wyoming'
         ]
 
@@ -193,9 +193,10 @@
         with pytest.warns(UserWarning):
             opd.datasets.summary_by_table_type()
         
         
 
 if __name__ == "__main__":
     csvfile = None
-    # csvfile = "C:\\Users\\matth\\repos\\opd-data\\opd_source_table.csv"
-    TestDatasets().test_summary_functions(csvfile,None,None,None,None)
+    csvfile = "C:\\Users\\matth\\repos\\opd-data\\opd_source_table.csv"
+    TestDatasets().test_years_multi(csvfile,None,None,None,None)
+    TestDatasets().test_table_types(csvfile,None,None,None,None)
```

### Comparing `openpolicedata-0.5.1/tests/test_opd_data1.py` & `openpolicedata-0.5.2/tests/test_opd_data1.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 		agency = "Arlington County Police Department"
 		opt_filter = src.datasets.iloc[0]["agency_field"] + " LIKE '%" + agency + "%'"
 		year = 2021
 		assert src.get_count(year=year, agency=agency) == loader.get_count(year=year, opt_filter=opt_filter)
 
 		print("Testing ArcGIS source")
 		src = data.Source("Charlotte-Mecklenburg")
-		count = src.get_count(table_type="EMPLOYEE")
+		count = src.get_count(year="NONE", table_type="EMPLOYEE")
 
 		url = "https://gis.charlottenc.gov/arcgis/rest/services/CMPD/CMPD/MapServer/16/"
 		gis = data_loaders.Arcgis(url)
 		assert count == gis.get_count()
 
 		print("Testing CSV source")
 		src = data.Source("Denver")
@@ -204,14 +204,18 @@
 	      ("Philadelphia", 2019, "OFFICER-INVOLVED SHOOTINGS", 500),
 	      ("Charlotte-Mecklenburg", "NONE", "Employee", 1000),
 		  ("Austin", 2012, "USE OF FORCE", 1000)]
 
 		for ds in datasets:
 			src = data.Source(ds[0])
 			df = src.load_from_url(ds[1], ds[2]).table
+			with warnings.catch_warnings():
+				warnings.filterwarnings("ignore",category=RuntimeWarning)
+				df = df.convert_dtypes()
+
 			offset = 0
 			for t in src.load_from_url_gen(ds[1], ds[2], nbatch=ds[3], force=True):
 				df_cur = df.iloc[offset:offset+len(t.table)].reset_index(drop=True)
 				df2 = t.table.copy()
 				if set(df.columns)!=set(df2.columns):
 					# Expecting that a column was not returned because it is empty in the subset requested in this iteration
 					assert len(df2.columns)<len(df.columns)
@@ -279,21 +283,21 @@
 					f.write("\n")
 
 if __name__ == "__main__":
 	# For testing
 	tp = TestData()
 	# (self, csvfile, source, last, skip, loghtml)
 	csvfile = None
-	# csvfile = r"..\opd-data\opd_source_table.csv"
+	csvfile = r"..\opd-data\opd_source_table.csv"
 	last = None
-	# last = 631-618+1
+	# last = 863-784+1
 	skip = None
-	skip = "Fayetteville,Seattle"
+	# skip = "Fayetteville,Seattle"
 	source = None
-	# source = "Philadelphia"
-	tp.test_load_gen(csvfile, source, last, skip, None) 
-	tp.check_table_type_warning(csvfile, source, last, skip, None) 
-	tp.test_source_download_limitable(csvfile, source, last, skip, None) 
+	# source = "Mesa"
+	# tp.check_table_type_warning(csvfile, source, last, skip, None) 
+	# tp.test_source_download_limitable(csvfile, source, last, skip, None) 
 	tp.test_check_version(csvfile, None, last, skip, None) 
-	tp.test_get_count(csvfile, None, last, skip, None)
-	tp.test_offsets_and_nrows(csvfile, source, last, skip, None) 
+	# tp.test_get_count(csvfile, None, last, skip, None)
+	# tp.test_offsets_and_nrows(csvfile, source, last, skip, None) 
+	# tp.test_load_gen(csvfile, source, last, skip, None)
```

### Comparing `openpolicedata-0.5.1/tests/test_opd_data2.py` & `openpolicedata-0.5.2/tests/test_opd_data2.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,19 +227,19 @@
 					f.write("\n")
 
 if __name__ == "__main__":
 	# For testing
 	tp = TestData()
 	# (self, csvfile, source, last, skip, loghtml)
 	csvfile = None
-	csvfile = r"..\opd-data\opd_source_table.csv"
+	csvfile = os.path.join("..","opd-data","opd_source_table.csv")
 	last = None
-	last = 633-501+1
+	last = 863-791+1
 	source = None
-	# source = "Detroit"
+	# source = "Washington D.C."
 	skip = None
-	skip = "Fayetteville,Seattle"
+	# skip = "Fayetteville,Seattle"
 	tp.test_get_years(csvfile, source, last, skip, None)
-	tp.test_get_agencies(csvfile, None, None, skip, None)
-	tp.test_get_agencies_name_match(csvfile, None, None, skip, None)
-	tp.test_agency_filter(csvfile, None, None, skip, None)
-	tp.test_to_csv(csvfile, None, None, skip, None)
+	# tp.test_get_agencies(csvfile, None, None, skip, None)
+	# tp.test_get_agencies_name_match(csvfile, None, None, skip, None)
+	# tp.test_agency_filter(csvfile, None, None, skip, None)
+	# tp.test_to_csv(csvfile, None, None, skip, None)
```

### Comparing `openpolicedata-0.5.1/tests/test_opd_data3.py` & `openpolicedata-0.5.2/tests/test_opd_data3.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         datasets.datasets = datasets._build(csvfile)
 
     return datasets.query()
 
 class TestData:
 	@pytest.mark.slow(reason="This is a slow test that should be run before a major commit.")
 	def test_load_year(self, csvfile, source, last, skip, loghtml):
+		max_count = 1e5
 		if last == None:
 			last = float('inf')
 		datasets = get_datasets(csvfile)
 		# Test that filtering for a year works at the boundaries
 		if skip != None:
 			skip = skip.split(",")
 			skip = [x.strip() for x in skip]
@@ -130,23 +131,25 @@
 				else:
 					years = years[:1]
 
 			for year in years:
 				print(f"Testing for year {year}")
 
 				table = src.load_from_url(year, datasets.iloc[i]["TableType"], 
-										agency=agency, pbar=False)
+										agency=agency, pbar=False, nrows=max_count)
 
 				sleep(sleep_time)
 
 				if table._date_field == None or datasets.iloc[i]["DataType"]==DataType.EXCEL.value or \
 					table._date_field.lower()=="year":
 					continue
 
 				dts = table.table[table._date_field]
+				# Remove all non-datestamps
+				dts = dts[dts.apply(lambda x: isinstance(x,pd._libs.tslibs.timestamps.Timestamp))].convert_dtypes()
 				dts = dts.sort_values(ignore_index=True)
 
 				all_years = dts.dt.year.unique().tolist()
 				
 				try:
 					assert len(all_years) == 1
 				except AssertionError as e:
@@ -181,29 +184,33 @@
 					else:
 						raise
 				except:
 					raise
 
 				sleep(sleep_time)
 				dts_start = table_start.table[table._date_field]
-
+				dts_start = dts_start[dts_start.apply(lambda x: isinstance(x,pd._libs.tslibs.timestamps.Timestamp))].convert_dtypes()
 				dts_start = dts_start.sort_values(ignore_index=True, na_position="first")
 
 				# If this isn't true then the stop date is too early
 				assert dts_start.iloc[-1].year == year
 
 				# Find first value date in year
 				dts_start = dts_start[dts_start.dt.year == year]
 				try:
 					assert dts.iloc[0] == dts_start.iloc[0]
 				except AssertionError as e:
 					# See comments in above try/except
 					assert dts.iloc[0] <= datetime.strptime(f"{year}-01-01 08:00:00", "%Y-%m-%d %H:%M:%S")
 				except:
 					raise(e)
+				
+				if len(table.table) == max_count:
+					# Whole dataset was not read. Don't compare to latest data in the year
+					continue
 
 				start_date = datetime.strftime(dts.iloc[-1]-timedelta(days=1), "%Y-%m-%d")
 				stop_date  = str(year+1) + "-01-10"  
 
 				table_stop = src.load_from_url([start_date, stop_date], datasets.iloc[i]["TableType"], 
 												agency=agency, pbar=False)
 				sleep(sleep_time)
@@ -331,14 +338,14 @@
 if __name__ == "__main__":
 	# For testing
 	tp = TestData()
 	# (self, csvfile, source, last, skip, loghtml)
 	csvfile = None
 	csvfile = r"..\opd-data\opd_source_table.csv"
 	last = None
-	# last = 607-93
+	# last = 860-392+1
 	skip = None
-	# skip = "Bloomington"
+	skip = "Chicago, Mesa"
 	source = None
-	source = "Philadelphia"
+	source = "Detroit"
 	tp.test_load_year(csvfile, source, last, skip, None)
-	tp.test_source_download_not_limitable(csvfile, source, last, skip, None)
+	# tp.test_source_download_not_limitable(csvfile, source, last, skip, None)
```

