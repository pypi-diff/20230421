# Comparing `tmp/circuitpython-cirque-pinnacle-0.0.4.tar.gz` & `tmp/circuitpython-cirque-pinnacle-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/circuitpython-cirque-pinnacle-0.0.4.tar", last modified: Wed Nov 11 06:23:04 2020, max compression
+gzip compressed data, was "circuitpython-cirque-pinnacle-1.0.0.tar", last modified: Fri Apr 21 00:10:38 2023, max compression
```

## Comparing `circuitpython-cirque-pinnacle-0.0.4.tar` & `circuitpython-cirque-pinnacle-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-11 06:23:04.516851 circuitpython-cirque-pinnacle-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-11 06:23:04.512851 circuitpython-cirque-pinnacle-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-11 06:23:04.512851 circuitpython-cirque-pinnacle-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1754 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2630 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1889 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)    16543 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)       62 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     5958 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1072 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)    10552 2020-11-11 06:23:04.516851 circuitpython-cirque-pinnacle-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8124 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-11 06:23:04.512851 circuitpython-cirque-pinnacle-0.0.4/circuitpython_cirque_pinnacle/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/circuitpython_cirque_pinnacle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    17672 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/circuitpython_cirque_pinnacle/glidepoint.py
--rw-r--r--   0 runner    (1001) docker     (116)     7810 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/circuitpython_cirque_pinnacle/glidepoint_lite.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-11 06:23:04.512851 circuitpython-cirque-pinnacle-0.0.4/circuitpython_cirque_pinnacle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    10552 2020-11-11 06:23:04.000000 circuitpython-cirque-pinnacle-0.0.4/circuitpython_cirque_pinnacle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      837 2020-11-11 06:23:04.000000 circuitpython-cirque-pinnacle-0.0.4/circuitpython_cirque_pinnacle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-11 06:23:04.000000 circuitpython-cirque-pinnacle-0.0.4/circuitpython_cirque_pinnacle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       49 2020-11-11 06:23:04.000000 circuitpython-cirque-pinnacle-0.0.4/circuitpython_cirque_pinnacle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       30 2020-11-11 06:23:04.000000 circuitpython-cirque-pinnacle-0.0.4/circuitpython_cirque_pinnacle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-11 06:23:04.512851 circuitpython-cirque-pinnacle-0.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-11 06:23:04.512851 circuitpython-cirque-pinnacle-0.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)   296110 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/docs/_static/Cirque_GlidePoint-Circle-Trackpad.png
--rw-r--r--   0 runner    (1001) docker     (116)    11294 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/docs/_static/darkness.css
--rw-r--r--   0 runner    (1001) docker     (116)    11062 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)    29605 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)     5836 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      744 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1104 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-11 06:23:04.516851 circuitpython-cirque-pinnacle-0.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     2620 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/examples/cirque_pinnacle_anymeas_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2114 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/examples/cirque_pinnacle_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (116)     1810 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/examples/cirque_pinnacle_usb_mouse.py
--rw-r--r--   0 runner    (1001) docker     (116)       51 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-11-11 06:23:04.516851 circuitpython-cirque-pinnacle-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2237 2020-11-11 06:22:52.000000 circuitpython-cirque-pinnacle-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:10:38.504312 circuitpython-cirque-pinnacle-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:10:38.500312 circuitpython-cirque-pinnacle-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:10:38.500312 circuitpython-cirque-pinnacle-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-21 00:10:38.504312 circuitpython-cirque-pinnacle-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:10:38.500312 circuitpython-cirque-pinnacle-1.0.0/circuitpython_cirque_pinnacle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-21 00:10:38.000000 circuitpython-cirque-pinnacle-1.0.0/circuitpython_cirque_pinnacle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-21 00:10:38.000000 circuitpython-cirque-pinnacle-1.0.0/circuitpython_cirque_pinnacle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:10:38.000000 circuitpython-cirque-pinnacle-1.0.0/circuitpython_cirque_pinnacle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 00:10:38.000000 circuitpython-cirque-pinnacle-1.0.0/circuitpython_cirque_pinnacle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-21 00:10:38.000000 circuitpython-cirque-pinnacle-1.0.0/circuitpython_cirque_pinnacle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    44966 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/circuitpython_cirque_pinnacle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:10:38.500312 circuitpython-cirque-pinnacle-1.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:10:38.504312 circuitpython-cirque-pinnacle-1.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   296110 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/docs/_static/Cirque_GlidePoint-Circle-Trackpad.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/docs/anymeas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/docs/rel_abs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:10:38.504312 circuitpython-cirque-pinnacle-1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/examples/cirque_pinnacle_absolute_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/examples/cirque_pinnacle_anymeas_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/examples/cirque_pinnacle_relative_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/examples/cirque_pinnacle_usb_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22604 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 00:10:38.504312 circuitpython-cirque-pinnacle-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 00:10:14.000000 circuitpython-cirque-pinnacle-1.0.0/setup.py
```

### Comparing `circuitpython-cirque-pinnacle-0.0.4/.gitignore` & `circuitpython-cirque-pinnacle-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-cirque-pinnacle-0.0.4/CODE_OF_CONDUCT.md` & `circuitpython-cirque-pinnacle-1.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-cirque-pinnacle-0.0.4/LICENSE` & `circuitpython-cirque-pinnacle-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-cirque-pinnacle-0.0.4/PKG-INFO` & `circuitpython-cirque-pinnacle-1.0.0/docs/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,194 +1,203 @@
-Metadata-Version: 2.1
-Name: circuitpython-cirque-pinnacle
-Version: 0.0.4
-Summary: A CircuitPython driver for Cirque Pinnacle (1CA027) touch controller used in Cirque Trackpads implementing the Adafruit_BusDevice library.
-Home-page: https://github.com/2bndy5/CircuitPython_Cirque_Pinnacle
-Author: Brendan Doherty
-Author-email: 2bndy5@gmail.com
-License: MIT
-Download-URL: https://github.com/2bndy5/CircuitPython_Cirque_Pinnacle/releases
-Project-URL: Documentation, https://circuitpython-cirque-pinnacle.readthedocs.io
-Description: 
-        .. image:: https://readthedocs.org/projects/circuitpython-cirque-pinnacle/badge/?version=latest
-            :target: https://circuitpython-cirque-pinnacle.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://github.com/2bndy5/CircuitPython_Cirque_Pinnacle/workflows/Build%20CI/badge.svg
-            :target: https://github.com/2bndy5/CircuitPython_Cirque_Pinnacle/actions/
-            :alt: Build Status
-        
-        .. image:: https://img.shields.io/pypi/v/circuitpython-cirque-pinnacle.svg
-            :alt: latest version on PyPI
-            :target: https://pypi.python.org/pypi/circuitpython-cirque-pinnacle
-        
-        .. image:: https://pepy.tech/badge/circuitpython-cirque-pinnacle
-            :alt: Total PyPI downloads
-            :target: https://pepy.tech/project/circuitpython-cirque-pinnacle
-        
-        
-        Introduction
-        ============
-        
-        A CircuitPython driver library that implements the Adafruit_BusDevice library
-        for interfacing with the Cirque Pinnacle (1CA027) touch controller used in Cirque Circle Trackpads.
-        
-        Supported Features
-        ------------------
-        
-        * Use SPI or I2C bus protocols to interface with the Pinnacle touch controller ASIC (Application
-          Specific Integrated Circuit).
-        * Relative mode data reporting (AKA Mouse mode) with optional tap detection.
-        * Absolute mode data reporting (x, y, & z axis positions).
-        * AnyMeas mode data reporting. This mode exposes the ADC (Analog to Digital Converter) values and is
-          not well documented in the numerous datasheets provided by the Cirque corporation about the
-          Pinnacle (1CA027), thus this is a rather experimental mode.
-        * Hardware input buttons' states included in data reports. There are 3 button input lines on
-          the Cirque circle trackpads -- see `Pinout`_ section.
-        * Configure measurements for finger or stylus (or automatically detirmine either) touch
-          events. The Cirque circle trackpads are natively capable of measuring only 1 touch
-          point per event.
-        * Download/upload the underlying compensation matrix for ADC measurements.
-        * Adjust the ADC matrix gain (sensitivity).
-        
-        .. tip:: The SPI protocol is the preferred method for interfacing with more than 1 Cirque circle
-            trackpad from the same MCU (microcontroller). The Cirque Pinnacle does not allow
-            changing the I2C slave device address (via software); this means only 1 Cirque circle trackpad
-            can be accessed over the I2C bus in the lifecycle of an application. That said, you could change
-            the I2C address from ``0x2A`` to ``0x2C`` by soldering a 470K ohm resistor at the junction
-            labeled "ADR" (see picture in `Pinout`_ section), although this is untested.
-        
-        Unsupported Features
-        --------------------
-        
-        * The legacy PS\\2 interface is pretty limited and not accessible by some CircuitPython MCUs.
-          Therefore, it has been neglected in this library.
-        * Cirque's circle trackpads ship with the newer non-AG (Advanced Gestures) variant of the
-          Pinnacle touch controller ASIC. Thus, this library focuses on the the non-AG variant's
-          functionality via testing, and it does not provide access to the older AG variant's features
-          (register addresses slightly differ which breaks compatibility).
-        
-        Pinout
-        ======
-        
-        .. image:: https://github.com/2bndy5/CircuitPython_Cirque_Pinnacle/raw/master/docs/_static/Cirque_GlidePoint-Circle-Trackpad.png
-            :target: https://www.mouser.com/new/cirque/glidepoint-circle-trackpads/
-        
-        The above picture is an example of the Cirque GlidePoint circle trackpad. This picture
-        is chosen as the test pads (larger copper circular pads) are clearly labeled. The test pads
-        are extended to the `12-pin FFC/FPC cable <https://www.mouser.com/Connectors/FFC-FPC/
-        FFC-FPC-Jumper-Cables/_/N-axro3?P=1yc8ojpZ1z0wxjx>`_ connector (the white block near the
-        bottom). The following table shows how the pins are connected in the `examples <examples.html>`_ (tested on an `ItsyBitys M4 <https://www.adafruit.com/product/3800>`_)
-        
-        .. csv-table:: pinout (ordered the same as the FFC/FPC cable connector)
-            :header: Label,"MCU pin",Description
-            :widths: 5,5,13
-        
-            SCK,SCK,"SPI clock line"
-            SO,MISO,"Master Input Slave Output"
-            SS,D7,"Slave Select (AKA Chip Select)"
-            DR,D2,"""data ready"" interrupt"
-            SI,MOSI,"SPI Master Output Slave Input"
-            B2,N/A,"Hardware input button #2"
-            B3,N/A,"Hardware input button #3"
-            B1,N/A,"Hardware input button #1"
-            SCL,SCL,"I2C clock line"
-            SDA,SDA,"I2C data line"
-            GND,GND,"Ground"
-            VDD,3V,"3V power supply"
-        
-        .. tip:: Of course, you can capture button data manually (if your application utilizes more
-            than 3 buttons), but if you connect the pins B1, B2, B3 to momentary push buttons that
-            (when pressed) provide a path to ground, the Pinnacle touch controller will report all 3
-            buttons' states for each touch (or even button only) events.
-        
-        Model Labeling Scheme
-        ---------------------
-        
-          TM\ [yyyxxx]_\ -202\ [i]_\ -\ [cc]_\ [o]_
-        
-          .. [yyyxxx] stands for the vertical & horizontal width of the trackpad, respectively.
-          .. [i] stands for the hardwired interface protocol (3 = I2C, 4 = SPI). Notice, if there is a
-            resistor populated at the R1 (470K ohm) junction (located just above the Pinnacle ASIC), it
-            is configured for SPI, otherwise it is configured for I2C.
-          .. [cc] stands for Custom Configuration which describes if a 470K ohm resistor is populated at
-            junction R4. "30" (resistor at R4 exists) means that the hardware is configured to disable
-            certain features despite what this library does. "00" (no resistor at R4) means that the
-            hardware is configured to allow certain features to be manipulated by this library. These
-            features include "secondary tap" (thought of as "right mouse button" in relative data mode),
-            Intellimouse scrolling (Microsoft patented scroll wheel behavior -- a throw back to when
-            scroll wheels were first introduced), and 180 degree orientation (your application can invert
-            the axis data anyway).
-          .. [o] stands for the overlay type (0 = none, 1 = adhesive, 2 = flat, 3 = curved)
-        
-        Dependencies
-        =============
-        This driver depends on:
-        
-        * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-        * `Bus Device <https://github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
-        
-        Please ensure all dependencies are available on the CircuitPython filesystem.
-        This is easily achieved by downloading `the Adafruit library and driver bundle
-        <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
-        
-        How to Install
-        =====================
-        This library is deployed to pypi.org, so you can easily install this library
-        using ``pip3 install circuitpython-cirque-pinnacle`` or use the following
-        commands:
-        
-        .. code-block:: shell
-        
-            git clone https://github.com/2bndy5/CircuitPython_Cirque_Pinnacle.git
-            cd CircuitPython_Cirque_Pinnacle
-            python3 setup.py install
-        
-        To install globally, prefix the last command with ``sudo``.
-        
-        Usage Example
-        =============
-        
-        Ensure you've connected the TMyyyxxx correctly by running the `examples/` located in the `examples
-        folder of this library <https://github.com/2bndy5/CircuitPython_Cirque_Pinnacle/tree/master/examples>`_.
-        
-        Contributing
-        ============
-        
-        Contributions are welcome! Please read our `Code of Conduct
-        <https://github.com/2bndy5/CircuitPython_Cirque_Pinnacle/blob/master/CODE_OF_CONDUCT.md>`_
-        before contributing to help this project stay welcoming.
-        
-        Sphinx documentation
-        -----------------------
-        
-        Sphinx is used to build the documentation based on rST files and comments in the code. First,
-        install dependencies (feel free to reuse the virtual environment from above):
-        
-        .. code-block:: shell
-        
-            python3 -m venv .env
-            source .env/bin/activate
-            pip install Sphinx sphinx-rtd-theme
-        
-        Now, once you have the virtual environment activated:
-        
-        .. code-block:: shell
-        
-            cd docs
-            sphinx-build -E -W -b html . _build/html
-        
-        This will output the documentation to ``docs/_build/html``. Open the index.html in your browser to
-        view them. It will also (due to -W) error out on any warning like Travis will. This is a good way to
-        locally verify it will pass.
-        
-Keywords: adafruit blinka circuitpython Pinnacle touch sensor driver Cirque trackpad
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: System :: Hardware
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Description-Content-Type: text/x-rst
+
+.. toctree::
+    :hidden:
+
+    self
+
+.. toctree::
+    :hidden:
+
+    examples
+
+.. toctree::
+    :caption: API Reference
+    :hidden:
+
+    api
+    rel_abs
+    anymeas
+
+.. toctree::
+    :hidden:
+
+    contributing
+
+.. toctree::
+    :caption: Related Products
+
+    Cirque Glidepoint circle trackpads <https://www.mouser.com/Search/Refine?Ntk=P_MarCom&Ntt=118816186>
+    12-pin FPC cable (0.5mm pitch) <https://www.mouser.com/Connectors/FFC-FPC/FFC-FPC-Jumper-Cables/_/N-axro3?P=1yc8ojpZ1z0wxjx>
+
+Introduction
+============
+
+A CircuitPython driver library that implements the Adafruit_BusDevice library
+for interfacing with the Cirque Pinnacle (1CA027) touch controller used in Cirque Circle Trackpads.
+
+Supported Features
+------------------
+
+* Use SPI or I2C bus protocols to interface with the Pinnacle touch controller ASIC (Application
+  Specific Integrated Circuit).
+* Relative mode data reporting (AKA Mouse mode) with optional tap detection.
+* Absolute mode data reporting (x, y, & z axis positions).
+* AnyMeas mode data reporting. This mode exposes the ADC (Analog to Digital Converter) values and is
+  not well documented in the numerous datasheets provided by the Cirque corporation about the
+  Pinnacle (1CA027), thus this is a rather experimental mode.
+* Hardware input buttons' states included in data reports. There are 3 button input lines on
+  the Cirque circle trackpads -- see `Pinout`_ section.
+* Configure measurements for finger or stylus (or automatically detirmine either) touch
+  events. The Cirque circle trackpads are natively capable of measuring only 1 touch
+  point per event.
+* Download/upload the underlying compensation matrix for ADC measurements.
+* Adjust the ADC matrix gain (sensitivity).
+
+.. tip::
+    The SPI protocol is the preferred method for interfacing with more than 1 Cirque circle
+    trackpad from the same MCU (microcontroller). The Cirque Pinnacle does not allow
+    changing the I2C slave device address (via software); this means only 1 Cirque circle trackpad
+    can be accessed over the I2C bus in the lifecycle of an application. That said, you could change
+    the I2C address from ``0x2A`` to ``0x2C`` by soldering a 470K ohm resistor at the junction
+    labeled "ADR" (see picture in `Pinout`_ section), although this is untested.
+
+Unsupported Features
+--------------------
+
+* The legacy PS\\2 interface is pretty limited and not accessible by some CircuitPython MCUs.
+  Therefore, it has been neglected in this library.
+* Cirque's circle trackpads ship with the newer non-AG (Advanced Gestures) variant of the
+  Pinnacle touch controller ASIC. Thus, this library focuses on the the non-AG variant's
+  functionality via testing, and it does not provide access to the older AG variant's features
+  (register addresses slightly differ which breaks compatibility).
+
+Pinout
+------
+
+.. warning::
+    The GPIO pins on these trackpads are **not** 5V tolerant. If your microcontroller uses 5V logic
+    (ie Arduino Nano, Uno, Pro, Micro), then you must remove the resistors at junctions "R7" and "R8".
+    Reportedly, this allows powering the trackpad with 5V (to VDD pin) and the trackpad GPIO pins become
+    tolerant of 5V logic levels.
+.. image:: https://github.com/2bndy5/CircuitPython_Cirque_Pinnacle/raw/master/docs/_static/Cirque_GlidePoint-Circle-Trackpad.png
+    :target: https://www.mouser.com/new/cirque/glidepoint-circle-trackpads/
+
+The above picture is an example of the Cirque GlidePoint circle trackpad. This picture
+is chosen as the test pads (larger copper circular pads) are clearly labeled. The test pads
+are extended to the `12-pin FFC/FPC cable
+<https://www.mouser.com/c/connectors/ffc-fpc/ffc-fpc-jumper-cables/?number%20of%20conductors=12%20Conductor&pitch=0.5%20mm>`_
+connector (the white block near the bottom). The following table shows how the pins are connected
+in the `examples <examples.html>`_ (tested on an `ItsyBitys M4 <https://www.adafruit.com/product/3800>`_ and a Raspberry Pi 2)
+
+.. csv-table:: pinout (ordered the same as the FFC/FPC cable connector)
+    :header: "cable pin number", Label, "MCU pin","RPi pin", Description
+    :widths: 4, 5, 5, 5, 13
+
+    1, SCK, SCK, SCK, "SPI clock line"
+    2, SO, MISO, MISO, "Master Input Slave Output"
+    3, SS, D2, "CE0 (GPIO8)", "Slave Select (AKA Chip Select)"
+    4, DR, D7, GPIO25, "Data Ready interrupt"
+    5, SI, MOSI, MOSI, "SPI Master Output Slave Input"
+    6, B2, N/A, N/A, "Hardware input button #2"
+    7, B3, N/A, N/A, "Hardware input button #3"
+    8, B1, N/A, N/A, "Hardware input button #1"
+    9, SCL, SCL,, SCL "I2C clock line (no builtin pull-up resistor)"
+    10, SDA, SDA, SDA, "I2C data line (no builtin pull-up resistor)"
+    11, GND, GND, GND, Ground
+    12, VDD, 3V, 3V, "3V power supply"
+
+.. tip::
+    Of course, you can capture button data manually (if your application utilizes more
+    than 3 buttons), but if you connect the pins B1, B2, B3 to momentary push buttons that
+    (when pressed) provide a path to ground, the Pinnacle touch controller will report all 3
+    buttons' states for each touch (or even button only) events.
+
+.. note::
+    These trackpads have no builtin pull-up resistors on the I2C bus' SDA and SCL lines.
+    Examples were tested with a 4.7K ohm resistor for each I2C line tied to 3v.
+
+    The Raspberry Pi boards (excluding any RP2040 boards) all have builtin 1.8K ohm pull-up
+    resistors, so the Linux examples were tested with no addition pull-up resistance.
+
+.. _HCO:
+
+Model Labeling Scheme
+*********************
+
+TM\ ``yyyxxx``\ -202\ ``i``\ -\ ``cc``\ ``o``
+
+- ``yyyxxx`` stands for the respective vertical & horizontal width of the trackpad in millimeters.
+- ``i`` stands for the hardwired interface protocol (3 = I2C, 4 = SPI). Notice, if there is a
+  resistor populated at the R1 (470K ohm) junction (located just above the Pinnacle ASIC), it
+  is configured for SPI, otherwise it is configured for I2C.
+- ``cc`` stands for Custom Configuration which describes if a 470K ohm resistor is populated at
+  junction R4. "30" (resistor at R4 exists) means that the hardware is configured to disable
+  certain features despite what this library does. "00" (no resistor at R4) means that the
+  hardware is configured to allow certain features to be manipulated by this library. These
+  features include "secondary tap" (thought of as "right mouse button" in relative data mode),
+  Intellimouse scrolling (Microsoft patented scroll wheel behavior -- a throw back to when
+  scroll wheels were first introduced), and 180 degree orientation (your application can invert
+  the axis data anyway).
+- ``o`` stands for the overlay type (0 = none, 1 = adhesive, 2 = flat, 3 = curved)
+
+Getting Started
+---------------
+
+Dependencies
+************
+
+This driver depends on:
+
+* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+* `Bus Device <https://github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
+
+Please ensure all dependencies are available on the CircuitPython filesystem.
+This is easily achieved by downloading `the Adafruit library and driver bundle
+<https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
+
+How to Install
+**************
+
+Using ``pip``
+~~~~~~~~~~~~~
+
+This library is deployed to pypi.org, so you can easily install this library
+using
+
+.. code-block:: shell
+
+    pip3 install circuitpython-cirque-pinnacle
+
+Using git source
+~~~~~~~~~~~~~~~~
+
+This library can also be installed from the git source repository.
+
+.. code-block:: shell
+
+    git clone https://github.com/2bndy5/CircuitPython_Cirque_Pinnacle.git
+    cd CircuitPython_Cirque_Pinnacle
+    python3 -m pip install .
+
+Usage Example
+*************
+
+Ensure you've connected the TMyyyxxx correctly by running the `examples/` located in the `examples
+folder of this library <https://github.com/2bndy5/CircuitPython_Cirque_Pinnacle/tree/master/examples>`_.
+
+Contributing
+------------
+
+Contributions are welcome! Please read our `Code of Conduct
+<https://github.com/2bndy5/CircuitPython_Cirque_Pinnacle/blob/master/CODE_OF_CONDUCT.md>`_
+before contributing to help this project stay welcoming.
+
+Please review our :doc:`contributing` for details on the development workflow and linting tools.
+
+To initiate a discussion of idea(s), you need only open an issue on the
+`source's git repository <https://github.com/2bndy5/CircuitPython_Cirque_Pinnacle>`_
+(it doesn't have to be a bug report).
+
+Sphinx documentation
+********************
+
+Please read our :doc:`contributing` for instructions on how to build the documentation.
```

### Comparing `circuitpython-cirque-pinnacle-0.0.4/circuitpython_cirque_pinnacle.egg-info/SOURCES.txt` & `circuitpython-cirque-pinnacle-1.0.0/circuitpython_cirque_pinnacle.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 .gitignore
-.pylintrc
+.pre-commit-config.yaml
 .readthedocs.yml
 CODE_OF_CONDUCT.md
+CONTRIBUTING.rst
 LICENSE
 README.rst
+circuitpython_cirque_pinnacle.py
+pyproject.toml
 requirements.txt
 setup.py
+.github/FUNDING.yml
 .github/workflows/build.yml
 .github/workflows/release.yml
-circuitpython_cirque_pinnacle/__init__.py
-circuitpython_cirque_pinnacle/glidepoint.py
-circuitpython_cirque_pinnacle/glidepoint_lite.py
 circuitpython_cirque_pinnacle.egg-info/PKG-INFO
 circuitpython_cirque_pinnacle.egg-info/SOURCES.txt
 circuitpython_cirque_pinnacle.egg-info/dependency_links.txt
 circuitpython_cirque_pinnacle.egg-info/requires.txt
 circuitpython_cirque_pinnacle.egg-info/top_level.txt
+docs/anymeas.rst
 docs/api.rst
 docs/conf.py
+docs/contributing.rst
 docs/examples.rst
 docs/index.rst
+docs/rel_abs.rst
+docs/requirements.txt
 docs/_static/Cirque_GlidePoint-Circle-Trackpad.png
-docs/_static/darkness.css
+docs/_static/Logo.png
+docs/_static/extra_css.css
 docs/_static/favicon.ico
-examples/cirque_pinnacle_anymeas_test.py
-examples/cirque_pinnacle_simpletest.py
+examples/cirque_pinnacle_absolute_mode.py
+examples/cirque_pinnacle_anymeas_mode.py
+examples/cirque_pinnacle_relative_mode.py
 examples/cirque_pinnacle_usb_mouse.py
```

### Comparing `circuitpython-cirque-pinnacle-0.0.4/docs/_static/Cirque_GlidePoint-Circle-Trackpad.png` & `circuitpython-cirque-pinnacle-1.0.0/docs/_static/Cirque_GlidePoint-Circle-Trackpad.png`

 * *Files identical despite different names*

### Comparing `circuitpython-cirque-pinnacle-0.0.4/docs/_static/favicon.ico` & `circuitpython-cirque-pinnacle-1.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

