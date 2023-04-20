# Comparing `tmp/libera_utils-2.1.0rc0.tar.gz` & `tmp/libera_utils-2.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libera_utils-2.1.0rc0.tar", max compression
+gzip compressed data, was "libera_utils-2.1.0rc1.tar", max compression
```

## Comparing `libera_utils-2.1.0rc0.tar` & `libera_utils-2.1.0rc1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1410 2023-04-20 20:33:03.948878 libera_utils-2.1.0rc0/CHANGES.md
--rw-r--r--   0        0        0     1465 2023-01-31 20:56:19.358288 libera_utils-2.1.0rc0/LICENSE
--rw-r--r--   0        0        0     1416 2023-04-03 23:48:10.022450 libera_utils-2.1.0rc0/README.md
--rw-r--r--   0        0        0       54 2023-02-07 21:10:06.403935 libera_utils-2.1.0rc0/libera_utils/__init__.py
--rw-r--r--   0        0        0       95 2023-04-20 20:30:46.629417 libera_utils-2.1.0rc0/libera_utils/backports/__init__.py
--rw-r--r--   0        0        0    78894 2023-04-20 20:30:46.630392 libera_utils-2.1.0rc0/libera_utils/backports/enum_3_11.py
--rw-r--r--   0        0        0     5124 2023-04-03 23:48:10.023492 libera_utils-2.1.0rc0/libera_utils/cli.py
--rw-r--r--   0        0        0     4916 2023-04-03 23:48:10.023746 libera_utils-2.1.0rc0/libera_utils/config.py
--rw-r--r--   0        0        0     1940 2023-01-31 20:56:19.381102 libera_utils-2.1.0rc0/libera_utils/data/config.json
--rw-r--r--   0        0        0    14209 2022-09-23 15:27:25.065932 libera_utils-2.1.0rc0/libera_utils/data/jpss1_geolocation_xtce_v1.xml
--rw-r--r--   0        0        0     7522 2022-09-23 15:27:25.067154 libera_utils-2.1.0rc0/libera_utils/data/spice/earth_assoc_itrf93.tf
--rw-r--r--   0        0        0     1608 2022-09-23 15:27:25.068514 libera_utils-2.1.0rc0/libera_utils/data/spice/jpss_sclk_v01.tsc
--rw-r--r--   0        0        0     7990 2022-09-23 15:27:25.069901 libera_utils-2.1.0rc0/libera_utils/data/spice/libera_fk_v01.tf
--rw-r--r--   0        0        0     1359 2023-02-07 21:10:06.406223 libera_utils-2.1.0rc0/libera_utils/db/__init__.py
--rw-r--r--   0        0        0     6127 2023-02-07 21:10:06.407492 libera_utils-2.1.0rc0/libera_utils/db/database.py
--rw-r--r--   0        0        0     3924 2023-01-31 20:56:19.384792 libera_utils-2.1.0rc0/libera_utils/db/mixins.py
--rw-r--r--   0        0        0     7833 2023-01-31 20:56:19.385945 libera_utils-2.1.0rc0/libera_utils/db/models.py
--rw-r--r--   0        0        0    19390 2022-09-23 15:27:25.074690 libera_utils-2.1.0rc0/libera_utils/geolocation.py
--rw-r--r--   0        0        0        0 2022-09-23 15:27:25.074796 libera_utils-2.1.0rc0/libera_utils/io/__init__.py
--rw-r--r--   0        0        0     1581 2022-09-23 15:27:25.076003 libera_utils-2.1.0rc0/libera_utils/io/caching.py
--rw-r--r--   0        0        0    21721 2023-04-03 23:48:10.024153 libera_utils-2.1.0rc0/libera_utils/io/construction_record.py
--rw-r--r--   0        0        0    32093 2023-04-20 20:30:46.631652 libera_utils-2.1.0rc0/libera_utils/io/filenaming.py
--rw-r--r--   0        0        0     1856 2023-01-31 20:56:19.390630 libera_utils-2.1.0rc0/libera_utils/io/hdf.py
--rw-r--r--   0        0        0     8596 2023-04-03 23:48:10.025919 libera_utils-2.1.0rc0/libera_utils/io/manifest.py
--rw-r--r--   0        0        0     7380 2023-04-03 23:48:10.026152 libera_utils-2.1.0rc0/libera_utils/io/packet_ingest.py
--rw-r--r--   0        0        0     7262 2023-04-03 23:48:10.026427 libera_utils-2.1.0rc0/libera_utils/io/smart_open.py
--rw-r--r--   0        0        0    17414 2023-04-20 20:30:46.633307 libera_utils-2.1.0rc0/libera_utils/kernel_maker.py
--rw-r--r--   0        0        0     6239 2023-01-31 20:56:19.393238 libera_utils-2.1.0rc0/libera_utils/logutil.py
--rw-r--r--   0        0        0     3417 2023-04-03 23:48:10.027250 libera_utils-2.1.0rc0/libera_utils/packets.py
--rw-r--r--   0        0        0     4620 2023-04-20 20:30:46.634535 libera_utils-2.1.0rc0/libera_utils/quality_flags.py
--rw-r--r--   0        0        0    17074 2022-09-23 15:27:25.084642 libera_utils-2.1.0rc0/libera_utils/spice_utils.py
--rw-r--r--   0        0        0     7482 2023-04-20 20:30:46.635212 libera_utils-2.1.0rc0/libera_utils/time.py
--rw-r--r--   0        0        0      203 2022-09-23 15:27:25.087434 libera_utils-2.1.0rc0/libera_utils/version.py
--rw-r--r--   0        0        0     1525 2023-04-20 20:46:20.133500 libera_utils-2.1.0rc0/pyproject.toml
--rw-r--r--   0        0        0     1436 1970-01-01 00:00:00.000000 libera_utils-2.1.0rc0/setup.py
--rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 libera_utils-2.1.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1410 2023-04-20 20:33:03.948878 libera_utils-2.1.0rc1/CHANGES.md
+-rw-r--r--   0        0        0     1465 2023-01-31 20:56:19.358288 libera_utils-2.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     1416 2023-04-03 23:48:10.022450 libera_utils-2.1.0rc1/README.md
+-rw-r--r--   0        0        0       54 2023-02-07 21:10:06.403935 libera_utils-2.1.0rc1/libera_utils/__init__.py
+-rw-r--r--   0        0        0       95 2023-04-20 20:30:46.629417 libera_utils-2.1.0rc1/libera_utils/backports/__init__.py
+-rw-r--r--   0        0        0    78894 2023-04-20 20:30:46.630392 libera_utils-2.1.0rc1/libera_utils/backports/enum_3_11.py
+-rw-r--r--   0        0        0     5124 2023-04-03 23:48:10.023492 libera_utils-2.1.0rc1/libera_utils/cli.py
+-rw-r--r--   0        0        0     4916 2023-04-03 23:48:10.023746 libera_utils-2.1.0rc1/libera_utils/config.py
+-rw-r--r--   0        0        0     1940 2023-01-31 20:56:19.381102 libera_utils-2.1.0rc1/libera_utils/data/config.json
+-rw-r--r--   0        0        0    14209 2022-09-23 15:27:25.065932 libera_utils-2.1.0rc1/libera_utils/data/jpss1_geolocation_xtce_v1.xml
+-rw-r--r--   0        0        0     7522 2022-09-23 15:27:25.067154 libera_utils-2.1.0rc1/libera_utils/data/spice/earth_assoc_itrf93.tf
+-rw-r--r--   0        0        0     1608 2022-09-23 15:27:25.068514 libera_utils-2.1.0rc1/libera_utils/data/spice/jpss_sclk_v01.tsc
+-rw-r--r--   0        0        0     7990 2022-09-23 15:27:25.069901 libera_utils-2.1.0rc1/libera_utils/data/spice/libera_fk_v01.tf
+-rw-r--r--   0        0        0     1359 2023-02-07 21:10:06.406223 libera_utils-2.1.0rc1/libera_utils/db/__init__.py
+-rw-r--r--   0        0        0     6127 2023-02-07 21:10:06.407492 libera_utils-2.1.0rc1/libera_utils/db/database.py
+-rw-r--r--   0        0        0     3924 2023-01-31 20:56:19.384792 libera_utils-2.1.0rc1/libera_utils/db/mixins.py
+-rw-r--r--   0        0        0     7833 2023-01-31 20:56:19.385945 libera_utils-2.1.0rc1/libera_utils/db/models.py
+-rw-r--r--   0        0        0    19390 2022-09-23 15:27:25.074690 libera_utils-2.1.0rc1/libera_utils/geolocation.py
+-rw-r--r--   0        0        0        0 2022-09-23 15:27:25.074796 libera_utils-2.1.0rc1/libera_utils/io/__init__.py
+-rw-r--r--   0        0        0     1581 2022-09-23 15:27:25.076003 libera_utils-2.1.0rc1/libera_utils/io/caching.py
+-rw-r--r--   0        0        0    21721 2023-04-03 23:48:10.024153 libera_utils-2.1.0rc1/libera_utils/io/construction_record.py
+-rw-r--r--   0        0        0    32155 2023-04-20 21:16:12.642534 libera_utils-2.1.0rc1/libera_utils/io/filenaming.py
+-rw-r--r--   0        0        0     1856 2023-01-31 20:56:19.390630 libera_utils-2.1.0rc1/libera_utils/io/hdf.py
+-rw-r--r--   0        0        0     8596 2023-04-03 23:48:10.025919 libera_utils-2.1.0rc1/libera_utils/io/manifest.py
+-rw-r--r--   0        0        0     7380 2023-04-03 23:48:10.026152 libera_utils-2.1.0rc1/libera_utils/io/packet_ingest.py
+-rw-r--r--   0        0        0     7262 2023-04-03 23:48:10.026427 libera_utils-2.1.0rc1/libera_utils/io/smart_open.py
+-rw-r--r--   0        0        0    17414 2023-04-20 20:30:46.633307 libera_utils-2.1.0rc1/libera_utils/kernel_maker.py
+-rw-r--r--   0        0        0     6239 2023-01-31 20:56:19.393238 libera_utils-2.1.0rc1/libera_utils/logutil.py
+-rw-r--r--   0        0        0     3417 2023-04-03 23:48:10.027250 libera_utils-2.1.0rc1/libera_utils/packets.py
+-rw-r--r--   0        0        0     4620 2023-04-20 20:30:46.634535 libera_utils-2.1.0rc1/libera_utils/quality_flags.py
+-rw-r--r--   0        0        0    17074 2022-09-23 15:27:25.084642 libera_utils-2.1.0rc1/libera_utils/spice_utils.py
+-rw-r--r--   0        0        0     7489 2023-04-20 21:16:12.634936 libera_utils-2.1.0rc1/libera_utils/time.py
+-rw-r--r--   0        0        0      203 2022-09-23 15:27:25.087434 libera_utils-2.1.0rc1/libera_utils/version.py
+-rw-r--r--   0        0        0     1526 2023-04-20 21:19:33.197709 libera_utils-2.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1436 1970-01-01 00:00:00.000000 libera_utils-2.1.0rc1/setup.py
+-rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 libera_utils-2.1.0rc1/PKG-INFO
```

### Comparing `libera_utils-2.1.0rc0/CHANGES.md` & `libera_utils-2.1.0rc1/CHANGES.md`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/LICENSE` & `libera_utils-2.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/README.md` & `libera_utils-2.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/backports/enum_3_11.py` & `libera_utils-2.1.0rc1/libera_utils/backports/enum_3_11.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/cli.py` & `libera_utils-2.1.0rc1/libera_utils/cli.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/config.py` & `libera_utils-2.1.0rc1/libera_utils/config.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/data/config.json` & `libera_utils-2.1.0rc1/libera_utils/data/config.json`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/data/jpss1_geolocation_xtce_v1.xml` & `libera_utils-2.1.0rc1/libera_utils/data/jpss1_geolocation_xtce_v1.xml`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/data/spice/earth_assoc_itrf93.tf` & `libera_utils-2.1.0rc1/libera_utils/data/spice/earth_assoc_itrf93.tf`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/data/spice/jpss_sclk_v01.tsc` & `libera_utils-2.1.0rc1/libera_utils/data/spice/jpss_sclk_v01.tsc`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/data/spice/libera_fk_v01.tf` & `libera_utils-2.1.0rc1/libera_utils/data/spice/libera_fk_v01.tf`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/db/__init__.py` & `libera_utils-2.1.0rc1/libera_utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/db/database.py` & `libera_utils-2.1.0rc1/libera_utils/db/database.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/db/mixins.py` & `libera_utils-2.1.0rc1/libera_utils/db/mixins.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/db/models.py` & `libera_utils-2.1.0rc1/libera_utils/db/models.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/geolocation.py` & `libera_utils-2.1.0rc1/libera_utils/geolocation.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/io/caching.py` & `libera_utils-2.1.0rc1/libera_utils/io/caching.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/io/construction_record.py` & `libera_utils-2.1.0rc1/libera_utils/io/construction_record.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/io/filenaming.py` & `libera_utils-2.1.0rc1/libera_utils/io/filenaming.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import os
 import re
 from types import SimpleNamespace
 from pathlib import Path
 # Installed
 from cloudpathlib import AnyPath, CloudPath
 # Local
-from libera_utils.time import PRINTABLE_TS_FORMAT, EDOS_TS_FORMAT
+from libera_utils.time import PRINTABLE_TS_FORMAT, NUMERIC_DOY_TS_FORMAT
 
-REVISION_TS_FORMAT = "r%y%j%H%M%S"
+REVISION_TS_FORMAT = f"r{NUMERIC_DOY_TS_FORMAT}"  # Just adds an r in front
 
 SPK_REGEX = re.compile(r"^libera_(?P<spk_object>jpss)"
                        r"_(?P<utc_start>[0-9]{8}t[0-9]{6})"
                        r"_(?P<utc_end>[0-9]{8}t[0-9]{6})"
                        r"_(?P<version>vM[0-9]*m[0-9]*p[0-9]*)"
                        r"_(?P<revision>r[0-9]{11})"
                        r"\.bsp$")
@@ -303,15 +303,15 @@
         """
         signal = signal if signal else ""
 
         return cls._fmt.format(id_char=id_char,
                                scid=scid,
                                first_apid=first_apid,
                                fill=fill,
-                               created_time=created_time.strftime(EDOS_TS_FORMAT),
+                               created_time=created_time.strftime(NUMERIC_DOY_TS_FORMAT),
                                numeric_id=numeric_id,
                                file_number=file_number,
                                extension=extension,
                                signal=signal)
 
     def _parse_filename_parts(self):
         """Parse the filename parts into objects from regex matched strings
@@ -322,15 +322,15 @@
             namespace object containing filename parts as parsed objects
         """
         d = self.regex_match(self.path)
         d['scid'] = int(d['scid'])
         d['first_apid'] = int(d['first_apid'])
         d['numeric_id'] = int(d['numeric_id'])
         d['file_number'] = int(d['file_number'])
-        d['created_time'] = datetime.strptime(d['created_time'], EDOS_TS_FORMAT)
+        d['created_time'] = datetime.strptime(d['created_time'], NUMERIC_DOY_TS_FORMAT)
         return SimpleNamespace(**d)
 
 
 class L1bFilename(AbstractValidFilename):
     """Filename validation class for L1b products"""
 
     _regex = LIBERA_L1B_REGEX
```

### Comparing `libera_utils-2.1.0rc0/libera_utils/io/hdf.py` & `libera_utils-2.1.0rc1/libera_utils/io/hdf.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/io/manifest.py` & `libera_utils-2.1.0rc1/libera_utils/io/manifest.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/io/packet_ingest.py` & `libera_utils-2.1.0rc1/libera_utils/io/packet_ingest.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/io/smart_open.py` & `libera_utils-2.1.0rc1/libera_utils/io/smart_open.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/kernel_maker.py` & `libera_utils-2.1.0rc1/libera_utils/kernel_maker.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/logutil.py` & `libera_utils-2.1.0rc1/libera_utils/logutil.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/packets.py` & `libera_utils-2.1.0rc1/libera_utils/packets.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/quality_flags.py` & `libera_utils-2.1.0rc1/libera_utils/quality_flags.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/spice_utils.py` & `libera_utils-2.1.0rc1/libera_utils/spice_utils.py`

 * *Files identical despite different names*

### Comparing `libera_utils-2.1.0rc0/libera_utils/time.py` & `libera_utils-2.1.0rc1/libera_utils/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 PRINTABLE_TS_REGEX = re.compile(r"^(?P<year>[0-9]{4})(?P<month>[0-9]{2})(?P<day>[0-9]{2})"
                                 r"[T|t]"
                                 r"(?P<hour>[0-9]{2})(?P<minute>[0-9]{2})(?P<second>[0-9]{2})$")
 
 PRINTABLE_TS_FORMAT = "%Y%m%dt%H%M%S"
 
-EDOS_TS_FORMAT = "%y%j%H%M%S"
+NUMERIC_DOY_TS_FORMAT = "%y%j%H%M%S"
 
 
 def et_2_timestamp(et: Union[float, Collection[float], np.ndarray],
                    fmt: str = '%Y%m%dt%H%M%S.%f') -> Union[str, Collection[str]]:
     """
     Convert ephemeris time to a custom formatted timestamp (default is lowercase version of ISO).
```

### Comparing `libera_utils-2.1.0rc0/pyproject.toml` & `libera_utils-2.1.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libera_utils"
-version = "2.1.0rc"
+version = "2.1.0rc1"
 description = "Utility package for Libera Science Data Processing and the Libera Science Data Center. Copyright 2022 University of Colorado."
 authors = [  # Alphabetical
     "Stephane Beland <stephane.beland@lasp.colorado.edu>",
     "Gavin Medley <gavin.medley@lasp.colorado.edu>",
     "Laura Sandoval <laura.sandoval@lasp.colorado.edu>",
     "Matt Watwood <matt.watwood@lasp.colorado.edu>"
 ]
```

### Comparing `libera_utils-2.1.0rc0/setup.py` & `libera_utils-2.1.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'xarray>=2023.1.0,<2024.0.0']
 
 entry_points = \
 {'console_scripts': ['libera-utils = libera_utils.cli:main']}
 
 setup_kwargs = {
     'name': 'libera-utils',
-    'version': '2.1.0rc0',
+    'version': '2.1.0rc1',
     'description': 'Utility package for Libera Science Data Processing and the Libera Science Data Center. Copyright 2022 University of Colorado.',
     'long_description': 'None',
     'author': 'Stephane Beland',
     'author_email': 'stephane.beland@lasp.colorado.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `libera_utils-2.1.0rc0/PKG-INFO` & `libera_utils-2.1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libera-utils
-Version: 2.1.0rc0
+Version: 2.1.0rc1
 Summary: Utility package for Libera Science Data Processing and the Libera Science Data Center. Copyright 2022 University of Colorado.
 License: BSD-3-Clause
 Author: Stephane Beland
 Author-email: stephane.beland@lasp.colorado.edu
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

