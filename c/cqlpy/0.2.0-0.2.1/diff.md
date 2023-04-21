# Comparing `tmp/cqlpy-0.2.0.tar.gz` & `tmp/cqlpy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqlpy-0.2.0.tar", max compression
+gzip compressed data, was "cqlpy-0.2.1.tar", max compression
```

## Comparing `cqlpy-0.2.0.tar` & `cqlpy-0.2.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0     1070 2023-04-20 17:27:18.332869 cqlpy-0.2.0/LICENSE
--rw-r--r--   0        0        0        8 2023-04-20 17:27:18.332869 cqlpy-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/__init__.py
--rw-r--r--   0        0        0     4992 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/context/context.py
--rw-r--r--   0        0        0      748 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/context/cql_value_set_provider.py
--rw-r--r--   0        0        0    17113 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/context/fhir_r4_data_model.py
--rw-r--r--   0        0        0      689 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/context/parameter_provider.py
--rw-r--r--   0        0        0     2319 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/context/resource_query.py
--rw-r--r--   0        0        0     1696 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/context/type_factory.py
--rw-r--r--   0        0        0       92 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/exceptions.py
--rw-r--r--   0        0        0      123 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/aggregate/count.py
--rw-r--r--   0        0        0      339 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/arithmetic/max_value.py
--rw-r--r--   0        0        0      320 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/arithmetic/min_value.py
--rw-r--r--   0        0        0      691 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/clinical/any_in_valueset.py
--rw-r--r--   0        0        0     1052 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/clinical/in_valueset.py
--rw-r--r--   0        0        0      120 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/equal.py
--rw-r--r--   0        0        0      511 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/equivalent.py
--rw-r--r--   0        0        0      735 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/greater.py
--rw-r--r--   0        0        0      763 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/greater_or_equal.py
--rw-r--r--   0        0        0      507 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/in_list.py
--rw-r--r--   0        0        0      726 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/less.py
--rw-r--r--   0        0        0      753 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/less_or_equal.py
--rw-r--r--   0        0        0      741 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/comparison/not_equal.py
--rw-r--r--   0        0        0      671 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/cql_in.py
--rw-r--r--   0        0        0     1165 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/add.py
--rw-r--r--   0        0        0      541 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/after.py
--rw-r--r--   0        0        0      558 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/before.py
--rw-r--r--   0        0        0      588 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/calculate_age_at.py
--rw-r--r--   0        0        0      157 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/date_time_precision.py
--rw-r--r--   0        0        0      898 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/difference_between.py
--rw-r--r--   0        0        0      890 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/duration_between.py
--rw-r--r--   0        0        0      378 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/same_or_before.py
--rw-r--r--   0        0        0     1181 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/date_time/subtract.py
--rw-r--r--   0        0        0     3800 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/interval/collapse.py
--rw-r--r--   0        0        0      381 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/interval/end.py
--rw-r--r--   0        0        0     1411 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/interval/in_interval.py
--rw-r--r--   0        0        0     1546 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/interval/included_in.py
--rw-r--r--   0        0        0      587 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/interval/overlaps.py
--rw-r--r--   0        0        0      976 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/interval/start.py
--rw-r--r--   0        0        0      348 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/distinct.py
--rw-r--r--   0        0        0      230 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/exists.py
--rw-r--r--   0        0        0      324 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/first.py
--rw-r--r--   0        0        0      291 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/flatten.py
--rw-r--r--   0        0        0     2195 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/intersect.py
--rw-r--r--   0        0        0      306 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/last.py
--rw-r--r--   0        0        0      391 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/singleton_from.py
--rw-r--r--   0        0        0      236 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/list/union.py
--rw-r--r--   0        0        0      409 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/nullological/coalesce.py
--rw-r--r--   0        0        0      212 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/nullological/is_false.py
--rw-r--r--   0        0        0      358 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/nullological/is_null.py
--rw-r--r--   0        0        0      193 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/nullological/is_true.py
--rw-r--r--   0        0        0      254 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/sort/sort_by_column.py
--rw-r--r--   0        0        0      134 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/sort/sort_by_direction.py
--rw-r--r--   0        0        0      173 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/sort/sort_by_expression.py
--rw-r--r--   0        0        0       51 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/sort/tuple_sort.py
--rw-r--r--   0        0        0      166 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/string/ends_with.py
--rw-r--r--   0        0        0      170 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/string/split.py
--rw-r--r--   0        0        0      149 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/to_list.py
--rw-r--r--   0        0        0      162 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/type/to_concept.py
--rw-r--r--   0        0        0      280 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/operators/type/to_datetime.py
--rw-r--r--   0        0        0      461 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/parameter.py
--rw-r--r--   0        0        0        0 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/types/__init__.py
--rw-r--r--   0        0        0     2901 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/types/any.py
--rw-r--r--   0        0        0      988 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/types/boolean.py
--rw-r--r--   0        0        0     1700 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/types/code.py
--rw-r--r--   0        0        0      851 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/types/code_system.py
--rw-r--r--   0        0        0     2459 2023-04-20 17:27:18.332869 cqlpy-0.2.0/cqlpy/_internal/types/concept.py
--rw-r--r--   0        0        0     1001 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/date.py
--rw-r--r--   0        0        0     2986 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/datetime.py
--rw-r--r--   0        0        0     1128 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/decimal.py
--rw-r--r--   0        0        0      756 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/integer.py
--rw-r--r--   0        0        0     3674 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/interval.py
--rw-r--r--   0        0        0     1605 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/list.py
--rw-r--r--   0        0        0       81 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/long.py
--rw-r--r--   0        0        0      430 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/null.py
--rw-r--r--   0        0        0      887 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/quantity.py
--rw-r--r--   0        0        0      989 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/string.py
--rw-r--r--   0        0        0     2003 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/types/value_set.py
--rw-r--r--   0        0        0      170 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/_internal/valueset_provider.py
--rw-r--r--   0        0        0      456 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/context.py
--rw-r--r--   0        0        0     4289 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/operators.py
--rw-r--r--   0        0        0        0 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/py.typed
--rw-r--r--   0        0        0     1988 2023-04-20 17:27:18.336869 cqlpy-0.2.0/cqlpy/types.py
--rw-r--r--   0        0        0      586 2023-04-20 17:27:41.509176 cqlpy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 cqlpy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-21 14:26:00.513291 cqlpy-0.2.1/LICENSE
+-rw-r--r--   0        0        0        8 2023-04-21 14:26:00.513291 cqlpy-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/__init__.py
+-rw-r--r--   0        0        0     5078 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/context/context.py
+-rw-r--r--   0        0        0      748 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/context/cql_value_set_provider.py
+-rw-r--r--   0        0        0    17348 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/context/fhir_r4_data_model.py
+-rw-r--r--   0        0        0      689 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/context/parameter_provider.py
+-rw-r--r--   0        0        0     2319 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/context/resource_query.py
+-rw-r--r--   0        0        0     1696 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/context/type_factory.py
+-rw-r--r--   0        0        0       92 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/exceptions.py
+-rw-r--r--   0        0        0      123 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/aggregate/count.py
+-rw-r--r--   0        0        0      339 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/arithmetic/max_value.py
+-rw-r--r--   0        0        0      320 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/arithmetic/min_value.py
+-rw-r--r--   0        0        0      691 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/clinical/any_in_valueset.py
+-rw-r--r--   0        0        0     1052 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/clinical/in_valueset.py
+-rw-r--r--   0        0        0      120 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/comparison/equal.py
+-rw-r--r--   0        0        0      511 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/comparison/equivalent.py
+-rw-r--r--   0        0        0      735 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/comparison/greater.py
+-rw-r--r--   0        0        0      763 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/comparison/greater_or_equal.py
+-rw-r--r--   0        0        0      507 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/comparison/in_list.py
+-rw-r--r--   0        0        0      726 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/comparison/less.py
+-rw-r--r--   0        0        0      753 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/comparison/less_or_equal.py
+-rw-r--r--   0        0        0      741 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/comparison/not_equal.py
+-rw-r--r--   0        0        0      671 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/cql_in.py
+-rw-r--r--   0        0        0     1165 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/date_time/add.py
+-rw-r--r--   0        0        0      541 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/date_time/after.py
+-rw-r--r--   0        0        0      558 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/date_time/before.py
+-rw-r--r--   0        0        0      588 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/date_time/calculate_age_at.py
+-rw-r--r--   0        0        0      157 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/date_time/date_time_precision.py
+-rw-r--r--   0        0        0      898 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/date_time/difference_between.py
+-rw-r--r--   0        0        0      890 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/date_time/duration_between.py
+-rw-r--r--   0        0        0      378 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/date_time/same_or_before.py
+-rw-r--r--   0        0        0     1181 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/date_time/subtract.py
+-rw-r--r--   0        0        0     3800 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/interval/collapse.py
+-rw-r--r--   0        0        0      381 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/interval/end.py
+-rw-r--r--   0        0        0     1411 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/interval/in_interval.py
+-rw-r--r--   0        0        0     1546 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/interval/included_in.py
+-rw-r--r--   0        0        0      587 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/interval/overlaps.py
+-rw-r--r--   0        0        0      976 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/interval/start.py
+-rw-r--r--   0        0        0      348 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/list/distinct.py
+-rw-r--r--   0        0        0      230 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/list/exists.py
+-rw-r--r--   0        0        0      324 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/list/first.py
+-rw-r--r--   0        0        0      291 2023-04-21 14:26:00.513291 cqlpy-0.2.1/cqlpy/_internal/operators/list/flatten.py
+-rw-r--r--   0        0        0     2195 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/list/intersect.py
+-rw-r--r--   0        0        0      306 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/list/last.py
+-rw-r--r--   0        0        0      404 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/list/singleton_from.py
+-rw-r--r--   0        0        0      236 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/list/union.py
+-rw-r--r--   0        0        0      409 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/nullological/coalesce.py
+-rw-r--r--   0        0        0      212 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/nullological/is_false.py
+-rw-r--r--   0        0        0      358 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/nullological/is_null.py
+-rw-r--r--   0        0        0      193 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/nullological/is_true.py
+-rw-r--r--   0        0        0      254 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/sort/sort_by_column.py
+-rw-r--r--   0        0        0      134 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/sort/sort_by_direction.py
+-rw-r--r--   0        0        0      173 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/sort/sort_by_expression.py
+-rw-r--r--   0        0        0       51 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/sort/tuple_sort.py
+-rw-r--r--   0        0        0      166 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/string/ends_with.py
+-rw-r--r--   0        0        0      170 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/string/split.py
+-rw-r--r--   0        0        0      149 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/to_list.py
+-rw-r--r--   0        0        0      162 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/type/to_concept.py
+-rw-r--r--   0        0        0      280 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/operators/type/to_datetime.py
+-rw-r--r--   0        0        0      509 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/parameter.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/__init__.py
+-rw-r--r--   0        0        0     2901 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/any.py
+-rw-r--r--   0        0        0      988 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/boolean.py
+-rw-r--r--   0        0        0     1700 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/code.py
+-rw-r--r--   0        0        0      851 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/code_system.py
+-rw-r--r--   0        0        0     2459 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/concept.py
+-rw-r--r--   0        0        0     1001 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/date.py
+-rw-r--r--   0        0        0     2986 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/datetime.py
+-rw-r--r--   0        0        0     1128 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/decimal.py
+-rw-r--r--   0        0        0      756 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/integer.py
+-rw-r--r--   0        0        0     3674 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/interval.py
+-rw-r--r--   0        0        0     1605 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/list.py
+-rw-r--r--   0        0        0       81 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/long.py
+-rw-r--r--   0        0        0      416 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/null.py
+-rw-r--r--   0        0        0      887 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/quantity.py
+-rw-r--r--   0        0        0      989 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/string.py
+-rw-r--r--   0        0        0     2003 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/types/value_set.py
+-rw-r--r--   0        0        0      170 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/_internal/valueset_provider.py
+-rw-r--r--   0        0        0      456 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/context.py
+-rw-r--r--   0        0        0     4289 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/operators.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/py.typed
+-rw-r--r--   0        0        0     1988 2023-04-21 14:26:00.517291 cqlpy-0.2.1/cqlpy/types.py
+-rw-r--r--   0        0        0      586 2023-04-21 14:26:21.201807 cqlpy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 cqlpy-0.2.1/PKG-INFO
```

### Comparing `cqlpy-0.2.0/LICENSE` & `cqlpy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/context/context.py` & `cqlpy-0.2.1/cqlpy/_internal/context/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,26 +45,29 @@
     Context Resource retrieve operations and Resource property retrieve operations are cached so that iterating through the bundle
     and parsing json is only performed once (at time of the first request).
     """
 
     def __init__(
         self,
         valueset_provider: ValueSetProvider,
-        bundle: Optional[str] = None,
+        bundle: Optional[Union[str, dict]] = None,
         bundle_file_name: Optional[str] = None,
         parameters: Optional[dict] = None,
     ):
         parsed_bundle = None
         if bundle_file_name:
             with open(bundle_file_name, encoding="utf-8") as f:
                 parsed_bundle = json.loads(f.read())
 
         if isinstance(bundle, str):
             parsed_bundle = json.loads(bundle)
 
+        if isinstance(bundle, dict):
+            parsed_bundle = bundle
+
         if parsed_bundle is None:
             raise ValueError("bundle or bundle_file_name must be specified")
 
         self.parameter_provider = ParameterProvider(parameters)
         self.model = FhirR4DataModel(parsed_bundle, self.parameter_provider)
         self.cql_valueset_provider = CqlValueSetProvider(
             valueset_provider=valueset_provider
```

### Comparing `cqlpy-0.2.0/cqlpy/_internal/context/cql_value_set_provider.py` & `cqlpy-0.2.1/cqlpy/_internal/context/cql_value_set_provider.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/context/fhir_r4_data_model.py` & `cqlpy-0.2.1/cqlpy/_internal/context/fhir_r4_data_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from cqlpy._internal.context.resource_query import ResourceQuery
 from cqlpy._internal.context.type_factory import TypeFactory
 from cqlpy._internal.operators.comparison.in_list import in_list
 from cqlpy._internal.operators.list.exists import exists
 from cqlpy._internal.operators.list.intersect import intersect
 from cqlpy._internal.operators.nullological.is_null import is_null
 from cqlpy._internal.parameter import Parameter
+from cqlpy._internal.types.any import CqlAny
 from cqlpy._internal.types.code import Code
 from cqlpy._internal.types.concept import Concept
 from cqlpy._internal.types.datetime import DateTime
 from cqlpy._internal.types.interval import Interval
 from cqlpy._internal.types.null import Null
 from cqlpy._internal.types.value_set import ValueSet
 from cqlpy._internal.valueset_provider import ValueSetProvider
@@ -161,15 +162,17 @@
         fhir_json: dict,
         resource_type: str,
         related_resource_provider: _RelatedFhirResourceProvider,
     ):
         self.__related_resource_provider = related_resource_provider
         super().__init__(fhir_json, resource_type)
 
-    def __getitem__(self, property_name: str) -> Union[list[FhirBase], FhirBase]:
+    def __getitem__(
+        self, property_name: str
+    ) -> Union[list[FhirBase], FhirBase, list[CqlAny], CqlAny]:
         if "Related:" in property_name:
             resource_name = property_name.split(":")[1]
 
             return [
                 resource
                 for resource in self.__related_resource_provider[resource_name]
                 if str(self["id"]) in str(resource[self._base_type.lower()])
@@ -335,26 +338,28 @@
 
                 if isinstance(resource_property, list):
                     for concept in resource_property:
                         if not isinstance(concept, Concept):
                             continue
 
                         intersection = intersect(concept.codes, filter_codes)
+                        assert isinstance(intersection, list)
                         if exists(intersection):
                             yield resource
 
                 elif isinstance(resource_property, Code) and in_list(
                     resource_property, filter_codes
                 ):
                     yield resource
 
-                elif isinstance(resource_property, Concept) and exists(
-                    intersect(resource_property.codes, filter_codes)
-                ):
-                    yield resource
+                elif isinstance(resource_property, Concept):
+                    intersection = intersect(resource_property.codes, filter_codes)
+                    assert isinstance(intersection, list)
+                    if exists(intersection):
+                        yield resource
 
     def __build_resource_proxies(
         self,
         resource_type: str,
         resources: list[Resource],
     ) -> Iterator[Resource]:
         for resource in resources:
```

### Comparing `cqlpy-0.2.0/cqlpy/_internal/context/parameter_provider.py` & `cqlpy-0.2.1/cqlpy/_internal/context/parameter_provider.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/context/resource_query.py` & `cqlpy-0.2.1/cqlpy/_internal/context/resource_query.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/context/type_factory.py` & `cqlpy-0.2.1/cqlpy/_internal/context/type_factory.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/clinical/any_in_valueset.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/clinical/any_in_valueset.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/clinical/in_valueset.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/clinical/in_valueset.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/comparison/greater.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/comparison/greater.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/comparison/greater_or_equal.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/comparison/greater_or_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/comparison/less.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/comparison/less.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/comparison/less_or_equal.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/comparison/less_or_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/comparison/not_equal.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/comparison/not_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/cql_in.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/cql_in.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/date_time/add.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/date_time/add.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/date_time/after.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/date_time/after.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/date_time/before.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/date_time/before.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/date_time/calculate_age_at.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/date_time/calculate_age_at.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/date_time/difference_between.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/date_time/difference_between.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/date_time/duration_between.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/date_time/duration_between.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/date_time/subtract.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/date_time/subtract.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/interval/collapse.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/interval/collapse.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/interval/in_interval.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/interval/in_interval.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/interval/included_in.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/interval/included_in.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/interval/overlaps.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/interval/overlaps.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/interval/start.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/interval/start.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/operators/list/intersect.py` & `cqlpy-0.2.1/cqlpy/_internal/operators/list/intersect.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/types/any.py` & `cqlpy-0.2.1/cqlpy/_internal/types/any.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/types/boolean.py` & `cqlpy-0.2.1/cqlpy/_internal/types/boolean.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/types/code.py` & `cqlpy-0.2.1/cqlpy/_internal/types/code.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/types/code_system.py` & `cqlpy-0.2.1/cqlpy/_internal/types/code_system.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/types/concept.py` & `cqlpy-0.2.1/cqlpy/_internal/types/concept.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/types/date.py` & `cqlpy-0.2.1/cqlpy/_internal/types/date.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/types/datetime.py` & `cqlpy-0.2.1/cqlpy/_internal/types/datetime.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/types/decimal.py` & `cqlpy-0.2.1/cqlpy/_internal/types/decimal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/types/integer.py` & `cqlpy-0.2.1/cqlpy/_internal/types/integer.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/types/interval.py` & `cqlpy-0.2.1/cqlpy/_internal/types/interval.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/types/list.py` & `cqlpy-0.2.1/cqlpy/_internal/types/list.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/types/quantity.py` & `cqlpy-0.2.1/cqlpy/_internal/types/quantity.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/types/string.py` & `cqlpy-0.2.1/cqlpy/_internal/types/string.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/_internal/types/value_set.py` & `cqlpy-0.2.1/cqlpy/_internal/types/value_set.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/operators.py` & `cqlpy-0.2.1/cqlpy/operators.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/cqlpy/types.py` & `cqlpy-0.2.1/cqlpy/types.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.0/pyproject.toml` & `cqlpy-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "John Wyderko <john@careevolution.com>",
   "Jeremy Fortune <jeremy@careevolution.com>",
 ]
 description = "Tooling to execute CQL-like Python against FHIR resources."
 license = "MIT"
 name = "cqlpy"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.1.1"
```

### Comparing `cqlpy-0.2.0/PKG-INFO` & `cqlpy-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqlpy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tooling to execute CQL-like Python against FHIR resources.
 License: MIT
 Author: John Wyderko
 Author-email: john@careevolution.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

