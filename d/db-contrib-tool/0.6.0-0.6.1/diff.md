# Comparing `tmp/db_contrib_tool-0.6.0.tar.gz` & `tmp/db_contrib_tool-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_contrib_tool-0.6.0.tar", max compression
+gzip compressed data, was "db_contrib_tool-0.6.1.tar", max compression
```

## Comparing `db_contrib_tool-0.6.0.tar` & `db_contrib_tool-0.6.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     5222 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/README.md
--rw-r--r--   0        0        0     2139 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       13 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/__init__.py
--rw-r--r--   0        0        0      883 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/cli.py
--rw-r--r--   0        0        0        0 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/clients/__init__.py
--rw-r--r--   0        0        0     7147 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/clients/download_client.py
--rw-r--r--   0        0        0     1329 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/clients/file_service.py
--rw-r--r--   0        0        0     2636 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/clients/git_client.py
--rw-r--r--   0        0        0      305 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/clients/io_client.py
--rw-r--r--   0        0        0      984 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/clients/platform_details.py
--rw-r--r--   0        0        0     2524 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/clients/resmoke_proxy.py
--rw-r--r--   0        0        0     6667 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/config/setup_repro_env_config.yml
--rw-r--r--   0        0        0     5999 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/config.py
--rw-r--r--   0        0        0     8844 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/evg_aware_bisect/__init__.py
--rw-r--r--   0        0        0     4639 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/evg_aware_bisect/cli.py
--rw-r--r--   0        0        0      110 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
--rw-r--r--   0        0        0      418 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
--rw-r--r--   0        0        0       52 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
--rw-r--r--   0        0        0        0 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/services/__init__.py
--rw-r--r--   0        0        0     9131 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/services/evergreen_service.py
--rw-r--r--   0        0        0     2404 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/services/git_service.py
--rw-r--r--   0        0        0     2027 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/services/platform_service.py
--rw-r--r--   0        0        0    13919 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/README.md
--rw-r--r--   0        0        0       13 2023-03-27 16:23:52.044457 db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/__init__.py
--rw-r--r--   0        0        0    17392 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
--rw-r--r--   0        0        0     8912 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/cli.py
--rw-r--r--   0        0        0     8290 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/download_service.py
--rw-r--r--   0        0        0     4513 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
--rw-r--r--   0        0        0     5586 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/release_models.py
--rw-r--r--   0        0        0     3155 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/request_models.py
--rw-r--r--   0        0        0    11018 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
--rw-r--r--   0        0        0      614 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/symbolizer/README.md
--rw-r--r--   0        0        0        0 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/symbolizer/__init__.py
--rw-r--r--   0        0        0     4190 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/symbolizer/cli.py
--rw-r--r--   0        0        0     4798 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
--rw-r--r--   0        0        0    26080 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/symbolizer/mongosymb.py
--rw-r--r--   0        0        0     2269 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/usage_analytics.py
--rw-r--r--   0        0        0      235 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/utils/__init__.py
--rw-r--r--   0        0        0     1855 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/utils/build_system_options.py
--rw-r--r--   0        0        0     2160 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/utils/evergreen_conn.py
--rw-r--r--   0        0        0     1085 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/utils/filesystem.py
--rw-r--r--   0        0        0    10608 2023-03-27 16:23:52.048457 db_contrib_tool-0.6.0/src/db_contrib_tool/utils/oauth.py
--rw-r--r--   0        0        0     6795 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.0/setup.py
--rw-r--r--   0        0        0     6436 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     5222 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/README.md
+-rw-r--r--   0        0        0     2139 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/__init__.py
+-rw-r--r--   0        0        0      883 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/cli.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/clients/__init__.py
+-rw-r--r--   0        0        0     7147 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/clients/download_client.py
+-rw-r--r--   0        0        0     1329 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/clients/file_service.py
+-rw-r--r--   0        0        0     2636 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/clients/git_client.py
+-rw-r--r--   0        0        0      305 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/clients/io_client.py
+-rw-r--r--   0        0        0      984 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/clients/platform_details.py
+-rw-r--r--   0        0        0     2524 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/clients/resmoke_proxy.py
+-rw-r--r--   0        0        0     6667 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/config/setup_repro_env_config.yml
+-rw-r--r--   0        0        0     5999 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/config.py
+-rw-r--r--   0        0        0     8844 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/evg_aware_bisect/__init__.py
+-rw-r--r--   0        0        0     4639 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/evg_aware_bisect/cli.py
+-rw-r--r--   0        0        0      110 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
+-rw-r--r--   0        0        0      418 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
+-rw-r--r--   0        0        0       52 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
+-rw-r--r--   0        0        0        0 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/services/__init__.py
+-rw-r--r--   0        0        0     9131 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/services/evergreen_service.py
+-rw-r--r--   0        0        0     2404 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/services/git_service.py
+-rw-r--r--   0        0        0     2027 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/services/platform_service.py
+-rw-r--r--   0        0        0    13919 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/README.md
+-rw-r--r--   0        0        0       13 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/__init__.py
+-rw-r--r--   0        0        0    17392 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
+-rw-r--r--   0        0        0     8912 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/cli.py
+-rw-r--r--   0        0        0     8290 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/download_service.py
+-rw-r--r--   0        0        0     4513 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
+-rw-r--r--   0        0        0     5586 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/release_models.py
+-rw-r--r--   0        0        0     3155 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/request_models.py
+-rw-r--r--   0        0        0    11018 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
+-rw-r--r--   0        0        0      614 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/__init__.py
+-rw-r--r--   0        0        0     4190 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/cli.py
+-rw-r--r--   0        0        0     4798 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
+-rw-r--r--   0        0        0    26368 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/mongosymb.py
+-rw-r--r--   0        0        0     2269 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/usage_analytics.py
+-rw-r--r--   0        0        0      235 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/utils/__init__.py
+-rw-r--r--   0        0        0     1855 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/utils/build_system_options.py
+-rw-r--r--   0        0        0     2160 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/utils/evergreen_conn.py
+-rw-r--r--   0        0        0     1085 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/utils/filesystem.py
+-rw-r--r--   0        0        0    10608 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/utils/oauth.py
+-rw-r--r--   0        0        0     6795 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.1/setup.py
+-rw-r--r--   0        0        0     6436 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.1/PKG-INFO
```

### Comparing `db_contrib_tool-0.6.0/README.md` & `db_contrib_tool-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/pyproject.toml` & `db_contrib_tool-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "db-contrib-tool"
-version = "0.6.0"
+version = "0.6.1"
 description = "The `db-contrib-tool` - MongoDB's tool for contributors."
 authors = ["DAG team <dev-prod-dag@mongodb.com>"]
 readme = "README.md"
 repository = "https://github.com/10gen/db-contrib-tool"
 include = [
     "src/db_contrib_tool/bisect/*.sh",
     "src/db_contrib_tool/config/*.yml",
```

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/cli.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/clients/download_client.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/clients/download_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/clients/file_service.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/clients/file_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/clients/git_client.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/clients/platform_details.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/clients/platform_details.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/clients/resmoke_proxy.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/clients/resmoke_proxy.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/config/setup_repro_env_config.yml` & `db_contrib_tool-0.6.1/src/db_contrib_tool/config/setup_repro_env_config.yml`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/config.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/config.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/evg_aware_bisect/__init__.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/evg_aware_bisect/__init__.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/evg_aware_bisect/cli.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/evg_aware_bisect/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/services/evergreen_service.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/services/evergreen_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/services/git_service.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/services/git_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/services/platform_service.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/services/platform_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/README.md` & `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/cli.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/download_service.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/download_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/release_discovery_service.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/release_discovery_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/release_models.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/release_models.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/request_models.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/request_models.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/setup_repro_env/setup_repro_env.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/setup_repro_env.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/symbolizer/README.md` & `db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/symbolizer/cli.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/symbolizer/mongosymb.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/mongosymb.py`

 * *Files 2% similar despite different names*

```diff
@@ -580,16 +580,15 @@
             if symbolizer_process.stdout:
                 frame["symbinfo"] = self.extract_symbols(symbolizer_process.stdout)
         if symbolizer_process.stdin:
             symbolizer_process.stdin.close()
         symbolizer_process.wait()
         return frames
 
-    @staticmethod
-    def extract_symbols(stdout: IO[AnyStr]) -> List[Dict[str, Any]]:
+    def extract_symbols(self, stdout: IO[AnyStr]) -> List[Dict[str, Any]]:
         """
         Extract symbol information from the output of llvm-symbolizer.
 
         Return a list of dictionaries, each of which has fn, file, column and line entries.
 
         The format of llvm-symbolizer output is that for every CODE line of input,
         it outputs zero or more pairs of lines, and then a blank line. This way, if
@@ -601,26 +600,38 @@
 
         :param stdout: Output of llvm-symbolizer.
         :return: List of symbol information.
         """
         result: List[Dict[str, Any]] = []
         step = 0
         while True:
-            line = str(stdout.readline())
+            line = self.ensure_str(stdout.readline())
             if line == "\n":
                 break
             if step == 0:
                 result.append({"fn": line.strip()})
                 step = 1
             else:
                 file_name, line, column = line.strip().rsplit(":", 3)
                 result[-1].update({"file": file_name, "column": int(column), "line": int(line)})
                 step = 0
         return result
 
+    @staticmethod
+    def ensure_str(any_str: AnyStr) -> str:
+        """
+        Convert AnyStr to str.
+
+        :param any_str: AnyStr line.
+        :return: Line as str
+        """
+        if hasattr(any_str, "decode"):
+            return any_str.decode()
+        return str(any_str)
+
     def preprocess_frames(
         self, trace_doc: TraceDoc, input_format: InputFormat
     ) -> List[Dict[str, Any]]:
         """
         Process the paths in frame objects.
 
         :param trace_doc: Traceback doc.
```

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/usage_analytics.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/usage_analytics.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/utils/build_system_options.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/utils/build_system_options.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/utils/evergreen_conn.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/utils/evergreen_conn.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/utils/filesystem.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/src/db_contrib_tool/utils/oauth.py` & `db_contrib_tool-0.6.1/src/db_contrib_tool/utils/oauth.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.0/setup.py` & `db_contrib_tool-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'tenacity>=8.0.1,<9.0.0']
 
 entry_points = \
 {'console_scripts': ['db-contrib-tool = db_contrib_tool.cli:cli']}
 
 setup_kwargs = {
     'name': 'db-contrib-tool',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': "The `db-contrib-tool` - MongoDB's tool for contributors.",
     'long_description': '# db-contrib-tool\n\nThe `db-contrib-tool` - MongoDB\'s tools for contributors.\n\n## Table of contents\n\n- [db-contrib-tool](#db-contrib-tool)\n  - [Table of contents](#table-of-contents)\n  - [Description](#description)\n  - [Dependencies](#dependencies)\n  - [Installation](#installation)\n  - [Usage](#usage)\n  - [Contributor\'s Guide (local development)](#contributors-guide-local-development)\n    - [Install project dependencies](#install-project-dependencies)\n    - [Run command line tool (local development)](#run-command-line-tool-local-development)\n    - [Run linters](#run-linters)\n    - [Run tests](#run-tests)\n    - [Pre-commit](#pre-commit)\n    - [Testing changes in mongo](#testing-changes-in-mongo)\n    - [Test pipx package](#test-pipx-package)\n    - [Versioning](#versioning)\n    - [Code Review](#code-review)\n    - [Deployment](#deployment)\n\n## Description\n\nThe command line tool with various subcommands:\n- `bisect` - performs an evergreen-aware git-bisect to find the \'last passing version\' and \'first failing version\' of mongo\n- `setup-repro-env`\n  - [README.md](https://github.com/10gen/db-contrib-tool/blob/main/src/db_contrib_tool/setup_repro_env/README.md)\n  - downloads and installs:\n    - particular MongoDB versions\n    - debug symbols\n    - artifacts (including resmoke, python scripts etc)\n    - python venv for resmoke, python scripts etc\n- `symbolize`\n  - [README.md](https://github.com/10gen/db-contrib-tool/blob/main/src/db_contrib_tool/symbolizer/README.md)\n  - Symbolizes stacktraces from recent `mongod` and `mongos` binaries compiled in Evergreen, including patch builds, mainline builds, and release/production builds.\n  - Requires authenticating to an internal MongoDB symbol mapping service.\n\n## Dependencies\n\n- Python 3.9 or later (python3 from the [MongoDB Toolchain](https://github.com/10gen/toolchain-builder/blob/master/INSTALL.md) is highly recommended)\n\n## Installation\n\nMake sure [dependencies](#dependencies) are installed.\nUse [pipx](https://pypa.github.io/pipx/) to install db-contrib-tool that will be available globally on your machine:\n```bash\n$ python3 -m pip install pipx\n$ python3 -m pipx ensurepath\n```\n\nInstalling db-contrib-tool:\n```bash\n$ python3 -m pipx install db-contrib-tool\n```\n\nUpgrading db-contrib-tool:\n```bash\n$ python3 -m pipx upgrade db-contrib-tool\n```\n\n## Usage\n\nPrint out help message:\n```bash\n$ db-contrib-tool -h\n```\nMore information on the usage of `setup-repro-env` can be found [here](https://github.com/10gen/db-contrib-tool/blob/main/src/db_contrib_tool/setup_repro_env/README.md).\n\n## Contributor\'s Guide (local development)\n\n### Install project dependencies\n\nThis project uses [poetry](https://python-poetry.org/) for dependency management.\n```bash\n$ poetry install\n```\n\n### Run command line tool (local development)\n\n```bash\n$ ENV=DEV poetry run db-contrib-tool -h\n```\n\n### Run linters\n\n```bash\n$ poetry run isort src tests\n$ poetry run black src tests\n```\n\n### Run tests\n\n```bash\n$ poetry run pytest\n```\n\n### Pre-commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time.<br>\nTo enable pre-commit on your local repository run:\n```bash\n$ poetry run pre-commit install\n```\n\nTo run pre-commit manually:\n```bash\n$ poetry run pre-commit run\n```\n\n### Testing changes in mongo\n\nThis tool is used to help run tests in the mongodb/mongo repository. On occasion, it may be\ndesirable to run a mongodb-mongo-* patch build with in-flight changes to this repository. The\nfollowing steps can be take to accomplish that.\n\n- Create a branch with the changes you wish to test.\n- Push the branch to the origin repository: `git push -u origin <branch_name>`.\n- In the "mongo" repository, edit the [evergreen/prelude_db_contrib_tool.sh](https://github.com/10gen/mongo/blob/b1a3a357af735a53981737d91fd49e5e3ae67b95/evergreen/prelude_db_contrib_tool.sh#L10)\n  to install from the git repository instead of from pypi:\n\n  ```bash\n  pipx install "git+ssh://git@github.com/<user_name>/db-contrib-tool.git@<branch_name>" || exit 1\n  ```\n\n- Create a patch build.\n\nThe patch build should now pull down the changes from your branch instead of using the published\ndb-contrib-tool.\n\n**Note**: Since the db-contrib-tool is pulled from your branch, if you need to make additional\nchanges to the tool, you can just push to the branch and then restart the desired tasks. There is\nno need to create an additional patch build unless you also need to make updates to the mongo\nrepository.\n\n### Test pipx package\n\nPipx installation recommendations can be found in [installation](#installation) section.<br>\nThe tool can be installed via pipx from your local repo:\n```bash\n$ python3 -m pipx install /path/to/db-contrib-tool\n```\n\n### Versioning\n\nThis project uses [semver](https://semver.org/) for versioning.\nPlease include a description what is added for each new version in `CHANGELOG.md`.\n\n### Code Review\n\nPlease open a Github Pull Request for code review.\nThis project uses the [Evergreen Commit Queue](https://github.com/evergreen-ci/evergreen/wiki/Commit-Queue#pr).\nAdd a PR comment with `evergreen merge` to trigger a merge.\n\n### Deployment\n\nDeployment to pypi is automatically triggered on merges to main.\n',
     'author': 'DAG team',
     'author_email': 'dev-prod-dag@mongodb.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/10gen/db-contrib-tool',
```

### Comparing `db_contrib_tool-0.6.0/PKG-INFO` & `db_contrib_tool-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-contrib-tool
-Version: 0.6.0
+Version: 0.6.1
 Summary: The `db-contrib-tool` - MongoDB's tool for contributors.
 Home-page: https://github.com/10gen/db-contrib-tool
 Author: DAG team
 Author-email: dev-prod-dag@mongodb.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

