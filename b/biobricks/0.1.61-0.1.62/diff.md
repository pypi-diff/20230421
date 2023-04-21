# Comparing `tmp/biobricks-0.1.61.tar.gz` & `tmp/biobricks-0.1.62.tar.gz`

## Comparing `biobricks-0.1.61.tar` & `biobricks-0.1.62.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks.svg
--rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 biobricks-0.1.61/coverage.xml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 biobricks-0.1.61/requirements.txt
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 biobricks-0.1.61/.github/workflows/biobricks.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.61/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.61/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.61/.pytest_cache/README.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.61/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 biobricks-0.1.61/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.61/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 biobricks-0.1.61/.vscode/tasks.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/api.py
--rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/brick.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/checks.py
--rwxr-xr-x   0        0        0     4653 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/cli.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/config.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/local_bb.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/.pytest_cache/README.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/test_init.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 biobricks-0.1.61/docker/Dockerfile
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.61/docker/test.sh
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 biobricks-0.1.61/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 biobricks-0.1.61/LICENSE
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 biobricks-0.1.61/README.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 biobricks-0.1.61/pyproject.toml
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 biobricks-0.1.61/PKG-INFO
+-rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks.svg
+-rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 biobricks-0.1.62/coverage.xml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 biobricks-0.1.62/requirements.txt
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 biobricks-0.1.62/.github/workflows/biobricks.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.62/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.62/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.62/.pytest_cache/README.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.62/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 biobricks-0.1.62/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.62/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 biobricks-0.1.62/.vscode/tasks.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/__init__.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/api.py
+-rw-r--r--   0        0        0     7701 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/brick.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/checks.py
+-rwxr-xr-x   0        0        0     4653 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/cli.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/config.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/local_bb.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/.pytest_cache/README.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/test_init.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 biobricks-0.1.62/docker/Dockerfile
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.62/docker/test.sh
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 biobricks-0.1.62/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 biobricks-0.1.62/LICENSE
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 biobricks-0.1.62/README.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 biobricks-0.1.62/pyproject.toml
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 biobricks-0.1.62/PKG-INFO
```

### Comparing `biobricks-0.1.61/biobricks.svg` & `biobricks-0.1.62/biobricks.svg`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.61/coverage.xml` & `biobricks-0.1.62/coverage.xml`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.61/.github/workflows/biobricks.yml` & `biobricks-0.1.62/.github/workflows/biobricks.yml`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.61/biobricks/api.py` & `biobricks-0.1.62/biobricks/api.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.61/biobricks/brick.py` & `biobricks-0.1.62/biobricks/brick.py`

 * *Files 5% similar despite different names*

```diff
@@ -157,39 +157,21 @@
     
     def load(self):
         "load this brick"
         bdir = self.path()
         if not bdir.exists(): 
             raise Exception(f"no path '{bdir}' try `biobricks install {self.url()}`")
         
-        def dirns(dir: Path):
-            filter = lambda d: d.name.endswith('.parquet')
-            paths = [d for d in dir.rglob('*') if filter(d)]
-            namespace = types.SimpleNamespace()
-            pkey = lambda p: re.sub(r'[.-]','_',p)
-            for p in paths:
-                path = p.relative_to(dir)
-                logger.info(f"loading {path}...")
-                current = namespace
-                for part in path.parts:
-                    key = pkey(part)
-                    if not hasattr(current, key) and part.endswith('.parquet'):
-                        setattr(current, key[:-8], pq.ParquetDataset(str(p)))
-                    elif not hasattr(current, key):
-                        setattr(current, key, types.SimpleNamespace())
-                        current = getattr(current, key)
-                    elif hasattr(current, key):
-                        current = getattr(current, key)
-            logger.info(f"loaded {len(paths)} tables from {dir}")
-            return namespace
-
-        ns1 = dirns(bdir / 'data')
-        ns2 = dirns(bdir / 'brick')
-        result = {**ns2.__dict__, **ns1.__dict__}
-        return types.SimpleNamespace(**result)
+        # get assets and strip .parquet from assets to make names
+        assets = [Path(p) for p in self.assets()]
+        names = [p.with_suffix('').name for p in assets]
+        
+        # make a simple namespace using names as keys and loading assets with pq.ParquetDataset
+        ds = [pq.ParquetDataset(str(p)) for p in assets]
+        return types.SimpleNamespace(**dict(zip(names, ds)))
     
     def assets(self):
         "get the assets for this brick"
         bdir = self.path()
         if not bdir.exists(): 
             raise Exception(f"no path '{bdir}' try `biobricks install {self.url()}`")
```

### Comparing `biobricks-0.1.61/biobricks/checks.py` & `biobricks-0.1.62/biobricks/checks.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.61/biobricks/cli.py` & `biobricks-0.1.62/biobricks/cli.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.61/biobricks/config.py` & `biobricks-0.1.62/biobricks/config.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.61/biobricks/local_bb.py` & `biobricks-0.1.62/biobricks/local_bb.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.61/biobricks/tests/test_init.py` & `biobricks-0.1.62/biobricks/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.61/docker/Dockerfile` & `biobricks-0.1.62/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.61/LICENSE` & `biobricks-0.1.62/LICENSE`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.61/README.md` & `biobricks-0.1.62/README.md`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.61/pyproject.toml` & `biobricks-0.1.62/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "biobricks"
-version = "0.1.61"
+version = "0.1.62"
 authors = [
   { name="Jose A. Jaramillo", email="jjv@utp.edu.co" },
   { name="Thomas Luechtefeld", email="tom@insilica.co" }
 ]
 description = "Biobricks automates bioinformatics data."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `biobricks-0.1.61/PKG-INFO` & `biobricks-0.1.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobricks
-Version: 0.1.61
+Version: 0.1.62
 Summary: Biobricks automates bioinformatics data.
 Project-URL: Homepage, https://github.com/biobricks-ai/biobricks
 Project-URL: Bug Tracker, https://github.com/biobricks-ai/biobricks/issues
 Author-email: "Jose A. Jaramillo" <jjv@utp.edu.co>, Thomas Luechtefeld <tom@insilica.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

