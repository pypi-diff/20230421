# Comparing `tmp/snowflake_cli_labs-0.2.5.tar.gz` & `tmp/snowflake_cli_labs-0.2.7.tar.gz`

## Comparing `snowflake_cli_labs-0.2.5.tar` & `snowflake_cli_labs-0.2.7.tar`

### file list

```diff
@@ -1,79 +1,80 @@
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11607 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/README.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/requirements-dev.txt
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/requirements.txt
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/snowcli.spec
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/tox.ini
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/docs/images/coverage_1.png
--rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/docs/images/coverage_2.png
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/docs/images/coverage_3.png
--rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/docs/images/coverage_4.png
--rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/docs/images/coverage_5.png
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/__init__.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/config.py
--rw-r--r--   0        0        0    16220 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/snow_connector.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/snowsql_config.py
--rw-r--r--   0        0        0    20498 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/utils.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/cli/__init__.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/cli/connection.py
--rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/cli/function.py
--rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/cli/package.py
--rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/cli/procedure.py
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/cli/render.py
--rw-r--r--   0        0        0    20029 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/cli/snowpark_shared.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/cli/sql.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/cli/stage.py
--rw-r--r--   0        0        0    10105 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/cli/streamlit.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/cli/warehouse.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/cli/procedure_coverage/__init__.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/cli/procedure_coverage/clear.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/cli/procedure_coverage/report.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/python_templates/environment.yml.jinja
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/python_templates/snowpark_coverage.py.jinja
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/python_templates/streamlit_app_launcher.py.jinja
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/call_procedure.sql
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/create_function.sql
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/create_procedure.sql
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/create_stage.sql
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/create_streamlit.sql
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/describe_function.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/describe_procedure.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/describe_streamlit.sql
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/drop_function.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/drop_procedure.sql
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/drop_stage.sql
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/drop_streamlit.sql
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/execute_function.sql
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/get_stage.sql
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/get_streamlit_url.sql
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/list_functions.sql
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/list_procedures.sql
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/list_stage.sql
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/list_stages.sql
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/list_streamlits.sql
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/put_stage.sql
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/remove_from_stage.sql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/set_procedure_comment.sql
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/share_streamlit.sql
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/snowcli/sql/show_warehouses.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/templates/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/templates/default_function/.gitignore
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/templates/default_function/app.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/templates/default_function/app.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/templates/default_function/requirements.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/templates/default_procedure/.gitignore
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/templates/default_procedure/app.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/templates/default_procedure/app.toml
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/templates/default_procedure/local_connection.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/src/templates/default_procedure/requirements.txt
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/tests/conftest.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/tests/test_main.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/tests/test_render.py
--rw-r--r--   0        0        0    14849 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/tests/test_snow_connector.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/tests/test_sql.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/tests/__snapshots__/test_snow_connector.ambr
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/LICENSE
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/LEGAL.md
+-rw-r--r--   0        0        0    11607 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/README.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/requirements-dev.txt
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/requirements.txt
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/snowcli.spec
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/tox.ini
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/docs/images/coverage_1.png
+-rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/docs/images/coverage_2.png
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/docs/images/coverage_3.png
+-rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/docs/images/coverage_4.png
+-rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/docs/images/coverage_5.png
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/__init__.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/config.py
+-rw-r--r--   0        0        0    16558 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/snow_connector.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/snowsql_config.py
+-rw-r--r--   0        0        0    21579 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/utils.py
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/__init__.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/connection.py
+-rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/function.py
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/package.py
+-rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/procedure.py
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/render.py
+-rw-r--r--   0        0        0    20029 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/snowpark_shared.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/sql.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/stage.py
+-rw-r--r--   0        0        0    10105 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/streamlit.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/warehouse.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/procedure_coverage/__init__.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/procedure_coverage/clear.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/procedure_coverage/report.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/python_templates/environment.yml.jinja
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/python_templates/snowpark_coverage.py.jinja
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/python_templates/streamlit_app_launcher.py.jinja
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/call_procedure.sql
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/create_function.sql
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/create_procedure.sql
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/create_stage.sql
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/create_streamlit.sql
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/describe_function.sql
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/describe_procedure.sql
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/describe_streamlit.sql
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/drop_function.sql
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/drop_procedure.sql
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/drop_stage.sql
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/drop_streamlit.sql
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/execute_function.sql
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/get_stage.sql
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/get_streamlit_url.sql
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/list_functions.sql
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/list_procedures.sql
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/list_stage.sql
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/list_stages.sql
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/list_streamlits.sql
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/put_stage.sql
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/remove_from_stage.sql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/set_procedure_comment.sql
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/share_streamlit.sql
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/show_warehouses.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_function/.gitignore
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_function/app.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_function/app.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_function/requirements.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_procedure/.gitignore
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_procedure/app.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_procedure/app.toml
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_procedure/local_connection.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_procedure/requirements.txt
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/tests/conftest.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/tests/test_main.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/tests/test_render.py
+-rw-r--r--   0        0        0    14849 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/tests/test_snow_connector.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/tests/test_sql.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/tests/__snapshots__/test_snow_connector.ambr
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/LICENSE
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/PKG-INFO
```

### Comparing `snowflake_cli_labs-0.2.5/.pre-commit-config.yaml` & `snowflake_cli_labs-0.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/README.md` & `snowflake_cli_labs-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/snowcli.spec` & `snowflake_cli_labs-0.2.7/snowcli.spec`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/docs/images/coverage_1.png` & `snowflake_cli_labs-0.2.7/docs/images/coverage_1.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/docs/images/coverage_2.png` & `snowflake_cli_labs-0.2.7/docs/images/coverage_2.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/docs/images/coverage_3.png` & `snowflake_cli_labs-0.2.7/docs/images/coverage_3.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/docs/images/coverage_4.png` & `snowflake_cli_labs-0.2.7/docs/images/coverage_4.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/docs/images/coverage_5.png` & `snowflake_cli_labs-0.2.7/docs/images/coverage_5.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/config.py` & `snowflake_cli_labs-0.2.7/src/snowcli/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,26 +33,25 @@
             return next(p.glob("app.toml"))
 
     def save(self):
         with open(self.path, "w") as f:
             toml.dump(self.config, f)
 
 
-def connectToSnowflake(connection: Optional[str] = None):  # type: ignore
+def connectToSnowflake(connection: Optional[str] = None, **overrides):  # type: ignore
     global snowflake_connection
     cfg = AppConfig()
     snowsql_config = SnowsqlConfig(path=cfg.config.get("snowsql_config_path"))
 
     # If there's no user-provided connection then read
     # the one specified by configuration file
     connection = connection or cfg.config.get("snowsql_connection_name")
 
     snowflake_connection = SnowflakeConnector(
-        snowsql_config,
-        connection,
+        snowsql_config, connection, overrides=overrides
     )
 
 
 def isAuth():
     cfg = AppConfig()
     if "snowsql_config_path" not in cfg.config:
         click.echo("You must login first with `snow login`")
```

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/snow_connector.py` & `snowflake_cli_labs-0.2.7/src/snowcli/snow_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 from __future__ import annotations
 
 import os
 import pkgutil
 from io import StringIO
 from pathlib import Path
+from typing import Optional
 
 import snowflake.connector
 from jinja2 import Environment, FileSystemLoader
 from snowflake.connector.cursor import SnowflakeCursor
 
 from snowcli.snowsql_config import SnowsqlConfig
 
 TEMPLATES_PATH = Path(__file__).parent / "sql"
 
 
 class SnowflakeConnector:
     """Initialize a connection from a snowsql-formatted config"""
 
-    def __init__(self, snowsql_config: SnowsqlConfig, connection_name: str):
+    def __init__(
+        self,
+        snowsql_config: SnowsqlConfig,
+        connection_name: str,
+        overrides: Optional[dict] = None,
+    ):
         self.snowsql_config = snowsql_config
         self.connection_name = connection_name
         self.connection_config: dict = snowsql_config.get_connection(
             connection_name,
         )
+        if overrides:
+            for config, value in ((k, v) for k, v in overrides.items() if v):
+                self.connection_config[config] = value
         self.connection_config["application"] = "SNOWCLI"
         self.ctx = snowflake.connector.connect(**self.connection_config)
         self.cs = self.ctx.cursor()
 
     def __del__(self):
-        self.cs.close()
-        self.ctx.close()
+        try:
+            self.cs.close()
+            self.ctx.close()
+        except (TypeError, AttributeError):
+            pass
 
     def getVersion(self):
         self.cs.execute("SELECT current_version()")
         return self.cs.fetchone()[0]
 
     def createFunction(
         self,
```

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/snowsql_config.py` & `snowflake_cli_labs-0.2.7/src/snowcli/snowsql_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/utils.py` & `snowflake_cli_labs-0.2.7/src/snowcli/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -298,14 +298,15 @@
 def installPackages(
     file_name: str | None,
     perform_anaconda_check: bool = True,
     package_native_libraries: YesNoAskOptionsType = "ask",
     package_name: str | None = None,
 ) -> tuple[bool, dict[str, list[str]] | None]:
     pip_install_result = None
+    second_chance_results = None
     if file_name is not None:
         try:
             process = subprocess.Popen(
                 [PIP_PATH, "install", "-t", ".packages/", "-r", file_name],
                 stdout=subprocess.PIPE,
                 universal_newlines=True,
             )
@@ -418,25 +419,47 @@
         if (
             not str(file).startswith(".")
             and not file.match(f"{pack_dir}/*")
             and not file.match(dest_zip)
         ):
             zipf.write(os.path.relpath(file))
 
+    for dir_path in os.getenv("SNOWCLI_INCLUDE_PATHS", "").split(":"):
+        directory = pathlib.Path(dir_path)
+        if directory.is_dir():
+            for file in pathlib.Path(directory).glob("**/*"):
+                if (
+                    not str(file).startswith(".")
+                    and not file.match("*.pyc")
+                    and not file.match("*__pycache__*")
+                ):
+                    zipf.write(file, arcname=os.path.relpath(file, directory))
+
     # close the zip file object
     zipf.close()
     return True
 
 
 def standardZipDir(dest_zip: str) -> bool:
     zipf = zipfile.ZipFile(dest_zip, "w", zipfile.ZIP_DEFLATED, allowZip64=True)
     for file in pathlib.Path(".").glob("*"):
         if not file.match(".*"):
             zipf.write(os.path.relpath(file))
 
+    for dir_path in os.getenv("SNOWCLI_INCLUDE_PATHS", "").split(":"):
+        directory = pathlib.Path(dir_path)
+        if directory.is_dir():
+            for file in pathlib.Path(directory).glob("**/*"):
+                if (
+                    not str(file).startswith(".")
+                    and not file.match("*.pyc")
+                    and not file.match("*__pycache__*")
+                ):
+                    zipf.write(file, arcname=os.path.relpath(file, directory))
+
     # close the zip file object
     zipf.close()
     return True
 
 
 def getSnowflakePackages() -> list[str]:
     if os.path.exists("requirements.snowflake.txt"):
@@ -521,17 +544,18 @@
     if value:
         try:
             app_config = AppConfig().config
 
             # Initialize the default map
             ctx.default_map = ctx.default_map or {}
             # if app_config has key 'default'
-            if "default" in app_config:
+            config_section = os.getenv("SNOWCLI_CONFIG_SECTION", "default")
+            if config_section in app_config:
                 ctx.default_map.update(
-                    app_config.get("default"),
+                    app_config.get(config_section),
                 )  # type: ignore
             if value in app_config:
                 # TODO: Merge the config dict into default_map
                 # type: ignore
                 ctx.default_map.update(app_config.get(value))
         except Exception as ex:
             raise typer.BadParameter(str(ex))
```

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/cli/__init__.py` & `snowflake_cli_labs-0.2.7/src/snowcli/cli/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
+import pkgutil
 import sys
+from collections.abc import Container
 from pathlib import Path
 
 import typer
 from rich import print
 
 from .. import __about__
 from ..config import AppConfig
@@ -136,22 +138,30 @@
     ),
 ) -> None:
     """
     SnowCLI - A CLI for Snowflake
     """
 
 
-app.add_typer(function.app, name="function")
-app.add_typer(procedure.app, name="procedure")
-app.add_typer(streamlit.app, name="streamlit")
-app.add_typer(connection.app, name="connection")
-app.add_typer(warehouse.app, name="warehouse")
-app.add_typer(stage.app, name="stage")
-app.add_typer(package.app, name="package")
-app.add_typer(render.app, name="render")
+MODULE_IGNORE_SET = frozenset(("procedure_coverage",))
+
+
+def register_cli_typers(ignore_container: Container[str] = MODULE_IGNORE_SET) -> None:
+    for _, name, _ in pkgutil.walk_packages(__path__):
+        if name not in ignore_container:
+            cli_app = __import__(f"{__name__}.{name}", fromlist=["_trash"])
+            try:
+                app.add_typer(cli_app.app, name=name)
+            except AttributeError:
+                # Ignore modules that don't define app global
+                pass
+
+
+register_cli_typers()
+
 app.command("sql")(sql.execute_sql)
 
 
 if __name__ == "__main__":
     app()
 
 if getattr(sys, "frozen", False):
```

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/cli/connection.py` & `snowflake_cli_labs-0.2.7/src/snowcli/cli/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/cli/function.py` & `snowflake_cli_labs-0.2.7/src/snowcli/cli/function.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/cli/package.py` & `snowflake_cli_labs-0.2.7/src/snowcli/cli/package.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/cli/procedure.py` & `snowflake_cli_labs-0.2.7/src/snowcli/cli/procedure.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/cli/render.py` & `snowflake_cli_labs-0.2.7/src/snowcli/cli/render.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/cli/snowpark_shared.py` & `snowflake_cli_labs-0.2.7/src/snowcli/cli/snowpark_shared.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/cli/sql.py` & `snowflake_cli_labs-0.2.7/src/snowcli/cli/sql.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,23 +25,29 @@
         self.table = table
         self.live = live
 
     def add_row(self, *args):
         self.table.add_row(*args)
         self.live.refresh()
 
+    def add_result_row(self, result):
+        self.table.add_row(str(result))
+        self.live.refresh()
+
 
 class LoggingCursor(SnowflakeCursor):
     def __init__(self, live_output: LiveOutput, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        super().__init__(*args, use_dict_result=True, **kwargs)
         self.live_output = live_output
 
     def execute(self, command: str, *args, **kwargs):
         self.live_output.add_row(command)
-        super(LoggingCursor, self).execute(command, *args, **kwargs)
+        result = super(LoggingCursor, self).execute(command, *args, **kwargs)
+        for result in result.fetchall():
+            self.live_output.add_result_row(result)
 
 
 def execute_sql(
     query: Optional[str] = typer.Option(
         None,
         "-q",
         "--query",
@@ -56,14 +62,36 @@
         dir_okay=False,
         readable=True,
         help="File to execute.",
     ),
     connection: Optional[str] = typer.Option(
         None, "-c", "--connection", help="Connection to be used"
     ),
+    account: Optional[str] = typer.Option(
+        None,
+        "-a",
+        "--accountname",
+        "--account",
+        help="Name assigned to your Snowflake account.",
+    ),
+    user: Optional[str] = typer.Option(
+        None, "-u", "--username", "--user", help="Username to connect to Snowflake."
+    ),
+    database: Optional[str] = typer.Option(
+        None, "-d", "--dbname", "--database", help="Database to use."
+    ),
+    schema: Optional[str] = typer.Option(
+        None, "-s", "--schemaname", "--schema", help=" Schema in the database to use."
+    ),
+    role: Optional[str] = typer.Option(
+        None, "-r", "--rolename", "--role", help="Role to be used"
+    ),
+    warehouse: Optional[str] = typer.Option(
+        None, "-w", "--warehouse", help="Warehouse to use."
+    ),
     verbose: Optional[bool] = typer.Option(
         True, "-v", "--verbose", help="Prints information about executed queries"
     ),
 ):
     """
     Executes Snowflake query.
 
@@ -89,15 +117,23 @@
         sql = sys_input
     else:
         sql = query if query else file.read_text()  # type: ignore
 
     if not config.isAuth():
         raise ValueError("Not authorize")
 
-    config.connectToSnowflake(connection)
+    config.connectToSnowflake(
+        connection,
+        account=account,
+        user=user,
+        role=role,
+        warehouse=warehouse,
+        database=database,
+        schema=schema,
+    )
 
     table = Table(show_lines=True, box=box.ASCII, width=120)
     table.add_column("Query")
 
     if verbose:
         with Live(table, auto_refresh=False) as live:
             config.snowflake_connection.ctx.execute_string(
```

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/cli/stage.py` & `snowflake_cli_labs-0.2.7/src/snowcli/cli/stage.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/cli/streamlit.py` & `snowflake_cli_labs-0.2.7/src/snowcli/cli/streamlit.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/cli/warehouse.py` & `snowflake_cli_labs-0.2.7/src/snowcli/cli/warehouse.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/cli/procedure_coverage/clear.py` & `snowflake_cli_labs-0.2.7/src/snowcli/cli/procedure_coverage/clear.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/cli/procedure_coverage/report.py` & `snowflake_cli_labs-0.2.7/src/snowcli/cli/procedure_coverage/report.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/python_templates/snowpark_coverage.py.jinja` & `snowflake_cli_labs-0.2.7/src/snowcli/python_templates/snowpark_coverage.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/python_templates/streamlit_app_launcher.py.jinja` & `snowflake_cli_labs-0.2.7/src/snowcli/python_templates/streamlit_app_launcher.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/snowcli/sql/create_procedure.sql` & `snowflake_cli_labs-0.2.7/src/snowcli/sql/create_procedure.sql`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/templates/default_procedure/app.py` & `snowflake_cli_labs-0.2.7/src/templates/default_procedure/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/src/templates/default_procedure/local_connection.py` & `snowflake_cli_labs-0.2.7/src/templates/default_procedure/local_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/tests/test_render.py` & `snowflake_cli_labs-0.2.7/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/tests/test_snow_connector.py` & `snowflake_cli_labs-0.2.7/tests/test_snow_connector.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/tests/__snapshots__/test_snow_connector.ambr` & `snowflake_cli_labs-0.2.7/tests/__snapshots__/test_snow_connector.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/LICENSE` & `snowflake_cli_labs-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.5/pyproject.toml` & `snowflake_cli_labs-0.2.7/pyproject.toml`

 * *Files identical despite different names*

