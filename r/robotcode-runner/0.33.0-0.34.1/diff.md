# Comparing `tmp/robotcode_runner-0.33.0.tar.gz` & `tmp/robotcode_runner-0.34.1.tar.gz`

## Comparing `robotcode_runner-0.33.0.tar` & `robotcode_runner-0.34.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/src/robotcode/runner/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/README.md
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/pyproject.toml
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 robotcode_runner-0.33.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/pyproject.toml
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.34.1/PKG-INFO
```

### Comparing `robotcode_runner-0.33.0/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.34.1/src/robotcode/runner/cli/libdoc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from pathlib import Path
-from typing import Any, Optional, Tuple, Union, cast
+from typing import Any, Optional, Tuple, cast
 
 import click
 from robot.errors import DataError, Information
 from robot.libdoc import USAGE, LibDoc
 from robot.version import get_full_version
 from robotcode.plugin import Application, pass_application
 from robotcode.robot.config.loader import load_config_from_path
@@ -33,41 +33,40 @@
 
         return options, arguments
 
     def main(self, arguments: Any, **options: Any) -> Any:
         if self.root_folder is not None:
             os.chdir(self.root_folder)
 
-        super().main(arguments, **options)
+        return super().main(arguments, **options)
 
 
 @click.command(
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
+    epilog='Use "-- --help" to see the `libdoc` help.',
 )
 @click.version_option(
     version=__version__,
     package_name="robotcode.runner.libdoc",
     prog_name="RobotCode LibDoc",
     message=f"%(prog)s %(version)s\n{USAGE.splitlines()[0].split(' -- ')[0].strip()} {get_full_version()}",
 )
 @click.argument("robot_options_and_args", nargs=-1, type=click.Path())
 @pass_application
 def libdoc(
     app: Application,
     robot_options_and_args: Tuple[str, ...],
-) -> Union[str, int, None]:
-    """Runs "libdoc" with the selected configuration, profiles, options and arguments.
+) -> None:
+    """Runs `libdoc` with the selected configuration, profiles, options and arguments.
 
-    The options and arguments are passed to "libdoc" as is.
-
-    Use "-- --help" to see the libdoc help.
+    The options and arguments are passed to `libdoc` as is.
     """
 
     robot_arguments = None
     try:
         _, robot_arguments = LibDoc().parse_arguments(robot_options_and_args)
     except (DataError, Information):
         pass
@@ -93,18 +92,18 @@
     options = libdoc_options.build_command_line()
 
     if profile.env:
         for k, v in profile.env.items():
             os.environ[k] = v
             app.verbose(lambda: f"Set environment variable {k} to {v}")
 
-    try:
-        app.verbose(
-            lambda: "Executing libdoc robot with the following options:\n    "
-            + " ".join(f'"{o}"' for o in (options + list(robot_options_and_args)))
-        )
-        return cast(
+    app.verbose(
+        lambda: "Executing libdoc robot with the following options:\n    "
+        + " ".join(f'"{o}"' for o in (options + list(robot_options_and_args)))
+    )
+
+    app.exit(
+        cast(
             int,
             LibDocEx(app.config.dry, root_folder).execute_cli((*options, *robot_options_and_args), exit=False),
         )
-    except SystemExit as e:
-        return cast(int, e.code)
+    )
```

### Comparing `robotcode_runner-0.33.0/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.34.1/src/robotcode/runner/cli/rebot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from pathlib import Path
-from typing import Any, Optional, Tuple, Union, cast
+from typing import Any, Optional, Tuple, cast
 
 import click
 from robot.errors import DataError, Information
 from robot.rebot import USAGE, Rebot
 from robot.version import get_full_version
 from robotcode.plugin import Application, pass_application
 from robotcode.robot.config.loader import load_config_from_path
@@ -33,42 +33,40 @@
 
         return options, arguments
 
     def main(self, arguments: Any, **options: Any) -> Any:
         if self.root_folder is not None:
             os.chdir(self.root_folder)
 
-        super().main(arguments, **options)
+        return super().main(arguments, **options)
 
 
 @click.command(
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
-    # short_help='Runs "rebot" with the selected configuration, profiles, options and arguments.',
+    epilog='Use "-- --help" to see `rebot` help.',
 )
 @click.version_option(
     version=__version__,
     package_name="robotcode.runner.libdoc",
     prog_name="RobotCode LibDoc",
     message=f"%(prog)s %(version)s\n{USAGE.splitlines()[0].split(' -- ')[0].strip()} {get_full_version()}",
 )
 @click.argument("robot_options_and_args", nargs=-1, type=click.Path())
 @pass_application
 def rebot(
     app: Application,
     robot_options_and_args: Tuple[str, ...],
-) -> Union[str, int, None]:
-    """Runs "rebot" with the selected configuration, profiles, options and arguments.
+) -> None:
+    """Runs `rebot` with the selected configuration, profiles, options and arguments.
 
-    The options and arguments are passed to "rebot" as is.
-
-    Use "-- --help" to see the rebot help.
+    The options and arguments are passed to `rebot` as is.
     """
 
     robot_arguments = None
     try:
         _, robot_arguments = Rebot().parse_arguments(robot_options_and_args)
     except (DataError, Information):
         pass
@@ -98,18 +96,18 @@
         raise click.ClickException(str(e)) from e
 
     if profile.env:
         for k, v in profile.env.items():
             os.environ[k] = v
             app.verbose(lambda: f"Set environment variable {k} to {v}")
 
-    try:
-        app.verbose(
-            lambda: "Executing rebot with the following options:\n    "
-            + " ".join(f'"{o}"' for o in (options + list(robot_options_and_args)))
-        )
-        return cast(
+    app.verbose(
+        lambda: "Executing rebot with the following options:\n    "
+        + " ".join(f'"{o}"' for o in (options + list(robot_options_and_args)))
+    )
+
+    app.exit(
+        cast(
             int,
             RebotEx(app.config.dry, root_folder).execute_cli((*options, *robot_options_and_args), exit=False),
         )
-    except SystemExit as e:
-        return cast(int, e.code)
+    )
```

### Comparing `robotcode_runner-0.33.0/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.34.1/src/robotcode/runner/cli/robot.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,41 +46,49 @@
 
         return options, arguments
 
     def main(self, arguments: Any, **options: Any) -> Any:
         if self.root_folder is not None:
             os.chdir(self.root_folder)
 
-        super().main(arguments, **options)
+        return super().main(arguments, **options)
 
 
 @click.command(
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
+    epilog='Use "-- --help" to see `robot` help.',
+)
+@click.option("--by-longname", type=str, multiple=True, help="Select tests/tasks or suites by longname.")
+@click.option(
+    "--exclude-by-longname",
+    type=str,
+    multiple=True,
+    help="Excludes tests/tasks or suites by longname.",
 )
 @click.version_option(
     version=__version__,
     package_name="robotcode.runner",
     prog_name="RobotCode Runner",
     message=f"%(prog)s %(version)s\n{USAGE.splitlines()[0].split(' -- ')[0].strip()} {get_full_version()}",
 )
 @click.argument("robot_options_and_args", nargs=-1, type=click.Path())
 @pass_application
 def robot(
     app: Application,
+    by_longname: Tuple[str, ...],
+    exclude_by_longname: Tuple[str, ...],
     robot_options_and_args: Tuple[str, ...],
-) -> Union[str, int, None]:
-    """Runs "robot" with the selected configuration, profiles, options and arguments.
-
-    The options and arguments are passed to "robot" as is.
+) -> None:
+    """Runs `robot` with the selected configuration, profiles, options and arguments.
 
-    Use "-- --help" to see the robot help.
+    The options and arguments are passed to `robot` as is.
     """
 
     robot_arguments: Optional[List[Union[str, Path]]] = None
     try:
         _, robot_arguments = RobotFramework().parse_arguments(robot_options_and_args)
     except (DataError, Information):
         pass
@@ -95,30 +103,38 @@
             .evaluated()
         )
     except (TypeError, ValueError) as e:
         raise click.ClickException(str(e)) from e
 
     options = profile.build_command_line()
 
+    if by_longname:
+        sep = ";" if any(True for l in by_longname if ":" in l) else ":"
+        options += ("--prerunmodifier", f"robotcode.modifiers.ByLongName:{sep.join(by_longname)}")
+
+    if exclude_by_longname:
+        sep = ";" if any(True for l in exclude_by_longname if ":" in l) else ":"
+        options += ("--prerunmodifier", f"robotcode.modifiers.ExcludedByLongName:{sep.join(exclude_by_longname)}")
+
     if profile.env:
         for k, v in profile.env.items():
             os.environ[k] = v
             app.verbose(lambda: f"Set environment variable {k} to {v}")
 
-    try:
-        app.verbose(
-            lambda: "Executing robot with the following options:\n    "
-            + " ".join(f'"{o}"' for o in (options + list(robot_options_and_args)))
-        )
-        return cast(
+    app.verbose(
+        lambda: "Executing robot with the following options:\n    "
+        + " ".join(f'"{o}"' for o in (options + list(robot_options_and_args)))
+    )
+
+    app.exit(
+        cast(
             int,
             RobotFrameworkEx(
                 [] if profile.paths is None else profile.paths if isinstance(profile.paths, list) else [profile.paths],
                 app.config.dry,
                 root_folder,
             ).execute_cli(
                 (*options, *robot_options_and_args),
                 exit=False,
             ),
         )
-    except SystemExit as e:
-        return cast(int, e.code)
+    )
```

### Comparing `robotcode_runner-0.33.0/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.34.1/src/robotcode/runner/cli/testdoc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from pathlib import Path
-from typing import Any, Optional, Tuple, Union, cast
+from typing import Any, Optional, Tuple, cast
 
 import click
 from robot.errors import DataError, Information
 from robot.testdoc import USAGE, TestDoc
 from robot.version import get_full_version
 from robotcode.plugin import Application, pass_application
 from robotcode.robot.config.loader import load_config_from_path
@@ -33,41 +33,40 @@
 
         return options, arguments
 
     def main(self, arguments: Any, **options: Any) -> Any:
         if self.root_folder is not None:
             os.chdir(self.root_folder)
 
-        super().main(arguments, **options)
+        return super().main(arguments, **options)
 
 
 @click.command(
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
+    epilog='Use "-- --help" to see `testdoc` help.',
 )
 @click.version_option(
     version=__version__,
     package_name="robotcode.runner.testdoc",
     prog_name="RobotCode TestDoc",
     message=f"%(prog)s %(version)s\n{USAGE.splitlines()[0].split(' -- ')[0].strip()} {get_full_version()}",
 )
 @click.argument("robot_options_and_args", nargs=-1, type=click.Path())
 @pass_application
 def testdoc(
     app: Application,
     robot_options_and_args: Tuple[str, ...],
-) -> Union[str, int, None]:
-    """Runs "testdoc" with the selected configuration, profiles, options and arguments.
+) -> None:
+    """Runs `testdoc` with the selected configuration, profiles, options and arguments.
 
-    The options and arguments are passed to "testdoc" as is.
-
-    Use "-- --help" to see the testdoc help.
+    The options and arguments are passed to `testdoc` as is.
     """
 
     robot_arguments = None
     try:
         _, robot_arguments = TestDoc().parse_arguments(robot_options_and_args)
     except (DataError, Information):
         pass
@@ -94,18 +93,15 @@
     options = testdoc_options.build_command_line()
 
     if profile.env:
         for k, v in profile.env.items():
             os.environ[k] = v
             app.verbose(lambda: f"Set environment variable {k} to {v}")
 
-    try:
-        app.verbose(
-            lambda: "Executing testdoc with the following options:\n    "
-            + " ".join(f'"{o}"' for o in (options + list(robot_options_and_args)))
-        )
-        return cast(
-            int,
-            TestDocEx(app.config.dry, root_folder).execute_cli((*options, *robot_options_and_args), exit=False),
-        )
-    except SystemExit as e:
-        return cast(int, e.code)
+    app.verbose(
+        lambda: "Executing testdoc with the following options:\n    "
+        + " ".join(f'"{o}"' for o in (options + list(robot_options_and_args)))
+    )
+
+    app.exit(
+        cast(int, TestDocEx(app.config.dry, root_folder).execute_cli((*options, *robot_options_and_args), exit=False))
+    )
```

### Comparing `robotcode_runner-0.33.0/.gitignore` & `robotcode_runner-0.34.1/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.33.0/LICENSE.txt` & `robotcode_runner-0.34.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.33.0/README.md` & `robotcode_runner-0.34.1/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.33.0/pyproject.toml` & `robotcode_runner-0.34.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -21,21 +21,21 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Operating System :: OS Independent",
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
+dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-plugin",
-  "robotcode-robot",
-  "robotcode",
+  "robotcode-robot==0.34.1",
+  "robotcode-modifiers==0.34.1",
+  "robotcode==0.34.1",
 ]
-dynamic = ["version"]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
```

### Comparing `robotcode_runner-0.33.0/PKG-INFO` & `robotcode_runner-0.34.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-runner
-Version: 0.33.0
+Version: 0.34.1
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode
-Requires-Dist: robotcode-plugin
-Requires-Dist: robotcode-robot
+Requires-Dist: robotcode-modifiers==0.34.1
+Requires-Dist: robotcode-robot==0.34.1
+Requires-Dist: robotcode==0.34.1
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```

