# Comparing `tmp/tsidpy-1.1.0.0.tar.gz` & `tmp/tsidpy-1.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsidpy-1.1.0.0.tar", last modified: Mon Apr 10 22:29:21 2023, max compression
+gzip compressed data, was "tsidpy-1.1.0.1.tar", last modified: Fri Apr 21 16:39:51 2023, max compression
```

## Comparing `tsidpy-1.1.0.0.tar` & `tsidpy-1.1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-10 22:29:21.347532 tsidpy-1.1.0.0/
--rw-r--r--   0 luis       (504) staff       (20)     1066 2023-04-09 01:27:26.000000 tsidpy-1.1.0.0/LICENSE
--rw-r--r--   0 luis       (504) staff       (20)    10499 2023-04-10 22:29:21.346385 tsidpy-1.1.0.0/PKG-INFO
--rw-r--r--   0 luis       (504) staff       (20)     9982 2023-04-10 22:16:17.000000 tsidpy-1.1.0.0/README.md
--rw-r--r--   0 luis       (504) staff       (20)      594 2023-04-10 22:17:00.000000 tsidpy-1.1.0.0/pyproject.toml
--rw-r--r--   0 luis       (504) staff       (20)       38 2023-04-10 22:29:21.347854 tsidpy-1.1.0.0/setup.cfg
-drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-10 22:29:21.335232 tsidpy-1.1.0.0/src/
-drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-10 22:29:21.341328 tsidpy-1.1.0.0/src/tsidpy/
--rw-r--r--   0 luis       (504) staff       (20)       63 2023-04-10 20:20:01.000000 tsidpy-1.1.0.0/src/tsidpy/__init__.py
--rw-r--r--   0 luis       (504) staff       (20)      690 2023-04-07 23:41:36.000000 tsidpy-1.1.0.0/src/tsidpy/basen.py
--rw-r--r--   0 luis       (504) staff       (20)    15237 2023-04-10 21:52:42.000000 tsidpy-1.1.0.0/src/tsidpy/tsid.py
-drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-10 22:29:21.345124 tsidpy-1.1.0.0/src/tsidpy.egg-info/
--rw-r--r--   0 luis       (504) staff       (20)    10499 2023-04-10 22:29:21.000000 tsidpy-1.1.0.0/src/tsidpy.egg-info/PKG-INFO
--rw-r--r--   0 luis       (504) staff       (20)      230 2023-04-10 22:29:21.000000 tsidpy-1.1.0.0/src/tsidpy.egg-info/SOURCES.txt
--rw-r--r--   0 luis       (504) staff       (20)        1 2023-04-10 22:29:21.000000 tsidpy-1.1.0.0/src/tsidpy.egg-info/dependency_links.txt
--rw-r--r--   0 luis       (504) staff       (20)        7 2023-04-10 22:29:21.000000 tsidpy-1.1.0.0/src/tsidpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:39:51.504803 tsidpy-1.1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-21 16:39:40.000000 tsidpy-1.1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-04-21 16:39:51.504803 tsidpy-1.1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-04-21 16:39:40.000000 tsidpy-1.1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-21 16:39:40.000000 tsidpy-1.1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 16:39:51.504803 tsidpy-1.1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:39:51.504803 tsidpy-1.1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:39:51.504803 tsidpy-1.1.0.1/src/tsidpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 16:39:40.000000 tsidpy-1.1.0.1/src/tsidpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-21 16:39:40.000000 tsidpy-1.1.0.1/src/tsidpy/basen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16048 2023-04-21 16:39:40.000000 tsidpy-1.1.0.1/src/tsidpy/tsid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:39:51.504803 tsidpy-1.1.0.1/src/tsidpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-04-21 16:39:51.000000 tsidpy-1.1.0.1/src/tsidpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-21 16:39:51.000000 tsidpy-1.1.0.1/src/tsidpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:39:51.000000 tsidpy-1.1.0.1/src/tsidpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 16:39:51.000000 tsidpy-1.1.0.1/src/tsidpy.egg-info/top_level.txt
```

### Comparing `tsidpy-1.1.0.0/LICENSE` & `tsidpy-1.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsidpy-1.1.0.0/PKG-INFO` & `tsidpy-1.1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsidpy
-Version: 1.1.0.0
+Version: 1.1.0.1
 Summary: A Python library for generating Time-Sorted Unique Identifiers (TSID)
 Author-email: Luis Medel <luis@luismedel.com>
 Project-URL: Homepage, https://github.com/luismedel/tsid-python
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tsidpy-1.1.0.0/README.md` & `tsidpy-1.1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tsidpy-1.1.0.0/pyproject.toml` & `tsidpy-1.1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tsidpy"
-version = "1.1.0.0"
+version = "1.1.0.1"
 authors = [
   { name="Luis Medel", email="luis@luismedel.com" },
 ]
 description = "A Python library for generating Time-Sorted Unique Identifiers (TSID)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tsidpy-1.1.0.0/src/tsidpy/basen.py` & `tsidpy-1.1.0.1/src/tsidpy/basen.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,11 +26,7 @@
     result: int = 0
 
     for c in value:
         result *= base
         result += ALPHABET.index(c)
 
     return result
-
-
-if __name__ == '__main__':
-    print(encode(256, 16))
```

### Comparing `tsidpy-1.1.0.0/src/tsidpy/tsid.py` & `tsidpy-1.1.0.1/src/tsidpy/tsid.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from datetime import datetime
 
 from .basen import decode, encode
 
 TSID_BYTES: int = 8
 TSID_CHARS: int = 13
+TSID_HEXCHARS: int = 16
 
 _EPOCH_ISO: str = '2020-01-01 00:00:00+00:00'
 TSID_EPOCH: float = datetime.fromisoformat(_EPOCH_ISO).timestamp() * 1000
 
 RANDOM_BITS: int = 22
 RANDOM_MASK: int = 0x3fffff
 
@@ -196,14 +197,20 @@
         >>> t = TSID(0xffffffffffffffff)
         >>> t.to_string()
         'FZZZZZZZZZZZZ'
 
         >>> t = TSID(0x000000000000000a)
         >>> t.to_string()
         '000000000000A'
+
+        >>> t = TSID(437283649808777971)
+        >>> t.to_string('d')
+        '437283649808777971'
+        >>> t.to_string('z')
+        'WIlLsHwljH'
         """
 
         result: str
 
         match fmt:
             case 'S':  # canonical string in upper case
                 result = self._to_canonical_string()
@@ -261,15 +268,15 @@
         True
         >>> TSID.from_bytes(b'\x00\x00\x00\x00\x00\x00\x00\x02') == TSID(2)
         True
         >>> TSID.from_bytes(b'\x00\x00\x00\x00\x00\x00\x00\x0b') == TSID(11)
         True
         """
         if len(bytes) != TSID_BYTES:
-            raise ValueError(f'Invalid TSID bytes (len {len(bytes)}, '
+            raise ValueError(f'Invalid TSID bytes (len={len(bytes)} bytes, '
                              f'expected {TSID_BYTES})')
 
         number: int = int.from_bytes(bytes, byteorder='big', signed=False)
         return TSID(number)
 
     @staticmethod
     def from_string(value: str, fmt: str = 'S') -> 'TSID':
@@ -289,20 +296,30 @@
         True
         """
         number: int
 
         match fmt:
             case 'S' | 's':
                 if len(value) != TSID_CHARS:
-                    raise ValueError("Invalid TSID string")
+                    raise ValueError(f'Invalid TSID string: '
+                                     f'(len={len(value)} chars, '
+                                     f'but expected {TSID_CHARS})')
                 number = sum(ALPHABET_VALUES[ord(value[i])] << h
                              for i, h in enumerate(range(60, -5, -5), 0))
             case 'X':  # hexadecimal in upper case
+                if len(value) != TSID_HEXCHARS:
+                    raise ValueError(f'Invalid TSID string: '
+                                     f'(len={len(value)} chars, '
+                                     f'but expected {TSID_HEXCHARS})')
                 number = decode(value, 16)
             case 'x':  # hexadecimal in lower case
+                if len(value) != TSID_HEXCHARS:
+                    raise ValueError(f'Invalid TSID string: '
+                                      f'(len={len(value)} chars, '
+                                     f'but expected {TSID_HEXCHARS})')
                 number = decode(value.upper(), 16)
             case 'd':  # base-10
                 number = decode(value, 10)
             case 'z':  # base-62
                 number = decode(value, 62)
             case _:
                 raise ValueError(f"Invalid format: '{fmt}'")
```

### Comparing `tsidpy-1.1.0.0/src/tsidpy.egg-info/PKG-INFO` & `tsidpy-1.1.0.1/src/tsidpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsidpy
-Version: 1.1.0.0
+Version: 1.1.0.1
 Summary: A Python library for generating Time-Sorted Unique Identifiers (TSID)
 Author-email: Luis Medel <luis@luismedel.com>
 Project-URL: Homepage, https://github.com/luismedel/tsid-python
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

