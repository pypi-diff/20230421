# Comparing `tmp/up_lpg-0.0.6.1-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/up_lpg-0.0.6.2-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1190304 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       36 b- defN 23-Apr-17 10:27 up_lpg/__init__.py
--rw-rw-rw-  2.0 fat     9713 b- defN 23-Apr-17 10:27 up_lpg/lpg_planner.py
--rw-rw-rw-  2.0 fat  3881596 b- defN 23-Apr-17 10:27 up_lpg/winlpg.exe
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Apr-17 10:33 up_lpg-0.0.6.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      336 b- defN 23-Apr-17 10:33 up_lpg-0.0.6.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Apr-17 10:33 up_lpg-0.0.6.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-17 10:33 up_lpg-0.0.6.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      619 b- defN 23-Apr-17 10:33 up_lpg-0.0.6.1.dist-info/RECORD
-8 files, 3903972 bytes uncompressed, 1189234 bytes compressed:  69.6%
+Zip file size: 1190324 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       36 b- defN 23-Apr-20 20:41 up_lpg/__init__.py
+-rw-rw-rw-  2.0 fat     9745 b- defN 23-Apr-20 20:41 up_lpg/lpg_planner.py
+-rw-rw-rw-  2.0 fat  3881596 b- defN 23-Apr-20 20:41 up_lpg/winlpg.exe
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Apr-20 20:50 up_lpg-0.0.6.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      336 b- defN 23-Apr-20 20:50 up_lpg-0.0.6.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Apr-20 20:50 up_lpg-0.0.6.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-20 20:50 up_lpg-0.0.6.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      619 b- defN 23-Apr-20 20:50 up_lpg-0.0.6.2.dist-info/RECORD
+8 files, 3904004 bytes uncompressed, 1189254 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: up_lpg/lpg_planner.py
 Comment: 
 
 Filename: up_lpg/winlpg.exe
 Comment: 
 
-Filename: up_lpg-0.0.6.1.dist-info/LICENSE
+Filename: up_lpg-0.0.6.2.dist-info/LICENSE
 Comment: 
 
-Filename: up_lpg-0.0.6.1.dist-info/METADATA
+Filename: up_lpg-0.0.6.2.dist-info/METADATA
 Comment: 
 
-Filename: up_lpg-0.0.6.1.dist-info/WHEEL
+Filename: up_lpg-0.0.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: up_lpg-0.0.6.1.dist-info/top_level.txt
+Filename: up_lpg-0.0.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: up_lpg-0.0.6.1.dist-info/RECORD
+Filename: up_lpg-0.0.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## up_lpg/lpg_planner.py

```diff
@@ -1,13 +1,14 @@
 import pkg_resources
 import re
 import os
 import sys
 import tempfile
 import unified_planning as up
+from fractions import Fraction
 from unified_planning.model import ProblemKind, AbstractProblem
 from unified_planning.plans import PlanKind, Plan
 from unified_planning.engines import PlanGenerationResult, PlanGenerationResultStatus
 from unified_planning.engines import PDDLPlanner, Credits, LogMessage, PlanGenerationResult
 from unified_planning.exceptions import UPException
 from unified_planning.engines.mixins import AnytimePlannerMixin
 from unified_planning.engines.mixins.plan_repairer import PlanRepairerMixin
@@ -20,30 +21,32 @@
                   '<license>',
                   'LPG is a planner based on local search and planning graphs.',
                   'LPG (Local search for Planning Graphs) is a planner based on local search and planning graphs.')
 
 lpg_os = {'win32':'winlpg.exe',
           'linux': 'lpg'}
 
+LPG_EPSILON = 0.00025
+
 class LPGEngine(PDDLPlanner):
 
     def __init__(self):
         super().__init__(needs_requirements=False)
         self._options = []
 
     @property
     def name(self) -> str:
         return 'lpg'
 
     def _get_cmd(self, domain_filename: str, problem_filename: str, plan_filename: str) -> List[str]:
         base_command = [pkg_resources.resource_filename(__name__, lpg_os[sys.platform]), '-o', domain_filename, '-f', problem_filename, '-n', '1', '-out', plan_filename]  + self._options
         return base_command
     
-    def  _get_engine_epsilon(self, new_epsilon:float):
-        self._options.extend(['-t', str(new_epsilon)])
+    def  _get_engine_epsilon(self) -> Optional[Fraction]:
+        return LPG_EPSILON
 
     def _plan_from_file(self, problem: 'up.model.Problem', plan_filename: str, get_item_named: Callable[[str],
             Union[
                 'up.model.Type',
                 'up.model.Action',
                 'up.model.Fluent',
                 'up.model.Object',
```

## Comparing `up_lpg-0.0.6.1.dist-info/LICENSE` & `up_lpg-0.0.6.2.dist-info/LICENSE`

 * *Files identical despite different names*

