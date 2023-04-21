# Comparing `tmp/pywriter-0.0.1-py3-none-any.whl.zip` & `tmp/pywriter-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2543 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      418 b- defN 23-Apr-14 01:48 pywriter/__init__.py
--rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-15 02:27 pywriter-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      703 b- defN 23-Apr-15 02:27 pywriter-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-15 02:27 pywriter-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-15 02:27 pywriter-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      465 b- defN 23-Apr-15 02:27 pywriter-0.0.1.dist-info/RECORD
-6 files, 2780 bytes uncompressed, 1697 bytes compressed:  39.0%
+Zip file size: 3693 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      417 b- defN 23-Apr-20 22:43 pywriter/__init__.py
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-21 00:24 pywriter-0.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3891 b- defN 23-Apr-21 00:24 pywriter-0.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 00:24 pywriter-0.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-21 00:24 pywriter-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      466 b- defN 23-Apr-21 00:24 pywriter-0.1.0.dist-info/RECORD
+6 files, 5968 bytes uncompressed, 2847 bytes compressed:  52.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pywriter/__init__.py
 Comment: 
 
-Filename: pywriter-0.0.1.dist-info/LICENSE
+Filename: pywriter-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: pywriter-0.0.1.dist-info/METADATA
+Filename: pywriter-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: pywriter-0.0.1.dist-info/WHEEL
+Filename: pywriter-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: pywriter-0.0.1.dist-info/top_level.txt
+Filename: pywriter-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pywriter-0.0.1.dist-info/RECORD
+Filename: pywriter-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywriter/__init__.py

```diff
@@ -1,11 +1,11 @@
 import time
 
 
-def write(text, rate:float | None = 0.01):
+def write(text, rate:float | None = 0.1):
     """Function to print output with typewriter effect
     
     >>> For instance:
         write(text="Hello world!", rate=1) 
         
         This will print all the elements of the string "Hello world!" one by one at the rate of 1 element per second
     """
```

## Comparing `pywriter-0.0.1.dist-info/LICENSE` & `pywriter-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

