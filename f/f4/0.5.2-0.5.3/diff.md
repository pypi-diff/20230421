# Comparing `tmp/f4-0.5.2.tar.gz` & `tmp/f4-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4-0.5.2.tar", last modified: Mon Apr 17 18:54:00 2023, max compression
+gzip compressed data, was "f4-0.5.3.tar", last modified: Fri Apr 21 10:11:53 2023, max compression
```

## Comparing `f4-0.5.2.tar` & `f4-0.5.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:54:00.717484 f4-0.5.2/
--rw-r--r--   0 srp33      (501) staff       (20)    11357 2023-02-09 00:36:34.000000 f4-0.5.2/LICENSE
--rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-17 18:54:00.717613 f4-0.5.2/PKG-INFO
--rwxr-xr-x   0 srp33      (501) staff       (20)       67 2023-02-19 23:03:17.000000 f4-0.5.2/README.md
--rw-r--r--   0 srp33      (501) staff       (20)      104 2023-02-09 00:40:41.000000 f4-0.5.2/pyproject.toml
--rw-r--r--   0 srp33      (501) staff       (20)      733 2023-04-17 18:54:00.718222 f4-0.5.2/setup.cfg
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:54:00.708361 f4-0.5.2/src/
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:54:00.713804 f4-0.5.2/src/f4/
--rwxr-xr-x   0 srp33      (501) staff       (20)    37651 2023-04-17 18:51:51.000000 f4-0.5.2/src/f4/Builder.py
--rwxr-xr-x   0 srp33      (501) staff       (20)    49304 2023-04-03 18:58:04.000000 f4-0.5.2/src/f4/Parser.py
--rwxr-xr-x   0 srp33      (501) staff       (20)     8780 2023-04-17 18:53:39.000000 f4-0.5.2/src/f4/Utilities.py
--rwxr-xr-x   0 srp33      (501) staff       (20)      446 2023-04-16 18:51:11.000000 f4-0.5.2/src/f4/__init__.py
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:54:00.716037 f4-0.5.2/src/f4.egg-info/
--rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-17 18:54:00.000000 f4-0.5.2/src/f4.egg-info/PKG-INFO
--rw-r--r--   0 srp33      (501) staff       (20)      278 2023-04-17 18:54:00.000000 f4-0.5.2/src/f4.egg-info/SOURCES.txt
--rw-r--r--   0 srp33      (501) staff       (20)        1 2023-04-17 18:54:00.000000 f4-0.5.2/src/f4.egg-info/dependency_links.txt
--rw-r--r--   0 srp33      (501) staff       (20)       67 2023-04-17 18:54:00.000000 f4-0.5.2/src/f4.egg-info/requires.txt
--rw-r--r--   0 srp33      (501) staff       (20)        3 2023-04-17 18:54:00.000000 f4-0.5.2/src/f4.egg-info/top_level.txt
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-17 18:54:00.716402 f4-0.5.2/test/
--rwxr-xr-x   0 srp33      (501) staff       (20)    52520 2023-04-17 09:22:56.000000 f4-0.5.2/test/test.py
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-21 10:11:53.445028 f4-0.5.3/
+-rw-r--r--   0 srp33      (501) staff       (20)    11357 2023-02-09 00:36:34.000000 f4-0.5.3/LICENSE
+-rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-21 10:11:53.445142 f4-0.5.3/PKG-INFO
+-rwxr-xr-x   0 srp33      (501) staff       (20)       67 2023-02-19 23:03:17.000000 f4-0.5.3/README.md
+-rw-r--r--   0 srp33      (501) staff       (20)      104 2023-02-09 00:40:41.000000 f4-0.5.3/pyproject.toml
+-rw-r--r--   0 srp33      (501) staff       (20)      733 2023-04-21 10:11:53.445709 f4-0.5.3/setup.cfg
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-21 10:11:53.437454 f4-0.5.3/src/
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-21 10:11:53.441849 f4-0.5.3/src/f4/
+-rwxr-xr-x   0 srp33      (501) staff       (20)    37928 2023-04-21 10:07:59.000000 f4-0.5.3/src/f4/Builder.py
+-rwxr-xr-x   0 srp33      (501) staff       (20)    49489 2023-04-21 10:07:49.000000 f4-0.5.3/src/f4/Parser.py
+-rwxr-xr-x   0 srp33      (501) staff       (20)     8872 2023-04-21 10:10:00.000000 f4-0.5.3/src/f4/Utilities.py
+-rwxr-xr-x   0 srp33      (501) staff       (20)      416 2023-04-21 09:55:49.000000 f4-0.5.3/src/f4/__init__.py
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-21 10:11:53.443649 f4-0.5.3/src/f4.egg-info/
+-rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-21 10:11:53.000000 f4-0.5.3/src/f4.egg-info/PKG-INFO
+-rw-r--r--   0 srp33      (501) staff       (20)      278 2023-04-21 10:11:53.000000 f4-0.5.3/src/f4.egg-info/SOURCES.txt
+-rw-r--r--   0 srp33      (501) staff       (20)        1 2023-04-21 10:11:53.000000 f4-0.5.3/src/f4.egg-info/dependency_links.txt
+-rw-r--r--   0 srp33      (501) staff       (20)       67 2023-04-21 10:11:53.000000 f4-0.5.3/src/f4.egg-info/requires.txt
+-rw-r--r--   0 srp33      (501) staff       (20)        3 2023-04-21 10:11:53.000000 f4-0.5.3/src/f4.egg-info/top_level.txt
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-21 10:11:53.443977 f4-0.5.3/test/
+-rwxr-xr-x   0 srp33      (501) staff       (20)    52609 2023-04-21 10:10:44.000000 f4-0.5.3/test/test.py
```

### Comparing `f4-0.5.2/LICENSE` & `f4-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `f4-0.5.2/PKG-INFO` & `f4-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.5.2
+Version: 0.5.3
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.5.2/setup.cfg` & `f4-0.5.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = f4
-version = 0.5.2
+version = 0.5.3
 author = Stephen R. Piccolo
 author_email = stephen.piccolo.byu@gmail.com
 description = A Python package for the Fast Fixed-width File Format (F4)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/srp33/f4py
 project_urls =
```

### Comparing `f4-0.5.2/src/f4/Builder.py` & `f4-0.5.3/src/f4/Builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,14 +260,16 @@
     build_one_column_index(f4_file_path, index_column, tmp_dir_path, verbose, reverse_string)
 
 #####################################################
 # Non-public function(s)
 #####################################################
 
 def write_meta_files(tmp_dir_path_outputs, column_sizes, line_lengths_dict, column_names=None, column_types=None, compression_type=None, column_compression_dicts=None, num_rows=None):
+    write_str_to_file(f"{tmp_dir_path_outputs}ver", get_current_version_major().encode())
+
     # Calculate and write the column coordinates and max length of these coordinates.
     column_start_coords = get_column_start_coords(column_sizes)
     column_coords_string, max_column_coord_length = build_string_map(column_start_coords)
     write_str_to_file(f"{tmp_dir_path_outputs}cc", column_coords_string)
     write_str_to_file(f"{tmp_dir_path_outputs}mccl", str(max_column_coord_length).encode())
 
     # Find and write the line length(s).
@@ -575,14 +577,16 @@
             value = parse_function(file_data, row_index, coords, bigram_size_dict=bigram_size_dict, column_name=index_column_encoded)
             values_positions.append([value, row_index])
 
         print_message(f"Building index file for {index_column} index for {f4_file_path}.", verbose)
         customize_index_values_positions(values_positions, [index_column_type], sort_first_column, custom_index_function)
         write_index_files(values_positions, tmp_dir_path_data, tmp_dir_path_other)
 
+        write_str_to_file(f"{tmp_dir_path_other}ver", get_current_version_major().encode())
+
         index_file_path = get_index_file_path(f4_file_path, index_column, custom_index_function)
         combine_into_single_file(tmp_dir_path_data, tmp_dir_path_other, index_file_path)
 
         print_message(f"Done building index file for {index_column} index for {f4_file_path}.", verbose)
 
 # TODO: Combine this function with the above one and make it generic enough to handle indexes with more columns.
 def build_two_column_index(f4_file_path, index_column_1, index_column_2, tmp_dir_path, verbose):
@@ -621,14 +625,16 @@
 
             values_positions.append([value_1, value_2, row_index])
 
         print_message(f"Building index file for {index_name}.", verbose)
         customize_index_values_positions(values_positions, [index_column_1_type, index_column_2_type], sort_first_two_columns, do_nothing)
         write_index_files(values_positions, tmp_dir_path_data, tmp_dir_path_other)
 
+        write_str_to_file(f"{tmp_dir_path_other}ver", get_current_version_major().encode())
+
         index_file_path = get_index_file_path(f4_file_path, index_name)
         combine_into_single_file(tmp_dir_path_data, tmp_dir_path_other, index_file_path)
 
         print_message(f"Done building two-column index file for {index_name}.", verbose)
 
 def customize_index_values_positions(values_positions, column_types, sort_function, custom_index_function):
     # Iterate through each "column" except the last one (which has row_indices) and convert the data.
```

### Comparing `f4-0.5.2/src/f4/Parser.py` & `f4-0.5.3/src/f4/Parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,19 +336,20 @@
     def __init__(self, column_name, lower_bound_value, upper_bound_value):
         filter1 = StringFilter(column_name, ge, lower_bound_value)
         filter2 = StringFilter(column_name, le, upper_bound_value)
 
         super().__init__(filter1, filter2)
 
 class FileData:
-    def __init__(self, data_file_path, file_handle, file_map_dict, stat_dict, decompression_type, decompressor):
+    def __init__(self, data_file_path, file_handle, file_map_dict, stat_dict, version, decompression_type, decompressor):
         self.data_file_path = data_file_path
         self.file_handle = file_handle
         self.file_map_dict = file_map_dict
         self.stat_dict = stat_dict
+        self.version = version
         self.decompression_type = decompression_type
         self.decompressor = decompressor
 
 #####################################################
 # Public function(s)
 #####################################################
 
@@ -490,14 +491,18 @@
 
 def tail(data_file_path, n = 10, select_columns=None, out_file_path=None, out_file_type="tsv"):
     if not select_columns:
         select_columns = []
 
     query(data_file_path, TailFilter(n, select_columns), select_columns, out_file_path=out_file_path, out_file_type=out_file_type)
 
+def get_version(data_file_path):
+    with initialize(data_file_path) as file_data:
+        return file_data.version.decode()
+
 def get_num_rows(data_file_path):
     with initialize(data_file_path) as file_data:
         return file_data.stat_dict["num_rows"]
 
 def get_num_cols(data_file_path):
     with initialize(data_file_path) as file_data:
         return file_data.stat_dict["num_cols"]
@@ -562,15 +567,15 @@
 
                 data_size = file_map_dict2["data"][1] - file_map_dict2["data"][0]
                 stat_dict["num_rows"] = fast_int(data_size / stat_dict["ll"])
 
             cc_size = file_map_dict2["cc"][1] - file_map_dict2["cc"][0]
             stat_dict["num_cols"] = fast_int(cc_size / stat_dict["mccl"]) - 1
 
-            yield FileData(data_file_path, mmap_handle, file_map_dict2, stat_dict, decompression_type, decompressor)
+            yield FileData(data_file_path, mmap_handle, file_map_dict2, stat_dict, other_dict["ver"], decompression_type, decompressor)
 
             mmap_handle.close()
             file_handle.close()
 
 def get_column_index_from_name(file_data, column_name):
     position = get_identifier_row_index(file_data, column_name.encode(), file_data.stat_dict["num_cols"], data_prefix="cn")
```

### Comparing `f4-0.5.2/src/f4/Utilities.py` & `f4-0.5.3/src/f4/Utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,22 @@
 from shutil import rmtree
 import sys
 from tempfile import mkdtemp
 from zstandard import ZstdCompressor, ZstdDecompressor
 
 # We use these dictionaries so that when we store the file map, it takes less space on disk.
 FILE_KEY_ABBREVIATIONS_STATS = {"mccl": 3, "mctl": 6, "cnmccl": 10, "cnll": 11}
-FILE_KEY_ABBREVIATIONS_OTHER = {"ll": 4, "cmpr": 7}
+FILE_KEY_ABBREVIATIONS_OTHER = {"ll": 4, "cmpr": 7, "ver": 12}
 FILE_KEY_ABBREVIATIONS_NOCACHE = {"data": 1, "cc": 2, "ct": 5, "cndata": 8, "cncc": 9}
 
 def get_current_version():
-    return "0.5.2"
+    return "0.5.3"
+
+def get_current_version_major():
+    return get_current_version().split(".")[0]
 
 def read_str_from_file(file_path, file_extension=""):
     with open(file_path + file_extension, 'rb') as the_file:
         return the_file.read()
 
 def write_str_to_file(file_path, the_string):
     with open(file_path, 'wb') as the_file:
```

### Comparing `f4-0.5.2/src/f4.egg-info/PKG-INFO` & `f4-0.5.3/src/f4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.5.2
+Version: 0.5.3
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.5.2/test/test.py` & `f4-0.5.3/test/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 
     try:
         f4.query("bogus_file_path")
         fail_test("Invalid file path.")
     except:
         pass_test("Invalid file path.")
 
+    check_result("Version", "Version number - major", f4.get_version(f4_file_path), "0")
     check_result("Dimensions", "Number of rows", f4.get_num_rows(f4_file_path), 5)
     check_result("Dimensions", "Number of columns", f4.get_num_cols(f4_file_path), 9)
 
     check_result("Column types", "ID column", f4.get_column_type_from_name(f4_file_path, "ID"), "s")
     check_result("Column types", "FloatA column", f4.get_column_type_from_name(f4_file_path, "FloatA"), "f")
     check_result("Column types", "FloatB column", f4.get_column_type_from_name(f4_file_path, "FloatB"), "f")
     check_result("Column types", "OrdinalA column", f4.get_column_type_from_name(f4_file_path, "OrdinalA"), "s")
```

