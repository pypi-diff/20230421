# Comparing `tmp/upyTest-3.0.1.tar.gz` & `tmp/UpyTest-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upyTest-3.0.1.tar", last modified: Thu Apr 20 22:36:53 2023, max compression
+gzip compressed data, was "UpyTest-3.0.2.tar", last modified: Thu Apr 20 22:48:29 2023, max compression
```

## Comparing `upyTest-3.0.1.tar` & `UpyTest-3.0.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:36:53.892637 upyTest-3.0.1/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      712 2023-04-20 22:36:53.892637 upyTest-3.0.1/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-04-20 22:36:53.892637 upyTest-3.0.1/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-04-20 22:36:43.000000 upyTest-3.0.1/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:36:53.876637 upyTest-3.0.1/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      844 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-21 23:03:34.000000 upyTest-3.0.1/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:36:53.880637 upyTest-3.0.1/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7053 2023-04-20 20:40:22.000000 upyTest-3.0.1/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35985 2023-04-20 22:26:38.000000 upyTest-3.0.1/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8152 2023-04-18 20:16:40.000000 upyTest-3.0.1/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4634 2023-04-19 22:19:22.000000 upyTest-3.0.1/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7022 2023-04-18 20:05:18.000000 upyTest-3.0.1/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:36:53.884636 upyTest-3.0.1/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      488 2023-04-08 15:47:21.000000 upyTest-3.0.1/thonnycontrib/backend/verdicts/EmptyTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      650 2023-03-19 17:23:31.000000 upyTest-3.0.1/thonnycontrib/backend/verdicts/ExceptionTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      880 2023-03-19 17:23:26.000000 upyTest-3.0.1/thonnycontrib/backend/verdicts/FailedTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      438 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      456 2023-03-21 23:57:32.000000 upyTest-3.0.1/thonnycontrib/backend/verdicts/PassedTest.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2128 2023-03-19 18:06:02.000000 upyTest-3.0.1/thonnycontrib/backend/verdicts/Test.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:36:53.884636 upyTest-3.0.1/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:36:53.884636 upyTest-3.0.1/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/docs/res/test_only_btn.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:36:53.884636 upyTest-3.0.1/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8661 2023-04-02 02:52:03.000000 upyTest-3.0.1/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1464 2023-03-21 23:53:12.000000 upyTest-3.0.1/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3917 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:36:53.884636 upyTest-3.0.1/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 upyTest-3.0.1/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:36:53.888637 upyTest-3.0.1/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      409 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2504 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2690 2023-03-15 10:38:40.000000 upyTest-3.0.1/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    15610 2023-03-25 14:55:16.000000 upyTest-3.0.1/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36655 2023-04-07 14:49:23.000000 upyTest-3.0.1/thonnycontrib/l1test_frontend/l1test_treeview.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2875 2023-04-20 19:27:21.000000 upyTest-3.0.1/thonnycontrib/outlines.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9844 2023-04-20 19:27:15.000000 upyTest-3.0.1/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2435 2023-03-25 19:48:01.000000 upyTest-3.0.1/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:36:53.888637 upyTest-3.0.1/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 upyTest-3.0.1/thonnycontrib/tests/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 upyTest-3.0.1/thonnycontrib/tests/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 upyTest-3.0.1/thonnycontrib/tests/test_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4853 2023-04-20 19:27:50.000000 upyTest-3.0.1/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14752 2023-04-20 21:19:23.000000 upyTest-3.0.1/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18493 2023-04-08 16:06:56.000000 upyTest-3.0.1/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9827 2023-03-15 10:38:42.000000 upyTest-3.0.1/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6388 2023-04-08 16:04:30.000000 upyTest-3.0.1/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12637 2023-03-15 10:38:42.000000 upyTest-3.0.1/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    20726 2023-04-08 15:48:58.000000 upyTest-3.0.1/thonnycontrib/utils.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:36:53.888637 upyTest-3.0.1/upyTest.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      712 2023-04-20 22:36:53.000000 upyTest-3.0.1/upyTest.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2109 2023-04-20 22:36:53.000000 upyTest-3.0.1/upyTest.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-04-20 22:36:53.000000 upyTest-3.0.1/upyTest.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-04-20 22:36:53.000000 upyTest-3.0.1/upyTest.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-04-20 22:36:53.000000 upyTest-3.0.1/upyTest.egg-info/top_level.txt
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.313171 UpyTest-3.0.2/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      712 2023-04-20 22:48:29.313171 UpyTest-3.0.2/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.289171 UpyTest-3.0.2/UpyTest.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      712 2023-04-20 22:48:29.000000 UpyTest-3.0.2/UpyTest.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2109 2023-04-20 22:48:29.000000 UpyTest-3.0.2/UpyTest.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-04-20 22:48:29.000000 UpyTest-3.0.2/UpyTest.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-04-20 22:48:29.000000 UpyTest-3.0.2/UpyTest.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-04-20 22:48:29.000000 UpyTest-3.0.2/UpyTest.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-04-20 22:48:29.313171 UpyTest-3.0.2/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-04-20 22:47:14.000000 UpyTest-3.0.2/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.297170 UpyTest-3.0.2/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      844 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-21 23:03:34.000000 UpyTest-3.0.2/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.305171 UpyTest-3.0.2/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7053 2023-04-20 20:40:22.000000 UpyTest-3.0.2/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35987 2023-04-20 22:46:44.000000 UpyTest-3.0.2/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8152 2023-04-18 20:16:40.000000 UpyTest-3.0.2/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4634 2023-04-19 22:19:22.000000 UpyTest-3.0.2/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7022 2023-04-18 20:05:18.000000 UpyTest-3.0.2/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.305171 UpyTest-3.0.2/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      488 2023-04-08 15:47:21.000000 UpyTest-3.0.2/thonnycontrib/backend/verdicts/EmptyTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      650 2023-03-19 17:23:31.000000 UpyTest-3.0.2/thonnycontrib/backend/verdicts/ExceptionTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      880 2023-03-19 17:23:26.000000 UpyTest-3.0.2/thonnycontrib/backend/verdicts/FailedTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      438 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      456 2023-03-21 23:57:32.000000 UpyTest-3.0.2/thonnycontrib/backend/verdicts/PassedTest.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2128 2023-03-19 18:06:02.000000 UpyTest-3.0.2/thonnycontrib/backend/verdicts/Test.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.309171 UpyTest-3.0.2/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.309171 UpyTest-3.0.2/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/res/test_only_btn.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.309171 UpyTest-3.0.2/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8661 2023-04-02 02:52:03.000000 UpyTest-3.0.2/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1464 2023-03-21 23:53:12.000000 UpyTest-3.0.2/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3917 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.309171 UpyTest-3.0.2/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.0.2/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.309171 UpyTest-3.0.2/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      409 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2504 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2690 2023-03-15 10:38:40.000000 UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    15610 2023-03-25 14:55:16.000000 UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36655 2023-04-07 14:49:23.000000 UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_treeview.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2875 2023-04-20 19:27:21.000000 UpyTest-3.0.2/thonnycontrib/outlines.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9844 2023-04-20 19:27:15.000000 UpyTest-3.0.2/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2435 2023-03-25 19:48:01.000000 UpyTest-3.0.2/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-04-20 22:48:29.313171 UpyTest-3.0.2/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.0.2/thonnycontrib/tests/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.0.2/thonnycontrib/tests/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.0.2/thonnycontrib/tests/test_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4853 2023-04-20 19:27:50.000000 UpyTest-3.0.2/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14752 2023-04-20 21:19:23.000000 UpyTest-3.0.2/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18493 2023-04-08 16:06:56.000000 UpyTest-3.0.2/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9827 2023-03-15 10:38:42.000000 UpyTest-3.0.2/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6388 2023-04-08 16:04:30.000000 UpyTest-3.0.2/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12637 2023-03-15 10:38:42.000000 UpyTest-3.0.2/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    20726 2023-04-08 15:48:58.000000 UpyTest-3.0.2/thonnycontrib/utils.py
```

### Comparing `upyTest-3.0.1/PKG-INFO` & `UpyTest-3.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: upyTest
-Version: 3.0.1
+Name: UpyTest
+Version: 3.0.2
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
 License: UNKNOWN
 Platform: Windows
 Platform: macOS
 Platform: Linux
```

### Comparing `upyTest-3.0.1/setup.py` & `UpyTest-3.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     other_packs = dict([(p, ["res/*"]) for p in packages if p.endswith("docs")])
     return py_packs | other_packs
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
-    name="upyTest",
-    version="3.0.1",
+    name="UpyTest",
+    version="3.0.2",
     author="Réda Id-taleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework""",
     url="https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `upyTest-3.0.1/thonnycontrib/ThonnyLogsGenerator.py` & `UpyTest-3.0.2/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/backend/ast_parser.py` & `UpyTest-3.0.2/thonnycontrib/backend/ast_parser.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/backend/doctest_parser.py` & `UpyTest-3.0.2/thonnycontrib/backend/doctest_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -583,15 +583,15 @@
             # Extract info from the regexp match.
             (source, options, want, exc_msg) = \
                 self._parse_example(m, name, invite, lineno)
             
             # Create an Example, and add it to the list.
             if not self._IS_BLANK_OR_COMMENT(source):
                 example = ExampleFactory(invite, name, source, want, exc_msg,
-                                         lineno=lineno, indent=min_indent+len(m.group('indent')),
+                                         lineno=lineno+1, indent=min_indent+len(m.group('indent')),
                                          options=options)
                        
                 output.append(example)
             # Update lineno (lines inside this example)
             lineno += string.count('\n', m.start(), m.end())
             # Update charno.
             charno = m.end()
```

### Comparing `upyTest-3.0.1/thonnycontrib/backend/evaluator.py` & `UpyTest-3.0.2/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/backend/l1test_backend.py` & `UpyTest-3.0.2/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/backend/test_finder.py` & `UpyTest-3.0.2/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/backend/verdicts/ExceptionTest.py` & `UpyTest-3.0.2/thonnycontrib/backend/verdicts/ExceptionTest.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/backend/verdicts/FailedTest.py` & `UpyTest-3.0.2/thonnycontrib/backend/verdicts/FailedTest.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/backend/verdicts/Test.py` & `UpyTest-3.0.2/thonnycontrib/backend/verdicts/Test.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/docs/res/failed.png` & `UpyTest-3.0.2/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/docs/res/l1test_icon.png` & `UpyTest-3.0.2/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/docs/res/l1test_icon_old.png` & `UpyTest-3.0.2/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/docs/res/passed.png` & `UpyTest-3.0.2/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/docs/res/pending_icon.png` & `UpyTest-3.0.2/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/docs/res/test_only_btn.png` & `UpyTest-3.0.2/thonnycontrib/docs/res/test_only_btn.png`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/docs/res/warning.png` & `UpyTest-3.0.2/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/docstring_generator/doc_generator.py` & `UpyTest-3.0.2/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/docstring_generator/doc_template.py` & `UpyTest-3.0.2/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/environement_vars.py` & `UpyTest-3.0.2/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/exceptions.py` & `UpyTest-3.0.2/thonnycontrib/exceptions.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/l1test_configuration/l1test_options.py` & `UpyTest-3.0.2/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/l1test_frontend/l1test_error_view.py` & `UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/l1test_frontend/l1test_reporter.py` & `UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/l1test_frontend/l1test_runner.py` & `UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/l1test_frontend/l1test_treeview.py` & `UpyTest-3.0.2/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/outlines.py` & `UpyTest-3.0.2/thonnycontrib/outlines.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/plugin_loader.py` & `UpyTest-3.0.2/thonnycontrib/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/properties.py` & `UpyTest-3.0.2/thonnycontrib/properties.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/tests/test_doc_generator.py` & `UpyTest-3.0.2/thonnycontrib/tests/test_doc_generator.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/tests/tests_example_no_expected.py` & `UpyTest-3.0.2/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/tests/tests_example_with_exception.py` & `UpyTest-3.0.2/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/tests/tests_example_with_expected.py` & `UpyTest-3.0.2/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/tests/tests_l1TestRunner.py` & `UpyTest-3.0.2/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/tests/tests_test_finder.py` & `UpyTest-3.0.2/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/tests/tests_view.py` & `UpyTest-3.0.2/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/thonnycontrib/utils.py` & `UpyTest-3.0.2/thonnycontrib/utils.py`

 * *Files identical despite different names*

### Comparing `upyTest-3.0.1/upyTest.egg-info/PKG-INFO` & `UpyTest-3.0.2/UpyTest.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: upyTest
-Version: 3.0.1
+Name: UpyTest
+Version: 3.0.2
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
 License: UNKNOWN
 Platform: Windows
 Platform: macOS
 Platform: Linux
```

### Comparing `upyTest-3.0.1/upyTest.egg-info/SOURCES.txt` & `UpyTest-3.0.2/UpyTest.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 setup.py
+UpyTest.egg-info/PKG-INFO
+UpyTest.egg-info/SOURCES.txt
+UpyTest.egg-info/dependency_links.txt
+UpyTest.egg-info/requires.txt
+UpyTest.egg-info/top_level.txt
 thonnycontrib/ThonnyLogsGenerator.py
 thonnycontrib/__init__.py
 thonnycontrib/environement_vars.py
 thonnycontrib/exceptions.py
 thonnycontrib/outlines.py
 thonnycontrib/plugin_loader.py
 thonnycontrib/properties.py
@@ -42,13 +47,8 @@
 thonnycontrib/tests/backend_mock.py
 thonnycontrib/tests/test_doc_generator.py
 thonnycontrib/tests/tests_example_no_expected.py
 thonnycontrib/tests/tests_example_with_exception.py
 thonnycontrib/tests/tests_example_with_expected.py
 thonnycontrib/tests/tests_l1TestRunner.py
 thonnycontrib/tests/tests_test_finder.py
-thonnycontrib/tests/tests_view.py
-upyTest.egg-info/PKG-INFO
-upyTest.egg-info/SOURCES.txt
-upyTest.egg-info/dependency_links.txt
-upyTest.egg-info/requires.txt
-upyTest.egg-info/top_level.txt
+thonnycontrib/tests/tests_view.py
```

