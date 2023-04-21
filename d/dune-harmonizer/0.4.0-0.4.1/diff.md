# Comparing `tmp/dune_harmonizer-0.4.0.tar.gz` & `tmp/dune_harmonizer-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_harmonizer-0.4.0.tar", max compression
+gzip compressed data, was "dune_harmonizer-0.4.1.tar", max compression
```

## Comparing `dune_harmonizer-0.4.0.tar` & `dune_harmonizer-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1061 2023-04-20 10:36:09.577470 dune_harmonizer-0.4.0/LICENSE
--rw-r--r--   0        0        0     2378 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/README.md
--rw-r--r--   0        0        0      440 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/dune/harmonizer/__init__.py
--rw-r--r--   0        0        0      849 2023-04-20 10:36:30.181023 dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    19835 2023-04-20 10:36:30.365021 dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc
--rw-r--r--   0        0        0      630 2023-04-20 10:36:30.365021 dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc
--rw-r--r--   0        0        0     3103 2023-04-20 10:36:30.365021 dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc
--rw-r--r--   0        0        0     3528 2023-04-20 10:36:30.181023 dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/translate.cpython-311.pyc
--rw-r--r--   0        0        0       54 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/dune/harmonizer/constants.py
--rw-r--r--   0        0        0    17211 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/dune/harmonizer/custom_transforms.py
--rw-r--r--   0        0        0      105 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/dune/harmonizer/errors.py
--rw-r--r--   0        0        0     2018 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/dune/harmonizer/table_replacements.py
--rw-r--r--   0        0        0     2914 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/dune/harmonizer/translate.py
--rw-r--r--   0        0        0      570 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2714 1970-01-01 00:00:00.000000 dune_harmonizer-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-20 13:51:20.550154 dune_harmonizer-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2378 2023-04-20 13:51:20.550154 dune_harmonizer-0.4.1/README.md
+-rw-r--r--   0        0        0      440 2023-04-20 13:51:20.550154 dune_harmonizer-0.4.1/dune/harmonizer/__init__.py
+-rw-r--r--   0        0        0      849 2023-04-20 13:51:41.386157 dune_harmonizer-0.4.1/dune/harmonizer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    19435 2023-04-20 13:51:41.574157 dune_harmonizer-0.4.1/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc
+-rw-r--r--   0        0        0      630 2023-04-20 13:51:41.574157 dune_harmonizer-0.4.1/dune/harmonizer/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0     3103 2023-04-20 13:51:41.574157 dune_harmonizer-0.4.1/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc
+-rw-r--r--   0        0        0     3449 2023-04-20 13:51:41.386157 dune_harmonizer-0.4.1/dune/harmonizer/__pycache__/translate.cpython-311.pyc
+-rw-r--r--   0        0        0       54 2023-04-20 13:51:20.550154 dune_harmonizer-0.4.1/dune/harmonizer/constants.py
+-rw-r--r--   0        0        0    16901 2023-04-20 13:51:20.554154 dune_harmonizer-0.4.1/dune/harmonizer/custom_transforms.py
+-rw-r--r--   0        0        0      105 2023-04-20 13:51:20.554154 dune_harmonizer-0.4.1/dune/harmonizer/errors.py
+-rw-r--r--   0        0        0     2018 2023-04-20 13:51:20.554154 dune_harmonizer-0.4.1/dune/harmonizer/table_replacements.py
+-rw-r--r--   0        0        0     2863 2023-04-20 13:51:20.554154 dune_harmonizer-0.4.1/dune/harmonizer/translate.py
+-rw-r--r--   0        0        0      570 2023-04-20 13:51:20.554154 dune_harmonizer-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2714 1970-01-01 00:00:00.000000 dune_harmonizer-0.4.1/PKG-INFO
```

### Comparing `dune_harmonizer-0.4.0/LICENSE` & `dune_harmonizer-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.4.0/README.md` & `dune_harmonizer-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc` & `dune_harmonizer-0.4.1/dune/harmonizer/__pycache__/__init__.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x99154164 (Thu Apr 20 10:36:09 2023 UTC)
+moddate:  0x58434164 (Thu Apr 20 13:51:20 2023 UTC)
 files sz: 440
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc` & `dune_harmonizer-0.4.1/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x99154164 (Thu Apr 20 10:36:09 2023 UTC)
-files sz: 17211
+moddate:  0x58434164 (Thu Apr 20 13:51:20 2023 UTC)
+files sz: 16901
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064016c035a
@@ -14,15 +14,15 @@
       0aac08a6020000ab0200000000000000005a0b020065026508640bac08a6
       020000ab0200000000000000005a0c020065026508640cac08a6020000ab
       0200000000000000005a0d640d84005a0e640e5a0f640f5a106410650f9b
       009d025a1165109b0064109d025a126411650f9b009d025a1365109b0064
       119d025a14641284005a15641384005a16641484005a17641584005a1864
       1684005a19641784005a1a641884005a1b641984005a1c641a84005a1d64
       1b84005a1e641c84005a1f641d84005a20641e84005a21641f84005a2264
-      2084005a23642184005a24642284005a25642384005a2664015300
+      2084005a23642184005a24642284005a2564015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (re)
                  8 STORE_NAME               0 (re)
    
@@ -156,63 +156,59 @@
                270 MAKE_FUNCTION            0
                272 STORE_NAME              25 (warn_unnest)
    
    269         274 LOAD_CONST              23 (<code object warn_sequence, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 269>)
                276 MAKE_FUNCTION            0
                278 STORE_NAME              26 (warn_sequence)
    
-   283         280 LOAD_CONST              24 (<code object prep_query, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 283>)
+   283         280 LOAD_CONST              24 (<code object rename_amount_column, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 283>)
                282 MAKE_FUNCTION            0
-               284 STORE_NAME              27 (prep_query)
+               284 STORE_NAME              27 (rename_amount_column)
    
-   295         286 LOAD_CONST              25 (<code object rename_amount_column, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 295>)
+   288         286 LOAD_CONST              25 (<code object bytea2numeric, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 288>)
                288 MAKE_FUNCTION            0
-               290 STORE_NAME              28 (rename_amount_column)
+               290 STORE_NAME              28 (bytea2numeric)
    
-   300         292 LOAD_CONST              26 (<code object bytea2numeric, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 300>)
+   302         292 LOAD_CONST              26 (<code object fix_bytearray_param, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 302>)
                294 MAKE_FUNCTION            0
-               296 STORE_NAME              29 (bytea2numeric)
+               296 STORE_NAME              29 (fix_bytearray_param)
    
-   314         298 LOAD_CONST              27 (<code object fix_bytearray_param, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 314>)
+   308         298 LOAD_CONST              27 (<code object fix_bytearray_lower, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 308>)
                300 MAKE_FUNCTION            0
-               302 STORE_NAME              30 (fix_bytearray_param)
+               302 STORE_NAME              30 (fix_bytearray_lower)
    
-   320         304 LOAD_CONST              28 (<code object fix_bytearray_lower, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 320>)
+   317         304 LOAD_CONST              28 (<code object chain_where, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 317>)
                306 MAKE_FUNCTION            0
-               308 STORE_NAME              31 (fix_bytearray_lower)
+               308 STORE_NAME              31 (chain_where)
    
-   329         310 LOAD_CONST              29 (<code object chain_where, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 329>)
+   327         310 LOAD_CONST              29 (<code object postgres_transforms, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 327>)
                312 MAKE_FUNCTION            0
-               314 STORE_NAME              32 (chain_where)
+               314 STORE_NAME              32 (postgres_transforms)
    
-   339         316 LOAD_CONST              30 (<code object postgres_transforms, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 339>)
+   350         316 LOAD_CONST              30 (<code object remove_quotes_around_0x_strings, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 350>)
                318 MAKE_FUNCTION            0
-               320 STORE_NAME              33 (postgres_transforms)
+               320 STORE_NAME              33 (remove_quotes_around_0x_strings)
    
-   362         322 LOAD_CONST              31 (<code object remove_quotes_around_0x_strings, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 362>)
+   359         322 LOAD_CONST              31 (<code object spark_function_replacements, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 359>)
                324 MAKE_FUNCTION            0
-               326 STORE_NAME              34 (remove_quotes_around_0x_strings)
+               326 STORE_NAME              34 (spark_function_replacements)
    
-   371         328 LOAD_CONST              32 (<code object spark_function_replacements, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 371>)
+   367         328 LOAD_CONST              32 (<code object spark_transforms, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 367>)
                330 MAKE_FUNCTION            0
-               332 STORE_NAME              35 (spark_function_replacements)
+               332 STORE_NAME              35 (spark_transforms)
    
-   379         334 LOAD_CONST              33 (<code object spark_transforms, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 379>)
+   386         334 LOAD_CONST              33 (<code object add_warnings_and_banner, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 386>)
                336 MAKE_FUNCTION            0
-               338 STORE_NAME              36 (spark_transforms)
+               338 STORE_NAME              36 (add_warnings_and_banner)
    
-   398         340 LOAD_CONST              34 (<code object add_warnings_and_banner, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 398>)
+   418         340 LOAD_CONST              34 (<code object parameter_placeholder, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 418>)
                342 MAKE_FUNCTION            0
-               344 STORE_NAME              37 (add_warnings_and_banner)
-   
-   430         346 LOAD_CONST              35 (<code object parameter_placeholder, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 430>)
-               348 MAKE_FUNCTION            0
-               350 STORE_NAME              38 (parameter_placeholder)
-               352 LOAD_CONST               1 (None)
-               354 RETURN_VALUE
+               344 STORE_NAME              37 (parameter_placeholder)
+               346 LOAD_CONST               1 (None)
+               348 RETURN_VALUE
    consts
       0
       None
       ('partial',)
       ('postgres_table_replacements',)
       code
          argcount  : 1
@@ -1773,91 +1769,26 @@
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'warn_sequence'
          firstlineno 269
          lnotab 0x0202360116012a0202fe040502fa1208
       code
          argcount  : 1
-         nlocals   : 2
-         stacksize : 7
-         flags     : 3
-         code
-            0x9700640144005d427d017401000000000000000000006a010000000000
-            00000064027401000000000000000000006a0200000000000000007c01a6
-            010000ab0100000000000000007a00000064037a00000064047c017a0000
-            0064047a0000007c007400000000000000000000006a0300000000000000
-            00ac05a6040000ab0400000000000000007d008c437c005300
-         283           0 RESUME                   0
-         
-         284           2 LOAD_CONST               1 (('replace',))
-                       4 GET_ITER
-                 >>    6 FOR_ITER                66 (to 140)
-                       8 STORE_FAST               1 (keyword)
-         
-         286          10 LOAD_GLOBAL              1 (NULL + re)
-                      22 LOAD_ATTR                1 (sub)
-         
-         287          32 LOAD_CONST               2 ('\\b')
-                      34 LOAD_GLOBAL              1 (NULL + re)
-                      46 LOAD_ATTR                2 (escape)
-                      56 LOAD_FAST                1 (keyword)
-                      58 PRECALL                  1
-                      62 CALL                     1
-                      72 BINARY_OP                0 (+)
-                      76 LOAD_CONST               3 ('(?!\\()')
-                      78 BINARY_OP                0 (+)
-         
-         288          82 LOAD_CONST               4 ('"')
-                      84 LOAD_FAST                1 (keyword)
-                      86 BINARY_OP                0 (+)
-                      90 LOAD_CONST               4 ('"')
-                      92 BINARY_OP                0 (+)
-         
-         289          96 LOAD_FAST                0 (query)
-         
-         290          98 LOAD_GLOBAL              0 (re)
-                     110 LOAD_ATTR                3 (IGNORECASE)
-         
-         286         120 KW_NAMES                 5
-                     122 PRECALL                  4
-                     126 CALL                     4
-                     136 STORE_FAST               0 (query)
-                     138 JUMP_BACKWARD           67 (to 6)
-         
-         292     >>  140 LOAD_FAST                0 (query)
-                     142 RETURN_VALUE
-         consts
-            None
-            ('replace',)
-            '\\b'
-            '(?!\\()'
-            '"'
-            ('flags',)
-         names      ('re', 'sub', 'escape', 'IGNORECASE')
-         varnames   ('query', 'keyword')
-         freevars   ()
-         cellvars   ()
-         filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
-         name       'prep_query'
-         firstlineno 283
-         lnotab 0x02010802160132010e01020116fc1406
-      code
-         argcount  : 1
          nlocals   : 1
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c00a00200
             000000000000000000000000000000000000006401ac02a6010000ab0100
             00000000000000a003000000000000000000000000000000000000000064
             036404a6020000ab0200000000000000006401ac05a6020000ab02000000
             00000000005300
-         295           0 RESUME                   0
+         283           0 RESUME                   0
          
-         297           2 LOAD_GLOBAL              1 (NULL + sqlglot)
+         285           2 LOAD_GLOBAL              1 (NULL + sqlglot)
                       14 LOAD_ATTR                1 (parse_one)
                       24 LOAD_FAST                0 (query)
                       26 LOAD_METHOD              2 (sql)
                       48 LOAD_CONST               1 ('trino')
                       50 KW_NAMES                 2
                       52 PRECALL                  1
                       56 CALL                     1
@@ -1880,15 +1811,15 @@
             ('read',)
          names      ('sqlglot', 'parse_one', 'sql', 'replace')
          varnames   ('query',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'rename_amount_column'
-         firstlineno 295
+         firstlineno 283
          lnotab 0x0202
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -1896,52 +1827,52 @@
             02a6010000ab0100000000000000007d0164037c01a00100000000000000
             00000000000000000000000000a6000000ab000000000000000000760072
             277405000000000000000000006a030000000000000000640364047c0174
             04000000000000000000006a040000000000000000ac05a6040000ab0400
             000000000000007d0164067c017a0000007d01740b000000000000000000
             006a0600000000000000007c016401ac07a6020000ab0200000000000000
             005300
-         300           0 RESUME                   0
+         288           0 RESUME                   0
          
-         302           2 LOAD_FAST                0 (node)
+         290           2 LOAD_FAST                0 (node)
                        4 LOAD_METHOD              0 (sql)
                       26 LOAD_CONST               1 ('trino')
                       28 KW_NAMES                 2
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_FAST               1 (query)
          
-         303          46 LOAD_CONST               3 ('bytea2numeric')
+         291          46 LOAD_CONST               3 ('bytea2numeric')
                       48 LOAD_FAST                1 (query)
                       50 LOAD_METHOD              1 (lower)
                       72 PRECALL                  0
                       76 CALL                     0
                       86 CONTAINS_OP              0
                       88 POP_JUMP_FORWARD_IF_FALSE    39 (to 168)
          
-         304          90 LOAD_GLOBAL              5 (NULL + re)
+         292          90 LOAD_GLOBAL              5 (NULL + re)
                      102 LOAD_ATTR                3 (sub)
                      112 LOAD_CONST               3 ('bytea2numeric')
                      114 LOAD_CONST               4 ('bytearray_to_bigint')
                      116 LOAD_FAST                1 (query)
                      118 LOAD_GLOBAL              4 (re)
                      130 LOAD_ATTR                4 (IGNORECASE)
                      140 KW_NAMES                 5
                      142 PRECALL                  4
                      146 CALL                     4
                      156 STORE_FAST               1 (query)
          
-         306         158 LOAD_CONST               6 ('/* !Bytea warning: We now have new bytearray functions to cover conversions and stuff like length, concat, substring, etc. Check out the docs here: https://dune.com/docs/reference/dune-v2/query-engine/#byte-array-to-numeric-functions */\n\n')
+         294         158 LOAD_CONST               6 ('/* !Bytea warning: We now have new bytearray functions to cover conversions and stuff like length, concat, substring, etc. Check out the docs here: https://dune.com/docs/reference/dune-v2/query-engine/#byte-array-to-numeric-functions */\n\n')
          
-         310         160 LOAD_FAST                1 (query)
+         298         160 LOAD_FAST                1 (query)
          
-         305         162 BINARY_OP                0 (+)
+         293         162 BINARY_OP                0 (+)
                      166 STORE_FAST               1 (query)
          
-         311     >>  168 LOAD_GLOBAL             11 (NULL + sqlglot)
+         299     >>  168 LOAD_GLOBAL             11 (NULL + sqlglot)
                      180 LOAD_ATTR                6 (parse_one)
                      190 LOAD_FAST                1 (query)
                      192 LOAD_CONST               1 ('trino')
                      194 KW_NAMES                 7
                      196 PRECALL                  2
                      200 CALL                     2
                      210 RETURN_VALUE
@@ -1956,31 +1887,31 @@
             ('read',)
          names      ('sql', 'lower', 're', 'sub', 'IGNORECASE', 'sqlglot', 'parse_one')
          varnames   ('node', 'query')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'bytea2numeric'
-         firstlineno 300
+         firstlineno 288
          lnotab 0x02022c012c014402020402fb0606
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
             0x970064017d017401000000000000000000006a0100000000000000007c
             0164027c007400000000000000000000006a020000000000000000ac03a6
             040000ab0400000000000000005300
-         314           0 RESUME                   0
+         302           0 RESUME                   0
          
-         316           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]\\{\\{(.*?)\\}\\}[\'\\"]\\s*\\)')
+         304           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]\\{\\{(.*?)\\}\\}[\'\\"]\\s*\\)')
                        4 STORE_FAST               1 (pattern)
          
-         317           6 LOAD_GLOBAL              1 (NULL + re)
+         305           6 LOAD_GLOBAL              1 (NULL + re)
                       18 LOAD_ATTR                1 (sub)
                       28 LOAD_FAST                1 (pattern)
                       30 LOAD_CONST               2 ('{{\\1}}')
                       32 LOAD_FAST                0 (query)
                       34 LOAD_GLOBAL              0 (re)
                       46 LOAD_ATTR                2 (IGNORECASE)
                       56 KW_NAMES                 3
@@ -1994,95 +1925,95 @@
             ('flags',)
          names      ('re', 'sub', 'IGNORECASE')
          varnames   ('query', 'pattern')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'fix_bytearray_param'
-         firstlineno 314
+         firstlineno 302
          lnotab 0x02020401
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x970064017d017401000000000000000000006a0100000000000000007c
             0164027c007400000000000000000000006a020000000000000000ac03a6
             040000ab0400000000000000007d027c025300
-         320           0 RESUME                   0
+         308           0 RESUME                   0
          
-         324           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]0x(.*?)[\'\\"]\\s*\\)')
+         312           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]0x(.*?)[\'\\"]\\s*\\)')
                        4 STORE_FAST               1 (pattern)
          
-         325           6 LOAD_GLOBAL              1 (NULL + re)
+         313           6 LOAD_GLOBAL              1 (NULL + re)
                       18 LOAD_ATTR                1 (sub)
                       28 LOAD_FAST                1 (pattern)
                       30 LOAD_CONST               2 ('0x\\1')
                       32 LOAD_FAST                0 (query)
                       34 LOAD_GLOBAL              0 (re)
                       46 LOAD_ATTR                2 (IGNORECASE)
                       56 KW_NAMES                 3
                       58 PRECALL                  4
                       62 CALL                     4
                       72 STORE_FAST               2 (substituted)
          
-         326          74 LOAD_FAST                2 (substituted)
+         314          74 LOAD_FAST                2 (substituted)
                       76 RETURN_VALUE
          consts
             "Remove lower function call around '0x...' string literals, and remove the string since we have native hex types.\n\n    This has to happen after SQLGlot, since it will parse a bare 0x as a string literal"
             'lower\\(\\s*[\'\\"]0x(.*?)[\'\\"]\\s*\\)'
             '0x\\1'
             ('flags',)
          names      ('re', 'sub', 'IGNORECASE')
          varnames   ('query', 'pattern', 'substituted')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'fix_bytearray_lower'
-         firstlineno 320
+         firstlineno 308
          lnotab 0x020404014401
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000740200000000000000000000740400
             000000000000000000740600000000000000000000740800000000000000
             00000064019c057c00190000000000000000005300
-         329           0 RESUME                   0
+         317           0 RESUME                   0
          
-         331           2 LOAD_GLOBAL              0 (chain_where_gnosis)
+         319           2 LOAD_GLOBAL              0 (chain_where_gnosis)
          
-         332          14 LOAD_GLOBAL              2 (chain_where_optimism)
+         320          14 LOAD_GLOBAL              2 (chain_where_optimism)
          
-         333          26 LOAD_GLOBAL              4 (chain_where_bnb)
+         321          26 LOAD_GLOBAL              4 (chain_where_bnb)
          
-         334          38 LOAD_GLOBAL              6 (chain_where_polygon)
+         322          38 LOAD_GLOBAL              6 (chain_where_polygon)
          
-         335          50 LOAD_GLOBAL              8 (chain_where_ethereum)
+         323          50 LOAD_GLOBAL              8 (chain_where_ethereum)
          
-         330          62 LOAD_CONST               1 (('gnosis', 'optimism', 'bnb', 'polygon', 'ethereum'))
+         318          62 LOAD_CONST               1 (('gnosis', 'optimism', 'bnb', 'polygon', 'ethereum'))
                       64 BUILD_CONST_KEY_MAP      5
          
-         336          66 LOAD_FAST                0 (dataset)
+         324          66 LOAD_FAST                0 (dataset)
          
-         330          68 BINARY_SUBSCR
+         318          68 BINARY_SUBSCR
                       78 RETURN_VALUE
          consts
             None
             ('gnosis', 'optimism', 'bnb', 'polygon', 'ethereum')
          names      ('chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'chain_where_ethereum')
          varnames   ('dataset',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'chain_where'
-         firstlineno 329
+         firstlineno 317
          lnotab 0x02020c010c010c010c010cfb040602fa
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 11
          flags     : 3
          code
@@ -2092,170 +2023,170 @@
             000000000000000000740a00000000000000000000740c00000000000000
             000000740e00000000000000000000741000000000000000000000741300
             0000000000000000007c01a6010000ab0100000000000000007414000000
             000000000000007416000000000000000000007418000000000000000000
             00660b7d037c0344005d177d047c02a00d00000000000000000000000000
             000000000000007c04a6010000ab0100000000000000007d028c187c0253
             00
-         339           0 RESUME                   0
+         327           0 RESUME                   0
          
-         343           2 LOAD_GLOBAL              1 (NULL + sqlglot)
+         331           2 LOAD_GLOBAL              1 (NULL + sqlglot)
                       14 LOAD_ATTR                1 (parse_one)
                       24 LOAD_FAST                0 (query)
                       26 LOAD_CONST               1 ('trino')
                       28 KW_NAMES                 2
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (query_tree)
          
-         345          46 LOAD_GLOBAL              5 (NULL + postgres_table_replacements)
+         333          46 LOAD_GLOBAL              5 (NULL + postgres_table_replacements)
                       58 LOAD_FAST                1 (dataset)
                       60 PRECALL                  1
                       64 CALL                     1
          
-         346          74 LOAD_GLOBAL              6 (fix_boolean)
+         334          74 LOAD_GLOBAL              6 (fix_boolean)
          
-         347          86 LOAD_GLOBAL              8 (cast_numeric)
+         335          86 LOAD_GLOBAL              8 (cast_numeric)
          
-         348          98 LOAD_GLOBAL             10 (cast_timestamp)
+         336          98 LOAD_GLOBAL             10 (cast_timestamp)
          
-         349         110 LOAD_GLOBAL             12 (warn_unnest)
+         337         110 LOAD_GLOBAL             12 (warn_unnest)
          
-         350         122 LOAD_GLOBAL             14 (warn_sequence)
+         338         122 LOAD_GLOBAL             14 (warn_sequence)
          
-         351         134 LOAD_GLOBAL             16 (dex_trades_fixes)
+         339         134 LOAD_GLOBAL             16 (dex_trades_fixes)
          
-         352         146 LOAD_GLOBAL             19 (NULL + chain_where)
+         340         146 LOAD_GLOBAL             19 (NULL + chain_where)
                      158 LOAD_FAST                1 (dataset)
                      160 PRECALL                  1
                      164 CALL                     1
          
-         353         174 LOAD_GLOBAL             20 (bytearray_parameter_fix)
+         341         174 LOAD_GLOBAL             20 (bytearray_parameter_fix)
          
-         354         186 LOAD_GLOBAL             22 (rename_amount_column)
+         342         186 LOAD_GLOBAL             22 (rename_amount_column)
          
-         355         198 LOAD_GLOBAL             24 (bytea2numeric)
+         343         198 LOAD_GLOBAL             24 (bytea2numeric)
          
-         344         210 BUILD_TUPLE             11
+         332         210 BUILD_TUPLE             11
                      212 STORE_FAST               3 (transforms)
          
-         357         214 LOAD_FAST                3 (transforms)
+         345         214 LOAD_FAST                3 (transforms)
                      216 GET_ITER
                  >>  218 FOR_ITER                23 (to 266)
                      220 STORE_FAST               4 (f)
          
-         358         222 LOAD_FAST                2 (query_tree)
+         346         222 LOAD_FAST                2 (query_tree)
                      224 LOAD_METHOD             13 (transform)
                      246 LOAD_FAST                4 (f)
                      248 PRECALL                  1
                      252 CALL                     1
                      262 STORE_FAST               2 (query_tree)
                      264 JUMP_BACKWARD           24 (to 218)
          
-         359     >>  266 LOAD_FAST                2 (query_tree)
+         347     >>  266 LOAD_FAST                2 (query_tree)
                      268 RETURN_VALUE
          consts
             "Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.\n\n    Each transform takes and returns a sqlglot.Expression"
             'trino'
             ('read',)
          names      ('sqlglot', 'parse_one', 'postgres_table_replacements', 'fix_boolean', 'cast_numeric', 'cast_timestamp', 'warn_unnest', 'warn_sequence', 'dex_trades_fixes', 'chain_where', 'bytearray_parameter_fix', 'rename_amount_column', 'bytea2numeric', 'transform')
          varnames   ('query', 'dataset', 'query_tree', 'transforms', 'f')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'postgres_transforms'
-         firstlineno 339
+         firstlineno 327
          lnotab
             0x02042c021c010c010c010c010c010c010c011c010c010c010cf5040d08
             012c01
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x970064017d017401000000000000000000006a0100000000000000007c
             0164027c007400000000000000000000006a020000000000000000ac03a6
             040000ab0400000000000000007d027c025300
-         362           0 RESUME                   0
+         350           0 RESUME                   0
          
-         366           2 LOAD_CONST               1 ("'0x(.*?)'")
+         354           2 LOAD_CONST               1 ("'0x(.*?)'")
                        4 STORE_FAST               1 (pattern)
          
-         367           6 LOAD_GLOBAL              1 (NULL + re)
+         355           6 LOAD_GLOBAL              1 (NULL + re)
                       18 LOAD_ATTR                1 (sub)
                       28 LOAD_FAST                1 (pattern)
                       30 LOAD_CONST               2 ('0x\\1')
                       32 LOAD_FAST                0 (query)
                       34 LOAD_GLOBAL              0 (re)
                       46 LOAD_ATTR                2 (IGNORECASE)
                       56 KW_NAMES                 3
                       58 PRECALL                  4
                       62 CALL                     4
                       72 STORE_FAST               2 (substituted)
          
-         368          74 LOAD_FAST                2 (substituted)
+         356          74 LOAD_FAST                2 (substituted)
                       76 RETURN_VALUE
          consts
             "Remove string quotes around '0x...' string literals\n\n    This has to happen after SQLGlot, since it will parse a bare 0x as a string literal"
             "'0x(.*?)'"
             '0x\\1'
             ('flags',)
          names      ('re', 'sub', 'IGNORECASE')
          varnames   ('query', 'pattern', 'substituted')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'remove_quotes_around_0x_strings'
-         firstlineno 362
+         firstlineno 350
          lnotab 0x020404014401
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
             0x97007c00a00000000000000000000000000000000000000000006401ac
             02a6010000ab0100000000000000007d0164037c01a00100000000000000
             00000000000000000000000000a6000000ab000000000000000000760072
             227405000000000000000000006a030000000000000000640464057c0174
             04000000000000000000006a040000000000000000ac06a6040000ab0400
             000000000000007d01740b000000000000000000006a0600000000000000
             007c016401ac07a6020000ab0200000000000000005300
-         371           0 RESUME                   0
+         359           0 RESUME                   0
          
-         373           2 LOAD_FAST                0 (node)
+         361           2 LOAD_FAST                0 (node)
                        4 LOAD_METHOD              0 (sql)
                       26 LOAD_CONST               1 ('trino')
                       28 KW_NAMES                 2
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_FAST               1 (query)
          
-         374          46 LOAD_CONST               3 ('timestamp(')
+         362          46 LOAD_CONST               3 ('timestamp(')
                       48 LOAD_FAST                1 (query)
                       50 LOAD_METHOD              1 (lower)
                       72 PRECALL                  0
                       76 CALL                     0
                       86 CONTAINS_OP              0
                       88 POP_JUMP_FORWARD_IF_FALSE    34 (to 158)
          
-         375          90 LOAD_GLOBAL              5 (NULL + re)
+         363          90 LOAD_GLOBAL              5 (NULL + re)
                      102 LOAD_ATTR                3 (sub)
                      112 LOAD_CONST               4 ('timestamp')
                      114 LOAD_CONST               5 ('from_unixtime')
                      116 LOAD_FAST                1 (query)
                      118 LOAD_GLOBAL              4 (re)
                      130 LOAD_ATTR                4 (IGNORECASE)
                      140 KW_NAMES                 6
                      142 PRECALL                  4
                      146 CALL                     4
                      156 STORE_FAST               1 (query)
          
-         376     >>  158 LOAD_GLOBAL             11 (NULL + sqlglot)
+         364     >>  158 LOAD_GLOBAL             11 (NULL + sqlglot)
                      170 LOAD_ATTR                6 (parse_one)
                      180 LOAD_FAST                1 (query)
                      182 LOAD_CONST               1 ('trino')
                      184 KW_NAMES                 7
                      186 PRECALL                  2
                      190 CALL                     2
                      200 RETURN_VALUE
@@ -2270,148 +2201,148 @@
             ('read',)
          names      ('sql', 'lower', 're', 'sub', 'IGNORECASE', 'sqlglot', 'parse_one')
          varnames   ('node', 'query')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'spark_function_replacements'
-         firstlineno 371
+         firstlineno 359
          lnotab 0x02022c012c014401
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c006401ac
             02a6020000ab0200000000000000007d0174040000000000000000000074
             0600000000000000000000740800000000000000000000740a0000000000
             0000000000740c00000000000000000000740e0000000000000000000074
             100000000000000000000066077d027c0244005d177d037c01a009000000
             00000000000000000000000000000000007c03a6010000ab010000000000
             0000007d018c187c015300
-         379           0 RESUME                   0
+         367           0 RESUME                   0
          
-         383           2 LOAD_GLOBAL              1 (NULL + sqlglot)
+         371           2 LOAD_GLOBAL              1 (NULL + sqlglot)
                       14 LOAD_ATTR                1 (parse_one)
                       24 LOAD_FAST                0 (query)
                       26 LOAD_CONST               1 ('trino')
                       28 KW_NAMES                 2
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               1 (query_tree)
          
-         385          46 LOAD_GLOBAL              4 (fix_boolean)
+         373          46 LOAD_GLOBAL              4 (fix_boolean)
          
-         386          58 LOAD_GLOBAL              6 (cast_numeric)
+         374          58 LOAD_GLOBAL              6 (cast_numeric)
          
-         387          70 LOAD_GLOBAL              8 (cast_timestamp)
+         375          70 LOAD_GLOBAL              8 (cast_timestamp)
          
-         388          82 LOAD_GLOBAL             10 (warn_unnest)
+         376          82 LOAD_GLOBAL             10 (warn_unnest)
          
-         389          94 LOAD_GLOBAL             12 (warn_sequence)
+         377          94 LOAD_GLOBAL             12 (warn_sequence)
          
-         390         106 LOAD_GLOBAL             14 (bytea2numeric)
+         378         106 LOAD_GLOBAL             14 (bytea2numeric)
          
-         391         118 LOAD_GLOBAL             16 (spark_function_replacements)
+         379         118 LOAD_GLOBAL             16 (spark_function_replacements)
          
-         384         130 BUILD_TUPLE              7
+         372         130 BUILD_TUPLE              7
                      132 STORE_FAST               2 (transforms)
          
-         393         134 LOAD_FAST                2 (transforms)
+         381         134 LOAD_FAST                2 (transforms)
                      136 GET_ITER
                  >>  138 FOR_ITER                23 (to 186)
                      140 STORE_FAST               3 (f)
          
-         394         142 LOAD_FAST                1 (query_tree)
+         382         142 LOAD_FAST                1 (query_tree)
                      144 LOAD_METHOD              9 (transform)
                      166 LOAD_FAST                3 (f)
                      168 PRECALL                  1
                      172 CALL                     1
                      182 STORE_FAST               1 (query_tree)
                      184 JUMP_BACKWARD           24 (to 138)
          
-         395     >>  186 LOAD_FAST                1 (query_tree)
+         383     >>  186 LOAD_FAST                1 (query_tree)
                      188 RETURN_VALUE
          consts
             "Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.\n\n    Each transform takes and returns a sqlglot.Expression"
             'trino'
             ('read',)
          names      ('sqlglot', 'parse_one', 'fix_boolean', 'cast_numeric', 'cast_timestamp', 'warn_unnest', 'warn_sequence', 'bytea2numeric', 'spark_function_replacements', 'transform')
          varnames   ('query', 'query_tree', 'transforms', 'f')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'spark_transforms'
-         firstlineno 379
+         firstlineno 367
          lnotab 0x02042c020c010c010c010c010c010c010cf9040908012c01
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x970064017c00a0000000000000000000000000000000000000000000a6
             000000ab0000000000000000007600720564027c007a0000007d00740300
             0000000000000000006a02000000000000000064037c00a6020000ab0200
             00000000000000720564047c007a0000007d0064057c00a0000000000000
             000000000000000000000000000000a6000000ab00000000000000000076
             00720564067c007a0000007d0064077c007a0000005300
-         398           0 RESUME                   0
+         386           0 RESUME                   0
          
-         400           2 LOAD_CONST               1 ("lower('{{")
+         388           2 LOAD_CONST               1 ("lower('{{")
                        4 LOAD_FAST                0 (query)
                        6 LOAD_METHOD              0 (lower)
                       28 PRECALL                  0
                       32 CALL                     0
                       42 CONTAINS_OP              0
                       44 POP_JUMP_FORWARD_IF_FALSE     5 (to 56)
          
-         402          46 LOAD_CONST               2 ("/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n")
+         390          46 LOAD_CONST               2 ("/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n")
          
-         405          48 LOAD_FAST                0 (query)
+         393          48 LOAD_FAST                0 (query)
          
-         401          50 BINARY_OP                0 (+)
+         389          50 BINARY_OP                0 (+)
                       54 STORE_FAST               0 (query)
          
-         408     >>   56 LOAD_GLOBAL              3 (NULL + re)
+         396     >>   56 LOAD_GLOBAL              3 (NULL + re)
                       68 LOAD_ATTR                2 (search)
                       78 LOAD_CONST               3 ('\\[.*\\]')
                       80 LOAD_FAST                0 (query)
                       82 PRECALL                  2
                       86 CALL                     2
                       96 POP_JUMP_FORWARD_IF_FALSE     5 (to 108)
          
-         410          98 LOAD_CONST               4 ('/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n')
+         398          98 LOAD_CONST               4 ('/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n')
          
-         413         100 LOAD_FAST                0 (query)
+         401         100 LOAD_FAST                0 (query)
          
-         409         102 BINARY_OP                0 (+)
+         397         102 BINARY_OP                0 (+)
                      106 STORE_FAST               0 (query)
          
-         415     >>  108 LOAD_CONST               5 ('dune_user_generated')
+         403     >>  108 LOAD_CONST               5 ('dune_user_generated')
                      110 LOAD_FAST                0 (query)
                      112 LOAD_METHOD              0 (lower)
                      134 PRECALL                  0
                      138 CALL                     0
                      148 CONTAINS_OP              0
                      150 POP_JUMP_FORWARD_IF_FALSE     5 (to 162)
          
-         417         152 LOAD_CONST               6 ("/* !Generated view warning: you can't query views in dune_user_generated anymore. All queries in DuneSQL are by default views though (try querying the table 'query_1747157') */\n\n")
+         405         152 LOAD_CONST               6 ("/* !Generated view warning: you can't query views in dune_user_generated anymore. All queries in DuneSQL are by default views though (try querying the table 'query_1747157') */\n\n")
          
-         420         154 LOAD_FAST                0 (query)
+         408         154 LOAD_FAST                0 (query)
          
-         416         156 BINARY_OP                0 (+)
+         404         156 BINARY_OP                0 (+)
                      160 STORE_FAST               0 (query)
          
-         424     >>  162 LOAD_CONST               7 ("/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n")
+         412     >>  162 LOAD_CONST               7 ("/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n")
          
-         427         164 LOAD_FAST                0 (query)
+         415         164 LOAD_FAST                0 (query)
          
-         423         166 BINARY_OP                0 (+)
+         411         166 BINARY_OP                0 (+)
                      170 RETURN_VALUE
          consts
             "Add a success banner at the top, and look for a few cases of things we don't fix and add a warning if present"
             "lower('{{"
             "/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n"
             '\\[.*\\]'
             '/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n'
@@ -2420,15 +2351,15 @@
             "/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n"
          names      ('lower', 're', 'search')
          varnames   ('query',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'add_warnings_and_banner'
-         firstlineno 398
+         firstlineno 386
          lnotab
             0x02022c02020302fc06072a02020302fc06062c02020302fc0608020302
             fc
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
@@ -2438,65 +2369,65 @@
             0200000000000000000000a6020000ab020000000000000000a000000000
             000000000000000000000000000000000064027404000000000000000000
             00a6020000ab020000000000000000a00000000000000000000000000000
             0000000000000064036404a6020000ab020000000000000000a000000000
             000000000000000000000000000000000064056404a6020000ab02000000
             0000000000a0030000000000000000000000000000000000000000a60000
             00ab0000000000000000005300
-         430           0 RESUME                   0
+         418           0 RESUME                   0
          
-         432           2 LOAD_FAST                0 (p)
+         420           2 LOAD_FAST                0 (p)
                        4 LOAD_METHOD              0 (replace)
                       26 LOAD_CONST               1 ('{{')
                       28 LOAD_GLOBAL              2 (param_left_placeholder)
                       40 PRECALL                  2
                       44 CALL                     2
          
-         433          54 LOAD_METHOD              0 (replace)
+         421          54 LOAD_METHOD              0 (replace)
                       76 LOAD_CONST               2 ('}}')
                       78 LOAD_GLOBAL              4 (param_right_placeholder)
                       90 PRECALL                  2
                       94 CALL                     2
          
-         434         104 LOAD_METHOD              0 (replace)
+         422         104 LOAD_METHOD              0 (replace)
                      126 LOAD_CONST               3 (' ')
                      128 LOAD_CONST               4 ('_')
                      130 PRECALL                  2
                      134 CALL                     2
          
-         435         144 LOAD_METHOD              0 (replace)
+         423         144 LOAD_METHOD              0 (replace)
                      166 LOAD_CONST               5 ('-')
                      168 LOAD_CONST               4 ('_')
                      170 PRECALL                  2
                      174 CALL                     2
          
-         436         184 LOAD_METHOD              3 (lower)
+         424         184 LOAD_METHOD              3 (lower)
                      206 PRECALL                  0
                      210 CALL                     0
          
-         431         220 RETURN_VALUE
+         419         220 RETURN_VALUE
          consts
             None
             '{{'
             '}}'
             ' '
             '_'
             '-'
          names      ('replace', 'param_left_placeholder', 'param_right_placeholder', 'lower')
          varnames   ('p',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'parameter_placeholder'
-         firstlineno 430
+         firstlineno 418
          lnotab 0x0202340132012801280124fb
-   names      ('re', 'functools', 'partial', 'sqlglot', 'dune.harmonizer.table_replacements', 'postgres_table_replacements', 'extract_nested_select', 'recurse_where', 'chain_where_blockchain', 'chain_where_ethereum', 'chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'dex_trades_fixes', 'param_left_placeholder', 'param_right_placeholder', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'bytearray_parameter_fix', 'cast_numeric', 'cast_timestamp', 'fix_boolean', 'warn_unnest', 'warn_sequence', 'prep_query', 'rename_amount_column', 'bytea2numeric', 'fix_bytearray_param', 'fix_bytearray_lower', 'chain_where', 'postgres_transforms', 'remove_quotes_around_0x_strings', 'spark_function_replacements', 'spark_transforms', 'add_warnings_and_banner', 'parameter_placeholder')
+   names      ('re', 'functools', 'partial', 'sqlglot', 'dune.harmonizer.table_replacements', 'postgres_table_replacements', 'extract_nested_select', 'recurse_where', 'chain_where_blockchain', 'chain_where_ethereum', 'chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'dex_trades_fixes', 'param_left_placeholder', 'param_right_placeholder', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'bytearray_parameter_fix', 'cast_numeric', 'cast_timestamp', 'fix_boolean', 'warn_unnest', 'warn_sequence', 'rename_amount_column', 'bytea2numeric', 'fix_bytearray_param', 'fix_bytearray_lower', 'chain_where', 'postgres_transforms', 'remove_quotes_around_0x_strings', 'spark_function_replacements', 'spark_transforms', 'add_warnings_and_banner', 'parameter_placeholder')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020108010c0208020c030613065906121a011a011a011a011a0306
-      2c040104010a010a010a010a03061b0609060f060a060e060e060c060506
-      0e06060609060a06170609060806130620
+      2c040104010a010a010a010a03061b0609060f060a060e060e0605060e06
+      060609060a06170609060806130620
```

### Comparing `dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc` & `dune_harmonizer-0.4.1/dune/harmonizer/__pycache__/errors.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x99154164 (Thu Apr 20 10:36:09 2023 UTC)
+moddate:  0x58434164 (Thu Apr 20 13:51:20 2023 UTC)
 files sz: 105
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc` & `dune_harmonizer-0.4.1/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x99154164 (Thu Apr 20 10:36:09 2023 UTC)
+moddate:  0x58434164 (Thu Apr 20 13:51:20 2023 UTC)
 files sz: 2018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x9700640064016c005a00640064016c015a01640284005a0264015300
```

### Comparing `dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/translate.cpython-311.pyc` & `dune_harmonizer-0.4.1/dune/harmonizer/__pycache__/translate.cpython-311.pyc`

 * *Files 26% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0x99154164 (Thu Apr 20 10:36:09 2023 UTC)
-files sz: 2914
+moddate:  0x58434164 (Thu Apr 20 13:51:20 2023 UTC)
+files sz: 2863
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c016d025a0201
       00640064036c036d045a046d055a056d065a066d075a076d085a086d095a
-      096d0a5a0a6d0b5a0b6d0c5a0c6d0d5a0d0100640064046c0e6d0f5a0f01
-      00640584005a106407640684015a1164015300
+      096d0a5a0a6d0b5a0b6d0c5a0c0100640064046c0d6d0e5a0e0100640584
+      005a0f6407640684015a1064015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (re)
                  8 STORE_NAME               0 (re)
    
@@ -27,15 +27,15 @@
                 20 LOAD_CONST               2 (('ParseError',))
                 22 IMPORT_NAME              1 (sqlglot)
                 24 IMPORT_FROM              2 (ParseError)
                 26 STORE_NAME               2 (ParseError)
                 28 POP_TOP
    
      6          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               3 (('add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'parameter_placeholder', 'postgres_transforms', 'prep_query', 'remove_quotes_around_0x_strings', 'spark_transforms'))
+                32 LOAD_CONST               3 (('add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'parameter_placeholder', 'postgres_transforms', 'remove_quotes_around_0x_strings', 'spark_transforms'))
                 34 IMPORT_NAME              3 (dune.harmonizer.custom_transforms)
                 36 IMPORT_FROM              4 (add_warnings_and_banner)
                 38 STORE_NAME               4 (add_warnings_and_banner)
                 40 IMPORT_FROM              5 (double_quoted_param_left_placeholder)
                 42 STORE_NAME               5 (double_quoted_param_left_placeholder)
                 44 IMPORT_FROM              6 (double_quoted_param_right_placeholder)
                 46 STORE_NAME               6 (double_quoted_param_right_placeholder)
@@ -43,78 +43,76 @@
                 50 STORE_NAME               7 (fix_bytearray_lower)
                 52 IMPORT_FROM              8 (fix_bytearray_param)
                 54 STORE_NAME               8 (fix_bytearray_param)
                 56 IMPORT_FROM              9 (parameter_placeholder)
                 58 STORE_NAME               9 (parameter_placeholder)
                 60 IMPORT_FROM             10 (postgres_transforms)
                 62 STORE_NAME              10 (postgres_transforms)
-                64 IMPORT_FROM             11 (prep_query)
-                66 STORE_NAME              11 (prep_query)
-                68 IMPORT_FROM             12 (remove_quotes_around_0x_strings)
-                70 STORE_NAME              12 (remove_quotes_around_0x_strings)
-                72 IMPORT_FROM             13 (spark_transforms)
-                74 STORE_NAME              13 (spark_transforms)
-                76 POP_TOP
+                64 IMPORT_FROM             11 (remove_quotes_around_0x_strings)
+                66 STORE_NAME              11 (remove_quotes_around_0x_strings)
+                68 IMPORT_FROM             12 (spark_transforms)
+                70 STORE_NAME              12 (spark_transforms)
+                72 POP_TOP
    
-    18          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               4 (('DuneTranslationError',))
-                82 IMPORT_NAME             14 (dune.harmonizer.errors)
-                84 IMPORT_FROM             15 (DuneTranslationError)
-                86 STORE_NAME              15 (DuneTranslationError)
-                88 POP_TOP
+    17          74 LOAD_CONST               0 (0)
+                76 LOAD_CONST               4 (('DuneTranslationError',))
+                78 IMPORT_NAME             13 (dune.harmonizer.errors)
+                80 IMPORT_FROM             14 (DuneTranslationError)
+                82 STORE_NAME              14 (DuneTranslationError)
+                84 POP_TOP
    
-    21          90 LOAD_CONST               5 (<code object _clean_dataset, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/translate.py", line 21>)
-                92 MAKE_FUNCTION            0
-                94 STORE_NAME              16 (_clean_dataset)
+    20          86 LOAD_CONST               5 (<code object _clean_dataset, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/translate.py", line 20>)
+                88 MAKE_FUNCTION            0
+                90 STORE_NAME              15 (_clean_dataset)
    
-    28          96 LOAD_CONST               7 ((None,))
-                98 LOAD_CONST               6 (<code object _translate_query, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/translate.py", line 28>)
-               100 MAKE_FUNCTION            1 (defaults)
-               102 STORE_NAME              17 (_translate_query)
-               104 LOAD_CONST               1 (None)
-               106 RETURN_VALUE
+    27          92 LOAD_CONST               7 ((None,))
+                94 LOAD_CONST               6 (<code object _translate_query, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/translate.py", line 27>)
+                96 MAKE_FUNCTION            1 (defaults)
+                98 STORE_NAME              16 (_translate_query)
+               100 LOAD_CONST               1 (None)
+               102 RETURN_VALUE
    consts
       0
       None
       ('ParseError',)
-      ('add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'parameter_placeholder', 'postgres_transforms', 'prep_query', 'remove_quotes_around_0x_strings', 'spark_transforms')
+      ('add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'parameter_placeholder', 'postgres_transforms', 'remove_quotes_around_0x_strings', 'spark_transforms')
       ('DuneTranslationError',)
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x9700640144005d1c7d017c017c00a00000000000000000000000000000
             00000000000000a6000000ab000000000000000000760072047c01630201
             0053008c1d74030000000000000000000064027c009b009d02a6010000ab
             0100000000000000008201
-          21           0 RESUME                   0
+          20           0 RESUME                   0
          
-          22           2 LOAD_CONST               1 (('gnosis', 'optimism', 'bnb', 'polygon', 'ethereum'))
+          21           2 LOAD_CONST               1 (('gnosis', 'optimism', 'bnb', 'polygon', 'ethereum'))
                        4 GET_ITER
                  >>    6 FOR_ITER                28 (to 64)
                        8 STORE_FAST               1 (d)
          
-          23          10 LOAD_FAST                1 (d)
+          22          10 LOAD_FAST                1 (d)
                       12 LOAD_FAST                0 (dataset)
                       14 LOAD_METHOD              0 (lower)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 CONTAINS_OP              0
                       52 POP_JUMP_FORWARD_IF_FALSE     4 (to 62)
          
-          24          54 LOAD_FAST                1 (d)
+          23          54 LOAD_FAST                1 (d)
                       56 SWAP                     2
                       58 POP_TOP
                       60 RETURN_VALUE
          
-          23     >>   62 JUMP_BACKWARD           29 (to 6)
+          22     >>   62 JUMP_BACKWARD           29 (to 6)
          
-          25     >>   64 LOAD_GLOBAL              3 (NULL + ValueError)
+          24     >>   64 LOAD_GLOBAL              3 (NULL + ValueError)
                       76 LOAD_CONST               2 ('Unknown dataset: ')
                       78 LOAD_FAST                0 (dataset)
                       80 FORMAT_VALUE             0
                       82 BUILD_STRING             2
                       84 PRECALL                  1
                       88 CALL                     1
                       98 RAISE_VARARGS            1
@@ -124,283 +122,276 @@
             'Unknown dataset: '
          names      ('lower', 'ValueError')
          varnames   ('dataset', 'd')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/translate.py'
          name       '_clean_dataset'
-         firstlineno 21
+         firstlineno 20
          lnotab 0x020108012c0108ff0202
       code
          argcount  : 3
          nlocals   : 10
          stacksize : 6
          flags     : 3
          code
             0x970009007401000000000000000000006a01000000000000000064017c
             007400000000000000000000006a020000000000000000ac02a6030000ab
             0300000000000000007d03640384007c034400a6000000ab000000000000
             0000007d047c04a0030000000000000000000000000000000000000000a6
             000000ab00000000000000000044005d1b5c0200007d057d067c00a00400
             000000000000000000000000000000000000007c067c05a6020000ab0200
-            000000000000007d008c1c740b000000000000000000007c00a6010000ab
-            0100000000000000007d00740d000000000000000000006a070000000000
+            000000000000007d008c1c740b000000000000000000006a060000000000
             0000007c007c0164046405ac06a6040000ab040000000000000000640719
-            0000000000000000007d007c0164086b0200000000721074110000000000
+            0000000000000000007d007c0164086b02000000007210740f0000000000
             00000000007c00a6010000ab0100000000000000007d076e2c7c0164096b
             020000000072267c00a00400000000000000000000000000000000000000
-            00640a640ba6020000ab0200000000000000007d00741300000000000000
-            0000007c007c02a6020000ab0200000000000000007d077c07a00a000000
+            00640a640ba6020000ab0200000000000000007d00741100000000000000
+            0000007c007c02a6020000ab0200000000000000007d077c07a009000000
             000000000000000000000000000000000064046405ac0ca6020000ab0200
             000000000000007d007c04a0030000000000000000000000000000000000
             000000a6000000ab00000000000000000044005d1b5c0200007d057d067c
             00a00400000000000000000000000000000000000000007c057c06a60200
-            00ab0200000000000000007d008c1c7417000000000000000000007c00a6
+            00ab0200000000000000007d008c1c7415000000000000000000007c00a6
+            010000ab0100000000000000007d007417000000000000000000007c00a6
             010000ab0100000000000000007d007419000000000000000000007c00a6
             010000ab0100000000000000007d00741b000000000000000000007c00a6
-            010000ab0100000000000000007d00741d000000000000000000007c00a6
-            010000ab01000000000000000053002300741e0000000000000000000024
-            0072937d087421000000000000000000007c08a6010000ab010000000000
+            010000ab01000000000000000053002300741c0000000000000000000024
+            0072937d08741f000000000000000000007c08a6010000ab010000000000
             000000a0040000000000000000000000000000000000000000640d640ea6
             020000ab020000000000000000a004000000000000000000000000000000
             0000000000640f640ea6020000ab020000000000000000a0040000000000
-            0000000000000000000000000000007422000000000000000000006410a6
+            0000000000000000000000000000007420000000000000000000006410a6
             020000ab020000000000000000a004000000000000000000000000000000
-            00000000007424000000000000000000006411a6020000ab020000000000
-            0000007d097401000000000000000000006a130000000000000000641264
-            137c09a6030000ab0300000000000000007d097429000000000000000000
+            00000000007422000000000000000000006411a6020000ab020000000000
+            0000007d097401000000000000000000006a120000000000000000641264
+            137c09a6030000ab0300000000000000007d097427000000000000000000
             007c09a6010000ab010000000000000000820164147d087e087701770078
             0359007701
-          28           0 RESUME                   0
+          27           0 RESUME                   0
          
-          30           2 NOP
+          29           2 NOP
          
-          32           4 LOAD_GLOBAL              1 (NULL + re)
+          31           4 LOAD_GLOBAL              1 (NULL + re)
                       16 LOAD_ATTR                1 (findall)
                       26 LOAD_CONST               1 ('({{.*?}})')
                       28 LOAD_FAST                0 (query)
                       30 LOAD_GLOBAL              0 (re)
                       42 LOAD_ATTR                2 (IGNORECASE)
                       52 KW_NAMES                 2
                       54 PRECALL                  3
                       58 CALL                     3
                       68 STORE_FAST               3 (parameters)
          
-          33          70 LOAD_CONST               3 (<code object <dictcomp>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/translate.py", line 33>)
+          32          70 LOAD_CONST               3 (<code object <dictcomp>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/translate.py", line 32>)
                       72 MAKE_FUNCTION            0
                       74 LOAD_FAST                3 (parameters)
                       76 GET_ITER
                       78 PRECALL                  0
                       82 CALL                     0
                       92 STORE_FAST               4 (parameter_map)
          
-          34          94 LOAD_FAST                4 (parameter_map)
+          33          94 LOAD_FAST                4 (parameter_map)
                       96 LOAD_METHOD              3 (items)
                      118 PRECALL                  0
                      122 CALL                     0
                      132 GET_ITER
                  >>  134 FOR_ITER                27 (to 190)
                      136 UNPACK_SEQUENCE          2
                      140 STORE_FAST               5 (replace)
                      142 STORE_FAST               6 (original)
          
-          35         144 LOAD_FAST                0 (query)
+          34         144 LOAD_FAST                0 (query)
                      146 LOAD_METHOD              4 (replace)
                      168 LOAD_FAST                6 (original)
                      170 LOAD_FAST                5 (replace)
                      172 PRECALL                  2
                      176 CALL                     2
                      186 STORE_FAST               0 (query)
                      188 JUMP_BACKWARD           28 (to 134)
          
-          37     >>  190 LOAD_GLOBAL             11 (NULL + prep_query)
-                     202 LOAD_FAST                0 (query)
-                     204 PRECALL                  1
-                     208 CALL                     1
-                     218 STORE_FAST               0 (query)
-         
-          40         220 LOAD_GLOBAL             13 (NULL + sqlglot)
-                     232 LOAD_ATTR                7 (transpile)
-                     242 LOAD_FAST                0 (query)
-                     244 LOAD_FAST                1 (sqlglot_dialect)
-                     246 LOAD_CONST               4 ('trino')
-                     248 LOAD_CONST               5 (True)
-                     250 KW_NAMES                 6
-                     252 PRECALL                  4
-                     256 CALL                     4
-                     266 LOAD_CONST               7 (0)
-                     268 BINARY_SUBSCR
-                     278 STORE_FAST               0 (query)
-         
-          43         280 LOAD_FAST                1 (sqlglot_dialect)
-                     282 LOAD_CONST               8 ('spark')
-                     284 COMPARE_OP               2 (==)
-                     290 POP_JUMP_FORWARD_IF_FALSE    16 (to 324)
-         
-          44         292 LOAD_GLOBAL             17 (NULL + spark_transforms)
-                     304 LOAD_FAST                0 (query)
-                     306 PRECALL                  1
-                     310 CALL                     1
-                     320 STORE_FAST               7 (query_tree)
-                     322 JUMP_FORWARD            44 (to 412)
-         
-          45     >>  324 LOAD_FAST                1 (sqlglot_dialect)
-                     326 LOAD_CONST               9 ('postgres')
-                     328 COMPARE_OP               2 (==)
-                     334 POP_JUMP_FORWARD_IF_FALSE    38 (to 412)
-         
-          47         336 LOAD_FAST                0 (query)
-                     338 LOAD_METHOD              4 (replace)
-                     360 LOAD_CONST              10 ('\\x')
-                     362 LOAD_CONST              11 ('0x')
-                     364 PRECALL                  2
-                     368 CALL                     2
-                     378 STORE_FAST               0 (query)
-         
-          48         380 LOAD_GLOBAL             19 (NULL + postgres_transforms)
-                     392 LOAD_FAST                0 (query)
-                     394 LOAD_FAST                2 (dataset)
-                     396 PRECALL                  2
-                     400 CALL                     2
-                     410 STORE_FAST               7 (query_tree)
-         
-          51     >>  412 LOAD_FAST                7 (query_tree)
-                     414 LOAD_METHOD             10 (sql)
-                     436 LOAD_CONST               4 ('trino')
-                     438 LOAD_CONST               5 (True)
-                     440 KW_NAMES                12
-                     442 PRECALL                  2
-                     446 CALL                     2
-                     456 STORE_FAST               0 (query)
-         
-          54         458 LOAD_FAST                4 (parameter_map)
-                     460 LOAD_METHOD              3 (items)
-                     482 PRECALL                  0
-                     486 CALL                     0
-                     496 GET_ITER
-                 >>  498 FOR_ITER                27 (to 554)
-                     500 UNPACK_SEQUENCE          2
-                     504 STORE_FAST               5 (replace)
-                     506 STORE_FAST               6 (original)
-         
-          55         508 LOAD_FAST                0 (query)
-                     510 LOAD_METHOD              4 (replace)
-                     532 LOAD_FAST                5 (replace)
-                     534 LOAD_FAST                6 (original)
-                     536 PRECALL                  2
-                     540 CALL                     2
-                     550 STORE_FAST               0 (query)
-                     552 JUMP_BACKWARD           28 (to 498)
+          37     >>  190 LOAD_GLOBAL             11 (NULL + sqlglot)
+                     202 LOAD_ATTR                6 (transpile)
+                     212 LOAD_FAST                0 (query)
+                     214 LOAD_FAST                1 (sqlglot_dialect)
+                     216 LOAD_CONST               4 ('trino')
+                     218 LOAD_CONST               5 (True)
+                     220 KW_NAMES                 6
+                     222 PRECALL                  4
+                     226 CALL                     4
+                     236 LOAD_CONST               7 (0)
+                     238 BINARY_SUBSCR
+                     248 STORE_FAST               0 (query)
+         
+          40         250 LOAD_FAST                1 (sqlglot_dialect)
+                     252 LOAD_CONST               8 ('spark')
+                     254 COMPARE_OP               2 (==)
+                     260 POP_JUMP_FORWARD_IF_FALSE    16 (to 294)
+         
+          41         262 LOAD_GLOBAL             15 (NULL + spark_transforms)
+                     274 LOAD_FAST                0 (query)
+                     276 PRECALL                  1
+                     280 CALL                     1
+                     290 STORE_FAST               7 (query_tree)
+                     292 JUMP_FORWARD            44 (to 382)
+         
+          42     >>  294 LOAD_FAST                1 (sqlglot_dialect)
+                     296 LOAD_CONST               9 ('postgres')
+                     298 COMPARE_OP               2 (==)
+                     304 POP_JUMP_FORWARD_IF_FALSE    38 (to 382)
+         
+          44         306 LOAD_FAST                0 (query)
+                     308 LOAD_METHOD              4 (replace)
+                     330 LOAD_CONST              10 ('\\x')
+                     332 LOAD_CONST              11 ('0x')
+                     334 PRECALL                  2
+                     338 CALL                     2
+                     348 STORE_FAST               0 (query)
+         
+          45         350 LOAD_GLOBAL             17 (NULL + postgres_transforms)
+                     362 LOAD_FAST                0 (query)
+                     364 LOAD_FAST                2 (dataset)
+                     366 PRECALL                  2
+                     370 CALL                     2
+                     380 STORE_FAST               7 (query_tree)
+         
+          48     >>  382 LOAD_FAST                7 (query_tree)
+                     384 LOAD_METHOD              9 (sql)
+                     406 LOAD_CONST               4 ('trino')
+                     408 LOAD_CONST               5 (True)
+                     410 KW_NAMES                12
+                     412 PRECALL                  2
+                     416 CALL                     2
+                     426 STORE_FAST               0 (query)
+         
+          51         428 LOAD_FAST                4 (parameter_map)
+                     430 LOAD_METHOD              3 (items)
+                     452 PRECALL                  0
+                     456 CALL                     0
+                     466 GET_ITER
+                 >>  468 FOR_ITER                27 (to 524)
+                     470 UNPACK_SEQUENCE          2
+                     474 STORE_FAST               5 (replace)
+                     476 STORE_FAST               6 (original)
+         
+          52         478 LOAD_FAST                0 (query)
+                     480 LOAD_METHOD              4 (replace)
+                     502 LOAD_FAST                5 (replace)
+                     504 LOAD_FAST                6 (original)
+                     506 PRECALL                  2
+                     510 CALL                     2
+                     520 STORE_FAST               0 (query)
+                     522 JUMP_BACKWARD           28 (to 468)
+         
+          55     >>  524 LOAD_GLOBAL             21 (NULL + fix_bytearray_param)
+                     536 LOAD_FAST                0 (query)
+                     538 PRECALL                  1
+                     542 CALL                     1
+                     552 STORE_FAST               0 (query)
          
-          58     >>  554 LOAD_GLOBAL             23 (NULL + fix_bytearray_param)
+          56         554 LOAD_GLOBAL             23 (NULL + fix_bytearray_lower)
                      566 LOAD_FAST                0 (query)
                      568 PRECALL                  1
                      572 CALL                     1
                      582 STORE_FAST               0 (query)
          
-          59         584 LOAD_GLOBAL             25 (NULL + fix_bytearray_lower)
+          57         584 LOAD_GLOBAL             25 (NULL + remove_quotes_around_0x_strings)
                      596 LOAD_FAST                0 (query)
                      598 PRECALL                  1
                      602 CALL                     1
                      612 STORE_FAST               0 (query)
          
-          60         614 LOAD_GLOBAL             27 (NULL + remove_quotes_around_0x_strings)
+          59         614 LOAD_GLOBAL             27 (NULL + add_warnings_and_banner)
                      626 LOAD_FAST                0 (query)
                      628 PRECALL                  1
                      632 CALL                     1
-                     642 STORE_FAST               0 (query)
+                     642 RETURN_VALUE
+                 >>  644 PUSH_EXC_INFO
          
-          62         644 LOAD_GLOBAL             29 (NULL + add_warnings_and_banner)
-                     656 LOAD_FAST                0 (query)
-                     658 PRECALL                  1
-                     662 CALL                     1
-                     672 RETURN_VALUE
-                 >>  674 PUSH_EXC_INFO
-         
-          64         676 LOAD_GLOBAL             30 (ParseError)
-                     688 CHECK_EXC_MATCH
-                     690 POP_JUMP_FORWARD_IF_FALSE   147 (to 986)
-                     692 STORE_FAST               8 (e)
-         
-          69         694 LOAD_GLOBAL             33 (NULL + str)
-                     706 LOAD_FAST                8 (e)
-                     708 PRECALL                  1
-                     712 CALL                     1
-         
-          70         722 LOAD_METHOD              4 (replace)
-                     744 LOAD_CONST              13 ('\x1b[4m')
-                     746 LOAD_CONST              14 ('')
-                     748 PRECALL                  2
-                     752 CALL                     2
-         
-          71         762 LOAD_METHOD              4 (replace)
-                     784 LOAD_CONST              15 ('\x1b[0m')
-                     786 LOAD_CONST              14 ('')
-                     788 PRECALL                  2
-                     792 CALL                     2
-         
-          72         802 LOAD_METHOD              4 (replace)
-                     824 LOAD_GLOBAL             34 (double_quoted_param_left_placeholder)
-                     836 LOAD_CONST              16 ('{{')
-                     838 PRECALL                  2
-                     842 CALL                     2
-         
-          73         852 LOAD_METHOD              4 (replace)
-                     874 LOAD_GLOBAL             36 (double_quoted_param_right_placeholder)
-                     886 LOAD_CONST              17 ('}}')
-                     888 PRECALL                  2
-                     892 CALL                     2
-         
-          68         902 STORE_FAST               9 (error_message)
-         
-          76         904 LOAD_GLOBAL              1 (NULL + re)
-                     916 LOAD_ATTR               19 (sub)
-         
-          77         926 LOAD_CONST              18 ('. Line [0-9]+, Col: [0-9]+.')
-         
-          78         928 LOAD_CONST              19 ('.')
-         
-          79         930 LOAD_FAST                9 (error_message)
-         
-          76         932 PRECALL                  3
-                     936 CALL                     3
-                     946 STORE_FAST               9 (error_message)
-         
-          81         948 LOAD_GLOBAL             41 (NULL + DuneTranslationError)
-                     960 LOAD_FAST                9 (error_message)
-                     962 PRECALL                  1
-                     966 CALL                     1
-                     976 RAISE_VARARGS            1
-                 >>  978 LOAD_CONST              20 (None)
-                     980 STORE_FAST               8 (e)
-                     982 DELETE_FAST              8 (e)
-                     984 RERAISE                  1
-         
-          64     >>  986 RERAISE                  0
-                 >>  988 COPY                     3
-                     990 POP_EXCEPT
-                     992 RERAISE                  1
+          61         646 LOAD_GLOBAL             28 (ParseError)
+                     658 CHECK_EXC_MATCH
+                     660 POP_JUMP_FORWARD_IF_FALSE   147 (to 956)
+                     662 STORE_FAST               8 (e)
+         
+          66         664 LOAD_GLOBAL             31 (NULL + str)
+                     676 LOAD_FAST                8 (e)
+                     678 PRECALL                  1
+                     682 CALL                     1
+         
+          67         692 LOAD_METHOD              4 (replace)
+                     714 LOAD_CONST              13 ('\x1b[4m')
+                     716 LOAD_CONST              14 ('')
+                     718 PRECALL                  2
+                     722 CALL                     2
+         
+          68         732 LOAD_METHOD              4 (replace)
+                     754 LOAD_CONST              15 ('\x1b[0m')
+                     756 LOAD_CONST              14 ('')
+                     758 PRECALL                  2
+                     762 CALL                     2
+         
+          69         772 LOAD_METHOD              4 (replace)
+                     794 LOAD_GLOBAL             32 (double_quoted_param_left_placeholder)
+                     806 LOAD_CONST              16 ('{{')
+                     808 PRECALL                  2
+                     812 CALL                     2
+         
+          70         822 LOAD_METHOD              4 (replace)
+                     844 LOAD_GLOBAL             34 (double_quoted_param_right_placeholder)
+                     856 LOAD_CONST              17 ('}}')
+                     858 PRECALL                  2
+                     862 CALL                     2
+         
+          65         872 STORE_FAST               9 (error_message)
+         
+          73         874 LOAD_GLOBAL              1 (NULL + re)
+                     886 LOAD_ATTR               18 (sub)
+         
+          74         896 LOAD_CONST              18 ('. Line [0-9]+, Col: [0-9]+.')
+         
+          75         898 LOAD_CONST              19 ('.')
+         
+          76         900 LOAD_FAST                9 (error_message)
+         
+          73         902 PRECALL                  3
+                     906 CALL                     3
+                     916 STORE_FAST               9 (error_message)
+         
+          78         918 LOAD_GLOBAL             39 (NULL + DuneTranslationError)
+                     930 LOAD_FAST                9 (error_message)
+                     932 PRECALL                  1
+                     936 CALL                     1
+                     946 RAISE_VARARGS            1
+                 >>  948 LOAD_CONST              20 (None)
+                     950 STORE_FAST               8 (e)
+                     952 DELETE_FAST              8 (e)
+                     954 RERAISE                  1
+         
+          61     >>  956 RERAISE                  0
+                 >>  958 COPY                     3
+                     960 POP_EXCEPT
+                     962 RERAISE                  1
          ExceptionTable:
-           4 to 670 -> 674 [0]
-           674 to 692 -> 988 [1] lasti
-           694 to 976 -> 978 [1] lasti
-           978 to 986 -> 988 [1] lasti
+           4 to 640 -> 644 [0]
+           644 to 662 -> 958 [1] lasti
+           664 to 946 -> 948 [1] lasti
+           948 to 956 -> 958 [1] lasti
          consts
             'Translate a query using SQLGLot plus custom rules'
             '({{.*?}})'
             ('flags',)
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 19
                code
                   0x970069007c005d127d017401000000000000000000007c01a6010000ab
                   0100000000000000007c0193028c135300
-                33           0 RESUME                   0
+                32           0 RESUME                   0
                              2 BUILD_MAP                0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                18 (to 44)
                              8 STORE_FAST               1 (p)
                             10 LOAD_GLOBAL              1 (NULL + parameter_placeholder)
                             22 LOAD_FAST                1 (p)
                             24 PRECALL                  1
@@ -412,15 +403,15 @@
                consts
                names      ('parameter_placeholder',)
                varnames   ('.0', 'p')
                freevars   ()
                cellvars   ()
                filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/translate.py'
                name       '<dictcomp>'
-               firstlineno 33
+               firstlineno 32
                lnotab 0x
             'trino'
             True
             ('read', 'write', 'pretty')
             0
             'spark'
             'postgres'
@@ -431,27 +422,27 @@
             ''
             '\x1b[0m'
             '{{'
             '}}'
             '. Line [0-9]+, Col: [0-9]+.'
             '.'
             None
-         names      ('re', 'findall', 'IGNORECASE', 'items', 'replace', 'prep_query', 'sqlglot', 'transpile', 'spark_transforms', 'postgres_transforms', 'sql', 'fix_bytearray_param', 'fix_bytearray_lower', 'remove_quotes_around_0x_strings', 'add_warnings_and_banner', 'ParseError', 'str', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'sub', 'DuneTranslationError')
+         names      ('re', 'findall', 'IGNORECASE', 'items', 'replace', 'sqlglot', 'transpile', 'spark_transforms', 'postgres_transforms', 'sql', 'fix_bytearray_param', 'fix_bytearray_lower', 'remove_quotes_around_0x_strings', 'add_warnings_and_banner', 'ParseError', 'str', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'sub', 'DuneTranslationError')
          varnames   ('query', 'sqlglot_dialect', 'dataset', 'parameters', 'parameter_map', 'replace', 'original', 'query_tree', 'e', 'error_message')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/translate.py'
          name       '_translate_query'
-         firstlineno 28
+         firstlineno 27
          lnotab
-            0x020202024201180132012e021e033c030c0120010c022c0120032e0332
-            012e031e011e011e02200212051c0128012801320132fb02081601020102
-            0102fd100526ef
+            0x020202024201180132012e033c030c0120010c022c0120032e0332012e
+            031e011e011e02200212051c0128012801320132fb020816010201020102
+            fd100526ef
       (None,)
-   names      ('re', 'sqlglot', 'ParseError', 'dune.harmonizer.custom_transforms', 'add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'parameter_placeholder', 'postgres_transforms', 'prep_query', 'remove_quotes_around_0x_strings', 'spark_transforms', 'dune.harmonizer.errors', 'DuneTranslationError', '_clean_dataset', '_translate_query')
+   names      ('re', 'sqlglot', 'ParseError', 'dune.harmonizer.custom_transforms', 'add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'parameter_placeholder', 'postgres_transforms', 'remove_quotes_around_0x_strings', 'spark_transforms', 'dune.harmonizer.errors', 'DuneTranslationError', '_clean_dataset', '_translate_query')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/translate.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201080208010c02300c0c030607
+   lnotab 0x00ff0201080208010c022c0b0c030607
```

### Comparing `dune_harmonizer-0.4.0/dune/harmonizer/custom_transforms.py` & `dune_harmonizer-0.4.1/dune/harmonizer/custom_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,26 +276,14 @@
                 "https://dune.com/docs/query/syntax-differences/"
             ),
             read="trino",
         )
     return node
 
 
-def prep_query(query):
-    for keyword in ["replace"]:
-        # use regex to replace the keyword with quotes around it
-        query = re.sub(
-            r"\b" + re.escape(keyword) + r"(?!\()",
-            '"' + keyword + '"',
-            query,
-            flags=re.IGNORECASE,
-        )
-    return query
-
-
 def rename_amount_column(query):
     """Rename the usd_amount column"""
     return sqlglot.parse_one(query.sql(dialect="trino").replace("usd_amount", "amount_usd"), read="trino")
 
 
 def bytea2numeric(node):
     """Replace and warn about bytearray functions"""
```

### Comparing `dune_harmonizer-0.4.0/dune/harmonizer/table_replacements.py` & `dune_harmonizer-0.4.1/dune/harmonizer/table_replacements.py`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.4.0/dune/harmonizer/translate.py` & `dune_harmonizer-0.4.1/dune/harmonizer/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     add_warnings_and_banner,
     double_quoted_param_left_placeholder,
     double_quoted_param_right_placeholder,
     fix_bytearray_lower,
     fix_bytearray_param,
     parameter_placeholder,
     postgres_transforms,
-    prep_query,
     remove_quotes_around_0x_strings,
     spark_transforms,
 )
 from dune.harmonizer.errors import DuneTranslationError
 
 
 def _clean_dataset(dataset):
@@ -30,16 +29,14 @@
     try:
         # Insert placeholders for the parameters we use in Dune (`{{ param }}`), SQLGlot doesn't handle those
         parameters = re.findall("({{.*?}})", query, flags=re.IGNORECASE)
         parameter_map = {parameter_placeholder(p): p for p in parameters}
         for replace, original in parameter_map.items():
             query = query.replace(original, replace)
 
-        query = prep_query(query)
-
         # Transpile to Trino
         query = sqlglot.transpile(query, read=sqlglot_dialect, write="trino", pretty=True)[0]
 
         # Perform custom transformations using SQLGlot's parsed representation
         if sqlglot_dialect == "spark":
             query_tree = spark_transforms(query)
         elif sqlglot_dialect == "postgres":
```

### Comparing `dune_harmonizer-0.4.0/pyproject.toml` & `dune_harmonizer-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dune-harmonizer"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["Vegard Stikbakke <vegard@dune.com>"]
 readme = "README.md"
 packages = [{include = "dune"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dune_harmonizer-0.4.0/PKG-INFO` & `dune_harmonizer-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-harmonizer
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: Vegard Stikbakke
 Author-email: vegard@dune.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlglot (>=11.5.5,<12.0.0)
```

