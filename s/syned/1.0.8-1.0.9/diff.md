# Comparing `tmp/syned-1.0.8.tar.gz` & `tmp/syned-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/syned-1.0.8.tar", last modified: Thu May 31 15:37:22 2018, max compression
+gzip compressed data, was "dist/syned-1.0.9.tar", last modified: Wed Oct  3 14:43:56 2018, max compression
```

## Comparing `syned-1.0.8.tar` & `syned-1.0.9.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/
--rwxr-xr-x   0 root         (0) staff       (20)       78 2017-09-07 12:41:27.000000 syned-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)     1472 2018-05-31 15:37:22.000000 syned-1.0.8/PKG-INFO
--rwxr-xr-x   0 root         (0) staff       (20)      263 2017-01-30 09:04:48.000000 syned-1.0.8/README.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2018-05-31 15:37:22.000000 syned-1.0.8/setup.cfg
--rwxr-xr-x   0 root         (0) staff       (20)     4222 2018-05-31 15:36:57.000000 syned-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/syned/
--rw-r--r--   0 root         (0) staff       (20)        0 2017-01-30 09:04:48.000000 syned-1.0.8/syned/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/syned/beamline/
--rw-r--r--   0 root         (0) staff       (20)        1 2017-01-30 09:04:48.000000 syned-1.0.8/syned/beamline/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     2691 2017-06-13 12:32:44.000000 syned-1.0.8/syned/beamline/beamline.py
--rw-r--r--   0 root         (0) staff       (20)      965 2017-02-28 10:18:30.000000 syned-1.0.8/syned/beamline/beamline_element.py
--rw-r--r--   0 root         (0) staff       (20)     1398 2017-06-13 11:48:29.000000 syned-1.0.8/syned/beamline/element_coordinates.py
--rw-r--r--   0 root         (0) staff       (20)      657 2017-02-28 10:18:30.000000 syned-1.0.8/syned/beamline/optical_element.py
--rw-r--r--   0 root         (0) staff       (20)      512 2017-02-28 10:18:30.000000 syned-1.0.8/syned/beamline/optical_element_with_surface_shape.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/syned/beamline/optical_elements/
--rw-r--r--   0 root         (0) staff       (20)       21 2017-01-30 09:04:48.000000 syned-1.0.8/syned/beamline/optical_elements/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/syned/beamline/optical_elements/absorbers/
--rw-r--r--   0 root         (0) staff       (20)        0 2017-01-30 09:04:48.000000 syned-1.0.8/syned/beamline/optical_elements/absorbers/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      292 2017-07-28 08:11:05.000000 syned-1.0.8/syned/beamline/optical_elements/absorbers/absorber.py
--rw-r--r--   0 root         (0) staff       (20)      610 2017-07-28 08:14:26.000000 syned-1.0.8/syned/beamline/optical_elements/absorbers/beam_stopper.py
--rw-r--r--   0 root         (0) staff       (20)      791 2017-07-28 08:14:26.000000 syned-1.0.8/syned/beamline/optical_elements/absorbers/filter.py
--rw-r--r--   0 root         (0) staff       (20)      605 2017-07-28 08:14:26.000000 syned-1.0.8/syned/beamline/optical_elements/absorbers/slit.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/syned/beamline/optical_elements/crystals/
--rw-r--r--   0 root         (0) staff       (20)        0 2017-01-30 09:04:48.000000 syned-1.0.8/syned/beamline/optical_elements/crystals/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1982 2017-07-23 16:20:42.000000 syned-1.0.8/syned/beamline/optical_elements/crystals/crystal.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/syned/beamline/optical_elements/gratings/
--rw-r--r--   0 root         (0) staff       (20)        0 2017-01-30 09:04:48.000000 syned-1.0.8/syned/beamline/optical_elements/gratings/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      979 2017-02-28 10:18:30.000000 syned-1.0.8/syned/beamline/optical_elements/gratings/grating.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/syned/beamline/optical_elements/ideal_elements/
--rw-r--r--   0 root         (0) staff       (20)        0 2017-01-30 09:04:48.000000 syned-1.0.8/syned/beamline/optical_elements/ideal_elements/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      296 2017-07-28 08:14:26.000000 syned-1.0.8/syned/beamline/optical_elements/ideal_elements/ideal_element.py
--rw-r--r--   0 root         (0) staff       (20)      761 2017-07-28 08:14:26.000000 syned-1.0.8/syned/beamline/optical_elements/ideal_elements/lens.py
--rw-r--r--   0 root         (0) staff       (20)      237 2017-07-28 08:14:26.000000 syned-1.0.8/syned/beamline/optical_elements/ideal_elements/screen.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/syned/beamline/optical_elements/mirrors/
--rw-r--r--   0 root         (0) staff       (20)        0 2017-01-30 09:04:48.000000 syned-1.0.8/syned/beamline/optical_elements/mirrors/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1159 2017-02-28 10:18:30.000000 syned-1.0.8/syned/beamline/optical_elements/mirrors/mirror.py
--rw-r--r--   0 root         (0) staff       (20)    11664 2018-04-16 08:25:10.000000 syned-1.0.8/syned/beamline/shape.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/syned/examples/
--rw-r--r--   0 root         (0) staff       (20)       20 2017-02-28 10:18:30.000000 syned-1.0.8/syned/examples/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4552 2017-07-29 08:39:33.000000 syned-1.0.8/syned/examples/example_beamline.py
--rw-r--r--   0 root         (0) staff       (20)     4254 2017-04-04 09:00:24.000000 syned-1.0.8/syned/examples/example_json_input_output.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/syned/storage_ring/
--rw-r--r--   0 root         (0) staff       (20)       22 2017-01-30 09:04:48.000000 syned-1.0.8/syned/storage_ring/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5202 2017-07-24 12:26:12.000000 syned-1.0.8/syned/storage_ring/electron_beam.py
--rw-r--r--   0 root         (0) staff       (20)     1121 2017-02-28 10:18:30.000000 syned-1.0.8/syned/storage_ring/light_source.py
--rw-r--r--   0 root         (0) staff       (20)      231 2017-02-28 10:18:30.000000 syned-1.0.8/syned/storage_ring/magnetic_structure.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/syned/storage_ring/magnetic_structures/
--rw-r--r--   0 root         (0) staff       (20)       22 2017-01-30 09:04:48.000000 syned-1.0.8/syned/storage_ring/magnetic_structures/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1793 2017-07-08 09:55:05.000000 syned-1.0.8/syned/storage_ring/magnetic_structures/bending_magnet.py
--rw-r--r--   0 root         (0) staff       (20)     2289 2017-07-26 10:16:17.000000 syned-1.0.8/syned/storage_ring/magnetic_structures/insertion_device.py
--rw-r--r--   0 root         (0) staff       (20)     2232 2017-07-26 15:32:19.000000 syned-1.0.8/syned/storage_ring/magnetic_structures/undulator.py
--rw-r--r--   0 root         (0) staff       (20)      551 2017-03-28 08:25:23.000000 syned-1.0.8/syned/storage_ring/magnetic_structures/wiggler.py
--rw-r--r--   0 root         (0) staff       (20)     3934 2017-02-28 10:18:30.000000 syned-1.0.8/syned/syned_object.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/syned/util/
--rw-r--r--   0 root         (0) staff       (20)        0 2017-04-04 08:58:43.000000 syned-1.0.8/syned/util/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5416 2017-05-11 10:06:06.000000 syned-1.0.8/syned/util/json_tools.py
--rw-r--r--   0 root         (0) staff       (20)      270 2018-05-31 15:37:22.000000 syned-1.0.8/syned/version.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/syned/widget/
--rw-r--r--   0 root         (0) staff       (20)        0 2017-05-02 11:50:07.000000 syned-1.0.8/syned/widget/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      443 2017-07-21 09:20:21.000000 syned-1.0.8/syned/widget/widget_decorator.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-31 15:37:22.000000 syned-1.0.8/syned.egg-info/
--rw-r--r--   0 root         (0) staff       (20)        1 2018-05-31 15:37:22.000000 syned-1.0.8/syned.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2017-01-30 09:05:42.000000 syned-1.0.8/syned.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)     1472 2018-05-31 15:37:22.000000 syned-1.0.8/syned.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)       23 2018-05-31 15:37:22.000000 syned-1.0.8/syned.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)     1981 2018-05-31 15:37:22.000000 syned-1.0.8/syned.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2018-05-31 15:37:22.000000 syned-1.0.8/syned.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/
+-rw-r--r--   0 root         (0) staff       (20)     1472 2018-10-03 14:43:56.000000 syned-1.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/syned/
+-rw-r--r--   0 root         (0) staff       (20)      270 2018-10-03 14:43:56.000000 syned-1.0.9/syned/version.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/syned/widget/
+-rw-r--r--   0 root         (0) staff       (20)      443 2018-08-15 09:07:34.000000 syned-1.0.9/syned/widget/widget_decorator.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2018-08-15 09:07:34.000000 syned-1.0.9/syned/widget/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/syned/util/
+-rw-r--r--   0 root         (0) staff       (20)     6365 2018-10-03 14:42:49.000000 syned-1.0.9/syned/util/json_tools.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2018-08-15 09:07:34.000000 syned-1.0.9/syned/util/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2018-08-15 09:07:34.000000 syned-1.0.9/syned/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3981 2018-09-18 15:16:45.000000 syned-1.0.9/syned/syned_object.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/syned/examples/
+-rw-r--r--   0 root         (0) staff       (20)     4254 2018-08-15 09:07:34.000000 syned-1.0.9/syned/examples/example_json_input_output.py
+-rw-r--r--   0 root         (0) staff       (20)       20 2018-08-15 09:07:34.000000 syned-1.0.9/syned/examples/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4630 2018-09-18 15:16:45.000000 syned-1.0.9/syned/examples/example_beamline.py
+-rw-r--r--   0 root         (0) staff       (20)     2665 2018-10-03 14:42:49.000000 syned-1.0.9/syned/examples/example_json_double_slit.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/syned/storage_ring/
+-rw-r--r--   0 root         (0) staff       (20)     1121 2018-08-15 09:07:34.000000 syned-1.0.9/syned/storage_ring/light_source.py
+-rw-r--r--   0 root         (0) staff       (20)       22 2018-08-15 09:07:34.000000 syned-1.0.9/syned/storage_ring/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/syned/storage_ring/magnetic_structures/
+-rw-r--r--   0 root         (0) staff       (20)     2289 2018-08-15 09:07:34.000000 syned-1.0.9/syned/storage_ring/magnetic_structures/insertion_device.py
+-rw-r--r--   0 root         (0) staff       (20)       22 2018-08-15 09:07:34.000000 syned-1.0.9/syned/storage_ring/magnetic_structures/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1793 2018-08-15 09:07:34.000000 syned-1.0.9/syned/storage_ring/magnetic_structures/bending_magnet.py
+-rw-r--r--   0 root         (0) staff       (20)      551 2018-08-15 09:07:34.000000 syned-1.0.9/syned/storage_ring/magnetic_structures/wiggler.py
+-rw-r--r--   0 root         (0) staff       (20)     2274 2018-09-18 15:16:45.000000 syned-1.0.9/syned/storage_ring/magnetic_structures/undulator.py
+-rw-r--r--   0 root         (0) staff       (20)      544 2018-09-20 13:57:32.000000 syned-1.0.9/syned/storage_ring/empty_light_source.py
+-rw-r--r--   0 root         (0) staff       (20)      231 2018-08-15 09:07:34.000000 syned-1.0.9/syned/storage_ring/magnetic_structure.py
+-rw-r--r--   0 root         (0) staff       (20)     5202 2018-08-15 09:07:34.000000 syned-1.0.9/syned/storage_ring/electron_beam.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/syned/beamline/
+-rw-r--r--   0 root         (0) staff       (20)     2848 2018-09-20 13:57:17.000000 syned-1.0.9/syned/beamline/beamline.py
+-rw-r--r--   0 root         (0) staff       (20)      512 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_element_with_surface_shape.py
+-rw-r--r--   0 root         (0) staff       (20)        1 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      657 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_element.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/syned/beamline/optical_elements/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/syned/beamline/optical_elements/ideal_elements/
+-rw-r--r--   0 root         (0) staff       (20)      237 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/ideal_elements/screen.py
+-rw-r--r--   0 root         (0) staff       (20)      761 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/ideal_elements/lens.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/ideal_elements/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      296 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/ideal_elements/ideal_element.py
+-rw-r--r--   0 root         (0) staff       (20)       21 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/syned/beamline/optical_elements/mirrors/
+-rw-r--r--   0 root         (0) staff       (20)     1159 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/mirrors/mirror.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/mirrors/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/syned/beamline/optical_elements/crystals/
+-rw-r--r--   0 root         (0) staff       (20)     1982 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/crystals/crystal.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/crystals/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/syned/beamline/optical_elements/absorbers/
+-rw-r--r--   0 root         (0) staff       (20)      872 2018-10-03 14:42:49.000000 syned-1.0.9/syned/beamline/optical_elements/absorbers/slit.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/absorbers/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      292 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/absorbers/absorber.py
+-rw-r--r--   0 root         (0) staff       (20)      610 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/absorbers/beam_stopper.py
+-rw-r--r--   0 root         (0) staff       (20)      791 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/absorbers/filter.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/syned/beamline/optical_elements/gratings/
+-rw-r--r--   0 root         (0) staff       (20)        0 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/gratings/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      979 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/optical_elements/gratings/grating.py
+-rw-r--r--   0 root         (0) staff       (20)    16563 2018-10-03 14:42:49.000000 syned-1.0.9/syned/beamline/shape.py
+-rw-r--r--   0 root         (0) staff       (20)     1398 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/element_coordinates.py
+-rw-r--r--   0 root         (0) staff       (20)      965 2018-08-15 09:07:34.000000 syned-1.0.9/syned/beamline/beamline_element.py
+-rwxr-xr-x   0 root         (0) staff       (20)       78 2018-08-15 09:07:34.000000 syned-1.0.9/MANIFEST.in
+-rwxr-xr-x   0 root         (0) staff       (20)     4222 2018-10-03 14:43:43.000000 syned-1.0.9/setup.py
+-rwxr-xr-x   0 root         (0) staff       (20)      263 2018-08-15 09:07:34.000000 syned-1.0.9/README.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2018-10-03 14:43:56.000000 syned-1.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2018-10-03 14:43:56.000000 syned-1.0.9/syned.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     1472 2018-10-03 14:43:56.000000 syned-1.0.9/syned.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)        1 2018-09-17 21:26:28.000000 syned-1.0.9/syned.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)     2065 2018-10-03 14:43:56.000000 syned-1.0.9/syned.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)       23 2018-10-03 14:43:56.000000 syned-1.0.9/syned.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2018-10-03 14:43:56.000000 syned-1.0.9/syned.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2018-10-03 14:43:56.000000 syned-1.0.9/syned.egg-info/dependency_links.txt
```

### Comparing `syned-1.0.8/PKG-INFO` & `syned-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: syned
-Version: 1.0.8
+Version: 1.0.9
 Summary: SYNED (SYNchrotron Elements Dictionary) kernel library
 Home-page: https://github.com/lucarebuffi/syned
 Author: Manuel Sanchez del Rio, Luca Rebuffi
 Author-email: srio@esrf.eu
 Maintainer: Luca Rebuffi
 Maintainer-email: luca.rebuffi@elettra.eu
 License: GPLv3
```

### Comparing `syned-1.0.8/setup.py` & `syned-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 try:
     from setuptools import find_packages, setup
 except AttributeError:
     from setuptools import find_packages, setup
 
 NAME = 'syned'
 
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 ISRELEASED = False
 
 DESCRIPTION = 'SYNED (SYNchrotron Elements Dictionary) kernel library'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.txt')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Manuel Sanchez del Rio, Luca Rebuffi'
 AUTHOR_EMAIL = 'srio@esrf.eu'
```

### Comparing `syned-1.0.8/syned/beamline/beamline.py` & `syned-1.0.9/syned/beamline/beamline.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,51 +3,52 @@
 
 BeamlineComponents can be attached at positions(BeamlinePosition), i.e. longitudinal, off-axis and inclined.
 We can iterate of the components, find their positions or look for a specific component.
 """
 
 from syned.syned_object import SynedObject
 from syned.storage_ring.light_source import LightSource
+from syned.storage_ring.empty_light_source import EmptyLightSource
 from syned.beamline.beamline_element import BeamlineElement
 
 from collections import OrderedDict
 
 class Beamline(SynedObject):
     def __init__(self, light_source=LightSource(), beamline_elements_list=[]):
         self._light_source = light_source
         self._beamline_elements_list = beamline_elements_list
 
         # support text containg name of variable, help text and unit. Will be stored in self._support_dictionary
         self._set_support_text([
                     ("light_source",       "Light Source",      ""),
-                    ("beamline_elements",  "Beamline Elements", ""),
+                    ("beamline_elements_list",  "Beamline Elements", ""),
             ] )
 
 
     # overwrites the SynedObject method for dealing with list
     def to_dictionary(self):
         dict_to_save = OrderedDict()
         dict_to_save.update({"CLASS_NAME":self.__class__.__name__})
 
         dict_to_save["light_source"] = self._light_source.to_dictionary()
-        dict_to_save["beamline_elements"] = [el.to_dictionary() for el in self._beamline_elements_list]
+        dict_to_save["beamline_elements_list"] = [el.to_dictionary() for el in self._beamline_elements_list]
 
         return dict_to_save
 
 
 
     def get_light_source(self):
         return self._light_source
 
     def get_beamline_elements(self):
         return self._beamline_elements_list
 
     def set_light_source(self, light_source=LightSource()):
-        if not isinstance(light_source,LightSource):
-            raise Exception("Input class must be of type: "+LightSource.__name__)
+        if not (isinstance(light_source,LightSource) or isinstance(light_source,EmptyLightSource)):
+            raise Exception("Input class must be of type: "+LightSource.__name__+" or "+EmptyLightSource.__name__)
         else:
             self._light_source = light_source
 
     def append_beamline_element(self, beamline_element=BeamlineElement()):
         if not isinstance(beamline_element,BeamlineElement):
             raise Exception("Input class must be of type: "+BeamlineElement.__name__)
         else:
```

### Comparing `syned-1.0.8/syned/beamline/beamline_element.py` & `syned-1.0.9/syned/beamline/beamline_element.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/beamline/element_coordinates.py` & `syned-1.0.9/syned/beamline/element_coordinates.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/beamline/optical_element.py` & `syned-1.0.9/syned/beamline/optical_element.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/beamline/optical_element_with_surface_shape.py` & `syned-1.0.9/syned/beamline/optical_element_with_surface_shape.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/beamline/optical_elements/absorbers/beam_stopper.py` & `syned-1.0.9/syned/beamline/optical_elements/absorbers/beam_stopper.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/beamline/optical_elements/absorbers/filter.py` & `syned-1.0.9/syned/beamline/optical_elements/absorbers/filter.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/beamline/optical_elements/crystals/crystal.py` & `syned-1.0.9/syned/beamline/optical_elements/crystals/crystal.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/beamline/optical_elements/gratings/grating.py` & `syned-1.0.9/syned/beamline/optical_elements/gratings/grating.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/beamline/optical_elements/ideal_elements/lens.py` & `syned-1.0.9/syned/beamline/optical_elements/ideal_elements/lens.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/beamline/optical_elements/mirrors/mirror.py` & `syned-1.0.9/syned/beamline/optical_elements/mirrors/mirror.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/beamline/shape.py` & `syned-1.0.9/syned/beamline/shape.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 import numpy
 from syned.syned_object import SynedObject
+from collections import OrderedDict
 
 class Convexity:
     NONE = -1
     UPWARD = 0
     DOWNWARD = 1
 
 class Direction:
@@ -233,18 +234,18 @@
         self._x_left   = x_left
         self._x_right  = x_right
         self._y_bottom = y_bottom
         self._y_top    = y_top
 
         # support text containg name of variable, help text and unit. Will be stored in self._support_dictionary
         self._set_support_text([
-                    ("x_left    "      , "x (width) minimum (signed)   ", "m" ),
-                    ("x_right   "      , "x (width) maximum (signed)   ", "m" ),
-                    ("y_bottom  "      , "y (length) minimum (signed)  ", "m" ),
-                    ("y_top     "      , "y (length) maximum (signed)  ", "m" ),
+                    ("x_left"          , "x (width) minimum (signed)   ", "m" ),
+                    ("x_right"         , "x (width) maximum (signed)   ", "m" ),
+                    ("y_bottom"        , "y (length) minimum (signed)  ", "m" ),
+                    ("y_top"           , "y (length) maximum (signed)  ", "m" ),
             ] )
 
     def get_boundaries(self):
         return self._x_left, self._x_right, self._y_bottom, self._y_top
 
     def set_boundaries(self,x_left=-0.010, x_right=0.010, y_bottom=-0.020, y_top=0.020):
         self._x_left = x_left
@@ -255,47 +256,47 @@
     def set_width_and_length(self,width=10e-3,length=30e-3):
         self._x_left = -0.5 * width
         self._x_right = 0.5 * width
         self._y_bottom = -0.5 * length
         self._y_top = 0.5 * length
 
 class Ellipse(BoundaryShape):
-    def __init__(self, min_ax_left, min_ax_right, maj_ax_bottom, maj_ax_top):
+    def __init__(self, a_axis_min=-10e-6, a_axis_max=10e-6, b_axis_min=-5e-6, b_axis_max=5e-6):
         super().__init__()
 
-        self._min_ax_left   = min_ax_left
-        self._min_ax_right  = min_ax_right
-        self._maj_ax_bottom = maj_ax_bottom
-        self._maj_ax_top    = maj_ax_top
+        self._min_ax_left   = a_axis_min
+        self._min_ax_right  = a_axis_max
+        self._maj_ax_bottom = b_axis_min
+        self._maj_ax_top    = b_axis_max
         # support text containg name of variable, help text and unit. Will be stored in self._support_dictionary
         self._set_support_text([
-                    ("min_ax_left   "      , "x (width) semiaxis starts (signed)  ", "m" ),
-                    ("min_ax_right  "      , "x (width) semiaxis ends (signed)    ", "m" ),
-                    ("maj_ax_bottom "      , "y (length) semiaxis starts (signed) ", "m" ),
-                    ("maj_ax_top    "      , "y (length) semiaxis ends (signed)   ", "m" ),
+                    ("min_ax_left"         , "x (width) axis starts (signed)  ", "m" ),
+                    ("min_ax_right"        , "x (width) axis ends (signed)    ", "m" ),
+                    ("maj_ax_bottom"       , "y (length) axis starts (signed) ", "m" ),
+                    ("maj_ax_top"          , "y (length) axis ends (signed)   ", "m" ),
             ] )
 
     def get_boundaries(self):
         return self._min_ax_left, self._min_ax_right, self._maj_ax_bottom, self._maj_ax_top
 
     def get_axis(self):
         return numpy.abs(self._min_ax_right-self._min_ax_left), numpy.abs(self._maj_ax_top-self._maj_ax_bottom)
 
 class Circle(BoundaryShape):
-    def __init__(self, radius, x_center=0.0, y_center=0.0):
+    def __init__(self,radius=50e-6,x_center=0.0,y_center=0.0):
         super().__init__()
 
         self._radius = radius
         self._x_center = x_center
         self._y_center = y_center
         # support text containg name of variable, help text and unit. Will be stored in self._support_dictionary
         self._set_support_text([
-                    ("radius        "      , "radius  ", "m" ),
-                    ("x_center      "      , "x center (signed)    ", "m" ),
-                    ("y_center      "      , "y center (signed)    ", "m" ),
+                    ("radius"              , "radius  ", "m" ),
+                    ("x_center"            , "x center (signed)    ", "m" ),
+                    ("y_center"            , "y center (signed)    ", "m" ),
             ] )
 
     def get_boundaries(self):
         return self._radius, self._x_center, self._y_center
 
     def set_boundaries(self, radius=1.0, x_center=0.0, y_center=0.0):
         self._radius = radius
@@ -304,23 +305,141 @@
 
     def get_radius(self):
         return self._radius
 
     def get_center(self):
         return [self._x_center,self._y_center]
 
+
+class MultiplePatch(BoundaryShape):
+    def __init__(self, patch_list=[]):
+        super().__init__()
+
+        self._patch_list = patch_list
+        self._set_support_text([
+                    ("multiple_patch_list",  "Multiple Patch", ""),
+            ])
+
+
+    # overwrites the SynedObject method for dealing with list
+    def to_dictionary(self):
+        dict_to_save = OrderedDict()
+        dict_to_save.update({"CLASS_NAME":self.__class__.__name__})
+
+        dict_to_save["multiple_patch_list"] = [el.to_dictionary() for el in self._patch_list]
+
+        return dict_to_save
+
+
+    def reset(self):
+        self._patch_list = []
+
+    def get_number_of_patches(self):
+        return len(self._patch_list)
+
+    def get_boundaries(self):
+        boundaries_list = []
+        for i in range(self.get_number_of_patches()):
+            boundaries_list.extend(list(self._patch_list[i].get_boundaries()))
+        return tuple(boundaries_list)
+
+    def append_patch(self,patch=BoundaryShape()):
+        self._patch_list.append(patch)
+
+    def append_rectangle(self,x_left=-0.010,x_right=0.010,y_bottom=-0.020,y_top=0.020):
+        self.append_patch(Rectangle(x_left=x_left, x_right=x_right, y_bottom=y_bottom, y_top=y_top))
+
+    def append_circle(self,radius, x_center=0.0, y_center=0.0):
+        self.append_patch(Circle(radius, x_center=x_center, y_center=y_center))
+
+    def append_ellipse(self,min_ax_left, min_ax_right, maj_ax_bottom, maj_ax_top):
+        self.append_patch(Ellipse(min_ax_left, min_ax_right, maj_ax_bottom, maj_ax_top))
+
+    def get_patches(self):
+        return self._patch_list
+
+    def get_patch(self,index):
+        return self.get_patches()[index]
+
+    def get_name_of_patch(self,index):
+        return self._patch_list[index].__class__.__name__
+
+class DoubleRectangle(MultiplePatch):
+    def __init__(self, x_left1=-0.010, x_right1=0.0, y_bottom1=-0.020, y_top1=0.0,
+                        x_left2=-0.010, x_right2=0.010, y_bottom2=-0.001, y_top2=0.020):
+        super().__init__()
+        self.reset()
+        self.append_patch(Rectangle(x_left=x_left1, x_right=x_right1, y_bottom=y_bottom1, y_top=y_top1))
+        self.append_patch(Rectangle(x_left=x_left2, x_right=x_right2, y_bottom=y_bottom2, y_top=y_top2))
+
+    def set_boundaries(self,x_left1=-0.010, x_right1=0.0, y_bottom1=-0.020, y_top1=0.0,
+                        x_left2=-0.010, x_right2=0.010, y_bottom2=-0.001, y_top2=0.020):
+        self._patch_list[0].set_boundaries(x_left1, x_right1, y_bottom1, y_top1)
+        self._patch_list[1].set_boundaries(x_left2, x_right2, y_bottom2, y_top2)
+
+class DoubleEllipse(MultiplePatch):
+    def __init__(self, a_axis_min1=-0.010, a_axis_max1=0.0,   b_axis_min1=-0.020, b_axis_max1=0.0,
+                       a_axis_min2=-0.010, a_axis_max2=0.010, b_axis_min2=-0.001, b_axis_max2=0.020):
+        super().__init__()
+        self.reset()
+        self.append_patch(Ellipse(a_axis_min1, a_axis_max1, b_axis_min1, b_axis_max1))
+        self.append_patch(Ellipse(a_axis_min2, a_axis_max2, b_axis_min2, b_axis_max2))
+
+    def set_boundaries(self,a_axis_min1=-0.010, a_axis_max1=0.0,   b_axis_min1=-0.020, b_axis_max1=0.0,
+                            a_axis_min2=-0.010, a_axis_max2=0.010, b_axis_min2=-0.001, b_axis_max2=0.020):
+        self._patch_list[0].set_boundaries(a_axis_min1,a_axis_max1,b_axis_min1,b_axis_max1)
+        self._patch_list[1].set_boundaries(a_axis_min2,a_axis_max2,b_axis_min2,b_axis_max2)
+
+class DoubleCircle(MultiplePatch):
+    def __init__(self, radius1=50e-6,x_center1=0.0,y_center1=0.0,
+                       radius2=50e-6,x_center2=100e-6,y_center2=100e-6):
+        super().__init__()
+        self.reset()
+        self.append_patch(Circle(radius1,x_center1,y_center1))
+        self.append_patch(Circle(radius2,x_center2,y_center2))
+
+    def set_boundaries(self,radius1=50e-6,x_center1=0.0,y_center1=0.0,
+                            radius2=50e-6,x_center2=100e-6,y_center2=100e-6):
+        self._patch_list[0].set_boundaries(radius1,x_center1,y_center1)
+        self._patch_list[1].set_boundaries(radius2,x_center2,y_center2)
+
+
+
 if __name__=="__main__":
 
     # ell = Ellipsoid()
     # ell.initialize_from_p_q(20, 10, 0.2618)
     #
     # print (ell._min_axis/2, ell._maj_axis/2)
     #
     # ell = Ellipsoid(min_axis=ell._min_axis, maj_axis=ell._maj_axis)
     #
     # print(ell.get_p_q(0.2618))
 
 
-    circle = Circle(3.0)
+    # circle = Circle(3.0)
+    #
+    # print(circle.get_radius(),circle.get_center())
+    # print(circle.get_boundaries())
+
+
+
 
-    print(circle.get_radius(),circle.get_center())
-    print(circle.get_boundaries())
+    # patches = MultiplePatch()
+    #
+    # patches.append_rectangle(-0.02,-0.01,-0.001,0.001)
+    # patches.append_rectangle(0.01,0.02,-0.001,0.001)
+    #
+    # print(patches.get_number_of_patches(),patches.get_boundaries())
+    #
+    # for patch in patches.get_patches():
+    #     print(patch.info())
+    #
+    # print("Patch 0 is: ",patches.get_name_of_patch(0))
+    # print("Patch 1 is: ",patches.get_name_of_patch(1))
+    # print(patches.get_boundaries())
+
+    double_rectangle = DoubleRectangle()
+    double_rectangle.set_boundaries(-0.02,-0.01,-0.001,0.001,0.01,0.02,-0.001,0.001)
+    print("Rectangle 0 is: ",double_rectangle.get_name_of_patch(0))
+    print("Rectangle 1 is: ",double_rectangle.get_name_of_patch(1))
+    print(double_rectangle.get_boundaries())
```

### Comparing `syned-1.0.8/syned/examples/example_beamline.py` & `syned-1.0.9/syned/examples/example_beamline.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,8 +160,11 @@
 
     mirror_coordinates = ElementCoordinates(p=2.5,
                                             q=10.0,
                                             angle_radial=89.828,
                                             angle_azimuthal=180.0)
 
     beamline.append_beamline_element(beamline_element=BeamlineElement(optical_element=mirror,
-                                                                      coordinates=mirror_coordinates))
+                                                                      coordinates=mirror_coordinates))
+
+    print(beamline.to_dictionary())
+    print(beamline.to_full_dictionary())
```

### Comparing `syned-1.0.8/syned/examples/example_json_input_output.py` & `syned-1.0.9/syned/examples/example_json_input_output.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/storage_ring/electron_beam.py` & `syned-1.0.9/syned/storage_ring/electron_beam.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/storage_ring/light_source.py` & `syned-1.0.9/syned/storage_ring/light_source.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/storage_ring/magnetic_structures/bending_magnet.py` & `syned-1.0.9/syned/storage_ring/magnetic_structures/bending_magnet.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/storage_ring/magnetic_structures/insertion_device.py` & `syned-1.0.9/syned/storage_ring/magnetic_structures/insertion_device.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/storage_ring/magnetic_structures/undulator.py` & `syned-1.0.9/syned/storage_ring/magnetic_structures/undulator.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,25 +13,25 @@
     def __init__(self,
                  K_vertical = 0.0,
                  K_horizontal = 0.0,
                  period_length = 0.0,
                  number_of_periods = 1):
         InsertionDevice.__init__(self, K_vertical, K_horizontal, period_length, number_of_periods)
 
-    def resonance_wavelength(self, gamma, theta_x=0.0, theta_z=0.0):
+    def resonance_wavelength(self, gamma, theta_x=0.0, theta_z=0.0, harmonic=1):
         wavelength = (self.period_length() / (2.0*gamma **2)) * \
                      (1 + self.K_vertical()**2 / 2.0 + self.K_horizontal()**2 / 2.0 + \
                       gamma**2 * (theta_x**2 + theta_z ** 2))
 
-        return wavelength
+        return wavelength/harmonic
 
-    def resonance_frequency(self, gamma, theta_x=0.0, theta_z=0.0):
+    def resonance_frequency(self, gamma, theta_x=0.0, theta_z=0.0, harmonic=1):
         frequency = codata.c / self.resonance_wavelength(gamma, theta_x, theta_z)
 
-        return frequency
+        return frequency*harmonic
 
     def resonance_energy(self, gamma, theta_x=0.0, theta_z=0.0, harmonic=1):
         energy_in_ev = codata.h * self.resonance_frequency(gamma, theta_x, theta_z) / codata.e
 
         return energy_in_ev*harmonic
 
     def gaussian_central_cone_aperture(self, gamma, n=1):
```

### Comparing `syned-1.0.8/syned/storage_ring/magnetic_structures/wiggler.py` & `syned-1.0.9/syned/storage_ring/magnetic_structures/wiggler.py`

 * *Files identical despite different names*

### Comparing `syned-1.0.8/syned/syned_object.py` & `syned-1.0.9/syned/syned_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,14 +91,15 @@
                         text += element.info()
                 else:
                     text += prefix + '    %s: %s %s # %s\n' %(key,  repr(fd[key][0]), fd[key][1][1], fd[key][1][0])
             else:
                 pass
         return text
 
+    # TODO: not working correctly for beamline
     def info(self):
         return self.info_recurrent( self.to_full_dictionary() )
 
 
     def set_value_from_key_name(self,key,value):
         if key in self.keys():
             try:
```

### Comparing `syned-1.0.8/syned/util/json_tools.py` & `syned-1.0.9/syned/util/json_tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,56 @@
 
 from syned.storage_ring.electron_beam import ElectronBeam
 from syned.storage_ring.magnetic_structures.undulator import Undulator
+from syned.storage_ring.magnetic_structure import MagneticStructure
 from syned.beamline.optical_elements.ideal_elements.screen import Screen
 from syned.beamline.optical_elements.ideal_elements.lens import IdealLens
 from syned.beamline.optical_elements.absorbers.filter import Filter
 from syned.beamline.optical_elements.absorbers.slit import Slit
 from syned.beamline.optical_elements.absorbers.beam_stopper import BeamStopper
 from syned.beamline.optical_elements.mirrors.mirror import Mirror
 from syned.beamline.optical_elements.crystals.crystal import Crystal
 from syned.beamline.optical_elements.gratings.grating import Grating
 
-from syned.beamline.shape import Rectangle
-from syned.beamline.shape import Conic
-from syned.beamline.shape import Plane
-from syned.beamline.shape import SurfaceShape
 from syned.beamline.shape import BoundaryShape
+from syned.beamline.shape import Rectangle, Circle, Ellipse
+from syned.beamline.shape import MultiplePatch
+
+from syned.beamline.shape import SurfaceShape
+from syned.beamline.shape import Conic, Sphere, SphericalCylinder, Toroidal
+from syned.beamline.shape import Plane
+
 from syned.storage_ring.light_source import LightSource
+from syned.storage_ring.empty_light_source import EmptyLightSource
 
 from syned.beamline.beamline import Beamline
 from syned.beamline.beamline_element import BeamlineElement
 from syned.beamline.element_coordinates import ElementCoordinates
 
 from collections import OrderedDict
 
-
 import json
 from urllib.request import urlopen
 
+#
+# this allows to load wofry-elements (e.g. WOSlit) in addition to syned elements (Slit)
+#
+try:
+    from wofry.beamline.optical_elements.ideal_elements.screen import WOScreen
+    from wofry.beamline.optical_elements.ideal_elements.lens import WOIdealLens
+    # from wofry.beamline.optical_elements.absorbers.filter import WOFilter
+    from wofry.beamline.optical_elements.absorbers.slit import WOSlit
+    from wofry.beamline.optical_elements.absorbers.beam_stopper import WOBeamStopper
+    # from wofry.beamline.optical_elements.mirrors.mirror import WOMirror
+    # from wofry.beamline.optical_elements.crystals.crystal import WOCrystal
+    # from wofry.beamline.optical_elements.gratings.grating import WOGrating
+except:
+    pass
+
+
 
 
 def load_from_json_file(file_name):
     f = open(file_name)
     text = f.read()
     f.close()
     return load_from_json_text(text)
@@ -119,15 +139,15 @@
 #         print("\n------------------------------------------------------------------------------\n")
 #
 #     return tmp1
 #
 #
 
 if __name__ == "__main__":
-    file_in = "/scisoft/xop2.4/extensions/shadowvui/shadow3-scripts/ESRF-LIGHTSOURCES/ESRF_ID1_EBS_ppu27_9.json"
-    syned_obj = load_from_json_file(file_in)
-    print(syned_obj.info())
+    # file_in = "/scisoft/xop2.4/extensions/shadowvui/shadow3-scripts/ESRF-LIGHTSOURCES/ESRF_ID1_EBS_ppu27_9.json"
+    # syned_obj = load_from_json_file(file_in)
+    # print(syned_obj.info())
 
-    file_url = "https://raw.githubusercontent.com/srio/shadow3-scripts/master/ESRF-LIGHTSOURCES/ESRF_ID1_EBS_ppu27_9.json"
+    file_url = "http://ftp.esrf.eu/pub/scisoft/syned/lightsources/ESRF_ID01_EBS_ppu27_11.json"
     syned_obj = load_from_json_url(file_url)
     print(syned_obj.info())
```

### Comparing `syned-1.0.8/syned.egg-info/PKG-INFO` & `syned-1.0.9/syned.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: syned
-Version: 1.0.8
+Version: 1.0.9
 Summary: SYNED (SYNchrotron Elements Dictionary) kernel library
 Home-page: https://github.com/lucarebuffi/syned
 Author: Manuel Sanchez del Rio, Luca Rebuffi
 Author-email: srio@esrf.eu
 Maintainer: Luca Rebuffi
 Maintainer-email: luca.rebuffi@elettra.eu
 License: GPLv3
```

### Comparing `syned-1.0.8/syned.egg-info/SOURCES.txt` & `syned-1.0.9/syned.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -31,17 +31,19 @@
 syned/beamline/optical_elements/ideal_elements/ideal_element.py
 syned/beamline/optical_elements/ideal_elements/lens.py
 syned/beamline/optical_elements/ideal_elements/screen.py
 syned/beamline/optical_elements/mirrors/__init__.py
 syned/beamline/optical_elements/mirrors/mirror.py
 syned/examples/__init__.py
 syned/examples/example_beamline.py
+syned/examples/example_json_double_slit.py
 syned/examples/example_json_input_output.py
 syned/storage_ring/__init__.py
 syned/storage_ring/electron_beam.py
+syned/storage_ring/empty_light_source.py
 syned/storage_ring/light_source.py
 syned/storage_ring/magnetic_structure.py
 syned/storage_ring/magnetic_structures/__init__.py
 syned/storage_ring/magnetic_structures/bending_magnet.py
 syned/storage_ring/magnetic_structures/insertion_device.py
 syned/storage_ring/magnetic_structures/undulator.py
 syned/storage_ring/magnetic_structures/wiggler.py
```

