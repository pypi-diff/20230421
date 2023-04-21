# Comparing `tmp/RGBMatrixEmulator-0.8.3.tar.gz` & `tmp/RGBMatrixEmulator-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RGBMatrixEmulator-0.8.3.tar", last modified: Sun Mar 12 20:17:40 2023, max compression
+gzip compressed data, was "dist\RGBMatrixEmulator-0.8.4.tar", last modified: Fri Apr 21 20:53:25 2023, max compression
```

## Comparing `RGBMatrixEmulator-0.8.3.tar` & `RGBMatrixEmulator-0.8.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 20:17:40.009083 RGBMatrixEmulator-0.8.3/
--rw-rw-rw-   0        0        0     1076 2021-04-21 03:23:52.000000 RGBMatrixEmulator-0.8.3/LICENSE
--rw-rw-rw-   0        0        0      370 2022-05-05 17:49:25.000000 RGBMatrixEmulator-0.8.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1733 2023-03-12 20:17:40.008085 RGBMatrixEmulator-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     7066 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-12 20:17:39.948081 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/
--rw-rw-rw-   0        0        0      219 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-12 20:17:39.983085 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/
--rw-rw-rw-   0        0        0     1804 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/__init__.py
--rw-rw-rw-   0        0        0     2491 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/base.py
-drwxrwxrwx   0        0        0        0 2023-03-12 20:17:39.989080 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/
--rw-rw-rw-   0        0        0        0 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/__init__.py
--rw-rw-rw-   0        0        0     2063 2023-03-12 20:15:05.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/adapter.py
--rw-rw-rw-   0        0        0     2774 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/server.py
-drwxrwxrwx   0        0        0        0 2023-03-12 20:17:39.991082 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/static/
-drwxrwxrwx   0        0        0        0 2023-03-12 20:17:39.995081 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/static/assets/
--rw-rw-rw-   0        0        0     3812 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/static/assets/client.js
--rw-rw-rw-   0        0        0     3426 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/static/assets/icon.ico
--rw-rw-rw-   0        0        0      311 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/static/assets/styles.css
--rw-rw-rw-   0        0        0     5068 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/static/index.html
--rw-rw-rw-   0        0        0      889 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/web_socket.py
--rw-rw-rw-   0        0        0     2547 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/pygame_adapter.py
--rw-rw-rw-   0        0        0     1387 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/terminal_adapter.py
--rw-rw-rw-   0        0        0     2666 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/tkinter_adapter.py
--rw-rw-rw-   0        0        0     3150 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/turtle_adapter.py
-drwxrwxrwx   0        0        0        0 2023-03-12 20:17:40.000085 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/emulators/
--rw-rw-rw-   0        0        0        0 2021-04-24 19:55:28.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/emulators/__init__.py
--rw-rw-rw-   0        0        0     1806 2022-09-03 18:17:23.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/emulators/canvas.py
--rw-rw-rw-   0        0        0     1449 2022-09-03 18:17:23.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/emulators/matrix.py
--rw-rw-rw-   0        0        0     7081 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/emulators/options.py
-drwxrwxrwx   0        0        0        0 2023-03-12 20:17:40.006082 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/graphics/
--rw-rw-rw-   0        0        0     4056 2022-09-05 03:56:29.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/graphics/__init__.py
--rw-rw-rw-   0        0        0      881 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/graphics/color.py
--rw-rw-rw-   0        0        0     1085 2022-05-05 19:55:29.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/graphics/font.py
--rw-rw-rw-   0        0        0     3426 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/icon.ico
--rw-rw-rw-   0        0        0     8514 2022-06-08 18:26:14.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/icon.png
--rw-rw-rw-   0        0        0      781 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/logger.py
--rw-rw-rw-   0        0        0      114 2023-03-12 20:17:17.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/version.py
-drwxrwxrwx   0        0        0        0 2023-03-12 20:17:39.972080 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator.egg-info/
--rw-rw-rw-   0        0        0     1733 2023-03-12 20:17:39.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1401 2023-03-12 20:17:39.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-12 20:17:39.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-03-12 20:17:39.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-03-12 20:17:39.000000 RGBMatrixEmulator-0.8.3/RGBMatrixEmulator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      760 2022-02-05 15:41:33.000000 RGBMatrixEmulator-0.8.3/description.md
--rw-rw-rw-   0        0        0       42 2023-03-12 20:17:40.009083 RGBMatrixEmulator-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0     2117 2022-09-05 03:56:29.000000 RGBMatrixEmulator-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.694353 RGBMatrixEmulator-0.8.4/
+-rw-rw-rw-   0        0        0     1076 2021-04-21 03:23:52.000000 RGBMatrixEmulator-0.8.4/LICENSE
+-rw-rw-rw-   0        0        0      370 2022-05-05 17:49:25.000000 RGBMatrixEmulator-0.8.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1733 2023-04-21 20:53:25.693352 RGBMatrixEmulator-0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7066 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.534359 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/
+-rw-rw-rw-   0        0        0      219 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.620351 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/
+-rw-rw-rw-   0        0        0     1804 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/__init__.py
+-rw-rw-rw-   0        0        0     2491 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/base.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.642352 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/
+-rw-rw-rw-   0        0        0        0 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/__init__.py
+-rw-rw-rw-   0        0        0     2063 2023-04-21 13:59:36.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/adapter.py
+-rw-rw-rw-   0        0        0     2774 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/server.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.644352 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/
+drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.656351 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/assets/
+-rw-rw-rw-   0        0        0     3812 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/assets/client.js
+-rw-rw-rw-   0        0        0     3426 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/assets/icon.ico
+-rw-rw-rw-   0        0        0      311 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/assets/styles.css
+-rw-rw-rw-   0        0        0     5068 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/index.html
+-rw-rw-rw-   0        0        0      889 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/web_socket.py
+-rw-rw-rw-   0        0        0     2547 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/pygame_adapter.py
+-rw-rw-rw-   0        0        0     1387 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/terminal_adapter.py
+-rw-rw-rw-   0        0        0     2666 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/tkinter_adapter.py
+-rw-rw-rw-   0        0        0     3150 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/turtle_adapter.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.681352 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/
+-rw-rw-rw-   0        0        0        0 2021-04-24 19:55:28.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/__init__.py
+-rw-rw-rw-   0        0        0     1806 2022-09-03 18:17:23.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/canvas.py
+-rw-rw-rw-   0        0        0     1449 2022-09-03 18:17:23.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/matrix.py
+-rw-rw-rw-   0        0        0     7081 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/options.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.692355 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/graphics/
+-rw-rw-rw-   0        0        0     4460 2023-04-21 13:59:14.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/graphics/__init__.py
+-rw-rw-rw-   0        0        0      881 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/graphics/color.py
+-rw-rw-rw-   0        0        0     1085 2022-05-05 19:55:29.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/graphics/font.py
+-rw-rw-rw-   0        0        0     3426 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/icon.ico
+-rw-rw-rw-   0        0        0     8514 2022-06-08 18:26:14.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/icon.png
+-rw-rw-rw-   0        0        0      781 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/logger.py
+-rw-rw-rw-   0        0        0      114 2023-04-21 13:59:58.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/version.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:53:25.569355 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/
+-rw-rw-rw-   0        0        0     1733 2023-04-21 20:53:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1401 2023-04-21 20:53:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 20:53:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-21 20:53:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-21 20:53:25.000000 RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      760 2022-02-05 15:41:33.000000 RGBMatrixEmulator-0.8.4/description.md
+-rw-rw-rw-   0        0        0       42 2023-04-21 20:53:25.694353 RGBMatrixEmulator-0.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     2117 2022-09-05 03:56:29.000000 RGBMatrixEmulator-0.8.4/setup.py
```

### Comparing `RGBMatrixEmulator-0.8.3/LICENSE` & `RGBMatrixEmulator-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/PKG-INFO` & `RGBMatrixEmulator-0.8.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RGBMatrixEmulator
-Version: 0.8.3
+Version: 0.8.4
 Summary: A PC emulator for Raspberry Pi LED matrices driven by rpi-rgb-led-matrix
 Home-page: https://github.com/ty-porter/RGBMatrixEmulator
 Author: Tyler Porter
 Author-email: tyler.b.porter@gmail.com
 License: MIT
 Description: # `RGBMatrixEmulator`
```

### Comparing `RGBMatrixEmulator-0.8.3/README.md` & `RGBMatrixEmulator-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/__init__.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/base.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/base.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/adapter.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/server.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/server.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/static/assets/client.js` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/assets/client.js`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/static/assets/icon.ico` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/static/index.html` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/static/index.html`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/browser_adapter/web_socket.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/browser_adapter/web_socket.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/pygame_adapter.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/pygame_adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/terminal_adapter.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/terminal_adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/tkinter_adapter.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/tkinter_adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/adapters/turtle_adapter.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/adapters/turtle_adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/emulators/canvas.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/canvas.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/emulators/matrix.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/matrix.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/emulators/options.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/emulators/options.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/graphics/__init__.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/graphics/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def DrawText(canvas, font, x, y, color, text):
     # Early return for empty string prevents bugs in bdfparser library
     # and makes good sense anyway
     if len(text) == 0:
         return
 
     # Support multiple spacings based on device width
-    character_widths = [font.CharacterWidth(ord(letter)) for letter in text]
+    character_widths = [__actual_width(font, letter) for letter in text]
     first_char_width = character_widths[0]
     max_char_width = max(character_widths)
     total_width = sum(character_widths)
 
     # Offscreen to the left, adjust by first character width
     if x < 0:
         adjustment = abs(x + first_char_width) // first_char_width
@@ -56,14 +56,26 @@
 def DrawCircle(canvas, x, y, r, color):
     int_points = __coerce_int(x, y)
     rows, cols = __circle_perimeter(*int_points, r)
 
     for point in zip(rows, cols):
         canvas.SetPixel(*point, color.red, color.green, color.blue)
 
+def __actual_width(font, letter):
+    '''
+    Returns the actual width of the letter in the font. If the font doesn't contain a glyph for this letter, it falls back to
+    the width of the default character (?) to prevent division by 0.
+    '''
+    width = font.CharacterWidth(ord(letter))
+    
+    if width > 0:
+        return width
+
+    return font.CharacterWidth(font.default_character.cp())
+
 def __coerce_int(*values):
     return [int(value) for value in values]
 
 def __line(x1, y1, x2, y2):
     '''
     Line drawing algorithm
```

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/graphics/color.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/graphics/color.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/graphics/font.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/graphics/font.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/icon.ico` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/icon.ico`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/icon.png` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/icon.png`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator/logger.py` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator/logger.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator.egg-info/PKG-INFO` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RGBMatrixEmulator
-Version: 0.8.3
+Version: 0.8.4
 Summary: A PC emulator for Raspberry Pi LED matrices driven by rpi-rgb-led-matrix
 Home-page: https://github.com/ty-porter/RGBMatrixEmulator
 Author: Tyler Porter
 Author-email: tyler.b.porter@gmail.com
 License: MIT
 Description: # `RGBMatrixEmulator`
```

### Comparing `RGBMatrixEmulator-0.8.3/RGBMatrixEmulator.egg-info/SOURCES.txt` & `RGBMatrixEmulator-0.8.4/RGBMatrixEmulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/description.md` & `RGBMatrixEmulator-0.8.4/description.md`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.8.3/setup.py` & `RGBMatrixEmulator-0.8.4/setup.py`

 * *Files identical despite different names*

