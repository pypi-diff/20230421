# Comparing `tmp/acdh-django-charts-0.5.3.tar.gz` & `tmp/acdh-django-charts-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\acdh-django-charts-0.5.3.tar", last modified: Tue Feb 12 10:07:08 2019, max compression
+gzip compressed data, was "acdh-django-charts-0.6.0.tar", last modified: Fri Apr 21 15:21:26 2023, max compression
```

## Comparing `acdh-django-charts-0.5.3.tar` & `acdh-django-charts-0.6.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxrwx   0        0        0        0 2019-02-12 10:07:08.000000 acdh-django-charts-0.5.3/
--rw-rw-rw-   0        0        0      178 2018-06-01 07:13:21.000000 acdh-django-charts-0.5.3/AUTHORS.rst
--rw-rw-rw-   0        0        0     3382 2018-06-01 09:00:11.000000 acdh-django-charts-0.5.3/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1122 2019-02-12 10:05:54.000000 acdh-django-charts-0.5.3/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2018-06-01 07:13:21.000000 acdh-django-charts-0.5.3/LICENSE
--rw-rw-rw-   0        0        0      180 2018-06-01 07:13:21.000000 acdh-django-charts-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6813 2019-02-12 10:07:08.000000 acdh-django-charts-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     3468 2018-12-05 13:04:23.000000 acdh-django-charts-0.5.3/README.rst
-drwxrwxrwx   0        0        0        0 2019-02-12 10:07:08.000000 acdh-django-charts-0.5.3/acdh_django_charts.egg-info/
--rw-rw-rw-   0        0        0     6813 2019-02-12 10:07:06.000000 acdh-django-charts-0.5.3/acdh_django_charts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1087 2019-02-12 10:07:06.000000 acdh-django-charts-0.5.3/acdh_django_charts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-02-12 10:07:06.000000 acdh-django-charts-0.5.3/acdh_django_charts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2018-06-01 09:07:51.000000 acdh-django-charts-0.5.3/acdh_django_charts.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2019-02-12 10:07:06.000000 acdh-django-charts-0.5.3/acdh_django_charts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2019-02-12 10:07:08.000000 acdh-django-charts-0.5.3/charts/
--rw-rw-rw-   0        0        0       23 2019-02-12 10:06:06.000000 acdh-django-charts-0.5.3/charts/__init__.py
--rw-rw-rw-   0        0        0      318 2018-12-18 15:31:25.000000 acdh-django-charts-0.5.3/charts/admin.py
--rw-rw-rw-   0        0        0       87 2018-11-20 13:21:36.000000 acdh-django-charts-0.5.3/charts/apps.py
-drwxrwxrwx   0        0        0        0 2019-02-12 10:07:08.000000 acdh-django-charts-0.5.3/charts/management/
-drwxrwxrwx   0        0        0        0 2019-02-12 10:07:08.000000 acdh-django-charts-0.5.3/charts/management/commands/
--rw-rw-rw-   0        0        0        0 2018-12-05 11:49:10.000000 acdh-django-charts-0.5.3/charts/management/commands/__init__.py
--rw-rw-rw-   0        0        0      576 2018-12-05 12:53:25.000000 acdh-django-charts-0.5.3/charts/management/commands/create_charts.py
--rw-rw-rw-   0        0        0      811 2018-12-05 11:59:06.000000 acdh-django-charts-0.5.3/charts/management/commands/create_charttypes.py
--rw-rw-rw-   0        0        0      451 2018-12-05 13:02:46.000000 acdh-django-charts-0.5.3/charts/management/commands/delete_charts.py
--rw-rw-rw-   0        0        0      436 2018-12-05 11:57:27.000000 acdh-django-charts-0.5.3/charts/management/commands/delete_charttypes.py
-drwxrwxrwx   0        0        0        0 2019-02-12 10:07:08.000000 acdh-django-charts-0.5.3/charts/migrations/
--rw-rw-rw-   0        0        0     1965 2018-11-20 13:21:36.000000 acdh-django-charts-0.5.3/charts/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      493 2018-11-20 13:21:36.000000 acdh-django-charts-0.5.3/charts/migrations/0002_chartconfig_app_name.py
--rw-rw-rw-   0        0        0        0 2018-11-20 13:21:36.000000 acdh-django-charts-0.5.3/charts/migrations/__init__.py
--rw-rw-rw-   0        0        0     1652 2018-11-20 13:21:36.000000 acdh-django-charts-0.5.3/charts/models.py
-drwxrwxrwx   0        0        0        0 2019-02-12 10:07:08.000000 acdh-django-charts-0.5.3/charts/templates/
-drwxrwxrwx   0        0        0        0 2019-02-12 10:07:08.000000 acdh-django-charts-0.5.3/charts/templates/charts/
--rw-rw-rw-   0        0        0      682 2018-11-20 13:21:36.000000 acdh-django-charts-0.5.3/charts/templates/charts/base.html
--rw-rw-rw-   0        0        0     1044 2018-12-10 09:19:43.000000 acdh-django-charts-0.5.3/charts/templates/charts/dynchart.html
--rw-rw-rw-   0        0        0     1469 2018-11-20 13:21:36.000000 acdh-django-charts-0.5.3/charts/templates/charts/select_chart.html
-drwxrwxrwx   0        0        0        0 2019-02-12 10:07:08.000000 acdh-django-charts-0.5.3/charts/templates/charts/tags/
--rw-rw-rw-   0        0        0     2100 2018-11-20 13:21:36.000000 acdh-django-charts-0.5.3/charts/templates/charts/tags/config_highcharts.html
--rw-rw-rw-   0        0        0      294 2018-11-20 13:21:36.000000 acdh-django-charts-0.5.3/charts/templates/charts/tags/load_highcharts_js.html
--rw-rw-rw-   0        0        0      635 2018-11-20 13:21:36.000000 acdh-django-charts-0.5.3/charts/templates/charts/tags/selector_dropdown.html
-drwxrwxrwx   0        0        0        0 2019-02-12 10:07:08.000000 acdh-django-charts-0.5.3/charts/templatetags/
--rw-rw-rw-   0        0        0       23 2018-11-20 13:21:36.000000 acdh-django-charts-0.5.3/charts/templatetags/__init__.py
--rw-rw-rw-   0        0        0      558 2018-11-20 13:21:36.000000 acdh-django-charts-0.5.3/charts/templatetags/charts_extras.py
--rw-rw-rw-   0        0        0      349 2018-11-20 13:21:36.000000 acdh-django-charts-0.5.3/charts/urls.py
--rw-rw-rw-   0        0        0     1572 2018-12-05 12:54:45.000000 acdh-django-charts-0.5.3/charts/utils.py
--rw-rw-rw-   0        0        0     4449 2019-02-12 10:04:30.000000 acdh-django-charts-0.5.3/charts/views.py
--rw-rw-rw-   0        0        0      340 2019-02-12 10:07:08.000000 acdh-django-charts-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     2292 2018-06-05 06:54:13.000000 acdh-django-charts-0.5.3/setup.py
+drwxrwxr-x   0 csae8092  (1000) csae8092  (1000)        0 2023-04-21 15:21:26.775175 acdh-django-charts-0.6.0/
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      165 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/AUTHORS.rst
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     3270 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/CONTRIBUTING.rst
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     1179 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/HISTORY.rst
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     1077 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/LICENSE
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      174 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/MANIFEST.in
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     5260 2023-04-21 15:21:26.775175 acdh-django-charts-0.6.0/PKG-INFO
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     3377 2023-04-21 15:21:10.000000 acdh-django-charts-0.6.0/README.rst
+drwxrwxr-x   0 csae8092  (1000) csae8092  (1000)        0 2023-04-21 15:21:26.763175 acdh-django-charts-0.6.0/acdh_django_charts.egg-info/
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     5260 2023-04-21 15:21:26.000000 acdh-django-charts-0.6.0/acdh_django_charts.egg-info/PKG-INFO
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     1108 2023-04-21 15:21:26.000000 acdh-django-charts-0.6.0/acdh_django_charts.egg-info/SOURCES.txt
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)        1 2023-04-21 15:21:26.000000 acdh-django-charts-0.6.0/acdh_django_charts.egg-info/dependency_links.txt
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)        1 2023-04-21 15:15:24.000000 acdh-django-charts-0.6.0/acdh_django_charts.egg-info/not-zip-safe
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)        7 2023-04-21 15:21:26.000000 acdh-django-charts-0.6.0/acdh_django_charts.egg-info/top_level.txt
+drwxrwxr-x   0 csae8092  (1000) csae8092  (1000)        0 2023-04-21 15:21:26.767175 acdh-django-charts-0.6.0/charts/
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)       22 2023-04-21 15:15:06.000000 acdh-django-charts-0.6.0/charts/__init__.py
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      318 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/admin.py
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      141 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/apps.py
+drwxrwxr-x   0 csae8092  (1000) csae8092  (1000)        0 2023-04-21 15:21:26.755175 acdh-django-charts-0.6.0/charts/management/
+drwxrwxr-x   0 csae8092  (1000) csae8092  (1000)        0 2023-04-21 15:21:26.767175 acdh-django-charts-0.6.0/charts/management/commands/
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)        0 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/management/commands/__init__.py
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      557 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/management/commands/create_charts.py
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      785 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/management/commands/create_charttypes.py
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      437 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/management/commands/delete_charts.py
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      422 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/management/commands/delete_charttypes.py
+drwxrwxr-x   0 csae8092  (1000) csae8092  (1000)        0 2023-04-21 15:21:26.771175 acdh-django-charts-0.6.0/charts/migrations/
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     1926 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/migrations/0001_initial.py
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      475 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/migrations/0002_chartconfig_app_name.py
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)        0 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/migrations/__init__.py
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     1652 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/models.py
+drwxrwxr-x   0 csae8092  (1000) csae8092  (1000)        0 2023-04-21 15:21:26.755175 acdh-django-charts-0.6.0/charts/templates/
+drwxrwxr-x   0 csae8092  (1000) csae8092  (1000)        0 2023-04-21 15:21:26.771175 acdh-django-charts-0.6.0/charts/templates/charts/
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      661 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/templates/charts/base.html
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     1004 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/templates/charts/dynchart.html
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     1417 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/templates/charts/select_chart.html
+drwxrwxr-x   0 csae8092  (1000) csae8092  (1000)        0 2023-04-21 15:21:26.771175 acdh-django-charts-0.6.0/charts/templates/charts/tags/
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     2035 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/templates/charts/tags/config_highcharts.html
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      290 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/templates/charts/tags/load_highcharts_js.html
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      620 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/templates/charts/tags/selector_dropdown.html
+drwxrwxr-x   0 csae8092  (1000) csae8092  (1000)        0 2023-04-21 15:21:26.775175 acdh-django-charts-0.6.0/charts/templatetags/
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)       22 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/templatetags/__init__.py
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      539 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/templatetags/charts_extras.py
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      337 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/urls.py
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     1529 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/utils.py
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     4319 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/charts/views.py
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      313 2023-04-21 15:21:26.775175 acdh-django-charts-0.6.0/setup.cfg
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)     2169 2023-04-21 15:19:58.000000 acdh-django-charts-0.6.0/setup.py
+drwxrwxr-x   0 csae8092  (1000) csae8092  (1000)        0 2023-04-21 15:21:26.775175 acdh-django-charts-0.6.0/tests/
+-rw-rw-r--   0 csae8092  (1000) csae8092  (1000)      347 2023-04-21 15:14:34.000000 acdh-django-charts-0.6.0/tests/test_models.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `acdh-django-charts-0.5.3/LICENSE` & `acdh-django-charts-0.6.0/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-
-MIT License
-
-Copyright (c) 2018, Peter Andorfer
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
-
-
+
+MIT License
+
+Copyright (c) 2018, Peter Andorfer
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
+
+
```

### Comparing `acdh-django-charts-0.5.3/README.rst` & `acdh-django-charts-0.6.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-=============================
-django_charts
-=============================
-
-.. image:: https://badge.fury.io/py/acdh-django-charts.svg
-    :target: https://badge.fury.io/py/acdh-django-charts
-
-.. image:: https://travis-ci.org/acdh-oeaw/acdh-django-charts.svg?branch=master
-    :target: https://travis-ci.org/acdh-oeaw/acdh-django-charts
-
-.. image:: https://codecov.io/gh/acdh-oeaw/acdh-django-charts/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/acdh-oeaw/acdh-django-charts
-
-An app to explore your data through charts based on Highcharts.js
-
-Documentation
--------------
-
-The full documentation is at https://acdh-django-charts.readthedocs.io.
-
-Quickstart
-----------
-
-Install django_charts::
-
-    pip install acdh-django-charts
-
-Add it to your `INSTALLED_APPS`:
-
-.. code-block:: python
-
-    INSTALLED_APPS = (
-        ...
-        'charts',
-        ...
-    )
-
-Add django_charts's URL patterns:
-
-.. code-block:: python
-
-    urlpatterns = [
-        ...
-        url(r'^charts/', include('charts.urls', namespace='charts')),
-        ...
-    ]
-
-By default the app's templates extend a base template `webpage/base.html`. To ovveride this, just define a `CHARTS_BASE_TEMPLATE` variable on your project's `settings.py` like e.g:
-
-.. code-block:: python
-
-    CHARTS_BASE_TEMPLATE = 'base.html'
-
-To link to the application's 'chart-selector-view' you can add something like the snippet below to your e.g. base-template:
-
-.. code-block:: html
-
-    <a href="{% url 'charts:chart_selector' %}">Charts</a>
-
-Configuration
-----
-
-To visualize any property of your model you have to pass in the models name (lowercase), the field-path (using django's lookup syntax `__` to follow foreign key and many2many relations) and the chart type (bar|line|pie) via keyword arguments to the `charts.views.DynChartView()`. In case those params are valid (i.d. the model and the lookup path acutally exist) the according chart should be drawn. But be aware that this only works if your project's `DEBUG` settings are set to `True`.
-As **recomended** alternative you should create `ChartConfig` objects for each property/model you'd like to explore via django admin-backend.
-
-management commands
-----
-
-The package ships with a management command to
-
-* create/delete chartconfig objects (Bar, Pie, Linecharts)
-
-.. code-block:: console
-
-    python manage.py create_charttypes
-
-.. code-block:: console
-
-    python manage.py delete_charttypes
-
-* create/delete ChartConfig objects per application
-
-.. code-block:: console
-
-    python manage.py create_charts <app_name>
-
-.. code-block:: console
-
-    python manage.py delete_charts <app_name>
-
-Build and publish
------
-
-.. code-block:: console
-
-    python setup.py sdist bdist_wheel
-    twine upload dist/*
-
-
-
-Features
---------
-
-* Visualizes aggregated values of your models as charts (pie/bar/line) using https://www.highcharts.com/
-* Charts can be configured via admin backend (see Configuration Section)
-
-Running Tests
--------------
-
-Does the code actually work?
-
-::
-
-    source <YOURVIRTUALENV>/bin/activate
-    (myenv) $ pip install tox
-    (myenv) $ tox
-
-Credits
--------
-
-Tools used in rendering this package:
-
-*  Cookiecutter_
-*  `cookiecutter-djangopackage`_
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
+=============================
+django_charts
+=============================
+
+.. image:: https://badge.fury.io/py/acdh-django-charts.svg
+    :target: https://badge.fury.io/py/acdh-django-charts
+
+.. image:: https://travis-ci.org/acdh-oeaw/acdh-django-charts.svg?branch=master
+    :target: https://travis-ci.org/acdh-oeaw/acdh-django-charts
+
+.. image:: https://codecov.io/gh/acdh-oeaw/acdh-django-charts/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/acdh-oeaw/acdh-django-charts
+
+An app to explore your data through charts based on Highcharts.js
+
+Documentation
+-------------
+
+The full documentation is at https://acdh-django-charts.readthedocs.io.
+
+Quickstart
+----------
+
+Install django_charts::
+
+    pip install acdh-django-charts
+
+Add it to your `INSTALLED_APPS`:
+
+.. code-block:: python
+
+    INSTALLED_APPS = (
+        ...
+        'charts',
+        ...
+    )
+
+Add django_charts's URL patterns:
+
+.. code-block:: python
+
+    urlpatterns = [
+        ...
+        url(r'^charts/', include('charts.urls', namespace='charts')),
+        ...
+    ]
+
+By default the app's templates extend a base template `webpage/base.html`. To ovveride this, just define a `CHARTS_BASE_TEMPLATE` variable on your project's `settings.py` like e.g:
+
+.. code-block:: python
+
+    CHARTS_BASE_TEMPLATE = 'base.html'
+
+To link to the application's 'chart-selector-view' you can add something like the snippet below to your e.g. base-template:
+
+.. code-block:: html
+
+    <a href="{% url 'charts:chart_selector' %}">Charts</a>
+
+Configuration
+-------------
+
+To visualize any property of your model you have to pass in the models name (lowercase), the field-path (using django's lookup syntax `__` to follow foreign key and many2many relations) and the chart type (bar|line|pie) via keyword arguments to the `charts.views.DynChartView()`. In case those params are valid (i.d. the model and the lookup path acutally exist) the according chart should be drawn. But be aware that this only works if your project's `DEBUG` settings are set to `True`.
+As **recomended** alternative you should create `ChartConfig` objects for each property/model you'd like to explore via django admin-backend.
+
+management commands
+-------------------
+
+The package ships with a management command to
+
+* create/delete chartconfig objects (Bar, Pie, Linecharts)
+
+.. code-block:: console
+
+    python manage.py create_charttypes
+
+.. code-block:: console
+
+    python manage.py delete_charttypes
+
+* create/delete ChartConfig objects per application
+
+.. code-block:: console
+
+    python manage.py create_charts <app_name>
+
+.. code-block:: console
+
+    python manage.py delete_charts <app_name>
+
+Build and publish
+-----------------
+
+.. code-block:: console
+
+    python setup.py sdist bdist_wheel
+    twine upload dist/*
+
+
+
+Features
+--------
+
+* Visualizes aggregated values of your models as charts (pie/bar/line) using https://www.highcharts.com/
+* Charts can be configured via admin backend (see Configuration Section)
+
+Running Tests
+-------------
+
+Does the code actually work?
+
+::
+
+    source <YOURVIRTUALENV>/bin/activate
+    (myenv) $ pip install tox
+    (myenv) $ tox
+
+Credits
+-------
+
+Tools used in rendering this package:
+
+*  Cookiecutter_
+*  `cookiecutter-djangopackage`_
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
```

#### html2text {}

```diff
@@ -12,30 +12,31 @@
 django_charts's URL patterns: .. code-block:: python urlpatterns = [ ... url
 (r'^charts/', include('charts.urls', namespace='charts')), ... ] By default the
 app's templates extend a base template `webpage/base.html`. To ovveride this,
 just define a `CHARTS_BASE_TEMPLATE` variable on your project's `settings.py`
 like e.g: .. code-block:: python CHARTS_BASE_TEMPLATE = 'base.html' To link to
 the application's 'chart-selector-view' you can add something like the snippet
 below to your e.g. base-template: .. code-block:: html Charts Configuration ---
-- To visualize any property of your model you have to pass in the models name
-(lowercase), the field-path (using django's lookup syntax `__` to follow
-foreign key and many2many relations) and the chart type (bar|line|pie) via
-keyword arguments to the `charts.views.DynChartView()`. In case those params
-are valid (i.d. the model and the lookup path acutally exist) the according
-chart should be drawn. But be aware that this only works if your project's
-`DEBUG` settings are set to `True`. As **recomended** alternative you should
-create `ChartConfig` objects for each property/model you'd like to explore via
-django admin-backend. management commands ---- The package ships with a
-management command to * create/delete chartconfig objects (Bar, Pie,
-Linecharts) .. code-block:: console python manage.py create_charttypes .. code-
-block:: console python manage.py delete_charttypes * create/delete ChartConfig
-objects per application .. code-block:: console python manage.py create_charts
-.. code-block:: console python manage.py delete_charts  Build and publish ----
-- .. code-block:: console python setup.py sdist bdist_wheel twine upload dist/
-* Features -------- * Visualizes aggregated values of your models as charts
-(pie/bar/line) using https://www.highcharts.com/ * Charts can be configured via
-admin backend (see Configuration Section) Running Tests ------------- Does the
-code actually work? :: source /bin/activate (myenv) $ pip install tox (myenv) $
-tox Credits ------- Tools used in rendering this package: * Cookiecutter_ *
-`cookiecutter-djangopackage`_ .. _Cookiecutter: https://github.com/audreyr/
-cookiecutter .. _`cookiecutter-djangopackage`: https://github.com/pydanny/
-cookiecutter-djangopackage
+---------- To visualize any property of your model you have to pass in the
+models name (lowercase), the field-path (using django's lookup syntax `__` to
+follow foreign key and many2many relations) and the chart type (bar|line|pie)
+via keyword arguments to the `charts.views.DynChartView()`. In case those
+params are valid (i.d. the model and the lookup path acutally exist) the
+according chart should be drawn. But be aware that this only works if your
+project's `DEBUG` settings are set to `True`. As **recomended** alternative you
+should create `ChartConfig` objects for each property/model you'd like to
+explore via django admin-backend. management commands ------------------- The
+package ships with a management command to * create/delete chartconfig objects
+(Bar, Pie, Linecharts) .. code-block:: console python manage.py
+create_charttypes .. code-block:: console python manage.py delete_charttypes *
+create/delete ChartConfig objects per application .. code-block:: console
+python manage.py create_charts  .. code-block:: console python manage.py
+delete_charts  Build and publish ----------------- .. code-block:: console
+python setup.py sdist bdist_wheel twine upload dist/* Features -------- *
+Visualizes aggregated values of your models as charts (pie/bar/line) using
+https://www.highcharts.com/ * Charts can be configured via admin backend (see
+Configuration Section) Running Tests ------------- Does the code actually work?
+:: source /bin/activate (myenv) $ pip install tox (myenv) $ tox Credits ------
+- Tools used in rendering this package: * Cookiecutter_ * `cookiecutter-
+djangopackage`_ .. _Cookiecutter: https://github.com/audreyr/cookiecutter ..
+_`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-
+djangopackage
```

### Comparing `acdh-django-charts-0.5.3/acdh_django_charts.egg-info/SOURCES.txt` & `acdh-django-charts-0.6.0/acdh_django_charts.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 charts/templates/charts/base.html
 charts/templates/charts/dynchart.html
 charts/templates/charts/select_chart.html
 charts/templates/charts/tags/config_highcharts.html
 charts/templates/charts/tags/load_highcharts_js.html
 charts/templates/charts/tags/selector_dropdown.html
 charts/templatetags/__init__.py
-charts/templatetags/charts_extras.py
+charts/templatetags/charts_extras.py
+tests/test_models.py
```

### Comparing `acdh-django-charts-0.5.3/charts/management/commands/create_charts.py` & `acdh-django-charts-0.6.0/charts/management/commands/create_charts.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from django.core.management.base import BaseCommand, CommandError
-
-from charts.utils import create_chart_config_obj
-
-
-class Command(BaseCommand):
-
-    help = "Create Chart objects for app"
-
-    def add_arguments(self, parser):
-        parser.add_argument(
-            'app_name', type=str,
-            help="Name of the app for which you'd like to create BrowsConf objects."
-        )
-
-    def handle(self, *args, **kwargs):
-        app_name = kwargs['app_name']
-        # exclude_fields = kwargs['exclude_fields']
-        create_chart_config_obj(app_name)
+from django.core.management.base import BaseCommand, CommandError
+
+from charts.utils import create_chart_config_obj
+
+
+class Command(BaseCommand):
+
+    help = "Create Chart objects for app"
+
+    def add_arguments(self, parser):
+        parser.add_argument(
+            'app_name', type=str,
+            help="Name of the app for which you'd like to create BrowsConf objects."
+        )
+
+    def handle(self, *args, **kwargs):
+        app_name = kwargs['app_name']
+        # exclude_fields = kwargs['exclude_fields']
+        create_chart_config_obj(app_name)
```

### Comparing `acdh-django-charts-0.5.3/charts/management/commands/create_charttypes.py` & `acdh-django-charts-0.6.0/charts/management/commands/create_charttypes.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from django.core.management.base import BaseCommand, CommandError
-
-from charts.models import ChartType
-
-CHART_TYPES = [
-    ('bar', '<i class="fas fa-chart-bar"></i>'),
-    ('pie', '<i class="fas fa-chart-pie"></i>'),
-    ('line', '<i class="fas fa-chart-line"></i>'),
-]
-
-
-class Command(BaseCommand):
-
-    help = "Populate database with basic char types"
-
-    def handle(self, *args, **kwargs):
-        all = ChartType.objects.all()
-        self.stdout.write("{} Chart Type objects already existed".format(all.count()))
-        for x in CHART_TYPES:
-            ChartType.objects.get_or_create(
-                name=x[0],
-                icon=x[1]
-            )
-        self.stdout.write(
-            "{} Chart Type objects exist now".format(ChartType.objects.all().count())
-        )
+from django.core.management.base import BaseCommand, CommandError
+
+from charts.models import ChartType
+
+CHART_TYPES = [
+    ('bar', '<i class="fas fa-chart-bar"></i>'),
+    ('pie', '<i class="fas fa-chart-pie"></i>'),
+    ('line', '<i class="fas fa-chart-line"></i>'),
+]
+
+
+class Command(BaseCommand):
+
+    help = "Populate database with basic char types"
+
+    def handle(self, *args, **kwargs):
+        all = ChartType.objects.all()
+        self.stdout.write("{} Chart Type objects already existed".format(all.count()))
+        for x in CHART_TYPES:
+            ChartType.objects.get_or_create(
+                name=x[0],
+                icon=x[1]
+            )
+        self.stdout.write(
+            "{} Chart Type objects exist now".format(ChartType.objects.all().count())
+        )
```

### Comparing `acdh-django-charts-0.5.3/charts/migrations/0001_initial.py` & `acdh-django-charts-0.6.0/charts/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,51 @@
-# Generated by Django 2.0.3 on 2018-06-13 12:34
-
-from django.db import migrations, models
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='ChartConfig',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('model_name', models.CharField(blank=True, help_text="The name of the model class you's like to analyse.", max_length=255)),
-                ('label', models.CharField(blank=True, help_text='A label of the chart.', max_length=255)),
-                ('field_path', models.CharField(blank=True, help_text='The constructor of to the plotted value.', max_length=255)),
-                ('help_text', models.CharField(blank=True, help_text='Contains a description of the chart', max_length=255)),
-                ('legend_x', models.CharField(blank=True, help_text='Text for the legend of the x-axis', max_length=255)),
-                ('legend_y', models.CharField(blank=True, help_text='Text for the legend of the y-axis', max_length=255)),
-            ],
-        ),
-        migrations.CreateModel(
-            name='ChartType',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(blank=True, help_text='A name of the chart type.', max_length=255)),
-                ('icon', models.CharField(blank=True, help_text='A HTML snippet which could be used to display a link to the chart', max_length=255)),
-            ],
-        ),
-        migrations.AddField(
-            model_name='chartconfig',
-            name='chart_types',
-            field=models.ManyToManyField(blank=True, help_text='A selection of chart types which should be accessible.', to='charts.ChartType'),
-        ),
-    ]
+from django.db import models
+
+
+class ChartType(models.Model):
+
+    """Describes possible chart types"""
+
+    name = models.CharField(
+        max_length=255, blank=True, help_text="A name of the chart type."
+    )
+    icon = models.CharField(
+        max_length=255, blank=True,
+        help_text="A HTML snippet which could be used to display a link to the chart"
+    )
+
+    def __str__(self):
+        return self.name
+
+
+class ChartConfig(models.Model):
+    """A class to store config-info for Charts"""
+
+    model_name = models.CharField(
+        max_length=255, blank=True,
+        help_text="The name of the model class you's like to analyse."
+    )
+    app_name = models.CharField(
+        max_length=255, blank=True,
+        help_text="The name of the app where the model you'd like to analyse is defined."
+    )
+    label = models.CharField(
+        max_length=255, blank=True, help_text="A label of the chart."
+    )
+    field_path = models.CharField(
+        max_length=255, blank=True, help_text="The constructor of to the plotted value."
+    )
+    chart_types = models.ManyToManyField(
+        ChartType, blank=True, help_text="A selection of chart types which should be accessible."
+    )
+    help_text = models.CharField(
+        max_length=255, blank=True, help_text="Contains a description of the chart"
+    )
+    legend_x = models.CharField(
+        max_length=255, blank=True, help_text="Text for the legend of the x-axis"
+    )
+    legend_y = models.CharField(
+        max_length=255, blank=True, help_text="Text for the legend of the y-axis"
+    )
+
+    def __str__(self):
+        return "{} ({})".format(self.label, self.field_path)
```

### Comparing `acdh-django-charts-0.5.3/charts/templates/charts/base.html` & `acdh-django-charts-0.6.0/charts/templates/charts/base.html`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-
-{% comment %}
-As the developer of this package, don't place anything here if you can help it
-since this allows developers to have interoperability between your template
-structure and their own.
-
-Example: Developer melding the 2SoD pattern to fit inside with another pattern::
-
-    {% extends "base.html" %}
-    {% load static %}
-
-    <!-- Their site uses old school block layout -->
-    {% block extra_js %}
-
-        <!-- Your package using 2SoD block layout -->
-        {% block javascript %}
-            <script src="{% static 'js/ninja.js' %}" type="text/javascript"></script>
-        {% endblock javascript %}
-
-    {% endblock extra_js %}
-{% endcomment %}
+
+{% comment %}
+As the developer of this package, don't place anything here if you can help it
+since this allows developers to have interoperability between your template
+structure and their own.
+
+Example: Developer melding the 2SoD pattern to fit inside with another pattern::
+
+    {% extends "base.html" %}
+    {% load static %}
+
+    <!-- Their site uses old school block layout -->
+    {% block extra_js %}
+
+        <!-- Your package using 2SoD block layout -->
+        {% block javascript %}
+            <script src="{% static 'js/ninja.js' %}" type="text/javascript"></script>
+        {% endblock javascript %}
+
+    {% endblock extra_js %}
+{% endcomment %}
```

### Comparing `acdh-django-charts-0.5.3/charts/templates/charts/select_chart.html` & `acdh-django-charts-0.6.0/charts/templates/charts/select_chart.html`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-{% extends base_template %}
-{% load staticfiles %}
-{% load django_tables2 crispy_forms_tags %}
-
-{% block content %}
-<div class="alert alert-warning alert-dismissable">
-  <a href="#" class="close" data-dismiss="alert" aria-label="close">&times;</a>
-  <strong>Warning!</strong> This overview and the related charts are still work in progress.
-</div>
-<div class="panel panel-default">
-        <div class="panel-heading detail-heading">
-            <h1 style="text-align:center;"><b>Make your choice</b></h1>
-        </div>
-
-
-
-<table class="table table-hover table-bordered">
-    <thead>
-        <tr>
-            <th>
-                Property to visualize
-            </th>
-            <th>
-                What will it show
-            </th>
-            <th>
-                Type of visualization
-            </th>
-        </tr>
-    </thead>
-    <tbody>
-        {% for x in object_list %}
-        <tr>
-            <td>
-                {{ x.label }}
-            </td>
-            <td>
-                {{ x.help_text }}
-            </td>
-            <td>
-                {% for chart in x.chart_types.all  %}
-                <a href="{% url 'charts:dynchart' model_name=x.model_name property=x.field_path charttype=chart.name %}">
-                    {{ chart.icon | safe }}
-                </a>
-                {% endfor %}
-            </td>
-        </tr>
-        {% endfor %}
-    </tbody>
-</table>
-</div>
-{% endblock %}
+{% extends base_template %}
+{% load staticfiles %}
+{% load django_tables2 crispy_forms_tags %}
+
+{% block content %}
+<div class="alert alert-warning alert-dismissable">
+  <a href="#" class="close" data-dismiss="alert" aria-label="close">&times;</a>
+  <strong>Warning!</strong> This overview and the related charts are still work in progress.
+</div>
+<div class="panel panel-default">
+        <div class="panel-heading detail-heading">
+            <h1 style="text-align:center;"><b>Make your choice</b></h1>
+        </div>
+
+
+
+<table class="table table-hover table-bordered">
+    <thead>
+        <tr>
+            <th>
+                Property to visualize
+            </th>
+            <th>
+                What will it show
+            </th>
+            <th>
+                Type of visualization
+            </th>
+        </tr>
+    </thead>
+    <tbody>
+        {% for x in object_list %}
+        <tr>
+            <td>
+                {{ x.label }}
+            </td>
+            <td>
+                {{ x.help_text }}
+            </td>
+            <td>
+                {% for chart in x.chart_types.all  %}
+                <a href="{% url 'charts:dynchart' model_name=x.model_name property=x.field_path charttype=chart.name %}">
+                    {{ chart.icon | safe }}
+                </a>
+                {% endfor %}
+            </td>
+        </tr>
+        {% endfor %}
+    </tbody>
+</table>
+</div>
+{% endblock %}
```

### Comparing `acdh-django-charts-0.5.3/charts/templates/charts/tags/selector_dropdown.html` & `acdh-django-charts-0.6.0/charts/templates/charts/tags/selector_dropdown.html`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-<div class="btn-group">
-    <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown" aria-expanded="true">
-    Visualize <span class="caret"></span></button>
-    <ul class="dropdown-menu" role="menu">
-        {% for x in vis_list %}
-            <li>
-                {% for y in x.chart_types.all %}
-                    <a class="dropdown-item" title="{{ x.help_text }}" href="?{{ request.GET.urlencode }}&charttype={{ y }}&property={{ x.field_path }}">{{ x.label }} {{ y.icon|safe }}</a>
-                {% endfor %}
-            </li>
-            <hr/>
-
-        {% endfor %}
-    </ul>
-</div>
+<div class="btn-group">
+    <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown" aria-expanded="true">
+    Visualize <span class="caret"></span></button>
+    <ul class="dropdown-menu" role="menu">
+        {% for x in vis_list %}
+            <li>
+                {% for y in x.chart_types.all %}
+                    <a class="dropdown-item" title="{{ x.help_text }}" href="?{{ request.GET.urlencode }}&charttype={{ y }}&property={{ x.field_path }}">{{ x.label }} {{ y.icon|safe }}</a>
+                {% endfor %}
+            </li>
+            <hr/>
+
+        {% endfor %}
+    </ul>
+</div>
```

### Comparing `acdh-django-charts-0.5.3/charts/utils.py` & `acdh-django-charts-0.6.0/charts/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from django.apps import apps
-
-from . models import ChartType, ChartConfig
-
-
-def create_chart_config_obj(app_name, exclude_fields=[]):
-    """
-    Creates ChartConfig objects for all models defined in chosen app
-    """
-    exclude = exclude_fields
-    try:
-        models = [x for x in apps.get_app_config(app_name).get_models()]
-    except LookupError:
-        print("The app '{}' does not exist".format(app_name))
-        return False
-
-    barchart, _ = ChartType.objects.get_or_create(name='bar')
-
-    for x in models:
-        model_name = "{}".format(x.__name__.lower())
-        print("Model: {}".format(model_name))
-        for f in x._meta.get_fields(include_parents=False):
-            if f.name not in exclude:
-                field_name = f.name
-                verbose_name = getattr(f, 'verbose_name', f.name)
-                help_text = getattr(f, 'help_text', 'no helptext')
-                print("{}: {} ({})".format(
-                    model_name,
-                    field_name,
-                    help_text
-                    )
-                )
-                chart_conf, _ = ChartConfig.objects.get_or_create(
-                    model_name=model_name,
-                    app_name=app_name,
-                    field_path=field_name
-                )
-                chart_conf.chart_types.add(barchart)
-                chart_conf.label = verbose_name
-                chart_conf.help_text = help_text
-                chart_conf.save()
-            else:
-                print("skipped: {}".format(f.name))
+from django.apps import apps
+
+from . models import ChartType, ChartConfig
+
+
+def create_chart_config_obj(app_name, exclude_fields=[]):
+    """
+    Creates ChartConfig objects for all models defined in chosen app
+    """
+    exclude = exclude_fields
+    try:
+        models = [x for x in apps.get_app_config(app_name).get_models()]
+    except LookupError:
+        print("The app '{}' does not exist".format(app_name))
+        return False
+
+    barchart, _ = ChartType.objects.get_or_create(name='bar')
+
+    for x in models:
+        model_name = "{}".format(x.__name__.lower())
+        print("Model: {}".format(model_name))
+        for f in x._meta.get_fields(include_parents=False):
+            if f.name not in exclude:
+                field_name = f.name
+                verbose_name = getattr(f, 'verbose_name', f.name)
+                help_text = getattr(f, 'help_text', 'no helptext')
+                print("{}: {} ({})".format(
+                    model_name,
+                    field_name,
+                    help_text
+                    )
+                )
+                chart_conf, _ = ChartConfig.objects.get_or_create(
+                    model_name=model_name,
+                    app_name=app_name,
+                    field_path=field_name
+                )
+                chart_conf.chart_types.add(barchart)
+                chart_conf.label = verbose_name
+                chart_conf.help_text = help_text
+                chart_conf.save()
+            else:
+                print("skipped: {}".format(f.name))
```

### Comparing `acdh-django-charts-0.5.3/charts/views.py` & `acdh-django-charts-0.6.0/charts/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-import json
-
-from collections import Counter
-
-from django.conf import settings
-from django.core.exceptions import ObjectDoesNotExist, FieldError
-from django.contrib.contenttypes.models import ContentType
-from django.db.models import Count
-from django.views.generic import TemplateView
-from django.views.generic.list import ListView
-
-from . models import ChartConfig
-
-try:
-    base_template = settings.CHARTS_BASE_TEMPLATE
-except AttributeError:
-    base_template = 'webpage/base.html'
-
-
-class ChartSelector(ListView):
-    model = ChartConfig
-    template_name = 'charts/select_chart.html'
-
-    def get_context_data(self, **kwargs):
-        context = super(ChartSelector, self).get_context_data()
-        context['base_template'] = base_template
-        return context
-
-
-def create_payload(model_name, property_name, charttype, qs, app_label=None):
-
-    """ creates a dict which can be processed by highcharts"""
-
-    context = {}
-    payload = []
-    objects = qs
-
-    try:
-        ct = ContentType.objects.get(
-            app_label=app_label, model=model_name
-        ).model_class()
-        modelname = ct.__name__
-    except ObjectDoesNotExist:
-        context['fatal_error'] = True
-        context['error_msg'] = "The model: <code>{}</code> you requested is not defined"\
-            .format(model_name.title())
-        return context
-
-    try:
-        chart = ChartConfig.objects.get(
-            field_path=property_name,
-            model_name=model_name,
-            app_name=app_label
-        )
-        chart = chart.__dict__
-    except ObjectDoesNotExist:
-        context['error'] = True
-        context['error_msg'] = """The ChartConfig Object:
-            <code>field_path={}, model_name={}</code> you requested couldn't be found."""\
-            .format(property_name, model_name.title())
-        chart = {
-            'legend_x': None,
-            'legend_y': None,
-            'label': 'not defined',
-            'help_text': 'not defined'
-        }
-        if settings.DEBUG:
-            pass
-        else:
-            context['fatal_error'] = True
-# https://stackoverflow.com/questions/3432673/get-distinct-values-of-queryset-by-field
-    try:
-        values = qs.values(property_name)
-        result = dict(Counter(
-            [x[property_name] for x in list(values)]
-        ))
-        try:
-            result['Field not populated'] = result.pop(None)
-        except KeyError:
-            pass
-        payload = [list(x) for x in list(result.items())]
-        context['all'] = ct.objects.count()
-        if chart['legend_x']:
-            legendx = chart['legend_x']
-        else:
-            legendx = "# of {}s".format(modelname)
-        data = {
-            "items": "{} out of {}".format(objects.count(), context['all']),
-            "title": "{}".format(chart['label']),
-            "subtitle": "{}".format(chart["help_text"]),
-            "legendy": chart["legend_y"],
-            "legendx": legendx,
-            "categories": "sorted(dates)",
-            "measuredObject": "{}s".format(modelname),
-            "ymin": 0,
-            "payload": payload
-        }
-        context['data'] = data
-    except FieldError:
-        context['error'] = True
-        context['error_msg'] = "The field: <code>{}</code> you requested does not exist"\
-            .format(property_name)
-
-    return context
-
-
-class DynChartView(TemplateView):
-
-    template_name = 'charts/dynchart.html'
-
-    def get_context_data(self, **kwargs):
-        context = super(DynChartView, self).get_context_data()
-        context['base_template'] = base_template
-        model_name = self.kwargs['model_name']
-        property_name = self.kwargs['property']
-        context['property_name'] = property_name
-        context['charttype'] = self.kwargs['charttype']
-        try:
-            ct = ContentType.objects.get(model=model_name).model_class()
-        except ObjectDoesNotExist:
-            context['fatal_error'] = True
-            context['error_msg'] = "The model: <code>{}</code> you requested is not defined"\
-                .format(model_name.title())
-            return context
-
-        chartdata = create_payload(
-            model_name,
-            property_name,
-            context['charttype'],
-            ct.objects.all()
-        )
-
-        context = dict(context, **chartdata)
-
-        return context
+import json
+
+from collections import Counter
+
+from django.conf import settings
+from django.core.exceptions import ObjectDoesNotExist, FieldError
+from django.contrib.contenttypes.models import ContentType
+from django.db.models import Count
+from django.views.generic import TemplateView
+from django.views.generic.list import ListView
+
+from . models import ChartConfig
+
+try:
+    base_template = settings.CHARTS_BASE_TEMPLATE
+except AttributeError:
+    base_template = 'webpage/base.html'
+
+
+class ChartSelector(ListView):
+    model = ChartConfig
+    template_name = 'charts/select_chart.html'
+
+    def get_context_data(self, **kwargs):
+        context = super(ChartSelector, self).get_context_data()
+        context['base_template'] = base_template
+        return context
+
+
+def create_payload(model_name, property_name, charttype, qs, app_label=None):
+
+    """ creates a dict which can be processed by highcharts"""
+
+    context = {}
+    payload = []
+    objects = qs
+
+    try:
+        ct = ContentType.objects.get(
+            app_label=app_label, model=model_name
+        ).model_class()
+        modelname = ct.__name__
+    except ObjectDoesNotExist:
+        context['fatal_error'] = True
+        context['error_msg'] = "The model: <code>{}</code> you requested is not defined"\
+            .format(model_name.title())
+        return context
+
+    try:
+        chart = ChartConfig.objects.get(
+            field_path=property_name,
+            model_name=model_name,
+            app_name=app_label
+        )
+        chart = chart.__dict__
+    except ObjectDoesNotExist:
+        context['error'] = True
+        context['error_msg'] = """The ChartConfig Object:
+            <code>field_path={}, model_name={}</code> you requested couldn't be found."""\
+            .format(property_name, model_name.title())
+        chart = {
+            'legend_x': None,
+            'legend_y': None,
+            'label': 'not defined',
+            'help_text': 'not defined'
+        }
+        if settings.DEBUG:
+            pass
+        else:
+            context['fatal_error'] = True
+# https://stackoverflow.com/questions/3432673/get-distinct-values-of-queryset-by-field
+    try:
+        values = qs.values(property_name)
+        result = dict(Counter(
+            [f"{x[property_name]}" for x in list(values)]
+        ))
+        try:
+            result['Field not populated'] = result.pop(None)
+        except KeyError:
+            pass
+        payload = [list(x) for x in list(result.items())]
+        context['all'] = ct.objects.count()
+        if chart['legend_x']:
+            legendx = chart['legend_x']
+        else:
+            legendx = "# of {}s".format(modelname)
+        data = {
+            "items": "{} out of {}".format(objects.count(), context['all']),
+            "title": "{}".format(chart['label']),
+            "subtitle": "{}".format(chart["help_text"]),
+            "legendy": chart["legend_y"],
+            "legendx": legendx,
+            "categories": "sorted(dates)",
+            "measuredObject": "{}s".format(modelname),
+            "ymin": 0,
+            "payload": payload
+        }
+        context['data'] = data
+    except FieldError:
+        context['error'] = True
+        context['error_msg'] = "The field: <code>{}</code> you requested does not exist"\
+            .format(property_name)
+
+    return context
+
+
+class DynChartView(TemplateView):
+
+    template_name = 'charts/dynchart.html'
+
+    def get_context_data(self, **kwargs):
+        context = super(DynChartView, self).get_context_data()
+        context['base_template'] = base_template
+        model_name = self.kwargs['model_name']
+        property_name = self.kwargs['property']
+        context['property_name'] = property_name
+        context['charttype'] = self.kwargs['charttype']
+        try:
+            ct = ContentType.objects.get(model=model_name).model_class()
+        except ObjectDoesNotExist:
+            context['fatal_error'] = True
+            context['error_msg'] = "The model: <code>{}</code> you requested is not defined"\
+                .format(model_name.title())
+            return context
+
+        chartdata = create_payload(
+            model_name,
+            property_name,
+            context['charttype'],
+            ct.objects.all()
+        )
+
+        context = dict(context, **chartdata)
+
+        return context
```

### Comparing `acdh-django-charts-0.5.3/setup.py` & `acdh-django-charts-0.6.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,73 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-import os
-import re
-import sys
-
-try:
-    from setuptools import setup
-except ImportError:
-    from distutils.core import setup
-
-
-def get_version(*file_paths):
-    """Retrieves the version from charts/__init__.py"""
-    filename = os.path.join(os.path.dirname(__file__), *file_paths)
-    version_file = open(filename).read()
-    version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]",
-                              version_file, re.M)
-    if version_match:
-        return version_match.group(1)
-    raise RuntimeError('Unable to find version string.')
-
-
-version = get_version("charts", "__init__.py")
-
-
-if sys.argv[-1] == 'publish':
-    try:
-        import wheel
-        print("Wheel version: ", wheel.__version__)
-    except ImportError:
-        print('Wheel library missing. Please run "pip install wheel"')
-        sys.exit()
-    os.system('python setup.py sdist upload')
-    os.system('python setup.py bdist_wheel upload')
-    sys.exit()
-
-if sys.argv[-1] == 'tag':
-    print("Tagging the version on git:")
-    os.system("git tag -a %s -m 'version %s'" % (version, version))
-    os.system("git push --tags")
-    sys.exit()
-
-readme = open('README.rst').read()
-history = open('HISTORY.rst').read().replace('.. :changelog:', '')
-
-setup(
-    name='acdh-django-charts',
-    version=version,
-    description="""An app to explore your data through charts based on Highcharts.js""",
-    long_description=readme + '\n\n' + history,
-    author='Peter Andorfer',
-    author_email='peter.andorfer@oeaw.ac.at',
-    url='https://github.com/acdh-oeaw/acdh-django-charts',
-    packages=[
-        'charts',
-    ],
-    include_package_data=True,
-    install_requires=[],
-    license="MIT",
-    zip_safe=False,
-    keywords='acdh-django-charts',
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Framework :: Django :: 2.0',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-    ],
-)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+import os
+import re
+import sys
+
+try:
+    from setuptools import setup
+except ImportError:
+    from distutils.core import setup
+
+
+def get_version(*file_paths):
+    """Retrieves the version from charts/__init__.py"""
+    filename = os.path.join(os.path.dirname(__file__), *file_paths)
+    version_file = open(filename).read()
+    version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]",
+                              version_file, re.M)
+    if version_match:
+        return version_match.group(1)
+    raise RuntimeError('Unable to find version string.')
+
+
+version = get_version("charts", "__init__.py")
+
+
+if sys.argv[-1] == 'publish':
+    try:
+        import wheel
+        print("Wheel version: ", wheel.__version__)
+    except ImportError:
+        print('Wheel library missing. Please run "pip install wheel"')
+        sys.exit()
+    os.system('python setup.py sdist upload')
+    os.system('python setup.py bdist_wheel upload')
+    sys.exit()
+
+if sys.argv[-1] == 'tag':
+    print("Tagging the version on git:")
+    os.system("git tag -a %s -m 'version %s'" % (version, version))
+    os.system("git push --tags")
+    sys.exit()
+
+readme = open('README.rst').read()
+history = open('HISTORY.rst').read().replace('.. :changelog:', '')
+
+setup(
+    name='acdh-django-charts',
+    version=version,
+    description="""An app to explore your data through charts based on Highcharts.js""",
+    long_description=readme + '\n\n' + history,
+    author='Peter Andorfer',
+    author_email='peter.andorfer@oeaw.ac.at',
+    url='https://github.com/acdh-oeaw/acdh-django-charts',
+    packages=[
+        'charts',
+    ],
+    include_package_data=True,
+    install_requires=[],
+    license="MIT",
+    zip_safe=False,
+    keywords='acdh-django-charts',
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Framework :: Django :: 2.0',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: BSD License',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+    ],
+)
```

