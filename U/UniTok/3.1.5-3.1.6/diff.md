# Comparing `tmp/UniTok-3.1.5.tar.gz` & `tmp/UniTok-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniTok-3.1.5.tar", last modified: Fri Apr 21 12:20:06 2023, max compression
+gzip compressed data, was "UniTok-3.1.6.tar", last modified: Fri Apr 21 12:21:12 2023, max compression
```

## Comparing `UniTok-3.1.5.tar` & `UniTok-3.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 12:20:06.441267 UniTok-3.1.5/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-21 12:20:06.441158 UniTok-3.1.5/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.1.5/README.md
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 12:20:06.437532 UniTok-3.1.5/UniTok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.1.5/UniTok/__init__.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 12:20:06.438891 UniTok-3.1.5/UniTok/analysis/
--rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.1.5/UniTok/analysis/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.1.5/UniTok/analysis/lengths.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.1.5/UniTok/analysis/plot.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.1.5/UniTok/cols.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     3787 2023-04-21 12:19:35.000000 UniTok-3.1.5/UniTok/column.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.1.5/UniTok/global_setting.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     4288 2023-04-20 08:16:56.000000 UniTok-3.1.5/UniTok/meta.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 12:20:06.440884 UniTok-3.1.5/UniTok/tok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.1.5/UniTok/tok/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      911 2023-04-21 12:17:40.000000 UniTok-3.1.5/UniTok/tok/bert_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.1.5/UniTok/tok/ent_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.1.5/UniTok/tok/id_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1442 2023-04-21 12:17:40.000000 UniTok-3.1.5/UniTok/tok/number_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.1.5/UniTok/tok/seq_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.1.5/UniTok/tok/split_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1660 2023-04-21 12:18:50.000000 UniTok-3.1.5/UniTok/tok/tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8838 2023-04-20 08:26:57.000000 UniTok-3.1.5/UniTok/unidep.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6491 2023-04-18 12:49:05.000000 UniTok-3.1.5/UniTok/unitok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8788 2023-04-21 12:18:43.000000 UniTok-3.1.5/UniTok/vocab.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1448 2023-04-18 12:43:49.000000 UniTok-3.1.5/UniTok/vocabs.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 12:20:06.438213 UniTok-3.1.5/UniTok.egg-info/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-21 12:20:06.000000 UniTok-3.1.5/UniTok.egg-info/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-04-21 12:20:06.000000 UniTok-3.1.5/UniTok.egg-info/SOURCES.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-04-21 12:20:06.000000 UniTok-3.1.5/UniTok.egg-info/dependency_links.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-04-21 12:20:06.000000 UniTok-3.1.5/UniTok.egg-info/requires.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-04-21 12:20:06.000000 UniTok-3.1.5/UniTok.egg-info/top_level.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-04-21 12:20:06.441303 UniTok-3.1.5/setup.cfg
--rw-r--r--   0 jyonnliu   (501) staff       (20)      724 2023-04-21 12:19:55.000000 UniTok-3.1.5/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 12:21:12.533585 UniTok-3.1.6/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-21 12:21:12.533481 UniTok-3.1.6/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.1.6/README.md
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 12:21:12.530101 UniTok-3.1.6/UniTok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.1.6/UniTok/__init__.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 12:21:12.531224 UniTok-3.1.6/UniTok/analysis/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.1.6/UniTok/analysis/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.1.6/UniTok/analysis/lengths.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.1.6/UniTok/analysis/plot.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.1.6/UniTok/cols.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     3787 2023-04-21 12:19:35.000000 UniTok-3.1.6/UniTok/column.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.1.6/UniTok/global_setting.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     4288 2023-04-20 08:16:56.000000 UniTok-3.1.6/UniTok/meta.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 12:21:12.533324 UniTok-3.1.6/UniTok/tok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.1.6/UniTok/tok/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      911 2023-04-21 12:17:40.000000 UniTok-3.1.6/UniTok/tok/bert_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.1.6/UniTok/tok/ent_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.1.6/UniTok/tok/id_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1442 2023-04-21 12:17:40.000000 UniTok-3.1.6/UniTok/tok/number_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.1.6/UniTok/tok/seq_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.1.6/UniTok/tok/split_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1697 2023-04-21 12:21:10.000000 UniTok-3.1.6/UniTok/tok/tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     8838 2023-04-20 08:26:57.000000 UniTok-3.1.6/UniTok/unidep.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6491 2023-04-18 12:49:05.000000 UniTok-3.1.6/UniTok/unitok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     8788 2023-04-21 12:18:43.000000 UniTok-3.1.6/UniTok/vocab.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1448 2023-04-18 12:43:49.000000 UniTok-3.1.6/UniTok/vocabs.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-21 12:21:12.530724 UniTok-3.1.6/UniTok.egg-info/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-21 12:21:12.000000 UniTok-3.1.6/UniTok.egg-info/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-04-21 12:21:12.000000 UniTok-3.1.6/UniTok.egg-info/SOURCES.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-04-21 12:21:12.000000 UniTok-3.1.6/UniTok.egg-info/dependency_links.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-04-21 12:21:12.000000 UniTok-3.1.6/UniTok.egg-info/requires.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-04-21 12:21:12.000000 UniTok-3.1.6/UniTok.egg-info/top_level.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-04-21 12:21:12.533614 UniTok-3.1.6/setup.cfg
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      724 2023-04-21 12:21:10.000000 UniTok-3.1.6/setup.py
```

### Comparing `UniTok-3.1.5/PKG-INFO` & `UniTok-3.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.1.5
+Version: 3.1.6
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.1.5/README.md` & `UniTok-3.1.6/README.md`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.5/UniTok/analysis/lengths.py` & `UniTok-3.1.6/UniTok/analysis/lengths.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.5/UniTok/analysis/plot.py` & `UniTok-3.1.6/UniTok/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.5/UniTok/column.py` & `UniTok-3.1.6/UniTok/column.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.5/UniTok/meta.py` & `UniTok-3.1.6/UniTok/meta.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.5/UniTok/tok/bert_tok.py` & `UniTok-3.1.6/UniTok/tok/bert_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.5/UniTok/tok/number_tok.py` & `UniTok-3.1.6/UniTok/tok/number_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.5/UniTok/tok/split_tok.py` & `UniTok-3.1.6/UniTok/tok/split_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.5/UniTok/tok/tok.py` & `UniTok-3.1.6/UniTok/tok/tok.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,15 +40,16 @@
         raise NotImplemented
 
     def _t(self, obj):
         """
         wrapped tokenize method, filter out unknown token
         """
         ids = self.t(obj)
-        self.vocab.counts(ids)
+
+        self.vocab.counts(ids if isinstance(ids, list) else [ids])
 
         if isinstance(ids, list):
             return list(filter(lambda index: index > -1, ids))
         if ids == -1:
             raise ValueError('Single Tokenizer should provide vocab, but -1 is given')
         return ids
```

### Comparing `UniTok-3.1.5/UniTok/unidep.py` & `UniTok-3.1.6/UniTok/unidep.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.5/UniTok/unitok.py` & `UniTok-3.1.6/UniTok/unitok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.5/UniTok/vocab.py` & `UniTok-3.1.6/UniTok/vocab.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.5/UniTok/vocabs.py` & `UniTok-3.1.6/UniTok/vocabs.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.5/UniTok.egg-info/PKG-INFO` & `UniTok-3.1.6/UniTok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.1.5
+Version: 3.1.6
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.1.5/UniTok.egg-info/SOURCES.txt` & `UniTok-3.1.6/UniTok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

