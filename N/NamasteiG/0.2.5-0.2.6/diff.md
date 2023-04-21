# Comparing `tmp/NamasteiG-0.2.5.tar.gz` & `tmp/NamasteiG-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NamasteiG-0.2.5.tar", last modified: Tue Apr 18 03:00:11 2023, max compression
+gzip compressed data, was "NamasteiG-0.2.6.tar", last modified: Fri Apr 21 14:15:13 2023, max compression
```

## Comparing `NamasteiG-0.2.5.tar` & `NamasteiG-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 03:00:11.388181 NamasteiG-0.2.5/
--rw-rw-rw-   0        0        0     1077 2022-12-10 14:24:59.000000 NamasteiG-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      838 2023-04-18 03:00:11.388181 NamasteiG-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      326 2022-12-14 19:04:09.000000 NamasteiG-0.2.5/README.md
--rw-rw-rw-   0        0        0      593 2023-04-18 02:58:50.000000 NamasteiG-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 03:00:11.388181 NamasteiG-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 03:00:11.372567 NamasteiG-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 03:00:11.372567 NamasteiG-0.2.5/src/NamasteiG/
--rw-rw-rw-   0        0        0    19940 2023-04-18 02:58:38.000000 NamasteiG-0.2.5/src/NamasteiG/__init__.py
--rw-rw-rw-   0        0        0      499 2022-12-14 18:59:48.000000 NamasteiG-0.2.5/src/NamasteiG/example.py
-drwxrwxrwx   0        0        0        0 2023-04-18 03:00:11.388181 NamasteiG-0.2.5/src/NamasteiG.egg-info/
--rw-rw-rw-   0        0        0      838 2023-04-18 03:00:11.000000 NamasteiG-0.2.5/src/NamasteiG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-04-18 03:00:11.000000 NamasteiG-0.2.5/src/NamasteiG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 03:00:11.000000 NamasteiG-0.2.5/src/NamasteiG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-18 03:00:11.000000 NamasteiG-0.2.5/src/NamasteiG.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 14:15:13.330563 NamasteiG-0.2.6/
+-rw-rw-rw-   0        0        0     1077 2022-12-10 14:24:59.000000 NamasteiG-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      838 2023-04-21 14:15:13.330563 NamasteiG-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2022-12-14 19:04:09.000000 NamasteiG-0.2.6/README.md
+-rw-rw-rw-   0        0        0      593 2023-04-21 14:10:11.000000 NamasteiG-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:15:13.332038 NamasteiG-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 14:15:13.317646 NamasteiG-0.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 14:15:13.325092 NamasteiG-0.2.6/src/NamasteiG/
+-rw-rw-rw-   0        0        0     8405 2023-04-16 13:01:55.000000 NamasteiG-0.2.6/src/NamasteiG/VerifyData.py
+-rw-rw-rw-   0        0        0    27820 2023-04-21 14:14:36.000000 NamasteiG-0.2.6/src/NamasteiG/__init__.py
+-rw-rw-rw-   0        0        0      501 2023-04-21 14:14:22.000000 NamasteiG-0.2.6/src/NamasteiG/example.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:15:13.329144 NamasteiG-0.2.6/src/NamasteiG.egg-info/
+-rw-rw-rw-   0        0        0      838 2023-04-21 14:15:13.000000 NamasteiG-0.2.6/src/NamasteiG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-21 14:15:13.000000 NamasteiG-0.2.6/src/NamasteiG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:15:13.000000 NamasteiG-0.2.6/src/NamasteiG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 14:15:13.000000 NamasteiG-0.2.6/src/NamasteiG.egg-info/top_level.txt
```

### Comparing `NamasteiG-0.2.5/LICENSE` & `NamasteiG-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `NamasteiG-0.2.5/PKG-INFO` & `NamasteiG-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NamasteiG
-Version: 0.2.5
+Version: 0.2.6
 Summary: Most PowerFull Instagram Library
 Author-email: Abhinav Bhardwaj <abhinav.bhardwaj.56614@gmail.com>
 Project-URL: Homepage, https://t.me/namastelibrary
 Project-URL: Bug Tracker, https://t.me/namastehackers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NamasteiG-0.2.5/pyproject.toml` & `NamasteiG-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NamasteiG"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Abhinav Bhardwaj", email="abhinav.bhardwaj.56614@gmail.com" },
 ]
 description = "Most PowerFull Instagram Library"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `NamasteiG-0.2.5/src/NamasteiG/__init__.py` & `NamasteiG-0.2.6/src/NamasteiG/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import uuid
 import string
-import requests
 import random
 import secrets
+import requests
 import time
+from VerifyData import IG_Verify
 from urllib.parse   import urlencode
-import base64
 from Cryptodome.Cipher import AES, PKCS1_v1_5
 from Cryptodome.PublicKey import RSA
 from Cryptodome.Random import get_random_bytes
+import base64
+
+
+
 
 value=[]
 value1=[]
 
 def password_encrypt(password):
     resp = requests.get('https://i.instagram.com/api/v1/qe/sync/')
     publickeyid = int(resp.headers.get('ig-set-password-encryption-key-id'))
@@ -39,24 +43,27 @@
     ]))
     return f'#PWD_INSTAGRAM:4:{timestamp}:{payload.decode()}'
 
 
 
 class Instagram:
 
-    def __init__(self,User,Password):
-        self.user = User
+    def __init__(self,User,Password,Proxy=None):
+        self.UserName = User
         self.passw=Password
         self.PigeonSession = f'UFS-{str(uuid.uuid4())}-0'
         self.IgDeviceId = uuid.uuid4()
         self.IgFamilyDeviceId = uuid.uuid4()
         self.AndroidID = f'android-{secrets.token_hex(8)}'
+        self.Waterfall= uuid.uuid4()
+        self.Qpl=uuid.uuid4()
         rnd=str(random.randint(150, 999))
         self.UserAgent = "Instagram 278.0.0.21.117 Android (" + ["23/6.0", "24/7.0", "25/7.1.1", "26/8.0", "27/8.1", "28/9.0"][random.randint(0, 5)] + "; " + str(random.randint(100, 1300)) + "dpi; " + str(random.randint(200, 2000)) + "x" + str(random.randint(200, 2000)) + "; " + ["SAMSUNG", "HUAWEI", "LGE/lge", "HTC", "ASUS", "ZTE", "ONEPLUS", "XIAOMI", "OPPO", "VIVO", "SONY", "REALME"][random.randint(0, 11)] + "; SM-T" + rnd + "; SM-T" + rnd + "; qcom; en_US; 464315254)"
         self.Blockversion = '329007815be126bc02ffebcd41f0e4f8d889d871c12ca57fe5cbc3ece5196505'
+        self.proxy = Proxy
 
     def generate_jazoest(self,symbols):
         amount = sum(ord(s) for s in symbols)
         return f'2{amount}'
 
     def GetMid(self):
         data = urlencode({
@@ -119,15 +126,15 @@
         if PassWordEnc==None:
             self.datapassword=f'#PWD_INSTAGRAM:0:{round(time.time())}:{self.passw}'
         else:
             self.datapassword = f'{password_encrypt(self.passw)}'
         data = urlencode({
             'signed_body': 'SIGNATURE.{"jazoest":"' + str(self.generate_jazoest(
                 str(self.IgFamilyDeviceId))) + '","country_codes":"[{\\"country_code\\":\\"91\\",\\"source\\":[\\"sim\\"]},{\\"country_code\\":\\"1\\",\\"source\\":[\\"default\\"]}]","phone_id":"' + str(
-                self.IgFamilyDeviceId) + '","enc_password":"'+str(self.datapassword) + '","username":"' + str(self.user) + '","adid":"' + str(uuid.uuid4()) + '","guid":"' + str(
+                self.IgFamilyDeviceId) + '","enc_password":"'+str(self.datapassword) + '","username":"' + str(self.UserName) + '","adid":"' + str(uuid.uuid4()) + '","guid":"' + str(
                 self.IgDeviceId) + '","device_id":"' + str(
                 self.AndroidID) + '","google_tokens":"[]","login_attempt_count":"0"}',
         })
         headers = {
             'Host': 'i.instagram.com',
             'X-Ig-App-Locale': 'en_US',
             'X-Ig-Device-Locale': 'en_US',
@@ -218,14 +225,165 @@
                 "IgFamilyDeviceId": self.IgFamilyDeviceId,
                 "AndroidID": self.AndroidID,
                 'UserAgent': self.UserAgent,
                 'BlockVersion': self.Blockversion
             }
 
         return value
+
+
+
+    def LoginV2(self,PassWordEnc=None):
+            try:
+
+
+                if PassWordEnc==None:
+                    self.datapassword=f'#PWD_INSTAGRAM:0:{round(time.time())}:{self.passw}'
+                else:
+                    self.datapassword = f'{IG_Verify.Enc_Passwd(self)}'
+
+                self.headers,self.mid,self.instance_id,self.marker_id,self.emlogin,self.pwlogin=IG_Verify.Dual_tokens(self)
+
+                del self.headers['X-Tigon-Is-Retry']
+                del self.headers['Connection']
+
+
+
+                data = urlencode({
+                    'params': '{"client_input_params":{"contact_point":"'+str(self.UserName)+'","password":"'+str(self.datapassword)+'","fb_ig_device_id":[],"event_flow":"login_manual","openid_tokens":{},"machine_id":"'+str(self.mid)+'","family_device_id":"'+str(self.IgFamilyDeviceId)+'","accounts_list":[],"try_num":1,"login_attempt_count":1,"device_id":"'+str(self.AndroidID)+'","auth_secure_device_id":"","device_emails":["'+str(self.UserName)+'@gmail.com"],"secure_family_device_id":"","event_step":"home_page"},"server_params":{"is_platform_login":0,"qe_device_id":"'+str(self.IgDeviceId)+'","family_device_id":"'+str(self.IgFamilyDeviceId)+'","credential_type":"password","waterfall_id":"'+str(self.Waterfall)+'","username_text_input_id":"'+str(self.emlogin)+'","password_text_input_id":"'+str(self.pwlogin)+'","offline_experiment_group":"caa_iteration_v3_perf_ig_4","INTERNAL__latency_qpl_instance_id":'+str(self.instance_id)+',"INTERNAL_INFRA_THEME":"default","device_id":"'+str(self.AndroidID)+'","server_login_source":"login","login_source":"Login","ar_event_source":"login_home_page","INTERNAL__latency_qpl_marker_id":'+str(self.marker_id)+'}}',
+                    'bk_client_context': '{"bloks_version":"'+str(self.Blockversion)+'","styles_id":"instagram"}',
+                    'bloks_versioning_id': str(self.Blockversion),
+                })
+
+                updict = {
+                    "Content-Length": str(len(data)),
+                    'X-Pigeon-Rawclienttime': str(round(time.time(), 3)),
+
+                }
+                self.headers = {key: updict.get(key, self.headers[key]) for key in self.headers}
+
+
+                response = requests.post(
+                    'https://i.instagram.com/api/v1/bloks/apps/com.bloks.www.bloks.caa.login.async.send_login_request/',
+                    headers=self.headers,
+                    data=data,
+                    proxies=self.proxy
+                )
+                if 'Incorrect Password: The password you entered is incorrect. Please try again.' in response.text:
+                    value = {
+                        "Response": 'Incorrect Password: The password you entered is incorrect. Please try again.',
+                    }
+                elif 'Please wait a few minutes before you try again.' in response.text:
+                    value = {
+                        "Response": 'Please wait a few minutes before you try again.',
+                    }
+
+                elif f". Try another phone number or email, or if you don't have an Instagram account, you can sign up." in response.text:
+
+                    value = {
+                        "Response": f"We can't find an account with {self.UserName}. Try another phone number or email, or if you don't have an Instagram account, you can sign up.",
+                    }
+
+                elif f"Login Error: An unexpected error occurred. Please try logging in again." in response.text:
+
+                    value = {
+                        "Response": f"Login Error: An unexpected error occurred. Please try logging in again.",
+                    }
+                elif 'Bearer IGT:2:' in  response.text:
+
+
+                    self.bearer=response.text.split(r'\\\\\\\", \\\\\\\"IG-Set-Password-Encryption-Key-Id\\\\\\\": \\\\\\\"')[0].split('"Bearer IGT:2:')[1]
+                    self.csrf = response.text.split(r'csrftoken=')[1].split('; Domain=.instagram.com; expires=')[0]
+                    self.rur = response.text.split(r'\\\\\\\", \\\\\\\"Cross-Origin-Embedder-Policy-Report-Only')[0].split(r'"ig-set-ig-u-rur\\\\\\\": \\\\\\\"')[1]
+                    self.UserId = response.text.split(r', \\\\\\\"ig-set-ig-u-rur\\\\\\\"')[0].split(r'"ig-set-ig-u-ds-user-id\\\\\\\": ')[1]
+
+                    self.xclaim,self.shbid,self.shbts,self.urur=IG_Verify.Dual_tokens2(self)
+
+                    # value = {
+                    #     "Response": 'Login Success',
+                    #     "Mid": self.mid,
+                    #     'PigeonSession': self.PigeonSession,
+                    #     "IgDeviceId": self.IgDeviceId,
+                    #     "IgFamilyDeviceId": self.IgFamilyDeviceId,
+                    #     "AndroidID": self.AndroidID,
+                    #     'UserAgent': self.UserAgent,
+                    #     'BlockVersion': self.Blockversion,
+                    #     'igrur': self.rur,
+                    #     'Xclaim': self.xclaim,
+                    #     'UserId':self.UserId,
+                    #     'BearerToken': self.bearer,
+                    #     'Csrf': self.csrf,
+                    #     'shbid':self.shbid,
+                    #     'shbts':self.shbts,
+                    #     'urur':self.urur,
+                    #     'igid':self.igid
+                    # }
+                    self.userid = self.urur.split(',')[1]
+                    self.igrur = self.urur.split(':')[1]
+                    self.igid = self.shbid.split(',')[0]
+
+                    value = {
+                        "Response": 'Login Success',
+                        "Mid": self.mid,
+                        'PigeonSession': self.PigeonSession,
+                        "IgDeviceId": self.IgDeviceId,
+                        "IgFamilyDeviceId": self.IgFamilyDeviceId,
+                        "AndroidID": self.AndroidID,
+                        'UserAgent': self.UserAgent,
+                        'BlockVersion': self.Blockversion,
+                        'igrur': self.igrur,
+                        'Xclaim': self.xclaim,
+                        'BearerToken': self.bearer,
+                        'igid': self.igid,
+                        'UserId':self.userid
+                    }
+                    self.sessionid=self.bearer
+                    print(value)
+
+
+                    return value
+
+
+                elif 'challenge_required' in response.text:
+                    value = {
+                        "Response": 'Challenge_Required',
+                    }
+
+
+
+                elif 'checkpoint_challenge_required' in response.text:
+
+                    value = {
+                        "Response": 'Checkpoint_Challenge_Required',
+                    }
+
+
+                elif 'checkpoint_required' in response.text:
+                    value = {
+                        "Response": 'checkpoint_required',
+                    }
+
+                else:
+                    value = {
+                        "Response": response.json(),
+                    }
+                print(value)
+                value = {
+                    "Response": value['Response'],
+                    "Mid": self.mid,
+                    'PigeonSession': self.PigeonSession,
+                    "IgDeviceId": self.IgDeviceId,
+                    "IgFamilyDeviceId": self.IgFamilyDeviceId,
+                    "AndroidID": self.AndroidID,
+                    'UserAgent': self.UserAgent,
+                    'BlockVersion': self.Blockversion
+                }
+                return value
+            except Exception as E:
+                print(E)
     def head(self):
 
 
         headers = {
             'Host': 'i.instagram.com',
             'X-Ig-App-Locale': 'en_US',
             'X-Ig-Device-Locale': 'en_US',
@@ -414,15 +572,18 @@
             )
             return response.text
 
         except Exception as E:
             print(E)
 
 
-#
+
+
+
+
 # if __name__ == '__main__':
 #     ig=Instagram('','')
-#     ig.Login(1)
+#     ig.LoginV2(1)
 #     print(ig.Scrape_Followers(''))
```

### Comparing `NamasteiG-0.2.5/src/NamasteiG.egg-info/PKG-INFO` & `NamasteiG-0.2.6/src/NamasteiG.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NamasteiG
-Version: 0.2.5
+Version: 0.2.6
 Summary: Most PowerFull Instagram Library
 Author-email: Abhinav Bhardwaj <abhinav.bhardwaj.56614@gmail.com>
 Project-URL: Homepage, https://t.me/namastelibrary
 Project-URL: Bug Tracker, https://t.me/namastehackers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

