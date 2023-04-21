# Comparing `tmp/gitlab-runner-tart-driver-0.1.2.tar.gz` & `tmp/gitlab-runner-tart-driver-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-runner-tart-driver-0.1.2.tar", last modified: Wed Apr 19 08:06:31 2023, max compression
+gzip compressed data, was "gitlab-runner-tart-driver-0.1.3.tar", last modified: Fri Apr 21 09:03:47 2023, max compression
```

## Comparing `gitlab-runner-tart-driver-0.1.2.tar` & `gitlab-runner-tart-driver-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:06:31.868012 gitlab-runner-tart-driver-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     3303 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    14631 2023-04-19 08:06:31.868012 gitlab-runner-tart-driver-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    14110 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:06:31.862012 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:06:31.866012 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/config.py
--rw-rw-rw-   0 root         (0) root         (0)     8981 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/prepare.py
--rw-rw-rw-   0 root         (0) root         (0)     2145 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:06:31.867012 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1061 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
--rw-rw-rw-   0 root         (0) root         (0)     6622 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/tart.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:06:31.864012 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14631 2023-04-19 08:06:31.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      986 2023-04-19 08:06:31.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 08:06:31.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-19 08:06:31.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 08:06:31.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-19 08:06:31.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-19 08:06:31.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 08:06:31.868012 gitlab-runner-tart-driver-0.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:03:47.405937 gitlab-runner-tart-driver-0.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)     3303 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    15758 2023-04-21 09:03:47.405937 gitlab-runner-tart-driver-0.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    15237 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:03:47.399937 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:03:47.403937 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9267 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/prepare.py
+-rw-rw-rw-   0 root         (0) root         (0)     2145 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:03:47.404937 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     7443 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/tart.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:03:47.401937 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15758 2023-04-21 09:03:47.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      986 2023-04-21 09:03:47.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 09:03:47.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-21 09:03:47.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 09:03:47.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-21 09:03:47.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-21 09:03:47.000000 gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 09:03:47.405937 gitlab-runner-tart-driver-0.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-21 09:03:36.000000 gitlab-runner-tart-driver-0.1.3/setup.py
```

### Comparing `gitlab-runner-tart-driver-0.1.2/LICENSE.txt` & `gitlab-runner-tart-driver-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.2/PKG-INFO` & `gitlab-runner-tart-driver-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
@@ -110,23 +110,26 @@
 
 **config.toml**
 
 ```ini
 [runners.custom]
     config_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     config_args = [ "config", '-x', '/opt/homebrew/bin/tart' ]
+    config_exec_timeout = 200
 
     prepare_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     prepare_args = [ "prepare", '-x', '/opt/homebrew/bin/tart' ]
+    prepare_exec_timeout = 200
 
     run_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     run_args = [ "run", '-x', '/opt/homebrew/bin/tart' ]
 
     cleanup_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     cleanup_args = [ "cleanup", '-x', '/opt/homebrew/bin/tart' ]
+    cleanup_exec_timeout = 200
 ```
 
 Now restart the gitlab-runner with `gitlab-runner restart`
 
 ## GitLab CI
 
 One of the great advantages in using [Tart](https://tart.run) is that it gives almost all functionality to we are used from the standard `docker` executors allowing us to write GitLabCI piplines that do not need any or minimal adaptions for OSX.
@@ -272,14 +275,30 @@
 To enable Host-local caching and builds, simply pass `--builds-dir` and `--cache-dir` to the `prepare` command
 
 ```ini
 prepare_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
 prepare_args = [ "prepare", '-x', '/opt/homebrew/bin/tart', '--concurrency', '2', '--auto-resources', '--cache-dir', '/Users/gitlab/gitlab-runner/cache', '--builds-dir', '/Users/gitlab/gitlab-runner/builds']
 ```
 
+### Volume Mounts
+
+Just like with `docker` the `gitlab-runner-tart-driver` allows you to mount any arbitrary host path into your VM. This can be especially useful if you have to mount runner-local resources like shared test-data or additional caches into the executor. You can follow the standard docker syntax for *volume mounts* `--volume /my/local/dir:/opt/remote/dir`. Additionally you can also pass the `ro` flag to make the mount *read-only* i.e.  `--volume /my/local/dir:/opt/remote/dir:ro`.
+
+```ini
+[runners.custom]
+  config_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
+  config_args = [ "config" ]
+
+  prepare_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
+  prepare_args = [ "prepare",
+    '-x', '/opt/homebrew/bin/tart',
+    '--concurrency', '2',
+    '--auto-resources',
+    '--volume /data/models/:/opt/data/models:ro']
+```
 ### Auto Host Resource Distribution
 
 `tart` images come with a pre-defined number of CPUs and Memory allocation. Typical numbers for default images are `cpu_count=4` and `memory=8192`. With the concurrency limitation of two VMs/images running at the same time this might not utilize your host system completely.
 Per default, `--auto-resources` is enable for the `gitlab-runner-tart-driver` which will split the host resources equally to the VMs defined by `--concurrency`. The default concurrency is `1` and therefore will assign all host resources to the VM.
 
 > **ATTENTION** make sure your `gitlab-runner` concurrency setting is the same as the `--concurrency` parameter you are passing to the `prepare` command
 
@@ -352,16 +371,18 @@
   --concurrency INTEGER           Number of concurrent processes that are
                                   supported. ATTENTION tart currently only
                                   support two concurrent VMs
   --cache-dir TEXT                Caching dir to be used.
   --builds-dir TEXT               Path to the builds directory.
   --timeout INTEGER               Timeout in seconds for the VM to be
                                   reachable via SSH.
+  --volume TEXT                   Volume mount definition with docker syntax.
+                                  <host_dir>:<vm_dir>[:ro]
   -x, --tart-executable TEXT      Path to the tart executable.
-  --help                          Show this message and exit.
+  --help                          Show this message and exit.                      Show this message and exit.
 ```
 
 ### Command `run`
 
 ```
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
```

### Comparing `gitlab-runner-tart-driver-0.1.2/README.md` & `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: gitlab-runner-tart-driver
+Version: 0.1.3
+Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
+Author: Matthias Schmieder
+Author-email: schmieder.matthias@gmail.com
+License: BSD
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Version Control
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Gitlab Runner Custom Tart Driver
 
 ## About
 
 [Tart](https://tart.run) is a virtualization toolset to build, run and manage macOS and Linux virtual machines on Apple Silicon. Tart is using Apple’s native Virtualization.Framework that was developed along with architecting the first M1 chip. This seamless integration between hardware and software ensures smooth performance without any drawbacks.
 
 For storing virtual machine images Tart integrates with **OCI-compatible container registries**. This allows you to work with virtual machines as you used to with Docker containers.
@@ -95,23 +110,26 @@
 
 **config.toml**
 
 ```ini
 [runners.custom]
     config_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     config_args = [ "config", '-x', '/opt/homebrew/bin/tart' ]
+    config_exec_timeout = 200
 
     prepare_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     prepare_args = [ "prepare", '-x', '/opt/homebrew/bin/tart' ]
+    prepare_exec_timeout = 200
 
     run_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     run_args = [ "run", '-x', '/opt/homebrew/bin/tart' ]
 
     cleanup_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     cleanup_args = [ "cleanup", '-x', '/opt/homebrew/bin/tart' ]
+    cleanup_exec_timeout = 200
 ```
 
 Now restart the gitlab-runner with `gitlab-runner restart`
 
 ## GitLab CI
 
 One of the great advantages in using [Tart](https://tart.run) is that it gives almost all functionality to we are used from the standard `docker` executors allowing us to write GitLabCI piplines that do not need any or minimal adaptions for OSX.
@@ -257,14 +275,30 @@
 To enable Host-local caching and builds, simply pass `--builds-dir` and `--cache-dir` to the `prepare` command
 
 ```ini
 prepare_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
 prepare_args = [ "prepare", '-x', '/opt/homebrew/bin/tart', '--concurrency', '2', '--auto-resources', '--cache-dir', '/Users/gitlab/gitlab-runner/cache', '--builds-dir', '/Users/gitlab/gitlab-runner/builds']
 ```
 
+### Volume Mounts
+
+Just like with `docker` the `gitlab-runner-tart-driver` allows you to mount any arbitrary host path into your VM. This can be especially useful if you have to mount runner-local resources like shared test-data or additional caches into the executor. You can follow the standard docker syntax for *volume mounts* `--volume /my/local/dir:/opt/remote/dir`. Additionally you can also pass the `ro` flag to make the mount *read-only* i.e.  `--volume /my/local/dir:/opt/remote/dir:ro`.
+
+```ini
+[runners.custom]
+  config_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
+  config_args = [ "config" ]
+
+  prepare_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
+  prepare_args = [ "prepare",
+    '-x', '/opt/homebrew/bin/tart',
+    '--concurrency', '2',
+    '--auto-resources',
+    '--volume /data/models/:/opt/data/models:ro']
+```
 ### Auto Host Resource Distribution
 
 `tart` images come with a pre-defined number of CPUs and Memory allocation. Typical numbers for default images are `cpu_count=4` and `memory=8192`. With the concurrency limitation of two VMs/images running at the same time this might not utilize your host system completely.
 Per default, `--auto-resources` is enable for the `gitlab-runner-tart-driver` which will split the host resources equally to the VMs defined by `--concurrency`. The default concurrency is `1` and therefore will assign all host resources to the VM.
 
 > **ATTENTION** make sure your `gitlab-runner` concurrency setting is the same as the `--concurrency` parameter you are passing to the `prepare` command
 
@@ -337,16 +371,18 @@
   --concurrency INTEGER           Number of concurrent processes that are
                                   supported. ATTENTION tart currently only
                                   support two concurrent VMs
   --cache-dir TEXT                Caching dir to be used.
   --builds-dir TEXT               Path to the builds directory.
   --timeout INTEGER               Timeout in seconds for the VM to be
                                   reachable via SSH.
+  --volume TEXT                   Volume mount definition with docker syntax.
+                                  <host_dir>:<vm_dir>[:ro]
   -x, --tart-executable TEXT      Path to the tart executable.
-  --help                          Show this message and exit.
+  --help                          Show this message and exit.                      Show this message and exit.
 ```
 
 ### Command `run`
 
 ```
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
 
@@ -367,8 +403,8 @@
 Usage: gitlab-runner-tart-driver cleanup [OPTIONS]
 
   Command to greet a user.
 
 Options:
   -x, --tart-executable TEXT  Path to the tart executable.
   --help                      Show this message and exit.
-```
+```
```

### Comparing `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/cli.py` & `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/cli.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/cleanup.py` & `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/cleanup.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/config.py` & `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/prepare.py` & `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/prepare.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 
 import click
 
 from gitlab_runner_tart_driver.modules.gitlab_custom_command_config import GitLabCustomCommandConfig
 from gitlab_runner_tart_driver.modules.tart import Tart
-from gitlab_runner_tart_driver.modules.tart import TartMount
+from gitlab_runner_tart_driver.modules.tart import TartVolume
 from gitlab_runner_tart_driver.modules.utils import get_host_spec
 from gitlab_runner_tart_driver.modules.utils import print_host_spec
 
 
 @click.command()
 @click.option(
     "--default-ssh-username", default="admin", required=False, type=str, help="username to login to a tart vm"
@@ -67,14 +67,23 @@
 @click.option(
     "--timeout",
     required=False,
     default=60,
     type=int,
     help="Timeout in seconds for the VM to be reachable via SSH.",
 )
+@click.option(
+    "--volume",
+    "volumes",
+    required=False,
+    default=[],
+    type=str,
+    multiple=True,
+    help="Volume mount definition with docker syntax. <host_dir>:<vm_dir>[:ro]",
+)
 @click.option("-x", "--tart-executable", required=False, default="tart", type=str, help="Path to the tart executable.")
 def prepare(
     default_ssh_username,
     default_ssh_password,
     registry_username,
     registry_password,
     registry,
@@ -83,14 +92,15 @@
     display,
     pull_policy,
     auto_resources,
     concurrency,
     cache_dir,
     builds_dir,
     timeout,
+    volumes,
     tart_executable,
 ):
     """Prepare the environment and start the tart VM."""
 
     print_host_spec()
 
     p = GitLabCustomCommandConfig()
@@ -113,31 +123,28 @@
     # OCI LOGIN
     ######################################################################
     click.echo(f"[INFO] Logging into GitLab Registry '{p.ci_registry}'")
     try:
         tart.login(username=p.ci_registry_user, password=p.ci_registry_password, host=p.ci_registry)
     except:
         click.secho(f"[ERROR] Failed to login to '{p.ci_registry}'", fg="red")
-        sys.exit(1)
 
     if registry_username and registry_password and registry:
         click.echo(f"[INFO] Logging into OCI Registry '{registry}'")
         try:
             tart.login(username=registry_username, password=registry_password, host=registry)
         except:
             click.secho(f"[ERROR] Failed to login to '{registry}'", fg="red")
-            sys.exit(1)
 
     if p.tart_registry_username and p.tart_registry_password and p.tart_registry:
         click.echo(f"[INFO] Logging into custom OCI Registry '{p.tart_registry}'")
         try:
             tart.login(username=p.tart_registry_username, password=p.tart_registry_password, host=p.tart_registry)
         except:
             click.secho(f"[ERROR] Failed to login to '{p.tart_registry}'", fg="red")
-            sys.exit(1)
 
     ######################################################################
     # PULL
     ######################################################################
     if (
         (pull_policy == "always")
         or (p.ci_job_image not in tart_vm_map and pull_policy != "never")
@@ -175,63 +182,62 @@
     elif auto_resources:
         click.echo("[INFO] Auto resource-disribution enabled.")
         host_spec = get_host_spec()
         tart.set(tart_vm_name, cpu=int(host_spec.cpu_count / concurrency), memory=int(host_spec.memory / concurrency))
 
     click.echo(f"[INFO] Starting VM instance '{tart_vm_name}'")
 
-    mount_dirs = []
+    remote_build_dir = "/opt/builds"
+    remote_script_dir = "/opt/temp"
+    remote_cache_dir = "/opt/cache"
+
+    volume_mounts = []
     if cache_dir:
         cache_dir = os.path.abspath(os.path.expanduser(cache_dir))
         os.makedirs(cache_dir, exist_ok=True)
         click.echo(f"[INFO] Cache directory set to '{cache_dir}'")
-        mount_dirs.append(TartMount(source=cache_dir, dest="cache"))
+        volume_mounts.append(TartVolume(source=cache_dir, dest=remote_cache_dir, name="cache", ro=False))
     if builds_dir:
         # Concurrency compatible builds directory
         # see https://docs.gitlab.com/runner/executors/shell.html#run-scripts-as-a-privileged-user
         # <builds_dir>/<short-token>/<concurrent-id>/<namespace>/<project-name>.
         builds_dir = os.path.join(
             os.path.abspath(os.path.expanduser(builds_dir)), p.ci_runner_short_token, p.ci_concurrent_project_id
         )
         os.makedirs(builds_dir, exist_ok=True)
         click.echo(f"[INFO] Builds directory set to '{builds_dir}'")
-        mount_dirs.append(TartMount(source=builds_dir, dest="builds"))
+        volume_mounts.append(TartVolume(source=builds_dir, dest=remote_build_dir, name="builds", ro=False))
+
+    for v in volumes:
+        volume_mounts.append(TartVolume.from_string(v))
 
-    tart.run(tart_vm_name, mount_dirs)
+    tart.run(tart_vm_name, volume_mounts)
     ip = tart.ip(tart_vm_name, timeout=timeout)
     if not ip:
         click.echo(f"[ERROR] Error, VM was not reacheable after '{timeout}' seconds")
         sys.exit(1)
 
     ssh_session = tart.ssh_session(name=p.vm_name(), username=p.tart_ssh_username, password=p.tart_ssh_password)
-
-    remote_build_dir = "/opt/builds"
-    remote_script_dir = "/opt/temp"
-    remote_cache_dir = "/opt/cache"
-
     ssh_session.exec_ssh_command(
         f"sudo mkdir -p {remote_script_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_script_dir}",
     )
 
-    if cache_dir:
-        click.echo("[INFO] Bootstrapping cache directory")
+    for volume in volume_mounts:
+        click.echo("[INFO] Setting up volume mount '{volume.name}'")
         ssh_session.exec_ssh_command(
-            f"sudo ln -sf '/Volumes/My Shared Files/cache' {remote_cache_dir}",
+            f"sudo mkdir -p $(dirname {volume.dest}); sudo ln -sf '/Volumes/My Shared Files/{volume.name}' {volume.dest}",
         )
-    else:
+
+    # if cache and builds volumes are not mounted, make sure to create them locally inside the VM
+    if not cache_dir:
         ssh_session.exec_ssh_command(
             f"sudo mkdir -p {remote_cache_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_cache_dir}",
         )
 
-    if builds_dir:
-        click.echo("[INFO] Bootstrapping builds directory")
-        ssh_session.exec_ssh_command(
-            f"sudo ln -sf '/Volumes/My Shared Files/builds' {remote_build_dir}",
-        )
-    else:
+    if not builds_dir:
         ssh_session.exec_ssh_command(
             f"sudo mkdir -p {remote_build_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_build_dir}",
         )
 
     tart.print_spec(tart_vm_name)
 
     sys.exit(0)
```

### Comparing `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/run.py` & `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/commands/run.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py` & `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/tart.py` & `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/tart.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,37 @@
     memory: int
     disk: int
     display: str
     running: bool
     ip_address: str
 
 
-class TartMount(BaseModel):
+class TartVolume(BaseModel):
+    name: str
     source: str
     dest: str
+    ro: bool = Field(default=False)
+
+    @classmethod
+    def from_string(cls, value):
+        components = value.split(":")
+        if len(components) < 2:
+            raise ValueError(f"'{value}' is not a valid volume mount definition")
+
+        source = os.path.abspath(os.path.expanduser(components[0])).rstrip("/")
+        dest = components[1].rstrip("/")
+        name = dest.strip("/").replace("/", "__")
+        ro = False
+        if len(components) > 2:
+            if "ro" == components[2]:
+                ro = True
+            else:
+                raise ValueError(f"'{components[2]}' flag unknown")
+
+        return cls(name=name, source=source, dest=dest, ro=ro)
 
 
 class TartSshSession:
     def __init__(self, username, password, ip):
         self.user = username
         self.ip = ip
         self.password = password
@@ -126,24 +146,26 @@
         ]
         print(tabulate(data, headers=["CPU", "Memory", "Disk", "Display", "Running", "IP Address"], tablefmt=tablefmt))
 
     def stop(self, name) -> None:
         """stops a given tart VM"""
         self.exec(["stop", name])
 
-    def run(self, name: str, dirs: list[TartMount] = [], no_graphics=True) -> None:
+    def run(self, name: str, volumes: list[TartVolume] = [], no_graphics=True) -> None:
         """starts a given tart VM"""
         args = ["run", name]
         if no_graphics:
             args.append("--no-graphics")
 
-        if dirs:
-            for d in dirs:
-                args.extend(["--dir", f"{d.dest}:{os.path.abspath(os.path.expanduser(d.source))}"])
-
+        if volumes:
+            for d in volumes:
+                source_path = os.path.abspath(os.path.expanduser(d.source))
+                if d.ro:
+                    source_path = f"{source_path}:ro"
+                args.extend(["--dir", f"{d.name}:{source_path}"])
         try:
             self.spawn_exec(args)
         except Exception as e:
             print(f"Error when running VM {name}")
             raise e
 
     def ip(self, name, timeout=30, resolver="dhcp") -> str:
```

### Comparing `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/utils.py` & `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver/modules/utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/PKG-INFO` & `gitlab-runner-tart-driver-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: gitlab-runner-tart-driver
-Version: 0.1.2
-Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
-Author: Matthias Schmieder
-Author-email: schmieder.matthias@gmail.com
-License: BSD
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Version Control
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Gitlab Runner Custom Tart Driver
 
 ## About
 
 [Tart](https://tart.run) is a virtualization toolset to build, run and manage macOS and Linux virtual machines on Apple Silicon. Tart is using Apple’s native Virtualization.Framework that was developed along with architecting the first M1 chip. This seamless integration between hardware and software ensures smooth performance without any drawbacks.
 
 For storing virtual machine images Tart integrates with **OCI-compatible container registries**. This allows you to work with virtual machines as you used to with Docker containers.
@@ -110,23 +95,26 @@
 
 **config.toml**
 
 ```ini
 [runners.custom]
     config_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     config_args = [ "config", '-x', '/opt/homebrew/bin/tart' ]
+    config_exec_timeout = 200
 
     prepare_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     prepare_args = [ "prepare", '-x', '/opt/homebrew/bin/tart' ]
+    prepare_exec_timeout = 200
 
     run_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     run_args = [ "run", '-x', '/opt/homebrew/bin/tart' ]
 
     cleanup_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     cleanup_args = [ "cleanup", '-x', '/opt/homebrew/bin/tart' ]
+    cleanup_exec_timeout = 200
 ```
 
 Now restart the gitlab-runner with `gitlab-runner restart`
 
 ## GitLab CI
 
 One of the great advantages in using [Tart](https://tart.run) is that it gives almost all functionality to we are used from the standard `docker` executors allowing us to write GitLabCI piplines that do not need any or minimal adaptions for OSX.
@@ -272,14 +260,30 @@
 To enable Host-local caching and builds, simply pass `--builds-dir` and `--cache-dir` to the `prepare` command
 
 ```ini
 prepare_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
 prepare_args = [ "prepare", '-x', '/opt/homebrew/bin/tart', '--concurrency', '2', '--auto-resources', '--cache-dir', '/Users/gitlab/gitlab-runner/cache', '--builds-dir', '/Users/gitlab/gitlab-runner/builds']
 ```
 
+### Volume Mounts
+
+Just like with `docker` the `gitlab-runner-tart-driver` allows you to mount any arbitrary host path into your VM. This can be especially useful if you have to mount runner-local resources like shared test-data or additional caches into the executor. You can follow the standard docker syntax for *volume mounts* `--volume /my/local/dir:/opt/remote/dir`. Additionally you can also pass the `ro` flag to make the mount *read-only* i.e.  `--volume /my/local/dir:/opt/remote/dir:ro`.
+
+```ini
+[runners.custom]
+  config_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
+  config_args = [ "config" ]
+
+  prepare_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
+  prepare_args = [ "prepare",
+    '-x', '/opt/homebrew/bin/tart',
+    '--concurrency', '2',
+    '--auto-resources',
+    '--volume /data/models/:/opt/data/models:ro']
+```
 ### Auto Host Resource Distribution
 
 `tart` images come with a pre-defined number of CPUs and Memory allocation. Typical numbers for default images are `cpu_count=4` and `memory=8192`. With the concurrency limitation of two VMs/images running at the same time this might not utilize your host system completely.
 Per default, `--auto-resources` is enable for the `gitlab-runner-tart-driver` which will split the host resources equally to the VMs defined by `--concurrency`. The default concurrency is `1` and therefore will assign all host resources to the VM.
 
 > **ATTENTION** make sure your `gitlab-runner` concurrency setting is the same as the `--concurrency` parameter you are passing to the `prepare` command
 
@@ -352,16 +356,18 @@
   --concurrency INTEGER           Number of concurrent processes that are
                                   supported. ATTENTION tart currently only
                                   support two concurrent VMs
   --cache-dir TEXT                Caching dir to be used.
   --builds-dir TEXT               Path to the builds directory.
   --timeout INTEGER               Timeout in seconds for the VM to be
                                   reachable via SSH.
+  --volume TEXT                   Volume mount definition with docker syntax.
+                                  <host_dir>:<vm_dir>[:ro]
   -x, --tart-executable TEXT      Path to the tart executable.
-  --help                          Show this message and exit.
+  --help                          Show this message and exit.                      Show this message and exit.
 ```
 
 ### Command `run`
 
 ```
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
 
@@ -382,8 +388,8 @@
 Usage: gitlab-runner-tart-driver cleanup [OPTIONS]
 
   Command to greet a user.
 
 Options:
   -x, --tart-executable TEXT  Path to the tart executable.
   --help                      Show this message and exit.
-```
+```
```

### Comparing `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/SOURCES.txt` & `gitlab-runner-tart-driver-0.1.3/gitlab_runner_tart_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.2/setup.py` & `gitlab-runner-tart-driver-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 # read the long description from README.md
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.1.2"
+version = "0.1.3"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
```

