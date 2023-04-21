# Comparing `tmp/grbl2image-1.1.0.tar.gz` & `tmp/grbl2image-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grbl2image-1.1.0.tar", last modified: Fri Apr 21 13:10:32 2023, max compression
+gzip compressed data, was "grbl2image-1.1.1.tar", last modified: Fri Apr 21 13:13:43 2023, max compression
```

## Comparing `grbl2image-1.1.0.tar` & `grbl2image-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:10:32.785449 grbl2image-1.1.0/
--rw-rw-r--   0 alan      (1000) alan      (1000)     1070 2023-04-17 08:15:45.000000 grbl2image-1.1.0/LICENSE
--rw-rw-r--   0 alan      (1000) alan      (1000)     4479 2023-04-21 13:10:32.785449 grbl2image-1.1.0/PKG-INFO
--rw-rw-r--   0 alan      (1000) alan      (1000)     3836 2023-04-21 13:10:10.000000 grbl2image-1.1.0/README.md
--rw-rw-r--   0 alan      (1000) alan      (1000)      742 2023-04-21 13:07:34.000000 grbl2image-1.1.0/pyproject.toml
--rw-rw-r--   0 alan      (1000) alan      (1000)       38 2023-04-21 13:10:32.785449 grbl2image-1.1.0/setup.cfg
-drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:10:32.781449 grbl2image-1.1.0/src/
-drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:10:32.785449 grbl2image-1.1.0/src/grbl2image/
--rw-rw-r--   0 alan      (1000) alan      (1000)        0 2023-04-21 05:24:54.000000 grbl2image-1.1.0/src/grbl2image/__init__.py
--rw-rw-r--   0 alan      (1000) alan      (1000)     6336 2023-04-21 13:05:52.000000 grbl2image-1.1.0/src/grbl2image/grbl2image.py
-drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:10:32.785449 grbl2image-1.1.0/src/grbl2image.egg-info/
--rw-rw-r--   0 alan      (1000) alan      (1000)     4479 2023-04-21 13:10:32.000000 grbl2image-1.1.0/src/grbl2image.egg-info/PKG-INFO
--rw-rw-r--   0 alan      (1000) alan      (1000)      331 2023-04-21 13:10:32.000000 grbl2image-1.1.0/src/grbl2image.egg-info/SOURCES.txt
--rw-rw-r--   0 alan      (1000) alan      (1000)        1 2023-04-21 13:10:32.000000 grbl2image-1.1.0/src/grbl2image.egg-info/dependency_links.txt
--rw-rw-r--   0 alan      (1000) alan      (1000)       12 2023-04-21 13:10:32.000000 grbl2image-1.1.0/src/grbl2image.egg-info/requires.txt
--rw-rw-r--   0 alan      (1000) alan      (1000)       11 2023-04-21 13:10:32.000000 grbl2image-1.1.0/src/grbl2image.egg-info/top_level.txt
-drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:10:32.785449 grbl2image-1.1.0/tests/
--rw-rw-r--   0 alan      (1000) alan      (1000)      774 2023-04-21 12:54:56.000000 grbl2image-1.1.0/tests/tests.py
--rw-rw-r--   0 alan      (1000) alan      (1000)      758 2023-04-21 13:04:07.000000 grbl2image-1.1.0/tests/tests_all.py
--rw-rw-r--   0 alan      (1000) alan      (1000)      679 2023-04-21 13:06:56.000000 grbl2image-1.1.0/tests/tests_size.py
+drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:13:43.870754 grbl2image-1.1.1/
+-rw-rw-r--   0 alan      (1000) alan      (1000)     1070 2023-04-17 08:15:45.000000 grbl2image-1.1.1/LICENSE
+-rw-rw-r--   0 alan      (1000) alan      (1000)     4523 2023-04-21 13:13:43.870754 grbl2image-1.1.1/PKG-INFO
+-rw-rw-r--   0 alan      (1000) alan      (1000)     3880 2023-04-21 13:12:19.000000 grbl2image-1.1.1/README.md
+-rw-rw-r--   0 alan      (1000) alan      (1000)      742 2023-04-21 13:13:06.000000 grbl2image-1.1.1/pyproject.toml
+-rw-rw-r--   0 alan      (1000) alan      (1000)       38 2023-04-21 13:13:43.870754 grbl2image-1.1.1/setup.cfg
+drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:13:43.866754 grbl2image-1.1.1/src/
+drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:13:43.866754 grbl2image-1.1.1/src/grbl2image/
+-rw-rw-r--   0 alan      (1000) alan      (1000)        0 2023-04-21 05:24:54.000000 grbl2image-1.1.1/src/grbl2image/__init__.py
+-rw-rw-r--   0 alan      (1000) alan      (1000)     6336 2023-04-21 13:05:52.000000 grbl2image-1.1.1/src/grbl2image/grbl2image.py
+drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:13:43.870754 grbl2image-1.1.1/src/grbl2image.egg-info/
+-rw-rw-r--   0 alan      (1000) alan      (1000)     4523 2023-04-21 13:13:43.000000 grbl2image-1.1.1/src/grbl2image.egg-info/PKG-INFO
+-rw-rw-r--   0 alan      (1000) alan      (1000)      331 2023-04-21 13:13:43.000000 grbl2image-1.1.1/src/grbl2image.egg-info/SOURCES.txt
+-rw-rw-r--   0 alan      (1000) alan      (1000)        1 2023-04-21 13:13:43.000000 grbl2image-1.1.1/src/grbl2image.egg-info/dependency_links.txt
+-rw-rw-r--   0 alan      (1000) alan      (1000)       12 2023-04-21 13:13:43.000000 grbl2image-1.1.1/src/grbl2image.egg-info/requires.txt
+-rw-rw-r--   0 alan      (1000) alan      (1000)       11 2023-04-21 13:13:43.000000 grbl2image-1.1.1/src/grbl2image.egg-info/top_level.txt
+drwxrwxr-x   0 alan      (1000) alan      (1000)        0 2023-04-21 13:13:43.870754 grbl2image-1.1.1/tests/
+-rw-rw-r--   0 alan      (1000) alan      (1000)      774 2023-04-21 12:54:56.000000 grbl2image-1.1.1/tests/tests.py
+-rw-rw-r--   0 alan      (1000) alan      (1000)      758 2023-04-21 13:04:07.000000 grbl2image-1.1.1/tests/tests_all.py
+-rw-rw-r--   0 alan      (1000) alan      (1000)      679 2023-04-21 13:06:56.000000 grbl2image-1.1.1/tests/tests_size.py
```

### Comparing `grbl2image-1.1.0/LICENSE` & `grbl2image-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grbl2image-1.1.0/PKG-INFO` & `grbl2image-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grbl2image
-Version: 1.1.0
+Version: 1.1.1
 Summary: Generates an image (PNG, JPEG, etc.) from a GRBL file (.NC, .GC, ...) in Python using pillow (python3)
 Author: AlanFromJapan
 Project-URL: Homepage, https://github.com/AlanFromJapan/grbl2image
 Project-URL: Bug Tracker, https://github.com/AlanFromJapan/grbl2image/issues
 Project-URL: Parent project, https://github.com/AlanFromJapan/GrblWebStreamer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -56,17 +56,20 @@
 ## Sample usage
 ### Generate an image from GRBL file
 ```python
 import grbl2image.grbl2image as G2I
 from PIL import Image
 
 #Generate the PIL Image object based on sample code
-img = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue")
+img, stats = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue")
+print(stats)
+
 #overlay another job in the same image
-img = G2I.processFile("sample.gcode/Test gcode 2.nc", targetImage=img, color="red", yoffset=300)
+img, stats = G2I.processFile("sample.gcode/Test gcode 2.nc", targetImage=img, color="red", yoffset=300)
+print(stats)
 
 #final flip because the image 0,0 is top left and for us human it's at the bottom left
 img = img.transpose(Image.FLIP_TOP_BOTTOM)
 
 #show popup
 img.show()
 ```
@@ -78,15 +81,15 @@
 
 #suppose your laser is a 40cm x 30xm for instance you could use these settings **before** calling processFile()
 G2I.PIXELS_PER_MM = 5
 G2I.AREA_W_MM = 300
 G2I.AREA_H_MM = 400
 
 #Generate the PIL Image object based on sample code
-img = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue")
+img, _ = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue")
 
 #final flip because the image 0,0 is top left and for us human it's at the bottom left
 img = img.transpose(Image.FLIP_TOP_BOTTOM)
 
 #save
 img.save("laser_job_001.png")
 ```
```

### Comparing `grbl2image-1.1.0/README.md` & `grbl2image-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -41,17 +41,20 @@
 ## Sample usage
 ### Generate an image from GRBL file
 ```python
 import grbl2image.grbl2image as G2I
 from PIL import Image
 
 #Generate the PIL Image object based on sample code
-img = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue")
+img, stats = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue")
+print(stats)
+
 #overlay another job in the same image
-img = G2I.processFile("sample.gcode/Test gcode 2.nc", targetImage=img, color="red", yoffset=300)
+img, stats = G2I.processFile("sample.gcode/Test gcode 2.nc", targetImage=img, color="red", yoffset=300)
+print(stats)
 
 #final flip because the image 0,0 is top left and for us human it's at the bottom left
 img = img.transpose(Image.FLIP_TOP_BOTTOM)
 
 #show popup
 img.show()
 ```
@@ -63,15 +66,15 @@
 
 #suppose your laser is a 40cm x 30xm for instance you could use these settings **before** calling processFile()
 G2I.PIXELS_PER_MM = 5
 G2I.AREA_W_MM = 300
 G2I.AREA_H_MM = 400
 
 #Generate the PIL Image object based on sample code
-img = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue")
+img, _ = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue")
 
 #final flip because the image 0,0 is top left and for us human it's at the bottom left
 img = img.transpose(Image.FLIP_TOP_BOTTOM)
 
 #save
 img.save("laser_job_001.png")
 ```
```

### Comparing `grbl2image-1.1.0/pyproject.toml` & `grbl2image-1.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "grbl2image"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="AlanFromJapan" },
 ]
 description = "Generates an image (PNG, JPEG, etc.) from a GRBL file (.NC, .GC, ...) in Python using pillow (python3)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `grbl2image-1.1.0/src/grbl2image/grbl2image.py` & `grbl2image-1.1.1/src/grbl2image/grbl2image.py`

 * *Files identical despite different names*

### Comparing `grbl2image-1.1.0/src/grbl2image.egg-info/PKG-INFO` & `grbl2image-1.1.1/src/grbl2image.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grbl2image
-Version: 1.1.0
+Version: 1.1.1
 Summary: Generates an image (PNG, JPEG, etc.) from a GRBL file (.NC, .GC, ...) in Python using pillow (python3)
 Author: AlanFromJapan
 Project-URL: Homepage, https://github.com/AlanFromJapan/grbl2image
 Project-URL: Bug Tracker, https://github.com/AlanFromJapan/grbl2image/issues
 Project-URL: Parent project, https://github.com/AlanFromJapan/GrblWebStreamer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -56,17 +56,20 @@
 ## Sample usage
 ### Generate an image from GRBL file
 ```python
 import grbl2image.grbl2image as G2I
 from PIL import Image
 
 #Generate the PIL Image object based on sample code
-img = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue")
+img, stats = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue")
+print(stats)
+
 #overlay another job in the same image
-img = G2I.processFile("sample.gcode/Test gcode 2.nc", targetImage=img, color="red", yoffset=300)
+img, stats = G2I.processFile("sample.gcode/Test gcode 2.nc", targetImage=img, color="red", yoffset=300)
+print(stats)
 
 #final flip because the image 0,0 is top left and for us human it's at the bottom left
 img = img.transpose(Image.FLIP_TOP_BOTTOM)
 
 #show popup
 img.show()
 ```
@@ -78,15 +81,15 @@
 
 #suppose your laser is a 40cm x 30xm for instance you could use these settings **before** calling processFile()
 G2I.PIXELS_PER_MM = 5
 G2I.AREA_W_MM = 300
 G2I.AREA_H_MM = 400
 
 #Generate the PIL Image object based on sample code
-img = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue")
+img, _ = G2I.processFile("sample.gcode/Test gcode 1.nc", color="blue")
 
 #final flip because the image 0,0 is top left and for us human it's at the bottom left
 img = img.transpose(Image.FLIP_TOP_BOTTOM)
 
 #save
 img.save("laser_job_001.png")
 ```
```

### Comparing `grbl2image-1.1.0/tests/tests.py` & `grbl2image-1.1.1/tests/tests.py`

 * *Files identical despite different names*

### Comparing `grbl2image-1.1.0/tests/tests_all.py` & `grbl2image-1.1.1/tests/tests_all.py`

 * *Files identical despite different names*

### Comparing `grbl2image-1.1.0/tests/tests_size.py` & `grbl2image-1.1.1/tests/tests_size.py`

 * *Files identical despite different names*

