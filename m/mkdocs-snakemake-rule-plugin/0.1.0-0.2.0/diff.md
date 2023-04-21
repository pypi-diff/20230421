# Comparing `tmp/mkdocs-snakemake-rule-plugin-0.1.0.tar.gz` & `tmp/mkdocs-snakemake-rule-plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-snakemake-rule-plugin-0.1.0.tar", last modified: Thu Apr 20 12:38:25 2023, max compression
+gzip compressed data, was "mkdocs-snakemake-rule-plugin-0.2.0.tar", last modified: Fri Apr 21 21:37:49 2023, max compression
```

## Comparing `mkdocs-snakemake-rule-plugin-0.1.0.tar` & `mkdocs-snakemake-rule-plugin-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:38:25.103968 mkdocs-snakemake-rule-plugin-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-04-20 12:38:16.000000 mkdocs-snakemake-rule-plugin-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-20 12:38:25.103968 mkdocs-snakemake-rule-plugin-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-20 12:38:16.000000 mkdocs-snakemake-rule-plugin-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:38:25.103968 mkdocs-snakemake-rule-plugin-0.1.0/mkdocs_snakemake_rule_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 12:38:16.000000 mkdocs-snakemake-rule-plugin-0.1.0/mkdocs_snakemake_rule_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 12:38:25.103968 mkdocs-snakemake-rule-plugin-0.1.0/mkdocs_snakemake_rule_plugin/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-20 12:38:16.000000 mkdocs-snakemake-rule-plugin-0.1.0/mkdocs_snakemake_rule_plugin/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-20 12:38:16.000000 mkdocs-snakemake-rule-plugin-0.1.0/mkdocs_snakemake_rule_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:38:25.103968 mkdocs-snakemake-rule-plugin-0.1.0/mkdocs_snakemake_rule_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-20 12:38:25.000000 mkdocs-snakemake-rule-plugin-0.1.0/mkdocs_snakemake_rule_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-20 12:38:25.000000 mkdocs-snakemake-rule-plugin-0.1.0/mkdocs_snakemake_rule_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:38:25.000000 mkdocs-snakemake-rule-plugin-0.1.0/mkdocs_snakemake_rule_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-20 12:38:25.000000 mkdocs-snakemake-rule-plugin-0.1.0/mkdocs_snakemake_rule_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 12:38:25.000000 mkdocs-snakemake-rule-plugin-0.1.0/mkdocs_snakemake_rule_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 12:38:25.000000 mkdocs-snakemake-rule-plugin-0.1.0/mkdocs_snakemake_rule_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 12:38:25.103968 mkdocs-snakemake-rule-plugin-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-20 12:38:16.000000 mkdocs-snakemake-rule-plugin-0.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-20 12:38:16.000000 mkdocs-snakemake-rule-plugin-0.1.0/versioneer.py
+drwxrwxr-x   0 patsm159  (1000) patsm159  (1000)        0 2023-04-21 21:37:49.650701 mkdocs-snakemake-rule-plugin-0.2.0/
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)    34961 2023-04-19 13:13:08.000000 mkdocs-snakemake-rule-plugin-0.2.0/LICENSE.md
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)     1812 2023-04-21 21:37:49.650701 mkdocs-snakemake-rule-plugin-0.2.0/PKG-INFO
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)     1068 2023-04-21 21:30:37.000000 mkdocs-snakemake-rule-plugin-0.2.0/README.md
+drwxrwxr-x   0 patsm159  (1000) patsm159  (1000)        0 2023-04-21 21:37:49.650701 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin/
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)       73 2023-04-19 13:13:08.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin/__init__.py
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)      497 2023-04-21 21:37:49.650701 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin/_version.py
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)    11327 2023-04-21 21:16:40.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin/markdown.py
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)      602 2023-04-21 07:59:26.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin/plugin.py
+drwxrwxr-x   0 patsm159  (1000) patsm159  (1000)        0 2023-04-21 21:37:49.650701 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)     1812 2023-04-21 21:37:49.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)      529 2023-04-21 21:37:49.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)        1 2023-04-21 21:37:49.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)       85 2023-04-21 21:37:49.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)       14 2023-04-21 21:37:49.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/requires.txt
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)       29 2023-04-21 21:37:49.000000 mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/top_level.txt
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)      283 2023-04-21 21:37:49.650701 mkdocs-snakemake-rule-plugin-0.2.0/setup.cfg
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)     1301 2023-04-20 07:41:50.000000 mkdocs-snakemake-rule-plugin-0.2.0/setup.py
+-rw-rw-r--   0 patsm159  (1000) patsm159  (1000)    83607 2023-04-19 13:13:08.000000 mkdocs-snakemake-rule-plugin-0.2.0/versioneer.py
```

### Comparing `mkdocs-snakemake-rule-plugin-0.1.0/LICENSE.md` & `mkdocs-snakemake-rule-plugin-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-snakemake-rule-plugin-0.1.0/PKG-INFO` & `mkdocs-snakemake-rule-plugin-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,53 @@
-Metadata-Version: 2.1
-Name: mkdocs-snakemake-rule-plugin
-Version: 0.1.0
-Summary: MkDocs Plugin used to extrace rule information, to generate code and tables.
-Home-page: https://github.com/smeds/mkdocs-snakemake-rule-plugin
-Author: Patrik Smeds
-Author-email: patrik.smeds@gmail.com
-License: MIT license
-Keywords: mkdocs,plugin,yaml,schema
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # MkDocs Snakemake Rule
 
 MkDocs Plugin used to extract rule information.
 
+## Installation
+
 To use this plugin, install it with pip in the same environment as MkDocs:
 
 ```
 pip install mkdocs-snakemake-rule-plugin
 ```
 
+## Config
+
 Then add the following entry to the MkDocs config file:
 
 ```yml
 plugins:
   - snakemake-rule:
       rule_folders:
         - 'workflow/rules'
+      schemas:
+        - 'workflow/schemas/rules.schema.yaml'
 ```
 
-In your target file, add a tag to be replaced with format
+## Tag 
+
+### format
 
-SNAKEMAKE_RULE_SOURCE__filename__rulename
+Format of tags are:
+- `#SNAKEMAKE_RULE_SOURCE__filename__rulename#` : for source code extraction
+- `#  SNAKEMAKE_RULE_TABLE__filename__rulename#` : for table generation
 
+Tab parts:
+- first section identifies if rule source or table should be created
 - filename is where the rule is stored, can be without '.skm'
 - rulename is the rule that will be extract
 
 
+### Usage
+
+Add tags to your target file and they will be replaced with rule source or tables
+
+MkDocs Markdown example
 ```
+# Rule information
+## Source 
 #SNAKEMAKE_RULE_SOURCE__fastp__fastp_pe#
+
+## Parameters
+#SNAKEMAKE_RULE_TABLEE__fastp__fastp_pe#
+
 ```
```

### Comparing `mkdocs-snakemake-rule-plugin-0.1.0/mkdocs_snakemake_rule_plugin/plugin.py` & `mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .markdown import markdown_gen
 
 
 class SnakemakeRule(plugins.BasePlugin):
 
     config_scheme = (
         ("rule_folders", config.config_options.Type(list, default=[])),
+        ("schemas", config.config_options.Type(list, default=[])),
     )
 
     generator = markdown_gen()
 
     def on_config(self, config):
         self.generator = markdown_gen()
         self.generator.set_config(self.config)
```

### Comparing `mkdocs-snakemake-rule-plugin-0.1.0/mkdocs_snakemake_rule_plugin.egg-info/SOURCES.txt` & `mkdocs-snakemake-rule-plugin-0.2.0/mkdocs_snakemake_rule_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-snakemake-rule-plugin-0.1.0/setup.py` & `mkdocs-snakemake-rule-plugin-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `mkdocs-snakemake-rule-plugin-0.1.0/versioneer.py` & `mkdocs-snakemake-rule-plugin-0.2.0/versioneer.py`

 * *Files identical despite different names*

