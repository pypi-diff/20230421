# Comparing `tmp/time_tracker-0.4.0.tar.gz` & `tmp/time_tracker-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_tracker-0.4.0.tar", max compression
+gzip compressed data, was "time_tracker-0.4.1.tar", max compression
```

## Comparing `time_tracker-0.4.0.tar` & `time_tracker-0.4.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-04-13 08:38:39.853413 time_tracker-0.4.0/LICENSE
--rw-r--r--   0        0        0     1256 2023-04-13 08:38:39.853577 time_tracker-0.4.0/README.md
--rw-r--r--   0        0        0      639 2023-04-19 11:07:31.905125 time_tracker-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-13 08:38:39.855268 time_tracker-0.4.0/time_tracker/__init__.py
--rw-r--r--   0        0        0     2768 2023-04-19 11:11:22.506094 time_tracker-0.4.0/time_tracker/log.py
--rw-r--r--   0        0        0     5179 2023-04-19 11:09:46.230168 time_tracker-0.4.0/time_tracker/main.py
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 time_tracker-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-21 16:00:56.633415 time_tracker-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1256 2023-04-21 16:00:56.633415 time_tracker-0.4.1/README.md
+-rw-r--r--   0        0        0      638 2023-04-21 16:00:56.633415 time_tracker-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 16:00:56.633415 time_tracker-0.4.1/time_tracker/__init__.py
+-rw-r--r--   0        0        0     2766 2023-04-21 16:00:56.633415 time_tracker-0.4.1/time_tracker/log.py
+-rw-r--r--   0        0        0     5179 2023-04-21 16:00:56.633415 time_tracker-0.4.1/time_tracker/main.py
+-rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 time_tracker-0.4.1/PKG-INFO
```

### Comparing `time_tracker-0.4.0/LICENSE` & `time_tracker-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `time_tracker-0.4.0/README.md` & `time_tracker-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `time_tracker-0.4.0/pyproject.toml` & `time_tracker-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "time-tracker"
-version = "0.4.0"
+version = "0.4.1"
 description = "CLI to track time spent on tasks using pomodoro technique"
 authors = ["Jose Cabeda <jecabeda@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 tt = "time_tracker.main:app"
 
@@ -13,15 +13,15 @@
 typer = "0.7.0"
 python-dotenv = "^0.19.2"
 pytest = "^7.3.1"
 rich = "^13.3.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
-black = "^21.12b0"
+black = "^23.3.0"
 mypy = "^1.2.0"
 ruff = "^0.0.261"
 
 [build-system]
 requires = ["poetry>=1.4"]
 build-backend = "poetry.masonry.api"
```

### Comparing `time_tracker-0.4.0/time_tracker/log.py` & `time_tracker-0.4.1/time_tracker/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,30 +17,28 @@
     ):
         self.log_folder = Path(os.getenv("TT_LOG_FOLDER", "."))
 
         self.log_file = self.log_folder / f"{(datetime.today()).strftime('%Y%m%d')}.log"
         logging.basicConfig(filename=self.log_file, format=format, level=logging.INFO)
 
     def write_thought(self, message: str):
-
         logger = logging.getLogger()  # Logger
         logger_handler = logging.FileHandler(
             filename=self.log_file
         )  # Handler for the logger
         logger.addHandler(logger_handler)
         FORMAT = "thought: %(message)s"
 
         # New formatter for the handler:
         logger_handler.setFormatter(logging.Formatter(FORMAT))
 
         logging.info(message)
         logger.removeHandler(logger_handler)
 
     def retrieve_thoughts(self):
-
         list_of_files = list(self.log_folder.glob("*.log"))
 
         thoughts: list[str] = []
 
         for file in list_of_files:
             with open(file, "r") as file:
                 content = file.readlines()
```

### Comparing `time_tracker-0.4.0/time_tracker/main.py` & `time_tracker-0.4.1/time_tracker/main.py`

 * *Files identical despite different names*

### Comparing `time_tracker-0.4.0/PKG-INFO` & `time_tracker-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time-tracker
-Version: 0.4.0
+Version: 0.4.1
 Summary: CLI to track time spent on tasks using pomodoro technique
 Author: Jose Cabeda
 Author-email: jecabeda@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
```

