# Comparing `tmp/issue_db_api-0.3.1.tar.gz` & `tmp/issue_db_api-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.3.1.tar", last modified: Thu Apr 20 11:28:02 2023, max compression
+gzip compressed data, was "issue_db_api-0.4.0.tar", last modified: Thu Apr 20 12:05:28 2023, max compression
```

## Comparing `issue_db_api-0.3.1.tar` & `issue_db_api-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 11:28:02.807672 issue_db_api-0.3.1/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.3.1/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-20 11:28:02.807672 issue_db_api-0.3.1/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 11:28:02.803672 issue_db_api-0.3.1/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      469 2023-04-20 10:15:51.000000 issue_db_api-0.3.1/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.3.1/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     7773 2023-04-20 11:26:15.000000 issue_db_api-0.3.1/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 11:28:02.807672 issue_db_api-0.3.1/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    41427 2023-04-20 09:17:20.000000 issue_db_api-0.3.1/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3767 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    35234 2023-04-20 10:11:50.000000 issue_db_api-0.3.1/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-20 10:10:15.000000 issue_db_api-0.3.1/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3710 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5660 2023-04-20 09:58:42.000000 issue_db_api-0.3.1/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 11:28:02.807672 issue_db_api-0.3.1/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 11:28:02.803672 issue_db_api-0.3.1/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-20 11:28:02.000000 issue_db_api-0.3.1/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-04-20 11:28:02.000000 issue_db_api-0.3.1/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 11:28:02.000000 issue_db_api-0.3.1/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.3.1/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-04-20 11:28:02.000000 issue_db_api-0.3.1/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-04-20 11:27:26.000000 issue_db_api-0.3.1/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-04-20 11:28:02.807672 issue_db_api-0.3.1/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.3.1/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 12:05:28.137680 issue_db_api-0.4.0/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.4.0/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.4.0/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.4.0/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-20 12:05:28.137680 issue_db_api-0.4.0/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.4.0/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 12:05:28.133680 issue_db_api-0.4.0/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      469 2023-04-20 12:05:16.000000 issue_db_api-0.4.0/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.4.0/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     7843 2023-04-20 12:01:48.000000 issue_db_api-0.4.0/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 12:05:28.137680 issue_db_api-0.4.0/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    41427 2023-04-20 09:17:20.000000 issue_db_api-0.4.0/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.4.0/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.4.0/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3773 2023-04-20 11:59:24.000000 issue_db_api-0.4.0/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.4.0/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.4.0/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.4.0/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    35430 2023-04-20 12:01:48.000000 issue_db_api-0.4.0/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-20 10:10:15.000000 issue_db_api-0.4.0/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3710 2023-04-20 08:15:34.000000 issue_db_api-0.4.0/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5906 2023-04-20 12:00:30.000000 issue_db_api-0.4.0/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 12:05:28.137680 issue_db_api-0.4.0/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.4.0/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.4.0/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.4.0/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-20 08:15:34.000000 issue_db_api-0.4.0/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-20 12:05:28.133680 issue_db_api-0.4.0/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-20 12:05:28.000000 issue_db_api-0.4.0/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-04-20 12:05:28.000000 issue_db_api-0.4.0/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 12:05:28.000000 issue_db_api-0.4.0/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.4.0/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-04-20 12:05:28.000000 issue_db_api-0.4.0/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-04-20 12:05:16.000000 issue_db_api-0.4.0/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-04-20 12:05:28.137680 issue_db_api-0.4.0/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.4.0/setup.py
```

### Comparing `issue_db_api-0.3.1/LICENSE` & `issue_db_api-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.3.1/PKG-INFO` & `issue_db_api-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.3.1
+Version: 0.4.0
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.3.1/issue_db_api/issue_api.pyi` & `issue_db_api-0.4.0/issue_db_api/issue_api.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,17 @@
     def add_new_tag(self, name: str, description: str):
         ...
 
     @property
     def embeddings(self) -> list[Embedding]:
         ...
 
+    def get_embedding_by_id(self, id: str) -> Embedding:
+        ...
+
     def create_embedding(self, name: str, config: dict[str, typing.Any]) -> Embedding:
         ...
 
     def find_issues_by_key(self, *args: tuple[str, str]) -> list[Issue]:
         ...
 
     @property
```

### Comparing `issue_db_api-0.3.1/issue_db_api/src/api_core.rs` & `issue_db_api-0.4.0/issue_db_api/src/api_core.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.3.1/issue_db_api/src/comments.rs` & `issue_db_api-0.4.0/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.3.1/issue_db_api/src/config.rs` & `issue_db_api-0.4.0/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.3.1/issue_db_api/src/embedding.rs` & `issue_db_api-0.4.0/issue_db_api/src/embedding.rs`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,16 @@
                       name: String,
                       config: HashMap<String, Value>,
                       has_file: bool,
                       update_policy: ConfigHandlingPolicy) -> Self {
         Embedding{api, id, name, config, has_file, update_policy}
     }
 
-    pub fn identifier(&self) -> &String {
-        &self.id
+    pub fn identifier(&self) -> String {
+        self.id.clone()
     }
 
     pub fn name(&self) -> APIResult<String> {
         match self.update_policy {
             ConfigHandlingPolicy::ReadFetchWriteWithFetch => {
                 let name = self.api.get_embedding(self.id.clone())?.name;
                 Ok(name)
```

### Comparing `issue_db_api-0.3.1/issue_db_api/src/errors.rs` & `issue_db_api-0.4.0/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.3.1/issue_db_api/src/issues.rs` & `issue_db_api-0.4.0/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.3.1/issue_db_api/src/labels.rs` & `issue_db_api-0.4.0/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.3.1/issue_db_api/src/lib.rs` & `issue_db_api-0.4.0/issue_db_api/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,19 @@
             let embeddings = api2py_error(self.repo.embeddings())?
                 .into_iter()
                 .map(|e| PyEmbedding{inner: e})
                 .collect();
             Ok(embeddings)
         }
 
+        fn get_embedding_by_id(&self, id: String) -> PyResult<PyEmbedding> {
+            let e = PyEmbedding{inner: api2py_error(self.repo.get_embedding_by_id(id))?};
+            Ok(e)
+        }
+
         fn create_embedding(&self, name: String, config: &PyAny) -> PyResult<PyEmbedding> {
             let json = py_to_json(config)?;
             if let Value::Object(c) = json {
                 let config = c.into_iter().collect();
                 Ok(PyEmbedding{inner: api2py_error(self.repo.create_embedding(name, config))?})
             } else {
                 Err(PyTypeError::new_err("Top-level JSON must be an object"))
```

### Comparing `issue_db_api-0.3.1/issue_db_api/src/models.rs` & `issue_db_api-0.4.0/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.3.1/issue_db_api/src/query.rs` & `issue_db_api-0.4.0/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.3.1/issue_db_api/src/repository.rs` & `issue_db_api-0.4.0/issue_db_api/src/repository.rs`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,20 @@
     pub fn embeddings(&self) -> APIResult<Vec<Embedding>> {
         let embeddings = self.api.get_all_embeddings()?
             .into_iter()
             .map(|e| e.into_bound_embedding(self.api.clone(), self.config_handling))
             .collect();
         Ok(embeddings)
     }
+    
+    pub fn get_embedding_by_id(&self, id: String) -> APIResult<Embedding> {
+        let raw = self.api.get_embedding(id)?;
+        let converted = raw.into_bound_embedding(self.api.clone(), self.config_handling);
+        Ok(converted)
+    }
 
     pub fn create_embedding(&self,
                             name: String,
                             config: HashMap<String, Value>) -> APIResult<Embedding> {
         let id = self.api.create_embedding(name.clone(), config.clone())?;
         let embedding = Embedding::new(
             self.api.clone(),
```

### Comparing `issue_db_api-0.3.1/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.4.0/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.3.1/issue_db_api/src/tags.rs` & `issue_db_api-0.4.0/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.3.1/issue_db_api/src/util.rs` & `issue_db_api-0.4.0/issue_db_api/src/util.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.3.1/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.4.0/issue_db_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.3.1
+Version: 0.4.0
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.3.1/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.4.0/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.3.1/pyproject.toml` & `issue_db_api-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.3.1"
+version = "0.4.0"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```

