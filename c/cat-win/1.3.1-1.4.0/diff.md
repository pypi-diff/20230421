# Comparing `tmp/cat_win-1.3.1.tar.gz` & `tmp/cat_win-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cat_win-1.3.1.tar", last modified: Mon Apr 10 10:49:31 2023, max compression
+gzip compressed data, was "cat_win-1.4.0.tar", last modified: Thu Apr 20 22:34:38 2023, max compression
```

## Comparing `cat_win-1.3.1.tar` & `cat_win-1.4.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1090 2023-02-19 10:54:41.226281 cat_win-1.3.1/LICENSE
--rw-r--r--   0        0        0    11362 2023-03-26 12:32:51.928403 cat_win-1.3.1/README.md
--rw-r--r--   0        0        0       39 2023-02-26 11:57:46.261532 cat_win-1.3.1/cat_win/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-02-26 11:57:46.261532 cat_win-1.3.1/cat_win/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2023-02-26 11:57:46.261532 cat_win-1.3.1/cat_win/.pytest_cache/README.md
--rw-r--r--   0        0        0     5653 2023-02-26 11:57:52.638849 cat_win-1.3.1/cat_win/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-02-26 11:57:52.639848 cat_win-1.3.1/cat_win/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      264 2023-04-10 10:25:58.393814 cat_win-1.3.1/cat_win/__init__.py
--rw-r--r--   0        0        0      354 2023-03-10 09:03:40.730873 cat_win-1.3.1/cat_win/__main__.py
--rw-r--r--   0        0        0    27768 2023-04-10 10:48:40.610515 cat_win-1.3.1/cat_win/cat.py
--rw-r--r--   0        0        0     3733 2023-03-27 19:58:37.854304 cat_win-1.3.1/cat_win/const/ArgConstants.py
--rw-r--r--   0        0        0     2258 2023-04-10 10:25:47.873896 cat_win-1.3.1/cat_win/const/ColorConstants.py
--rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.3.1/cat_win/const/__init__.py
--rw-r--r--   0        0        0     8018 2023-03-27 19:59:01.931758 cat_win-1.3.1/cat_win/persistence/Config.py
--rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.3.1/cat_win/persistence/__init__.py
--rw-r--r--   0        0        0        0 2023-02-19 10:54:41.304282 cat_win-1.3.1/cat_win/tests/__init__.py
--rw-r--r--   0        0        0     1147 2023-03-27 19:59:24.939031 cat_win-1.3.1/cat_win/tests/test_ArgConstants.py
--rw-r--r--   0        0        0     7330 2023-03-27 19:59:45.680091 cat_win-1.3.1/cat_win/tests/test_ArgParser.py
--rw-r--r--   0        0        0     1176 2023-03-27 19:59:53.853442 cat_win-1.3.1/cat_win/tests/test_Base64.py
--rw-r--r--   0        0        0     3703 2023-03-27 20:00:47.420987 cat_win-1.3.1/cat_win/tests/test_Converter.py
--rw-r--r--   0        0        0      906 2023-04-06 12:21:45.835140 cat_win-1.3.1/cat_win/tests/test_File.py
--rw-r--r--   0        0        0     1403 2023-03-27 20:01:02.041966 cat_win-1.3.1/cat_win/tests/test_FileAttributes.py
--rw-r--r--   0        0        0     4384 2023-04-06 12:13:16.999006 cat_win-1.3.1/cat_win/tests/test_Holder.py
--rw-r--r--   0        0        0     7079 2023-03-27 20:01:53.177345 cat_win-1.3.1/cat_win/tests/test_RawViewer.py
--rw-r--r--   0        0        0      386 2023-03-27 20:02:00.130018 cat_win-1.3.1/cat_win/tests/test_StdInHelper.py
--rw-r--r--   0        0        0     3199 2023-03-27 20:02:08.299116 cat_win-1.3.1/cat_win/tests/test_StringFinder.py
--rw-r--r--   0        0        0     3972 2023-03-27 20:02:15.478171 cat_win-1.3.1/cat_win/tests/test_UpdateChecker.py
--rw-r--r--   0        0        0     5829 2023-04-10 10:25:32.430203 cat_win-1.3.1/cat_win/tests/test_cat.py
--rw-r--r--   0        0        0     1622 2023-03-27 20:00:37.654265 cat_win-1.3.1/cat_win/tests/test_checksum.py
--rw-r--r--   0        0        0     6600 2023-03-27 20:01:23.311198 cat_win-1.3.1/cat_win/tests/test_full.py
--rw-r--r--   0        0        0      170 2023-02-19 10:54:41.307281 cat_win-1.3.1/cat_win/tests/texts/full_test_result_B.txt
--rw-r--r--   0        0        0      196 2023-02-19 10:54:41.307281 cat_win-1.3.1/cat_win/tests/texts/full_test_result_C.txt
--rw-r--r--   0        0        0      139 2023-02-19 10:54:41.308281 cat_win-1.3.1/cat_win/tests/texts/full_test_result_D.txt
--rw-r--r--   0        0        0      189 2023-02-19 10:54:41.308281 cat_win-1.3.1/cat_win/tests/texts/test.txt
--rw-r--r--   0        0        0        0 2023-03-26 11:37:07.806578 cat_win-1.3.1/cat_win/tests/texts/test_empty.txt
--rw-r--r--   0        0        0       19 2023-02-19 10:54:41.308281 cat_win-1.3.1/cat_win/tests/texts/test_holderEdgeCase_1.txt
--rw-r--r--   0        0        0       21 2023-02-19 10:54:41.308281 cat_win-1.3.1/cat_win/tests/texts/test_holderEdgeCase_2.txt
--rw-r--r--   0        0        0       28 2023-03-26 12:18:11.309629 cat_win-1.3.1/cat_win/tests/texts/test_holderEdgeCase_3.txt
--rw-r--r--   0        0        0       10 2023-02-22 11:49:01.641263 cat_win-1.3.1/cat_win/tests/texts/test_holderEdgeCase_4.txt
--rw-r--r--   0        0        0       62 2023-03-26 12:18:56.747176 cat_win-1.3.1/cat_win/tests/texts/test_peek.txt
--rw-r--r--   0        0        0     4269 2023-03-27 20:02:42.432245 cat_win-1.3.1/cat_win/util/ArgParser.py
--rw-r--r--   0        0        0     2829 2023-02-25 11:27:08.471904 cat_win-1.3.1/cat_win/util/Base64.py
--rw-r--r--   0        0        0     3104 2023-02-25 11:32:26.664586 cat_win-1.3.1/cat_win/util/Converter.py
--rw-r--r--   0        0        0      331 2023-04-06 12:14:05.915760 cat_win-1.3.1/cat_win/util/File.py
--rw-r--r--   0        0        0     3780 2023-04-05 14:29:14.761170 cat_win-1.3.1/cat_win/util/FileAttributes.py
--rw-r--r--   0        0        0     5555 2023-04-06 12:08:56.673409 cat_win-1.3.1/cat_win/util/Holder.py
--rw-r--r--   0        0        0     1999 2023-03-25 22:48:31.614578 cat_win-1.3.1/cat_win/util/RawViewer.py
--rw-r--r--   0        0        0     5971 2023-04-10 10:48:36.074958 cat_win-1.3.1/cat_win/util/StdInHelper.py
--rw-r--r--   0        0        0     3740 2023-03-27 20:03:53.006577 cat_win-1.3.1/cat_win/util/StringFinder.py
--rw-r--r--   0        0        0      389 2023-02-19 10:54:41.299281 cat_win-1.3.1/cat_win/util/TmpFileHelper.py
--rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.3.1/cat_win/util/__init__.py
--rw-r--r--   0        0        0     1620 2023-03-27 20:02:51.793512 cat_win-1.3.1/cat_win/util/checksum.py
--rw-r--r--   0        0        0     5585 2023-03-29 11:31:31.822808 cat_win-1.3.1/cat_win/web/UpdateChecker.py
--rw-r--r--   0        0        0        0 2023-02-23 20:58:12.051941 cat_win-1.3.1/cat_win/web/__init__.py
--rw-r--r--   0        0        0     1355 2023-03-25 23:10:16.240600 cat_win-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    12210 1970-01-01 00:00:00.000000 cat_win-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-02-19 10:54:41.226281 cat_win-1.4.0/LICENSE
+-rw-r--r--   0        0        0    12243 2023-04-19 11:11:16.578516 cat_win-1.4.0/README.md
+-rw-r--r--   0        0        0       39 2023-02-26 11:57:46.261532 cat_win-1.4.0/cat_win/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-02-26 11:57:46.261532 cat_win-1.4.0/cat_win/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-02-26 11:57:46.261532 cat_win-1.4.0/cat_win/.pytest_cache/README.md
+-rw-r--r--   0        0        0     5653 2023-02-26 11:57:52.638849 cat_win-1.4.0/cat_win/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-02-26 11:57:52.639848 cat_win-1.4.0/cat_win/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      289 2023-04-20 12:34:28.496799 cat_win-1.4.0/cat_win/__init__.py
+-rw-r--r--   0        0        0      344 2023-04-11 08:42:55.435968 cat_win-1.4.0/cat_win/__main__.py
+-rw-r--r--   0        0        0    29624 2023-04-20 22:27:04.760434 cat_win-1.4.0/cat_win/cat.py
+-rw-r--r--   0        0        0     3869 2023-04-14 08:51:24.082968 cat_win-1.4.0/cat_win/const/ArgConstants.py
+-rw-r--r--   0        0        0     2316 2023-04-12 15:55:33.141057 cat_win-1.4.0/cat_win/const/ColorConstants.py
+-rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.0/cat_win/const/__init__.py
+-rw-r--r--   0        0        0     8018 2023-04-12 15:54:59.223056 cat_win-1.4.0/cat_win/persistence/Config.py
+-rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.0/cat_win/persistence/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:54:41.304282 cat_win-1.4.0/cat_win/tests/__init__.py
+-rw-r--r--   0        0        0     1147 2023-03-27 19:59:24.939031 cat_win-1.4.0/cat_win/tests/test_ArgConstants.py
+-rw-r--r--   0        0        0     7330 2023-03-27 19:59:45.680091 cat_win-1.4.0/cat_win/tests/test_ArgParser.py
+-rw-r--r--   0        0        0     1176 2023-03-27 19:59:53.853442 cat_win-1.4.0/cat_win/tests/test_Base64.py
+-rw-r--r--   0        0        0     3703 2023-03-27 20:00:47.420987 cat_win-1.4.0/cat_win/tests/test_Converter.py
+-rw-r--r--   0        0        0      906 2023-04-06 12:21:45.835140 cat_win-1.4.0/cat_win/tests/test_File.py
+-rw-r--r--   0        0        0     1403 2023-03-27 20:01:02.041966 cat_win-1.4.0/cat_win/tests/test_FileAttributes.py
+-rw-r--r--   0        0        0     4384 2023-04-06 12:13:16.999006 cat_win-1.4.0/cat_win/tests/test_Holder.py
+-rw-r--r--   0        0        0     7161 2023-04-13 19:54:00.253510 cat_win-1.4.0/cat_win/tests/test_RawViewer.py
+-rw-r--r--   0        0        0      386 2023-03-27 20:02:00.130018 cat_win-1.4.0/cat_win/tests/test_StdInHelper.py
+-rw-r--r--   0        0        0     3199 2023-03-27 20:02:08.299116 cat_win-1.4.0/cat_win/tests/test_StringFinder.py
+-rw-r--r--   0        0        0     3972 2023-03-27 20:02:15.478171 cat_win-1.4.0/cat_win/tests/test_UpdateChecker.py
+-rw-r--r--   0        0        0     5829 2023-04-10 10:25:32.430203 cat_win-1.4.0/cat_win/tests/test_cat.py
+-rw-r--r--   0        0        0     1622 2023-03-27 20:00:37.654265 cat_win-1.4.0/cat_win/tests/test_checksum.py
+-rw-r--r--   0        0        0     6600 2023-04-14 08:29:10.170716 cat_win-1.4.0/cat_win/tests/test_full.py
+-rw-r--r--   0        0        0      170 2023-02-19 10:54:41.307281 cat_win-1.4.0/cat_win/tests/texts/full_test_result_B.txt
+-rw-r--r--   0        0        0      196 2023-02-19 10:54:41.307281 cat_win-1.4.0/cat_win/tests/texts/full_test_result_C.txt
+-rw-r--r--   0        0        0      139 2023-02-19 10:54:41.308281 cat_win-1.4.0/cat_win/tests/texts/full_test_result_D.txt
+-rw-r--r--   0        0        0      189 2023-02-19 10:54:41.308281 cat_win-1.4.0/cat_win/tests/texts/test.txt
+-rw-r--r--   0        0        0        0 2023-03-26 11:37:07.806578 cat_win-1.4.0/cat_win/tests/texts/test_empty.txt
+-rw-r--r--   0        0        0       19 2023-02-19 10:54:41.308281 cat_win-1.4.0/cat_win/tests/texts/test_holderEdgeCase_1.txt
+-rw-r--r--   0        0        0       21 2023-02-19 10:54:41.308281 cat_win-1.4.0/cat_win/tests/texts/test_holderEdgeCase_2.txt
+-rw-r--r--   0        0        0       28 2023-03-26 12:18:11.309629 cat_win-1.4.0/cat_win/tests/texts/test_holderEdgeCase_3.txt
+-rw-r--r--   0        0        0       10 2023-02-22 11:49:01.641263 cat_win-1.4.0/cat_win/tests/texts/test_holderEdgeCase_4.txt
+-rw-r--r--   0        0        0       62 2023-03-26 12:18:56.747176 cat_win-1.4.0/cat_win/tests/texts/test_peek.txt
+-rw-r--r--   0        0        0     4319 2023-04-12 15:45:05.960051 cat_win-1.4.0/cat_win/util/ArgParser.py
+-rw-r--r--   0        0        0     2767 2023-04-14 08:30:01.328140 cat_win-1.4.0/cat_win/util/Base64.py
+-rw-r--r--   0        0        0     3104 2023-02-25 11:32:26.664586 cat_win-1.4.0/cat_win/util/Converter.py
+-rw-r--r--   0        0        0      331 2023-04-06 12:14:05.915760 cat_win-1.4.0/cat_win/util/File.py
+-rw-r--r--   0        0        0     3917 2023-04-16 10:54:57.990970 cat_win-1.4.0/cat_win/util/FileAttributes.py
+-rw-r--r--   0        0        0     5729 2023-04-14 08:24:12.581241 cat_win-1.4.0/cat_win/util/Holder.py
+-rw-r--r--   0        0        0     2706 2023-04-19 12:44:27.293437 cat_win-1.4.0/cat_win/util/RawViewer.py
+-rw-r--r--   0        0        0     6520 2023-04-19 17:28:53.675269 cat_win-1.4.0/cat_win/util/StdInHelper.py
+-rw-r--r--   0        0        0     3724 2023-04-12 15:28:42.676941 cat_win-1.4.0/cat_win/util/StringFinder.py
+-rw-r--r--   0        0        0      389 2023-02-19 10:54:41.299281 cat_win-1.4.0/cat_win/util/TmpFileHelper.py
+-rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.0/cat_win/util/__init__.py
+-rw-r--r--   0        0        0     1614 2023-04-12 15:36:43.277060 cat_win-1.4.0/cat_win/util/checksum.py
+-rw-r--r--   0        0        0     5585 2023-03-29 11:31:31.822808 cat_win-1.4.0/cat_win/web/UpdateChecker.py
+-rw-r--r--   0        0        0        0 2023-02-23 20:58:12.051941 cat_win-1.4.0/cat_win/web/__init__.py
+-rw-r--r--   0        0        0     1552 2023-04-14 15:23:59.559474 cat_win-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    13244 1970-01-01 00:00:00.000000 cat_win-1.4.0/PKG-INFO
```

### Comparing `cat_win-1.3.1/LICENSE` & `cat_win-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/README.md` & `cat_win-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -61,16 +61,16 @@
    </ol>
 </details>
 
 ## About The Project
 
 [![Unittests]](https://github.com/SilenZcience/cat_win/actions/workflows/unit_test.yml)
 [![Build-and-Check]](https://github.com/SilenZcience/cat_win/actions/workflows/package_test.yml)
-[![Coverage]]()
-[![Tests]]()
+[![Coverage]](https://raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-coverage.svg)
+[![Tests]](https://raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-tests.svg)
 <!-- [![Compile-and-Push]](https://github.com/SilenZcience/cat_win/actions/workflows/build_executable.yml/badge.svg) -->
 
 This project copies the fundamental framework of the cat command-line tool from Linux and translates its features to an OS Independent program using Python. </br> Over time the project evolved in subject areas of other tools like 'echo', 'grep', 'ls', 'base64'.
 
 Additionally it includes the feature to strip and reverse the content of any given file, make use of the standard-input, which enables cat piping into each other, generating the checksum of any file, converting decimal, hexadecimal and binary numbers within any text, and much <a href="#usage">more</a> ...
 
 Contrary to the name of the project it is of course possible to use cat_win on Linux or MacOS!
@@ -119,62 +119,63 @@
 ```console
 catw [FILE]... [OPTION]...
 catw --help
 ```
 
 > ⚠️ *from v1.0.33 to v1.1.0 the entrypoint changes from `cat` to `catw`. If you wish to keep the old command, you will have to define an alias yourself.*
 
-| Argument / Option      | Description                                       |
-|------------------------|---------------------------------------------------|
-| *-h, --help*           | show help message and exit                        |
-| *-v, --version*        | output version information                        |
-| *-d, --debug*          | show debug information                            |
-|                        |                                                   |
-| *-n, --number*         | number all output lines                           |
-| *-l, --linelength*     | display the length of each line                   |
-| *-e, --ends*           | display $ at the end of each line                 |
-| *-t, --tabs*           | display TAB characters as ^I                      |
-| *--eof, --eof*         | display EOF characters as ^EOF                    |
-| *-u, --unique*         | suppress repeated output lines                    |
-| *-b, --blank*          | hide empty lines                                  |
-| *-r, --reverse*        | reverse output                                    |
-| *-p, --peek*           | only print the first and last lines               |
-| *-s, --sum*            | show sum of lines                                 |
-| *-S, --SUM*            | ONLY show sum of lines                            |
-| *-f, --files*          | list applied files                                |
-| *-F, --FILES*          | ONLY list applied files and file sizes            |
-| *-g, --grep*           | only show lines containing queried keywords       |
-| *-i, --interactive*    | use stdin                                         |
-| *-o, --oneline*        | take only the first stdin-line                    |
-| *-E, --ECHO*           | handle every following parameter as stdin         |
-| *-c, --clip*           | copy output to clipboard                          |
-| *-m, --checksum*       | show the checksums of all files                   |
-| *-a, --attributes*     | show meta-information about the files             |
-|                        |                                                   |
-| *--dec, --DEC*         | convert decimal numbers to hexadecimal and binary |
-| *--hex, --HEX*         | convert hexadecimal numbers to decimal and binary |
-| *--bin, --BIN*         | convert binary numbers to decimal and hexadecimal |
-| *--b64e, --b64e*       | encode the input to base64                        |
-| *--b64d, --b64d*       | decode the input from base64                      |
-|                        |                                                   |
-| *--hexview, --HEXVIEW* | display the raw byte representation in hexadecimal|
-| *--binview, --binview* | display the raw byte representation in binary     |
-|                        |                                                   |
-| *--nc, --nocolor*      | disable colored output                            |
-| *--nb, --nobreak*      | do not interrupt the output on queried keywords   |
-| *--nk, --nokeyword*    | inverse the grep output                           |
-| *--config, --config*   | change color configuration                        |
-|                        |                                                   |
-| *enc=X*                | set file enconding to X (default is utf-8)        |
-| *find=X*               | find/query a substring X in the given files       |
-| *match=X*              | find/query a pattern X in the given files         |
-| *trunc=X:Y*            | truncate file to lines X and Y (python-like)      |
-|                        |                                                   |
-| *[a,b]*                | replace a with b in every line                    |
-| *[a:​b:c]*              | python-like string indexing syntax (line by line) |
+| Argument / Option      | Description                                               |
+|------------------------|-----------------------------------------------------------|
+| *-h, --help*           | show help message and exit                                |
+| *-v, --version*        | output version information                                |
+| *-d, --debug*          | show debug information                                    |
+|                        |                                                           |
+| *-n, --number*         | number all output lines                                   |
+| *-l, --linelength*     | display the length of each line                           |
+| *-e, --ends*           | display $ at the end of each line                         |
+| *-t, --tabs*           | display TAB characters as ^I                              |
+| *--eof, --eof*         | display EOF characters as ^EOF                            |
+| *-u, --unique*         | suppress repeated output lines                            |
+| *-b, --blank*          | hide empty lines                                          |
+| *-r, --reverse*        | reverse output                                            |
+| *-p, --peek*           | only print the first and last lines                       |
+| *-s, --sum*            | show sum of lines                                         |
+| *-S, --SUM*            | ONLY show sum of lines                                    |
+| *-f, --files*          | list applied files                                        |
+| *-F, --FILES*          | ONLY list applied files and file sizes                    |
+| *-g, --grep*           | only show lines containing queried keywords               |
+| *-i, --interactive*    | use stdin                                                 |
+| *-o, --oneline*        | take only the first stdin-line                            |
+| *-E, --ECHO*           | handle every following parameter as stdin                 |
+| *-c, --clip*           | copy output to clipboard                                  |
+| *-m, --checksum*       | show the checksums of all files                           |
+| *-a, --attributes*     | show meta-information about the files                     |
+|                        |                                                           |
+| *--dec, --DEC*         | convert decimal numbers to hexadecimal and binary         |
+| *--hex, --HEX*         | convert hexadecimal numbers to decimal and binary         |
+| *--bin, --BIN*         | convert binary numbers to decimal and hexadecimal         |
+| *--b64e, --b64e*       | encode the input to base64                                |
+| *--b64d, --b64d*       | decode the input from base64                              |
+|                        |                                                           |
+| *--hexview, --HEXVIEW* | display the raw byte representation in hexadecimal        |
+| *--binview, --binview* | display the raw byte representation in binary             |
+|                        |                                                           |
+| *--nc, --nocolor*      | disable colored output                                    |
+| *--nb, --nobreak*      | do not interrupt the output on queried keywords           |
+| *--nk, --nokeyword*    | inverse the grep output                                   |
+| *-R, --reconfigure*    | reconfigure the stdin and stdout with the parsed encoding |
+| *--config, --config*   | change color configuration                                |
+|                        |                                                           |
+| *enc=X*                | set file enconding to X (default is utf-8)                |
+| *find=X*               | find/query a substring X in the given files               |
+| *match=X*              | find/query a pattern X in the given files                 |
+| *trunc=X:Y*            | truncate file to lines X and Y (python-like)              |
+|                        |                                                           |
+| *[a,b]*                | replace a with b in every line                            |
+| *[a:​b:c]*              | python-like string indexing syntax (line by line)         |
 
 ### Examples
 
 <details open>
 	<summary><b>📂 Images 📂</b></summary>
 
 ![Example1](https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example1.png "example1")
@@ -192,14 +193,23 @@
 </details>
 
 ```console
 $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1] -ln
 > 1) [8] ): dlroW
 ```
 
+```c
+$ cats --dec -nl
+> >>> 12345
+> 1) [53] 12345 {Hexadecimal: 0x3039; Binary: 0b11000000111001}
+> >>> 54321
+> 2) [55] 54321 {Hexadecimal: 0xd431; Binary: 0b1101010000110001}
+> ...
+```
+
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Changelog
 
 Take a look at the [Changelog](https://github.com/SilenZcience/cat_win/blob/main/CHANGELOG.md) file.
 
 ## License
@@ -215,16 +225,16 @@
 [OS-Linux]: https://svgshare.com/i/Zhy.svg
 [OS-MacOS]: https://svgshare.com/i/ZjP.svg
 
 [Unittests]: https://github.com/SilenZcience/cat_win/actions/workflows/unit_test.yml/badge.svg
 [Build-and-Check]: https://github.com/SilenZcience/cat_win/actions/workflows/package_test.yml/badge.svg
 [Compile-and-Push]: https://github.com/SilenZcience/cat_win/actions/workflows/build_executable.yml/badge.svg
 
-[Coverage]: https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/badge-coverage.svg
-[Tests]: https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/badge-tests.svg
+[Coverage]: https://raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-coverage.svg
+[Tests]: https://raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-tests.svg
 
 [MadeWith-Python]: https://img.shields.io/badge/Made%20with-Python-brightgreen
 [Python-Version]: https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20pypy--3.8%20%7C%20pypy--3.9-blue
 
 [CurrentVersion]: https://img.shields.io/pypi/v/cat_win.svg
 
 [GitHub-SilenZcience]: https://img.shields.io/badge/GitHub-SilenZcience-orange
```

#### html2text {}

```diff
@@ -17,25 +17,28 @@
    3. Usage
           o Examples
    4. Changelog
    5. License
    6. Contact
  ## About The Project [![Unittests]](https://github.com/SilenZcience/cat_win/
 actions/workflows/unit_test.yml) [![Build-and-Check]](https://github.com/
-SilenZcience/cat_win/actions/workflows/package_test.yml) [![Coverage]]() [!
-[Tests]]()  This project copies the fundamental framework of the cat command-
-line tool from Linux and translates its features to an OS Independent program
-using Python.  Over time the project evolved in subject areas of other tools
-like 'echo', 'grep', 'ls', 'base64'. Additionally it includes the feature to
-strip and reverse the content of any given file, make use of the standard-
-input, which enables cat piping into each other, generating the checksum of any
-file, converting decimal, hexadecimal and binary numbers within any text, and
-much more ... Contrary to the name of the project it is of course possible to
-use cat_win on Linux or MacOS! ### Made With [![MadeWith-Python]](https://
-www.python.org/) [![Python][Python-Version]](https://www.python.org/)
+SilenZcience/cat_win/actions/workflows/package_test.yml) [![Coverage]](https://
+raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-
+coverage.svg) [![Tests]](https://raw.githubusercontent.com/SilenZcience/
+cat_win/badges/.github/badges/badge-tests.svg)  This project copies the
+fundamental framework of the cat command-line tool from Linux and translates
+its features to an OS Independent program using Python.  Over time the project
+evolved in subject areas of other tools like 'echo', 'grep', 'ls', 'base64'.
+Additionally it includes the feature to strip and reverse the content of any
+given file, make use of the standard-input, which enables cat piping into each
+other, generating the checksum of any file, converting decimal, hexadecimal and
+binary numbers within any text, and much more ... Contrary to the name of the
+project it is of course possible to use cat_win on Linux or MacOS! ### Made
+With [![MadeWith-Python]](https://www.python.org/) [![Python][Python-Version]]
+(https://www.python.org/)
                                                                   (back_to_top)
 ## Getting Started ### Prerequisites - Using cat_win as a Python-Package
 demands a Python-Interpreter (>= 3.7). - Using cat_win as an Executable
 (Windows only!) demands no prerequisites, hereby the stand-alone executable
 `catw.exe` is sufficient. ### Installation [![Version][CurrentVersion]](https:/
 /pypi.org/project/cat-win/) Simply install the python package (via [PyPI-
 cat_win](https://pypi.org/project/cat-win/)): ```console python -m pip install
@@ -56,16 +59,16 @@
 corresponding [workflow](https://github.com/SilenZcience/cat_win/blob/
 main/.github/workflows/build_executable.yml) used.
                                                                   (back_to_top)
 ## Usage ```console catw [FILE]... [OPTION]... catw --help ``` > â ï¸ *from
 v1.0.33 to v1.1.0 the entrypoint changes from `cat` to `catw`. If you wish to
 keep the old command, you will have to define an alias yourself.* | Argument /
 Option | Description | |------------------------|------------------------------
----------------------| | *-h, --help* | show help message and exit | | *-v, --
-version* | output version information | | *-d, --debug* | show debug
+-----------------------------| | *-h, --help* | show help message and exit | |
+*-v, --version* | output version information | | *-d, --debug* | show debug
 information | | | | | *-n, --number* | number all output lines | | *-l, --
 linelength* | display the length of each line | | *-e, --ends* | display $ at
 the end of each line | | *-t, --tabs* | display TAB characters as ^I | | *--
 eof, --eof* | display EOF characters as ^EOF | | *-u, --unique* | suppress
 repeated output lines | | *-b, --blank* | hide empty lines | | *-r, --reverse*
 | reverse output | | *-p, --peek* | only print the first and last lines | | *-
 s, --sum* | show sum of lines | | *-S, --SUM* | ONLY show sum of lines | | *-f,
@@ -76,47 +79,51 @@
 c, --clip* | copy output to clipboard | | *-m, --checksum* | show the checksums
 of all files | | *-a, --attributes* | show meta-information about the files | |
 | | | *--dec, --DEC* | convert decimal numbers to hexadecimal and binary | | *-
 -hex, --HEX* | convert hexadecimal numbers to decimal and binary | | *--bin, --
 BIN* | convert binary numbers to decimal and hexadecimal | | *--b64e, --b64e* |
 encode the input to base64 | | *--b64d, --b64d* | decode the input from base64
 | | | | | *--hexview, --HEXVIEW* | display the raw byte representation in
-hexadecimal| | *--binview, --binview* | display the raw byte representation in
+hexadecimal | | *--binview, --binview* | display the raw byte representation in
 binary | | | | | *--nc, --nocolor* | disable colored output | | *--nb, --
 nobreak* | do not interrupt the output on queried keywords | | *--nk, --
-nokeyword* | inverse the grep output | | *--config, --config* | change color
-configuration | | | | | *enc=X* | set file enconding to X (default is utf-8) |
-| *find=X* | find/query a substring X in the given files | | *match=X* | find/
-query a pattern X in the given files | | *trunc=X:Y* | truncate file to lines X
-and Y (python-like) | | | | | *[a,b]* | replace a with b in every line | | *[a:
-âb:c]* | python-like string indexing syntax (line by line) | ### Examples
-ð Images ð ![Example1](https://raw.githubusercontent.com/SilenZcience/
-cat_win/main/img/example1.png "example1") ![Example2](https://
+nokeyword* | inverse the grep output | | *-R, --reconfigure* | reconfigure the
+stdin and stdout with the parsed encoding | | *--config, --config* | change
+color configuration | | | | | *enc=X* | set file enconding to X (default is
+utf-8) | | *find=X* | find/query a substring X in the given files | | *match=X*
+| find/query a pattern X in the given files | | *trunc=X:Y* | truncate file to
+lines X and Y (python-like) | | | | | *[a,b]* | replace a with b in every line
+| | *[a:âb:c]* | python-like string indexing syntax (line by line) | ###
+Examples  ð Images ð ![Example1](https://raw.githubusercontent.com/
+SilenZcience/cat_win/main/img/example1.png "example1") ![Example2](https://
 raw.githubusercontent.com/SilenZcience/cat_win/main/img/example2.png
 "example2") ![Example3](https://raw.githubusercontent.com/SilenZcience/cat_win/
 main/img/example3.png "example3") ![Example4](https://
 raw.githubusercontent.com/SilenZcience/cat_win/main/img/example4.png
 "example4") ![Example5](https://raw.githubusercontent.com/SilenZcience/cat_win/
 main/img/example5.png "example5") ![Example6](https://
 raw.githubusercontent.com/SilenZcience/cat_win/main/img/example6.png
 "example6")  ```console $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1]
--ln > 1) [8] ): dlroW ```
+-ln > 1) [8] ): dlroW ``` ```c $ cats --dec -nl > >>> 12345 > 1) [53] 12345
+{Hexadecimal: 0x3039; Binary: 0b11000000111001} > >>> 54321 > 2) [55] 54321
+{Hexadecimal: 0xd431; Binary: 0b1101010000110001} > ... ```
                                                                   (back_to_top)
 ## Changelog Take a look at the [Changelog](https://github.com/SilenZcience/
 cat_win/blob/main/CHANGELOG.md) file. ## License This project is licensed under
 the MIT License - see the [LICENSE](https://github.com/SilenZcience/cat_win/
 blob/main/LICENSE) file for details ## Contact > **SilenZcience**
 [![GitHub-SilenZcience][GitHub-SilenZcience]](https://github.com/SilenZcience)
 [OS-Windows]: https://svgshare.com/i/ZhY.svg [OS-Linux]: https://svgshare.com/
 i/Zhy.svg [OS-MacOS]: https://svgshare.com/i/ZjP.svg [Unittests]: https://
 github.com/SilenZcience/cat_win/actions/workflows/unit_test.yml/badge.svg
 [Build-and-Check]: https://github.com/SilenZcience/cat_win/actions/workflows/
 package_test.yml/badge.svg [Compile-and-Push]: https://github.com/SilenZcience/
 cat_win/actions/workflows/build_executable.yml/badge.svg [Coverage]: https://
-raw.githubusercontent.com/SilenZcience/cat_win/main/img/badge-coverage.svg
-[Tests]: https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/badge-
-tests.svg [MadeWith-Python]: https://img.shields.io/badge/Made%20with-Python-
-brightgreen [Python-Version]: https://img.shields.io/badge/Python-
+raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-
+coverage.svg [Tests]: https://raw.githubusercontent.com/SilenZcience/cat_win/
+badges/.github/badges/badge-tests.svg [MadeWith-Python]: https://
+img.shields.io/badge/Made%20with-Python-brightgreen [Python-Version]: https://
+img.shields.io/badge/Python-
 3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20pypy--
 3.8%20%7C%20pypy--3.9-blue [CurrentVersion]: https://img.shields.io/pypi/v/
 cat_win.svg [GitHub-SilenZcience]: https://img.shields.io/badge/GitHub-
 SilenZcience-orange
```

### Comparing `cat_win-1.3.1/cat_win/.pytest_cache/v/cache/nodeids` & `cat_win-1.4.0/cat_win/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/cat.py` & `cat_win-1.4.0/cat_win/cat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 try:
     from colorama import init as coloramaInit
 except ImportError:
     nop = lambda *_, **__: None; coloramaInit = nop
 from datetime import datetime
 from functools import lru_cache
 from itertools import groupby
+from platform import system
 from re import sub as resub
 import os
 import sys
 
 from cat_win.const.ArgConstants import *
 from cat_win.const.ColorConstants import C_KW
 from cat_win.util.Base64 import decodeBase64, encodeBase64
@@ -20,32 +21,34 @@
 import cat_win.util.checksum as checksum
 import cat_win.util.Converter as Converter
 import cat_win.util.Holder as Holder
 import cat_win.util.StdInHelper as StdInHelper
 import cat_win.util.StringFinder as StringFinder
 import cat_win.util.TmpFileHelper as TmpFileHelper
 
-from cat_win import __version__, __sysversion__, __author__, __url__
+from cat_win import __project__, __version__, __sysversion__, __author__, __url__
 workingDir = os.path.dirname(os.path.realpath(__file__))
 
 coloramaInit()
 config = Config.Config(workingDir)
 
 color_dic = config.loadConfig()
 
 converter = Converter.Converter()
 holder = Holder.Holder()
 tmpFileHelper = TmpFileHelper.TmpFileHelper()
 
+on_windows_os = (system() == 'Windows')
+
 def exception_handler(exception_type: type, exception, traceback, debug_hook=sys.excepthook) -> None:
     print(color_dic[C_KW.RESET_ALL])
     if holder.args_id[ARGS_DEBUG]:
         debug_hook(exception_type, exception, traceback)
         return
-    print(f"\nError: {exception_type.__name__} {exception}")
+    print(f"\n{exception_type.__name__}{':' * bool(str(exception))} {exception}")
     if exception_type != KeyboardInterrupt:
         print(f"If this Exception is unexpected, please raise an official Issue at:\n{__url__}/issues")
 
 
 sys.excepthook = exception_handler
 
 
@@ -67,15 +70,15 @@
     helpMessage += f"\t{'[a:b:c]': <25}python-like string indexing syntax (line by line)\n"
     helpMessage += '\n'
     helpMessage += 'Examples:\n'
     helpMessage += f"\t{'cat f g -r' : <25}Output g's contents in reverse order, then f's content in reverse order\n"
     helpMessage += f"\t{'cat f g -ne': <25}Output f's, then g's content, while numerating and showing the end of lines\n"
     helpMessage += f"\t{'cat f trunc=a:b:c': <25}Output f's content starting at line a, ending at line b, stepping c\n"
     print(helpMessage)
-    printUpdateInformation('cat_win', __version__, color_dic)
+    printUpdateInformation(__project__, __version__, color_dic)
 
 
 def _showVersion() -> None:
     """
     Show the Version message and exit.
     """
     catVersion = f"Catw {__version__} - from {workingDir}\n"
@@ -87,15 +90,15 @@
     versionMessage += f"Built with: \tPython {__sysversion__}\n"  # sys.version
     try:
         versionMessage += f"Install time: \t{datetime.fromtimestamp(os.path.getctime(os.path.realpath(__file__)))}\n"
     except OSError: # fails on pyinstaller executable
         versionMessage += f"Install time: \t-\n"
     versionMessage += f"Author: \t{__author__}\n"
     print(versionMessage)
-    printUpdateInformation('cat_win', __version__, color_dic)
+    printUpdateInformation(__project__, __version__, color_dic)
 
 
 def _showDebug(args: list, unknown_args: list, known_files: list, unknown_files: list, echo_args: list) -> None:
     """
     Print all neccassary debug information
     """
     print('Debug Information:')
@@ -130,57 +133,51 @@
         print(f"{color_dic[C_KW.COUNT_AND_FILES]}{'File': <{longestFileName}}LineCount{color_dic[C_KW.RESET_ALL]}")
         for file in holder.allFilesLines.keys():
             print(f"{color_dic[C_KW.COUNT_AND_FILES]}{file: <{longestFileName}}{holder.allFilesLines[file]: >{holder.fileLineNumberPlaceHolder}}{color_dic[C_KW.RESET_ALL]}")
         print('')
     print(f"{color_dic[C_KW.COUNT_AND_FILES]}Lines (Sum): {holder.allFilesLinesSum}{color_dic[C_KW.RESET_ALL]}")
 
 
-def _showFiles(files: list = None) -> None:
+def _showFiles() -> None:
     """
-    displays files including their size and calculates
+    displays holder.files including their size and calculates
     their size sum.
-    
-    Parameters:
-    files (list):
-        all files to display, a list containing File objects,
-        the files inside the holder object if None
-    """
-    if files == None:
-        files = holder.files
-    if len(files) == 0:
+    """
+    if len(holder.files) == 0:
         return
     file_sizes = []
     msg = 'found' if holder.args_id[ARGS_FFILES] else 'applied'
     print(color_dic[C_KW.COUNT_AND_FILES], end='')
     print(f"{msg} FILE(s):", end='')
     print(color_dic[C_KW.RESET_ALL])
-    for file in files:
+    for file in holder.files:
         size = getFileSize(file.path)
         file_sizes.append(size)
         print(f"\t{color_dic[C_KW.COUNT_AND_FILES]}{_convert_size(size): <10}{'*' if file.containsQueried else ' '}{file.displayname}{color_dic[C_KW.RESET_ALL]}")
     print(color_dic[C_KW.COUNT_AND_FILES], end='')
     print(f"Sum:\t{_convert_size(sum(file_sizes))}", end='')
     print(color_dic[C_KW.RESET_ALL])
     print(color_dic[C_KW.COUNT_AND_FILES], end='')
-    print(f"Amount:\t{len(files)}", end='')
+    print(f"Amount:\t{len(holder.files)}", end='')
     print(color_dic[C_KW.RESET_ALL])
 
 
 def _printMeta(file: str) -> None:
     """
     print the information retrieved by getFileMetaData()
     
     Parameters:
     file (str):
         a string representation of a file (-path)
     """
-    metaData = getFileMetaData(file, [color_dic[C_KW.RESET_ALL],
-                                      color_dic[C_KW.ATTRIB],
-                                      color_dic[C_KW.ATTRIB_POSITIVE],
-                                      color_dic[C_KW.ATTRIB_NEGATIVE]])
+    metaData = getFileMetaData(file, on_windows_os,
+                               [color_dic[C_KW.RESET_ALL],
+                               color_dic[C_KW.ATTRIB],
+                               color_dic[C_KW.ATTRIB_POSITIVE],
+                               color_dic[C_KW.ATTRIB_NEGATIVE]])
     print(metaData)
 
 
 def _printChecksum(file: str) -> None:
     """
     print the information retrieved by getChecksumFromFile()
     
@@ -234,15 +231,15 @@
 
 # def removeAnsiCodes(content: list) -> list:
 #     return [(removeAnsiCodesFromLine(prefix), removeAnsiCodesFromLine(line)) for prefix, line in content]
 
 
 @lru_cache(maxsize=None)
 def _CalculateLinePrefixSpacing(lineCharLength: int,
-                                includeFilePrefix: bool = False, fileCharLength: int = None) -> str:
+                                includeFilePrefix: bool = False, fileCharLength: int = 0) -> str:
     """
     calculate a string template for the line prefix.
     
     Parameters:
     lineCharLength (int):
         the length of the line number
     includeFilePrefix (bool):
@@ -315,32 +312,30 @@
         the new line prefix including the line length.
     """
     if not holder.args_id[ARGS_NOCOL] and type(line) == str:
         line = removeAnsiCodesFromLine(line)
     return _CalculateLineLengthPrefixSpacing(len(str(len(line)))) % (prefix, len(line))
 
 
-def printFile(content: list, bytecode: bool) -> bool:
+def printFile(content: list) -> bool:
     """
     print a file and possibly include the substrings and patterns to search for.
     
     Parameters:
     content (list):
         the content of a file like [(prefix, line), ...]
-    bytecode (bool):
-        if the lines are in bytes the value is True
         
     Returns
     (bool):
         identifies if the given content parameter contained any
         queried keyword/pattern.
     """
     if not content:
         return False
-    if not (ArgParser.FILE_SEARCH or ArgParser.FILE_MATCH) or bytecode:
+    if not (ArgParser.FILE_SEARCH or ArgParser.FILE_MATCH):
         print(*[prefix + line for prefix, line in content], sep='\n')
         return False
 
     containsQueried = False
     stringFinder = StringFinder.StringFinder(ArgParser.FILE_SEARCH, ArgParser.FILE_MATCH)
 
     for line_prefix, line in content:
@@ -376,15 +371,15 @@
             print('--------------- Matched', mKeywords, '---------------', end='')
             print(color_dic[C_KW.RESET_ALL])
             found_sth = True
 
         if found_sth:
             try:  # fails when using -i mode, because the stdin will send en EOF char to input without prompting the user
                 input()
-            except EOFError:
+            except (EOFError, UnicodeDecodeError):
                 pass
             
     return containsQueried
 
 
 def printExcludedByPeek(content: list, excludedByPeek: int) -> None:
     """
@@ -409,59 +404,35 @@
     print(color_dic[C_KW.NUMBER], end='')
     print(excludedByPeekIndent, excludedByPeekIndentAdd, ' •', sep='')
     print(excludedByPeekIndent, '(', excludedByPeek, ')', sep='')
     print(excludedByPeekIndent, excludedByPeekIndentAdd, ' •', sep='', end='')
     print(color_dic[C_KW.RESET_ALL])
 
 
-def editFile(fileIndex: int = 0) -> None:
+def editContent(content: list, show_bytecode: bool, fileIndex: int = 0, lineOffset: int = 0) -> None:
     """
-    apply all parameters to a file.
+    apply all parameters to a string (file Content).
     
     Parameters:
+    content (list):
+        the content of a file like [(prefix, line), ...]
+    show_bytecode (bool).
+        indicates if the content lines are string or bytes
     fileIndex (int):
-        the index regarding which file is currently being edited
+        the index of the holder.files list, pointing to the file that
+        is currently being processed. a negative value can be used for
+        the shell mode
     """
-    show_bytecode = False
     excludedByPeek = 0
-    content = [('', '')]
-    try:
-        with open(holder.files[fileIndex].path, 'r', encoding=ArgParser.FILE_ENCODING) as f:
-            # splitlines() gives a slight inaccuracy, in case the last line is empty.
-            # the alternative would be worse: split('\n') would increase the linecount each
-            # time cat touches a file.
-            content = [('', line) for line in f.read().splitlines()]
-    except:
-        print('Failed to open:', holder.files[fileIndex].displayname)
-        try:
-            enterChar = '⏎'
-            try:
-                enterChar.encode(ArgParser.FILE_ENCODING)
-            except UnicodeError:
-                enterChar = 'ENTER'
-            inp = input(f"Do you want to open the file as a binary, without parameters? [Y/{enterChar}]:")
-            if not 'Y' in inp.upper() and inp:
-                print('Aborting...')
-                return
-        except EOFError:
-            pass
-        try:
-            with open(holder.files[fileIndex].path, 'rb') as f:
-                # in binary splitlines() is our only option
-                content = [('', line) for line in f.read().splitlines()]
-            show_bytecode = True
-        except:
-            print('Operation failed! Try using the enc=X parameter.')
-            return
     
     if not show_bytecode and holder.args_id[ARGS_B64D]:
         content = decodeBase64(content, ArgParser.FILE_ENCODING)
     
     if holder.args_id[ARGS_NUMBER]:
-        content = [(_getLinePrefix(j, fileIndex+1), c[1])
+        content = [(_getLinePrefix(j+lineOffset, fileIndex+1), c[1])
                    for j, c in enumerate(content, start=1)]
     content = content[ArgParser.FILE_TRUNCATE[0]:ArgParser.FILE_TRUNCATE[1]:ArgParser.FILE_TRUNCATE[2]]
     if holder.args_id[ARGS_PEEK] and len(content) > 10:
         excludedByPeek = len(content) - 10
         content = content[:5] + content[-5:]
 
     if not show_bytecode:
@@ -502,28 +473,79 @@
                            for prefix, line  in content]
             elif arg == ARGS_EOF:
                 content = [(prefix, line.replace(chr(26), color_dic[C_KW.REPLACE] + '^EOF' + color_dic[C_KW.RESET_ALL]))
                            for prefix, line in content]
             
     if holder.args_id[ARGS_LLENGTH]:
         content = [(_getLineLengthPrefix(c[0], c[1]), c[1]) for c in content]
-    if show_bytecode:
-        content = [(prefix, str(line)) for prefix, line in content]
     if holder.args_id[ARGS_B64E]:
         content = encodeBase64(content, ArgParser.FILE_ENCODING)
 
-    holder.files[fileIndex].setContainsQueried(printFile(content[:len(content)//2], show_bytecode))
+    foundQueried = printFile(content[:len(content)//2])
+    if fileIndex >= 0:
+        holder.files[fileIndex].setContainsQueried(foundQueried)
     printExcludedByPeek(content, excludedByPeek)
-    holder.files[fileIndex].setContainsQueried(printFile(content[len(content)//2:], show_bytecode))
-
+    foundQueried = printFile(content[len(content)//2:])
+    if fileIndex >= 0:
+        holder.files[fileIndex].setContainsQueried(foundQueried)
+    
     if not show_bytecode:
         if holder.args_id[ARGS_CLIP]:
             holder.clipBoard += '\n'.join([prefix + line for prefix, line in content])
 
 
+def editFile(fileIndex: int = 0) -> None:
+    """
+    apply all parameters to a file.
+    
+    Parameters:
+    fileIndex (int):
+        the index regarding which file is currently being edited
+    """
+    show_bytecode = False
+    
+    content = [('', '')]
+    try:
+        with open(holder.files[fileIndex].path, 'r', encoding=ArgParser.FILE_ENCODING) as f:
+            # splitlines() gives a slight inaccuracy, in case the last line is empty.
+            # the alternative would be worse: split('\n') would increase the linecount each
+            # time catw touches a file.
+            content = [('', line) for line in f.read().splitlines()]
+    except:
+        print('Failed to open:', holder.files[fileIndex].displayname)
+        try:
+            enterChar = '⏎'
+            try:
+                if len(enterChar.encode(ArgParser.FILE_ENCODING)) != 3:
+                    raise UnicodeEncodeError('', '', -1, -1, '')
+            except UnicodeEncodeError:
+                enterChar = 'ENTER'
+            print(f"Do you want to open the file as a binary, without parameters? [Y/{enterChar}]:", end='')
+            inp = input()
+            if not 'Y' in inp.upper() and inp:
+                print('Aborting...')
+                return
+        except EOFError:
+            pass
+        except UnicodeError:
+            print(f"Input is not recognized in the given encoding: {ArgParser.FILE_ENCODING}")
+            print('Aborting...')
+            return
+        try:
+            with open(holder.files[fileIndex].path, 'rb') as f:
+                # in binary splitlines() is our only option
+                content = [('', repr(line)[2:-1]) for line in f.read().splitlines()]
+            show_bytecode = True
+        except:
+            print('Operation failed! Try using the enc=X parameter.')
+            return
+    
+    editContent(content, show_bytecode, fileIndex)
+
+
 def _copyToClipboard(content: str, __dependency: int = 3, __clipBoardError: bool = False) -> None:
     """
     copy a string to the clipboard, by recursively checking which module exists and could
     be used, this function should only be called by copyToClipboard()
     
     Parameters:
     content (str):
@@ -577,15 +599,15 @@
     fileIndex (int):
         the index regarding which file is currently being edited
     mode (str):
         either 'x', 'X' for hexadecimal (lower- or upper case letters),
         or 'b' for binary
     """
     print(holder.files[fileIndex].displayname, ':', sep='')
-    for line in getRawViewLinesGen(holder.files[fileIndex].path, mode, [color_dic[C_KW.RAWVIEWER], color_dic[C_KW.RESET_ALL]]):
+    for line in getRawViewLinesGen(holder.files[fileIndex].path, mode, [color_dic[C_KW.RAWVIEWER], color_dic[C_KW.RESET_ALL]], ArgParser.FILE_ENCODING):
         print(line)
     print('')
 
 
 def editFiles() -> None:
     """
     manage the calls to editFile() for each file.
@@ -614,55 +636,75 @@
     if holder.args_id[ARGS_FILES]:
         print('')
         _showFiles()
     if holder.args_id[ARGS_CLIP]:
         copyToClipboard(removeAnsiCodesFromLine(holder.clipBoard))
 
 
-def main():
-    piped_input = temp_file = ''
-
+def init(shell: bool = False) -> tuple:
+    """
+    initiate the code by calling the argparser and handling the default
+    parameters: -h, -v, -d, --config.
+    
+    Parameters:
+    contenshellt (bool):
+        indicates if the shell entry point was used, and the stdin will therefor
+        be used by default
+        
+    Returns
+    (tuple):
+        contains (known_files, unknown_files, echo_args) from the argparser
+    """
     # read parameter-args
     args, unknown_args, known_files, unknown_files, echo_args = ArgParser.getArguments(sys.argv)
 
     holder.setArgs(args)
 
-    sys.stdout.reconfigure(encoding=ArgParser.FILE_ENCODING)
-    sys.stdin.reconfigure(encoding=ArgParser.FILE_ENCODING)
+    if holder.args_id[ARGS_RECONFIGURE]:
+        sys.stdout.reconfigure(encoding=ArgParser.FILE_ENCODING)
+        sys.stdin.reconfigure(encoding=ArgParser.FILE_ENCODING)
     
     # do not use colors if requested, or output will be piped anyways
     if holder.args_id[ARGS_NOCOL] or (not sys.stdout.isatty() or sys.stdout.closed):
         global color_dic
         color_dic = dict.fromkeys(color_dic,'')
     
     # check for special cases
     if holder.args_id[ARGS_DEBUG]:
         _showDebug(args, unknown_args, known_files, unknown_files, echo_args)
-    if (len(known_files) + len(unknown_files) + len(holder.args) == 0) or holder.args_id[ARGS_HELP]:
+    if (len(known_files) + len(unknown_files) + len(holder.args) == 0 and not shell) or holder.args_id[ARGS_HELP]:
         _showHelp()
-        return
+        sys.exit(0)
     if holder.args_id[ARGS_VERSION]:
         _showVersion()
-        return
+        sys.exit(0)
     if holder.args_id[ARGS_CONFIG]:
         config.saveConfig()
-        return
+        sys.exit(0)
+    
+    return (known_files, unknown_files, echo_args)
+
+
+def main():
+    piped_input = temp_file = ''
+    known_files, unknown_files, echo_args = init(False)
+    
     if holder.args_id[ARGS_ECHO]:
         temp_file = StdInHelper.writeTemp(' '.join(echo_args), tmpFileHelper.generateTempFileName(), ArgParser.FILE_ENCODING)
         known_files.append(temp_file)
         holder.setTempFileEcho(temp_file)
     if holder.args_id[ARGS_INTERACTIVE]:
-        piped_input = StdInHelper.getStdInContent(holder.args_id[ARGS_ONELINE])
+        piped_input = ''.join(StdInHelper.getStdInContent(holder.args_id[ARGS_ONELINE]))
         temp_file = StdInHelper.writeTemp(piped_input, tmpFileHelper.generateTempFileName(), ArgParser.FILE_ENCODING)
         known_files.append(temp_file)
         unknown_files = StdInHelper.writeFiles(unknown_files, piped_input, ArgParser.FILE_ENCODING)
         holder.setTempFileStdIn(temp_file)
     else:
         unknown_files = StdInHelper.readWriteFilesFromStdIn(
-            unknown_files, ArgParser.FILE_ENCODING, holder.args_id[ARGS_ONELINE])
+            unknown_files, ArgParser.FILE_ENCODING, on_windows_os, holder.args_id[ARGS_ONELINE])
 
     if (len(known_files) + len(unknown_files) == 0):
         return
 
     # fill holder object with neccessary values
     holder.setFiles([*known_files, *unknown_files])
     
@@ -695,15 +737,25 @@
         try:
             os.remove(tmp_file)
         except FileNotFoundError:
             if holder.args_id[ARGS_DEBUG]:
                 print('FileNotFoundError', tmp_file)
 
 
-def deprecated_main():
-    print(color_dic[C_KW.MESSAGE_IMPORTANT], end='')
-    print("The 'cat'-command is soon to be deprecated. Please consider using 'catw'.", end='')
-    print(color_dic[C_KW.RESET_ALL], end='\n\n')
-    main()
+def shell_main():
+    init(True)
+    
+    shellPrefix = '>>> '
+    EOFControlChar = 'Z' if on_windows_os else 'D'
+    
+    print(__project__, 'v' + __version__, 'shell', '(' + __url__ + ')')
+    print(f"Use 'catw' to handle files. Type ^{EOFControlChar} (Ctrl + {EOFControlChar}) to exit.")
+    
+    print(shellPrefix, end='', flush=True)
+    for i, line in enumerate(StdInHelper.getStdInContent(holder.args_id[ARGS_ONELINE])):
+        editContent([('', line.rstrip('\n'))], False, -1, i)
+        if not holder.args_id[ARGS_ONELINE]:
+            print(shellPrefix, end='', flush=True)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `cat_win-1.3.1/cat_win/const/ArgConstants.py` & `cat_win-1.4.0/cat_win/const/ArgConstants.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ARGS_HELP, ARGS_NUMBER, ARGS_ENDS, ARGS_TABS, ARGS_SQUEEZE = range(0, 5)
 ARGS_REVERSE, ARGS_COUNT, ARGS_BLANK, ARGS_FILES, ARGS_INTERACTIVE = range(5, 10)
 ARGS_CLIP, ARGS_CHECKSUM, ARGS_DEC, ARGS_HEX, ARGS_BIN = range(10, 15)
 ARGS_VERSION, ARGS_DEBUG, ARGS_CUT, ARGS_REPLACE, ARGS_DATA = range(15, 20)
 ARGS_CONFIG, ARGS_LLENGTH, ARGS_ONELINE, ARGS_PEEK, ARGS_NOCOL = range(20, 25)
 ARGS_EOF, ARGS_B64E, ARGS_B64D, ARGS_FFILES, ARGS_GREP = range(25, 30)
 ARGS_NOBREAK, ARGS_ECHO, ARGS_CCOUNT, ARGS_HEXVIEW, ARGS_BINVIEW = range(30, 35)
-ARGS_NOKEYWORD, = range(35, 36)
+ARGS_NOKEYWORD, ARGS_RECONFIGURE = range(35, 37)
 
 ALL_ARGS = [[['-h', '--help'], 'show this help message and exit', ARGS_HELP],
             [['-v', '--version'], 'output version information and exit', ARGS_VERSION],
             [['-d', '--debug'], 'show debug information', ARGS_DEBUG],
             [['-n', '--number'], 'number all output lines', ARGS_NUMBER],
             [['-l', '--linelength'], 'display the length of each line', ARGS_LLENGTH],
             [['-e', '--ends'], 'display $ at the end of each line', ARGS_ENDS],
@@ -45,11 +45,12 @@
             [['--b64e', '--b64e'], 'encode the input to base64', ARGS_B64E],
             [['--b64d', '--b64d'], 'decode the input from base64', ARGS_B64D],
             [['--hexview', '--HEXVIEW'], 'display the raw byte representation in hexadecimal', ARGS_HEXVIEW],
             [['--binview', '--binview'], 'display the raw byte representation in binary', ARGS_BINVIEW],
             [['--nc', '--nocolor'], 'disable colored output', ARGS_NOCOL],
             [['--nb', '--nobreak'], 'do not interrupt the output on queried keywords', ARGS_NOBREAK],
             [['--nk', '--nokeyword'], 'inverse the grep output', ARGS_NOKEYWORD],
+            [['-R', '--reconfigure'], 'reconfigure the stdin and stdout with the parsed encoding', ARGS_RECONFIGURE],
             [['--config', '--config'], 'change color configuration', ARGS_CONFIG]]
 
 ALL_ARGS = [ArgConstant(x[0][0], x[0][1], x[1], x[2]) for x in ALL_ARGS]
 HIGHEST_ARG_ID = max([m.id for m in ALL_ARGS])
```

### Comparing `cat_win-1.3.1/cat_win/const/ColorConstants.py` & `cat_win-1.4.0/cat_win/const/ColorConstants.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def idToCode(code: int) -> str:
     return f"{ESC_CODE}[{code}m"
 
 
 class ColorOptions:
-    Fore = {
+    __Fore = {
         'RESET': 39,
             
         'BLACK':   30,
         'RED':     31,
         'GREEN':   32,
         'YELLOW':  33,
         'BLUE':    34,
@@ -24,15 +24,15 @@
         'LIGHTGREEN':   92,
         'LIGHTYELLOW':  93,
         'LIGHTBLUE':    94,
         'LIGHTMAGENTA': 95,
         'LIGHTCYAN':    96,
         'LIGHTWHITE':   97
         }
-    Back = {
+    __Back = {
         'RESET': 49,
             
         'BLACK':   40,
         'RED':     41,
         'GREEN':   42,
         'YELLOW':  43,
         'BLUE':    44,
@@ -45,26 +45,28 @@
         'LIGHTGREEN':   102,
         'LIGHTYELLOW':  103,
         'LIGHTBLUE':    104,
         'LIGHTMAGENTA': 105,
         'LIGHTCYAN':    106,
         'LIGHTWHITE':   107
         }
-    Style = {
+    __Style = {
         'RESET': 0
         }
 
-    for key in Fore:
-        Fore[key] = idToCode(Fore[key])
-    Fore['NONE'] = ''
-    for key in Back:
-        Back[key] = idToCode(Back[key])
-    Back['NONE'] = ''
-    for key in Style:
-        Style[key] = idToCode(Style[key])
+    Fore  = {'NONE': ''}
+    Back  = {'NONE': ''}
+    Style = {'NONE': ''}
+    
+    for key in __Fore:
+        Fore[key]  = idToCode(__Fore[key])
+    for key in __Back:
+        Back[key]  = idToCode(__Back[key])
+    for key in __Style:
+        Style[key] = idToCode(__Style[key])
 
 
 class C_KW:
     RESET_ALL = 'reset_all'
     RESET_FOUND = 'reset_found'
     RESET_MATCHED = 'reset_matched'
```

### Comparing `cat_win-1.3.1/cat_win/persistence/Config.py` & `cat_win-1.4.0/cat_win/persistence/Config.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/tests/test_ArgConstants.py` & `cat_win-1.4.0/cat_win/tests/test_ArgConstants.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/tests/test_ArgParser.py` & `cat_win-1.4.0/cat_win/tests/test_ArgParser.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/tests/test_Base64.py` & `cat_win-1.4.0/cat_win/tests/test_Base64.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/tests/test_Converter.py` & `cat_win-1.4.0/cat_win/tests/test_Converter.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/tests/test_File.py` & `cat_win-1.4.0/cat_win/tests/test_File.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/tests/test_FileAttributes.py` & `cat_win-1.4.0/cat_win/tests/test_FileAttributes.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/tests/test_Holder.py` & `cat_win-1.4.0/cat_win/tests/test_Holder.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/tests/test_RawViewer.py` & `cat_win-1.4.0/cat_win/tests/test_RawViewer.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,74 +4,76 @@
 from cat_win.util.RawViewer import getRawViewLinesGen
 
 
 test_file_path = os.path.join(os.path.dirname(__file__), 'texts', 'test.txt')
 
 
 class TestRawViewer(TestCase):
+    maxDiff = None
+    
     def testModeX(self):
         expected_result = """Address  00 01 02 03 04 05 06 07 08 09 0A 0B 0C 0D 0E 0F # Decoded Text                   
-00000000 53 61 6D 70 6C 65 20 54 65 78 74 3A 0D 0A 54 68 # S a m p l e   T e x t : · · T h
+00000000 53 61 6D 70 6C 65 20 54 65 78 74 3A 0D 0A 54 68 # S a m p l e   T e x t : ␍ ␤ T h
 00000010 69 73 20 69 73 20 61 20 54 61 62 2D 43 68 61 72 # i s   i s   a   T a b - C h a r
-00000020 61 63 74 65 72 3A 20 3E 09 3C 0D 0A 54 68 65 73 # a c t e r :   > · < · · T h e s
+00000020 61 63 74 65 72 3A 20 3E 09 3C 0D 0A 54 68 65 73 # a c t e r :   > · < ␍ ␤ T h e s
 00000030 65 20 61 72 65 20 53 70 65 63 69 61 6C 20 43 68 # e   a r e   S p e c i a l   C h
 00000040 61 72 73 3A 20 C3 A4 C3 B6 C3 BC C3 84 C3 96 C3 # a r s :   · · · · · · · · · · ·
-00000050 9C 0D 0A 4E 2D 41 72 79 20 53 75 6D 6D 61 74 69 # · · · N - A r y   S u m m a t i
-00000060 6F 6E 3A 20 E2 88 91 0D 0A 54 68 65 20 66 6F 6C # o n :   · · · · · T h e   f o l
+00000050 9C 0D 0A 4E 2D 41 72 79 20 53 75 6D 6D 61 74 69 # · ␍ ␤ N - A r y   S u m m a t i
+00000060 6F 6E 3A 20 E2 88 91 0D 0A 54 68 65 20 66 6F 6C # o n :   · · · ␍ ␤ T h e   f o l
 00000070 6C 6F 77 69 6E 67 20 4C 69 6E 65 20 69 73 20 45 # l o w i n g   L i n e   i s   E
-00000080 6D 70 74 79 3A 0D 0A 0D 0A 54 68 69 73 20 4C 69 # m p t y : · · · · T h i s   L i
+00000080 6D 70 74 79 3A 0D 0A 0D 0A 54 68 69 73 20 4C 69 # m p t y : ␍ ␤ ␍ ␤ T h i s   L i
 00000090 6E 65 20 69 73 20 61 20 44 75 70 6C 69 63 61 74 # n e   i s   a   D u p l i c a t
-000000A0 65 21 0D 0A 54 68 69 73 20 4C 69 6E 65 20 69 73 # e ! · · T h i s   L i n e   i s
+000000A0 65 21 0D 0A 54 68 69 73 20 4C 69 6E 65 20 69 73 # e ! ␍ ␤ T h i s   L i n e   i s
 000000B0 20 61 20 44 75 70 6C 69 63 61 74 65 21          #   a   D u p l i c a t e !"""
     
         self.assertEqual('\n'.join(getRawViewLinesGen(test_file_path, 'X')), expected_result)
         
     def testModex(self):
         expected_result = """Address  00 01 02 03 04 05 06 07 08 09 0A 0B 0C 0D 0E 0F # Decoded Text                   
-00000000 53 61 6d 70 6c 65 20 54 65 78 74 3a 0d 0a 54 68 # S a m p l e   T e x t : · · T h
+00000000 53 61 6d 70 6c 65 20 54 65 78 74 3a 0d 0a 54 68 # S a m p l e   T e x t : ␍ ␤ T h
 00000010 69 73 20 69 73 20 61 20 54 61 62 2d 43 68 61 72 # i s   i s   a   T a b - C h a r
-00000020 61 63 74 65 72 3a 20 3e 09 3c 0d 0a 54 68 65 73 # a c t e r :   > · < · · T h e s
+00000020 61 63 74 65 72 3a 20 3e 09 3c 0d 0a 54 68 65 73 # a c t e r :   > · < ␍ ␤ T h e s
 00000030 65 20 61 72 65 20 53 70 65 63 69 61 6c 20 43 68 # e   a r e   S p e c i a l   C h
 00000040 61 72 73 3a 20 c3 a4 c3 b6 c3 bc c3 84 c3 96 c3 # a r s :   · · · · · · · · · · ·
-00000050 9c 0d 0a 4e 2d 41 72 79 20 53 75 6d 6d 61 74 69 # · · · N - A r y   S u m m a t i
-00000060 6f 6e 3a 20 e2 88 91 0d 0a 54 68 65 20 66 6f 6c # o n :   · · · · · T h e   f o l
+00000050 9c 0d 0a 4e 2d 41 72 79 20 53 75 6d 6d 61 74 69 # · ␍ ␤ N - A r y   S u m m a t i
+00000060 6f 6e 3a 20 e2 88 91 0d 0a 54 68 65 20 66 6f 6c # o n :   · · · ␍ ␤ T h e   f o l
 00000070 6c 6f 77 69 6e 67 20 4c 69 6e 65 20 69 73 20 45 # l o w i n g   L i n e   i s   E
-00000080 6d 70 74 79 3a 0d 0a 0d 0a 54 68 69 73 20 4c 69 # m p t y : · · · · T h i s   L i
+00000080 6d 70 74 79 3a 0d 0a 0d 0a 54 68 69 73 20 4c 69 # m p t y : ␍ ␤ ␍ ␤ T h i s   L i
 00000090 6e 65 20 69 73 20 61 20 44 75 70 6c 69 63 61 74 # n e   i s   a   D u p l i c a t
-000000A0 65 21 0d 0a 54 68 69 73 20 4c 69 6e 65 20 69 73 # e ! · · T h i s   L i n e   i s
+000000A0 65 21 0d 0a 54 68 69 73 20 4c 69 6e 65 20 69 73 # e ! ␍ ␤ T h i s   L i n e   i s
 000000B0 20 61 20 44 75 70 6c 69 63 61 74 65 21          #   a   D u p l i c a t e !"""
     
         self.assertEqual('\n'.join(getRawViewLinesGen(test_file_path, 'x')), expected_result)
         
     def testModeb(self):
         expected_result = """Address  00       01       02       03       04       05       06       07       08       09       0A       0B       0C       0D       0E       0F       # Decoded Text                   
-00000000 01010011 01100001 01101101 01110000 01101100 01100101 00100000 01010100 01100101 01111000 01110100 00111010 00001101 00001010 01010100 01101000 # S a m p l e   T e x t : · · T h
+00000000 01010011 01100001 01101101 01110000 01101100 01100101 00100000 01010100 01100101 01111000 01110100 00111010 00001101 00001010 01010100 01101000 # S a m p l e   T e x t : ␍ ␤ T h
 00000010 01101001 01110011 00100000 01101001 01110011 00100000 01100001 00100000 01010100 01100001 01100010 00101101 01000011 01101000 01100001 01110010 # i s   i s   a   T a b - C h a r
-00000020 01100001 01100011 01110100 01100101 01110010 00111010 00100000 00111110 00001001 00111100 00001101 00001010 01010100 01101000 01100101 01110011 # a c t e r :   > · < · · T h e s
+00000020 01100001 01100011 01110100 01100101 01110010 00111010 00100000 00111110 00001001 00111100 00001101 00001010 01010100 01101000 01100101 01110011 # a c t e r :   > · < ␍ ␤ T h e s
 00000030 01100101 00100000 01100001 01110010 01100101 00100000 01010011 01110000 01100101 01100011 01101001 01100001 01101100 00100000 01000011 01101000 # e   a r e   S p e c i a l   C h
 00000040 01100001 01110010 01110011 00111010 00100000 11000011 10100100 11000011 10110110 11000011 10111100 11000011 10000100 11000011 10010110 11000011 # a r s :   · · · · · · · · · · ·
-00000050 10011100 00001101 00001010 01001110 00101101 01000001 01110010 01111001 00100000 01010011 01110101 01101101 01101101 01100001 01110100 01101001 # · · · N - A r y   S u m m a t i
-00000060 01101111 01101110 00111010 00100000 11100010 10001000 10010001 00001101 00001010 01010100 01101000 01100101 00100000 01100110 01101111 01101100 # o n :   · · · · · T h e   f o l
+00000050 10011100 00001101 00001010 01001110 00101101 01000001 01110010 01111001 00100000 01010011 01110101 01101101 01101101 01100001 01110100 01101001 # · ␍ ␤ N - A r y   S u m m a t i
+00000060 01101111 01101110 00111010 00100000 11100010 10001000 10010001 00001101 00001010 01010100 01101000 01100101 00100000 01100110 01101111 01101100 # o n :   · · · ␍ ␤ T h e   f o l
 00000070 01101100 01101111 01110111 01101001 01101110 01100111 00100000 01001100 01101001 01101110 01100101 00100000 01101001 01110011 00100000 01000101 # l o w i n g   L i n e   i s   E
-00000080 01101101 01110000 01110100 01111001 00111010 00001101 00001010 00001101 00001010 01010100 01101000 01101001 01110011 00100000 01001100 01101001 # m p t y : · · · · T h i s   L i
+00000080 01101101 01110000 01110100 01111001 00111010 00001101 00001010 00001101 00001010 01010100 01101000 01101001 01110011 00100000 01001100 01101001 # m p t y : ␍ ␤ ␍ ␤ T h i s   L i
 00000090 01101110 01100101 00100000 01101001 01110011 00100000 01100001 00100000 01000100 01110101 01110000 01101100 01101001 01100011 01100001 01110100 # n e   i s   a   D u p l i c a t
-000000A0 01100101 00100001 00001101 00001010 01010100 01101000 01101001 01110011 00100000 01001100 01101001 01101110 01100101 00100000 01101001 01110011 # e ! · · T h i s   L i n e   i s
+000000A0 01100101 00100001 00001101 00001010 01010100 01101000 01101001 01110011 00100000 01001100 01101001 01101110 01100101 00100000 01101001 01110011 # e ! ␍ ␤ T h i s   L i n e   i s
 000000B0 00100000 01100001 00100000 01000100 01110101 01110000 01101100 01101001 01100011 01100001 01110100 01100101 00100001                            #   a   D u p l i c a t e !"""
     
         self.assertEqual('\n'.join(getRawViewLinesGen(test_file_path, 'b')), expected_result)
         
     def testModeXColored(self):
         expected_result = """*Address  00 01 02 03 04 05 06 07 08 09 0A 0B 0C 0D 0E 0F # Decoded Text                   !
-*00000000! 53 61 6D 70 6C 65 20 54 65 78 74 3A 0D 0A 54 68 *#! S a m p l e   T e x t : · · T h
+*00000000! 53 61 6D 70 6C 65 20 54 65 78 74 3A 0D 0A 54 68 *#! S a m p l e   T e x t : ␍ ␤ T h
 *00000010! 69 73 20 69 73 20 61 20 54 61 62 2D 43 68 61 72 *#! i s   i s   a   T a b - C h a r
-*00000020! 61 63 74 65 72 3A 20 3E 09 3C 0D 0A 54 68 65 73 *#! a c t e r :   > · < · · T h e s
+*00000020! 61 63 74 65 72 3A 20 3E 09 3C 0D 0A 54 68 65 73 *#! a c t e r :   > · < ␍ ␤ T h e s
 *00000030! 65 20 61 72 65 20 53 70 65 63 69 61 6C 20 43 68 *#! e   a r e   S p e c i a l   C h
 *00000040! 61 72 73 3A 20 C3 A4 C3 B6 C3 BC C3 84 C3 96 C3 *#! a r s :   · · · · · · · · · · ·
-*00000050! 9C 0D 0A 4E 2D 41 72 79 20 53 75 6D 6D 61 74 69 *#! · · · N - A r y   S u m m a t i
-*00000060! 6F 6E 3A 20 E2 88 91 0D 0A 54 68 65 20 66 6F 6C *#! o n :   · · · · · T h e   f o l
+*00000050! 9C 0D 0A 4E 2D 41 72 79 20 53 75 6D 6D 61 74 69 *#! · ␍ ␤ N - A r y   S u m m a t i
+*00000060! 6F 6E 3A 20 E2 88 91 0D 0A 54 68 65 20 66 6F 6C *#! o n :   · · · ␍ ␤ T h e   f o l
 *00000070! 6C 6F 77 69 6E 67 20 4C 69 6E 65 20 69 73 20 45 *#! l o w i n g   L i n e   i s   E
-*00000080! 6D 70 74 79 3A 0D 0A 0D 0A 54 68 69 73 20 4C 69 *#! m p t y : · · · · T h i s   L i
+*00000080! 6D 70 74 79 3A 0D 0A 0D 0A 54 68 69 73 20 4C 69 *#! m p t y : ␍ ␤ ␍ ␤ T h i s   L i
 *00000090! 6E 65 20 69 73 20 61 20 44 75 70 6C 69 63 61 74 *#! n e   i s   a   D u p l i c a t
-*000000A0! 65 21 0D 0A 54 68 69 73 20 4C 69 6E 65 20 69 73 *#! e ! · · T h i s   L i n e   i s
+*000000A0! 65 21 0D 0A 54 68 69 73 20 4C 69 6E 65 20 69 73 *#! e ! ␍ ␤ T h i s   L i n e   i s
 *000000B0! 20 61 20 44 75 70 6C 69 63 61 74 65 21          *#!   a   D u p l i c a t e !"""
     
         self.assertEqual('\n'.join(getRawViewLinesGen(test_file_path, 'X', ['*', '!'])), expected_result)
```

### Comparing `cat_win-1.3.1/cat_win/tests/test_StringFinder.py` & `cat_win-1.4.0/cat_win/tests/test_StringFinder.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/tests/test_UpdateChecker.py` & `cat_win-1.4.0/cat_win/tests/test_UpdateChecker.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/tests/test_cat.py` & `cat_win-1.4.0/cat_win/tests/test_cat.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/tests/test_checksum.py` & `cat_win-1.4.0/cat_win/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/tests/test_full.py` & `cat_win-1.4.0/cat_win/tests/test_full.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/util/ArgParser.py` & `cat_win-1.4.0/cat_win/util/ArgParser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from glob import iglob
 from os.path import isfile, realpath, isdir
 from re import match
 
 from cat_win.const.ArgConstants import *
 
 
-FILE_ENCODING = 'utf-8'
+FILE_ENCODING: str = 'utf-8'
 FILE_SEARCH = []
 FILE_MATCH = []
 FILE_TRUNCATE = [None, None, None]
 
 
 def __addArgument__(args: list, unknown_args: list, known_files: list, unknown_files: list, param: str) -> bool:
     """
@@ -45,21 +45,21 @@
     # 'find' + ('=' or ':') + FILE_SEARCH
     elif match(r"\Afind[\=\:].+\Z", param):
         global FILE_SEARCH
         FILE_SEARCH.append(param[5:])
         return False
     # 'trunc' + ('=' or ':') + FILE_TRUNCATE[0] + ':' + FILE_TRUNCATE[1] + ':' + FILE_TRUNCATE[2]
     elif match(r"\Atrunc[\=\:][0-9()+\-*\/]*\:[0-9()+\-*\/]*\:?[0-9()+\-*\/]*\Z", param):
-        param = param[6:].split(':')
+        paramSplit = param[6:].split(':')
         global FILE_TRUNCATE
-        FILE_TRUNCATE[0] = None if param[0] == '' else (
-            0 if param[0] == '0' else int(eval(param[0]))-1)
-        FILE_TRUNCATE[1] = None if param[1] == '' else int(eval(param[1]))
-        if len(param) == 3:
-            FILE_TRUNCATE[2] = None if param[2] == '' else int(eval(param[2]))
+        FILE_TRUNCATE[0] = None if paramSplit[0] == '' else (
+            0 if paramSplit[0] == '0' else int(eval(paramSplit[0]))-1)
+        FILE_TRUNCATE[1] = None if paramSplit[1] == '' else int(eval(paramSplit[1]))
+        if len(paramSplit) == 3:
+            FILE_TRUNCATE[2] = None if paramSplit[2] == '' else int(eval(paramSplit[2]))
         return False
     # '[' + ARGS_CUT + ']'
     elif match(r"\A\[[0-9()+\-*\/]*\:[0-9()+\-*\/]*\:?[0-9()+\-*\/]*\]\Z", param):
         args.append((ARGS_CUT, param))
         return False
     # '[' + ARGS_REPLACE + ']'
     elif match(r"\A\[.+\,.+\]\Z", param):
```

### Comparing `cat_win-1.3.1/cat_win/util/Base64.py` & `cat_win-1.4.0/cat_win/util/Base64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from base64 import b64encode, b64decode
 
 
-def _encodeBase64(content: str, encoding: str) -> str:
+def _encodeBase64(content: str, encoding: str) -> bytes:
     """
     Encode a string to base64.
     
     Parameters:
     content (str):
         the string to encode
     encoding (str):
         the encoding the string is using
         
     Returns:
-    encoded_content (str):
+    encoded_content (bytes):
         the base64 encoded string
     """
     # encode the string to bytes and encode with base64
     contentBytes = content.encode(encoding=encoding)
-    base64_bytes = b64encode(contentBytes)
-    encoded_content = base64_bytes.decode(encoding='ascii')
+    encoded_content = b64encode(contentBytes)
+    
     # return as a single line
     return encoded_content
 
 
 def encodeBase64(content: list, encoding: str = 'utf-8') -> list:
     """
     Encode the file content to base64 by calling _encodeBase64()
@@ -38,36 +38,35 @@
         the encoded base64 content as a single line without any prefix
     """
     # concatenate all lines and join them with line breaks
     contentLines = list(map(lambda x: x[1], content))
     contentLine = '\n'.join(contentLines)
     
     encoded_content = _encodeBase64(contentLine, encoding)
+    encoded_content = encoded_content.decode(encoding='ascii')
     # return as a list containing a single line
     return [('', encoded_content)]
 
 
-def _decodeBase64(content: str, encoding: str) -> str:
+def _decodeBase64(content: str) -> bytes:
     """
     Decode a string from base64.
     
     Parameters:
     content (str):
         the string to decode
-    encoding (str):
-        the encoding the string is using
         
     Returns:
-    decoded_content (str):
+    decoded_content (bytes):
         the base64 decoded string
     """
     # encode the string to bytes and decode with base64
     base64_bytes = content.encode(encoding='ascii')
     decoded_content = b64decode(base64_bytes)
-    decoded_content = decoded_content.decode(encoding=encoding)
+    
     # return as a single line
     return decoded_content
 
 
 def decodeBase64(content: list, encoding: str = 'utf-8') -> list:
     """
     decode the file content from base64 by calling _decodeBase64()
@@ -82,12 +81,13 @@
     [('', line), ...] (list):
         the decoded base64 content line by line without any prefix
     """
     # concatenate all lines and join them
     contentLines = list(map(lambda x: x[1], content))
     contentLine = ''.join(contentLines)
     
-    decoded_content = _decodeBase64(contentLine, encoding)
+    decoded_content = _decodeBase64(contentLine)
+    decoded_content = decoded_content.decode(encoding=encoding)
     
     # return as content list, split at line breaks
     decoded_content = decoded_content.split('\n')
     return [('', line) for line in decoded_content]
```

### Comparing `cat_win-1.3.1/cat_win/util/Converter.py` & `cat_win-1.4.0/cat_win/util/Converter.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/cat_win/util/FileAttributes.py` & `cat_win-1.4.0/cat_win/util/FileAttributes.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,21 +76,24 @@
     """
     try:
         return stat(file).st_size
     except OSError:
         return 0
 
 
-def getFileMetaData(file: str, colors: list = None) -> str:
+def getFileMetaData(file: str, on_windows_os: bool, colors = None) -> str:
     """
     calculate file metadata information.
     
     Parameters:
     file (str):
         a string representation of a file (-path)
+    on_windows_os (bool):
+        indicates if the user is on windows os using
+        platform.system() == 'Windows'
     colors (list):
         a list containing the ANSI-Colorcodes to display
         the attributes like [RESET_ALL, ATTRIB, +ATTRIB, -ATTRIB]
     
     Returns:
     metaData (str):
         representation containing file size, creation/modified/accessed time.
@@ -104,21 +107,21 @@
         metaData = colors[1] + file + colors[0] + '\n'
         
         metaData += f"{colors[1]}{'Size:' : <16}{_convert_size(stats.st_size)}{colors[0]}\n"
         metaData += f"{colors[1]}{'ATime:': <16}{datetime.fromtimestamp(stats.st_atime)}{colors[0]}\n"
         metaData += f"{colors[1]}{'MTime:': <16}{datetime.fromtimestamp(stats.st_mtime)}{colors[0]}\n"
         metaData += f"{colors[1]}{'CTime:': <16}{datetime.fromtimestamp(stats.st_ctime)}{colors[0]}\n"
         
-        if system() != 'Windows':
+        if not on_windows_os:
             metaData += '\n'
             return metaData
         
         attribs = read_attribs(file)
         metaData += colors[2]
         metaData += '+' + ", ".join([x for x, y in attribs if y])
         metaData += colors[0] + '\n'
         metaData += colors[3]
         metaData += '-' + ", ".join([x for x, y in attribs if not y])
         metaData += colors[0] + '\n'
         return metaData
     except OSError:
-        pass
+        return ''
```

### Comparing `cat_win-1.3.1/cat_win/util/Holder.py` & `cat_win-1.4.0/cat_win/util/Holder.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,15 +68,24 @@
         
     def setTempFileEcho(self, file: str) -> None:
         self.temp_file_echo = file
     
     def __calcFileNumberPlaceHolder__(self) -> None:
         self.fileNumberPlaceHolder = len(str(len(self.files)))
 
-    def __count_generator__(self, reader) -> bytes:
+    def __count_generator__(self, reader):
+        """
+        Parameters:
+        reader (method):
+            the method to read from
+        
+        Yields:
+        b (bytes):
+            the bytes in chunks read from the reader
+        """
         b = reader(1024 * 1024)
         while b:
             yield b
             b = reader(1024 * 1024)
 
     @lru_cache(maxsize=10)
     def __getFileLinesSum__(self, file: str) -> int:
@@ -131,12 +140,12 @@
         self._inner_files = temp_files[:]
 
     def generateValues(self, encoding: str) -> None:
         self.__calcFileNumberPlaceHolder__()
         if self.args_id[ARGS_B64D]:
             from cat_win.util.Base64 import _decodeBase64
             for i, file in enumerate(self.files):
-                with open(file.path, 'r', encoding=encoding) as fp:
-                    with open(self._inner_files[i], 'w', encoding='ascii') as f:
-                        f.write(_decodeBase64(fp.read(), encoding))
+                with open(file.path, 'rb') as fp:
+                    with open(self._inner_files[i], 'wb') as f:
+                        f.write(_decodeBase64(fp.read().decode(encoding)))
         self.__calcPlaceHolder__()
         self.__calcFileLineLengthPlaceHolder__()
```

### Comparing `cat_win-1.3.1/cat_win/util/StdInHelper.py` & `cat_win-1.4.0/cat_win/util/StdInHelper.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,42 +14,43 @@
     file_encoding (str):
         an encoding the open the file with
     
     Returns:
     tmp_file (str):
         the path to the temporary file written
     """
-    with open(tmp_file, 'w', encoding=file_encoding) as f:
-        f.write(content)
+    with open(tmp_file, 'wb') as f:
+        f.write(content.encode(file_encoding))
     return tmp_file
 
 
-def getStdInContent(oneLine: bool = False) -> str:
+def getStdInContent(oneLine: bool = False):
     """
     read the stdin.
     
     Parameters:
     oneLine (bool):
         determines if only the first stdin line should be read
         
-    Returns:
-    input (str):
-        the input delivered by stdin
+    Yields:
+    line (str):
+        the input (line by line) delivered by stdin
         until the first EOF (Chr(26)) character
     """
     if oneLine:
-        first_line = stdin.readline()
-        return first_line.rstrip('\n')
-    input = ''
+        first_line = stdin.readline().rstrip('\n')
+        if first_line[-1:] == chr(26):
+            first_line = first_line[:-1]
+        yield first_line
+        return
     for line in stdin:
-        if line[-2:] == chr(26) + '\n':
-            input += line[:-2]
+        if line[-2:-1] == chr(26):
+            yield line[:-2]
             break
-        input += line
-    return input
+        yield line
 
 
 def path_parts(path: str) -> list:
     """
     split a path recursively into its parts.
     
     Parameters:
@@ -94,16 +95,16 @@
         for subpath in unknown_subpaths:
             try:
                 os.rmdir(subpath)
             except OSError:
                 continue
         return False
     try:
-        with open(file, 'w', encoding=file_encoding) as f:
-            f.write(content)
+        with open(file, 'wb') as f:
+            f.write(content.encode(file_encoding))
     except OSError:
         print(f"Error: The file '{file}' could not be written.")
         # cleanup (delete the folders that have been created)
         for subpath in unknown_subpaths:
             try:
                 os.rmdir(subpath)
             except OSError:
@@ -136,61 +137,71 @@
         return file_list
     
     if content == '':
         abort_command = '' 
         try:
             print('You are about to create an empty file. Do you want to continue?')
             enterChar = '⏎'
+
             try:
-                enterChar.encode(file_encoding)
-            except UnicodeError:
+                if len(enterChar.encode(file_encoding)) != 3:
+                    raise UnicodeEncodeError('', '', -1, -1, '')
+            except UnicodeEncodeError:
                 enterChar = 'ENTER'
-            abort_command = input(f"[Y/{enterChar}] Yes, Continue       [N] No, Abort :")
+            print(f"[Y/{enterChar}] Yes, Continue       [N] No, Abort :", end='')
+            abort_command = input()
         except EOFError:
             pass
+        except UnicodeDecodeError:
+            print(f"Input is not recognized in the given encoding: {file_encoding}")
+            abort_command = 'n'
         finally:
             if abort_command and abort_command.upper() != 'Y':
                 print('Aborting...')
                 file_list.clear()
     
     success_file_list = []
     
     for file in file_list:
         try:
-            with open(file, 'w', encoding=file_encoding) as f:
-                f.write(content)
+            with open(file, 'wb') as f:
+                f.write(content.encode(file_encoding))
             success_file_list.append(file)
         except FileNotFoundError: # the os.pardir path to the file does not exist
             if createFile(file, content, file_encoding):
                 success_file_list.append(file)
         except OSError:
             print(f"Error: The file '{file}' could not be written.")
             
     return success_file_list
 
 
-def readWriteFilesFromStdIn(file_list: list, file_encoding: str, oneLine: bool = False) -> list:
+def readWriteFilesFromStdIn(file_list: list, file_encoding: str, on_windows_os: bool, oneLine: bool = False) -> list:
     """
     Write stdin input to multiple files.
     
     Parameters:
     file_list (list):
         all files that should be written
     file_encoding (str):
         the encoding to use for writing the files
+    on_windows_os (bool):
+        indicates if the user is on windows os using
+        platform.system() == 'Windows'
     oneLine (bool):
         determines if only the first stdin line should be read
         
     Returns:
     (list):
         containing all files, that could succesfully be written.
     """
     if len(file_list) == 0:
         return file_list
 
     print('The given FILE(s)', end='')
     print('', *file_list, sep='\n\t')
-    print("do/does not exist. Write the FILE(s) and finish with the '^Z'-suffix ((Ctrl + Z) + Enter):")
+    EOFControlChar = 'Z' if on_windows_os else 'D'
+    print(f"do/does not exist. Write the FILE(s) and finish with the ^{EOFControlChar}-suffix (Ctrl + {EOFControlChar}):")
 
-    input = getStdInContent(oneLine)
+    input = ''.join(getStdInContent(oneLine))
 
     return writeFiles(file_list, input, file_encoding)
```

### Comparing `cat_win-1.3.1/cat_win/util/StringFinder.py` & `cat_win-1.4.0/cat_win/util/StringFinder.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class StringFinder:
     def __init__(self, literals: list, regex: list) -> None:
         self.kw_literals = literals
         self.kw_regex = regex
 
-    def _findliterals(self, sub: str, s: str) -> list:
+    def _findliterals(self, sub: str, s: str):
         """
         Generate lists containing the position of sub in s.
         
         Parameters:
         sub (str):
             the substring to search for
         s (str):
@@ -24,15 +24,15 @@
         """
         l = len(sub)
         i = s.find(sub)
         while i != -1:
             yield [i, i+l]
             i = s.find(sub, i+1)
 
-    def _findregex(self, pattern: str, s: str) -> list:
+    def _findregex(self, pattern: str, s: str):
         """
         Generate lists containing the position of pattern in s.
         
         Parameters:
         pattern (str):
             the regex pattern to search for
         s (str):
```

### Comparing `cat_win-1.3.1/cat_win/util/checksum.py` & `cat_win-1.4.0/cat_win/util/checksum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from zlib import crc32 as crc32_hash
 import hashlib
 
 
-def getChecksumFromFile(file: str, colors: list = None) -> str:
+def getChecksumFromFile(file: str, colors = None) -> str:
     """
     Calculates and returns the CRC32, MD5, SHA1, SHA256, SHA512
     hashes of a file.
     
     Parameters:
     file (str):
         a string representation of a file (-path)
```

### Comparing `cat_win-1.3.1/cat_win/web/UpdateChecker.py` & `cat_win-1.4.0/cat_win/web/UpdateChecker.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.3.1/pyproject.toml` & `cat_win-1.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -14,23 +14,26 @@
     "console",
     "crossplatform",
     "python",
     "terminal",
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: Implementation :: PyPy",
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Topic :: Terminals",
+    "Topic :: Text Processing :: Linguistic",
 ]
 dynamic = [
     "version",
     "description",
 ]
 dependencies = [
     "colorama~=0.4.6",
@@ -41,17 +44,18 @@
     "pyperclip~=1.8.0",
 ]
 
 [tool.flit.sdist]
 exclude = 	[
     "cat_win/build",
     "**/**.spec",
-    "**/**.config"
+    "**/**.config",
 ]
 
 [project.scripts]
 catw = "cat_win.__main__:entry_point"
+cats = "cat_win.__main__:shell_entry_point"
 
 [project.urls]
 Github = "https://github.com/SilenZcience/cat_win"
 Download = "https://github.com/SilenZcience/cat_win/tarball/master"
 Tracker = "https://github.com/SilenZcience/cat_win/issues"
```

### Comparing `cat_win-1.3.1/PKG-INFO` & `cat_win-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: cat_win
-Version: 1.3.1
+Version: 1.4.0
 Summary: Simple OS Independent 'cat' Command-line Tool made in Python.
 Keywords: cat,cli,console,crossplatform,python,terminal
 Author-email: "Silas A. Kraume" <silas.kraume1552@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Terminals
+Classifier: Topic :: Text Processing :: Linguistic
 Requires-Dist: colorama~=0.4.6
 Requires-Dist: pyperclip~=1.8.0 ; extra == "clip"
 Project-URL: Download, https://github.com/SilenZcience/cat_win/tarball/master
 Project-URL: Github, https://github.com/SilenZcience/cat_win
 Project-URL: Tracker, https://github.com/SilenZcience/cat_win/issues
 Provides-Extra: clip
 
@@ -86,16 +89,16 @@
    </ol>
 </details>
 
 ## About The Project
 
 [![Unittests]](https://github.com/SilenZcience/cat_win/actions/workflows/unit_test.yml)
 [![Build-and-Check]](https://github.com/SilenZcience/cat_win/actions/workflows/package_test.yml)
-[![Coverage]]()
-[![Tests]]()
+[![Coverage]](https://raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-coverage.svg)
+[![Tests]](https://raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-tests.svg)
 <!-- [![Compile-and-Push]](https://github.com/SilenZcience/cat_win/actions/workflows/build_executable.yml/badge.svg) -->
 
 This project copies the fundamental framework of the cat command-line tool from Linux and translates its features to an OS Independent program using Python. </br> Over time the project evolved in subject areas of other tools like 'echo', 'grep', 'ls', 'base64'.
 
 Additionally it includes the feature to strip and reverse the content of any given file, make use of the standard-input, which enables cat piping into each other, generating the checksum of any file, converting decimal, hexadecimal and binary numbers within any text, and much <a href="#usage">more</a> ...
 
 Contrary to the name of the project it is of course possible to use cat_win on Linux or MacOS!
@@ -144,62 +147,63 @@
 ```console
 catw [FILE]... [OPTION]...
 catw --help
 ```
 
 > ⚠️ *from v1.0.33 to v1.1.0 the entrypoint changes from `cat` to `catw`. If you wish to keep the old command, you will have to define an alias yourself.*
 
-| Argument / Option      | Description                                       |
-|------------------------|---------------------------------------------------|
-| *-h, --help*           | show help message and exit                        |
-| *-v, --version*        | output version information                        |
-| *-d, --debug*          | show debug information                            |
-|                        |                                                   |
-| *-n, --number*         | number all output lines                           |
-| *-l, --linelength*     | display the length of each line                   |
-| *-e, --ends*           | display $ at the end of each line                 |
-| *-t, --tabs*           | display TAB characters as ^I                      |
-| *--eof, --eof*         | display EOF characters as ^EOF                    |
-| *-u, --unique*         | suppress repeated output lines                    |
-| *-b, --blank*          | hide empty lines                                  |
-| *-r, --reverse*        | reverse output                                    |
-| *-p, --peek*           | only print the first and last lines               |
-| *-s, --sum*            | show sum of lines                                 |
-| *-S, --SUM*            | ONLY show sum of lines                            |
-| *-f, --files*          | list applied files                                |
-| *-F, --FILES*          | ONLY list applied files and file sizes            |
-| *-g, --grep*           | only show lines containing queried keywords       |
-| *-i, --interactive*    | use stdin                                         |
-| *-o, --oneline*        | take only the first stdin-line                    |
-| *-E, --ECHO*           | handle every following parameter as stdin         |
-| *-c, --clip*           | copy output to clipboard                          |
-| *-m, --checksum*       | show the checksums of all files                   |
-| *-a, --attributes*     | show meta-information about the files             |
-|                        |                                                   |
-| *--dec, --DEC*         | convert decimal numbers to hexadecimal and binary |
-| *--hex, --HEX*         | convert hexadecimal numbers to decimal and binary |
-| *--bin, --BIN*         | convert binary numbers to decimal and hexadecimal |
-| *--b64e, --b64e*       | encode the input to base64                        |
-| *--b64d, --b64d*       | decode the input from base64                      |
-|                        |                                                   |
-| *--hexview, --HEXVIEW* | display the raw byte representation in hexadecimal|
-| *--binview, --binview* | display the raw byte representation in binary     |
-|                        |                                                   |
-| *--nc, --nocolor*      | disable colored output                            |
-| *--nb, --nobreak*      | do not interrupt the output on queried keywords   |
-| *--nk, --nokeyword*    | inverse the grep output                           |
-| *--config, --config*   | change color configuration                        |
-|                        |                                                   |
-| *enc=X*                | set file enconding to X (default is utf-8)        |
-| *find=X*               | find/query a substring X in the given files       |
-| *match=X*              | find/query a pattern X in the given files         |
-| *trunc=X:Y*            | truncate file to lines X and Y (python-like)      |
-|                        |                                                   |
-| *[a,b]*                | replace a with b in every line                    |
-| *[a:​b:c]*              | python-like string indexing syntax (line by line) |
+| Argument / Option      | Description                                               |
+|------------------------|-----------------------------------------------------------|
+| *-h, --help*           | show help message and exit                                |
+| *-v, --version*        | output version information                                |
+| *-d, --debug*          | show debug information                                    |
+|                        |                                                           |
+| *-n, --number*         | number all output lines                                   |
+| *-l, --linelength*     | display the length of each line                           |
+| *-e, --ends*           | display $ at the end of each line                         |
+| *-t, --tabs*           | display TAB characters as ^I                              |
+| *--eof, --eof*         | display EOF characters as ^EOF                            |
+| *-u, --unique*         | suppress repeated output lines                            |
+| *-b, --blank*          | hide empty lines                                          |
+| *-r, --reverse*        | reverse output                                            |
+| *-p, --peek*           | only print the first and last lines                       |
+| *-s, --sum*            | show sum of lines                                         |
+| *-S, --SUM*            | ONLY show sum of lines                                    |
+| *-f, --files*          | list applied files                                        |
+| *-F, --FILES*          | ONLY list applied files and file sizes                    |
+| *-g, --grep*           | only show lines containing queried keywords               |
+| *-i, --interactive*    | use stdin                                                 |
+| *-o, --oneline*        | take only the first stdin-line                            |
+| *-E, --ECHO*           | handle every following parameter as stdin                 |
+| *-c, --clip*           | copy output to clipboard                                  |
+| *-m, --checksum*       | show the checksums of all files                           |
+| *-a, --attributes*     | show meta-information about the files                     |
+|                        |                                                           |
+| *--dec, --DEC*         | convert decimal numbers to hexadecimal and binary         |
+| *--hex, --HEX*         | convert hexadecimal numbers to decimal and binary         |
+| *--bin, --BIN*         | convert binary numbers to decimal and hexadecimal         |
+| *--b64e, --b64e*       | encode the input to base64                                |
+| *--b64d, --b64d*       | decode the input from base64                              |
+|                        |                                                           |
+| *--hexview, --HEXVIEW* | display the raw byte representation in hexadecimal        |
+| *--binview, --binview* | display the raw byte representation in binary             |
+|                        |                                                           |
+| *--nc, --nocolor*      | disable colored output                                    |
+| *--nb, --nobreak*      | do not interrupt the output on queried keywords           |
+| *--nk, --nokeyword*    | inverse the grep output                                   |
+| *-R, --reconfigure*    | reconfigure the stdin and stdout with the parsed encoding |
+| *--config, --config*   | change color configuration                                |
+|                        |                                                           |
+| *enc=X*                | set file enconding to X (default is utf-8)                |
+| *find=X*               | find/query a substring X in the given files               |
+| *match=X*              | find/query a pattern X in the given files                 |
+| *trunc=X:Y*            | truncate file to lines X and Y (python-like)              |
+|                        |                                                           |
+| *[a,b]*                | replace a with b in every line                            |
+| *[a:​b:c]*              | python-like string indexing syntax (line by line)         |
 
 ### Examples
 
 <details open>
 	<summary><b>📂 Images 📂</b></summary>
 
 ![Example1](https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example1.png "example1")
@@ -217,14 +221,23 @@
 </details>
 
 ```console
 $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1] -ln
 > 1) [8] ): dlroW
 ```
 
+```c
+$ cats --dec -nl
+> >>> 12345
+> 1) [53] 12345 {Hexadecimal: 0x3039; Binary: 0b11000000111001}
+> >>> 54321
+> 2) [55] 54321 {Hexadecimal: 0xd431; Binary: 0b1101010000110001}
+> ...
+```
+
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Changelog
 
 Take a look at the [Changelog](https://github.com/SilenZcience/cat_win/blob/main/CHANGELOG.md) file.
 
 ## License
@@ -240,16 +253,16 @@
 [OS-Linux]: https://svgshare.com/i/Zhy.svg
 [OS-MacOS]: https://svgshare.com/i/ZjP.svg
 
 [Unittests]: https://github.com/SilenZcience/cat_win/actions/workflows/unit_test.yml/badge.svg
 [Build-and-Check]: https://github.com/SilenZcience/cat_win/actions/workflows/package_test.yml/badge.svg
 [Compile-and-Push]: https://github.com/SilenZcience/cat_win/actions/workflows/build_executable.yml/badge.svg
 
-[Coverage]: https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/badge-coverage.svg
-[Tests]: https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/badge-tests.svg
+[Coverage]: https://raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-coverage.svg
+[Tests]: https://raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-tests.svg
 
 [MadeWith-Python]: https://img.shields.io/badge/Made%20with-Python-brightgreen
 [Python-Version]: https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20pypy--3.8%20%7C%20pypy--3.9-blue
 
 [CurrentVersion]: https://img.shields.io/pypi/v/cat_win.svg
 
 [GitHub-SilenZcience]: https://img.shields.io/badge/GitHub-SilenZcience-orange
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 2.1 Name: cat_win Version: 1.3.1 Summary: Simple OS
+Metadata-Version: 2.1 Name: cat_win Version: 1.4.0 Summary: Simple OS
 Independent 'cat' Command-line Tool made in Python. Keywords:
 cat,cli,console,crossplatform,python,terminal Author-email: "Silas A. Kraume"
 kraume1552@gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Environment :: Console Classifier: Operating System :: OS Independent
-Classifier: Topic :: Terminals Requires-Dist: colorama~=0.4.6 Requires-Dist:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
+Implementation :: PyPy Classifier: Environment :: Console Classifier: Operating
+System :: OS Independent Classifier: Topic :: Terminals Classifier: Topic ::
+Text Processing :: Linguistic Requires-Dist: colorama~=0.4.6 Requires-Dist:
 pyperclip~=1.8.0 ; extra == "clip" Project-URL: Download, https://github.com/
 SilenZcience/cat_win/tarball/master Project-URL: Github, https://github.com/
 SilenZcience/cat_win Project-URL: Tracker, https://github.com/SilenZcience/
 cat_win/issues Provides-Extra: clip
 [https://static.pepy.tech/personalized-badge/cat-
 win?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads]
 [https://visitor-badge.laobi.icu/badge?page_id=SilenZcience.cat_win] [https://
@@ -32,25 +34,28 @@
    3. Usage
           o Examples
    4. Changelog
    5. License
    6. Contact
  ## About The Project [![Unittests]](https://github.com/SilenZcience/cat_win/
 actions/workflows/unit_test.yml) [![Build-and-Check]](https://github.com/
-SilenZcience/cat_win/actions/workflows/package_test.yml) [![Coverage]]() [!
-[Tests]]()  This project copies the fundamental framework of the cat command-
-line tool from Linux and translates its features to an OS Independent program
-using Python.  Over time the project evolved in subject areas of other tools
-like 'echo', 'grep', 'ls', 'base64'. Additionally it includes the feature to
-strip and reverse the content of any given file, make use of the standard-
-input, which enables cat piping into each other, generating the checksum of any
-file, converting decimal, hexadecimal and binary numbers within any text, and
-much more ... Contrary to the name of the project it is of course possible to
-use cat_win on Linux or MacOS! ### Made With [![MadeWith-Python]](https://
-www.python.org/) [![Python][Python-Version]](https://www.python.org/)
+SilenZcience/cat_win/actions/workflows/package_test.yml) [![Coverage]](https://
+raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-
+coverage.svg) [![Tests]](https://raw.githubusercontent.com/SilenZcience/
+cat_win/badges/.github/badges/badge-tests.svg)  This project copies the
+fundamental framework of the cat command-line tool from Linux and translates
+its features to an OS Independent program using Python.  Over time the project
+evolved in subject areas of other tools like 'echo', 'grep', 'ls', 'base64'.
+Additionally it includes the feature to strip and reverse the content of any
+given file, make use of the standard-input, which enables cat piping into each
+other, generating the checksum of any file, converting decimal, hexadecimal and
+binary numbers within any text, and much more ... Contrary to the name of the
+project it is of course possible to use cat_win on Linux or MacOS! ### Made
+With [![MadeWith-Python]](https://www.python.org/) [![Python][Python-Version]]
+(https://www.python.org/)
                                                                   (back_to_top)
 ## Getting Started ### Prerequisites - Using cat_win as a Python-Package
 demands a Python-Interpreter (>= 3.7). - Using cat_win as an Executable
 (Windows only!) demands no prerequisites, hereby the stand-alone executable
 `catw.exe` is sufficient. ### Installation [![Version][CurrentVersion]](https:/
 /pypi.org/project/cat-win/) Simply install the python package (via [PyPI-
 cat_win](https://pypi.org/project/cat-win/)): ```console python -m pip install
@@ -71,16 +76,16 @@
 corresponding [workflow](https://github.com/SilenZcience/cat_win/blob/
 main/.github/workflows/build_executable.yml) used.
                                                                   (back_to_top)
 ## Usage ```console catw [FILE]... [OPTION]... catw --help ``` > â ï¸ *from
 v1.0.33 to v1.1.0 the entrypoint changes from `cat` to `catw`. If you wish to
 keep the old command, you will have to define an alias yourself.* | Argument /
 Option | Description | |------------------------|------------------------------
----------------------| | *-h, --help* | show help message and exit | | *-v, --
-version* | output version information | | *-d, --debug* | show debug
+-----------------------------| | *-h, --help* | show help message and exit | |
+*-v, --version* | output version information | | *-d, --debug* | show debug
 information | | | | | *-n, --number* | number all output lines | | *-l, --
 linelength* | display the length of each line | | *-e, --ends* | display $ at
 the end of each line | | *-t, --tabs* | display TAB characters as ^I | | *--
 eof, --eof* | display EOF characters as ^EOF | | *-u, --unique* | suppress
 repeated output lines | | *-b, --blank* | hide empty lines | | *-r, --reverse*
 | reverse output | | *-p, --peek* | only print the first and last lines | | *-
 s, --sum* | show sum of lines | | *-S, --SUM* | ONLY show sum of lines | | *-f,
@@ -91,47 +96,51 @@
 c, --clip* | copy output to clipboard | | *-m, --checksum* | show the checksums
 of all files | | *-a, --attributes* | show meta-information about the files | |
 | | | *--dec, --DEC* | convert decimal numbers to hexadecimal and binary | | *-
 -hex, --HEX* | convert hexadecimal numbers to decimal and binary | | *--bin, --
 BIN* | convert binary numbers to decimal and hexadecimal | | *--b64e, --b64e* |
 encode the input to base64 | | *--b64d, --b64d* | decode the input from base64
 | | | | | *--hexview, --HEXVIEW* | display the raw byte representation in
-hexadecimal| | *--binview, --binview* | display the raw byte representation in
+hexadecimal | | *--binview, --binview* | display the raw byte representation in
 binary | | | | | *--nc, --nocolor* | disable colored output | | *--nb, --
 nobreak* | do not interrupt the output on queried keywords | | *--nk, --
-nokeyword* | inverse the grep output | | *--config, --config* | change color
-configuration | | | | | *enc=X* | set file enconding to X (default is utf-8) |
-| *find=X* | find/query a substring X in the given files | | *match=X* | find/
-query a pattern X in the given files | | *trunc=X:Y* | truncate file to lines X
-and Y (python-like) | | | | | *[a,b]* | replace a with b in every line | | *[a:
-âb:c]* | python-like string indexing syntax (line by line) | ### Examples
-ð Images ð ![Example1](https://raw.githubusercontent.com/SilenZcience/
-cat_win/main/img/example1.png "example1") ![Example2](https://
+nokeyword* | inverse the grep output | | *-R, --reconfigure* | reconfigure the
+stdin and stdout with the parsed encoding | | *--config, --config* | change
+color configuration | | | | | *enc=X* | set file enconding to X (default is
+utf-8) | | *find=X* | find/query a substring X in the given files | | *match=X*
+| find/query a pattern X in the given files | | *trunc=X:Y* | truncate file to
+lines X and Y (python-like) | | | | | *[a,b]* | replace a with b in every line
+| | *[a:âb:c]* | python-like string indexing syntax (line by line) | ###
+Examples  ð Images ð ![Example1](https://raw.githubusercontent.com/
+SilenZcience/cat_win/main/img/example1.png "example1") ![Example2](https://
 raw.githubusercontent.com/SilenZcience/cat_win/main/img/example2.png
 "example2") ![Example3](https://raw.githubusercontent.com/SilenZcience/cat_win/
 main/img/example3.png "example3") ![Example4](https://
 raw.githubusercontent.com/SilenZcience/cat_win/main/img/example4.png
 "example4") ![Example5](https://raw.githubusercontent.com/SilenZcience/cat_win/
 main/img/example5.png "example5") ![Example6](https://
 raw.githubusercontent.com/SilenZcience/cat_win/main/img/example6.png
 "example6")  ```console $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1]
--ln > 1) [8] ): dlroW ```
+-ln > 1) [8] ): dlroW ``` ```c $ cats --dec -nl > >>> 12345 > 1) [53] 12345
+{Hexadecimal: 0x3039; Binary: 0b11000000111001} > >>> 54321 > 2) [55] 54321
+{Hexadecimal: 0xd431; Binary: 0b1101010000110001} > ... ```
                                                                   (back_to_top)
 ## Changelog Take a look at the [Changelog](https://github.com/SilenZcience/
 cat_win/blob/main/CHANGELOG.md) file. ## License This project is licensed under
 the MIT License - see the [LICENSE](https://github.com/SilenZcience/cat_win/
 blob/main/LICENSE) file for details ## Contact > **SilenZcience**
 [![GitHub-SilenZcience][GitHub-SilenZcience]](https://github.com/SilenZcience)
 [OS-Windows]: https://svgshare.com/i/ZhY.svg [OS-Linux]: https://svgshare.com/
 i/Zhy.svg [OS-MacOS]: https://svgshare.com/i/ZjP.svg [Unittests]: https://
 github.com/SilenZcience/cat_win/actions/workflows/unit_test.yml/badge.svg
 [Build-and-Check]: https://github.com/SilenZcience/cat_win/actions/workflows/
 package_test.yml/badge.svg [Compile-and-Push]: https://github.com/SilenZcience/
 cat_win/actions/workflows/build_executable.yml/badge.svg [Coverage]: https://
-raw.githubusercontent.com/SilenZcience/cat_win/main/img/badge-coverage.svg
-[Tests]: https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/badge-
-tests.svg [MadeWith-Python]: https://img.shields.io/badge/Made%20with-Python-
-brightgreen [Python-Version]: https://img.shields.io/badge/Python-
+raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-
+coverage.svg [Tests]: https://raw.githubusercontent.com/SilenZcience/cat_win/
+badges/.github/badges/badge-tests.svg [MadeWith-Python]: https://
+img.shields.io/badge/Made%20with-Python-brightgreen [Python-Version]: https://
+img.shields.io/badge/Python-
 3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20pypy--
 3.8%20%7C%20pypy--3.9-blue [CurrentVersion]: https://img.shields.io/pypi/v/
 cat_win.svg [GitHub-SilenZcience]: https://img.shields.io/badge/GitHub-
 SilenZcience-orange
```

