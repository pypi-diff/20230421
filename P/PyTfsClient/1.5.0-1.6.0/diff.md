# Comparing `tmp/PyTfsClient-1.5.0.tar.gz` & `tmp/PyTfsClient-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyTfsClient-1.5.0.tar", last modified: Thu Apr 13 20:16:44 2023, max compression
+gzip compressed data, was "dist\PyTfsClient-1.6.0.tar", last modified: Fri Apr 21 18:17:15 2023, max compression
```

## Comparing `PyTfsClient-1.5.0.tar` & `PyTfsClient-1.6.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.924593 PyTfsClient-1.5.0/
--rw-rw-rw-   0        0        0      642 2023-04-13 20:16:44.924593 PyTfsClient-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 20:16:44.932733 PyTfsClient-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1437 2023-04-13 20:16:37.000000 PyTfsClient-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.590897 PyTfsClient-1.5.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.691203 PyTfsClient-1.5.0/src/PyTfsClient.egg-info/
--rw-rw-rw-   0        0        0      642 2023-04-13 20:16:43.000000 PyTfsClient-1.5.0/src/PyTfsClient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2049 2023-04-13 20:16:44.000000 PyTfsClient-1.5.0/src/PyTfsClient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 20:16:43.000000 PyTfsClient-1.5.0/src/PyTfsClient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-02 15:09:42.000000 PyTfsClient-1.5.0/src/PyTfsClient.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2023-04-13 20:16:43.000000 PyTfsClient-1.5.0/src/PyTfsClient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-13 20:16:43.000000 PyTfsClient-1.5.0/src/PyTfsClient.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.747708 PyTfsClient-1.5.0/src/pytfsclient/
--rw-rw-rw-   0        0        0        0 2022-03-04 20:05:30.000000 PyTfsClient-1.5.0/src/pytfsclient/__init__.py
--rw-rw-rw-   0        0        0     3536 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/client_connection.py
--rw-rw-rw-   0        0        0     6046 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/client_factory.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.787366 PyTfsClient-1.5.0/src/pytfsclient/models/
--rw-rw-rw-   0        0        0        0 2023-03-22 16:13:58.000000 PyTfsClient-1.5.0/src/pytfsclient/models/__init__.py
--rw-rw-rw-   0        0        0      118 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/client_error.py
--rw-rw-rw-   0        0        0      720 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/deprecated.py
--rw-rw-rw-   0        0        0      700 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/obsolete.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.804530 PyTfsClient-1.5.0/src/pytfsclient/models/project/
--rw-rw-rw-   0        0        0        0 2023-03-22 16:43:11.000000 PyTfsClient-1.5.0/src/pytfsclient/models/project/__init__.py
--rw-rw-rw-   0        0        0     2628 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/project/tfs_project.py
--rw-rw-rw-   0        0        0     1925 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/project/tfs_team.py
--rw-rw-rw-   0        0        0     3082 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/project/tfs_team_member.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.836623 PyTfsClient-1.5.0/src/pytfsclient/models/workitems/
--rw-rw-rw-   0        0        0        0 2023-03-22 19:36:56.000000 PyTfsClient-1.5.0/src/pytfsclient/models/workitems/__init__.py
--rw-rw-rw-   0        0        0      364 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_update_relations_result.py
--rw-rw-rw-   0        0        0     1816 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_wiql_result.py
--rw-rw-rw-   0        0        0     8989 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_workitem.py
--rw-rw-rw-   0        0        0     6842 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_workitem_changes.py
--rw-rw-rw-   0        0        0     3829 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_workitem_relation.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.844616 PyTfsClient-1.5.0/src/pytfsclient/services/
--rw-rw-rw-   0        0        0        0 2023-03-21 17:34:23.000000 PyTfsClient-1.5.0/src/pytfsclient/services/__init__.py
--rw-rw-rw-   0        0        0     1100 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/base_client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.850873 PyTfsClient-1.5.0/src/pytfsclient/services/helpers/
--rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/helpers/__init__.py
--rw-rw-rw-   0        0        0      303 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/helpers/batch_iterable.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.863565 PyTfsClient-1.5.0/src/pytfsclient/services/http/
--rw-rw-rw-   0        0        0        0 2023-03-21 17:05:15.000000 PyTfsClient-1.5.0/src/pytfsclient/services/http/__init__.py
--rw-rw-rw-   0        0        0     5035 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/http/http_client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.873850 PyTfsClient-1.5.0/src/pytfsclient/services/mention_client/
--rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/mention_client/__init__.py
--rw-rw-rw-   0        0        0     2302 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/mention_client/mention_client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.887364 PyTfsClient-1.5.0/src/pytfsclient/services/project_client/
--rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/project_client/__init__.py
--rw-rw-rw-   0        0        0    13722 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/project_client/project_client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.896489 PyTfsClient-1.5.0/src/pytfsclient/services/workitem_client/
--rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/workitem_client/__init__.py
--rw-rw-rw-   0        0        0    26102 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/workitem_client/workitem_client.py
--rw-rw-rw-   0        0        0     2674 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_client.py
--rw-rw-rw-   0        0        0     2904 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_client_factory.py
--rw-rw-rw-   0        0        0     4181 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_project_client.py
--rw-rw-rw-   0        0        0     4527 2023-04-01 16:47:59.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_project_model.py
--rw-rw-rw-   0        0        0     1042 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_wiql_model.py
--rw-rw-rw-   0        0        0    13483 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_workitem_client.py
--rw-rw-rw-   0        0        0     6809 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_workitem_model.py
--rw-rw-rw-   0        0        0     3074 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_workitem_relation_model.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.922271 PyTfsClient-1.5.0/test/
--rw-rw-rw-   0        0        0     5924 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/test/test_backward_compatibility.py
--rw-rw-rw-   0        0        0     1052 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/test/test_client_connection.py
--rw-rw-rw-   0        0        0     1361 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/test/test_http_client_auth.py
--rw-rw-rw-   0        0        0     4568 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/test/test_http_client_basic.py
--rw-rw-rw-   0        0        0     9903 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/test/test_integration.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:17:15.563705 PyTfsClient-1.6.0/
+-rw-rw-rw-   0        0        0      642 2023-04-21 18:17:15.561884 PyTfsClient-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-21 18:17:15.563705 PyTfsClient-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1437 2023-04-21 18:14:47.000000 PyTfsClient-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:17:15.307857 PyTfsClient-1.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 18:17:15.385116 PyTfsClient-1.6.0/src/PyTfsClient.egg-info/
+-rw-rw-rw-   0        0        0      642 2023-04-21 18:17:14.000000 PyTfsClient-1.6.0/src/PyTfsClient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2049 2023-04-21 18:17:14.000000 PyTfsClient-1.6.0/src/PyTfsClient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 18:17:14.000000 PyTfsClient-1.6.0/src/PyTfsClient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-02 15:09:42.000000 PyTfsClient-1.6.0/src/PyTfsClient.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2023-04-21 18:17:14.000000 PyTfsClient-1.6.0/src/PyTfsClient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 18:17:14.000000 PyTfsClient-1.6.0/src/PyTfsClient.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 18:17:15.424648 PyTfsClient-1.6.0/src/pytfsclient/
+-rw-rw-rw-   0        0        0        0 2022-03-04 20:05:30.000000 PyTfsClient-1.6.0/src/pytfsclient/__init__.py
+-rw-rw-rw-   0        0        0     3536 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/client_connection.py
+-rw-rw-rw-   0        0        0     6046 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/client_factory.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:17:15.439643 PyTfsClient-1.6.0/src/pytfsclient/models/
+-rw-rw-rw-   0        0        0        0 2023-03-22 16:13:58.000000 PyTfsClient-1.6.0/src/pytfsclient/models/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/models/client_error.py
+-rw-rw-rw-   0        0        0      720 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/models/deprecated.py
+-rw-rw-rw-   0        0        0      700 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/models/obsolete.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:17:15.458784 PyTfsClient-1.6.0/src/pytfsclient/models/project/
+-rw-rw-rw-   0        0        0        0 2023-03-22 16:43:11.000000 PyTfsClient-1.6.0/src/pytfsclient/models/project/__init__.py
+-rw-rw-rw-   0        0        0     2628 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/models/project/tfs_project.py
+-rw-rw-rw-   0        0        0     1925 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/models/project/tfs_team.py
+-rw-rw-rw-   0        0        0     3082 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/models/project/tfs_team_member.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:17:15.485556 PyTfsClient-1.6.0/src/pytfsclient/models/workitems/
+-rw-rw-rw-   0        0        0        0 2023-03-22 19:36:56.000000 PyTfsClient-1.6.0/src/pytfsclient/models/workitems/__init__.py
+-rw-rw-rw-   0        0        0      364 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/models/workitems/tfs_update_relations_result.py
+-rw-rw-rw-   0        0        0     1816 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/models/workitems/tfs_wiql_result.py
+-rw-rw-rw-   0        0        0     8989 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/models/workitems/tfs_workitem.py
+-rw-rw-rw-   0        0        0     6850 2023-04-15 15:18:40.000000 PyTfsClient-1.6.0/src/pytfsclient/models/workitems/tfs_workitem_changes.py
+-rw-rw-rw-   0        0        0     3829 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/models/workitems/tfs_workitem_relation.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:17:15.492761 PyTfsClient-1.6.0/src/pytfsclient/services/
+-rw-rw-rw-   0        0        0        0 2023-03-21 17:34:23.000000 PyTfsClient-1.6.0/src/pytfsclient/services/__init__.py
+-rw-rw-rw-   0        0        0     1100 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/services/base_client.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:17:15.501418 PyTfsClient-1.6.0/src/pytfsclient/services/helpers/
+-rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/services/helpers/__init__.py
+-rw-rw-rw-   0        0        0      303 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/services/helpers/batch_iterable.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:17:15.511751 PyTfsClient-1.6.0/src/pytfsclient/services/http/
+-rw-rw-rw-   0        0        0        0 2023-03-21 17:05:15.000000 PyTfsClient-1.6.0/src/pytfsclient/services/http/__init__.py
+-rw-rw-rw-   0        0        0     5035 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/services/http/http_client.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:17:15.515551 PyTfsClient-1.6.0/src/pytfsclient/services/mention_client/
+-rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/services/mention_client/__init__.py
+-rw-rw-rw-   0        0        0     2305 2023-04-21 18:14:10.000000 PyTfsClient-1.6.0/src/pytfsclient/services/mention_client/mention_client.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:17:15.523443 PyTfsClient-1.6.0/src/pytfsclient/services/project_client/
+-rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/services/project_client/__init__.py
+-rw-rw-rw-   0        0        0     8846 2023-04-14 17:19:50.000000 PyTfsClient-1.6.0/src/pytfsclient/services/project_client/project_client.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:17:15.532620 PyTfsClient-1.6.0/src/pytfsclient/services/workitem_client/
+-rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/services/workitem_client/__init__.py
+-rw-rw-rw-   0        0        0    26102 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/services/workitem_client/workitem_client.py
+-rw-rw-rw-   0        0        0     2674 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/tfs_client.py
+-rw-rw-rw-   0        0        0     2904 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/tfs_client_factory.py
+-rw-rw-rw-   0        0        0     4181 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/tfs_project_client.py
+-rw-rw-rw-   0        0        0     4527 2023-04-01 16:47:59.000000 PyTfsClient-1.6.0/src/pytfsclient/tfs_project_model.py
+-rw-rw-rw-   0        0        0     1042 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/tfs_wiql_model.py
+-rw-rw-rw-   0        0        0    13483 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/tfs_workitem_client.py
+-rw-rw-rw-   0        0        0     6809 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/tfs_workitem_model.py
+-rw-rw-rw-   0        0        0     3074 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/src/pytfsclient/tfs_workitem_relation_model.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:17:15.555773 PyTfsClient-1.6.0/test/
+-rw-rw-rw-   0        0        0     5924 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/test/test_backward_compatibility.py
+-rw-rw-rw-   0        0        0     1052 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/test/test_client_connection.py
+-rw-rw-rw-   0        0        0     1361 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/test/test_http_client_auth.py
+-rw-rw-rw-   0        0        0     4568 2023-04-13 20:16:25.000000 PyTfsClient-1.6.0/test/test_http_client_basic.py
+-rw-rw-rw-   0        0        0     9903 2023-04-14 18:48:58.000000 PyTfsClient-1.6.0/test/test_integration.py
```

### Comparing `PyTfsClient-1.5.0/PKG-INFO` & `PyTfsClient-1.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PyTfsClient
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python Microsoft Team Foundation Server Library is a  client that can work with Microsoft TFS workitems
 Home-page: https://github.com/TopTuK/PyTfsClient
 Author: TopTuK
 Author-email: cydoor88@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: TFS,AZURE,TFS API,Team Foundation Server
```

### Comparing `PyTfsClient-1.5.0/README.md` & `PyTfsClient-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/setup.py` & `PyTfsClient-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ### Execute
 # python setup.py sdist
 # twine upload dist/*
 
 # https://docs.python.org/3/distutils/setupscript.html
 setup(
     name='PyTfsClient',
-    version='1.5.0',
+    version='1.6.0',
     license='MIT',
     description='Python Microsoft Team Foundation Server Library is a  client that can work with Microsoft TFS workitems',
     url='https://github.com/TopTuK/PyTfsClient',
     author='TopTuK',
     author_email='cydoor88@gmail.com',
     package_dir={'': 'src'},
     packages=find_packages(where='src', include=['pytfsclient*'], exclude=['.test', '*.test', 'test', 'test*', 'test.*']),
```

### Comparing `PyTfsClient-1.5.0/src/PyTfsClient.egg-info/PKG-INFO` & `PyTfsClient-1.6.0/src/PyTfsClient.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PyTfsClient
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python Microsoft Team Foundation Server Library is a  client that can work with Microsoft TFS workitems
 Home-page: https://github.com/TopTuK/PyTfsClient
 Author: TopTuK
 Author-email: cydoor88@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: TFS,AZURE,TFS API,Team Foundation Server
```

### Comparing `PyTfsClient-1.5.0/src/PyTfsClient.egg-info/SOURCES.txt` & `PyTfsClient-1.6.0/src/PyTfsClient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/client_connection.py` & `PyTfsClient-1.6.0/src/pytfsclient/client_connection.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/client_factory.py` & `PyTfsClient-1.6.0/src/pytfsclient/client_factory.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/models/deprecated.py` & `PyTfsClient-1.6.0/src/pytfsclient/models/deprecated.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/models/obsolete.py` & `PyTfsClient-1.6.0/src/pytfsclient/models/obsolete.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/models/project/tfs_project.py` & `PyTfsClient-1.6.0/src/pytfsclient/models/project/tfs_project.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/models/project/tfs_team.py` & `PyTfsClient-1.6.0/src/pytfsclient/models/project/tfs_team.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/models/project/tfs_team_member.py` & `PyTfsClient-1.6.0/src/pytfsclient/models/project/tfs_team_member.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_wiql_result.py` & `PyTfsClient-1.6.0/src/pytfsclient/models/workitems/tfs_wiql_result.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_workitem.py` & `PyTfsClient-1.6.0/src/pytfsclient/models/workitems/tfs_workitem.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_workitem_changes.py` & `PyTfsClient-1.6.0/src/pytfsclient/models/workitems/tfs_workitem_changes.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Class contains information of field change of workitem.
     '''
 
     @property
     def name(self) -> str:
         '''
         Returns:
-            Field name
+            Changed field name
         '''
 
         return self.__name
 
     @property
     def old_value(self) -> Union[str, TeamMember, dict]:
         '''
```

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_workitem_relation.py` & `PyTfsClient-1.6.0/src/pytfsclient/models/workitems/tfs_workitem_relation.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/services/base_client.py` & `PyTfsClient-1.6.0/src/pytfsclient/services/base_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/services/http/http_client.py` & `PyTfsClient-1.6.0/src/pytfsclient/services/http/http_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/services/mention_client/mention_client.py` & `PyTfsClient-1.6.0/src/pytfsclient/services/mention_client/mention_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     '''
     Mention client for mention users of TFS/Azure service
     '''
 
     _TFS_HISTORY_FIELD = 'System.History'
     
     @staticmethod
-    def send_mention(self, workitem: Workitem, to_user: TeamMember, \
+    def send_mention(workitem: Workitem, to_user: TeamMember, \
                     message: str, from_user: TeamMember = None) -> MentionResult:
         '''
         Sends mention to user. Writes mention to History of workitem
         WARNING: this function uses non-public API
 
         Args:
             workitem (Workitem): workitem where mention will send
@@ -55,14 +55,14 @@
 
         mention = f'<a href=\"#\" data-vss-mention=\"version:2.0,{to_user.id}\">@{to_user.display_name}</a>: {message}'
 
         if (from_user) and (from_user.id != to_user.id):
             mention += f'<br>CC: <a href=\"#\" data-vss-mention=\"version:2.0,{from_user.Id}\">@{from_user.DisplayName}</a>'
 
         try:
-            workitem[self._TFS_HISTORY_FIELD] = mention
+            workitem[MentionClient._TFS_HISTORY_FIELD] = mention
             update_result = workitem.update_fields()
 
             return MentionResult.MENTION_SUCCESS \
                 if update_result == UpdateFieldsResult.UPDATE_SUCCESS else MentionResult.MENTION_ERROR
         except:
             return MentionResult.MENTION_EXCEPTION
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
 from enum import Enum from ...models.workitems.tfs_workitem import
 UpdateFieldsResult, Workitem from ...models.project.tfs_team_member import
 TeamMember from ...models.client_error import ClientError class MentionResult
 (Enum): ''' ENUM: send mention result Values: MENTION_SUCCESS MENTION_ERROR
 MENTION_EXCEPTION ''' MENTION_SUCCESS = 0 MENTION_ERROR = 1 MENTION_EXCEPTION =
 2 class MentionClient: ''' Mention client for mention users of TFS/Azure
 service ''' _TFS_HISTORY_FIELD = 'System.History' @staticmethod def
-send_mention(self, workitem: Workitem, to_user: TeamMember, \ message: str,
+send_mention(workitem: Workitem, to_user: TeamMember, \ message: str,
 from_user: TeamMember = None) -> MentionResult: ''' Sends mention to user.
 Writes mention to History of workitem WARNING: this function uses non-public
 API Args: workitem (Workitem): workitem where mention will send to_user
 (TeamMember): mentioned user message (str): mention text from_user
 (TeamMember): copy user who will be mentioned. Default: None Returns: Send
 mention result: MentionResult (incl. MENTION_EXCEPTION) Raises: ClientError: if
 workitem, to_user or message is None ''' if not workitem: raise ClientError
 ('workitem can\'t be None') if not to_user: raise ClientError('To User can\'t
 be None') if not message: raise ClientError('Mention message can\'t be None')
 mention = f'@{to_user.display_name}: {message}' if (from_user) and
 (from_user.id != to_user.id): mention += f'
-CC: @{from_user.DisplayName}' try: workitem[self._TFS_HISTORY_FIELD] = mention
-update_result = workitem.update_fields() return MentionResult.MENTION_SUCCESS \
-if update_result == UpdateFieldsResult.UPDATE_SUCCESS else
-MentionResult.MENTION_ERROR except: return MentionResult.MENTION_EXCEPTION
+CC: @{from_user.DisplayName}' try: workitem[MentionClient._TFS_HISTORY_FIELD] =
+mention update_result = workitem.update_fields() return
+MentionResult.MENTION_SUCCESS \ if update_result ==
+UpdateFieldsResult.UPDATE_SUCCESS else MentionResult.MENTION_ERROR except:
+return MentionResult.MENTION_EXCEPTION
```

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/services/project_client/project_client.py` & `PyTfsClient-1.6.0/src/pytfsclient/services/project_client/project_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             
             return projects
         except Exception as ex:
             raise ClientError(f'ProjectClient::get_projects: exception raised. Msg: {ex}', ex)
 
     def get_all_teams(self, current_user: bool = False) -> List[Team]:
         '''
-        Return list of TFS/Azure teams.
+        Returns list of TFS/Azure teams.
         Docs: https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get-teams?view=azure-devops-rest-6.0
 
         Args:
             current_user (bool): If true return all the teams requesting user is member, otherwise return all the teams user has read access.
         
         Returns:
             List of TFS/Azure teams: List[Team]
@@ -101,125 +101,14 @@
                 raise ClientError('ProjectClient::get_all_teams: response doesn\'t have \'value\' attribute')
         except Exception as ex:
             raise ClientError(f'ProjectClient::get_all_teams: exception raised. Msg: {ex}', ex)
 
     def get_project_teams(self, project: Project, expand: bool = False, \
                           current_user: bool = False, skip: int = 0) -> List[Team]:
         '''
-        Get a list of teams of given project.
-        Docs: https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get-teams?view=azure-devops-rest-6.0
-
-        Args:
-            project (Project): Project class instance
-            expand (bool): a value indicating whether or not to expand Identity information in the result WebApiTeam object. Default: False
-            current_user (bool): If true return all the teams requesting user is member, otherwise return all the teams user has read access. Default: False
-            skip (int): Number of teams to skip. Default: 0
-        
-        Returns:
-            List of teams: List[Team]
-        
-        Raises:
-            ClientError if project is None or bad request
-        '''
-
-        if not project:
-            raise ClientError('ProjectClient::get_project_teams: project can\'t be None')
-
-        request_url = f'{self.client_connection.api_url}{self._URL_PROJECTS}/{project.id}/{self._URL_TEAMS}'
-        query_params = {
-            'api-version' : self.api_version,
-            '$expandIdentity' : str(expand),
-            '$mine' : str(current_user),
-            '$skip' : str(skip)
-        }
-
-        try:
-            teams = list()
-
-            hasNext = True
-            while hasNext:
-                response = self.http_client.get(request_url, query_params=query_params)
-
-                if not response:
-                    raise ClientError('ProjectClient::get_project_teams: can\'t get response from TFS server')
-        
-                json_items = response.json()
-                if ('count' in json_items) and (int(json_items['count']) == 0):
-                    hasNext = False
-                    continue
-
-                if 'value' in json_items:
-                    json_items = json_items['value']
-                    teams += [Team.from_json(json_item) for json_item in json_items]
-                    query_params['$skip'] = str(len(teams))
-                else:
-                    raise ClientError('ProjectClient::get_project_teams: response doesn\'t have \'value\' attribute')
-                
-            return teams
-        except Exception as ex:
-            raise ClientError(f'ProjectClient::get_project_teams: exception raised. Msg: {ex}', ex)
-        
-    def get_project_team_members(self, project: Project, team: Team) -> List[TeamMember]:
-        '''
-        Get a list of members for a specific team and a project.
-        Docs: https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get-team-members-with-extended-properties?view=azure-devops-rest-6.0
-
-        Args:
-            project (Project): project instance of the team project the team belongs to.
-            team (Team): team instance
-
-        Returns:
-            List of team members: List[TeamMember]
-        
-        Raises:
-            ClientError if project or team is None
-            ClientError if bad request
-        '''
-        
-        if not project:
-            raise ClientError('ProjectClient::get_project_team_members: project can\'t be None')
-        
-        if not team:
-            raise ClientError('ProjectClient::get_project_team_members: team can\'t be None')
-
-        request_url = f'{self.client_connection.api_url}{self._URL_PROJECTS}/{project.id}/{self._URL_TEAMS}/{team.id}/{self._URL_TEAM_MEMBERS}'
-        query_params = {
-            'api-version' : self.api_version,
-            '$skip' : '0'
-        }
-
-        try:
-            members = list()
-
-            hasNext = True
-            while hasNext:
-                response = self.http_client.get(request_url, query_params=query_params)
-
-                if not response:
-                        raise ClientError('ProjectClient::get_project_team_members: can\'t get response from TFS server')    
-                
-                json_items = response.json()
-                if ('count' in json_items) and (int(json_items['count']) == 0):
-                        hasNext = False
-                        continue
-                
-                if 'value' in json_items:
-                    json_items = json_items['value']
-                    members += [TeamMember.from_json(json_item['identity']) for json_item in json_items]
-                    query_params['$skip'] = str(len(members))
-                else:
-                    raise ClientError('ProjectClient::get_project_team_members: response doesn\'t have \'value\' attribute')
-                
-            return members
-        except Exception as ex:
-            raise ClientError(f'ProjectClient::get_project_team_members: exception raised. Msg: {ex}', ex)
-
-    def get_project_teams(self, project: Project, expand: bool = False, \
-                          current_user: bool = False, skip: int = 0) -> List[Team]:
-        '''
         Get a list of members for a specific team and a project.
         Docs: https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get-teams?view=azure-devops-rest-6.0
 
         Args:
             project (Project): project instance. Can't be None
             expand (bool): A value indicating whether or not to expand Identity information in the result WebApiTeam object. Default: False
             current_user (bool): If true return all the teams requesting user is member, otherwise return all the teams user has read access. Default: False
```

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/services/workitem_client/workitem_client.py` & `PyTfsClient-1.6.0/src/pytfsclient/services/workitem_client/workitem_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/tfs_client.py` & `PyTfsClient-1.6.0/src/pytfsclient/tfs_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/tfs_client_factory.py` & `PyTfsClient-1.6.0/src/pytfsclient/tfs_client_factory.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/tfs_project_client.py` & `PyTfsClient-1.6.0/src/pytfsclient/tfs_project_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/tfs_project_model.py` & `PyTfsClient-1.6.0/src/pytfsclient/tfs_project_model.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/tfs_wiql_model.py` & `PyTfsClient-1.6.0/src/pytfsclient/tfs_wiql_model.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/tfs_workitem_client.py` & `PyTfsClient-1.6.0/src/pytfsclient/tfs_workitem_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/tfs_workitem_model.py` & `PyTfsClient-1.6.0/src/pytfsclient/tfs_workitem_model.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/src/pytfsclient/tfs_workitem_relation_model.py` & `PyTfsClient-1.6.0/src/pytfsclient/tfs_workitem_relation_model.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/test/test_backward_compatibility.py` & `PyTfsClient-1.6.0/test/test_backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/test/test_client_connection.py` & `PyTfsClient-1.6.0/test/test_client_connection.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/test/test_http_client_auth.py` & `PyTfsClient-1.6.0/test/test_http_client_auth.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/test/test_http_client_basic.py` & `PyTfsClient-1.6.0/test/test_http_client_basic.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.5.0/test/test_integration.py` & `PyTfsClient-1.6.0/test/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     # Assert
     assert wi, 'Can\'t create Workitem!'
     assert wi.title == wi_title, 'Workitem title differs!'
 
     assert wi.relations, 'Workitem relations are None'
     assert len(relations) == len(wi.relations), 'Workitem relations count is not same!'
 
-    # Check onlu one relation
+    # Check only one relation
     assert wi.relations[0].destination_id == relations[0].destination_id
 
 def test_update_workitem_fields(workitem_client: WorkitemClient):
     # Arrange
     today = datetime.date.today()
     workitem_id = 2
```

