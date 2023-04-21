# Comparing `tmp/apache-airflow-providers-docker-3.5.1rc1.tar.gz` & `tmp/apache-airflow-providers-docker-3.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-docker-3.5.1rc1.tar", last modified: Sat Feb 18 20:35:29 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-docker-3.6.0rc1.tar", last modified: Fri Apr 21 19:48:23 2023, max compression
```

## Comparing `apache-airflow-providers-docker-3.5.1rc1.tar` & `apache-airflow-providers-docker-3.6.0rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-docker-3.5.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-02-18 20:35:28.000000 apache-airflow-providers-docker-3.5.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-docker-3.5.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    15226 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13679 2023-02-18 20:35:28.000000 apache-airflow-providers-docker-3.5.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6925 2023-02-18 19:30:13.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/decorators/docker.py
--rw-r--r--   0 root         (0) root         (0)     3189 2023-02-18 20:35:28.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7834 2023-01-24 18:52:14.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/hooks/docker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21914 2023-01-24 18:52:14.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/operators/docker.py
--rw-r--r--   0 root         (0) root         (0)     9635 2023-01-11 12:48:25.000000 apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/operators/docker_swarm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/apache_airflow_providers_docker.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15226 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/apache_airflow_providers_docker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      861 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/apache_airflow_providers_docker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/apache_airflow_providers_docker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/apache_airflow_providers_docker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       63 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/apache_airflow_providers_docker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/apache_airflow_providers_docker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3814 2023-02-11 18:49:53.000000 apache-airflow-providers-docker-3.5.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1866 2023-02-18 20:35:29.000000 apache-airflow-providers-docker-3.5.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1464 2023-02-18 20:35:28.000000 apache-airflow-providers-docker-3.5.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-docker-3.6.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:48:21.000000 apache-airflow-providers-docker-3.6.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-docker-3.6.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15898 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14371 2023-04-21 19:48:21.000000 apache-airflow-providers-docker-3.6.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2023-03-16 20:46:35.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/decorators/docker.py
+-rw-r--r--   0 root         (0) root         (0)     3238 2023-04-21 19:48:21.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2023-04-14 11:39:41.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/hooks/docker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22633 2023-04-21 10:05:41.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/operators/docker.py
+-rw-r--r--   0 root         (0) root         (0)     9635 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/operators/docker_swarm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15898 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      861 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-docker-3.6.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-04-21 19:48:21.000000 apache-airflow-providers-docker-3.6.0rc1/setup.py
```

### Comparing `apache-airflow-providers-docker-3.5.1rc1/LICENSE` & `apache-airflow-providers-docker-3.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.5.1rc1/MANIFEST.in` & `apache-airflow-providers-docker-3.6.0rc1/MANIFEST.in`

 * *Files 6% similar despite different names*

```diff
@@ -23,10 +23,9 @@
 # `MANIFEST_TEMPLATE.py.jinja2` IN the `provider_packages` DIRECTORY
 
 
 
 
 include NOTICE
 include LICENSE
-include CHANGELOG.txt
-include README.md
+include CHANGELOG.rst
 global-exclude __pycache__  *.pyc
```

### Comparing `apache-airflow-providers-docker-3.5.1rc1/PKG-INFO` & `apache-airflow-providers-docker-3.6.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-docker
-Version: 3.5.1rc1
+Version: 3.6.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-docker package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.5.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.6.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
@@ -49,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.5.1rc1``
+Release: ``3.6.0rc1``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``docker`` provider. All classes for this provider package
 are in ``airflow.providers.docker`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-docker/3.5.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-docker/3.6.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -111,14 +110,34 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.6.0
+.....
+
+Features
+~~~~~~~~
+
+* ``Add multiple exit code handling in skip logic for 'DockerOperator' and 'KubernetesPodOperator' (#30769)``
+* ``In 'DockerOperator', adding an attribute 'tls_verify' to choose whether to validate certificate (#30309) (#30310)``
+
+Misc
+~~~~
+
+* ``Deprecate 'skip_exit_code' in 'DockerOperator' and 'KubernetesPodOperator' (#30733)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Fix and augment 'check-for-inclusive-language' CI check (#29549)``
+   * ``Remove "boilerplate" from all taskflow decorators (#30118)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.5.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``fix template_fields in the decorator 'task.docker' (#29586)``
@@ -493,9 +512,7 @@
 * ``Fix error on DockerSwarmOperator with auto_remove True (#13532) (#13852)``
 
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-docker-3.5.1rc1/README.rst` & `apache-airflow-providers-docker-3.6.0rc1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.5.1rc1``
+Release: ``3.6.0rc1``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``docker`` provider. All classes for this provider package
 are in ``airflow.providers.docker`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-docker/3.5.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-docker/3.6.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -77,14 +77,34 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.6.0
+.....
+
+Features
+~~~~~~~~
+
+* ``Add multiple exit code handling in skip logic for 'DockerOperator' and 'KubernetesPodOperator' (#30769)``
+* ``In 'DockerOperator', adding an attribute 'tls_verify' to choose whether to validate certificate (#30309) (#30310)``
+
+Misc
+~~~~
+
+* ``Deprecate 'skip_exit_code' in 'DockerOperator' and 'KubernetesPodOperator' (#30733)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Fix and augment 'check-for-inclusive-language' CI check (#29549)``
+   * ``Remove "boilerplate" from all taskflow decorators (#30118)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.5.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``fix template_fields in the decorator 'task.docker' (#29586)``
```

### Comparing `apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/__init__.py` & `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/decorators/__init__.py` & `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/decorators/docker.py` & `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/decorators/docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,26 +75,22 @@
         Defaults to False.
     """
 
     custom_operator_name = "@task.docker"
 
     template_fields: Sequence[str] = (*DockerOperator.template_fields, "op_args", "op_kwargs")
 
-    # since we won't mutate the arguments, we should just do the shallow copy
-    # there are some cases we can't deepcopy the objects (e.g protobuf).
-    shallow_copy_attrs: Sequence[str] = ("python_callable",)
-
     def __init__(
         self,
         use_dill=False,
         python_command="python3",
         expect_airflow: bool = True,
         **kwargs,
     ) -> None:
-        command = "dummy command"
+        command = "placeholder command"
         self.python_command = python_command
         self.expect_airflow = expect_airflow
         self.pickling_library = dill if use_dill else pickle
         super().__init__(
             command=command, retrieve_output=True, retrieve_output_path="/tmp/script.out", **kwargs
         )
 
@@ -110,15 +106,15 @@
         with TemporaryDirectory(prefix="venv") as tmp_dir:
             input_filename = os.path.join(tmp_dir, "script.in")
             script_filename = os.path.join(tmp_dir, "script.py")
 
             with open(input_filename, "wb") as file:
                 if self.op_args or self.op_kwargs:
                     self.pickling_library.dump({"args": self.op_args, "kwargs": self.op_kwargs}, file)
-            py_source = self._get_python_source()
+            py_source = self.get_python_source()
             write_python_script(
                 jinja_context=dict(
                     op_args=self.op_args,
                     op_kwargs=self.op_kwargs,
                     pickling_library=self.pickling_library.__name__,
                     python_callable=self.python_callable.__name__,
                     python_callable_source=py_source,
@@ -136,18 +132,19 @@
                 self.environment["__PYTHON_INPUT"] = _b64_encode_file(input_filename)
             else:
                 self.environment["__PYTHON_INPUT"] = ""
 
             self.command = self.generate_command()
             return super().execute(context)
 
-    def _get_python_source(self):
+    # TODO: Remove me once this provider min supported Airflow version is 2.6
+    def get_python_source(self):
         raw_source = inspect.getsource(self.python_callable)
         res = dedent(raw_source)
-        res = remove_task_decorator(res, "@task.docker")
+        res = remove_task_decorator(res, self.custom_operator_name)
         return res
 
 
 def docker_task(
     python_callable: Callable | None = None,
     multiple_outputs: bool | None = None,
     **kwargs,
```

### Comparing `apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/get_provider_info.py` & `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/get_provider_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-docker",
         "name": "Docker",
         "description": "`Docker <https://docs.docker.com/install/>`__\n",
+        "suspended": False,
         "versions": [
+            "3.6.0",
             "3.5.1",
             "3.5.0",
             "3.4.0",
             "3.3.0",
             "3.2.0",
             "3.1.0",
             "3.0.0",
```

### Comparing `apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/hooks/__init__.py` & `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/hooks/docker.py` & `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/hooks/docker.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,34 +83,36 @@
         self._client_created = False
 
     @staticmethod
     def construct_tls_config(
         ca_cert: str | None = None,
         client_cert: str | None = None,
         client_key: str | None = None,
+        verify: bool = True,
         assert_hostname: str | bool | None = None,
         ssl_version: str | None = None,
     ) -> TLSConfig | bool:
         """
         Construct TLSConfig object from parts.
 
         :param ca_cert: Path to a PEM-encoded CA (Certificate Authority) certificate file.
         :param client_cert: Path to PEM-encoded certificate file.
         :param client_key: Path to PEM-encoded key file.
+        :param verify: Set ``True`` to verify the validity of the provided certificate.
         :param assert_hostname: Hostname to match against the docker server certificate
             or ``False`` to disable the check.
         :param ssl_version: Version of SSL to use when communicating with docker daemon.
         """
         if ca_cert and client_cert and client_key:
             # Ignore type error on SSL version here.
             # It is deprecated and type annotation is wrong, and it should be string.
             return TLSConfig(
                 ca_cert=ca_cert,
                 client_cert=(client_cert, client_key),
-                verify=True,
+                verify=verify,
                 ssl_version=ssl_version,
                 assert_hostname=assert_hostname,
             )
         return False
 
     @cached_property
     def api_client(self) -> APIClient:
```

### Comparing `apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/operators/__init__.py` & `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/operators/docker.py` & `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/operators/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 """Implements Docker operator"""
 from __future__ import annotations
 
 import ast
 import pickle
 import tarfile
 import warnings
+from collections.abc import Container
 from io import BytesIO, StringIO
 from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING, Iterable, Sequence
 
 from docker.constants import DEFAULT_TIMEOUT_SECONDS
 from docker.errors import APIError
 from docker.types import LogConfig, Mount
@@ -108,14 +109,15 @@
         '<network-name>|<network-id>' - Connects the container to user created network
         (using `docker network create` command)
     :param tls_ca_cert: Path to a PEM-encoded certificate authority
         to secure the docker connection.
     :param tls_client_cert: Path to the PEM-encoded certificate
         used to authenticate docker client.
     :param tls_client_key: Path to the PEM-encoded key used to authenticate docker client.
+    :param tls_verify: Set ``True`` to verify the validity of the provided certificate.
     :param tls_hostname: Hostname to match against
         the docker server certificate or False to disable the check.
     :param tls_ssl_version: Version of SSL to use when communicating with docker daemon.
     :param mount_tmp_dir: Specify whether the temporary directory should be bind-mounted
         from the host to the container. Defaults to True
     :param tmp_dir: Mount point inside the container to
         a temporary directory created on the host by the operator.
@@ -150,15 +152,15 @@
     :param log_opts_max_size: The maximum size of the log before it is rolled.
         A positive integer plus a modifier representing the unit of measure (k, m, or g).
         Eg: 10m or 1g Defaults to -1 (unlimited).
     :param log_opts_max_file: The maximum number of log files that can be present.
         If rolling the logs creates excess files, the oldest file is removed.
         Only effective when max-size is also set. A positive integer. Defaults to 1.
     :param ipc_mode: Set the IPC mode for the container.
-    :param skip_exit_code: If task exits with this exit code, leave the task
+    :param skip_on_exit_code: If task exits with this exit code, leave the task
         in ``skipped`` state (default: None). If set to ``None``, any non-zero
         exit code will be treated as a failure.
     """
 
     template_fields: Sequence[str] = ("image", "command", "environment", "env_file", "container_name")
     template_fields_renderers = {"env_file": "yaml"}
     template_ext: Sequence[str] = (
@@ -182,14 +184,15 @@
         force_pull: bool = False,
         mem_limit: float | str | None = None,
         host_tmp_dir: str | None = None,
         network_mode: str | None = None,
         tls_ca_cert: str | None = None,
         tls_client_cert: str | None = None,
         tls_client_key: str | None = None,
+        tls_verify: bool = True,
         tls_hostname: str | bool | None = None,
         tls_ssl_version: str | None = None,
         mount_tmp_dir: bool = True,
         tmp_dir: str = "/tmp/airflow",
         user: str | int | None = None,
         mounts: list[Mount] | None = None,
         entrypoint: str | list[str] | None = None,
@@ -209,14 +212,15 @@
         retrieve_output_path: str | None = None,
         timeout: int = DEFAULT_TIMEOUT_SECONDS,
         device_requests: list[DeviceRequest] | None = None,
         log_opts_max_size: str | None = None,
         log_opts_max_file: str | None = None,
         ipc_mode: str | None = None,
         skip_exit_code: int | None = None,
+        skip_on_exit_code: int | Container[int] | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.api_version = api_version
         if type(auto_remove) == bool:
             warnings.warn(
                 "bool value for auto_remove is deprecated, please use 'never', 'success', or 'force' instead",
@@ -244,14 +248,15 @@
         self.image = image
         self.mem_limit = mem_limit
         self.host_tmp_dir = host_tmp_dir
         self.network_mode = network_mode
         self.tls_ca_cert = tls_ca_cert
         self.tls_client_cert = tls_client_cert
         self.tls_client_key = tls_client_key
+        self.tls_verify = tls_verify
         self.tls_hostname = tls_hostname
         self.tls_ssl_version = tls_ssl_version
         self.mount_tmp_dir = mount_tmp_dir
         self.tmp_dir = tmp_dir
         self.user = user
         self.mounts = mounts or []
         self.entrypoint = entrypoint
@@ -269,23 +274,36 @@
         self.retrieve_output = retrieve_output
         self.retrieve_output_path = retrieve_output_path
         self.timeout = timeout
         self.device_requests = device_requests
         self.log_opts_max_size = log_opts_max_size
         self.log_opts_max_file = log_opts_max_file
         self.ipc_mode = ipc_mode
-        self.skip_exit_code = skip_exit_code
+        if skip_exit_code is not None:
+            warnings.warn(
+                "skip_exit_code is deprecated. Please use skip_on_exit_code", DeprecationWarning, stacklevel=2
+            )
+            skip_on_exit_code = skip_exit_code
+
+        self.skip_on_exit_code = (
+            skip_on_exit_code
+            if isinstance(skip_on_exit_code, Container)
+            else [skip_on_exit_code]
+            if skip_on_exit_code
+            else []
+        )
 
     @cached_property
     def hook(self) -> DockerHook:
         """Create and return an DockerHook (cached)."""
         tls_config = DockerHook.construct_tls_config(
             ca_cert=self.tls_ca_cert,
             client_cert=self.tls_client_cert,
             client_key=self.tls_client_key,
+            verify=self.tls_verify,
             assert_hostname=self.tls_hostname,
             ssl_version=self.tls_ssl_version,
         )
         return DockerHook(
             docker_conn_id=self.docker_conn_id,
             base_url=self.docker_url,
             version=self.api_version,
@@ -369,17 +387,17 @@
             log_lines = []
             for log_chunk in logstream:
                 log_chunk = stringify(log_chunk).strip()
                 log_lines.append(log_chunk)
                 self.log.info("%s", log_chunk)
 
             result = self.cli.wait(self.container["Id"])
-            if result["StatusCode"] == self.skip_exit_code:
+            if result["StatusCode"] in self.skip_on_exit_code:
                 raise AirflowSkipException(
-                    f"Docker container returned exit code {self.skip_exit_code}. Skipping."
+                    f"Docker container returned exit code {self.skip_on_exit_code}. Skipping."
                 )
             elif result["StatusCode"] != 0:
                 joined_log_lines = "\n".join(log_lines)
                 raise AirflowException(f"Docker container failed: {repr(result)} lines {joined_log_lines}")
 
             if self.retrieve_output:
                 return self._attempt_to_retrieve_result()
```

### Comparing `apache-airflow-providers-docker-3.5.1rc1/airflow/providers/docker/operators/docker_swarm.py` & `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/operators/docker_swarm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.5.1rc1/apache_airflow_providers_docker.egg-info/PKG-INFO` & `apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-docker
-Version: 3.5.1rc1
+Version: 3.6.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-docker package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.5.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.6.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
@@ -49,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.5.1rc1``
+Release: ``3.6.0rc1``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``docker`` provider. All classes for this provider package
 are in ``airflow.providers.docker`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-docker/3.5.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-docker/3.6.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -111,14 +110,34 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.6.0
+.....
+
+Features
+~~~~~~~~
+
+* ``Add multiple exit code handling in skip logic for 'DockerOperator' and 'KubernetesPodOperator' (#30769)``
+* ``In 'DockerOperator', adding an attribute 'tls_verify' to choose whether to validate certificate (#30309) (#30310)``
+
+Misc
+~~~~
+
+* ``Deprecate 'skip_exit_code' in 'DockerOperator' and 'KubernetesPodOperator' (#30733)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Fix and augment 'check-for-inclusive-language' CI check (#29549)``
+   * ``Remove "boilerplate" from all taskflow decorators (#30118)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.5.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``fix template_fields in the decorator 'task.docker' (#29586)``
@@ -493,9 +512,7 @@
 * ``Fix error on DockerSwarmOperator with auto_remove True (#13532) (#13852)``
 
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-docker-3.5.1rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt` & `apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.5.1rc1/pyproject.toml` & `apache-airflow-providers-docker-3.6.0rc1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 [tool.ruff]
 typing-modules = ["airflow.typing_compat"]
 line-length = 110
 extend-exclude = [
     ".eggs",
     "airflow/_vendor/*",
-
+    "airflow/providers/google/ads/_vendor/*",
     # The files generated by stubgen aren't 100% valid syntax it turns out, and we don't ship them, so we can
     # ignore them in ruff
     "airflow/providers/common/sql/*/*.pyi"
 ]
 
 # TODO: Bump to Python 3.8 when support for Python 3.7 is dropped in Airflow.
 target-version = "py37"
@@ -63,14 +63,46 @@
     "D212",
     "D213",
     "D214",
     "D215",
     "E731",
 ]
 
+[tool.pytest.ini_options]
+# * Disable `flaky` plugin for pytest. This plugin conflicts with `rerunfailures` because provide same marker.
+# * Disable `nose` builtin plugin for pytest. This feature deprecated in 7.2 and will be removed in pytest>=8
+# * And we focus on use native pytest capabilities rather than adopt another frameworks.
+addopts = "-rasl --verbosity=2 -p no:flaky -p no:nose --asyncio-mode=strict"
+norecursedirs = [
+    ".eggs",
+    "airflow",
+    "tests/dags_with_system_exit",
+    "tests/test_utils",
+    "tests/dags_corrupted",
+    "tests/dags",
+    "tests/system/providers/google/cloud/dataproc/resources",
+    "tests/system/providers/google/cloud/gcs/resources",
+]
+log_level = "INFO"
+filterwarnings = [
+    "error::pytest.PytestCollectionWarning",
+    "ignore::DeprecationWarning:flask_appbuilder.filemanager",
+    "ignore::DeprecationWarning:flask_appbuilder.widgets",
+    # https://github.com/dpgaspar/Flask-AppBuilder/pull/1940
+    "ignore::DeprecationWarning:flask_sqlalchemy",
+    # https://github.com/dpgaspar/Flask-AppBuilder/pull/1903
+    "ignore::DeprecationWarning:apispec.utils",
+]
+python_files = [
+    "*.py",
+]
+testpaths = [
+    "tests",
+]
+
 [tool.ruff.isort]
 known-first-party = ["airflow", "airflow_breeze", "docker_tests", "docs", "kubernetes_tests", "tests"]
 required-imports = ["from __future__ import annotations"]
 combine-as-imports = true
 
 # TODO: for now, https://github.com/charliermarsh/ruff/issues/1817
 known-third-party = [
@@ -101,14 +133,18 @@
 "airflow/models/sqla_models.py" = ["F401"]
 
 
 # The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
 # needed for the test to work
 "tests/decorators/test_python.py" = ["I002"]
 
+# The Pydantic representations of SqlAlchemy Models are not parsed well with Pydantic
+# when __future__.annotations is used so we need to skip them from upgrading
+"airflow/serialization/pydantic/*.py" = ["I002"]
+
 # Ignore pydoc style from these
 "*.pyi" = ["D"]
 "tests/*" = ["D"]
 "scripts/*" = ["D"]
 "dev/*" = ["D"]
 "docs/*" = ["D"]
 "provider_packages/*" = ["D"]
```

### Comparing `apache-airflow-providers-docker-3.5.1rc1/setup.cfg` & `apache-airflow-providers-docker-3.6.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-docker/3.5.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-docker/3.6.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-docker-3.5.1rc1/setup.py` & `apache-airflow-providers-docker-3.6.0rc1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,21 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-docker package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.5.1"
+version = "3.6.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-docker setup."""
     setup(
         version=version,
         extras_require={},
-        packages=find_namespace_packages(include=["airflow.providers.docker", "airflow.providers.docker.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.docker",
+                "airflow.providers.docker.*",
+                "airflow.providers.docker_vendor",
+                "airflow.providers.docker_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

