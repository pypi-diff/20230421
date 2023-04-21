# Comparing `tmp/yamllint-1.8.2.tar.gz` & `tmp/yamllint-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yamllint-1.8.2.tar", last modified: Tue Oct 10 10:31:26 2017, max compression
+gzip compressed data, was "dist/yamllint-1.9.0.tar", last modified: Mon Oct 16 20:54:26 2017, max compression
```

## Comparing `yamllint-1.8.2.tar` & `yamllint-1.9.0.tar`

### file list

```diff
@@ -1,218 +1,57 @@
-drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-10 10:31:26.000000 yamllint-1.8.2/
-drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-10 10:31:26.000000 yamllint-1.8.2/yamllint.egg-info/
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     7455 2017-10-10 10:31:26.000000 yamllint-1.8.2/yamllint.egg-info/SOURCES.txt
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       47 2017-10-10 10:31:26.000000 yamllint-1.8.2/yamllint.egg-info/entry_points.txt
--rw-rw-r--   0 adrien    (1000) adrien    (1000)        9 2017-10-10 10:31:26.000000 yamllint-1.8.2/yamllint.egg-info/top_level.txt
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       23 2017-10-10 10:31:26.000000 yamllint-1.8.2/yamllint.egg-info/requires.txt
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1017 2017-10-10 10:31:26.000000 yamllint-1.8.2/yamllint.egg-info/PKG-INFO
--rw-rw-r--   0 adrien    (1000) adrien    (1000)        1 2017-10-10 10:31:26.000000 yamllint-1.8.2/yamllint.egg-info/dependency_links.txt
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       50 2016-04-18 14:34:17.000000 yamllint-1.8.2/MANIFEST.in
-drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-10 10:31:26.000000 yamllint-1.8.2/tests/
--rw-rw-r--   0 adrien    (1000) adrien    (1000)    16560 2017-07-04 20:11:41.000000 yamllint-1.8.2/tests/test_config.py
-drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-10 10:31:26.000000 yamllint-1.8.2/tests/rules/
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     2523 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_document_end.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1693 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_new_lines.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)        0 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/__init__.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1645 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_common.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     6521 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_line_length.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     3538 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_document_start.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     5811 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_key_duplicates.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)    10063 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_commas.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     6476 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_comments.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1765 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_trailing_spaces.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)    10614 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_brackets.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     3379 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_empty_lines.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     9282 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_colons.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)    77096 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_indentation.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     5372 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_comments_indentation.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1555 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_new_line_at_end_of_file.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     3751 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_hyphens.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)    10671 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/rules/test_braces.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      749 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/__init__.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     2417 2017-07-04 20:11:41.000000 yamllint-1.8.2/tests/common.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)    12665 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/test_yamllint_directives.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     7568 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/test_spec_examples.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     2150 2017-07-04 20:11:41.000000 yamllint-1.8.2/tests/test_linter.py
-drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-10 10:31:26.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       80 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.2
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      123 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.22
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       13 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.19
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       77 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.20
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       26 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.7
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       94 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.4
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       96 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-5.12
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      145 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-10.8
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       59 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.4
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       19 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.7
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       27 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.16
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      644 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.27
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       82 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.5
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       32 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.6
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       27 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-5.14
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       28 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.3
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       53 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-9.6
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       89 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-5.13
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       55 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.11
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       50 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.6
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      108 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.1
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       74 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.21
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       36 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-9.2
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       40 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.14
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       21 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.20
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       49 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-5.11
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       27 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-9.1
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      203 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-10.9
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      298 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.24
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       28 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.2
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       74 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.17
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       48 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.21
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      139 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.16
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       59 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-5.4
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       86 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.13
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      301 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.1
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       63 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.5
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      133 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.3
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      101 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.21
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       41 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-5.10
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      106 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.20
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       54 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.22
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       32 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.13
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       41 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.3
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      142 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.11
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       16 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-5.1
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       63 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.19
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       51 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.16
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      130 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.7
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       59 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.8
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       86 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.5
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       58 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.27
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       70 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.4
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       43 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-5.2
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       50 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.24
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       24 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.15
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       94 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.17
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       53 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-10.6
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      218 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.10
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       65 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-10.4
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       49 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.21
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       92 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.15
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       82 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.18
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      152 2016-02-01 22:27:33.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.5
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       52 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.20
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       94 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.18
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       42 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.16
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      127 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.10
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      414 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.28
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       38 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.23
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       50 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.9
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       16 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-5.5
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      132 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.1
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      136 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.12
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       89 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.14
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       87 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.12
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      141 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-10.1
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       24 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.3
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       91 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-10.3
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       29 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.9
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       17 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.9
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       66 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.14
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       42 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.1
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       19 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-5.9
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       74 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.19
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      159 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.26
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       60 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.15
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       80 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.26
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       97 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.12
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       30 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-5.8
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      115 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.9
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       48 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.4
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       62 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.22
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      137 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.25
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       80 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.6
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       62 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.18
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       50 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.18
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       88 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.11
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       43 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.23
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      265 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.23
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       17 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.10
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       44 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.13
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      130 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-10.2
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       34 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.2
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      111 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-10.7
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       55 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.28
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       62 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-5.3
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       43 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.8
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      177 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.17
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       69 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.2
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       77 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.13
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       49 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-5.7
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       46 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.12
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       67 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.22
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       45 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.24
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       23 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-7.7
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       30 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.6
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       28 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.8
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       74 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-9.3
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       46 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-5.6
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       88 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.10
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       60 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-9.5
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      120 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.15
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       59 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.29
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       24 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.25
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       46 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-8.19
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      125 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.8
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       43 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.11
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       43 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-9.4
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       63 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-2.14
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       72 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-10.5
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       28 2016-02-01 19:12:38.000000 yamllint-1.8.2/tests/yaml-1.2-spec-examples/example-6.17
--rw-rw-r--   0 adrien    (1000) adrien    (1000)    13416 2017-07-04 20:11:41.000000 yamllint-1.8.2/tests/test_cli.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     6763 2017-07-04 20:11:41.000000 yamllint-1.8.2/tests/test_parser.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     3133 2017-07-04 19:36:19.000000 yamllint-1.8.2/tests/test_syntax_errors.py
-drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-10 10:31:26.000000 yamllint-1.8.2/yamllint/
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       67 2017-04-25 15:08:42.000000 yamllint-1.8.2/yamllint/__main__.py
-drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-10 10:31:26.000000 yamllint-1.8.2/yamllint/conf/
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1067 2017-09-19 17:29:44.000000 yamllint-1.8.2/yamllint/conf/default.yaml
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      505 2016-12-22 20:45:35.000000 yamllint-1.8.2/yamllint/conf/relaxed.yaml
-drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-10 10:31:26.000000 yamllint-1.8.2/yamllint/rules/
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     3425 2016-06-27 19:59:30.000000 yamllint-1.8.2/yamllint/rules/comments_indentation.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1570 2016-02-03 20:10:20.000000 yamllint-1.8.2/yamllint/rules/new_lines.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     4388 2017-04-25 15:08:42.000000 yamllint-1.8.2/yamllint/rules/braces.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1706 2017-09-19 17:29:44.000000 yamllint-1.8.2/yamllint/rules/__init__.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     3226 2016-06-27 19:59:30.000000 yamllint-1.8.2/yamllint/rules/common.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1634 2016-02-03 20:10:20.000000 yamllint-1.8.2/yamllint/rules/trailing_spaces.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     2409 2016-12-22 20:45:35.000000 yamllint-1.8.2/yamllint/rules/document_start.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1357 2016-02-03 20:10:20.000000 yamllint-1.8.2/yamllint/rules/new_line_at_end_of_file.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     2808 2016-06-27 19:59:30.000000 yamllint-1.8.2/yamllint/rules/empty_lines.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     2487 2016-12-22 20:45:35.000000 yamllint-1.8.2/yamllint/rules/truthy.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1956 2016-04-18 14:34:04.000000 yamllint-1.8.2/yamllint/rules/hyphens.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     2776 2016-04-18 14:34:04.000000 yamllint-1.8.2/yamllint/rules/key_duplicates.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     4493 2016-12-22 20:45:35.000000 yamllint-1.8.2/yamllint/rules/line_length.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     3634 2016-04-18 14:34:04.000000 yamllint-1.8.2/yamllint/rules/commas.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)    18788 2017-02-25 21:35:09.000000 yamllint-1.8.2/yamllint/rules/indentation.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     2757 2016-04-18 14:34:04.000000 yamllint-1.8.2/yamllint/rules/colons.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     4429 2017-04-25 15:08:42.000000 yamllint-1.8.2/yamllint/rules/brackets.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     2780 2016-12-22 20:45:35.000000 yamllint-1.8.2/yamllint/rules/comments.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     2658 2016-12-22 20:45:35.000000 yamllint-1.8.2/yamllint/rules/document_end.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1097 2017-10-10 10:28:54.000000 yamllint-1.8.2/yamllint/__init__.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     4993 2016-06-28 09:50:17.000000 yamllint-1.8.2/yamllint/parser.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     8617 2017-06-28 13:26:49.000000 yamllint-1.8.2/yamllint/linter.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     5935 2017-07-19 12:56:29.000000 yamllint-1.8.2/yamllint/config.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     6205 2017-06-28 13:26:49.000000 yamllint-1.8.2/yamllint/cli.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     2914 2017-06-28 13:26:49.000000 yamllint-1.8.2/README.rst
-drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-10 10:31:26.000000 yamllint-1.8.2/docs/
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      458 2017-07-19 12:56:31.000000 yamllint-1.8.2/docs/index.rst
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     2215 2017-04-25 15:08:42.000000 yamllint-1.8.2/docs/disable_with_comments.rst
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1222 2017-04-25 15:08:42.000000 yamllint-1.8.2/docs/text_editors.rst
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     6770 2016-01-22 17:38:27.000000 yamllint-1.8.2/docs/Makefile
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      472 2017-09-03 13:41:26.000000 yamllint-1.8.2/docs/integration.rst
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      180 2016-01-24 17:07:07.000000 yamllint-1.8.2/docs/development.rst
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1596 2017-09-19 17:29:44.000000 yamllint-1.8.2/docs/rules.rst
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     4338 2017-06-28 13:26:49.000000 yamllint-1.8.2/docs/configuration.rst
--rw-rw-r--   0 adrien    (1000) adrien    (1000)    41729 2016-02-01 21:38:52.000000 yamllint-1.8.2/docs/screenshot.png
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     2347 2016-12-22 20:45:35.000000 yamllint-1.8.2/docs/quickstart.rst
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1272 2017-09-03 14:08:36.000000 yamllint-1.8.2/docs/conf.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1017 2017-10-10 10:31:26.000000 yamllint-1.8.2/PKG-INFO
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1998 2017-07-19 16:53:02.000000 yamllint-1.8.2/setup.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)    35147 2016-01-13 21:08:00.000000 yamllint-1.8.2/LICENSE
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      103 2017-10-10 10:31:26.000000 yamllint-1.8.2/setup.cfg
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-16 20:54:26.000000 yamllint-1.9.0/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1017 2017-10-16 20:54:26.000000 yamllint-1.9.0/PKG-INFO
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1998 2017-10-16 20:54:00.000000 yamllint-1.9.0/setup.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      103 2017-10-16 20:54:26.000000 yamllint-1.9.0/setup.cfg
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2914 2017-10-16 20:54:00.000000 yamllint-1.9.0/README.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       50 2017-10-16 20:54:00.000000 yamllint-1.9.0/MANIFEST.in
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    35147 2017-10-16 20:54:00.000000 yamllint-1.9.0/LICENSE
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-16 20:54:26.000000 yamllint-1.9.0/yamllint.egg-info/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)        9 2017-10-16 20:54:26.000000 yamllint-1.9.0/yamllint.egg-info/top_level.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       23 2017-10-16 20:54:26.000000 yamllint-1.9.0/yamllint.egg-info/requires.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       47 2017-10-16 20:54:26.000000 yamllint-1.9.0/yamllint.egg-info/entry_points.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)        1 2017-10-16 20:54:26.000000 yamllint-1.9.0/yamllint.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1220 2017-10-16 20:54:26.000000 yamllint-1.9.0/yamllint.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1017 2017-10-16 20:54:26.000000 yamllint-1.9.0/yamllint.egg-info/PKG-INFO
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-16 20:54:26.000000 yamllint-1.9.0/yamllint/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     4993 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/parser.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     8617 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/linter.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     5935 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/config.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     6205 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/cli.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       67 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/__main__.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1097 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/__init__.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-16 20:54:26.000000 yamllint-1.9.0/yamllint/rules/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2487 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/truthy.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1634 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/trailing_spaces.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1570 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/new_lines.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1357 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/new_line_at_end_of_file.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     4493 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/line_length.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     3093 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/key_ordering.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2776 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/key_duplicates.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    18941 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/indentation.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1956 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/hyphens.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2808 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/empty_lines.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2409 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/document_start.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2658 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/document_end.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     3226 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/common.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     3425 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/comments_indentation.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2780 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/comments.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     3634 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/commas.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2757 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/colons.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     4429 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/brackets.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     4388 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/braces.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1759 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/rules/__init__.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-16 20:54:26.000000 yamllint-1.9.0/yamllint/conf/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      505 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/conf/relaxed.yaml
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1091 2017-10-16 20:54:00.000000 yamllint-1.9.0/yamllint/conf/default.yaml
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2017-10-16 20:54:26.000000 yamllint-1.9.0/docs/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1222 2017-10-16 20:54:00.000000 yamllint-1.9.0/docs/text_editors.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    41729 2017-10-16 20:54:00.000000 yamllint-1.9.0/docs/screenshot.png
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1670 2017-10-16 20:54:00.000000 yamllint-1.9.0/docs/rules.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2347 2017-10-16 20:54:00.000000 yamllint-1.9.0/docs/quickstart.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      472 2017-10-16 20:54:00.000000 yamllint-1.9.0/docs/integration.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      458 2017-10-16 20:54:00.000000 yamllint-1.9.0/docs/index.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2215 2017-10-16 20:54:00.000000 yamllint-1.9.0/docs/disable_with_comments.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      180 2017-10-16 20:54:00.000000 yamllint-1.9.0/docs/development.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     4338 2017-10-16 20:54:00.000000 yamllint-1.9.0/docs/configuration.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1272 2017-10-16 20:54:00.000000 yamllint-1.9.0/docs/conf.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     6770 2017-10-16 20:54:00.000000 yamllint-1.9.0/docs/Makefile
```

### Comparing `yamllint-1.8.2/yamllint.egg-info/PKG-INFO` & `yamllint-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: yamllint
-Version: 1.8.2
+Version: 1.9.0
 Summary: A linter for YAML files.
 Home-page: https://github.com/adrienverge/yamllint
 Author: Adrien Vergé
 Author-email: UNKNOWN
 License: GPLv3
 Description: A linter for YAML files.
```

### Comparing `yamllint-1.8.2/yamllint/conf/default.yaml` & `yamllint-1.9.0/yamllint/conf/default.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
   hyphens:
     max-spaces-after: 1
   indentation:
     spaces: consistent
     indent-sequences: true
     check-multi-line-strings: false
   key-duplicates: enable
+  key-ordering: disable
   line-length:
     max: 80
     allow-non-breakable-words: true
     allow-non-breakable-inline-mappings: false
   new-line-at-end-of-file: enable
   new-lines:
     type: unix
```

### Comparing `yamllint-1.8.2/yamllint/rules/comments_indentation.py` & `yamllint-1.9.0/yamllint/rules/comments_indentation.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/new_lines.py` & `yamllint-1.9.0/yamllint/rules/new_lines.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/braces.py` & `yamllint-1.9.0/yamllint/rules/braces.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/__init__.py` & `yamllint-1.9.0/yamllint/rules/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     comments_indentation,
     document_end,
     document_start,
     empty_lines,
     hyphens,
     indentation,
     key_duplicates,
+    key_ordering,
     line_length,
     new_line_at_end_of_file,
     new_lines,
     trailing_spaces,
     truthy,
 )
 
@@ -43,14 +44,15 @@
     comments_indentation.ID: comments_indentation,
     document_end.ID: document_end,
     document_start.ID: document_start,
     empty_lines.ID: empty_lines,
     hyphens.ID: hyphens,
     indentation.ID: indentation,
     key_duplicates.ID: key_duplicates,
+    key_ordering.ID: key_ordering,
     line_length.ID: line_length,
     new_line_at_end_of_file.ID: new_line_at_end_of_file,
     new_lines.ID: new_lines,
     trailing_spaces.ID: trailing_spaces,
     truthy.ID: truthy,
 }
```

### Comparing `yamllint-1.8.2/yamllint/rules/common.py` & `yamllint-1.9.0/yamllint/rules/common.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/trailing_spaces.py` & `yamllint-1.9.0/yamllint/rules/trailing_spaces.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/document_start.py` & `yamllint-1.9.0/yamllint/rules/document_start.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/new_line_at_end_of_file.py` & `yamllint-1.9.0/yamllint/rules/new_line_at_end_of_file.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/empty_lines.py` & `yamllint-1.9.0/yamllint/rules/empty_lines.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/truthy.py` & `yamllint-1.9.0/yamllint/rules/truthy.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/hyphens.py` & `yamllint-1.9.0/yamllint/rules/hyphens.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/key_duplicates.py` & `yamllint-1.9.0/yamllint/rules/key_duplicates.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/line_length.py` & `yamllint-1.9.0/yamllint/rules/line_length.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/commas.py` & `yamllint-1.9.0/yamllint/rules/commas.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/indentation.py` & `yamllint-1.9.0/yamllint/rules/indentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,14 +395,18 @@
             context['stack'].append(Parent(B_SEQ, token.start_mark.column))
             context['stack'][-1].implicit_block_seq = True
 
         if next.start_mark.line == token.end_mark.line:
             #   - item 1
             #   - item 2
             indent = next.start_mark.column
+        elif next.start_mark.column == token.start_mark.column:
+            #   -
+            #   key: value
+            indent = next.start_mark.column
         else:
             #   -
             #     item 1
             #   -
             #     key:
             #       value
             indent = detect_indent(token.start_mark.column, next)
```

### Comparing `yamllint-1.8.2/yamllint/rules/colons.py` & `yamllint-1.9.0/yamllint/rules/colons.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/brackets.py` & `yamllint-1.9.0/yamllint/rules/brackets.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/comments.py` & `yamllint-1.9.0/yamllint/rules/comments.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/rules/document_end.py` & `yamllint-1.9.0/yamllint/rules/document_end.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/__init__.py` & `yamllint-1.9.0/yamllint/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 
 yamllint does not only check for syntax validity, but for weirdnesses like key
 repetition and cosmetic problems such as lines length, trailing spaces,
 indentation, etc."""
 
 
 APP_NAME = 'yamllint'
-APP_VERSION = '1.8.2'
+APP_VERSION = '1.9.0'
 APP_DESCRIPTION = __doc__
 
 __author__ = u'Adrien Vergé'
 __copyright__ = u'Copyright 2016, Adrien Vergé'
 __license__ = 'GPLv3'
 __version__ = APP_VERSION
```

### Comparing `yamllint-1.8.2/yamllint/parser.py` & `yamllint-1.9.0/yamllint/parser.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/linter.py` & `yamllint-1.9.0/yamllint/linter.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/config.py` & `yamllint-1.9.0/yamllint/config.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/yamllint/cli.py` & `yamllint-1.9.0/yamllint/cli.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/README.rst` & `yamllint-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/docs/disable_with_comments.rst` & `yamllint-1.9.0/docs/disable_with_comments.rst`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/docs/text_editors.rst` & `yamllint-1.9.0/docs/text_editors.rst`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/docs/Makefile` & `yamllint-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/docs/rules.rst` & `yamllint-1.9.0/docs/rules.rst`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,19 @@
 .. automodule:: yamllint.rules.indentation
 
 key-duplicates
 --------------
 
 .. automodule:: yamllint.rules.key_duplicates
 
+key-ordering
+--------------
+
+.. automodule:: yamllint.rules.key_ordering
+
 line-length
 -----------
 
 .. automodule:: yamllint.rules.line_length
 
 new-line-at-end-of-file
 -----------------------
```

### Comparing `yamllint-1.8.2/docs/configuration.rst` & `yamllint-1.9.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/docs/screenshot.png` & `yamllint-1.9.0/docs/screenshot.png`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/docs/quickstart.rst` & `yamllint-1.9.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/docs/conf.py` & `yamllint-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/PKG-INFO` & `yamllint-1.9.0/yamllint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: yamllint
-Version: 1.8.2
+Version: 1.9.0
 Summary: A linter for YAML files.
 Home-page: https://github.com/adrienverge/yamllint
 Author: Adrien Vergé
 Author-email: UNKNOWN
 License: GPLv3
 Description: A linter for YAML files.
```

### Comparing `yamllint-1.8.2/setup.py` & `yamllint-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `yamllint-1.8.2/LICENSE` & `yamllint-1.9.0/LICENSE`

 * *Files identical despite different names*

