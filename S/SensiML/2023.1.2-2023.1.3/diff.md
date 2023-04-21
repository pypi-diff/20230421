# Comparing `tmp/SensiML-2023.1.2.tar.gz` & `tmp/SensiML-2023.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SensiML-2023.1.2.tar", last modified: Tue Feb 28 03:53:57 2023, max compression
+gzip compressed data, was "SensiML-2023.1.3.tar", last modified: Fri Apr 21 06:08:37 2023, max compression
```

## Comparing `SensiML-2023.1.2.tar` & `SensiML-2023.1.3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-02-28 03:53:57.908210 SensiML-2023.1.2/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2186 2022-02-08 07:37:16.000000 SensiML-2023.1.2/LICENSE
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1666 2023-02-28 03:53:57.908210 SensiML-2023.1.2/PKG-INFO
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1304 2022-02-03 00:12:15.000000 SensiML-2023.1.2/README.md
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-02-28 03:53:57.896210 SensiML-2023.1.2/SensiML.egg-info/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1666 2023-02-28 03:53:57.000000 SensiML-2023.1.2/SensiML.egg-info/PKG-INFO
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3072 2023-02-28 03:53:57.000000 SensiML-2023.1.2/SensiML.egg-info/SOURCES.txt
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        1 2023-02-28 03:53:57.000000 SensiML-2023.1.2/SensiML.egg-info/dependency_links.txt
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      157 2023-02-28 03:53:57.000000 SensiML-2023.1.2/SensiML.egg-info/requires.txt
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        8 2023-02-28 03:53:57.000000 SensiML-2023.1.2/SensiML.egg-info/top_level.txt
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-02-28 03:53:57.896210 SensiML-2023.1.2/sensiml/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      309 2022-09-07 03:55:16.000000 SensiML-2023.1.2/sensiml/__init__.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-02-28 03:53:57.900210 SensiML-2023.1.2/sensiml/base/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/base/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1061 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/base/exceptions.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     9828 2022-05-19 23:26:20.000000 SensiML-2023.1.2/sensiml/base/snippets.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    14417 2023-02-02 21:47:32.000000 SensiML-2023.1.2/sensiml/base/utility.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    29328 2023-02-28 03:42:07.000000 SensiML-2023.1.2/sensiml/client.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-02-28 03:53:57.900210 SensiML-2023.1.2/sensiml/connection/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      129 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/connection/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    18404 2023-02-28 03:42:07.000000 SensiML-2023.1.2/sensiml/connection/connection.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4730 2021-09-22 23:18:11.000000 SensiML-2023.1.2/sensiml/connection/connection_config.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      626 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/connection/errors.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-02-28 03:53:57.900210 SensiML-2023.1.2/sensiml/data/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/data/__init__.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-02-28 03:53:57.904210 SensiML-2023.1.2/sensiml/datamanager/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      583 2022-05-19 23:26:20.000000 SensiML-2023.1.2/sensiml/datamanager/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6285 2022-08-05 16:07:43.000000 SensiML-2023.1.2/sensiml/datamanager/base.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     9449 2023-02-28 03:42:07.000000 SensiML-2023.1.2/sensiml/datamanager/capture.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3853 2022-02-03 00:12:15.000000 SensiML-2023.1.2/sensiml/datamanager/capture_configuration.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3708 2022-02-03 00:12:15.000000 SensiML-2023.1.2/sensiml/datamanager/capture_configurations.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     8670 2023-02-28 03:42:07.000000 SensiML-2023.1.2/sensiml/datamanager/captures.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    11830 2022-02-03 00:12:15.000000 SensiML-2023.1.2/sensiml/datamanager/clientplatformdescription.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3505 2021-10-29 11:29:06.000000 SensiML-2023.1.2/sensiml/datamanager/clientplatformdescriptions.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    26226 2022-02-03 00:12:15.000000 SensiML-2023.1.2/sensiml/datamanager/confusion_matrix.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6017 2021-11-03 22:39:59.000000 SensiML-2023.1.2/sensiml/datamanager/custom_functions.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2089 2021-09-22 23:18:11.000000 SensiML-2023.1.2/sensiml/datamanager/deviceconfig.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      646 2021-09-22 23:18:11.000000 SensiML-2023.1.2/sensiml/datamanager/errors.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6796 2023-02-02 21:47:32.000000 SensiML-2023.1.2/sensiml/datamanager/featurefile.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4952 2023-02-02 21:47:32.000000 SensiML-2023.1.2/sensiml/datamanager/featurefiles.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2382 2022-03-23 19:36:48.000000 SensiML-2023.1.2/sensiml/datamanager/foundation_model.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6281 2021-11-03 22:39:59.000000 SensiML-2023.1.2/sensiml/datamanager/function.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    16530 2022-08-05 16:07:43.000000 SensiML-2023.1.2/sensiml/datamanager/functions.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    33872 2023-02-02 21:47:32.000000 SensiML-2023.1.2/sensiml/datamanager/knowledgepack.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5024 2022-10-03 21:54:12.000000 SensiML-2023.1.2/sensiml/datamanager/label.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5519 2022-08-05 16:07:43.000000 SensiML-2023.1.2/sensiml/datamanager/labelvalue.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3907 2021-09-22 23:18:11.000000 SensiML-2023.1.2/sensiml/datamanager/library_pack.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1179 2022-10-03 21:54:12.000000 SensiML-2023.1.2/sensiml/datamanager/metadata.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     7277 2022-10-03 21:54:12.000000 SensiML-2023.1.2/sensiml/datamanager/metadata_relationship.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2341 2021-09-22 23:18:11.000000 SensiML-2023.1.2/sensiml/datamanager/metadata_value.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    17361 2022-02-03 00:12:15.000000 SensiML-2023.1.2/sensiml/datamanager/modelresults.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2843 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/datamanager/pipeline.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    14633 2023-02-02 21:47:32.000000 SensiML-2023.1.2/sensiml/datamanager/project.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4089 2022-03-02 07:28:57.000000 SensiML-2023.1.2/sensiml/datamanager/projects.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5226 2022-02-15 23:58:11.000000 SensiML-2023.1.2/sensiml/datamanager/queries.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    19674 2022-02-15 23:58:11.000000 SensiML-2023.1.2/sensiml/datamanager/query.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    31933 2023-02-02 21:47:32.000000 SensiML-2023.1.2/sensiml/datamanager/sandbox.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3615 2022-03-02 07:28:57.000000 SensiML-2023.1.2/sensiml/datamanager/sandboxes.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5660 2022-08-05 16:07:43.000000 SensiML-2023.1.2/sensiml/datamanager/segment.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4223 2021-09-22 23:18:11.000000 SensiML-2023.1.2/sensiml/datamanager/segmenter.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1041 2022-11-18 15:39:39.000000 SensiML-2023.1.2/sensiml/datamanager/team.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     7885 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/datasets.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-02-28 03:53:57.904210 SensiML-2023.1.2/sensiml/dclproj/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      570 2023-02-28 03:42:07.000000 SensiML-2023.1.2/sensiml/dclproj/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    27439 2023-02-28 03:42:07.000000 SensiML-2023.1.2/sensiml/dclproj/confusion_matrix.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3901 2022-04-07 18:29:01.000000 SensiML-2023.1.2/sensiml/dclproj/csv_to_dcli.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    33503 2023-02-28 03:42:07.000000 SensiML-2023.1.2/sensiml/dclproj/datasegments.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    20937 2023-02-28 03:42:07.000000 SensiML-2023.1.2/sensiml/dclproj/dclproj.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    10783 2023-02-28 03:42:07.000000 SensiML-2023.1.2/sensiml/dclproj/upload.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    13292 2023-02-28 03:42:07.000000 SensiML-2023.1.2/sensiml/dclproj/utils.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3376 2023-02-28 03:42:07.000000 SensiML-2023.1.2/sensiml/dclproj/vizualization.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-02-28 03:53:57.904210 SensiML-2023.1.2/sensiml/image/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/image/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    14012 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/image/sensiml.png
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-02-28 03:53:57.908210 SensiML-2023.1.2/sensiml/method_calls/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1434 2022-08-05 16:07:43.000000 SensiML-2023.1.2/sensiml/method_calls/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      650 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/method_calls/augmentationcall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3481 2021-09-22 23:18:11.000000 SensiML-2023.1.2/sensiml/method_calls/augmentationcallset.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      783 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/method_calls/basemethodcall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1533 2022-08-05 16:07:43.000000 SensiML-2023.1.2/sensiml/method_calls/capturefilecall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      294 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/method_calls/classifiercall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1659 2022-08-05 16:07:43.000000 SensiML-2023.1.2/sensiml/method_calls/datafilecall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2042 2022-08-05 16:07:43.000000 SensiML-2023.1.2/sensiml/method_calls/featurefilecall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2029 2021-09-22 23:18:11.000000 SensiML-2023.1.2/sensiml/method_calls/functioncall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1160 2021-09-22 23:18:11.000000 SensiML-2023.1.2/sensiml/method_calls/functioncalls.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      756 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/method_calls/generatorcall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2563 2021-09-22 23:18:11.000000 SensiML-2023.1.2/sensiml/method_calls/generatorcallset.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      408 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/method_calls/optimizercall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1142 2021-07-29 17:52:20.000000 SensiML-2023.1.2/sensiml/method_calls/querycall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      642 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/method_calls/selectorcall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4401 2021-09-22 23:18:11.000000 SensiML-2023.1.2/sensiml/method_calls/selectorcallset.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4857 2021-09-22 23:18:11.000000 SensiML-2023.1.2/sensiml/method_calls/trainandvalidationcall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      463 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/method_calls/trainingalgorithmcall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      429 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/method_calls/validationmethodcall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    58121 2022-10-19 15:09:13.000000 SensiML-2023.1.2/sensiml/pipeline.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-02-28 03:53:57.908210 SensiML-2023.1.2/sensiml/profile/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       91 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/profile/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6739 2021-07-29 17:52:20.000000 SensiML-2023.1.2/sensiml/profile/profile_data_parser.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       97 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/render.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    39041 2023-02-28 03:42:07.000000 SensiML-2023.1.2/sensiml/sml_runner.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-02-28 03:53:57.908210 SensiML-2023.1.2/sensiml/tensorflow/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/tensorflow/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6619 2021-11-29 20:51:38.000000 SensiML-2023.1.2/sensiml/tensorflow/utils.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-02-28 03:53:57.908210 SensiML-2023.1.2/sensiml/visualize/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       80 2021-07-02 06:14:18.000000 SensiML-2023.1.2/sensiml/visualize/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1170 2021-10-29 11:29:06.000000 SensiML-2023.1.2/sensiml/visualize/knowledgepack_visualize_mixin.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    14329 2022-02-03 00:12:15.000000 SensiML-2023.1.2/sensiml/visualize/visualize.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       38 2023-02-28 03:53:57.908210 SensiML-2023.1.2/setup.cfg
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1479 2023-02-28 03:42:07.000000 SensiML-2023.1.2/setup.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-04-21 06:08:36.994924 SensiML-2023.1.3/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2186 2022-02-07 08:21:21.000000 SensiML-2023.1.3/LICENSE
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1666 2023-04-21 06:08:36.994924 SensiML-2023.1.3/PKG-INFO
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1304 2022-01-31 22:03:39.000000 SensiML-2023.1.3/README.md
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-04-21 06:08:36.978924 SensiML-2023.1.3/SensiML.egg-info/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1666 2023-04-21 06:08:36.000000 SensiML-2023.1.3/SensiML.egg-info/PKG-INFO
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3072 2023-04-21 06:08:36.000000 SensiML-2023.1.3/SensiML.egg-info/SOURCES.txt
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        1 2023-04-21 06:08:36.000000 SensiML-2023.1.3/SensiML.egg-info/dependency_links.txt
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      157 2023-04-21 06:08:36.000000 SensiML-2023.1.3/SensiML.egg-info/requires.txt
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        8 2023-04-21 06:08:36.000000 SensiML-2023.1.3/SensiML.egg-info/top_level.txt
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-04-21 06:08:36.978924 SensiML-2023.1.3/sensiml/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      309 2022-09-16 19:38:41.000000 SensiML-2023.1.3/sensiml/__init__.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-04-21 06:08:36.982924 SensiML-2023.1.3/sensiml/base/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2022-01-10 22:12:20.000000 SensiML-2023.1.3/sensiml/base/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1061 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/base/exceptions.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    10583 2023-04-10 19:43:04.000000 SensiML-2023.1.3/sensiml/base/snippets.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    14417 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/base/utility.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    29328 2023-04-14 19:03:50.000000 SensiML-2023.1.3/sensiml/client.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-04-21 06:08:36.982924 SensiML-2023.1.3/sensiml/connection/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      129 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/connection/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    18404 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/connection/connection.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4730 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/connection/connection_config.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      626 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/connection/errors.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-04-21 06:08:36.982924 SensiML-2023.1.3/sensiml/data/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2022-01-10 22:12:20.000000 SensiML-2023.1.3/sensiml/data/__init__.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-04-21 06:08:36.990924 SensiML-2023.1.3/sensiml/datamanager/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      583 2022-06-17 19:04:08.000000 SensiML-2023.1.3/sensiml/datamanager/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6285 2022-08-04 23:19:27.000000 SensiML-2023.1.3/sensiml/datamanager/base.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     9449 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/datamanager/capture.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3853 2022-01-31 04:51:43.000000 SensiML-2023.1.3/sensiml/datamanager/capture_configuration.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3708 2022-01-31 04:51:43.000000 SensiML-2023.1.3/sensiml/datamanager/capture_configurations.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     8670 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/datamanager/captures.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    11830 2022-01-31 04:51:43.000000 SensiML-2023.1.3/sensiml/datamanager/clientplatformdescription.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3505 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/datamanager/clientplatformdescriptions.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    26226 2022-01-31 04:51:43.000000 SensiML-2023.1.3/sensiml/datamanager/confusion_matrix.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6017 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/datamanager/custom_functions.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2089 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/datamanager/deviceconfig.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      646 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/datamanager/errors.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6796 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/datamanager/featurefile.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4952 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/datamanager/featurefiles.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2382 2022-06-17 19:04:08.000000 SensiML-2023.1.3/sensiml/datamanager/foundation_model.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6281 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/datamanager/function.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    16530 2022-08-04 23:19:27.000000 SensiML-2023.1.3/sensiml/datamanager/functions.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    33872 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/datamanager/knowledgepack.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5024 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/datamanager/label.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5519 2022-08-04 23:19:27.000000 SensiML-2023.1.3/sensiml/datamanager/labelvalue.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3907 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/datamanager/library_pack.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1179 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/datamanager/metadata.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     7277 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/datamanager/metadata_relationship.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2341 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/datamanager/metadata_value.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    17363 2023-04-10 19:43:04.000000 SensiML-2023.1.3/sensiml/datamanager/modelresults.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2843 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/datamanager/pipeline.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    14633 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/datamanager/project.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4089 2022-08-15 05:43:24.000000 SensiML-2023.1.3/sensiml/datamanager/projects.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5226 2022-03-02 05:46:49.000000 SensiML-2023.1.3/sensiml/datamanager/queries.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    19674 2022-02-15 23:01:31.000000 SensiML-2023.1.3/sensiml/datamanager/query.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    31933 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/datamanager/sandbox.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3615 2022-03-03 21:36:41.000000 SensiML-2023.1.3/sensiml/datamanager/sandboxes.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5660 2022-08-04 23:19:27.000000 SensiML-2023.1.3/sensiml/datamanager/segment.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4223 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/datamanager/segmenter.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1041 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/datamanager/team.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     7885 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/datasets.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-04-21 06:08:36.990924 SensiML-2023.1.3/sensiml/dclproj/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      570 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/dclproj/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    27439 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/dclproj/confusion_matrix.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3901 2022-06-17 19:04:08.000000 SensiML-2023.1.3/sensiml/dclproj/csv_to_dcli.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    33503 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/dclproj/datasegments.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    21333 2023-04-12 19:59:21.000000 SensiML-2023.1.3/sensiml/dclproj/dclproj.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    11206 2023-04-12 19:59:21.000000 SensiML-2023.1.3/sensiml/dclproj/upload.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    13292 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/dclproj/utils.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3397 2023-03-07 20:40:35.000000 SensiML-2023.1.3/sensiml/dclproj/vizualization.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-04-21 06:08:36.990924 SensiML-2023.1.3/sensiml/image/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2022-01-10 22:12:20.000000 SensiML-2023.1.3/sensiml/image/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    14012 2022-01-10 22:12:20.000000 SensiML-2023.1.3/sensiml/image/sensiml.png
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-04-21 06:08:36.994924 SensiML-2023.1.3/sensiml/method_calls/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1434 2022-08-04 23:19:27.000000 SensiML-2023.1.3/sensiml/method_calls/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      650 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/method_calls/augmentationcall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3425 2023-04-10 19:43:04.000000 SensiML-2023.1.3/sensiml/method_calls/augmentationcallset.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      783 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/method_calls/basemethodcall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1533 2022-08-04 23:19:27.000000 SensiML-2023.1.3/sensiml/method_calls/capturefilecall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      294 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/method_calls/classifiercall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1659 2022-08-04 23:19:27.000000 SensiML-2023.1.3/sensiml/method_calls/datafilecall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2042 2022-08-04 23:19:27.000000 SensiML-2023.1.3/sensiml/method_calls/featurefilecall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2029 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/method_calls/functioncall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1160 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/method_calls/functioncalls.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      756 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/method_calls/generatorcall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2563 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/method_calls/generatorcallset.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      408 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/method_calls/optimizercall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1142 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/method_calls/querycall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      642 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/method_calls/selectorcall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4401 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/method_calls/selectorcallset.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4857 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/method_calls/trainandvalidationcall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      463 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/method_calls/trainingalgorithmcall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      429 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/method_calls/validationmethodcall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    59026 2023-04-10 19:43:04.000000 SensiML-2023.1.3/sensiml/pipeline.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-04-21 06:08:36.994924 SensiML-2023.1.3/sensiml/profile/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       91 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/profile/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6739 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/profile/profile_data_parser.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       97 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/render.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    39305 2023-04-21 02:00:40.000000 SensiML-2023.1.3/sensiml/sml_runner.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-04-21 06:08:36.994924 SensiML-2023.1.3/sensiml/tensorflow/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/tensorflow/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6619 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/tensorflow/utils.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-04-21 06:08:36.994924 SensiML-2023.1.3/sensiml/visualize/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       80 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/visualize/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1170 2022-01-24 22:04:38.000000 SensiML-2023.1.3/sensiml/visualize/knowledgepack_visualize_mixin.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    14329 2022-01-31 04:51:43.000000 SensiML-2023.1.3/sensiml/visualize/visualize.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       38 2023-04-21 06:08:36.994924 SensiML-2023.1.3/setup.cfg
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1479 2023-04-14 19:03:50.000000 SensiML-2023.1.3/setup.py
```

### Comparing `SensiML-2023.1.2/LICENSE` & `SensiML-2023.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/PKG-INFO` & `SensiML-2023.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SensiML
-Version: 2023.1.2
+Version: 2023.1.3
 Summary: SensiML Python SDK
 Home-page: UNKNOWN
 Author: SensiML
 Author-email: support@sensiml.com
 License: Proprietary
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `SensiML-2023.1.2/README.md` & `SensiML-2023.1.3/README.md`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/SensiML.egg-info/PKG-INFO` & `SensiML-2023.1.3/SensiML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SensiML
-Version: 2023.1.2
+Version: 2023.1.3
 Summary: SensiML Python SDK
 Home-page: UNKNOWN
 Author: SensiML
 Author-email: support@sensiml.com
 License: Proprietary
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `SensiML-2023.1.2/SensiML.egg-info/SOURCES.txt` & `SensiML-2023.1.3/SensiML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/base/exceptions.py` & `SensiML-2023.1.3/sensiml/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/base/snippets.py` & `SensiML-2023.1.3/sensiml/base/snippets.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,19 @@
         )
 
     if func.type == "Feature Selector":
         return """client.pipeline.add_feature_selector([{{'name':'{}', 'params':{{{}}}}}], params={{'number_of_features':(int)}})""".format(
             func.name, param_tabs.join(params)
         )
 
+    if func.type == "Augmentation":
+        return """client.pipeline.add_augmentation(["name":"{}", "params":{{{}}}])""".format(
+            func.name, param_tabs.join(params)
+        )
+
     if func.type in ["Segmenter", "Transform", "Sampler"]:
         return """client.pipeline.add_transform("{}", params={{{}}})""".format(
             func.name, param_tabs.join(params)
         )
 
     if func.type == "Training Algorithm":
         return """client.pipeline.set_training_algorithm("{}", params={{{}}})""".format(
@@ -194,14 +199,19 @@
         )
 
     if func.type == "Feature Selector":
         return """{{'name':'{}', 'params':{{{}}}}}, """.format(
             func.name, param_tabs.join(params)
         )
 
+    if func.type == "Augmentation":
+        return """\n{}{{"name": "{}", "params": {{{}}}}},""".format(
+            " " * 32, func.name, param_tabs.join(params)
+        )
+
     if func.type in ["Segmenter", "Transform", "Sampler"]:
         return """client.pipeline.add_transform("{}", params={{{}}})""".format(
             func.name, param_tabs.join(params)
         )
 
     if func.type == "Training Algorithm":
         return """client.pipeline.set_training_algorithm("{}", params={{{}}})""".format(
@@ -244,14 +254,23 @@
                     pipeline_function_help(function_list, selector)
                 )
             pipeline_steps.append(
                 "client.pipeline.add_feature_selector([{}])"
                 "".format("\n{}".format(" " * 40).join(feature_selectors))
             )
 
+        elif step.get("type") == "augmentationset":
+            data_augmentors = []
+            for augmentor in step["set"]:
+                data_augmentors.append(pipeline_function_help(function_list, augmentor))
+            pipeline_steps.append(
+                "client.pipeline.add_augmentation([{}])"
+                "".format("{}".format(" " * 40).join(data_augmentors))
+            )
+
         elif step.get("type") == "tvo":
             for key in ["classifiers", "validation_methods", "optimizers"]:
                 if step[key]:
                     pipeline_steps.append(
                         pipeline_function_help(function_list, step[key][0])
                     )
```

### Comparing `SensiML-2023.1.2/sensiml/base/utility.py` & `SensiML-2023.1.3/sensiml/base/utility.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/client.py` & `SensiML-2023.1.3/sensiml/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 SERVER_URL = "https://sensiml.cloud/"
 
 AUTH2_PRIMARY = True
 
 logger = logging.getLogger("SensiML")
 
-__version__ = "2023.1.2"
+__version__ = "2023.1.3"
 
 
 def project_set(func):
     def wrapper(*args, **kwargs):
         self = args[0]
         if self._project is None:
             print("Project must be set.")
```

### Comparing `SensiML-2023.1.2/sensiml/connection/connection.py` & `SensiML-2023.1.3/sensiml/connection/connection.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/connection/connection_config.py` & `SensiML-2023.1.3/sensiml/connection/connection_config.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/connection/errors.py` & `SensiML-2023.1.3/sensiml/connection/errors.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/__init__.py` & `SensiML-2023.1.3/sensiml/datamanager/__init__.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/base.py` & `SensiML-2023.1.3/sensiml/datamanager/base.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/capture.py` & `SensiML-2023.1.3/sensiml/datamanager/capture.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/capture_configuration.py` & `SensiML-2023.1.3/sensiml/datamanager/capture_configuration.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/capture_configurations.py` & `SensiML-2023.1.3/sensiml/datamanager/capture_configurations.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/captures.py` & `SensiML-2023.1.3/sensiml/datamanager/captures.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/clientplatformdescription.py` & `SensiML-2023.1.3/sensiml/datamanager/clientplatformdescription.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/clientplatformdescriptions.py` & `SensiML-2023.1.3/sensiml/datamanager/clientplatformdescriptions.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/confusion_matrix.py` & `SensiML-2023.1.3/sensiml/datamanager/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/custom_functions.py` & `SensiML-2023.1.3/sensiml/datamanager/custom_functions.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/deviceconfig.py` & `SensiML-2023.1.3/sensiml/datamanager/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/errors.py` & `SensiML-2023.1.3/sensiml/datamanager/errors.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/featurefile.py` & `SensiML-2023.1.3/sensiml/datamanager/featurefile.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/featurefiles.py` & `SensiML-2023.1.3/sensiml/datamanager/featurefiles.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/foundation_model.py` & `SensiML-2023.1.3/sensiml/datamanager/foundation_model.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/function.py` & `SensiML-2023.1.3/sensiml/datamanager/function.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/functions.py` & `SensiML-2023.1.3/sensiml/datamanager/functions.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/knowledgepack.py` & `SensiML-2023.1.3/sensiml/datamanager/knowledgepack.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/label.py` & `SensiML-2023.1.3/sensiml/datamanager/label.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/labelvalue.py` & `SensiML-2023.1.3/sensiml/datamanager/labelvalue.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/library_pack.py` & `SensiML-2023.1.3/sensiml/datamanager/library_pack.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/metadata.py` & `SensiML-2023.1.3/sensiml/datamanager/metadata.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/metadata_relationship.py` & `SensiML-2023.1.3/sensiml/datamanager/metadata_relationship.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/metadata_value.py` & `SensiML-2023.1.3/sensiml/datamanager/metadata_value.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/modelresults.py` & `SensiML-2023.1.3/sensiml/datamanager/modelresults.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import json
-from pandas import DataFrame, Series
-from numpy import NaN
 import logging
+
+from numpy import NaN
+from pandas import DataFrame, Series
+
+import sensiml.base.utility as utility
 from sensiml.datamanager.confusion_matrix import (
     ConfusionMatrix,
     ConfusionMatrixException,
 )
-import sensiml.base.utility as utility
 
 logger = logging.getLogger("ModelMetrics")
 
 
 METRICS = [
     "f1_score",
     "precision",
```

### Comparing `SensiML-2023.1.2/sensiml/datamanager/pipeline.py` & `SensiML-2023.1.3/sensiml/datamanager/pipeline.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/project.py` & `SensiML-2023.1.3/sensiml/datamanager/project.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/projects.py` & `SensiML-2023.1.3/sensiml/datamanager/projects.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/queries.py` & `SensiML-2023.1.3/sensiml/datamanager/queries.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/query.py` & `SensiML-2023.1.3/sensiml/datamanager/query.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/sandbox.py` & `SensiML-2023.1.3/sensiml/datamanager/sandbox.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/sandboxes.py` & `SensiML-2023.1.3/sensiml/datamanager/sandboxes.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/segment.py` & `SensiML-2023.1.3/sensiml/datamanager/segment.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/segmenter.py` & `SensiML-2023.1.3/sensiml/datamanager/segmenter.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datamanager/team.py` & `SensiML-2023.1.3/sensiml/datamanager/team.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/datasets.py` & `SensiML-2023.1.3/sensiml/datasets.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/dclproj/__init__.py` & `SensiML-2023.1.3/sensiml/dclproj/__init__.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/dclproj/confusion_matrix.py` & `SensiML-2023.1.3/sensiml/dclproj/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/dclproj/csv_to_dcli.py` & `SensiML-2023.1.3/sensiml/dclproj/csv_to_dcli.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/dclproj/datasegments.py` & `SensiML-2023.1.3/sensiml/dclproj/datasegments.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/dclproj/dclproj.py` & `SensiML-2023.1.3/sensiml/dclproj/dclproj.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from collections import OrderedDict
 from typing import Dict, List, Optional, Tuple
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from pandas.core.frame import DataFrame
+
 from sensiml.dclproj.datasegments import (
-    DataSegments,
     DataSegment,
+    DataSegments,
     segment_list_to_datasegments,
 )
 from sensiml.dclproj.utils import mfcc, plot_segments_labels
 from sensiml.dclproj.vizualization import plot_segments
 
 
 class DCLProject:
@@ -126,31 +127,35 @@
             }
             df["local_status"] = (
                 df["local_status"].fillna("Synced").apply(lambda x: local_status[x])
             )
 
         return df
 
-    def _list_table_raw(self, tablename: str) -> DataFrame:
+    def _list_table_raw(self, tablename: str, filter_deleted: bool = True) -> DataFrame:
 
         if tablename not in self._tables:
             print("Table is not part of the database.")
             return None
 
         query = "SELECT * FROM {tablename} ".format(tablename=tablename)
 
+        if filter_deleted:
+            query += f"WHERE ({tablename}.local_status != 2 OR {tablename}.local_status IS NULL)"
+
         return self._execute_query(query)
 
     def _list_table(
         self,
         tablename: str,
         fields: List[str],
         fk_fields: Optional[Dict] = None,
         query_filter: Optional[str] = None,
         header=None,
+        filter_deleted: bool = True,
     ):
 
         if tablename not in self._tables:
             print("Table is not part of the database.")
             return None
 
         select_fields = ", ".join(
@@ -173,26 +178,31 @@
 
         query_join = ""
 
         if fk_fields:
             join_fields = []
             for fk_table, fk_field in fk_fields.items():
                 join_fields.append(
-                    "JOIN {fk_table} ON {fk_table}.id = {tablename}.{fk_field} ".format(
+                    "LEFT JOIN {fk_table} ON {fk_table}.id = {tablename}.{fk_field} ".format(
                         fk_table=fk_table, tablename=tablename, fk_field=fk_field
                     )
                 )
             query_join += " ".join(join_fields)
 
-        if query_filter:
-            query_where = (
-                query_filter  # + "AND {}.local_status != 2 ".format(tablename)
+        if query_filter and filter_deleted:
+            query_where = " ".join(
+                [
+                    query_filter,
+                    f"AND ({tablename}.local_status != 2  OR {tablename}.local_status IS NULL)",
+                ]
             )
+        elif filter_deleted:
+            query_where = f" WHERE ({tablename}.local_status != 2  OR {tablename}.local_status IS NULL)"
         else:
-            query_where = ""  # "WHERE {}.local_status != 2 ".format(tablename)
+            query_where = " "
 
         if fk_fields and not header:
             header = fields + list(fk_fields.values())
 
         return self._execute_query(query_select + query_join + query_where, header)
 
     def _list_captures_metadata(self) -> DataFrame:
```

### Comparing `SensiML-2023.1.2/sensiml/dclproj/upload.py` & `SensiML-2023.1.3/sensiml/dclproj/upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from sensiml.datamanager.labelvalue import LabelValue
 from sensiml.datamanager.metadata import Metadata
 from sensiml.datamanager.metadata_relationship import MetadataRelationship
 from sensiml.datamanager.metadata_value import MetadataValue
 from sensiml.datamanager.segment import Segment
 from sensiml.dclproj import DCLProject
 
-
 color_list = [
     "#FF1D7DC4",
     "#FF58D963",
     "#FFF49534",
     "#FF7754AB",
     "#FFD14D49",
     "#FFC8CF4E",
@@ -44,15 +43,15 @@
     # TODO: plugin config
     # plugin_config = dclproj.get("ProjectCapturePluginConfig", None)
     # if plugin_config is not None:
     #    client.project.plugin_config = plugin_config
     #    print("Capture Config Found, Updating...")
     #    client.project.update()
 
-    session_set = []
+    session_set = {}
     for _, session in dclproj.list_sessions().iterrows():
         if session["parameters"]:
             params = json.loads(session["parameters"])
             call = client.functions.create_function_call(params["name"])
             for k, v in params["inputs"].items():
                 setattr(call, k, v)
         else:
@@ -60,15 +59,15 @@
 
         new_segmenter = client.project.add_segmenter(
             session["name"],
             call,
             preprocess=session["preprocess"],
             custom=True if session["parameters"] else False,
         )
-        session_set.append(new_segmenter)
+        session_set[session["id"]] = new_segmenter
 
     label_set = {}
 
     for _, item in dclproj._list_table_raw("Label").iterrows():
         if item["metadata"] == 0:
             label = Label(client._connection, client.project)
             label.name = item["name"]
@@ -131,23 +130,37 @@
 
         # TODO: Bulk label creation
         for _, label_relationship in dclproj.list_capture_segments(
             capture["name"], include_ids=True
         ).iterrows():
             label_value = label_value_set[label_relationship["label_value_id"]]
             label = label_set[label_relationship["label_id"]]
-            segmenter = session_set[label_relationship["segmenter_id"] - 1]["id"]
+
+            if not session_set.get(label_relationship["segmenter_id"], None):
+                continue
+
+            segmenter = session_set[label_relationship["segmenter_id"]]["id"]
             label_relationship_obj = Segment(
                 client._connection,
                 client.project,
                 capture_obj,
                 segmenter,
                 label,
                 label_value,
             )
+
+            if (
+                label_relationship["capture_sample_sequence_start"] < 0
+                or label_relationship["capture_sample_sequence_end"]
+                <= label_relationship["capture_sample_sequence_start"]
+            ):
+                print("Invalid Segment: Skipping")
+                print(label_relationship)
+                continue
+
             label_relationship_obj.sample_start = label_relationship[
                 "capture_sample_sequence_start"
             ]
             label_relationship_obj.sample_end = label_relationship[
                 "capture_sample_sequence_end"
             ]
             label_relationship_obj.insert()
@@ -170,17 +183,15 @@
     color_index = {}
     for capture_info in dcli:
 
         if not os.path.exists(os.path.join(capture_dir, capture_info["file_name"])):
             print(f"Skipping: Capture {capture_info['file_name']} not found.")
             continue
 
-        print(
-            f"Uploading Capture {capture_info['file_name']}, data, metadata, and labels"
-        )
+        print(f"Uploading Capture {capture_info['file_name']}")
         capture_obj = client.project.captures.create_capture(
             os.path.basename(capture_info["file_name"]),
             os.path.join(capture_dir, capture_info["file_name"]),
         )
 
         if capture_info.get("metadata"):
             for metadata in capture_info["metadata"]:
```

### Comparing `SensiML-2023.1.2/sensiml/dclproj/utils.py` & `SensiML-2023.1.3/sensiml/dclproj/utils.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/dclproj/vizualization.py` & `SensiML-2023.1.3/sensiml/dclproj/vizualization.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     capture,
     column,
     datasegments=None,
     labels=None,
     threshold_type="sum",
     threshold_width=25,
     xlim=None,
+    figsize=(16, 4),
 ):
     M = []
     for i in range(capture.shape[0]):
         if threshold_type == "absolute sum":
             M.append(np.abs(capture[column].values[i : i + threshold_width]).sum())
         elif threshold_type == "sum":
             M.append(capture[column].values[i : i + threshold_width].sum())
@@ -112,16 +113,16 @@
         else:
             print("Invalid threshold type")
             return
 
     test_capture = pd.DataFrame(M)
     if xlim is None:
         xlim = (0, len(M))
-    ax = test_capture.plot(figsize=(30, 4), xlim=xlim)
+    ax = test_capture.plot(figsize=figsize, xlim=xlim)
     if datasegments is not None:
         datasegments.plot_segments(
-            figsize=(30, 4),
+            figsize=figsize,
             capture=test_capture,
             currentAxis=ax,
             labels=labels,
             xlim=xlim,
         )
```

### Comparing `SensiML-2023.1.2/sensiml/image/sensiml.png` & `SensiML-2023.1.3/sensiml/image/sensiml.png`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/method_calls/__init__.py` & `SensiML-2023.1.3/sensiml/method_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/method_calls/augmentationcall.py` & `SensiML-2023.1.3/sensiml/method_calls/augmentationcall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/method_calls/augmentationcallset.py` & `SensiML-2023.1.3/sensiml/method_calls/augmentationcallset.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,13 +112,12 @@
             self, "_passthrough_columns"
         )
         set_dict["inputs"]["label_column"] = getattr(self, "_label_column")
 
         set_dict["inputs"]["group_columns"] = getattr(self, "_group_columns")
 
         set_dict["inputs"]["input_data"] = getattr(self, "_input_data")
-        set_dict["percent"] = getattr(self, "_percent")
         set_dict["label_column"] = getattr(self, "_label_column")
 
         set_dict["outputs"] = self._outputs
 
         return set_dict
```

### Comparing `SensiML-2023.1.2/sensiml/method_calls/basemethodcall.py` & `SensiML-2023.1.3/sensiml/method_calls/basemethodcall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/method_calls/capturefilecall.py` & `SensiML-2023.1.3/sensiml/method_calls/capturefilecall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/method_calls/datafilecall.py` & `SensiML-2023.1.3/sensiml/method_calls/datafilecall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/method_calls/featurefilecall.py` & `SensiML-2023.1.3/sensiml/method_calls/featurefilecall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/method_calls/functioncall.py` & `SensiML-2023.1.3/sensiml/method_calls/functioncall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/method_calls/functioncalls.py` & `SensiML-2023.1.3/sensiml/method_calls/functioncalls.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/method_calls/generatorcall.py` & `SensiML-2023.1.3/sensiml/method_calls/generatorcall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/method_calls/generatorcallset.py` & `SensiML-2023.1.3/sensiml/method_calls/generatorcallset.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/method_calls/querycall.py` & `SensiML-2023.1.3/sensiml/method_calls/querycall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/method_calls/selectorcall.py` & `SensiML-2023.1.3/sensiml/method_calls/selectorcall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/method_calls/selectorcallset.py` & `SensiML-2023.1.3/sensiml/method_calls/selectorcallset.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/method_calls/trainandvalidationcall.py` & `SensiML-2023.1.3/sensiml/method_calls/trainandvalidationcall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/pipeline.py` & `SensiML-2023.1.3/sensiml/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -870,44 +870,50 @@
         """Add a step to the pipeline. Automatically tie the previous step and current step.
 
         Args:
             func (function): A sensiml function method call
         """
         self._sandbox.add_linear_step(func)
 
-    def add_segmenter(self, name, params={}):
+    def add_segmenter(self, name, params=None):
         """Add a Segmenter to the pipeline.
 
         Args:
             name (str): Name of the segmenter method to add.
             params (dict, optional): Dictionary containing the parameters of the transform.
 
         """
 
+        if params is None:
+            params = {}
+
         self._add_transform({"name": name, "params": params})
 
-    def add_transform(self, name, params={}, overwrite=True):
+    def add_transform(self, name, params=None, overwrite=True):
         """Add a Transform to the pipeline.
 
         Args:
             name (str): Name of the transform method to add.
             params (dict, optional): Dictionary containing the parameters of the transform.
             overwrite (boolean): when adding multiple instances of the same transform, set
                 overwrite to False for the additional steps and the first instance will not
                 be overwritten (default is True)
 
         """
 
+        if params is None:
+            params = {}
+
         self._add_transform({"name": name, "params": params}, overwrite)
 
     def add_feature_generator(
         self,
         feature_generators,
-        params={},
-        function_defaults={},
+        params=None,
+        function_defaults=None,
         return_generator_set=False,
     ):
         """Add a feature generator set to the pipeline.
 
         Args:
             feature_generators (list): List of feature generators. As names or dictionaries.
             params (dict, {}}): Parameters to apply to the feature generator set.
@@ -950,14 +956,21 @@
             >>> client.pipeline.add_feature_generator([{'name': 'Downsample', 'params': {'new_length': 5, 'columns': sensor_columns[0]}},
                                                     {'name': 'Downsample', 'params': {'new_length': 12}},
                                                     ],
                                                     function_defaults={'columns': sensor_columns},
                                                     )
 
         """
+
+        if params is None:
+            params = {}
+
+        if function_defaults is None:
+            function_defaults = {}
+
         # if we get a list of strings
         feature_generators = copy.deepcopy(feature_generators)
         if isinstance(feature_generators[0], str):
             feature_generators = list(
                 map(lambda x: {"name": x, "params": {}}, feature_generators)
             )
             for fg in feature_generators:
@@ -986,68 +999,85 @@
                 "Feature Generator was improperly specified. See Documentation (client.pipeline.add_feature_generator?) for examples."
             )
 
         return self._add_feature_generator(
             feature_generators, params, return_generator_set=return_generator_set
         )
 
-    def add_feature_selector(self, feature_selectors, params={}):
+    def add_feature_selector(self, feature_selectors, params=None):
         """Add a feature selection set to the pipeline.
 
         Args:
             feature_selectors (List): List of dictionaries containing feature selectors
             params (dict, {}): Parameters of the feature selector set.
 
         Examples:
             >>> client.pipeline.add_feature_selector([{"name":"Recursive Feature Elimination", "params":{"method":"Log R"}}],
             >>>                                    params = {"number_of_features":20})
         """
 
+        if params is None:
+            params = {}
+
         self._add_feature_selector(feature_selectors, params)
 
-    def add_augmentation(self, augmentation, params={}):
+    def add_augmentation(self, augmentation, params=None, overwrite=True):
         """
         Add augmentation set to the pipeline.
 
         Args:
             augmentation (List): List of dictionaries containing time series augmentations
-            params (dict, {}): Parameters of the feature selector set.
+            params (dict, {}): Parameters of the augmentation set.
 
         Examples:
-            >>> client.pipeline.add_augmentation([{"name": "Add Noise", "params": {"scale": [0.05, 0.1, 0.15 ],  # , 0.1, 0.15
+            >>> client.pipeline.add_augmentation([{"name": "Add Noise", "params": {
+            >>>                                                                 "background_scale_range": [100, 1000],
             >>>                                                                 "target_labels": ['idle','walking'],
-            >>>                                                                 "target_sensors": ['AccelerometerX', 'GyroscopeX']
-            >>>                                                                }}
-            >>>                                   ])
+            >>>                                                                 "target_sensors": ['AccelerometerX', 'GyroscopeZ'],
+            >>>                                                                 "fraction": 1.2,
+            >>>                                                                 "noise_types": ["pink", "white"],
+            >>>                                                                 "filter": {"Set": ["Train"]}
+            >>>                                                                 }
+            >>>                                   }])
 
         """
+        if params is None:
+            params = {}
 
-        self._add_augmentation(augmentation, params)
+        self._add_augmentation(augmentation, params, overwrite)
 
-    def set_validation_method(self, name, params={}):
+    def set_validation_method(self, name, params=None):
         """Set the validation method for the tvo step.
 
         Args:
             name (str): Name of the validation method to use.
             params (dict, optional): Parameters for the validation method.
 
         """
+
+        if params is None:
+            params = {}
+
         self._validation_call = call = self._kb.functions.create_validation_method_call(
             name
         )
         for k, v in params.items():
             setattr(call, k, v)
 
-    def set_classifier(self, name, params={}):
+    def set_classifier(self, name, params=None):
         """Classification method for the TVO step to use.
 
         Args:
             name (str): Name of the classification method.
             params (dict, optional): Parameters of the classification method.
         """
+
+        if params is None:
+            params = {}
+
         self._classifier_call = call = self._kb.functions.create_classifier_call(name)
         for k, v in params.items():
             setattr(call, k, v)
 
     def set_training_algorithm(self, name, params={}):
         """Training algorithm for the TVO step to use.
 
@@ -1239,15 +1269,15 @@
 
         self._add_group_columns(generator_set)
 
         self._generator_index = self.get_pipeline_length()
 
         self._sandbox.add_linear_step(generator_set)
 
-    def _add_augmentation(self, augmentations, augmentation_set_params={}):
+    def _add_augmentation(self, augmentations, augmentation_set_params, overwrite=True):
 
         self._check_for_input_data()
 
         augmentation_set = self._kb.functions.create_augmentation_call_set(
             "augmentation_set"
         )
 
@@ -1255,30 +1285,30 @@
 
         for k, v in augmentation_set_params.items():
             setattr(augmentation_set, k, v)
 
         for augmentation in augmentations:
             logger.debug("augmentations:" + augmentation["name"])
 
-            call = self._kb.functions.create_function_call(augmentation["name"])
+            call = self._kb.functions.create_augmentation_call(augmentation["name"])
 
             for k, v in augmentation["params"].items():
                 setattr(call, k, v)
 
             augmentation_set.add_augmentation_call(call)
 
         self._add_group_columns(augmentation_set)
 
         self._add_passthrough_columns(augmentation_set)
 
         self._add_label_column(augmentation_set)
 
         self._augmentation_index = self.get_pipeline_length()
 
-        self._sandbox.add_linear_step(augmentation_set)
+        self._sandbox.add_linear_step(augmentation_set, overwrite)
 
     def _add_feature_selector(self, feature_selectors, selector_set_params={}):
 
         self._check_for_input_data()
         selector_set = self._kb.functions.create_selector_call_set("selector_set")
         logger.debug("feature_selector_set")
```

### Comparing `SensiML-2023.1.2/sensiml/profile/profile_data_parser.py` & `SensiML-2023.1.3/sensiml/profile/profile_data_parser.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/sml_runner.py` & `SensiML-2023.1.3/sensiml/sml_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,32 +7,35 @@
 from tkinter import E
 
 try:
     from typing import Literal
 except:
     from typing_extensions import Literal
 
-from typing import Dict, List, Optional
-
-from numpy import ndarray
-from pandas import DataFrame, Series
-
 try:
     from wurlitzer import pipes
 except:
-    print("unable to import wurlitzer for pipes")
+    pass
 
+from typing import Dict, List, Optional
+
+from numpy import ndarray
+from pandas import DataFrame, Series
 
 USE_PIPES = True if os.name == "posix" else False
 
 
 class ImportPathException(Exception):
     pass
 
 
+def get_activation(tensor):
+    return (max(tensor) + 128) / 256.0
+
+
 def dummy_function(*args, **kwrags):
     print("Not Supported by this version of the Knowledge Pack.")
     return None
 
 
 def compile_libsensiml_shared_library(path):
 
@@ -63,14 +66,39 @@
         model_info = json.load(open(os.path.join(path, "model.json"), "r"))
         class_maps = [x["ClassMaps"] for x in model_info["ModelDescriptions"]]
         return [{int(k): v for k, v in class_map.items()} for class_map in class_maps]
 
     return None
 
 
+def parse_model_json_for_model_type(path):
+
+    if os.path.exists(os.path.join(path, "model.json")):
+        model_info = json.load(open(os.path.join(path, "model.json"), "r"))
+        return [
+            description["ModelType"] for description in model_info["ModelDescriptions"]
+        ]
+
+    return None
+
+
+def is_tensorflow(ModelType):
+
+    if type(ModelType) != str:
+        return False
+
+    if "TF Micro" in ModelType:
+        return True
+
+    if "TensorFlow Lite for Microcontrollers" in ModelType:
+        return True
+
+    return False
+
+
 class struct_pme_pattern(ctypes.Structure):
     __slots__ = ["influence", "category", "vector"]
 
     _fields_ = [
         ("influence", ctypes.c_uint16),
         ("category", ctypes.c_uint16),
         ("vector", ctypes.POINTER(ctypes.c_uint8)),
@@ -149,52 +177,32 @@
         self._feature_summary = [{"Feature": str(x)} for x in value]
 
     def feature_summary_from_neurons(self):
         feature_vector = self.neuron_array[0]["Vector"]
         self.feature_summary = [{"Feature": str(x)} for x in range(len(feature_vector))]
 
 
-class SMLRunner(object):
-    """
-    This class provides a python interface to the Knowledge Pack library generated by SensiML.
-
-
-    Args:
-        path (str): Path to the downloaded Knowledge Pack .zip, the libsensiml.so, or libsensiml.dll
-        class_map (Optional[Dict], optional): The class map to use for this model. Defaults to None.
-
-    Example:
-
-    After downloading the Knowledge Pack for Windows or Linux.
-
-        sml = SMLRunner(<path_to_knowledgepack.zip>)
-        sml.init_model()
-
-    Then, you can use the python API to call the C functions in kb.h. For example, if you have a Dataframe df which has your sensor data
-    stored in it,
-
-        print(df.head(2))
-        > AccX, AccY, AccZ
-            9    10     11
-            12   8      23
+class SMLRunner:
+    def __init__(self, path: str, class_map: Optional[Dict] = None):
+        """
+        This class provides a Python interface to the Knowledge Pack library C code.
 
-    you can call recognize_capture API
+        Args:
+            path (str): Path to the downloaded Knowledge Pack .zip, the libsensiml.so, or libsensiml.dll.
+            class_map (Dict, optional): The class map to use for this model. Defaults to None.
 
-    results = recognize_capture(df)
+        Example:
 
-    """
+            After downloading the Knowledge Pack for Windows or Linux:
 
-    def __init__(self, path: str, class_map: Optional[Dict] = None):
-        """Initialize the SMLRunner with a downloaded Knowledge Pack
-
-        Args:
-            path (str): Path to the downloaded Knowledge Pack .zip, the libsensiml.so, or libsensiml.dll
-            class_map (Optional[Dict], optional): The class map to use for this model. Defaults to None.
+                sml = SMLRunner(<path_to_knowledgepack.zip>)
+                sml.init_model()
 
         """
+
         self._run_type = None
         self._model_initialized = False
 
         if path[-3:] == "zip":
             unzip_dir = os.path.basename(path)[:-4]
             with zipfile.ZipFile(path, "r") as zip_ref:
                 zip_ref.extractall(unzip_dir)
@@ -236,14 +244,16 @@
                 for model_class_map in class_map:
                     self.class_map.append(
                         {int(k): v for k, v in model_class_map.items()}
                     )
         else:
             self.class_map = parse_model_json_for_class_map(path)
 
+        self.model_type = parse_model_json_for_model_type(path)
+
         self._model_init = clf_lib.kb_model_init
         self._model_init.argtypes = []
 
         self._run_model = clf_lib.kb_run_model
         self._run_model.argtypes = [
             ctypes.POINTER(ctypes.c_int16),
             ctypes.c_int,
@@ -518,16 +528,16 @@
         with a new category and influence field
 
         Args:
            model_index(int): Index of the model to update
            category(uint16): category of the vector to add
            aif(uint16): weight function for the new pattern
 
-         Returns:
-             int: 0 if model does not support dynamic updates, -1 if model cannot be updated anymore, 1 if model was successfully updated
+        Returns:
+            int: 0 if model does not support dynamic updates, -1 if model cannot be updated anymore, 1 if model was successfully updated
         """
 
         if not self._initialized():
             return
 
         model_index_ctype = ctypes.c_int(model_index)
         category_ctype = ctypes.c_uint16(category)
@@ -604,17 +614,17 @@
         Args:
             data_sample(array):  single timepoint of data as an array from all sensors
             nsensors(int): unused
             model_index(int): Index of the model to run
             debug_log(bool): Prints the debug output from the Knowledge Pack
             model_api(str): use run_model, run_model_cascade_features or sml_recognition_run. These correspond to the API's in the kb.h file
 
-         Returns:
-             Classification results will be 0 if unknown through the classification numbers
-                 you have. This function returns -1 when a segment hasn't yet been identified.
+        Returns:
+            Classification results will be 0 if unknown through the classification numbers
+                you have. This function returns -1 when a segment hasn't yet been identified.
 
         """
         if not self._initialized():
             return
 
         if self._run_with("run_model") is False:
             return
@@ -653,14 +663,15 @@
         model_index: int = 0,
         model_api: Literal[
             "run_model", "run_model_cascade_features", "sml_recognition_run"
         ] = "run_model",
         get_feature_vector: bool = False,
         get_sensor_data: bool = False,
         get_output_tensor: bool = True,
+        verbose: bool = True,
     ) -> DataFrame:
         """Run the model against a DataFrame of sensor data
 
         Args:
             data (DataFrame): Input sensor data
             model_index (int, optional): The index of model to use. Defaults to 0.
             model_api (Literal[&quot;run_model&quot;,&quot;run_model_cascade_features&quot;,&quot;sml_recognition_run&quot;], optional): Model API to use. Defaults to "run_model".
@@ -704,23 +715,26 @@
 
                 if get_sensor_data:
                     for i in range(n_sensors):
                         sensor_data = self.get_segment_data(model_index)
                         output_columns["sensor_data_%d" % i] = sensor_data[i]
 
                 if get_output_tensor:
-                    output_columns["output_tensor"] = self.get_model_result(model_index)
+                    output_tensor = self.get_model_result(model_index)
+                    output_columns["output_tensor"] = output_tensor
+                    if self.model_type and is_tensorflow(self.model_type[model_index]):
+                        output_columns["activation"] = get_activation(output_tensor)
 
                 M.append(output_columns)
 
                 # After a classification is received, call sml_reset model to advance the internal buffer.
                 if model_api != "sml_recognition_run":
                     self.reset_model(model_index=model_index)
 
-            if i in status:
+            if verbose and i in status:
                 print("processed {samples} samples".format(samples=i))
 
         print("finished processing {samples} samples".format(samples=len(data)))
 
         return DataFrame(M)
 
     def run_segment(
@@ -732,17 +746,17 @@
         (Warning: using this call will flush the models internal ring buffer. Alternating between this and run_and_score model may produce incorrect results or crashes)
 
         Args:
             data(array):  Array of timseries data
             model_index(int): Index of the model to run
             debug_log(bool): Prints the debug output from the Knowledge Pack
 
-         Returns:
-             Classification results will be 0 if unknown through the classification numbers
-                 you have. This function returns -1 when a segment hasn't yet been identified.
+        Returns:
+            Classification results will be 0 if unknown through the classification numbers
+            you have. This function returns -1 when a segment hasn't yet been identified.
 
         """
         if not self._initialized():
             return
 
         if self._run_with("run_segment") is False:
             return
@@ -782,15 +796,14 @@
     def reset_model(self, model_index: int = 0):
         """
         Advances the model state to so that it is ready for a more input data. Use
         only after classification steps.
 
         (Note: this does not reset the model to a clean state, only init_model does this)
 
-
         Args:
            model_index(int): Index of the model to update
         """
 
         if not self._initialized():
             return
```

### Comparing `SensiML-2023.1.2/sensiml/tensorflow/utils.py` & `SensiML-2023.1.3/sensiml/tensorflow/utils.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/visualize/knowledgepack_visualize_mixin.py` & `SensiML-2023.1.3/sensiml/visualize/knowledgepack_visualize_mixin.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/sensiml/visualize/visualize.py` & `SensiML-2023.1.3/sensiml/visualize/visualize.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.1.2/setup.py` & `SensiML-2023.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 
 from setuptools import find_packages, setup
 
-__version__ = "2023.1.2"
+__version__ = "2023.1.3"
 
 # 'setup.py publish' shortcut.
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist bdist_wheel")
     os.system("twine upload dist/*")
     sys.exit()
```

