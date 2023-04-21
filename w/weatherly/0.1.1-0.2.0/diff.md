# Comparing `tmp/weatherly-0.1.1-py3.11.egg` & `tmp/weatherly-0.2.0-py3.11.egg`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 35446 bytes, number of entries: 24
--rw-rw-rw-  2.0 fat     2206 b- defN 23-Apr-17 18:33 EGG-INFO/PKG-INFO
--rw-rw-rw-  2.0 fat      383 b- defN 23-Apr-17 18:33 EGG-INFO/SOURCES.txt
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-17 18:33 EGG-INFO/dependency_links.txt
--rw-rw-rw-  2.0 fat       39 b- defN 23-Apr-17 18:33 EGG-INFO/requires.txt
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-17 18:33 EGG-INFO/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-17 18:33 EGG-INFO/zip-safe
--rw-rw-rw-  2.0 fat      811 b- defN 23-Apr-17 18:32 weatherly/__init__.py
--rw-rw-rw-  2.0 fat     4046 b- defN 23-Apr-17 09:10 weatherly/abc.py
+Zip file size: 40223 bytes, number of entries: 24
+-rw-rw-rw-  2.0 fat     3022 b- defN 23-Apr-21 08:50 EGG-INFO/PKG-INFO
+-rw-rw-rw-  2.0 fat      383 b- defN 23-Apr-21 08:50 EGG-INFO/SOURCES.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-21 08:50 EGG-INFO/dependency_links.txt
+-rw-rw-rw-  2.0 fat       39 b- defN 23-Apr-21 08:50 EGG-INFO/requires.txt
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-21 08:50 EGG-INFO/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-21 08:50 EGG-INFO/zip-safe
+-rw-rw-rw-  2.0 fat      813 b- defN 23-Apr-21 08:47 weatherly/__init__.py
+-rw-rw-rw-  2.0 fat     5297 b- defN 23-Apr-21 08:27 weatherly/abc.py
 -rw-rw-rw-  2.0 fat     4647 b- defN 23-Apr-17 09:10 weatherly/enums.py
--rw-rw-rw-  2.0 fat     3871 b- defN 23-Apr-17 09:10 weatherly/errors.py
--rw-rw-rw-  2.0 fat     4487 b- defN 23-Apr-17 09:19 weatherly/responses.py
--rw-rw-rw-  2.0 fat     2640 b- defN 23-Apr-17 09:10 weatherly/utils.py
--rw-rw-rw-  2.0 fat     1354 b- defN 23-Apr-17 18:33 weatherly/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-  2.0 fat     4932 b- defN 23-Apr-17 18:33 weatherly/__pycache__/abc.cpython-311.pyc
--rw-rw-rw-  2.0 fat     5906 b- defN 23-Apr-17 18:33 weatherly/__pycache__/enums.cpython-311.pyc
--rw-rw-rw-  2.0 fat     5266 b- defN 23-Apr-17 18:33 weatherly/__pycache__/errors.cpython-311.pyc
--rw-rw-rw-  2.0 fat     5506 b- defN 23-Apr-17 18:33 weatherly/__pycache__/responses.cpython-311.pyc
--rw-rw-rw-  2.0 fat     3316 b- defN 23-Apr-17 18:33 weatherly/__pycache__/utils.cpython-311.pyc
+-rw-rw-rw-  2.0 fat     3854 b- defN 23-Apr-21 08:18 weatherly/errors.py
+-rw-rw-rw-  2.0 fat     6809 b- defN 23-Apr-21 08:25 weatherly/responses.py
+-rw-rw-rw-  2.0 fat     2855 b- defN 23-Apr-21 08:41 weatherly/utils.py
+-rw-rw-rw-  2.0 fat     1359 b- defN 23-Apr-21 08:50 weatherly/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-  2.0 fat     6514 b- defN 23-Apr-21 08:50 weatherly/__pycache__/abc.cpython-311.pyc
+-rw-rw-rw-  2.0 fat     5906 b- defN 23-Apr-21 08:50 weatherly/__pycache__/enums.cpython-311.pyc
+-rw-rw-rw-  2.0 fat     5249 b- defN 23-Apr-21 08:50 weatherly/__pycache__/errors.cpython-311.pyc
+-rw-rw-rw-  2.0 fat     8392 b- defN 23-Apr-21 08:50 weatherly/__pycache__/responses.cpython-311.pyc
+-rw-rw-rw-  2.0 fat     3648 b- defN 23-Apr-21 08:50 weatherly/__pycache__/utils.cpython-311.pyc
 -rw-rw-rw-  2.0 fat     1258 b- defN 23-Apr-17 09:10 weatherly/api/__init__.py
--rw-rw-rw-  2.0 fat     6410 b- defN 23-Apr-17 09:10 weatherly/api/client.py
--rw-rw-rw-  2.0 fat     2732 b- defN 23-Apr-17 09:10 weatherly/api/core.py
--rw-rw-rw-  2.0 fat     1419 b- defN 23-Apr-17 18:33 weatherly/api/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-  2.0 fat     7812 b- defN 23-Apr-17 18:33 weatherly/api/__pycache__/client.cpython-311.pyc
--rw-rw-rw-  2.0 fat     3641 b- defN 23-Apr-17 18:33 weatherly/api/__pycache__/core.cpython-311.pyc
-24 files, 72695 bytes uncompressed, 32166 bytes compressed:  55.8%
+-rw-rw-rw-  2.0 fat     9793 b- defN 23-Apr-21 08:45 weatherly/api/client.py
+-rw-rw-rw-  2.0 fat     2752 b- defN 23-Apr-21 08:18 weatherly/api/core.py
+-rw-rw-rw-  2.0 fat     1419 b- defN 23-Apr-21 08:50 weatherly/api/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-  2.0 fat    11907 b- defN 23-Apr-21 08:50 weatherly/api/__pycache__/client.cpython-311.pyc
+-rw-rw-rw-  2.0 fat     3661 b- defN 23-Apr-21 08:50 weatherly/api/__pycache__/core.cpython-311.pyc
+24 files, 89590 bytes uncompressed, 36943 bytes compressed:  58.8%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: weatherly
-Version: 0.1.1
-Summary: A Python wrapper for the Discord API
+Version: 0.2.0
+Summary: A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...
 Home-page: https://github.com/konradsic/weatherly
 Author: konradsic
 License: MIT
 Project-URL: Issues, https://github.com/konradsic/weatherly/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -22,14 +22,27 @@
 Requires-Python: >=3.10.0
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 License-File: LICENSE
 
 ⛅ weatherly
 ====================
+.. image:: https://img.shields.io/github/license/konradsic/weatherly?color=blue&style=for-the-badge
+    :target: https://github.com/konradsic/weatherly/blob/master/LICENSE
+    :alt: Weatherly license
+.. image:: https://img.shields.io/pypi/v/weatherly?color=blue&style=for-the-badge
+    :target: https://pypi.python.org/project/weatherly
+    :alt: Weatherly version on PyPI
+.. image:: https://img.shields.io/pypi/pyversions/weatherly?color=blue&style=for-the-badge
+    :target: https://pypi.python.org/project/weatherly
+    :alt: Supported Python versions
+.. image:: https://img.shields.io/github/actions/workflow/status/konradsic/weatherly/build.yml?style=for-the-badge
+    :target: https://github.com/konradsic/weatherly
+    :alt: Build status
+
 Weatherly is a simple package that retrieves weather data from WeatherAPI.com. It provides an easy to use interface to access current and historical weather data for a specific location.
 
 📜 Features
 ---------------
 * Easy to use,
 * Intuitive design,
 * Can provide current weather data aswell as forecast, historical data, future predictions and even more!
```

## weatherly/__init__.py

```diff
@@ -7,15 +7,15 @@
 :license: MIT license, see LICENSE for details
 """
 
 __title__ = 'weatherly'
 __author__ = 'konradsic'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023-present konradsic'
-__version__ = '0.1.1'
+__version__ = '0.2.0'
 
 from typing import NamedTuple, Literal
 
 from .api import *
 from .errors import *
 from .enums import *
 from .responses import *
@@ -25,11 +25,11 @@
 
 class VersionInfo(NamedTuple):
     major: int
     minor: int
     micro: int
     release_type: Literal["alpha", "beta", "pre", "final"]
     
-version_info = VersionInfo(major=0, minor=1, micro=1, release_type="final")
+version_info = VersionInfo(major=0, minor=2, micro=0, release_type="final")
 
 
-del NamedTuple, Literal, VersionInfo
+del NamedTuple, Literal, VersionInfo
```

## weatherly/abc.py

```diff
@@ -22,14 +22,15 @@
 SOFTWARE.
 """
 
 from typing import (
     Any,
     Literal,
     Dict,
+    Optional
 )
 from abc import ABC
 
 __all__ = (
     "ResponseModel",
     "CurrentWeather",
 )
@@ -56,15 +57,17 @@
     """
     An ABC defining current weather data.
 
     The following classes implement this ABC:
     - :class:`~weatherly.CurrentWeatherData`
 
     Attributes
-    ----------
+    ------------
+    location: :class:`~weatherly.LocationData`
+        Location of the requested weather data
     last_updated_epoch: :class:`int`
         The timestamp when the weather data was last updated.
     temp_c: :class:`float`
         Weather temperature in Celsius
     temp_f: :class:`float`
         Weather temperature in Fahrenheit
     is_day: :class:`bool`
@@ -118,7 +121,41 @@
     precip_mm: float
     precip_in: float
     humidity: int
     cloud: int
     feelslike_c: float
     feelslike_f: float
     uv: float
+
+class LocationModel(ResponseModel):
+    """An ABC that provides information about a location
+
+    Attributes
+    --------------
+    id: :class:`int`
+        A specific ID of the location. Can be ``None``
+    name: :class:`str`
+        Name of the location (e.g. London)
+    region: :class:`str`
+        A region of the location
+    country: :class:`str`
+        Country where the location is
+    latitude: :class:`float`
+        Latitude coordinate of the location
+    longitude: :class:`float`
+        Longitude coordinate of the location
+    timezone_id: Optional[:class:`str`]
+        Timezone ID of the location (e.g. Europe/London). Could be ``None`` when using the Search/Autocomplete API.
+    localtime_epoch: Optional[:class:`int`]
+        Local time of the location as a timestamp
+    localtime_formatted: Optional[:class:`str`]
+        Formatted local time of the location
+    """
+    id: Optional[int]
+    name: str
+    region: str
+    country: str
+    latitude: float
+    longitude: float
+    timezone_id: Optional[str]
+    localtime_epoch: Optional[int]
+    localtime_formatted: Optional[str]
```

## weatherly/errors.py

```diff
@@ -61,62 +61,62 @@
         self.formatted_message = f"{self.status} (error code {self.code}): {message}"
         super().__init__(self.formatted_message, *args)
 
 class NoLocationFound(WeatherAPIException): 
     """
     Exception like this is raised when no location was found when searching for weather data.
 
-    Usually has status code of 400 and error code 1006.
+    Usually has status code  400 and error code 1006.
     
     Inherits from :class:`WeatherAPIException`.
     """
     pass
 
 class InvalidAPIKey(WeatherAPIException): 
     """
     Exception like this is raised when provided API key is invalid
 
-    Usually has status code of 401 and error code 2006.
+    Usually has status code 401 and error code 2006.
     
     Inherits from :class:`WeatherAPIException`.
     """
     pass
 
 class APILimitExceeded(WeatherAPIException): 
     """
     Exception like this is raised when API key has exceeded monthly calls limit.
 
-    Usually has status code of 400 and error code 2007.
+    Usually has status code 400 and error code 2007.
     
     Inherits from :class:`WeatherAPIException`.
     """
     pass
 
 class APIKeyDisabled(WeatherAPIException): 
     """
     Exception like this is raised when API key has been disabled.
 
-    Usually has status code of 403 and error code 2008.
+    Usually has status code 403 and error code 2008.
     
     Inherits from :class:`WeatherAPIException`.
     """
     pass
 
 class AccessDenied(WeatherAPIException): 
     """
     Exception like this is raised when API key does not have access to requested resource.
 
-    Usually has status code of 403 and error code 2009.
+    Usually has status code 403 and error code 2009.
     
     Inherits from :class:`WeatherAPIException`.
     """
     pass
 
 class InternalApplicationError(WeatherAPIException): 
     """
     Exception like this is raised when an internal application error occured. There is nothing to do about it.
 
-    Usually has status code of 400 and error code 9999.
+    Usually has status code 400 and error code 9999.
     
     Inherits from :class:`WeatherAPIException`.
     """
     pass
```

## weatherly/responses.py

```diff
@@ -18,35 +18,45 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-from .abc import CurrentWeather
+from .abc import CurrentWeather, LocationModel
 from typing import (
     Dict,
     Any,
     Union
 )
 
+__all__ = (
+    "CurrentWeatherData",
+    "LocationData",
+)
+
 class CurrentWeatherData(CurrentWeather):
     """
     Current weather data, a common return type from methods that requests this from WeatherAPI.com.
     
     Please note, that only ``condition_text`` is translated into requested language.
+    
+    .. note::
+        This class should not be created manually, instead it will be returned from methods like ``get_current_weather`` of the :class:`WeatherAPIClient` class.
 
     Attributes
     ----------
     raw: Dict[:class:`str`, Any]
         Raw response in a JSON-like format (converted to a python dictionary)
     status: :class:`int`
         HTTP status of the response. 200 is OK, and is the most common status.
     code: Union[:class:`int`, None]
         Response code. In some cases this can be ``None``
+    location: :class:`LocationData`
+        Location of the requested weather data
     last_updated_epoch: :class:`int`
         The timestamp when the weather data was last updated.
     temp_c: :class:`float`
         Weather temperature in Celsius
     temp_f: :class:`float`
         Weather temperature in Fahrenheit
     is_day: :class:`bool`
@@ -91,14 +101,18 @@
         code: Union[int, None]
     ) -> None:
         super().__init__()
         
         self.status = status
         self.code = code
         self.raw = raw
+        
+        self.location = LocationData(raw["location"], status, code)
+        raw = raw["current"]
+        
         self.last_updated_epoch = raw["last_updated_epoch"]
         self.temp_c = raw["temp_c"]
         self.temp_f = raw["temp_f"]
         self.is_day = bool(raw["is_day"])
         self.condition_text = raw["condition"]["text"]
         self.condition_icon = raw["condition"]["icon"]
         self.condition_code = raw["condition"]["code"]
@@ -111,7 +125,58 @@
         self.precip_mm = raw["precip_mm"]
         self.precip_in = raw["precip_in"]
         self.humidity = raw["humidity"]
         self.cloud = raw["cloud"]
         self.feelslike_c = raw["feelslike_c"]
         self.feelslike_f = raw["feelslike_f"]
         self.uv = raw["uv"]
+
+class LocationData(LocationModel):
+    """
+    Location data, returned with most requests.
+    
+    Attributes
+    --------------
+    raw: Dict[:class:`str`, Any]
+        Raw response in a JSON-like format (converted to a python dictionary)
+    status: :class:`int`
+        HTTP status of the response. 200 is OK, and is the most common status.
+    code: Union[:class:`int`, None]
+        Response code. In some cases this can be ``None``
+    id: Optional[:class:`int`]
+        A specific ID of the location. Can be ``None``
+    name: :class:`str`
+        Name of the location (e.g. London)
+    region: :class:`str`
+        A region of the location
+    country: :class:`str`
+        Country where the location is
+    latitude: :class:`float`
+        Latitude coordinate of the location
+    longitude: :class:`float`
+        Longitude coordinate of the location
+    timezone_id: Optional[:class:`str`]
+        Timezone ID of the location (e.g. Europe/London). Could be ``None`` when using the Search/Autocomplete API.
+    localtime_epoch: Optional[:class:`int`]
+        Local time of the location as a timestamp
+    localtime_formatted: Optional[:class:`str`]
+        Formatted local time of the location
+    """
+    def __init__(
+        self, 
+        raw: Dict[str, Any],
+        status: int,
+        code: Union[int, None]
+    ) -> None:
+        self.raw = raw
+        self.status = status
+        self.code = code
+
+        self.id = raw.get('id', None)
+        self.name = raw['name']
+        self.region = raw['region']
+        self.country = raw['country']
+        self.latitude = raw['lat']
+        self.longitude = raw['lon']
+        self.timezone_id = raw.get('tz_id', None)
+        self.localtime_epoch = raw.get('localtime_epoch')
+        self.localtime_formatted = raw.get('localtime', None)
```

## weatherly/utils.py

```diff
@@ -51,40 +51,44 @@
     
     for k,v in kwargs.items():
         args_string += f"{'?' if first else '&'}{k}={v}"
         first = False
     return args_string
 
 @overload
-def find_language(lang: str) -> None:
+def find_language(lang: str, asobj: bool=False) -> None:
+    ...
+    
+@overload
+def find_language(lang: str, asobj: bool=False) -> Languages:
     ...
 
-def find_language(lang: str) -> str:
+def find_language(lang: str, asobj: bool=False) -> str:
     """
     Used to find language code from available languages.
 
     Paremeters
     ----------
     lang: :class:`str`
         A language you want to search for
 
     Returns
     -------
-    Union[:class:`str`, None]
-        Language code, could be ``None``
+    Union[:class:`str`, :class:`Languages`, None]
+        Language code, could be ``None``, could be a :class:`Languages` enum.
     """
-    lang_code = None
 
     if isinstance(lang, Languages):
         try:
+            if asobj: return lang
             return lang.value
         except: 
             return None
 
     lang = lang.lower()
 
     for language in Languages:
         if language.name.lower() == lang or language.value == lang:
-            lang_code = lang.value
-            break
-    
-    return lang_code
+            if asobj: return language
+            return language.value
+        
+    return None
```

## weatherly/__pycache__/__init__.cpython-311.pyc

### Python bytecode

```diff
@@ -1,22 +1,22 @@
 magic:    0xa70d0d0a
-moddate:  0x8a743d64 (Mon Apr 17 16:32:10 2023 UTC)
-files sz: 811
+moddate:  0x65314264 (Fri Apr 21 06:47:01 2023 UTC)
+files sz: 813
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x970064005a0064015a0164025a0264035a0364045a0464055a05640664
       076c066d075a076d085a080100640864096c095400640864096c0a540064
       0864096c0b5400640864096c0c54006408640a6c0d6d0e5a0e0100020047
       00640b8400640c6507a6030000ab0300000000000000005a0f0200650f64
-      0664086408640dac0ea6040000ab0400000000000000005a105b075b085b
-      0f640f5300
+      06640d6406640eac0fa6040000ab0400000000000000005a105b075b085b
+      0f64105300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('\nweatherly\n===============\nA simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more.\n\n:copyright: (c) 2023-present @konradsic\n:license: MIT license, see LICENSE for details\n')
                  4 STORE_NAME               0 (__doc__)
    
     10           6 LOAD_CONST               1 ('weatherly')
                  8 STORE_NAME               1 (__title__)
@@ -26,15 +26,15 @@
    
     12          14 LOAD_CONST               3 ('MIT')
                 16 STORE_NAME               3 (__license__)
    
     13          18 LOAD_CONST               4 ('Copyright 2023-present konradsic')
                 20 STORE_NAME               4 (__copyright__)
    
-    14          22 LOAD_CONST               5 ('0.1.1')
+    14          22 LOAD_CONST               5 ('0.2.0')
                 24 STORE_NAME               5 (__version__)
    
     16          26 LOAD_CONST               6 (0)
                 28 LOAD_CONST               7 (('NamedTuple', 'Literal'))
                 30 IMPORT_NAME              6 (typing)
                 32 IMPORT_FROM              7 (NamedTuple)
                 34 STORE_NAME               7 (NamedTuple)
@@ -78,34 +78,34 @@
                 98 PRECALL                  3
                102 CALL                     3
                112 STORE_NAME              15 (VersionInfo)
    
     32         114 PUSH_NULL
                116 LOAD_NAME               15 (VersionInfo)
                118 LOAD_CONST               6 (0)
-               120 LOAD_CONST               8 (1)
-               122 LOAD_CONST               8 (1)
-               124 LOAD_CONST              13 ('final')
-               126 KW_NAMES                14
+               120 LOAD_CONST              13 (2)
+               122 LOAD_CONST               6 (0)
+               124 LOAD_CONST              14 ('final')
+               126 KW_NAMES                15
                128 PRECALL                  4
                132 CALL                     4
                142 STORE_NAME              16 (version_info)
    
     35         144 DELETE_NAME              7 (NamedTuple)
                146 DELETE_NAME              8 (Literal)
                148 DELETE_NAME             15 (VersionInfo)
-               150 LOAD_CONST              15 (None)
+               150 LOAD_CONST              16 (None)
                152 RETURN_VALUE
    consts
       '\nweatherly\n===============\nA simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more.\n\n:copyright: (c) 2023-present @konradsic\n:license: MIT license, see LICENSE for details\n'
       'weatherly'
       'konradsic'
       'MIT'
       'Copyright 2023-present konradsic'
-      '0.1.1'
+      '0.2.0'
       0
       ('NamedTuple', 'Literal')
       1
       ('*',)
       ('utils',)
       code
          argcount  : 0
@@ -159,14 +159,15 @@
          freevars   ()
          cellvars   ()
          filename   'build\\bdist.win-amd64\\egg\\weatherly\\__init__.py'
          name       'VersionInfo'
          firstlineno 26
          lnotab 0x0c010a010a010a01
       'VersionInfo'
+      2
       'final'
       ('major', 'minor', 'micro', 'release_type')
       None
    names      ('__doc__', '__title__', '__author__', '__license__', '__copyright__', '__version__', 'typing', 'NamedTuple', 'Literal', 'api', 'errors', 'enums', 'responses', '', 'utils', 'VersionInfo', 'version_info')
    varnames   ()
    freevars   ()
    cellvars   ()
```

## weatherly/__pycache__/abc.cpython-311.pyc

### Python bytecode

```diff
@@ -1,107 +1,120 @@
 magic:    0xa70d0d0a
-moddate:  0xdaf03c64 (Mon Apr 17 07:10:18 2023 UTC)
-files sz: 4046
+moddate:  0xcf2c4264 (Fri Apr 21 06:27:27 2023 UTC)
+files sz: 5297
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x970064005a00640164026c016d025a026d035a036d045a040100640164
-      036c056d065a06010064045a07020047006405840064066506a6030000ab
-      0300000000000000005a08020047006407840064086508a6030000ab0300
-      000000000000005a0964095300
+      0x970064005a00640164026c016d025a026d035a036d045a046d055a0501
+      00640164036c066d075a07010064045a08020047006405840064066507a6
+      030000ab0300000000000000005a09020047006407840064086509a60300
+      00ab0300000000000000005a0a0200470064098400640a6509a6030000ab
+      0300000000000000005a0b640b5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('\nMIT License\n\nCopyright (c) 2023 Konrad (@konradsic)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n')
                  4 STORE_NAME               0 (__doc__)
    
     25           6 LOAD_CONST               1 (0)
-                 8 LOAD_CONST               2 (('Any', 'Literal', 'Dict'))
+                 8 LOAD_CONST               2 (('Any', 'Literal', 'Dict', 'Optional'))
                 10 IMPORT_NAME              1 (typing)
                 12 IMPORT_FROM              2 (Any)
                 14 STORE_NAME               2 (Any)
                 16 IMPORT_FROM              3 (Literal)
                 18 STORE_NAME               3 (Literal)
                 20 IMPORT_FROM              4 (Dict)
                 22 STORE_NAME               4 (Dict)
-                24 POP_TOP
+                24 IMPORT_FROM              5 (Optional)
+                26 STORE_NAME               5 (Optional)
+                28 POP_TOP
    
-    30          26 LOAD_CONST               1 (0)
-                28 LOAD_CONST               3 (('ABC',))
-                30 IMPORT_NAME              5 (abc)
-                32 IMPORT_FROM              6 (ABC)
-                34 STORE_NAME               6 (ABC)
-                36 POP_TOP
+    31          30 LOAD_CONST               1 (0)
+                32 LOAD_CONST               3 (('ABC',))
+                34 IMPORT_NAME              6 (abc)
+                36 IMPORT_FROM              7 (ABC)
+                38 STORE_NAME               7 (ABC)
+                40 POP_TOP
    
-    32          38 LOAD_CONST               4 (('ResponseModel', 'CurrentWeather'))
-                40 STORE_NAME               7 (__all__)
+    33          42 LOAD_CONST               4 (('ResponseModel', 'CurrentWeather'))
+                44 STORE_NAME               8 (__all__)
    
-    37          42 PUSH_NULL
-                44 LOAD_BUILD_CLASS
-                46 LOAD_CONST               5 (<code object ResponseModel, file "build\bdist.win-amd64\egg\weatherly\abc.py", line 37>)
-                48 MAKE_FUNCTION            0
-                50 LOAD_CONST               6 ('ResponseModel')
-                52 LOAD_NAME                6 (ABC)
-                54 PRECALL                  3
-                58 CALL                     3
-                68 STORE_NAME               8 (ResponseModel)
+    38          46 PUSH_NULL
+                48 LOAD_BUILD_CLASS
+                50 LOAD_CONST               5 (<code object ResponseModel, file "build\bdist.win-amd64\egg\weatherly\abc.py", line 38>)
+                52 MAKE_FUNCTION            0
+                54 LOAD_CONST               6 ('ResponseModel')
+                56 LOAD_NAME                7 (ABC)
+                58 PRECALL                  3
+                62 CALL                     3
+                72 STORE_NAME               9 (ResponseModel)
    
-    55          70 PUSH_NULL
-                72 LOAD_BUILD_CLASS
-                74 LOAD_CONST               7 (<code object CurrentWeather, file "build\bdist.win-amd64\egg\weatherly\abc.py", line 55>)
-                76 MAKE_FUNCTION            0
-                78 LOAD_CONST               8 ('CurrentWeather')
-                80 LOAD_NAME                8 (ResponseModel)
-                82 PRECALL                  3
-                86 CALL                     3
-                96 STORE_NAME               9 (CurrentWeather)
-                98 LOAD_CONST               9 (None)
-               100 RETURN_VALUE
+    56          74 PUSH_NULL
+                76 LOAD_BUILD_CLASS
+                78 LOAD_CONST               7 (<code object CurrentWeather, file "build\bdist.win-amd64\egg\weatherly\abc.py", line 56>)
+                80 MAKE_FUNCTION            0
+                82 LOAD_CONST               8 ('CurrentWeather')
+                84 LOAD_NAME                9 (ResponseModel)
+                86 PRECALL                  3
+                90 CALL                     3
+               100 STORE_NAME              10 (CurrentWeather)
+   
+   129         102 PUSH_NULL
+               104 LOAD_BUILD_CLASS
+               106 LOAD_CONST               9 (<code object LocationModel, file "build\bdist.win-amd64\egg\weatherly\abc.py", line 129>)
+               108 MAKE_FUNCTION            0
+               110 LOAD_CONST              10 ('LocationModel')
+               112 LOAD_NAME                9 (ResponseModel)
+               114 PRECALL                  3
+               118 CALL                     3
+               128 STORE_NAME              11 (LocationModel)
+               130 LOAD_CONST              11 (None)
+               132 RETURN_VALUE
    consts
       '\nMIT License\n\nCopyright (c) 2023 Konrad (@konradsic)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n'
       0
-      ('Any', 'Literal', 'Dict')
+      ('Any', 'Literal', 'Dict', 'Optional')
       ('ABC',)
       ('ResponseModel', 'CurrentWeather')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a02550064015a0365046505650666021900000000
             0000000000650764023c0000006508650764033c000000650864047a0700
             00650764053c00000064045300
-          37           0 RESUME                   0
+          38           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ResponseModel')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          38          12 LOAD_CONST               1 ('\n    ResponseModel is an ABC that defines a basic response model from WeatherAPI.\n    Almost all models inherit from this class.\n    \n    Attributes\n    ----------\n    raw: Dict[:class:`str`, Any]\n        Raw response in a JSON-like format (converted to a python dictionary)\n    status: :class:`int`\n        HTTP status of the response. 200 is OK, and is the most common status.\n    code: Union[:class:`int`, None]\n        Response code. In some cases this can be ``None``\n    ')
+          39          12 LOAD_CONST               1 ('\n    ResponseModel is an ABC that defines a basic response model from WeatherAPI.\n    Almost all models inherit from this class.\n    \n    Attributes\n    ----------\n    raw: Dict[:class:`str`, Any]\n        Raw response in a JSON-like format (converted to a python dictionary)\n    status: :class:`int`\n        HTTP status of the response. 200 is OK, and is the most common status.\n    code: Union[:class:`int`, None]\n        Response code. In some cases this can be ``None``\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-          51          16 LOAD_NAME                4 (Dict)
+          52          16 LOAD_NAME                4 (Dict)
                       18 LOAD_NAME                5 (str)
                       20 LOAD_NAME                6 (Any)
                       22 BUILD_TUPLE              2
                       24 BINARY_SUBSCR
                       34 LOAD_NAME                7 (__annotations__)
                       36 LOAD_CONST               2 ('raw')
                       38 STORE_SUBSCR
          
-          52          42 LOAD_NAME                8 (int)
+          53          42 LOAD_NAME                8 (int)
                       44 LOAD_NAME                7 (__annotations__)
                       46 LOAD_CONST               3 ('status')
                       48 STORE_SUBSCR
          
-          53          52 LOAD_NAME                8 (int)
+          54          52 LOAD_NAME                8 (int)
                       54 LOAD_CONST               4 (None)
                       56 BINARY_OP                7 (|)
                       60 LOAD_NAME                7 (__annotations__)
                       62 LOAD_CONST               5 ('code')
                       64 STORE_SUBSCR
                       68 LOAD_CONST               4 (None)
                       70 RETURN_VALUE
@@ -114,15 +127,15 @@
             'code'
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Dict', 'str', 'Any', '__annotations__', 'int')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'build\\bdist.win-amd64\\egg\\weatherly\\abc.py'
          name       'ResponseModel'
-         firstlineno 37
+         firstlineno 38
          lnotab 0x0c01040d1a010a01
       'ResponseModel'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
@@ -131,128 +144,128 @@
             0564033c0000006506650564043c0000006507650564053c000000650865
             0564063c0000006508650564073c0000006504650564083c000000650665
             0564093c00000065066505640a3c00000065046505640b3c000000650865
             05640c3c00000065066505640d3c00000065066505640e3c000000650665
             05640f3c0000006506650564103c0000006504650564113c000000650465
             0564123c0000006506650564133c0000006506650564143c000000650665
             0564153c00000064165300
-          55           0 RESUME                   0
+          56           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CurrentWeather')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          56          12 LOAD_CONST               1 ('\n    An ABC defining current weather data.\n\n    The following classes implement this ABC:\n    - :class:`~weatherly.CurrentWeatherData`\n\n    Attributes\n    ----------\n    last_updated_epoch: :class:`int`\n        The timestamp when the weather data was last updated.\n    temp_c: :class:`float`\n        Weather temperature in Celsius\n    temp_f: :class:`float`\n        Weather temperature in Fahrenheit\n    is_day: :class:`bool`\n        Wherever the current time is considered day time.\n    condition_text: :class:`str`\n        Weather condition text\n    condition_icon: :class:`str`\n        Link to the weather condition icon\n    condition_code: :class:`int`\n        Code of current weather condition\n    wind_mph: :class:`float`\n        Current wind speed in miles per hour (mph)\n    wind_kph: :class:`float`\n        Current wind speed in kilometers per hour (kph)\n    wind_degree: :class:`int`\n        Direction of wind in degrees\n    wind_dir: :class:`str`\n        Direction of wind as a string (e.g. "W")\n    pressure_mb: :class:`float`\n        Pressure in millibars (mb)\n    pressure_in: :class:`float`\n        Pressure in inches (in)\n    precip_mm: :class:`float`\n        Precipation (water that is falling out of the sky) in millimeters (mm)\n    precip_in: :class:`float`\n        Precipation (water that is falling in the sky) in inches (in)\n    humidity: :class:`int`\n        Humidity in integer percentage\n    cloud: :class:`int`\n        Cloud cover as percentage\n    feelslike_c: :class:`float`\n        Feels like temperature in Celsius\n    feelslike_f: :class:`float`\n        Feels like temperature in Fahrenheit\n    uv: :class:`float`\n        UV Index\n    ')
+          57          12 LOAD_CONST               1 ('\n    An ABC defining current weather data.\n\n    The following classes implement this ABC:\n    - :class:`~weatherly.CurrentWeatherData`\n\n    Attributes\n    ------------\n    location: :class:`~weatherly.LocationData`\n        Location of the requested weather data\n    last_updated_epoch: :class:`int`\n        The timestamp when the weather data was last updated.\n    temp_c: :class:`float`\n        Weather temperature in Celsius\n    temp_f: :class:`float`\n        Weather temperature in Fahrenheit\n    is_day: :class:`bool`\n        Wherever the current time is considered day time.\n    condition_text: :class:`str`\n        Weather condition text\n    condition_icon: :class:`str`\n        Link to the weather condition icon\n    condition_code: :class:`int`\n        Code of current weather condition\n    wind_mph: :class:`float`\n        Current wind speed in miles per hour (mph)\n    wind_kph: :class:`float`\n        Current wind speed in kilometers per hour (kph)\n    wind_degree: :class:`int`\n        Direction of wind in degrees\n    wind_dir: :class:`str`\n        Direction of wind as a string (e.g. "W")\n    pressure_mb: :class:`float`\n        Pressure in millibars (mb)\n    pressure_in: :class:`float`\n        Pressure in inches (in)\n    precip_mm: :class:`float`\n        Precipation (water that is falling out of the sky) in millimeters (mm)\n    precip_in: :class:`float`\n        Precipation (water that is falling in the sky) in inches (in)\n    humidity: :class:`int`\n        Humidity in integer percentage\n    cloud: :class:`int`\n        Cloud cover as percentage\n    feelslike_c: :class:`float`\n        Feels like temperature in Celsius\n    feelslike_f: :class:`float`\n        Feels like temperature in Fahrenheit\n    uv: :class:`float`\n        UV Index\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-         105          16 LOAD_NAME                4 (int)
+         108          16 LOAD_NAME                4 (int)
                       18 LOAD_NAME                5 (__annotations__)
                       20 LOAD_CONST               2 ('last_updated_epoch')
                       22 STORE_SUBSCR
          
-         106          26 LOAD_NAME                6 (float)
+         109          26 LOAD_NAME                6 (float)
                       28 LOAD_NAME                5 (__annotations__)
                       30 LOAD_CONST               3 ('temp_c')
                       32 STORE_SUBSCR
          
-         107          36 LOAD_NAME                6 (float)
+         110          36 LOAD_NAME                6 (float)
                       38 LOAD_NAME                5 (__annotations__)
                       40 LOAD_CONST               4 ('temp_f')
                       42 STORE_SUBSCR
          
-         108          46 LOAD_NAME                7 (bool)
+         111          46 LOAD_NAME                7 (bool)
                       48 LOAD_NAME                5 (__annotations__)
                       50 LOAD_CONST               5 ('is_day')
                       52 STORE_SUBSCR
          
-         109          56 LOAD_NAME                8 (str)
+         112          56 LOAD_NAME                8 (str)
                       58 LOAD_NAME                5 (__annotations__)
                       60 LOAD_CONST               6 ('condition_text')
                       62 STORE_SUBSCR
          
-         110          66 LOAD_NAME                8 (str)
+         113          66 LOAD_NAME                8 (str)
                       68 LOAD_NAME                5 (__annotations__)
                       70 LOAD_CONST               7 ('condition_icon')
                       72 STORE_SUBSCR
          
-         111          76 LOAD_NAME                4 (int)
+         114          76 LOAD_NAME                4 (int)
                       78 LOAD_NAME                5 (__annotations__)
                       80 LOAD_CONST               8 ('condition_code')
                       82 STORE_SUBSCR
          
-         112          86 LOAD_NAME                6 (float)
+         115          86 LOAD_NAME                6 (float)
                       88 LOAD_NAME                5 (__annotations__)
                       90 LOAD_CONST               9 ('wind_mph')
                       92 STORE_SUBSCR
          
-         113          96 LOAD_NAME                6 (float)
+         116          96 LOAD_NAME                6 (float)
                       98 LOAD_NAME                5 (__annotations__)
                      100 LOAD_CONST              10 ('wind_kph')
                      102 STORE_SUBSCR
          
-         114         106 LOAD_NAME                4 (int)
+         117         106 LOAD_NAME                4 (int)
                      108 LOAD_NAME                5 (__annotations__)
                      110 LOAD_CONST              11 ('wind_degree')
                      112 STORE_SUBSCR
          
-         115         116 LOAD_NAME                8 (str)
+         118         116 LOAD_NAME                8 (str)
                      118 LOAD_NAME                5 (__annotations__)
                      120 LOAD_CONST              12 ('wind_dir')
                      122 STORE_SUBSCR
          
-         116         126 LOAD_NAME                6 (float)
+         119         126 LOAD_NAME                6 (float)
                      128 LOAD_NAME                5 (__annotations__)
                      130 LOAD_CONST              13 ('pressure_mb')
                      132 STORE_SUBSCR
          
-         117         136 LOAD_NAME                6 (float)
+         120         136 LOAD_NAME                6 (float)
                      138 LOAD_NAME                5 (__annotations__)
                      140 LOAD_CONST              14 ('pressure_in')
                      142 STORE_SUBSCR
          
-         118         146 LOAD_NAME                6 (float)
+         121         146 LOAD_NAME                6 (float)
                      148 LOAD_NAME                5 (__annotations__)
                      150 LOAD_CONST              15 ('precip_mm')
                      152 STORE_SUBSCR
          
-         119         156 LOAD_NAME                6 (float)
+         122         156 LOAD_NAME                6 (float)
                      158 LOAD_NAME                5 (__annotations__)
                      160 LOAD_CONST              16 ('precip_in')
                      162 STORE_SUBSCR
          
-         120         166 LOAD_NAME                4 (int)
+         123         166 LOAD_NAME                4 (int)
                      168 LOAD_NAME                5 (__annotations__)
                      170 LOAD_CONST              17 ('humidity')
                      172 STORE_SUBSCR
          
-         121         176 LOAD_NAME                4 (int)
+         124         176 LOAD_NAME                4 (int)
                      178 LOAD_NAME                5 (__annotations__)
                      180 LOAD_CONST              18 ('cloud')
                      182 STORE_SUBSCR
          
-         122         186 LOAD_NAME                6 (float)
+         125         186 LOAD_NAME                6 (float)
                      188 LOAD_NAME                5 (__annotations__)
                      190 LOAD_CONST              19 ('feelslike_c')
                      192 STORE_SUBSCR
          
-         123         196 LOAD_NAME                6 (float)
+         126         196 LOAD_NAME                6 (float)
                      198 LOAD_NAME                5 (__annotations__)
                      200 LOAD_CONST              20 ('feelslike_f')
                      202 STORE_SUBSCR
          
-         124         206 LOAD_NAME                6 (float)
+         127         206 LOAD_NAME                6 (float)
                      208 LOAD_NAME                5 (__annotations__)
                      210 LOAD_CONST              21 ('uv')
                      212 STORE_SUBSCR
                      216 LOAD_CONST              22 (None)
                      218 RETURN_VALUE
          consts
             'CurrentWeather'
-            '\n    An ABC defining current weather data.\n\n    The following classes implement this ABC:\n    - :class:`~weatherly.CurrentWeatherData`\n\n    Attributes\n    ----------\n    last_updated_epoch: :class:`int`\n        The timestamp when the weather data was last updated.\n    temp_c: :class:`float`\n        Weather temperature in Celsius\n    temp_f: :class:`float`\n        Weather temperature in Fahrenheit\n    is_day: :class:`bool`\n        Wherever the current time is considered day time.\n    condition_text: :class:`str`\n        Weather condition text\n    condition_icon: :class:`str`\n        Link to the weather condition icon\n    condition_code: :class:`int`\n        Code of current weather condition\n    wind_mph: :class:`float`\n        Current wind speed in miles per hour (mph)\n    wind_kph: :class:`float`\n        Current wind speed in kilometers per hour (kph)\n    wind_degree: :class:`int`\n        Direction of wind in degrees\n    wind_dir: :class:`str`\n        Direction of wind as a string (e.g. "W")\n    pressure_mb: :class:`float`\n        Pressure in millibars (mb)\n    pressure_in: :class:`float`\n        Pressure in inches (in)\n    precip_mm: :class:`float`\n        Precipation (water that is falling out of the sky) in millimeters (mm)\n    precip_in: :class:`float`\n        Precipation (water that is falling in the sky) in inches (in)\n    humidity: :class:`int`\n        Humidity in integer percentage\n    cloud: :class:`int`\n        Cloud cover as percentage\n    feelslike_c: :class:`float`\n        Feels like temperature in Celsius\n    feelslike_f: :class:`float`\n        Feels like temperature in Fahrenheit\n    uv: :class:`float`\n        UV Index\n    '
+            '\n    An ABC defining current weather data.\n\n    The following classes implement this ABC:\n    - :class:`~weatherly.CurrentWeatherData`\n\n    Attributes\n    ------------\n    location: :class:`~weatherly.LocationData`\n        Location of the requested weather data\n    last_updated_epoch: :class:`int`\n        The timestamp when the weather data was last updated.\n    temp_c: :class:`float`\n        Weather temperature in Celsius\n    temp_f: :class:`float`\n        Weather temperature in Fahrenheit\n    is_day: :class:`bool`\n        Wherever the current time is considered day time.\n    condition_text: :class:`str`\n        Weather condition text\n    condition_icon: :class:`str`\n        Link to the weather condition icon\n    condition_code: :class:`int`\n        Code of current weather condition\n    wind_mph: :class:`float`\n        Current wind speed in miles per hour (mph)\n    wind_kph: :class:`float`\n        Current wind speed in kilometers per hour (kph)\n    wind_degree: :class:`int`\n        Direction of wind in degrees\n    wind_dir: :class:`str`\n        Direction of wind as a string (e.g. "W")\n    pressure_mb: :class:`float`\n        Pressure in millibars (mb)\n    pressure_in: :class:`float`\n        Pressure in inches (in)\n    precip_mm: :class:`float`\n        Precipation (water that is falling out of the sky) in millimeters (mm)\n    precip_in: :class:`float`\n        Precipation (water that is falling in the sky) in inches (in)\n    humidity: :class:`int`\n        Humidity in integer percentage\n    cloud: :class:`int`\n        Cloud cover as percentage\n    feelslike_c: :class:`float`\n        Feels like temperature in Celsius\n    feelslike_f: :class:`float`\n        Feels like temperature in Fahrenheit\n    uv: :class:`float`\n        UV Index\n    '
             'last_updated_epoch'
             'temp_c'
             'temp_f'
             'is_day'
             'condition_text'
             'condition_icon'
             'condition_code'
@@ -272,21 +285,119 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'int', '__annotations__', 'float', 'bool', 'str')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'build\\bdist.win-amd64\\egg\\weatherly\\abc.py'
          name       'CurrentWeather'
-         firstlineno 55
+         firstlineno 56
          lnotab
-            0x0c0104310a010a010a010a010a010a010a010a010a010a010a010a010a
+            0x0c0104330a010a010a010a010a010a010a010a010a010a010a010a010a
             010a010a010a010a010a010a01
       'CurrentWeather'
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 3
+         flags     : 0
+         code
+            0x970065005a0164005a02550064015a0365046505190000000000000000
+            00650664023c0000006507650664033c0000006507650664043c00000065
+            07650664053c0000006508650664063c0000006508650664073c00000065
+            04650719000000000000000000650664083c000000650465051900000000
+            0000000000650664093c0000006504650719000000000000000000650664
+            0a3c000000640b5300
+         129           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('LocationModel')
+                       8 STORE_NAME               2 (__qualname__)
+                      10 SETUP_ANNOTATIONS
+         
+         130          12 LOAD_CONST               1 ('An ABC that provides information about a location\n\n    Attributes\n    --------------\n    id: :class:`int`\n        A specific ID of the location. Can be ``None``\n    name: :class:`str`\n        Name of the location (e.g. London)\n    region: :class:`str`\n        A region of the location\n    country: :class:`str`\n        Country where the location is\n    latitude: :class:`float`\n        Latitude coordinate of the location\n    longitude: :class:`float`\n        Longitude coordinate of the location\n    timezone_id: Optional[:class:`str`]\n        Timezone ID of the location (e.g. Europe/London). Could be ``None`` when using the Search/Autocomplete API.\n    localtime_epoch: Optional[:class:`int`]\n        Local time of the location as a timestamp\n    localtime_formatted: Optional[:class:`str`]\n        Formatted local time of the location\n    ')
+                      14 STORE_NAME               3 (__doc__)
+         
+         153          16 LOAD_NAME                4 (Optional)
+                      18 LOAD_NAME                5 (int)
+                      20 BINARY_SUBSCR
+                      30 LOAD_NAME                6 (__annotations__)
+                      32 LOAD_CONST               2 ('id')
+                      34 STORE_SUBSCR
+         
+         154          38 LOAD_NAME                7 (str)
+                      40 LOAD_NAME                6 (__annotations__)
+                      42 LOAD_CONST               3 ('name')
+                      44 STORE_SUBSCR
+         
+         155          48 LOAD_NAME                7 (str)
+                      50 LOAD_NAME                6 (__annotations__)
+                      52 LOAD_CONST               4 ('region')
+                      54 STORE_SUBSCR
+         
+         156          58 LOAD_NAME                7 (str)
+                      60 LOAD_NAME                6 (__annotations__)
+                      62 LOAD_CONST               5 ('country')
+                      64 STORE_SUBSCR
+         
+         157          68 LOAD_NAME                8 (float)
+                      70 LOAD_NAME                6 (__annotations__)
+                      72 LOAD_CONST               6 ('latitude')
+                      74 STORE_SUBSCR
+         
+         158          78 LOAD_NAME                8 (float)
+                      80 LOAD_NAME                6 (__annotations__)
+                      82 LOAD_CONST               7 ('longitude')
+                      84 STORE_SUBSCR
+         
+         159          88 LOAD_NAME                4 (Optional)
+                      90 LOAD_NAME                7 (str)
+                      92 BINARY_SUBSCR
+                     102 LOAD_NAME                6 (__annotations__)
+                     104 LOAD_CONST               8 ('timezone_id')
+                     106 STORE_SUBSCR
+         
+         160         110 LOAD_NAME                4 (Optional)
+                     112 LOAD_NAME                5 (int)
+                     114 BINARY_SUBSCR
+                     124 LOAD_NAME                6 (__annotations__)
+                     126 LOAD_CONST               9 ('localtime_epoch')
+                     128 STORE_SUBSCR
+         
+         161         132 LOAD_NAME                4 (Optional)
+                     134 LOAD_NAME                7 (str)
+                     136 BINARY_SUBSCR
+                     146 LOAD_NAME                6 (__annotations__)
+                     148 LOAD_CONST              10 ('localtime_formatted')
+                     150 STORE_SUBSCR
+                     154 LOAD_CONST              11 (None)
+                     156 RETURN_VALUE
+         consts
+            'LocationModel'
+            'An ABC that provides information about a location\n\n    Attributes\n    --------------\n    id: :class:`int`\n        A specific ID of the location. Can be ``None``\n    name: :class:`str`\n        Name of the location (e.g. London)\n    region: :class:`str`\n        A region of the location\n    country: :class:`str`\n        Country where the location is\n    latitude: :class:`float`\n        Latitude coordinate of the location\n    longitude: :class:`float`\n        Longitude coordinate of the location\n    timezone_id: Optional[:class:`str`]\n        Timezone ID of the location (e.g. Europe/London). Could be ``None`` when using the Search/Autocomplete API.\n    localtime_epoch: Optional[:class:`int`]\n        Local time of the location as a timestamp\n    localtime_formatted: Optional[:class:`str`]\n        Formatted local time of the location\n    '
+            'id'
+            'name'
+            'region'
+            'country'
+            'latitude'
+            'longitude'
+            'timezone_id'
+            'localtime_epoch'
+            'localtime_formatted'
+            None
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'Optional', 'int', '__annotations__', 'str', 'float')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   'build\\bdist.win-amd64\\egg\\weatherly\\abc.py'
+         name       'LocationModel'
+         firstlineno 129
+         lnotab 0x0c01041716010a010a010a010a010a0116011601
+      'LocationModel'
       None
-   names      ('__doc__', 'typing', 'Any', 'Literal', 'Dict', 'abc', 'ABC', '__all__', 'ResponseModel', 'CurrentWeather')
+   names      ('__doc__', 'typing', 'Any', 'Literal', 'Dict', 'Optional', 'abc', 'ABC', '__all__', 'ResponseModel', 'CurrentWeather', 'LocationModel')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'build\\bdist.win-amd64\\egg\\weatherly\\abc.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201041814050c0204051c12
+   lnotab 0x00ff0201041818060c0204051c121c49
```

## weatherly/__pycache__/errors.cpython-311.pyc

### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xdaf03c64 (Mon Apr 17 07:10:18 2023 UTC)
-files sz: 3871
+moddate:  0xc52a4264 (Fri Apr 21 06:18:45 2023 UTC)
+files sz: 3854
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a0064015a01020047006402840064036502a6030000ab0300
@@ -264,22 +264,22 @@
          code 0x970065005a0164005a0264015a0364025300
           64           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('NoLocationFound')
                        8 STORE_NAME               2 (__qualname__)
          
-          65          10 LOAD_CONST               1 ('\n    Exception like this is raised when no location was found when searching for weather data.\n\n    Usually has status code of 400 and error code 1006.\n    \n    Inherits from :class:`WeatherAPIException`.\n    ')
+          65          10 LOAD_CONST               1 ('\n    Exception like this is raised when no location was found when searching for weather data.\n\n    Usually has status code  400 and error code 1006.\n    \n    Inherits from :class:`WeatherAPIException`.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
           72          14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'NoLocationFound'
-            '\n    Exception like this is raised when no location was found when searching for weather data.\n\n    Usually has status code of 400 and error code 1006.\n    \n    Inherits from :class:`WeatherAPIException`.\n    '
+            '\n    Exception like this is raised when no location was found when searching for weather data.\n\n    Usually has status code  400 and error code 1006.\n    \n    Inherits from :class:`WeatherAPIException`.\n    '
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'build\\bdist.win-amd64\\egg\\weatherly\\errors.py'
          name       'NoLocationFound'
@@ -294,22 +294,22 @@
          code 0x970065005a0164005a0264015a0364025300
           74           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InvalidAPIKey')
                        8 STORE_NAME               2 (__qualname__)
          
-          75          10 LOAD_CONST               1 ('\n    Exception like this is raised when provided API key is invalid\n\n    Usually has status code of 401 and error code 2006.\n    \n    Inherits from :class:`WeatherAPIException`.\n    ')
+          75          10 LOAD_CONST               1 ('\n    Exception like this is raised when provided API key is invalid\n\n    Usually has status code 401 and error code 2006.\n    \n    Inherits from :class:`WeatherAPIException`.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
           82          14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'InvalidAPIKey'
-            '\n    Exception like this is raised when provided API key is invalid\n\n    Usually has status code of 401 and error code 2006.\n    \n    Inherits from :class:`WeatherAPIException`.\n    '
+            '\n    Exception like this is raised when provided API key is invalid\n\n    Usually has status code 401 and error code 2006.\n    \n    Inherits from :class:`WeatherAPIException`.\n    '
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'build\\bdist.win-amd64\\egg\\weatherly\\errors.py'
          name       'InvalidAPIKey'
@@ -324,22 +324,22 @@
          code 0x970065005a0164005a0264015a0364025300
           84           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('APILimitExceeded')
                        8 STORE_NAME               2 (__qualname__)
          
-          85          10 LOAD_CONST               1 ('\n    Exception like this is raised when API key has exceeded monthly calls limit.\n\n    Usually has status code of 400 and error code 2007.\n    \n    Inherits from :class:`WeatherAPIException`.\n    ')
+          85          10 LOAD_CONST               1 ('\n    Exception like this is raised when API key has exceeded monthly calls limit.\n\n    Usually has status code 400 and error code 2007.\n    \n    Inherits from :class:`WeatherAPIException`.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
           92          14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'APILimitExceeded'
-            '\n    Exception like this is raised when API key has exceeded monthly calls limit.\n\n    Usually has status code of 400 and error code 2007.\n    \n    Inherits from :class:`WeatherAPIException`.\n    '
+            '\n    Exception like this is raised when API key has exceeded monthly calls limit.\n\n    Usually has status code 400 and error code 2007.\n    \n    Inherits from :class:`WeatherAPIException`.\n    '
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'build\\bdist.win-amd64\\egg\\weatherly\\errors.py'
          name       'APILimitExceeded'
@@ -354,22 +354,22 @@
          code 0x970065005a0164005a0264015a0364025300
           94           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('APIKeyDisabled')
                        8 STORE_NAME               2 (__qualname__)
          
-          95          10 LOAD_CONST               1 ('\n    Exception like this is raised when API key has been disabled.\n\n    Usually has status code of 403 and error code 2008.\n    \n    Inherits from :class:`WeatherAPIException`.\n    ')
+          95          10 LOAD_CONST               1 ('\n    Exception like this is raised when API key has been disabled.\n\n    Usually has status code 403 and error code 2008.\n    \n    Inherits from :class:`WeatherAPIException`.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
          102          14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'APIKeyDisabled'
-            '\n    Exception like this is raised when API key has been disabled.\n\n    Usually has status code of 403 and error code 2008.\n    \n    Inherits from :class:`WeatherAPIException`.\n    '
+            '\n    Exception like this is raised when API key has been disabled.\n\n    Usually has status code 403 and error code 2008.\n    \n    Inherits from :class:`WeatherAPIException`.\n    '
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'build\\bdist.win-amd64\\egg\\weatherly\\errors.py'
          name       'APIKeyDisabled'
@@ -384,22 +384,22 @@
          code 0x970065005a0164005a0264015a0364025300
          104           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AccessDenied')
                        8 STORE_NAME               2 (__qualname__)
          
-         105          10 LOAD_CONST               1 ('\n    Exception like this is raised when API key does not have access to requested resource.\n\n    Usually has status code of 403 and error code 2009.\n    \n    Inherits from :class:`WeatherAPIException`.\n    ')
+         105          10 LOAD_CONST               1 ('\n    Exception like this is raised when API key does not have access to requested resource.\n\n    Usually has status code 403 and error code 2009.\n    \n    Inherits from :class:`WeatherAPIException`.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
          112          14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'AccessDenied'
-            '\n    Exception like this is raised when API key does not have access to requested resource.\n\n    Usually has status code of 403 and error code 2009.\n    \n    Inherits from :class:`WeatherAPIException`.\n    '
+            '\n    Exception like this is raised when API key does not have access to requested resource.\n\n    Usually has status code 403 and error code 2009.\n    \n    Inherits from :class:`WeatherAPIException`.\n    '
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'build\\bdist.win-amd64\\egg\\weatherly\\errors.py'
          name       'AccessDenied'
@@ -414,22 +414,22 @@
          code 0x970065005a0164005a0264015a0364025300
          114           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InternalApplicationError')
                        8 STORE_NAME               2 (__qualname__)
          
-         115          10 LOAD_CONST               1 ('\n    Exception like this is raised when an internal application error occured. There is nothing to do about it.\n\n    Usually has status code of 400 and error code 9999.\n    \n    Inherits from :class:`WeatherAPIException`.\n    ')
+         115          10 LOAD_CONST               1 ('\n    Exception like this is raised when an internal application error occured. There is nothing to do about it.\n\n    Usually has status code 400 and error code 9999.\n    \n    Inherits from :class:`WeatherAPIException`.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
          122          14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'InternalApplicationError'
-            '\n    Exception like this is raised when an internal application error occured. There is nothing to do about it.\n\n    Usually has status code of 400 and error code 9999.\n    \n    Inherits from :class:`WeatherAPIException`.\n    '
+            '\n    Exception like this is raised when an internal application error occured. There is nothing to do about it.\n\n    Usually has status code 400 and error code 9999.\n    \n    Inherits from :class:`WeatherAPIException`.\n    '
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'build\\bdist.win-amd64\\egg\\weatherly\\errors.py'
          name       'InternalApplicationError'
```

## weatherly/__pycache__/responses.cpython-311.pyc

### Python bytecode

```diff
@@ -1,307 +1,344 @@
 magic:    0xa70d0d0a
-moddate:  0xf9f23c64 (Mon Apr 17 07:19:21 2023 UTC)
-files sz: 4487
+moddate:  0x762c4264 (Fri Apr 21 06:25:58 2023 UTC)
+files sz: 6809
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x970064005a00640164026c016d025a020100640364046c036d045a046d
-      055a056d065a060100020047006405840064066502a6030000ab03000000
-      00000000005a0764075300
+      0x970064005a00640164026c016d025a026d035a030100640364046c046d
+      055a056d065a066d075a07010064055a08020047006406840064076502a6
+      030000ab0300000000000000005a09020047006408840064096503a60300
+      00ab0300000000000000005a0a640a5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('\nMIT License\n\nCopyright (c) 2023 Konrad (@konradsic)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n')
                  4 STORE_NAME               0 (__doc__)
    
     25           6 LOAD_CONST               1 (1)
-                 8 LOAD_CONST               2 (('CurrentWeather',))
+                 8 LOAD_CONST               2 (('CurrentWeather', 'LocationModel'))
                 10 IMPORT_NAME              1 (abc)
                 12 IMPORT_FROM              2 (CurrentWeather)
                 14 STORE_NAME               2 (CurrentWeather)
-                16 POP_TOP
+                16 IMPORT_FROM              3 (LocationModel)
+                18 STORE_NAME               3 (LocationModel)
+                20 POP_TOP
    
-    26          18 LOAD_CONST               3 (0)
-                20 LOAD_CONST               4 (('Dict', 'Any', 'Union'))
-                22 IMPORT_NAME              3 (typing)
-                24 IMPORT_FROM              4 (Dict)
-                26 STORE_NAME               4 (Dict)
-                28 IMPORT_FROM              5 (Any)
-                30 STORE_NAME               5 (Any)
-                32 IMPORT_FROM              6 (Union)
-                34 STORE_NAME               6 (Union)
-                36 POP_TOP
+    26          22 LOAD_CONST               3 (0)
+                24 LOAD_CONST               4 (('Dict', 'Any', 'Union'))
+                26 IMPORT_NAME              4 (typing)
+                28 IMPORT_FROM              5 (Dict)
+                30 STORE_NAME               5 (Dict)
+                32 IMPORT_FROM              6 (Any)
+                34 STORE_NAME               6 (Any)
+                36 IMPORT_FROM              7 (Union)
+                38 STORE_NAME               7 (Union)
+                40 POP_TOP
    
-    32          38 PUSH_NULL
-                40 LOAD_BUILD_CLASS
-                42 LOAD_CONST               5 (<code object CurrentWeatherData, file "build\bdist.win-amd64\egg\weatherly\responses.py", line 32>)
-                44 MAKE_FUNCTION            0
-                46 LOAD_CONST               6 ('CurrentWeatherData')
-                48 LOAD_NAME                2 (CurrentWeather)
-                50 PRECALL                  3
-                54 CALL                     3
-                64 STORE_NAME               7 (CurrentWeatherData)
-                66 LOAD_CONST               7 (None)
-                68 RETURN_VALUE
+    32          42 LOAD_CONST               5 (('CurrentWeatherData', 'LocationData'))
+                44 STORE_NAME               8 (__all__)
+   
+    37          46 PUSH_NULL
+                48 LOAD_BUILD_CLASS
+                50 LOAD_CONST               6 (<code object CurrentWeatherData, file "build\bdist.win-amd64\egg\weatherly\responses.py", line 37>)
+                52 MAKE_FUNCTION            0
+                54 LOAD_CONST               7 ('CurrentWeatherData')
+                56 LOAD_NAME                2 (CurrentWeather)
+                58 PRECALL                  3
+                62 CALL                     3
+                72 STORE_NAME               9 (CurrentWeatherData)
+   
+   133          74 PUSH_NULL
+                76 LOAD_BUILD_CLASS
+                78 LOAD_CONST               8 (<code object LocationData, file "build\bdist.win-amd64\egg\weatherly\responses.py", line 133>)
+                80 MAKE_FUNCTION            0
+                82 LOAD_CONST               9 ('LocationData')
+                84 LOAD_NAME                3 (LocationModel)
+                86 PRECALL                  3
+                90 CALL                     3
+               100 STORE_NAME              10 (LocationData)
+               102 LOAD_CONST              10 (None)
+               104 RETURN_VALUE
    consts
       '\nMIT License\n\nCopyright (c) 2023 Konrad (@konradsic)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n'
       1
-      ('CurrentWeather',)
+      ('CurrentWeather', 'LocationModel')
       0
       ('Dict', 'Any', 'Union')
+      ('CurrentWeatherData', 'LocationData')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 8
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364026504650565066602190000
             000000000000006403650764046508650764056602190000000000000000
             00640664056608880066016407840c5a09880078015a0a5300
                        0 MAKE_CELL                0 (__class__)
          
-          32           2 RESUME                   0
+          37           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('CurrentWeatherData')
                       10 STORE_NAME               2 (__qualname__)
          
-          33          12 LOAD_CONST               1 ('\n    Current weather data, a common return type from methods that requests this from WeatherAPI.com.\n    \n    Please note, that only ``condition_text`` is translated into requested language.\n\n    Attributes\n    ----------\n    raw: Dict[:class:`str`, Any]\n        Raw response in a JSON-like format (converted to a python dictionary)\n    status: :class:`int`\n        HTTP status of the response. 200 is OK, and is the most common status.\n    code: Union[:class:`int`, None]\n        Response code. In some cases this can be ``None``\n    last_updated_epoch: :class:`int`\n        The timestamp when the weather data was last updated.\n    temp_c: :class:`float`\n        Weather temperature in Celsius\n    temp_f: :class:`float`\n        Weather temperature in Fahrenheit\n    is_day: :class:`bool`\n        Wherever the current time is considered day time.\n    condition_text: :class:`str`\n        Weather condition text\n    condition_icon: :class:`str`\n        Link to the weather condition icon\n    condition_code: :class:`int`\n        Code of current weather condition\n    wind_mph: :class:`float`\n        Current wind speed in miles per hour (mph)\n    wind_kph: :class:`float`\n        Current wind speed in kilometers per hour (kph)\n    wind_degree: :class:`int`\n        Direction of wind in degrees\n    wind_dir: :class:`str`\n        Direction of wind as a string (e.g. "W")\n    pressure_mb: :class:`float`\n        Pressure in millibars (mb)\n    pressure_in: :class:`float`\n        Pressure in inches (in)\n    precip_mm: :class:`float`\n        Precipation (water that is falling out of the sky) in millimeters (mm)\n    precip_in: :class:`float`\n        Precipation (water that is falling in the sky) in inches (in)\n    humidity: :class:`int`\n        Humidity in integer percentage\n    cloud: :class:`int`\n        Cloud cover as percentage\n    feelslike_c: :class:`float`\n        Feels like temperature in Celsius\n    feelslike_f: :class:`float`\n        Feels like temperature in Fahrenheit\n    uv: :class:`float`\n        UV Index\n    ')
+          38          12 LOAD_CONST               1 ('\n    Current weather data, a common return type from methods that requests this from WeatherAPI.com.\n    \n    Please note, that only ``condition_text`` is translated into requested language.\n    \n    .. note::\n        This class should not be created manually, instead it will be returned from methods like ``get_current_weather`` of the :class:`WeatherAPIClient` class.\n\n    Attributes\n    ----------\n    raw: Dict[:class:`str`, Any]\n        Raw response in a JSON-like format (converted to a python dictionary)\n    status: :class:`int`\n        HTTP status of the response. 200 is OK, and is the most common status.\n    code: Union[:class:`int`, None]\n        Response code. In some cases this can be ``None``\n    location: :class:`LocationData`\n        Location of the requested weather data\n    last_updated_epoch: :class:`int`\n        The timestamp when the weather data was last updated.\n    temp_c: :class:`float`\n        Weather temperature in Celsius\n    temp_f: :class:`float`\n        Weather temperature in Fahrenheit\n    is_day: :class:`bool`\n        Wherever the current time is considered day time.\n    condition_text: :class:`str`\n        Weather condition text\n    condition_icon: :class:`str`\n        Link to the weather condition icon\n    condition_code: :class:`int`\n        Code of current weather condition\n    wind_mph: :class:`float`\n        Current wind speed in miles per hour (mph)\n    wind_kph: :class:`float`\n        Current wind speed in kilometers per hour (kph)\n    wind_degree: :class:`int`\n        Direction of wind in degrees\n    wind_dir: :class:`str`\n        Direction of wind as a string (e.g. "W")\n    pressure_mb: :class:`float`\n        Pressure in millibars (mb)\n    pressure_in: :class:`float`\n        Pressure in inches (in)\n    precip_mm: :class:`float`\n        Precipation (water that is falling out of the sky) in millimeters (mm)\n    precip_in: :class:`float`\n        Precipation (water that is falling in the sky) in inches (in)\n    humidity: :class:`int`\n        Humidity in integer percentage\n    cloud: :class:`int`\n        Cloud cover as percentage\n    feelslike_c: :class:`float`\n        Feels like temperature in Celsius\n    feelslike_f: :class:`float`\n        Feels like temperature in Fahrenheit\n    uv: :class:`float`\n        UV Index\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-          87          16 LOAD_CONST               2 ('raw')
+          97          16 LOAD_CONST               2 ('raw')
          
-          89          18 LOAD_NAME                4 (Dict)
+          99          18 LOAD_NAME                4 (Dict)
                       20 LOAD_NAME                5 (str)
                       22 LOAD_NAME                6 (Any)
                       24 BUILD_TUPLE              2
                       26 BINARY_SUBSCR
          
-          87          36 LOAD_CONST               3 ('status')
+          97          36 LOAD_CONST               3 ('status')
          
-          90          38 LOAD_NAME                7 (int)
+         100          38 LOAD_NAME                7 (int)
          
-          87          40 LOAD_CONST               4 ('code')
+          97          40 LOAD_CONST               4 ('code')
          
-          91          42 LOAD_NAME                8 (Union)
+         101          42 LOAD_NAME                8 (Union)
                       44 LOAD_NAME                7 (int)
                       46 LOAD_CONST               5 (None)
                       48 BUILD_TUPLE              2
                       50 BINARY_SUBSCR
          
-          87          60 LOAD_CONST               6 ('return')
+          97          60 LOAD_CONST               6 ('return')
          
-          92          62 LOAD_CONST               5 (None)
+         102          62 LOAD_CONST               5 (None)
          
-          87          64 BUILD_TUPLE              8
+          97          64 BUILD_TUPLE              8
                       66 LOAD_CLOSURE             0 (__class__)
                       68 BUILD_TUPLE              1
-                      70 LOAD_CONST               7 (<code object __init__, file "build\bdist.win-amd64\egg\weatherly\responses.py", line 87>)
+                      70 LOAD_CONST               7 (<code object __init__, file "build\bdist.win-amd64\egg\weatherly\responses.py", line 97>)
                       72 MAKE_FUNCTION           12 (annotations, closure)
                       74 STORE_NAME               9 (__init__)
                       76 LOAD_CLOSURE             0 (__class__)
                       78 COPY                     1
                       80 STORE_NAME              10 (__classcell__)
                       82 RETURN_VALUE
          consts
             'CurrentWeatherData'
-            '\n    Current weather data, a common return type from methods that requests this from WeatherAPI.com.\n    \n    Please note, that only ``condition_text`` is translated into requested language.\n\n    Attributes\n    ----------\n    raw: Dict[:class:`str`, Any]\n        Raw response in a JSON-like format (converted to a python dictionary)\n    status: :class:`int`\n        HTTP status of the response. 200 is OK, and is the most common status.\n    code: Union[:class:`int`, None]\n        Response code. In some cases this can be ``None``\n    last_updated_epoch: :class:`int`\n        The timestamp when the weather data was last updated.\n    temp_c: :class:`float`\n        Weather temperature in Celsius\n    temp_f: :class:`float`\n        Weather temperature in Fahrenheit\n    is_day: :class:`bool`\n        Wherever the current time is considered day time.\n    condition_text: :class:`str`\n        Weather condition text\n    condition_icon: :class:`str`\n        Link to the weather condition icon\n    condition_code: :class:`int`\n        Code of current weather condition\n    wind_mph: :class:`float`\n        Current wind speed in miles per hour (mph)\n    wind_kph: :class:`float`\n        Current wind speed in kilometers per hour (kph)\n    wind_degree: :class:`int`\n        Direction of wind in degrees\n    wind_dir: :class:`str`\n        Direction of wind as a string (e.g. "W")\n    pressure_mb: :class:`float`\n        Pressure in millibars (mb)\n    pressure_in: :class:`float`\n        Pressure in inches (in)\n    precip_mm: :class:`float`\n        Precipation (water that is falling out of the sky) in millimeters (mm)\n    precip_in: :class:`float`\n        Precipation (water that is falling in the sky) in inches (in)\n    humidity: :class:`int`\n        Humidity in integer percentage\n    cloud: :class:`int`\n        Cloud cover as percentage\n    feelslike_c: :class:`float`\n        Feels like temperature in Celsius\n    feelslike_f: :class:`float`\n        Feels like temperature in Fahrenheit\n    uv: :class:`float`\n        UV Index\n    '
+            '\n    Current weather data, a common return type from methods that requests this from WeatherAPI.com.\n    \n    Please note, that only ``condition_text`` is translated into requested language.\n    \n    .. note::\n        This class should not be created manually, instead it will be returned from methods like ``get_current_weather`` of the :class:`WeatherAPIClient` class.\n\n    Attributes\n    ----------\n    raw: Dict[:class:`str`, Any]\n        Raw response in a JSON-like format (converted to a python dictionary)\n    status: :class:`int`\n        HTTP status of the response. 200 is OK, and is the most common status.\n    code: Union[:class:`int`, None]\n        Response code. In some cases this can be ``None``\n    location: :class:`LocationData`\n        Location of the requested weather data\n    last_updated_epoch: :class:`int`\n        The timestamp when the weather data was last updated.\n    temp_c: :class:`float`\n        Weather temperature in Celsius\n    temp_f: :class:`float`\n        Weather temperature in Fahrenheit\n    is_day: :class:`bool`\n        Wherever the current time is considered day time.\n    condition_text: :class:`str`\n        Weather condition text\n    condition_icon: :class:`str`\n        Link to the weather condition icon\n    condition_code: :class:`int`\n        Code of current weather condition\n    wind_mph: :class:`float`\n        Current wind speed in miles per hour (mph)\n    wind_kph: :class:`float`\n        Current wind speed in kilometers per hour (kph)\n    wind_degree: :class:`int`\n        Direction of wind in degrees\n    wind_dir: :class:`str`\n        Direction of wind as a string (e.g. "W")\n    pressure_mb: :class:`float`\n        Pressure in millibars (mb)\n    pressure_in: :class:`float`\n        Pressure in inches (in)\n    precip_mm: :class:`float`\n        Precipation (water that is falling out of the sky) in millimeters (mm)\n    precip_in: :class:`float`\n        Precipation (water that is falling in the sky) in inches (in)\n    humidity: :class:`int`\n        Humidity in integer percentage\n    cloud: :class:`int`\n        Cloud cover as percentage\n    feelslike_c: :class:`float`\n        Feels like temperature in Celsius\n    feelslike_f: :class:`float`\n        Feels like temperature in Fahrenheit\n    uv: :class:`float`\n        UV Index\n    '
             'raw'
             'status'
             'code'
             None
             'return'
             code
                argcount  : 4
                nlocals   : 4
-               stacksize : 4
+               stacksize : 5
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a0010000000000000000000000000000000000000000a6000000ab0000
                   0000000000000001007c027c005f0200000000000000007c037c005f0300
-                  000000000000007c017c005f0400000000000000007c0164011900000000
-                  00000000007c005f0500000000000000007c016402190000000000000000
-                  007c005f0600000000000000007c016403190000000000000000007c005f
-                  0700000000000000007411000000000000000000007c0164041900000000
-                  0000000000a6010000ab0100000000000000007c005f0900000000000000
-                  007c016405190000000000000000006406190000000000000000007c005f
-                  0a00000000000000007c0164051900000000000000000064071900000000
-                  00000000007c005f0b00000000000000007c016405190000000000000000
-                  006408190000000000000000007c005f0c00000000000000007c01640919
-                  0000000000000000007c005f0d00000000000000007c01640a1900000000
-                  00000000007c005f0e00000000000000007c01640b190000000000000000
-                  007c005f0f00000000000000007c01640c190000000000000000007c005f
-                  1000000000000000007c01640d190000000000000000007c005f11000000
-                  00000000007c01640e190000000000000000007c005f1200000000000000
-                  007c01640f190000000000000000007c005f1300000000000000007c0164
-                  10190000000000000000007c005f1400000000000000007c016411190000
-                  000000000000007c005f1500000000000000007c01641219000000000000
-                  0000007c005f1600000000000000007c016413190000000000000000007c
-                  005f1700000000000000007c016414190000000000000000007c005f1800
-                  000000000000007c016415190000000000000000007c005f190000000000
-                  00000064005300
+                  000000000000007c017c005f040000000000000000740b00000000000000
+                  0000007c016401190000000000000000007c027c03a6030000ab03000000
+                  00000000007c005f0600000000000000007c016402190000000000000000
+                  007d017c016403190000000000000000007c005f0700000000000000007c
+                  016404190000000000000000007c005f0800000000000000007c01640519
+                  0000000000000000007c005f090000000000000000741500000000000000
+                  0000007c01640619000000000000000000a6010000ab0100000000000000
+                  007c005f0b00000000000000007c01640719000000000000000000640819
+                  0000000000000000007c005f0c00000000000000007c0164071900000000
+                  00000000006409190000000000000000007c005f0d00000000000000007c
+                  01640719000000000000000000640a190000000000000000007c005f0e00
+                  000000000000007c01640b190000000000000000007c005f0f0000000000
+                  0000007c01640c190000000000000000007c005f1000000000000000007c
+                  01640d190000000000000000007c005f1100000000000000007c01640e19
+                  0000000000000000007c005f1200000000000000007c01640f1900000000
+                  00000000007c005f1300000000000000007c016410190000000000000000
+                  007c005f1400000000000000007c016411190000000000000000007c005f
+                  1500000000000000007c016412190000000000000000007c005f16000000
+                  00000000007c016413190000000000000000007c005f1700000000000000
+                  007c016414190000000000000000007c005f1800000000000000007c0164
+                  15190000000000000000007c005f1900000000000000007c016416190000
+                  000000000000007c005f1a00000000000000007c01641719000000000000
+                  0000007c005f1b000000000000000064005300
                              0 COPY_FREE_VARS           1
                
-                87           2 RESUME                   0
+                97           2 RESUME                   0
                
-                93           4 LOAD_GLOBAL              1 (NULL + super)
+               103           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (__init__)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 POP_TOP
                
-                95          68 LOAD_FAST                2 (status)
+               105          68 LOAD_FAST                2 (status)
                             70 LOAD_FAST                0 (self)
                             72 STORE_ATTR               2 (status)
                
-                96          82 LOAD_FAST                3 (code)
+               106          82 LOAD_FAST                3 (code)
                             84 LOAD_FAST                0 (self)
                             86 STORE_ATTR               3 (code)
                
-                97          96 LOAD_FAST                1 (raw)
+               107          96 LOAD_FAST                1 (raw)
                             98 LOAD_FAST                0 (self)
                            100 STORE_ATTR               4 (raw)
                
-                98         110 LOAD_FAST                1 (raw)
-                           112 LOAD_CONST               1 ('last_updated_epoch')
-                           114 BINARY_SUBSCR
-                           124 LOAD_FAST                0 (self)
-                           126 STORE_ATTR               5 (last_updated_epoch)
-               
-                99         136 LOAD_FAST                1 (raw)
-                           138 LOAD_CONST               2 ('temp_c')
-                           140 BINARY_SUBSCR
-                           150 LOAD_FAST                0 (self)
-                           152 STORE_ATTR               6 (temp_c)
-               
-               100         162 LOAD_FAST                1 (raw)
-                           164 LOAD_CONST               3 ('temp_f')
-                           166 BINARY_SUBSCR
-                           176 LOAD_FAST                0 (self)
-                           178 STORE_ATTR               7 (temp_f)
-               
-               101         188 LOAD_GLOBAL             17 (NULL + bool)
-                           200 LOAD_FAST                1 (raw)
-                           202 LOAD_CONST               4 ('is_day')
-                           204 BINARY_SUBSCR
-                           214 PRECALL                  1
-                           218 CALL                     1
-                           228 LOAD_FAST                0 (self)
-                           230 STORE_ATTR               9 (is_day)
-               
-               102         240 LOAD_FAST                1 (raw)
-                           242 LOAD_CONST               5 ('condition')
-                           244 BINARY_SUBSCR
-                           254 LOAD_CONST               6 ('text')
-                           256 BINARY_SUBSCR
-                           266 LOAD_FAST                0 (self)
-                           268 STORE_ATTR              10 (condition_text)
-               
-               103         278 LOAD_FAST                1 (raw)
-                           280 LOAD_CONST               5 ('condition')
-                           282 BINARY_SUBSCR
-                           292 LOAD_CONST               7 ('icon')
-                           294 BINARY_SUBSCR
-                           304 LOAD_FAST                0 (self)
-                           306 STORE_ATTR              11 (condition_icon)
-               
-               104         316 LOAD_FAST                1 (raw)
-                           318 LOAD_CONST               5 ('condition')
-                           320 BINARY_SUBSCR
-                           330 LOAD_CONST               8 ('code')
-                           332 BINARY_SUBSCR
-                           342 LOAD_FAST                0 (self)
-                           344 STORE_ATTR              12 (condition_code)
-               
-               105         354 LOAD_FAST                1 (raw)
-                           356 LOAD_CONST               9 ('wind_mph')
-                           358 BINARY_SUBSCR
-                           368 LOAD_FAST                0 (self)
-                           370 STORE_ATTR              13 (wind_mph)
-               
-               106         380 LOAD_FAST                1 (raw)
-                           382 LOAD_CONST              10 ('wind_kph')
-                           384 BINARY_SUBSCR
-                           394 LOAD_FAST                0 (self)
-                           396 STORE_ATTR              14 (wind_kph)
-               
-               107         406 LOAD_FAST                1 (raw)
-                           408 LOAD_CONST              11 ('wind_degree')
-                           410 BINARY_SUBSCR
-                           420 LOAD_FAST                0 (self)
-                           422 STORE_ATTR              15 (wind_degree)
-               
-               108         432 LOAD_FAST                1 (raw)
-                           434 LOAD_CONST              12 ('wind_dir')
-                           436 BINARY_SUBSCR
-                           446 LOAD_FAST                0 (self)
-                           448 STORE_ATTR              16 (wind_dir)
-               
-               109         458 LOAD_FAST                1 (raw)
-                           460 LOAD_CONST              13 ('pressure_mb')
-                           462 BINARY_SUBSCR
-                           472 LOAD_FAST                0 (self)
-                           474 STORE_ATTR              17 (pressure_mb)
-               
-               110         484 LOAD_FAST                1 (raw)
-                           486 LOAD_CONST              14 ('pressure_in')
-                           488 BINARY_SUBSCR
-                           498 LOAD_FAST                0 (self)
-                           500 STORE_ATTR              18 (pressure_in)
-               
-               111         510 LOAD_FAST                1 (raw)
-                           512 LOAD_CONST              15 ('precip_mm')
-                           514 BINARY_SUBSCR
-                           524 LOAD_FAST                0 (self)
-                           526 STORE_ATTR              19 (precip_mm)
-               
-               112         536 LOAD_FAST                1 (raw)
-                           538 LOAD_CONST              16 ('precip_in')
-                           540 BINARY_SUBSCR
-                           550 LOAD_FAST                0 (self)
-                           552 STORE_ATTR              20 (precip_in)
-               
-               113         562 LOAD_FAST                1 (raw)
-                           564 LOAD_CONST              17 ('humidity')
-                           566 BINARY_SUBSCR
-                           576 LOAD_FAST                0 (self)
-                           578 STORE_ATTR              21 (humidity)
-               
-               114         588 LOAD_FAST                1 (raw)
-                           590 LOAD_CONST              18 ('cloud')
-                           592 BINARY_SUBSCR
-                           602 LOAD_FAST                0 (self)
-                           604 STORE_ATTR              22 (cloud)
-               
-               115         614 LOAD_FAST                1 (raw)
-                           616 LOAD_CONST              19 ('feelslike_c')
-                           618 BINARY_SUBSCR
-                           628 LOAD_FAST                0 (self)
-                           630 STORE_ATTR              23 (feelslike_c)
-               
-               116         640 LOAD_FAST                1 (raw)
-                           642 LOAD_CONST              20 ('feelslike_f')
-                           644 BINARY_SUBSCR
-                           654 LOAD_FAST                0 (self)
-                           656 STORE_ATTR              24 (feelslike_f)
-               
-               117         666 LOAD_FAST                1 (raw)
-                           668 LOAD_CONST              21 ('uv')
-                           670 BINARY_SUBSCR
-                           680 LOAD_FAST                0 (self)
-                           682 STORE_ATTR              25 (uv)
-                           692 LOAD_CONST               0 (None)
-                           694 RETURN_VALUE
+               109         110 LOAD_GLOBAL             11 (NULL + LocationData)
+                           122 LOAD_FAST                1 (raw)
+                           124 LOAD_CONST               1 ('location')
+                           126 BINARY_SUBSCR
+                           136 LOAD_FAST                2 (status)
+                           138 LOAD_FAST                3 (code)
+                           140 PRECALL                  3
+                           144 CALL                     3
+                           154 LOAD_FAST                0 (self)
+                           156 STORE_ATTR               6 (location)
+               
+               110         166 LOAD_FAST                1 (raw)
+                           168 LOAD_CONST               2 ('current')
+                           170 BINARY_SUBSCR
+                           180 STORE_FAST               1 (raw)
+               
+               112         182 LOAD_FAST                1 (raw)
+                           184 LOAD_CONST               3 ('last_updated_epoch')
+                           186 BINARY_SUBSCR
+                           196 LOAD_FAST                0 (self)
+                           198 STORE_ATTR               7 (last_updated_epoch)
+               
+               113         208 LOAD_FAST                1 (raw)
+                           210 LOAD_CONST               4 ('temp_c')
+                           212 BINARY_SUBSCR
+                           222 LOAD_FAST                0 (self)
+                           224 STORE_ATTR               8 (temp_c)
+               
+               114         234 LOAD_FAST                1 (raw)
+                           236 LOAD_CONST               5 ('temp_f')
+                           238 BINARY_SUBSCR
+                           248 LOAD_FAST                0 (self)
+                           250 STORE_ATTR               9 (temp_f)
+               
+               115         260 LOAD_GLOBAL             21 (NULL + bool)
+                           272 LOAD_FAST                1 (raw)
+                           274 LOAD_CONST               6 ('is_day')
+                           276 BINARY_SUBSCR
+                           286 PRECALL                  1
+                           290 CALL                     1
+                           300 LOAD_FAST                0 (self)
+                           302 STORE_ATTR              11 (is_day)
+               
+               116         312 LOAD_FAST                1 (raw)
+                           314 LOAD_CONST               7 ('condition')
+                           316 BINARY_SUBSCR
+                           326 LOAD_CONST               8 ('text')
+                           328 BINARY_SUBSCR
+                           338 LOAD_FAST                0 (self)
+                           340 STORE_ATTR              12 (condition_text)
+               
+               117         350 LOAD_FAST                1 (raw)
+                           352 LOAD_CONST               7 ('condition')
+                           354 BINARY_SUBSCR
+                           364 LOAD_CONST               9 ('icon')
+                           366 BINARY_SUBSCR
+                           376 LOAD_FAST                0 (self)
+                           378 STORE_ATTR              13 (condition_icon)
+               
+               118         388 LOAD_FAST                1 (raw)
+                           390 LOAD_CONST               7 ('condition')
+                           392 BINARY_SUBSCR
+                           402 LOAD_CONST              10 ('code')
+                           404 BINARY_SUBSCR
+                           414 LOAD_FAST                0 (self)
+                           416 STORE_ATTR              14 (condition_code)
+               
+               119         426 LOAD_FAST                1 (raw)
+                           428 LOAD_CONST              11 ('wind_mph')
+                           430 BINARY_SUBSCR
+                           440 LOAD_FAST                0 (self)
+                           442 STORE_ATTR              15 (wind_mph)
+               
+               120         452 LOAD_FAST                1 (raw)
+                           454 LOAD_CONST              12 ('wind_kph')
+                           456 BINARY_SUBSCR
+                           466 LOAD_FAST                0 (self)
+                           468 STORE_ATTR              16 (wind_kph)
+               
+               121         478 LOAD_FAST                1 (raw)
+                           480 LOAD_CONST              13 ('wind_degree')
+                           482 BINARY_SUBSCR
+                           492 LOAD_FAST                0 (self)
+                           494 STORE_ATTR              17 (wind_degree)
+               
+               122         504 LOAD_FAST                1 (raw)
+                           506 LOAD_CONST              14 ('wind_dir')
+                           508 BINARY_SUBSCR
+                           518 LOAD_FAST                0 (self)
+                           520 STORE_ATTR              18 (wind_dir)
+               
+               123         530 LOAD_FAST                1 (raw)
+                           532 LOAD_CONST              15 ('pressure_mb')
+                           534 BINARY_SUBSCR
+                           544 LOAD_FAST                0 (self)
+                           546 STORE_ATTR              19 (pressure_mb)
+               
+               124         556 LOAD_FAST                1 (raw)
+                           558 LOAD_CONST              16 ('pressure_in')
+                           560 BINARY_SUBSCR
+                           570 LOAD_FAST                0 (self)
+                           572 STORE_ATTR              20 (pressure_in)
+               
+               125         582 LOAD_FAST                1 (raw)
+                           584 LOAD_CONST              17 ('precip_mm')
+                           586 BINARY_SUBSCR
+                           596 LOAD_FAST                0 (self)
+                           598 STORE_ATTR              21 (precip_mm)
+               
+               126         608 LOAD_FAST                1 (raw)
+                           610 LOAD_CONST              18 ('precip_in')
+                           612 BINARY_SUBSCR
+                           622 LOAD_FAST                0 (self)
+                           624 STORE_ATTR              22 (precip_in)
+               
+               127         634 LOAD_FAST                1 (raw)
+                           636 LOAD_CONST              19 ('humidity')
+                           638 BINARY_SUBSCR
+                           648 LOAD_FAST                0 (self)
+                           650 STORE_ATTR              23 (humidity)
+               
+               128         660 LOAD_FAST                1 (raw)
+                           662 LOAD_CONST              20 ('cloud')
+                           664 BINARY_SUBSCR
+                           674 LOAD_FAST                0 (self)
+                           676 STORE_ATTR              24 (cloud)
+               
+               129         686 LOAD_FAST                1 (raw)
+                           688 LOAD_CONST              21 ('feelslike_c')
+                           690 BINARY_SUBSCR
+                           700 LOAD_FAST                0 (self)
+                           702 STORE_ATTR              25 (feelslike_c)
+               
+               130         712 LOAD_FAST                1 (raw)
+                           714 LOAD_CONST              22 ('feelslike_f')
+                           716 BINARY_SUBSCR
+                           726 LOAD_FAST                0 (self)
+                           728 STORE_ATTR              26 (feelslike_f)
+               
+               131         738 LOAD_FAST                1 (raw)
+                           740 LOAD_CONST              23 ('uv')
+                           742 BINARY_SUBSCR
+                           752 LOAD_FAST                0 (self)
+                           754 STORE_ATTR              27 (uv)
+                           764 LOAD_CONST               0 (None)
+                           766 RETURN_VALUE
                consts
                   None
+                  'location'
+                  'current'
                   'last_updated_epoch'
                   'temp_c'
                   'temp_f'
                   'is_day'
                   'condition'
                   'text'
                   'icon'
@@ -315,35 +352,219 @@
                   'precip_mm'
                   'precip_in'
                   'humidity'
                   'cloud'
                   'feelslike_c'
                   'feelslike_f'
                   'uv'
-               names      ('super', '__init__', 'status', 'code', 'raw', 'last_updated_epoch', 'temp_c', 'temp_f', 'bool', 'is_day', 'condition_text', 'condition_icon', 'condition_code', 'wind_mph', 'wind_kph', 'wind_degree', 'wind_dir', 'pressure_mb', 'pressure_in', 'precip_mm', 'precip_in', 'humidity', 'cloud', 'feelslike_c', 'feelslike_f', 'uv')
+               names      ('super', '__init__', 'status', 'code', 'raw', 'LocationData', 'location', 'last_updated_epoch', 'temp_c', 'temp_f', 'bool', 'is_day', 'condition_text', 'condition_icon', 'condition_code', 'wind_mph', 'wind_kph', 'wind_degree', 'wind_dir', 'pressure_mb', 'pressure_in', 'precip_mm', 'precip_in', 'humidity', 'cloud', 'feelslike_c', 'feelslike_f', 'uv')
                varnames   ('self', 'raw', 'status', 'code')
                freevars   ('__class__',)
                cellvars   ()
                filename   'build\\bdist.win-amd64\\egg\\weatherly\\responses.py'
                name       '__init__'
-               firstlineno 87
+               firstlineno 97
                lnotab
-                  0x040640020e010e010e011a011a011a0134012601260126011a011a011a
-                  011a011a011a011a011a011a011a011a011a01
+                  0x040640020e010e010e02380110021a011a011a0134012601260126011a
+                  011a011a011a011a011a011a011a011a011a011a011a01
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Dict', 'str', 'Any', 'int', 'Union', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'build\\bdist.win-amd64\\egg\\weatherly\\responses.py'
          name       'CurrentWeatherData'
-         firstlineno 32
-         lnotab 0x0c010436020212fe020302fd020412fc020502fb
+         firstlineno 37
+         lnotab 0x0c01043b020212fe020302fd020412fc020502fb
       'CurrentWeatherData'
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 8
+         flags     : 0
+         code
+            0x970065005a0164005a0264015a03640265046505650666021900000000
+            000000000064036507640465086507640566021900000000000000000064
+            0664056608640784045a0964055300
+         133           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('LocationData')
+                       8 STORE_NAME               2 (__qualname__)
+         
+         134          10 LOAD_CONST               1 ('\n    Location data, returned with most requests.\n    \n    Attributes\n    --------------\n    raw: Dict[:class:`str`, Any]\n        Raw response in a JSON-like format (converted to a python dictionary)\n    status: :class:`int`\n        HTTP status of the response. 200 is OK, and is the most common status.\n    code: Union[:class:`int`, None]\n        Response code. In some cases this can be ``None``\n    id: Optional[:class:`int`]\n        A specific ID of the location. Can be ``None``\n    name: :class:`str`\n        Name of the location (e.g. London)\n    region: :class:`str`\n        A region of the location\n    country: :class:`str`\n        Country where the location is\n    latitude: :class:`float`\n        Latitude coordinate of the location\n    longitude: :class:`float`\n        Longitude coordinate of the location\n    timezone_id: Optional[:class:`str`]\n        Timezone ID of the location (e.g. Europe/London). Could be ``None`` when using the Search/Autocomplete API.\n    localtime_epoch: Optional[:class:`int`]\n        Local time of the location as a timestamp\n    localtime_formatted: Optional[:class:`str`]\n        Formatted local time of the location\n    ')
+                      12 STORE_NAME               3 (__doc__)
+         
+         164          14 LOAD_CONST               2 ('raw')
+         
+         166          16 LOAD_NAME                4 (Dict)
+                      18 LOAD_NAME                5 (str)
+                      20 LOAD_NAME                6 (Any)
+                      22 BUILD_TUPLE              2
+                      24 BINARY_SUBSCR
+         
+         164          34 LOAD_CONST               3 ('status')
+         
+         167          36 LOAD_NAME                7 (int)
+         
+         164          38 LOAD_CONST               4 ('code')
+         
+         168          40 LOAD_NAME                8 (Union)
+                      42 LOAD_NAME                7 (int)
+                      44 LOAD_CONST               5 (None)
+                      46 BUILD_TUPLE              2
+                      48 BINARY_SUBSCR
+         
+         164          58 LOAD_CONST               6 ('return')
+         
+         169          60 LOAD_CONST               5 (None)
+         
+         164          62 BUILD_TUPLE              8
+                      64 LOAD_CONST               7 (<code object __init__, file "build\bdist.win-amd64\egg\weatherly\responses.py", line 164>)
+                      66 MAKE_FUNCTION            4 (annotations)
+                      68 STORE_NAME               9 (__init__)
+                      70 LOAD_CONST               5 (None)
+                      72 RETURN_VALUE
+         consts
+            'LocationData'
+            '\n    Location data, returned with most requests.\n    \n    Attributes\n    --------------\n    raw: Dict[:class:`str`, Any]\n        Raw response in a JSON-like format (converted to a python dictionary)\n    status: :class:`int`\n        HTTP status of the response. 200 is OK, and is the most common status.\n    code: Union[:class:`int`, None]\n        Response code. In some cases this can be ``None``\n    id: Optional[:class:`int`]\n        A specific ID of the location. Can be ``None``\n    name: :class:`str`\n        Name of the location (e.g. London)\n    region: :class:`str`\n        A region of the location\n    country: :class:`str`\n        Country where the location is\n    latitude: :class:`float`\n        Latitude coordinate of the location\n    longitude: :class:`float`\n        Longitude coordinate of the location\n    timezone_id: Optional[:class:`str`]\n        Timezone ID of the location (e.g. Europe/London). Could be ``None`` when using the Search/Autocomplete API.\n    localtime_epoch: Optional[:class:`int`]\n        Local time of the location as a timestamp\n    localtime_formatted: Optional[:class:`str`]\n        Formatted local time of the location\n    '
+            'raw'
+            'status'
+            'code'
+            None
+            'return'
+            code
+               argcount  : 4
+               nlocals   : 4
+               stacksize : 4
+               flags     : 3
+               code
+                  0x97007c017c005f0000000000000000007c027c005f0100000000000000
+                  007c037c005f0200000000000000007c01a0030000000000000000000000
+                  00000000000000000064016400a6020000ab0200000000000000007c005f
+                  0400000000000000007c016402190000000000000000007c005f05000000
+                  00000000007c016403190000000000000000007c005f0600000000000000
+                  007c016404190000000000000000007c005f0700000000000000007c0164
+                  05190000000000000000007c005f0800000000000000007c016406190000
+                  000000000000007c005f0900000000000000007c01a00300000000000000
+                  0000000000000000000000000064076400a6020000ab0200000000000000
+                  007c005f0a00000000000000007c01a00300000000000000000000000000
+                  000000000000006408a6010000ab0100000000000000007c005f0b000000
+                  00000000007c01a003000000000000000000000000000000000000000064
+                  096400a6020000ab0200000000000000007c005f0c000000000000000064
+                  005300
+               164           0 RESUME                   0
+               
+               170           2 LOAD_FAST                1 (raw)
+                             4 LOAD_FAST                0 (self)
+                             6 STORE_ATTR               0 (raw)
+               
+               171          16 LOAD_FAST                2 (status)
+                            18 LOAD_FAST                0 (self)
+                            20 STORE_ATTR               1 (status)
+               
+               172          30 LOAD_FAST                3 (code)
+                            32 LOAD_FAST                0 (self)
+                            34 STORE_ATTR               2 (code)
+               
+               174          44 LOAD_FAST                1 (raw)
+                            46 LOAD_METHOD              3 (get)
+                            68 LOAD_CONST               1 ('id')
+                            70 LOAD_CONST               0 (None)
+                            72 PRECALL                  2
+                            76 CALL                     2
+                            86 LOAD_FAST                0 (self)
+                            88 STORE_ATTR               4 (id)
+               
+               175          98 LOAD_FAST                1 (raw)
+                           100 LOAD_CONST               2 ('name')
+                           102 BINARY_SUBSCR
+                           112 LOAD_FAST                0 (self)
+                           114 STORE_ATTR               5 (name)
+               
+               176         124 LOAD_FAST                1 (raw)
+                           126 LOAD_CONST               3 ('region')
+                           128 BINARY_SUBSCR
+                           138 LOAD_FAST                0 (self)
+                           140 STORE_ATTR               6 (region)
+               
+               177         150 LOAD_FAST                1 (raw)
+                           152 LOAD_CONST               4 ('country')
+                           154 BINARY_SUBSCR
+                           164 LOAD_FAST                0 (self)
+                           166 STORE_ATTR               7 (country)
+               
+               178         176 LOAD_FAST                1 (raw)
+                           178 LOAD_CONST               5 ('lat')
+                           180 BINARY_SUBSCR
+                           190 LOAD_FAST                0 (self)
+                           192 STORE_ATTR               8 (latitude)
+               
+               179         202 LOAD_FAST                1 (raw)
+                           204 LOAD_CONST               6 ('lon')
+                           206 BINARY_SUBSCR
+                           216 LOAD_FAST                0 (self)
+                           218 STORE_ATTR               9 (longitude)
+               
+               180         228 LOAD_FAST                1 (raw)
+                           230 LOAD_METHOD              3 (get)
+                           252 LOAD_CONST               7 ('tz_id')
+                           254 LOAD_CONST               0 (None)
+                           256 PRECALL                  2
+                           260 CALL                     2
+                           270 LOAD_FAST                0 (self)
+                           272 STORE_ATTR              10 (timezone_id)
+               
+               181         282 LOAD_FAST                1 (raw)
+                           284 LOAD_METHOD              3 (get)
+                           306 LOAD_CONST               8 ('localtime_epoch')
+                           308 PRECALL                  1
+                           312 CALL                     1
+                           322 LOAD_FAST                0 (self)
+                           324 STORE_ATTR              11 (localtime_epoch)
+               
+               182         334 LOAD_FAST                1 (raw)
+                           336 LOAD_METHOD              3 (get)
+                           358 LOAD_CONST               9 ('localtime')
+                           360 LOAD_CONST               0 (None)
+                           362 PRECALL                  2
+                           366 CALL                     2
+                           376 LOAD_FAST                0 (self)
+                           378 STORE_ATTR              12 (localtime_formatted)
+                           388 LOAD_CONST               0 (None)
+                           390 RETURN_VALUE
+               consts
+                  None
+                  'id'
+                  'name'
+                  'region'
+                  'country'
+                  'lat'
+                  'lon'
+                  'tz_id'
+                  'localtime_epoch'
+                  'localtime'
+               names      ('raw', 'status', 'code', 'get', 'id', 'name', 'region', 'country', 'latitude', 'longitude', 'timezone_id', 'localtime_epoch', 'localtime_formatted')
+               varnames   ('self', 'raw', 'status', 'code')
+               freevars   ()
+               cellvars   ()
+               filename   'build\\bdist.win-amd64\\egg\\weatherly\\responses.py'
+               name       '__init__'
+               firstlineno 164
+               lnotab 0x02060e010e010e0236011a011a011a011a011a0136013401
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'Dict', 'str', 'Any', 'int', 'Union', '__init__')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   'build\\bdist.win-amd64\\egg\\weatherly\\responses.py'
+         name       'LocationData'
+         firstlineno 133
+         lnotab 0x0a01041e020212fe020302fd020412fc020502fb
+      'LocationData'
       None
-   names      ('__doc__', 'abc', 'CurrentWeather', 'typing', 'Dict', 'Any', 'Union', 'CurrentWeatherData')
+   names      ('__doc__', 'abc', 'CurrentWeather', 'LocationModel', 'typing', 'Dict', 'Any', 'Union', '__all__', 'CurrentWeatherData', 'LocationData')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'build\\bdist.win-amd64\\egg\\weatherly\\responses.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020104180c011406
+   lnotab 0x00ff020104181001140604051c60
```

## weatherly/__pycache__/utils.cpython-311.pyc

### Python bytecode

```diff
@@ -1,21 +1,22 @@
 magic:    0xa70d0d0a
-moddate:  0xdaf03c64 (Mon Apr 17 07:10:18 2023 UTC)
-files sz: 2640
+moddate:  0x2c304264 (Fri Apr 21 06:41:48 2023 UTC)
+files sz: 2855
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 5
+   stacksize : 8
    flags     : 0
    code
       0x970064005a00640164026c016d025a026d035a036d045a040100640364
       046c056d065a060100640565026507650366021900000000000000000064
-      0665076604640784045a08650464086507640664096604640a8404a60000
-      00ab0000000000000000005a0964086507640665076604640b84045a0964
-      095300
+      0665076604640784045a086504640f64096507640a65096406640b660664
+      0c8405a6000000ab0000000000000000005a0a6504640f64096507640a65
+      09640665066606640d8405a6000000ab0000000000000000005a0a640f64
+      096507640a6509640665076606640e84055a0a640b5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('\nMIT License\n\nCopyright (c) 2023 Konrad (@konradsic)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n')
                  4 STORE_NAME               0 (__doc__)
    
     25           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('Dict', 'Any', 'overload'))
@@ -46,37 +47,61 @@
                 62 BUILD_TUPLE              4
                 64 LOAD_CONST               7 (<code object parse_kwargs_to_urlargs, file "build\bdist.win-amd64\egg\weatherly\utils.py", line 32>)
                 66 MAKE_FUNCTION            4 (annotations)
                 68 STORE_NAME               8 (parse_kwargs_to_urlargs)
    
     57          70 LOAD_NAME                4 (overload)
    
-    58          72 LOAD_CONST               8 ('lang')
-                74 LOAD_NAME                7 (str)
-                76 LOAD_CONST               6 ('return')
-                78 LOAD_CONST               9 (None)
-                80 BUILD_TUPLE              4
-                82 LOAD_CONST              10 (<code object find_language, file "build\bdist.win-amd64\egg\weatherly\utils.py", line 57>)
-                84 MAKE_FUNCTION            4 (annotations)
-   
-    57          86 PRECALL                  0
-                90 CALL                     0
-   
-    58         100 STORE_NAME               9 (find_language)
-   
-    61         102 LOAD_CONST               8 ('lang')
-               104 LOAD_NAME                7 (str)
-               106 LOAD_CONST               6 ('return')
-               108 LOAD_NAME                7 (str)
-               110 BUILD_TUPLE              4
-               112 LOAD_CONST              11 (<code object find_language, file "build\bdist.win-amd64\egg\weatherly\utils.py", line 61>)
-               114 MAKE_FUNCTION            4 (annotations)
-               116 STORE_NAME               9 (find_language)
-               118 LOAD_CONST               9 (None)
-               120 RETURN_VALUE
+    58          72 LOAD_CONST              15 ((False,))
+                74 LOAD_CONST               9 ('lang')
+                76 LOAD_NAME                7 (str)
+                78 LOAD_CONST              10 ('asobj')
+                80 LOAD_NAME                9 (bool)
+                82 LOAD_CONST               6 ('return')
+                84 LOAD_CONST              11 (None)
+                86 BUILD_TUPLE              6
+                88 LOAD_CONST              12 (<code object find_language, file "build\bdist.win-amd64\egg\weatherly\utils.py", line 57>)
+                90 MAKE_FUNCTION            5 (defaults, annotations)
+   
+    57          92 PRECALL                  0
+                96 CALL                     0
+   
+    58         106 STORE_NAME              10 (find_language)
+   
+    61         108 LOAD_NAME                4 (overload)
+   
+    62         110 LOAD_CONST              15 ((False,))
+               112 LOAD_CONST               9 ('lang')
+               114 LOAD_NAME                7 (str)
+               116 LOAD_CONST              10 ('asobj')
+               118 LOAD_NAME                9 (bool)
+               120 LOAD_CONST               6 ('return')
+               122 LOAD_NAME                6 (Languages)
+               124 BUILD_TUPLE              6
+               126 LOAD_CONST              13 (<code object find_language, file "build\bdist.win-amd64\egg\weatherly\utils.py", line 61>)
+               128 MAKE_FUNCTION            5 (defaults, annotations)
+   
+    61         130 PRECALL                  0
+               134 CALL                     0
+   
+    62         144 STORE_NAME              10 (find_language)
+   
+    65         146 LOAD_CONST              15 ((False,))
+               148 LOAD_CONST               9 ('lang')
+               150 LOAD_NAME                7 (str)
+               152 LOAD_CONST              10 ('asobj')
+               154 LOAD_NAME                9 (bool)
+               156 LOAD_CONST               6 ('return')
+               158 LOAD_NAME                7 (str)
+               160 BUILD_TUPLE              6
+               162 LOAD_CONST              14 (<code object find_language, file "build\bdist.win-amd64\egg\weatherly\utils.py", line 65>)
+               164 MAKE_FUNCTION            5 (defaults, annotations)
+               166 STORE_NAME              10 (find_language)
+               168 LOAD_CONST              11 (None)
+               170 RETURN_VALUE
    consts
       '\nMIT License\n\nCopyright (c) 2023 Konrad (@konradsic)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n'
       0
       ('Dict', 'Any', 'overload')
       1
       ('Languages',)
       'kwargs'
@@ -148,130 +173,162 @@
          varnames   ('kwargs', 'args_string', 'first', 'k', 'v')
          freevars   ()
          cellvars   ()
          filename   'build\\bdist.win-amd64\\egg\\weatherly\\utils.py'
          name       'parse_kwargs_to_urlargs'
          firstlineno 32
          lnotab 0x020f080204010402320120010601
+      False
       'lang'
+      'asobj'
       None
       code
-         argcount  : 1
-         nlocals   : 1
+         argcount  : 2
+         nlocals   : 2
          stacksize : 1
          flags     : 3
          code 0x970064005300
           57           0 RESUME                   0
          
           59           2 LOAD_CONST               0 (None)
                        4 RETURN_VALUE
          consts
             None
          names      ()
-         varnames   ('lang',)
+         varnames   ('lang', 'asobj')
          freevars   ()
          cellvars   ()
          filename   'build\\bdist.win-amd64\\egg\\weatherly\\utils.py'
          name       'find_language'
          firstlineno 57
          lnotab 0x0202
       code
-         argcount  : 1
+         argcount  : 2
+         nlocals   : 2
+         stacksize : 1
+         flags     : 3
+         code 0x970064005300
+          61           0 RESUME                   0
+         
+          63           2 LOAD_CONST               0 (None)
+                       4 RETURN_VALUE
+         consts
+            None
+         names      ()
+         varnames   ('lang', 'asobj')
+         freevars   ()
+         cellvars   ()
+         filename   'build\\bdist.win-amd64\\egg\\weatherly\\utils.py'
+         name       'find_language'
+         firstlineno 61
+         lnotab 0x0202
+      code
+         argcount  : 2
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
-            0x970064017d017401000000000000000000007c00740200000000000000
-            000000a6020000ab020000000000000000721009007c006a020000000000
-            0000005300230001005900640153007803590077017c00a0030000000000
-            000000000000000000000000000000a6000000ab0000000000000000007d
-            0074020000000000000000000044005d337d027c026a0400000000000000
-            00a0030000000000000000000000000000000000000000a6000000ab0000
-            000000000000007c006b0200000000730b7c026a0200000000000000007c
-            006b020000000072097c006a0200000000000000007d0101006e018c347c
-            015300
-          61           0 RESUME                   0
-         
-          75           2 LOAD_CONST               1 (None)
-                       4 STORE_FAST               1 (lang_code)
+            0x97007401000000000000000000007c00740200000000000000000000a6
+            020000ab020000000000000000721409007c0172027c0053007c006a0200
+            000000000000005300230001005900640153007803590077017c00a00300
+            00000000000000000000000000000000000000a6000000ab000000000000
+            0000007d0074020000000000000000000044005d397d027c026a04000000
+            0000000000a0030000000000000000000000000000000000000000a60000
+            00ab0000000000000000007c006b0200000000730b7c026a020000000000
+            0000007c006b0200000000720f7c0172047c026302010053007c026a0200
+            000000000000006302010053008c3a64015300
+          65           0 RESUME                   0
+         
+          80           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                      14 LOAD_FAST                0 (lang)
+                      16 LOAD_GLOBAL              2 (Languages)
+                      28 PRECALL                  2
+                      32 CALL                     2
+                      42 POP_JUMP_FORWARD_IF_FALSE    20 (to 84)
+         
+          81          44 NOP
+         
+          82          46 LOAD_FAST                1 (asobj)
+                      48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
+                      50 LOAD_FAST                0 (lang)
+                      52 RETURN_VALUE
+         
+          83     >>   54 LOAD_FAST                0 (lang)
+                      56 LOAD_ATTR                2 (value)
+                      66 RETURN_VALUE
+                 >>   68 PUSH_EXC_INFO
+         
+          84          70 POP_TOP
+         
+          85          72 POP_EXCEPT
+                      74 LOAD_CONST               1 (None)
+                      76 RETURN_VALUE
+                 >>   78 COPY                     3
+                      80 POP_EXCEPT
+                      82 RERAISE                  1
+         
+          87     >>   84 LOAD_FAST                0 (lang)
+                      86 LOAD_METHOD              3 (lower)
+                     108 PRECALL                  0
+                     112 CALL                     0
+                     122 STORE_FAST               0 (lang)
+         
+          89         124 LOAD_GLOBAL              2 (Languages)
+                     136 GET_ITER
+                 >>  138 FOR_ITER                57 (to 254)
+                     140 STORE_FAST               2 (language)
+         
+          90         142 LOAD_FAST                2 (language)
+                     144 LOAD_ATTR                4 (name)
+                     154 LOAD_METHOD              3 (lower)
+                     176 PRECALL                  0
+                     180 CALL                     0
+                     190 LOAD_FAST                0 (lang)
+                     192 COMPARE_OP               2 (==)
+                     198 POP_JUMP_FORWARD_IF_TRUE    11 (to 222)
+                     200 LOAD_FAST                2 (language)
+                     202 LOAD_ATTR                2 (value)
+                     212 LOAD_FAST                0 (lang)
+                     214 COMPARE_OP               2 (==)
+                     220 POP_JUMP_FORWARD_IF_FALSE    15 (to 252)
+         
+          91     >>  222 LOAD_FAST                1 (asobj)
+                     224 POP_JUMP_FORWARD_IF_FALSE     4 (to 234)
+                     226 LOAD_FAST                2 (language)
+                     228 SWAP                     2
+                     230 POP_TOP
+                     232 RETURN_VALUE
+         
+          92     >>  234 LOAD_FAST                2 (language)
+                     236 LOAD_ATTR                2 (value)
+                     246 SWAP                     2
+                     248 POP_TOP
+                     250 RETURN_VALUE
          
-          77           6 LOAD_GLOBAL              1 (NULL + isinstance)
-                      18 LOAD_FAST                0 (lang)
-                      20 LOAD_GLOBAL              2 (Languages)
-                      32 PRECALL                  2
-                      36 CALL                     2
-                      46 POP_JUMP_FORWARD_IF_FALSE    16 (to 80)
-         
-          78          48 NOP
-         
-          79          50 LOAD_FAST                0 (lang)
-                      52 LOAD_ATTR                2 (value)
-                      62 RETURN_VALUE
-                 >>   64 PUSH_EXC_INFO
-         
-          80          66 POP_TOP
-         
-          81          68 POP_EXCEPT
-                      70 LOAD_CONST               1 (None)
-                      72 RETURN_VALUE
-                 >>   74 COPY                     3
-                      76 POP_EXCEPT
-                      78 RERAISE                  1
-         
-          83     >>   80 LOAD_FAST                0 (lang)
-                      82 LOAD_METHOD              3 (lower)
-                     104 PRECALL                  0
-                     108 CALL                     0
-                     118 STORE_FAST               0 (lang)
-         
-          85         120 LOAD_GLOBAL              2 (Languages)
-                     132 GET_ITER
-                 >>  134 FOR_ITER                51 (to 238)
-                     136 STORE_FAST               2 (language)
-         
-          86         138 LOAD_FAST                2 (language)
-                     140 LOAD_ATTR                4 (name)
-                     150 LOAD_METHOD              3 (lower)
-                     172 PRECALL                  0
-                     176 CALL                     0
-                     186 LOAD_FAST                0 (lang)
-                     188 COMPARE_OP               2 (==)
-                     194 POP_JUMP_FORWARD_IF_TRUE    11 (to 218)
-                     196 LOAD_FAST                2 (language)
-                     198 LOAD_ATTR                2 (value)
-                     208 LOAD_FAST                0 (lang)
-                     210 COMPARE_OP               2 (==)
-                     216 POP_JUMP_FORWARD_IF_FALSE     9 (to 236)
-         
-          87     >>  218 LOAD_FAST                0 (lang)
-                     220 LOAD_ATTR                2 (value)
-                     230 STORE_FAST               1 (lang_code)
+          90     >>  252 JUMP_BACKWARD           58 (to 138)
          
-          88         232 POP_TOP
-                     234 JUMP_FORWARD             1 (to 238)
-         
-          86     >>  236 JUMP_BACKWARD           52 (to 134)
-         
-          90     >>  238 LOAD_FAST                1 (lang_code)
-                     240 RETURN_VALUE
+          94     >>  254 LOAD_CONST               1 (None)
+                     256 RETURN_VALUE
          ExceptionTable:
-           50 to 60 -> 64 [0]
-           64 to 66 -> 74 [1] lasti
+           46 to 50 -> 68 [0]
+           54 to 64 -> 68 [0]
+           68 to 70 -> 78 [1] lasti
          consts
-            '\n    Used to find language code from available languages.\n\n    Paremeters\n    ----------\n    lang: :class:`str`\n        A language you want to search for\n\n    Returns\n    -------\n    Union[:class:`str`, None]\n        Language code, could be ``None``\n    '
+            '\n    Used to find language code from available languages.\n\n    Paremeters\n    ----------\n    lang: :class:`str`\n        A language you want to search for\n\n    Returns\n    -------\n    Union[:class:`str`, :class:`Languages`, None]\n        Language code, could be ``None``, could be a :class:`Languages` enum.\n    '
             None
          names      ('isinstance', 'Languages', 'value', 'lower', 'name')
-         varnames   ('lang', 'lang_code', 'language')
+         varnames   ('lang', 'asobj', 'language')
          freevars   ()
          cellvars   ()
          filename   'build\\bdist.win-amd64\\egg\\weatherly\\utils.py'
          name       'find_language'
-         firstlineno 61
-         lnotab 0x020e04022a010201100102010c022802120150010e0104fe0204
-   names      ('__doc__', 'typing', 'Dict', 'Any', 'overload', 'enums', 'Languages', 'str', 'parse_kwargs_to_urlargs', 'find_language')
+         firstlineno 65
+         lnotab 0x020f2a0102010801100102010c022802120150010c0112fe0204
+      (False,)
+   names      ('__doc__', 'typing', 'Dict', 'Any', 'overload', 'enums', 'Languages', 'str', 'parse_kwargs_to_urlargs', 'bool', 'find_language')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'build\\bdist.win-amd64\\egg\\weatherly\\utils.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201041814050c02201902010eff0e010203
+   lnotab 0x00ff0201041814050c022019020114ff0e010203020114ff0e010203
```

## weatherly/api/client.py

```diff
@@ -20,15 +20,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from .core import BaseAPIClient
 from ..enums import Languages
-from ..responses import CurrentWeatherData
+from ..responses import CurrentWeatherData, LocationData
 from ..errors import (
     WeatherAPIException,
     NoLocationFound,
     InvalidAPIKey,
     APILimitExceeded,
     APIKeyDisabled,
     AccessDenied,
@@ -39,15 +39,16 @@
 )
 
 from typing import (
     Any,
     Literal,
     Dict,
     Optional,
-    Union
+    Union,
+    List
 )
 
 WEATHERAPI_BASE_URL = "http://api.weatherapi.com/v1/"
 
 __all__ = (
     "WeatherAPIClient",
 )
@@ -58,15 +59,15 @@
 
     Parameters
     ----------
     api_key: :class:`str`
         API Key used to authenticate when sending requests
     lang: Optional[ Union[:class:`str`, :class:`Languages`] ]
         Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
-        To get a list of languages visit :class:`Languages`.
+        To get a list of languages visit :class:`Languages`. If ``None`` then the default language is used (English)
     dt: Optional[:class:`int`]
         Restrict date output for Forecast and History API method. (Required for History and Future API)
     end_dt: Optional[:class:`int`]
         Restrict date output for History API method. Only works for API on Pro plan and above. (Available for History API)
     hour: Optional[:class:`int`]
         Restricting forecast or history output to a specific hour in a given day.
     aqi: Literal["yes", "no"]
@@ -85,44 +86,84 @@
         hour: Optional[int] = None,
         aqi: Literal["yes", "no"] = "no",
         tides: Literal["yes", "no"] = "no",
         **kwargs: Dict[str, Any]
     ) -> None:
         lang_code = None
         if lang is not None: 
-            lang_code = utils.find_language(lang)
+            lang_code = utils.find_language(lang, asobj=True)
         opts = {
             "key": api_key,
             **kwargs
         }
-        if lang_code: opts.update(lang=lang_code)
+        if lang_code: opts.update(lang = lang_code.value if lang_code is not None else None)
 
         super().__init__(base_url=WEATHERAPI_BASE_URL,
                          default_options=opts)
         
         self.dt = dt
         self.end_dt = end_dt
         self.hour = hour
         self.aqi = aqi
         self.tides = tides
         self.kwargs = kwargs
+        self.lang = Languages(lang_code) if lang_code else None
+    
     
     def _call_request(self, endpoint: str, options: Dict[str, Any]) -> Dict[str, Any]:
         """Private method used to make requests to WeatherAPI"""
         final_options = self.default_options.copy()
 
         for k,v in final_options.items(): # check - remove NoneType values
             if v is None: del final_options[k]
         # add options to final_options
         for k,v in options.items():
             if v is not None: final_options[k] = v
 
         resp = self._request(endpoint, **final_options)
+
+        if not resp[1].status_code < 400:
+            # raise errors yay
+            error_data = resp[0]["error"]
+            code = error_data["code"]
+            status = resp[1].status_code
+            msg = error_data["message"]
+
+            if code == 1006: raise NoLocationFound(status, code, msg)
+            elif code == 2006: raise InvalidAPIKey(status, code, msg)
+            elif code == 2007: raise APILimitExceeded(status, code, msg)
+            elif code == 2008: raise APIKeyDisabled(status, code, msg)
+            elif code == 2009: raise AccessDenied(status, code, msg)
+            elif code == 9999: raise InternalApplicationError(status, code, msg)
+            else: raise WeatherAPIException(status, code, msg)
+
         return resp
 
+    def set_language(self, lang: Union[str, Languages]) -> Union[Languages, None]:
+        """
+        Set client's language when requesting data.
+        
+        Parameters
+        -----------
+        lang: Union[:class:`str`, :class:`Languages`]
+            Language to set. Can be either a string that is lanuage's name or code or a :class:`Languages` enum object.
+            
+        Returns
+        ---------
+        :class:`bool`
+            A boolean indicating whether the language was successfully set. If it's ``False``, then something went wrong, probably because of the wrong ``lang`` value.
+        """
+        lang_class = utils.find_language(lang, asobj=True)
+        if not lang_class:
+            self.lang = None
+            return False
+
+        self.lang = lang_class 
+        return True
+
     def get_current_weather(self, 
         query: str,
         lang: Optional[Union[str, Languages]] = None,
         aqi: Literal["yes", "no", None] = None,
         **kwargs: Dict[str, Any]
     ) -> CurrentWeatherData:
         """
@@ -131,42 +172,89 @@
         Parameters
         ----------
         query: :class:`str`
             Query string - location you want to get weather data for
         lang: Optional[Union[:class:`str`, Languages]]
             Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
             To get a list of languages visit :class:`Languages`.
-        aqi: Literal["yes", "no"]
-            Enable/Disable Air Quality data in forecast API output. Defaults to "no".
+        aqi: Literal["yes", "no", None]
+            Enable/Disable Air Quality data in forecast API output. If nothing is passes, then it defaults to client default value.
         kwargs: Dict[:class:`str`, Any]
             Additional keyword arguments to request
 
         Returns
         -------
         :class:`CurrentWeatherData`
             Current weather data class
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when no location for given query was found
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
         """
         options = {
             "aqi": aqi or self.aqi,
             "q": query,
             **kwargs
         }
         if lang is not None: options["lang"] = lang
         resp = self._call_request("current.json", options)
-        
-        if not resp[1].status_code < 400:
-            # raise errors yay
-            error_data = resp[0]["error"]
-            code = error_data["code"]
-            status = resp[1].status_code
-            msg = error_data["message"]
 
-            if code == 1006: raise NoLocationFound(status, code, msg)
-            elif code == 2006: raise InvalidAPIKey(status, code, msg)
-            elif code == 2007: raise APILimitExceeded(status, code, msg)
-            elif code == 2008: raise APIKeyDisabled(status, code, msg)
-            elif code == 2009: raise AccessDenied(status, code, msg)
-            elif code == 9999: raise InternalApplicationError(status, code, msg)
-            else: raise WeatherAPIException(status, code, msg)
+        weather = CurrentWeatherData(resp[0], resp[1].status_code, None)
+        return weather
+
+    def get_locations(self, query: str):
+        """
+        Get locations for given query
+
+        Parameters
+        ---------------
+        query: :class:`str`
+            Query string, a location you are searching for
+
+        Returns
+        -----------
+        List[:class:`LocationData`]
+            A list of :class:`LocationData` classes.
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when no location for given query was found
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
+        """
+        resp = self._call_request("search.json",{"q": query})
 
-        weather = CurrentWeatherData(resp[0]["current"], resp[1].status_code, None)
-        return weather
+        locations = []
+        for loc in resp[0]:
+            locations.append(LocationData(loc, resp[1].status_code, None))
+        return locations
+    
+    def __str__(self):
+        return f"<{self.__class__.__name__} api_key={self.default_options['key']} lang={self.lang}>"
+    
+    def __repr__(self):
+        return repr(f"<{self.__class__.__name__} api_key={self.default_options['key']} lang={self.lang}>")
+
```

## weatherly/api/core.py

```diff
@@ -47,15 +47,15 @@
     Represents a base API client that can handle requests. Used as a base class for ``WeatherAPIClient``
     
     Parameters
     ----------
     base_url: :class:`str`
         An URL that will be used as a base for requests.
     default_options: Optional[Dict[:class:`str`, Any]]
-        Default options for request that will be automatically added.
+        Default options for requests made by the client that will be automatically added.
     """
     def __init__(
         self,
         base_url: str,
         default_options: Optional[Dict[str, Any]]
     ) -> None:
         self.url = base_url
```

## weatherly/api/__pycache__/client.cpython-311.pyc

### Python bytecode

```diff
@@ -1,22 +1,22 @@
 magic:    0xa70d0d0a
-moddate:  0xdaf03c64 (Mon Apr 17 07:10:18 2023 UTC)
-files sz: 6410
+moddate:  0x16314264 (Fri Apr 21 06:45:42 2023 UTC)
+files sz: 9793
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a00640164026c016d025a020100640364046c036d045a0401
-      00640364056c056d065a060100640364066c076d085a086d095a096d0a5a
-      0a6d0b5a0b6d0c5a0c6d0d5a0d6d0e5a0e0100640364076c0f6d105a1001
-      00640864096c116d125a126d135a136d145a146d155a156d165a16010064
-      0a5a17640b5a1802004700640c8400640d6502a6030000ab030000000000
-      0000005a19640e5300
+      00640364056c056d065a066d075a070100640364066c086d095a096d0a5a
+      0a6d0b5a0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f0100640364076c106d
+      115a110100640864096c126d135a136d145a146d155a156d165a166d175a
+      176d185a180100640a5a19640b5a1a02004700640c8400640d6502a60300
+      00ab0300000000000000005a1b640e5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('\nMIT License\n\nCopyright (c) 2023 Konrad (@konradsic)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n')
                  4 STORE_NAME               0 (__doc__)
    
     25           6 LOAD_CONST               1 (1)
                  8 LOAD_CONST               2 (('BaseAPIClient',))
@@ -29,263 +29,301 @@
                 20 LOAD_CONST               4 (('Languages',))
                 22 IMPORT_NAME              3 (enums)
                 24 IMPORT_FROM              4 (Languages)
                 26 STORE_NAME               4 (Languages)
                 28 POP_TOP
    
     27          30 LOAD_CONST               3 (2)
-                32 LOAD_CONST               5 (('CurrentWeatherData',))
+                32 LOAD_CONST               5 (('CurrentWeatherData', 'LocationData'))
                 34 IMPORT_NAME              5 (responses)
                 36 IMPORT_FROM              6 (CurrentWeatherData)
                 38 STORE_NAME               6 (CurrentWeatherData)
-                40 POP_TOP
+                40 IMPORT_FROM              7 (LocationData)
+                42 STORE_NAME               7 (LocationData)
+                44 POP_TOP
    
-    28          42 LOAD_CONST               3 (2)
-                44 LOAD_CONST               6 (('WeatherAPIException', 'NoLocationFound', 'InvalidAPIKey', 'APILimitExceeded', 'APIKeyDisabled', 'AccessDenied', 'InternalApplicationError'))
-                46 IMPORT_NAME              7 (errors)
-                48 IMPORT_FROM              8 (WeatherAPIException)
-                50 STORE_NAME               8 (WeatherAPIException)
-                52 IMPORT_FROM              9 (NoLocationFound)
-                54 STORE_NAME               9 (NoLocationFound)
-                56 IMPORT_FROM             10 (InvalidAPIKey)
-                58 STORE_NAME              10 (InvalidAPIKey)
-                60 IMPORT_FROM             11 (APILimitExceeded)
-                62 STORE_NAME              11 (APILimitExceeded)
-                64 IMPORT_FROM             12 (APIKeyDisabled)
-                66 STORE_NAME              12 (APIKeyDisabled)
-                68 IMPORT_FROM             13 (AccessDenied)
-                70 STORE_NAME              13 (AccessDenied)
-                72 IMPORT_FROM             14 (InternalApplicationError)
-                74 STORE_NAME              14 (InternalApplicationError)
-                76 POP_TOP
+    28          46 LOAD_CONST               3 (2)
+                48 LOAD_CONST               6 (('WeatherAPIException', 'NoLocationFound', 'InvalidAPIKey', 'APILimitExceeded', 'APIKeyDisabled', 'AccessDenied', 'InternalApplicationError'))
+                50 IMPORT_NAME              8 (errors)
+                52 IMPORT_FROM              9 (WeatherAPIException)
+                54 STORE_NAME               9 (WeatherAPIException)
+                56 IMPORT_FROM             10 (NoLocationFound)
+                58 STORE_NAME              10 (NoLocationFound)
+                60 IMPORT_FROM             11 (InvalidAPIKey)
+                62 STORE_NAME              11 (InvalidAPIKey)
+                64 IMPORT_FROM             12 (APILimitExceeded)
+                66 STORE_NAME              12 (APILimitExceeded)
+                68 IMPORT_FROM             13 (APIKeyDisabled)
+                70 STORE_NAME              13 (APIKeyDisabled)
+                72 IMPORT_FROM             14 (AccessDenied)
+                74 STORE_NAME              14 (AccessDenied)
+                76 IMPORT_FROM             15 (InternalApplicationError)
+                78 STORE_NAME              15 (InternalApplicationError)
+                80 POP_TOP
    
-    37          78 LOAD_CONST               3 (2)
-                80 LOAD_CONST               7 (('utils',))
-                82 IMPORT_NAME             15
-                84 IMPORT_FROM             16 (utils)
-                86 STORE_NAME              16 (utils)
-                88 POP_TOP
+    37          82 LOAD_CONST               3 (2)
+                84 LOAD_CONST               7 (('utils',))
+                86 IMPORT_NAME             16
+                88 IMPORT_FROM             17 (utils)
+                90 STORE_NAME              17 (utils)
+                92 POP_TOP
    
-    41          90 LOAD_CONST               8 (0)
-                92 LOAD_CONST               9 (('Any', 'Literal', 'Dict', 'Optional', 'Union'))
-                94 IMPORT_NAME             17 (typing)
-                96 IMPORT_FROM             18 (Any)
-                98 STORE_NAME              18 (Any)
-               100 IMPORT_FROM             19 (Literal)
-               102 STORE_NAME              19 (Literal)
-               104 IMPORT_FROM             20 (Dict)
-               106 STORE_NAME              20 (Dict)
-               108 IMPORT_FROM             21 (Optional)
-               110 STORE_NAME              21 (Optional)
-               112 IMPORT_FROM             22 (Union)
-               114 STORE_NAME              22 (Union)
-               116 POP_TOP
+    41          94 LOAD_CONST               8 (0)
+                96 LOAD_CONST               9 (('Any', 'Literal', 'Dict', 'Optional', 'Union', 'List'))
+                98 IMPORT_NAME             18 (typing)
+               100 IMPORT_FROM             19 (Any)
+               102 STORE_NAME              19 (Any)
+               104 IMPORT_FROM             20 (Literal)
+               106 STORE_NAME              20 (Literal)
+               108 IMPORT_FROM             21 (Dict)
+               110 STORE_NAME              21 (Dict)
+               112 IMPORT_FROM             22 (Optional)
+               114 STORE_NAME              22 (Optional)
+               116 IMPORT_FROM             23 (Union)
+               118 STORE_NAME              23 (Union)
+               120 IMPORT_FROM             24 (List)
+               122 STORE_NAME              24 (List)
+               124 POP_TOP
    
-    49         118 LOAD_CONST              10 ('http://api.weatherapi.com/v1/')
-               120 STORE_NAME              23 (WEATHERAPI_BASE_URL)
+    50         126 LOAD_CONST              10 ('http://api.weatherapi.com/v1/')
+               128 STORE_NAME              25 (WEATHERAPI_BASE_URL)
    
-    51         122 LOAD_CONST              11 (('WeatherAPIClient',))
-               124 STORE_NAME              24 (__all__)
+    52         130 LOAD_CONST              11 (('WeatherAPIClient',))
+               132 STORE_NAME              26 (__all__)
    
-    55         126 PUSH_NULL
-               128 LOAD_BUILD_CLASS
-               130 LOAD_CONST              12 (<code object WeatherAPIClient, file "build\bdist.win-amd64\egg\weatherly\api\client.py", line 55>)
-               132 MAKE_FUNCTION            0
-               134 LOAD_CONST              13 ('WeatherAPIClient')
-               136 LOAD_NAME                2 (BaseAPIClient)
-               138 PRECALL                  3
-               142 CALL                     3
-               152 STORE_NAME              25 (WeatherAPIClient)
-               154 LOAD_CONST              14 (None)
-               156 RETURN_VALUE
+    56         134 PUSH_NULL
+               136 LOAD_BUILD_CLASS
+               138 LOAD_CONST              12 (<code object WeatherAPIClient, file "build\bdist.win-amd64\egg\weatherly\api\client.py", line 56>)
+               140 MAKE_FUNCTION            0
+               142 LOAD_CONST              13 ('WeatherAPIClient')
+               144 LOAD_NAME                2 (BaseAPIClient)
+               146 PRECALL                  3
+               150 CALL                     3
+               160 STORE_NAME              27 (WeatherAPIClient)
+               162 LOAD_CONST              14 (None)
+               164 RETURN_VALUE
    consts
       '\nMIT License\n\nCopyright (c) 2023 Konrad (@konradsic)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n'
       1
       ('BaseAPIClient',)
       2
       ('Languages',)
-      ('CurrentWeatherData',)
+      ('CurrentWeatherData', 'LocationData')
       ('WeatherAPIException', 'NoLocationFound', 'InvalidAPIKey', 'APILimitExceeded', 'APIKeyDisabled', 'AccessDenied', 'InternalApplicationError')
       ('utils',)
       0
-      ('Any', 'Literal', 'Dict', 'Optional', 'Union')
+      ('Any', 'Literal', 'Dict', 'Optional', 'Union', 'List')
       'http://api.weatherapi.com/v1/'
       ('WeatherAPIClient',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 19
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0309000900090009000900090064
-            156404650464056505650665046507660219000000000000000000190000
+            196404650464056505650665046507660219000000000000000000190000
             000000000000006406650565081900000000000000000064076505650819
             000000000000000000640865056508190000000000000000006409650964
             0a19000000000000000000640b6509640a19000000000000000000640c65
             0a6504650b660219000000000000000000640d6402661288006601640e84
             0d5a0c640f65046410650a6504650b660219000000000000000000640d65
-            0a6504650b6602190000000000000000006606641184045a0d0900090064
-            166412650464056505650665046507660219000000000000000000190000
-            0000000000000064096509641319000000000000000000640c650a650465
-            0b660219000000000000000000640d650e660a641484055a0f880078015a
-            105300
+            0a6504650b6602190000000000000000006606641184045a0d6405650665
+            046507660219000000000000000000640d65066507640266021900000000
+            00000000006604641284045a0e09000900641a6413650464056505650665
+            046507660219000000000000000000190000000000000000006409650964
+            1419000000000000000000640c650a6504650b6602190000000000000000
+            00640d650f660a641584055a10641365046602641684045a11641784005a
+            12641884005a13880078015a145300
                        0 MAKE_CELL                0 (__class__)
          
-          55           2 RESUME                   0
+          56           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('WeatherAPIClient')
                       10 STORE_NAME               2 (__qualname__)
          
-          56          12 LOAD_CONST               1 ('\n    A WeatherAPI.com client for fetching various weather information\n\n    Parameters\n    ----------\n    api_key: :class:`str`\n        API Key used to authenticate when sending requests\n    lang: Optional[ Union[:class:`str`, :class:`Languages`] ]\n        Language from the :class:`Languages` enum or a string representing the language or language code (preferably).\n        To get a list of languages visit :class:`Languages`.\n    dt: Optional[:class:`int`]\n        Restrict date output for Forecast and History API method. (Required for History and Future API)\n    end_dt: Optional[:class:`int`]\n        Restrict date output for History API method. Only works for API on Pro plan and above. (Available for History API)\n    hour: Optional[:class:`int`]\n        Restricting forecast or history output to a specific hour in a given day.\n    aqi: Literal["yes", "no"]\n        Enable/Disable Air Quality data in forecast API output. Defaults to "no".\n    tides: Literal["yes", "no"]\n        Enable/Disable Tide data in Marine API output. Defaults to "no".\n    kwargs: Dict[:class:`str`, Any]\n        Additional keyword arguments passed by default to requests made by the client\n    ')
+          57          12 LOAD_CONST               1 ('\n    A WeatherAPI.com client for fetching various weather information\n\n    Parameters\n    ----------\n    api_key: :class:`str`\n        API Key used to authenticate when sending requests\n    lang: Optional[ Union[:class:`str`, :class:`Languages`] ]\n        Language from the :class:`Languages` enum or a string representing the language or language code (preferably).\n        To get a list of languages visit :class:`Languages`. If ``None`` then the default language is used (English)\n    dt: Optional[:class:`int`]\n        Restrict date output for Forecast and History API method. (Required for History and Future API)\n    end_dt: Optional[:class:`int`]\n        Restrict date output for History API method. Only works for API on Pro plan and above. (Available for History API)\n    hour: Optional[:class:`int`]\n        Restricting forecast or history output to a specific hour in a given day.\n    aqi: Literal["yes", "no"]\n        Enable/Disable Air Quality data in forecast API output. Defaults to "no".\n    tides: Literal["yes", "no"]\n        Enable/Disable Tide data in Marine API output. Defaults to "no".\n    kwargs: Dict[:class:`str`, Any]\n        Additional keyword arguments passed by default to requests made by the client\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-          82          16 NOP
+          83          16 NOP
          
-          83          18 NOP
+          84          18 NOP
          
-          84          20 NOP
+          85          20 NOP
          
-          85          22 NOP
+          86          22 NOP
          
-          86          24 NOP
+          87          24 NOP
          
-          87          26 NOP
+          88          26 NOP
          
-          79          28 LOAD_CONST              21 ((None, None, None, None, 'no', 'no'))
+          80          28 LOAD_CONST              25 ((None, None, None, None, 'no', 'no'))
                       30 LOAD_CONST               4 ('api_key')
          
-          81          32 LOAD_NAME                4 (str)
+          82          32 LOAD_NAME                4 (str)
          
-          79          34 LOAD_CONST               5 ('lang')
+          80          34 LOAD_CONST               5 ('lang')
          
-          82          36 LOAD_NAME                5 (Optional)
+          83          36 LOAD_NAME                5 (Optional)
                       38 LOAD_NAME                6 (Union)
                       40 LOAD_NAME                4 (str)
                       42 LOAD_NAME                7 (Languages)
                       44 BUILD_TUPLE              2
                       46 BINARY_SUBSCR
                       56 BINARY_SUBSCR
          
-          79          66 LOAD_CONST               6 ('dt')
+          80          66 LOAD_CONST               6 ('dt')
          
-          83          68 LOAD_NAME                5 (Optional)
+          84          68 LOAD_NAME                5 (Optional)
                       70 LOAD_NAME                8 (int)
                       72 BINARY_SUBSCR
          
-          79          82 LOAD_CONST               7 ('end_dt')
+          80          82 LOAD_CONST               7 ('end_dt')
          
-          84          84 LOAD_NAME                5 (Optional)
+          85          84 LOAD_NAME                5 (Optional)
                       86 LOAD_NAME                8 (int)
                       88 BINARY_SUBSCR
          
-          79          98 LOAD_CONST               8 ('hour')
+          80          98 LOAD_CONST               8 ('hour')
          
-          85         100 LOAD_NAME                5 (Optional)
+          86         100 LOAD_NAME                5 (Optional)
                      102 LOAD_NAME                8 (int)
                      104 BINARY_SUBSCR
          
-          79         114 LOAD_CONST               9 ('aqi')
+          80         114 LOAD_CONST               9 ('aqi')
          
-          86         116 LOAD_NAME                9 (Literal)
+          87         116 LOAD_NAME                9 (Literal)
                      118 LOAD_CONST              10 (('yes', 'no'))
                      120 BINARY_SUBSCR
          
-          79         130 LOAD_CONST              11 ('tides')
+          80         130 LOAD_CONST              11 ('tides')
          
-          87         132 LOAD_NAME                9 (Literal)
+          88         132 LOAD_NAME                9 (Literal)
                      134 LOAD_CONST              10 (('yes', 'no'))
                      136 BINARY_SUBSCR
          
-          79         146 LOAD_CONST              12 ('kwargs')
+          80         146 LOAD_CONST              12 ('kwargs')
          
-          88         148 LOAD_NAME               10 (Dict)
+          89         148 LOAD_NAME               10 (Dict)
                      150 LOAD_NAME                4 (str)
                      152 LOAD_NAME               11 (Any)
                      154 BUILD_TUPLE              2
                      156 BINARY_SUBSCR
          
-          79         166 LOAD_CONST              13 ('return')
+          80         166 LOAD_CONST              13 ('return')
          
-          89         168 LOAD_CONST               2 (None)
+          90         168 LOAD_CONST               2 (None)
          
-          79         170 BUILD_TUPLE             18
+          80         170 BUILD_TUPLE             18
                      172 LOAD_CLOSURE             0 (__class__)
                      174 BUILD_TUPLE              1
-                     176 LOAD_CONST              14 (<code object __init__, file "build\bdist.win-amd64\egg\weatherly\api\client.py", line 79>)
+                     176 LOAD_CONST              14 (<code object __init__, file "build\bdist.win-amd64\egg\weatherly\api\client.py", line 80>)
                      178 MAKE_FUNCTION           13 (defaults, annotations, closure)
                      180 STORE_NAME              12 (__init__)
          
-         109         182 LOAD_CONST              15 ('endpoint')
+         112         182 LOAD_CONST              15 ('endpoint')
                      184 LOAD_NAME                4 (str)
                      186 LOAD_CONST              16 ('options')
                      188 LOAD_NAME               10 (Dict)
                      190 LOAD_NAME                4 (str)
                      192 LOAD_NAME               11 (Any)
                      194 BUILD_TUPLE              2
                      196 BINARY_SUBSCR
                      206 LOAD_CONST              13 ('return')
                      208 LOAD_NAME               10 (Dict)
                      210 LOAD_NAME                4 (str)
                      212 LOAD_NAME               11 (Any)
                      214 BUILD_TUPLE              2
                      216 BINARY_SUBSCR
                      226 BUILD_TUPLE              6
-                     228 LOAD_CONST              17 (<code object _call_request, file "build\bdist.win-amd64\egg\weatherly\api\client.py", line 109>)
+                     228 LOAD_CONST              17 (<code object _call_request, file "build\bdist.win-amd64\egg\weatherly\api\client.py", line 112>)
                      230 MAKE_FUNCTION            4 (annotations)
                      232 STORE_NAME              13 (_call_request)
          
-         124         234 NOP
-         
-         125         236 NOP
-         
-         122         238 LOAD_CONST              22 ((None, None))
-                     240 LOAD_CONST              18 ('query')
-         
-         123         242 LOAD_NAME                4 (str)
-         
-         122         244 LOAD_CONST               5 ('lang')
-         
-         124         246 LOAD_NAME                5 (Optional)
-                     248 LOAD_NAME                6 (Union)
-                     250 LOAD_NAME                4 (str)
-                     252 LOAD_NAME                7 (Languages)
-                     254 BUILD_TUPLE              2
-                     256 BINARY_SUBSCR
-                     266 BINARY_SUBSCR
-         
-         122         276 LOAD_CONST               9 ('aqi')
-         
-         125         278 LOAD_NAME                9 (Literal)
-                     280 LOAD_CONST              19 (('yes', 'no', None))
-                     282 BINARY_SUBSCR
-         
-         122         292 LOAD_CONST              12 ('kwargs')
-         
-         126         294 LOAD_NAME               10 (Dict)
-                     296 LOAD_NAME                4 (str)
-                     298 LOAD_NAME               11 (Any)
-                     300 BUILD_TUPLE              2
-                     302 BINARY_SUBSCR
-         
-         122         312 LOAD_CONST              13 ('return')
-         
-         127         314 LOAD_NAME               14 (CurrentWeatherData)
-         
-         122         316 BUILD_TUPLE             10
-                     318 LOAD_CONST              20 (<code object get_current_weather, file "build\bdist.win-amd64\egg\weatherly\api\client.py", line 122>)
-                     320 MAKE_FUNCTION            5 (defaults, annotations)
-                     322 STORE_NAME              15 (get_current_weather)
-                     324 LOAD_CLOSURE             0 (__class__)
-                     326 COPY                     1
-                     328 STORE_NAME              16 (__classcell__)
-                     330 RETURN_VALUE
+         141         234 LOAD_CONST               5 ('lang')
+                     236 LOAD_NAME                6 (Union)
+                     238 LOAD_NAME                4 (str)
+                     240 LOAD_NAME                7 (Languages)
+                     242 BUILD_TUPLE              2
+                     244 BINARY_SUBSCR
+                     254 LOAD_CONST              13 ('return')
+                     256 LOAD_NAME                6 (Union)
+                     258 LOAD_NAME                7 (Languages)
+                     260 LOAD_CONST               2 (None)
+                     262 BUILD_TUPLE              2
+                     264 BINARY_SUBSCR
+                     274 BUILD_TUPLE              4
+                     276 LOAD_CONST              18 (<code object set_language, file "build\bdist.win-amd64\egg\weatherly\api\client.py", line 141>)
+                     278 MAKE_FUNCTION            4 (annotations)
+                     280 STORE_NAME              14 (set_language)
+         
+         165         282 NOP
+         
+         166         284 NOP
+         
+         163         286 LOAD_CONST              26 ((None, None))
+                     288 LOAD_CONST              19 ('query')
+         
+         164         290 LOAD_NAME                4 (str)
+         
+         163         292 LOAD_CONST               5 ('lang')
+         
+         165         294 LOAD_NAME                5 (Optional)
+                     296 LOAD_NAME                6 (Union)
+                     298 LOAD_NAME                4 (str)
+                     300 LOAD_NAME                7 (Languages)
+                     302 BUILD_TUPLE              2
+                     304 BINARY_SUBSCR
+                     314 BINARY_SUBSCR
+         
+         163         324 LOAD_CONST               9 ('aqi')
+         
+         166         326 LOAD_NAME                9 (Literal)
+                     328 LOAD_CONST              20 (('yes', 'no', None))
+                     330 BINARY_SUBSCR
+         
+         163         340 LOAD_CONST              12 ('kwargs')
+         
+         167         342 LOAD_NAME               10 (Dict)
+                     344 LOAD_NAME                4 (str)
+                     346 LOAD_NAME               11 (Any)
+                     348 BUILD_TUPLE              2
+                     350 BINARY_SUBSCR
+         
+         163         360 LOAD_CONST              13 ('return')
+         
+         168         362 LOAD_NAME               15 (CurrentWeatherData)
+         
+         163         364 BUILD_TUPLE             10
+                     366 LOAD_CONST              21 (<code object get_current_weather, file "build\bdist.win-amd64\egg\weatherly\api\client.py", line 163>)
+                     368 MAKE_FUNCTION            5 (defaults, annotations)
+                     370 STORE_NAME              16 (get_current_weather)
+         
+         217         372 LOAD_CONST              19 ('query')
+                     374 LOAD_NAME                4 (str)
+                     376 BUILD_TUPLE              2
+                     378 LOAD_CONST              22 (<code object get_locations, file "build\bdist.win-amd64\egg\weatherly\api\client.py", line 217>)
+                     380 MAKE_FUNCTION            4 (annotations)
+                     382 STORE_NAME              17 (get_locations)
+         
+         255         384 LOAD_CONST              23 (<code object __str__, file "build\bdist.win-amd64\egg\weatherly\api\client.py", line 255>)
+                     386 MAKE_FUNCTION            0
+                     388 STORE_NAME              18 (__str__)
+         
+         258         390 LOAD_CONST              24 (<code object __repr__, file "build\bdist.win-amd64\egg\weatherly\api\client.py", line 258>)
+                     392 MAKE_FUNCTION            0
+                     394 STORE_NAME              19 (__repr__)
+                     396 LOAD_CLOSURE             0 (__class__)
+                     398 COPY                     1
+                     400 STORE_NAME              20 (__classcell__)
+                     402 RETURN_VALUE
          consts
             'WeatherAPIClient'
-            '\n    A WeatherAPI.com client for fetching various weather information\n\n    Parameters\n    ----------\n    api_key: :class:`str`\n        API Key used to authenticate when sending requests\n    lang: Optional[ Union[:class:`str`, :class:`Languages`] ]\n        Language from the :class:`Languages` enum or a string representing the language or language code (preferably).\n        To get a list of languages visit :class:`Languages`.\n    dt: Optional[:class:`int`]\n        Restrict date output for Forecast and History API method. (Required for History and Future API)\n    end_dt: Optional[:class:`int`]\n        Restrict date output for History API method. Only works for API on Pro plan and above. (Available for History API)\n    hour: Optional[:class:`int`]\n        Restricting forecast or history output to a specific hour in a given day.\n    aqi: Literal["yes", "no"]\n        Enable/Disable Air Quality data in forecast API output. Defaults to "no".\n    tides: Literal["yes", "no"]\n        Enable/Disable Tide data in Marine API output. Defaults to "no".\n    kwargs: Dict[:class:`str`, Any]\n        Additional keyword arguments passed by default to requests made by the client\n    '
+            '\n    A WeatherAPI.com client for fetching various weather information\n\n    Parameters\n    ----------\n    api_key: :class:`str`\n        API Key used to authenticate when sending requests\n    lang: Optional[ Union[:class:`str`, :class:`Languages`] ]\n        Language from the :class:`Languages` enum or a string representing the language or language code (preferably).\n        To get a list of languages visit :class:`Languages`. If ``None`` then the default language is used (English)\n    dt: Optional[:class:`int`]\n        Restrict date output for Forecast and History API method. (Required for History and Future API)\n    end_dt: Optional[:class:`int`]\n        Restrict date output for History API method. Only works for API on Pro plan and above. (Available for History API)\n    hour: Optional[:class:`int`]\n        Restricting forecast or history output to a specific hour in a given day.\n    aqi: Literal["yes", "no"]\n        Enable/Disable Air Quality data in forecast API output. Defaults to "no".\n    tides: Literal["yes", "no"]\n        Enable/Disable Tide data in Marine API output. Defaults to "no".\n    kwargs: Dict[:class:`str`, Any]\n        Additional keyword arguments passed by default to requests made by the client\n    '
             None
             'no'
             'api_key'
             'lang'
             'dt'
             'end_dt'
             'hour'
@@ -296,431 +334,661 @@
             'return'
             code
                argcount  : 8
                nlocals   : 11
                stacksize : 4
                flags     : 11
                code
-                  0x9501970064007d097c0281147401000000000000000000006a01000000
-                  00000000007c02a6010000ab0100000000000000007d0964017c0169017c
-                  08a5017d0a7c0972167c0aa0020000000000000000000000000000000000
-                  0000007c09ac02a6010000ab010000000000000000010074070000000000
-                  0000000000a6000000ab000000000000000000a004000000000000000000
-                  0000000000000000000000740a000000000000000000007c0aac03a60200
-                  00ab02000000000000000001007c037c005f0600000000000000007c047c
-                  005f0700000000000000007c057c005f0800000000000000007c067c005f
-                  0900000000000000007c077c005f0a00000000000000007c087c005f0b00
-                  0000000000000064005300
+                  0x9501970064007d097c0281167401000000000000000000006a01000000
+                  00000000007c026401ac02a6020000ab0200000000000000007d0964037c
+                  0169017c08a5017d0a7c09721f7c0aa00200000000000000000000000000
+                  000000000000007c0981077c096a0300000000000000006e016400ac04a6
+                  010000ab0100000000000000000100740900000000000000000000a60000
+                  00ab000000000000000000a0050000000000000000000000000000000000
+                  000000740c000000000000000000007c0aac05a6020000ab020000000000
+                  00000001007c037c005f0700000000000000007c047c005f080000000000
+                  0000007c057c005f0900000000000000007c067c005f0a00000000000000
+                  007c077c005f0b00000000000000007c087c005f0c00000000000000007c
+                  09720f741b000000000000000000007c09a6010000ab0100000000000000
+                  006e0164007c005f0e000000000000000064005300
                              0 COPY_FREE_VARS           1
                
-                79           2 RESUME                   0
+                80           2 RESUME                   0
                
-                90           4 LOAD_CONST               0 (None)
+                91           4 LOAD_CONST               0 (None)
                              6 STORE_FAST               9 (lang_code)
                
-                91           8 LOAD_FAST                2 (lang)
-                            10 POP_JUMP_FORWARD_IF_NONE    20 (to 52)
+                92           8 LOAD_FAST                2 (lang)
+                            10 POP_JUMP_FORWARD_IF_NONE    22 (to 56)
                
-                92          12 LOAD_GLOBAL              1 (NULL + utils)
+                93          12 LOAD_GLOBAL              1 (NULL + utils)
                             24 LOAD_ATTR                1 (find_language)
                             34 LOAD_FAST                2 (lang)
-                            36 PRECALL                  1
-                            40 CALL                     1
-                            50 STORE_FAST               9 (lang_code)
-               
-                94     >>   52 LOAD_CONST               1 ('key')
-                            54 LOAD_FAST                1 (api_key)
-               
-                93          56 BUILD_MAP                1
-               
-                95          58 LOAD_FAST                8 (kwargs)
-               
-                93          60 DICT_UPDATE              1
-                            62 STORE_FAST              10 (opts)
-               
-                97          64 LOAD_FAST                9 (lang_code)
-                            66 POP_JUMP_FORWARD_IF_FALSE    22 (to 112)
-                            68 LOAD_FAST               10 (opts)
-                            70 LOAD_METHOD              2 (update)
-                            92 LOAD_FAST                9 (lang_code)
-                            94 KW_NAMES                 2
-                            96 PRECALL                  1
-                           100 CALL                     1
-                           110 POP_TOP
-               
-                99     >>  112 LOAD_GLOBAL              7 (NULL + super)
-                           124 PRECALL                  0
-                           128 CALL                     0
-                           138 LOAD_METHOD              4 (__init__)
-                           160 LOAD_GLOBAL             10 (WEATHERAPI_BASE_URL)
-               
-               100         172 LOAD_FAST               10 (opts)
-               
-                99         174 KW_NAMES                 3
-                           176 PRECALL                  2
-                           180 CALL                     2
-                           190 POP_TOP
-               
-               102         192 LOAD_FAST                3 (dt)
-                           194 LOAD_FAST                0 (self)
-                           196 STORE_ATTR               6 (dt)
-               
-               103         206 LOAD_FAST                4 (end_dt)
-                           208 LOAD_FAST                0 (self)
-                           210 STORE_ATTR               7 (end_dt)
-               
-               104         220 LOAD_FAST                5 (hour)
-                           222 LOAD_FAST                0 (self)
-                           224 STORE_ATTR               8 (hour)
-               
-               105         234 LOAD_FAST                6 (aqi)
-                           236 LOAD_FAST                0 (self)
-                           238 STORE_ATTR               9 (aqi)
-               
-               106         248 LOAD_FAST                7 (tides)
-                           250 LOAD_FAST                0 (self)
-                           252 STORE_ATTR              10 (tides)
-               
-               107         262 LOAD_FAST                8 (kwargs)
-                           264 LOAD_FAST                0 (self)
-                           266 STORE_ATTR              11 (kwargs)
-                           276 LOAD_CONST               0 (None)
-                           278 RETURN_VALUE
+                            36 LOAD_CONST               1 (True)
+                            38 KW_NAMES                 2
+                            40 PRECALL                  2
+                            44 CALL                     2
+                            54 STORE_FAST               9 (lang_code)
+               
+                95     >>   56 LOAD_CONST               3 ('key')
+                            58 LOAD_FAST                1 (api_key)
+               
+                94          60 BUILD_MAP                1
+               
+                96          62 LOAD_FAST                8 (kwargs)
+               
+                94          64 DICT_UPDATE              1
+                            66 STORE_FAST              10 (opts)
+               
+                98          68 LOAD_FAST                9 (lang_code)
+                            70 POP_JUMP_FORWARD_IF_FALSE    31 (to 134)
+                            72 LOAD_FAST               10 (opts)
+                            74 LOAD_METHOD              2 (update)
+                            96 LOAD_FAST                9 (lang_code)
+                            98 POP_JUMP_FORWARD_IF_NONE     7 (to 114)
+                           100 LOAD_FAST                9 (lang_code)
+                           102 LOAD_ATTR                3 (value)
+                           112 JUMP_FORWARD             1 (to 116)
+                       >>  114 LOAD_CONST               0 (None)
+                       >>  116 KW_NAMES                 4
+                           118 PRECALL                  1
+                           122 CALL                     1
+                           132 POP_TOP
+               
+               100     >>  134 LOAD_GLOBAL              9 (NULL + super)
+                           146 PRECALL                  0
+                           150 CALL                     0
+                           160 LOAD_METHOD              5 (__init__)
+                           182 LOAD_GLOBAL             12 (WEATHERAPI_BASE_URL)
+               
+               101         194 LOAD_FAST               10 (opts)
+               
+               100         196 KW_NAMES                 5
+                           198 PRECALL                  2
+                           202 CALL                     2
+                           212 POP_TOP
+               
+               103         214 LOAD_FAST                3 (dt)
+                           216 LOAD_FAST                0 (self)
+                           218 STORE_ATTR               7 (dt)
+               
+               104         228 LOAD_FAST                4 (end_dt)
+                           230 LOAD_FAST                0 (self)
+                           232 STORE_ATTR               8 (end_dt)
+               
+               105         242 LOAD_FAST                5 (hour)
+                           244 LOAD_FAST                0 (self)
+                           246 STORE_ATTR               9 (hour)
+               
+               106         256 LOAD_FAST                6 (aqi)
+                           258 LOAD_FAST                0 (self)
+                           260 STORE_ATTR              10 (aqi)
+               
+               107         270 LOAD_FAST                7 (tides)
+                           272 LOAD_FAST                0 (self)
+                           274 STORE_ATTR              11 (tides)
+               
+               108         284 LOAD_FAST                8 (kwargs)
+                           286 LOAD_FAST                0 (self)
+                           288 STORE_ATTR              12 (kwargs)
+               
+               109         298 LOAD_FAST                9 (lang_code)
+                           300 POP_JUMP_FORWARD_IF_FALSE    15 (to 332)
+                           302 LOAD_GLOBAL             27 (NULL + Languages)
+                           314 LOAD_FAST                9 (lang_code)
+                           316 PRECALL                  1
+                           320 CALL                     1
+                           330 JUMP_FORWARD             1 (to 334)
+                       >>  332 LOAD_CONST               0 (None)
+                       >>  334 LOAD_FAST                0 (self)
+                           336 STORE_ATTR              14 (lang)
+                           346 LOAD_CONST               0 (None)
+                           348 RETURN_VALUE
                consts
                   None
+                  True
+                  ('asobj',)
                   'key'
                   ('lang',)
                   ('base_url', 'default_options')
-               names      ('utils', 'find_language', 'update', 'super', '__init__', 'WEATHERAPI_BASE_URL', 'dt', 'end_dt', 'hour', 'aqi', 'tides', 'kwargs')
+               names      ('utils', 'find_language', 'update', 'value', 'super', '__init__', 'WEATHERAPI_BASE_URL', 'dt', 'end_dt', 'hour', 'aqi', 'tides', 'kwargs', 'Languages', 'lang')
                varnames   ('self', 'api_key', 'lang', 'dt', 'end_dt', 'hour', 'aqi', 'tides', 'kwargs', 'lang_code', 'opts')
                freevars   ('__class__',)
                cellvars   ()
                filename   'build\\bdist.win-amd64\\egg\\weatherly\\api\\client.py'
                name       '__init__'
-               firstlineno 79
+               firstlineno 80
                lnotab
-                  0x040b04010401280204ff020202fe040430023c0102ff12030e010e010e
-                  010e010e01
+                  0x040b040104012c0204ff020202fe040442023c0102ff12030e010e010e
+                  010e010e010e01
             'endpoint'
             'options'
             code
                argcount  : 3
-               nlocals   : 7
+               nlocals   : 11
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab0000000000000000007d037c03a002000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   0044005d0a5c0200007d047d057c0580037c037c043d008c0b7c02a00200
                   00000000000000000000000000000000000000a6000000ab000000000000
                   00000044005d0c5c0200007d047d057c0581057c057c037c043c0000008c
                   0d02007c006a0300000000000000007c01660169007c03a4018e017d067c
-                  065300
-               109           0 RESUME                   0
+                  066402190000000000000000006a04000000000000000064036b00000000
+                  0073c67c066404190000000000000000006405190000000000000000007d
+                  077c076406190000000000000000007d087c066402190000000000000000
+                  006a0400000000000000007d097c076407190000000000000000007d0a7c
+                  0864086b02000000007211740b000000000000000000007c097c087c0aa6
+                  030000ab03000000000000000082017c0864096b02000000007211740d00
+                  0000000000000000007c097c087c0aa6030000ab03000000000000000082
+                  017c08640a6b02000000007211740f000000000000000000007c097c087c
+                  0aa6030000ab03000000000000000082017c08640b6b0200000000721174
+                  11000000000000000000007c097c087c0aa6030000ab0300000000000000
+                  0082017c08640c6b020000000072117413000000000000000000007c097c
+                  087c0aa6030000ab03000000000000000082017c08640d6b020000000072
+                  117415000000000000000000007c097c087c0aa6030000ab030000000000
+                  00000082017417000000000000000000007c097c087c0aa6030000ab0300
+                  0000000000000082017c065300
+               112           0 RESUME                   0
                
-               111           2 LOAD_FAST                0 (self)
+               114           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (default_options)
                             14 LOAD_METHOD              1 (copy)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 STORE_FAST               3 (final_options)
                
-               113          52 LOAD_FAST                3 (final_options)
+               116          52 LOAD_FAST                3 (final_options)
                             54 LOAD_METHOD              2 (items)
                             76 PRECALL                  0
                             80 CALL                     0
                             90 GET_ITER
                        >>   92 FOR_ITER                10 (to 114)
                             94 UNPACK_SEQUENCE          2
                             98 STORE_FAST               4 (k)
                            100 STORE_FAST               5 (v)
                
-               114         102 LOAD_FAST                5 (v)
+               117         102 LOAD_FAST                5 (v)
                            104 POP_JUMP_FORWARD_IF_NOT_NONE     3 (to 112)
                            106 LOAD_FAST                3 (final_options)
                            108 LOAD_FAST                4 (k)
                            110 DELETE_SUBSCR
                        >>  112 JUMP_BACKWARD           11 (to 92)
                
-               116     >>  114 LOAD_FAST                2 (options)
+               119     >>  114 LOAD_FAST                2 (options)
                            116 LOAD_METHOD              2 (items)
                            138 PRECALL                  0
                            142 CALL                     0
                            152 GET_ITER
                        >>  154 FOR_ITER                12 (to 180)
                            156 UNPACK_SEQUENCE          2
                            160 STORE_FAST               4 (k)
                            162 STORE_FAST               5 (v)
                
-               117         164 LOAD_FAST                5 (v)
+               120         164 LOAD_FAST                5 (v)
                            166 POP_JUMP_FORWARD_IF_NONE     5 (to 178)
                            168 LOAD_FAST                5 (v)
                            170 LOAD_FAST                3 (final_options)
                            172 LOAD_FAST                4 (k)
                            174 STORE_SUBSCR
                        >>  178 JUMP_BACKWARD           13 (to 154)
                
-               119     >>  180 PUSH_NULL
+               122     >>  180 PUSH_NULL
                            182 LOAD_FAST                0 (self)
                            184 LOAD_ATTR                3 (_request)
                            194 LOAD_FAST                1 (endpoint)
                            196 BUILD_TUPLE              1
                            198 BUILD_MAP                0
                            200 LOAD_FAST                3 (final_options)
                            202 DICT_MERGE               1
                            204 CALL_FUNCTION_EX         1
                            206 STORE_FAST               6 (resp)
                
-               120         208 LOAD_FAST                6 (resp)
-                           210 RETURN_VALUE
+               124         208 LOAD_FAST                6 (resp)
+                           210 LOAD_CONST               2 (1)
+                           212 BINARY_SUBSCR
+                           222 LOAD_ATTR                4 (status_code)
+                           232 LOAD_CONST               3 (400)
+                           234 COMPARE_OP               0 (<)
+                           240 POP_JUMP_FORWARD_IF_TRUE   198 (to 638)
+               
+               126         242 LOAD_FAST                6 (resp)
+                           244 LOAD_CONST               4 (0)
+                           246 BINARY_SUBSCR
+                           256 LOAD_CONST               5 ('error')
+                           258 BINARY_SUBSCR
+                           268 STORE_FAST               7 (error_data)
+               
+               127         270 LOAD_FAST                7 (error_data)
+                           272 LOAD_CONST               6 ('code')
+                           274 BINARY_SUBSCR
+                           284 STORE_FAST               8 (code)
+               
+               128         286 LOAD_FAST                6 (resp)
+                           288 LOAD_CONST               2 (1)
+                           290 BINARY_SUBSCR
+                           300 LOAD_ATTR                4 (status_code)
+                           310 STORE_FAST               9 (status)
+               
+               129         312 LOAD_FAST                7 (error_data)
+                           314 LOAD_CONST               7 ('message')
+                           316 BINARY_SUBSCR
+                           326 STORE_FAST              10 (msg)
+               
+               131         328 LOAD_FAST                8 (code)
+                           330 LOAD_CONST               8 (1006)
+                           332 COMPARE_OP               2 (==)
+                           338 POP_JUMP_FORWARD_IF_FALSE    17 (to 374)
+                           340 LOAD_GLOBAL             11 (NULL + NoLocationFound)
+                           352 LOAD_FAST                9 (status)
+                           354 LOAD_FAST                8 (code)
+                           356 LOAD_FAST               10 (msg)
+                           358 PRECALL                  3
+                           362 CALL                     3
+                           372 RAISE_VARARGS            1
+               
+               132     >>  374 LOAD_FAST                8 (code)
+                           376 LOAD_CONST               9 (2006)
+                           378 COMPARE_OP               2 (==)
+                           384 POP_JUMP_FORWARD_IF_FALSE    17 (to 420)
+                           386 LOAD_GLOBAL             13 (NULL + InvalidAPIKey)
+                           398 LOAD_FAST                9 (status)
+                           400 LOAD_FAST                8 (code)
+                           402 LOAD_FAST               10 (msg)
+                           404 PRECALL                  3
+                           408 CALL                     3
+                           418 RAISE_VARARGS            1
+               
+               133     >>  420 LOAD_FAST                8 (code)
+                           422 LOAD_CONST              10 (2007)
+                           424 COMPARE_OP               2 (==)
+                           430 POP_JUMP_FORWARD_IF_FALSE    17 (to 466)
+                           432 LOAD_GLOBAL             15 (NULL + APILimitExceeded)
+                           444 LOAD_FAST                9 (status)
+                           446 LOAD_FAST                8 (code)
+                           448 LOAD_FAST               10 (msg)
+                           450 PRECALL                  3
+                           454 CALL                     3
+                           464 RAISE_VARARGS            1
+               
+               134     >>  466 LOAD_FAST                8 (code)
+                           468 LOAD_CONST              11 (2008)
+                           470 COMPARE_OP               2 (==)
+                           476 POP_JUMP_FORWARD_IF_FALSE    17 (to 512)
+                           478 LOAD_GLOBAL             17 (NULL + APIKeyDisabled)
+                           490 LOAD_FAST                9 (status)
+                           492 LOAD_FAST                8 (code)
+                           494 LOAD_FAST               10 (msg)
+                           496 PRECALL                  3
+                           500 CALL                     3
+                           510 RAISE_VARARGS            1
+               
+               135     >>  512 LOAD_FAST                8 (code)
+                           514 LOAD_CONST              12 (2009)
+                           516 COMPARE_OP               2 (==)
+                           522 POP_JUMP_FORWARD_IF_FALSE    17 (to 558)
+                           524 LOAD_GLOBAL             19 (NULL + AccessDenied)
+                           536 LOAD_FAST                9 (status)
+                           538 LOAD_FAST                8 (code)
+                           540 LOAD_FAST               10 (msg)
+                           542 PRECALL                  3
+                           546 CALL                     3
+                           556 RAISE_VARARGS            1
+               
+               136     >>  558 LOAD_FAST                8 (code)
+                           560 LOAD_CONST              13 (9999)
+                           562 COMPARE_OP               2 (==)
+                           568 POP_JUMP_FORWARD_IF_FALSE    17 (to 604)
+                           570 LOAD_GLOBAL             21 (NULL + InternalApplicationError)
+                           582 LOAD_FAST                9 (status)
+                           584 LOAD_FAST                8 (code)
+                           586 LOAD_FAST               10 (msg)
+                           588 PRECALL                  3
+                           592 CALL                     3
+                           602 RAISE_VARARGS            1
+               
+               137     >>  604 LOAD_GLOBAL             23 (NULL + WeatherAPIException)
+                           616 LOAD_FAST                9 (status)
+                           618 LOAD_FAST                8 (code)
+                           620 LOAD_FAST               10 (msg)
+                           622 PRECALL                  3
+                           626 CALL                     3
+                           636 RAISE_VARARGS            1
+               
+               139     >>  638 LOAD_FAST                6 (resp)
+                           640 RETURN_VALUE
                consts
                   'Private method used to make requests to WeatherAPI'
-               names      ('default_options', 'copy', 'items', '_request')
-               varnames   ('self', 'endpoint', 'options', 'final_options', 'k', 'v', 'resp')
+                  None
+                  1
+                  400
+                  0
+                  'error'
+                  'code'
+                  'message'
+                  1006
+                  2006
+                  2007
+                  2008
+                  2009
+                  9999
+               names      ('default_options', 'copy', 'items', '_request', 'status_code', 'NoLocationFound', 'InvalidAPIKey', 'APILimitExceeded', 'APIKeyDisabled', 'AccessDenied', 'InternalApplicationError', 'WeatherAPIException')
+               varnames   ('self', 'endpoint', 'options', 'final_options', 'k', 'v', 'resp', 'error_data', 'code', 'status', 'msg')
                freevars   ()
                cellvars   ()
                filename   'build\\bdist.win-amd64\\egg\\weatherly\\api\\client.py'
                name       '_call_request'
-               firstlineno 109
-               lnotab 0x0202320232010c02320110021c01
+               firstlineno 112
+               lnotab
+                  0x0202320232010c02320110021c0222021c0110011a0110022e012e012e
+                  012e012e012e012202
+            code
+               argcount  : 2
+               nlocals   : 3
+               stacksize : 4
+               flags     : 3
+               code
+                  0x97007401000000000000000000006a0100000000000000007c016401ac
+                  02a6020000ab0200000000000000007d027c02730964037c005f02000000
+                  0000000000640453007c027c005f02000000000000000064015300
+               141           0 RESUME                   0
+               
+               155           2 LOAD_GLOBAL              1 (NULL + utils)
+                            14 LOAD_ATTR                1 (find_language)
+                            24 LOAD_FAST                1 (lang)
+                            26 LOAD_CONST               1 (True)
+                            28 KW_NAMES                 2
+                            30 PRECALL                  2
+                            34 CALL                     2
+                            44 STORE_FAST               2 (lang_class)
+               
+               156          46 LOAD_FAST                2 (lang_class)
+                            48 POP_JUMP_FORWARD_IF_TRUE     9 (to 68)
+               
+               157          50 LOAD_CONST               3 (None)
+                            52 LOAD_FAST                0 (self)
+                            54 STORE_ATTR               2 (lang)
+               
+               158          64 LOAD_CONST               4 (False)
+                            66 RETURN_VALUE
+               
+               160     >>   68 LOAD_FAST                2 (lang_class)
+                            70 LOAD_FAST                0 (self)
+                            72 STORE_ATTR               2 (lang)
+               
+               161          82 LOAD_CONST               1 (True)
+                            84 RETURN_VALUE
+               consts
+                  "\n        Set client's language when requesting data.\n        \n        Parameters\n        -----------\n        lang: Union[:class:`str`, :class:`Languages`]\n            Language to set. Can be either a string that is lanuage's name or code or a :class:`Languages` enum object.\n            \n        Returns\n        ---------\n        :class:`bool`\n            A boolean indicating whether the language was successfully set. If it's ``False``, then something went wrong, probably because of the wrong ``lang`` value.\n        "
+                  True
+                  ('asobj',)
+                  None
+                  False
+               names      ('utils', 'find_language', 'lang')
+               varnames   ('self', 'lang', 'lang_class')
+               freevars   ()
+               cellvars   ()
+               filename   'build\\bdist.win-amd64\\egg\\weatherly\\api\\client.py'
+               name       'set_language'
+               firstlineno 141
+               lnotab 0x020e2c0104010e0104020e01
             'query'
             ('yes', 'no', None)
             code
                argcount  : 4
-               nlocals   : 12
+               nlocals   : 8
                stacksize : 5
                flags     : 11
                code
                   0x97007c0370067c006a0000000000000000007c0164019c027c04a5017d
                   057c0281057c027c0564033c0000007c00a0010000000000000000000000
-                  00000000000000000064047c05a6020000ab0200000000000000007d067c
-                  066405190000000000000000006a02000000000000000064066b00000000
-                  0073c67c066407190000000000000000006408190000000000000000007d
-                  077c076409190000000000000000007d087c066405190000000000000000
-                  006a0200000000000000007d097c07640a190000000000000000007d0a7c
-                  08640b6b020000000072117407000000000000000000007c097c087c0aa6
-                  030000ab03000000000000000082017c08640c6b02000000007211740900
-                  0000000000000000007c097c087c0aa6030000ab03000000000000000082
-                  017c08640d6b02000000007211740b000000000000000000007c097c087c
-                  0aa6030000ab03000000000000000082017c08640e6b0200000000721174
-                  0d000000000000000000007c097c087c0aa6030000ab0300000000000000
-                  0082017c08640f6b02000000007211740f000000000000000000007c097c
-                  087c0aa6030000ab03000000000000000082017c0864106b020000000072
-                  117411000000000000000000007c097c087c0aa6030000ab030000000000
-                  00000082017413000000000000000000007c097c087c0aa6030000ab0300
-                  0000000000000082017415000000000000000000007c0664071900000000
-                  00000000006411190000000000000000007c066405190000000000000000
-                  006a0200000000000000006402a6030000ab0300000000000000007d0b7c
-                  0b5300
-               122           0 RESUME                   0
+                  00000000000000000064047c05a6020000ab0200000000000000007d0674
+                  05000000000000000000007c066405190000000000000000007c06640619
+                  0000000000000000006a0300000000000000006402a6030000ab03000000
+                  00000000007d077c075300
+               163           0 RESUME                   0
                
-               149           2 LOAD_FAST                3 (aqi)
+               207           2 LOAD_FAST                3 (aqi)
                              4 JUMP_IF_TRUE_OR_POP      6 (to 18)
                              6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (aqi)
                
-               150     >>   18 LOAD_FAST                1 (query)
+               208     >>   18 LOAD_FAST                1 (query)
                
-               148          20 LOAD_CONST               1 (('aqi', 'q'))
+               206          20 LOAD_CONST               1 (('aqi', 'q'))
                             22 BUILD_CONST_KEY_MAP      2
                
-               151          24 LOAD_FAST                4 (kwargs)
+               209          24 LOAD_FAST                4 (kwargs)
                
-               148          26 DICT_UPDATE              1
+               206          26 DICT_UPDATE              1
                             28 STORE_FAST               5 (options)
                
-               153          30 LOAD_FAST                2 (lang)
+               211          30 LOAD_FAST                2 (lang)
                             32 POP_JUMP_FORWARD_IF_NONE     5 (to 44)
                             34 LOAD_FAST                2 (lang)
                             36 LOAD_FAST                5 (options)
                             38 LOAD_CONST               3 ('lang')
                             40 STORE_SUBSCR
                
-               154     >>   44 LOAD_FAST                0 (self)
+               212     >>   44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (_call_request)
                             68 LOAD_CONST               4 ('current.json')
                             70 LOAD_FAST                5 (options)
                             72 PRECALL                  2
                             76 CALL                     2
                             86 STORE_FAST               6 (resp)
                
-               156          88 LOAD_FAST                6 (resp)
-                            90 LOAD_CONST               5 (1)
-                            92 BINARY_SUBSCR
-                           102 LOAD_ATTR                2 (status_code)
-                           112 LOAD_CONST               6 (400)
-                           114 COMPARE_OP               0 (<)
-                           120 POP_JUMP_FORWARD_IF_TRUE   198 (to 518)
-               
-               158         122 LOAD_FAST                6 (resp)
-                           124 LOAD_CONST               7 (0)
-                           126 BINARY_SUBSCR
-                           136 LOAD_CONST               8 ('error')
-                           138 BINARY_SUBSCR
-                           148 STORE_FAST               7 (error_data)
-               
-               159         150 LOAD_FAST                7 (error_data)
-                           152 LOAD_CONST               9 ('code')
-                           154 BINARY_SUBSCR
-                           164 STORE_FAST               8 (code)
-               
-               160         166 LOAD_FAST                6 (resp)
-                           168 LOAD_CONST               5 (1)
-                           170 BINARY_SUBSCR
-                           180 LOAD_ATTR                2 (status_code)
-                           190 STORE_FAST               9 (status)
-               
-               161         192 LOAD_FAST                7 (error_data)
-                           194 LOAD_CONST              10 ('message')
-                           196 BINARY_SUBSCR
-                           206 STORE_FAST              10 (msg)
-               
-               163         208 LOAD_FAST                8 (code)
-                           210 LOAD_CONST              11 (1006)
-                           212 COMPARE_OP               2 (==)
-                           218 POP_JUMP_FORWARD_IF_FALSE    17 (to 254)
-                           220 LOAD_GLOBAL              7 (NULL + NoLocationFound)
-                           232 LOAD_FAST                9 (status)
-                           234 LOAD_FAST                8 (code)
-                           236 LOAD_FAST               10 (msg)
-                           238 PRECALL                  3
-                           242 CALL                     3
-                           252 RAISE_VARARGS            1
-               
-               164     >>  254 LOAD_FAST                8 (code)
-                           256 LOAD_CONST              12 (2006)
-                           258 COMPARE_OP               2 (==)
-                           264 POP_JUMP_FORWARD_IF_FALSE    17 (to 300)
-                           266 LOAD_GLOBAL              9 (NULL + InvalidAPIKey)
-                           278 LOAD_FAST                9 (status)
-                           280 LOAD_FAST                8 (code)
-                           282 LOAD_FAST               10 (msg)
-                           284 PRECALL                  3
-                           288 CALL                     3
-                           298 RAISE_VARARGS            1
-               
-               165     >>  300 LOAD_FAST                8 (code)
-                           302 LOAD_CONST              13 (2007)
-                           304 COMPARE_OP               2 (==)
-                           310 POP_JUMP_FORWARD_IF_FALSE    17 (to 346)
-                           312 LOAD_GLOBAL             11 (NULL + APILimitExceeded)
-                           324 LOAD_FAST                9 (status)
-                           326 LOAD_FAST                8 (code)
-                           328 LOAD_FAST               10 (msg)
-                           330 PRECALL                  3
-                           334 CALL                     3
-                           344 RAISE_VARARGS            1
-               
-               166     >>  346 LOAD_FAST                8 (code)
-                           348 LOAD_CONST              14 (2008)
-                           350 COMPARE_OP               2 (==)
-                           356 POP_JUMP_FORWARD_IF_FALSE    17 (to 392)
-                           358 LOAD_GLOBAL             13 (NULL + APIKeyDisabled)
-                           370 LOAD_FAST                9 (status)
-                           372 LOAD_FAST                8 (code)
-                           374 LOAD_FAST               10 (msg)
-                           376 PRECALL                  3
-                           380 CALL                     3
-                           390 RAISE_VARARGS            1
-               
-               167     >>  392 LOAD_FAST                8 (code)
-                           394 LOAD_CONST              15 (2009)
-                           396 COMPARE_OP               2 (==)
-                           402 POP_JUMP_FORWARD_IF_FALSE    17 (to 438)
-                           404 LOAD_GLOBAL             15 (NULL + AccessDenied)
-                           416 LOAD_FAST                9 (status)
-                           418 LOAD_FAST                8 (code)
-                           420 LOAD_FAST               10 (msg)
-                           422 PRECALL                  3
-                           426 CALL                     3
-                           436 RAISE_VARARGS            1
-               
-               168     >>  438 LOAD_FAST                8 (code)
-                           440 LOAD_CONST              16 (9999)
-                           442 COMPARE_OP               2 (==)
-                           448 POP_JUMP_FORWARD_IF_FALSE    17 (to 484)
-                           450 LOAD_GLOBAL             17 (NULL + InternalApplicationError)
-                           462 LOAD_FAST                9 (status)
-                           464 LOAD_FAST                8 (code)
-                           466 LOAD_FAST               10 (msg)
-                           468 PRECALL                  3
-                           472 CALL                     3
-                           482 RAISE_VARARGS            1
-               
-               169     >>  484 LOAD_GLOBAL             19 (NULL + WeatherAPIException)
-                           496 LOAD_FAST                9 (status)
-                           498 LOAD_FAST                8 (code)
-                           500 LOAD_FAST               10 (msg)
-                           502 PRECALL                  3
-                           506 CALL                     3
-                           516 RAISE_VARARGS            1
-               
-               171     >>  518 LOAD_GLOBAL             21 (NULL + CurrentWeatherData)
-                           530 LOAD_FAST                6 (resp)
-                           532 LOAD_CONST               7 (0)
-                           534 BINARY_SUBSCR
-                           544 LOAD_CONST              17 ('current')
-                           546 BINARY_SUBSCR
-                           556 LOAD_FAST                6 (resp)
-                           558 LOAD_CONST               5 (1)
-                           560 BINARY_SUBSCR
-                           570 LOAD_ATTR                2 (status_code)
-                           580 LOAD_CONST               2 (None)
-                           582 PRECALL                  3
-                           586 CALL                     3
-                           596 STORE_FAST              11 (weather)
+               214          88 LOAD_GLOBAL              5 (NULL + CurrentWeatherData)
+                           100 LOAD_FAST                6 (resp)
+                           102 LOAD_CONST               5 (0)
+                           104 BINARY_SUBSCR
+                           114 LOAD_FAST                6 (resp)
+                           116 LOAD_CONST               6 (1)
+                           118 BINARY_SUBSCR
+                           128 LOAD_ATTR                3 (status_code)
+                           138 LOAD_CONST               2 (None)
+                           140 PRECALL                  3
+                           144 CALL                     3
+                           154 STORE_FAST               7 (weather)
                
-               172         598 LOAD_FAST               11 (weather)
-                           600 RETURN_VALUE
+               215         156 LOAD_FAST                7 (weather)
+                           158 RETURN_VALUE
                consts
-                  '\n        Get current weather data\n\n        Parameters\n        ----------\n        query: :class:`str`\n            Query string - location you want to get weather data for\n        lang: Optional[Union[:class:`str`, Languages]]\n            Language from the :class:`Languages` enum or a string representing the language or language code (preferably).\n            To get a list of languages visit :class:`Languages`.\n        aqi: Literal["yes", "no"]\n            Enable/Disable Air Quality data in forecast API output. Defaults to "no".\n        kwargs: Dict[:class:`str`, Any]\n            Additional keyword arguments to request\n\n        Returns\n        -------\n        :class:`CurrentWeatherData`\n            Current weather data class\n        '
+                  '\n        Get current weather data\n\n        Parameters\n        ----------\n        query: :class:`str`\n            Query string - location you want to get weather data for\n        lang: Optional[Union[:class:`str`, Languages]]\n            Language from the :class:`Languages` enum or a string representing the language or language code (preferably).\n            To get a list of languages visit :class:`Languages`.\n        aqi: Literal["yes", "no", None]\n            Enable/Disable Air Quality data in forecast API output. If nothing is passes, then it defaults to client default value.\n        kwargs: Dict[:class:`str`, Any]\n            Additional keyword arguments to request\n\n        Returns\n        -------\n        :class:`CurrentWeatherData`\n            Current weather data class\n\n        Raises\n        ---------\n        :exc:`NoLocationFound`\n            Raised when no location for given query was found\n        :exc:`InvalidAPIKey`\n            Raised when the API key is invalid\n        :exc:`APILimitExceeded`\n            Raised when API key calls limit was exceeded\n        :exc:`APIKeyDisabled`\n            Raised when API key is disabled\n        :exc:`AccessDenied`\n            Raised when access to given resource was denied\n        :exc:`InternalApplicationError`\n            Raised when there was a very rare internal application error\n        :exc:`WeatherAPIException`\n            Raised when something else went wrong, that does not have a specific exception class.\n        '
                   ('aqi', 'q')
                   None
                   'lang'
                   'current.json'
-                  1
-                  400
                   0
-                  'error'
-                  'code'
-                  'message'
-                  1006
-                  2006
-                  2007
-                  2008
-                  2009
-                  9999
-                  'current'
-               names      ('aqi', '_call_request', 'status_code', 'NoLocationFound', 'InvalidAPIKey', 'APILimitExceeded', 'APIKeyDisabled', 'AccessDenied', 'InternalApplicationError', 'WeatherAPIException', 'CurrentWeatherData')
-               varnames   ('self', 'query', 'lang', 'aqi', 'kwargs', 'options', 'resp', 'error_data', 'code', 'status', 'msg', 'weather')
+                  1
+               names      ('aqi', '_call_request', 'CurrentWeatherData', 'status_code')
+               varnames   ('self', 'query', 'lang', 'aqi', 'kwargs', 'options', 'resp', 'weather')
                freevars   ()
                cellvars   ()
                filename   'build\\bdist.win-amd64\\egg\\weatherly\\api\\client.py'
                name       'get_current_weather'
-               firstlineno 122
-               lnotab
-                  0x021b100102fe040302fd04050e012c0222021c0110011a0110022e012e
-                  012e012e012e012e0122025001
+               firstlineno 163
+               lnotab 0x022c100102fe040302fd04050e012c024401
+            code
+               argcount  : 2
+               nlocals   : 5
+               stacksize : 8
+               flags     : 3
+               code
+                  0x97007c00a0000000000000000000000000000000000000000000640164
+                  027c016901a6020000ab0200000000000000007d0267007d037c02640319
+                  00000000000000000044005d317d047c03a0010000000000000000000000
+                  0000000000000000007405000000000000000000007c047c026404190000
+                  000000000000006a0300000000000000006405a6030000ab030000000000
+                  000000a6010000ab01000000000000000001008c327c035300
+               217           0 RESUME                   0
+               
+               248           2 LOAD_FAST                0 (self)
+                             4 LOAD_METHOD              0 (_call_request)
+                            26 LOAD_CONST               1 ('search.json')
+                            28 LOAD_CONST               2 ('q')
+                            30 LOAD_FAST                1 (query)
+                            32 BUILD_MAP                1
+                            34 PRECALL                  2
+                            38 CALL                     2
+                            48 STORE_FAST               2 (resp)
+               
+               250          50 BUILD_LIST               0
+                            52 STORE_FAST               3 (locations)
+               
+               251          54 LOAD_FAST                2 (resp)
+                            56 LOAD_CONST               3 (0)
+                            58 BINARY_SUBSCR
+                            68 GET_ITER
+                       >>   70 FOR_ITER                49 (to 170)
+                            72 STORE_FAST               4 (loc)
+               
+               252          74 LOAD_FAST                3 (locations)
+                            76 LOAD_METHOD              1 (append)
+                            98 LOAD_GLOBAL              5 (NULL + LocationData)
+                           110 LOAD_FAST                4 (loc)
+                           112 LOAD_FAST                2 (resp)
+                           114 LOAD_CONST               4 (1)
+                           116 BINARY_SUBSCR
+                           126 LOAD_ATTR                3 (status_code)
+                           136 LOAD_CONST               5 (None)
+                           138 PRECALL                  3
+                           142 CALL                     3
+                           152 PRECALL                  1
+                           156 CALL                     1
+                           166 POP_TOP
+                           168 JUMP_BACKWARD           50 (to 70)
+               
+               253     >>  170 LOAD_FAST                3 (locations)
+                           172 RETURN_VALUE
+               consts
+                  '\n        Get locations for given query\n\n        Parameters\n        ---------------\n        query: :class:`str`\n            Query string, a location you are searching for\n\n        Returns\n        -----------\n        List[:class:`LocationData`]\n            A list of :class:`LocationData` classes.\n\n        Raises\n        ---------\n        :exc:`NoLocationFound`\n            Raised when no location for given query was found\n        :exc:`InvalidAPIKey`\n            Raised when the API key is invalid\n        :exc:`APILimitExceeded`\n            Raised when API key calls limit was exceeded\n        :exc:`APIKeyDisabled`\n            Raised when API key is disabled\n        :exc:`AccessDenied`\n            Raised when access to given resource was denied\n        :exc:`InternalApplicationError`\n            Raised when there was a very rare internal application error\n        :exc:`WeatherAPIException`\n            Raised when something else went wrong, that does not have a specific exception class.\n        '
+                  'search.json'
+                  'q'
+                  0
+                  1
+                  None
+               names      ('_call_request', 'append', 'LocationData', 'status_code')
+               varnames   ('self', 'query', 'resp', 'locations', 'loc')
+               freevars   ()
+               cellvars   ()
+               filename   'build\\bdist.win-amd64\\egg\\weatherly\\api\\client.py'
+               name       'get_locations'
+               firstlineno 217
+               lnotab 0x021f3002040114016001
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 7
+               flags     : 3
+               code
+                  0x970064017c006a0000000000000000006a0100000000000000009b0064
+                  027c006a0200000000000000006403190000000000000000009b0064047c
+                  006a0300000000000000009b0064059d075300
+               255           0 RESUME                   0
+               
+               256           2 LOAD_CONST               1 ('<')
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (__class__)
+                            16 LOAD_ATTR                1 (__name__)
+                            26 FORMAT_VALUE             0
+                            28 LOAD_CONST               2 (' api_key=')
+                            30 LOAD_FAST                0 (self)
+                            32 LOAD_ATTR                2 (default_options)
+                            42 LOAD_CONST               3 ('key')
+                            44 BINARY_SUBSCR
+                            54 FORMAT_VALUE             0
+                            56 LOAD_CONST               4 (' lang=')
+                            58 LOAD_FAST                0 (self)
+                            60 LOAD_ATTR                3 (lang)
+                            70 FORMAT_VALUE             0
+                            72 LOAD_CONST               5 ('>')
+                            74 BUILD_STRING             7
+                            76 RETURN_VALUE
+               consts
+                  None
+                  '<'
+                  ' api_key='
+                  'key'
+                  ' lang='
+                  '>'
+               names      ('__class__', '__name__', 'default_options', 'lang')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   'build\\bdist.win-amd64\\egg\\weatherly\\api\\client.py'
+               name       '__str__'
+               firstlineno 255
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 9
+               flags     : 3
+               code
+                  0x970074010000000000000000000064017c006a0100000000000000006a
+                  0200000000000000009b0064027c006a0300000000000000006403190000
+                  000000000000009b0064047c006a0400000000000000009b0064059d07a6
+                  010000ab0100000000000000005300
+               258           0 RESUME                   0
+               
+               259           2 LOAD_GLOBAL              1 (NULL + repr)
+                            14 LOAD_CONST               1 ('<')
+                            16 LOAD_FAST                0 (self)
+                            18 LOAD_ATTR                1 (__class__)
+                            28 LOAD_ATTR                2 (__name__)
+                            38 FORMAT_VALUE             0
+                            40 LOAD_CONST               2 (' api_key=')
+                            42 LOAD_FAST                0 (self)
+                            44 LOAD_ATTR                3 (default_options)
+                            54 LOAD_CONST               3 ('key')
+                            56 BINARY_SUBSCR
+                            66 FORMAT_VALUE             0
+                            68 LOAD_CONST               4 (' lang=')
+                            70 LOAD_FAST                0 (self)
+                            72 LOAD_ATTR                4 (lang)
+                            82 FORMAT_VALUE             0
+                            84 LOAD_CONST               5 ('>')
+                            86 BUILD_STRING             7
+                            88 PRECALL                  1
+                            92 CALL                     1
+                           102 RETURN_VALUE
+               consts
+                  None
+                  '<'
+                  ' api_key='
+                  'key'
+                  ' lang='
+                  '>'
+               names      ('repr', '__class__', '__name__', 'default_options', 'lang')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   'build\\bdist.win-amd64\\egg\\weatherly\\api\\client.py'
+               name       '__repr__'
+               firstlineno 258
+               lnotab 0x0201
             (None, None, None, None, 'no', 'no')
             (None, None)
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', 'Optional', 'Union', 'Languages', 'int', 'Literal', 'Dict', 'Any', '__init__', '_call_request', 'CurrentWeatherData', 'get_current_weather', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', 'Optional', 'Union', 'Languages', 'int', 'Literal', 'Dict', 'Any', '__init__', '_call_request', 'set_language', 'CurrentWeatherData', 'get_current_weather', 'get_locations', '__str__', '__repr__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'build\\bdist.win-amd64\\egg\\weatherly\\api\\client.py'
          name       'WeatherAPIClient'
-         firstlineno 55
+         firstlineno 56
          lnotab
             0x0c01041a0201020102010201020102f8040202fe02031efd02040efc02
-            050efb02060efa02070ef902080ef8020912f7020a02f60c1e340f020102
-            fd040102ff02021efe02030efd020412fc020502fb
+            050efb02060efa02070ef902080ef8020912f7020a02f60c20341d301802
+            0102fd040102ff02021efe02030efd020412fc020502fb08360c260603
       'WeatherAPIClient'
       None
-   names      ('__doc__', 'core', 'BaseAPIClient', 'enums', 'Languages', 'responses', 'CurrentWeatherData', 'errors', 'WeatherAPIException', 'NoLocationFound', 'InvalidAPIKey', 'APILimitExceeded', 'APIKeyDisabled', 'AccessDenied', 'InternalApplicationError', '', 'utils', 'typing', 'Any', 'Literal', 'Dict', 'Optional', 'Union', 'WEATHERAPI_BASE_URL', '__all__', 'WeatherAPIClient')
+   names      ('__doc__', 'core', 'BaseAPIClient', 'enums', 'Languages', 'responses', 'CurrentWeatherData', 'LocationData', 'errors', 'WeatherAPIException', 'NoLocationFound', 'InvalidAPIKey', 'APILimitExceeded', 'APIKeyDisabled', 'AccessDenied', 'InternalApplicationError', '', 'utils', 'typing', 'Any', 'Literal', 'Dict', 'Optional', 'Union', 'List', 'WEATHERAPI_BASE_URL', '__all__', 'WeatherAPIClient')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'build\\bdist.win-amd64\\egg\\weatherly\\api\\client.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020104180c010c010c0124090c041c0804020404
+   lnotab 0x00ff020104180c010c01100124090c04200904020404
```

## weatherly/api/__pycache__/core.cpython-311.pyc

### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xdaf03c64 (Mon Apr 17 07:10:18 2023 UTC)
-files sz: 2732
+moddate:  0xc52a4264 (Fri Apr 21 06:18:45 2023 UTC)
+files sz: 2752
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x970064005a00640164026c016d025a026d035a036d045a046d055a056d
@@ -101,15 +101,15 @@
             045a0c64055300
           45           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BaseAPIClient')
                        8 STORE_NAME               2 (__qualname__)
          
-          46          10 LOAD_CONST               1 ('\n    Represents a base API client that can handle requests. Used as a base class for ``WeatherAPIClient``\n    \n    Parameters\n    ----------\n    base_url: :class:`str`\n        An URL that will be used as a base for requests.\n    default_options: Optional[Dict[:class:`str`, Any]]\n        Default options for request that will be automatically added.\n    ')
+          46          10 LOAD_CONST               1 ('\n    Represents a base API client that can handle requests. Used as a base class for ``WeatherAPIClient``\n    \n    Parameters\n    ----------\n    base_url: :class:`str`\n        An URL that will be used as a base for requests.\n    default_options: Optional[Dict[:class:`str`, Any]]\n        Default options for requests made by the client that will be automatically added.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
           56          14 LOAD_CONST               2 ('base_url')
          
           58          16 LOAD_NAME                4 (str)
          
           56          18 LOAD_CONST               3 ('default_options')
@@ -162,15 +162,15 @@
                      146 LOAD_CONST               9 (<code object _request, file "build\bdist.win-amd64\egg\weatherly\api\core.py", line 64>)
                      148 MAKE_FUNCTION            4 (annotations)
                      150 STORE_NAME              12 (_request)
                      152 LOAD_CONST               5 (None)
                      154 RETURN_VALUE
          consts
             'BaseAPIClient'
-            '\n    Represents a base API client that can handle requests. Used as a base class for ``WeatherAPIClient``\n    \n    Parameters\n    ----------\n    base_url: :class:`str`\n        An URL that will be used as a base for requests.\n    default_options: Optional[Dict[:class:`str`, Any]]\n        Default options for request that will be automatically added.\n    '
+            '\n    Represents a base API client that can handle requests. Used as a base class for ``WeatherAPIClient``\n    \n    Parameters\n    ----------\n    base_url: :class:`str`\n        An URL that will be used as a base for requests.\n    default_options: Optional[Dict[:class:`str`, Any]]\n        Default options for requests made by the client that will be automatically added.\n    '
             'base_url'
             'default_options'
             'return'
             None
             code
                argcount  : 3
                nlocals   : 3
```

