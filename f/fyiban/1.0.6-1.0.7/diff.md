# Comparing `tmp/fyiban-1.0.6.tar.gz` & `tmp/fyiban-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyiban-1.0.6.tar", last modified: Fri Oct 28 10:03:43 2022, max compression
+gzip compressed data, was "fyiban-1.0.7.tar", last modified: Fri Apr 21 07:56:39 2023, max compression
```

## Comparing `fyiban-1.0.6.tar` & `fyiban-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 10:03:43.785407 fyiban-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     2769 2022-10-28 10:03:43.785407 fyiban-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-10-28 10:03:32.000000 fyiban-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 10:03:43.785407 fyiban-1.0.6/fyiban.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2769 2022-10-28 10:03:43.000000 fyiban-1.0.6/fyiban.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-10-28 10:03:43.000000 fyiban-1.0.6/fyiban.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 10:03:43.000000 fyiban-1.0.6/fyiban.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-28 10:03:43.000000 fyiban-1.0.6/fyiban.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-28 10:03:43.000000 fyiban-1.0.6/fyiban.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-10-28 10:03:32.000000 fyiban-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-10-28 10:03:43.789407 fyiban-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 10:03:43.781407 fyiban-1.0.6/yiban/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 10:03:43.781407 fyiban-1.0.6/yiban/Apis/
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-10-28 10:03:32.000000 fyiban-1.0.6/yiban/Apis/Task.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-10-28 10:03:32.000000 fyiban-1.0.6/yiban/Apis/User.py
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-10-28 10:03:32.000000 fyiban-1.0.6/yiban/Apis/Yiban.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-28 10:03:32.000000 fyiban-1.0.6/yiban/Apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 10:03:43.785407 fyiban-1.0.6/yiban/Core/
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-10-28 10:03:32.000000 fyiban-1.0.6/yiban/Core/BaseReq.py
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2022-10-28 10:03:32.000000 fyiban-1.0.6/yiban/Core/EpidemicPrevention.py
--rw-r--r--   0 runner    (1001) docker     (121)     3682 2022-10-28 10:03:32.000000 fyiban-1.0.6/yiban/Core/Login.py
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-10-28 10:03:32.000000 fyiban-1.0.6/yiban/Core/SchoolBased.py
--rw-r--r--   0 runner    (1001) docker     (121)     2919 2022-10-28 10:03:32.000000 fyiban-1.0.6/yiban/Core/SchoolBasedAuth.py
--rw-r--r--   0 runner    (1001) docker     (121)     8776 2022-10-28 10:03:32.000000 fyiban-1.0.6/yiban/Core/TaskFeedback.py
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-28 10:03:32.000000 fyiban-1.0.6/yiban/Core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-10-28 10:03:32.000000 fyiban-1.0.6/yiban/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:56:39.815772 fyiban-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-21 07:56:39.815772 fyiban-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-21 07:56:28.000000 fyiban-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:56:39.815772 fyiban-1.0.7/fyiban.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-21 07:56:39.000000 fyiban-1.0.7/fyiban.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-21 07:56:39.000000 fyiban-1.0.7/fyiban.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 07:56:39.000000 fyiban-1.0.7/fyiban.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 07:56:39.000000 fyiban-1.0.7/fyiban.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 07:56:39.000000 fyiban-1.0.7/fyiban.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-21 07:56:28.000000 fyiban-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-21 07:56:39.815772 fyiban-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:56:39.811772 fyiban-1.0.7/yiban/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:56:39.815772 fyiban-1.0.7/yiban/Apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-21 07:56:28.000000 fyiban-1.0.7/yiban/Apis/Task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-21 07:56:28.000000 fyiban-1.0.7/yiban/Apis/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-21 07:56:28.000000 fyiban-1.0.7/yiban/Apis/Yiban.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-21 07:56:28.000000 fyiban-1.0.7/yiban/Apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:56:39.815772 fyiban-1.0.7/yiban/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-21 07:56:28.000000 fyiban-1.0.7/yiban/Core/BaseReq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-21 07:56:28.000000 fyiban-1.0.7/yiban/Core/EpidemicPrevention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-21 07:56:28.000000 fyiban-1.0.7/yiban/Core/Login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-21 07:56:28.000000 fyiban-1.0.7/yiban/Core/SchoolBased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-21 07:56:28.000000 fyiban-1.0.7/yiban/Core/SchoolBasedAuth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-04-21 07:56:28.000000 fyiban-1.0.7/yiban/Core/TaskFeedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-21 07:56:28.000000 fyiban-1.0.7/yiban/Core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-21 07:56:28.000000 fyiban-1.0.7/yiban/__init__.py
```

### Comparing `fyiban-1.0.6/PKG-INFO` & `fyiban-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyiban
-Version: 1.0.6
+Version: 1.0.7
 Summary: Apis lib for yiban.
 Home-page: https://github.com/sricor/yiban
 Author: Sricor
 Author-email: josricor@outlook.com
 License: MIT
 Project-URL: Source, https://github.com/sricor/yiban
 Project-URL: Bug Tracker, https://github.com/sricor/yiban/issues
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.7.*
 Description-Content-Type: text/markdown
 
 <h1 align="center"> 易班 🔔</h1>  
   
 - 🔥 简单、易用、可扩展的易班 API 接口  
 - 📕 适用于校本化分应用打卡
 - ⏰ 适用于校本化晚点签到
```

### Comparing `fyiban-1.0.6/README.md` & `fyiban-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fyiban-1.0.6/fyiban.egg-info/PKG-INFO` & `fyiban-1.0.7/fyiban.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyiban
-Version: 1.0.6
+Version: 1.0.7
 Summary: Apis lib for yiban.
 Home-page: https://github.com/sricor/yiban
 Author: Sricor
 Author-email: josricor@outlook.com
 License: MIT
 Project-URL: Source, https://github.com/sricor/yiban
 Project-URL: Bug Tracker, https://github.com/sricor/yiban/issues
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.7.*
 Description-Content-Type: text/markdown
 
 <h1 align="center"> 易班 🔔</h1>  
   
 - 🔥 简单、易用、可扩展的易班 API 接口  
 - 📕 适用于校本化分应用打卡
 - ⏰ 适用于校本化晚点签到
```

### Comparing `fyiban-1.0.6/setup.cfg` & `fyiban-1.0.7/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 	Development Status :: 4 - Beta
 keywords = yiban school task health
 
 [options]
 package_dir = 
 	= .
 packages = find:
-python_requires = >=3.7.*
 install_requires = 
 	requests
 	pycryptodome
 
 [options.packages.find]
 where = .
 exclude =
```

### Comparing `fyiban-1.0.6/yiban/Apis/Task.py` & `fyiban-1.0.7/yiban/Apis/Task.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from yiban.Core import SchoolBased
 from yiban.Core import TaskFeedback
 from yiban.Core import SchoolBasedAuth
 from yiban.Core import EpidemicPrevention
 
 class Task:
-    def __init__(self, access_token):
-        req = SchoolBasedAuth(access_token)._auth()
+    def __init__(self, mobile: str, password: str):
+        req = SchoolBasedAuth(mobile=mobile, password=password)._auth()
 
         self.task_feedback = TaskFeedback(req)             # 任务反馈
         self.epidemic_prevention = EpidemicPrevention(req) # 疫情防控
 
     def get_task_feedback_completed_task(self):
         return self.task_feedback.get_completed_task()
```

### Comparing `fyiban-1.0.6/yiban/Apis/User.py` & `fyiban-1.0.7/yiban/Apis/User.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 # @Author: Sricor
 # @Date: 2022-10-25
 
 """ User Class """
 
-from yiban.Core import Login
+from yiban.Core import SchoolBasedAuth
 
 class User:
     def __init__(self, mobile: str, password: str):
         self.__mobile = mobile
         self.__password = password
-        self.__access_token = Login().get_user_access_token(self.__mobile, self.__password)
+        # self.__access_token = Login().get_user_access_token(self.__mobile, self.__password)
 
-    def get_user_access_token(self) -> str:
-        """获取用户登录密钥"""
-        return self.__access_token
+    # def get_user_access_token(self) -> str:
+    #     """获取用户登录密钥"""
+    #     return self.__access_token
 
     # def get_user_name(self) -> str:
     #     """获取用户名"""
     #     return self.user['user']['name']
 
     # def get_user_phone(self) -> str:
     #     """获取用户手机号"""
```

### Comparing `fyiban-1.0.6/yiban/Apis/Yiban.py` & `fyiban-1.0.7/yiban/Apis/Yiban.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,10 +22,10 @@
         易班 Python API service
         :param mobile:   (必须) 用户账号
         :param password: (必须) 用户密码
         """
         super().__init__(mobile=mobile, password=password)  # init User
         
         try:
-            super(User, self).__init__(access_token=self.get_user_access_token())  # init Task
+            super(User, self).__init__(mobile=mobile, password=password)  # init Task
         except:
             pass
```

### Comparing `fyiban-1.0.6/yiban/Core/BaseReq.py` & `fyiban-1.0.7/yiban/Core/BaseReq.py`

 * *Files identical despite different names*

### Comparing `fyiban-1.0.6/yiban/Core/EpidemicPrevention.py` & `fyiban-1.0.7/yiban/Core/EpidemicPrevention.py`

 * *Files identical despite different names*

### Comparing `fyiban-1.0.6/yiban/Core/Login.py` & `fyiban-1.0.7/yiban/Core/Login.py`

 * *Files identical despite different names*

### Comparing `fyiban-1.0.6/yiban/Core/SchoolBased.py` & `fyiban-1.0.7/yiban/Core/SchoolBased.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,16 @@
         return '00000'
 
     @staticmethod
     def headers() -> Dict: 
         return { "Origin": "https://c.uyiban.com", "User-Agent": "Yiban", "AppVersion": "5.0" }
 
     @staticmethod
-    def cookies(access_token) -> Dict: 
-        return { "yiban_user_token": access_token, "loginToken": access_token, "csrf_token": "00000" }
+    def cookies() -> Dict: 
+        return {  "csrf_token": "00000" }
 
     @staticmethod
     def _log(msg: str = None, level: int = 20) -> None:
         msg = f"Yiban {msg}"
         log(msg=msg, level=level)
 
     @staticmethod
```

### Comparing `fyiban-1.0.6/yiban/Core/SchoolBasedAuth.py` & `fyiban-1.0.7/yiban/Core/SchoolBasedAuth.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,25 +7,32 @@
 
 from re import findall
 from requests.utils import add_dict_to_cookiejar
 
 from yiban.Core import BaseReq
 from yiban.Core import SchoolBased
 
+from base64 import b64encode
+from Crypto.PublicKey import RSA
+from Crypto.Cipher import PKCS1_v1_5
+
+from typing import AnyStr
 
 class SchoolBasedAuth:
-    def __init__(self, access_token: str) -> None :
+    def __init__(self, mobile: str, password: str) -> None :
         self.req = BaseReq()
         self.user_info = {}
+        self.mobile = mobile
+        self.password = password
 
         # Set auth requests headers and cookies
         self.req.session.headers.update(SchoolBased.headers())
 
         add_dict_to_cookiejar(
-            self.req.session.cookies, SchoolBased.cookies(access_token))
+            self.req.session.cookies, SchoolBased.cookies())
 
     def _re_auth(self, verify: str) -> None:
         client_id = '95626fa3080300ea'
         redirect_uri = 'https://f.yiban.cn/iapp7463'
 
         self.req.get(
             url='https://api.uyiban.com/base/c/auth/yiban',
@@ -51,14 +58,29 @@
             }
         )
 
     def _auth(self) -> None:
         "https://f.yiban.cn/iapp/index"
         "https://f.yiban.cn/iframe/index"
 
+        login_res = self.req.get(
+            url='https://oauth.yiban.cn/code/html?client_id=95626fa3080300ea&redirect_uri=https://f.yiban.cn/iapp7463'
+        )
+        rsa_key = login_res.text.split('id="key" value="')[1].split('"')[0]
+        login_data = {
+            'oauth_uname' : self.mobile,
+            'oauth_upwd' : self.encrypt_rsa(self.password, rsa_key),
+            'client_id' : '95626fa3080300ea',
+            'redirect_uri' : 'https://f.yiban.cn/iapp7463'
+        }
+        login_res = self.req.post(
+            url="https://oauth.yiban.cn/code/usersure",
+            data=login_data
+        )
+
         response = self.req.get(
             url='https://f.yiban.cn/iframe/index',
             params={'act': 'iapp7463'},
             allow_redirects=False
         )
 
         verify = findall(r"verify_request=(.*?)&", response.headers.get("Location"))[0]
@@ -72,18 +94,34 @@
                 'verifyRequest': verify, 
                 'CSRF': SchoolBased.csrf()
             },
         ).json()
 
         # if auth done return requests class else raise
         if response['code'] == 0:
+            self.user_info = response['data']
             return self.req
         else:
             raise Exception(f"Auth Error {response['msg']}")
 
+    def _get_name(self) -> AnyStr:
+        return self.user_info['PersonName']
+
+    @staticmethod
+    def encrypt_rsa(data: str, rsa_key: str) -> AnyStr:
+        """
+        登录密码加密
+        :param data: （必须）待加密密码
+        :return: Any
+        """
+        data = bytes(data, encoding="utf8")
+        encrypt = PKCS1_v1_5.new(RSA.importKey(rsa_key))
+        sencrypt = b64encode(encrypt.encrypt(data))
+        return sencrypt.decode("utf-8")
+
 
 """
 {
 'code': 0, 
 'msg': '', 
 'data': {
     'UniversityName': '',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fyiban-1.0.6/yiban/Core/TaskFeedback.py` & `fyiban-1.0.7/yiban/Core/TaskFeedback.py`

 * *Files identical despite different names*

