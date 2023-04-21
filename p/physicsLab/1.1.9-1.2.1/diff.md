# Comparing `tmp/physicsLab-1.1.9.tar.gz` & `tmp/physicsLab-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\physicsLab-1.1.9.tar", last modified: Sat Apr  8 15:46:11 2023, max compression
+gzip compressed data, was "dist\physicsLab-1.2.1.tar", last modified: Fri Apr 21 15:10:13 2023, max compression
```

## Comparing `physicsLab-1.1.9.tar` & `physicsLab-1.2.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/
--rw-rw-rw-   0        0        0     1094 2023-04-05 15:16:06.000000 physicsLab-1.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0     4458 2023-04-08 15:46:11.000000 physicsLab-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     3898 2023-04-08 15:42:02.000000 physicsLab-1.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab/
--rw-rw-rw-   0        0        0      391 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/__init__.py
--rw-rw-rw-   0        0        0      453 2023-04-08 15:31:13.000000 physicsLab-1.1.9/physicsLab/_colorUtils.py
--rw-rw-rw-   0        0        0     3345 2023-04-08 15:31:13.000000 physicsLab-1.1.9/physicsLab/_fileGlobals.py
--rw-rw-rw-   0        0        0      534 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab/astrophysics/
--rw-rw-rw-   0        0        0        0 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/astrophysics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab/electricity/
--rw-rw-rw-   0        0        0      335 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/__init__.py
--rw-rw-rw-   0        0        0     4152 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/element.py
--rw-rw-rw-   0        0        0      478 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementPin.py
--rw-rw-rw-   0        0        0     2248 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementXYZ.py
-drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab/electricity/elementsClass/
--rw-rw-rw-   0        0        0      311 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementsClass/__init__.py
--rw-rw-rw-   0        0        0     4321 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementsClass/_elementClassHead.py
--rw-rw-rw-   0        0        0     9276 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementsClass/artificialCircuit.py
--rw-rw-rw-   0        0        0     8736 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementsClass/basicCircuit.py
--rw-rw-rw-   0        0        0    17238 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementsClass/logicCircuit.py
--rw-rw-rw-   0        0        0     4599 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/elementsClass/otherCircuit.py
--rw-rw-rw-   0        0        0     3039 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electricity/wire.py
-drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab/electromagnetism/
--rw-rw-rw-   0        0        0        0 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/electromagnetism/__init__.py
--rw-rw-rw-   0        0        0      319 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/errors.py
--rw-rw-rw-   0        0        0    11091 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/experiment.py
-drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab/unionElements/
--rw-rw-rw-   0        0        0      137 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/unionElements/__init__.py
--rw-rw-rw-   0        0        0     6894 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/unionElements/unionLogic.py
--rw-rw-rw-   0        0        0       54 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/unionElements/unionPin.py
--rw-rw-rw-   0        0        0     1259 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/unionElements/union_music.py
--rw-rw-rw-   0        0        0        0 2023-04-08 12:26:18.000000 physicsLab-1.1.9/physicsLab/userlog.py
-drwxrwxrwx   0        0        0        0 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab.egg-info/
--rw-rw-rw-   0        0        0     4458 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1073 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-08 15:46:11.000000 physicsLab-1.1.9/physicsLab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      581 2023-03-16 14:16:49.000000 physicsLab-1.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 15:46:11.000000 physicsLab-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-04-08 15:33:37.000000 physicsLab-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/
+-rw-rw-rw-   0        0        0     1094 2023-04-05 15:16:06.000000 physicsLab-1.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4440 2023-04-21 15:10:13.000000 physicsLab-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3880 2023-04-19 15:49:15.000000 physicsLab-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab/
+-rw-rw-rw-   0        0        0      391 2023-04-08 12:26:18.000000 physicsLab-1.2.1/physicsLab/__init__.py
+-rw-rw-rw-   0        0        0      966 2023-04-14 14:26:12.000000 physicsLab-1.2.1/physicsLab/_colorUtils.py
+-rw-rw-rw-   0        0        0     3384 2023-04-21 14:57:54.000000 physicsLab-1.2.1/physicsLab/_fileGlobals.py
+-rw-rw-rw-   0        0        0      715 2023-04-21 13:17:54.000000 physicsLab-1.2.1/physicsLab/_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab/astrophysics/
+-rw-rw-rw-   0        0        0       13 2023-04-21 15:04:35.000000 physicsLab-1.2.1/physicsLab/astrophysics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab/electricity/
+-rw-rw-rw-   0        0        0      335 2023-04-08 12:26:18.000000 physicsLab-1.2.1/physicsLab/electricity/__init__.py
+-rw-rw-rw-   0        0        0     4319 2023-04-21 14:37:03.000000 physicsLab-1.2.1/physicsLab/electricity/element.py
+-rw-rw-rw-   0        0        0      478 2023-04-08 12:26:18.000000 physicsLab-1.2.1/physicsLab/electricity/elementPin.py
+-rw-rw-rw-   0        0        0     2435 2023-04-21 14:03:16.000000 physicsLab-1.2.1/physicsLab/electricity/elementXYZ.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab/electricity/elementsClass/
+-rw-rw-rw-   0        0        0      342 2023-04-21 15:04:35.000000 physicsLab-1.2.1/physicsLab/electricity/elementsClass/__init__.py
+-rw-rw-rw-   0        0        0     4936 2023-04-21 14:31:05.000000 physicsLab-1.2.1/physicsLab/electricity/elementsClass/_elementClassHead.py
+-rw-rw-rw-   0        0        0     9181 2023-04-21 13:46:31.000000 physicsLab-1.2.1/physicsLab/electricity/elementsClass/artificialCircuit.py
+-rw-rw-rw-   0        0        0     8656 2023-04-21 12:38:58.000000 physicsLab-1.2.1/physicsLab/electricity/elementsClass/basicCircuit.py
+-rw-rw-rw-   0        0        0    17020 2023-04-21 13:47:04.000000 physicsLab-1.2.1/physicsLab/electricity/elementsClass/logicCircuit.py
+-rw-rw-rw-   0        0        0     4590 2023-04-21 12:38:59.000000 physicsLab-1.2.1/physicsLab/electricity/elementsClass/otherCircuit.py
+-rw-rw-rw-   0        0        0     3043 2023-04-21 14:31:05.000000 physicsLab-1.2.1/physicsLab/electricity/wire.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab/electromagnetism/
+-rw-rw-rw-   0        0        0       13 2023-04-21 15:04:35.000000 physicsLab-1.2.1/physicsLab/electromagnetism/__init__.py
+-rw-rw-rw-   0        0        0      319 2023-04-08 12:26:18.000000 physicsLab-1.2.1/physicsLab/errors.py
+-rw-rw-rw-   0        0        0    11450 2023-04-21 14:31:05.000000 physicsLab-1.2.1/physicsLab/experiment.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab/unionElements/
+-rw-rw-rw-   0        0        0      166 2023-04-21 15:04:35.000000 physicsLab-1.2.1/physicsLab/unionElements/__init__.py
+-rw-rw-rw-   0        0        0       13 2023-04-21 12:39:34.000000 physicsLab-1.2.1/physicsLab/unionElements/_unionClassHead.py
+-rw-rw-rw-   0        0        0     6835 2023-04-21 12:32:51.000000 physicsLab-1.2.1/physicsLab/unionElements/unionLogic.py
+-rw-rw-rw-   0        0        0       69 2023-04-21 12:39:18.000000 physicsLab-1.2.1/physicsLab/unionElements/unionPin.py
+-rw-rw-rw-   0        0        0     1369 2023-04-21 12:38:49.000000 physicsLab-1.2.1/physicsLab/unionElements/union_music.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 12:26:18.000000 physicsLab-1.2.1/physicsLab/userlog.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab.egg-info/
+-rw-rw-rw-   0        0        0     4440 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1117 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      581 2023-03-16 14:16:49.000000 physicsLab-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 15:10:13.000000 physicsLab-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1151 2023-04-21 15:10:05.000000 physicsLab-1.2.1/setup.py
```

### Comparing `physicsLab-1.1.9/LICENSE.txt` & `physicsLab-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.9/PKG-INFO` & `physicsLab-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsLab
-Version: 1.1.9
+Version: 1.2.1
 Summary: Doing experiments in the physics lab AR by python
 Home-page: https://gitee.com/script2000/physicsLab
 Author: Goodenough
 Author-email: 2381642961@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 1.  请确保你的电脑有[Python](https://www.python.org)与[物理实验室PC版](https://www.turtlesim.com/)（也可以联系[开发者Jone-Chen](https://gitee.com/civitasjohn)）
 2.  在cmd或shell输入：
 ```diff
 pip install physicsLab
 ```
 
 ## 开发环境
-python 3.7, PyCharm, win7  
+python 3.7.8, win7  
 目测对其他版本支持应该也很好
 3.6及以上应该没问题
 
 ## 使用说明
 
 ```Python
 from physicsLab import *
@@ -52,15 +52,15 @@
  # crt_wire输入格式：  
  #    crt_wire(SourcePin, TargetPin, color = "蓝")  
 crt_Wire(o.i_up, o.i_low)  
  # 将程序中生成的原件，导线等等写入存档  
 write_Experiment()  
  # 然后用物实打开存档见证奇迹  
 ```
-更详细的内容请查看[functions.md](physicsLab/functions.md)  
+更详细的内容请查看[functions.md](functions.md)  
 请注意：Python采用GBK编码，而物实用的是utf-8，尽管尽量确保编码格式正确，但中文仍有可能出现问题，因此建议多用英文。  
 
 ## 优点
 1. 通过read_Experiment()，你无须把所有工作交给代码。因为用代码写并不总是意味着方便（比如连接导线）。  
 你现在可以手动连接部分导线或者添加原件，并通过保存的形式，让程序在下次也可以轻松读取。  
 这也意味着你不用一口气把控制整个电路的脚本写出来，而是每次写一部分，并把更适合代码的工作交给代码完成。  
 也就是说，写这个脚本的感觉更像在控制台上操作，非常灵活。
```

### Comparing `physicsLab-1.1.9/README.md` & `physicsLab-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 1.  请确保你的电脑有[Python](https://www.python.org)与[物理实验室PC版](https://www.turtlesim.com/)（也可以联系[开发者Jone-Chen](https://gitee.com/civitasjohn)）
 2.  在cmd或shell输入：
 ```diff
 pip install physicsLab
 ```
 
 ## 开发环境
-python 3.7, PyCharm, win7  
+python 3.7.8, win7  
 目测对其他版本支持应该也很好
 3.6及以上应该没问题
 
 ## 使用说明
 
 ```Python
 from physicsLab import *
@@ -35,15 +35,15 @@
  # crt_wire输入格式：  
  #    crt_wire(SourcePin, TargetPin, color = "蓝")  
 crt_Wire(o.i_up, o.i_low)  
  # 将程序中生成的原件，导线等等写入存档  
 write_Experiment()  
  # 然后用物实打开存档见证奇迹  
 ```
-更详细的内容请查看[functions.md](physicsLab/functions.md)  
+更详细的内容请查看[functions.md](functions.md)  
 请注意：Python采用GBK编码，而物实用的是utf-8，尽管尽量确保编码格式正确，但中文仍有可能出现问题，因此建议多用英文。  
 
 ## 优点
 1. 通过read_Experiment()，你无须把所有工作交给代码。因为用代码写并不总是意味着方便（比如连接导线）。  
 你现在可以手动连接部分导线或者添加原件，并通过保存的形式，让程序在下次也可以轻松读取。  
 这也意味着你不用一口气把控制整个电路的脚本写出来，而是每次写一部分，并把更适合代码的工作交给代码完成。  
 也就是说，写这个脚本的感觉更像在控制台上操作，非常灵活。
```

### Comparing `physicsLab-1.1.9/physicsLab/_fileGlobals.py` & `physicsLab-1.2.1/physicsLab/_fileGlobals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+#coding=utf-8
 from getpass import getuser as _getuser
-from typing import Union
 
 FILE_HEAD = f'C:\\Users\\{_getuser()}\\AppData\\LocalLow\\CIVITAS\\Quantum Physics\\Circuit'
 # _xxx 不是文件向外暴露出的接口，文件外无法访问
-savName = ""  # sav的文件名
-StatusSave = {"SimulationSpeed": 1.0, "Elements": [], "Wires": []}
-Elements = []  # 装原件的_arguments
-Wires = []
-sav = {}
+savName: str = ""  # sav的文件名
+StatusSave: dict = {"SimulationSpeed": 1.0, "Elements": [], "Wires": []}
+Elements: list = []  # 装原件的_arguments
+Wires: list = []
+sav: dict = {}
+
+# 通过坐标索引元件
+elements_Position: dict = {}  # key: self._position，value: dict([self], ...)
+# 通过index（元件生成顺序）索引元件
+elements_Index: list = [] # List[self]
 
-elements_Address = {}  # key: self._position，value: self
-elements_Index = {}  # key: self.index, value: self
 
 def fileGlobals_init() -> None:
-    global sav, savName, StatusSave, Elements, Wires, elements_Index, elements_Address
+    global sav, savName, StatusSave, Elements, Wires, elements_Index, elements_Position
     savName = ""  # sav的文件名
     StatusSave = {"SimulationSpeed": 1.0, "Elements": [], "Wires": []}
     Elements = []  # 装原件的_arguments
     Wires = []
     sav = {
         "Type": 0,
         "Experiment": {
@@ -95,9 +98,9 @@
         "Bookmarks": {},
         "Interfaces": {
             "Play-Expanded": False,
             "Chart-Expanded": False
         }
     }
 
-    elements_Address = {}  # key: self._position，value: self
-    elements_Index = {}  # key: self.index, value: self
+    elements_Position = {}
+    elements_Index = []
```

### Comparing `physicsLab-1.1.9/physicsLab/_tools.py` & `physicsLab-1.2.1/physicsLab/_tools.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 #coding=utf-8
-from typing import Union
+import typing as _typing
+
+# type hint
+numType = _typing.Union[int, float]
 
 # 四舍五入physicsLab中的数据
-def roundData(num: Union[int, float]):
-    if isinstance(num, int):
-        return float(num)
-    return round(num, 4)
+# 支持传入多个数据
+def roundData(*num):
+    if not any(
+        isinstance(i, (int, float)) for i in num
+     ):
+        raise TypeError
+    
+    if len(num) == 1:
+        return round(num[0], 4)
+    return (round(i, 4) for i in num)
 
 # 生成随机字符串
 def randString(strLength: int) -> str:
     if not isinstance(strLength, int):
         raise TypeError
 
     from string import ascii_letters as _ascii_letters, digits as _digits
```

### Comparing `physicsLab-1.1.9/physicsLab/electricity/element.py` & `physicsLab-1.2.1/physicsLab/electricity/element.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 #coding=utf-8
-import physicsLab._tools as _tool
+import physicsLab._tools as _tools
 import physicsLab._fileGlobals as _fileGlobals
 from physicsLab.electricity.elementsClass import *
 import physicsLab.electricity.elementXYZ as _elementXYZ
 
 # 创建原件，本质上仍然是实例化
-def crt_Element(name: str, x : float = 0, y : float = 0, z : float = 0, elementXYZ = None):
-    if not (isinstance(name, str) and isinstance(x, (int, float)) and
-            isinstance(y, (int, float)) and isinstance(z, (int, float))
+def crt_Element(
+        name: str,
+        x: _tools.numType = 0,
+        y: _tools.numType = 0,
+        z: _tools.numType = 0,
+        elementXYZ: bool = None
+    ):
+    if not (isinstance(name, str)
+            and isinstance(x, (int, float))
+            and isinstance(y, (int, float))
+            and isinstance(z, (int, float))
     ):
         raise RuntimeError("Wrong parameter type")
+    name = name.strip()
     if name == '':
         raise RuntimeError('Name cannot be an empty string')
         # 元件坐标系
     if elementXYZ == True or (_elementXYZ.elementXYZ == True and elementXYZ is None):
         x, y, z = _elementXYZ.xyzTranslate(x, y, z)
-    x, y, z = _tool.roundData(x), _tool.roundData(y), _tool.roundData(z)
+    x, y, z = _tools.roundData(x, y, z)
     if (name == '555 Timer'):
         return NE555(x, y, z)
     elif (name == '8bit Input'):
         return eight_bit_Input(x, y, z)
     elif (name == '8bit Display'):
         return eight_bit_Display(x, y, z)
     else:
@@ -27,25 +36,26 @@
             return eval(name.replace(' ', '_').replace('-', '_') + f'({x},{y},{z})')
         except SyntaxError:
             raise RuntimeError(f"{name} original that does not exist")
 
 # 获取对应坐标的self
 def get_Element(*args, **kwargs):
     # 通过坐标索引元件
-    def position_Element(x: Union[int, float], y: Union[int, float], z: Union[int, float]):
+    def position_Element(x: _tools.numType, y: _tools.numType, z: _tools.numType):
         if not (isinstance(x, (int, float)) and isinstance(y, (int, float)) and isinstance(z, (int, float))):
-            raise RuntimeError('illegal argument')
-        x, y, z = _tool.roundData(x), _tool.roundData(y), _tool.roundData(z)
-        if (x, y, z) not in _fileGlobals.elements_Address.keys():
+            raise TypeError('illegal argument')
+        x, y, z = _tools.roundData(x), _tools.roundData(y), _tools.roundData(z)
+        if (x, y, z) not in _fileGlobals.elements_Position.keys():
             raise RuntimeError("Error coordinates that do not exist")
-        return _fileGlobals.elements_Address[(x, y, z)]
+        result: list = _fileGlobals.elements_Position[(x, y, z)]['self']
+        return result[0] if len(result) == 1 else result
     # 通过index（元件生成顺序）索引元件
     def index_Element(index: int):
         if 0 < index <= len(_fileGlobals.elements_Index):
-            return _fileGlobals.elements_Index[index]
+            return _fileGlobals.elements_Index[index - 1]
         else:
             raise RuntimeError
 
     # 如果输入参数为 x=, y=, z=
     if list(kwargs.keys()) == ['x', 'y', 'z']:
         return position_Element(kwargs['x'], kwargs['y'], kwargs['z'])
     # 如果输入参数为 index=
@@ -64,22 +74,22 @@
     else:
         raise TypeError
 
 # 删除原件
 def del_Element(self) -> None:
     try:
         identifier = self._arguments['Identifier']
-        if (self.father_type() == 'element'):
+        if self.father_type() == 'element':
             for element in _fileGlobals.Elements:
-                if (identifier == element['Identifier']):
+                if identifier == element['Identifier']:
                     # 删除原件
                     _fileGlobals.Elements.remove(element)
                     # 删除导线
                     i = 0
-                    while (i < _fileGlobals.Wires.__len__()):
+                    while i < _fileGlobals.Wires.__len__():
                         wire = _fileGlobals.Wires[i]
                         if (wire['Source'] == identifier or wire['Target'] == identifier):
                             _fileGlobals.Wires.pop(i)
                         else:
                             i += 1
                     return
     except:
@@ -94,8 +104,8 @@
     return len(_fileGlobals.Elements)
 
 # 清空原件
 def clear_Elements() -> None:
     _fileGlobals.Elements.clear()
     _fileGlobals.Wires.clear()
     _fileGlobals.elements_Index.clear()
-    _fileGlobals.elements_Address.clear()
+    _fileGlobals.elements_Position.clear()
```

### Comparing `physicsLab-1.1.9/physicsLab/electricity/elementsClass/_elementClassHead.py` & `physicsLab-1.2.1/physicsLab/electricity/elementsClass/_elementClassHead.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 # coding=utf-8
-import physicsLab._tools as _tool
-from typing import Callable, Union
+import physicsLab._tools as _tools
+from typing import Callable as _Callable
 import physicsLab._fileGlobals as _fileGlobals
 import physicsLab.electricity.elementPin as _elementPin
 import physicsLab.electricity.elementXYZ as _elementXYZ
 
+# 是否为big_Element
+is_big_Element: bool = False
 
 # 所有元件的父类
 class elementObject:
     # 设置原件的角度
-    def set_Rotation(self, xRotation: Union[int, float] = 0, yRotation: Union[int, float] = 0,
-                     zRotation: Union[int, float] = 180):
+    def set_Rotation(self, xRotation: _tools.numType = 0, yRotation: _tools.numType = 0,
+                     zRotation: _tools.numType = 180):
         if not (isinstance(xRotation, (int, float)) and isinstance(yRotation, (int, float)) and isinstance(zRotation, (
         int, float))):
             raise RuntimeError('illegal argument')
         self._arguments[
-            "Rotation"] = f"{_tool.roundData(xRotation)},{_tool.roundData(zRotation)},{_tool.roundData(yRotation)}"
+            "Rotation"] = f"{_tools.roundData(xRotation)},{_tools.roundData(zRotation)},{_tools.roundData(yRotation)}"
         return self
 
     # 重新设置元件的坐标
-    def set_Position(self, x: Union[int, float], y: Union[int, float], z: Union[int, float]):
+    def set_Position(self, x: _tools.numType, y: _tools.numType, z: _tools.numType):
         if not (isinstance(x, (int, float)) and isinstance(y, (int, float)) and isinstance(z, (int, float))):
             raise RuntimeError('illegal argument')
-        x, y, z = _tool.roundData(x), _tool.roundData(y), _tool.roundData(z)
-        del _fileGlobals.elements_Address[self._position]
+        x, y, z = _tools.roundData(x), _tools.roundData(y), _tools.roundData(z)
+        del _fileGlobals.elements_Position[self._position]
         self._position = (x, y, z)
         self._arguments['Position'] = f"{x},{z},{y}"
-        _fileGlobals.elements_Address[self._position] = self
+        _fileGlobals.elements_Position[self._position] = self
         return self
 
     # 格式化坐标参数，主要避免浮点误差
     def format_Position(self) -> tuple:
         if not isinstance(self._position, tuple) or self._position.__len__() != 3:
             raise RuntimeError("Position must be a tuple of length three but gets some other value")
-        self._position = (_tool.roundData(self._position[0]), _tool.roundData(self._position[1]),
-                          _tool.roundData(self._position[2]))
+        self._position = (_tools.roundData(self._position[0]), _tools.roundData(self._position[1]),
+                          _tools.roundData(self._position[2]))
         return self._position
 
     # 获取原件的坐标
     def get_Position(self) -> tuple:
         return self._position
 
     # 获取父类的类型
@@ -58,46 +60,62 @@
         print(self._arguments)
 
 
 # __init__ 装饰器
 _index = 1
 
 
-def element_Init_HEAD(func: Callable) -> Callable:
+def element_Init_HEAD(func: _Callable) -> _Callable:
     def result(
             self,
-            x: Union[int, float] = 0,
-            y: Union[int, float] = 0,
-            z: Union[int, float] = 0,
+            x: _tools.numType = 0,
+            y: _tools.numType = 0,
+            z: _tools.numType = 0,
             elementXYZ: bool = None
     ) -> None:
         if not (
                 isinstance(x, (float, int)) and
                 isinstance(y, (float, int)) and
                 isinstance(z, (float, int))
         ):
             raise TypeError('illegal argument')
-        x, y, z = _tool.roundData(x), _tool.roundData(y), _tool.roundData(z)
+        # 初始化全局变量
+        global is_big_Element
+        is_big_Element = False
+
+        x, y, z = _tools.roundData(x, y, z)
         self._position = (x, y, z)
         # 元件坐标系
         if elementXYZ == True or (_elementXYZ.elementXYZ == True and elementXYZ is None):
             x, y, z = _elementXYZ.xyzTranslate(x, y, z)
-        # 该坐标是否已存在
-        if self._position in _fileGlobals.elements_Address.keys():
-            raise RuntimeError("The position already exists")
         func(self, x, y, z)
-        self._arguments["Identifier"] = _tool.randString(32)
+        # 若是big_Element，则修正坐标
+        if is_big_Element:
+            x, y, z = _elementXYZ.amend_big_Element(x, y, z)
+
+        self._arguments["Identifier"] = _tools.randString(32)
+        # x, z, y 物实采用欧拉坐标系
         self._arguments["Position"] = f"{x},{z},{y}"
         _fileGlobals.Elements.append(self._arguments)
-        _fileGlobals.elements_Address[self._position] = self
+
+        # 该坐标是否已存在，则存入列表
+        if self._position in _fileGlobals.elements_Position.keys():
+            _fileGlobals.elements_Position[self._position]['self'].append(self)
+        else:
+            elementDict: dict = {
+                'self': [self],
+                'elementXYZ': _elementXYZ.elementXYZ,  # 是否为元件坐标系
+                'originPosition': tuple(_elementXYZ.get_OriginPosition())  # 坐标原点
+            }
+            _fileGlobals.elements_Position[self._position] = elementDict
         self.set_Rotation()
         # 通过元件生成顺序来索引元件
         global _index
         self._index = _index
-        _fileGlobals.elements_Index[self._index] = self
+        _fileGlobals.elements_Index.append(self)
         # 元件index索引加1
         _index += 1
     return result
 
 
 # 双引脚模拟电路原件的引脚
 def two_pin_ArtificialCircuit_Pin(cls):
```

### Comparing `physicsLab-1.1.9/physicsLab/electricity/elementsClass/artificialCircuit.py` & `physicsLab-1.2.1/physicsLab/electricity/elementsClass/basicCircuit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,205 +1,178 @@
 #coding=utf-8
-from typing import Union
-from ..elementXYZ import amend_big_Element
+import physicsLab._tools as _tools
 import physicsLab.electricity.elementPin as _elementPin
 import physicsLab.electricity.elementsClass._elementClassHead as _elementClassHead
 
+# 开关基类
 
-# 555定时器
-class NE555(_elementClassHead.elementObject):
+class _switch_Element(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
-        self._arguments = {'ModelID': '555 Timer', 'Identifier': '', 'IsBroken': False,
-                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '锁定': 1.0},
-                           'Statistics': {'供电': 10, '放电': 0.0, '阈值': 4,
-                                          '控制': 6.6666666666666666, '触发': 4,
-                                          '输出': 0, '重设': 10, '接地': 0},
-                           'Position': '', 'Rotation': '', 'DiagramCached': False,
-                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
-        x, y, z = amend_big_Element(x, y, z)
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+        self._arguments = {"ModelID": "", "Identifier": "", "IsBroken": False,
+                          "IsLocked": False, "Properties": {"开关": 0, "锁定": 1.0},
+                          "Statistics": {}, "Position": "",
+                          "Rotation": '', "DiagramCached": False,
+                          "DiagramPosition": {"X": 0, "Y": 0, "Z": 0, "Magnitude": 0}, "DiagramRotation": 0}
+
+# 简单开关
+@_elementClassHead.two_pin_ArtificialCircuit_Pin
+class Simple_Switch(_switch_Element):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+        super(Simple_Switch, self).__init__(x, y, z, elementXYZ)
+        self._arguments['ModelID'] = 'Simple Switch'
+
+# 单刀双掷开关
+class SPDT_Switch(_switch_Element):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+        super(SPDT_Switch, self).__init__(x, y, z, elementXYZ)
+        self._arguments['ModelID'] = 'SPDT Switch'
 
     @property
-    def VCC(self):
+    def l(self):
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def Dis(self):
+    def mid(self):
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def Thr(self):
+    def r(self):
         return _elementPin.element_Pin(self, 2)
 
+# 双刀双掷开关
+class DPDT_Switch(_switch_Element):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+        super(DPDT_Switch, self).__init__(x, y, z, elementXYZ)
+        self._arguments['ModelID'] = 'DPDT Switch'
+
     @property
-    def Ctrl(self):
+    def l_up(self):
         return _elementPin.element_Pin(self, 3)
 
     @property
-    def Trig(self):
+    def mid_up(self):
         return _elementPin.element_Pin(self, 4)
 
     @property
-    def Out(self):
+    def r_up(self):
         return _elementPin.element_Pin(self, 5)
 
     @property
-    def Reset(self):
-        return _elementPin.element_Pin(self, 6)
+    def l_low(self):
+        return _elementPin.element_Pin(self, 0)
 
     @property
-    def Ground(self):
-        return _elementPin.element_Pin(self, 7)
+    def mid_low(self):
+        return _elementPin.element_Pin(self, 1)
 
-# 电容
-@_elementClassHead.two_pin_ArtificialCircuit_Pin
-class Basic_Capacitor(_elementClassHead.elementObject):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'Basic Capacitor', 'Identifier': '',
-                           'IsBroken': False, 'IsLocked': False, 'Properties': {'耐压': 16.0, '电容': 1e-06, '内阻': 5.0, '锁定': 1.0},
-                           'Statistics': {}, 'Position': '',
-                           'Rotation': '', 'DiagramCached': False,
-                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
+    @property
+    def r_low(self):
+        return _elementPin.element_Pin(self, 2)
 
-# 接地
-class Ground_Component(_elementClassHead.elementObject):
+# 按钮开关
+@_elementClassHead.two_pin_ArtificialCircuit_Pin
+class Push_Switch(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'Ground Component', 'Identifier': '',
-                           'IsBroken': False, 'IsLocked': False, 'Properties': {'锁定': 1.0},
-                           'Statistics': {'电流': 0}, 'Position': '',
-                           'Rotation': '', 'DiagramCached': False,
-                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+        self._arguments = {
+            'ModelID': 'Push Switch', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
+            'Properties': {'开关': 0.0, '默认开关': 0.0, '锁定': 1.0}, 'Statistics': {'电流': 0.0}, 'Position': '',
+            'Rotation': '', 'DiagramCached': False, 'DiagramPosition': {
+                'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
-    @property
-    def i(self):
-        return _elementPin.element_Pin(self, 0)
 
-# 运算放大器
-class Operational_Amplifier(_elementClassHead.elementObject):
+# 一节电池
+@_elementClassHead.two_pin_ArtificialCircuit_Pin
+class Battery_Source(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'Operational Amplifier', 'Identifier': '',
-                           'IsBroken': False, 'IsLocked': False,
-                           'Properties': {'增益系数': 100_0000.0, '最大电压': 15.0, '最小电压': -15.0, '锁定': 1.0},
-                           'Statistics': {'电压-': 0, '电压+': 0, '输出电压': 0,
-                                          '输出电流': 0, '输出功率': 0},
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'Battery Source', 'Identifier': '',
+                           'IsBroken': False, 'IsLocked': False, 'Properties': {'最大功率': 16.2, '电压': 3.0, '内阻': 0.5},
+                           'Statistics': {'电流': 0, '功率': 0, '电压': 0},
                            'Position': '',
                            'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
-    @property
-    def i_up(self):
-        return _elementPin.element_Pin(self, 0)
-
-    @property
-    def i_low(self):
-        return _elementPin.element_Pin(self, 1)
-
-    @property
-    def o(self):
-        return _elementPin.element_Pin(self, 2)
-
-# 继电器
-class Relay_Component(_elementClassHead.elementObject):
+# 学生电源
+class Student_Source(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'Relay Component', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
-                           'Properties': {'开关': 0.0, '线圈电感': 0.2, '线圈电阻': 20.0,
-                                          '接通电流': 0.02, '额定电流': 1.0, '锁定': 1.0}, 'Statistics': {},
-                           'Position': '', 'Rotation': '',
-                           'DiagramCached': False, 'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0},
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'Student Source', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
+                           'Properties': {'交流电压': 3.0, '直流电压': 3.0, '开关': 0.0, '频率': 50.0},
+                           'Statistics': {'瞬间功率': 0.0, '瞬间电压': 0.0, '瞬间电流': 0.0,
+                                          '瞬间电阻': 0.0, '功率': 0.0, '电阻': 0.0, '电流': 0.0,
+                                          '瞬间功率1': 0.0, '瞬间电压1': 0.0, '瞬间电流1': 0.0,
+                                          '瞬间电阻1': 0.0,
+                                          '功率1': 0.0, '电阻1': 0.0, '电流1': 0.0},
+                           'Position': '',
+                           'Rotation': '', 'DiagramCached': False,
+                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0},
                            'DiagramRotation': 0}
 
     @property
-    def l_up(self):
+    def l(self):
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def l_low(self):
-        return _elementPin.element_Pin(self, 2)
-
-    @property
-    def mid(self):
+    def l_mid(self):
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def r_up(self):
-        return _elementPin.element_Pin(self, 4)
+    def r_mid(self):
+        return _elementPin.element_Pin(self, 2)
 
     @property
-    def r_low(self):
-        return _elementPin.element_Pin(self, 5)
+    def r(self):
+        return _elementPin.element_Pin(self, 3)
 
-# n mos
-class N_MOSFET(_elementClassHead.elementObject):
+# 电阻
+@_elementClassHead.two_pin_ArtificialCircuit_Pin
+class Resistor(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'N-MOSFET', 'Identifier': '', 'IsBroken': False,
-                           'IsLocked': False, 'Properties': {'PNP': 1.0, '放大系数': 0.027, '阈值电压': 1.5, '最大功率': 100.0, '锁定': 1.0},
-                           'Statistics': {'电压GS': 0.0, '电压': 0.0, '电流': 0.0, '功率': 0.0, '状态': 0.0},
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'Resistor', 'Identifier': '', 'IsBroken': False,
+                           'IsLocked': False,
+                           'Properties': {'最大电阻': 1000_0000.0, '最小电阻': 0.1, '电阻': 10, '锁定': 1.0},
+                           'Statistics': {'瞬间功率': 0, '瞬间电流': 0,
+                                          '瞬间电压': 0, '功率': 0,
+                                          '电压': 0, '电流': 0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
-    @property
-    def D(self):
-        return _elementPin.element_Pin(self, 2)
-
-    @property
-    def S(self):
-        return _elementPin.element_Pin(self, 1)
-
-    @property
-    def G(self):
-        return _elementPin.element_Pin(self, 0)
+# 保险丝
+@_elementClassHead.two_pin_ArtificialCircuit_Pin
+class Fuse_Component(_elementClassHead.elementObject):
+    @_elementClassHead.element_Init_HEAD
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'Fuse Component', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
+                           'Properties': {'开关': 1.0, '额定电流': 0.30000001192092896, '熔断电流': 0.5, '锁定': 1.0},
+                           'Statistics': {'瞬间功率': 0.0, '瞬间电流': 0.0, '瞬间电压': 0.0, '功率': 0.0, '电压': 0.0, '电流': 0.0},
+                           'Position': '', 'Rotation': '', 'DiagramCached': False,
+                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
-# 波形发生器基类
-class _source_element(_elementClassHead.elementObject):
+# 滑动变阻器
+class Slide_Rheostat(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
-        self._arguments = {'ModelID': '', 'Identifier': '',
-                           'IsBroken': False, 'IsLocked': False,
-                           'Properties': {'电压': 3.0, '内阻': 0.5, '频率': 20000.0, '偏移': 0.0, '占空比': 0.5, '锁定': 1.0},
-                           'Statistics': {'电流': 0.0, '功率': 0.0, '电压': -3.0},
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'Slide Rheostat', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
+                           'Properties': {'额定电阻': 10.0, '滑块位置': 0.0, '电阻1': 10, '电阻2': 10.0, '锁定': 1.0},
+                           'Statistics': {'瞬间功率': 0.0, '瞬间电流': 0.0, '瞬间电压': 0.0, '功率': 0.0, '电压': 0.0, '电流': 0.0,
+                                          '瞬间功率1': 0.0, '瞬间电流1': 0.0, '瞬间电压1': 0.0, '功率1': 0.0, '电压1': 0.0, '电流1': 0.0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def l(self):
+    def l_low(self):
         return _elementPin.element_Pin(self, 0)
-    i = l
 
     @property
-    def r(self):
+    def r_low(self):
         return _elementPin.element_Pin(self, 1)
-    o = r
 
-# 正弦波发生器
-class Sinewave_Source(_source_element):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
-        super(Sinewave_Source, self).__init__(x, y, z, elementXYZ)
-        self._arguments['ModelID'] = 'Sinewave Source'
-
-# 方波发生器
-class Square_Source(_source_element):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
-        super(Square_Source, self).__init__(x, y, z, elementXYZ)
-        self._arguments['ModelID'] = 'Square Source'
-
-# 三角波发生器
-class Triangle_Source(_source_element):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
-        super(Triangle_Source, self).__init__(x, y, z, elementXYZ)
-        self._arguments['ModelID'] = 'Triangle Source'
-
-# 锯齿波发生器
-class Sawtooth_Source(_source_element):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
-        super(Sawtooth_Source, self).__init__(x, y, z, elementXYZ)
-        self._arguments['ModelID'] = 'Sawtooth Source'
-
-# 尖峰波发生器
-class Pulse_Source(_source_element):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
-        super(Pulse_Source, self).__init__(x, y, z, elementXYZ)
-        self._arguments['ModelID'] = 'Pulse Source'
+    @property
+    def l_up(self):
+        return _elementPin.element_Pin(self, 2)
+
+    @property
+    def r_up(self):
+        return _elementPin.element_Pin(self, 3)
```

### Comparing `physicsLab-1.1.9/physicsLab/electricity/elementsClass/logicCircuit.py` & `physicsLab-1.2.1/physicsLab/electricity/elementsClass/logicCircuit.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 #coding=utf-8
-from typing import Union
+import physicsLab._tools as _tools
 from ..elementXYZ import amend_big_Element
 import physicsLab.electricity.elementPin as _elementPin
 import physicsLab.electricity.elementsClass._elementClassHead as _elementClassHead
 
 # 逻辑电路类装饰器
 def logic_Circuit_Method(cls):
     # 设置高电平的值
-    def set_HighLeaveValue(self, num: Union[int, float]) -> None:
+    def set_HighLeaveValue(self, num: _tools.numType) -> None:
         if not isinstance(num, (int, float)):
             raise RuntimeError('illegal argument')
         self._arguments['Properties']['高电平'] = num
     cls.set_HighLeaveValue = set_HighLeaveValue
 
     # 设置低电平的值
-    def set_LowLeaveValue(self, num : Union[int, float]) -> None:
+    def set_LowLeaveValue(self, num : _tools.numType) -> None:
         if not isinstance(num, (int, float)):
             raise RuntimeError('illegal argument')
         self._arguments['Properties']['低电平'] = num
     cls.set_LowLeaveValue = set_LowLeaveValue
 
     return cls
 
 # _arguments是参数的意思
 
 # 逻辑输入
 @logic_Circuit_Method
 class Logic_Input(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {"ModelID": "Logic Input", "Identifier": "",
                           "IsBroken": False, "IsLocked": False, "Properties": {"高电平": 3.0, "低电平": 0.0, "锁定": 1.0, "开关": 0},
                           "Statistics": {"电流": 0.0, "电压": 0.0, "功率": 0.0},
                           "Position": "",
                           "Rotation": "", "DiagramCached": False,
                           "DiagramPosition": {"X": 0, "Y": 0, "Magnitude": 0.0},
                           "DiagramRotation": 0}
@@ -44,15 +44,15 @@
     def o(self):
         return _elementPin.element_Pin(self, 0)
 
 # 逻辑输出
 @logic_Circuit_Method
 class Logic_Output(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Logic Output', 'Identifier': "",
                           'IsBroken': False, 'IsLocked': False,
                           'Properties': {'状态': 0.0, '高电平': 3.0, '低电平': 0.0, '锁定': 1.0}, 'Statistics': {},
                           'Position': "",
                           'Rotation': '0,180,0', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
@@ -60,15 +60,15 @@
     def i(self):
             return _elementPin.element_Pin(self, 0)
 
 # 2引脚门电路
 @logic_Circuit_Method
 class _2_pin_Gate(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '', 'Identifier': "", 'IsBroken': False,
                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '最大电流': 0.1, '锁定': 1.0},
                           'Statistics': {}, 'Position': "", 'Rotation': '', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
     def i(self):
@@ -76,29 +76,29 @@
 
     @property
     def o(self):
         return _elementPin.element_Pin(self, 1)
 
 # 是门
 class Yes_Gate(_2_pin_Gate):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Yes_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Yes Gate'
 
 # 非门
 class No_Gate(_2_pin_Gate):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(No_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'No Gate'
 
 # 3引脚门电路
 @logic_Circuit_Method
 class _3_pin_Gate(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '', 'Identifier': '', 'IsBroken': False,
                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '最大电流': 0.1, '锁定': 1.0},
                           'Statistics': {}, 'Position': "", 'Rotation': "", 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
     def i_up(self):
@@ -110,74 +110,74 @@
 
     @property
     def o(self):
         return _elementPin.element_Pin(self, 2)
 
 # 或门
 class Or_Gate(_3_pin_Gate):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Or_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Or Gate'
 
 # 与门
 class And_Gate(_3_pin_Gate):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(And_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'And Gate'
 
 # 或非门
 class Nor_Gate(_3_pin_Gate):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Nor_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Nor Gate'
 
 # 与非门
 class Nand_Gate(_3_pin_Gate):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Nand_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Nand Gate'
 
 # 异或门
 class Xor_Gate(_3_pin_Gate):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Xor_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Xor Gate'
 
 # 同或门
 class Xnor_Gate(_3_pin_Gate):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Xnor_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Xnor Gate'
 
 # 蕴含门
 class Imp_Gate(_3_pin_Gate):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Imp_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Imp Gate'
 
 # 蕴含非门
 class Nimp_Gate(_3_pin_Gate):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Nimp_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Nimp Gate'
 
 # 2体积元件父类
 @logic_Circuit_Method
 class _big_element(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '', 'Identifier': '', 'IsBroken': False,
                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '锁定': 1.0}, 'Statistics': {},
                           'Position': '', 'Rotation': '', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
-        x, y, z = amend_big_Element(x, y, z)
+        _elementClassHead.is_big_Element = True
 
 # 半加器
 class Half_Adder(_big_element):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Half_Adder, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Half Adder'
 
     @property
     def i_up(self):
         return _elementPin.element_Pin(self, 2)
 
@@ -191,15 +191,15 @@
 
     @property
     def o_low(self):
         return _elementPin.element_Pin(self, 1)
 
 # 全加器
 class Full_Adder(_big_element):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Full_Adder, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Full Adder'
 
     @property
     def i_up(self):
         return _elementPin.element_Pin(self, 2)
 
@@ -217,15 +217,15 @@
 
     @property
     def o_low(self):
         return _elementPin.element_Pin(self, 1)
 
 # 二位乘法器
 class Multiplier(_big_element):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Multiplier, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Multiplier'
 
     @property
     def i_up(self):
         return _elementPin.element_Pin(self, 4)
 
@@ -255,15 +255,15 @@
 
     @property
     def o_low(self):
         return _elementPin.element_Pin(self, 3)
 
 # D触发器
 class D_Flipflop(_big_element):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(D_Flipflop, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'D Flipflop'
 
     @property
     def i_up(self):
         return _elementPin.element_Pin(self, 2)
 
@@ -277,15 +277,15 @@
 
     @property
     def o_low(self):
         return _elementPin.element_Pin(self, 1)
 
 # T触发器
 class T_Flipflop(_big_element):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(T_Flipflop, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'T Flipflop'
 
     @property
     def i_up(self):
         return _elementPin.element_Pin(self, 2)
 
@@ -299,15 +299,15 @@
 
     @property
     def o_low(self):
         return _elementPin.element_Pin(self, 1)
 
 # JK触发器
 class JK_Flipflop(_big_element):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(JK_Flipflop, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'JK Flipflop'
 
     @property
     def i_up(self):
         return _elementPin.element_Pin(self, 2)
 
@@ -325,15 +325,15 @@
 
     @property
     def o_low(self):
         return _elementPin.element_Pin(self, 1)
 
 # 计数器
 class Counter(_big_element):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Counter, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Counter'
 
     @property
     def i_up(self):
         return _elementPin.element_Pin(self, 4)
 
@@ -355,15 +355,15 @@
 
     @property
     def o_low(self):
         return _elementPin.element_Pin(self, 3)
 
 # 随机数发生器
 class Random_Generator(_big_element):
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Random_Generator, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Random Generator'
 
     @property
     def i_up(self):
         return _elementPin.element_Pin(self, 4)
 
@@ -387,15 +387,15 @@
     def o_low(self):
         return _elementPin.element_Pin(self, 3)
 
 # 8位输入器
 @logic_Circuit_Method
 class eight_bit_Input(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '8bit Input', 'Identifier': '', 'IsBroken': False,
                            'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '十进制': 0.0, '锁定': 1.0},
                            'Statistics': {}, 'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     def set_num(self, num : int):
         if 0 <= num <= 255:
@@ -435,15 +435,15 @@
     def o_low(self):
         return _elementPin.element_Pin(self, 7)
 
 # 8位显示器
 @logic_Circuit_Method
 class eight_bit_Display(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '8bit Display', 'Identifier': '',
                           'IsBroken': False, 'IsLocked': False,
                           'Properties': {'高电平': 3.0, '低电平': 0.0, '状态': 0.0, '锁定': 1.0},
                           'Statistics': {'7': 0.0, '6': 0.0, '5': 0.0, '4': 0.0, '3': 0.0, '2': 0.0, '1': 0.0, '0': 0.0,
                                          '十进制': 0.0}, 'Position': '',
                           'Rotation': '', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
```

### Comparing `physicsLab-1.1.9/physicsLab/electricity/elementsClass/otherCircuit.py` & `physicsLab-1.2.1/physicsLab/electricity/elementsClass/otherCircuit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #coding=utf-8
-from typing import Union
+import physicsLab._tools as _tools
 from string import digits as _digits
 import physicsLab.electricity.elementPin as _elementPin
 import physicsLab.electricity.elementsClass._elementClassHead as _elementClassHead
 
 # 小电扇
 @_elementClassHead.two_pin_ArtificialCircuit_Pin
 class Electric_Fan(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Electric Fan', 'Identifier': '',
                            'IsBroken': False, 'IsLocked': False,
                            'Properties': {'额定电阻': 1.0, '马达常数': 0.1, '转动惯量': 0.01, '电感': 5e-05, '负荷扭矩': 0.01,
                                           '反电动势系数': 0.001, '粘性摩擦系数': 0.01, '角速度': 0, '锁定': 1.0},
                            'Statistics': {'瞬间功率': 0, '瞬间电流': 0, '瞬间电压': 0, '功率': 0,
                                           '电压': 0, '电流': 0, '摩擦扭矩': 0, '角速度': 0,
                                           '反电动势': 0, '转速': 0, '输入功率': 0, '输出功率': 0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
 # 简单乐器（更多功能的源代码在union_music）
 class Simple_Instrument(_elementClassHead.elementObject):
     @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, elementXYZ = None):
+    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Simple Instrument', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
                            'Properties': {'额定电压': 3.0, '额定功率': 0.3, '音量': 1.0, '音高': 60.0, '节拍': 70.0, '锁定': 1.0,
                                           '乐器': 1.0},
                            'Statistics': {'瞬间功率': 0, '瞬间电流': 0, '瞬间电压': 0, '功率': 0, '电压': 0, '电流': 0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
@@ -49,15 +49,15 @@
             ... 
             7 -> xi
         低1个八度： '.1', '.1#', '.2' ...
         低2个八度： '..1', '..1#', '..2' ...
         升1个八度： '1.', '1#.', '2' ...
         以此类推即可
     '''
-    def set_Tonality(self, tonality: Union[int, str]) -> None:
+    def set_Tonality(self, tonality: _tools.numType) -> None:
         if isinstance(tonality, int):
             if 0 < tonality < 8:
                 raise RuntimeError('Input data error')
             tonality = str(tonality)
         elif isinstance(tonality, str):
             tonality.strip()
             for char in tonality:
```

### Comparing `physicsLab-1.1.9/physicsLab/electricity/wire.py` & `physicsLab-1.2.1/physicsLab/electricity/wire.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import physicsLab._fileGlobals as _fileGlobals
 import physicsLab.electricity.elementPin as _elementPin
 
 # 老版本连接导线函数，不推荐使用
 def old_crt_wire(SourceLabel, SourcePin : int, TargetLabel, TargetPin : int, color = "蓝") -> None: # SourceLabel : Union[_element, tuple]
     SourcePin, TargetPin = int(SourcePin), int(TargetPin)
     if (isinstance(SourceLabel, tuple) and len(SourceLabel) == 3):
-        SourceLabel = _fileGlobals.elements_Address[SourceLabel]
-    elif (SourceLabel not in _fileGlobals.elements_Address.values()):
+        SourceLabel = _fileGlobals.elements_Position[SourceLabel]
+    elif (SourceLabel not in _fileGlobals.elements_Position.values()):
         raise RuntimeError("SourceLabel must be a Positon or self")
     if (isinstance(TargetLabel, tuple) and len(TargetLabel) == 3):
-        TargetLabel = _fileGlobals.elements_Address[TargetLabel]
-    elif (TargetLabel not in _fileGlobals.elements_Address.values()):
+        TargetLabel = _fileGlobals.elements_Position[TargetLabel]
+    elif (TargetLabel not in _fileGlobals.elements_Position.values()):
         raise RuntimeError("TargetLabel must be a Positon or self")
 
     if (color not in ["黑", "蓝", "红", "绿", "黄"]):
         raise RuntimeError("illegal color")
     _fileGlobals.Wires.append({"Source": SourceLabel._arguments["Identifier"], "SourcePin": SourcePin,
                    "Target": TargetLabel._arguments["Identifier"], "TargetPin": TargetPin,
                    "ColorName": f"{color}色导线"})
```

### Comparing `physicsLab-1.1.9/physicsLab/experiment.py` & `physicsLab-1.2.1/physicsLab/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,69 +1,92 @@
 #coding=utf-8
 import os as _os
 import sys as _sys
 import json as _json
 
-import physicsLab._tools as _tool
+import physicsLab._tools as _tools
 import physicsLab.errors as errors
 import physicsLab._colorUtils as _colorUtils
 import physicsLab._fileGlobals as _fileGlobals
 from physicsLab.electricity.element import crt_Element
 
 ### define ###
 
-# 是否已经有存档被打开或创建
-_ifndef_open_Experiment = False
-
 def print_Elements():
     print(_fileGlobals.Elements)
 
 def print_wires():
     print(_fileGlobals.Wires)
 
 def print_elements_Address():
-    print(_fileGlobals.elements_Address)
+    print(_fileGlobals.elements_Position)
 
 ### end define ###
 
+# 实验（存档）类，主要与'with'关键字搭配使用
+class experiment:
+    def __init__(
+            self,
+            file: str,
+            read: bool = False # 是否读取存档原有状态
+    ) -> None:
+        if not (
+            isinstance(file, str)
+            and isinstance(read, bool)
+        ):
+            raise TypeError
+
+        self.file = file
+        self.read = read
+
+    # 上下文管理器，搭配with使用
+    def __enter__(self):
+        try:
+            open_Experiment(self.file)
+        except errors.openExperimentError: # 如果存档不存在
+            crt_Experiment(self.file)
+        if self.read:
+            read_Experiment()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        write_Experiment()
+
 # 输入sav文件名并读取（旧函数，不建议使用）
 def old_open_Experiment(file: str) -> None:
     file = file.strip()
     if (not file.endswith('.sav')):
         raise RuntimeError("The input parameters are incorrect")
 
-    global _ifndef_open_Experiment
-    if (_ifndef_open_Experiment):
-        raise RuntimeError("This function can only be run once")
-    _ifndef_open_Experiment = True
-
     _fileGlobals.savName = f"{_fileGlobals.FILE_HEAD}\\{file}"
     with open(_fileGlobals.savName, encoding="UTF-8") as f:
-        InternalName = (_json.loads(f.read().replace('\n', '')))["Summary"]["Subject"]
-        _fileGlobals.sav["Summary"]["Subject"] = InternalName
-        _fileGlobals.sav["InternalName"] = _fileGlobals.sav["Summary"]["Subject"]
+        InternalName = (_json.loads(f.read().replace('\n', '')))["InternalName"]
+        _fileGlobals.sav["InternalName"] = InternalName
+        try: # 当Summary为None时触发TypeError
+            _fileGlobals.sav["Summary"]["Subject"] = InternalName
+        except TypeError:
+            pass
 
 # 将import了physicsLab的文件的第一行添加上 #coding=utf-8
 def _utf8_coding(func):
-    def result(string: str) -> None:
+    def result(*args, **kwargs) -> None:
         try: # 在cmd或者shell上无法执行该功能
             import sys
             s = ''
             with open(sys.argv[0], encoding='utf-8') as f:
                 s = f.read()
             if not s.replace('\n', '').startswith('#coding=utf-8'):
                 with open(sys.argv[0], 'w', encoding='utf-8') as f:
                     if s.startswith('\n'):
                         f.write(f'#coding=utf-8{s}')
                     else:
                         f.write(f'#coding=utf-8\n{s}')
         except FileNotFoundError:
             # 在cmd或IDLE上运行时会关闭打印彩字功能
             _colorUtils.printColor = False
-        func(string)
+        func(*args, **kwargs)
     return result
 
 # 打开一个指定的sav文件（支持输入本地实验的名字或sav文件名）
 @_utf8_coding
 def open_Experiment(file : str) -> None:
     _fileGlobals.fileGlobals_init()
     file = file.strip()
@@ -85,19 +108,14 @@
                         return
         raise errors.openExperimentError(f'No such experiment "{file}"')
 
 # 创建存档
 @_utf8_coding
 def crt_Experiment(name : str) -> None:
     _fileGlobals.fileGlobals_init()
-    global _ifndef_open_Experiment
-    # 该函数与open_Experiment一起，每次只能运行一次
-    if (_ifndef_open_Experiment):
-        raise RuntimeError("This function can only be run once")
-    _ifndef_open_Experiment = True
     # 检查是否存在重名的存档
     savs = [i for i in _os.walk(_fileGlobals.FILE_HEAD)][0]
     savs = savs[savs.__len__() - 1]
     savs = [aSav for aSav in savs if aSav.endswith('sav')]
     for aSav in savs:
         with open(f"{_fileGlobals.FILE_HEAD}\\{aSav}", encoding='utf-8') as f:
             try:
@@ -106,15 +124,15 @@
                 pass
             else:
                 if f['InternalName'] == name:
                     raise RuntimeError('Duplicate name archives are forbidden')
     # 创建存档
     if not isinstance(name, str):
         name = str(name)
-    _fileGlobals.savName = _tool.randString(34)
+    _fileGlobals.savName = _tools.randString(34)
     _fileGlobals.savName = f'{_fileGlobals.FILE_HEAD}\\{_fileGlobals.savName}.sav'
     with open(_fileGlobals.savName, 'w', encoding='utf-8'):
         pass
     rename_Experiment(name)
 
 # 将编译完成的json写入sav
 def write_Experiment() -> None:
@@ -164,27 +182,26 @@
 # 读取sav文件已有的原件与导线
 def read_Experiment() -> None:
     with open(_fileGlobals.savName, encoding='UTF-8') as f:
         readmem = _json.loads(f.read().replace('\n', ''))
         # 元件
         _local_Elements = _json.loads(readmem["Experiment"]["StatusSave"])["Elements"]
         # 导线
-        for aWire in _json.loads(readmem['Experiment']['StatusSave'])['Wires']:
-            _fileGlobals.Wires.append(aWire)
+        _fileGlobals.Wires = _json.loads(readmem['Experiment']['StatusSave'])['Wires']
 
         for element in _local_Elements:
             # 坐标标准化（消除浮点误差）
             sign1 = element['Position'].find(',')
             sign2 = element['Position'].find(',', sign1 + 1)
-            num1 = _tool.roundData(float(element['Position'][:sign1:]))
-            num2 = _tool.roundData(float(element['Position'][sign1 + 1: sign2:]))
-            num3 = _tool.roundData(float(element['Position'][sign2 + 1::]))
+            num1 = _tools.roundData(float(element['Position'][:sign1:]))
+            num2 = _tools.roundData(float(element['Position'][sign1 + 1: sign2:]))
+            num3 = _tools.roundData(float(element['Position'][sign2 + 1::]))
             element['Position'] = f"{num1},{num2},{num3}"  # x, z, y
             # 实例化对象
-            obj = crt_Element(element["ModelID"], num1, num3, num2)
+            obj = crt_Element(element["ModelID"], num1, num3, num2, elementXYZ=False)
             sign1 = element['Rotation'].find(',')
             sign2 = element['Rotation'].find(',', sign1 + 1)
             x = float(element['Rotation'][:sign1:])
             z = float(element['Rotation'][sign1 + 1: sign2:])
             y = float(element['Rotation'][sign2 + 1::])
             obj.set_Rotation(x, y, z)
             obj._arguments['Identifier'] = element['Identifier']
```

### Comparing `physicsLab-1.1.9/physicsLab/unionElements/unionLogic.py` & `physicsLab-1.2.1/physicsLab/unionElements/unionLogic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 #coding=utf-8
 # 模块化电路
-from typing import Union
-import physicsLab._tools as _tool
+import physicsLab._tools as _tools
 import physicsLab.electricity as eletricity
 
 # 任意引脚加法电路
 class union_Sum:
-    def __init__(self, x : Union[int, Union[int, float]] = 0, y : Union[int, float] = 0, z : Union[int, float] = 0, bitCount : int = 1):
+    def __init__(self, x : _tools.numType = 0, y : _tools.numType = 0, z : _tools.numType = 0, bitCount : int = 1):
         if not (
                 isinstance(x, (float, int)) and isinstance(y, (float, int)) and
                 isinstance(z, (float, int)) and isinstance(bitCount, int) and bitCount > 0
         ):
             raise RuntimeError('Error in input parameters')
-        x, y, z = _tool.roundData(x), _tool.roundData(y), _tool.roundData(z)
+        x, y, z = _tools.roundData(x), _tools.roundData(y), _tools.roundData(z)
         eletricity.Full_Adder(x, y, z)
         for count in range(1, bitCount):
             if count % 8 != 0:
-                y = _tool.roundData(y + 0.2)
+                y = _tools.roundData(y + 0.2)
                 eletricity.crt_Wire(
                     eletricity.Full_Adder(x, y, z).i_low,
                     eletricity.get_Element(x, y - 0.2, z).o_low
                 )
             else:
                 y -= 1.4
-                z = _tool.roundData(z + 0.1)
+                z = _tools.roundData(z + 0.1)
                 eletricity.crt_Wire(
                     eletricity.Full_Adder(x, y, z).i_low,
                     eletricity.get_Element(x, y + 1.4, z - 0.1).o_low
                 )
 
 # 任意引脚减法电路
 class union_Sub:
     pass
 
 # 2-4译码器
 class union_2_4_Decoder:
-    def __init__(self, x : Union[int, float] = 0, y : Union[int, float] = 0, z : Union[int, float] = 0):
+    def __init__(self, x : _tools.numType = 0, y : _tools.numType = 0, z : _tools.numType = 0):
         if not (isinstance(x, (int, float)) and isinstance(y, (int, float)) and isinstance(z, (int, float))):
             raise RuntimeError('illegal argument')
         self.x = x
         self.y = y
         self.z = z
         obj1 = eletricity.Nor_Gate(x, y, z)
         obj2 = eletricity.Nimp_Gate(x, y + 0.1, z)
@@ -54,15 +53,15 @@
 
     @property
     def i_low(self):
         return eletricity.element_Pin(eletricity.get_Element(self.x, self.y + 0.3, self.z), 1)
 
 # 4-16译码器
 class union_4_16_Decoder:
-    def __init__(self, x : Union[int, float] = 0, y : Union[int, float] = 0, z : Union[int, float] = 0):
+    def __init__(self, x : _tools.numType = 0, y : _tools.numType = 0, z : _tools.numType = 0):
         if not (isinstance(x, (int, float)) and isinstance(y, (int, float)) and isinstance(z, (int, float))):
             raise RuntimeError('illegal argument')
         self.x = x
         self.y = y
         self.z = z
         obj1 = eletricity.Nor_Gate(x, y, z); obj2 = eletricity.Nimp_Gate(x, y + 0.1, z)
         obj3 = eletricity.Nimp_Gate(x, y + 0.2, z); obj4 = eletricity.And_Gate(x, y + 0.3, z)
```

### Comparing `physicsLab-1.1.9/physicsLab/unionElements/union_music.py` & `physicsLab-1.2.1/physicsLab/unionElements/union_music.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #coding=utf-8
-import physicsLab.electricity as eletricity
-from typing import Union
 import math as _math
+from typing import Union as _Union
+import physicsLab._tools as _tools
+import physicsLab.electricity as eletricity
 '''
 How do you play music in physics Lab AR?
 Music extension might make it easier than before!
 
     How to use it?
 >>> music(a_list_or_a_tuple)
 >>> write_Experiment()
@@ -21,13 +22,19 @@
 输入格式：
 [
     [一些音符，每次会同时演奏这些音符],
     [一些音符，每次会同时演奏这些音符]
 ] # 元组也可以
 '''
 class union_music:
-    def __init__(self, x: Union[int, float] = 0, y: Union[int, float] = 0, z: Union[int, float] = 0, musicArray: Union[list, tuple] = ()):
+    def __init__(
+            self,
+            x: _tools.numType = 0,
+            y: _tools.numType = 0,
+            z: _tools.numType = 0,
+            musicArray: _Union[list, tuple] = ()
+    ):
         tick = eletricity.Nimp_Gate(x, y + 0.1, z)
         eletricity.crt_Wire(eletricity.Logic_Input(x, y, z).o, tick.i_up), eletricity.crt_Wire(tick.o, tick.i_low)
         eletricity.crt_Wire(tick.o, eletricity.Counter(x + 0.2, y, z).i_up)
         side = _math.ceil(_math.sqrt(musicArray.__len__()))
         pass
```

### Comparing `physicsLab-1.1.9/physicsLab.egg-info/PKG-INFO` & `physicsLab-1.2.1/physicsLab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsLab
-Version: 1.1.9
+Version: 1.2.1
 Summary: Doing experiments in the physics lab AR by python
 Home-page: https://gitee.com/script2000/physicsLab
 Author: Goodenough
 Author-email: 2381642961@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 1.  请确保你的电脑有[Python](https://www.python.org)与[物理实验室PC版](https://www.turtlesim.com/)（也可以联系[开发者Jone-Chen](https://gitee.com/civitasjohn)）
 2.  在cmd或shell输入：
 ```diff
 pip install physicsLab
 ```
 
 ## 开发环境
-python 3.7, PyCharm, win7  
+python 3.7.8, win7  
 目测对其他版本支持应该也很好
 3.6及以上应该没问题
 
 ## 使用说明
 
 ```Python
 from physicsLab import *
@@ -52,15 +52,15 @@
  # crt_wire输入格式：  
  #    crt_wire(SourcePin, TargetPin, color = "蓝")  
 crt_Wire(o.i_up, o.i_low)  
  # 将程序中生成的原件，导线等等写入存档  
 write_Experiment()  
  # 然后用物实打开存档见证奇迹  
 ```
-更详细的内容请查看[functions.md](physicsLab/functions.md)  
+更详细的内容请查看[functions.md](functions.md)  
 请注意：Python采用GBK编码，而物实用的是utf-8，尽管尽量确保编码格式正确，但中文仍有可能出现问题，因此建议多用英文。  
 
 ## 优点
 1. 通过read_Experiment()，你无须把所有工作交给代码。因为用代码写并不总是意味着方便（比如连接导线）。  
 你现在可以手动连接部分导线或者添加原件，并通过保存的形式，让程序在下次也可以轻松读取。  
 这也意味着你不用一口气把控制整个电路的脚本写出来，而是每次写一部分，并把更适合代码的工作交给代码完成。  
 也就是说，写这个脚本的感觉更像在控制台上操作，非常灵活。
```

### Comparing `physicsLab-1.1.9/physicsLab.egg-info/SOURCES.txt` & `physicsLab-1.2.1/physicsLab.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,10 +23,11 @@
 physicsLab/electricity/elementsClass/_elementClassHead.py
 physicsLab/electricity/elementsClass/artificialCircuit.py
 physicsLab/electricity/elementsClass/basicCircuit.py
 physicsLab/electricity/elementsClass/logicCircuit.py
 physicsLab/electricity/elementsClass/otherCircuit.py
 physicsLab/electromagnetism/__init__.py
 physicsLab/unionElements/__init__.py
+physicsLab/unionElements/_unionClassHead.py
 physicsLab/unionElements/unionLogic.py
 physicsLab/unionElements/unionPin.py
 physicsLab/unionElements/union_music.py
```

### Comparing `physicsLab-1.1.9/pyproject.toml` & `physicsLab-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `physicsLab-1.1.9/setup.py` & `physicsLab-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #coding=utf-8
 import setuptools  # 导入setuptools打包工具
 
-with open("D:/program physicsLab/hub/README.md", "r", encoding="utf-8") as fh:
+with open("D:/program_physicsLab/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="physicsLab",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.1.9",  # 包版本号，便于维护版本
+    version="1.2.1",  # 包版本号，便于维护版本
     author="Goodenough",  # 作者，可以写自己的姓名
     author_email="2381642961@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="Doing experiments in the physics lab AR by python",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://gitee.com/script2000/physicsLab",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

