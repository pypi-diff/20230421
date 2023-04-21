# Comparing `tmp/fuzzly-0.0.2.tar.gz` & `tmp/fuzzly-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzly-0.0.2.tar", last modified: Wed Feb 15 03:46:10 2023, max compression
+gzip compressed data, was "fuzzly-0.0.3.tar", last modified: Fri Apr 21 02:31:23 2023, max compression
```

## Comparing `fuzzly-0.0.2.tar` & `fuzzly-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 03:46:10.685457 fuzzly-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-02-15 03:45:46.000000 fuzzly-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-02-15 03:46:10.685457 fuzzly-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 03:46:10.685457 fuzzly-0.0.2/fuzzly/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 03:46:10.685457 fuzzly-0.0.2/fuzzly/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/api/post.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/api/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 03:46:10.685457 fuzzly-0.0.2/fuzzly/client/
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 03:46:10.685457 fuzzly-0.0.2/fuzzly/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/models/_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/models/_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/models/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/models/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/models/post.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-15 03:45:46.000000 fuzzly-0.0.2/fuzzly/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 03:46:10.685457 fuzzly-0.0.2/fuzzly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-02-15 03:46:10.000000 fuzzly-0.0.2/fuzzly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-02-15 03:46:10.000000 fuzzly-0.0.2/fuzzly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 03:46:10.000000 fuzzly-0.0.2/fuzzly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-15 03:46:10.000000 fuzzly-0.0.2/fuzzly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-15 03:46:10.000000 fuzzly-0.0.2/fuzzly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 03:46:10.685457 fuzzly-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-15 03:45:46.000000 fuzzly-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:31:23.114749 fuzzly-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-21 02:30:53.000000 fuzzly-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-21 02:31:23.114749 fuzzly-0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:31:23.110749 fuzzly-0.0.3/fuzzly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:31:23.114749 fuzzly-0.0.3/fuzzly/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/api/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/api/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:31:23.114749 fuzzly-0.0.3/fuzzly/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:31:23.114749 fuzzly-0.0.3/fuzzly/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17383 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:31:23.114749 fuzzly-0.0.3/fuzzly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-21 02:31:23.000000 fuzzly-0.0.3/fuzzly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-21 02:31:23.000000 fuzzly-0.0.3/fuzzly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 02:31:23.000000 fuzzly-0.0.3/fuzzly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 02:31:23.000000 fuzzly-0.0.3/fuzzly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 02:31:23.000000 fuzzly-0.0.3/fuzzly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 02:31:23.114749 fuzzly-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-21 02:30:53.000000 fuzzly-0.0.3/setup.py
```

### Comparing `fuzzly-0.0.2/LICENSE` & `fuzzly-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.2/PKG-INFO` & `fuzzly-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzly
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fuzz.ly client library for Python3
 Home-page: https://github.com/kheina-com/fuzzly
 Author: kheina
 License: Mozilla Public License 2.0
 Requires-Python: >=3.9.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fuzzly Version: 0.0.2 Summary: Fuzz.ly client
+Metadata-Version: 2.1 Name: fuzzly Version: 0.0.3 Summary: Fuzz.ly client
 library for Python3 Home-page: https://github.com/kheina-com/fuzzly Author:
 kheina License: Mozilla Public License 2.0 Requires-Python: >=3.9.*
 Description-Content-Type: text/markdown License-File: LICENSE
                                 [fuzzly Logo]
                [python-package_workflow] [pypi_package_version]
                       A python client library for fuzz.ly
 # Installation ```bash $ pip install fuzzly ``` # Usage ```python from fuzzly
```

### Comparing `fuzzly-0.0.2/fuzzly/__init__.py` & `fuzzly-0.0.3/fuzzly/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A python client library for fuzz.ly"""  # this comment should match the package slogan under the logo in the readme
 
 
-__version__: str = '0.0.2'
+__version__: str = '0.0.3'
 
 
 from typing import List
 
 from .api.post import FetchMyPosts, FetchPost
 from .api.tag import FetchPostTags, FetchTag
 from .client import Client
```

### Comparing `fuzzly-0.0.2/fuzzly/client/__init__.py` & `fuzzly-0.0.3/fuzzly/client/__init__.py`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.2/fuzzly/constants.py` & `fuzzly-0.0.3/fuzzly/constants.py`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.2/fuzzly/models/_shared.py` & `fuzzly-0.0.3/fuzzly/models/_shared.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,25 @@
 
 	NOTE: when used in fastapi or pydantic ensure PostId is called directly. either through a validator or manually.
 	EX: _post_id_validator = validator('post_id', pre=True, always=True, allow_reuse=True)(PostId)
 	"""
 
 	__str_format__: Pattern = re_compile(r'^[a-zA-Z0-9_-]{8}$')
 
+
+	@lru_cache(maxsize=128)
+	def _str_from_int(value: int) -> str :
+		return b64encode(int.to_bytes(value, 6, 'big')).decode()
+
+
+	@lru_cache(maxsize=128)
+	def _str_from_bytes(value: bytes) -> str :
+		return b64encode(value).decode()
+
+
 	def __new__(cls, value: Union[str, bytes, int]) :
 		# technically, the only thing needed to be done here to utilize the full 64 bit range is update the 6 bytes encoding to 8 and the allowed range in the int subtype
 
 		value_type: type = type(value)
 
 		if value_type == PostId :
 			return super(PostId, cls).__new__(cls, value)
@@ -44,24 +55,30 @@
 			return super(PostId, cls).__new__(cls, value)
 
 		elif value_type == int :
 			# the range of a 48 bit int stored in a 64 bit int (both starting at min values)
 			if not 0 <= value <= 281474976710655 :
 				raise ValueError('int values must be between 0 and 281474976710655.')
 
-			return super(PostId, cls).__new__(cls, b64encode(int.to_bytes(value, 6, 'big')).decode())
+			return super(PostId, cls).__new__(cls, PostId._str_from_int(value))
 
 		elif value_type == bytes :
 			if len(value) != 6 :
 				raise ValueError('bytes values must be exactly 6 bytes.')
 
-			return super(PostId, cls).__new__(cls, b64encode(value).decode())
+			return super(PostId, cls).__new__(cls, PostId._str_from_bytes(value))
+
+		# just in case there's some weirdness happening with types, but it's still a string
+		if isinstance(value, str) :
+			if not PostId.__str_format__.match(value) :
+				raise ValueError('str values must be in the format of /^[a-zA-Z0-9_-]{8}$/')
+
+			return super(PostId, cls).__new__(cls, value)
 
-		else :
-			raise NotImplementedError('value must be of type str, bytes, or int.')
+		raise NotImplementedError('value must be of type str, bytes, or int.')
 
 
 	@lru_cache(maxsize=128)
 	def int(self: 'PostId') -> int :
 		return int.from_bytes(b64decode(self), 'big')
 
 	__int__ = int
```

### Comparing `fuzzly-0.0.2/fuzzly/models/config.py` & `fuzzly-0.0.3/fuzzly/models/config.py`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.2/fuzzly/models/post.py` & `fuzzly-0.0.3/fuzzly/models/post.py`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.2/fuzzly/models/tag.py` & `fuzzly-0.0.3/fuzzly/models/tag.py`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.2/fuzzly.egg-info/PKG-INFO` & `fuzzly-0.0.3/fuzzly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzly
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fuzz.ly client library for Python3
 Home-page: https://github.com/kheina-com/fuzzly
 Author: kheina
 License: Mozilla Public License 2.0
 Requires-Python: >=3.9.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fuzzly Version: 0.0.2 Summary: Fuzz.ly client
+Metadata-Version: 2.1 Name: fuzzly Version: 0.0.3 Summary: Fuzz.ly client
 library for Python3 Home-page: https://github.com/kheina-com/fuzzly Author:
 kheina License: Mozilla Public License 2.0 Requires-Python: >=3.9.*
 Description-Content-Type: text/markdown License-File: LICENSE
                                 [fuzzly Logo]
                [python-package_workflow] [pypi_package_version]
                       A python client library for fuzz.ly
 # Installation ```bash $ pip install fuzzly ``` # Usage ```python from fuzzly
```

### Comparing `fuzzly-0.0.2/fuzzly.egg-info/SOURCES.txt` & `fuzzly-0.0.3/fuzzly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.2/setup.py` & `fuzzly-0.0.3/setup.py`

 * *Files identical despite different names*

