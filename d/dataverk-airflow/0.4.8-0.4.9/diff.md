# Comparing `tmp/dataverk-airflow-0.4.8.tar.gz` & `tmp/dataverk-airflow-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverk-airflow-0.4.8.tar", last modified: Thu Nov 17 12:25:09 2022, max compression
+gzip compressed data, was "dataverk-airflow-0.4.9.tar", last modified: Thu Nov 17 13:12:54 2022, max compression
```

## Comparing `dataverk-airflow-0.4.8.tar` & `dataverk-airflow-0.4.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 12:25:09.525522 dataverk-airflow-0.4.8/
--rw-r--r--   0 root         (0) root         (0)      410 2022-11-17 12:25:09.525522 dataverk-airflow-0.4.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2215 2022-11-17 12:25:01.000000 dataverk-airflow-0.4.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-17 12:25:09.525522 dataverk-airflow-0.4.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      675 2022-11-17 12:25:01.000000 dataverk-airflow-0.4.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 12:25:09.521522 dataverk-airflow-0.4.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 12:25:09.521522 dataverk-airflow-0.4.8/src/dataverk_airflow/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-17 12:25:01.000000 dataverk-airflow-0.4.8/src/dataverk_airflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)      768 2022-11-17 12:25:01.000000 dataverk-airflow-0.4.8/src/dataverk_airflow/init_containers.py
--rw-r--r--   0 root         (0) root         (0)     9649 2022-11-17 12:25:01.000000 dataverk-airflow-0.4.8/src/dataverk_airflow/knada_operators.py
--rw-r--r--   0 root         (0) root         (0)     1070 2022-11-17 12:25:01.000000 dataverk-airflow-0.4.8/src/dataverk_airflow/notifications.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 12:25:09.521522 dataverk-airflow-0.4.8/src/dataverk_airflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      410 2022-11-17 12:25:09.000000 dataverk-airflow-0.4.8/src/dataverk_airflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      388 2022-11-17 12:25:09.000000 dataverk-airflow-0.4.8/src/dataverk_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-17 12:25:09.000000 dataverk-airflow-0.4.8/src/dataverk_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2022-11-17 12:25:09.000000 dataverk-airflow-0.4.8/src/dataverk_airflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-11-17 12:25:09.000000 dataverk-airflow-0.4.8/src/dataverk_airflow.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:12:54.274663 dataverk-airflow-0.4.9/
+-rw-r--r--   0 root         (0) root         (0)      410 2022-11-17 13:12:54.274663 dataverk-airflow-0.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2215 2022-11-17 13:12:45.000000 dataverk-airflow-0.4.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2022-11-17 13:12:54.274663 dataverk-airflow-0.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      675 2022-11-17 13:12:45.000000 dataverk-airflow-0.4.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:12:54.270663 dataverk-airflow-0.4.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:12:54.270663 dataverk-airflow-0.4.9/src/dataverk_airflow/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-17 13:12:45.000000 dataverk-airflow-0.4.9/src/dataverk_airflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      768 2022-11-17 13:12:45.000000 dataverk-airflow-0.4.9/src/dataverk_airflow/init_containers.py
+-rw-r--r--   0 root         (0) root         (0)     9707 2022-11-17 13:12:45.000000 dataverk-airflow-0.4.9/src/dataverk_airflow/knada_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2022-11-17 13:12:45.000000 dataverk-airflow-0.4.9/src/dataverk_airflow/notifications.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:12:54.274663 dataverk-airflow-0.4.9/src/dataverk_airflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      410 2022-11-17 13:12:54.000000 dataverk-airflow-0.4.9/src/dataverk_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      388 2022-11-17 13:12:54.000000 dataverk-airflow-0.4.9/src/dataverk_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-17 13:12:54.000000 dataverk-airflow-0.4.9/src/dataverk_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2022-11-17 13:12:54.000000 dataverk-airflow-0.4.9/src/dataverk_airflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2022-11-17 13:12:54.000000 dataverk-airflow-0.4.9/src/dataverk_airflow.egg-info/top_level.txt
```

### Comparing `dataverk-airflow-0.4.8/README.md` & `dataverk-airflow-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `dataverk-airflow-0.4.8/setup.py` & `dataverk-airflow-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open('requirements.txt') as f:
     install_requires = f.read().strip().split('\n')
 
 setup(
     name='dataverk-airflow',
-    version='0.4.8',
+    version='0.4.9',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     python_requires='>=3.6',
     install_requires=install_requires,
     # metadata to display on PyPI
     author="NAV IKT",
     url="https://github.com/navikt/dataverk-airflow",
```

### Comparing `dataverk-airflow-0.4.8/src/dataverk_airflow/init_containers.py` & `dataverk-airflow-0.4.9/src/dataverk_airflow/init_containers.py`

 * *Files identical despite different names*

### Comparing `dataverk-airflow-0.4.8/src/dataverk_airflow/knada_operators.py` & `dataverk-airflow-0.4.9/src/dataverk_airflow/knada_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,16 @@
         "NOTEBOOK_PATH": f"{POD_WORKSPACE_DIR}/{Path(nb_path).parent}",
         "NOTEBOOK_NAME": Path(nb_path).name,
         "TZ": os.environ["TZ"],
         "REQUESTS_CA_BUNDLE": CA_BUNDLE_PATH,
         "NLS_LANG": nls_lang,
         "KNADA_TEAM_SECRET": os.environ["KNADA_TEAM_SECRET"]
     }
+    
+    namespace = os.getenv("TEAM") if os.getenv("TEAM") else namespace
 
     if extra_envs:
         env_vars = dict(env_vars, **extra_envs)
 
     def on_failure(context):
         if email:
             send_email = create_email_notification(email, name, namespace, dag)
@@ -87,15 +89,15 @@
         init_containers=[create_git_clone_init_container(
             repo, branch, POD_WORKSPACE_DIR)],
         image_pull_secrets=os.environ["K8S_IMAGE_PULL_SECRETS"],
         dag=dag,
         on_failure_callback=on_failure,
         name=name,
         cmds=["/bin/bash", "/execute_notebook.sh"],
-        namespace=os.getenv("TEAM") if os.getenv("TEAM") else namespace,
+        namespace=namespace,
         task_id=name,
         startup_timeout_seconds=startup_timeout_seconds,
         is_delete_operator_pod=delete_on_finish,
         image=os.getenv("KNADA_NOTEBOOK_OP_IMAGE",
                         "ghcr.io/navikt/knada-airflow:2022-10-14-8ec3b2c"),
         env_vars=env_vars,
         do_xcom_push=do_xcom_push,
@@ -182,14 +184,16 @@
         "NOTEBOOK_PATH": f"{POD_WORKSPACE_DIR}/{Path(script_path).parent}",
         "NOTEBOOK_NAME": Path(script_path).name,
         "TZ": os.environ["TZ"],
         "REQUESTS_CA_BUNDLE": CA_BUNDLE_PATH,
         "NLS_LANG": nls_lang
     }
 
+    namespace = os.getenv("TEAM") if os.getenv("TEAM") else namespace
+
     if extra_envs:
         env_vars = dict(env_vars, **extra_envs)
 
     def on_failure(context):
         if email:
             send_email = create_email_notification(email, name, namespace, dag)
             send_email.execute(context)
@@ -204,15 +208,15 @@
             repo, branch, POD_WORKSPACE_DIR)],
         image_pull_secrets=os.environ["K8S_IMAGE_PULL_SECRETS"],
         dag=dag,
         on_failure_callback=on_failure,
         startup_timeout_seconds=startup_timeout_seconds,
         name=name,
         cmds=["/bin/bash", "/execute_python.sh"],
-        namespace=os.getenv("TEAM") if os.getenv("TEAM") else namespace,
+        namespace=namespace,
         task_id=name,
         is_delete_operator_pod=delete_on_finish,
         image=os.getenv("KNADA_PYTHON_POD_OP_IMAGE",
                         "ghcr.io/navikt/knada-airflow:2022-05-25-bd8c92b"),
         env_vars=env_vars,
         volume_mounts=[
             VolumeMount(
```

### Comparing `dataverk-airflow-0.4.8/src/dataverk_airflow/notifications.py` & `dataverk-airflow-0.4.9/src/dataverk_airflow/notifications.py`

 * *Files identical despite different names*

