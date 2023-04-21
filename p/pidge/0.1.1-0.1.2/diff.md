# Comparing `tmp/pidge-0.1.1.tar.gz` & `tmp/pidge-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pidge-0.1.1.tar", max compression
+gzip compressed data, was "pidge-0.1.2.tar", max compression
```

## Comparing `pidge-0.1.1.tar` & `pidge-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,28 @@
--rw-r--r--   0        0        0     1070 2023-04-01 16:29:20.717592 pidge-0.1.1/LICENSE
--rw-r--r--   0        0        0     2926 2023-04-05 09:05:43.159458 pidge-0.1.1/README.md
--rw-r--r--   0        0        0       38 2023-04-01 16:29:20.717592 pidge-0.1.1/pidge/__init__.py
--rw-r--r--   0        0        0       65 2023-04-01 16:29:20.717592 pidge-0.1.1/pidge/__main__.py
--rw-r--r--   0        0        0     1974 2023-04-01 16:29:20.717592 pidge-0.1.1/pidge/core.py
--rw-r--r--   0        0        0      188 2023-03-30 16:12:14.803646 pidge-0.1.1/pidge/examples.py
--rw-r--r--   0        0        0      571 2023-04-04 21:00:19.063856 pidge-0.1.1/pidge/main.py
--rw-r--r--   0        0        0    13884 2023-04-01 16:29:20.717592 pidge-0.1.1/pidge/sample_data/fake_expenses.csv
--rw-r--r--   0        0        0        0 2023-03-30 16:12:14.803646 pidge-0.1.1/pidge/tests/__init__.py
--rw-r--r--   0        0        0       44 2023-03-30 16:12:14.803646 pidge-0.1.1/pidge/tests/conftest.py
--rw-r--r--   0        0        0       81 2023-03-30 16:12:14.803646 pidge-0.1.1/pidge/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      905 2023-03-30 16:12:14.803646 pidge-0.1.1/pidge/tests/fixtures/data.py
--rw-r--r--   0        0        0     1076 2023-04-01 16:29:20.717592 pidge-0.1.1/pidge/tests/fixtures/rules.py
--rw-r--r--   0        0        0     3319 2023-04-01 16:29:20.717592 pidge-0.1.1/pidge/tests/test_core.py
--rw-r--r--   0        0        0      185 2023-04-01 16:29:20.717592 pidge-0.1.1/pidge/tests/test_examples.py
--rw-r--r--   0        0        0       59 2023-04-01 16:29:20.717592 pidge-0.1.1/pidge/tests/test_main.py
--rw-r--r--   0        0        0     3049 2023-04-04 18:02:59.263856 pidge-0.1.1/pidge/tests/test_ui.py
--rw-r--r--   0        0        0     9120 2023-04-04 21:00:19.063856 pidge-0.1.1/pidge/ui.py
--rw-r--r--   0        0        0     6992 2023-04-04 21:00:19.063856 pidge-0.1.1/pidge/web_ui_template.html
--rw-r--r--   0        0        0      638 2023-04-05 09:07:19.729458 pidge-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3770 1970-01-01 00:00:00.000000 pidge-0.1.1/setup.py
--rw-r--r--   0        0        0     3460 1970-01-01 00:00:00.000000 pidge-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-01 16:29:20.717592 pidge-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2939 2023-04-21 04:17:16.768589 pidge-0.1.2/README.md
+-rw-r--r--   0        0        0       38 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/__main__.py
+-rw-r--r--   0        0        0     1974 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/core.py
+-rw-r--r--   0        0        0      188 2023-03-30 16:12:14.803646 pidge-0.1.2/pidge/examples.py
+-rw-r--r--   0        0        0      783 2023-04-16 20:50:02.091384 pidge-0.1.2/pidge/main.py
+-rw-r--r--   0        0        0    13884 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/sample_data/fake_expenses.csv
+-rw-r--r--   0        0        0        0 2023-03-30 16:12:14.803646 pidge-0.1.2/pidge/tests/__init__.py
+-rw-r--r--   0        0        0       44 2023-03-30 16:12:14.803646 pidge-0.1.2/pidge/tests/conftest.py
+-rw-r--r--   0        0        0      123 2023-04-15 17:05:58.566718 pidge-0.1.2/pidge/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      937 2023-04-15 17:05:58.566718 pidge-0.1.2/pidge/tests/fixtures/data.py
+-rw-r--r--   0        0        0      366 2023-04-15 17:05:58.566718 pidge-0.1.2/pidge/tests/fixtures/mapper.py
+-rw-r--r--   0        0        0     1076 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/tests/fixtures/rules.py
+-rw-r--r--   0        0        0     3319 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/tests/test_core.py
+-rw-r--r--   0        0        0      185 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/tests/test_examples.py
+-rw-r--r--   0        0        0       59 2023-04-01 16:29:20.717592 pidge-0.1.2/pidge/tests/test_main.py
+-rw-r--r--   0        0        0     2954 2023-04-15 17:05:58.566718 pidge-0.1.2/pidge/tests/test_mapper.py
+-rw-r--r--   0        0        0     3946 2023-04-16 20:50:02.091384 pidge-0.1.2/pidge/tests/test_ui.py
+-rw-r--r--   0        0        0      114 2023-04-15 17:05:58.566718 pidge-0.1.2/pidge/ui/__init__.py
+-rw-r--r--   0        0        0      859 2023-04-16 20:50:02.091384 pidge-0.1.2/pidge/ui/assets/favicon-16x16.png
+-rw-r--r--   0        0        0     2209 2023-04-16 20:50:02.091384 pidge-0.1.2/pidge/ui/css/webui.css
+-rw-r--r--   0        0        0     3256 2023-04-15 17:05:58.566718 pidge-0.1.2/pidge/ui/mapper.py
+-rw-r--r--   0        0        0     7426 2023-04-21 04:32:42.658589 pidge-0.1.2/pidge/ui/ui.py
+-rw-r--r--   0        0        0     6014 2023-04-16 20:50:02.091384 pidge-0.1.2/pidge/ui/web_ui_template.html
+-rw-r--r--   0        0        0      638 2023-04-21 04:33:01.058589 pidge-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3832 1970-01-01 00:00:00.000000 pidge-0.1.2/setup.py
+-rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 pidge-0.1.2/PKG-INFO
```

### Comparing `pidge-0.1.1/LICENSE` & `pidge-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pidge-0.1.1/README.md` & `pidge-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 1. Launch the UI in a notebook
 
     ```python
     from pidge import pidge_ui
     import panel as pn
 
-    pn.extensions('tabulator')
+    pn.extensions('tabulator','jsoneditor')
 
     pidge_ui(my_input_dataframe)
     ```
 
 1. Create and export a mapping named `pidge_mapping.json`
 
 1. In your data pipeline import `pidge` and apply the mapping
```

### Comparing `pidge-0.1.1/pidge/core.py` & `pidge-0.1.2/pidge/core.py`

 * *Files identical despite different names*

### Comparing `pidge-0.1.1/pidge/sample_data/fake_expenses.csv` & `pidge-0.1.2/pidge/sample_data/fake_expenses.csv`

 * *Files identical despite different names*

### Comparing `pidge-0.1.1/pidge/tests/fixtures/rules.py` & `pidge-0.1.2/pidge/tests/fixtures/rules.py`

 * *Files identical despite different names*

### Comparing `pidge-0.1.1/pidge/tests/test_core.py` & `pidge-0.1.2/pidge/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pidge-0.1.1/pidge/tests/test_ui.py` & `pidge-0.1.2/pidge/tests/test_mapper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,51 @@
-import panel as pn
-import pytest
+from contextlib import contextmanager
 
-from pidge.ui import PidgeMapper, create_panel, create_web_ui, insert_panel_in_template
+from pidge.ui.mapper import PidgeMapper
 
 
-@pytest.fixture
-def mapper(raw_shops, multiple_rules):
-    return PidgeMapper(raw_shops, multiple_rules)
+@contextmanager
+def assert_value_changed_once(p, name):
+    assertion_state = {"change_counter": 0}
 
+    def inc(*args, **kwargs):
+        assertion_state["change_counter"] += 1
 
-@pytest.fixture
-def empty_mapper(raw_shops, multiple_rules):
-    empty_expense_rule = {"source": "shop_raw", "target": "expense_type", "rules": {}}
-    return PidgeMapper(raw_shops, empty_expense_rule)
+    p.param.watch_values(inc, [name])
+
+    yield
+    assert_error = "Value did not change exactly once"
+
+    assert assertion_state["change_counter"] == 1, assert_error
 
 
 def test_mapper_initilization(mapper):
-    assert hasattr(mapper, "_mapped_data")
-    assert "shop" in mapper._mapped_data
-    assert hasattr(mapper, "_gap_summary")
-    assert "Edeka Bockenheim" in mapper._gap_summary.index
-    assert hasattr(mapper, "_target_summary")
-    assert "EDEKA" not in mapper._target_summary.index
-    assert "ALDI" in mapper._target_summary.index
-    assert "REWE" in mapper._target_summary.index
-    assert mapper.gap_view is None
-    assert mapper.target_view is None
+    assert hasattr(mapper, "mapped_data")
+    assert "shop" in mapper.mapped_data
+    assert hasattr(mapper, "gap_summary")
+    assert "Edeka Bockenheim" in mapper.gap_summary.index
+    assert hasattr(mapper, "target_summary")
+    assert "EDEKA" not in mapper.target_summary.index
+    assert "ALDI" in mapper.target_summary.index
+    assert "REWE" in mapper.target_summary.index
+    assert "pidge_version" in mapper.mapping_rule
+
+
+def test_pidge_version_on_rule_reset(mapper):
+    assert "pidge_version" in mapper.mapping_rule
+    mapper.reset_rule()
+    assert "pidge_version" in mapper.mapping_rule
 
 
 def test_mapper_insert(mapper):
     mapper.category = "EDEKA"
     mapper.pattern = "EDEKA"
     mapper.insert(mapper)
-    assert "Edeka Bockenheim" not in mapper._gap_summary.index
-    assert "EDEKA" in mapper._target_summary.index
+    assert "Edeka Bockenheim" not in mapper.gap_summary.index
+    assert "EDEKA" in mapper.target_summary.index
 
 
 def test_multi_insert(empty_mapper):
     empty_mapper.category = "Supermarket"
     empty_mapper.pattern = "EDEKA"
     PidgeMapper.insert(empty_mapper)
 
@@ -49,44 +57,42 @@
 
     # allow multiple inserts
     empty_mapper.category = "Supermarket"
     empty_mapper.pattern = "REWE"
     PidgeMapper.insert(empty_mapper)
 
     assert len(empty_mapper.mapping_rule["rules"]["Supermarket"]) == 2
-    assert not empty_mapper._gap_summary.index.str.contains("Edeka", case=False).any()
-    assert not empty_mapper._gap_summary.index.str.contains("Rewe", case=False).any()
-    assert "Supermarket" in empty_mapper._target_summary.index
-
-
-def test_views(mapper):
-    assert isinstance(mapper.view_gaps, pn.widgets.Tabulator)
-    assert isinstance(mapper.gap_view, pn.widgets.Tabulator)
-    assert isinstance(mapper.view_targets, pn.widgets.Tabulator)
-    assert isinstance(mapper.target_view, pn.widgets.Tabulator)
-    json_widget = mapper.view_rule()
-    assert isinstance(json_widget, pn.pane.JSON)
-    assert json_widget.object == mapper.mapping_rule_json
+    assert not empty_mapper.gap_summary.index.str.contains("Edeka", case=False).any()
+    assert not empty_mapper.gap_summary.index.str.contains("Rewe", case=False).any()
+    assert "Supermarket" in empty_mapper.target_summary.index
 
-    assert mapper.view_gaps.value.equals(mapper._gap_summary)
-    assert mapper.view_targets.value.equals(mapper._target_summary)
+
+def test_insert_triggers_gap_updated(mapper):
     mapper.category = "EDEKA"
     mapper.pattern = "EDEKA"
-    mapper.insert(mapper)
 
-    assert mapper.view_gaps.value.equals(mapper._gap_summary)
-    assert mapper.view_targets.value.equals(mapper._target_summary)
+    with assert_value_changed_once(mapper, "gap_summary_updated"):
+        mapper.insert(mapper)
+
 
+def test_insert_triggers_target_updated(mapper):
+    mapper.category = "EDEKA"
+    mapper.pattern = "EDEKA"
 
-def test_create_panel_smoke(mapper):
-    panel = create_panel(mapper)
-    assert isinstance(panel, pn.Tabs)
+    with assert_value_changed_once(mapper, "target_summary_updated"):
+        mapper.insert(mapper)
 
-    create_panel(mapper, width=500)
 
+def test_insert_triggers_mapped_data_updated(mapper):
+    mapper.category = "EDEKA"
+    mapper.pattern = "EDEKA"
 
-def test_insert_panel_in_template_smoke():
-    insert_panel_in_template(pn.Row())
+    with assert_value_changed_once(mapper, "mapped_data_updated"):
+        mapper.insert(mapper)
 
 
-def test_create_web_ui_smoke(mapper):
-    create_web_ui(mapper)
+def test_insert_triggers_mapping_rule_updated(mapper):
+    mapper.category = "EDEKA"
+    mapper.pattern = "EDEKA"
+
+    with assert_value_changed_once(mapper, "mapping_updated"):
+        mapper.insert(mapper)
```

### Comparing `pidge-0.1.1/pidge/web_ui_template.html` & `pidge-0.1.2/pidge/ui/web_ui_template.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,125 +1,49 @@
 {% extends base %}
+{% block title %}pidge web ui{% endblock %}
 {% block preamble %}
 <meta name="viewport" content="width=device-width, initial-scale=1" />
 {% endblock %}
 {% block postamble %}
-<style>
-  * {
-  margin: 0;
-  }
-  body {
-  background-color: #F0FFFF;
-  }
-  p {
-  margin: 0.5em 0 0.5em 0;
-  }
-  h1,h2,h3 {
-  margin: 1.5em 0 0.7em 0;
-  }
-  header {
-  display: block;
-  position: fixed;
-  top: 0;
-  left: 0;
-  width: 100%;
-  background-color: #90EE90;
-  padding: 10px;
-  z-index: 10;
-  }
-  header > nav a{
-  color: #000;
-  text-decoration: none;
-  }
-  header > nav > ul {
-  display: inline;
-  padding: 0;
-  }
-  header > nav > ul > li {
-  display: inline-block;
-  list-style: none;
-  margin: 0 5px 0 5px;
-  }
-  #leftmenu {
-  padding-top: 3em;
-  display: none;
-  }
-  #main {
-  padding-top: 3em;
-  float: left;
-  width: 75%;
-  margin-left: auto;
-  margin-right: auto;
-  padding-left: 10px;
-  padding-right: 10px;
-  }
-  aside > nav a{
-  color: #000;
-  text-decoration: none;
-  font-weight: bold;
-  }
-  aside > nav > ul {
-  list-style: none;
-  margin: 0;
-  padding : 1em 0 0 0;
-  }
-  aside > nav > ul >li {
-  padding : 0 0 0.8em 1.5em ;
-  }
-  main {
-  display: block;
-  padding-bottom: 3em;
-  min-height: 85%;
-  }
-  @media only screen and (min-width: 768px) {
-  #leftmenu {
-  display: unset;
-  float: left;
-  width: 20%;
-  height: 100%;
-  position: fixed;
-  background-color: #D3D3D3;
-  }
-  #main {
-  float: right;
-  }
-  }
-</style>
+<link rel="stylesheet" href="/css/webui.css">
+<link rel="icon" type="image/png" sizes="16x16"  href="/assets/favicon-16x16.png">
 {% endblock %}
 <!-- goes in body -->
 {% block contents %}
 <header>
   <nav>
     <ul>
       <li>
         <a href="https://github.com/KonradUdoHannes/pidge" target="_blank">pidge on Github</a>
       </li>
       <li><a href="https://pypi.org/project/pidge/" target="_blank">pidge on PyPI</a></li>
     </ul>
   </nav>
 </header>
-<main>
-  <aside id="leftmenu">
+<main class="row">
+  <aside id="leftmenu" class="column leftmenu large-1-2 no-scroll">
     <nav>
       <ul>
         <li><a href="#pidge-ui">pidge UI</a></li>
         <li><a href="#ui-summary">UI summary</a></li>
         <li><a href="#what-is-pidge">What is pidge?</a></li>
         <li><a href="#project-status">Help with the MVP</a></li>
         <li><a href="#example-data">Example Data</a></li>
         <li><a href="#ui-usage">UI Usage</a></li>
       </ul>
     </nav>
   </aside>
-  <div id="main">
-    <h2 id="pidge-ui" class="center">pidge UI</h2>
-    <div class="center">
-      {{ embed(roots.DASHBOARD) }}
+  <div id="main" class="column limited small-12 large-2-12">
+    <div id="ui">
+      <h2 id="pidge-ui">pidge UI</h2>
+      <div>
+        {{ embed(roots.DASHBOARD) }}
+      </div>
     </div>
-    <article class="center">
+    <article>
       <h2 id="ui-summary">What does the UI show?</h2>
       <p>
         This is the pidge UI with example data that takes the table found under
         <strong> Input Data </strong> and maps it to the table found under
         <strong> Mapped Data </strong>. In this example the column <strong> recipient</strong> is
         mapped to the column <strong> expense_category </strong>. A few mappings are already part of the example
         data and new mappings can be added via the UI. For details regrding the mapping logic see
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
-{% extends base %} {% block preamble %}
+{% extends base %} {% block title %}pidge web ui{% endblock %} {% block
+preamble %}
  {% endblock %} {% block postamble %}
+
  {% endblock %}  {% block contents %}
     * pidge_on_Github
     * pidge_on_PyPI
 
     * pidge_UI
     * UI_summary
     * What_is_pidge?
```

### Comparing `pidge-0.1.1/pyproject.toml` & `pidge-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.2.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pidge"
-version = "0.1.1"
+version = "0.1.2"
 description = "pidge helps with the creation of mappings for tabular string data"
 readme = "README.md"
 authors = ["Konrad Wölms <konrad.woelms@gmail.com>",]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 panel = "^0.14.4"
```

### Comparing `pidge-0.1.1/setup.py` & `pidge-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['pidge', 'pidge.tests', 'pidge.tests.fixtures']
+['pidge', 'pidge.tests', 'pidge.tests.fixtures', 'pidge.ui']
 
 package_data = \
-{'': ['*'], 'pidge': ['sample_data/fake_expenses.csv']}
+{'': ['*'],
+ 'pidge': ['sample_data/fake_expenses.csv'],
+ 'pidge.ui': ['assets/*', 'css/*']}
 
 install_requires = \
 ['pandas>=1.5.3,<2.0.0', 'panel>=0.14.4,<0.15.0']
 
 setup_kwargs = {
     'name': 'pidge',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'pidge helps with the creation of mappings for tabular string data',
-    'long_description': "# pidge\n\npidge helps with the creation of mappings for tabular string data. The primary use cases for\nthis are data cleaning and data categorization.\n\npidge consists out of two parts:\n\n1. An interactive UI to help with the creation of mappings and assessing their completeness\n2. Library functionality to apply mappings inside of data pipelines, after they have been exported from the UI\n\n\n## Usage\n\n1. install `pidge`\n\n        pip install pidge\n\n1. Launch the UI in a notebook\n\n    ```python\n    from pidge import pidge_ui\n    import panel as pn\n\n    pn.extensions('tabulator')\n\n    pidge_ui(my_input_dataframe)\n    ```\n\n1. Create and export a mapping named `pidge_mapping.json`\n\n1. In your data pipeline import `pidge` and apply the mapping\n\n    ```python\n    from pidge import pidge\n\n    transformed_data = pidge(my_input_dataframe,rule_file= 'pidge_mapping.json')\n    ```\n\n### The web-ui outside of Jupyter\n\nPidge can also run the UI as a standalone web server outside of jupyter, using the command.\n\n> python -m pidge\n\nThis starts up the UI in a local web server, which is primarily intended for illustration purposes.\nTherefore it starts up with example data already loaded. However new data can be loaded and the\npredefined rules can easily be reset. The main limitation at this moment, however, is the\nconstraint on the upload format for data. It only supports `.csv` and reads it with default\n`pandas.read_csv` settings.\n\n## Mapping Logic\n\nPidge mappings map a source string column to a newly created target string column. The logic can\nbe broken down as follows.\n\n1. One defines a possible value, a category, for the target column.\n1. One associates one or more patterns with that category.\n1. When a value of the source column matches one of the category's patterns, that category is chosen.\n1. Pattern matching checks whether the pattern is part of the source string. It is case insensitive\n    and allows for regular expressions.\n1. This is repeated for as many categories as desired.\n\n\n## Contribution\n\nPidge is in an early MVP stage. At this stage the following is particularly appreciated\n\n1. Any feedback regarding, bugs, issues usability feature requests etc. Ideally this can be done directly\n    as github issues.\n1. Any sharing of the project to potentially help with the previous point.\n\n## Known Limitations\n\nThere are a few known limitations particularly due to the MVP stage of the project. These\nwill be prioritized according to feedback and general usage of the project.\n\n- Mapping is not optimized for speed at all and might slow down for large dataframes\n- Patterns do not check for multiple inconsistent matches and simply the first applicable pattern\n    is chosen\n- the web-ui does only support small file uploads (around < 10Mb).\n- file uploads can only read in the data with `pandas.read_csv` default settings\n- The rule name used for the .json export can currently not be changed in the UI.\n",
+    'long_description': "# pidge\n\npidge helps with the creation of mappings for tabular string data. The primary use cases for\nthis are data cleaning and data categorization.\n\npidge consists out of two parts:\n\n1. An interactive UI to help with the creation of mappings and assessing their completeness\n2. Library functionality to apply mappings inside of data pipelines, after they have been exported from the UI\n\n\n## Usage\n\n1. install `pidge`\n\n        pip install pidge\n\n1. Launch the UI in a notebook\n\n    ```python\n    from pidge import pidge_ui\n    import panel as pn\n\n    pn.extensions('tabulator','jsoneditor')\n\n    pidge_ui(my_input_dataframe)\n    ```\n\n1. Create and export a mapping named `pidge_mapping.json`\n\n1. In your data pipeline import `pidge` and apply the mapping\n\n    ```python\n    from pidge import pidge\n\n    transformed_data = pidge(my_input_dataframe,rule_file= 'pidge_mapping.json')\n    ```\n\n### The web-ui outside of Jupyter\n\nPidge can also run the UI as a standalone web server outside of jupyter, using the command.\n\n> python -m pidge\n\nThis starts up the UI in a local web server, which is primarily intended for illustration purposes.\nTherefore it starts up with example data already loaded. However new data can be loaded and the\npredefined rules can easily be reset. The main limitation at this moment, however, is the\nconstraint on the upload format for data. It only supports `.csv` and reads it with default\n`pandas.read_csv` settings.\n\n## Mapping Logic\n\nPidge mappings map a source string column to a newly created target string column. The logic can\nbe broken down as follows.\n\n1. One defines a possible value, a category, for the target column.\n1. One associates one or more patterns with that category.\n1. When a value of the source column matches one of the category's patterns, that category is chosen.\n1. Pattern matching checks whether the pattern is part of the source string. It is case insensitive\n    and allows for regular expressions.\n1. This is repeated for as many categories as desired.\n\n\n## Contribution\n\nPidge is in an early MVP stage. At this stage the following is particularly appreciated\n\n1. Any feedback regarding, bugs, issues usability feature requests etc. Ideally this can be done directly\n    as github issues.\n1. Any sharing of the project to potentially help with the previous point.\n\n## Known Limitations\n\nThere are a few known limitations particularly due to the MVP stage of the project. These\nwill be prioritized according to feedback and general usage of the project.\n\n- Mapping is not optimized for speed at all and might slow down for large dataframes\n- Patterns do not check for multiple inconsistent matches and simply the first applicable pattern\n    is chosen\n- the web-ui does only support small file uploads (around < 10Mb).\n- file uploads can only read in the data with `pandas.read_csv` default settings\n- The rule name used for the .json export can currently not be changed in the UI.\n",
     'author': 'Konrad Wölms',
     'author_email': 'konrad.woelms@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pidge-0.1.1/PKG-INFO` & `pidge-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pidge
-Version: 0.1.1
+Version: 0.1.2
 Summary: pidge helps with the creation of mappings for tabular string data
 Author: Konrad Wölms
 Author-email: konrad.woelms@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -32,15 +32,15 @@
 
 1. Launch the UI in a notebook
 
     ```python
     from pidge import pidge_ui
     import panel as pn
 
-    pn.extensions('tabulator')
+    pn.extensions('tabulator','jsoneditor')
 
     pidge_ui(my_input_dataframe)
     ```
 
 1. Create and export a mapping named `pidge_mapping.json`
 
 1. In your data pipeline import `pidge` and apply the mapping
```

