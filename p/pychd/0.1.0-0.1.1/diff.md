# Comparing `tmp/pychd-0.1.0.tar.gz` & `tmp/pychd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychd-0.1.0.tar", max compression
+gzip compressed data, was "pychd-0.1.1.tar", max compression
```

## Comparing `pychd-0.1.0.tar` & `pychd-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-04-19 22:05:09.083953 pychd-0.1.0/LICENSE
--rw-r--r--   0        0        0    19111 2023-04-21 03:33:26.493614 pychd-0.1.0/README.md
--rw-r--r--   0        0        0      785 2023-04-21 03:23:39.207151 pychd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 21:37:37.817710 pychd-0.1.0/src/pychd/__init__.py
--rw-r--r--   0        0        0      685 2023-04-21 02:25:57.414400 pychd-0.1.0/src/pychd/compile.py
--rw-r--r--   0        0        0     3091 2023-04-21 03:12:30.874370 pychd-0.1.0/src/pychd/decompile.py
--rw-r--r--   0        0        0      439 2023-04-21 02:25:57.435574 pychd-0.1.0/src/pychd/logging.conf.template
--rw-r--r--   0        0        0     1643 2023-04-21 02:25:57.435773 pychd-0.1.0/src/pychd/main.py
--rw-r--r--   0        0        0    19920 1970-01-01 00:00:00.000000 pychd-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-19 22:05:09.083953 pychd-0.1.1/LICENSE
+-rw-r--r--   0        0        0    19111 2023-04-21 03:33:26.493614 pychd-0.1.1/README.md
+-rw-r--r--   0        0        0      785 2023-04-21 03:40:04.606726 pychd-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 21:37:37.817710 pychd-0.1.1/src/pychd/__init__.py
+-rw-r--r--   0        0        0      685 2023-04-21 02:25:57.414400 pychd-0.1.1/src/pychd/compile.py
+-rw-r--r--   0        0        0     3091 2023-04-21 03:12:30.874370 pychd-0.1.1/src/pychd/decompile.py
+-rw-r--r--   0        0        0      439 2023-04-21 02:25:57.435574 pychd-0.1.1/src/pychd/logging.conf.template
+-rw-r--r--   0        0        0     1709 2023-04-21 03:39:52.243145 pychd-0.1.1/src/pychd/main.py
+-rw-r--r--   0        0        0    19920 1970-01-01 00:00:00.000000 pychd-0.1.1/PKG-INFO
```

### Comparing `pychd-0.1.0/LICENSE` & `pychd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pychd-0.1.0/README.md` & `pychd-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pychd-0.1.0/pyproject.toml` & `pychd-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "The ChatGPT-powered Python decompiler provided superior code analysis capabilities"
 keywords = ["decompiler", "python", "poetry", "bytecode"]
 license = "MIT"
 name = "pychd"
 packages = [{include = "src/pychd"}]
 readme = "README.md"
 repository = "https://github.com/diohabara/pychd"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 openai = "^0.27.4"
 pytest = "^7.3.1"
 python = ">=3.8, <3.11"
 pytype = "^2023.4.18"
```

### Comparing `pychd-0.1.0/src/pychd/compile.py` & `pychd-0.1.1/src/pychd/compile.py`

 * *Files identical despite different names*

### Comparing `pychd-0.1.0/src/pychd/decompile.py` & `pychd-0.1.1/src/pychd/decompile.py`

 * *Files identical despite different names*

### Comparing `pychd-0.1.0/src/pychd/main.py` & `pychd-0.1.1/src/pychd/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,21 +27,22 @@
         "compile", help="Compile Python source files into bytecode."
     )
     parser_compile.add_argument("path", help="Path to compile", type=str)
 
     return parser.parse_args()
 
 
-def setup() -> None:
-    logging_config = Path(__file__).parent / "logging.conf"
-    fileConfig(logging_config)
+def setup(logging_path: Path) -> None:
+    fileConfig(logging_path)
 
 
 def cli() -> None:
-    setup()
+    logging_config = Path(__file__).parent / "logging.conf"
+    if logging_config.exists():
+        setup(logging_config)
     args = parse_args()
     logging.info(args)
     if args.command == "compile":
         to_compile = Path(args.path)
         compile.compile(to_compile=to_compile)
     elif args.command == "decompile":
         to_decompile = Path(args.path)
```

### Comparing `pychd-0.1.0/PKG-INFO` & `pychd-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychd
-Version: 0.1.0
+Version: 0.1.1
 Summary: The ChatGPT-powered Python decompiler provided superior code analysis capabilities
 Home-page: https://github.com/diohabara/pychd
 License: MIT
 Keywords: decompiler,python,poetry,bytecode
 Author: 卍diohabara卍
 Author-email: diohabara@gmail.com
 Requires-Python: >=3.8,<3.11
```

