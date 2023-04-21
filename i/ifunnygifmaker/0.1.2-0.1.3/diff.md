# Comparing `tmp/ifunnygifmaker-0.1.2.tar.gz` & `tmp/ifunnygifmaker-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifunnygifmaker-0.1.2.tar", last modified: Thu Apr 20 03:23:47 2023, max compression
+gzip compressed data, was "ifunnygifmaker-0.1.3.tar", last modified: Fri Apr 21 02:54:25 2023, max compression
```

## Comparing `ifunnygifmaker-0.1.2.tar` & `ifunnygifmaker-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       12 2023-04-17 15:21:16.673815 ifunnygifmaker-0.1.2/README.md
--rw-r--r--   0        0        0       39 2023-04-20 03:23:31.127817 ifunnygifmaker-0.1.2/ifunnygifmaker/__init__.py
--rw-r--r--   0        0        0     4584 2023-04-20 03:18:39.381272 ifunnygifmaker-0.1.2/ifunnygifmaker/mememaker.py
--rw-r--r--   0        0        0      416 2023-04-20 03:23:42.932258 ifunnygifmaker-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 ifunnygifmaker-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-04-17 15:21:16.673815 ifunnygifmaker-0.1.3/README.md
+-rw-r--r--   0        0        0    25492 2020-05-28 04:55:50.000000 ifunnygifmaker-0.1.3/ifunnygifmaker/Futura Condensed Extra Bold.otf
+-rw-r--r--   0        0        0       39 2023-04-20 03:35:46.032714 ifunnygifmaker-0.1.3/ifunnygifmaker/__init__.py
+-rw-r--r--   0        0        0     4699 2023-04-21 02:52:06.293630 ifunnygifmaker-0.1.3/ifunnygifmaker/mememaker.py
+-rw-r--r--   0        0        0      416 2023-04-21 02:54:21.139395 ifunnygifmaker-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 ifunnygifmaker-0.1.3/PKG-INFO
```

### Comparing `ifunnygifmaker-0.1.2/ifunnygifmaker/mememaker.py` & `ifunnygifmaker-0.1.3/ifunnygifmaker/mememaker.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,26 +65,26 @@
                 # Paste the original GIF image onto the new image
                 new_im.paste(im, (0, 100))
 
                 # Create a drawing object
                 draw = ImageDraw.Draw(new_im)
 
                 # Define the font for the text
-                font = ImageFont.truetype("Futura Condensed Extra Bold.otf", 15)
+                font = ImageFont.truetype("ifunnygifmaker/Futura Condensed Extra Bold.otf", 15)
                 
                 # Get the size of the text
                 text_size = draw.textsize(text, font=font)
 
                 # Calculate the position for the text
                 text_y = ((padding_size - 50) - text_size[1]) // 2
                 wrap = new_im.width * 0.1
-                size = self.__calculate_fontsize(text=text, rect_len=padding_size, rect_width=new_im.width, wrap=wrap, font_name="Futura Condensed Extra Bold.otf") 
+                size = self.__calculate_fontsize(text=text, rect_len=padding_size, rect_width=new_im.width, wrap=wrap, font_name="ifunnygifmaker/Futura Condensed Extra Bold.otf") 
 
                 # Define the font for the text
-                font = ImageFont.truetype("Futura Condensed Extra Bold.otf", size)
+                font = ImageFont.truetype("ifunnygifmaker/Futura Condensed Extra Bold.otf", size)
 
                 # Draw the text on the rectangle
                 text_lines = textwrap.wrap(text, width=wrap)
                 for line in text_lines:
                     line_size = draw.textsize(line, font=font) #draw the text
                     line_x = (new_im.width - line_size[0]) // 2
                     draw.text((line_x, text_y), line, font=font, fill=0)
@@ -108,15 +108,15 @@
        load_dotenv() 
        if self.query is None:
             self.query = self.text.replace(" ", "+")
        if self.query is not None and self.url is not None:
             self.query = None
        if self.query is not None:
             self.query = self.query.replace(" ", "+")
-       self.__create_gif(self.query)
+       self.__create_gif(query=self.query, url=self.url)
        self.__edit_gif(self.text) 
        self.__clean_up() 
 
 if __name__ == "__main__":
-    m = MemeMaker("example text")
+    m = MemeMaker("when alex gets -10 for not zipping his makefile", query="funny")
     m.make_meme()
```

