# Comparing `tmp/slurmui-0.3.0.3-py3-none-any.whl.zip` & `tmp/slurmui-0.3.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6685 bytes, number of entries: 10
+Zip file size: 6711 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx       27 b- defN 23-Apr-20 15:06 slurmui/__init__.py
--rw-rw-r--  2.0 unx       23 b- defN 23-Apr-20 15:19 slurmui/_version.py
+-rw-rw-r--  2.0 unx       23 b- defN 23-Apr-21 08:46 slurmui/_version.py
 -rw-rw-r--  2.0 unx     9278 b- defN 23-Jan-13 19:20 slurmui/debug_strings.py
--rw-rw-r--  2.0 unx    11844 b- defN 23-Apr-20 15:18 slurmui/slurmui.py
+-rw-rw-r--  2.0 unx    11948 b- defN 23-Apr-21 08:46 slurmui/slurmui.py
 -rw-rw-r--  2.0 unx      269 b- defN 23-Jan-03 17:14 slurmui/slurmui_cli.py
--rw-rw-r--  2.0 unx      836 b- defN 23-Apr-20 15:19 slurmui-0.3.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 15:19 slurmui-0.3.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       60 b- defN 23-Apr-20 15:19 slurmui-0.3.0.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-20 15:19 slurmui-0.3.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      784 b- defN 23-Apr-20 15:19 slurmui-0.3.0.3.dist-info/RECORD
-10 files, 23221 bytes uncompressed, 5343 bytes compressed:  77.0%
+-rw-rw-r--  2.0 unx      836 b- defN 23-Apr-21 08:46 slurmui-0.3.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-21 08:46 slurmui-0.3.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       60 b- defN 23-Apr-21 08:46 slurmui-0.3.0.4.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-21 08:46 slurmui-0.3.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      784 b- defN 23-Apr-21 08:46 slurmui-0.3.0.4.dist-info/RECORD
+10 files, 23325 bytes uncompressed, 5369 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: slurmui/slurmui.py
 Comment: 
 
 Filename: slurmui/slurmui_cli.py
 Comment: 
 
-Filename: slurmui-0.3.0.3.dist-info/METADATA
+Filename: slurmui-0.3.0.4.dist-info/METADATA
 Comment: 
 
-Filename: slurmui-0.3.0.3.dist-info/WHEEL
+Filename: slurmui-0.3.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: slurmui-0.3.0.3.dist-info/entry_points.txt
+Filename: slurmui-0.3.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: slurmui-0.3.0.3.dist-info/top_level.txt
+Filename: slurmui-0.3.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: slurmui-0.3.0.3.dist-info/RECORD
+Filename: slurmui-0.3.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## slurmui/_version.py

```diff
@@ -1 +1 @@
-__version__ = "0.3.0.3"
+__version__ = "0.3.0.4"
```

## slurmui/slurmui.py

```diff
@@ -1,9 +1,10 @@
 import io
 from textual.app import App, ComposeResult
+from textual.binding import Binding
 from textual.widgets import DataTable
 from textual.widgets import Button, Header, Footer, Static, Label, TextLog, Input
 from textual.containers import Container, Vertical 
 from textual.containers import Grid
 from textual.screen import Screen
 import subprocess
 import pandas as pd
@@ -18,26 +19,26 @@
 DEBUG = False
 if DEBUG:
     from slurmui.debug_strings import SINFO_DEBUG, SQUEUE_DEBUG
 
 class SlurmUI(App):
 
     BINDINGS = [
-        ("d", "stage_delete", "Delete job"),
-        ("l", "display_log", "Log"),
-        ("g", "display_gpu", "GPU"),
-        ("r", "refresh", "Refresh"),
-        ("s", "sort", "Sort"),
-        ("q", "abort_quit", "Quit"),
-        ("enter", "confirm", "Confirm"),
-        ("escape", "abort_quit", "Abort"),  
+        Binding("d", "stage_delete", "Delete job"),
+        Binding("l", "display_log", "Log"),
+        Binding("g", "display_gpu", "GPU"),
+        Binding("r", "refresh", "Refresh"),
+        Binding("s", "sort", "Sort"),
+        Binding("q", "abort_quit", "Quit"),
+        Binding("enter", "confirm", "Confirm", priority=True),
+        Binding("escape", "abort_quit", "Abort"),
         # ("k", "scroll_up", "Up")    
 
     ]
-    STAGE = {"action": "monitor"} 
+    STAGE = {"action": "monitor"}
     gpu_overview_df = None
     sqeue_df =None
 
     def compose(self) -> ComposeResult:
         self.header = Header()
         self.footer = Footer()
         self.table = DataTable( id="table")
```

## Comparing `slurmui-0.3.0.3.dist-info/METADATA` & `slurmui-0.3.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmui
-Version: 0.3.0.3
+Version: 0.3.0.4
 Summary: Terminal UI for Slurm
 Home-page: https://github.com/SirWyver/slurmui
 Author: Norman Müller
 Author-email: norman.mueller@tum.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `slurmui-0.3.0.3.dist-info/RECORD` & `slurmui-0.3.0.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 slurmui/__init__.py,sha256=BVNOMLHFAyGklO8r4IWoXKL-miYRwTy0R3yaPTqINVg,27
-slurmui/_version.py,sha256=qzaip15ihZ-sz-Z7wOU7tMHu_weizIUxrpoHOAFOyic,23
+slurmui/_version.py,sha256=yeOUTyHryyXGB5l9CE2-VE5IDkyjd-dbuyoZ6gCs10k,23
 slurmui/debug_strings.py,sha256=oMimK75barJFA0SHZC6rp1YN7IE1qOA80FRpthPm3Kc,9278
-slurmui/slurmui.py,sha256=QjLiNVBdShRFHbWfA1QRyuLlF6yMSSs_tsAU6UdwIHg,11844
+slurmui/slurmui.py,sha256=nTEb01rW3NjfrQ0zXJCNhFxVZbfjG8X1AfLmJeZhiN0,11948
 slurmui/slurmui_cli.py,sha256=sw6Rm-prSO6v3ErtWfwN7T7KVh0MNvbAV2WZG1pEQfo,269
-slurmui-0.3.0.3.dist-info/METADATA,sha256=z3Ar8wOAeueIShzPeys3QOxPoB95MjTHpTXW5v0UXSg,836
-slurmui-0.3.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-slurmui-0.3.0.3.dist-info/entry_points.txt,sha256=jSENaCY2DRNuV8d3E5YOf4cYXWLB_DsBx74-lfl2_ow,60
-slurmui-0.3.0.3.dist-info/top_level.txt,sha256=a9nYoG_4X7NSFipwEd72kKiZ2PuL-z3COkZfeqkgmu4,8
-slurmui-0.3.0.3.dist-info/RECORD,,
+slurmui-0.3.0.4.dist-info/METADATA,sha256=eqEQfguaF7eH0WFWBBLQ8IYJdRiQpnydjThZ--3z3Bo,836
+slurmui-0.3.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+slurmui-0.3.0.4.dist-info/entry_points.txt,sha256=jSENaCY2DRNuV8d3E5YOf4cYXWLB_DsBx74-lfl2_ow,60
+slurmui-0.3.0.4.dist-info/top_level.txt,sha256=a9nYoG_4X7NSFipwEd72kKiZ2PuL-z3COkZfeqkgmu4,8
+slurmui-0.3.0.4.dist-info/RECORD,,
```

