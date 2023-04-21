# Comparing `tmp/lakeshore-1.6.0.tar.gz` & `tmp/lakeshore-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakeshore-1.6.0.tar", last modified: Mon Mar 27 14:00:43 2023, max compression
+gzip compressed data, was "lakeshore-1.6.1.tar", last modified: Fri Apr 21 15:42:02 2023, max compression
```

## Comparing `lakeshore-1.6.0.tar` & `lakeshore-1.6.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 14:00:43.645445 lakeshore-1.6.0/
--rw-rw-rw-   0        0        0     4003 2023-03-27 13:59:48.000000 lakeshore-1.6.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1106 2023-03-27 13:59:48.000000 lakeshore-1.6.0/LICENSE
--rw-rw-rw-   0        0        0       48 2023-03-27 13:59:49.000000 lakeshore-1.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4958 2023-03-27 14:00:43.645445 lakeshore-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     4525 2023-03-27 13:59:49.000000 lakeshore-1.6.0/README.md
--rw-rw-rw-   0        0        0        5 2023-03-27 13:59:49.000000 lakeshore-1.6.0/VERSION
-drwxrwxrwx   0        0        0        0 2023-03-27 14:00:43.645445 lakeshore-1.6.0/lakeshore/
--rw-rw-rw-   0        0        0     1384 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/__init__.py
--rw-rw-rw-   0        0        0    63668 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/fast_hall_controller.py
--rw-rw-rw-   0        0        0    10942 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/generic_instrument.py
--rw-rw-rw-   0        0        0     1065 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/model_121.py
--rw-rw-rw-   0        0        0    17159 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/model_155.py
--rw-rw-rw-   0        0        0    54949 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/model_224.py
--rw-rw-rw-   0        0        0    18745 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/model_240.py
--rw-rw-rw-   0        0        0    30747 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/model_335.py
--rw-rw-rw-   0        0        0    31409 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/model_336.py
--rw-rw-rw-   0        0        0     1069 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/model_350.py
--rw-rw-rw-   0        0        0    72172 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/model_372.py
--rw-rw-rw-   0        0        0     1025 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/model_425.py
--rw-rw-rw-   0        0        0     1071 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/model_643.py
--rw-rw-rw-   0        0        0     1057 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/model_648.py
--rw-rw-rw-   0        0        0     1120 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/requires_firmware_version.py
--rw-rw-rw-   0        0        0     1404 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/ssm_base_module.py
--rw-rw-rw-   0        0        0    38123 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/ssm_measure_module.py
--rw-rw-rw-   0        0        0     3608 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/ssm_settings_profiles.py
--rw-rw-rw-   0        0        0    44694 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/ssm_source_module.py
--rw-rw-rw-   0        0        0    22257 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/ssm_system.py
--rw-rw-rw-   0        0        0     4941 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/ssm_system_enums.py
--rw-rw-rw-   0        0        0    60182 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/temperature_controllers.py
--rw-rw-rw-   0        0        0    29728 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/teslameter.py
--rw-rw-rw-   0        0        0    15782 2023-03-27 13:59:49.000000 lakeshore-1.6.0/lakeshore/xip_instrument.py
-drwxrwxrwx   0        0        0        0 2023-03-27 14:00:43.645445 lakeshore-1.6.0/lakeshore.egg-info/
--rw-rw-rw-   0        0        0     4958 2023-03-27 14:00:43.000000 lakeshore-1.6.0/lakeshore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      873 2023-03-27 14:00:43.000000 lakeshore-1.6.0/lakeshore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 14:00:43.000000 lakeshore-1.6.0/lakeshore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-03-27 14:00:43.000000 lakeshore-1.6.0/lakeshore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-27 14:00:43.000000 lakeshore-1.6.0/lakeshore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 14:00:43.645445 lakeshore-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0      917 2023-03-27 13:59:49.000000 lakeshore-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:42:02.980605 lakeshore-1.6.1/
+-rw-rw-rw-   0        0        0     4167 2023-04-21 15:41:25.000000 lakeshore-1.6.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1106 2023-04-21 15:41:25.000000 lakeshore-1.6.1/LICENSE
+-rw-rw-rw-   0        0        0       48 2023-04-21 15:41:25.000000 lakeshore-1.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4958 2023-04-21 15:42:02.980605 lakeshore-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4525 2023-04-21 15:41:25.000000 lakeshore-1.6.1/README.md
+-rw-rw-rw-   0        0        0        5 2023-04-21 15:41:25.000000 lakeshore-1.6.1/VERSION
+drwxrwxrwx   0        0        0        0 2023-04-21 15:42:02.964980 lakeshore-1.6.1/lakeshore/
+-rw-rw-rw-   0        0        0     1384 2023-04-21 15:41:25.000000 lakeshore-1.6.1/lakeshore/__init__.py
+-rw-rw-rw-   0        0        0    63668 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/fast_hall_controller.py
+-rw-rw-rw-   0        0        0    10942 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/generic_instrument.py
+-rw-rw-rw-   0        0        0     1065 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_121.py
+-rw-rw-rw-   0        0        0    17159 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_155.py
+-rw-rw-rw-   0        0        0    54949 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_224.py
+-rw-rw-rw-   0        0        0    18745 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_240.py
+-rw-rw-rw-   0        0        0    30747 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_335.py
+-rw-rw-rw-   0        0        0    31409 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_336.py
+-rw-rw-rw-   0        0        0     1069 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_350.py
+-rw-rw-rw-   0        0        0    72172 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_372.py
+-rw-rw-rw-   0        0        0     1025 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_425.py
+-rw-rw-rw-   0        0        0     1071 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_643.py
+-rw-rw-rw-   0        0        0     1057 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/model_648.py
+-rw-rw-rw-   0        0        0     1120 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/requires_firmware_version.py
+-rw-rw-rw-   0        0        0     1404 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/ssm_base_module.py
+-rw-rw-rw-   0        0        0    38123 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/ssm_measure_module.py
+-rw-rw-rw-   0        0        0     3608 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/ssm_settings_profiles.py
+-rw-rw-rw-   0        0        0    48487 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/ssm_source_module.py
+-rw-rw-rw-   0        0        0    22443 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/ssm_system.py
+-rw-rw-rw-   0        0        0     4941 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/ssm_system_enums.py
+-rw-rw-rw-   0        0        0    60182 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/temperature_controllers.py
+-rw-rw-rw-   0        0        0    29728 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/teslameter.py
+-rw-rw-rw-   0        0        0    15782 2023-04-21 15:41:26.000000 lakeshore-1.6.1/lakeshore/xip_instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:42:02.980605 lakeshore-1.6.1/lakeshore.egg-info/
+-rw-rw-rw-   0        0        0     4958 2023-04-21 15:42:02.000000 lakeshore-1.6.1/lakeshore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      873 2023-04-21 15:42:02.000000 lakeshore-1.6.1/lakeshore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 15:42:02.000000 lakeshore-1.6.1/lakeshore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-04-21 15:42:02.000000 lakeshore-1.6.1/lakeshore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 15:42:02.000000 lakeshore-1.6.1/lakeshore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 15:42:02.980605 lakeshore-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      953 2023-04-21 15:41:25.000000 lakeshore-1.6.1/setup.py
```

### Comparing `lakeshore-1.6.0/CHANGELOG.md` & `lakeshore-1.6.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Change Log
 ==========
 
+Release 1.6.1
+-------------
+Added:
+- Added explicit requirement for packaging package
+
+Fixed:
+- Catch error on wakepy import that breaks in some scenarios
+
 Release 1.6.0
 -------------
 Added:
 - M81 data sources enumeration and example
 - Enable and disable for lock-in IIR filter on M81
 - Read subsystem support for M81
 - Settings profiles for M81 include summary and notes queries
```

### Comparing `lakeshore-1.6.0/LICENSE` & `lakeshore-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/PKG-INFO` & `lakeshore-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakeshore
-Version: 1.6.0
+Version: 1.6.1
 Summary: A package to connect to and interact with Lake Shore instruments.
 Home-page: https://github.com/lakeshorecryotronics/python-driver
 Maintainer: Lake Shore Cryotronics, Inc.
 Maintainer-email: service@lakeshore.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lakeshore-1.6.0/README.md` & `lakeshore-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/__init__.py` & `lakeshore-1.6.1/lakeshore/__init__.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/fast_hall_controller.py` & `lakeshore-1.6.1/lakeshore/fast_hall_controller.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/generic_instrument.py` & `lakeshore-1.6.1/lakeshore/generic_instrument.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/model_121.py` & `lakeshore-1.6.1/lakeshore/model_121.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/model_155.py` & `lakeshore-1.6.1/lakeshore/model_155.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/model_224.py` & `lakeshore-1.6.1/lakeshore/model_224.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/model_240.py` & `lakeshore-1.6.1/lakeshore/model_240.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/model_335.py` & `lakeshore-1.6.1/lakeshore/model_335.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/model_336.py` & `lakeshore-1.6.1/lakeshore/model_336.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/model_350.py` & `lakeshore-1.6.1/lakeshore/model_350.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/model_372.py` & `lakeshore-1.6.1/lakeshore/model_372.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/model_425.py` & `lakeshore-1.6.1/lakeshore/model_425.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/model_643.py` & `lakeshore-1.6.1/lakeshore/model_643.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/model_648.py` & `lakeshore-1.6.1/lakeshore/model_648.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/requires_firmware_version.py` & `lakeshore-1.6.1/lakeshore/requires_firmware_version.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/ssm_base_module.py` & `lakeshore-1.6.1/lakeshore/ssm_base_module.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/ssm_measure_module.py` & `lakeshore-1.6.1/lakeshore/ssm_measure_module.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/ssm_settings_profiles.py` & `lakeshore-1.6.1/lakeshore/ssm_settings_profiles.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/ssm_source_module.py` & `lakeshore-1.6.1/lakeshore/ssm_source_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Implements functionality unique to the M81 Source Modules."""
 
+import math
 from datetime import datetime
 from warnings import warn
 
 from lakeshore.xip_instrument import RegisterBase
 from lakeshore.ssm_base_module import SSMSystemModuleQuestionableRegister, BaseModule
 from lakeshore.requires_firmware_version import requires_firmware_version
 
@@ -466,18 +467,14 @@
         """Returns the current amplitude for the module in Amps"""
 
         return float(self.device.query(f'SOURce{self.module_number}:CURRent:LEVel:AMPLitude?'))
 
     def get_i_amplitude(self):
         """
         Returns the current amplitude for the module in Amps
-
-            Args:
-                amplitude (float):
-                    The new current amplitude in Amps
         
         .. deprecated:: 1.5.4
            Use get_current_amplitude instead.
         """
 
         warn("The get_i_amplitude method is deprecated, use get_current_amplitude instead", DeprecationWarning)
         return self.get_current_amplitude()
@@ -1096,20 +1093,20 @@
         Args:
             sweep_type (SourceSweepType):
                 The sweep type for which to return the sweep settings.
         """
 
         return self.device.SourceSweepSettings(
             sweep_type,
-            self.device.query(f'SOURce{self.module_number}:{sweep_type}:STARt?'),
-            self.device.query(f'SOURce{self.module_number}:{sweep_type}:STOP?'),
-            self.device.query(f'SOURce{self.module_number}:SWEep:POINts?'),
-            self.device.query(f'SOURce{self.module_number}:SWEep:DWELl?'),
+            float(self.device.query(f'SOURce{self.module_number}:{sweep_type}:STARt?')),
+            float(self.device.query(f'SOURce{self.module_number}:{sweep_type}:STOP?')),
+            int(self.device.query(f'SOURce{self.module_number}:SWEep:POINts?')),
+            float(self.device.query(f'SOURce{self.module_number}:SWEep:DWELl?')),
             self.device.query(f'SOURce{self.module_number}:SWEep:DIRection?'),
-            self.device.query(f'SOURce{self.module_number}:SWEep:DIRection:RTRip?'),
+            bool(int(self.device.query(f'SOURce{self.module_number}:SWEep:DIRection:RTRip?'))),
             self.device.query(f'SOURce{self.module_number}:SWEep:SPACing?'))
 
     @requires_firmware_version('1.7.0')
     def disable_all_sweeping(self):
         """Disables all source signals that support sweeping on the specified module."""
 
         for sweep_type in self.device.SourceSweepType:
@@ -1122,7 +1119,75 @@
 
         Args:
             sweep_type (SourceSweepType):
                 The type of sweep to disable.
         """
 
         self.device.command(f'SOURce{self.module_number}:{sweep_type}:MODE FIXED')
+
+    def set_voltage_ramp_configuration(self, stop_amplitude, start_amplitude=None, slew_rate=1.0):
+        """
+        Sets up a parameter sweep that ramps the voltage output to the desired amplitude using the smallest
+        possible step size.
+
+        Args:
+            stop_amplitude (float):
+                The voltage amplitude of the output when the ramp completes.
+
+            start_amplitude (float):
+                The voltage amplitude of the output when the ramp starts. Default is the present amplitude setting.
+
+            slew_rate (float):
+                The rate in volts per second to ramp the output. Default is 1 volt per second.
+        """
+        # Use the present voltage amplitude as the starting point if no start is specified
+        if start_amplitude is None:
+            start_amplitude = self.get_voltage_amplitude()
+
+        ramp_total_time = abs(stop_amplitude - start_amplitude) / abs(slew_rate)
+
+        # Determine the shortest dwell time that can be used without exceeding the maximum number of points
+        dwell_time = math.ceil(ramp_total_time / (self.device.min_sweep_dwell * self.device.max_sweep_points)) * self.device.min_sweep_dwell
+        num_points = round(ramp_total_time / dwell_time)
+
+        sweep_config = self.device.SourceSweepSettings(sweep_type=self.device.SourceSweepType.VOLTAGE_AMPLITUDE,
+                                                       start=start_amplitude,
+                                                       stop=stop_amplitude,
+                                                       points=num_points,
+                                                       dwell=dwell_time,
+                                                       direction=self.device.SourceSweepSettings.Direction.UP,
+                                                       round_trip=False)
+        self.set_sweep_configuration(sweep_config)
+
+    def set_current_ramp_configuration(self, stop_amplitude, start_amplitude=None, slew_rate=0.001):
+        """
+        Sets up a parameter sweep that ramps the current output to the desired amplitude using the smallest
+        possible step size.
+
+        Args:
+            stop_amplitude (float):
+                The current amplitude of the output when the ramp completes.
+
+            start_amplitude (float):
+                The current amplitude of the output when the ramp starts. Default is the present amplitude setting.
+
+            slew_rate (float):
+                The rate in amps per second to ramp the output. Default is 1 mA per second.
+        """
+        # Use the present voltage amplitude as the starting point if no start is specified
+        if start_amplitude is None:
+            start_amplitude = self.get_current_amplitude()
+
+        ramp_total_time = abs(stop_amplitude - start_amplitude) / abs(slew_rate)
+
+        # Determine the shortest dwell time that can be used without exceeding the maximum number of points
+        dwell_time = math.ceil(ramp_total_time / (self.device.min_sweep_dwell * self.device.max_sweep_points)) * self.device.min_sweep_dwell
+        num_points = round(ramp_total_time / dwell_time)
+
+        sweep_config = self.device.SourceSweepSettings(sweep_type=self.device.SourceSweepType.CURRENT_AMPLITUDE,
+                                                       start=start_amplitude,
+                                                       stop=stop_amplitude,
+                                                       points=num_points,
+                                                       dwell=dwell_time,
+                                                       direction=self.device.SourceSweepSettings.Direction.UP,
+                                                       round_trip=False)
+        self.set_sweep_configuration(sweep_config)
```

### Comparing `lakeshore-1.6.0/lakeshore/ssm_system.py` & `lakeshore-1.6.1/lakeshore/ssm_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from lakeshore.ssm_settings_profiles import SettingsProfiles
 from lakeshore.requires_firmware_version import requires_firmware_version
 
 try:
     from wakepy import keepawake
 except NotImplementedError:
     pass  # Proceed without wakepy on linux without systemd
+except KeyError:
+    pass  # Proceed without wakepy on linux without dbus
 
 
 class SSMSystemOperationRegister(RegisterBase):
     """Class object representing the operation status register"""
 
     bit_names = [
         "s1_summary",
@@ -124,14 +126,18 @@
         self.source_modules = [SourceModule(i + 1, self) for i in range(self.get_num_source_channels())]
         self.measure_modules = [MeasureModule(i + 1, self) for i in range(self.get_num_measure_channels())]
 
         self.settings_profiles = SettingsProfiles(self)
 
         self.stream_lock = Lock()
 
+        # Sweeping limits
+        self.min_sweep_dwell = 0.000_2
+        self.max_sweep_points = 100_001
+
     def load_modules(self):
         """Loads all unloaded modules. Connected modules must be loaded before they can be used"""
         self.command('SYSTem:LOAD')
 
     def get_num_measure_channels(self):
         """Returns the number of measure channels supported by the instrument"""
```

### Comparing `lakeshore-1.6.0/lakeshore/ssm_system_enums.py` & `lakeshore-1.6.1/lakeshore/ssm_system_enums.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/temperature_controllers.py` & `lakeshore-1.6.1/lakeshore/temperature_controllers.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/teslameter.py` & `lakeshore-1.6.1/lakeshore/teslameter.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore/xip_instrument.py` & `lakeshore-1.6.1/lakeshore/xip_instrument.py`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/lakeshore.egg-info/PKG-INFO` & `lakeshore-1.6.1/lakeshore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakeshore
-Version: 1.6.0
+Version: 1.6.1
 Summary: A package to connect to and interact with Lake Shore instruments.
 Home-page: https://github.com/lakeshorecryotronics/python-driver
 Maintainer: Lake Shore Cryotronics, Inc.
 Maintainer-email: service@lakeshore.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lakeshore-1.6.0/lakeshore.egg-info/SOURCES.txt` & `lakeshore-1.6.1/lakeshore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lakeshore-1.6.0/setup.py` & `lakeshore-1.6.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,11 +17,12 @@
     description='A package to connect to and interact with Lake Shore instruments.',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=[r'lakeshore'],
     url='https://github.com/lakeshorecryotronics/python-driver',
     install_requires=['pyserial>=3.0',
                       'iso8601',
+                      'packaging',
                       "enum34;python_version<'3.4'",
                       'wakepy>=0.4.0'],
     classifiers=['Programming Language :: Python :: 3']
 )
```

