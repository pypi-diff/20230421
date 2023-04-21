# Comparing `tmp/yara-python-4.3.0.tar.gz` & `tmp/yara-python-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yara-python-4.3.0.tar", last modified: Mon Mar 27 14:38:43 2023, max compression
+gzip compressed data, was "yara-python-4.3.1.tar", last modified: Fri Apr 21 09:39:07 2023, max compression
```

## Comparing `yara-python-4.3.0.tar` & `yara-python-4.3.1.tar`

### file list

```diff
@@ -1,206 +1,206 @@
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:43.000000 yara-python-4.3.0/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2890 2023-03-27 14:38:43.000000 yara-python-4.3.0/PKG-INFO
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    11358 2021-10-06 07:40:40.000000 yara-python-4.3.0/LICENSE
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    77465 2022-12-19 15:45:02.000000 yara-python-4.3.0/yara-python.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:43.000000 yara-python-4.3.0/yara_python.egg-info/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2890 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara_python.egg-info/PKG-INFO
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)        1 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara_python.egg-info/not-zip-safe
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5224 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara_python.egg-info/SOURCES.txt
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)        5 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara_python.egg-info/top_level.txt
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)        1 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara_python.egg-info/dependency_links.txt
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:43.000000 yara-python-4.3.0/yara/tests/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5607 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/tests/test-alignment.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)   109762 2023-03-22 09:00:37.000000 yara-python-4.3.0/yara/tests/test-rules.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1969 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/tests/test-version.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    18015 2022-03-04 08:54:33.000000 yara-python-4.3.0/yara/tests/util.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5841 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/tests/test-arena.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2777 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/tests/test-re-split.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5883 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/tests/test-dotnet.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    11056 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/tests/test-async.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)   172092 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/tests/blob.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    22297 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/tests/test-atoms.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2694 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/tests/test-stack.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    26663 2023-03-22 09:00:37.000000 yara-python-4.3.0/yara/tests/test-api.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     9691 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/tests/test-macho.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6258 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/tests/test-bitmask.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3322 2022-12-30 10:32:25.000000 yara-python-4.3.0/yara/tests/test-string.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4078 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/tests/test-dex.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     7513 2023-03-22 09:00:37.000000 yara-python-4.3.0/yara/tests/test-elf.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    16475 2022-03-04 08:54:33.000000 yara-python-4.3.0/yara/tests/util.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2496 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/tests/test-pb.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5996 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/tests/test-math.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     7558 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/tests/test-exception.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1338 2023-03-22 09:00:37.000000 yara-python-4.3.0/yara/tests/test-magic.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    33831 2023-03-22 09:02:27.000000 yara-python-4.3.0/yara/tests/test-pe.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2741 2022-03-04 08:53:36.000000 yara-python-4.3.0/yara/tests/mapper.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/cli/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6390 2022-03-04 08:54:33.000000 yara-python-4.3.0/yara/cli/common.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     7839 2022-08-09 07:50:12.000000 yara-python-4.3.0/yara/cli/args.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2660 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/cli/threading.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6803 2022-08-09 07:50:12.000000 yara-python-4.3.0/yara/cli/yarac.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2233 2022-08-09 07:50:12.000000 yara-python-4.3.0/yara/cli/unicode.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3665 2022-08-09 07:50:12.000000 yara-python-4.3.0/yara/cli/args.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1891 2022-03-04 08:53:36.000000 yara-python-4.3.0/yara/cli/common.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    40075 2023-03-22 09:02:27.000000 yara-python-4.3.0/yara/cli/yara.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5207 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/cli/threading.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:43.000000 yara-python-4.3.0/yara/libyara/proc/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5280 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/proc/freebsd.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5190 2022-08-09 07:50:12.000000 yara-python-4.3.0/yara/libyara/proc/mach.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5793 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/proc/openbsd.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2163 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/proc/none.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    11385 2023-03-22 09:02:27.000000 yara-python-4.3.0/yara/libyara/proc/linux.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5827 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/proc/windows.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    10196 2023-03-22 09:00:37.000000 yara-python-4.3.0/yara/libyara/filemap.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    21894 2023-03-22 09:00:37.000000 yara-python-4.3.0/yara/libyara/scanner.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5712 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    26235 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/object.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:43.000000 yara-python-4.3.0/yara/libyara/tlshc/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      629 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/tlshc/tlsh_util.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1209 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/tlshc/tlsh.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3217 2023-03-22 09:02:27.000000 yara-python-4.3.0/yara/libyara/tlshc/tlsh_impl.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)   272510 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/tlshc/tlsh_util.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    31799 2023-03-22 09:02:27.000000 yara-python-4.3.0/yara/libyara/tlshc/tlsh_impl.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    64176 2023-03-22 09:00:37.000000 yara-python-4.3.0/yara/libyara/exec.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    43396 2023-03-22 09:00:37.000000 yara-python-4.3.0/yara/libyara/atoms.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4229 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/stopwatch.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3962 2022-03-04 08:54:33.000000 yara-python-4.3.0/yara/libyara/stack.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)   185156 2022-12-30 10:32:25.000000 yara-python-4.3.0/yara/libyara/grammar.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3410 2022-03-04 08:53:36.000000 yara-python-4.3.0/yara/libyara/mem.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    13288 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/rules.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/include/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1846 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara.h
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/include/tlshc/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1907 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/tlshc/tlsh.h
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/include/yara/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6888 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/error.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5071 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/utils.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2925 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/unaligned.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1748 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/exefiles.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2183 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/proc.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3031 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/strutils.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    13823 2022-12-30 10:32:25.000000 yara-python-4.3.0/yara/libyara/include/yara/compiler.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1865 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/base64.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      527 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/elf_utils.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3382 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/hex_lexer.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    30041 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/types.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6081 2022-03-04 08:54:33.000000 yara-python-4.3.0/yara/libyara/include/yara/limits.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2669 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/ahocorasick.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2951 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/endian.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4075 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/parser.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5664 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/re.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2310 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/threading.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3476 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/bitmask.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3963 2022-12-30 10:32:25.000000 yara-python-4.3.0/yara/libyara/include/yara/libyara.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2102 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/stream.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2858 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/dex.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4599 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/globals.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2883 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/sizedstr.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      489 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/simple_str.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    10628 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/elf.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    14641 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/modules.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    27171 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/pe.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3306 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/scanner.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2451 2021-10-22 07:47:52.000000 yara-python-4.3.0/yara/libyara/include/yara/filemap.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2352 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/stopwatch.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3738 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/atoms.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2249 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/stack.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2188 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/pe_utils.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     7826 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/exec.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    16232 2023-03-22 09:02:27.000000 yara-python-4.3.0/yara/libyara/include/yara/macho.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    13273 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/yara/dotnet.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4340 2022-03-10 09:24:58.000000 yara-python-4.3.0/yara/libyara/include/yara/object.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3141 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/lexer.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3325 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/re_lexer.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3061 2022-03-04 08:54:33.000000 yara-python-4.3.0/yara/libyara/include/yara/integers.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2075 2022-03-04 08:53:36.000000 yara-python-4.3.0/yara/libyara/include/yara/mem.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5054 2022-03-04 08:54:33.000000 yara-python-4.3.0/yara/libyara/include/yara/rules.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     8948 2023-03-22 09:00:37.000000 yara-python-4.3.0/yara/libyara/include/yara/arena.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      356 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/notebook.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3829 2022-03-04 08:54:33.000000 yara-python-4.3.0/yara/libyara/include/yara/hash.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2055 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/include/yara/scan.h
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/include/authenticode-parser/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     8449 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/include/authenticode-parser/authenticode.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3126 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/hex_grammar.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    75086 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/re_lexer.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    97358 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/lexer.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    29155 2023-03-22 09:00:37.000000 yara-python-4.3.0/yara/libyara/scan.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3678 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/re_grammar.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    12438 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/hash.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5872 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/notebook.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    20907 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/arena.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5601 2022-12-30 10:32:25.000000 yara-python-4.3.0/yara/libyara/crypto.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    67756 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/hex_lexer.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     7653 2022-12-30 10:32:25.000000 yara-python-4.3.0/yara/libyara/grammar.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    13283 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/base64.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    11742 2023-03-22 09:02:27.000000 yara-python-4.3.0/yara/libyara/exefiles.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    28991 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/compiler.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3460 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/proc.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6187 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/strutils.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    54980 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/hex_grammar.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    71585 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/re.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4102 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/bitmask.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4310 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/threading.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2164 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/endian.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    25787 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/ahocorasick.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/modules/
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/modules/demo/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2048 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/demo/demo.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:43.000000 yara-python-4.3.0/yara/libyara/modules/pe/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)   128887 2023-03-22 09:02:27.000000 yara-python-4.3.0/yara/libyara/modules/pe/pe.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    41920 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/pe/pe_utils.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:43.000000 yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2084 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/countersignature.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2271 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/helper.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    12614 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/certificate.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3548 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/structs.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    20520 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/authenticode.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1678 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/certificate.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2310 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/helper.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    11228 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/countersignature.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3157 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/structs.h
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/modules/magic/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5213 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/magic/magic.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/modules/hash/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    23882 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/hash/hash.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/modules/macho/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    45919 2023-03-22 09:02:27.000000 yara-python-4.3.0/yara/libyara/modules/macho/macho.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:43.000000 yara-python-4.3.0/yara/libyara/modules/tests/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5976 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/tests/tests.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/modules/math/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    19010 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/math/math.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:43.000000 yara-python-4.3.0/yara/libyara/modules/time/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2158 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/modules/time/time.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/modules/dotnet/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    99340 2023-03-22 09:02:27.000000 yara-python-4.3.0/yara/libyara/modules/dotnet/dotnet.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/modules/cuckoo/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    11063 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/cuckoo/cuckoo.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/modules/dex/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    43958 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/dex/dex.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:43.000000 yara-python-4.3.0/yara/libyara/modules/string/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3277 2022-12-30 10:32:25.000000 yara-python-4.3.0/yara/libyara/modules/string/string.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      392 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/module_list
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/modules/elf/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    64717 2023-03-22 09:02:27.000000 yara-python-4.3.0/yara/libyara/modules/elf/elf.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:42.000000 yara-python-4.3.0/yara/libyara/modules/console/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     7742 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/console/console.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:43.000000 yara-python-4.3.0/yara/libyara/modules/pb_tests/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    30364 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/modules/pb_tests/pb_tests.pb-c.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      130 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/modules/pb_tests/yara.pb-c.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     7790 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/modules/pb_tests/pb_tests.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    11806 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/modules/pb_tests/pb_tests.pb-c.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     8301 2022-03-04 08:54:33.000000 yara-python-4.3.0/yara/libyara/exception.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    40193 2023-03-22 09:00:37.000000 yara-python-4.3.0/yara/libyara/parser.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3214 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/simple_str.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6963 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/sizedstr.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    58976 2022-12-19 15:50:06.000000 yara-python-4.3.0/yara/libyara/re_grammar.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    19815 2022-03-04 08:54:33.000000 yara-python-4.3.0/yara/libyara/libyara.c
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1942 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/libyara/stream.c
-drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-03-27 14:38:43.000000 yara-python-4.3.0/yara/sandbox/
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1889 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/sandbox/collect_matches.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4549 2021-10-06 07:40:45.000000 yara-python-4.3.0/yara/sandbox/yara_transaction.h
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      100 2021-10-06 07:40:40.000000 yara-python-4.3.0/MANIFEST.in
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    13747 2023-03-22 09:03:21.000000 yara-python-4.3.0/setup.py
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      130 2023-03-27 14:38:43.000000 yara-python-4.3.0/setup.cfg
--rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1882 2022-12-19 16:31:14.000000 yara-python-4.3.0/README.rst
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.068909 yara-python-4.3.1/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    11358 2021-10-06 07:40:40.000000 yara-python-4.3.1/LICENSE
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      100 2021-10-06 07:40:40.000000 yara-python-4.3.1/MANIFEST.in
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2612 2023-04-21 09:39:07.069027 yara-python-4.3.1/PKG-INFO
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2113 2023-03-31 08:15:29.000000 yara-python-4.3.1/README.rst
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      130 2023-04-21 09:39:07.069509 yara-python-4.3.1/setup.cfg
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    13747 2023-04-21 08:29:47.000000 yara-python-4.3.1/setup.py
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:06.963215 yara-python-4.3.1/yara/
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:06.972811 yara-python-4.3.1/yara/cli/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     7839 2022-08-09 07:50:12.000000 yara-python-4.3.1/yara/cli/args.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3665 2022-08-09 07:50:12.000000 yara-python-4.3.1/yara/cli/args.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6390 2022-03-04 08:54:33.000000 yara-python-4.3.1/yara/cli/common.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1891 2022-03-04 08:53:36.000000 yara-python-4.3.1/yara/cli/common.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5207 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/cli/threading.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2660 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/cli/threading.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2233 2022-08-09 07:50:12.000000 yara-python-4.3.1/yara/cli/unicode.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    40075 2023-03-22 09:02:27.000000 yara-python-4.3.1/yara/cli/yara.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6803 2022-08-09 07:50:12.000000 yara-python-4.3.1/yara/cli/yarac.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.003297 yara-python-4.3.1/yara/libyara/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    25787 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/ahocorasick.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    20907 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/arena.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    43396 2023-03-22 09:00:37.000000 yara-python-4.3.1/yara/libyara/atoms.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    13283 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/base64.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4102 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/bitmask.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    28991 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/compiler.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5601 2022-12-30 10:32:25.000000 yara-python-4.3.1/yara/libyara/crypto.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2164 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/endian.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     8301 2022-03-04 08:54:33.000000 yara-python-4.3.1/yara/libyara/exception.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    64176 2023-03-22 09:00:37.000000 yara-python-4.3.1/yara/libyara/exec.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    11742 2023-03-22 09:02:27.000000 yara-python-4.3.1/yara/libyara/exefiles.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    10196 2023-03-22 09:00:37.000000 yara-python-4.3.1/yara/libyara/filemap.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)   185156 2022-12-30 10:32:25.000000 yara-python-4.3.1/yara/libyara/grammar.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     7653 2022-12-30 10:32:25.000000 yara-python-4.3.1/yara/libyara/grammar.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    12438 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/hash.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    54980 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/hex_grammar.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3126 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/hex_grammar.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    67756 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/hex_lexer.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.003697 yara-python-4.3.1/yara/libyara/include/
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.004091 yara-python-4.3.1/yara/libyara/include/authenticode-parser/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     8449 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/authenticode-parser/authenticode.h
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.004488 yara-python-4.3.1/yara/libyara/include/tlshc/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1907 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/tlshc/tlsh.h
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.027566 yara-python-4.3.1/yara/libyara/include/yara/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2669 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/ahocorasick.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     8948 2023-03-22 09:00:37.000000 yara-python-4.3.1/yara/libyara/include/yara/arena.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3738 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/atoms.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1865 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/base64.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3476 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/bitmask.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    13823 2022-12-30 10:32:25.000000 yara-python-4.3.1/yara/libyara/include/yara/compiler.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2858 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/dex.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    13273 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/dotnet.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    10628 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/elf.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      527 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/elf_utils.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2951 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/endian.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6888 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/error.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     7826 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/exec.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1748 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/exefiles.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2451 2021-10-22 07:47:52.000000 yara-python-4.3.1/yara/libyara/include/yara/filemap.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4599 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/globals.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3829 2022-03-04 08:54:33.000000 yara-python-4.3.1/yara/libyara/include/yara/hash.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3382 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/hex_lexer.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3061 2022-03-04 08:54:33.000000 yara-python-4.3.1/yara/libyara/include/yara/integers.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3141 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/lexer.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3959 2023-04-21 07:43:13.000000 yara-python-4.3.1/yara/libyara/include/yara/libyara.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6081 2022-03-04 08:54:33.000000 yara-python-4.3.1/yara/libyara/include/yara/limits.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    16232 2023-03-22 09:02:27.000000 yara-python-4.3.1/yara/libyara/include/yara/macho.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2075 2022-03-04 08:53:36.000000 yara-python-4.3.1/yara/libyara/include/yara/mem.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    14641 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/modules.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      356 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/notebook.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4340 2022-03-10 09:24:58.000000 yara-python-4.3.1/yara/libyara/include/yara/object.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4075 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/parser.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    27171 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/pe.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2188 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/pe_utils.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2183 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/proc.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5664 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/re.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3325 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/re_lexer.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5054 2022-03-04 08:54:33.000000 yara-python-4.3.1/yara/libyara/include/yara/rules.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2055 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/scan.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3306 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/scanner.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      489 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/simple_str.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2883 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/sizedstr.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2249 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/stack.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2352 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/stopwatch.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2102 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/stream.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3031 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/strutils.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2310 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/include/yara/threading.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    30041 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/types.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2925 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/unaligned.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5071 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara/utils.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1846 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/include/yara.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    97358 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/lexer.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    19815 2022-03-04 08:54:33.000000 yara-python-4.3.1/yara/libyara/libyara.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3410 2022-03-04 08:53:36.000000 yara-python-4.3.1/yara/libyara/mem.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.027942 yara-python-4.3.1/yara/libyara/modules/
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.028552 yara-python-4.3.1/yara/libyara/modules/console/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     7742 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/console/console.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.029071 yara-python-4.3.1/yara/libyara/modules/cuckoo/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    11063 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/cuckoo/cuckoo.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.029697 yara-python-4.3.1/yara/libyara/modules/demo/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2048 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/demo/demo.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.030179 yara-python-4.3.1/yara/libyara/modules/dex/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    43958 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/dex/dex.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.030899 yara-python-4.3.1/yara/libyara/modules/dotnet/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    99343 2023-04-21 07:42:31.000000 yara-python-4.3.1/yara/libyara/modules/dotnet/dotnet.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.032092 yara-python-4.3.1/yara/libyara/modules/elf/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    64717 2023-03-22 09:02:27.000000 yara-python-4.3.1/yara/libyara/modules/elf/elf.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.033313 yara-python-4.3.1/yara/libyara/modules/hash/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    23882 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/hash/hash.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.034040 yara-python-4.3.1/yara/libyara/modules/macho/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    45919 2023-03-22 09:02:27.000000 yara-python-4.3.1/yara/libyara/modules/macho/macho.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.034659 yara-python-4.3.1/yara/libyara/modules/magic/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5213 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/magic/magic.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.035009 yara-python-4.3.1/yara/libyara/modules/math/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    19010 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/math/math.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      392 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/module_list
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.037548 yara-python-4.3.1/yara/libyara/modules/pb_tests/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     7790 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/pb_tests/pb_tests.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    30364 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/modules/pb_tests/pb_tests.pb-c.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    11806 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/modules/pb_tests/pb_tests.pb-c.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      130 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/modules/pb_tests/yara.pb-c.h
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.038925 yara-python-4.3.1/yara/libyara/modules/pe/
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.043632 yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    20520 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/authenticode.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    12614 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/certificate.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1678 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/certificate.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    11228 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/countersignature.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2084 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/countersignature.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2310 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/helper.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2271 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/helper.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3548 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/structs.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3157 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/structs.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)   128893 2023-04-21 07:42:31.000000 yara-python-4.3.1/yara/libyara/modules/pe/pe.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    41920 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/pe/pe_utils.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.044033 yara-python-4.3.1/yara/libyara/modules/string/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3277 2022-12-30 10:32:25.000000 yara-python-4.3.1/yara/libyara/modules/string/string.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.044619 yara-python-4.3.1/yara/libyara/modules/tests/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5976 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules/tests/tests.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.045004 yara-python-4.3.1/yara/libyara/modules/time/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2158 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/modules/time/time.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5712 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/modules.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6234 2023-04-21 07:43:13.000000 yara-python-4.3.1/yara/libyara/notebook.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    26235 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/object.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    40193 2023-03-22 09:00:37.000000 yara-python-4.3.1/yara/libyara/parser.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.048095 yara-python-4.3.1/yara/libyara/proc/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5280 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/proc/freebsd.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    11385 2023-03-22 09:02:27.000000 yara-python-4.3.1/yara/libyara/proc/linux.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5190 2022-08-09 07:50:12.000000 yara-python-4.3.1/yara/libyara/proc/mach.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2163 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/proc/none.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5793 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/proc/openbsd.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5827 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/proc/windows.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3460 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/proc.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    71585 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/re.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    58976 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/re_grammar.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3678 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/re_grammar.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    75086 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/re_lexer.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    13288 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/rules.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    29155 2023-03-22 09:00:37.000000 yara-python-4.3.1/yara/libyara/scan.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    21894 2023-03-22 09:00:37.000000 yara-python-4.3.1/yara/libyara/scanner.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3214 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/simple_str.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6963 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/sizedstr.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3962 2022-03-04 08:54:33.000000 yara-python-4.3.1/yara/libyara/stack.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4229 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/stopwatch.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1942 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/stream.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6187 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/strutils.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4310 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/libyara/threading.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.051337 yara-python-4.3.1/yara/libyara/tlshc/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1209 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/tlshc/tlsh.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    31799 2023-03-22 09:02:27.000000 yara-python-4.3.1/yara/libyara/tlshc/tlsh_impl.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3217 2023-03-22 09:02:27.000000 yara-python-4.3.1/yara/libyara/tlshc/tlsh_impl.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)   272510 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/tlshc/tlsh_util.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)      629 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/libyara/tlshc/tlsh_util.h
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.052032 yara-python-4.3.1/yara/sandbox/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1889 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/sandbox/collect_matches.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4549 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/sandbox/yara_transaction.h
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.066692 yara-python-4.3.1/yara/tests/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)   172092 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/tests/blob.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2741 2022-03-04 08:53:36.000000 yara-python-4.3.1/yara/tests/mapper.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5607 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/tests/test-alignment.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    26663 2023-03-22 09:00:37.000000 yara-python-4.3.1/yara/tests/test-api.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5841 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/tests/test-arena.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    11056 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/tests/test-async.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    22297 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/tests/test-atoms.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     6258 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/tests/test-bitmask.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     4078 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/tests/test-dex.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5883 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/tests/test-dotnet.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     7513 2023-03-22 09:00:37.000000 yara-python-4.3.1/yara/tests/test-elf.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     7558 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/tests/test-exception.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     9691 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/tests/test-macho.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1338 2023-03-22 09:00:37.000000 yara-python-4.3.1/yara/tests/test-magic.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5996 2022-12-19 15:50:06.000000 yara-python-4.3.1/yara/tests/test-math.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2496 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/tests/test-pb.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    34099 2023-04-21 07:42:31.000000 yara-python-4.3.1/yara/tests/test-pe.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2777 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/tests/test-re-split.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)   109762 2023-03-22 09:00:37.000000 yara-python-4.3.1/yara/tests/test-rules.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2694 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/tests/test-stack.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     3322 2022-12-30 10:32:25.000000 yara-python-4.3.1/yara/tests/test-string.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     1969 2021-10-06 07:40:45.000000 yara-python-4.3.1/yara/tests/test-version.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    18015 2022-03-04 08:54:33.000000 yara-python-4.3.1/yara/tests/util.c
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    16475 2022-03-04 08:54:33.000000 yara-python-4.3.1/yara/tests/util.h
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)    77465 2022-12-19 15:45:02.000000 yara-python-4.3.1/yara-python.c
+drwxr-xr-x   0 vmalvarez (178948) primarygroup (89939)        0 2023-04-21 09:39:07.068596 yara-python-4.3.1/yara_python.egg-info/
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     2612 2023-04-21 09:39:06.000000 yara-python-4.3.1/yara_python.egg-info/PKG-INFO
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)     5224 2023-04-21 09:39:06.000000 yara-python-4.3.1/yara_python.egg-info/SOURCES.txt
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)        1 2023-04-21 09:39:06.000000 yara-python-4.3.1/yara_python.egg-info/dependency_links.txt
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)        1 2023-04-21 09:39:06.000000 yara-python-4.3.1/yara_python.egg-info/not-zip-safe
+-rw-r--r--   0 vmalvarez (178948) primarygroup (89939)        5 2023-04-21 09:39:06.000000 yara-python-4.3.1/yara_python.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yara-python-4.3.0/LICENSE` & `yara-python-4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara-python.c` & `yara-python-4.3.1/yara-python.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara_python.egg-info/SOURCES.txt` & `yara-python-4.3.1/yara_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-alignment.c` & `yara-python-4.3.1/yara/tests/test-alignment.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-rules.c` & `yara-python-4.3.1/yara/tests/test-rules.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-version.c` & `yara-python-4.3.1/yara/tests/test-version.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/util.c` & `yara-python-4.3.1/yara/tests/util.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-arena.c` & `yara-python-4.3.1/yara/tests/test-arena.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-re-split.c` & `yara-python-4.3.1/yara/tests/test-re-split.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-dotnet.c` & `yara-python-4.3.1/yara/tests/test-dotnet.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-async.c` & `yara-python-4.3.1/yara/tests/test-async.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/blob.h` & `yara-python-4.3.1/yara/tests/blob.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-atoms.c` & `yara-python-4.3.1/yara/tests/test-atoms.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-stack.c` & `yara-python-4.3.1/yara/tests/test-stack.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-api.c` & `yara-python-4.3.1/yara/tests/test-api.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-macho.c` & `yara-python-4.3.1/yara/tests/test-macho.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-bitmask.c` & `yara-python-4.3.1/yara/tests/test-bitmask.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-string.c` & `yara-python-4.3.1/yara/tests/test-string.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-dex.c` & `yara-python-4.3.1/yara/tests/test-dex.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-elf.c` & `yara-python-4.3.1/yara/tests/test-elf.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/util.h` & `yara-python-4.3.1/yara/tests/util.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-pb.c` & `yara-python-4.3.1/yara/tests/test-pb.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-math.c` & `yara-python-4.3.1/yara/tests/test-math.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-exception.c` & `yara-python-4.3.1/yara/tests/test-exception.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-magic.c` & `yara-python-4.3.1/yara/tests/test-magic.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/tests/test-pe.c` & `yara-python-4.3.1/yara/tests/test-pe.c`

 * *Files 0% similar despite different names*

```diff
@@ -878,30 +878,34 @@
           for any section in pe.sections : ( \
               section.name == \"/4\" and\
               section.full_name == \".debug_aranges\" \
           )\
       }",
       "tests/data/pe_mingw");
 
+  // These are intentionally using DLL and function names with incorrect case
+  // to be sure the string compare is case insensitive.
   assert_true_rule_file(
       "import \"pe\" \
       rule test { \
         condition: \
-          pe.import_rva(\"PtImageRW.dll\", \"ord4\") == 254924 and \
-          pe.import_rva(\"PtPDF417Decode.dll\", 4) == 254948 \
+          pe.import_rva(\"ptimagerw.dll\", \"ORD4\") == 254924 and \
+          pe.import_rva(\"ptPDF417decode.dll\", 4) == 254948 \
       }",
       "tests/data/"
       "ca21e1c32065352d352be6cde97f89c141d7737ea92434831f998080783d5386");
 
+  // These are intentionally using DLL and function names with incorrect case
+  // to be sure the string compare is case insensitive.
   assert_true_rule_file(
       "import \"pe\" \
       rule test { \
         condition: \
-          pe.delayed_import_rva(\"QDB.dll\", \"ord116\") == \
-          pe.delayed_import_rva(\"QDB.dll\", 116) \
+          pe.delayed_import_rva(\"qdb.dll\", \"ORD116\") == \
+          pe.delayed_import_rva(\"qdb.dll\", 116) \
       }",
       "tests/data/"
       "079a472d22290a94ebb212aa8015cdc8dd28a968c6b4d3b88acdd58ce2d3b885");
 
   // The first 0x410 bytes of
   // c6f9709feccf42f2d9e22057182fe185f177fb9daaa2649b4669a24f2ee7e3ba are enough
   // to trigger the bug in https://github.com/VirusTotal/yara/pull/1561
```

### Comparing `yara-python-4.3.0/yara/tests/mapper.c` & `yara-python-4.3.1/yara/tests/mapper.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/cli/common.c` & `yara-python-4.3.1/yara/cli/common.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/cli/args.c` & `yara-python-4.3.1/yara/cli/args.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/cli/threading.h` & `yara-python-4.3.1/yara/cli/threading.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/cli/yarac.c` & `yara-python-4.3.1/yara/cli/yarac.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/cli/unicode.h` & `yara-python-4.3.1/yara/cli/unicode.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/cli/args.h` & `yara-python-4.3.1/yara/cli/args.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/cli/common.h` & `yara-python-4.3.1/yara/cli/common.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/cli/yara.c` & `yara-python-4.3.1/yara/cli/yara.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/cli/threading.c` & `yara-python-4.3.1/yara/cli/threading.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/proc/freebsd.c` & `yara-python-4.3.1/yara/libyara/proc/freebsd.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/proc/mach.c` & `yara-python-4.3.1/yara/libyara/proc/mach.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/proc/openbsd.c` & `yara-python-4.3.1/yara/libyara/proc/openbsd.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/proc/none.c` & `yara-python-4.3.1/yara/libyara/proc/none.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/proc/linux.c` & `yara-python-4.3.1/yara/libyara/proc/linux.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/proc/windows.c` & `yara-python-4.3.1/yara/libyara/proc/windows.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/filemap.c` & `yara-python-4.3.1/yara/libyara/filemap.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/scanner.c` & `yara-python-4.3.1/yara/libyara/scanner.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules.c` & `yara-python-4.3.1/yara/libyara/modules.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/object.c` & `yara-python-4.3.1/yara/libyara/object.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/tlshc/tlsh_util.h` & `yara-python-4.3.1/yara/libyara/tlshc/tlsh_util.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/tlshc/tlsh.c` & `yara-python-4.3.1/yara/libyara/tlshc/tlsh.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/tlshc/tlsh_impl.h` & `yara-python-4.3.1/yara/libyara/tlshc/tlsh_impl.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/tlshc/tlsh_util.c` & `yara-python-4.3.1/yara/libyara/tlshc/tlsh_util.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/tlshc/tlsh_impl.c` & `yara-python-4.3.1/yara/libyara/tlshc/tlsh_impl.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/exec.c` & `yara-python-4.3.1/yara/libyara/exec.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/atoms.c` & `yara-python-4.3.1/yara/libyara/atoms.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/stopwatch.c` & `yara-python-4.3.1/yara/libyara/stopwatch.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/stack.c` & `yara-python-4.3.1/yara/libyara/stack.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/grammar.c` & `yara-python-4.3.1/yara/libyara/grammar.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/mem.c` & `yara-python-4.3.1/yara/libyara/mem.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/rules.c` & `yara-python-4.3.1/yara/libyara/rules.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara.h` & `yara-python-4.3.1/yara/libyara/include/yara.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/tlshc/tlsh.h` & `yara-python-4.3.1/yara/libyara/include/tlshc/tlsh.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/error.h` & `yara-python-4.3.1/yara/libyara/include/yara/error.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/utils.h` & `yara-python-4.3.1/yara/libyara/include/yara/utils.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/unaligned.h` & `yara-python-4.3.1/yara/libyara/include/yara/unaligned.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/exefiles.h` & `yara-python-4.3.1/yara/libyara/include/yara/exefiles.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/proc.h` & `yara-python-4.3.1/yara/libyara/include/yara/proc.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/strutils.h` & `yara-python-4.3.1/yara/libyara/include/yara/strutils.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/compiler.h` & `yara-python-4.3.1/yara/libyara/include/yara/compiler.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/base64.h` & `yara-python-4.3.1/yara/libyara/include/yara/base64.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/elf_utils.h` & `yara-python-4.3.1/yara/libyara/include/yara/elf_utils.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/hex_lexer.h` & `yara-python-4.3.1/yara/libyara/include/yara/hex_lexer.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/types.h` & `yara-python-4.3.1/yara/libyara/include/yara/types.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/limits.h` & `yara-python-4.3.1/yara/libyara/include/yara/limits.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/ahocorasick.h` & `yara-python-4.3.1/yara/libyara/include/yara/ahocorasick.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/endian.h` & `yara-python-4.3.1/yara/libyara/include/yara/endian.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/parser.h` & `yara-python-4.3.1/yara/libyara/include/yara/parser.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/re.h` & `yara-python-4.3.1/yara/libyara/include/yara/re.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/threading.h` & `yara-python-4.3.1/yara/libyara/include/yara/threading.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/bitmask.h` & `yara-python-4.3.1/yara/libyara/include/yara/bitmask.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/libyara.h` & `yara-python-4.3.1/yara/libyara/include/yara/libyara.h`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 #ifndef YR_LIBYARA_H
 #define YR_LIBYARA_H
 
 #include <yara/utils.h>
 
 #define YR_MAJOR_VERSION 4
 #define YR_MINOR_VERSION 3
-#define YR_MICRO_VERSION 0
+#define YR_MICRO_VERSION 1
 
 #define version_str(s)  _version_str(s)
 #define _version_str(s) #s
 
 // Version as a string
 #define YR_VERSION                               \
   version_str(YR_MAJOR_VERSION) "." version_str( \
@@ -74,18 +74,18 @@
   YR_CONFIG_MAX_MATCH_DATA,
   YR_CONFIG_MAX_PROCESS_MEMORY_CHUNK,
 
   YR_CONFIG_LAST  // End-of-enum marker, not a configuration
 
 } YR_CONFIG_NAME;
 
-#define DEFAULT_STACK_SIZE                16384
-#define DEFAULT_MAX_STRINGS_PER_RULE      10000
-#define DEFAULT_MAX_MATCH_DATA            512
-#define DEFAULT_MAX_PROCESS_MEMORY_CHUNK  1073741824
+#define DEFAULT_STACK_SIZE               16384
+#define DEFAULT_MAX_STRINGS_PER_RULE     10000
+#define DEFAULT_MAX_MATCH_DATA           512
+#define DEFAULT_MAX_PROCESS_MEMORY_CHUNK 1073741824
 
 YR_API int yr_initialize(void);
 
 YR_API int yr_finalize(void);
 
 YR_API int yr_set_configuration(YR_CONFIG_NAME, void*);
 YR_API int yr_set_configuration_uint32(YR_CONFIG_NAME, uint32_t);
```

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/stream.h` & `yara-python-4.3.1/yara/libyara/include/yara/stream.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/dex.h` & `yara-python-4.3.1/yara/libyara/include/yara/dex.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/globals.h` & `yara-python-4.3.1/yara/libyara/include/yara/globals.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/sizedstr.h` & `yara-python-4.3.1/yara/libyara/include/yara/sizedstr.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/elf.h` & `yara-python-4.3.1/yara/libyara/include/yara/elf.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/modules.h` & `yara-python-4.3.1/yara/libyara/include/yara/modules.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/pe.h` & `yara-python-4.3.1/yara/libyara/include/yara/pe.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/scanner.h` & `yara-python-4.3.1/yara/libyara/include/yara/scanner.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/filemap.h` & `yara-python-4.3.1/yara/libyara/include/yara/filemap.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/stopwatch.h` & `yara-python-4.3.1/yara/libyara/include/yara/stopwatch.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/atoms.h` & `yara-python-4.3.1/yara/libyara/include/yara/atoms.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/stack.h` & `yara-python-4.3.1/yara/libyara/include/yara/stack.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/pe_utils.h` & `yara-python-4.3.1/yara/libyara/include/yara/pe_utils.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/exec.h` & `yara-python-4.3.1/yara/libyara/include/yara/exec.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/macho.h` & `yara-python-4.3.1/yara/libyara/include/yara/macho.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/dotnet.h` & `yara-python-4.3.1/yara/libyara/include/yara/dotnet.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/object.h` & `yara-python-4.3.1/yara/libyara/include/yara/object.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/lexer.h` & `yara-python-4.3.1/yara/libyara/include/yara/lexer.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/re_lexer.h` & `yara-python-4.3.1/yara/libyara/include/yara/re_lexer.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/integers.h` & `yara-python-4.3.1/yara/libyara/include/yara/integers.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/mem.h` & `yara-python-4.3.1/yara/libyara/include/yara/mem.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/rules.h` & `yara-python-4.3.1/yara/libyara/include/yara/rules.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/arena.h` & `yara-python-4.3.1/yara/libyara/include/yara/arena.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/hash.h` & `yara-python-4.3.1/yara/libyara/include/yara/hash.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/yara/scan.h` & `yara-python-4.3.1/yara/libyara/include/yara/scan.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/include/authenticode-parser/authenticode.h` & `yara-python-4.3.1/yara/libyara/include/authenticode-parser/authenticode.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/hex_grammar.h` & `yara-python-4.3.1/yara/libyara/hex_grammar.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/re_lexer.c` & `yara-python-4.3.1/yara/libyara/re_lexer.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/lexer.c` & `yara-python-4.3.1/yara/libyara/lexer.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/scan.c` & `yara-python-4.3.1/yara/libyara/scan.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/re_grammar.h` & `yara-python-4.3.1/yara/libyara/re_grammar.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/hash.c` & `yara-python-4.3.1/yara/libyara/hash.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/notebook.c` & `yara-python-4.3.1/yara/libyara/notebook.c`

 * *Files 12% similar despite different names*

```diff
@@ -44,23 +44,25 @@
 // a new page when necessary. It's recommended that the page size is at least
 // 4x the size of the buffers you plan to allocate with yr_notebook_alloc().
 //
 // Once the notebook is destroyed all the pages are freed, and consequently
 // all the buffers allocated via yr_notebook_alloc().
 struct YR_NOTEBOOK
 {
-  // Size of each page in the notebook.
-  size_t page_size;
+  // The mininum size of each page in the notebook.
+  size_t min_page_size;
   // Pointer to the first page in the book, this is also the most recently
   // created page, the one that is being filled.
   YR_NOTEBOOK_PAGE* page_list_head;
 };
 
 struct YR_NOTEBOOK_PAGE
 {
+  // Size of this page.
+  size_t size;
   // Amount of bytes in the page that are actually used.
   size_t used;
   // Pointer to next page.
   YR_NOTEBOOK_PAGE* next;
   // Page's data.
   uint8_t data[0];
 };
@@ -73,31 +75,32 @@
 //   page_size: Size of each page in the notebook.
 //   notebook: Address of a pointer to the newly created notebook.
 //
 // Returns:
 //   ERROR_SUCCESS
 //   ERROR_INSUFFICIENT_MEMORY
 //
-int yr_notebook_create(size_t page_size, YR_NOTEBOOK** notebook)
+int yr_notebook_create(size_t min_page_size, YR_NOTEBOOK** notebook)
 {
   YR_NOTEBOOK* new_notebook = yr_malloc(sizeof(YR_NOTEBOOK));
 
   if (new_notebook == NULL)
     return ERROR_INSUFFICIENT_MEMORY;
 
   new_notebook->page_list_head = yr_malloc(
-      sizeof(YR_NOTEBOOK_PAGE) + page_size);
+      sizeof(YR_NOTEBOOK_PAGE) + min_page_size);
 
   if (new_notebook->page_list_head == NULL)
   {
     yr_free(new_notebook);
     return ERROR_INSUFFICIENT_MEMORY;
   }
 
-  new_notebook->page_size = page_size;
+  new_notebook->min_page_size = min_page_size;
+  new_notebook->page_list_head->size = min_page_size;
   new_notebook->page_list_head->used = 0;
   new_notebook->page_list_head->next = NULL;
 
   *notebook = new_notebook;
 
   return ERROR_SUCCESS;
 }
@@ -143,27 +146,34 @@
 {
   // Round up the size to a multiple of 8, which also implies that the returned
   // pointers are aligned to 8 bytes. The 8-byte alignment is required by some
   // platforms (e.g. ARM and Sparc) that have strict alignment requirements when
   // deferrencing pointers to types larger than a byte.
   size = (size + 7) & ~0x7;
 
-  // The requested memory size can't be larger than a notebook's page.
-  assert(size <= notebook->page_size);
+  YR_NOTEBOOK_PAGE* current_page = notebook->page_list_head;
 
   // If the requested size doesn't fit in current page's free space, allocate
   // a new page.
-  if (notebook->page_size - notebook->page_list_head->used < size)
+  if (current_page->size - current_page->used < size)
   {
+    size_t min_size = notebook->min_page_size;
+
+    // The new page must be able to fit the requested buffer, so find the
+    // multiple of notebook->min_page_size that is larger or equal than than
+    // size.
+    size_t page_size = (size / min_size) * min_size + min_size;
+
     YR_NOTEBOOK_PAGE* new_page = yr_malloc(
-        sizeof(YR_NOTEBOOK_PAGE) + notebook->page_size);
+        sizeof(YR_NOTEBOOK_PAGE) + page_size);
 
     if (new_page == NULL)
       return NULL;
 
+    new_page->size = page_size;
     new_page->used = 0;
     new_page->next = notebook->page_list_head;
     notebook->page_list_head = new_page;
   }
 
   void* ptr = notebook->page_list_head->data + notebook->page_list_head->used;
```

### Comparing `yara-python-4.3.0/yara/libyara/arena.c` & `yara-python-4.3.1/yara/libyara/arena.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/crypto.h` & `yara-python-4.3.1/yara/libyara/crypto.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/hex_lexer.c` & `yara-python-4.3.1/yara/libyara/hex_lexer.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/grammar.h` & `yara-python-4.3.1/yara/libyara/grammar.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/base64.c` & `yara-python-4.3.1/yara/libyara/base64.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/exefiles.c` & `yara-python-4.3.1/yara/libyara/exefiles.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/compiler.c` & `yara-python-4.3.1/yara/libyara/compiler.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/proc.c` & `yara-python-4.3.1/yara/libyara/proc.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/strutils.c` & `yara-python-4.3.1/yara/libyara/strutils.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/hex_grammar.c` & `yara-python-4.3.1/yara/libyara/hex_grammar.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/re.c` & `yara-python-4.3.1/yara/libyara/re.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/bitmask.c` & `yara-python-4.3.1/yara/libyara/bitmask.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/threading.c` & `yara-python-4.3.1/yara/libyara/threading.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/endian.c` & `yara-python-4.3.1/yara/libyara/endian.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/ahocorasick.c` & `yara-python-4.3.1/yara/libyara/ahocorasick.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/demo/demo.c` & `yara-python-4.3.1/yara/libyara/modules/demo/demo.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/pe/pe.c` & `yara-python-4.3.1/yara/libyara/modules/pe/pe.c`

 * *Files 1% similar despite different names*

```diff
@@ -3015,30 +3015,30 @@
   if (IS_UNDEFINED(num_imports))
     return_integer(YR_UNDEFINED);
 
   for (int i = 0; i < num_imports; i++)
   {
     dll_name = yr_get_string(module, "import_details[%i].library_name", i);
     if (dll_name == NULL || IS_UNDEFINED(dll_name) ||
-        ss_compare(in_dll_name, dll_name) != 0)
+        ss_icompare(in_dll_name, dll_name) != 0)
       continue;
 
     int64_t num_functions = yr_get_integer(
         module, "import_details[%i].number_of_functions", i);
     if (IS_UNDEFINED(num_functions))
       return_integer(YR_UNDEFINED);
 
     for (int j = 0; j < num_functions; j++)
     {
       function_name = yr_get_string(
           module, "import_details[%i].functions[%i].name", i, j);
       if (function_name == NULL || IS_UNDEFINED(function_name))
         continue;
 
-      if (ss_compare(in_function_name, function_name) == 0)
+      if (ss_icompare(in_function_name, function_name) == 0)
         return_integer(yr_get_integer(
             module, "import_details[%i].functions[%i].rva", i, j));
     }
   }
 
   return_integer(YR_UNDEFINED);
 }
@@ -3060,15 +3060,15 @@
   if (IS_UNDEFINED(num_imports))
     return_integer(YR_UNDEFINED);
 
   for (int i = 0; i < num_imports; i++)
   {
     dll_name = yr_get_string(module, "import_details[%i].library_name", i);
     if (dll_name == NULL || IS_UNDEFINED(dll_name) ||
-        ss_compare(in_dll_name, dll_name) != 0)
+        ss_icompare(in_dll_name, dll_name) != 0)
       continue;
 
     int64_t num_functions = yr_get_integer(
         module, "import_details[%i].number_of_functions", i);
     if (IS_UNDEFINED(num_functions))
       return_integer(YR_UNDEFINED);
 
@@ -3108,15 +3108,15 @@
 
   for (int i = 0; i < num_imports; i++)
   {
     dll_name = yr_get_string(
         module, "delayed_import_details[%i].library_name", i);
 
     if (dll_name == NULL || IS_UNDEFINED(dll_name) ||
-        ss_compare(in_dll_name, dll_name) != 0)
+        ss_icompare(in_dll_name, dll_name) != 0)
       continue;
 
     int64_t num_functions = yr_get_integer(
         module, "delayed_import_details[%i].number_of_functions", i);
 
     if (IS_UNDEFINED(num_functions))
       return_integer(YR_UNDEFINED);
@@ -3125,15 +3125,15 @@
     {
       function_name = yr_get_string(
           module, "delayed_import_details[%i].functions[%i].name", i, j);
 
       if (function_name == NULL || IS_UNDEFINED(function_name))
         continue;
 
-      if (ss_compare(in_function_name, function_name) == 0)
+      if (ss_icompare(in_function_name, function_name) == 0)
         return_integer(yr_get_integer(
             module, "delayed_import_details[%i].functions[%i].rva", i, j));
     }
   }
 
   return_integer(YR_UNDEFINED);
 }
@@ -3157,15 +3157,15 @@
 
   for (int i = 0; i < num_imports; i++)
   {
     dll_name = yr_get_string(
         module, "delayed_import_details[%i].library_name", i);
 
     if (dll_name == NULL || IS_UNDEFINED(dll_name) ||
-        ss_compare(in_dll_name, dll_name) != 0)
+        ss_icompare(in_dll_name, dll_name) != 0)
       continue;
 
     int64_t num_functions = yr_get_integer(
         module, "delayed_import_details[%i].number_of_functions", i);
 
     if (IS_UNDEFINED(num_functions))
       return_integer(YR_UNDEFINED);
```

### Comparing `yara-python-4.3.0/yara/libyara/modules/pe/pe_utils.c` & `yara-python-4.3.1/yara/libyara/modules/pe/pe_utils.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/countersignature.h` & `yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/countersignature.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/helper.h` & `yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/helper.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/certificate.c` & `yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/certificate.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/structs.c` & `yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/structs.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/authenticode.c` & `yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/authenticode.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/certificate.h` & `yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/certificate.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/helper.c` & `yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/helper.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/countersignature.c` & `yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/countersignature.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/pe/authenticode-parser/structs.h` & `yara-python-4.3.1/yara/libyara/modules/pe/authenticode-parser/structs.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/magic/magic.c` & `yara-python-4.3.1/yara/libyara/modules/magic/magic.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/hash/hash.c` & `yara-python-4.3.1/yara/libyara/modules/hash/hash.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/macho/macho.c` & `yara-python-4.3.1/yara/libyara/modules/macho/macho.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/tests/tests.c` & `yara-python-4.3.1/yara/libyara/modules/tests/tests.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/math/math.c` & `yara-python-4.3.1/yara/libyara/modules/math/math.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/time/time.c` & `yara-python-4.3.1/yara/libyara/modules/time/time.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/dotnet/dotnet.c` & `yara-python-4.3.1/yara/libyara/modules/dotnet/dotnet.c`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
   }
 }
 
 // returns allocated string <namespace>.<name>, must be freed
 static char* create_full_name(const char* name, const char* namespace)
 {
   if (!name || !strlen(name))
-    return namespace ? strdup(namespace) : NULL;
+    return namespace ? yr_strdup(namespace) : NULL;
 
   // No namespace -> return name only
   if (!namespace || !strlen(namespace))
   {
     // fix generic names
     char* name_copy = yr_strdup(name);
     char* end = strchr(name_copy, '`');
```

### Comparing `yara-python-4.3.0/yara/libyara/modules/cuckoo/cuckoo.c` & `yara-python-4.3.1/yara/libyara/modules/cuckoo/cuckoo.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/dex/dex.c` & `yara-python-4.3.1/yara/libyara/modules/dex/dex.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/string/string.c` & `yara-python-4.3.1/yara/libyara/modules/string/string.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/elf/elf.c` & `yara-python-4.3.1/yara/libyara/modules/elf/elf.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/console/console.c` & `yara-python-4.3.1/yara/libyara/modules/console/console.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/pb_tests/pb_tests.pb-c.c` & `yara-python-4.3.1/yara/libyara/modules/pb_tests/pb_tests.pb-c.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/pb_tests/pb_tests.c` & `yara-python-4.3.1/yara/libyara/modules/pb_tests/pb_tests.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/modules/pb_tests/pb_tests.pb-c.h` & `yara-python-4.3.1/yara/libyara/modules/pb_tests/pb_tests.pb-c.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/exception.h` & `yara-python-4.3.1/yara/libyara/exception.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/parser.c` & `yara-python-4.3.1/yara/libyara/parser.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/simple_str.c` & `yara-python-4.3.1/yara/libyara/simple_str.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/sizedstr.c` & `yara-python-4.3.1/yara/libyara/sizedstr.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/re_grammar.c` & `yara-python-4.3.1/yara/libyara/re_grammar.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/libyara.c` & `yara-python-4.3.1/yara/libyara/libyara.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/libyara/stream.c` & `yara-python-4.3.1/yara/libyara/stream.c`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/sandbox/collect_matches.h` & `yara-python-4.3.1/yara/sandbox/collect_matches.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/yara/sandbox/yara_transaction.h` & `yara-python-4.3.1/yara/sandbox/yara_transaction.h`

 * *Files identical despite different names*

### Comparing `yara-python-4.3.0/setup.py` & `yara-python-4.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,15 +368,15 @@
 
 
 with open('README.rst', 'r', 'utf-8') as f:
   readme = f.read()
 
 setup(
     name='yara-python',
-    version='4.3.0',
+    version='4.3.1',
     description='Python interface for YARA',
     long_description=readme,
     license='Apache 2.0',
     author='Victor M. Alvarez',
     author_email='plusvic@gmail.com, vmalvarez@virustotal.com',
     url='https://github.com/VirusTotal/yara-python',
     classifiers=[
```

### Comparing `yara-python-4.3.0/README.rst` & `yara-python-4.3.1/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,23 @@
     >>> print(matches)
     [foo]
     >>> print(matches[0].rule)
     foo
     >>> print(matches[0].tags)
     ['bar']
     >>> print(matches[0].strings)
-    [(10L, '$a', 'lmn')]
+    [$a]
+    >>> print(matches[0].strings[0].identifier)
+    $a
+    >>> print(matches[0].strings[0].instances)
+    [lmn]
+    >>> print(matches[0].strings[0].instances[0].offset)
+    10
+    >>> print(matches[0].strings[0].instances[0].matched_length)
+    3
 
 
 Installation
 ------------
 
 The easiest way of installing YARA is by using ``pip``:
```

