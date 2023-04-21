# Comparing `tmp/avro.py-2023.4.21.tar.gz` & `tmp/avro.py-2023.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avro.py-2023.4.21.tar", last modified: Fri Apr 21 16:45:24 2023, max compression
+gzip compressed data, was "avro.py-2023.4.3.tar", last modified: Mon Apr  3 06:07:59 2023, max compression
```

## Comparing `avro.py-2023.4.21.tar` & `avro.py-2023.4.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:45:24.151537 avro.py-2023.4.21/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-21 16:45:10.000000 avro.py-2023.4.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 16:45:10.000000 avro.py-2023.4.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-21 16:45:24.151537 avro.py-2023.4.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-21 16:45:10.000000 avro.py-2023.4.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:45:24.147537 avro.py-2023.4.21/avro/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1316 2023-04-21 16:45:10.000000 avro.py-2023.4.21/avro/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-04-21 16:45:10.000000 avro.py-2023.4.21/avro/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11719 2023-04-21 16:45:10.000000 avro.py-2023.4.21/avro/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:45:24.151537 avro.py-2023.4.21/avro/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-21 16:45:10.000000 avro.py-2023.4.21/avro/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59057 2023-04-21 16:45:10.000000 avro.py-2023.4.21/avro/resources/avrodict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:45:24.151537 avro.py-2023.4.21/avro/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-21 16:45:10.000000 avro.py-2023.4.21/avro/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1645 2023-04-21 16:45:10.000000 avro.py-2023.4.21/avro/utils/count.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2800 2023-04-21 16:45:10.000000 avro.py-2023.4.21/avro/utils/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:45:24.151537 avro.py-2023.4.21/avro.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-21 16:45:24.000000 avro.py-2023.4.21/avro.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-21 16:45:24.000000 avro.py-2023.4.21/avro.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:45:24.000000 avro.py-2023.4.21/avro.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 16:45:24.000000 avro.py-2023.4.21/avro.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-21 16:45:10.000000 avro.py-2023.4.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 16:45:24.151537 avro.py-2023.4.21/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-04-21 16:45:10.000000 avro.py-2023.4.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:45:24.151537 avro.py-2023.4.21/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5744 2023-04-21 16:45:10.000000 avro.py-2023.4.21/tests/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2109 2023-04-21 16:45:10.000000 avro.py-2023.4.21/tests/test_utils_count.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3750 2023-04-21 16:45:10.000000 avro.py-2023.4.21/tests/test_utils_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:07:59.498247 avro.py-2023.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-03 06:07:47.000000 avro.py-2023.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-03 06:07:47.000000 avro.py-2023.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-03 06:07:59.498247 avro.py-2023.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-03 06:07:47.000000 avro.py-2023.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:07:59.494247 avro.py-2023.4.3/avro/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11711 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:07:59.498247 avro.py-2023.4.3/avro/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58945 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/resources/avrodict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:07:59.498247 avro.py-2023.4.3/avro/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1637 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/utils/count.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2792 2023-04-03 06:07:47.000000 avro.py-2023.4.3/avro/utils/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:07:59.494247 avro.py-2023.4.3/avro.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-03 06:07:59.000000 avro.py-2023.4.3/avro.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-03 06:07:59.000000 avro.py-2023.4.3/avro.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 06:07:59.000000 avro.py-2023.4.3/avro.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-03 06:07:59.000000 avro.py-2023.4.3/avro.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-03 06:07:47.000000 avro.py-2023.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 06:07:59.498247 avro.py-2023.4.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-04-03 06:07:47.000000 avro.py-2023.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:07:59.498247 avro.py-2023.4.3/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5735 2023-04-03 06:07:47.000000 avro.py-2023.4.3/tests/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-04-03 06:07:47.000000 avro.py-2023.4.3/tests/test_utils_count.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3742 2023-04-03 06:07:47.000000 avro.py-2023.4.3/tests/test_utils_validate.py
```

### Comparing `avro.py-2023.4.21/LICENSE` & `avro.py-2023.4.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 MIT License
 
 Copyright (c) 2022-present HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the 'Software'), to deal
+of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

### Comparing `avro.py-2023.4.21/PKG-INFO` & `avro.py-2023.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro.py
-Version: 2023.4.21
+Version: 2023.4.3
 Summary: A modern Pythonic implementation of Avro Phonetic.
 Home-page: https://github.com/hitblast/avro.py
 Author: HitBlast
 Author-email: hitblastlive@gmail.com
 License: MIT
 Keywords: python,avro,avro phonetic,bangla,bangla phonetics,bengali,bengali phonetics
 Classifier: Intended Audience :: Developers
```

### Comparing `avro.py-2023.4.21/README.md` & `avro.py-2023.4.3/README.md`

 * *Files identical despite different names*

### Comparing `avro.py-2023.4.21/avro/__init__.py` & `avro.py-2023.4.3/avro/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## A modern Pythonic implementation of Avro Phonetic.
 
 ---
 
 MIT License
 
-Copyright (c) 2022-present HitBlast
+Copyright (c) 2022 HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the 'Software'), to deal
+of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
@@ -26,13 +26,13 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 '''
 
 
 # Set version information.
-__version_info__ = ('2023', '4', '21')  # YYYY / MM / DD
+__version_info__ = ('2023', '4', '3')  # YYYY / MM / DD
 __version__ = '.'.join(__version_info__)
 
 
 # Import local modules.
 from .main import *
```

### Comparing `avro.py-2023.4.21/avro/config.py` & `avro.py-2023.4.3/avro/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## A modern Pythonic implementation of Avro Phonetic.
 
 ---
 
 MIT License
 
-Copyright (c) 2022-present HitBlast
+Copyright (c) 2022 HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the 'Software'), to deal
+of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

### Comparing `avro.py-2023.4.21/avro/main.py` & `avro.py-2023.4.3/avro/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## A modern Pythonic implementation of Avro Phonetic.
 
 ---
 
 MIT License
 
-Copyright (c) 2022-present HitBlast
+Copyright (c) 2022 HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the 'Software'), to deal
+of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

### Comparing `avro.py-2023.4.21/avro/resources/__init__.py` & `avro.py-2023.4.3/avro/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `avro.py-2023.4.21/avro/resources/avrodict.py` & `avro.py-2023.4.3/avro/resources/avrodict.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 ## The Avro Dictionary (Adapted)
 
 ---
 
 MIT License
 
-Copyright (c) 2022-present HitBlast
+Copyright (c) 2022 HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the 'Software'), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
@@ -36,17 +36,17 @@
 # The dictionary variable.
 AVRO_DICT: Dict[str, str] = {
     "meta": {
         "file_name": "avrodict.py",
         "file_description": "Provides Avro Dictionary in native Python dictionary. Adapted from avrodict.json",
         "package": "avro.py",
         "license": "MIT License",
-        "source": "https://github.com/hitblast/avro.py/blob/main/avro/resources/avrodict.py",
+        "source": "https://github.com/kaustavdm/pyAvroPhonetic/blob/master/pyavrophonetic/resources/avrodict.json",
         "adapted_by": "HitBlast",
-        "updated": "20230421",
+        "updated": "20230403",
         "encoding": "utf-8"
     },
     "data": {
         "patterns": [
             {
                 "find": "bhl",
                 "replace": "ভ্ল"
@@ -113,15 +113,16 @@
             {
                 "find": "cc",
                 "replace": "চ্চ",
                 "reverse": "cc"
             },
             {
                 "find": "ch",
-                "replace": "ছ"
+                "replace": "ছ",
+                "reverse": "s"
             },
             {
                 "find": "c",
                 "replace": "চ",
                 "reverse": "ch"
             },
             {
@@ -2017,18 +2018,15 @@
             # }
         ],
 
         # Remapped words
         "exceptions": {
             "ফেসবুক": "Facebook",
             "গুগল": "Google",
-            "উইকিপিডিয়া": "Wikipedia",
-            "হোয়াটসঅ্যাপ": "Whatsapp",
-            "টুইটার": "Twitter",
-            "লিঙ্কডইন": "Linkedin"
+            "উইকিপিডিয়া": "Wikipedia"
         },
 
         # Constant values
         "vowel": "aeiou",
         "consonant": "bcdfghjklmnpqrstvwxyz",
         "casesensitive": "oiudgjnrstyz",
         "number": "0123456789",
```

### Comparing `avro.py-2023.4.21/avro/utils/__init__.py` & `avro.py-2023.4.3/avro/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## Utils package for avro.py
 
 ---
 
 MIT License
 
-Copyright (c) 2022-present HitBlast
+Copyright (c) 2022 HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the 'Software'), to deal
+of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

### Comparing `avro.py-2023.4.21/avro/utils/count.py` & `avro.py-2023.4.3/avro/utils/count.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## Count functions (avro.utils) for avro.py
 
 ---
 
 MIT License
 
-Copyright (c) 2022-present HitBlast
+Copyright (c) 2022 HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the 'Software'), to deal
+of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

### Comparing `avro.py-2023.4.21/avro/utils/validate.py` & `avro.py-2023.4.3/avro/utils/validate.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## Validation functions (avro.utils) for avro.py
 
 ---
 
 MIT License
 
-Copyright (c) 2022-present HitBlast
+Copyright (c) 2022 HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the 'Software'), to deal
+of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

### Comparing `avro.py-2023.4.21/avro.py.egg-info/PKG-INFO` & `avro.py-2023.4.3/avro.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro.py
-Version: 2023.4.21
+Version: 2023.4.3
 Summary: A modern Pythonic implementation of Avro Phonetic.
 Home-page: https://github.com/hitblast/avro.py
 Author: HitBlast
 Author-email: hitblastlive@gmail.com
 License: MIT
 Keywords: python,avro,avro phonetic,bangla,bangla phonetics,bengali,bengali phonetics
 Classifier: Intended Audience :: Developers
```

### Comparing `avro.py-2023.4.21/setup.py` & `avro.py-2023.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `avro.py-2023.4.21/tests/test_main.py` & `avro.py-2023.4.3/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## Test cases for avro.main
 
 ---
 
 MIT License
 
-Copyright (c) 2022-present HitBlast
+Copyright (c) 2022 HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the 'Software'), to deal
+of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
@@ -185,10 +185,10 @@
 
 def test_reverse_func() -> None:
     '''
     ### Test reverse-parsing with sentences.
     '''
 
     assert 'ami banglay gan gai' == avro.reverse('আমি বাংলায় গান গাই')
-    assert 'rahim, tomake korim dakche. ekhon ki rowna debe?' == avro.reverse(
+    assert 'rahim, tomake korim dakse. ekhon ki rowna debe?' == avro.reverse(
         'রাহিম, তোমাকে করিম ডাকছে। এখন কি রওনা দেবে?'
     )
```

### Comparing `avro.py-2023.4.21/tests/test_utils_count.py` & `avro.py-2023.4.3/tests/test_utils_count.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## Test cases for avro.utils.count
 
 ---
 
 MIT License
 
-Copyright (c) 2022-present HitBlast
+Copyright (c) 2022 HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the 'Software'), to deal
+of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

### Comparing `avro.py-2023.4.21/tests/test_utils_validate.py` & `avro.py-2023.4.3/tests/test_utils_validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ## Test cases for avro.utils.validate
 
 ---
 
 MIT License
 
-Copyright (c) 2022-present HitBlast
+Copyright (c) 2022 HitBlast
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the 'Software'), to deal
+of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

