# Comparing `tmp/ifunnygifmaker-0.1.7.tar.gz` & `tmp/ifunnygifmaker-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifunnygifmaker-0.1.7.tar", last modified: Fri Apr 21 04:29:42 2023, max compression
+gzip compressed data, was "ifunnygifmaker-0.1.8.tar", last modified: Fri Apr 21 04:36:52 2023, max compression
```

## Comparing `ifunnygifmaker-0.1.7.tar` & `ifunnygifmaker-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       12 2023-04-17 15:21:16.673815 ifunnygifmaker-0.1.7/README.md
--rw-r--r--   0        0        0     6148 2023-04-21 04:24:08.705576 ifunnygifmaker-0.1.7/ifunnygifmaker/.DS_Store
--rw-r--r--   0        0        0       39 2023-04-20 03:35:46.032714 ifunnygifmaker-0.1.7/ifunnygifmaker/__init__.py
--rw-r--r--   0        0        0    25492 2020-05-28 04:55:50.000000 ifunnygifmaker-0.1.7/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf
--rw-r--r--   0        0        0     4492 2023-04-21 04:24:24.239227 ifunnygifmaker-0.1.7/ifunnygifmaker/mememaker.py
--rw-r--r--   0        0        0      459 2023-04-21 04:29:38.548001 ifunnygifmaker-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 ifunnygifmaker-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-04-17 15:21:16.673815 ifunnygifmaker-0.1.8/README.md
+-rw-r--r--   0        0        0     6148 2023-04-21 04:24:08.705576 ifunnygifmaker-0.1.8/ifunnygifmaker/.DS_Store
+-rw-r--r--   0        0        0       39 2023-04-20 03:35:46.032714 ifunnygifmaker-0.1.8/ifunnygifmaker/__init__.py
+-rw-r--r--   0        0        0    25492 2020-05-28 04:55:50.000000 ifunnygifmaker-0.1.8/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf
+-rw-r--r--   0        0        0     4537 2023-04-21 04:36:28.948060 ifunnygifmaker-0.1.8/ifunnygifmaker/mememaker.py
+-rw-r--r--   0        0        0      459 2023-04-21 04:36:38.105602 ifunnygifmaker-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 ifunnygifmaker-0.1.8/PKG-INFO
```

### Comparing `ifunnygifmaker-0.1.7/ifunnygifmaker/.DS_Store` & `ifunnygifmaker-0.1.8/ifunnygifmaker/.DS_Store`

 * *Files identical despite different names*

### Comparing `ifunnygifmaker-0.1.7/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf` & `ifunnygifmaker-0.1.8/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf`

 * *Files identical despite different names*

### Comparing `ifunnygifmaker-0.1.7/ifunnygifmaker/mememaker.py` & `ifunnygifmaker-0.1.8/ifunnygifmaker/mememaker.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,26 +63,26 @@
                 # Paste the original GIF image onto the new image
                 new_im.paste(im, (0, 100))
 
                 # Create a drawing object
                 draw = ImageDraw.Draw(new_im)
 
                 # Define the font for the text
-                font = ImageFont.truetype("fonts/Futura Condensed Extra Bold.otf", 15)
+                font = ImageFont.truetype("ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf", 15)
                 
                 # Get the size of the text
                 text_size = draw.textsize(text, font=font)
 
                 # Calculate the position for the text
                 text_y = ((padding_size - 50) - text_size[1]) // 2
                 wrap = new_im.width * 0.1
-                size = self.__calculate_fontsize(text=text, rect_len=padding_size, rect_width=new_im.width, wrap=wrap, font_name="fonts/Futura Condensed Extra Bold.otf") 
+                size = self.__calculate_fontsize(text=text, rect_len=padding_size, rect_width=new_im.width, wrap=wrap, font_name="ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf") 
 
                 # Define the font for the text
-                font = ImageFont.truetype("fonts/Futura Condensed Extra Bold.otf", size)
+                font = ImageFont.truetype("ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf", size)
 
                 # Draw the text on the rectangle
                 text_lines = textwrap.wrap(text, width=wrap)
                 for line in text_lines:
                     line_size = draw.textsize(line, font=font) #draw the text
                     line_x = (new_im.width - line_size[0]) // 2
                     draw.text((line_x, text_y), line, font=font, fill=0)
```

