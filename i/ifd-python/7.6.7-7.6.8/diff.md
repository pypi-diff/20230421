# Comparing `tmp/ifd_python-7.6.7.tar.gz` & `tmp/ifd_python-7.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifd_python-7.6.7.tar", max compression
+gzip compressed data, was "ifd_python-7.6.8.tar", max compression
```

## Comparing `ifd_python-7.6.7.tar` & `ifd_python-7.6.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.6.7/LICENSE
--rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.6.7/README.md
--rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.6.7/ifd/__init__.py
--rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.6.7/ifd/entities/Abstract/ADetection.py
--rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.6.7/ifd/entities/Abstract/__init__.py
--rw-r--r--   0        0        0      734 2023-04-19 13:21:34.036921 ifd_python-7.6.7/ifd/entities/Classification.py
--rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.6.7/ifd/entities/Couleur.py
--rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-7.6.7/ifd/entities/Detection.py
--rw-r--r--   0        0        0     2303 2023-04-19 08:19:41.294208 ifd_python-7.6.7/ifd/entities/Image.py
--rw-r--r--   0        0        0     1377 2023-04-19 11:57:33.930576 ifd_python-7.6.7/ifd/entities/LogResult.py
--rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-7.6.7/ifd/entities/Modele.py
--rw-r--r--   0        0        0      666 2023-04-14 14:33:26.310964 ifd_python-7.6.7/ifd/entities/OCR.py
--rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.6.7/ifd/entities/RabbitMqMessage.py
--rw-r--r--   0        0        0      709 2023-04-19 08:27:21.531854 ifd_python-7.6.7/ifd/entities/Tag.py
--rw-r--r--   0        0        0      262 2023-04-19 09:19:06.169869 ifd_python-7.6.7/ifd/entities/__init__.py
--rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-7.6.7/ifd/entities/bbox.py
--rw-r--r--   0        0        0     2219 2023-04-14 12:09:37.448293 ifd_python-7.6.7/ifd/repository/AmqpImageRepository.py
--rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.6.7/ifd/repository/Interfaces/IImageRepository.py
--rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.6.7/ifd/repository/Interfaces/__init__.py
--rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.6.7/ifd/repository/MemoryImageRepository.py
--rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.6.7/ifd/repository/__init__.py
--rw-r--r--   0        0        0      644 2023-04-17 07:37:46.512419 ifd_python-7.6.7/ifd/spec.py
--rw-r--r--   0        0        0      526 2023-04-19 08:19:41.298208 ifd_python-7.6.7/ifd/tools.py
--rw-r--r--   0        0        0      131 2023-04-14 12:36:19.030168 ifd_python-7.6.7/ifd/usecase/Interfaces/IFonction.py
--rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.6.7/ifd/usecase/Interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 13:21:50.637127 ifd_python-7.6.7/ifd/usecase/__init__.py
--rw-r--r--   0        0        0      329 2023-04-19 13:22:00.629251 ifd_python-7.6.7/pyproject.toml
--rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 ifd_python-7.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.6.8/LICENSE
+-rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.6.8/README.md
+-rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/entities/Abstract/ADetection.py
+-rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/entities/Abstract/__init__.py
+-rw-r--r--   0        0        0      734 2023-04-19 13:21:34.036921 ifd_python-7.6.8/ifd/entities/Classification.py
+-rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/entities/Couleur.py
+-rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-7.6.8/ifd/entities/Detection.py
+-rw-r--r--   0        0        0     2303 2023-04-19 08:19:41.294208 ifd_python-7.6.8/ifd/entities/Image.py
+-rw-r--r--   0        0        0     1377 2023-04-19 11:57:33.930576 ifd_python-7.6.8/ifd/entities/LogResult.py
+-rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-7.6.8/ifd/entities/Modele.py
+-rw-r--r--   0        0        0      777 2023-04-21 09:53:14.432345 ifd_python-7.6.8/ifd/entities/OCR.py
+-rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/entities/RabbitMqMessage.py
+-rw-r--r--   0        0        0      709 2023-04-19 08:27:21.531854 ifd_python-7.6.8/ifd/entities/Tag.py
+-rw-r--r--   0        0        0      262 2023-04-19 09:19:06.169869 ifd_python-7.6.8/ifd/entities/__init__.py
+-rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-7.6.8/ifd/entities/bbox.py
+-rw-r--r--   0        0        0     2219 2023-04-14 12:09:37.448293 ifd_python-7.6.8/ifd/repository/AmqpImageRepository.py
+-rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/repository/Interfaces/IImageRepository.py
+-rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/repository/Interfaces/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/repository/MemoryImageRepository.py
+-rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/repository/__init__.py
+-rw-r--r--   0        0        0      644 2023-04-17 07:37:46.512419 ifd_python-7.6.8/ifd/spec.py
+-rw-r--r--   0        0        0      526 2023-04-19 08:19:41.298208 ifd_python-7.6.8/ifd/tools.py
+-rw-r--r--   0        0        0      131 2023-04-14 12:36:19.030168 ifd_python-7.6.8/ifd/usecase/Interfaces/IFonction.py
+-rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/usecase/Interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:53:31.196553 ifd_python-7.6.8/ifd/usecase/__init__.py
+-rw-r--r--   0        0        0      329 2023-04-21 09:53:40.652670 ifd_python-7.6.8/pyproject.toml
+-rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 ifd_python-7.6.8/PKG-INFO
```

### Comparing `ifd_python-7.6.7/LICENSE` & `ifd_python-7.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.7/README.md` & `ifd_python-7.6.8/README.md`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.7/ifd/entities/Abstract/ADetection.py` & `ifd_python-7.6.8/ifd/entities/Abstract/ADetection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.7/ifd/entities/Classification.py` & `ifd_python-7.6.8/ifd/entities/Classification.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.7/ifd/entities/Detection.py` & `ifd_python-7.6.8/ifd/entities/Detection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.7/ifd/entities/Image.py` & `ifd_python-7.6.8/ifd/entities/Image.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.7/ifd/entities/LogResult.py` & `ifd_python-7.6.8/ifd/entities/LogResult.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.7/ifd/entities/OCR.py` & `ifd_python-7.6.8/ifd/entities/OCR.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from .Abstract import ADetection
 
 class OCR(ADetection):
-    score_ocr: float
+    score : float
     label_ocr: str
     score_match: float
 
     def serialize(self):
         data = super().serialize()
+        data["score"] = self.score
         data["label_ocr"] = self.label_ocr
         data["score_match"] = self.score_match
         return data
         
     def deserialize(self, data):
         super().deserialize(data)
 
         for field in data:
             if data[field] is None:
                 pass
             elif field == "label_ocr":
                 self.label_ocr = data[field]
             elif field == "score_match":
                 self.score_match = data[field]
+            elif field == "score":
+                self.score = data[field]
         return self
```

### Comparing `ifd_python-7.6.7/ifd/entities/RabbitMqMessage.py` & `ifd_python-7.6.8/ifd/entities/RabbitMqMessage.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.7/ifd/entities/Tag.py` & `ifd_python-7.6.8/ifd/entities/Tag.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.7/ifd/entities/bbox.py` & `ifd_python-7.6.8/ifd/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.7/ifd/repository/AmqpImageRepository.py` & `ifd_python-7.6.8/ifd/repository/AmqpImageRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.7/ifd/spec.py` & `ifd_python-7.6.8/ifd/spec.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.7/ifd/tools.py` & `ifd_python-7.6.8/ifd/tools.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.7/PKG-INFO` & `ifd_python-7.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifd-python
-Version: 7.6.7
+Version: 7.6.8
 Summary: 
 Author: Antonin Lemoine
 Author-email: antonin.lemoine@altitudeinfra.fr
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

