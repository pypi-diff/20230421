# Comparing `tmp/mw-aiohttp-security-0.1.8.tar.gz` & `tmp/mw-aiohttp-security-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mw-aiohttp-security-0.1.8.tar", last modified: Thu Jul  8 08:28:28 2021, max compression
+gzip compressed data, was "dist\mw-aiohttp-security-0.1.9.tar", last modified: Wed Jul 14 09:41:38 2021, max compression
```

## Comparing `mw-aiohttp-security-0.1.8.tar` & `mw-aiohttp-security-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-07-08 08:28:28.000000 mw-aiohttp-security-0.1.8/
--rw-rw-rw-   0        0        0      547 2021-07-08 08:28:05.000000 mw-aiohttp-security-0.1.8/CHANGES.txt
--rw-rw-rw-   0        0        0     1100 2018-05-04 06:36:08.000000 mw-aiohttp-security-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0       94 2018-10-30 09:57:57.000000 mw-aiohttp-security-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      919 2021-07-08 08:28:28.000000 mw-aiohttp-security-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       72 2021-03-11 03:12:53.000000 mw-aiohttp-security-0.1.8/README.rst
-drwxrwxrwx   0        0        0        0 2021-07-08 08:28:28.000000 mw-aiohttp-security-0.1.8/mw_aiohttp_security/
--rw-rw-rw-   0        0        0     4945 2021-07-08 08:19:35.000000 mw-aiohttp-security-0.1.8/mw_aiohttp_security/__init__.py
--rw-rw-rw-   0        0        0     3496 2021-07-08 07:03:55.000000 mw-aiohttp-security-0.1.8/mw_aiohttp_security/auth.py
-drwxrwxrwx   0        0        0        0 2021-07-08 08:28:28.000000 mw-aiohttp-security-0.1.8/mw_aiohttp_security.egg-info/
--rw-rw-rw-   0        0        0      919 2021-07-08 08:28:27.000000 mw-aiohttp-security-0.1.8/mw_aiohttp_security.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2021-07-08 08:28:27.000000 mw-aiohttp-security-0.1.8/mw_aiohttp_security.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-08 08:28:27.000000 mw-aiohttp-security-0.1.8/mw_aiohttp_security.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2021-07-08 08:28:27.000000 mw-aiohttp-security-0.1.8/mw_aiohttp_security.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2021-07-08 08:28:27.000000 mw-aiohttp-security-0.1.8/mw_aiohttp_security.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-07-08 08:28:28.000000 mw-aiohttp-security-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     2268 2021-07-08 08:28:05.000000 mw-aiohttp-security-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-07-14 09:41:38.000000 mw-aiohttp-security-0.1.9/
+-rw-rw-rw-   0        0        0      625 2021-07-14 09:41:27.000000 mw-aiohttp-security-0.1.9/CHANGES.txt
+-rw-rw-rw-   0        0        0     1100 2018-05-04 06:36:08.000000 mw-aiohttp-security-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       94 2018-10-30 09:57:57.000000 mw-aiohttp-security-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      919 2021-07-14 09:41:38.000000 mw-aiohttp-security-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2021-03-11 03:12:53.000000 mw-aiohttp-security-0.1.9/README.rst
+drwxrwxrwx   0        0        0        0 2021-07-14 09:41:38.000000 mw-aiohttp-security-0.1.9/mw_aiohttp_security/
+-rw-rw-rw-   0        0        0     5133 2021-07-14 09:34:06.000000 mw-aiohttp-security-0.1.9/mw_aiohttp_security/__init__.py
+-rw-rw-rw-   0        0        0     3561 2021-07-14 09:15:51.000000 mw-aiohttp-security-0.1.9/mw_aiohttp_security/auth.py
+drwxrwxrwx   0        0        0        0 2021-07-14 09:41:38.000000 mw-aiohttp-security-0.1.9/mw_aiohttp_security.egg-info/
+-rw-rw-rw-   0        0        0      919 2021-07-14 09:41:37.000000 mw-aiohttp-security-0.1.9/mw_aiohttp_security.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2021-07-14 09:41:37.000000 mw-aiohttp-security-0.1.9/mw_aiohttp_security.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-14 09:41:37.000000 mw-aiohttp-security-0.1.9/mw_aiohttp_security.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2021-07-14 09:41:37.000000 mw-aiohttp-security-0.1.9/mw_aiohttp_security.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2021-07-14 09:41:37.000000 mw-aiohttp-security-0.1.9/mw_aiohttp_security.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-07-14 09:41:38.000000 mw-aiohttp-security-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2268 2021-07-14 09:40:18.000000 mw-aiohttp-security-0.1.9/setup.py
```

### Comparing `mw-aiohttp-security-0.1.8/LICENSE.txt` & `mw-aiohttp-security-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mw-aiohttp-security-0.1.8/PKG-INFO` & `mw-aiohttp-security-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mw-aiohttp-security
-Version: 0.1.8
+Version: 0.1.9
 Summary: maxwin aiohttp security
 Home-page: https://bitbucket.org/maxwin-inc/mw-aiohttp-security/src
 Author: cxhjet
 Author-email: cxhjet@qq.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://bitbucket.org/maxwin-inc/auth/issues?status=new&status=open
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `mw-aiohttp-security-0.1.8/mw_aiohttp_security/__init__.py` & `mw-aiohttp-security-0.1.9/mw_aiohttp_security/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,17 +65,19 @@
             async def wrapped(*args, **kwargs):
                 request = args[-1]
                 if not isinstance(request, web.BaseRequest):
                     msg = ("Incorrect decorator usage. "
                            "Expecting `def handler(request)` "
                            "or `def handler(self, request)`.")
                     raise RuntimeError(msg)
-                await check_permission(request,
-                                       ','.join(subsystem) if isinstance(subsystem,list) else subsystem,
-                                       action)
+                # 只有登录用户的类型为appuser才需要检查权限，empuser和member跳过权限检查
+                if request['current_user'].type=='appuser':
+                    await check_permission(request,
+                                           ','.join(subsystem) if isinstance(subsystem,list) else subsystem,
+                                           action)
                 return await fn(*args, **kwargs)
             return wrapped
         assert isinstance(action, (str,list)),'action(%s) must be str'%action
         return wrapper
 
     async def check_permission(self,user_id, subsystem3 , action):
         '''
```

### Comparing `mw-aiohttp-security-0.1.8/mw_aiohttp_security/auth.py` & `mw-aiohttp-security-0.1.9/mw_aiohttp_security/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
         session = await get_session(request)
         # "uid": "2222", "uname": "dev", "systemuser": true, "manageuser": false, "manageuserid": null}
         current_user = User(user_id = session.get('uid'),
                             user_name = session.get('uname'),
                             systemuser=session.get('systemuser', False),
                             manageuser=session.get('manageuser', False),
                             manageuserid=session.get('manageuserid'),
-                            companyid=session.get('companyid'))
+                            companyid=session.get('companyid'),
+                            type=session.get('type','appuser'))
         request['current_user'] = current_user
         return session.get('uid')
 
     async def remember(self, request, response, identity, **kwargs):
         # 不提供登入
         pass
```

### Comparing `mw-aiohttp-security-0.1.8/mw_aiohttp_security.egg-info/PKG-INFO` & `mw-aiohttp-security-0.1.9/mw_aiohttp_security.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mw-aiohttp-security
-Version: 0.1.8
+Version: 0.1.9
 Summary: maxwin aiohttp security
 Home-page: https://bitbucket.org/maxwin-inc/mw-aiohttp-security/src
 Author: cxhjet
 Author-email: cxhjet@qq.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://bitbucket.org/maxwin-inc/auth/issues?status=new&status=open
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `mw-aiohttp-security-0.1.8/setup.py` & `mw-aiohttp-security-0.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Fields marked as "Optional" may be commented out.
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     # And where it will live on PyPI: https://pypi.org/project/mw-aiohttp-security/
     name='mw-aiohttp-security',  # Required
-    version='0.1.8',  # Required
+    version='0.1.9',  # Required
     description='maxwin aiohttp security',  # Required
     # long_description='\n\n'.join((read('README.rst'), read('CHANGES.txt'))),
     # long_description=long_description,  # Optional
     # long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://bitbucket.org/maxwin-inc/mw-aiohttp-security/src',  # Optional
     author='cxhjet',  # Optional
     author_email='cxhjet@qq.com',  # Optional
```

