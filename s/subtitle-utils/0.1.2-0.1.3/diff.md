# Comparing `tmp/subtitle_utils-0.1.2.tar.gz` & `tmp/subtitle_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subtitle_utils-0.1.2.tar", max compression
+gzip compressed data, was "subtitle_utils-0.1.3.tar", max compression
```

## Comparing `subtitle_utils-0.1.2.tar` & `subtitle_utils-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      875 2023-02-08 04:56:39.726503 subtitle_utils-0.1.2/README.md
--rw-r--r--   0        0        0      602 2023-02-08 04:56:39.726503 subtitle_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2812 2023-02-08 04:56:39.726503 subtitle_utils-0.1.2/subtitle_utils/AssConverter.py
--rw-r--r--   0        0        0    10523 2023-02-08 04:56:39.726503 subtitle_utils-0.1.2/subtitle_utils/BccConverter.py
--rw-r--r--   0        0        0     3890 2023-02-08 04:56:39.726503 subtitle_utils-0.1.2/subtitle_utils/__init__.py
--rw-r--r--   0        0        0   270460 2023-02-08 04:56:39.726503 subtitle_utils-0.1.2/subtitle_utils/cover.png
--rw-r--r--   0        0        0       55 2023-02-08 04:56:39.726503 subtitle_utils-0.1.2/subtitle_utils/requirements.txt
--rw-r--r--   0        0        0      469 2023-02-08 04:56:39.726503 subtitle_utils-0.1.2/subtitle_utils/utils.py
--rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 subtitle_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      875 2023-04-21 14:55:59.293364 subtitle_utils-0.1.3/README.md
+-rw-r--r--   0        0        0      602 2023-04-21 14:55:59.293364 subtitle_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2812 2023-04-21 14:55:59.297364 subtitle_utils-0.1.3/subtitle_utils/AssConverter.py
+-rw-r--r--   0        0        0    11402 2023-04-21 14:55:59.297364 subtitle_utils-0.1.3/subtitle_utils/BccConverter.py
+-rw-r--r--   0        0        0     4363 2023-04-21 14:55:59.297364 subtitle_utils-0.1.3/subtitle_utils/__init__.py
+-rw-r--r--   0        0        0   270460 2023-04-21 14:55:59.297364 subtitle_utils-0.1.3/subtitle_utils/cover.png
+-rw-r--r--   0        0        0       55 2023-04-21 14:55:59.297364 subtitle_utils-0.1.3/subtitle_utils/requirements.txt
+-rw-r--r--   0        0        0      469 2023-04-21 14:55:59.297364 subtitle_utils-0.1.3/subtitle_utils/utils.py
+-rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 subtitle_utils-0.1.3/PKG-INFO
```

### Comparing `subtitle_utils-0.1.2/README.md` & `subtitle_utils-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `subtitle_utils-0.1.2/pyproject.toml` & `subtitle_utils-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "subtitle-utils"
-version = "0.1.2"
+version = "0.1.3"
 description = "Subtilte Conversion utils - ass2srt vtt2bcc srt2bcc ass2bcc and more"
 authors = ["sudoskys <coldlando@hotmail.com>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "subtitle_utils"}]
 repository = "https://github.com/sudoskys/subtitle_utils"
```

### Comparing `subtitle_utils-0.1.2/subtitle_utils/AssConverter.py` & `subtitle_utils-0.1.3/subtitle_utils/AssConverter.py`

 * *Files identical despite different names*

### Comparing `subtitle_utils-0.1.2/subtitle_utils/BccConverter.py` & `subtitle_utils-0.1.3/subtitle_utils/BccConverter.py`

 * *Files 6% similar despite different names*

```diff
@@ -165,14 +165,17 @@
                 "content": sub.text,
             }
             for sub in subs
         ])
         _fix = self.merge_timeline(_origin)
         return _fix
 
+    def time2str(self, time: float):
+        return datetime.utcfromtimestamp(time).strftime("%H:%M:%S,%f")[:-3]
+
     def srt2bcc(self, files: Union[str], about: str = None):
         """
         srt2bcc 将 srt 转换为 bcc B站字幕格式
         :return:
         """
         path = files if files else ""
         if os.path.exists(path):
@@ -186,14 +189,37 @@
             "background_alpha": 0.5,
             "background_color": "#9C27B0",
             "Stroke": "none",
             "body": body
         }
         return bcc if subs else {}
 
+    def bcc2srt(self, files: Union[str]):
+        """
+        bcc2srt 将 bcc 转换为 srt 字幕格式
+        :return:
+        """
+        path = files if files else ""
+        if os.path.exists(path):
+            with open(path, "r", encoding="utf-8") as f:
+                subs = json.load(f)
+        else:
+            subs = json.loads(path)
+        srt = ""
+        count = 0
+        for single_str in subs["body"]:
+            count += 1
+            content_str = single_str['content']
+            from_str = single_str['from']
+            to_str = single_str['to']
+            srt += f"{count}\n"
+            srt += f"{self.time2str(from_str)} --> {self.time2str(to_str)}\n"
+            srt += f"{content_str}\n\n"
+        return srt[:-1] if subs else ""
+
     def vtt2bcc(self, files, threshold=0.1, word=True, about: str = None):
         path = files if files else ""
         if os.path.exists(path):
             subs = pyvtt.open(path)
         else:
             subs = pyvtt.from_string(path)
         # NOTE 按照 vtt 的断词模式分隔 bcc
```

### Comparing `subtitle_utils-0.1.2/subtitle_utils/__init__.py` & `subtitle_utils-0.1.3/subtitle_utils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,36 +56,53 @@
                 strs: Union[str],
                 header: str = "",
                 **kwargs
                 ) -> str:
         result = AssConvert().srt2ass(strs=strs, header=header)
         return result
 
+    def bcc2srt(self,
+                strs: Union[str],
+                **kwargs
+                ) -> str:
+        result = BccConvert().bcc2srt(files=strs)
+        return result
+
+    def bcc2ass(self,
+                strs: Union[str],
+                **kwargs
+                ) -> str:
+        result = BccConvert().bcc2srt(files=strs)
+        result = AssConvert().srt2ass(strs=result)
+        return result
+
 
 class Returner(BaseModel):
     status: bool = False
     pre: str
     aft: str
     msg: str = "Unknown"
     data: str = None
 
 
 __kira = _Converter()
 
 _to_table = {
     "2srt": {
         "ass": __kira.ass2srt,
+        "bcc": __kira.bcc2srt,
     },
     "2bcc": {
         "vtt": __kira.vtt2bcc,
         "srt": __kira.srt2bcc,
         "ass": __kira.ass2bcc,
     },
     "2ass": {
         "srt": __kira.srt2ass,
+        "bcc": __kira.bcc2ass,
     },
 }
 
 
 def SeeAvailableMethods() -> list:
     """
     查询可用方法，返回功能列表
```

### Comparing `subtitle_utils-0.1.2/subtitle_utils/cover.png` & `subtitle_utils-0.1.3/subtitle_utils/cover.png`

 * *Files identical despite different names*

### Comparing `subtitle_utils-0.1.2/PKG-INFO` & `subtitle_utils-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subtitle-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Subtilte Conversion utils - ass2srt vtt2bcc srt2bcc ass2bcc and more
 Home-page: https://github.com/sudoskys/subtitle_utils
 License: LGPL-3.0-or-later
 Author: sudoskys
 Author-email: coldlando@hotmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

