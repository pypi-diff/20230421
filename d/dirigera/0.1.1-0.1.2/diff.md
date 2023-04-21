# Comparing `tmp/dirigera-0.1.1.tar.gz` & `tmp/dirigera-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-0.1.1.tar", last modified: Thu Apr  6 19:20:35 2023, max compression
+gzip compressed data, was "dirigera-0.1.2.tar", last modified: Fri Apr 21 14:19:17 2023, max compression
```

## Comparing `dirigera-0.1.1.tar` & `dirigera-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:20:35.588326 dirigera-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-06 19:20:26.000000 dirigera-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-06 19:20:35.588326 dirigera-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-06 19:20:26.000000 dirigera-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-06 19:20:26.000000 dirigera-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 19:20:35.588326 dirigera-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-06 19:20:26.000000 dirigera-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:20:35.584326 dirigera-0.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 19:20:26.000000 dirigera-0.1.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:20:35.584326 dirigera-0.1.1/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-06 19:20:26.000000 dirigera-0.1.1/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:20:35.588326 dirigera-0.1.1/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 19:20:26.000000 dirigera-0.1.1/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-06 19:20:26.000000 dirigera-0.1.1/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-06 19:20:26.000000 dirigera-0.1.1/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-06 19:20:26.000000 dirigera-0.1.1/src/dirigera/devices/light.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:20:35.588326 dirigera-0.1.1/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 19:20:26.000000 dirigera-0.1.1/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-06 19:20:26.000000 dirigera-0.1.1/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-06 19:20:26.000000 dirigera-0.1.1/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-06 19:20:26.000000 dirigera-0.1.1/src/dirigera/hub/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:20:35.588326 dirigera-0.1.1/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-06 19:20:35.000000 dirigera-0.1.1/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-06 19:20:35.000000 dirigera-0.1.1/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:20:35.000000 dirigera-0.1.1/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-06 19:20:35.000000 dirigera-0.1.1/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-06 19:20:35.000000 dirigera-0.1.1/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-06 19:20:35.000000 dirigera-0.1.1/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:20:35.588326 dirigera-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-06 19:20:26.000000 dirigera-0.1.1/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-04-06 19:20:26.000000 dirigera-0.1.1/tests/test_light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:17.053646 dirigera-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-21 14:19:07.000000 dirigera-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-21 14:19:17.053646 dirigera-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-21 14:19:07.000000 dirigera-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-21 14:19:07.000000 dirigera-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:19:17.057646 dirigera-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-21 14:19:07.000000 dirigera-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:17.053646 dirigera-0.1.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:17.053646 dirigera-0.1.2/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:17.053646 dirigera-0.1.2/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/devices/light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:17.053646 dirigera-0.1.2/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-21 14:19:07.000000 dirigera-0.1.2/src/dirigera/hub/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:17.053646 dirigera-0.1.2/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-21 14:19:17.000000 dirigera-0.1.2/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-21 14:19:17.000000 dirigera-0.1.2/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:19:17.000000 dirigera-0.1.2/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-21 14:19:17.000000 dirigera-0.1.2/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-21 14:19:17.000000 dirigera-0.1.2/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 14:19:17.000000 dirigera-0.1.2/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:19:17.053646 dirigera-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-21 14:19:07.000000 dirigera-0.1.2/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-21 14:19:07.000000 dirigera-0.1.2/tests/test_light.py
```

### Comparing `dirigera-0.1.1/LICENSE` & `dirigera-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.1/PKG-INFO` & `dirigera-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.1
+Version: 0.1.2
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dirigera-0.1.1/README.md` & `dirigera-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.1/pyproject.toml` & `dirigera-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
    "setuptools",
    "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "0.1.1"
+version = "0.1.2"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = ["python", "iot", "smarthome", "hub", "lighting", "ikea", "tradfri", "dirigera"]
 dependencies = [
     "requests >= 2.22.0",
```

### Comparing `dirigera-0.1.1/src/dirigera/devices/environment_sensor.py` & `dirigera-0.1.2/src/dirigera/devices/environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.1/src/dirigera/devices/light.py` & `dirigera-0.1.2/src/dirigera/devices/light.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from ..hub.abstract_smart_home_hub import AbstractSmartHomeHub
 
 
 class StartupEnum(Enum):
     START_ON = "startOn"
     START_OFF = "startOff"
+    START_PREVIOUS = "startPrevious"
+    START_TOGGLE = "startToggle"
 
 
 @dataclass
 class Light(Device):
     dirigera_client: AbstractSmartHomeHub
     is_reachable: bool
     is_on: bool
@@ -105,14 +107,16 @@
         self.color_saturation = saturation
 
     def set_startup_behaviour(self, behaviour: StartupEnum) -> None:
         """
         Sets the behaviour of the lamp in case of a power outage.
         When set to START_ON the lamp will turn on once the power is back.
         When set to START_OFF the lamp will stay off once the power is back.
+        When set to START_PREVIOUS the lamp will resume its state at power outage.
+        When set to START_TOGGLE, a sequence of power-off -> power-on, will toggle the lamp state
         """
         data = [{"attributes": {"startupOnOff": behaviour}}]
         self.dirigera_client.patch(route=f"/devices/{self.device_id}", data=data)
         self.startup_on_off = behaviour
 
 
 def dict_to_light(data: dict[str, Any], dirigera_client: AbstractSmartHomeHub):
```

### Comparing `dirigera-0.1.1/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-0.1.2/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.1/src/dirigera/hub/auth.py` & `dirigera-0.1.2/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.1/src/dirigera/hub/hub.py` & `dirigera-0.1.2/src/dirigera/hub/hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.1/src/dirigera.egg-info/PKG-INFO` & `dirigera-0.1.2/src/dirigera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.1
+Version: 0.1.2
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dirigera-0.1.1/src/dirigera.egg-info/SOURCES.txt` & `dirigera-0.1.2/src/dirigera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.1/tests/test_environment_sensor.py` & `dirigera-0.1.2/tests/test_environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.1/tests/test_light.py` & `dirigera-0.1.2/tests/test_light.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,14 +115,33 @@
     behaviour = StartupEnum.START_ON
     fake_light.set_startup_behaviour(behaviour)
     action = fake_client.patch_actions.pop()
     assert action["route"] == f"/devices/{fake_light.device_id}"
     assert action["data"] == [{"attributes": {"startupOnOff": behaviour}}]
     assert fake_light.startup_on_off == behaviour
 
+def test_set_startup_behaviour_previous(
+    fake_light: Light, fake_client: FakeDirigeraHub
+) -> None:
+    behaviour = StartupEnum.START_PREVIOUS
+    fake_light.set_startup_behaviour(behaviour)
+    action = fake_client.patch_actions.pop()
+    assert action["route"] == f"/devices/{fake_light.device_id}"
+    assert action["data"] == [{"attributes": {"startupOnOff": behaviour}}]
+    assert fake_light.startup_on_off == behaviour
+
+def test_set_startup_behaviour_toggle(
+    fake_light: Light, fake_client: FakeDirigeraHub
+) -> None:
+    behaviour = StartupEnum.START_TOGGLE
+    fake_light.set_startup_behaviour(behaviour)
+    action = fake_client.patch_actions.pop()
+    assert action["route"] == f"/devices/{fake_light.device_id}"
+    assert action["data"] == [{"attributes": {"startupOnOff": behaviour}}]
+    assert fake_light.startup_on_off == behaviour
 
 def test_dict_to_light(fake_client: FakeDirigeraHub):
     data = {
         "id": "1237-343-2dfa",
         "type": "light",
         "deviceType": "light",
         "isReachable": True,
```

