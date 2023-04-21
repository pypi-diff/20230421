# Comparing `tmp/sshlab-0.1.3.tar.gz` & `tmp/sshlab-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshlab-0.1.3.tar", last modified: Tue Apr 18 19:14:50 2023, max compression
+gzip compressed data, was "sshlab-0.2.0.tar", last modified: Fri Apr 21 14:24:49 2023, max compression
```

## Comparing `sshlab-0.1.3.tar` & `sshlab-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:14:50.736395 sshlab-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-18 19:14:39.000000 sshlab-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-18 19:14:50.732396 sshlab-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-18 19:14:39.000000 sshlab-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 19:14:50.736395 sshlab-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-18 19:14:39.000000 sshlab-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:14:50.732396 sshlab-0.1.3/sshlab/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 19:14:39.000000 sshlab-0.1.3/sshlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-18 19:14:39.000000 sshlab-0.1.3/sshlab/sshlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-18 19:14:39.000000 sshlab-0.1.3/sshlab/sshlab_kill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-18 19:14:39.000000 sshlab-0.1.3/sshlab/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 19:14:39.000000 sshlab-0.1.3/sshlab/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:14:50.732396 sshlab-0.1.3/sshlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-18 19:14:50.000000 sshlab-0.1.3/sshlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-18 19:14:50.000000 sshlab-0.1.3/sshlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:14:50.000000 sshlab-0.1.3/sshlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 19:14:50.000000 sshlab-0.1.3/sshlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 19:14:50.000000 sshlab-0.1.3/sshlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 19:14:50.000000 sshlab-0.1.3/sshlab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:24:49.208774 sshlab-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-21 14:24:38.000000 sshlab-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-21 14:24:49.208774 sshlab-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-21 14:24:38.000000 sshlab-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:24:49.208774 sshlab-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-21 14:24:38.000000 sshlab-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:24:49.204774 sshlab-0.2.0/sshlab/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-21 14:24:38.000000 sshlab-0.2.0/sshlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-21 14:24:38.000000 sshlab-0.2.0/sshlab/sshlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-21 14:24:38.000000 sshlab-0.2.0/sshlab/sshlab_kill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-21 14:24:38.000000 sshlab-0.2.0/sshlab/sshtensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-21 14:24:38.000000 sshlab-0.2.0/sshlab/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 14:24:38.000000 sshlab-0.2.0/sshlab/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:24:49.208774 sshlab-0.2.0/sshlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-21 14:24:49.000000 sshlab-0.2.0/sshlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-21 14:24:49.000000 sshlab-0.2.0/sshlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:24:49.000000 sshlab-0.2.0/sshlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-21 14:24:49.000000 sshlab-0.2.0/sshlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 14:24:49.000000 sshlab-0.2.0/sshlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 14:24:49.000000 sshlab-0.2.0/sshlab.egg-info/top_level.txt
```

### Comparing `sshlab-0.1.3/LICENSE` & `sshlab-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sshlab-0.1.3/PKG-INFO` & `sshlab-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: sshlab
-Version: 0.1.3
+Version: 0.2.0
 Summary: A tool for launching Jupyter Notebooks on remote servers using SSH
 Home-page: https://github.com/vuillaut/sshlab
 Author: Thomas Vuillaume
 Author-email: thomas.vuillaume@lapp.in2p3.fr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+Provides-Extra: doc
 License-File: LICENSE
 
 # sshlab
 
-Jupyter notebook / lab through ssh with a single command and config file
+Jupyter notebook / lab and tensorboard through ssh with a single command and config file
 
 This script is inspired by https://github.com/nicolaschotard/stackyter but reimplemented to allow starting Jupyter in a container (singularity or docker) in the remote server
 
+# Documentation
+
+Visit https://vuillaut.github.io/sshlab/
+
 # Usage
 
 Copy the example settings file `.sshlab_config.yml` to your HOME and edit it to your needs.
 
 ## Install
```

### Comparing `sshlab-0.1.3/sshlab/sshlab.py` & `sshlab-0.2.0/sshlab/sshlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from . import utils
 
 
 DEFAULT_CONFIG_FILE = os.getenv("HOME") + "/.sshlab_config.yml"
 
 
-
 def cleanup(user, server, process):
     # Get the PID of the remote Jupyter process
     utils.kill_remote_jupyter(user, server)
 
     # Check if the process is still running
     if process.poll() is None:
         # Terminate the SSH connection
@@ -52,15 +51,15 @@
     # Get the SSH settings from the config file
     user = config['SSH']['user']
     server = config['SSH']['server']
     specified_port = int(config['SSH'].get('port', '8888'))
     ip = config['SSH'].get('ip', '127.0.0.1')
 
     # Check if the specified port is available, and find an available port if it's not
-    port = specified_port if utils.is_port_available(specified_port) else find_available_port(specified_port)
+    port = specified_port if utils.is_port_available(specified_port) else utils.find_available_port(specified_port)
 
     # Build the SSH command string
     ssh_cmd = f'ssh -L {port}:{ip}:{port} {user}@{server}'
 
     # Get the environment settings from the config file
     env_cmd = config['Environment']['cmd']
     env_target = config['Environment']['target']
```

### Comparing `sshlab-0.1.3/sshlab/sshlab_kill.py` & `sshlab-0.2.0/sshlab/sshlab_kill.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import argparse
 import os
 import yaml
 from pathlib import Path
-from . utils import get_remote_jupyter_pid, kill_remote_jupyter
+from . utils import kill_remote_process
 
 DEFAULT_CONFIG_FILE = os.getenv("HOME") + "/.sshlab_config.yml"
 
 def build_argparser():
     # Parse command-line arguments
     parser = argparse.ArgumentParser()
-    parser.add_argument('--config', '-c', default=None, help='User configuration name to use (defined in the config file)')
-    parser.add_argument('--file', '-f', default=DEFAULT_CONFIG_FILE, type=Path, help=f'YAML configuration file, default: {DEFAULT_CONFIG_FILE}')
+    parser.add_argument('--config', '-c', 
+                        default=None, 
+                        help='User configuration name to use (defined in the config file)')
+    parser.add_argument('--file', '-f', 
+                        default=DEFAULT_CONFIG_FILE,
+                         type=Path,
+                         help=f'YAML configuration file, default: {DEFAULT_CONFIG_FILE}')
+    parser.add_argument('--process', '-p', default='jupyter', type=str,
+                         help=f'Process name to kill, default: jupyter')
     args = parser.parse_args()
     return args
 
 
 def main():
     args = build_argparser()
 
@@ -31,11 +38,11 @@
     print(f'Using configuration: {config_name}\n')
 
     # Get the SSH settings from the config file
     user = config['SSH']['user']
     server = config['SSH']['server']
 
     # Kill the remote Jupyter process
-    kill_remote_jupyter(user, server)
+    kill_remote_process(user, server, args.process)
 
 if __name__ == '__main__':
     main()
```

### Comparing `sshlab-0.1.3/sshlab/utils.py` & `sshlab-0.2.0/sshlab/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,44 +13,70 @@
 def find_available_port(start_port=8888):
     port = start_port
     while not is_port_available(port):
         port += 1
     return port
 
 
-# Function to get the PID of the remote Jupyter process
-def get_remote_jupyter_pid(user, server):
-    jupyter_pid_cmd = f"ssh {user}@{server} 'pgrep -f jupyter -u {user}'"
+def get_remote_cmd_pid(user, server, cmd):
+    pid_cmd = f"ssh {user}@{server} 'pgrep -f \"{cmd}\" -u {user}'"
     try:
-        output = subprocess.check_output(jupyter_pid_cmd, shell=True).decode().strip().split('\n')[0].strip()
+        output = subprocess.check_output(pid_cmd, shell=True).decode().strip().split('\n')[0].strip()
         pid = int(output)
     except (subprocess.CalledProcessError, ValueError):
         pid = None
 
     return pid
 
 
-def kill_remote_jupyter(user, server):
-    pid = get_remote_jupyter_pid(user, server)
+def get_remote_jupyter_pid(user, server):
+    jupyter_cmd = 'jupyter'
+    return get_remote_cmd_pid(user, server, jupyter_cmd)
+
+
+def get_remote_tensorboard_pid(user, server):
+    tensorboard_cmd = 'tensorboard'
+    return get_remote_cmd_pid(user, server, tensorboard_cmd)
+
+
+def kill_remote_process(user, server, cmd):
+    pid = get_remote_cmd_pid(user, server, cmd)
+    print(f"PID {pid}")
     
     if pid:
-        print(f"Jupyter server PID on remote machine: {pid}")
+        print(f"Process PID on remote machine: {pid}")
         kill_cmd = f"ssh {user}@{server} 'kill -TERM {pid} &> /dev/null'"
         subprocess.run(kill_cmd, shell=True)
-        print(f"Sent termination signal to Jupyter server {pid} on the remote machine.")
+        print(f"Sent termination signal to process {pid} on the remote machine.")
         
-        # Wait for the Jupyter process to terminate
+        # Wait for the process to terminate
         max_retries = 5
         retry_count = 0
         while retry_count < max_retries:
             time.sleep(1)
-            current_pid = get_remote_jupyter_pid(user, server)
+            current_pid = get_remote_cmd_pid(user, server, cmd)
             if not current_pid:
-                print(f"Terminated the Jupyter server {pid} on the remote machine.")
+                print(f"Terminated the process {pid} on the remote machine.")
                 break
             else:
-                print(f"Jupyter server {pid} still running. Retry count: {retry_count}")
+                print(f"Process {pid} still running. Retry count: {retry_count}")
             retry_count += 1
         else:
-            print(f"Unable to terminate the Jupyter server {pid} on the remote machine.")
+            print(f"Unable to terminate the process {pid} on the remote machine.")
     else:
-        print("No Jupyter server found on the remote machine.")
+        print("No process found on the remote machine.")
+
+
+def kill_remote_jupyter(user, server):
+    jupyter_cmd = 'jupyter'
+    kill_remote_process(user, server, jupyter_cmd)
+
+
+def kill_remote_tensorboard(user, server):
+    tensorboard_cmd = 'tensorboard'
+    kill_remote_process(user, server, tensorboard_cmd)
+
+
+def delete_remote_dir(user, server, dir_path):
+    print(f"Deleting temporary directory {dir_path} on the remote machine.")
+    delete_cmd = f"ssh {user}@{server} 'rm -rf {dir_path}'"
+    subprocess.run(delete_cmd, shell=True)
```

### Comparing `sshlab-0.1.3/sshlab.egg-info/PKG-INFO` & `sshlab-0.2.0/sshlab.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: sshlab
-Version: 0.1.3
+Version: 0.2.0
 Summary: A tool for launching Jupyter Notebooks on remote servers using SSH
 Home-page: https://github.com/vuillaut/sshlab
 Author: Thomas Vuillaume
 Author-email: thomas.vuillaume@lapp.in2p3.fr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+Provides-Extra: doc
 License-File: LICENSE
 
 # sshlab
 
-Jupyter notebook / lab through ssh with a single command and config file
+Jupyter notebook / lab and tensorboard through ssh with a single command and config file
 
 This script is inspired by https://github.com/nicolaschotard/stackyter but reimplemented to allow starting Jupyter in a container (singularity or docker) in the remote server
 
+# Documentation
+
+Visit https://vuillaut.github.io/sshlab/
+
 # Usage
 
 Copy the example settings file `.sshlab_config.yml` to your HOME and edit it to your needs.
 
 ## Install
```

