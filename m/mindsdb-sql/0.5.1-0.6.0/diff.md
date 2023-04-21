# Comparing `tmp/mindsdb_sql-0.5.1.tar.gz` & `tmp/mindsdb_sql-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mindsdb_sql-0.5.1.tar", last modified: Fri Apr  7 09:50:46 2023, max compression
+gzip compressed data, was "dist\mindsdb_sql-0.6.0.tar", last modified: Fri Apr 21 07:42:31 2023, max compression
```

## Comparing `mindsdb_sql-0.5.1.tar` & `mindsdb_sql-0.6.0.tar`

### file list

```diff
@@ -1,93 +1,141 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/
--rw-rw-rw-   0        0        0      535 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     7245 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql/
--rw-rw-rw-   0        0        0      365 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/__about__.py
--rw-rw-rw-   0        0        0     1195 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/__init__.py
--rw-rw-rw-   0        0        0      170 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/
--rw-rw-rw-   0        0        0        0 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/
--rw-rw-rw-   0        0        0      537 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/__init__.py
--rw-rw-rw-   0        0        0      842 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/alter_table.py
--rw-rw-rw-   0        0        0     1343 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/base.py
--rw-rw-rw-   0        0        0      460 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/commit_transaction.py
--rw-rw-rw-   0        0        0     2287 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/create.py
--rw-rw-rw-   0        0        0      994 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/delete.py
--rw-rw-rw-   0        0        0      942 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/describe.py
--rw-rw-rw-   0        0        0     3056 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/drop.py
--rw-rw-rw-   0        0        0      659 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/explain.py
--rw-rw-rw-   0        0        0     3099 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/insert.py
--rw-rw-rw-   0        0        0      466 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/rollback_transaction.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/
--rw-rw-rw-   0        0        0      567 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/__init__.py
--rw-rw-rw-   0        0        0     1482 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/case.py
--rw-rw-rw-   0        0        0     1113 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/common_table_expression.py
--rw-rw-rw-   0        0        0     1593 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/constant.py
--rw-rw-rw-   0        0        0     2372 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/identifier.py
--rw-rw-rw-   0        0        0     1381 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/join.py
--rw-rw-rw-   0        0        0      662 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/native_query.py
--rw-rw-rw-   0        0        0     5949 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/operation.py
--rw-rw-rw-   0        0        0      806 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/order_by.py
--rw-rw-rw-   0        0        0      464 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/parameter.py
--rw-rw-rw-   0        0        0     5904 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/select.py
--rw-rw-rw-   0        0        0      504 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/star.py
--rw-rw-rw-   0        0        0      648 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/tuple.py
--rw-rw-rw-   0        0        0      774 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/type_cast.py
--rw-rw-rw-   0        0        0     1178 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/union.py
--rw-rw-rw-   0        0        0     3296 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/set.py
--rw-rw-rw-   0        0        0     2979 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/show.py
--rw-rw-rw-   0        0        0      469 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/start_transaction.py
--rw-rw-rw-   0        0        0     2407 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/update.py
--rw-rw-rw-   0        0        0      639 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/use.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/
--rw-rw-rw-   0        0        0        0 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/
--rw-rw-rw-   0        0        0      672 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/__init__.py
--rw-rw-rw-   0        0        0     1582 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/create_database.py
--rw-rw-rw-   0        0        0      953 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/create_file.py
--rw-rw-rw-   0        0        0     2078 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/create_job.py
--rw-rw-rw-   0        0        0     1201 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
--rw-rw-rw-   0        0        0     5361 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
--rw-rw-rw-   0        0        0     1534 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/create_view.py
--rw-rw-rw-   0        0        0      704 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
--rw-rw-rw-   0        0        0      713 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
--rw-rw-rw-   0        0        0      737 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py
--rw-rw-rw-   0        0        0      692 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
--rw-rw-rw-   0        0        0      708 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
--rw-rw-rw-   0        0        0      906 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
--rw-rw-rw-   0        0        0      223 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
--rw-rw-rw-   0        0        0      359 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/latest.py
--rw-rw-rw-   0        0        0     8125 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/lexer.py
--rw-rw-rw-   0        0        0    43489 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/parser.py
--rw-rw-rw-   0        0        0      311 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mysql/
--rw-rw-rw-   0        0        0       67 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mysql/__init__.py
--rw-rw-rw-   0        0        0     1046 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mysql/lexer.py
--rw-rw-rw-   0        0        0    29432 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mysql/parser.py
--rw-rw-rw-   0        0        0      904 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mysql/show_index.py
--rw-rw-rw-   0        0        0      686 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mysql/variable.py
--rw-rw-rw-   0        0        0     6292 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/lexer.py
--rw-rw-rw-   0        0        0      751 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/logger.py
--rw-rw-rw-   0        0        0    21323 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/parser.py
--rw-rw-rw-   0        0        0     2497 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql/planner/
--rw-rw-rw-   0        0        0      150 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/planner/__init__.py
--rw-rw-rw-   0        0        0      878 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/planner/query_plan.py
--rw-rw-rw-   0        0        0    49858 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/planner/query_planner.py
--rw-rw-rw-   0        0        0    21367 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/planner/query_prepare.py
--rw-rw-rw-   0        0        0      536 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/planner/step_result.py
--rw-rw-rw-   0        0        0     8280 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/planner/steps.py
--rw-rw-rw-   0        0        0     2981 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/planner/ts_utils.py
--rw-rw-rw-   0        0        0    17886 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/planner/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql/render/
--rw-rw-rw-   0        0        0        0 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/render/__init__.py
--rw-rw-rw-   0        0        0    20561 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/mindsdb_sql/render/sqlalchemy_render.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql.egg-info/
--rw-rw-rw-   0        0        0      535 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3150 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/mindsdb_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 09:50:46.000000 mindsdb_sql-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      843 2023-04-07 09:50:24.000000 mindsdb_sql-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/
+-rw-rw-rw-   0        0        0      535 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7245 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql/
+-rw-rw-rw-   0        0        0      365 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/__about__.py
+-rw-rw-rw-   0        0        0     1195 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/__init__.py
+-rw-rw-rw-   0        0        0      170 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/
+-rw-rw-rw-   0        0        0      537 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/alter_table.py
+-rw-rw-rw-   0        0        0     1343 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/base.py
+-rw-rw-rw-   0        0        0      460 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/commit_transaction.py
+-rw-rw-rw-   0        0        0     2287 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/create.py
+-rw-rw-rw-   0        0        0      994 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/delete.py
+-rw-rw-rw-   0        0        0      942 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/describe.py
+-rw-rw-rw-   0        0        0     3056 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/drop.py
+-rw-rw-rw-   0        0        0      659 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/explain.py
+-rw-rw-rw-   0        0        0     3099 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/insert.py
+-rw-rw-rw-   0        0        0      466 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/rollback_transaction.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/
+-rw-rw-rw-   0        0        0      567 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/__init__.py
+-rw-rw-rw-   0        0        0     1482 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/case.py
+-rw-rw-rw-   0        0        0     1113 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/common_table_expression.py
+-rw-rw-rw-   0        0        0     1593 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/constant.py
+-rw-rw-rw-   0        0        0     2372 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/identifier.py
+-rw-rw-rw-   0        0        0     1381 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/join.py
+-rw-rw-rw-   0        0        0      662 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/native_query.py
+-rw-rw-rw-   0        0        0     5949 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/operation.py
+-rw-rw-rw-   0        0        0      806 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/order_by.py
+-rw-rw-rw-   0        0        0      464 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/parameter.py
+-rw-rw-rw-   0        0        0     5904 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/select.py
+-rw-rw-rw-   0        0        0      504 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/star.py
+-rw-rw-rw-   0        0        0      648 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/tuple.py
+-rw-rw-rw-   0        0        0      774 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/type_cast.py
+-rw-rw-rw-   0        0        0     1178 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/union.py
+-rw-rw-rw-   0        0        0     3296 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/set.py
+-rw-rw-rw-   0        0        0     2979 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/show.py
+-rw-rw-rw-   0        0        0      469 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/start_transaction.py
+-rw-rw-rw-   0        0        0     2407 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/update.py
+-rw-rw-rw-   0        0        0      639 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/use.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/
+-rw-rw-rw-   0        0        0      720 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/__init__.py
+-rw-rw-rw-   0        0        0     1595 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/create_database.py
+-rw-rw-rw-   0        0        0      953 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/create_file.py
+-rw-rw-rw-   0        0        0     2078 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/create_job.py
+-rw-rw-rw-   0        0        0     1201 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
+-rw-rw-rw-   0        0        0     5361 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
+-rw-rw-rw-   0        0        0     1534 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/create_view.py
+-rw-rw-rw-   0        0        0      704 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
+-rw-rw-rw-   0        0        0      713 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
+-rw-rw-rw-   0        0        0      737 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py
+-rw-rw-rw-   0        0        0      692 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
+-rw-rw-rw-   0        0        0      708 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
+-rw-rw-rw-   0        0        0      906 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
+-rw-rw-rw-   0        0        0     1313 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
+-rw-rw-rw-   0        0        0      223 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
+-rw-rw-rw-   0        0        0      359 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/latest.py
+-rw-rw-rw-   0        0        0     8101 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/lexer.py
+-rw-rw-rw-   0        0        0    44279 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/parser.py
+-rw-rw-rw-   0        0        0      311 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mysql/
+-rw-rw-rw-   0        0        0       67 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mysql/__init__.py
+-rw-rw-rw-   0        0        0     1046 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mysql/lexer.py
+-rw-rw-rw-   0        0        0    29470 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mysql/parser.py
+-rw-rw-rw-   0        0        0      904 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mysql/show_index.py
+-rw-rw-rw-   0        0        0      686 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mysql/variable.py
+-rw-rw-rw-   0        0        0     6226 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/lexer.py
+-rw-rw-rw-   0        0        0      751 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/logger.py
+-rw-rw-rw-   0        0        0    21361 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/parser.py
+-rw-rw-rw-   0        0        0     2497 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql/planner/
+-rw-rw-rw-   0        0        0      150 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/planner/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/planner/query_plan.py
+-rw-rw-rw-   0        0        0    50020 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/planner/query_planner.py
+-rw-rw-rw-   0        0        0    21367 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/planner/query_prepare.py
+-rw-rw-rw-   0        0        0      536 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/planner/step_result.py
+-rw-rw-rw-   0        0        0     8276 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/planner/steps.py
+-rw-rw-rw-   0        0        0     2981 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/planner/ts_utils.py
+-rw-rw-rw-   0        0        0    17886 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/planner/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql/render/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/render/__init__.py
+-rw-rw-rw-   0        0        0    20561 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/mindsdb_sql/render/sqlalchemy_render.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5187 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/mindsdb_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      843 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/tests/test_parser/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/__init__.py
+-rw-rw-rw-   0        0        0      776 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_ast.py
+-rw-rw-rw-   0        0        0    11910 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_base_lexer.py
+-rw-rw-rw-   0        0        0      223 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_base_sql.py
+-rw-rw-rw-   0        0        0     1480 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_create.py
+-rw-rw-rw-   0        0        0     2481 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_ddl.py
+-rw-rw-rw-   0        0        0     1075 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_delete.py
+-rw-rw-rw-   0        0        0     1094 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_describe.py
+-rw-rw-rw-   0        0        0     2426 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_insert.py
+-rw-rw-rw-   0        0        0     6945 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_misc_sql_queries.py
+-rw-rw-rw-   0        0        0     3625 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_select_common_table_expression.py
+-rw-rw-rw-   0        0        0    24379 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_select_operations.py
+-rw-rw-rw-   0        0        0    45563 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_select_structure.py
+-rw-rw-rw-   0        0        0    13620 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_show.py
+-rw-rw-rw-   0        0        0     3114 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_union.py
+-rw-rw-rw-   0        0        0     2462 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_update.py
+-rw-rw-rw-   0        0        0      514 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_base_sql/test_use.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/__init__.py
+-rw-rw-rw-   0        0        0      605 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_create_file.py
+-rw-rw-rw-   0        0        0     4203 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_create_integration.py
+-rw-rw-rw-   0        0        0     6617 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_create_predictor.py
+-rw-rw-rw-   0        0        0     2651 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_create_view.py
+-rw-rw-rw-   0        0        0      520 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_drop_dataset.py
+-rw-rw-rw-   0        0        0      861 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_drop_datasource.py
+-rw-rw-rw-   0        0        0      866 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_drop_integration.py
+-rw-rw-rw-   0        0        0     1708 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_drop_predictor.py
+-rw-rw-rw-   0        0        0     1824 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_evaluate.py
+-rw-rw-rw-   0        0        0     1339 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_finetune_predictor.py
+-rw-rw-rw-   0        0        0     2073 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_jobs.py
+-rw-rw-rw-   0        0        0     1587 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_ml_engine.py
+-rw-rw-rw-   0        0        0     2242 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_retrain_predictor.py
+-rw-rw-rw-   0        0        0     3572 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_selects.py
+-rw-rw-rw-   0        0        0     1226 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_show_mindsdb.py
+-rw-rw-rw-   0        0        0      959 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mindsdb/test_timeseries.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mysql/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mysql/__init__.py
+-rw-rw-rw-   0        0        0      714 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mysql/test_mysql_lexer.py
+-rw-rw-rw-   0        0        0     3050 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_parser/test_mysql/test_mysql_parser.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:42:31.000000 mindsdb_sql-0.6.0/tests/test_render/
+-rw-rw-rw-   0        0        0        0 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_render/__init__.py
+-rw-rw-rw-   0        0        0     6391 2023-04-21 07:40:55.000000 mindsdb_sql-0.6.0/tests/test_render/test_sqlalchemyrender.py
```

### Comparing `mindsdb_sql-0.5.1/PKG-INFO` & `mindsdb_sql-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mindsdb_sql
-Version: 0.5.1
+Version: 0.6.0
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.5.1/README.md` & `mindsdb_sql-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/__init__.py` & `mindsdb_sql-0.6.0/mindsdb_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/__init__.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/alter_table.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/alter_table.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/base.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/base.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/create.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/create.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/delete.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/delete.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/describe.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/describe.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/drop.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/drop.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/explain.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/explain.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/insert.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/insert.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/__init__.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/case.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/case.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/common_table_expression.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/common_table_expression.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/constant.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/constant.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/identifier.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/identifier.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/join.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/join.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/native_query.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/native_query.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/operation.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/operation.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/order_by.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/order_by.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/select.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/select.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/tuple.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/tuple.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/type_cast.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/type_cast.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/select/union.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/select/union.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/set.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/set.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/show.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/show.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/update.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/update.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/ast/use.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/ast/use.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/__init__.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from .create_predictor import CreatePredictor
 from .drop_predictor import DropPredictor
 from .retrain_predictor import RetrainPredictor
 from .finetune_predictor import FinetunePredictor
 from .drop_integration import DropIntegration
 from .drop_datasource import DropDatasource
 from .drop_dataset import DropDataset
+from .evaluate import Evaluate
 from .latest import Latest
 from .create_file import CreateFile
 from .create_ml_engine import CreateMLEngine
 from .drop_ml_engine import DropMLEngine
 from .create_job import CreateJob
 from .drop_job import DropJob
 
-# Temporary
+# remove it in next release
 CreateDatasource = CreateDatabase
```

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/create_database.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/create_database.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.engine = engine
         self.parameters = parameters
         self.is_replace = is_replace
 
     def to_tree(self, *args, level=0, **kwargs):
         ind = indent(level)
         ind1 = indent(level+1)
-        name_str = f'\n{ind1}name={repr(self.name)},'
+        name_str = f'\n{ind1}name={self.name.to_string()},'
         engine_str = f'\n{ind1}engine={repr(self.engine)},'
         parameters_str = f'\n{ind1}parameters={str(self.parameters)},'
 
         replace_str = ''
         if self.is_replace:
             replace_str = f'\n{ind1}is_replace=True'
 
@@ -39,9 +39,9 @@
         replace_str = ''
         if self.is_replace:
             replace_str = f' OR REPLACE'
 
         parameters_str = ''
         if self.parameters:
             parameters_str = f', PARAMETERS = {json.dumps(self.parameters)}'
-        out_str = f'CREATE{replace_str} DATABASE {str(self.name)} WITH ENGINE = {repr(self.engine)}{parameters_str}'
+        out_str = f'CREATE{replace_str} DATABASE {self.name.to_string()} WITH ENGINE = {repr(self.engine)}{parameters_str}'
         return out_str
```

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/create_file.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/create_file.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/create_job.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/create_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/create_view.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/create_view.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/drop_job.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/drop_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/lexer.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         SERIALIZABLE, ONLY, CONVERT, BEGIN,
 
         # Mindsdb special
 
         PREDICTOR, PREDICTORS, DATASOURCE, INTEGRATION, INTEGRATIONS,DATASOURCES,
         STREAM, STREAMS, PUBLICATION, PUBLICATIONS, VIEW, VIEWS, DATASETS, DATASET,
         MODEL, MODELS, ML_ENGINE, ML_ENGINES, HANDLERS,
-        FINETUNE,
+        FINETUNE, EVALUATE,
         LATEST, HORIZON, USING,
         ENGINE, TRAIN, PREDICT, PARAMETERS, JOB, EVERY,PROJECT,
 
         # SHOW/DDL Keywords
 
         SHOW, SCHEMAS, SCHEMA, DATABASES, DATABASE, TABLES, TABLE, FULL, EXTENDED, PROCESSLIST,
         MUTEX, CODE, SLAVE, REPLICA, REPLICAS, CHANNEL, TRIGGERS, KEYS, STORAGE, LOGS, BINARY,
@@ -103,14 +103,15 @@
     MODELS = r'\bMODELS\b'
     ML_ENGINE = r'\bML_ENGINE\b'
     ML_ENGINES = r'\bML_ENGINES\b'
     HANDLERS = r'\bHANDLERS\b'
     JOB = r'\bJOB\b'
     EVERY = r'\bEVERY\b'
     PROJECT = r'\bPROJECT\b'
+    EVALUATE = r'\bEVALUATE\b'
 
     # Misc
     SET = r'\bSET\b'
     START = r'\bSTART\b'
     TRANSACTION = r'\bTRANSACTION\b'
     COMMIT = r'\bCOMMIT\b'
     ROLLBACK = r'\bROLLBACK\b'
@@ -268,15 +269,15 @@
 
 
     # Data types
     NULL = r'\bNULL\b'
     TRUE = r'\bTRUE\b'
     FALSE = r'\bFALSE\b'
 
-    @_(r'(?:([a-zA-Z_$0-9]*[a-zA-Z_$]+[a-zA-Z_$0-9]*)|(?:`([^`]+)`))(?:\.(?:([a-zA-Z_$0-9]*[a-zA-Z_$]+[a-zA-Z_$0-9]*)|(?:`([^`]+)`)))*')
+    @_(r'(?:([a-zA-Z_$0-9]*[a-zA-Z_$]+[a-zA-Z_$0-9]*)|(?:`([^`]+)`))')
     def ID(self, t):
         return t
 
     @_(r'\d+\.\d*')
     def FLOAT(self, t):
         return t
```

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mindsdb/parser.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mindsdb/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from mindsdb_sql.parser.dialects.mindsdb.create_predictor import CreatePredictor
 from mindsdb_sql.parser.dialects.mindsdb.create_database import CreateDatabase
 from mindsdb_sql.parser.dialects.mindsdb.create_ml_engine import CreateMLEngine
 from mindsdb_sql.parser.dialects.mindsdb.create_view import CreateView
 from mindsdb_sql.parser.dialects.mindsdb.create_job import CreateJob
 from mindsdb_sql.parser.dialects.mindsdb.drop_job import DropJob
 from mindsdb_sql.parser.dialects.mindsdb.latest import Latest
+from mindsdb_sql.parser.dialects.mindsdb.evaluate import Evaluate
 from mindsdb_sql.parser.dialects.mindsdb.create_file import CreateFile
 from mindsdb_sql.exceptions import ParsingException
 from mindsdb_sql.parser.dialects.mindsdb.lexer import MindsDBLexer
 from mindsdb_sql.parser.dialects.mindsdb.retrain_predictor import RetrainPredictor
 from mindsdb_sql.parser.dialects.mindsdb.finetune_predictor import FinetunePredictor
 from mindsdb_sql.parser.logger import ParserLogger
 from mindsdb_sql.parser.utils import ensure_select_keyword_order, JoinType, tokens_to_string
@@ -60,14 +61,15 @@
        'drop_dataset',
        'union',
        'select',
        'select_using',
        'insert',
        'update',
        'delete',
+       'evaluate',
        'drop_database',
        'drop_view',
        'drop_table',
        'create_table',
        'create_job',
        'drop_job',
        )
@@ -669,14 +671,34 @@
 
         return FinetunePredictor(
             name=name,
             integration_name=getattr(p, 'identifier1', None),
             query_str=query_str,
         )
 
+    @_('EVALUATE identifier FROM LPAREN raw_query RPAREN',
+       'EVALUATE identifier FROM LPAREN raw_query RPAREN USING kw_parameter_list',)
+    def evaluate(self, p):
+        if hasattr(p, 'identifier'):
+            # single identifier field
+            name = p.identifier
+        else:
+            name = p.identifier0
+
+        if hasattr(p, 'USING'):
+            using = p.kw_parameter_list
+        else:
+            using = None
+
+        return Evaluate(
+            name=name,
+            query_str=tokens_to_string(p.raw_query),
+            using=using
+        )
+
     # ------------
 
     # ML ENGINE
     # CREATE
     @_('CREATE ML_ENGINE identifier FROM id USING kw_parameter_list',
        'CREATE ML_ENGINE identifier FROM id')
     def create_integration(self, p):
@@ -704,30 +726,30 @@
         if hasattr(p, 'REPLACE'):
             is_replace = True
 
         parameters = None
         if hasattr(p, 'json'):
             parameters = p.json
 
-        return CreateDatabase(name=p.database_engine['id'],
+        return CreateDatabase(name=p.database_engine['identifier'],
                                 engine=p.database_engine['engine'],
                                 is_replace=is_replace,
                                 parameters=parameters)
 
-    @_('DATABASE id',
-       'PROJECT id',
-       'DATABASE id ENGINE string',
-       'DATABASE id ENGINE EQUALS string',
-       'DATABASE id WITH ENGINE string',
-       'DATABASE id WITH ENGINE EQUALS string')
+    @_('DATABASE identifier',
+       'PROJECT identifier',
+       'DATABASE identifier ENGINE string',
+       'DATABASE identifier ENGINE EQUALS string',
+       'DATABASE identifier WITH ENGINE string',
+       'DATABASE identifier WITH ENGINE EQUALS string')
     def database_engine(self, p):
-        string = None
+        engine = None
         if hasattr(p, 'string'):
-            string = p.string
-        return {'id': p.id, 'engine': string}
+            engine = p.string
+        return {'identifier': p.identifier, 'engine': engine}
 
     # UNION / UNION ALL
     @_('select UNION select')
     def union(self, p):
         return Union(left=p.select0, right=p.select1, unique=True)
 
     @_('select UNION ALL select')
@@ -1368,14 +1390,15 @@
        'COLLATION',
        'COLUMNS',
        'COMMIT',
        'COMMITTED',
        'CONCAT',
        'DATASET',
        'DATASETS',
+       'DATABASE',
        'DATASOURCE',
        'DATASOURCES',
        'ENGINE',
        'ENGINES',
        'EXTENDED',
        'FIELDS',
        # 'FULL', # fixme: is parsed as alias
@@ -1411,14 +1434,15 @@
        'REPLACE',
        'REPLICA',
        'REPLICAS',
        'RETRAIN',
        'ROLLBACK',
        'SERIALIZABLE',
        'SESSION',
+       'SCHEMA',
        'SLAVE',
        'START',
        'STATUS',
        'STORAGE',
        'STREAM',
        'STREAMS',
        'TABLES',
```

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mysql/lexer.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mysql/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mysql/parser.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mysql/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -962,14 +962,15 @@
        'CHARSET',
        'CODE',
        'COLLATION',
        'COLUMNS',
        'COMMIT',
        'COMMITTED',
        'CONCAT',
+       'DATABASE',
        'ENGINE',
        'ENGINES',
        'EXTENDED',
        'FIELDS',
        # 'FULL', # fixme: is parsed as alias
        'GLOBAL',
        'HOSTS',
@@ -991,14 +992,15 @@
        'PROFILES',
        'REPEATABLE',
        'REPLICA',
        'REPLICAS',
        'ROLLBACK',
        'SERIALIZABLE',
        'SESSION',
+       'SCHEMA',
        'SLAVE',
        'START',
        'STATUS',
        'STORAGE',
        'TABLES',
        'TRANSACTION',
        'TRIGGERS',
```

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mysql/show_index.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mysql/show_index.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/dialects/mysql/variable.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/dialects/mysql/variable.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/lexer.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
     PARTITION_BY = r'\bPARTITION BY\b'
 
     # Data types
     NULL = r'\bNULL\b'
     TRUE = r'\bTRUE\b'
     FALSE = r'\bFALSE\b'
 
-    @_(r'(?:([a-zA-Z_$0-9]*[a-zA-Z_$]+[a-zA-Z_$0-9]*)|(?:`([^`]+)`))(?:\.(?:([a-zA-Z_$0-9]*[a-zA-Z_$]+[a-zA-Z_$0-9]*)|(?:`([^`]+)`)))*')
+    @_(r'(?:([a-zA-Z_$0-9]*[a-zA-Z_$]+[a-zA-Z_$0-9]*)|(?:`([^`]+)`))')
     def ID(self, t):
         return t
 
     @_(r'\d+\.\d*')
     def FLOAT(self, t):
         return t
```

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/logger.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/logger.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/parser.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -717,14 +717,16 @@
 
     # convert to types
     @_('ID',
        'CHARSET',
        'TABLES',
        'STATUS',
        'VIEW',
+       'DATABASE',
+       'SCHEMA',
        'FIELDS',
        'EXTENDED',
        'PROCESSLIST',
        'MUTEX',
        'CODE',
        'SLAVE',
        'REPLICA',
```

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/parser/utils.py` & `mindsdb_sql-0.6.0/mindsdb_sql/parser/utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/planner/query_plan.py` & `mindsdb_sql-0.6.0/mindsdb_sql/planner/query_plan.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/planner/query_planner.py` & `mindsdb_sql-0.6.0/mindsdb_sql/planner/query_planner.py`

 * *Files 0% similar despite different names*

```diff
@@ -930,15 +930,18 @@
                 ):
                     # add integration name to table
                     query.from_table.parts.insert(0, integration)
 
             join_left = join_left.from_table
 
             if orig_query.limit is not None:
-                query.limit = orig_query.limit
+                if query.limit is None or query.limit.value > orig_query.limit.value:
+                    query.limit = orig_query.limit
+            query.parentheses = False
+            query.alias = None
 
         aliased_fields = self.get_aliased_fields(query.targets)
 
         recursively_check_join_identifiers_for_ambiguity(query.where)
         recursively_check_join_identifiers_for_ambiguity(query.group_by, aliased_fields=aliased_fields)
         recursively_check_join_identifiers_for_ambiguity(query.having)
         recursively_check_join_identifiers_for_ambiguity(query.order_by, aliased_fields=aliased_fields)
```

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/planner/query_prepare.py` & `mindsdb_sql-0.6.0/mindsdb_sql/planner/query_prepare.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/planner/step_result.py` & `mindsdb_sql-0.6.0/mindsdb_sql/planner/step_result.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/planner/steps.py` & `mindsdb_sql-0.6.0/mindsdb_sql/planner/steps.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,9 +237,8 @@
 
 class SubSelectStep(PlanStep):
     def __init__(self, query, dataframe, table_name=None, *args, **kwargs):
         """Performs select from dataframe"""
         super().__init__(*args, **kwargs)
         self.query = query
         self.dataframe = dataframe
-        self.table_name = table_name
-
+        self.table_name = table_name
```

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/planner/ts_utils.py` & `mindsdb_sql-0.6.0/mindsdb_sql/planner/ts_utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/planner/utils.py` & `mindsdb_sql-0.6.0/mindsdb_sql/planner/utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql/render/sqlalchemy_render.py` & `mindsdb_sql-0.6.0/mindsdb_sql/render/sqlalchemy_render.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.5.1/mindsdb_sql.egg-info/PKG-INFO` & `mindsdb_sql-0.6.0/mindsdb_sql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mindsdb-sql
-Version: 0.5.1
+Version: 0.6.0
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.5.1/setup.py` & `mindsdb_sql-0.6.0/setup.py`

 * *Files identical despite different names*

