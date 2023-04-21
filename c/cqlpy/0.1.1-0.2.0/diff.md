# Comparing `tmp/cqlpy-0.1.1.tar.gz` & `tmp/cqlpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqlpy-0.1.1.tar", max compression
+gzip compressed data, was "cqlpy-0.2.0.tar", max compression
```

## Comparing `cqlpy-0.1.1.tar` & `cqlpy-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,86 @@
--rw-r--r--   0        0        0        0 2023-03-28 17:14:05.870407 cqlpy-0.1.1/cqlpy/__init__.py
--rw-r--r--   0        0        0    23534 2023-03-28 17:23:21.435857 cqlpy-0.1.1/cqlpy/context.py
--rw-r--r--   0        0        0    18305 2023-03-27 19:55:51.670364 cqlpy-0.1.1/cqlpy/operators.py
--rw-r--r--   0        0        0    13428 2023-03-27 19:55:39.983410 cqlpy-0.1.1/cqlpy/types.py
--rw-r--r--   0        0        0      133 2023-03-27 19:53:25.205595 cqlpy-0.1.1/cqlpy/valueset_provider.py
--rw-r--r--   0        0        0     1091 2023-03-28 14:53:39.741101 cqlpy-0.1.1/LICENSE
--rw-r--r--   0        0        0      574 2023-03-28 19:41:25.504425 cqlpy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        9 2023-03-28 14:53:28.082592 cqlpy-0.1.1/README.md
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 cqlpy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-20 17:27:18.332869 cqlpy-0.2.0/LICENSE
+-rw-r--r--   0        0        0        8 2023-04-20 17:27:18.332869 cqlpy-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/__init__.py
+-rw-r--r--   0        0        0     4992 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/context/context.py
+-rw-r--r--   0        0        0      748 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/context/cql_value_set_provider.py
+-rw-r--r--   0        0        0    17113 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/context/fhir_r4_data_model.py
+-rw-r--r--   0        0        0      689 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/context/parameter_provider.py
+-rw-r--r--   0        0        0     2319 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/context/resource_query.py
+-rw-r--r--   0        0        0     1696 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/context/type_factory.py
+-rw-r--r--   0        0        0       92 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/exceptions.py
+-rw-r--r--   0        0        0      123 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/aggregate/count.py
+-rw-r--r--   0        0        0      339 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/arithmetic/max_value.py
+-rw-r--r--   0        0        0      320 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/arithmetic/min_value.py
+-rw-r--r--   0        0        0      691 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/clinical/any_in_valueset.py
+-rw-r--r--   0        0        0     1052 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/clinical/in_valueset.py
+-rw-r--r--   0        0        0      120 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/equal.py
+-rw-r--r--   0        0        0      511 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/equivalent.py
+-rw-r--r--   0        0        0      735 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/greater.py
+-rw-r--r--   0        0        0      763 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/greater_or_equal.py
+-rw-r--r--   0        0        0      507 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/in_list.py
+-rw-r--r--   0        0        0      726 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/less.py
+-rw-r--r--   0        0        0      753 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/less_or_equal.py
+-rw-r--r--   0        0        0      741 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/not_equal.py
+-rw-r--r--   0        0        0      671 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/cql_in.py
+-rw-r--r--   0        0        0     1165 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/add.py
+-rw-r--r--   0        0        0      541 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/after.py
+-rw-r--r--   0        0        0      558 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/before.py
+-rw-r--r--   0        0        0      588 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/calculate_age_at.py
+-rw-r--r--   0        0        0      157 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/date_time_precision.py
+-rw-r--r--   0        0        0      898 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/difference_between.py
+-rw-r--r--   0        0        0      890 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/duration_between.py
+-rw-r--r--   0        0        0      378 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/same_or_before.py
+-rw-r--r--   0        0        0     1181 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/subtract.py
+-rw-r--r--   0        0        0     3800 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/interval/collapse.py
+-rw-r--r--   0        0        0      381 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/interval/end.py
+-rw-r--r--   0        0        0     1411 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/interval/in_interval.py
+-rw-r--r--   0        0        0     1546 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/interval/included_in.py
+-rw-r--r--   0        0        0      587 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/interval/overlaps.py
+-rw-r--r--   0        0        0      976 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/interval/start.py
+-rw-r--r--   0        0        0      348 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/distinct.py
+-rw-r--r--   0        0        0      230 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/exists.py
+-rw-r--r--   0        0        0      324 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/first.py
+-rw-r--r--   0        0        0      291 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/flatten.py
+-rw-r--r--   0        0        0     2195 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/intersect.py
+-rw-r--r--   0        0        0      306 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/last.py
+-rw-r--r--   0        0        0      391 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/singleton_from.py
+-rw-r--r--   0        0        0      236 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/union.py
+-rw-r--r--   0        0        0      409 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/nullological/coalesce.py
+-rw-r--r--   0        0        0      212 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/nullological/is_false.py
+-rw-r--r--   0        0        0      358 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/nullological/is_null.py
+-rw-r--r--   0        0        0      193 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/nullological/is_true.py
+-rw-r--r--   0        0        0      254 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/sort/sort_by_column.py
+-rw-r--r--   0        0        0      134 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/sort/sort_by_direction.py
+-rw-r--r--   0        0        0      173 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/sort/sort_by_expression.py
+-rw-r--r--   0        0        0       51 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/sort/tuple_sort.py
+-rw-r--r--   0        0        0      166 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/string/ends_with.py
+-rw-r--r--   0        0        0      170 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/string/split.py
+-rw-r--r--   0        0        0      149 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/to_list.py
+-rw-r--r--   0        0        0      162 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/type/to_concept.py
+-rw-r--r--   0        0        0      280 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/type/to_datetime.py
+-rw-r--r--   0        0        0      461 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/parameter.py
+-rw-r--r--   0        0        0        0 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/types/__init__.py
+-rw-r--r--   0        0        0     2901 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/types/any.py
+-rw-r--r--   0        0        0      988 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/types/boolean.py
+-rw-r--r--   0        0        0     1700 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/types/code.py
+-rw-r--r--   0        0        0      851 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/types/code_system.py
+-rw-r--r--   0        0        0     2459 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/types/concept.py
+-rw-r--r--   0        0        0     1001 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/date.py
+-rw-r--r--   0        0        0     2986 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/datetime.py
+-rw-r--r--   0        0        0     1128 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/decimal.py
+-rw-r--r--   0        0        0      756 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/integer.py
+-rw-r--r--   0        0        0     3674 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/interval.py
+-rw-r--r--   0        0        0     1605 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/list.py
+-rw-r--r--   0        0        0       81 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/long.py
+-rw-r--r--   0        0        0      430 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/null.py
+-rw-r--r--   0        0        0      887 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/quantity.py
+-rw-r--r--   0        0        0      989 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/string.py
+-rw-r--r--   0        0        0     2003 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/value_set.py
+-rw-r--r--   0        0        0      170 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/valueset_provider.py
+-rw-r--r--   0        0        0      456 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/context.py
+-rw-r--r--   0        0        0     4289 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/operators.py
+-rw-r--r--   0        0        0        0 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/py.typed
+-rw-r--r--   0        0        0     1988 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/types.py
+-rw-r--r--   0        0        0      586 2023-04-20 17:27:41.509176 cqlpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 cqlpy-0.2.0/PKG-INFO
```

### Comparing `cqlpy-0.1.1/LICENSE` & `cqlpy-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 CareEvolution
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 CareEvolution
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `cqlpy-0.1.1/PKG-INFO` & `cqlpy-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqlpy
-Version: 0.1.1
+Version: 0.2.0
 Summary: Tooling to execute CQL-like Python against FHIR resources.
 License: MIT
 Author: John Wyderko
 Author-email: john@careevolution.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

