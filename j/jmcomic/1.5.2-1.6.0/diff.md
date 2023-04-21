# Comparing `tmp/jmcomic-1.5.2.tar.gz` & `tmp/jmcomic-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-xgyf_ajn/jmcomic-1.5.2.tar", last modified: Mon Apr 17 12:24:02 2023, max compression
+gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-rlqqn138/jmcomic-1.6.0.tar", last modified: Fri Apr 21 08:02:13 2023, max compression
```

## Comparing `jmcomic-1.5.2.tar` & `jmcomic-1.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:24:02.000000 jmcomic-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 12:23:53.000000 jmcomic-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-17 12:24:02.000000 jmcomic-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-17 12:23:53.000000 jmcomic-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 12:24:02.000000 jmcomic-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-17 12:23:53.000000 jmcomic-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/jm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/jm_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-17 12:23:53.000000 jmcomic-1.5.2/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 12:24:02.000000 jmcomic-1.5.2/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:02:13.000000 jmcomic-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 08:02:02.000000 jmcomic-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-21 08:02:13.000000 jmcomic-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-21 08:02:02.000000 jmcomic-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:02:13.000000 jmcomic-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-21 08:02:02.000000 jmcomic-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/jm_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/jm_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-21 08:02:02.000000 jmcomic-1.6.0/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 08:02:13.000000 jmcomic-1.6.0/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-1.5.2/LICENSE` & `jmcomic-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-1.5.2/PKG-INFO` & `jmcomic-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 1.5.2
+Version: 1.6.0
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-1.5.2/README.md` & `jmcomic-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-1.5.2/setup.py` & `jmcomic-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.5.2/src/jmcomic/api.py` & `jmcomic-1.6.0/src/jmcomic/api.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.5.2/src/jmcomic/jm_client.py` & `jmcomic-1.6.0/src/jmcomic/jm_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,16 +98,16 @@
         # 检查 from_album
         if photo_detail.from_album is None:
             photo_detail.from_album = self.get_album_detail(photo_detail.album_id)
 
         # 检查 page_arr 和 data_original_domain
         if photo_detail.page_arr is None or photo_detail.data_original_domain is None:
             new = self.get_photo_detail(photo_detail.photo_id, False)
-            photo_detail.page_arr = new.page_arr
-            photo_detail.data_original_domain = new.data_original_domain
+            new.from_album = photo_detail.from_album
+            photo_detail.__dict__.update(new.__dict__)
 
     # -- search --
 
     def search_album(self, search_query, main_tag=0) -> JmSearchPage:
         params = {
             'main_tag': main_tag,
             'search_query': search_query,
```

### Comparing `jmcomic-1.5.2/src/jmcomic/jm_config.py` & `jmcomic-1.6.0/src/jmcomic/jm_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,17 +74,15 @@
     @classmethod
     def get_jmcomic_url(cls, postman=None):
         """
         访问禁漫的永久网域，从而得到一个可用的禁漫网址，
         """
         if postman is None:
             from common import Postmans
-            postman = Postmans \
-                .get_impl_clazz('cffi') \
-                .create(headers=cls.headers(cls.JM_REDIRECT_URL))
+            postman = Postmans.get_impl_clazz('cffi_Session').create()
 
         domain = postman.with_redirect_catching().get(cls.JM_REDIRECT_URL)
         cls.jm_debug('获取禁漫地址', f'[{cls.JM_REDIRECT_URL}] → [{domain}]')
         return domain
 
     @classmethod
     def check_html(cls, html: str, url=None):
```

### Comparing `jmcomic-1.5.2/src/jmcomic/jm_entity.py` & `jmcomic-1.6.0/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.5.2/src/jmcomic/jm_option.py` & `jmcomic-1.6.0/src/jmcomic/jm_option.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.5.2/src/jmcomic/jm_service.py` & `jmcomic-1.6.0/src/jmcomic/jm_service.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.5.2/src/jmcomic/jm_toolkit.py` & `jmcomic-1.6.0/src/jmcomic/jm_toolkit.py`

 * *Files identical despite different names*

### Comparing `jmcomic-1.5.2/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-1.6.0/src/jmcomic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 1.5.2
+Version: 1.6.0
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

