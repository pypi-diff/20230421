# Comparing `tmp/pyworxcloud-3.1.3.tar.gz` & `tmp/pyworxcloud-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyworxcloud-3.1.3.tar", max compression
+gzip compressed data, was "pyworxcloud-3.1.4.tar", max compression
```

## Comparing `pyworxcloud-3.1.3.tar` & `pyworxcloud-3.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/LICENSE
--rw-r--r--   0        0        0      929 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/README.md
--rw-r--r--   0        0        0      610 2023-04-18 12:33:28.642206 pyworxcloud-3.1.3/pyproject.toml
--rw-r--r--   0        0        0    28714 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/__init__.py
--rw-r--r--   0        0        0     3751 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/api.py
--rw-r--r--   0        0        0     1134 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/clouds.py
--rw-r--r--   0        0        0      927 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/const.py
--rw-r--r--   0        0        0      204 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/day_map.py
--rw-r--r--   0        0        0     3647 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/events.py
--rw-r--r--   0        0        0     1826 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/exceptions.py
--rw-r--r--   0        0        0      204 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/helpers/__init__.py
--rw-r--r--   0        0        0      637 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/helpers/logger.py
--rw-r--r--   0        0        0     2794 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/helpers/time_format.py
--rw-r--r--   0        0        0      838 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/__init__.py
--rw-r--r--   0        0        0     3338 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/battery.py
--rw-r--r--   0        0        0     2091 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/blades.py
--rw-r--r--   0        0        0     1924 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/capability.py
--rw-r--r--   0        0        0     3609 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/devices.py
--rw-r--r--   0        0        0      617 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/firmware.py
--rw-r--r--   0        0        0      281 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/landroid_class.py
--rw-r--r--   0        0        0      306 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/lawn.py
--rw-r--r--   0        0        0      427 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/location.py
--rw-r--r--   0        0        0     8183 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/mqtt.py
--rw-r--r--   0        0        0      411 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/orientation.py
--rw-r--r--   0        0        0     1348 2023-04-18 12:33:17.161929 pyworxcloud-3.1.3/pyworxcloud/utils/product.py
--rw-r--r--   0        0        0     1109 2023-04-18 12:33:17.165929 pyworxcloud-3.1.3/pyworxcloud/utils/rainsensor.py
--rw-r--r--   0        0        0     2410 2023-04-18 12:33:17.165929 pyworxcloud-3.1.3/pyworxcloud/utils/requests.py
--rw-r--r--   0        0        0     6191 2023-04-18 12:33:17.165929 pyworxcloud-3.1.3/pyworxcloud/utils/schedules.py
--rw-r--r--   0        0        0     2050 2023-04-18 12:33:17.165929 pyworxcloud-3.1.3/pyworxcloud/utils/state.py
--rw-r--r--   0        0        0      657 2023-04-18 12:33:17.165929 pyworxcloud-3.1.3/pyworxcloud/utils/statistics.py
--rw-r--r--   0        0        0      726 2023-04-18 12:33:17.165929 pyworxcloud-3.1.3/pyworxcloud/utils/warranty.py
--rw-r--r--   0        0        0     1423 2023-04-18 12:33:17.165929 pyworxcloud-3.1.3/pyworxcloud/utils/zone.py
--rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 pyworxcloud-3.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/LICENSE
+-rw-r--r--   0        0        0      929 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/README.md
+-rw-r--r--   0        0        0      609 2023-04-21 12:28:09.086120 pyworxcloud-3.1.4/pyproject.toml
+-rw-r--r--   0        0        0    28713 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/__init__.py
+-rw-r--r--   0        0        0     4736 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/api.py
+-rw-r--r--   0        0        0     1134 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/clouds.py
+-rw-r--r--   0        0        0      927 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/const.py
+-rw-r--r--   0        0        0      204 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/day_map.py
+-rw-r--r--   0        0        0     3647 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/events.py
+-rw-r--r--   0        0        0     1918 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/exceptions.py
+-rw-r--r--   0        0        0      204 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/helpers/__init__.py
+-rw-r--r--   0        0        0      637 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/helpers/logger.py
+-rw-r--r--   0        0        0     2794 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/helpers/time_format.py
+-rw-r--r--   0        0        0      838 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/__init__.py
+-rw-r--r--   0        0        0     3338 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/battery.py
+-rw-r--r--   0        0        0     2091 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/blades.py
+-rw-r--r--   0        0        0     1924 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/capability.py
+-rw-r--r--   0        0        0     3619 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/devices.py
+-rw-r--r--   0        0        0      617 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/firmware.py
+-rw-r--r--   0        0        0      281 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/landroid_class.py
+-rw-r--r--   0        0        0      306 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/lawn.py
+-rw-r--r--   0        0        0      427 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/location.py
+-rw-r--r--   0        0        0     8183 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/mqtt.py
+-rw-r--r--   0        0        0      411 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/orientation.py
+-rw-r--r--   0        0        0     1348 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/product.py
+-rw-r--r--   0        0        0     1109 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/rainsensor.py
+-rw-r--r--   0        0        0     3188 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/requests.py
+-rw-r--r--   0        0        0     6191 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/schedules.py
+-rw-r--r--   0        0        0     2050 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/state.py
+-rw-r--r--   0        0        0      657 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/statistics.py
+-rw-r--r--   0        0        0      726 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/warranty.py
+-rw-r--r--   0        0        0     1423 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/zone.py
+-rw-r--r--   0        0        0     1747 1970-01-01 00:00:00.000000 pyworxcloud-3.1.4/PKG-INFO
```

### Comparing `pyworxcloud-3.1.3/LICENSE` & `pyworxcloud-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/README.md` & `pyworxcloud-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyproject.toml` & `pyworxcloud-3.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyworxcloud"
-version = "v3.1.3"
+version = "v3.1.4"
 description = "Landroid cloud (Positec) API library"
 authors = ["Malene Trab <malene@trab.dk>"]
 documentation = "https://github.com/mtrab/pyworxcloud"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/mtrab/pyworxcloud/issues"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 urllib3 = "^1.26.10"
 requests = "^2.26.0"
 paho-mqtt = "^1.6.1"
```

### Comparing `pyworxcloud-3.1.3/pyworxcloud/__init__.py` & `pyworxcloud-3.1.4/pyworxcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     Statistic,
     Weekdays,
 )
 from .utils.mqtt import Command
 from .utils.schedules import TYPE_TO_STRING
 
 if sys.version_info < (3, 9, 0):
-    sys.exit("The pyWorxcloud module requires Python 3.10.0 or later")
+    sys.exit("The pyWorxcloud module requires Python 3.9.0 or later")
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class WorxCloud(dict):
     """
     Worx by Landroid Cloud connector.
```

### Comparing `pyworxcloud-3.1.3/pyworxcloud/api.py` & `pyworxcloud-3.1.4/pyworxcloud/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -100,15 +100,44 @@
             str: JSON object containing available mowers associated with the account.
         """
         mowers = GET(
             f"https://{self.cloud.ENDPOINT}/api/v2/product-items?status=1",
             HEADERS(self.access_token),
         )
         for mower in mowers:
+            model = self.get_model(mower["product_id"])
+            mower["model"] = {
+                "code": model["code"],
+                "friendly_name": str.format(
+                    "{}{}", model["default_name"], model["meters"]
+                ),
+                "model_year": model["product_year"],
+                "cutting_width": model["cutting_width"],
+            }
             mower["firmware_version"] = "{:.2f}".format(mower["firmware_version"])
 
         return mowers
 
+    def get_model(self, product_id: int) -> str | None:
+        """Get model from product_id.
+
+        Returns:
+            str: JSON object containing detailed product information.
+            None: Returned when product_id couldn't be matched to a product.
+        """
+        products = GET(
+            f"https://{self.cloud.ENDPOINT}/api/v2/products",
+            HEADERS(self.access_token),
+        )
+
+        product_info = None
+        for product in products:
+            if product["id"] == product_id:
+                product_info = product
+                break
+
+        return product_info
+
     @property
     def data(self) -> str:
         """Return the latest dataset of information and states from the API."""
         return self.api_data
```

### Comparing `pyworxcloud-3.1.3/pyworxcloud/clouds.py` & `pyworxcloud-3.1.4/pyworxcloud/clouds.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/const.py` & `pyworxcloud-3.1.4/pyworxcloud/const.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/events.py` & `pyworxcloud-3.1.4/pyworxcloud/events.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/exceptions.py` & `pyworxcloud-3.1.4/pyworxcloud/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,7 +74,11 @@
 
 class APIError(Exception):
     """Error representing a generic API error."""
 
 
 class MowerNotFoundError(Exception):
     """Error raised when a specific requested mower was not found in the result."""
+
+
+class NoConnectionError(Exception):
+    """Raised when the endpoint cannot be reached."""
```

### Comparing `pyworxcloud-3.1.3/pyworxcloud/helpers/logger.py` & `pyworxcloud-3.1.4/pyworxcloud/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/helpers/time_format.py` & `pyworxcloud-3.1.4/pyworxcloud/helpers/time_format.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/__init__.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/battery.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/battery.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/blades.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/blades.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/capability.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/capability.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/devices.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,14 +104,16 @@
         self.in_topic = data["mqtt_topics"]["command_in"]
         self.out_topic = data["mqtt_topics"]["command_out"]
 
         if data in ["lawn_perimeter", "lawn_size"]:
             self.lawn = Lawn(data["lawn_perimeter"], data["lawn_size"])
 
         self.name = data["name"]
-        self.model = "Model info not available in API"  # f"{self.chassis.default_name}{self.chassis.meters}"
+        self.model = str.format(
+            "{} ({})", data["model"]["friendly_name"], data["model"]["code"]
+        )
 
         for attr in UNWANTED_ATTRIBS:
             if hasattr(self, attr):
                 delattr(self, attr)
 
         self.is_decoded = True
```

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/firmware.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/firmware.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/mqtt.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/product.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/product.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/rainsensor.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/rainsensor.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/requests.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/requests.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 """For handling HTTP/HTTPS requests."""
 from __future__ import annotations
 
+from time import sleep
+
 import requests
 
 from ..exceptions import (
     APIError,
     AuthorizationError,
     ForbiddenError,
     InternalServerError,
+    NoConnectionError,
     NotFoundError,
     RequestError,
     ServiceUnavailableError,
     TooManyRequestsError,
 )
 
 # pylint: disable=invalid-name
 
+NUM_RETRIES = 5
+MAX_BACKOFF = 120
+BACKOFF_FACTOR = 3
+
+
+def backoff(retry: int) -> float:
+    """Calculate backoff time."""
+    val: float = BACKOFF_FACTOR * (2 ** (retry - 1))
+
+    return val if val <= MAX_BACKOFF else MAX_BACKOFF
+
 
 def HEADERS(access_token: str | None = None) -> dict:
     """Generate headers dictionary."""
     head = {
         "Accept": "application/json",
     }
 
@@ -29,65 +43,78 @@
         head.update({"Authorization": f"Bearer {access_token}"})
 
     return head
 
 
 def POST(URL: str, REQUEST_BODY: str, HEADER: dict | None = None) -> str:
     """A request POST"""
+
     if isinstance(HEADER, type(None)):
         HEADER = HEADERS()
 
-    try:
-        req = requests.post(URL, REQUEST_BODY, headers=HEADER)
+    for retry in range(NUM_RETRIES):
+        try:
+            req = requests.post(URL, REQUEST_BODY, headers=HEADER)
+
+            req.raise_for_status()
+
+            return req.json()
+        except requests.exceptions.HTTPError as err:
+            code = err.response.status_code
+            if code == 400:
+                raise RequestError()
+            elif code == 401:
+                raise AuthorizationError()
+            elif code == 403:
+                raise ForbiddenError()
+            elif code == 404:
+                raise NotFoundError()
+            elif code == 429:
+                raise TooManyRequestsError()
+            elif code == 500:
+                raise InternalServerError()
+            elif code == 503:
+                raise ServiceUnavailableError()
+            elif code == 504:
+                sleep(backoff(retry))
+                pass
+            else:
+                raise APIError(err)
 
-        req.raise_for_status()
-    except requests.exceptions.HTTPError as err:
-        code = err.response.status_code
-        if code == 400:
-            raise RequestError()
-        elif code == 401:
-            raise AuthorizationError()
-        elif code == 403:
-            raise ForbiddenError()
-        elif code == 404:
-            raise NotFoundError()
-        elif code == 429:
-            raise TooManyRequestsError()
-        elif code == 500:
-            raise InternalServerError()
-        elif code == 503:
-            raise ServiceUnavailableError()
-        else:
-            raise APIError(err)
-
-    return req.json()
+    raise NoConnectionError()
 
 
 def GET(URL: str, HEADER: dict | None = None) -> str:
     """A request GET"""
     if isinstance(HEADER, type(None)):
         HEADER = HEADERS()
 
-    try:
-        req = requests.get(URL, headers=HEADER)
-
-        req.raise_for_status()
-    except requests.exceptions.HTTPError as err:
-        code = err.response.status_code
-        if code == 400:
-            raise RequestError()
-        elif code == 401:
-            raise AuthorizationError()
-        elif code == 403:
-            raise ForbiddenError()
-        elif code == 404:
-            raise NotFoundError()
-        elif code == 429:
-            raise TooManyRequestsError()
-        elif code == 500:
-            raise InternalServerError()
-        elif code == 503:
-            raise ServiceUnavailableError()
-        else:
-            raise APIError(err)
+    for retry in range(NUM_RETRIES):
+        try:
+            req = requests.get(URL, headers=HEADER)
+
+            req.raise_for_status()
+
+            return req.json()
+        except requests.exceptions.HTTPError as err:
+            code = err.response.status_code
+            if code == 400:
+                raise RequestError()
+            elif code == 401:
+                raise AuthorizationError()
+            elif code == 403:
+                raise ForbiddenError()
+            elif code == 404:
+                raise NotFoundError()
+            elif code == 429:
+                raise TooManyRequestsError()
+            elif code == 500:
+                raise InternalServerError()
+            elif code == 503:
+                raise ServiceUnavailableError()
+            elif code == 504:
+                sleep(backoff(retry))
+                pass
+            else:
+                raise APIError(err)
 
-    return req.json()
+    raise NoConnectionError()
```

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/schedules.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/schedules.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/state.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/state.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/statistics.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/warranty.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/warranty.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/pyworxcloud/utils/zone.py` & `pyworxcloud-3.1.4/pyworxcloud/utils/zone.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.3/PKG-INFO` & `pyworxcloud-3.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pyworxcloud
-Version: 3.1.3
+Version: 3.1.4
 Summary: Landroid cloud (Positec) API library
 License: MIT
 Author: Malene Trab
 Author-email: malene@trab.dk
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.10,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/mtrab/pyworxcloud/issues
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.3 Summary: Landroid cloud
+Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.4 Summary: Landroid cloud
 (Positec) API library License: MIT Author: Malene Trab Author-email:
-malene@trab.dk Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved
+malene@trab.dk Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0) Requires-Dist: requests
-(>=2.26.0,<3.0.0) Requires-Dist: urllib3 (>=1.26.10,<2.0.0) Project-URL: Bug
-Tracker, https://github.com/mtrab/pyworxcloud/issues Project-URL:
-Documentation, https://github.com/mtrab/pyworxcloud Description-Content-Type:
-text/markdown [Buy_Me_A_Coffee] # pyWorxCloud This is a PyPI module for
-communicating with Worx Cloud mowers, primarily developed for use with [Home
-Assistant](https://home-assistant.io), but I try to keep it as widely usable as
-possible.
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Requires-Dist:
+paho-mqtt (>=1.6.1,<2.0.0) Requires-Dist: requests (>=2.26.0,<3.0.0) Requires-
+Dist: urllib3 (>=1.26.10,<2.0.0) Project-URL: Bug Tracker, https://github.com/
+mtrab/pyworxcloud/issues Project-URL: Documentation, https://github.com/mtrab/
+pyworxcloud Description-Content-Type: text/markdown [Buy_Me_A_Coffee] #
+pyWorxCloud This is a PyPI module for communicating with Worx Cloud mowers,
+primarily developed for use with [Home Assistant](https://home-assistant.io),
+but I try to keep it as widely usable as possible.
 
 The module are compatible with cloud enabled devices from [these vendors]
 (https://github.com/MTrab/pyworxcloud/wiki#current-supported-brands--vendors)
 ## Documentation The documentation have been moved to the [Wiki](https://
 github.com/MTrab/pyworxcloud/wiki)
 This is unfortunately a little out-of-date due to the huge changes in version
 3.
```

