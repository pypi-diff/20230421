# Comparing `tmp/proteinTools-1.2.7.tar.gz` & `tmp/proteinTools-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.2.7.tar", last modified: Thu Apr 20 17:23:30 2023, max compression
+gzip compressed data, was "proteinTools-1.2.8.tar", last modified: Fri Apr 21 04:53:06 2023, max compression
```

## Comparing `proteinTools-1.2.7.tar` & `proteinTools-1.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 17:23:30.407026 proteinTools-1.2.7/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.2.7/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 17:23:30.401889 proteinTools-1.2.7/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.2.7/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 17:23:30.268824 proteinTools-1.2.7/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    51744 2023-04-20 17:23:15.000000 proteinTools-1.2.7/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.2.7/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 17:23:30.365679 proteinTools-1.2.7/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 17:23:30.000000 proteinTools-1.2.7/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-20 17:23:30.000000 proteinTools-1.2.7/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-20 17:23:30.000000 proteinTools-1.2.7/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-20 17:23:30.000000 proteinTools-1.2.7/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-20 17:23:30.000000 proteinTools-1.2.7/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-20 17:23:30.415181 proteinTools-1.2.7/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-20 17:23:22.000000 proteinTools-1.2.7/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-21 04:53:06.040289 proteinTools-1.2.8/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.2.8/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-21 04:53:06.037398 proteinTools-1.2.8/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.2.8/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-21 04:53:05.921794 proteinTools-1.2.8/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    52047 2023-04-21 04:52:30.000000 proteinTools-1.2.8/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.2.8/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-21 04:53:06.018133 proteinTools-1.2.8/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-21 04:53:05.000000 proteinTools-1.2.8/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-21 04:53:05.000000 proteinTools-1.2.8/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-21 04:53:05.000000 proteinTools-1.2.8/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-21 04:53:05.000000 proteinTools-1.2.8/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-21 04:53:05.000000 proteinTools-1.2.8/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-21 04:53:06.046394 proteinTools-1.2.8/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-21 04:52:58.000000 proteinTools-1.2.8/setup.py
```

### Comparing `proteinTools-1.2.7/LICENSE` & `proteinTools-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.2.7/proteinTools/PT.py` & `proteinTools-1.2.8/proteinTools/PT.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,19 +469,27 @@
                             end = int(line[8])
                             chain = line[4]
                         except:
                             try:
                                 start = int(line[6])
                                 end = int(line[9])
                                 chain = line[5]
+                
                             except:
                                 start = int(line[5][1:])
                                 end = int(line[8])
                                 chain = line[5][:1]
-                        chainindex = chainkeys.index(chain)
+                        try:
+                            chainindex = chainkeys.index(chain)
+                        except:
+                            try:
+                                chainindex = chainkeys.index(line[2])
+                            except:
+                                continue
+                                
                         for i in range(0, chainindex):
                             start += self.chains[chainkeys[i]]
                             end += self.chains[chainkeys[i]]
 
                         for i in range(start, end + 1):
                             sheet.append(i)
                     elif line[0:5] == 'HELIX':
```

### Comparing `proteinTools-1.2.7/setup.py` & `proteinTools-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.2.7",
+    version = "1.2.8",
     author = "Christian de Frondeville",
     description = "Lightweight, object-oriented bioinformatics package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
 )
```

