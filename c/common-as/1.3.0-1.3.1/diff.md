# Comparing `tmp/common_as-1.3.0.tar.gz` & `tmp/common_as-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_as-1.3.0.tar", last modified: Sun Feb 26 15:42:19 2023, max compression
+gzip compressed data, was "common_as-1.3.1.tar", last modified: Fri Apr 21 17:41:23 2023, max compression
```

## Comparing `common_as-1.3.0.tar` & `common_as-1.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-02-26 15:42:19.752927 common_as-1.3.0/
--rw-rw-rw-   0        0        0     1093 2023-01-25 06:12:19.000000 common_as-1.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0      212 2023-02-26 15:42:19.752927 common_as-1.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-26 15:42:19.706060 common_as-1.3.0/common_as/
--rw-rw-rw-   0        0        0      119 2023-01-13 05:01:03.000000 common_as-1.3.0/common_as/__init__.py
--rw-rw-rw-   0        0        0     1249 2023-01-26 05:09:44.000000 common_as-1.3.0/common_as/base_helper.py
--rw-rw-rw-   0        0        0    15291 2023-01-26 17:54:26.000000 common_as-1.3.0/common_as/calculate_ta.py
--rw-rw-rw-   0        0        0     1691 2023-01-26 17:59:22.000000 common_as-1.3.0/common_as/date_util.py
--rw-rw-rw-   0        0        0     2527 2023-01-26 07:59:12.000000 common_as-1.3.0/common_as/dbmysql.py
--rw-rw-rw-   0        0        0      360 2023-01-13 05:01:03.000000 common_as-1.3.0/common_as/enums.py
--rw-rw-rw-   0        0        0      385 2023-01-13 05:01:03.000000 common_as-1.3.0/common_as/file_util.py
--rw-rw-rw-   0        0        0    19434 2023-02-01 01:39:27.000000 common_as-1.3.0/common_as/helper_breeze.py
--rw-rw-rw-   0        0        0    11979 2023-02-09 08:02:24.000000 common_as-1.3.0/common_as/helper_ks.py
--rw-rw-rw-   0        0        0    16861 2023-01-26 11:08:46.000000 common_as-1.3.0/common_as/kitehelper.py
--rw-rw-rw-   0        0        0     7309 2023-01-26 11:30:07.000000 common_as-1.3.0/common_as/levels.py
--rw-rw-rw-   0        0        0     1350 2023-02-01 01:41:07.000000 common_as-1.3.0/common_as/log_util.py
--rw-rw-rw-   0        0        0     2351 2023-01-26 18:07:06.000000 common_as-1.3.0/common_as/telegram_util.py
--rw-rw-rw-   0        0        0     2237 2023-01-25 08:49:37.000000 common_as-1.3.0/common_as/util.py
-drwxrwxrwx   0        0        0        0 2023-02-26 15:42:19.737306 common_as-1.3.0/common_as.egg-info/
--rw-rw-rw-   0        0        0      212 2023-02-26 15:42:19.000000 common_as-1.3.0/common_as.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-02-26 15:42:19.000000 common_as-1.3.0/common_as.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-26 15:42:19.000000 common_as-1.3.0/common_as.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-02-26 15:42:19.000000 common_as-1.3.0/common_as.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-26 15:42:19.000000 common_as-1.3.0/common_as.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-26 15:42:19.752927 common_as-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      354 2023-02-26 15:39:21.000000 common_as-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 17:41:23.378647 common_as-1.3.1/
+-rw-rw-rw-   0        0        0     1093 2023-01-04 12:01:22.000000 common_as-1.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      212 2023-04-21 17:41:23.374103 common_as-1.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 17:41:23.338237 common_as-1.3.1/common_as/
+-rw-rw-rw-   0        0        0      133 2023-04-21 17:24:28.000000 common_as-1.3.1/common_as/__init__.py
+-rw-rw-rw-   0        0        0     1249 2023-02-01 17:58:41.000000 common_as-1.3.1/common_as/base_helper.py
+-rw-rw-rw-   0        0        0    15291 2023-04-21 02:44:22.000000 common_as-1.3.1/common_as/calculate_ta.py
+-rw-rw-rw-   0        0        0     1691 2023-04-21 02:44:53.000000 common_as-1.3.1/common_as/date_util.py
+-rw-rw-rw-   0        0        0     2527 2023-04-21 02:38:37.000000 common_as-1.3.1/common_as/dbmysql.py
+-rw-rw-rw-   0        0        0      360 2023-04-21 02:45:15.000000 common_as-1.3.1/common_as/enums.py
+-rw-rw-rw-   0        0        0      385 2023-04-21 02:45:31.000000 common_as-1.3.1/common_as/file_util.py
+-rw-rw-rw-   0        0        0    19434 2023-04-21 02:42:12.000000 common_as-1.3.1/common_as/helper_breeze.py
+-rw-rw-rw-   0        0        0    11979 2023-04-21 02:47:15.000000 common_as-1.3.1/common_as/helper_ks.py
+-rw-rw-rw-   0        0        0    16861 2023-04-21 02:45:46.000000 common_as-1.3.1/common_as/kitehelper.py
+-rw-rw-rw-   0        0        0     7355 2023-04-21 02:43:37.000000 common_as-1.3.1/common_as/levels.py
+-rw-rw-rw-   0        0        0     1350 2023-04-21 02:46:10.000000 common_as-1.3.1/common_as/log_util.py
+-rw-rw-rw-   0        0        0     2351 2023-04-21 02:46:35.000000 common_as-1.3.1/common_as/telegram_util.py
+-rw-rw-rw-   0        0        0     2237 2023-04-21 02:47:03.000000 common_as-1.3.1/common_as/util.py
+drwxrwxrwx   0        0        0        0 2023-04-21 17:41:23.374103 common_as-1.3.1/common_as.egg-info/
+-rw-rw-rw-   0        0        0      212 2023-04-21 17:41:23.000000 common_as-1.3.1/common_as.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-04-21 17:41:23.000000 common_as-1.3.1/common_as.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 17:41:23.000000 common_as-1.3.1/common_as.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-21 17:41:23.000000 common_as-1.3.1/common_as.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 17:41:23.000000 common_as-1.3.1/common_as.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 17:41:23.378647 common_as-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      354 2023-04-21 17:31:14.000000 common_as-1.3.1/setup.py
```

### Comparing `common_as-1.3.0/LICENSE.txt` & `common_as-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `common_as-1.3.0/common_as/base_helper.py` & `common_as-1.3.1/common_as/base_helper.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.0/common_as/calculate_ta.py` & `common_as-1.3.1/common_as/calculate_ta.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.0/common_as/date_util.py` & `common_as-1.3.1/common_as/date_util.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.0/common_as/dbmysql.py` & `common_as-1.3.1/common_as/dbmysql.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.0/common_as/helper_breeze.py` & `common_as-1.3.1/common_as/helper_breeze.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.0/common_as/helper_ks.py` & `common_as-1.3.1/common_as/helper_ks.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.0/common_as/kitehelper.py` & `common_as-1.3.1/common_as/kitehelper.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.0/common_as/levels.py` & `common_as-1.3.1/common_as/levels.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,16 +149,19 @@
             self.at_time=datetime.now()
         else:
             self.at_time=at_time
         self.symbol=symbol
         self.exchangeToken=exchangeToken
         self.token=exchangeToken
 
+    def __str__():
+        return f'code: {self.code}, qty: {self.qty}, price: {self.price}, b/s: {self.buysell}, token: {self.token}'
+
     def to_string(self):
-        return f'symbol: {self.symbol}, token: {self.token}, qty: {self.qty}, code: {self.code}, b/s: {self.buysell}'
+        return __str__()
 
     @classmethod
     def fromjson(self, ordjson):
         "Initialize MyData from a file"
         ord = self(ordjson['symbol'], 1,2,3,4,5,6,7)
         return ord
```

### Comparing `common_as-1.3.0/common_as/log_util.py` & `common_as-1.3.1/common_as/log_util.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.0/common_as/telegram_util.py` & `common_as-1.3.1/common_as/telegram_util.py`

 * *Files identical despite different names*

### Comparing `common_as-1.3.0/common_as/util.py` & `common_as-1.3.1/common_as/util.py`

 * *Files identical despite different names*

