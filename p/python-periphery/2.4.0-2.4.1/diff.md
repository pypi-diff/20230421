# Comparing `tmp/python-periphery-2.4.0.tar.gz` & `tmp/python-periphery-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-periphery-2.4.0.tar", last modified: Tue Apr 18 04:09:03 2023, max compression
+gzip compressed data, was "python-periphery-2.4.1.tar", last modified: Fri Apr 21 06:19:12 2023, max compression
```

## Comparing `python-periphery-2.4.0.tar` & `python-periphery-2.4.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-04-18 04:09:03.215770 python-periphery-2.4.0/
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1099 2023-04-18 04:01:48.000000 python-periphery-2.4.0/LICENSE
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1457 2023-04-18 04:09:03.215770 python-periphery-2.4.0/PKG-INFO
--rw-r--r--   0 anteater  (1000) anteater  (1000)     5634 2023-04-14 08:42:18.000000 python-periphery-2.4.0/README.md
-drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-04-18 04:09:03.215770 python-periphery-2.4.0/periphery/
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1030 2023-04-18 04:02:08.000000 python-periphery-2.4.0/periphery/__init__.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)      698 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/__init__.pyi
--rw-r--r--   0 anteater  (1000) anteater  (1000)     9960 2023-04-18 03:59:26.000000 python-periphery-2.4.0/periphery/gpio.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1935 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/gpio.pyi
--rw-r--r--   0 anteater  (1000) anteater  (1000)    20665 2023-04-18 03:59:26.000000 python-periphery-2.4.0/periphery/gpio_cdev1.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)    21051 2023-04-18 03:59:26.000000 python-periphery-2.4.0/periphery/gpio_cdev2.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)    11903 2023-04-18 03:59:26.000000 python-periphery-2.4.0/periphery/gpio_sysfs.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)     6769 2019-10-29 03:46:27.000000 python-periphery-2.4.0/periphery/i2c.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)      752 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/i2c.pyi
--rw-r--r--   0 anteater  (1000) anteater  (1000)     5997 2019-10-29 03:46:27.000000 python-periphery-2.4.0/periphery/led.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)      704 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/led.pyi
--rw-r--r--   0 anteater  (1000) anteater  (1000)    10469 2023-04-18 03:59:26.000000 python-periphery-2.4.0/periphery/mmio.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1032 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/mmio.pyi
--rw-r--r--   0 anteater  (1000) anteater  (1000)    10220 2023-04-18 03:59:26.000000 python-periphery-2.4.0/periphery/pwm.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)      749 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/pwm.pyi
--rw-r--r--   0 anteater  (1000) anteater  (1000)        0 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/py.typed
--rw-r--r--   0 anteater  (1000) anteater  (1000)    25275 2020-05-28 05:33:30.000000 python-periphery-2.4.0/periphery/serial.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1114 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/serial.pyi
--rw-r--r--   0 anteater  (1000) anteater  (1000)    15568 2021-02-04 07:36:15.000000 python-periphery-2.4.0/periphery/spi.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)      806 2023-04-18 04:01:40.000000 python-periphery-2.4.0/periphery/spi.pyi
-drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-04-18 04:09:03.215770 python-periphery-2.4.0/python_periphery.egg-info/
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1457 2023-04-18 04:09:03.000000 python-periphery-2.4.0/python_periphery.egg-info/PKG-INFO
--rw-r--r--   0 anteater  (1000) anteater  (1000)      757 2023-04-18 04:09:03.000000 python-periphery-2.4.0/python_periphery.egg-info/SOURCES.txt
--rw-r--r--   0 anteater  (1000) anteater  (1000)        1 2023-04-18 04:09:03.000000 python-periphery-2.4.0/python_periphery.egg-info/dependency_links.txt
--rw-r--r--   0 anteater  (1000) anteater  (1000)       10 2023-04-18 04:09:03.000000 python-periphery-2.4.0/python_periphery.egg-info/top_level.txt
--rw-r--r--   0 anteater  (1000) anteater  (1000)      131 2023-04-18 04:09:03.215770 python-periphery-2.4.0/setup.cfg
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1688 2023-04-18 04:02:08.000000 python-periphery-2.4.0/setup.py
-drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-04-18 04:09:03.215770 python-periphery-2.4.0/tests/
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1258 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)    11956 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test_gpio.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)     8499 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test_gpio_sysfs.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)     3001 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test_i2c.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)     3592 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test_led.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)     5896 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test_mmio.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)     7312 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test_pwm.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)     8865 2020-05-29 06:20:50.000000 python-periphery-2.4.0/tests/test_serial.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)     5681 2020-12-10 07:07:56.000000 python-periphery-2.4.0/tests/test_spi.py
+drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-04-21 06:19:12.809902 python-periphery-2.4.1/
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1099 2023-04-18 04:01:48.000000 python-periphery-2.4.1/LICENSE
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1457 2023-04-21 06:19:12.809902 python-periphery-2.4.1/PKG-INFO
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     5634 2023-04-14 08:42:18.000000 python-periphery-2.4.1/README.md
+drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-04-21 06:19:12.809902 python-periphery-2.4.1/periphery/
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1030 2023-04-21 06:15:11.000000 python-periphery-2.4.1/periphery/__init__.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      698 2023-04-18 04:01:40.000000 python-periphery-2.4.1/periphery/__init__.pyi
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     9960 2023-04-18 03:59:26.000000 python-periphery-2.4.1/periphery/gpio.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1935 2023-04-18 04:01:40.000000 python-periphery-2.4.1/periphery/gpio.pyi
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    20665 2023-04-18 03:59:26.000000 python-periphery-2.4.1/periphery/gpio_cdev1.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    21199 2023-04-21 06:15:01.000000 python-periphery-2.4.1/periphery/gpio_cdev2.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    11903 2023-04-18 03:59:26.000000 python-periphery-2.4.1/periphery/gpio_sysfs.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     6769 2019-10-29 03:46:27.000000 python-periphery-2.4.1/periphery/i2c.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      752 2023-04-18 04:01:40.000000 python-periphery-2.4.1/periphery/i2c.pyi
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     5997 2019-10-29 03:46:27.000000 python-periphery-2.4.1/periphery/led.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      704 2023-04-18 04:01:40.000000 python-periphery-2.4.1/periphery/led.pyi
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    10469 2023-04-18 03:59:26.000000 python-periphery-2.4.1/periphery/mmio.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1032 2023-04-18 04:01:40.000000 python-periphery-2.4.1/periphery/mmio.pyi
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    10220 2023-04-18 03:59:26.000000 python-periphery-2.4.1/periphery/pwm.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      749 2023-04-18 04:01:40.000000 python-periphery-2.4.1/periphery/pwm.pyi
+-rw-r--r--   0 anteater  (1000) anteater  (1000)        0 2023-04-18 04:01:40.000000 python-periphery-2.4.1/periphery/py.typed
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    25275 2020-05-28 05:33:30.000000 python-periphery-2.4.1/periphery/serial.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1114 2023-04-18 04:01:40.000000 python-periphery-2.4.1/periphery/serial.pyi
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    15568 2021-02-04 07:36:15.000000 python-periphery-2.4.1/periphery/spi.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      806 2023-04-18 04:01:40.000000 python-periphery-2.4.1/periphery/spi.pyi
+drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-04-21 06:19:12.809902 python-periphery-2.4.1/python_periphery.egg-info/
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1457 2023-04-21 06:19:12.000000 python-periphery-2.4.1/python_periphery.egg-info/PKG-INFO
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      757 2023-04-21 06:19:12.000000 python-periphery-2.4.1/python_periphery.egg-info/SOURCES.txt
+-rw-r--r--   0 anteater  (1000) anteater  (1000)        1 2023-04-21 06:19:12.000000 python-periphery-2.4.1/python_periphery.egg-info/dependency_links.txt
+-rw-r--r--   0 anteater  (1000) anteater  (1000)       10 2023-04-21 06:19:12.000000 python-periphery-2.4.1/python_periphery.egg-info/top_level.txt
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      131 2023-04-21 06:19:12.809902 python-periphery-2.4.1/setup.cfg
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1688 2023-04-21 06:15:11.000000 python-periphery-2.4.1/setup.py
+drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-04-21 06:19:12.809902 python-periphery-2.4.1/tests/
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1258 2020-05-29 06:20:50.000000 python-periphery-2.4.1/tests/test.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    11956 2020-05-29 06:20:50.000000 python-periphery-2.4.1/tests/test_gpio.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     8499 2020-05-29 06:20:50.000000 python-periphery-2.4.1/tests/test_gpio_sysfs.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     3001 2020-05-29 06:20:50.000000 python-periphery-2.4.1/tests/test_i2c.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     3592 2020-05-29 06:20:50.000000 python-periphery-2.4.1/tests/test_led.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     5896 2020-05-29 06:20:50.000000 python-periphery-2.4.1/tests/test_mmio.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     7312 2020-05-29 06:20:50.000000 python-periphery-2.4.1/tests/test_pwm.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     8865 2020-05-29 06:20:50.000000 python-periphery-2.4.1/tests/test_serial.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     5681 2020-12-10 07:07:56.000000 python-periphery-2.4.1/tests/test_spi.py
```

### Comparing `python-periphery-2.4.0/LICENSE` & `python-periphery-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/PKG-INFO` & `python-periphery-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-periphery
-Version: 2.4.0
+Version: 2.4.1
 Summary: A pure Python 2/3 library for peripheral I/O (GPIO, LED, PWM, SPI, I2C, MMIO, Serial) in Linux.
 Home-page: https://github.com/vsergeev/python-periphery
 Author: vsergeev
 Author-email: v@sergeev.io
 License: MIT
 Keywords: gpio spi led pwm i2c mmio serial uart embedded linux beaglebone raspberrypi rpi odroid
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-periphery-2.4.0/README.md` & `python-periphery-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/__init__.py` & `python-periphery-2.4.1/periphery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 "Module version string."
 
-version = (2, 4, 0)
+version = (2, 4, 1)
 "Module version tuple."
 
 
 def sleep(seconds):
     """Sleep for the specified number of seconds.
 
     Args:
```

### Comparing `python-periphery-2.4.0/periphery/__init__.pyi` & `python-periphery-2.4.1/periphery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/gpio.py` & `python-periphery-2.4.1/periphery/gpio.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/gpio.pyi` & `python-periphery-2.4.1/periphery/gpio.pyi`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/gpio_cdev1.py` & `python-periphery-2.4.1/periphery/gpio_cdev1.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/gpio_cdev2.py` & `python-periphery-2.4.1/periphery/gpio_cdev2.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
     _GPIO_V2_LINE_FLAG_EDGE_RISING = 0x10
     _GPIO_V2_LINE_FLAG_EDGE_FALLING = 0x20
     _GPIO_V2_LINE_FLAG_OPEN_DRAIN = 0x40
     _GPIO_V2_LINE_FLAG_OPEN_SOURCE = 0x80
     _GPIO_V2_LINE_FLAG_BIAS_PULL_UP = 0x100
     _GPIO_V2_LINE_FLAG_BIAS_PULL_DOWN = 0x200
     _GPIO_V2_LINE_FLAG_BIAS_DISABLED = 0x400
+    _GPIO_V2_LINE_FLAG_EVENT_CLOCK_REALTIME = 0x800
 
     SUPPORTED = KERNEL_VERSION >= (5, 10)
 
     def __init__(self, path, line, direction, edge="none", bias="default", drive="default", inverted=False, label=None):
         """**Character device GPIO (ABI version 2)**
 
         Instantiate a GPIO object and open the character device GPIO with the
@@ -253,14 +254,15 @@
 
             self._line_fd = None
 
         line_request = _CGpioV2LineRequest()
 
         if direction == "in":
             flags |= Cdev2GPIO._GPIO_V2_LINE_FLAG_EDGE_RISING if edge == "rising" else Cdev2GPIO._GPIO_V2_LINE_FLAG_EDGE_FALLING if edge == "falling" else (Cdev2GPIO._GPIO_V2_LINE_FLAG_EDGE_RISING | Cdev2GPIO._GPIO_V2_LINE_FLAG_EDGE_FALLING) if edge == "both" else 0
+            flags |= Cdev2GPIO._GPIO_V2_LINE_FLAG_EVENT_CLOCK_REALTIME if edge != "none" else 0
 
             line_request.offsets[0] = self._line
             line_request.consumer = self._label
             line_request.config.flags = flags | Cdev2GPIO._GPIO_V2_LINE_FLAG_INPUT
             line_request.num_lines = 1
 
             try:
```

### Comparing `python-periphery-2.4.0/periphery/gpio_sysfs.py` & `python-periphery-2.4.1/periphery/gpio_sysfs.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/i2c.py` & `python-periphery-2.4.1/periphery/i2c.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/i2c.pyi` & `python-periphery-2.4.1/periphery/i2c.pyi`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/led.py` & `python-periphery-2.4.1/periphery/led.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/led.pyi` & `python-periphery-2.4.1/periphery/led.pyi`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/mmio.py` & `python-periphery-2.4.1/periphery/mmio.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/mmio.pyi` & `python-periphery-2.4.1/periphery/mmio.pyi`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/pwm.py` & `python-periphery-2.4.1/periphery/pwm.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/pwm.pyi` & `python-periphery-2.4.1/periphery/pwm.pyi`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/serial.py` & `python-periphery-2.4.1/periphery/serial.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/serial.pyi` & `python-periphery-2.4.1/periphery/serial.pyi`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/spi.py` & `python-periphery-2.4.1/periphery/spi.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/periphery/spi.pyi` & `python-periphery-2.4.1/periphery/spi.pyi`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/python_periphery.egg-info/PKG-INFO` & `python-periphery-2.4.1/python_periphery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-periphery
-Version: 2.4.0
+Version: 2.4.1
 Summary: A pure Python 2/3 library for peripheral I/O (GPIO, LED, PWM, SPI, I2C, MMIO, Serial) in Linux.
 Home-page: https://github.com/vsergeev/python-periphery
 Author: vsergeev
 Author-email: v@sergeev.io
 License: MIT
 Keywords: gpio spi led pwm i2c mmio serial uart embedded linux beaglebone raspberrypi rpi odroid
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-periphery-2.4.0/python_periphery.egg-info/SOURCES.txt` & `python-periphery-2.4.1/python_periphery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/setup.py` & `python-periphery-2.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='python-periphery',
-    version='2.4.0',
+    version='2.4.1',
     description='A pure Python 2/3 library for peripheral I/O (GPIO, LED, PWM, SPI, I2C, MMIO, Serial) in Linux.',
     author='vsergeev',
     author_email='v@sergeev.io',
     url='https://github.com/vsergeev/python-periphery',
     packages=['periphery'],
     package_data={'periphery': ['*.pyi', 'py.typed']},
     long_description="""python-periphery is a pure Python library for GPIO, LED, PWM, SPI, I2C, MMIO, and Serial peripheral I/O interface access in userspace Linux. It is useful in embedded Linux environments (including Raspberry Pi, BeagleBone, etc. platforms) for interfacing with external peripherals. python-periphery is compatible with Python 2 and Python 3, is written in pure Python, and is MIT licensed. See https://github.com/vsergeev/python-periphery for more information.""",
```

### Comparing `python-periphery-2.4.0/tests/test.py` & `python-periphery-2.4.1/tests/test.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/tests/test_gpio.py` & `python-periphery-2.4.1/tests/test_gpio.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/tests/test_gpio_sysfs.py` & `python-periphery-2.4.1/tests/test_gpio_sysfs.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/tests/test_i2c.py` & `python-periphery-2.4.1/tests/test_i2c.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/tests/test_led.py` & `python-periphery-2.4.1/tests/test_led.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/tests/test_mmio.py` & `python-periphery-2.4.1/tests/test_mmio.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/tests/test_pwm.py` & `python-periphery-2.4.1/tests/test_pwm.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/tests/test_serial.py` & `python-periphery-2.4.1/tests/test_serial.py`

 * *Files identical despite different names*

### Comparing `python-periphery-2.4.0/tests/test_spi.py` & `python-periphery-2.4.1/tests/test_spi.py`

 * *Files identical despite different names*

