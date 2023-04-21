# Comparing `tmp/ifunnygifmaker-0.1.4.tar.gz` & `tmp/ifunnygifmaker-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifunnygifmaker-0.1.4.tar", last modified: Fri Apr 21 03:07:47 2023, max compression
+gzip compressed data, was "ifunnygifmaker-0.1.5.tar", last modified: Fri Apr 21 04:17:35 2023, max compression
```

## Comparing `ifunnygifmaker-0.1.4.tar` & `ifunnygifmaker-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       12 2023-04-17 15:21:16.673815 ifunnygifmaker-0.1.4/README.md
--rw-r--r--   0        0        0    25492 2020-05-28 04:55:50.000000 ifunnygifmaker-0.1.4/ifunnygifmaker/Futura Condensed Extra Bold.otf
--rw-r--r--   0        0        0       39 2023-04-20 03:35:46.032714 ifunnygifmaker-0.1.4/ifunnygifmaker/__init__.py
--rw-r--r--   0        0        0     4515 2023-04-21 03:07:09.655700 ifunnygifmaker-0.1.4/ifunnygifmaker/mememaker.py
--rw-r--r--   0        0        0      416 2023-04-21 03:07:42.402814 ifunnygifmaker-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 ifunnygifmaker-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-04-17 15:21:16.673815 ifunnygifmaker-0.1.5/README.md
+-rw-r--r--   0        0        0     6148 2023-04-21 04:15:30.948860 ifunnygifmaker-0.1.5/ifunnygifmaker/.DS_Store
+-rw-r--r--   0        0        0       39 2023-04-20 03:35:46.032714 ifunnygifmaker-0.1.5/ifunnygifmaker/__init__.py
+-rw-r--r--   0        0        0     4492 2023-04-21 04:16:43.733682 ifunnygifmaker-0.1.5/ifunnygifmaker/mememaker.py
+-rw-r--r--   0        0        0      416 2023-04-21 04:17:30.587395 ifunnygifmaker-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 ifunnygifmaker-0.1.5/PKG-INFO
```

### Comparing `ifunnygifmaker-0.1.4/ifunnygifmaker/mememaker.py` & `ifunnygifmaker-0.1.5/ifunnygifmaker/mememaker.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,26 +63,26 @@
                 # Paste the original GIF image onto the new image
                 new_im.paste(im, (0, 100))
 
                 # Create a drawing object
                 draw = ImageDraw.Draw(new_im)
 
                 # Define the font for the text
-                font = ImageFont.truetype("ifunnygifmaker/Futura Condensed Extra Bold.otf", 15)
+                font = ImageFont.truetype("fonts/Futura Condensed Extra Bold.otf", 15)
                 
                 # Get the size of the text
                 text_size = draw.textsize(text, font=font)
 
                 # Calculate the position for the text
                 text_y = ((padding_size - 50) - text_size[1]) // 2
                 wrap = new_im.width * 0.1
-                size = self.__calculate_fontsize(text=text, rect_len=padding_size, rect_width=new_im.width, wrap=wrap, font_name="ifunnygifmaker/Futura Condensed Extra Bold.otf") 
+                size = self.__calculate_fontsize(text=text, rect_len=padding_size, rect_width=new_im.width, wrap=wrap, font_name="fonts/Futura Condensed Extra Bold.otf") 
 
                 # Define the font for the text
-                font = ImageFont.truetype("ifunnygifmaker/Futura Condensed Extra Bold.otf", size)
+                font = ImageFont.truetype("fonts/Futura Condensed Extra Bold.otf", size)
 
                 # Draw the text on the rectangle
                 text_lines = textwrap.wrap(text, width=wrap)
                 for line in text_lines:
                     line_size = draw.textsize(line, font=font) #draw the text
                     line_x = (new_im.width - line_size[0]) // 2
                     draw.text((line_x, text_y), line, font=font, fill=0)
@@ -112,9 +112,8 @@
             query = query.replace(" ", "+")
        self.__create_gif(query=query, url=url)
        self.__edit_gif(text) 
        self.__clean_up() 
 
 if __name__ == "__main__":
     m = MemeMaker()
-    m.make_meme(text="")
-
+    m.make_meme(text="funny")
```

