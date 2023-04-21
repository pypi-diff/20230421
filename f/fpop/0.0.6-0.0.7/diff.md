# Comparing `tmp/fpop-0.0.6.tar.gz` & `tmp/fpop-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpop-0.0.6.tar", last modified: Mon Apr 17 13:05:04 2023, max compression
+gzip compressed data, was "fpop-0.0.7.tar", last modified: Fri Apr 21 14:15:17 2023, max compression
```

## Comparing `fpop-0.0.6.tar` & `fpop-0.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 4294967294 4294967294        0 2023-04-17 13:05:04.759537 fpop-0.0.6/
--rw-r--r--   0 4294967294 4294967294     7650 2023-04-17 12:56:30.000000 fpop-0.0.6/LICENSE
--rw-r--r--   0 4294967294 4294967294       16 2023-04-17 12:56:30.000000 fpop-0.0.6/MANIFEST.in
--rw-r--r--   0 4294967294 4294967294      935 2023-04-17 13:05:04.755285 fpop-0.0.6/PKG-INFO
--rw-r--r--   0 4294967294 4294967294      443 2023-04-17 12:56:30.000000 fpop-0.0.6/README.md
-drwxr-xr-x   0 4294967294 4294967294        0 2023-04-17 13:05:04.473580 fpop-0.0.6/fpop/
--rw-r--r--   0 4294967294 4294967294       24 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/__about__.py
--rw-r--r--   0 4294967294 4294967294        0 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/__init__.py
--rw-r--r--   0 4294967294 4294967294    18359 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/abacus.py
--rw-r--r--   0 4294967294 4294967294     6271 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/prep_fp.py
--rw-r--r--   0 4294967294 4294967294     6496 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/preprun_fp.py
--rw-r--r--   0 4294967294 4294967294     6387 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/run_fp.py
-drwxr-xr-x   0 4294967294 4294967294        0 2023-04-17 13:05:04.568984 fpop-0.0.6/fpop/utils/
--rw-r--r--   0 4294967294 4294967294        0 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/utils/__init__.py
--rw-r--r--   0 4294967294 4294967294      407 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/utils/step_config.py
--rw-r--r--   0 4294967294 4294967294     8936 2023-04-17 12:56:30.000000 fpop-0.0.6/fpop/vasp.py
-drwxr-xr-x   0 4294967294 4294967294        0 2023-04-17 13:05:04.545326 fpop-0.0.6/fpop.egg-info/
--rw-r--r--   0 4294967294 4294967294      935 2023-04-17 13:05:04.000000 fpop-0.0.6/fpop.egg-info/PKG-INFO
--rw-r--r--   0 4294967294 4294967294      614 2023-04-17 13:05:04.000000 fpop-0.0.6/fpop.egg-info/SOURCES.txt
--rw-r--r--   0 4294967294 4294967294        1 2023-04-17 13:05:04.000000 fpop-0.0.6/fpop.egg-info/dependency_links.txt
--rw-r--r--   0 4294967294 4294967294       31 2023-04-17 13:05:04.000000 fpop-0.0.6/fpop.egg-info/requires.txt
--rw-r--r--   0 4294967294 4294967294       11 2023-04-17 13:05:04.000000 fpop-0.0.6/fpop.egg-info/top_level.txt
--rw-r--r--   0 4294967294 4294967294       38 2023-04-17 13:05:04.761684 fpop-0.0.6/setup.cfg
--rw-r--r--   0 4294967294 4294967294      847 2023-04-17 12:56:30.000000 fpop-0.0.6/setup.py
-drwxr-xr-x   0 4294967294 4294967294        0 2023-04-17 13:05:04.741001 fpop-0.0.6/tests/
--rw-r--r--   0 4294967294 4294967294        0 2023-04-17 12:56:30.000000 fpop-0.0.6/tests/__init__.py
--rw-r--r--   0 4294967294 4294967294     2097 2023-04-17 12:56:30.000000 fpop-0.0.6/tests/constants.py
--rw-r--r--   0 4294967294 4294967294      716 2023-04-17 12:56:30.000000 fpop-0.0.6/tests/context.py
--rw-r--r--   0 4294967294 4294967294     2401 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/mocked_ops.py
--rw-r--r--   0 4294967294 4294967294     8032 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_abacus_inputs.py
--rw-r--r--   0 4294967294 4294967294     6686 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_prep_abacus.py
--rw-r--r--   0 4294967294 4294967294     7994 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_prep_run_vasp.py
--rw-r--r--   0 4294967294 4294967294     7321 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_prep_vasp.py
--rw-r--r--   0 4294967294 4294967294     5919 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_run_abacus.py
--rw-r--r--   0 4294967294 4294967294      943 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_run_fp.py
--rw-r--r--   0 4294967294 4294967294     6387 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_run_vasp.py
--rw-r--r--   0 4294967294 4294967294     2844 2023-04-17 12:56:31.000000 fpop-0.0.6/tests/test_vasp_inputs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 14:15:17.230385 fpop-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)     7650 2023-04-21 13:24:02.000000 fpop-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-21 13:24:02.000000 fpop-0.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      935 2023-04-21 14:15:17.230385 fpop-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      443 2023-04-21 13:24:02.000000 fpop-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 14:15:17.227384 fpop-0.0.7/fpop/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-21 13:24:02.000000 fpop-0.0.7/fpop/__about__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 13:24:02.000000 fpop-0.0.7/fpop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18426 2023-04-21 14:07:13.000000 fpop-0.0.7/fpop/abacus.py
+-rw-r--r--   0 root         (0) root         (0)     6248 2023-04-21 13:36:23.000000 fpop-0.0.7/fpop/prep_fp.py
+-rw-r--r--   0 root         (0) root         (0)     6496 2023-04-21 13:24:02.000000 fpop-0.0.7/fpop/preprun_fp.py
+-rw-r--r--   0 root         (0) root         (0)     6285 2023-04-21 13:36:56.000000 fpop-0.0.7/fpop/run_fp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 14:15:17.228385 fpop-0.0.7/fpop/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 13:24:02.000000 fpop-0.0.7/fpop/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-04-21 13:24:02.000000 fpop-0.0.7/fpop/utils/step_config.py
+-rw-r--r--   0 root         (0) root         (0)     8936 2023-04-21 13:24:02.000000 fpop-0.0.7/fpop/vasp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 14:15:17.228385 fpop-0.0.7/fpop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      935 2023-04-21 14:15:17.000000 fpop-0.0.7/fpop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      614 2023-04-21 14:15:17.000000 fpop-0.0.7/fpop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 14:15:17.000000 fpop-0.0.7/fpop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-21 14:15:17.000000 fpop-0.0.7/fpop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-21 14:15:17.000000 fpop-0.0.7/fpop.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 14:15:17.230385 fpop-0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      847 2023-04-21 14:08:17.000000 fpop-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 14:15:17.230385 fpop-0.0.7/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 13:24:02.000000 fpop-0.0.7/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-04-21 13:24:02.000000 fpop-0.0.7/tests/constants.py
+-rw-r--r--   0 root         (0) root         (0)      716 2023-04-21 13:24:02.000000 fpop-0.0.7/tests/context.py
+-rw-r--r--   0 root         (0) root         (0)     2401 2023-04-21 13:24:02.000000 fpop-0.0.7/tests/mocked_ops.py
+-rw-r--r--   0 root         (0) root         (0)     8032 2023-04-21 13:24:02.000000 fpop-0.0.7/tests/test_abacus_inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6686 2023-04-21 13:24:02.000000 fpop-0.0.7/tests/test_prep_abacus.py
+-rw-r--r--   0 root         (0) root         (0)     7994 2023-04-21 13:24:02.000000 fpop-0.0.7/tests/test_prep_run_vasp.py
+-rw-r--r--   0 root         (0) root         (0)     7321 2023-04-21 13:24:02.000000 fpop-0.0.7/tests/test_prep_vasp.py
+-rw-r--r--   0 root         (0) root         (0)     5919 2023-04-21 13:24:02.000000 fpop-0.0.7/tests/test_run_abacus.py
+-rw-r--r--   0 root         (0) root         (0)      943 2023-04-21 13:24:02.000000 fpop-0.0.7/tests/test_run_fp.py
+-rw-r--r--   0 root         (0) root         (0)     6387 2023-04-21 13:24:02.000000 fpop-0.0.7/tests/test_run_vasp.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-04-21 13:24:02.000000 fpop-0.0.7/tests/test_vasp_inputs.py
```

### Comparing `fpop-0.0.6/LICENSE` & `fpop-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fpop-0.0.6/PKG-INFO` & `fpop-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpop
-Version: 0.0.6
+Version: 0.0.7
 Summary: Operators related to first-principles calculation
 Home-page: https://github.com/deepmodeling/fpop
 Author: Chengqian Zhang
 Author-email: 2043899742@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `fpop-0.0.6/fpop/abacus.py` & `fpop-0.0.7/fpop/abacus.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 from fpop.prep_fp import PrepFp
 from fpop.run_fp import RunFp
-import dpdata, sys, subprocess, os, shutil,re
+import sys, subprocess, os, shutil,re
 from pathlib import Path
 from dflow.utils import run_command
 from typing import (
     Any,
     Tuple,
     List,
     Set,
     Dict,
     Optional,
     Union,
 )
 import numpy as np
-from dargs import (
-    dargs, 
-    Argument, 
-    Variant, 
-    ArgumentEncoder,
-)
 from dflow.python import (
     OP,
     OPIO,
     OPIOSign,
     Artifact,
     TransientError,
     FatalError,
@@ -518,15 +512,15 @@
         for i in element_list:
             mass.append(self._mass.get(i,MASS_DICT.get(i,1.0)))
         return mass
 
 class PrepAbacus(PrepFp):
     def prep_task(
             self,
-            conf_frame: dpdata.System,
+            conf_frame,
             abacus_inputs: AbacusInputs,
             prepare_image_config: Optional[Dict] = None,
             optional_input: Optional[Dict] = None,
             optional_artifact: Optional[Dict] = None,
     ):
         r"""Define how one Abacus task is prepared.
 
@@ -602,39 +596,42 @@
         return files
 
     def run_task(
         self,
         backward_dir_name,
         log_name,
         backward_list: List[str],
-        run_config: Optional[Dict]=None,
+        run_image_config: Optional[Dict]=None,
         optional_input: Optional[Dict]=None,
     ) -> str:
         r'''Defines how one FP task runs
         Parameters
         ----------
         backward_dir_name:
             The name of the directory which contains the backward files.
         log_name:
             The name of log file.
         backward_list:
             The output files the users need.
-        run_config:
-            Keyword args defined by the developer.
-            The fp/run_config session of the input file will be passed to this function.
+        run_image_config:
+            Keyword args defined by the developer.For example:
+            {
+              "command": "source /opt/intel/oneapi/setvars.sh && mpirun -n 16 abacus"
+            }
         optional_input:
             The parameters developers need in runtime.
         
         Returns
         -------
         backward_dir_name: str
             The directory name which containers the files users need.
         '''
-        if run_config:
-            command = run_config["command"]
+        
+        if run_image_config:
+            command = run_image_config["command"]
         else:
             command = "abacus"
         # run abacus
         command = " ".join([command, ">", log_name])
         ret, out, err = run_command(command, raise_error=False, try_bash=True,)
         if ret != 0:
             raise TransientError(
@@ -643,15 +640,18 @@
         if not self.check_run_success(log_name):
             raise TransientError(
                 "abacus failed , we could not check the exact cause . Please check log file ."
             )
         os.makedirs(Path(backward_dir_name))
         shutil.copyfile(log_name,Path(backward_dir_name)/log_name)
         for ii in backward_list:
-            shutil.copyfile(ii,Path(backward_dir_name)/ii)
+            try:
+                shutil.copyfile(ii,Path(backward_dir_name)/ii)
+            except:
+                shutil.copytree(ii,Path(backward_dir_name)/ii)
         return backward_dir_name
 
     def check_run_success(self,log_name):
         with open(log_name,"r") as f:
             lines = f.readlines()
         if "SEE INFORMATION IN" in lines[-1]:
             return True
```

### Comparing `fpop-0.0.6/fpop/prep_fp.py` & `fpop-0.0.7/fpop/prep_fp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from abc import ABC,abstractmethod
 import os
-import dpdata
 from pathlib import Path
 from dflow.utils import set_directory
 from dflow.python import (
     PythonOPTemplate,
     OP,
     OPIO,
     OPIOSign,
@@ -51,15 +50,15 @@
             "task_names": List[str],
             "task_paths" : Artifact(List[Path]),
         })
 
     @abstractmethod
     def prep_task(
             self,
-            conf_frame: dpdata.System,
+            conf_frame,
             inputs: Any,
             prepare_image_config: Optional[Dict] = None,
             optional_input: Optional[Dict] = None,
             optional_artifact: Optional[Dict] = None,
     ):
         r"""Define how one FP task is prepared.
 
@@ -113,14 +112,15 @@
         -------
         op : dict 
             Output dict with components:
 
             - `task_names`: (`List[str]`) The name of tasks. Will be used as the identities of the tasks. The names of different tasks are different.
             - `task_paths`: (`Artifact(List[Path])`) The parepared working paths of the tasks. Contains all input files needed to start the FP. The order fo the Paths should be consistent with `op["task_names"]`
         """
+        import dpdata
 
         inputs = ip['inputs']
         confs = ip['confs']
         type_map = ip['type_map']
         prepare_image_config = ip["prep_image_config"]
         optional_artifact = ip["optional_artifact"]
         optional_input = ip["optional_input"]
@@ -149,15 +149,15 @@
         })
 
 
     def _exec_one_frame(
             self,
             idx,
             inputs,
-            conf_frame : dpdata.System,
+            conf_frame,
             prepare_image_config = None,
             optional_input = None,
             optional_artifact = None,
     ) -> Tuple[str, Path]:
         task_name = 'task.' + '%06d' % idx
         task_path = Path(task_name)
         with set_directory(task_path,mkdir=True):
```

### Comparing `fpop-0.0.6/fpop/preprun_fp.py` & `fpop-0.0.7/fpop/preprun_fp.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.6/fpop/run_fp.py` & `fpop-0.0.7/fpop/run_fp.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,33 +15,26 @@
     Step,
     upload_artifact,
     download_artifact,
     InputArtifact,
     OutputArtifact,
     ShellOPTemplate
 )
-import os, json, dpdata, shutil
+import os, json, shutil
 from pathlib import Path
 from typing import (
     Any,
     Tuple,
     List,
     Set,
     Dict,
     Optional,
     Union,
 )
 import numpy as np
-import dargs
-from dargs import (
-    dargs,
-    Argument,
-    Variant,
-    ArgumentEncoder,
-)
 
 class RunFp(OP, ABC):
     r'''Execute a first-principles (FP) task.
     A working directory named `task_name` is created. All input files
     are copied or symbol linked to directory `task_name`. The FP
     command is exectuted from directory `task_name`. 
     '''
```

### Comparing `fpop-0.0.6/fpop/vasp.py` & `fpop-0.0.7/fpop/vasp.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.6/fpop.egg-info/PKG-INFO` & `fpop-0.0.7/fpop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpop
-Version: 0.0.6
+Version: 0.0.7
 Summary: Operators related to first-principles calculation
 Home-page: https://github.com/deepmodeling/fpop
 Author: Chengqian Zhang
 Author-email: 2043899742@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `fpop-0.0.6/fpop.egg-info/SOURCES.txt` & `fpop-0.0.7/fpop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fpop-0.0.6/setup.py` & `fpop-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fpop",
-    version="0.0.6",
+    version="0.0.7",
     author="Chengqian Zhang",
     author_email="2043899742@qq.com",
     description="Operators related to first-principles calculation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepmodeling/fpop",
     packages=setuptools.find_packages(),
```

### Comparing `fpop-0.0.6/tests/constants.py` & `fpop-0.0.7/tests/constants.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.6/tests/context.py` & `fpop-0.0.7/tests/context.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.6/tests/mocked_ops.py` & `fpop-0.0.7/tests/mocked_ops.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.6/tests/test_abacus_inputs.py` & `fpop-0.0.7/tests/test_abacus_inputs.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.6/tests/test_prep_abacus.py` & `fpop-0.0.7/tests/test_prep_abacus.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.6/tests/test_prep_run_vasp.py` & `fpop-0.0.7/tests/test_prep_run_vasp.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.6/tests/test_prep_vasp.py` & `fpop-0.0.7/tests/test_prep_vasp.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.6/tests/test_run_abacus.py` & `fpop-0.0.7/tests/test_run_abacus.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.6/tests/test_run_fp.py` & `fpop-0.0.7/tests/test_run_fp.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.6/tests/test_run_vasp.py` & `fpop-0.0.7/tests/test_run_vasp.py`

 * *Files identical despite different names*

### Comparing `fpop-0.0.6/tests/test_vasp_inputs.py` & `fpop-0.0.7/tests/test_vasp_inputs.py`

 * *Files identical despite different names*

