# Comparing `tmp/tts_arranger-0.1.6.tar.gz` & `tmp/tts_arranger-0.1.7.tar.gz`

## Comparing `tts_arranger-0.1.6.tar` & `tts_arranger-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/requirements.txt
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0    24724 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/tts_processor.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/tts_processor_example.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/tts_simple_writer.py
--rw-r--r--   0        0        0    15834 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/tts_writer.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/data/replace.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/data/replace_de.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/data/replace_en.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/items/__init__.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/items/tts_chapter.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/items/tts_item.py
--rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/items/tts_project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/utils/audio.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0    20461 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/LICENSE
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/README.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tts_arranger-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/requirements.txt
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0    24724 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/tts_processor_example.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/tts_simple_writer.py
+-rw-r--r--   0        0        0    16085 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/data/replace.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/data/replace_de.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/data/replace_en.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/utils/audio.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0    20460 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tts_arranger-0.1.7/PKG-INFO
```

### Comparing `tts_arranger-0.1.6/src/tts_arranger/tts_processor.py` & `tts_arranger-0.1.7/src/tts_arranger/tts_processor.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.6/src/tts_arranger/tts_processor_example.py` & `tts_arranger-0.1.7/src/tts_arranger/tts_processor_example.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.6/src/tts_arranger/tts_simple_writer.py` & `tts_arranger-0.1.7/src/tts_arranger/tts_simple_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.6/src/tts_arranger/tts_writer.py` & `tts_arranger-0.1.7/src/tts_arranger/tts_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,16 @@
         :return: None
         :rtype: None
         """
 
         log(LOG_TYPE.INFO, f'Preprocessing items.')
 
         for chapter in chapters:
-            chapter.tts_items = tts_processor.preprocess_items(chapter.tts_items)
             chapter.optimize(max_pause_duration)
+            chapter.tts_items = tts_processor.preprocess_items(chapter.tts_items)
 
         tts_processor.initialize()
 
         total_items = 0
 
         for chapter in chapters:
             total_items += len(chapter.tts_items)
@@ -198,14 +198,19 @@
             audio = ffmpeg.input(input_file)['a']
 
             # Save the project as a temporary image
             image_format = 'jpeg'
 
             image_path = os.path.join(temp_dir, f'tts_image.{image_format}')
 
+            if image.format == 'PNG' and image.mode != 'RGBA':
+                image = image.convert('RGBA')
+                background = Image.new('RGBA', image.size, (255, 255, 255))
+                image = Image.alpha_composite(background, image)
+
             # Convert to RGB if necessary
             if image.mode != 'RGB':
                 image = image.convert('RGB')
 
             # Fix for ffmpeg problem when image size is not divisible by 2
             image.crop((0, 0, math.ceil(image_width/2)*2, math.ceil(image_height/2)*2)).save(image_path, format=image_format, quality=90)
```

### Comparing `tts_arranger-0.1.6/src/tts_arranger/items/tts_chapter.py` & `tts_arranger-0.1.7/src/tts_arranger/items/tts_chapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,8 +68,16 @@
 
         # Limit pause duration for pause items, ignore if max_pause_duration == 0
         for final_item in final_items:
             if final_item.speaker_idx == -1 and max_pause_duration > 0:
                 if final_item.length > max_pause_duration:
                     final_item.length = max_pause_duration
 
-        self.tts_items = final_items
+        non_empty_items: list[TTS_Item] = []
+
+        # Remove remaining empty items
+        for final_item in final_items:
+            if final_item.text.strip() or final_item.speaker_idx == -1:
+                final_item.text = final_item.text.strip()
+                non_empty_items.append(final_item)
+
+        self.tts_items = non_empty_items
```

### Comparing `tts_arranger-0.1.6/src/tts_arranger/items/tts_item.py` & `tts_arranger-0.1.7/src/tts_arranger/items/tts_item.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.6/src/tts_arranger/items/tts_project.py` & `tts_arranger-0.1.7/src/tts_arranger/items/tts_project.py`

 * *Files 20% similar despite different names*

```diff
@@ -123,60 +123,24 @@
         """
         try:
             with open(filename, 'wb') as file:
                 pickle.dump(self, file)
         except IOError:
             log(LOG_TYPE.WARNING, f'TTS Project export file "{filename}" could not be opened for writing.')
 
-    def _add_image(self, image: Image.Image) -> None:
-        """
-        Prepares the specified image and adds it to the project.
-
-        :param image: The image to be added.
-        :type image: Image.Image
-
-        :return: None
-        """
-        format = image.format
-
-        if image.format == 'PNG' and image.mode != 'RGBA':
-            image = image.convert('RGBA')
-            background = Image.new('RGBA', image.size, (255, 255, 255))
-            image = Image.alpha_composite(background, image)
-
-        if image.mode != 'RGB':
-            image = image.convert('RGB')
-
-        image_file = BytesIO()
-        image.save(image_file, format=format)
-        self.image_bytes = base64.b64encode(image_file.getvalue())
-
-    def add_image(self, image_file: str) -> None:
-        """
-        Opens the image from the given path and adds it via the private function.
-
-        :param image_file: The file path of the image to be added.
-        :type image_file: str
-
-        :return: None
-        """
-        image = Image.open(image_file)
-        self._add_image(image)
-
     def add_image_from_url(self, image_url: str) -> None:
         """
         Opens the image from the given URL and adds it via the private function.
 
         :param image_url: The URL of the image to be added.
         :type image_url: str
 
         :return: None
         """
         if image_url:
-            # self._add_image(image)
             self.image_bytes = base64.b64encode(requests.get(image_url).content)
 
     def clean_empty_chapters(self):
         final_chapters: list[TTS_Chapter] = []
 
         for chapter in self.tts_chapters:
             if len(chapter.tts_items) > 0:
```

### Comparing `tts_arranger-0.1.6/src/tts_arranger/utils/audio.py` & `tts_arranger-0.1.7/src/tts_arranger/utils/audio.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.6/src/tts_arranger/utils/log.py` & `tts_arranger-0.1.7/src/tts_arranger/utils/log.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.6/tests/tts_arranger_test.py` & `tts_arranger-0.1.7/tests/tts_arranger_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
         items.append(TTS_Item(length=1000))
         items.append(TTS_Item('2'))
         items.append(TTS_Item(length=1000))
         items.append(TTS_Item(' 3'))
 
         project = TTS_Project()
         project.tts_chapters.append(TTS_Chapter(items))
-        project.optimize()
+        # project.optimize()
         items = project.tts_chapters[0].tts_items
 
         self.assertEqual(items[0].text, '1 ')
         self.assertEqual(items[1].length, 1000)
         self.assertEqual(items[2].text, '2')
         self.assertEqual(items[3].length, 1000)
         self.assertEqual(items[4].text, ' 3')
@@ -392,23 +392,23 @@
         project = TTS_Project()
         project.tts_chapters.append(TTS_Chapter(items))
         project.optimize(max_pause_duration=100)
         items = project.tts_chapters[0].tts_items
 
         self.assertEqual(items[0].text, '1 2')
         self.assertEqual(items[1].length, 100)
-        self.assertEqual(items[2].text, ' 3')
+        self.assertEqual(items[2].text, '3')
         self.assertEqual(items[3].length, 100)
 
     def test_merge_items4(self):
         item = TTS_Item('1 (1234), test')
         t = TTS_Processor()
         tts_items = t._prepare_item(item)
         
         project = TTS_Project()
         project.tts_chapters.append(TTS_Chapter(tts_items))
         project.optimize(max_pause_duration=100)
         items = project.tts_chapters[0].tts_items
 
-        self.assertEqual(items[0].text, '1 ')
+        self.assertEqual(items[0].text, '1')
         self.assertEqual(items[2].text, '1234,')
-        self.assertEqual(items[4].text, ' test')
+        self.assertEqual(items[4].text, 'test')
```

### Comparing `tts_arranger-0.1.6/LICENSE` & `tts_arranger-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.6/README.md` & `tts_arranger-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.6/pyproject.toml` & `tts_arranger-0.1.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   "Operating System :: OS Independent",
 ]
 description = "Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS"
 dynamic = ["dependencies"]
 name = "tts_arranger"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.1.6"
+version = "0.1.7"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/knochenhans/tts_arranger/issues"
 "Homepage" = "https://github.com/knochenhans/tts_arranger"
 
 [tool.hatch.build]
 exclude = [
```

### Comparing `tts_arranger-0.1.6/PKG-INFO` & `tts_arranger-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

