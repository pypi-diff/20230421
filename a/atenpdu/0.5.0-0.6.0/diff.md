# Comparing `tmp/atenpdu-0.5.0.tar.gz` & `tmp/atenpdu-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atenpdu-0.5.0.tar", max compression
+gzip compressed data, was "atenpdu-0.6.0.tar", max compression
```

## Comparing `atenpdu-0.5.0.tar` & `atenpdu-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2022-12-19 14:13:25.197000 atenpdu-0.5.0/LICENSE
--rw-r--r--   0        0        0     1095 2022-12-19 15:24:35.982000 atenpdu-0.5.0/README.md
--rw-r--r--   0        0        0     6678 2023-01-12 22:01:55.678000 atenpdu-0.5.0/atenpdu/__init__.py
--rw-r--r--   0        0        0   102790 2022-12-19 15:04:28.586000 atenpdu-0.5.0/atenpdu/mibs/ATEN-PE-CFG.py
--rwxr-xr-x   0        0        0     6343 2022-12-19 15:16:22.450000 atenpdu-0.5.0/atenpdu/pductl.py
--rw-r--r--   0        0        0     1045 2023-01-18 00:15:23.528000 atenpdu-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1952 1970-01-01 00:00:00.000000 atenpdu-0.5.0/setup.py
--rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 atenpdu-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-12-19 14:13:25.197000 atenpdu-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1095 2022-12-19 15:24:35.982000 atenpdu-0.6.0/README.md
+-rw-r--r--   0        0        0     6672 2023-04-21 20:13:52.937060 atenpdu-0.6.0/atenpdu/__init__.py
+-rw-r--r--   0        0        0   102790 2022-12-19 15:04:28.586000 atenpdu-0.6.0/atenpdu/mibs/ATEN-PE-CFG.py
+-rwxr-xr-x   0        0        0     6343 2022-12-19 15:16:22.450000 atenpdu-0.6.0/atenpdu/pductl.py
+-rw-r--r--   0        0        0     1045 2023-04-21 20:15:13.975062 atenpdu-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1952 1970-01-01 00:00:00.000000 atenpdu-0.6.0/setup.py
+-rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 atenpdu-0.6.0/PKG-INFO
```

### Comparing `atenpdu-0.5.0/LICENSE` & `atenpdu-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atenpdu-0.5.0/README.md` & `atenpdu-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `atenpdu-0.5.0/atenpdu/__init__.py` & `atenpdu-0.6.0/atenpdu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         async with self._lock:
             for _ in range(3):
                 try:
                     async with async_timeout.timeout(3):
                         get_result = await getCmd(
                             *self._snmp_args, *[ObjectType(ObjectIdentity(self._MIB_MODULE, *obj)) for obj in objects]
                         )
-                        err_indication, err_status, _, varbind_table = await get_result
+                        err_indication, err_status, _, varbind_table = get_result
                 except asyncio.exceptions.TimeoutError:
                     pass
                 else:
                     break
             else:
                 raise AtenPEError("Timeout")
```

### Comparing `atenpdu-0.5.0/atenpdu/mibs/ATEN-PE-CFG.py` & `atenpdu-0.6.0/atenpdu/mibs/ATEN-PE-CFG.py`

 * *Files identical despite different names*

### Comparing `atenpdu-0.5.0/atenpdu/pductl.py` & `atenpdu-0.6.0/atenpdu/pductl.py`

 * *Files identical despite different names*

### Comparing `atenpdu-0.5.0/pyproject.toml` & `atenpdu-0.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 target-version = ['py38']
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "atenpdu"
-version = "0.5.0"
+version = "0.6.0"
 description = "Interface for ATEN-PE PDUs"
 authors = ["Andreas Oberritter <obi@saftware.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mtdcr/pductl"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -24,15 +24,15 @@
     "Topic :: System :: Systems Administration",
     "Topic :: Utilities"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 async-timeout = "^4.0.2"
-pysnmplib = "^5.0.20"
+pysnmplib = "^5.0.21"
 
 [tool.poetry.scripts]
 pductl = "atenpdu.pductl:run"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.4"
 mypy = "^0.991"
```

### Comparing `atenpdu-0.5.0/setup.py` & `atenpdu-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['atenpdu', 'atenpdu.mibs']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['async-timeout>=4.0.2,<5.0.0', 'pysnmplib>=5.0.20,<6.0.0']
+['async-timeout>=4.0.2,<5.0.0', 'pysnmplib>=5.0.21,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['pductl = atenpdu.pductl:run']}
 
 setup_kwargs = {
     'name': 'atenpdu',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'Interface for ATEN-PE PDUs',
     'long_description': '# pductl - Control outlets of ATEN PE PDUs\n\n## Installation\n\n```sh\npip install atenpdu\n```\n \n## Example configuration [~/.pductl]\n```json\n{\n  "format": 1,\n  "pdus": {\n    "pdu1": {\n      "node": "pdu1",\n      "service": "snmp",\n      "username": "administrator",\n      "authkey": "AAAAAAAAAAAAAA",\n      "privkey": "BBBBBBBBBBBBBB"\n    },\n    "pdu2": {\n      "authkey": "CCCCCCCCCCCCCC",\n      "privkey": "DDDDDDDDDDDDDD"\n    },\n    "pdu3": {\n      "node": "192.168.21.19",\n      "service": "16161",\n      "username": "joe",\n      "authkey": "EEEEEEEEEEEEEE",\n      "privkey": "FFFFFFFFFFFFFF"\n    },\n    "pdu4": {\n      "community": "private"\n    },\n    "pdu5": {\n    }\n  }\n}\n```\n\n* `authkey` and `privkey` are required for SNMPv3. On absence, SNMPv2c gets used.\n* `community` defaults to `private` for SNMPv2c.\n* `node` defaults to PDU entry\'s name.\n* `service` defaults to `snmp`, i.e. port 161.\n* `username` defaults to `administrator` for SNMPv3.\n\n## Usage\n\n```sh\npductl [-p <PDU>] list\npductl [-p <PDU>] <on|off|reboot|status> <OUTLET> [<OUTLET> ...]\n```\n\nUse `ALL` to select all outlets.\n',
     'author': 'Andreas Oberritter',
     'author_email': 'obi@saftware.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mtdcr/pductl',
```

### Comparing `atenpdu-0.5.0/PKG-INFO` & `atenpdu-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atenpdu
-Version: 0.5.0
+Version: 0.6.0
 Summary: Interface for ATEN-PE PDUs
 Home-page: https://github.com/mtdcr/pductl
 License: MIT
 Author: Andreas Oberritter
 Author-email: obi@saftware.de
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Dist: async-timeout (>=4.0.2,<5.0.0)
-Requires-Dist: pysnmplib (>=5.0.20,<6.0.0)
+Requires-Dist: pysnmplib (>=5.0.21,<6.0.0)
 Project-URL: Repository, https://github.com/mtdcr/pductl
 Description-Content-Type: text/markdown
 
 # pductl - Control outlets of ATEN PE PDUs
 
 ## Installation
```

