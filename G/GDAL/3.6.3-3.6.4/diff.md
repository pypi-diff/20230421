# Comparing `tmp/GDAL-3.6.3.tar.gz` & `tmp/GDAL-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GDAL-3.6.3.tar", last modified: Mon Mar 13 21:00:33 2023, max compression
+gzip compressed data, was "GDAL-3.6.4.tar", last modified: Fri Apr 21 13:03:22 2023, max compression
```

## Comparing `GDAL-3.6.3.tar` & `GDAL-3.6.4.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-03-13 21:00:33.070448 GDAL-3.6.3/
--rw-rw-r--   0 even      (1000) even      (1000)     6605 2023-03-13 21:00:33.070448 GDAL-3.6.3/PKG-INFO
--rw-rw-r--   0 even      (1000) even      (1000)     5743 2023-03-13 20:59:47.000000 GDAL-3.6.3/README.rst
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-03-13 21:00:33.046449 GDAL-3.6.3/extensions/
--rw-rw-r--   0 even      (1000) even      (1000)   240623 2023-03-13 21:00:07.000000 GDAL-3.6.3/extensions/gdal_array_wrap.cpp
--rw-rw-r--   0 even      (1000) even      (1000)  1698259 2023-03-13 21:00:08.000000 GDAL-3.6.3/extensions/gdal_wrap.cpp
--rw-rw-r--   0 even      (1000) even      (1000)   125229 2023-03-13 21:00:06.000000 GDAL-3.6.3/extensions/gdalconst_wrap.c
--rw-rw-r--   0 even      (1000) even      (1000)   216783 2023-03-13 21:00:07.000000 GDAL-3.6.3/extensions/gnm_wrap.cpp
--rw-rw-r--   0 even      (1000) even      (1000)  1307054 2023-03-13 21:00:08.000000 GDAL-3.6.3/extensions/ogr_wrap.cpp
--rw-rw-r--   0 even      (1000) even      (1000)   725967 2023-03-13 21:00:07.000000 GDAL-3.6.3/extensions/osr_wrap.cpp
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-03-13 21:00:33.042449 GDAL-3.6.3/gdal-utils/
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-03-13 21:00:33.046449 GDAL-3.6.3/gdal-utils/GDAL.egg-info/
--rw-rw-r--   0 even      (1000) even      (1000)     6605 2023-03-13 21:00:32.000000 GDAL-3.6.3/gdal-utils/GDAL.egg-info/PKG-INFO
--rw-rw-r--   0 even      (1000) even      (1000)     5228 2023-03-13 21:00:32.000000 GDAL-3.6.3/gdal-utils/GDAL.egg-info/SOURCES.txt
--rw-rw-r--   0 even      (1000) even      (1000)        1 2023-03-13 21:00:32.000000 GDAL-3.6.3/gdal-utils/GDAL.egg-info/dependency_links.txt
--rw-rw-r--   0 even      (1000) even      (1000)        1 2022-11-11 10:46:54.000000 GDAL-3.6.3/gdal-utils/GDAL.egg-info/not-zip-safe
--rw-rw-r--   0 even      (1000) even      (1000)       21 2023-03-13 21:00:32.000000 GDAL-3.6.3/gdal-utils/GDAL.egg-info/requires.txt
--rw-rw-r--   0 even      (1000) even      (1000)       18 2023-03-13 21:00:32.000000 GDAL-3.6.3/gdal-utils/GDAL.egg-info/top_level.txt
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-03-13 21:00:33.050449 GDAL-3.6.3/gdal-utils/osgeo_utils/
--rw-rw-r--   0 even      (1000) even      (1000)      432 2023-03-07 17:10:08.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/__init__.py
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-03-13 21:00:33.054449 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/
--rw-rw-r--   0 even      (1000) even      (1000)        0 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/__init__.py
--rw-rw-r--   0 even      (1000) even      (1000)     2635 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/array_util.py
--rw-rw-r--   0 even      (1000) even      (1000)     4044 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/base.py
--rw-rw-r--   0 even      (1000) even      (1000)     3447 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/batch_creator.py
--rw-rw-r--   0 even      (1000) even      (1000)    15215 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/color_palette.py
--rw-rw-r--   0 even      (1000) even      (1000)     5649 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/color_table.py
--rw-rw-r--   0 even      (1000) even      (1000)     5384 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/extent_util.py
--rw-rw-r--   0 even      (1000) even      (1000)     6566 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/gdal_argparse.py
--rw-rw-r--   0 even      (1000) even      (1000)     2721 2023-01-11 18:52:28.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/numpy_util.py
--rw-rw-r--   0 even      (1000) even      (1000)     5467 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/osr_util.py
--rw-rw-r--   0 even      (1000) even      (1000)     3340 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/progress.py
--rw-rw-r--   0 even      (1000) even      (1000)     6671 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/raster_creation.py
--rw-rw-r--   0 even      (1000) even      (1000)     8828 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/rectangle.py
--rw-rw-r--   0 even      (1000) even      (1000)    16651 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/util.py
--rw-rw-r--   0 even      (1000) even      (1000)   166201 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/gdal2tiles.py
--rw-rw-r--   0 even      (1000) even      (1000)    14544 2023-03-13 20:53:18.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/gdal2xyz.py
--rw-rw-r--   0 even      (1000) even      (1000)    36264 2023-01-11 18:52:28.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_calc.py
--rw-rw-r--   0 even      (1000) even      (1000)    15155 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_edit.py
--rw-rw-r--   0 even      (1000) even      (1000)     8936 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_fillnodata.py
--rw-rw-r--   0 even      (1000) even      (1000)    18299 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_merge.py
--rw-rw-r--   0 even      (1000) even      (1000)    11772 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_pansharpen.py
--rw-rw-r--   0 even      (1000) even      (1000)    10303 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_polygonize.py
--rw-rw-r--   0 even      (1000) even      (1000)     7052 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_proximity.py
--rw-rw-r--   0 even      (1000) even      (1000)    35616 2023-01-27 19:56:58.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_retile.py
--rw-rw-r--   0 even      (1000) even      (1000)     6441 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_sieve.py
--rw-rw-r--   0 even      (1000) even      (1000)     4794 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/gdalattachpct.py
--rw-rw-r--   0 even      (1000) even      (1000)    11399 2023-03-13 20:53:18.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/gdalcompare.py
--rw-rw-r--   0 even      (1000) even      (1000)     9796 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/gdalmove.py
--rw-rw-r--   0 even      (1000) even      (1000)    18128 2022-12-12 12:52:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/ogr_layer_algebra.py
--rw-rw-r--   0 even      (1000) even      (1000)    22455 2023-01-11 18:52:28.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/ogrmerge.py
--rw-rw-r--   0 even      (1000) even      (1000)     7664 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/pct2rgb.py
--rw-rw-r--   0 even      (1000) even      (1000)     7145 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/rgb2pct.py
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-03-13 21:00:33.066449 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/
--rw-rw-r--   0 even      (1000) even      (1000)        0 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/__init__.py
--rw-rw-r--   0 even      (1000) even      (1000)     4632 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/assemblepoly.py
--rw-rw-r--   0 even      (1000) even      (1000)    17347 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/build_jp2_from_xml.py
--rw-rw-r--   0 even      (1000) even      (1000)     2828 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/classify.py
--rw-rw-r--   0 even      (1000) even      (1000)    12326 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/crs2crs2grid.py
--rw-rw-r--   0 even      (1000) even      (1000)    16769 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/densify.py
--rw-rw-r--   0 even      (1000) even      (1000)     8126 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/dump_jp2.py
--rw-rw-r--   0 even      (1000) even      (1000)     9915 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/epsg_tr.py
--rw-rw-r--   0 even      (1000) even      (1000)     3238 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/esri2wkt.py
--rw-rw-r--   0 even      (1000) even      (1000)     4274 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/fft.py
--rw-rw-r--   0 even      (1000) even      (1000)     3008 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/fix_gpkg.py
--rw-rw-r--   0 even      (1000) even      (1000)     3193 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gcps2ogr.py
--rw-rw-r--   0 even      (1000) even      (1000)     5419 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gcps2vec.py
--rw-rw-r--   0 even      (1000) even      (1000)     2580 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gcps2wld.py
--rw-rw-r--   0 even      (1000) even      (1000)     5281 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal2grd.py
--rw-rw-r--   0 even      (1000) even      (1000)     4451 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_auth.py
--rw-rw-r--   0 even      (1000) even      (1000)    11309 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_cp.py
--rw-rw-r--   0 even      (1000) even      (1000)     2561 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_create_pdf.py
--rw-rw-r--   0 even      (1000) even      (1000)     8693 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_ls.py
--rw-rw-r--   0 even      (1000) even      (1000)     6668 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_lut.py
--rw-rw-r--   0 even      (1000) even      (1000)     2403 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_mkdir.py
--rw-rw-r--   0 even      (1000) even      (1000)     4426 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_remove_towgs84.py
--rw-rw-r--   0 even      (1000) even      (1000)     4035 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_rm.py
--rw-rw-r--   0 even      (1000) even      (1000)     2538 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_rmdir.py
--rw-rw-r--   0 even      (1000) even      (1000)    11900 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_vrtmerge.py
--rw-rw-r--   0 even      (1000) even      (1000)     4069 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_zip.py
--rw-rw-r--   0 even      (1000) even      (1000)     3004 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdalchksum.py
--rw-rw-r--   0 even      (1000) even      (1000)     3004 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdalcopyproj.py
--rw-rw-r--   0 even      (1000) even      (1000)     6067 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdalfilter.py
--rw-rw-r--   0 even      (1000) even      (1000)     3021 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdalident.py
--rw-rw-r--   0 even      (1000) even      (1000)     3036 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdalimport.py
--rw-rw-r--   0 even      (1000) even      (1000)    22185 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdalinfo.py
--rw-rw-r--   0 even      (1000) even      (1000)    20066 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdallocationinfo.py
--rw-rw-r--   0 even      (1000) even      (1000)     4095 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/get_soundg.py
--rw-rw-r--   0 even      (1000) even      (1000)     3374 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/histrep.py
--rw-rw-r--   0 even      (1000) even      (1000)     8150 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/hsv_merge.py
--rw-rw-r--   0 even      (1000) even      (1000)    10510 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/jpeg_in_tiff_extract.py
--rw-rw-r--   0 even      (1000) even      (1000)     6440 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/load2odbc.py
--rw-rw-r--   0 even      (1000) even      (1000)     8847 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/loslas2ntv2.py
--rw-rw-r--   0 even      (1000) even      (1000)     2739 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/magphase.py
--rw-rw-r--   0 even      (1000) even      (1000)     2167 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/make_fuzzer_friendly_archive.py
--rw-rw-r--   0 even      (1000) even      (1000)     7547 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/mkgraticule.py
--rw-rw-r--   0 even      (1000) even      (1000)    70278 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/ogr2ogr.py
--rw-rw-r--   0 even      (1000) even      (1000)    12582 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/ogr2vrt.py
--rw-rw-r--   0 even      (1000) even      (1000)     7567 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/ogr_build_junction_table.py
--rw-rw-r--   0 even      (1000) even      (1000)    14345 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/ogr_dispatch.py
--rw-rw-r--   0 even      (1000) even      (1000)    21229 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/ogrinfo.py
--rw-rw-r--   0 even      (1000) even      (1000)    19843 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/ogrupdate.py
--rw-rw-r--   0 even      (1000) even      (1000)     7724 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/rel.py
--rw-rw-r--   0 even      (1000) even      (1000)     7578 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/tigerpoly.py
--rw-rw-r--   0 even      (1000) even      (1000)     4368 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/tile_extent_from_raster.py
--rw-rw-r--   0 even      (1000) even      (1000)     4055 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/tolatlong.py
--rw-rw-r--   0 even      (1000) even      (1000)     4344 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/val_repl.py
--rw-rw-r--   0 even      (1000) even      (1000)    18476 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/validate_cloud_optimized_geotiff.py
--rw-rw-r--   0 even      (1000) even      (1000)   108556 2023-01-11 18:52:28.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/validate_gpkg.py
--rw-rw-r--   0 even      (1000) even      (1000)    70659 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/validate_jp2.py
--rw-rw-r--   0 even      (1000) even      (1000)     4768 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/vec_tr.py
--rw-rw-r--   0 even      (1000) even      (1000)     4843 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/vec_tr_spat.py
--rw-rw-r--   0 even      (1000) even      (1000)     7103 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/osgeo_utils/samples/wcs_virtds_params.py
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-03-13 21:00:33.070448 GDAL-3.6.3/gdal-utils/scripts/
--rwxrwxr-x   0 even      (1000) even      (1000)      504 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/gdal2tiles.py
--rwxrwxr-x   0 even      (1000) even      (1000)      279 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/gdal2xyz.py
--rwxrwxr-x   0 even      (1000) even      (1000)      283 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/gdal_calc.py
--rwxrwxr-x   0 even      (1000) even      (1000)      283 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/gdal_edit.py
--rwxrwxr-x   0 even      (1000) even      (1000)      307 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/gdal_fillnodata.py
--rwxrwxr-x   0 even      (1000) even      (1000)      287 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/gdal_merge.py
--rwxrwxr-x   0 even      (1000) even      (1000)      307 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/gdal_pansharpen.py
--rwxrwxr-x   0 even      (1000) even      (1000)      307 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/gdal_polygonize.py
--rwxrwxr-x   0 even      (1000) even      (1000)      303 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/gdal_proximity.py
--rwxrwxr-x   0 even      (1000) even      (1000)      291 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/gdal_retile.py
--rwxrwxr-x   0 even      (1000) even      (1000)      287 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/gdal_sieve.py
--rwxrwxr-x   0 even      (1000) even      (1000)      299 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/gdalattachpct.py
--rwxrwxr-x   0 even      (1000) even      (1000)      291 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/gdalcompare.py
--rwxrwxr-x   0 even      (1000) even      (1000)      279 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/gdalmove.py
--rwxrwxr-x   0 even      (1000) even      (1000)      315 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/ogr_layer_algebra.py
--rwxrwxr-x   0 even      (1000) even      (1000)      279 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/ogrmerge.py
--rwxrwxr-x   0 even      (1000) even      (1000)      275 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/pct2rgb.py
--rwxrwxr-x   0 even      (1000) even      (1000)      275 2022-11-03 17:38:53.000000 GDAL-3.6.3/gdal-utils/scripts/rgb2pct.py
-drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-03-13 21:00:33.070448 GDAL-3.6.3/osgeo/
--rw-rw-r--   0 even      (1000) even      (1000)     5418 2023-03-13 21:00:07.000000 GDAL-3.6.3/osgeo/__init__.py
--rw-rw-r--   0 even      (1000) even      (1000)   208954 2023-03-13 21:00:10.000000 GDAL-3.6.3/osgeo/gdal.py
--rw-rw-r--   0 even      (1000) even      (1000)    27755 2023-03-13 21:00:08.000000 GDAL-3.6.3/osgeo/gdal_array.py
--rw-rw-r--   0 even      (1000) even      (1000)    11844 2023-03-13 21:00:07.000000 GDAL-3.6.3/osgeo/gdalconst.py
--rw-rw-r--   0 even      (1000) even      (1000)      214 2023-03-13 21:00:07.000000 GDAL-3.6.3/osgeo/gdalnumeric.py
--rw-rw-r--   0 even      (1000) even      (1000)     9892 2023-03-13 21:00:07.000000 GDAL-3.6.3/osgeo/gnm.py
--rw-rw-r--   0 even      (1000) even      (1000)   221000 2023-03-13 21:00:09.000000 GDAL-3.6.3/osgeo/ogr.py
--rw-rw-r--   0 even      (1000) even      (1000)    55075 2023-03-13 21:00:09.000000 GDAL-3.6.3/osgeo/osr.py
--rw-rw-r--   0 even      (1000) even      (1000)       38 2023-03-13 21:00:33.070448 GDAL-3.6.3/setup.cfg
--rw-rw-r--   0 even      (1000) even      (1000)    13847 2023-03-13 20:59:47.000000 GDAL-3.6.3/setup.py
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-04-21 13:03:22.912005 GDAL-3.6.4/
+-rw-rw-r--   0 even      (1000) even      (1000)     6605 2023-04-21 13:03:22.912005 GDAL-3.6.4/PKG-INFO
+-rw-rw-r--   0 even      (1000) even      (1000)     5743 2023-04-21 12:57:58.000000 GDAL-3.6.4/README.rst
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-04-21 13:03:22.888005 GDAL-3.6.4/extensions/
+-rw-rw-r--   0 even      (1000) even      (1000)   240623 2023-04-21 13:02:17.000000 GDAL-3.6.4/extensions/gdal_array_wrap.cpp
+-rw-rw-r--   0 even      (1000) even      (1000)  1698259 2023-04-21 13:02:11.000000 GDAL-3.6.4/extensions/gdal_wrap.cpp
+-rw-rw-r--   0 even      (1000) even      (1000)   125229 2023-04-21 13:02:11.000000 GDAL-3.6.4/extensions/gdalconst_wrap.c
+-rw-rw-r--   0 even      (1000) even      (1000)   216783 2023-04-21 13:02:12.000000 GDAL-3.6.4/extensions/gnm_wrap.cpp
+-rw-rw-r--   0 even      (1000) even      (1000)  1307054 2023-04-21 13:02:14.000000 GDAL-3.6.4/extensions/ogr_wrap.cpp
+-rw-rw-r--   0 even      (1000) even      (1000)   725967 2023-04-21 13:02:15.000000 GDAL-3.6.4/extensions/osr_wrap.cpp
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-04-21 13:03:22.888005 GDAL-3.6.4/gdal-utils/
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-04-21 13:03:22.892005 GDAL-3.6.4/gdal-utils/GDAL.egg-info/
+-rw-rw-r--   0 even      (1000) even      (1000)     6605 2023-04-21 13:03:22.000000 GDAL-3.6.4/gdal-utils/GDAL.egg-info/PKG-INFO
+-rw-rw-r--   0 even      (1000) even      (1000)     5228 2023-04-21 13:03:22.000000 GDAL-3.6.4/gdal-utils/GDAL.egg-info/SOURCES.txt
+-rw-rw-r--   0 even      (1000) even      (1000)        1 2023-04-21 13:03:22.000000 GDAL-3.6.4/gdal-utils/GDAL.egg-info/dependency_links.txt
+-rw-rw-r--   0 even      (1000) even      (1000)        1 2022-11-11 10:46:54.000000 GDAL-3.6.4/gdal-utils/GDAL.egg-info/not-zip-safe
+-rw-rw-r--   0 even      (1000) even      (1000)       21 2023-04-21 13:03:22.000000 GDAL-3.6.4/gdal-utils/GDAL.egg-info/requires.txt
+-rw-rw-r--   0 even      (1000) even      (1000)       18 2023-04-21 13:03:22.000000 GDAL-3.6.4/gdal-utils/GDAL.egg-info/top_level.txt
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-04-21 13:03:22.896005 GDAL-3.6.4/gdal-utils/osgeo_utils/
+-rw-rw-r--   0 even      (1000) even      (1000)      432 2023-04-17 11:44:56.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/__init__.py
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-04-21 13:03:22.896005 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/
+-rw-rw-r--   0 even      (1000) even      (1000)        0 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/__init__.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2635 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/array_util.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4044 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/base.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3447 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/batch_creator.py
+-rw-rw-r--   0 even      (1000) even      (1000)    15215 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/color_palette.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5649 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/color_table.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5384 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/extent_util.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6566 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/gdal_argparse.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2721 2023-01-11 18:52:28.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/numpy_util.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5467 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/osr_util.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3340 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/progress.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6671 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/raster_creation.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8828 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/rectangle.py
+-rw-rw-r--   0 even      (1000) even      (1000)    16651 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/util.py
+-rw-rw-r--   0 even      (1000) even      (1000)   166201 2023-04-11 22:51:25.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/gdal2tiles.py
+-rw-rw-r--   0 even      (1000) even      (1000)    15776 2023-03-13 21:01:59.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/gdal2xyz.py
+-rw-rw-r--   0 even      (1000) even      (1000)    36264 2023-01-11 18:52:28.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_calc.py
+-rw-rw-r--   0 even      (1000) even      (1000)    15155 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_edit.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8936 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_fillnodata.py
+-rw-rw-r--   0 even      (1000) even      (1000)    18299 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_merge.py
+-rw-rw-r--   0 even      (1000) even      (1000)    11772 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_pansharpen.py
+-rw-rw-r--   0 even      (1000) even      (1000)    10303 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_polygonize.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7052 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_proximity.py
+-rw-rw-r--   0 even      (1000) even      (1000)    35616 2023-01-27 19:56:58.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_retile.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6441 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_sieve.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4794 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/gdalattachpct.py
+-rw-rw-r--   0 even      (1000) even      (1000)    11855 2023-03-13 21:01:59.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/gdalcompare.py
+-rw-rw-r--   0 even      (1000) even      (1000)     9796 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/gdalmove.py
+-rw-rw-r--   0 even      (1000) even      (1000)    18128 2022-12-12 12:52:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/ogr_layer_algebra.py
+-rw-rw-r--   0 even      (1000) even      (1000)    22455 2023-01-11 18:52:28.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/ogrmerge.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7664 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/pct2rgb.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7145 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/rgb2pct.py
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-04-21 13:03:22.908005 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/
+-rw-rw-r--   0 even      (1000) even      (1000)        0 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/__init__.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4632 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/assemblepoly.py
+-rw-rw-r--   0 even      (1000) even      (1000)    17347 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/build_jp2_from_xml.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2828 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/classify.py
+-rw-rw-r--   0 even      (1000) even      (1000)    12326 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/crs2crs2grid.py
+-rw-rw-r--   0 even      (1000) even      (1000)    16769 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/densify.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8126 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/dump_jp2.py
+-rw-rw-r--   0 even      (1000) even      (1000)     9915 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/epsg_tr.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3238 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/esri2wkt.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4274 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/fft.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3008 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/fix_gpkg.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3193 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gcps2ogr.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5419 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gcps2vec.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2580 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gcps2wld.py
+-rw-rw-r--   0 even      (1000) even      (1000)     5281 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal2grd.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4451 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_auth.py
+-rw-rw-r--   0 even      (1000) even      (1000)    11309 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_cp.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2561 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_create_pdf.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8693 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_ls.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6668 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_lut.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2403 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_mkdir.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4426 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_remove_towgs84.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4035 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_rm.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2538 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_rmdir.py
+-rw-rw-r--   0 even      (1000) even      (1000)    11900 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_vrtmerge.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4069 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_zip.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3004 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdalchksum.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3004 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdalcopyproj.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6067 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdalfilter.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3021 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdalident.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3036 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdalimport.py
+-rw-rw-r--   0 even      (1000) even      (1000)    22185 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdalinfo.py
+-rw-rw-r--   0 even      (1000) even      (1000)    20066 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdallocationinfo.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4095 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/get_soundg.py
+-rw-rw-r--   0 even      (1000) even      (1000)     3374 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/histrep.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8150 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/hsv_merge.py
+-rw-rw-r--   0 even      (1000) even      (1000)    10510 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/jpeg_in_tiff_extract.py
+-rw-rw-r--   0 even      (1000) even      (1000)     6440 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/load2odbc.py
+-rw-rw-r--   0 even      (1000) even      (1000)     8847 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/loslas2ntv2.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2739 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/magphase.py
+-rw-rw-r--   0 even      (1000) even      (1000)     2167 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/make_fuzzer_friendly_archive.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7547 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/mkgraticule.py
+-rw-rw-r--   0 even      (1000) even      (1000)    70278 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/ogr2ogr.py
+-rw-rw-r--   0 even      (1000) even      (1000)    12582 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/ogr2vrt.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7567 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/ogr_build_junction_table.py
+-rw-rw-r--   0 even      (1000) even      (1000)    14345 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/ogr_dispatch.py
+-rw-rw-r--   0 even      (1000) even      (1000)    21229 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/ogrinfo.py
+-rw-rw-r--   0 even      (1000) even      (1000)    19843 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/ogrupdate.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7724 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/rel.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7578 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/tigerpoly.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4368 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/tile_extent_from_raster.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4055 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/tolatlong.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4344 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/val_repl.py
+-rw-rw-r--   0 even      (1000) even      (1000)    18476 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/validate_cloud_optimized_geotiff.py
+-rw-rw-r--   0 even      (1000) even      (1000)   108556 2023-01-11 18:52:28.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/validate_gpkg.py
+-rw-rw-r--   0 even      (1000) even      (1000)    70659 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/validate_jp2.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4768 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/vec_tr.py
+-rw-rw-r--   0 even      (1000) even      (1000)     4843 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/vec_tr_spat.py
+-rw-rw-r--   0 even      (1000) even      (1000)     7103 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/osgeo_utils/samples/wcs_virtds_params.py
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-04-21 13:03:22.908005 GDAL-3.6.4/gdal-utils/scripts/
+-rwxrwxr-x   0 even      (1000) even      (1000)      504 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/gdal2tiles.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      279 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/gdal2xyz.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      283 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/gdal_calc.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      283 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/gdal_edit.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      307 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/gdal_fillnodata.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      287 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/gdal_merge.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      307 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/gdal_pansharpen.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      307 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/gdal_polygonize.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      303 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/gdal_proximity.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      291 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/gdal_retile.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      287 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/gdal_sieve.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      299 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/gdalattachpct.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      291 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/gdalcompare.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      279 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/gdalmove.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      315 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/ogr_layer_algebra.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      279 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/ogrmerge.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      275 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/pct2rgb.py
+-rwxrwxr-x   0 even      (1000) even      (1000)      275 2022-11-03 17:38:53.000000 GDAL-3.6.4/gdal-utils/scripts/rgb2pct.py
+drwxrwxr-x   0 even      (1000) even      (1000)        0 2023-04-21 13:03:22.912005 GDAL-3.6.4/osgeo/
+-rw-rw-r--   0 even      (1000) even      (1000)     5418 2023-04-21 13:02:18.000000 GDAL-3.6.4/osgeo/__init__.py
+-rw-rw-r--   0 even      (1000) even      (1000)   208954 2023-04-21 13:02:18.000000 GDAL-3.6.4/osgeo/gdal.py
+-rw-rw-r--   0 even      (1000) even      (1000)    27755 2023-04-21 13:02:18.000000 GDAL-3.6.4/osgeo/gdal_array.py
+-rw-rw-r--   0 even      (1000) even      (1000)    11844 2023-04-21 13:02:18.000000 GDAL-3.6.4/osgeo/gdalconst.py
+-rw-rw-r--   0 even      (1000) even      (1000)      214 2023-04-21 13:02:18.000000 GDAL-3.6.4/osgeo/gdalnumeric.py
+-rw-rw-r--   0 even      (1000) even      (1000)     9892 2023-04-21 13:02:18.000000 GDAL-3.6.4/osgeo/gnm.py
+-rw-rw-r--   0 even      (1000) even      (1000)   221000 2023-04-21 13:02:18.000000 GDAL-3.6.4/osgeo/ogr.py
+-rw-rw-r--   0 even      (1000) even      (1000)    55075 2023-04-21 13:02:18.000000 GDAL-3.6.4/osgeo/osr.py
+-rw-rw-r--   0 even      (1000) even      (1000)       38 2023-04-21 13:03:22.912005 GDAL-3.6.4/setup.cfg
+-rw-rw-r--   0 even      (1000) even      (1000)    13847 2023-04-21 12:57:58.000000 GDAL-3.6.4/setup.py
```

### Comparing `GDAL-3.6.3/PKG-INFO` & `GDAL-3.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GDAL
-Version: 3.6.3
+Version: 3.6.4
 Summary: GDAL: Geospatial Data Abstraction Library
 Home-page: http://www.gdal.org
 Author: Frank Warmerdam
 Author-email: warmerdam@pobox.com
 Maintainer: Howard Butler
 Maintainer-email: hobu.inc@gmail.com
 License: MIT
@@ -37,15 +37,15 @@
 bindings for GDAL and OGR. Generally speaking the classes and methods mostly
 match those of the GDAL and OGR C++ classes. There is no Python specific
 reference documentation, but the `GDAL API Tutorial`_ includes Python examples.
 
 Dependencies
 ------------
 
- * libgdal (3.6.3 or greater) and header files (gdal-devel)
+ * libgdal (3.6.4 or greater) and header files (gdal-devel)
  * numpy (1.0.0 or greater) and header files (numpy-devel) (not explicitly
    required, but many examples and utilities will not work without it)
 
 Installation
 ------------
 
 Conda
```

### Comparing `GDAL-3.6.3/README.rst` & `GDAL-3.6.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 bindings for GDAL and OGR. Generally speaking the classes and methods mostly
 match those of the GDAL and OGR C++ classes. There is no Python specific
 reference documentation, but the `GDAL API Tutorial`_ includes Python examples.
 
 Dependencies
 ------------
 
- * libgdal (3.6.3 or greater) and header files (gdal-devel)
+ * libgdal (3.6.4 or greater) and header files (gdal-devel)
  * numpy (1.0.0 or greater) and header files (numpy-devel) (not explicitly
    required, but many examples and utilities will not work without it)
 
 Installation
 ------------
 
 Conda
```

### Comparing `GDAL-3.6.3/extensions/gdal_array_wrap.cpp` & `GDAL-3.6.4/extensions/gdal_array_wrap.cpp`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/extensions/gdal_wrap.cpp` & `GDAL-3.6.4/extensions/gdal_wrap.cpp`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/extensions/gdalconst_wrap.c` & `GDAL-3.6.4/extensions/gdalconst_wrap.c`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/extensions/gnm_wrap.cpp` & `GDAL-3.6.4/extensions/gnm_wrap.cpp`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/extensions/ogr_wrap.cpp` & `GDAL-3.6.4/extensions/ogr_wrap.cpp`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/extensions/osr_wrap.cpp` & `GDAL-3.6.4/extensions/osr_wrap.cpp`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/GDAL.egg-info/PKG-INFO` & `GDAL-3.6.4/gdal-utils/GDAL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GDAL
-Version: 3.6.3
+Version: 3.6.4
 Summary: GDAL: Geospatial Data Abstraction Library
 Home-page: http://www.gdal.org
 Author: Frank Warmerdam
 Author-email: warmerdam@pobox.com
 Maintainer: Howard Butler
 Maintainer-email: hobu.inc@gmail.com
 License: MIT
@@ -37,15 +37,15 @@
 bindings for GDAL and OGR. Generally speaking the classes and methods mostly
 match those of the GDAL and OGR C++ classes. There is no Python specific
 reference documentation, but the `GDAL API Tutorial`_ includes Python examples.
 
 Dependencies
 ------------
 
- * libgdal (3.6.3 or greater) and header files (gdal-devel)
+ * libgdal (3.6.4 or greater) and header files (gdal-devel)
  * numpy (1.0.0 or greater) and header files (numpy-devel) (not explicitly
    required, but many examples and utilities will not work without it)
 
 Installation
 ------------
 
 Conda
```

### Comparing `GDAL-3.6.3/gdal-utils/GDAL.egg-info/SOURCES.txt` & `GDAL-3.6.4/gdal-utils/GDAL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/array_util.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/array_util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/base.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/base.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/batch_creator.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/batch_creator.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/color_palette.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/color_palette.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/color_table.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/color_table.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/extent_util.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/extent_util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/gdal_argparse.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/gdal_argparse.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/numpy_util.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/numpy_util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/osr_util.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/osr_util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/progress.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/progress.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/raster_creation.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/raster_creation.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/rectangle.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/rectangle.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/auxiliary/util.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/auxiliary/util.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/gdal2tiles.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/gdal2tiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -3910,16 +3910,16 @@
         h1 { margin: 0; padding: 6px; border:0; font-size: 20pt; }
         #header { height: 43px; padding: 0; background-color: #eee; border: 1px solid #888; }
         #subheader { height: 12px; text-align: right; font-size: 10px; color: #555;}
         #map { height: 90%%; border: 1px solid #888; }
     </style>
     <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/openlayers/openlayers.github.io@main/dist/en/v7.0.0/legacy/ol.css" type="text/css">
     <script src="https://cdn.jsdelivr.net/gh/openlayers/openlayers.github.io@main/dist/en/v7.0.0/legacy/ol.js"></script>
-    <script src="https://unpkg.com/ol-layerswitcher@3.5.0"></script>
-    <link rel="stylesheet" href="https://unpkg.com/ol-layerswitcher@3.5.0/src/ol-layerswitcher.css" />
+    <script src="https://unpkg.com/ol-layerswitcher@4.1.1"></script>
+    <link rel="stylesheet" href="https://unpkg.com/ol-layerswitcher@4.1.1/src/ol-layerswitcher.css" />
 </head>
 <body>
     <div id="header"><h1>%(xml_escaped_title)s</h1></div>
     <div id="subheader">Generated by <a href="https://gdal.org/programs/gdal2tiles.html">GDAL2Tiles</a>&nbsp;&nbsp;&nbsp;&nbsp;</div>
     <div id="map" class="map"></div>
     <div id="mouse-position"></div>
     <script type="text/javascript">
```

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/gdal2xyz.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/gdal2xyz.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 ###############################################################################
 import sys
 import textwrap
-from numbers import Number, Real
+from numbers import Number
 from typing import Optional, Sequence, Tuple, Union
 
 import numpy as np
 
 from osgeo import gdal
 from osgeo_utils.auxiliary.base import PathLikeOrStr
 from osgeo_utils.auxiliary.gdal_argparse import GDALArgumentParser, GDALScript
@@ -304,25 +304,25 @@
             help="Exclude the output lines with nodata value (as determined by srcnodata).",
         )
 
         parser.add_argument(
             "-srcnodata",
             "-nodatavalue",
             dest="src_nodata",
-            type=Real,
+            type=float,
             nargs="*",
             help="The nodata value of the dataset (for skipping or replacing) "
             "Default (None) - Use the dataset nodata value; "
             "Sequence/Number - Use the given nodata value (per band or per dataset).",
         )
 
         parser.add_argument(
             "-dstnodata",
             dest="dst_nodata",
-            type=Real,
+            type=float,
             nargs="*",
             help="Replace source nodata with a given nodata. "
             "Has an effect only if not setting -skipnodata. "
             "Default(None) - Use srcnodata, no replacement; "
             "Sequence/Number - Replace the srcnodata with the given nodata value "
             "(per band or per dataset).",
         )
@@ -348,39 +348,70 @@
         def checkInt(s):
             try:
                 int(s)
                 return True
             except ValueError:
                 return False
 
+        def checkFloat(s):
+            try:
+                float(s)
+                return True
+            except ValueError:
+                return False
+
         # We allowed "-b band_number_1 [... band_number_X] srcfile dstfile" syntax
         # before switching to ArgParse. But ArgParse doesn't like that.
         # So manually parse -b argument and strip it before ArgParse.
         count = len(argv)
         new_argv = []
         i = 0
         band_nums = []
+        src_nodata = []
+        dst_nodata = []
         while i < count:
             arg = argv[i]
             if arg in ("-b", "-band", "--band"):
                 if i == count - 1:
                     raise Exception(f"Missing argument following {arg}: ")
                 i += 1
                 if not checkInt(argv[i]):
                     raise Exception(f"Argument following {arg} should be a integer")
                 while i < count and checkInt(argv[i]):
                     band_nums.append(int(argv[i]))
                     i += 1
+            elif arg in ("-srcnodata", "-nodatavalue"):
+                if i == count - 1:
+                    raise Exception(f"Missing argument following {arg}: ")
+                i += 1
+                if not checkFloat(argv[i]):
+                    raise Exception(f"Argument following {arg} should be a float")
+                while i < count and checkFloat(argv[i]):
+                    src_nodata.append(float(argv[i]))
+                    i += 1
+            elif arg in ("-dstnodata"):
+                if i == count - 1:
+                    raise Exception(f"Missing argument following {arg}: ")
+                i += 1
+                if not checkFloat(argv[i]):
+                    raise Exception(f"Argument following {arg} should be a float")
+                while i < count and checkFloat(argv[i]):
+                    dst_nodata.append(float(argv[i]))
+                    i += 1
             else:
                 i += 1
                 new_argv.append(arg)
 
         kwargs = super(GDAL2XYZ, self).parse(new_argv)
         if band_nums:
             kwargs["band_nums"] = band_nums
+        if src_nodata:
+            kwargs["src_nodata"] = src_nodata
+        if dst_nodata:
+            kwargs["dst_nodata"] = dst_nodata
         return kwargs
 
     def augment_kwargs(self, kwargs) -> dict:
         if kwargs.get("allbands"):
             kwargs["band_nums"] = None
         elif not kwargs.get("band_nums"):
             kwargs["band_nums"] = 1
```

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_calc.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_calc.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_edit.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_edit.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_fillnodata.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_fillnodata.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_merge.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_merge.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_pansharpen.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_pansharpen.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_polygonize.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_polygonize.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_proximity.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_proximity.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_retile.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_retile.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/gdal_sieve.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/gdal_sieve.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/gdalattachpct.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/gdalattachpct.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/gdalcompare.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/gdalcompare.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 #  THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 # ******************************************************************************
 
 import filecmp
+import math
 import os
 import sys
 
 from osgeo import gdal, osr
 
 #######################################################
 from osgeo_utils.auxiliary.base import PathLikeOrStr
@@ -95,19 +96,28 @@
 
     if golden_band.DataType != new_band.DataType:
         print("Band %s pixel types differ." % ident)
         print("  Golden: " + gdal.GetDataTypeName(golden_band.DataType))
         print("  New:    " + gdal.GetDataTypeName(new_band.DataType))
         found_diff += 1
 
-    if golden_band.GetNoDataValue() != new_band.GetNoDataValue():
-        print("Band %s nodata values differ." % ident)
-        print("  Golden: " + str(golden_band.GetNoDataValue()))
-        print("  New:    " + str(new_band.GetNoDataValue()))
-        found_diff += 1
+    golden_band_nodata = golden_band.GetNoDataValue()
+    new_band_nodata = new_band.GetNoDataValue()
+    if golden_band_nodata != new_band_nodata:
+        if golden_band_nodata and new_band_nodata:
+            if not (math.isnan(golden_band_nodata) and math.isnan(new_band_nodata)):
+                print("Band %s nodata values differ." % ident)
+                print("  Golden: " + str(golden_band_nodata))
+                print("  New:    " + str(new_band_nodata))
+                found_diff += 1
+        else:
+            print("Band %s nodata values differ." % ident)
+            print("  Golden: " + str(golden_band_nodata))
+            print("  New:    " + str(new_band_nodata))
+            found_diff += 1
 
     if golden_band.GetColorInterpretation() != new_band.GetColorInterpretation():
         print("Band %s color interpretation values differ." % ident)
         print(
             "  Golden: "
             + gdal.GetColorInterpretationName(golden_band.GetColorInterpretation())
         )
```

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/gdalmove.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/gdalmove.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/ogr_layer_algebra.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/ogr_layer_algebra.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/ogrmerge.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/ogrmerge.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/pct2rgb.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/pct2rgb.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/rgb2pct.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/rgb2pct.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/assemblepoly.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/assemblepoly.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/build_jp2_from_xml.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/build_jp2_from_xml.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/classify.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/classify.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/crs2crs2grid.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/crs2crs2grid.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/densify.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/densify.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/dump_jp2.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/dump_jp2.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/epsg_tr.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/epsg_tr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/esri2wkt.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/esri2wkt.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/fft.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/fft.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/fix_gpkg.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/fix_gpkg.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gcps2ogr.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gcps2ogr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gcps2vec.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gcps2vec.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gcps2wld.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gcps2wld.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal2grd.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal2grd.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_auth.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_auth.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_cp.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_cp.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_create_pdf.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_create_pdf.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_ls.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_ls.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_lut.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_lut.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_mkdir.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_mkdir.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_remove_towgs84.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_remove_towgs84.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_rm.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_rm.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_rmdir.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_rmdir.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_vrtmerge.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_vrtmerge.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdal_zip.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdal_zip.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdalchksum.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdalchksum.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdalcopyproj.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdalcopyproj.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdalfilter.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdalfilter.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdalident.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdalident.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdalimport.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdalimport.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdalinfo.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdalinfo.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/gdallocationinfo.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/gdallocationinfo.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/get_soundg.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/get_soundg.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/histrep.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/histrep.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/hsv_merge.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/hsv_merge.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/jpeg_in_tiff_extract.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/jpeg_in_tiff_extract.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/load2odbc.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/load2odbc.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/loslas2ntv2.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/loslas2ntv2.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/magphase.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/magphase.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/make_fuzzer_friendly_archive.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/make_fuzzer_friendly_archive.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/mkgraticule.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/mkgraticule.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/ogr2ogr.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/ogr2ogr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/ogr2vrt.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/ogr2vrt.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/ogr_build_junction_table.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/ogr_build_junction_table.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/ogr_dispatch.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/ogr_dispatch.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/ogrinfo.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/ogrinfo.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/ogrupdate.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/ogrupdate.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/rel.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/rel.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/tigerpoly.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/tigerpoly.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/tile_extent_from_raster.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/tile_extent_from_raster.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/tolatlong.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/tolatlong.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/val_repl.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/val_repl.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/validate_cloud_optimized_geotiff.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/validate_cloud_optimized_geotiff.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/validate_gpkg.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/validate_gpkg.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/validate_jp2.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/validate_jp2.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/vec_tr.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/vec_tr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/vec_tr_spat.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/vec_tr_spat.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/gdal-utils/osgeo_utils/samples/wcs_virtds_params.py` & `GDAL-3.6.4/gdal-utils/osgeo_utils/samples/wcs_virtds_params.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/osgeo/__init__.py` & `GDAL-3.6.4/osgeo/__init__.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/osgeo/gdal.py` & `GDAL-3.6.4/osgeo/gdal.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/osgeo/gdal_array.py` & `GDAL-3.6.4/osgeo/gdal_array.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/osgeo/gdalconst.py` & `GDAL-3.6.4/osgeo/gdalconst.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/osgeo/gnm.py` & `GDAL-3.6.4/osgeo/gnm.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/osgeo/ogr.py` & `GDAL-3.6.4/osgeo/ogr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/osgeo/osr.py` & `GDAL-3.6.4/osgeo/osr.py`

 * *Files identical despite different names*

### Comparing `GDAL-3.6.3/setup.py` & `GDAL-3.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 packages = find_packages(utils_package_root)
 packages = ['osgeo'] + packages
 package_dir = {'osgeo': 'osgeo', '': utils_package_root}
 
 readme = open('README.rst', encoding="utf-8").read()
 
 name = 'GDAL'
-version = '3.6.3'
+version = '3.6.4'
 author = "Frank Warmerdam"
 author_email = "warmerdam@pobox.com"
 maintainer = "Howard Butler"
 maintainer_email = "hobu.inc@gmail.com"
 description = "GDAL: Geospatial Data Abstraction Library"
 license_type = "MIT"
 url = "http://www.gdal.org"
```

