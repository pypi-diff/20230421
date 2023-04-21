# Comparing `tmp/pywriter-0.1.0-py3-none-any.whl.zip` & `tmp/pywriter-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3693 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      417 b- defN 23-Apr-20 22:43 pywriter/__init__.py
--rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-21 00:24 pywriter-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3891 b- defN 23-Apr-21 00:24 pywriter-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 00:24 pywriter-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-21 00:24 pywriter-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      466 b- defN 23-Apr-21 00:24 pywriter-0.1.0.dist-info/RECORD
-6 files, 5968 bytes uncompressed, 2847 bytes compressed:  52.3%
+Zip file size: 3697 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      446 b- defN 23-Apr-21 00:36 pywriter/__init__.py
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-21 00:37 pywriter-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3891 b- defN 23-Apr-21 00:37 pywriter-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 00:37 pywriter-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-21 00:37 pywriter-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      466 b- defN 23-Apr-21 00:37 pywriter-0.1.1.dist-info/RECORD
+6 files, 5997 bytes uncompressed, 2851 bytes compressed:  52.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pywriter/__init__.py
 Comment: 
 
-Filename: pywriter-0.1.0.dist-info/LICENSE
+Filename: pywriter-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pywriter-0.1.0.dist-info/METADATA
+Filename: pywriter-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pywriter-0.1.0.dist-info/WHEEL
+Filename: pywriter-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pywriter-0.1.0.dist-info/top_level.txt
+Filename: pywriter-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pywriter-0.1.0.dist-info/RECORD
+Filename: pywriter-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywriter/__init__.py

```diff
@@ -1,15 +1,16 @@
+import sys
 import time
 
-
 def write(text, rate:float | None = 0.1):
     """Function to print output with typewriter effect
     
     >>> For instance:
         write(text="Hello world!", rate=1) 
         
         This will print all the elements of the string "Hello world!" one by one at the rate of 1 element per second
     """
 
-    for i in range(len(text)):
-        print(text[i], end="")
+    for char in text:
+        sys.stdout.write(char)
+        sys.stdout.flush()
         time.sleep(rate)
```

## Comparing `pywriter-0.1.0.dist-info/LICENSE` & `pywriter-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywriter-0.1.0.dist-info/METADATA` & `pywriter-0.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywriter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Typewriter effect for python
 Home-page: https://github.com/amarquaye/pywriter
 Author: Jesse Amarquaye
 Author-email: jesseamarquayelegendary@gmail.com
 Keywords: python,pywriter,type,writer,typewriter,typewritereffect
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -64,15 +64,15 @@
 
 ![ui_glow_up](https://user-images.githubusercontent.com/96346994/233510322-9397b5b3-8626-447a-9453-0e580beae656.gif)
 
 <br/>
 
 ## Changelog
 
-### v0.1.0 (21/04/2023)
+### v0.1.1 (21/04/2023)
 
 ### Feature
 
 - First minor update of `pywriter`
 - Added compatibility with terminal and any console.
 
 ### Fix
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pywriter Version: 0.1.0 Summary: Typewriter effect
+Metadata-Version: 2.1 Name: pywriter Version: 0.1.1 Summary: Typewriter effect
 for python Home-page: https://github.com/amarquaye/pywriter Author: Jesse
 Amarquaye Author-email: jesseamarquayelegendary@gmail.com Keywords:
 python,pywriter,type,writer,typewriter,typewritereffect Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Topic :: Printing Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
@@ -17,15 +17,15 @@
 World!' character by character at the rate of one character per second write
 ('Hello World!', rate=1) # However, it is recommended that you use
 pywriter.write instead of using the write function directly. # Since this will
 help prevent any conflict in case there is another python module which also has
 a write function. ```
 ## Demo ![ui_glow_up](https://user-images.githubusercontent.com/96346994/
 233510322-9397b5b3-8626-447a-9453-0e580beae656.gif)
-## Changelog ### v0.1.0 (21/04/2023) ### Feature - First minor update of
+## Changelog ### v0.1.1 (21/04/2023) ### Feature - First minor update of
 `pywriter` - Added compatibility with terminal and any console. ### Fix - Fixed
 issue with windows cmd waiting for the entire program to run before output in
 seen. ### v0.0.1 (15/04/2023) - First release of `pywriter`
 ## Contributing Pull requests are welcome. For major changes, please open an
 issue first to discuss what you would like to change. Please make sure to
 update tests as appropriate. ## License [MIT](https://github.com/amarquaye/
 pywriter/blob/master/LICENSE) ## Authors - [Jesse Amarquaye](https://
```

