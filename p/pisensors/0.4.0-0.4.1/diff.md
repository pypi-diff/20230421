# Comparing `tmp/pisensors-0.4.0.tar.gz` & `tmp/pisensors-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisensors-0.4.0.tar", last modified: Wed Apr 19 18:53:00 2023, max compression
+gzip compressed data, was "pisensors-0.4.1.tar", last modified: Fri Apr 21 06:41:15 2023, max compression
```

## Comparing `pisensors-0.4.0.tar` & `pisensors-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:53:00.796304 pisensors-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-19 18:53:00.796304 pisensors-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-19 18:52:46.000000 pisensors-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:53:00.796304 pisensors-0.4.0/pisensors/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-19 18:52:46.000000 pisensors-0.4.0/pisensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-19 18:52:47.000000 pisensors-0.4.0/pisensors/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-19 18:52:47.000000 pisensors-0.4.0/pisensors/sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:53:00.796304 pisensors-0.4.0/pisensors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-19 18:53:00.000000 pisensors-0.4.0/pisensors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-19 18:53:00.000000 pisensors-0.4.0/pisensors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:53:00.000000 pisensors-0.4.0/pisensors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 18:53:00.000000 pisensors-0.4.0/pisensors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 18:53:00.000000 pisensors-0.4.0/pisensors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:53:00.796304 pisensors-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-19 18:52:47.000000 pisensors-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:41:15.035365 pisensors-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-21 06:41:15.035365 pisensors-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-21 06:41:04.000000 pisensors-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:41:15.035365 pisensors-0.4.1/pisensors/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 06:41:04.000000 pisensors-0.4.1/pisensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-21 06:41:04.000000 pisensors-0.4.1/pisensors/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-21 06:41:04.000000 pisensors-0.4.1/pisensors/sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:41:15.035365 pisensors-0.4.1/pisensors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-21 06:41:14.000000 pisensors-0.4.1/pisensors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-21 06:41:14.000000 pisensors-0.4.1/pisensors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:41:14.000000 pisensors-0.4.1/pisensors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-21 06:41:14.000000 pisensors-0.4.1/pisensors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 06:41:14.000000 pisensors-0.4.1/pisensors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 06:41:15.035365 pisensors-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-21 06:41:04.000000 pisensors-0.4.1/setup.py
```

### Comparing `pisensors-0.4.0/PKG-INFO` & `pisensors-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisensors
-Version: 0.4.0
+Version: 0.4.1
 Summary: Raspberry Pi Sensors script for Temperature & Humidity
 Home-page: https://github.com/Phornee/pisensors
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # pisensors
         Raspberry Pi Sensors script for Temperature & Humidity.
```

### Comparing `pisensors-0.4.0/pisensors/sensors.py` & `pisensors-0.4.1/pisensors/sensors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """ Read DHT22 sensors """
 import os
 from pathlib import Path
 from influxdb_wrapper import influxdb_factory
-from baseutils_phornee import is_raspberry_pi
 from log_mgr import Logger
 from config_yml import Config
 
 
 class Sensors():
     """Read inputs from DHT22 sensors (temperature & humidity) and write it to influx database"""
 
@@ -29,30 +28,28 @@
 
     def sensor_read(self):
         """
         Read sensors information
         """
         have_readings = False
 
-        if is_raspberry_pi():
-            try:
-                import adafruit_dht  # pylint: disable=import-outside-toplevel
-
-                dht_sensor = adafruit_dht.DHT22(self.config["pin"])
+        try:
+            import adafruit_dht  # pylint: disable=import-outside-toplevel
 
-                humidity = dht_sensor.humidity
-                temp_c = dht_sensor.temperature
-
-                have_readings = True
-            except Exception as ex:
-                self.logger.error(f"Error reading sensor DHT22: {ex}")
-        else:
+            dht_sensor = adafruit_dht.DHT22(self.config["pin"])
+            humidity = dht_sensor.humidity
+            temp_c = dht_sensor.temperature
+            have_readings = True
+        except ModuleNotFoundError:
+            self.logger.warning("No adafruit supported: returning default values.")
             humidity = 50
             temp_c = 25
             have_readings = True
+        except Exception as ex:
+            self.logger.error(f"Error reading sensor DHT22: {ex}")
 
         if have_readings:
             try:
                 points = [
                     {
                         "tags": {"sensorid": self.config["id"]},
                         "fields": {"temp": float(temp_c), "humidity": float(humidity)},
```

### Comparing `pisensors-0.4.0/pisensors.egg-info/PKG-INFO` & `pisensors-0.4.1/pisensors.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisensors
-Version: 0.4.0
+Version: 0.4.1
 Summary: Raspberry Pi Sensors script for Temperature & Humidity
 Home-page: https://github.com/Phornee/pisensors
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # pisensors
         Raspberry Pi Sensors script for Temperature & Humidity.
```

### Comparing `pisensors-0.4.0/setup.py` & `pisensors-0.4.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pisensors",
-    version="0.4.0",
+    version="0.4.1",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Sensors script for Temperature & Humidity",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/pisensors",
     packages=setuptools.find_packages(),
@@ -19,15 +19,14 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Topic :: Home Automation"
     ],
     install_requires=[
-        'baseutils_phornee>=0.1.2',
         'config_yml>=0.2.0',
         'log_mgr>=0.0.1',
         'influxdb_wrapper>=0.0.3',
         'adafruit-circuitpython-dht>=3.5.1'
     ],
     python_requires='>=3.6',
 )
```

