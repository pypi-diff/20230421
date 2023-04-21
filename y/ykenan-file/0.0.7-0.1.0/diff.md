# Comparing `tmp/ykenan_file-0.0.7.tar.gz` & `tmp/ykenan_file-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_file-0.0.7.tar", last modified: Thu Apr  6 02:17:18 2023, max compression
+gzip compressed data, was "ykenan_file-0.1.0.tar", last modified: Fri Apr 21 09:20:29 2023, max compression
```

## Comparing `ykenan_file-0.0.7.tar` & `ykenan_file-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 02:17:18.948580 ykenan_file-0.0.7/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      833 2023-04-06 02:17:18.948580 ykenan_file-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-04-06 01:58:07.000000 ykenan_file-0.0.7/README.md
--rw-rw-rw-   0        0        0      676 2023-04-06 02:15:35.000000 ykenan_file-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 02:17:18.949580 ykenan_file-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-06 02:17:18.932580 ykenan_file-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-06 02:17:18.940580 ykenan_file-0.0.7/src/ykenan_file/
--rw-rw-rw-   0        0        0    20803 2023-04-06 02:15:35.000000 ykenan_file-0.0.7/src/ykenan_file/__init__.py
--rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.0.7/src/ykenan_file/util.py
-drwxrwxrwx   0        0        0        0 2023-04-06 02:17:18.947580 ykenan_file-0.0.7/src/ykenan_file.egg-info/
--rw-rw-rw-   0        0        0      833 2023-04-06 02:17:18.000000 ykenan_file-0.0.7/src/ykenan_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-06 02:17:18.000000 ykenan_file-0.0.7/src/ykenan_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 02:17:18.000000 ykenan_file-0.0.7/src/ykenan_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-06 02:17:18.000000 ykenan_file-0.0.7/src/ykenan_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-06 02:17:18.000000 ykenan_file-0.0.7/src/ykenan_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 09:20:29.911106 ykenan_file-0.1.0/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      829 2023-04-21 09:20:29.910106 ykenan_file-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-21 09:16:49.000000 ykenan_file-0.1.0/README.md
+-rw-rw-rw-   0        0        0      676 2023-04-21 09:16:49.000000 ykenan_file-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 09:20:29.911106 ykenan_file-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 09:20:29.882994 ykenan_file-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 09:20:29.902106 ykenan_file-0.1.0/src/ykenan_file/
+-rw-rw-rw-   0        0        0    23284 2023-04-21 09:15:52.000000 ykenan_file-0.1.0/src/ykenan_file/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.0/src/ykenan_file/util.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:20:29.909106 ykenan_file-0.1.0/src/ykenan_file.egg-info/
+-rw-rw-rw-   0        0        0      829 2023-04-21 09:20:29.000000 ykenan_file-0.1.0/src/ykenan_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-21 09:20:29.000000 ykenan_file-0.1.0/src/ykenan_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:20:29.000000 ykenan_file-0.1.0/src/ykenan_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-21 09:20:29.000000 ykenan_file-0.1.0/src/ykenan_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 09:20:29.000000 ykenan_file-0.1.0/src/ykenan_file.egg-info/top_level.txt
```

### Comparing `ykenan_file-0.0.7/LICENSE` & `ykenan_file-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.0.7/PKG-INFO` & `ykenan_file-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_file
-Version: 0.0.7
+Version: 0.1.0
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,9 +31,7 @@
 > import
 
 ```shell
 import ykenan_file as yf
 ```
 
 
-
-
```

### Comparing `ykenan_file-0.0.7/pyproject.toml` & `ykenan_file-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_file"
-version = "0.0.7"
+version = "0.1.0"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "file", "read", "write"]
 description = "File read and write operations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `ykenan_file-0.0.7/src/ykenan_file/__init__.py` & `ykenan_file-0.1.0/src/ykenan_file/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding: UTF-8 -*-
 
 import itertools
 import os
 
 import pandas as pd
-import ykenan_log
+from ykenan_log import Logger
 from pandas import DataFrame
 
-logger = ykenan_log.Logger("ykenan_file", is_form_file=False)
-
 '''
  * @Author       : YKenan
  * @Description  : file handler
 '''
 
 
 class Create:
@@ -22,37 +20,42 @@
     """
 
     def __init__(self, sep='\t',
                  line_terminator="\n",
                  encoding: str = 'utf_8_sig',
                  index: bool = False,
                  header: bool = True,
-                 sheet_name='new_sheet'):
+                 sheet_name='new_sheet',
+                 log_file: str = "ykenan_file",
+                 is_form_log_file: bool = True):
         """
         Initialization creation information, public information
         :param sep: File Separator
         :param line_terminator: File Line Break
         :param encoding: Document code
         :param index: Whether there is a row index
         :param header: Whether there is a title
         :param sheet_name: sheet name
+        :param log_file: Path to form a log file
+        :param is_form_log_file: Is a log file formed
         """
+        self.log = Logger(log_file, is_form_file=is_form_log_file)
         self.sep = sep
         self.line_terminator = line_terminator
         self.encoding = encoding
         self.index = index
         self.header = header
         self.sheet_name = sheet_name
 
     def to_file(self, df: DataFrame, file: str) -> None:
         """
         :param df: DataFrame
         :param file: File path plus name
         """
-        logger.debug(f"create a file: {file}")
+        self.log.debug(f"create a file: {file}")
         # 导出文件
         if str(file).endswith(".txt"):
             df.to_csv(file, sep=self.sep, lineterminator=self.line_terminator, header=self.header, encoding=self.encoding, index=self.index)
         elif str(file).endswith(".csv"):
             df.to_csv(file, sep=',', lineterminator=self.line_terminator, header=self.header, encoding=self.encoding, index=self.index)
         elif str(file).endswith(".xls") or str(file).endswith(".xlsx"):
             df.to_excel(file, sheet_name=self.sheet_name, header=self.header, index=self.index)
@@ -65,30 +68,30 @@
         Modify the file column name
         :param df: source document
         :param columns: New column name
         :param output_file: Output file path
         :return:
         """
         # 重新命名
-        logger.debug(f"Modify the file column name: {columns}")
+        self.log.debug(f"Modify the file column name: {columns}")
         df.columns = columns
         # 保存
         if output_file is not None:
             self.to_file(df, output_file)
 
     def drop_columns(self, df: DataFrame, columns: list, output_file: str = None) -> None:
         """
         Delete File Column Name
         :param df: source document
         :param columns: 删除的列名
         :param output_file: Output file path
         :return:
         """
         # 删除列
-        logger.debug(f"删除文件列名: {columns}")
+        self.log.debug(f"删除文件列名: {columns}")
         df.drop(columns, axis=1, inplace=True)
         # 保存文件
         if output_file is not None:
             self.to_file(df, output_file)
 
     def add_content(self, df: DataFrame, list_content: list, columns=None, is_log: bool = False, output_file: str = None) -> None:
         """
@@ -100,15 +103,15 @@
         :param is_log: 是否打印 log
         :return:
         """
         # 添加内容
         if columns is None:
             columns: list = list(df.columns)
         if is_log:
-            logger.debug(f"添加内容 {list_content} ...")
+            self.log.debug(f"添加内容 {list_content} ...")
         df.loc[len(df)] = pd.Series(list_content, index=columns)
         # 保存文件
         if output_file is not None:
             self.to_file(df, output_file)
 
     def add_difference_column(self, df: DataFrame, column: str, a: str, b: str, output_file: str = None) -> None:
         """
@@ -116,30 +119,30 @@
         :param df: DataFrame
         :param column: 添加的一个新列名
         :param a: 被减数
         :param b: 减数
         :param output_file: Output file path
         :return:
         """
-        logger.debug(f"添加一个减法列: {column}")
+        self.log.debug(f"添加一个减法列: {column}")
         df[column] = df[a] - df[b]
         # 保存文件
         if output_file is not None:
             self.to_file(df, output_file)
 
     def add_rank_group_by(self, df: DataFrame, group: list, column: str, output_file: str = None) -> None:
         """
         添加五个 rank 列
         :param df: DataFrame
         :param group: 分组的列
         :param column: 需要秩的列
         :param output_file: Output file path
         :return:
         """
-        logger.debug(f"添加五个 rank 列: {group}, {column}")
+        self.log.debug(f"添加五个 rank 列: {group}, {column}")
         # 添加排名
         for method in ['average', 'min', 'max', 'dense', 'first']:
             df[f'{method}_rank'] = df.groupby(group)[column].rank(method)
         # 保存文件
         if output_file is not None:
             self.to_file(df, output_file)
 
@@ -149,15 +152,15 @@
         :param df: DataFrame
         :param group: 分组的列
         :param column: 需要和的列
         :param output_file: Output file path
         :return:
         """
         # 总和
-        logger.debug(f"通过分组计算某列数总和: {group}, {column}")
+        self.log.debug(f"通过分组计算某列数总和: {group}, {column}")
         column_sum = df.groupby(group)[column].sum().reset_index()
         group.append(f"{column}_sum")
         column_sum.columns = group
         # 保存文件
         if output_file is not None:
             self.to_file(column_sum, output_file)
         return column_sum
@@ -168,15 +171,15 @@
         :param df: DataFrame
         :param group: 分组的列
         :param column: 需要数量的列
         :param output_file: Output file path
         :return:
         """
         # 总和
-        logger.debug(f"通过分组计算某列数总和: {group}, {column}")
+        self.log.debug(f"通过分组计算某列数总和: {group}, {column}")
         column_sum = df.groupby(group)[column].count().reset_index()
         group.append(f"{column}_count")
         column_sum.columns = group
         # 保存文件
         if output_file is not None:
             self.to_file(column_sum, output_file)
         return column_sum
@@ -189,15 +192,15 @@
         :param column: 需要秩的列
         :param on: 合并的列
         :param output_file: Output file path
         :param add_merge_files: 添加 merge 文件
         :return:
         """
         # 总和
-        logger.debug(f"通过分组进行一系列数值计算: {group}, {column}")
+        self.log.debug(f"通过分组进行一系列数值计算: {group}, {column}")
         # 个数大小
         column_size = df.groupby(group)[column].size().reset_index()
         group.append(f"{column}_size")
         column_size.columns = group
         # 平均值
         column_mean = df.groupby(group)[column].mean().reset_index()
         group.append(f"{column}_mean")
@@ -249,19 +252,19 @@
         :param files: 多个文件
         :param on: 关键 key
         :param output_file: Output file path
         :return:
         """
         # 总和
         size = len(files)
-        logger.debug(f"将文件进行合并: {size}, {on}")
+        self.log.debug(f"将文件进行合并: {size}, {on}")
         new_file = files[0]
         i = 1
         while i < size:
-            logger.debug(f"将文件进行合并第 {i} 次")
+            self.log.debug(f"将文件进行合并第 {i} 次")
             new_file = pd.merge(new_file, files[i], on=on)
             i += 1
         # 保存文件
         if output_file is not None:
             self.to_file(new_file, output_file)
 
 
@@ -273,26 +276,31 @@
     def __init__(self, sep='\t',
                  line_terminator="\n",
                  encoding: str = "utf-8",
                  orient: str = "records",
                  lines: bool = True,
                  header="infer",
                  sheet_name=0,
-                 low_memory: bool = False):
+                 low_memory: bool = False,
+                 log_file: str = "ykenan_file",
+                 is_form_log_file: bool = True):
         """
         Read file initialization information, public information
         :param sep: file separator
         :param line_terminator: file line break
         :param encoding: file encoding
         :param orient: Indicates the expected JSON string format, which is valid only when reading a json file
         :param lines: Read the file as a json object per line
         :param header: The first row header situation
         :param sheet_name: Specify the sheet number when reading Excel
         :param low_memory: Process files in internal chunks to reduce memory usage during parsing
+        :param log_file: Path to form a log file
+        :param is_form_log_file: Is a log file formed
         """
+        self.log = Logger(log_file, is_form_file=is_form_log_file)
         self.sep = sep
         self.line_terminator = line_terminator
         self.encoding = encoding
         self.orient = orient
         self.lines = lines
         self.header = header
         self.sheet_name = sheet_name
@@ -300,15 +308,15 @@
 
     def get_content(self, file: str):
         """
         Get file content
         :param file: File path information
         :return:
         """
-        logger.debug(f"Start reading {file} file...")
+        self.log.debug(f"Start reading {file} file...")
         if str(file).endswith(".txt") or str(file).endswith(".bed"):
             return pd.read_table(file, sep=self.sep, header=self.header, encoding=self.encoding, low_memory=self.low_memory)
         elif str(file).endswith(".csv"):
             return pd.read_csv(file, sep=',', header=self.header, encoding=self.encoding, low_memory=self.low_memory)
         elif str(file).endswith(".xls") or str(file).endswith(".xlsx"):
             return pd.read_excel(file, sheet_name=self.sheet_name, header=self.header if isinstance(self.header, int) else 0)
         elif str(file).endswith(".html") or str(file).endswith(".htm"):
@@ -334,250 +342,260 @@
         :param output_file:
         :param join: How to merge files
         :param index:
         :param encoding: Encoding of output files
         :return:
         """
         file_content = self.read_file(*files)
-        logger.debug(f"Start merging files {files} ...")
+        self.log.debug(f"Start merging files {files} ...")
         pd_concat = pd.concat(file_content, join=join, ignore_index=True)
         pd.DataFrame(pd_concat).to_csv(output_file, encoding=encoding, sep=self.sep, index=index)
 
 
-def read_file_line(path: str, mode: str = 'r', encoding: str = "utf-8") -> list:
-    """
-    Read file by line
-    :param path:
-    :param mode:
-    :param encoding:
-    :return:
-    """
-    content = []
-    with open(path, mode, encoding=encoding) as f:
-        while True:
-            line = f.readline().strip()
-            content.append(line)
-            if not line:
-                break
-    return content
-
-
-def write_file_line(path: str, content: list, line: str = '\n', mode: str = 'a', encoding: str = "utf-8") -> None:
+class staticMethod:
     """
-    Write a file (write by line, and it will not be cleared if the original file is called again by default)
-    :param path:
-    :param content:
-    :param line:
-    :param mode:
-    :param encoding:
-    :return:
+    文件或者路径的静态方法
     """
-    with open(path, mode, encoding=encoding) as f:
-        for li in content:
-            f.write(li + line)
 
+    def __init__(self, log_file: str = "ykenan_file", is_form_log_file: bool = True):
+        """
+        :param log_file: Path to form a log file
+        :param is_form_log_file: Is a log file formed
+        """
+        self.log = Logger(log_file, is_form_file=is_form_log_file)
 
-def read_write_line(path: str, output: str, callback, column=None, rm: str = 'r', om: str = 'w',
-                    encoding: str = "utf-8", buffering: int = 1, newline: str = "\n") -> None:
-    """
-    Write one file to another
-    :param column: Output column name
-    :param path: Enter a path
-    :param output: output path
-    :param callback: A callback function that returns the input data
-    :param rm: Read mode
-    :param om: Output mode
-    :param encoding: encoding
-    :param buffering: Number of loaded lines in the output file
-    :param newline: The newline character of the output file
-    :return:
-    """
-    with open(output, om, encoding=encoding, buffering=buffering, newline=newline) as w:
-        with open(path, rm, encoding=encoding) as f:
-            if column:
-                name: str = "\t".join(column)
-                logger.debug(f"Add Column Name: {name}")
-                w.write(f"{name}\n")
+    def read_file_line(self, path: str, mode: str = 'r', encoding: str = "utf-8") -> list:
+        """
+        Read file by line
+        :param path:
+        :param mode:
+        :param encoding:
+        :return:
+        """
+        content = []
+        self.log.info(f"Start reading file {path}")
+        with open(path, mode, encoding=encoding) as f:
             while True:
-                line: str = f.readline().strip()
+                line = f.readline().strip()
+                content.append(line)
                 if not line:
                     break
-                new_line: list = callback(line)
-                if new_line and len(new_line) != 0 and new_line != "":
-                    content = "\t".join(new_line)
-                    w.write(f"{content}\n")
-
-
-def get_contents(path: str) -> list:
-    """
-    Obtain all files and folders under the specified path
-    :param path: path
-    :return: files and folders
-    """
-    return list(os.listdir(path))
-
-
-def entry_contents(path: str, type_: int = 0) -> list:
-    """
-    Obtain all files and (or) folders under the specified path
-    :param path: path
-    :param type_: judge file or dir
-    :return: files and (or) folders
-    """
-    contents: list = []
-    with os.scandir(path) as it:
-        for entry in it:
-            entry: os.DirEntry
-            if type_ == 0:
-                contents.append(entry.name)
-            elif type_ == 1 and entry.is_file():
-                contents.append(entry.name)
-            elif type_ == 2 and entry.is_dir():
-                contents.append(entry.name)
-            else:
-                raise ValueError("type input error, type is 0 or 1 or 2.")
-    return contents
-
-
-def entry_contents_path(path: str, type_: int = 0) -> list:
-    """
-    Obtain all files and (or) folders under the specified path
-    :param path: path
-    :param type_: judge file or dir
-    :return: files and (or) folders path
-    """
-    contents: list = []
-    with os.scandir(path) as it:
-        for entry in it:
-            entry: os.DirEntry
-            if type_ == 0:
-                contents.append(entry.path)
-            elif type_ == 1:
-                if entry.is_file():
-                    contents.append(entry.path)
-            elif type_ == 2:
-                if entry.is_dir():
-                    contents.append(entry.path)
-            else:
-                raise ValueError("type input error, type is 0 or 1 or 2.")
-    return contents
-
-
-def get_files(path: str) -> list:
-    """
-    Obtain all files in the specified path
-    :param path:  path
-    :return: files
-    """
-    files: list = []
-    with os.scandir(path) as it:
-        for entry in it:
-            entry: os.DirEntry
-            if entry.is_file():
-                files.append(entry.name)
-    return files
-
-
-def get_files_path(path: str) -> list:
-    """
-    Obtain all files in the specified path
-    :param path:  path
-    :return: files
-    """
-    files: list = []
-    with os.scandir(path) as it:
-        for entry in it:
-            entry: os.DirEntry
-            if entry.is_file():
-                files.append(entry.path)
-    return files
-
-
-def get_dirs(path: str) -> list:
-    """
-    Obtain all files in the specified path
-    :param path:  path
-    :return: files
-    """
-    dirs: list = []
-    with os.scandir(path) as it:
-        for entry in it:
-            entry: os.DirEntry
-            if entry.is_dir():
-                dirs.append(entry.name)
-    return dirs
-
-
-def get_dirs_path(path: str) -> list:
-    """
-    Obtain all files in the specified path
-    :param path:  path
-    :return: files
-    """
-    dirs: list = []
-    with os.scandir(path) as it:
-        for entry in it:
-            entry: os.DirEntry
-            if entry.is_dir():
-                dirs.append(entry.path)
-    return dirs
-
+        return content
 
-def entry_contents_dict(path: str, type_: int = 0, suffix: str = None) -> dict:
-    """
-    Obtain all files in the specified path
-    :param path: path
-    :param type_: type_
-    :param suffix: 筛选的条件
-    :return: files and (or) dirs
-    """
-    files: list = []
-    dirs: list = []
-    contents: list = []
-    dict_: dict = {}
-    with os.scandir(path) as it:
-        for entry in it:
-            entry: os.DirEntry
-            # 判断是否满足情况
-            if suffix is None or entry.name.endswith(entry.name):
+    def write_file_line(self, path: str, content: list, line: str = '\n', mode: str = 'a', encoding: str = "utf-8") -> None:
+        """
+        Write a file (write by line, and it will not be cleared if the original file is called again by default)
+        :param path:
+        :param content:
+        :param line:
+        :param mode:
+        :param encoding:
+        :return:
+        """
+        self.log.info(f"Start writing file {path}")
+        with open(path, mode, encoding=encoding) as f:
+            for li in content:
+                f.write(li + line)
+
+    def read_write_line(self, path: str, output: str, callback, column=None, rm: str = 'r', om: str = 'w',
+                        encoding: str = "utf-8", buffering: int = 1, newline: str = "\n") -> None:
+        """
+        Write one file to another
+        :param column: Output column name
+        :param path: Enter a path
+        :param output: output path
+        :param callback: A callback function that returns the input data
+        :param rm: Read mode
+        :param om: Output mode
+        :param encoding: encoding
+        :param buffering: Number of loaded lines in the output file
+        :param newline: The newline character of the output file
+        :return:
+        """
+        with open(output, om, encoding=encoding, buffering=buffering, newline=newline) as w:
+            with open(path, rm, encoding=encoding) as f:
+                if column:
+                    name: str = "\t".join(column)
+                    self.log.debug(f"Add Column Name: {name}")
+                    w.write(f"{name}\n")
+                while True:
+                    line: str = f.readline().strip()
+                    if not line:
+                        break
+                    new_line: list = callback(line)
+                    if new_line and len(new_line) != 0 and new_line != "":
+                        content = "\t".join(new_line)
+                        w.write(f"{content}\n")
+
+    def get_contents(self, path: str) -> list:
+        """
+        Obtain all files and folders under the specified path
+        :param path: path
+        :return: files and folders
+        """
+        self.log.info("Starting to retrieve content under this path")
+        return list(os.listdir(path))
+
+    def entry_contents(self, path: str, type_: int = 0) -> list:
+        """
+        Obtain all files and (or) folders under the specified path
+        :param path: path
+        :param type_: judge file or dir
+        :return: files and (or) folders
+        """
+        self.log.info("Starting to retrieve content under this path")
+        contents: list = []
+        with os.scandir(path) as it:
+            for entry in it:
+                entry: os.DirEntry
                 if type_ == 0:
-                    dict_ = dict(itertools.chain(dict_.items(), {
-                        entry.name: entry.path
-                    }.items()))
                     contents.append(entry.name)
+                elif type_ == 1 and entry.is_file():
+                    contents.append(entry.name)
+                elif type_ == 2 and entry.is_dir():
+                    contents.append(entry.name)
+                else:
+                    raise ValueError("type input error, type is 0 or 1 or 2.")
+        return contents
+
+    def entry_contents_path(self, path: str, type_: int = 0) -> list:
+        """
+        Obtain all files and (or) folders under the specified path
+        :param path: path
+        :param type_: judge file or dir
+        :return: files and (or) folders path
+        """
+        self.log.info("Starting to retrieve content under this path")
+        contents: list = []
+        with os.scandir(path) as it:
+            for entry in it:
+                entry: os.DirEntry
+                if type_ == 0:
+                    contents.append(entry.path)
                 elif type_ == 1:
-                    # 此处判断不能和 type_ == 1 连写，因为需要进行提示 ValueError("type input error, type is 0 or 1 or 2.")
                     if entry.is_file():
-                        dict_ = dict(itertools.chain(dict_.items(), {
-                            entry.name: entry.path
-                        }.items()))
-                        files.append(entry.name)
+                        contents.append(entry.path)
                 elif type_ == 2:
                     if entry.is_dir():
-                        dict_ = dict(itertools.chain(dict_.items(), {
-                            entry.name: entry.path
-                        }.items()))
-                        dirs.append(entry.name)
+                        contents.append(entry.path)
                 else:
                     raise ValueError("type input error, type is 0 or 1 or 2.")
-    dict_ = dict(itertools.chain(dict_.items(), {
-        "name": contents if type_ == 0 else files if type_ == 1 else dirs
-    }.items()))
-    return dict_
+        return contents
 
+    def get_files(self, path: str) -> list:
+        """
+        Obtain all files in the specified path
+        :param path:  path
+        :return: files
+        """
+        self.log.info("Starting to retrieve files under this path")
+        files: list = []
+        with os.scandir(path) as it:
+            for entry in it:
+                entry: os.DirEntry
+                if entry.is_file():
+                    files.append(entry.name)
+        return files
 
-def entry_files_dict(path: str) -> dict:
-    """
-    Obtain all files in the specified path
-    :param path: path
-    :return: files
-    """
-    return entry_contents_dict(path, 1)
+    def get_files_path(self, path: str) -> list:
+        """
+        Obtain all files in the specified path
+        :param path:  path
+        :return: files
+        """
+        self.log.info("Starting to retrieve files under this path")
+        files: list = []
+        with os.scandir(path) as it:
+            for entry in it:
+                entry: os.DirEntry
+                if entry.is_file():
+                    files.append(entry.path)
+        return files
+
+    def get_dirs(self, path: str) -> list:
+        """
+        Obtain all files in the specified path
+        :param path:  path
+        :return: dirs
+        """
+        self.log.info("Starting to retrieve directories under this path")
+        dirs: list = []
+        with os.scandir(path) as it:
+            for entry in it:
+                entry: os.DirEntry
+                if entry.is_dir():
+                    dirs.append(entry.name)
+        return dirs
 
+    def get_dirs_path(self, path: str) -> list:
+        """
+        Obtain all files in the specified path
+        :param path:  path
+        :return: dirs
+        """
+        self.log.info("Starting to retrieve directories under this path")
+        dirs: list = []
+        with os.scandir(path) as it:
+            for entry in it:
+                entry: os.DirEntry
+                if entry.is_dir():
+                    dirs.append(entry.path)
+        return dirs
 
-def entry_dirs_dict(path: str) -> dict:
-    """
-    Obtain all files in the specified path
-    :param path: path
-    :return: dirs
-    """
-    return entry_contents_dict(path, 2)
+    def entry_contents_dict(self, path: str, type_: int = 0, suffix: str = None) -> dict:
+        """
+        Obtain all files in the specified path
+        :param path: path
+        :param type_: type_
+        :param suffix: 筛选的条件
+        :return: files and (or) dirs
+        """
+        self.log.info("Starting to retrieve content under this path")
+        files: list = []
+        dirs: list = []
+        contents: list = []
+        dict_: dict = {}
+        with os.scandir(path) as it:
+            for entry in it:
+                entry: os.DirEntry
+                # 判断是否满足情况
+                if suffix is None or entry.name.endswith(entry.name):
+                    if type_ == 0:
+                        dict_ = dict(itertools.chain(dict_.items(), {
+                            entry.name: entry.path
+                        }.items()))
+                        contents.append(entry.name)
+                    elif type_ == 1:
+                        # 此处判断不能和 type_ == 1 连写，因为需要进行提示 ValueError("type input error, type is 0 or 1 or 2.")
+                        if entry.is_file():
+                            dict_ = dict(itertools.chain(dict_.items(), {
+                                entry.name: entry.path
+                            }.items()))
+                            files.append(entry.name)
+                    elif type_ == 2:
+                        if entry.is_dir():
+                            dict_ = dict(itertools.chain(dict_.items(), {
+                                entry.name: entry.path
+                            }.items()))
+                            dirs.append(entry.name)
+                    else:
+                        raise ValueError("type input error, type is 0 or 1 or 2.")
+        dict_ = dict(itertools.chain(dict_.items(), {
+            "name": contents if type_ == 0 else files if type_ == 1 else dirs
+        }.items()))
+        return dict_
+
+    def entry_files_dict(self, path: str) -> dict:
+        """
+        Obtain all files in the specified path
+        :param path: path
+        :return: files
+        """
+        return self.entry_contents_dict(path, 1)
+
+    def entry_dirs_dict(self, path: str) -> dict:
+        """
+        Obtain all files in the specified path
+        :param path: path
+        :return: dirs
+        """
+        return self.entry_contents_dict(path, 2)
```

### Comparing `ykenan_file-0.0.7/src/ykenan_file.egg-info/PKG-INFO` & `ykenan_file-0.1.0/src/ykenan_file.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-file
-Version: 0.0.7
+Version: 0.1.0
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,9 +31,7 @@
 > import
 
 ```shell
 import ykenan_file as yf
 ```
 
 
-
-
```

