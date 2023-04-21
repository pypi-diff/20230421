# Comparing `tmp/gluetool-2.3.tar.gz` & `tmp/gluetool-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gluetool-2.3.tar", max compression
+gzip compressed data, was "gluetool-2.4.tar", max compression
```

## Comparing `gluetool-2.3.tar` & `gluetool-2.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1072 2023-03-14 16:49:21.402618 gluetool-2.3/README.rst
--rw-r--r--   0        0        0     4522 2023-03-14 16:49:21.402618 gluetool-2.3/assets/html-log/prism.css
--rw-r--r--   0        0        0    13651 2023-03-14 16:49:21.402618 gluetool-2.3/assets/html-log/prism.js
--rw-r--r--   0        0        0   628536 2023-03-14 16:49:21.404618 gluetool-2.3/assets/html-log/semantic.min.css
--rw-r--r--   0        0        0   275730 2023-03-14 16:49:21.405618 gluetool-2.3/assets/html-log/semantic.min.js
--rw-r--r--   0        0        0      351 2023-03-14 16:49:21.406618 gluetool-2.3/gluetool/__init__.py
--rw-r--r--   0        0        0    12916 2023-03-14 16:49:21.406618 gluetool-2.3/gluetool/action.py
--rw-r--r--   0        0        0     2167 2023-03-14 16:49:21.406618 gluetool-2.3/gluetool/color.py
--rw-r--r--   0        0        0      765 2023-03-14 16:49:21.406618 gluetool-2.3/gluetool/core.moduleinfo
--rw-r--r--   0        0        0    97437 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/glue.py
--rw-r--r--   0        0        0    19758 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/help.py
--rw-r--r--   0        0        0    14613 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/html_log.py
--rw-r--r--   0        0        0    47722 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/log.py
--rw-r--r--   0        0        0     3752 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/proxy.py
--rw-r--r--   0        0        0        0 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/py.typed
--rw-r--r--   0        0        0     4254 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/pylint/__init__.py
--rw-r--r--   0        0        0     5248 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/pylint/option_default.py
--rw-r--r--   0        0        0     4698 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/pylint/shared_defined.py
--rw-r--r--   0        0        0     3221 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/pylint/unknown_option.py
--rw-r--r--   0        0        0     6265 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/result.py
--rw-r--r--   0        0        0     9411 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/sentry.py
--rw-r--r--   0        0        0     2620 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/tests/__init__.py
--rw-r--r--   0        0        0      311 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/tests/assets/parse_config/configroot/config/data_config_root_a
--rw-r--r--   0        0        0      321 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/tests/assets/parse_config/configroot/config/data_config_root_b
--rw-r--r--   0        0        0       42 2023-03-14 16:49:21.407618 gluetool-2.3/gluetool/tests/assets/parse_config/configroot/config/data_not_unicode
--rw-r--r--   0        0        0      346 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/assets/parse_config/configroota/config/data_config_root_a
--rw-r--r--   0        0        0      321 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/assets/parse_config/configrootb/config/data_config_root_b
--rw-r--r--   0        0        0     1134 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/conftest.py
--rw-r--r--   0        0        0     5550 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_core.py
--rw-r--r--   0        0        0     4395 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_error.py
--rw-r--r--   0        0        0      930 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_eval_context.py
--rw-r--r--   0        0        0     1280 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_help.py
--rw-r--r--   0        0        0     1996 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_json.py
--rw-r--r--   0        0        0     1716 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_load_yaml.py
--rw-r--r--   0        0        0     2342 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_log_exception.py
--rw-r--r--   0        0        0     1288 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_logging.py
--rw-r--r--   0        0        0     4470 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_module_discovery.py
--rw-r--r--   0        0        0      573 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_new_xml_element.py
--rw-r--r--   0        0        0     3296 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_normalize_option.py
--rw-r--r--   0        0        0     1132 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_option.py
--rw-r--r--   0        0        0     4021 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_parse_config.py
--rw-r--r--   0        0        0     1791 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_pipeline_step.py
--rw-r--r--   0        0        0      734 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_render_template.py
--rw-r--r--   0        0        0      665 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_requests.py
--rw-r--r--   0        0        0     2637 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_result.py
--rw-r--r--   0        0        0     8672 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_run_command.py
--rw-r--r--   0        0        0     8165 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_run_modules.py
--rw-r--r--   0        0        0     2517 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_tool.py
--rw-r--r--   0        0        0      754 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_treat_url.py
--rw-r--r--   0        0        0     2813 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_utils.py
--rw-r--r--   0        0        0     1987 2023-03-14 16:49:21.408618 gluetool-2.3/gluetool/tests/test_wait.py
--rw-r--r--   0        0        0    16521 2023-03-14 16:49:21.409618 gluetool-2.3/gluetool/tool.py
--rw-r--r--   0        0        0    55037 2023-03-14 16:49:21.409618 gluetool-2.3/gluetool/utils.py
--rw-r--r--   0        0        0      165 2023-03-14 16:49:21.409618 gluetool-2.3/gluetool/version.py
--rw-r--r--   0        0        0        0 2023-03-14 16:49:21.409618 gluetool-2.3/gluetool_modules/__init__.py
--rw-r--r--   0        0        0     4062 2023-03-14 16:49:21.409618 gluetool-2.3/gluetool_modules/bash_completion.py
--rw-r--r--   0        0        0    10863 2023-03-14 16:49:21.409618 gluetool-2.3/gluetool_modules/dep_list.py
--rw-r--r--   0        0        0     7490 2023-03-14 16:49:21.409618 gluetool-2.3/gluetool_modules/yaml_pipeline.py
--rw-r--r--   0        0        0     3387 2023-03-15 09:07:35.997971 gluetool-2.3/pyproject.toml
--rw-r--r--   0        0        0     2770 2023-03-15 09:09:27.265249 gluetool-2.3/setup.py
--rw-r--r--   0        0        0     2694 2023-03-15 09:09:27.265557 gluetool-2.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-14 16:49:21.402618 gluetool-2.4/README.rst
+-rw-r--r--   0        0        0     4522 2023-03-14 16:49:21.402618 gluetool-2.4/assets/html-log/prism.css
+-rw-r--r--   0        0        0    13651 2023-03-14 16:49:21.402618 gluetool-2.4/assets/html-log/prism.js
+-rw-r--r--   0        0        0   628536 2023-03-14 16:49:21.404618 gluetool-2.4/assets/html-log/semantic.min.css
+-rw-r--r--   0        0        0   275730 2023-03-14 16:49:21.405618 gluetool-2.4/assets/html-log/semantic.min.js
+-rw-r--r--   0        0        0      351 2023-03-14 16:49:21.406618 gluetool-2.4/gluetool/__init__.py
+-rw-r--r--   0        0        0    12916 2023-03-14 16:49:21.406618 gluetool-2.4/gluetool/action.py
+-rw-r--r--   0        0        0     2167 2023-03-14 16:49:21.406618 gluetool-2.4/gluetool/color.py
+-rw-r--r--   0        0        0      765 2023-03-14 16:49:21.406618 gluetool-2.4/gluetool/core.moduleinfo
+-rw-r--r--   0        0        0    97437 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/glue.py
+-rw-r--r--   0        0        0    19758 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/help.py
+-rw-r--r--   0        0        0    14613 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/html_log.py
+-rw-r--r--   0        0        0    47722 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/log.py
+-rw-r--r--   0        0        0     3752 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/proxy.py
+-rw-r--r--   0        0        0        0 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/py.typed
+-rw-r--r--   0        0        0     4254 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/pylint/__init__.py
+-rw-r--r--   0        0        0     5248 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/pylint/option_default.py
+-rw-r--r--   0        0        0     4698 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/pylint/shared_defined.py
+-rw-r--r--   0        0        0     3221 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/pylint/unknown_option.py
+-rw-r--r--   0        0        0     6265 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/result.py
+-rw-r--r--   0        0        0     9411 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/sentry.py
+-rw-r--r--   0        0        0     2620 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/tests/__init__.py
+-rw-r--r--   0        0        0      311 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/tests/assets/parse_config/configroot/config/data_config_root_a
+-rw-r--r--   0        0        0      321 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/tests/assets/parse_config/configroot/config/data_config_root_b
+-rw-r--r--   0        0        0       42 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/tests/assets/parse_config/configroot/config/data_not_unicode
+-rw-r--r--   0        0        0      346 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/assets/parse_config/configroota/config/data_config_root_a
+-rw-r--r--   0        0        0      321 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/assets/parse_config/configrootb/config/data_config_root_b
+-rw-r--r--   0        0        0     1134 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/conftest.py
+-rw-r--r--   0        0        0     5550 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_core.py
+-rw-r--r--   0        0        0     4395 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_error.py
+-rw-r--r--   0        0        0      930 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_eval_context.py
+-rw-r--r--   0        0        0     1280 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_help.py
+-rw-r--r--   0        0        0     1996 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_json.py
+-rw-r--r--   0        0        0     3303 2023-04-21 12:14:52.374302 gluetool-2.4/gluetool/tests/test_load_yaml.py
+-rw-r--r--   0        0        0     2342 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_log_exception.py
+-rw-r--r--   0        0        0     1288 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_logging.py
+-rw-r--r--   0        0        0     4470 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_module_discovery.py
+-rw-r--r--   0        0        0      573 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_new_xml_element.py
+-rw-r--r--   0        0        0     3296 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_normalize_option.py
+-rw-r--r--   0        0        0     1132 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_option.py
+-rw-r--r--   0        0        0     4021 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_parse_config.py
+-rw-r--r--   0        0        0     1791 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_pipeline_step.py
+-rw-r--r--   0        0        0      734 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_render_template.py
+-rw-r--r--   0        0        0      665 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_requests.py
+-rw-r--r--   0        0        0     2637 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_result.py
+-rw-r--r--   0        0        0     8672 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_run_command.py
+-rw-r--r--   0        0        0     8165 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_run_modules.py
+-rw-r--r--   0        0        0     2517 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_tool.py
+-rw-r--r--   0        0        0      754 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_treat_url.py
+-rw-r--r--   0        0        0     2813 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_utils.py
+-rw-r--r--   0        0        0     1987 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_wait.py
+-rw-r--r--   0        0        0    16475 2023-04-21 12:14:52.375302 gluetool-2.4/gluetool/tool.py
+-rw-r--r--   0        0        0    58058 2023-04-21 12:14:52.375302 gluetool-2.4/gluetool/utils.py
+-rw-r--r--   0        0        0      165 2023-03-14 16:49:21.409618 gluetool-2.4/gluetool/version.py
+-rw-r--r--   0        0        0        0 2023-03-14 16:49:21.409618 gluetool-2.4/gluetool_modules/__init__.py
+-rw-r--r--   0        0        0     4062 2023-03-14 16:49:21.409618 gluetool-2.4/gluetool_modules/bash_completion.py
+-rw-r--r--   0        0        0    10863 2023-03-14 16:49:21.409618 gluetool-2.4/gluetool_modules/dep_list.py
+-rw-r--r--   0        0        0     7490 2023-03-14 16:49:21.409618 gluetool-2.4/gluetool_modules/yaml_pipeline.py
+-rw-r--r--   0        0        0     3412 2023-04-21 13:01:42.155351 gluetool-2.4/pyproject.toml
+-rw-r--r--   0        0        0     2823 2023-04-21 13:02:05.329002 gluetool-2.4/setup.py
+-rw-r--r--   0        0        0     2775 2023-04-21 13:02:05.329256 gluetool-2.4/PKG-INFO
```

### Comparing `gluetool-2.3/README.rst` & `gluetool-2.4/README.rst`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/assets/html-log/prism.css` & `gluetool-2.4/assets/html-log/prism.css`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/assets/html-log/prism.js` & `gluetool-2.4/assets/html-log/prism.js`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/assets/html-log/semantic.min.css` & `gluetool-2.4/assets/html-log/semantic.min.css`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/assets/html-log/semantic.min.js` & `gluetool-2.4/assets/html-log/semantic.min.js`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/action.py` & `gluetool-2.4/gluetool/action.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/color.py` & `gluetool-2.4/gluetool/color.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/core.moduleinfo` & `gluetool-2.4/gluetool/core.moduleinfo`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/glue.py` & `gluetool-2.4/gluetool/glue.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/help.py` & `gluetool-2.4/gluetool/help.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/html_log.py` & `gluetool-2.4/gluetool/html_log.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/log.py` & `gluetool-2.4/gluetool/log.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/proxy.py` & `gluetool-2.4/gluetool/proxy.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/pylint/__init__.py` & `gluetool-2.4/gluetool/pylint/__init__.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/pylint/option_default.py` & `gluetool-2.4/gluetool/pylint/option_default.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/pylint/shared_defined.py` & `gluetool-2.4/gluetool/pylint/shared_defined.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/pylint/unknown_option.py` & `gluetool-2.4/gluetool/pylint/unknown_option.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/result.py` & `gluetool-2.4/gluetool/result.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/sentry.py` & `gluetool-2.4/gluetool/sentry.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/__init__.py` & `gluetool-2.4/gluetool/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/conftest.py` & `gluetool-2.4/gluetool/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_core.py` & `gluetool-2.4/gluetool/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_error.py` & `gluetool-2.4/gluetool/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_eval_context.py` & `gluetool-2.4/gluetool/tests/test_eval_context.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_help.py` & `gluetool-2.4/gluetool/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_json.py` & `gluetool-2.4/gluetool/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_log_exception.py` & `gluetool-2.4/gluetool/tests/test_log_exception.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_logging.py` & `gluetool-2.4/gluetool/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_module_discovery.py` & `gluetool-2.4/gluetool/tests/test_module_discovery.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_new_xml_element.py` & `gluetool-2.4/gluetool/tests/test_new_xml_element.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_normalize_option.py` & `gluetool-2.4/gluetool/tests/test_normalize_option.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_option.py` & `gluetool-2.4/gluetool/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_parse_config.py` & `gluetool-2.4/gluetool/tests/test_parse_config.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_pipeline_step.py` & `gluetool-2.4/gluetool/tests/test_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_render_template.py` & `gluetool-2.4/gluetool/tests/test_render_template.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_requests.py` & `gluetool-2.4/gluetool/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_result.py` & `gluetool-2.4/gluetool/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_run_command.py` & `gluetool-2.4/gluetool/tests/test_run_command.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_run_modules.py` & `gluetool-2.4/gluetool/tests/test_run_modules.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_tool.py` & `gluetool-2.4/gluetool/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_treat_url.py` & `gluetool-2.4/gluetool/tests/test_treat_url.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_utils.py` & `gluetool-2.4/gluetool/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tests/test_wait.py` & `gluetool-2.4/gluetool/tests/test_wait.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool/tool.py` & `gluetool-2.4/gluetool/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,32 +136,32 @@
         for step in pipeline_desc:
             cmdline.append([step.module_designation] + step.argv)
 
         assert self.Glue is not None
         self.Glue.info('command-line:\n{}'.format(format_command_line(cmdline)))
 
     @cached_property
-    def _exit_logger(self) -> Union[logging.Logger, gluetool.log.ContextAdapter]:
+    def _exit_logger(self) -> gluetool.log.ContextAdapter:
 
         """
         Return logger for use when finishing the ``gluetool`` pipeline.
         """
 
         # We want to use the current logger, if there's any set up.
-        logger: Union[logging.Logger, gluetool.log.ContextAdapter] = gluetool.log.Logging.get_logger()
+        logger = gluetool.log.Logging.get_logger()
 
         if logger:
             return logger
 
         # This may happen only when something went wrong during logger initialization
         # when Glue instance was created. Falling back to a very basic Logger seems
         # to be the best option here.
 
         logging.basicConfig(level=logging.DEBUG)
-        logger = logging.getLogger()
+        logger = gluetool.log.ContextAdapter(logging.getLogger())
 
         logger.warning('Cannot use custom logger, falling back to a default one')
 
         return logger
 
     def _quit(self, exit_status: int) -> NoReturn:
```

### Comparing `gluetool-2.3/gluetool/utils.py` & `gluetool-2.4/gluetool/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,25 +27,27 @@
 from six.moves import http_client, urllib
 
 import bs4
 import urlnormalizer
 import jinja2
 import requests as original_requests
 import ruamel.yaml
+import cattrs
 
 from .glue import GlueError, SoftGlueError, GlueCommandError
 from .result import Result
 from .log import Logging, ContextAdapter, PackageAdapter, LoggerMixin, BlobLogger, \
     log_blob, log_dict, print_wrapper
 
 # Type annotations
 # pylint: disable=unused-import, wrong-import-order
-from typing import IO, cast  # noqa
-from typing import Any, Callable, Deque, Dict, List, Optional, Pattern, Tuple, TypeVar, Union  # noqa
+from typing import IO, cast, overload  # noqa
+from typing import Any, Callable, Deque, Dict, List, Optional, Pattern, Tuple, TypeVar, Union, Generic, Type  # noqa
 from .log import LoggingFunctionType  # noqa
+from typing_extensions import Literal  # noqa
 
 import logging  # noqa
 
 
 # Type variable used in generic types
 # pylint: disable=invalid-name
 T = TypeVar('T')
@@ -726,15 +728,15 @@
         try:
             Command(['/bin/bash', '-c', 'command -v {}'.format(cmd)]).run(stdout=DEVNULL)
 
         except GlueError as exc:
             raise GlueError("Command '{}' not found on the system".format(ensure_str(cmd))) from exc
 
 
-class cached_property(object):
+class cached_property(Generic[T]):
     # pylint: disable=invalid-name,too-few-public-methods
     """
     ``property``-like decorator - at first access, it calls decorated
     method to acquire the real value, and then replaces itself with
     this value, making it effectively "cached". Useful for properties
     whose value does not change over time, and where getting the real
     value could penalize execution with unnecessary (network, memory)
@@ -743,20 +745,20 @@
     Delete attribute to clear the cached value - on next access, decorated
     method will be called again, to acquire the real value.
 
     Of possible options, only read-only instance attribute access is
     supported so far.
     """
 
-    def __init__(self, method: Callable[..., Any]) -> None:
+    def __init__(self, method: Callable[..., T]) -> None:
 
         self._method = method
         self.__doc__ = getattr(method, '__doc__')
 
-    def __get__(self, obj: Any, cls: Any) -> Any:
+    def __get__(self, obj: Any, cls: Any) -> T:
 
         # does not support class attribute access, only instance
         assert obj is not None
 
         # get the real value of this property
         value = self._method(obj)
 
@@ -1016,23 +1018,74 @@
     :param str loader_type: type of YAML parser and loader. ``None`` or ``rt`` for round-trip (default),
         ``safe``, ``unsafe`` or ``base``.
     """
 
     return YAML(loader_type).load(yaml_string)
 
 
-def load_yaml(filepath: str, loader_type: Optional[str] = None, logger: Optional[ContextAdapter] = None) -> Any:
+def create_cattrs_converter(**kwargs: Any) -> cattrs.Converter:
+    """
+    Create a customized `cattrs.Converter` instance.
+
+    This converter, while structuring data, does not try to convert pieces of data into primitive data types (int, str,
+    etc.). By default, this converting is enabled, e.g. feeding a list to a field annotated as ``str`` would convert the
+    list to string. This can lead to surprises as it would even pass ``attrs`` validation (if enabled), since it is
+    performed after ``cattrs`` constructing.
+    """
+    def nop(value: Any, _: Any) -> Any:
+        return value
+
+    converter = cattrs.Converter(**kwargs)
+    for cls in [int, float, str, bool, bytes]:
+        converter.register_structure_hook(cls, nop)
+    return converter
+
+
+def create_cattrs_unserializer(cls: Type[T], converter: Optional[cattrs.Converter] = None) -> Callable[[Any], T]:
+    """
+    Create a function which unserializes data into attrs-class modelled structures using cattrs library.
+    Intended to be used with `load_yaml()` function as its `unserialize` parameter.
+
+    :param type cls: type representing the data structure
+    :param cattrs.Converter converter: optional custom `cattrs` converter
+    :returns: function for unserializing data into class-based structure
+    """
+
+    converter = converter or create_cattrs_converter()
+
+    def unserializer(data: Any) -> T:
+        assert converter
+        return converter.structure(data, cls)
+    return unserializer
+
+
+@overload
+def load_yaml(filepath: str, loader_type: Optional[str] = None, logger: Optional[ContextAdapter] = None,
+              unserialize: None = None) -> Any:
+    pass
+
+
+@overload
+def load_yaml(filepath: str, loader_type: Optional[str] = None, logger: Optional[ContextAdapter] = None,
+              *, unserialize: Callable[[Any], T]) -> T:
+    pass
+
+
+def load_yaml(filepath: str, loader_type: Optional[str] = None, logger: Optional[ContextAdapter] = None,
+              unserialize: Optional[Callable[[Any], T]] = None) -> Any:
 
     """
     Load data stored in YAML file, and return their Python representation.
 
     :param text filepath: Path to a file. ``~`` or ``~<username>`` are expanded before using.
     :param str loader_type: type of YAML parser and loader. ``None`` or ``rt`` for round-trip (default),
         ``safe``, ``unsafe`` or ``base``.
     :param gluetool.log.ContextLogger logger: Logger used for logging.
+    :param callable unserialize: function to convert data into a specific structure, see e.g.
+        `create_cattrs_unserializer` function
     :rtype: object
     :returns: structures representing data in the file.
     :raises gluetool.glue.GlueError: if it was not possible to successfully load content of the file.
     """
 
     if not filepath:
         raise GlueError('File path is not valid: {}'.format(filepath))
@@ -1048,14 +1101,18 @@
 
     try:
         with open(real_filepath, 'r') as f:
             data = YAML(loader_type=loader_type).load(f)
 
         log_dict(logger.debug, "loaded YAML data from '{}'".format(filepath), data)
 
+        if unserialize:
+            structure = unserialize(data)
+            logger.debug('converted loaded YAML data into a structure: {}'.format(str(structure)))
+            return structure
         return data
 
     except ruamel.yaml.error.YAMLError as e:
         raise GlueError("Unable to load YAML file '{}': {}".format(filepath, e)) from e
 
 
 def dump_yaml(data: Any, filepath: str, logger: Optional[ContextAdapter] = None) -> None:
@@ -1444,15 +1501,30 @@
 
                     converter = spices[spice](converter)
 
                 compiled_chains.append(converter)
 
             self._compiled_map.append((compiled_pattern, compiled_chains))
 
-    def match(self, s: str, multiple: bool = False) -> Union[str, List[str]]:
+    # Using noqa F811 because flake8 doesn't like overloading methods
+    @overload  # noqa F811
+    def match(self, s: str, multiple: Literal[False] = False) -> str:  # noqa F811s
+        pass
+
+    @overload  # noqa F811s
+    def match(self, s: str, *, multiple: Literal[True]) -> List[str]:  # noqa F811s
+        pass
+
+    # This 3rd overload looks redundand (direct copy of the actual method definition). But without it, mypy would
+    # complain: 'No overload variant of "match" of "PatternMap" matches argument types "str", "bool"  [call-overload]'
+    @overload  # noqa F811s
+    def match(self, s: str, multiple: bool = False) -> Union[str, List[str]]:  # noqa F811s
+        pass
+
+    def match(self, s: str, multiple: bool = False) -> Union[str, List[str]]:  # noqa F811s
 
         """
         Try to match ``s`` by the map. If the match is found - the first one wins - then its
         conversions are applied to the ``s``.
 
         There can be multiple conversions for a pattern, by default only the product of
         the first one is returned. If ``multiple`` is set to ``True``, list of all products
```

### Comparing `gluetool-2.3/gluetool_modules/bash_completion.py` & `gluetool-2.4/gluetool_modules/bash_completion.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool_modules/dep_list.py` & `gluetool-2.4/gluetool_modules/dep_list.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/gluetool_modules/yaml_pipeline.py` & `gluetool-2.4/gluetool_modules/yaml_pipeline.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.3/pyproject.toml` & `gluetool-2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gluetool"
-version = "2.3"
+version = "2.4"
 description = "Python framework for constructing command-line pipelines."
 authors = [
   "Milos Prchlik <mprchlik@redhat.com>",
   "Miroslav Vadkerti <mvadkert@redhat.com>",
   "Martin Kluson <mkluson@redhat.com>",
   "Ondrej Ptak <optak@redhat.com>",
   "Evgeny Fedin <efedin@redhat.com>",
@@ -65,17 +65,18 @@
 # While *mypy* is a tool to check type annotations, *mypy-extensions* is a package that brings extensions
 # to the standard typing module - therefore it is not a developer dependency, as it is needed by types
 # depending on extended argument annotations.
 mypy-extensions = "*"
 zipp = "*"
 packaging = "*"
 MarkupSafe = "^2.0.0"
+attrs = "^22.2.0"
+cattrs = "^22.2.0"
 
 [tool.poetry.dev-dependencies]
-attrs = "*"
 # flake8 5 introduced a bug https://github.com/tholo/pytest-flake8/issues/87
 flake8 = "<5.0.0"
 lazy-object_proxy = "*"
 hypothesis = "*"
 importlib-metadata = "*"
 mypy = "*"
 pylint = "*"
```

### Comparing `gluetool-2.3/setup.py` & `gluetool-2.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,17 @@
                     'assets/parse_config/configroota/config/*',
                     'assets/parse_config/configrootb/config/*']}
 
 install_requires = \
 ['Jinja2>=3.0.0,<4.0.0',
  'MarkupSafe>=2.0.0,<3.0.0',
  'Sphinx>=5.0.0,<6.0.0',
+ 'attrs>=22.2.0,<23.0.0',
  'beautifulsoup4',
+ 'cattrs>=22.2.0,<23.0.0',
  'colorama',
  'configparser',
  'docutils',
  'lxml',
  'mock',
  'mypy-extensions',
  'packaging',
@@ -38,15 +40,15 @@
                       'gluetool_modules.bash_completion:BashCompletion',
                       '.dep_list = gluetool_modules.dep_list:DepList',
                       '.yaml_pipeline = '
                       'gluetool_modules.yaml_pipeline:YAMLPipeline']}
 
 setup_kwargs = {
     'name': 'gluetool',
-    'version': '2.3',
+    'version': '2.4',
     'description': 'Python framework for constructing command-line pipelines.',
     'long_description': 'gluetool - A tool for gluing together one-file python modules in a sequential command-line pipeline\n---------------------------------------------------------------------------------------------------\n\n``gluetool`` is a command line centric generic framework useable for glueing modules into pipeline\n\n\n.. image:: https://travis-ci.org/gluetool/gluetool.svg?branch=master\n    :target: https://travis-ci.org/gluetool/gluetool\n\n.. image:: https://codecov.io/gh/gluetool/gluetool/branch/master/graph/badge.svg\n     :target: https://codecov.io/gh/gluetool/gluetool\n     :alt: Code coverage\n\n.. image:: https://requires.io/github/gluetool/gluetool/requirements.svg?branch=master\n     :target: https://requires.io/github/gluetool/gluetool/requirements/?branch=master\n     :alt: Requirements Status\n\n.. image:: https://readthedocs.org/projects/gluetool/badge/?version=latest\n     :target: http://gluetool.readthedocs.io/en/latest/?badge=latest\n     :alt: Documentation Status\n\n\nDocumentation\n-------------\n\nFor more information see documentation:\n\nhttp://gluetool.readthedocs.io/\n',
     'author': 'Milos Prchlik',
     'author_email': 'mprchlik@redhat.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gluetool.readthedocs.org/',
```

### Comparing `gluetool-2.3/PKG-INFO` & `gluetool-2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluetool
-Version: 2.3
+Version: 2.4
 Summary: Python framework for constructing command-line pipelines.
 Home-page: https://gluetool.readthedocs.org/
 License: BSD
 Author: Milos Prchlik
 Author-email: mprchlik@redhat.com
 Requires-Python: >=3.7.2,<3.10
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Utilities
 Requires-Dist: Jinja2 (>=3.0.0,<4.0.0)
 Requires-Dist: MarkupSafe (>=2.0.0,<3.0.0)
 Requires-Dist: Sphinx (>=5.0.0,<6.0.0)
+Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: beautifulsoup4
+Requires-Dist: cattrs (>=22.2.0,<23.0.0)
 Requires-Dist: colorama
 Requires-Dist: configparser
 Requires-Dist: docutils
 Requires-Dist: lxml
 Requires-Dist: mock
 Requires-Dist: mypy-extensions
 Requires-Dist: packaging
```

