# Comparing `tmp/ephysiopy-1.9.11.tar.gz` & `tmp/ephysiopy-1.9.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysiopy-1.9.11.tar", last modified: Thu Apr 20 14:20:30 2023, max compression
+gzip compressed data, was "ephysiopy-1.9.12.tar", last modified: Fri Apr 21 08:54:08 2023, max compression
```

## Comparing `ephysiopy-1.9.11.tar` & `ephysiopy-1.9.12.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:30.380493 ephysiopy-1.9.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-20 14:20:30.380493 ephysiopy-1.9.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:30.372493 ephysiopy-1.9.11/ephysiopy/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:30.372493 ephysiopy-1.9.11/ephysiopy/axona/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/axona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/axona/axonaIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/axona/file_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/axona/tetrode_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/axona/tintcolours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:30.376493 ephysiopy-1.9.11/ephysiopy/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31243 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/common/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/common/ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/common/fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/common/gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/common/mle_von_mises_vals.py
--rw-r--r--   0 runner    (1001) docker     (123)    49463 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/common/phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/common/rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/common/spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/common/statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:30.376493 ephysiopy-1.9.11/ephysiopy/format_converters/
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/format_converters/OE_Axona.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/format_converters/OE_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/format_converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:30.376493 ephysiopy-1.9.11/ephysiopy/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23104 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/io/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:30.376493 ephysiopy-1.9.11/ephysiopy/openephys2py/
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/openephys2py/KiloSort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/openephys2py/OESettings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/openephys2py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:30.380493 ephysiopy-1.9.11/ephysiopy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 14:20:20.000000 ephysiopy-1.9.11/ephysiopy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/tests/test_axona_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/tests/test_axona_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/tests/test_dacq2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/tests/test_ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/tests/test_fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/tests/test_gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/tests/test_openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/tests/test_phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/tests/test_rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/tests/test_spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/tests/test_statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:30.380493 ephysiopy-1.9.11/ephysiopy/visualise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/visualise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32228 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/ephysiopy/visualise/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:20:30.372493 ephysiopy-1.9.11/ephysiopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-20 14:20:30.000000 ephysiopy-1.9.11/ephysiopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-20 14:20:30.000000 ephysiopy-1.9.11/ephysiopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:20:30.000000 ephysiopy-1.9.11/ephysiopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 14:20:30.000000 ephysiopy-1.9.11/ephysiopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 14:20:30.000000 ephysiopy-1.9.11/ephysiopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 14:20:30.380493 ephysiopy-1.9.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-20 14:20:21.000000 ephysiopy-1.9.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:08.923818 ephysiopy-1.9.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-21 08:54:08.923818 ephysiopy-1.9.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:08.919818 ephysiopy-1.9.12/ephysiopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:08.919818 ephysiopy-1.9.12/ephysiopy/axona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/axona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/axona/axonaIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/axona/file_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/axona/tetrode_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/axona/tintcolours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:08.919818 ephysiopy-1.9.12/ephysiopy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31243 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/common/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/common/ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/common/fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/common/gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/common/mle_von_mises_vals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49463 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/common/phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/common/rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/common/spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/common/statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:08.919818 ephysiopy-1.9.12/ephysiopy/format_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/format_converters/OE_Axona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/format_converters/OE_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/format_converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:08.919818 ephysiopy-1.9.12/ephysiopy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23342 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/io/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:08.919818 ephysiopy-1.9.12/ephysiopy/openephys2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/openephys2py/KiloSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/openephys2py/OESettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/openephys2py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:08.923818 ephysiopy-1.9.12/ephysiopy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/test_axona_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/test_axona_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/test_dacq2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/test_ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/test_fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/test_gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/test_openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/test_phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/test_rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/test_spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/test_statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:08.923818 ephysiopy-1.9.12/ephysiopy/visualise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/visualise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32289 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/ephysiopy/visualise/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:54:08.919818 ephysiopy-1.9.12/ephysiopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-21 08:54:08.000000 ephysiopy-1.9.12/ephysiopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-21 08:54:08.000000 ephysiopy-1.9.12/ephysiopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:54:08.000000 ephysiopy-1.9.12/ephysiopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 08:54:08.000000 ephysiopy-1.9.12/ephysiopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 08:54:08.000000 ephysiopy-1.9.12/ephysiopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 08:54:08.923818 ephysiopy-1.9.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-21 08:54:02.000000 ephysiopy-1.9.12/setup.py
```

### Comparing `ephysiopy-1.9.11/LICENSE` & `ephysiopy-1.9.12/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/PKG-INFO` & `ephysiopy-1.9.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.11
+Version: 1.9.12
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.11/README.md` & `ephysiopy-1.9.12/README.md`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/axona/axonaIO.py` & `ephysiopy-1.9.12/ephysiopy/axona/axonaIO.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/axona/file_headers.py` & `ephysiopy-1.9.12/ephysiopy/axona/file_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/axona/tetrode_dict.py` & `ephysiopy-1.9.12/ephysiopy/axona/tetrode_dict.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/axona/tintcolours.py` & `ephysiopy-1.9.12/ephysiopy/axona/tintcolours.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/common/binning.py` & `ephysiopy-1.9.12/ephysiopy/common/binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/common/ephys_generic.py` & `ephysiopy-1.9.12/ephysiopy/common/ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/common/fieldcalcs.py` & `ephysiopy-1.9.12/ephysiopy/common/fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/common/gridcell.py` & `ephysiopy-1.9.12/ephysiopy/common/gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/common/mle_von_mises_vals.py` & `ephysiopy-1.9.12/ephysiopy/common/mle_von_mises_vals.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/common/phasecoding.py` & `ephysiopy-1.9.12/ephysiopy/common/phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/common/rhythmicity.py` & `ephysiopy-1.9.12/ephysiopy/common/rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/common/spikecalcs.py` & `ephysiopy-1.9.12/ephysiopy/common/spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/common/statscalcs.py` & `ephysiopy-1.9.12/ephysiopy/common/statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/common/utils.py` & `ephysiopy-1.9.12/ephysiopy/common/utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/format_converters/OE_Axona.py` & `ephysiopy-1.9.12/ephysiopy/format_converters/OE_Axona.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/format_converters/OE_numpy.py` & `ephysiopy-1.9.12/ephysiopy/format_converters/OE_numpy.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/io/recording.py` & `ephysiopy-1.9.12/ephysiopy/io/recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,23 +405,24 @@
     def load_settings(self, *args, **kwargs):
         if self._settings is None:
             # pname_root gets walked through and over-written with
             # correct location of settings.xml
             self.settings = Settings(self.pname)
 
     def load_cluster_data(self, *args, **kwargs):
-        if self.pname is not None:
-            if os.path.exists(self.pname):
-                clusterData = KiloSortSession(self.pname)
-            if clusterData is not None:
-                if clusterData.load():
-                    try:
-                        clusterData.removeKSNoiseClusters()
-                    except Exception:
-                        pass
+        if self.path2KiloSortData is not None:
+            clusterData = KiloSortSession(self.pname)
+        if clusterData is not None:
+            if clusterData.load():
+                print("Loaded KiloSort data")
+                try:
+                    clusterData.removeKSNoiseClusters()
+                    print("Removed noise clusters")
+                except Exception:
+                    pass
         self.clusterData = clusterData
 
     def load_pos_data(self, ppm: int = 300, jumpmax: int = 100,
                       *args, **kwargs) -> None:
         # Only sub-class that doesn't use this is OpenEphysNWB
         # which needs updating
         # TODO: Update / overhaul OpenEphysNWB
@@ -594,14 +595,17 @@
                     if "full_words.npy" in ff:
                         if PurePath(d).match(str(Events_match)):
                             self.path2EventsData = os.path.join(d)
                             print(f"Event data at: {self.path2EventsData}")
                     if ".nwb" in ff:
                         self.path2NWBData = os.path.join(d, ff)
                         print(f"nwb data at: {self.path2NWBData}")
+                    if "spike_templates.npy" in ff:
+                        self.path2KiloSortData = os.path.join(d)
+                        print(f"Found KiloSort data at {self.path2KiloSortData}")
 
 
 class OpenEphysNWB(OpenEphysBase):
     def __init__(self, pname: Path, **kwargs) -> None:
         super().__init__(pname, **kwargs)
 
     def load_neural_data(self, pname: Path, *args, **kwargs) -> None:
```

### Comparing `ephysiopy-1.9.11/ephysiopy/openephys2py/KiloSort.py` & `ephysiopy-1.9.12/ephysiopy/openephys2py/KiloSort.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/openephys2py/OESettings.py` & `ephysiopy-1.9.12/ephysiopy/openephys2py/OESettings.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/tests/conftest.py` & `ephysiopy-1.9.12/ephysiopy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/tests/test_axona_headers.py` & `ephysiopy-1.9.12/ephysiopy/tests/test_axona_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/tests/test_axona_io.py` & `ephysiopy-1.9.12/ephysiopy/tests/test_axona_io.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/tests/test_binning.py` & `ephysiopy-1.9.12/ephysiopy/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/tests/test_dacq2py.py` & `ephysiopy-1.9.12/ephysiopy/tests/test_dacq2py.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/tests/test_ephys_generic.py` & `ephysiopy-1.9.12/ephysiopy/tests/test_ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/tests/test_fieldcalcs.py` & `ephysiopy-1.9.12/ephysiopy/tests/test_fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/tests/test_gridcell.py` & `ephysiopy-1.9.12/ephysiopy/tests/test_gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/tests/test_phasecoding.py` & `ephysiopy-1.9.12/ephysiopy/tests/test_phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/tests/test_rhythmicity.py` & `ephysiopy-1.9.12/ephysiopy/tests/test_rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/tests/test_spikecalcs.py` & `ephysiopy-1.9.12/ephysiopy/tests/test_spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/tests/test_statscalcs.py` & `ephysiopy-1.9.12/ephysiopy/tests/test_statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/tests/test_utils.py` & `ephysiopy-1.9.12/ephysiopy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/ephysiopy/visualise/plotting.py` & `ephysiopy-1.9.12/ephysiopy/visualise/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         plt.xticks([spd_bins[0], spd_bins[-1]], ['0', '{:.2g}'.format(
             spd_bins[-1])], fontweight='normal', size=6)
         plt.yticks([0, np.nanmax(
             mn_rate)*self.PosCalcs.sample_rate], ['0', '{:.2f}'.format(
                 np.nanmax(mn_rate))], fontweight='normal', size=6)
         return ax
 
-    @stripAxes
+    # @stripAxes
     def makeSpeedVsHeadDirectionPlot(self, spk_times: np.array,
                                      ax: matplotlib.axes = None,
                                      **kwargs) -> matplotlib.axes:
         self.initialise()
         spk_times_in_pos_samples = self.getSpikePosIndices(spk_times)
         idx = np.array(spk_times_in_pos_samples, dtype=int)
         if np.ma.is_masked(self.PosCalcs.speed):
@@ -259,14 +259,15 @@
             fig = plt.figure()
             ax = fig.add_subplot(111)
         ax.pcolormesh(x, y, im.T, cmap=jet_cmap,
                       edgecolors='face',
                       vmax=vmax, shading='auto')
         plt.xticks([90, 180, 270], fontweight='normal', size=6)
         plt.yticks([10, 20], fontweight='normal', size=6)
+        plt.xlabel("Heading", fontweight='normal', size=6)
         return ax
 
     def makePowerSpectrum(
             self, freqs: np.array, power: np.array, sm_power: np.array,
             band_max_power: float, freq_at_band_max_power: float,
             max_freq: int = 50, theta_range: tuple = [6, 12],
             ax: matplotlib.axes = None, **kwargs) -> matplotlib.axes:
```

### Comparing `ephysiopy-1.9.11/ephysiopy.egg-info/PKG-INFO` & `ephysiopy-1.9.12/ephysiopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.11
+Version: 1.9.12
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.11/ephysiopy.egg-info/SOURCES.txt` & `ephysiopy-1.9.12/ephysiopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.11/setup.py` & `ephysiopy-1.9.12/setup.py`

 * *Files identical despite different names*

