# Comparing `tmp/keyvalues3-0.1a1.tar.gz` & `tmp/keyvalues3-0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyvalues3-0.1a1.tar", last modified: Wed Mar 22 15:29:58 2023, max compression
+gzip compressed data, was "keyvalues3-0.1a2.tar", last modified: Fri Apr 21 14:42:48 2023, max compression
```

## Comparing `keyvalues3-0.1a1.tar` & `keyvalues3-0.1a2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0      879 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1141 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/.github/workflows/test.yml
--rw-r--r--   0        0        0        7 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/.gitignore
--rw-r--r--   0        0        0     1066 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/LICENSE
--rw-r--r--   0        0        0     1424 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/README.md
--rw-r--r--   0        0        0     2872 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/keyvalues3/__init__.py
--rw-r--r--   0        0        0     5450 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/keyvalues3/binarywriter.py
--rw-r--r--   0        0        0     4550 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/keyvalues3/keyvalues3.py
--rw-r--r--   0        0        0     1372 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/keyvalues3/kv3file.py
--rw-r--r--   0        0        0     7253 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/keyvalues3/textreader.py
--rw-r--r--   0        0        0     2891 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/keyvalues3/textwriter.py
--rw-r--r--   0        0        0      533 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/__init__.py
--rw-r--r--   0        0        0      354 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/documents/arrays.kv3
--rw-r--r--   0        0        0      406 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/documents/binary/example.kv3
--rw-r--r--   0        0        0      356 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/documents/binary/example_lz4.kv3
--rw-r--r--   0        0        0    53884 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/documents/binary/lightmap_query_data.kv3
--rw-r--r--   0        0        0    20858 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/documents/bt_config.kv3
--rw-r--r--   0        0        0      371 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/documents/byte_arrays.kv3
--rw-r--r--   0        0        0      782 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/documents/example.kv3
--rw-r--r--   0        0        0       20 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/documents/example_noheader.kv3
--rw-r--r--   0        0        0       37 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/documents/not_kv3.kv3
--rw-r--r--   0        0        0      915 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/documents/numbers.kv3
--rw-r--r--   0        0        0      449 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/documents/objects.kv3
--rw-r--r--   0        0        0     1023 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/documents/strings.kv3
--rw-r--r--   0        0        0      158 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/documents/weird_header_whitespace.kv3
--rw-r--r--   0        0        0      669 2023-03-22 15:29:50.614755 keyvalues3-0.1a1/tests/stresstest.py
--rw-r--r--   0        0        0     1736 2023-03-22 15:29:50.618755 keyvalues3-0.1a1/tests/test_api.py
--rw-r--r--   0        0        0     2159 2023-03-22 15:29:50.618755 keyvalues3-0.1a1/tests/test_binarywriter.py
--rw-r--r--   0        0        0     4392 2023-03-22 15:29:50.618755 keyvalues3-0.1a1/tests/test_kv3file.py
--rw-r--r--   0        0        0      637 2023-03-22 15:29:50.618755 keyvalues3-0.1a1/tests/test_repr.py
--rw-r--r--   0        0        0     8072 2023-03-22 15:29:50.618755 keyvalues3-0.1a1/tests/test_textreader.py
--rw-r--r--   0        0        0     3024 2023-03-22 15:29:50.618755 keyvalues3-0.1a1/tests/test_textwriter.py
--rw-r--r--   0        0        0     1884 1970-01-01 00:00:00.000000 keyvalues3-0.1a1/PKG-INFO
+-rw-r--r--   0        0        0      879 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1141 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/.github/workflows/test.yml
+-rw-r--r--   0        0        0        7 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/.gitignore
+-rw-r--r--   0        0        0     1066 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/LICENSE
+-rw-r--r--   0        0        0     1608 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/README.md
+-rw-r--r--   0        0        0     4366 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/keyvalues3/__init__.py
+-rw-r--r--   0        0        0     5450 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/keyvalues3/binarywriter.py
+-rw-r--r--   0        0        0     4620 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/keyvalues3/keyvalues3.py
+-rw-r--r--   0        0        0     2614 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/keyvalues3/kv3file.py
+-rw-r--r--   0        0        0     7253 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/keyvalues3/textreader.py
+-rw-r--r--   0        0        0     2891 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/keyvalues3/textwriter.py
+-rw-r--r--   0        0        0      533 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/tests/__init__.py
+-rw-r--r--   0        0        0      354 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/tests/documents/arrays.kv3
+-rw-r--r--   0        0        0      406 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/tests/documents/binary/example.kv3
+-rw-r--r--   0        0        0      356 2023-04-21 14:42:41.279458 keyvalues3-0.1a2/tests/documents/binary/example_lz4.kv3
+-rw-r--r--   0        0        0    53884 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/documents/binary/lightmap_query_data.kv3
+-rw-r--r--   0        0        0    20858 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/documents/bt_config.kv3
+-rw-r--r--   0        0        0      371 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/documents/byte_arrays.kv3
+-rw-r--r--   0        0        0      782 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/documents/example.kv3
+-rw-r--r--   0        0        0       20 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/documents/example_noheader.kv3
+-rw-r--r--   0        0        0       37 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/documents/not_kv3.kv3
+-rw-r--r--   0        0        0      915 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/documents/numbers.kv3
+-rw-r--r--   0        0        0      449 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/documents/objects.kv3
+-rw-r--r--   0        0        0     1598 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/documents/slick_jaguar_white.vcompmat
+-rw-r--r--   0        0        0     1023 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/documents/strings.kv3
+-rw-r--r--   0        0        0      158 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/documents/weird_header_whitespace.kv3
+-rw-r--r--   0        0        0      778 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/stresstest.py
+-rw-r--r--   0        0        0     2726 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/test_api.py
+-rw-r--r--   0        0        0     2159 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/test_binarywriter.py
+-rw-r--r--   0        0        0     7396 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/test_kv3file.py
+-rw-r--r--   0        0        0      637 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/test_repr.py
+-rw-r--r--   0        0        0     8166 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/test_textreader.py
+-rw-r--r--   0        0        0     3024 2023-04-21 14:42:41.283458 keyvalues3-0.1a2/tests/test_textwriter.py
+-rw-r--r--   0        0        0     2068 1970-01-01 00:00:00.000000 keyvalues3-0.1a2/PKG-INFO
```

### Comparing `keyvalues3-0.1a1/.github/workflows/release.yml` & `keyvalues3-0.1a2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/.github/workflows/test.yml` & `keyvalues3-0.1a2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/LICENSE` & `keyvalues3-0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/README.md` & `keyvalues3-0.1a2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 ## keyvalues3
 KeyValues3 is a Valve developed data format. It is similar in structure to JSON, but supports binary encodings, versioning, and data annotations. The text syntax also has some minor ergonomic improvements (support for single- and multi-line comments, trailing commas, and multi-line strings.)
 
 ## Usage
 ```py
 import keyvalues3 as kv3
-file = kv3.read("tests/documents/bt_config.kv3")
-```
-```py
->>> file.value.keys()
+bt_config = kv3.read("tests/documents/bt_config.kv3")
+
+>>> bt_config.keys()
 dict_keys(['default', 'low', 'fair', 'normal', 'tough', 'hard', 'very_hard', 'expert', 'elite'])
-```
 
-```py
->>> file.value["elite"]["reaction_time"]
+>>> bt_config["elite"]["reaction_time"]
 0.12
 ```
+
 ```py
->>> type(file.value)
+# The root value is most of the time a dict
+>>> type(bt_config.value)
 <class 'dict'>
 
->>> file.original_encoding
+>>> bt_config.original_encoding
 Encoding(name='text', version=UUID('e21c7f3c-8a33-41c5-9977-a76d3a32aa0d'))
 
->>> file.format
+>>> bt_config.format
 Format(name='generic', version=UUID('7412167c-06e9-4698-aff2-e63eb59037e7'))
+
+# To write it back
+>>> kv3.write(bt_config, "tests/documents/bt_config.kv3", use_original_encoding=True)
 ```
 
 ## Install
-
+```bash
+pip install keyvalues3
+```
 
 ## Supported encodings
 | Encoding 👩‍💻 | Read 📖 | Write ✍️ |
 | ----------- | :-----: | :-------: |
 | Text UTF-8 | Yes ✔️ | Yes ✔️ |
 | Text UTF-8 Headerless | Yes ✔️ | Yes ✔️ |
 | Binary Uncompressed | No ⛔ | Yes ✔️ |
```

### Comparing `keyvalues3-0.1a1/keyvalues3/__init__.py` & `keyvalues3-0.1a2/keyvalues3/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,45 +5,47 @@
 import os, io, typing
 from .keyvalues3 import *
 from .kv3file import KV3File
 from .binarywriter import BinaryMagics
 from .textreader import KV3TextReader
 from . import textwriter
 
-__version__ = "0.1a1"
+__version__ = "0.1a2"
 __all__ = [ "read", "write" ]
 
+#region: read
+
 @typing.overload
 def read(text_stream: typing.TextIO) -> KV3File:
     """Read a text KV3 stream."""
 
 @typing.overload
 def read(binary_stream: typing.BinaryIO) -> KV3File:
     """Read a binary KV3 stream."""
 
 @typing.overload
 def read(path: str | os.PathLike) -> KV3File:
     """
     Read a text or binary KV3 file from a path.
-    
+
     If a binary magic is present, read in binary mode, otherwise text.
 
     Raises:
         KV3DecodeError: Error decoding in any of the modes.
     """
 
 def read(path_or_stream: str | os.PathLike | typing.IO) -> KV3File:
 
     def read_binary(binary_stream: typing.BinaryIO):
         magic = binary_stream.read(4)
         binary_stream.seek(0)
 
         if not BinaryMagics.is_defined(magic):
             raise InvalidKV3Magic("Invalid binary KV3 magic: " + repr(magic))
-    
+
         if magic != BinaryMagics.VKV3:
             raise NotImplementedError("Unsupported binary KV3 magic: " + repr(magic))
 
         return KV3File({"binary": "reader", "todo": "implement"}, original_encoding=ENCODING_BINARY_UNCOMPRESSED)
 
     def read_text(text_stream: typing.TextIO):
         return KV3TextReader().parse(text_stream.read())
@@ -56,28 +58,76 @@
     with open(path_or_stream, "rb") as fp:
         try:
             rv = read_binary(fp)
         except InvalidKV3Magic as not_binary_error:
             try:
                 rv = read_text(io.TextIOWrapper(fp, encoding="utf-8"))
             except KV3DecodeError as text_error:
-                text_for_sure = "<!--" in (text_err_str:=str(not_binary_error))
+                text_for_sure = "<!--" in (binary_err_str:=str(not_binary_error))
                 if (text_for_sure):
                     raise text_error
                 raise KV3DecodeError(
-                    "Failed to read KV3 file in both text and binary modes." +
-                    f"\n\tBinary: {not_binary_error}" +
-                    f"\n\tText: " + text_err_str
+                    "Failed to read KV3 file in text mode (binary magic didn't even match). " + str(text_error)
                 ) from text_error
         return rv
 
-def write(kv3: KV3File | ValueType, path: str | os.PathLike, encoding: Encoding = ENCODING_TEXT, format: Format = FORMAT_GENERIC):
-    raise NotImplementedError()
+#endregion
+
+#region: write
+
+def write(kv3: KV3File | ValueType, path_or_stream: str | os.PathLike | typing.IO, encoding: Encoding = ENCODING_TEXT, *,
+          format: Format = FORMAT_GENERIC,
+          use_original_encoding: bool = False
+    ):
+    """
+    Write a KV3File to a file or stream.
+
+    Args:
+        kv3: The KV3File or KV3 value to write.
+        path_or_stream: The file path to write to. Or a text/binary stream.
+        encoding: The encoding to use.
+
+        format: If a raw kv3 value is passed, this is the format to build it with. Default is 'generic'.
+        use_original_encoding: If a kv3 file is passed, use its original encoding.
+    """
+
     if not isinstance(kv3, KV3File):
         kv3 = KV3File(kv3, format=format, validate_value=True)
 
+    if use_original_encoding:
+        encoding = kv3file.original_encoding
+        if encoding is None:
+            raise ValueError("Cannot use original encoding if provided kv3 doesn't have one.")
+
+    # TODO: clean this up with a context manager
+    fp = None
+    is_file = False
+
+    match path_or_stream:
+        case io.IOBase():
+            fp = path_or_stream
+        case str():
+            fp = open(path_or_stream, "wb")
+            is_file = True
+        case _:
+            raise TypeError("Argument path_or_stream must be a path or stream")
+
     if encoding == ENCODING_TEXT:
-        textwriter.encode(kv3)
-    elif encoding == ENCODING_BINARY_UNCOMPRESSED:
-       binarywriter.BinaryV1UncompressedWriter(kv3).write(None)
-    elif encoding == ENCODING_BINARY_BLOCK_LZ4:
-        binarywriter.BinaryLZ4(kv3).write(None)
+        text_result = textwriter.encode(kv3)
+        if isinstance(fp, io.TextIOBase):
+            fp.write(text_result)
+        else:
+            fp.write(text_result.encode("utf-8"))
+    else:
+        if isinstance(fp, io.TextIOBase):
+            raise TypeError("Cannot write binary KV3 to a text stream. If this is a file, please open it in binary mode ('wb').")
+        if encoding == ENCODING_BINARY_UNCOMPRESSED:
+            binarywriter.BinaryV1UncompressedWriter(kv3).write(fp)
+        elif encoding == ENCODING_BINARY_BLOCK_LZ4:
+            binarywriter.BinaryLZ4(kv3).write(fp)
+        else:
+            raise NotImplementedError(f"Encoding type {encoding} not implemented.")
+    
+    if is_file:
+        fp.close()
+
+#endregion
```

### Comparing `keyvalues3-0.1a1/keyvalues3/binarywriter.py` & `keyvalues3-0.1a2/keyvalues3/binarywriter.py`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/keyvalues3/keyvalues3.py` & `keyvalues3-0.1a2/keyvalues3/keyvalues3.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,17 +67,17 @@
                     raise ValueError("list contains itself")
                 check_valid(nested_value)
         case dict():
             for key, nested_value in value.items():
                 if nested_value is value:
                     raise ValueError("dict contains itself")
                 if not isinstance(key, str):
-                    raise ValueError("dict key is not a string")
+                    raise ValueError(f"dict key is not a string type, but {type(key)}")
                 if not key.isidentifier():
-                    raise ValueError("dict key is not a valid identifier") # I think
+                    raise ValueError(f"dict key '{key}' is not accepted (not a valid identifier)") # TODO: spaces and . are allowed
                 check_valid(nested_value)
         case array.array() | bytes() | bytearray():
             pass
         case _:
             raise TypeError(f"Invalid type {type(value)} for KV3 value.")
 
 def is_valid(value: ValueType) -> bool:
```

### Comparing `keyvalues3-0.1a1/keyvalues3/textreader.py` & `keyvalues3-0.1a2/keyvalues3/textreader.py`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/keyvalues3/textwriter.py` & `keyvalues3-0.1a2/keyvalues3/textwriter.py`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/pyproject.toml` & `keyvalues3-0.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/tests/documents/binary/lightmap_query_data.kv3` & `keyvalues3-0.1a2/tests/documents/binary/lightmap_query_data.kv3`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/tests/documents/bt_config.kv3` & `keyvalues3-0.1a2/tests/documents/bt_config.kv3`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/tests/documents/example.kv3` & `keyvalues3-0.1a2/tests/documents/example.kv3`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/tests/documents/numbers.kv3` & `keyvalues3-0.1a2/tests/documents/numbers.kv3`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/tests/documents/strings.kv3` & `keyvalues3-0.1a2/tests/documents/strings.kv3`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/tests/stresstest.py` & `keyvalues3-0.1a2/tests/stresstest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """
 Test parser against Dota 2 Particles.
 
+On hot runs:
+    Ran through 100 files in 2.6 seconds
+    Ran through 1000 files in 27 seconds
+
 Run with:
     python -m pytest tests/stresstest.py -s
 """
 
 from pathlib import Path
 
 # dota 2 path
 dota2_path =  Path(r'D:\Games\steamapps\common\dota 2 beta')
-CAP = 100
+MAX_FILES = 100
 
 import keyvalues3
 import time
 
 start = time.time()
 count = 0
 def finish(count: int):
     print(f"Ran through {count} files in", time.time() - start, "seconds")
 
 for vpcf in (dota2_path / "content").glob("**/*.vpcf"):
-    if count > CAP:
+    if count >= MAX_FILES:
         break
     try:
         kv = keyvalues3.read(vpcf)
     except (keyvalues3.KV3DecodeError, KeyboardInterrupt):
         print(vpcf)
         finish(count)
         raise
```

### Comparing `keyvalues3-0.1a1/tests/test_api.py` & `keyvalues3-0.1a2/tests/test_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 
 def verify_example(text_kv3: keyvalues3.KV3File):
     assert text_kv3.original_encoding == keyvalues3.ENCODING_TEXT
     assert text_kv3.format == keyvalues3.FORMAT_GENERIC
     assert isinstance(text_kv3.value, dict)
     assert text_kv3.value["boolValue"] == False
 
+    # dict proxy
+    assert text_kv3["boolValue"] == False
+
 def test_api_read_from_path():
     text_kv3 = keyvalues3.read("tests/documents/example.kv3")
     verify_example(text_kv3)
 
-    with pytest.raises(keyvalues3.KV3DecodeError, match="Failed to read KV3 file in both text and binary modes."):
+    with pytest.raises(keyvalues3.KV3DecodeError, match="Failed to read KV3 file in text mode."):
         keyvalues3.read("tests/documents/not_kv3.kv3")
 
 def test_api_read_from_stream():
     with open("tests/documents/example.kv3") as fp:
         text_kv3 = keyvalues3.read(fp)
         verify_example(text_kv3)
     
@@ -33,12 +36,39 @@
     assert isinstance(binary_kv3.value, dict)
     assert binary_kv3.value["binary"] == "reader"
 
     binary_kv3 = keyvalues3.read("tests/documents/binary/example_lz4.kv3")
     assert isinstance(binary_kv3.value, dict)
     assert binary_kv3.value["binary"] == "reader"
 
-    with pytest.raises(NotImplementedError):
+    # good magic, but not implemented
+    with pytest.raises(NotImplementedError, match="Unsupported binary KV3 magic"):
         keyvalues3.read("tests/documents/binary/lightmap_query_data.kv3")
 
+    # a bad magic
     with pytest.raises(keyvalues3.InvalidKV3Magic, match="Invalid binary KV3 magic: b'VDF3'"):
         keyvalues3.read(io.BytesIO(b"VDF3\x01\x03\x03\x07"))
+
+
+def test_api_write():
+    my_object = {
+        "_class": "HelloWorld",
+    }
+
+    with io.BytesIO() as my_stream:
+        keyvalues3.write(my_object, my_stream)
+
+    with io.StringIO() as my_stream:
+        keyvalues3.write(my_object, my_stream)
+
+    import tempfile
+    with tempfile.TemporaryFile("w") as fp: keyvalues3.write(my_object, getattr(fp, "file", fp))
+    with tempfile.TemporaryFile("wb") as fp: keyvalues3.write(my_object, getattr(fp, "file", fp))
+
+    null_VKV = b'VKV\x03\x00\x05\x86\x1b\xd8\xf7\xc1@\xad\x82u\xa4\x82g\xe7\x14|\x16\x12t\xe9\x06\x98F\xaf\xf2\xe6>\xb5\x907\xe7\x00\x00\x00\x00\x01\xFF\xFF\xFF\xFF'
+    with io.BytesIO(null_VKV) as my_stream:
+        keyvalues3.write(
+            None,
+            my_stream,
+            keyvalues3.ENCODING_BINARY_UNCOMPRESSED
+        )
+        assert my_stream.getvalue() == null_VKV
```

### Comparing `keyvalues3-0.1a1/tests/test_binarywriter.py` & `keyvalues3-0.1a2/tests/test_binarywriter.py`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/tests/test_kv3file.py` & `keyvalues3-0.1a2/tests/test_kv3file.py`

 * *Files 26% similar despite different names*

```diff
@@ -88,7 +88,73 @@
         textwriter.encode(KV3File(value=flagged_value(str(), Flag.multilinestring)))
         textwriter.encode(KV3File(value=flagged_value(str(), Flag.resource)))
         textwriter.encode(KV3File(value=[]))
         textwriter.encode(KV3File(value={}))
         textwriter.encode(KV3File(value=self.MyKV3Format(), format=self.MyKV3Format.format))
         textwriter.encode(KV3File(value=bytes(byte for byte in range(256))))
         textwriter.encode(KV3File(value=bytearray(byte for byte in range(256))))
+
+    def test_json_dump(self):
+        import json
+        my_kv = KV3File(value={'_class': 'CCompositeMaterialEditorDoc', 'key': 'value'})
+
+        # passes
+        json.dumps(my_kv.value)
+
+        # fails (is not JSON serializable)
+        with self.assertRaises(TypeError): json.dumps(my_kv)
+
+    def test_dict_proxy(self):
+        usual_kv3 = KV3File(value={'_class': 'CParticleSystemDefinition', 'b': 2, 'c': 3})
+        list_based_kv3 = KV3File(value=["a", "b", "c"])
+        leet_kv3 = KV3File(value=1337)
+
+        self.assertEqual(usual_kv3['_class'], "CParticleSystemDefinition")
+
+        self.assertSetEqual(set(usual_kv3.keys()), {'_class', 'b', 'c'})
+        self.assertSetEqual(set(usual_kv3.values()), {'CParticleSystemDefinition', 2, 3})
+
+        self.assertEqual(repr([*usual_kv3.keys()]), "['_class', 'b', 'c']")
+        self.assertEqual(repr([*usual_kv3.values()]), "['CParticleSystemDefinition', 2, 3]")
+
+        self.assertEqual(repr(usual_kv3.keys()), "dict_keys(['_class', 'b', 'c'])")
+        self.assertEqual(repr(usual_kv3.values()), "dict_values(['CParticleSystemDefinition', 2, 3])")
+
+        with self.assertRaises(TypeError) as exception: list_based_kv3['a']
+        with self.assertRaises(TypeError) as exception: list_based_kv3[1]
+        with self.assertRaises(TypeError) as exception: list_based_kv3.keys()
+
+        self.assertTrue("KV3 root value is of type 'list'" in str(exception.exception))
+    
+        with self.assertRaises(TypeError) as exception: reversed(usual_kv3)
+        with self.assertRaises(TypeError) as exception: reversed(list_based_kv3)
+
+        null_kv3 = KV3File()
+        with self.assertRaises(TypeError): null_kv3["my"] = "value"
+        with self.assertRaises(TypeError): null_kv3["my"]
+        with self.assertRaises(TypeError): del null_kv3["my"]
+        with self.assertRaises(TypeError): len(null_kv3)
+        with self.assertRaises(TypeError): iter(null_kv3)
+
+        class PMResult(enum.Enum):
+            PARTICLE_SYSTEM = enum.auto()
+            LIST_BASED = enum.auto()
+            LEET = enum.auto()
+            NULL = enum.auto()
+            ANY_OTHER = enum.auto()
+            NONE = enum.auto()
+
+        def pattern_match(v) -> PMResult:
+            match v:
+                case KV3File(value={ '_class': 'CParticleSystemDefinition'}): return PMResult.PARTICLE_SYSTEM
+                case KV3File(value=list()): return PMResult.LIST_BASED
+                case KV3File(value=None): return PMResult.NULL
+                case KV3File(value=1337): return PMResult.LEET
+                case KV3File(): return PMResult.ANY_OTHER
+                case _: return PMResult.NONE
+
+        self.assertEqual(pattern_match(usual_kv3), PMResult.PARTICLE_SYSTEM)
+        self.assertEqual(pattern_match(list_based_kv3), PMResult.LIST_BASED)
+        self.assertEqual(pattern_match(leet_kv3), PMResult.LEET)
+        self.assertEqual(pattern_match(null_kv3), PMResult.NULL)
+
+        self.assertEqual(pattern_match(KV3File("asd")), PMResult.ANY_OTHER)
```

### Comparing `keyvalues3-0.1a1/tests/test_repr.py` & `keyvalues3-0.1a2/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/tests/test_textreader.py` & `keyvalues3-0.1a2/tests/test_textreader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+import itertools
 
 import keyvalues3 as kv3
 from keyvalues3.textreader import KV3TextReader, KV3TextReaderNoHeader, kv3grammar
 import keyvalues3.textwriter as kv3textwriter
 
 default_header = "<!-- kv3 encoding:text:version{e21c7f3c-8a33-41c5-9977-a76d3a32aa0d} format:generic:version{7412167c-06e9-4698-aff2-e63eb59037e7} -->\n"
 
@@ -137,15 +138,20 @@
         vpfc_files.clear()
         shutil.rmtree(workdir, ignore_errors=True)
         shutil.rmtree(gamedir, ignore_errors=True)
 
 kv3_files = []
 vpfc_files = []
 
-for kv3file in Path("tests/documents").glob('*.kv3'):
+docs = Path("tests/documents")
+
+for kv3file in itertools.chain(
+        docs.glob('*.kv3'),
+        docs.glob('*.vcompmat')
+    ):
     assumed_valid = kv3file.stem != "not_kv3"
     no_header = "noheader" in kv3file.stem
     parameters = (assumed_valid, no_header)
     
     kv3_files.append((kv3file, *parameters))
     if resourcecompiler.is_file():
         vpcf_to_compile = (workdir / kv3file.name).with_suffix('.vpcf')
```

### Comparing `keyvalues3-0.1a1/tests/test_textwriter.py` & `keyvalues3-0.1a2/tests/test_textwriter.py`

 * *Files identical despite different names*

### Comparing `keyvalues3-0.1a1/PKG-INFO` & `keyvalues3-0.1a2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyvalues3
-Version: 0.1a1
+Version: 0.1a2
 Summary: Read and write Valve's KeyValues3 format
 Keywords: parser,kv3,keyvalues,keyvalues3,valve
 Author-email: kristiker <kristik06@outlook.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: parsimonious >=0.10,<1.0
 Requires-Dist: lz4 >=4.3.2,<5.0
@@ -14,38 +14,42 @@
 
 ## keyvalues3
 KeyValues3 is a Valve developed data format. It is similar in structure to JSON, but supports binary encodings, versioning, and data annotations. The text syntax also has some minor ergonomic improvements (support for single- and multi-line comments, trailing commas, and multi-line strings.)
 
 ## Usage
 ```py
 import keyvalues3 as kv3
-file = kv3.read("tests/documents/bt_config.kv3")
-```
-```py
->>> file.value.keys()
+bt_config = kv3.read("tests/documents/bt_config.kv3")
+
+>>> bt_config.keys()
 dict_keys(['default', 'low', 'fair', 'normal', 'tough', 'hard', 'very_hard', 'expert', 'elite'])
-```
 
-```py
->>> file.value["elite"]["reaction_time"]
+>>> bt_config["elite"]["reaction_time"]
 0.12
 ```
+
 ```py
->>> type(file.value)
+# The root value is most of the time a dict
+>>> type(bt_config.value)
 <class 'dict'>
 
->>> file.original_encoding
+>>> bt_config.original_encoding
 Encoding(name='text', version=UUID('e21c7f3c-8a33-41c5-9977-a76d3a32aa0d'))
 
->>> file.format
+>>> bt_config.format
 Format(name='generic', version=UUID('7412167c-06e9-4698-aff2-e63eb59037e7'))
+
+# To write it back
+>>> kv3.write(bt_config, "tests/documents/bt_config.kv3", use_original_encoding=True)
 ```
 
 ## Install
-
+```bash
+pip install keyvalues3
+```
 
 ## Supported encodings
 | Encoding 👩‍💻 | Read 📖 | Write ✍️ |
 | ----------- | :-----: | :-------: |
 | Text UTF-8 | Yes ✔️ | Yes ✔️ |
 | Text UTF-8 Headerless | Yes ✔️ | Yes ✔️ |
 | Binary Uncompressed | No ⛔ | Yes ✔️ |
```

