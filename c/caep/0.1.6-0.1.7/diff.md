# Comparing `tmp/caep-0.1.6.tar.gz` & `tmp/caep-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caep-0.1.6.tar", last modified: Mon Apr 10 07:37:22 2023, max compression
+gzip compressed data, was "caep-0.1.7.tar", last modified: Fri Apr 21 06:55:30 2023, max compression
```

## Comparing `caep-0.1.6.tar` & `caep-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-10 07:37:22.935539 caep-0.1.6/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      773 2020-03-11 11:42:29.000000 caep-0.1.6/LICENSE
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-04-10 07:37:22.935539 caep-0.1.6/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9157 2023-03-28 14:28:15.000000 caep-0.1.6/README.md
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-10 07:37:22.932205 caep-0.1.6/caep/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      369 2023-03-28 05:50:28.000000 caep-0.1.6/caep/__init__.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     8106 2023-04-10 07:37:20.000000 caep-0.1.6/caep/config.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)      922 2023-01-30 06:37:56.000000 caep-0.1.6/caep/example.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1396 2023-03-28 05:50:28.000000 caep-0.1.6/caep/helpers.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    11081 2023-01-30 11:31:45.000000 caep-0.1.6/caep/schema.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1548 2023-01-02 09:23:36.000000 caep-0.1.6/caep/xdg.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-10 07:37:22.932205 caep-0.1.6/caep.egg-info/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-04-10 07:37:22.000000 caep-0.1.6/caep.egg-info/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      343 2023-04-10 07:37:22.000000 caep-0.1.6/caep.egg-info/SOURCES.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2023-04-10 07:37:22.000000 caep-0.1.6/caep.egg-info/dependency_links.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       23 2023-04-10 07:37:22.000000 caep-0.1.6/caep.egg-info/requires.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        5 2023-04-10 07:37:22.000000 caep-0.1.6/caep.egg-info/top_level.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-03-11 11:43:17.000000 caep-0.1.6/caep.egg-info/zip-safe
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       38 2023-04-10 07:37:22.935539 caep-0.1.6/setup.cfg
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      953 2023-04-10 07:37:20.000000 caep-0.1.6/setup.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-10 07:37:22.935539 caep-0.1.6/tests/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2420 2023-01-02 09:23:36.000000 caep-0.1.6/tests/test_config.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1455 2023-03-28 05:50:28.000000 caep-0.1.6/tests/test_helpers.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9448 2023-04-10 07:37:20.000000 caep-0.1.6/tests/test_schema.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-21 06:55:30.287869 caep-0.1.7/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      773 2020-03-11 11:42:29.000000 caep-0.1.7/LICENSE
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-04-21 06:55:30.287869 caep-0.1.7/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9157 2023-03-28 14:28:15.000000 caep-0.1.7/README.md
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-21 06:55:30.284536 caep-0.1.7/caep/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      369 2023-03-28 05:50:28.000000 caep-0.1.7/caep/__init__.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     8171 2023-04-21 06:55:27.000000 caep-0.1.7/caep/config.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)      922 2023-01-30 06:37:56.000000 caep-0.1.7/caep/example.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1396 2023-03-28 05:50:28.000000 caep-0.1.7/caep/helpers.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    11081 2023-01-30 11:31:45.000000 caep-0.1.7/caep/schema.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1548 2023-01-02 09:23:36.000000 caep-0.1.7/caep/xdg.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-21 06:55:30.284536 caep-0.1.7/caep.egg-info/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-04-21 06:55:30.000000 caep-0.1.7/caep.egg-info/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      343 2023-04-21 06:55:30.000000 caep-0.1.7/caep.egg-info/SOURCES.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2023-04-21 06:55:30.000000 caep-0.1.7/caep.egg-info/dependency_links.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       23 2023-04-21 06:55:30.000000 caep-0.1.7/caep.egg-info/requires.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        5 2023-04-21 06:55:30.000000 caep-0.1.7/caep.egg-info/top_level.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-03-11 11:43:17.000000 caep-0.1.7/caep.egg-info/zip-safe
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       38 2023-04-21 06:55:30.287869 caep-0.1.7/setup.cfg
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      953 2023-04-21 06:55:27.000000 caep-0.1.7/setup.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-21 06:55:30.287869 caep-0.1.7/tests/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2420 2023-01-02 09:23:36.000000 caep-0.1.7/tests/test_config.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1455 2023-03-28 05:50:28.000000 caep-0.1.7/tests/test_helpers.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    10271 2023-04-21 06:55:27.000000 caep-0.1.7/tests/test_schema.py
```

### Comparing `caep-0.1.6/LICENSE` & `caep-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `caep-0.1.6/PKG-INFO` & `caep-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caep
-Version: 0.1.6
+Version: 0.1.7
 Summary: Config Argument Env Parser (CAEP)
 Home-page: https://github.com/mnemonic-no/caep
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: ISC
 Keywords: mnemonic
 Classifier: Development Status :: 4 - Beta
```

### Comparing `caep-0.1.6/README.md` & `caep-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `caep-0.1.6/caep/config.py` & `caep-0.1.7/caep/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,33 +117,35 @@
         description="configfile parser", add_help=False
     )
     early_parser.add_argument(
         "--config",
         dest="config",
         type=argparse.FileType("r", encoding="UTF-8"),
         default=None,
+        nargs="+",
         help="change default configuration location",
     )
 
     args, remainder_argv = early_parser.parse_known_args(opts)
 
-    config = args.config
+    config = []
 
-    if config:
-        config = config.read()
+    if args.config:
+        config = [cfg_file.read() for cfg_file in args.config]
 
     # No config file specified on command line, attempt to find
     # in default locations
     else:
         if config_id and config_name:
-            config = find_default_ini(config_id, config_name)
+            config = [find_default_ini(config_id, config_name)]
 
     if config:
         cp = configparser.ConfigParser()
-        cp.read_string(config)
+        for cfg in config:
+            cp.read_string(cfg)
         return cp, remainder_argv
 
     return None, remainder_argv
 
 
 def get_env(key: str) -> Dict[str, str]:
     """
@@ -267,15 +269,15 @@
 
     if cp and section_name:
         # Add (empty) section. In this way we can still access
         # the DEFAULT section
         if not cp.has_section(section_name):
             cp.add_section(section_name)
         config = dict(cp[section_name])
-    elif cp and cp.has_section("DEFAULT"):
-        config = dict(cp["DEFAULT"])
+    elif cp and cp.defaults():
+        config = dict(cp.defaults())
     else:
         config = {}
 
     parser.set_defaults(**all_defaults(parser, config))
 
     return parser.parse_args(remainder_argv)
```

### Comparing `caep-0.1.6/caep/example.py` & `caep-0.1.7/caep/example.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.6/caep/helpers.py` & `caep-0.1.7/caep/helpers.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.6/caep/schema.py` & `caep-0.1.7/caep/schema.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.6/caep/xdg.py` & `caep-0.1.7/caep/xdg.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.6/caep.egg-info/PKG-INFO` & `caep-0.1.7/caep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caep
-Version: 0.1.6
+Version: 0.1.7
 Summary: Config Argument Env Parser (CAEP)
 Home-page: https://github.com/mnemonic-no/caep
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: ISC
 Keywords: mnemonic
 Classifier: Development Status :: 4 - Beta
```

### Comparing `caep-0.1.6/setup.py` & `caep-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), "rb") as f:
     long_description = f.read().decode("utf-8")
 
 setup(
     name="caep",
-    version="0.1.6",
+    version="0.1.7",
     author="mnemonic AS",
     zip_safe=True,
     author_email="opensource@mnemonic.no",
     description="Config Argument Env Parser (CAEP)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="ISC",
```

### Comparing `caep-0.1.6/tests/test_config.py` & `caep-0.1.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.6/tests/test_helpers.py` & `caep-0.1.7/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.6/tests/test_schema.py` & `caep-0.1.7/tests/test_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     DictInfo,
     FieldError,
     escape_split,
     split_dict,
     split_list,
 )
 
-INI_TEST_FILE = os.path.join(os.path.dirname(__file__), "data/config_testdata.ini")
+TEST_DATA_DIR = Path(__file__).parent / "data"
+INI_TEST_FILE = TEST_DATA_DIR / "config_testdata.ini"
+SECOND_INI_TEST_FILE = TEST_DATA_DIR / "config_testdata2.ini"
 
 
 class Arguments(BaseModel):
     str_arg: str = Field(description="Required String Argument")
     number: int = Field(default=1, description="Integer with default value")
     enabled: bool = Field(default=False, description="Boolean with default value")
 
@@ -69,14 +71,20 @@
     number: int = Field(default=1, description="Integer with default value")
 
 
 class Arg3(BaseModel):
     enabled: bool = Field(default=False, description="Boolean with default value")
 
 
+class MultipleFiles(BaseModel):
+    number: int = Field(default=1, description="Integer with default value")
+    first_file: bool = Field(description="Value set in first config file")
+    second_file: bool = Field(description="Value set in second config file")
+
+
 class ArgCombined(Arg1, Arg2, Arg3):
     pass
 
 
 def parse_args(
     model: Type[caep.schema.BaseModelType],
     commandline: Optional[List[str]] = None,
@@ -242,14 +250,28 @@
     commandline = shlex.split(f"--config {INI_TEST_FILE}")
 
     config = caep.load(Arg2, "Program description", opts=commandline)
 
     assert config.number == 3
 
 
+def test_schema_ini_default_multiple_files() -> None:
+    """all arguments from ini file and default section"""
+    commandline = shlex.split(f"--config {INI_TEST_FILE} {SECOND_INI_TEST_FILE}")
+
+    config = caep.load(MultipleFiles, "Program description", opts=commandline)
+
+    # Make sure files has been read in the correct order
+    assert config.number == 2
+
+    # Make sure both files has been read
+    assert config.first_file is True
+    assert config.second_file is True
+
+
 def test_argparse_env() -> None:
     """all arguments from env"""
 
     env = {
         "STR_ARG": "from env",
         "NUMBER": 4,
         "ENABLED": "yes",  # accepts both yes and true
```

