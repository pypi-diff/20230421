# Comparing `tmp/bit_boolean_flags-1.0.tar.gz` & `tmp/bit_boolean_flags-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bit_boolean_flags-1.0.tar", last modified: Fri Apr 10 15:43:09 2020, max compression
+gzip compressed data, was "bit_boolean_flags-2.0.tar", last modified: Fri Apr 21 14:03:38 2023, max compression
```

## Comparing `bit_boolean_flags-1.0.tar` & `bit_boolean_flags-2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 beep      (1000) beep      (1000)        0 2020-04-10 15:43:09.000000 bit_boolean_flags-1.0/
-drwxr-xr-x   0 beep      (1000) beep      (1000)        0 2020-04-10 15:43:09.000000 bit_boolean_flags-1.0/src/
-drwxr-xr-x   0 beep      (1000) beep      (1000)        0 2020-04-10 15:43:09.000000 bit_boolean_flags-1.0/src/bit_boolean_flags.egg-info/
--rw-r--r--   0 beep      (1000) beep      (1000)       33 2020-04-10 15:43:09.000000 bit_boolean_flags-1.0/src/bit_boolean_flags.egg-info/top_level.txt
--rw-r--r--   0 beep      (1000) beep      (1000)      920 2020-04-10 15:43:09.000000 bit_boolean_flags-1.0/src/bit_boolean_flags.egg-info/PKG-INFO
--rw-r--r--   0 beep      (1000) beep      (1000)      262 2020-04-10 15:43:09.000000 bit_boolean_flags-1.0/src/bit_boolean_flags.egg-info/SOURCES.txt
--rw-r--r--   0 beep      (1000) beep      (1000)        1 2020-04-10 15:43:09.000000 bit_boolean_flags-1.0/src/bit_boolean_flags.egg-info/dependency_links.txt
--rw-r--r--   0 beep      (1000) beep      (1000)     1218 2020-04-10 15:01:29.000000 bit_boolean_flags-1.0/src/example.py
--rw-r--r--   0 beep      (1000) beep      (1000)      119 2020-02-15 10:53:25.000000 bit_boolean_flags-1.0/src/__init__.py
--rw-r--r--   0 beep      (1000) beep      (1000)     1747 2020-04-10 15:10:32.000000 bit_boolean_flags-1.0/src/BitBooleanFlags.py
--rw-r--r--   0 beep      (1000) beep      (1000)     2063 2020-04-10 15:24:05.000000 bit_boolean_flags-1.0/README.md
--rw-r--r--   0 beep      (1000) beep      (1000)     1416 2020-04-10 15:43:00.000000 bit_boolean_flags-1.0/setup.py
--rw-r--r--   0 beep      (1000) beep      (1000)      920 2020-04-10 15:43:09.000000 bit_boolean_flags-1.0/PKG-INFO
--rw-r--r--   0 beep      (1000) beep      (1000)       79 2020-04-10 15:43:09.000000 bit_boolean_flags-1.0/setup.cfg
+drwxrwxr-x   0 beep      (1000) beep      (1000)        0 2023-04-21 14:03:38.550388 bit_boolean_flags-2.0/
+-rw-rw-r--   0 beep      (1000) beep      (1000)     1061 2023-04-21 13:41:28.000000 bit_boolean_flags-2.0/LICENSE.txt
+-rw-rw-r--   0 beep      (1000) beep      (1000)      860 2023-04-21 14:03:38.550388 bit_boolean_flags-2.0/PKG-INFO
+-rw-rw-r--   0 beep      (1000) beep      (1000)     2125 2023-04-21 13:41:28.000000 bit_boolean_flags-2.0/README.md
+-rw-rw-r--   0 beep      (1000) beep      (1000)       79 2023-04-21 14:03:38.550388 bit_boolean_flags-2.0/setup.cfg
+-rw-rw-r--   0 beep      (1000) beep      (1000)     1374 2023-04-21 14:03:31.000000 bit_boolean_flags-2.0/setup.py
+drwxrwxr-x   0 beep      (1000) beep      (1000)        0 2023-04-21 14:03:38.550388 bit_boolean_flags-2.0/src/
+-rw-rw-r--   0 beep      (1000) beep      (1000)     2000 2023-04-21 13:53:31.000000 bit_boolean_flags-2.0/src/BitBooleanFlags.py
+-rw-rw-r--   0 beep      (1000) beep      (1000)      119 2023-04-21 13:41:28.000000 bit_boolean_flags-2.0/src/__init__.py
+drwxrwxr-x   0 beep      (1000) beep      (1000)        0 2023-04-21 14:03:38.550388 bit_boolean_flags-2.0/src/bit_boolean_flags.egg-info/
+-rw-rw-r--   0 beep      (1000) beep      (1000)      860 2023-04-21 14:03:38.000000 bit_boolean_flags-2.0/src/bit_boolean_flags.egg-info/PKG-INFO
+-rw-rw-r--   0 beep      (1000) beep      (1000)      274 2023-04-21 14:03:38.000000 bit_boolean_flags-2.0/src/bit_boolean_flags.egg-info/SOURCES.txt
+-rw-rw-r--   0 beep      (1000) beep      (1000)        1 2023-04-21 14:03:38.000000 bit_boolean_flags-2.0/src/bit_boolean_flags.egg-info/dependency_links.txt
+-rw-rw-r--   0 beep      (1000) beep      (1000)       33 2023-04-21 14:03:38.000000 bit_boolean_flags-2.0/src/bit_boolean_flags.egg-info/top_level.txt
+-rw-rw-r--   0 beep      (1000) beep      (1000)     1218 2023-04-21 13:41:28.000000 bit_boolean_flags-2.0/src/example.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bit_boolean_flags-1.0/src/example.py` & `bit_boolean_flags-2.0/src/example.py`

 * *Files identical despite different names*

### Comparing `bit_boolean_flags-1.0/src/BitBooleanFlags.py` & `bit_boolean_flags-2.0/src/BitBooleanFlags.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,57 @@
-import math
+import threading
+import functools
 
 class BitBooleanFlags:
     def __init__(self, *args):
-        self._bitflags = {}
-        for index, arg in enumerate(args):
-            self._bitflags[arg] = 1 << index
+        self._bitflags = {arg: 1 << index for index, arg in enumerate(args)}
         self.max_power = len(self._bitflags)
-        
+        self._lock = threading.Lock()
 
-    def __call__(self,*holders):
-        holder_combined = 0
-        for holder in holders:
-            bit_len = 0
-            if(holder>0):
-                bit_len = int(math.log(int(holder),2)) + 1 #Find bit length
-            if (type(holder) is int and holder>=0 and  bit_len<=self.max_power):
-                holder_combined = holder_combined | holder
-            else:
-                raise Exception('Invalid Flag Store, flag variable should be an integer under the bit range of flags !')
-        return self.Inner(self,holder_combined)
+    def __call__(self, *holders):
+        with self._lock:
+            holder_combined = 0
+            for holder in holders:
+                bit_len = self._highest_set_bit_position(holder) + 1 if holder > 0 else 0
+                if isinstance(holder, int) and holder >= 0 and bit_len <= self.max_power:
+                    holder_combined |= holder
+                else:
+                    raise Exception('Invalid Flag Store, flag variable should be an integer under the bit range of flags!')
+            return self.Inner(self, holder_combined)
 
+    @functools.lru_cache(maxsize=None)
     def mappedFlags(self):
-        return self._bitflags
-        
-    
+        with self._lock:
+            return self._bitflags.copy()
+
+    def _highest_set_bit_position(self, n):
+        position = -1
+        while n:
+            position += 1
+            n >>= 1
+        return position
+
     class Inner:
-        def __init__(self, booleanFlags,holder):
+        def __init__(self, booleanFlags, holder):
             self._holder = holder
             self.booleanFlags = booleanFlags
+            self._lock = booleanFlags._lock
 
         def add(self, *flags):
-            for flag in flags:
-                self._holder = self._holder | self.booleanFlags._bitflags[flag]
-            return self._holder
+            with self._lock:
+                for flag in flags:
+                    self._holder |= self.booleanFlags._bitflags[flag]
+                return self._holder
 
         def remove(self, *flags):
-            for flag in flags:
-                self._holder = self._holder ^ self.booleanFlags._bitflags[flag]
-            return self._holder 
+            with self._lock:
+                for flag in flags:
+                    self._holder &= ~self.booleanFlags._bitflags[flag]
+                return self._holder
 
         def orHas(self, *flags):
-            for flag in flags:
-                if ((self._holder & self.booleanFlags._bitflags[flag])!=0):
-                    return True
-            return False
+            with self._lock:
+                return any(self._holder & self.booleanFlags._bitflags[flag] for flag in flags)
 
         def has(self, *flags):
-            for flag in flags:
-                if ((self._holder & self.booleanFlags._bitflags[flag])==0):
-                    return False
-            return True
+            with self._lock:
+                return all(self._holder & self.booleanFlags._bitflags[flag] for flag in flags)
```

### Comparing `bit_boolean_flags-1.0/README.md` & `bit_boolean_flags-2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# [BitBooleanFlags - Wrapper Syntax'ed](https://github.com/redocnib/BitBooleanFlags)
+# BitBooleanFlags - Wrapper Syntax'ed [#](https://github.com/redocnib/BitBooleanFlags)
 
 Bit boolean flag wrapper, allows you to store flags inside a single number. 
 Each flag uses powers of two, and the number of flags you can store depends on the capacity of the numeric data type.
 You can do combined and or operations on the flag as per your requirement, refer examples.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/).
 
 ```bash
-pip install BitBooleanFlags
+pip install bit-boolean-flags
 ```
 
 ## Sample
 
 ```python
 from BitBooleanFlags import BitBooleanFlags
 #initialize with a set of static flags which are available to set
@@ -43,17 +43,20 @@
 
 print("orHas(): ")
 print("Process 1 =>  ROOT_ACCESS or CREATE_FILE : "+ str(BBF(process1).orHas("ROOT_ACCESS","CREATE_FILE")))
 
 print("has(): and operation")
 print("Process 2 =>  DELETE_FOLDER and CREATE_FOLDER : "+ str(BBF(process2).has("DELETE_FOLDER","CREATE_FOLDER")))
 
-#store process1,process2,process3 in db or another storage medium as it a number.
+#store process1,process2,process3 in db or another storage medium as it is a number.
 ```
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
+## Contributors
+[Vysakh](https://github.com/vyshuks)
+
 ## License
-[MIT](https://choosealicense.com/licenses/mit/)
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `bit_boolean_flags-1.0/setup.py` & `bit_boolean_flags-2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from os.path import splitext
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name="bit_boolean_flags",
-    version="1.0",
+    version="2.0",
     packages=find_packages('src'),
     package_dir={'': 'src'},
     py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     # metadata for upload to PyPI
     author="Kiran AK",
     author_email="kiran.txt@gmail.com",
     description='Bit boolean flag wrapper, allows you to store flags inside a single number.',
@@ -26,13 +26,12 @@
 """,
     license="MIT",
     download_url="https://github.com/redocnib/BitBooleanFlags/archive/v1.0.tar.gz",
     keywords="bit flags, boolean bit flags",
     url='https://github.com/redocnib/BitBooleanFlags',
     platforms='Cross platform',
     classifiers=[
-        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
     ],
 )
```

