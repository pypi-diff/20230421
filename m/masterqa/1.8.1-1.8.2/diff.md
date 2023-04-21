# Comparing `tmp/masterqa-1.8.1.tar.gz` & `tmp/masterqa-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masterqa-1.8.1.tar", last modified: Tue Feb  7 05:14:47 2023, max compression
+gzip compressed data, was "masterqa-1.8.2.tar", last modified: Fri Apr 21 19:37:46 2023, max compression
```

## Comparing `masterqa-1.8.1.tar` & `masterqa-1.8.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-07 05:14:47.486508 masterqa-1.8.1/
--rw-r--r--   0 michael    (501) staff       (20)     1682 2022-12-06 03:15:26.000000 masterqa-1.8.1/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)     1080 2022-12-06 03:15:26.000000 masterqa-1.8.1/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)      100 2022-12-06 03:15:26.000000 masterqa-1.8.1/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     3015 2023-02-07 05:14:47.486545 masterqa-1.8.1/PKG-INFO
--rwxr-xr-x   0 michael    (501) staff       (20)     2616 2023-01-24 04:43:53.000000 masterqa-1.8.1/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-07 05:14:47.485836 masterqa-1.8.1/masterqa/
--rwxr-xr-x   0 michael    (501) staff       (20)       48 2022-12-06 03:15:26.000000 masterqa-1.8.1/masterqa/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)    17647 2022-12-06 03:15:26.000000 masterqa-1.8.1/masterqa/master_qa.py
--rwxr-xr-x   0 michael    (501) staff       (20)      718 2022-12-06 03:15:26.000000 masterqa-1.8.1/masterqa/settings.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-02-07 05:14:47.486416 masterqa-1.8.1/masterqa.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     3015 2023-02-07 05:14:47.000000 masterqa-1.8.1/masterqa.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      310 2023-02-07 05:14:47.000000 masterqa-1.8.1/masterqa.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-02-07 05:14:47.000000 masterqa-1.8.1/masterqa.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       77 2023-02-07 05:14:47.000000 masterqa-1.8.1/masterqa.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        9 2023-02-07 05:14:47.000000 masterqa-1.8.1/masterqa.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)     1436 2023-01-24 04:35:47.000000 masterqa-1.8.1/pytest.ini
--rwxr-xr-x   0 michael    (501) staff       (20)       82 2023-02-07 05:13:38.000000 masterqa-1.8.1/requirements.txt
--rwxr-xr-x   0 michael    (501) staff       (20)      188 2023-02-07 05:14:47.486714 masterqa-1.8.1/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     3214 2023-02-07 05:13:38.000000 masterqa-1.8.1/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-21 19:37:46.187779 masterqa-1.8.2/
+-rw-r--r--   0 michael    (501) staff       (20)     1682 2022-12-06 03:15:26.000000 masterqa-1.8.2/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)     1080 2022-12-06 03:15:26.000000 masterqa-1.8.2/LICENSE
+-rw-r--r--   0 michael    (501) staff       (20)      100 2022-12-06 03:15:26.000000 masterqa-1.8.2/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     3015 2023-04-21 19:37:46.187828 masterqa-1.8.2/PKG-INFO
+-rwxr-xr-x   0 michael    (501) staff       (20)     2616 2023-01-24 04:43:53.000000 masterqa-1.8.2/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-21 19:37:46.187153 masterqa-1.8.2/masterqa/
+-rwxr-xr-x   0 michael    (501) staff       (20)       48 2022-12-06 03:15:26.000000 masterqa-1.8.2/masterqa/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    17697 2023-04-21 19:32:04.000000 masterqa-1.8.2/masterqa/master_qa.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      718 2022-12-06 03:15:26.000000 masterqa-1.8.2/masterqa/settings.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-21 19:37:46.187679 masterqa-1.8.2/masterqa.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     3015 2023-04-21 19:37:46.000000 masterqa-1.8.2/masterqa.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      310 2023-04-21 19:37:46.000000 masterqa-1.8.2/masterqa.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-21 19:37:46.000000 masterqa-1.8.2/masterqa.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       77 2023-04-21 19:37:46.000000 masterqa-1.8.2/masterqa.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        9 2023-04-21 19:37:46.000000 masterqa-1.8.2/masterqa.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1440 2023-04-21 19:32:04.000000 masterqa-1.8.2/pytest.ini
+-rwxr-xr-x   0 michael    (501) staff       (20)       82 2023-04-21 19:32:04.000000 masterqa-1.8.2/requirements.txt
+-rwxr-xr-x   0 michael    (501) staff       (20)      188 2023-04-21 19:37:46.188017 masterqa-1.8.2/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     3481 2023-04-21 19:32:04.000000 masterqa-1.8.2/setup.py
```

### Comparing `masterqa-1.8.1/.gitignore` & `masterqa-1.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.1/LICENSE` & `masterqa-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.1/PKG-INFO` & `masterqa-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterqa
-Version: 1.8.1
+Version: 1.8.2
 Summary: Automation-Assisted Manual Testing - https://masterqa.com
 Home-page: https://github.com/masterqa/MasterQA
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Platform: Windows
```

### Comparing `masterqa-1.8.1/README.md` & `masterqa-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.1/masterqa/master_qa.py` & `masterqa-1.8.2/masterqa/master_qa.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,16 @@
         if js_utils.is_jquery_confirm_activated(self.driver):
             use_jqc = True
         else:
             js_utils.activate_jquery_confirm(self.driver)
             get_jqc = None
             try:
                 get_jqc = self.execute_script("return jconfirm")
-                get_jqc = get_jqc["instances"]
+                if get_jqc is None:
+                    raise Exception("jconfirm did not load")
                 use_jqc = True
             except Exception:
                 use_jqc = False
 
         if use_jqc:
             wait_time_before_verify = WAIT_TIME_BEFORE_VERIFY
             if self.verify_delay:
```

### Comparing `masterqa-1.8.1/masterqa/settings.py` & `masterqa-1.8.2/masterqa/settings.py`

 * *Files identical despite different names*

### Comparing `masterqa-1.8.1/masterqa.egg-info/PKG-INFO` & `masterqa-1.8.2/masterqa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterqa
-Version: 1.8.1
+Version: 1.8.2
 Summary: Automation-Assisted Manual Testing - https://masterqa.com
 Home-page: https://github.com/masterqa/MasterQA
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Platform: Windows
```

### Comparing `masterqa-1.8.1/pytest.ini` & `masterqa-1.8.2/pytest.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [pytest]
 
-# Display console output, disable cacheprovider:
+# Display console output. Disable cacheprovider:
 addopts = --capture=no -p no:cacheprovider
 
-# Ignore warnings such as DeprecationWarning and PytestUnknownMarkWarning
+# Skip these directories during test collection:
+norecursedirs = .* build dist recordings temp assets
+
+# Ignore DeprecationWarning, PytestUnknownMarkWarning
 filterwarnings =
     ignore::pytest.PytestWarning
     ignore:.*U.*mode is deprecated:DeprecationWarning
 
 # Configure the junit_family option explicitly:
 junit_family = legacy
 
 # Set pytest discovery rules:
 # (Most of the rules here are similar to the default rules.)
-# (unittest.TestCase rules override the rules here for classes and functions.)
+# (Inheriting unittest.TestCase could override these rules.)
 python_files = test_*.py *_test.py *_tests.py *_suite.py
 python_classes = Test* *Test* *Test *Tests *Suite
 python_functions = test_*
 
-# Here are some common pytest markers:
-# (Some are used in the example tests.)
-# (pytest v4.5.0 and newer requires marker registration to prevent warnings.)
-# (Future versions of pytest may turn those marker warnings into errors.)
+# Common pytest markers used in examples:
+# (pytest may require marker registration to prevent warnings.)
+# (Future versions may turn those marker warnings into errors.)
 markers =
     marker1: custom marker
     marker2: custom marker
     marker3: custom marker
     marker_test_suite: custom marker
     expected_failure: custom marker
     local: custom marker
```

### Comparing `masterqa-1.8.1/setup.py` & `masterqa-1.8.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,26 +25,31 @@
     input_method = input
     if not sys.version_info[0] >= 3:
         input_method = raw_input  # noqa
     reply = str(input_method(
         ">>> Confirm release PUBLISH to PyPI? (yes/no): ")).lower().strip()
     if reply == "yes":
         print("\n*** Checking code health with flake8:\n")
-        os.system("python -m pip install 'flake8==5.0.4'")
+        if sys.version_info >= (3, 9):
+            os.system("python -m pip install 'flake8==6.0.0'")
+        else:
+            os.system("python -m pip install 'flake8==5.0.4'")
         flake8_status = os.system("flake8 --exclude=recordings,temp")
         if flake8_status != 0:
             print("\nWARNING! Fix flake8 issues before publishing to PyPI!\n")
             sys.exit()
         else:
             print("*** No flake8 issues detected. Continuing...")
         print("\n*** Removing existing distribution packages: ***\n")
         os.system("rm -f dist/*.egg; rm -f dist/*.tar.gz; rm -f dist/*.whl")
         os.system("rm -rf build/bdist.*; rm -rf build/lib")
         print("\n*** Installing build: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'build>=0.10.0'")
+        print("\n*** Installing pkginfo: *** (Required for PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'pkginfo>=1.9.6'")
         print("\n*** Installing twine: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'twine>=4.0.2'")
         print("\n*** Installing tqdm: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade tqdm")
         print("\n*** Rebuilding distribution packages: ***\n")
         os.system("python -m build")  # Create new tar/wheel
         print("\n*** Publishing The Release to PyPI: ***\n")
@@ -52,29 +57,29 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name="masterqa",
-    version="1.8.1",
+    version="1.8.2",
     description="Automation-Assisted Manual Testing - https://masterqa.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     platforms=["Windows", "Linux", "Mac OS-X"],
     url="https://github.com/masterqa/MasterQA",
     author="Michael Mintz",
     author_email="mdmintz@gmail.com",
     maintainer="Michael Mintz",
     license="MIT",
     python_requires=">=3.6",
     install_requires=[
-        "seleniumbase>=4.12.7",
-        "pdbp>=1.2.8",
-        "tabcompleter>=1.1.0",
+        "seleniumbase>=4.14.1",
+        "pdbp>=1.3.1",
+        "tabcompleter>=1.2.0",
         "sbvirtualdisplay>=1.2.0",
     ],
     packages=["masterqa"],
     entry_points={
         "nose.plugins": []
     }
 )
```

