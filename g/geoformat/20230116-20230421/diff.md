# Comparing `tmp/geoformat-20230116.tar.gz` & `tmp/geoformat-20230421.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoformat-20230116.tar", last modified: Mon Jan 16 17:08:36 2023, max compression
+gzip compressed data, was "geoformat-20230421.tar", last modified: Fri Apr 21 13:15:47 2023, max compression
```

## Comparing `geoformat-20230116.tar` & `geoformat-20230421.tar`

### file list

```diff
@@ -1,240 +1,240 @@
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.168404 geoformat-20230116/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1305 2022-10-13 08:02:35.000000 geoformat-20230116/LICENSE
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20655 2023-01-16 17:08:36.164404 geoformat-20230116/PKG-INFO
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    19758 2023-01-03 15:06:35.000000 geoformat-20230116/README.md
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.724414 geoformat-20230116/geoformat/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    14558 2023-01-16 17:06:24.000000 geoformat-20230116/geoformat/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      280 2023-01-16 17:08:12.000000 geoformat-20230116/geoformat/_version.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.744414 geoformat-20230116/geoformat/conf/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/conf/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2044 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/conf/decorator.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      836 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/conf/driver_variable.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3625 2023-01-11 15:16:53.000000 geoformat-20230116/geoformat/conf/error_messages.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3832 2023-01-03 14:30:13.000000 geoformat-20230116/geoformat/conf/fields_variable.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1744 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/conf/format_data.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)       35 2022-12-12 09:38:12.000000 geoformat-20230116/geoformat/conf/geoformat_var.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3990 2023-01-03 14:19:37.000000 geoformat-20230116/geoformat/conf/geometry_variable.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4897 2023-01-03 14:30:13.000000 geoformat-20230116/geoformat/conf/path.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      700 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/conf/proj_var.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10042 2023-01-03 14:29:45.000000 geoformat-20230116/geoformat/conf/timer.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.744414 geoformat-20230116/geoformat/constraints/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/constraints/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1810 2022-11-24 15:49:21.000000 geoformat-20230116/geoformat/constraints/primary_key.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.812412 geoformat-20230116/geoformat/conversion/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/conversion/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1381 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/conversion/bbox_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4858 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/conversion/bytes_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7914 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/conversion/coordinates_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      992 2023-01-03 14:29:45.000000 geoformat-20230116/geoformat/conversion/datetime_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    46110 2023-01-03 14:30:13.000000 geoformat-20230116/geoformat/conversion/feature_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    16223 2023-01-03 14:30:13.000000 geoformat-20230116/geoformat/conversion/fields_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6898 2023-01-09 16:05:09.000000 geoformat-20230116/geoformat/conversion/geolayer_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    50975 2023-01-03 14:29:45.000000 geoformat-20230116/geoformat/conversion/geometry_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7331 2023-01-05 15:34:29.000000 geoformat-20230116/geoformat/conversion/metadata_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      701 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/conversion/precision_tolerance_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1732 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/conversion/segment_conversion.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.824412 geoformat-20230116/geoformat/db/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/db/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2070 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/db/db_request.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.824412 geoformat-20230116/geoformat/driver/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/driver/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2652 2023-01-03 14:30:13.000000 geoformat-20230116/geoformat/driver/common_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    13306 2023-01-03 14:30:13.000000 geoformat-20230116/geoformat/driver/csv_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    40428 2023-01-03 14:29:45.000000 geoformat-20230116/geoformat/driver/esri_shapefile_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    12370 2023-01-03 14:30:13.000000 geoformat-20230116/geoformat/driver/geojson_driver.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.824412 geoformat-20230116/geoformat/driver/ogr/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/driver/ogr/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    41141 2022-11-24 15:49:21.000000 geoformat-20230116/geoformat/driver/ogr/ogr_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     9889 2022-11-24 15:49:21.000000 geoformat-20230116/geoformat/driver/postgresql_driver.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.828412 geoformat-20230116/geoformat/explore_data/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/explore_data/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5345 2023-01-16 15:38:19.000000 geoformat-20230116/geoformat/explore_data/duplicate.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    16452 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/explore_data/print_data.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1403 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/explore_data/random_geometry.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.852411 geoformat-20230116/geoformat/geoprocessing/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1256 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/area.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.852411 geoformat-20230116/geoformat/geoprocessing/connectors/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/connectors/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2143 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/geoprocessing/connectors/operations.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    12104 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/connectors/predicates.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.856411 geoformat-20230116/geoformat/geoprocessing/generalization/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/geoprocessing/generalization/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2209 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/geoprocessing/generalization/ramer_douglas_peucker.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4989 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/geoprocessing/generalization/visvalingam_whyatt.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.856411 geoformat-20230116/geoformat/geoprocessing/geoparameters/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/geoparameters/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3396 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/geoprocessing/geoparameters/bbox.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      877 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/geoparameters/boundaries.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5335 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/geoparameters/lines.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1362 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/length.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    11567 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/line_merge.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.868411 geoformat-20230116/geoformat/geoprocessing/matrix/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/matrix/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5464 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/matrix/adjacency.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.868411 geoformat-20230116/geoformat/geoprocessing/measure/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/measure/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1328 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/geoprocessing/measure/area.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3560 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/geoprocessing/measure/distance.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      560 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/measure/length.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7282 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/merge_geometries.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7441 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/point_on_linestring.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3824 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/geoprocessing/simplify.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5237 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/geoprocessing/split.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2084 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/geoprocessing/union.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.868411 geoformat-20230116/geoformat/index/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/index/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.872411 geoformat-20230116/geoformat/index/attributes/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/index/attributes/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      670 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/index/attributes/hash.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.888410 geoformat-20230116/geoformat/index/geometry/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/index/geometry/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    14746 2022-11-24 15:49:21.000000 geoformat-20230116/geoformat/index/geometry/grid.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.888410 geoformat-20230116/geoformat/manipulation/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/manipulation/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2859 2022-11-24 15:49:21.000000 geoformat-20230116/geoformat/manipulation/feature_manipulation.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20815 2023-01-03 14:42:19.000000 geoformat-20230116/geoformat/manipulation/geolayer_manipulation.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10051 2023-01-03 14:30:13.000000 geoformat-20230116/geoformat/manipulation/metadata_manipulation.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.900410 geoformat-20230116/geoformat/obj/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/obj/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      774 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/obj/geometry.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.900410 geoformat-20230116/geoformat/processing/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/processing/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.924410 geoformat-20230116/geoformat/processing/data/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/geoformat/processing/data/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     9722 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/processing/data/clauses.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10536 2022-11-24 15:49:21.000000 geoformat-20230116/geoformat/processing/data/field_statistics.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.924410 geoformat-20230116/geoformat/processing/data/join/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230116/geoformat/processing/data/join/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    26996 2023-01-10 10:39:11.000000 geoformat-20230116/geoformat/processing/data/join/join.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    11975 2023-01-03 14:30:13.000000 geoformat-20230116/geoformat/processing/data/join/merge_objects.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5199 2022-11-24 15:49:21.000000 geoformat-20230116/geoformat/processing/data/union.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.740414 geoformat-20230116/geoformat.egg-info/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20655 2023-01-16 17:08:35.000000 geoformat-20230116/geoformat.egg-info/PKG-INFO
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7676 2023-01-16 17:08:35.000000 geoformat-20230116/geoformat.egg-info/SOURCES.txt
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        1 2023-01-16 17:08:35.000000 geoformat-20230116/geoformat.egg-info/dependency_links.txt
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)       16 2023-01-16 17:08:35.000000 geoformat-20230116/geoformat.egg-info/top_level.txt
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)       38 2023-01-16 17:08:36.168404 geoformat-20230116/setup.cfg
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1210 2022-09-13 14:34:13.000000 geoformat-20230116/setup.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.692415 geoformat-20230116/tests/
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.992408 geoformat-20230116/tests/data/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/data/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15423 2022-10-13 08:02:35.000000 geoformat-20230116/tests/data/coordinates.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    43859 2023-01-03 14:30:13.000000 geoformat-20230116/tests/data/features.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2394 2022-10-13 08:02:35.000000 geoformat-20230116/tests/data/fields_metadata.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)  9850700 2023-01-03 14:30:13.000000 geoformat-20230116/tests/data/geolayers.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    26458 2023-01-03 14:30:13.000000 geoformat-20230116/tests/data/geometries.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    58422 2022-09-13 14:34:13.000000 geoformat-20230116/tests/data/geometry_index.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1227 2022-10-13 08:02:35.000000 geoformat-20230116/tests/data/index.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      232 2022-09-13 14:34:13.000000 geoformat-20230116/tests/data/matrix.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5099 2023-01-03 14:30:13.000000 geoformat-20230116/tests/data/metadata.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      435 2022-09-13 14:34:13.000000 geoformat-20230116/tests/data/segments.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.992408 geoformat-20230116/tests/geoformat/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.992408 geoformat-20230116/tests/geoformat/conf/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/conf/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3617 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/conf/test_format_data.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     8633 2023-01-03 14:30:13.000000 geoformat-20230116/tests/geoformat/conf/test_path.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:35.992408 geoformat-20230116/tests/geoformat/constraints/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/constraints/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2987 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/constraints/test_primary_key.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.016407 geoformat-20230116/tests/geoformat/conversion/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/conversion/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2380 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/conversion/test_bbox_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17731 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/conversion/test_bytes_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17709 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/conversion/test_coordinates_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      986 2023-01-03 14:29:45.000000 geoformat-20230116/tests/geoformat/conversion/test_datetime_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   205565 2023-01-03 14:30:13.000000 geoformat-20230116/tests/geoformat/conversion/test_feature_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   161950 2023-01-03 14:30:13.000000 geoformat-20230116/tests/geoformat/conversion/test_fields_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)  5602810 2022-11-24 15:49:21.000000 geoformat-20230116/tests/geoformat/conversion/test_geolayer_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    92781 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/conversion/test_geometry_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    65479 2023-01-03 14:30:13.000000 geoformat-20230116/tests/geoformat/conversion/test_metadata_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1238 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/conversion/test_precision_tolerance_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3245 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/conversion/test_segment_conversion.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.016407 geoformat-20230116/tests/geoformat/db/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/db/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.024407 geoformat-20230116/tests/geoformat/driver/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/driver/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.028407 geoformat-20230116/tests/geoformat/driver/ogr/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/driver/ogr/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      369 2023-01-03 14:30:13.000000 geoformat-20230116/tests/geoformat/driver/ogr/compare_ogr_files.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1251 2023-01-03 14:29:45.000000 geoformat-20230116/tests/geoformat/driver/ogr/geolayer_to_geojson.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1263 2023-01-03 14:30:13.000000 geoformat-20230116/tests/geoformat/driver/ogr/geolayer_to_postgresql.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2155 2023-01-03 14:29:45.000000 geoformat-20230116/tests/geoformat/driver/ogr/geolayer_to_shapefile.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    16224 2023-01-03 14:29:45.000000 geoformat-20230116/tests/geoformat/driver/test_common_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    29687 2023-01-03 14:30:13.000000 geoformat-20230116/tests/geoformat/driver/test_csv_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   321121 2023-01-03 14:29:45.000000 geoformat-20230116/tests/geoformat/driver/test_esri_shapefile_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)  1461478 2023-01-03 14:30:13.000000 geoformat-20230116/tests/geoformat/driver/test_geojson_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   114134 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/driver/test_postgresql_driver.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.032407 geoformat-20230116/tests/geoformat/explore_data/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/explore_data/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17339 2023-01-16 16:20:06.000000 geoformat-20230116/tests/geoformat/explore_data/test_duplicate.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    66158 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/explore_data/test_print_data.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.060406 geoformat-20230116/tests/geoformat/geoprocessing/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/geoprocessing/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.064406 geoformat-20230116/tests/geoformat/geoprocessing/connectors/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/geoprocessing/connectors/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4728 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/connectors/test_operations.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15761 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/connectors/test_predicates.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.072406 geoformat-20230116/tests/geoformat/geoprocessing/generalization/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/generalization/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2176 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/generalization/test_ramer_douglas_peucker.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1845 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/generalization/test_visvalingam_whyatt.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.072406 geoformat-20230116/tests/geoformat/geoprocessing/geoparameters/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/geoprocessing/geoparameters/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3562 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/geoparameters/test_bbox.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      901 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/geoparameters/test_boundaries.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     9425 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/geoparameters/test_lines.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.084406 geoformat-20230116/tests/geoformat/geoprocessing/matrix/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/geoprocessing/matrix/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1645 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/matrix/test_adjacency.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.092406 geoformat-20230116/tests/geoformat/geoprocessing/measure/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/geoprocessing/measure/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2234 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/measure/test_area.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3736 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/measure/test_distance.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1525 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/measure/test_length.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1758 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/test_area.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2337 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/test_length.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15898 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/test_line_merge.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4976 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/test_merge_geometries.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4575 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/test_point_on_linestring.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    14514 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/test_simplify.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    53164 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/test_split.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1387 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/geoprocessing/test_union.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.096406 geoformat-20230116/tests/geoformat/index/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/index/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.104405 geoformat-20230116/tests/geoformat/index/attributes/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/index/attributes/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1279 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/index/attributes/test_hash.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.104405 geoformat-20230116/tests/geoformat/index/geometry/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/index/geometry/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15928 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/index/geometry/test_grid.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.120405 geoformat-20230116/tests/geoformat/manipulation/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/manipulation/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    12109 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/manipulation/test_feature_manipulation.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   256166 2023-01-03 14:30:13.000000 geoformat-20230116/tests/geoformat/manipulation/test_geolayer_manipulation.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    38639 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/manipulation/test_metadata_manipulation.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.124405 geoformat-20230116/tests/geoformat/obj/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/obj/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1928 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/obj/test_geometry.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.124405 geoformat-20230116/tests/geoformat/processing/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/processing/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.136405 geoformat-20230116/tests/geoformat/processing/data/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/geoformat/processing/data/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.144404 geoformat-20230116/tests/geoformat/processing/data/join/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/processing/data/join/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   608012 2023-01-10 10:39:51.000000 geoformat-20230116/tests/geoformat/processing/data/join/test_join.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20394 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/processing/data/join/test_merge_objects.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6946 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/processing/data/test_clauses.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7537 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/processing/data/test_field_statistics.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6065 2022-10-13 08:02:35.000000 geoformat-20230116/tests/geoformat/processing/data/test_union.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.152404 geoformat-20230116/tests/inspector/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230116/tests/inspector/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17877 2023-01-03 14:30:13.000000 geoformat-20230116/tests/inspector/geoformat_inspector.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.156404 geoformat-20230116/tests/perf/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230116/tests/perf/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10403 2023-01-03 14:30:13.000000 geoformat-20230116/tests/perf/compare_func.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-01-16 17:08:36.156404 geoformat-20230116/tests/utils/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230116/tests/utils/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1379 2023-01-03 14:29:45.000000 geoformat-20230116/tests/utils/compare.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6701 2023-01-03 14:30:13.000000 geoformat-20230116/tests/utils/tests_utils.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.504982 geoformat-20230421/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1305 2022-10-13 08:02:35.000000 geoformat-20230421/LICENSE
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20635 2023-04-21 13:15:47.500982 geoformat-20230421/PKG-INFO
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    19758 2023-04-21 13:10:35.000000 geoformat-20230421/README.md
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.356985 geoformat-20230421/geoformat/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    14558 2023-01-16 19:36:49.000000 geoformat-20230421/geoformat/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      280 2023-04-21 13:15:34.000000 geoformat-20230421/geoformat/_version.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.360985 geoformat-20230421/geoformat/conf/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conf/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2044 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conf/decorator.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      836 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/conf/driver_variable.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3625 2023-01-16 19:36:49.000000 geoformat-20230421/geoformat/conf/error_messages.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3832 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/conf/fields_variable.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1744 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conf/format_data.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)       35 2022-12-12 09:38:12.000000 geoformat-20230421/geoformat/conf/geoformat_var.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3990 2023-01-03 14:19:37.000000 geoformat-20230421/geoformat/conf/geometry_variable.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4897 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/conf/path.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      700 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/conf/proj_var.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10042 2023-01-03 14:29:45.000000 geoformat-20230421/geoformat/conf/timer.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.364985 geoformat-20230421/geoformat/constraints/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/constraints/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1810 2022-11-24 15:49:21.000000 geoformat-20230421/geoformat/constraints/primary_key.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.372985 geoformat-20230421/geoformat/conversion/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conversion/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1381 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conversion/bbox_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4858 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conversion/bytes_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     8010 2023-04-21 13:15:34.000000 geoformat-20230421/geoformat/conversion/coordinates_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      992 2023-01-03 14:29:45.000000 geoformat-20230421/geoformat/conversion/datetime_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    46110 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/conversion/feature_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    16223 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/conversion/fields_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6898 2023-01-16 19:36:49.000000 geoformat-20230421/geoformat/conversion/geolayer_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    50975 2023-01-03 14:29:45.000000 geoformat-20230421/geoformat/conversion/geometry_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7331 2023-01-16 19:36:49.000000 geoformat-20230421/geoformat/conversion/metadata_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      701 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conversion/precision_tolerance_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1732 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conversion/segment_conversion.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.372985 geoformat-20230421/geoformat/db/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/db/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2070 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/db/db_request.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.376985 geoformat-20230421/geoformat/driver/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/driver/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2652 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/driver/common_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    13306 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/driver/csv_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    40428 2023-01-03 14:29:45.000000 geoformat-20230421/geoformat/driver/esri_shapefile_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    12370 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/driver/geojson_driver.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.376985 geoformat-20230421/geoformat/driver/ogr/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/driver/ogr/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    41141 2022-11-24 15:49:21.000000 geoformat-20230421/geoformat/driver/ogr/ogr_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     9889 2022-11-24 15:49:21.000000 geoformat-20230421/geoformat/driver/postgresql_driver.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.380985 geoformat-20230421/geoformat/explore_data/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/explore_data/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5345 2023-01-16 19:36:49.000000 geoformat-20230421/geoformat/explore_data/duplicate.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    16452 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/explore_data/print_data.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1403 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/explore_data/random_geometry.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.380985 geoformat-20230421/geoformat/geoprocessing/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1256 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/area.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.380985 geoformat-20230421/geoformat/geoprocessing/connectors/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/connectors/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2143 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/connectors/operations.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    12104 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/connectors/predicates.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.388985 geoformat-20230421/geoformat/geoprocessing/generalization/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/generalization/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2209 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/generalization/ramer_douglas_peucker.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4989 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/generalization/visvalingam_whyatt.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.392984 geoformat-20230421/geoformat/geoprocessing/geoparameters/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/geoparameters/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3396 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/geoparameters/bbox.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      877 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/geoparameters/boundaries.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5335 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/geoparameters/lines.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1362 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/length.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    11567 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/line_merge.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.392984 geoformat-20230421/geoformat/geoprocessing/matrix/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/matrix/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5464 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/matrix/adjacency.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.392984 geoformat-20230421/geoformat/geoprocessing/measure/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/measure/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1328 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/measure/area.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3560 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/measure/distance.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      560 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/measure/length.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7282 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/merge_geometries.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7441 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/point_on_linestring.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3824 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/simplify.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5237 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/split.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2084 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/union.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.392984 geoformat-20230421/geoformat/index/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/index/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.392984 geoformat-20230421/geoformat/index/attributes/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/index/attributes/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      670 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/index/attributes/hash.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.392984 geoformat-20230421/geoformat/index/geometry/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/index/geometry/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    14746 2022-11-24 15:49:21.000000 geoformat-20230421/geoformat/index/geometry/grid.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.396984 geoformat-20230421/geoformat/manipulation/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/manipulation/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2859 2022-11-24 15:49:21.000000 geoformat-20230421/geoformat/manipulation/feature_manipulation.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20815 2023-01-03 14:42:19.000000 geoformat-20230421/geoformat/manipulation/geolayer_manipulation.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10051 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/manipulation/metadata_manipulation.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.396984 geoformat-20230421/geoformat/obj/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/obj/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      774 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/obj/geometry.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.396984 geoformat-20230421/geoformat/processing/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/processing/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.396984 geoformat-20230421/geoformat/processing/data/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/processing/data/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     9722 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/processing/data/clauses.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10536 2022-11-24 15:49:21.000000 geoformat-20230421/geoformat/processing/data/field_statistics.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.400984 geoformat-20230421/geoformat/processing/data/join/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/processing/data/join/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    26996 2023-01-16 19:36:49.000000 geoformat-20230421/geoformat/processing/data/join/join.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    11975 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/processing/data/join/merge_objects.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5199 2022-11-24 15:49:21.000000 geoformat-20230421/geoformat/processing/data/union.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.356985 geoformat-20230421/geoformat.egg-info/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20635 2023-04-21 13:15:47.000000 geoformat-20230421/geoformat.egg-info/PKG-INFO
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7676 2023-04-21 13:15:47.000000 geoformat-20230421/geoformat.egg-info/SOURCES.txt
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        1 2023-04-21 13:15:47.000000 geoformat-20230421/geoformat.egg-info/dependency_links.txt
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)       16 2023-04-21 13:15:47.000000 geoformat-20230421/geoformat.egg-info/top_level.txt
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)       38 2023-04-21 13:15:47.504982 geoformat-20230421/setup.cfg
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1210 2023-04-21 13:10:35.000000 geoformat-20230421/setup.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.356985 geoformat-20230421/tests/
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.428984 geoformat-20230421/tests/data/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/data/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15423 2022-10-13 08:02:35.000000 geoformat-20230421/tests/data/coordinates.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    43859 2023-01-03 14:30:13.000000 geoformat-20230421/tests/data/features.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2394 2022-10-13 08:02:35.000000 geoformat-20230421/tests/data/fields_metadata.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)  9850700 2023-01-03 14:30:13.000000 geoformat-20230421/tests/data/geolayers.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    26450 2023-04-21 13:15:34.000000 geoformat-20230421/tests/data/geometries.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    58422 2022-09-13 14:34:13.000000 geoformat-20230421/tests/data/geometry_index.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1227 2022-10-13 08:02:35.000000 geoformat-20230421/tests/data/index.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      232 2022-09-13 14:34:13.000000 geoformat-20230421/tests/data/matrix.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5099 2023-01-03 14:30:13.000000 geoformat-20230421/tests/data/metadata.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      435 2022-09-13 14:34:13.000000 geoformat-20230421/tests/data/segments.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.428984 geoformat-20230421/tests/geoformat/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.432983 geoformat-20230421/tests/geoformat/conf/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/conf/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3617 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/conf/test_format_data.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     8633 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/conf/test_path.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.432983 geoformat-20230421/tests/geoformat/constraints/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/constraints/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2987 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/constraints/test_primary_key.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.460983 geoformat-20230421/tests/geoformat/conversion/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/conversion/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2380 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/conversion/test_bbox_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17731 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/conversion/test_bytes_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17709 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/conversion/test_coordinates_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      986 2023-01-03 14:29:45.000000 geoformat-20230421/tests/geoformat/conversion/test_datetime_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   205565 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/conversion/test_feature_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   161950 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/conversion/test_fields_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)  5602810 2022-11-24 15:49:21.000000 geoformat-20230421/tests/geoformat/conversion/test_geolayer_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    92781 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/conversion/test_geometry_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    65479 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/conversion/test_metadata_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1238 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/conversion/test_precision_tolerance_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3245 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/conversion/test_segment_conversion.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.460983 geoformat-20230421/tests/geoformat/db/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/db/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.472983 geoformat-20230421/tests/geoformat/driver/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/driver/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.472983 geoformat-20230421/tests/geoformat/driver/ogr/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/driver/ogr/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      369 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/driver/ogr/compare_ogr_files.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1251 2023-01-03 14:29:45.000000 geoformat-20230421/tests/geoformat/driver/ogr/geolayer_to_geojson.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1263 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/driver/ogr/geolayer_to_postgresql.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2155 2023-01-03 14:29:45.000000 geoformat-20230421/tests/geoformat/driver/ogr/geolayer_to_shapefile.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    16224 2023-01-03 14:29:45.000000 geoformat-20230421/tests/geoformat/driver/test_common_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    29687 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/driver/test_csv_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   321121 2023-01-03 14:29:45.000000 geoformat-20230421/tests/geoformat/driver/test_esri_shapefile_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)  1461478 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/driver/test_geojson_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   114134 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/driver/test_postgresql_driver.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.476982 geoformat-20230421/tests/geoformat/explore_data/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/explore_data/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17339 2023-01-16 19:36:49.000000 geoformat-20230421/tests/geoformat/explore_data/test_duplicate.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    66158 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/explore_data/test_print_data.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.476982 geoformat-20230421/tests/geoformat/geoprocessing/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/geoprocessing/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.480982 geoformat-20230421/tests/geoformat/geoprocessing/connectors/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/geoprocessing/connectors/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4728 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/connectors/test_operations.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15761 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/connectors/test_predicates.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.480982 geoformat-20230421/tests/geoformat/geoprocessing/generalization/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/generalization/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2176 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/generalization/test_ramer_douglas_peucker.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1845 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/generalization/test_visvalingam_whyatt.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.480982 geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3562 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/test_bbox.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      901 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/test_boundaries.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     9425 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/test_lines.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.480982 geoformat-20230421/tests/geoformat/geoprocessing/matrix/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/geoprocessing/matrix/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1645 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/matrix/test_adjacency.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.484982 geoformat-20230421/tests/geoformat/geoprocessing/measure/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/geoprocessing/measure/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2234 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/measure/test_area.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3736 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/measure/test_distance.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1525 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/measure/test_length.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1758 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_area.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2337 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_length.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15898 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_line_merge.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4976 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_merge_geometries.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4575 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_point_on_linestring.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    14514 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_simplify.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    53164 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_split.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1387 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_union.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.484982 geoformat-20230421/tests/geoformat/index/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/index/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.484982 geoformat-20230421/tests/geoformat/index/attributes/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/index/attributes/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1279 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/index/attributes/test_hash.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.488982 geoformat-20230421/tests/geoformat/index/geometry/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/index/geometry/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15928 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/index/geometry/test_grid.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.496982 geoformat-20230421/tests/geoformat/manipulation/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/manipulation/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    12109 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/manipulation/test_feature_manipulation.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   256166 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/manipulation/test_geolayer_manipulation.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    38639 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/manipulation/test_metadata_manipulation.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.496982 geoformat-20230421/tests/geoformat/obj/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/obj/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1928 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/obj/test_geometry.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.496982 geoformat-20230421/tests/geoformat/processing/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/processing/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.496982 geoformat-20230421/tests/geoformat/processing/data/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/processing/data/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.500982 geoformat-20230421/tests/geoformat/processing/data/join/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/processing/data/join/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   608012 2023-01-16 19:36:49.000000 geoformat-20230421/tests/geoformat/processing/data/join/test_join.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20394 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/processing/data/join/test_merge_objects.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6946 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/processing/data/test_clauses.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7537 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/processing/data/test_field_statistics.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6065 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/processing/data/test_union.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.500982 geoformat-20230421/tests/inspector/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/inspector/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17877 2023-01-03 14:30:13.000000 geoformat-20230421/tests/inspector/geoformat_inspector.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.500982 geoformat-20230421/tests/perf/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/tests/perf/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10403 2023-01-03 14:30:13.000000 geoformat-20230421/tests/perf/compare_func.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.500982 geoformat-20230421/tests/utils/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/tests/utils/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1379 2023-01-03 14:29:45.000000 geoformat-20230421/tests/utils/compare.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6701 2023-01-03 14:30:13.000000 geoformat-20230421/tests/utils/tests_utils.py
```

### Comparing `geoformat-20230116/LICENSE` & `geoformat-20230421/LICENSE`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/PKG-INFO` & `geoformat-20230421/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: geoformat
-Version: 20230116
+Version: 20230421
 Summary: Geoformat is a GDAL/OGR library overlayer
 Home-page: https://framagit.org/Guilhain/Geoformat
 Author: Guilhain Averlant
 Author-email: g.averlant@mailfence.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -311,9 +310,7 @@
 | 6      | 87471243.0 | St-Méen       | O    | N         | 472000     | 1.0  | 68+200  | 315077.0   | 6800114.0  | -243043.0 | 6138128.0 | St-Méen-le-Grand | Ille-et-Vilaine | Point | [-2.1832958937261893, 48. ...] |
 | 7      | 87476200.0 | Auray         | O    | O         | 473000     | 1.0  | 584+946 | 250286.0   | 6748188.0  | -333913.0 | 6053823.0 | Auray            | Morbihan        | Point | [-2.99959548260269, 47.68 ...] |
 | 8      | 87476408.0 | Belz-Ploemel  | N    | O         | 473000     | 1.0  | 591+597 | 244616.0   | 6745536.0  | -341998.0 | 6049244.0 | Ploemel          | Morbihan        | Point | [-3.072226071667076, 47.6 ...] |
 | 9      | 87473330.0 | Quintin       | O    | O         | 475000     | 1.0  | 492+810 | 264298.0   | 6827046.0  | -321902.0 | 6173216.0 | St-Brandan       | Côte-d'Armor    | Point | [-2.8917008446444417, 48. ...] |
 +--------+------------+---------------+------+-----------+------------+------+---------+------------+------------+-----------+-----------+------------------+-----------------+-------+--------------------------------+
 
 ```
-
-
```

### Comparing `geoformat-20230116/README.md` & `geoformat-20230421/README.md`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/__init__.py` & `geoformat-20230421/geoformat/__init__.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conf/decorator.py` & `geoformat-20230421/geoformat/conf/decorator.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conf/driver_variable.py` & `geoformat-20230421/geoformat/conf/driver_variable.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conf/error_messages.py` & `geoformat-20230421/geoformat/conf/error_messages.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conf/fields_variable.py` & `geoformat-20230421/geoformat/conf/fields_variable.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conf/format_data.py` & `geoformat-20230421/geoformat/conf/format_data.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conf/geometry_variable.py` & `geoformat-20230421/geoformat/conf/geometry_variable.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conf/path.py` & `geoformat-20230421/geoformat/conf/path.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conf/proj_var.py` & `geoformat-20230421/geoformat/conf/proj_var.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conf/timer.py` & `geoformat-20230421/geoformat/conf/timer.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/constraints/primary_key.py` & `geoformat-20230421/geoformat/constraints/primary_key.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conversion/bbox_conversion.py` & `geoformat-20230421/geoformat/conversion/bbox_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conversion/bytes_conversion.py` & `geoformat-20230421/geoformat/conversion/bytes_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conversion/coordinates_conversion.py` & `geoformat-20230421/geoformat/conversion/coordinates_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from geoformat.geoprocessing.connectors.operations import (
     coordinates_to_point
 )
 
 from geoformat.conf.error_messages import import_pyproj_error
 
 try:
-    import pyproj
-
+    from pyproj import Transformer
     import_pyproj_success = True
 except ImportError:
     import_pyproj_success = False
 
 
 def format_coordinates(
         coordinates_list_tuple,
@@ -47,15 +46,16 @@
                 point_list = True
                 output_coordinates_list_tuple = [output_coordinates_list_tuple]
 
             if isinstance(output_coordinates_list_tuple[0][0], (int, float)):
                 # reproject if necessary
                 if in_crs is not None and out_crs is not None:
                     x_coords, y_coords = zip(*output_coordinates_list_tuple)
-                    transform_coords = pyproj.transform(in_crs, out_crs, x_coords, y_coords, always_xy=True)
+                    transformer = Transformer.from_crs(f"EPSG:{in_crs}", f"EPSG:{out_crs}", always_xy=True)
+                    transform_coords = transformer.transform(x_coords, y_coords)
                     output_coordinates_list_tuple = zip(*transform_coords)
 
                 if precision is not None:
                     # change precision
                     output_coordinates_list_tuple = [[round(xyz, precision) for xyz in coordinates] for coordinates in
                                                      output_coordinates_list_tuple]
```

### Comparing `geoformat-20230116/geoformat/conversion/datetime_conversion.py` & `geoformat-20230421/geoformat/conversion/datetime_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conversion/feature_conversion.py` & `geoformat-20230421/geoformat/conversion/feature_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conversion/fields_conversion.py` & `geoformat-20230421/geoformat/conversion/fields_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conversion/geolayer_conversion.py` & `geoformat-20230421/geoformat/conversion/geolayer_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conversion/geometry_conversion.py` & `geoformat-20230421/geoformat/conversion/geometry_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conversion/metadata_conversion.py` & `geoformat-20230421/geoformat/conversion/metadata_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conversion/precision_tolerance_conversion.py` & `geoformat-20230421/geoformat/conversion/precision_tolerance_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/conversion/segment_conversion.py` & `geoformat-20230421/geoformat/conversion/segment_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/db/db_request.py` & `geoformat-20230421/geoformat/db/db_request.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/driver/common_driver.py` & `geoformat-20230421/geoformat/driver/common_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/driver/csv_driver.py` & `geoformat-20230421/geoformat/driver/csv_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/driver/esri_shapefile_driver.py` & `geoformat-20230421/geoformat/driver/esri_shapefile_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/driver/geojson_driver.py` & `geoformat-20230421/geoformat/driver/geojson_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/driver/ogr/ogr_driver.py` & `geoformat-20230421/geoformat/driver/ogr/ogr_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/driver/postgresql_driver.py` & `geoformat-20230421/geoformat/driver/postgresql_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/explore_data/duplicate.py` & `geoformat-20230421/geoformat/explore_data/duplicate.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/explore_data/print_data.py` & `geoformat-20230421/geoformat/explore_data/print_data.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/explore_data/random_geometry.py` & `geoformat-20230421/geoformat/explore_data/random_geometry.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/area.py` & `geoformat-20230421/geoformat/geoprocessing/area.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/connectors/operations.py` & `geoformat-20230421/geoformat/geoprocessing/connectors/operations.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/connectors/predicates.py` & `geoformat-20230421/geoformat/geoprocessing/connectors/predicates.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/generalization/ramer_douglas_peucker.py` & `geoformat-20230421/geoformat/geoprocessing/generalization/ramer_douglas_peucker.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/generalization/visvalingam_whyatt.py` & `geoformat-20230421/geoformat/geoprocessing/generalization/visvalingam_whyatt.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/geoparameters/bbox.py` & `geoformat-20230421/geoformat/geoprocessing/geoparameters/bbox.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/geoparameters/boundaries.py` & `geoformat-20230421/geoformat/geoprocessing/geoparameters/boundaries.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/geoparameters/lines.py` & `geoformat-20230421/geoformat/geoprocessing/geoparameters/lines.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/length.py` & `geoformat-20230421/geoformat/geoprocessing/length.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/line_merge.py` & `geoformat-20230421/geoformat/geoprocessing/line_merge.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/matrix/adjacency.py` & `geoformat-20230421/geoformat/geoprocessing/matrix/adjacency.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/measure/area.py` & `geoformat-20230421/geoformat/geoprocessing/measure/area.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/measure/distance.py` & `geoformat-20230421/geoformat/geoprocessing/measure/distance.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/measure/length.py` & `geoformat-20230421/geoformat/geoprocessing/measure/length.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/merge_geometries.py` & `geoformat-20230421/geoformat/geoprocessing/merge_geometries.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/point_on_linestring.py` & `geoformat-20230421/geoformat/geoprocessing/point_on_linestring.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/simplify.py` & `geoformat-20230421/geoformat/geoprocessing/simplify.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/split.py` & `geoformat-20230421/geoformat/geoprocessing/split.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/geoprocessing/union.py` & `geoformat-20230421/geoformat/geoprocessing/union.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/index/attributes/hash.py` & `geoformat-20230421/geoformat/index/attributes/hash.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/index/geometry/grid.py` & `geoformat-20230421/geoformat/index/geometry/grid.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/manipulation/feature_manipulation.py` & `geoformat-20230421/geoformat/manipulation/feature_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/manipulation/geolayer_manipulation.py` & `geoformat-20230421/geoformat/manipulation/geolayer_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/manipulation/metadata_manipulation.py` & `geoformat-20230421/geoformat/manipulation/metadata_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/obj/geometry.py` & `geoformat-20230421/geoformat/obj/geometry.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/processing/data/clauses.py` & `geoformat-20230421/geoformat/processing/data/clauses.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/processing/data/field_statistics.py` & `geoformat-20230421/geoformat/processing/data/field_statistics.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/processing/data/join/join.py` & `geoformat-20230421/geoformat/processing/data/join/join.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/processing/data/join/merge_objects.py` & `geoformat-20230421/geoformat/processing/data/join/merge_objects.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat/processing/data/union.py` & `geoformat-20230421/geoformat/processing/data/union.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/geoformat.egg-info/PKG-INFO` & `geoformat-20230421/geoformat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: geoformat
-Version: 20230116
+Version: 20230421
 Summary: Geoformat is a GDAL/OGR library overlayer
 Home-page: https://framagit.org/Guilhain/Geoformat
 Author: Guilhain Averlant
 Author-email: g.averlant@mailfence.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -311,9 +310,7 @@
 | 6      | 87471243.0 | St-Méen       | O    | N         | 472000     | 1.0  | 68+200  | 315077.0   | 6800114.0  | -243043.0 | 6138128.0 | St-Méen-le-Grand | Ille-et-Vilaine | Point | [-2.1832958937261893, 48. ...] |
 | 7      | 87476200.0 | Auray         | O    | O         | 473000     | 1.0  | 584+946 | 250286.0   | 6748188.0  | -333913.0 | 6053823.0 | Auray            | Morbihan        | Point | [-2.99959548260269, 47.68 ...] |
 | 8      | 87476408.0 | Belz-Ploemel  | N    | O         | 473000     | 1.0  | 591+597 | 244616.0   | 6745536.0  | -341998.0 | 6049244.0 | Ploemel          | Morbihan        | Point | [-3.072226071667076, 47.6 ...] |
 | 9      | 87473330.0 | Quintin       | O    | O         | 475000     | 1.0  | 492+810 | 264298.0   | 6827046.0  | -321902.0 | 6173216.0 | St-Brandan       | Côte-d'Armor    | Point | [-2.8917008446444417, 48. ...] |
 +--------+------------+---------------+------+-----------+------------+------+---------+------------+------------+-----------+-----------+------------------+-----------------+-------+--------------------------------+
 
 ```
-
-
```

### Comparing `geoformat-20230116/geoformat.egg-info/SOURCES.txt` & `geoformat-20230421/geoformat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/setup.py` & `geoformat-20230421/setup.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/data/coordinates.py` & `geoformat-20230421/tests/data/coordinates.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/data/features.py` & `geoformat-20230421/tests/data/features.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/data/fields_metadata.py` & `geoformat-20230421/tests/data/fields_metadata.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/data/geolayers.py` & `geoformat-20230421/tests/data/geolayers.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/data/geometries.py` & `geoformat-20230421/tests/data/geometries.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,17 +242,15 @@
         },
         {"type": "MultiPolygon", "coordinates": []},
     ],
     "bbox": (-130.95, -34.25, 23.194, 77.95),
 }
 
 # format : WKB with big endian
-POINT_WKB_BIG_ENDIAN = (
-    b"\x00\x00\x00\x00\x01\xc0\\\xf3\xd7\n=p\xa4@B\x9e\xb8Q\xeb\x85\x1f"
-)
+POINT_WKB_BIG_ENDIAN = b"\x00\x00\x00\x00\x01\xc0\\\xf3\xd7\n=p\xa4@B\x9e\xb8Q\xeb\x85\x1f"
 POINT_EMPTY_WKB_BIG_ENDIAN = b"\x00\x00\x00\x00\x01\x7f\xf8\x00\x00\x00\x00\x00\x00\x7f\xf8\x00\x00\x00\x00\x00\x00"
 LINESTRING_WKB_BIG_ENDIAN = b"\x00\x00\x00\x00\x02\x00\x00\x00\x02@!\xd6\x87+\x02\x0cJ@F4%\xae\xe61\xf9@!\xd8\x93t\xbcj\x7f@F4(\xf5\xc2\x8f\\"
 LINESTRING_EMPTY_WKB_BIG_ENDIAN = b"\x00\x00\x00\x00\x02\x00\x00\x00\x00"
 POLYGON_WKB_BIG_ENDIAN = b"\x00\x00\x00\x00\x03\x00\x00\x00\x02\x00\x00\x00\x04@\x03\n=p\xa3\xd7\n@L\xa97K\xc6\xa7\xf0@71\xa9\xfb\xe7l\x8b\xc04G\xae\x14z\xe1H\xc0^\x1b\x85\x1e\xb8Q\xec@3&fffff@\x03\n=p\xa3\xd7\n@L\xa97K\xc6\xa7\xf0\x00\x00\x00\x04\xc0\x14\xd7\n=p\xa3\xd7@7\x82\x8f\\(\xf5\xc3@.k\x85\x1e\xb8Q\xec\xc0%\x9e\xb8Q\xeb\x85\x1f\xc04\x82\x8f\\(\xf5\xc3?\xf8(\xf5\xc2\x8f\\)\xc0\x14\xd7\n=p\xa3\xd7@7\x82\x8f\\(\xf5\xc3"
 POLYGON_EMPTY_WKB_BIG_ENDIAN = b"\x00\x00\x00\x00\x03\x00\x00\x00\x00"
 MULTIPOINT_WKB_BIG_ENDIAN = b"\x00\x00\x00\x00\x04\x00\x00\x00\x03\x00\x00\x00\x00\x01\xc0cp\xa3\xd7\n=q@3\x9c(\xf5\xc2\x8f\\\x00\x00\x00\x00\x01\xc0c\x87\n=p\xa3\xd7@4\xbdp\xa3\xd7\n=\x00\x00\x00\x00\x01\xc0c\xbf\n=p\xa3\xd7@5u\xc2\x8f\\(\xf6"
 MULTIPOINT_EMPTY_WKB_BIG_ENDIAN = b"\x00\x00\x00\x00\x04\x00\x00\x00\x00"
```

### Comparing `geoformat-20230116/tests/data/geometry_index.py` & `geoformat-20230421/tests/data/geometry_index.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/data/index.py` & `geoformat-20230421/tests/data/index.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/data/metadata.py` & `geoformat-20230421/tests/data/metadata.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/conf/test_format_data.py` & `geoformat-20230421/tests/geoformat/conf/test_format_data.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/conf/test_path.py` & `geoformat-20230421/tests/geoformat/conf/test_path.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/constraints/test_primary_key.py` & `geoformat-20230421/tests/geoformat/constraints/test_primary_key.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/conversion/test_bbox_conversion.py` & `geoformat-20230421/tests/geoformat/conversion/test_bbox_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/conversion/test_bytes_conversion.py` & `geoformat-20230421/tests/geoformat/conversion/test_bytes_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/conversion/test_coordinates_conversion.py` & `geoformat-20230421/tests/geoformat/conversion/test_coordinates_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/conversion/test_datetime_conversion.py` & `geoformat-20230421/tests/geoformat/conversion/test_datetime_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/conversion/test_feature_conversion.py` & `geoformat-20230421/tests/geoformat/conversion/test_feature_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/conversion/test_fields_conversion.py` & `geoformat-20230421/tests/geoformat/conversion/test_fields_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/conversion/test_geolayer_conversion.py` & `geoformat-20230421/tests/geoformat/conversion/test_geolayer_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/conversion/test_geometry_conversion.py` & `geoformat-20230421/tests/geoformat/conversion/test_geometry_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/conversion/test_metadata_conversion.py` & `geoformat-20230421/tests/geoformat/conversion/test_metadata_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/conversion/test_precision_tolerance_conversion.py` & `geoformat-20230421/tests/geoformat/conversion/test_precision_tolerance_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/conversion/test_segment_conversion.py` & `geoformat-20230421/tests/geoformat/conversion/test_segment_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/driver/ogr/geolayer_to_geojson.py` & `geoformat-20230421/tests/geoformat/driver/ogr/geolayer_to_geojson.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/driver/ogr/geolayer_to_postgresql.py` & `geoformat-20230421/tests/geoformat/driver/ogr/geolayer_to_postgresql.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/driver/ogr/geolayer_to_shapefile.py` & `geoformat-20230421/tests/geoformat/driver/ogr/geolayer_to_shapefile.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/driver/test_common_driver.py` & `geoformat-20230421/tests/geoformat/driver/test_common_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/driver/test_csv_driver.py` & `geoformat-20230421/tests/geoformat/driver/test_csv_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/driver/test_esri_shapefile_driver.py` & `geoformat-20230421/tests/geoformat/driver/test_esri_shapefile_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/driver/test_geojson_driver.py` & `geoformat-20230421/tests/geoformat/driver/test_geojson_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/driver/test_postgresql_driver.py` & `geoformat-20230421/tests/geoformat/driver/test_postgresql_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/explore_data/test_duplicate.py` & `geoformat-20230421/tests/geoformat/explore_data/test_duplicate.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/explore_data/test_print_data.py` & `geoformat-20230421/tests/geoformat/explore_data/test_print_data.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/connectors/test_operations.py` & `geoformat-20230421/tests/geoformat/geoprocessing/connectors/test_operations.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/connectors/test_predicates.py` & `geoformat-20230421/tests/geoformat/geoprocessing/connectors/test_predicates.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/generalization/test_ramer_douglas_peucker.py` & `geoformat-20230421/tests/geoformat/geoprocessing/generalization/test_ramer_douglas_peucker.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/generalization/test_visvalingam_whyatt.py` & `geoformat-20230421/tests/geoformat/geoprocessing/generalization/test_visvalingam_whyatt.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/geoparameters/test_bbox.py` & `geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/test_bbox.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/geoparameters/test_boundaries.py` & `geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/geoparameters/test_lines.py` & `geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/test_lines.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/matrix/test_adjacency.py` & `geoformat-20230421/tests/geoformat/geoprocessing/matrix/test_adjacency.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/measure/test_area.py` & `geoformat-20230421/tests/geoformat/geoprocessing/measure/test_area.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/measure/test_distance.py` & `geoformat-20230421/tests/geoformat/geoprocessing/measure/test_distance.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/measure/test_length.py` & `geoformat-20230421/tests/geoformat/geoprocessing/measure/test_length.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/test_area.py` & `geoformat-20230421/tests/geoformat/geoprocessing/test_area.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/test_length.py` & `geoformat-20230421/tests/geoformat/geoprocessing/test_length.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/test_line_merge.py` & `geoformat-20230421/tests/geoformat/geoprocessing/test_line_merge.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/test_merge_geometries.py` & `geoformat-20230421/tests/geoformat/geoprocessing/test_merge_geometries.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/test_point_on_linestring.py` & `geoformat-20230421/tests/geoformat/geoprocessing/test_point_on_linestring.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/test_simplify.py` & `geoformat-20230421/tests/geoformat/geoprocessing/test_simplify.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/test_split.py` & `geoformat-20230421/tests/geoformat/geoprocessing/test_split.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/geoprocessing/test_union.py` & `geoformat-20230421/tests/geoformat/geoprocessing/test_union.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/index/attributes/test_hash.py` & `geoformat-20230421/tests/geoformat/index/attributes/test_hash.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/index/geometry/test_grid.py` & `geoformat-20230421/tests/geoformat/index/geometry/test_grid.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/manipulation/test_feature_manipulation.py` & `geoformat-20230421/tests/geoformat/manipulation/test_feature_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/manipulation/test_geolayer_manipulation.py` & `geoformat-20230421/tests/geoformat/manipulation/test_geolayer_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/manipulation/test_metadata_manipulation.py` & `geoformat-20230421/tests/geoformat/manipulation/test_metadata_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/obj/test_geometry.py` & `geoformat-20230421/tests/geoformat/obj/test_geometry.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/processing/data/join/test_join.py` & `geoformat-20230421/tests/geoformat/processing/data/join/test_join.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/processing/data/join/test_merge_objects.py` & `geoformat-20230421/tests/geoformat/processing/data/join/test_merge_objects.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/processing/data/test_clauses.py` & `geoformat-20230421/tests/geoformat/processing/data/test_clauses.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/processing/data/test_field_statistics.py` & `geoformat-20230421/tests/geoformat/processing/data/test_field_statistics.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/geoformat/processing/data/test_union.py` & `geoformat-20230421/tests/geoformat/processing/data/test_union.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/inspector/geoformat_inspector.py` & `geoformat-20230421/tests/inspector/geoformat_inspector.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/perf/compare_func.py` & `geoformat-20230421/tests/perf/compare_func.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/utils/compare.py` & `geoformat-20230421/tests/utils/compare.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230116/tests/utils/tests_utils.py` & `geoformat-20230421/tests/utils/tests_utils.py`

 * *Files identical despite different names*

