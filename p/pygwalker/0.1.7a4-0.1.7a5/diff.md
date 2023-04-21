# Comparing `tmp/pygwalker-0.1.7a4.tar.gz` & `tmp/pygwalker-0.1.7a5.tar.gz`

## Comparing `pygwalker-0.1.7a4.tar` & `pygwalker-0.1.7a5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/.gitignore
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/index.html
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/package.json
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/tsconfig.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/vite.config.ts
--rw-r--r--   0        0        0   124304 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/yarn.lock
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/src/index.tsx
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/src/components/options.tsx
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/src/interfaces/index.ts
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/__init__.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/__main__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/__version__.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/base.py
--rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/gwalker.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/templates/.gitignore
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/templates/index.html
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/templates/walk.js
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/templates/dist/index.d.ts
--rw-r--r--   0        0        0  1765339 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/templates/dist/pygwalker-app.iife.js
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/templates/dist/components/options.d.ts
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/templates/dist/interfaces/index.d.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/utils/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/utils/check_update.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/utils/config.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/utils/defaults.json
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/utils/fname_encodings.py
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/utils/gwalker_props.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/utils/render.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/scripts/__init__.py
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/scripts/compile.sh
--rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/scripts/develop.sh
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/scripts/test-init.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/scripts/test-init.sh
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/.gitignore
--rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/LICENSE
--rw-r--r--   0        0        0    12861 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/README.md
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pyproject.toml
--rw-r--r--   0        0        0    14004 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/app/.gitignore
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/app/index.html
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/app/package.json
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/app/tsconfig.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/app/vite.config.ts
+-rw-r--r--   0        0        0   124304 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/app/yarn.lock
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/app/src/index.tsx
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/app/src/components/options.tsx
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/app/src/interfaces/index.ts
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/__init__.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/__main__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/__version__.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/base.py
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/gwalker.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/templates/.gitignore
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/templates/index.html
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/templates/walk.js
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/templates/dist/index.d.ts
+-rw-r--r--   0        0        0  1765339 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/templates/dist/pygwalker-app.iife.js
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/templates/dist/components/options.d.ts
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/templates/dist/interfaces/index.d.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/utils/__init__.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/utils/check_update.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/utils/config.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/utils/defaults.json
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/utils/fname_encodings.py
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/utils/gwalker_props.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pygwalker/utils/render.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/scripts/__init__.py
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/scripts/compile.sh
+-rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/scripts/develop.sh
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/scripts/test-init.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/scripts/test-init.sh
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/.gitignore
+-rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/LICENSE
+-rw-r--r--   0        0        0    12861 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/README.md
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/pyproject.toml
+-rw-r--r--   0        0        0    14004 2020-02-02 00:00:00.000000 pygwalker-0.1.7a5/PKG-INFO
```

### Comparing `pygwalker-0.1.7a4/app/package.json` & `pygwalker-0.1.7a5/app/package.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/app/tsconfig.json` & `pygwalker-0.1.7a5/app/tsconfig.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/app/vite.config.ts` & `pygwalker-0.1.7a5/app/vite.config.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/app/yarn.lock` & `pygwalker-0.1.7a5/app/yarn.lock`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/app/src/index.tsx` & `pygwalker-0.1.7a5/app/src/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/app/src/components/options.tsx` & `pygwalker-0.1.7a5/app/src/components/options.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/pygwalker/__init__.py` & `pygwalker-0.1.7a5/pygwalker/__init__.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/pygwalker/__main__.py` & `pygwalker-0.1.7a5/pygwalker/__main__.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/pygwalker/base.py` & `pygwalker-0.1.7a5/pygwalker/base.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/pygwalker/gwalker.py` & `pygwalker-0.1.7a5/pygwalker/gwalker.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/pygwalker/templates/walk.js` & `pygwalker-0.1.7a5/pygwalker/templates/walk.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/pygwalker/templates/dist/pygwalker-app.iife.js` & `pygwalker-0.1.7a5/pygwalker/templates/dist/pygwalker-app.iife.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/pygwalker/utils/check_update.py` & `pygwalker-0.1.7a5/pygwalker/utils/check_update.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 from .. import base
 __update_url__ = 'https://5agko11g7e.execute-api.us-west-1.amazonaws.com/default/check_updates'
 
 async def check_update_async():
+    import logging
     payload = {'pkg': 'pygwalker', 'v': base.__version__, 'hashcode': base.__hash__}
     try:
         resp = {}
         if "pyodide" in sys.modules:
             import pyodide
             payload['pkg'] = 'pygwalker-pyodide'
             params = '&'.join([f"{k}={v}" for k, v in payload.items()])
@@ -18,17 +19,20 @@
             async with aiohttp.ClientSession() as session:
                 resp = await session.get(f"{__update_url__}?{params}")
                 resp = await resp.json()
         if resp['data']['outdated'] == True:
             import logging
             release = resp['data']['latest']['release']
             # logging.info(f"[pygwalker]: A new release {release} available.")
+        return resp
     except:
-        pass
+        import traceback
+        logging.warn(traceback.format_exc())
 
 def check_update():
     import asyncio
     try:
         main_loop = asyncio.get_running_loop()
+        main_loop.create_task(check_update_async())
     except:
         main_loop = asyncio.new_event_loop()
-    main_loop.run_until_complete(check_update_async())
+        main_loop.run_until_complete(check_update_async())
```

### Comparing `pygwalker-0.1.7a4/pygwalker/utils/config.py` & `pygwalker-0.1.7a5/pygwalker/utils/config.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/pygwalker/utils/gwalker_props.py` & `pygwalker-0.1.7a5/pygwalker/utils/gwalker_props.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/pygwalker/utils/render.py` & `pygwalker-0.1.7a5/pygwalker/utils/render.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/scripts/test-init.py` & `pygwalker-0.1.7a5/scripts/test-init.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/scripts/test-init.sh` & `pygwalker-0.1.7a5/scripts/test-init.sh`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/.gitignore` & `pygwalker-0.1.7a5/.gitignore`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/LICENSE` & `pygwalker-0.1.7a5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/README.md` & `pygwalker-0.1.7a5/README.md`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/pyproject.toml` & `pygwalker-0.1.7a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a4/PKG-INFO` & `pygwalker-0.1.7a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygwalker
-Version: 0.1.7a4
+Version: 0.1.7a5
 Summary: pygwalker: Combining Jupyter Notebook with a Tableau-like UI
 Project-URL: homepage, https://github.com/Kanaries/pygwalker
 Project-URL: repository, https://github.com/Kanaries/pygwalker
 Author-email: "Asm.Def" <woojson@zju.edu.cn>
 License-File: LICENSE
 Keywords: data-analysis,data-exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygwalker Version: 0.1.7a4 Summary: pygwalker:
+Metadata-Version: 2.1 Name: pygwalker Version: 0.1.7a5 Summary: pygwalker:
 Combining Jupyter Notebook with a Tableau-like UI Project-URL: homepage, https:
 //github.com/Kanaries/pygwalker Project-URL: repository, https://github.com/
 Kanaries/pygwalker Author-email: "Asm.Def"
 zju.edu.cn> License-File: LICENSE Keywords: data-analysis,data-
 exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.6 Requires-Dist:
```

