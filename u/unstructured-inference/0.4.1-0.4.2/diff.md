# Comparing `tmp/unstructured_inference-0.4.1.tar.gz` & `tmp/unstructured_inference-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_inference-0.4.1.tar", last modified: Thu Apr 20 17:38:11 2023, max compression
+gzip compressed data, was "unstructured_inference-0.4.2.tar", last modified: Fri Apr 21 04:10:10 2023, max compression
```

## Comparing `unstructured_inference-0.4.1.tar` & `unstructured_inference-0.4.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:38:11.517226 unstructured_inference-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-20 17:38:11.517226 unstructured_inference-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:38:11.513226 unstructured_inference-0.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-20 17:38:11.521226 unstructured_inference-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:38:11.513226 unstructured_inference-0.4.1/unstructured_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:38:11.517226 unstructured_inference-0.4.1/unstructured_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/inference/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/inference/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/inference/layoutelement.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:38:11.517226 unstructured_inference-0.4.1/unstructured_inference/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/donut.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/paddle_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/table_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/tesseract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/unstructuredmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/yolox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:38:11.513226 unstructured_inference-0.4.1/unstructured_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-20 17:38:11.000000 unstructured_inference-0.4.1/unstructured_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-20 17:38:11.000000 unstructured_inference-0.4.1/unstructured_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 17:38:11.000000 unstructured_inference-0.4.1/unstructured_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-20 17:38:11.000000 unstructured_inference-0.4.1/unstructured_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 17:38:11.000000 unstructured_inference-0.4.1/unstructured_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:10:10.094570 unstructured_inference-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-21 04:10:10.094570 unstructured_inference-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:10:10.078570 unstructured_inference-0.4.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-21 04:10:10.094570 unstructured_inference-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:10:10.082570 unstructured_inference-0.4.2/unstructured_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:10:10.086570 unstructured_inference-0.4.2/unstructured_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/inference/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/inference/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/inference/layoutelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:10:10.094570 unstructured_inference-0.4.2/unstructured_inference/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/donut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/paddle_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/table_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/tesseract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/unstructuredmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/models/yolox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-04-21 04:07:46.000000 unstructured_inference-0.4.2/unstructured_inference/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:10:10.082570 unstructured_inference-0.4.2/unstructured_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-21 04:10:09.000000 unstructured_inference-0.4.2/unstructured_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-21 04:10:10.000000 unstructured_inference-0.4.2/unstructured_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 04:10:09.000000 unstructured_inference-0.4.2/unstructured_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-21 04:10:09.000000 unstructured_inference-0.4.2/unstructured_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 04:10:09.000000 unstructured_inference-0.4.2/unstructured_inference.egg-info/top_level.txt
```

### Comparing `unstructured_inference-0.4.1/PKG-INFO` & `unstructured_inference-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured_inference
-Version: 0.4.1
+Version: 0.4.2
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.4.1/README.md` & `unstructured_inference-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.1/setup.py` & `unstructured_inference-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.1/unstructured_inference/api.py` & `unstructured_inference-0.4.2/unstructured_inference/api.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.1/unstructured_inference/inference/elements.py` & `unstructured_inference-0.4.2/unstructured_inference/inference/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.1/unstructured_inference/inference/layout.py` & `unstructured_inference-0.4.2/unstructured_inference/inference/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,16 +275,19 @@
     pdf_objects: Optional[List[TextRegion]] = None,
     ocr_strategy: str = "auto",
     ocr_languages: str = "eng",
     extract_tables: bool = False,
 ) -> LayoutElement:
     """Creates a LayoutElement from a given layout or image by finding all the text that lies within
     a given block."""
-    element = LayoutElement.from_region(block)
-    element.text = block.extract_text(
+    if isinstance(block, LayoutElement):
+        element = block
+    else:
+        element = LayoutElement.from_region(block)
+    element.text = element.extract_text(
         objects=pdf_objects,
         image=image,
         extract_tables=extract_tables,
         ocr_strategy=ocr_strategy,
         ocr_languages=ocr_languages,
     )
     return element
```

### Comparing `unstructured_inference-0.4.1/unstructured_inference/inference/layoutelement.py` & `unstructured_inference-0.4.2/unstructured_inference/inference/layoutelement.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,27 +18,23 @@
         objects: Optional[List[TextRegion]],
         image: Optional[Image.Image] = None,
         extract_tables: bool = False,
         ocr_strategy: str = "auto",
         ocr_languages: str = "eng",
     ):
         """Extracts text contained in region"""
-        if self.text is not None:
-            # If block text is already populated, we'll assume it's correct
-            text = self.text
-        elif extract_tables and isinstance(self, LayoutElement) and self.type == "Table":
-            text = interprete_table_block(self, image)
-        else:
-            text = super().extract_text(
-                objects=objects,
-                image=image,
-                extract_tables=extract_tables,
-                ocr_strategy=ocr_strategy,
-                ocr_languages=ocr_languages,
-            )
+        text = super().extract_text(
+            objects=objects,
+            image=image,
+            extract_tables=extract_tables,
+            ocr_strategy=ocr_strategy,
+            ocr_languages=ocr_languages,
+        )
+        if extract_tables and self.type == "Table":
+            self.text_as_html = interpret_table_block(self, image)
         return text
 
     def to_dict(self) -> dict:
         """Converts the class instance to dictionary form."""
         out_dict = {
             "coordinates": self.coordinates,
             "text": self.text,
@@ -59,15 +55,15 @@
         """Create LayoutElement from layoutparser TextBlock object."""
         x1, y1, x2, y2 = textblock.coordinates
         text = textblock.text
         type = textblock.type
         return cls(x1, y1, x2, y2, text, type)
 
 
-def interprete_table_block(text_block: TextRegion, image: Image.Image) -> str:
+def interpret_table_block(text_block: TextRegion, image: Image.Image) -> str:
     """Extract the contents of a table."""
     tables.load_agent()
     if tables.tables_agent is None:
         raise RuntimeError("Unable to load table extraction agent.")
     padded_block = text_block.pad(12)
     cropped_image = image.crop((padded_block.x1, padded_block.y1, padded_block.x2, padded_block.y2))
     return tables.tables_agent.predict(cropped_image)
```

### Comparing `unstructured_inference-0.4.1/unstructured_inference/models/base.py` & `unstructured_inference-0.4.2/unstructured_inference/models/base.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.1/unstructured_inference/models/detectron2.py` & `unstructured_inference-0.4.2/unstructured_inference/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.1/unstructured_inference/models/donut.py` & `unstructured_inference-0.4.2/unstructured_inference/models/donut.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.1/unstructured_inference/models/table_postprocess.py` & `unstructured_inference-0.4.2/unstructured_inference/models/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.1/unstructured_inference/models/tables.py` & `unstructured_inference-0.4.2/unstructured_inference/models/tables.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.1/unstructured_inference/models/tesseract.py` & `unstructured_inference-0.4.2/unstructured_inference/models/tesseract.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.1/unstructured_inference/models/unstructuredmodel.py` & `unstructured_inference-0.4.2/unstructured_inference/models/unstructuredmodel.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.1/unstructured_inference/models/yolox.py` & `unstructured_inference-0.4.2/unstructured_inference/models/yolox.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.1/unstructured_inference/utils.py` & `unstructured_inference-0.4.2/unstructured_inference/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.1/unstructured_inference/visualize.py` & `unstructured_inference-0.4.2/unstructured_inference/visualize.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.1/unstructured_inference.egg-info/PKG-INFO` & `unstructured_inference-0.4.2/unstructured_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured-inference
-Version: 0.4.1
+Version: 0.4.2
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.4.1/unstructured_inference.egg-info/SOURCES.txt` & `unstructured_inference-0.4.2/unstructured_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

