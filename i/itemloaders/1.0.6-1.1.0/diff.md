# Comparing `tmp/itemloaders-1.0.6.tar.gz` & `tmp/itemloaders-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itemloaders-1.0.6.tar", last modified: Mon Aug 29 10:03:19 2022, max compression
+gzip compressed data, was "itemloaders-1.1.0.tar", last modified: Fri Apr 21 09:00:08 2023, max compression
```

## Comparing `itemloaders-1.0.6.tar` & `itemloaders-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 10:03:19.962710 itemloaders-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-08-29 10:03:08.000000 itemloaders-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-29 10:03:08.000000 itemloaders-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3705 2022-08-29 10:03:19.962710 itemloaders-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2608 2022-08-29 10:03:08.000000 itemloaders-1.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 10:03:19.958710 itemloaders-1.0.6/itemloaders/
--rw-r--r--   0 runner    (1001) docker     (121)    16599 2022-08-29 10:03:08.000000 itemloaders-1.0.6/itemloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-08-29 10:03:08.000000 itemloaders-1.0.6/itemloaders/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     8550 2022-08-29 10:03:08.000000 itemloaders-1.0.6/itemloaders/processors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-08-29 10:03:08.000000 itemloaders-1.0.6/itemloaders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 10:03:19.962710 itemloaders-1.0.6/itemloaders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3705 2022-08-29 10:03:19.000000 itemloaders-1.0.6/itemloaders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-08-29 10:03:19.000000 itemloaders-1.0.6/itemloaders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-29 10:03:19.000000 itemloaders-1.0.6/itemloaders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-29 10:03:19.000000 itemloaders-1.0.6/itemloaders.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-08-29 10:03:19.000000 itemloaders-1.0.6/itemloaders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-29 10:03:19.000000 itemloaders-1.0.6/itemloaders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-08-29 10:03:19.962710 itemloaders-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-08-29 10:03:08.000000 itemloaders-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:08.439595 itemloaders-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-21 08:59:57.000000 itemloaders-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 08:59:57.000000 itemloaders-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-21 09:00:08.439595 itemloaders-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-21 08:59:57.000000 itemloaders-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:08.435594 itemloaders-1.1.0/itemloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)    19047 2023-04-21 08:59:57.000000 itemloaders-1.1.0/itemloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-21 08:59:57.000000 itemloaders-1.1.0/itemloaders/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-04-21 08:59:57.000000 itemloaders-1.1.0/itemloaders/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-21 08:59:57.000000 itemloaders-1.1.0/itemloaders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:08.439595 itemloaders-1.1.0/itemloaders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-21 09:00:08.000000 itemloaders-1.1.0/itemloaders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-21 09:00:08.000000 itemloaders-1.1.0/itemloaders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:00:08.000000 itemloaders-1.1.0/itemloaders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:00:08.000000 itemloaders-1.1.0/itemloaders.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 09:00:08.000000 itemloaders-1.1.0/itemloaders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 09:00:08.000000 itemloaders-1.1.0/itemloaders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-21 09:00:08.439595 itemloaders-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-21 08:59:57.000000 itemloaders-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:00:08.439595 itemloaders-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_base_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_loader_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_nested_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_nested_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_output_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_select_jmes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_selector_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-21 08:59:57.000000 itemloaders-1.1.0/tests/test_utils_python.py
```

### Comparing `itemloaders-1.0.6/LICENSE` & `itemloaders-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `itemloaders-1.0.6/PKG-INFO` & `itemloaders-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: itemloaders
-Version: 1.0.6
+Version: 1.1.0
 Summary: Base library for scrapy's ItemLoader
 Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte
 Author-email: opensource@zyte.com
 License: BSD
 Project-URL: Documentation, https://itemloaders.readthedocs.io/
 Project-URL: Source, https://github.com/scrapy/itemloaders
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===========
 itemloaders
 ===========
 
@@ -96,8 +96,9 @@
   `Pull Requests here <https://github.com/scrapy/itemloaders/pulls>`_
 
 * If you want to submit a code change
 
    * File an `issue here <https://github.com/scrapy/itemloaders/issues>`_, if there isn't one yet
    * Fork this repository
    * Create a branch to work on your changes
+   * Run `pre-commit install` to install pre-commit hooks
    * Push your local branch and submit a Pull Request
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: itemloaders Version: 1.0.6 Summary: Base library
+Metadata-Version: 2.1 Name: itemloaders Version: 1.1.0 Summary: Base library
 for scrapy's ItemLoader Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte Author-email: opensource@zyte.com License: BSD Project-URL:
 Documentation, https://itemloaders.readthedocs.io/ Project-URL: Source, https:/
 /github.com/scrapy/itemloaders Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Requires-Python: >=3.6
+Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/x-rst License-File: LICENSE ===========
 itemloaders =========== .. image:: https://img.shields.io/pypi/v/
 itemloaders.svg :target: https://pypi.python.org/pypi/itemloaders :alt: PyPI
 Version .. image:: https://img.shields.io/pypi/pyversions/itemloaders.svg :
 target: https://pypi.python.org/pypi/itemloaders :alt: Supported Python
 Versions .. image:: https://github.com/scrapy/itemloaders/workflows/CI/
 badge.svg?branch=master :target: https://github.com/scrapy/itemloaders/
@@ -42,9 +42,9 @@
 out the `documentation
 itemloaders.readthedocs.io/en/latest/>`_. Contributing ============ All
 contributions are welcome! * If you want to review some code, check open `Pull
 Requests here
 github.com/scrapy/itemloaders/pulls>`_ * If you want to submit a code change *
 File an `issue here
 github.com/scrapy/itemloaders/issues>`_, if there isn't one yet * Fork this
-repository * Create a branch to work on your changes * Push your local branch
-and submit a Pull Request
+repository * Create a branch to work on your changes * Run `pre-commit install`
+to install pre-commit hooks * Push your local branch and submit a Pull Request
```

### Comparing `itemloaders-1.0.6/README.rst` & `itemloaders-1.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -69,8 +69,9 @@
   `Pull Requests here <https://github.com/scrapy/itemloaders/pulls>`_
 
 * If you want to submit a code change
 
    * File an `issue here <https://github.com/scrapy/itemloaders/issues>`_, if there isn't one yet
    * Fork this repository
    * Create a branch to work on your changes
+   * Run `pre-commit install` to install pre-commit hooks
    * Push your local branch and submit a Pull Request
```

#### html2text {}

```diff
@@ -27,9 +27,9 @@
 out the `documentation
 itemloaders.readthedocs.io/en/latest/>`_. Contributing ============ All
 contributions are welcome! * If you want to review some code, check open `Pull
 Requests here
 github.com/scrapy/itemloaders/pulls>`_ * If you want to submit a code change *
 File an `issue here
 github.com/scrapy/itemloaders/issues>`_, if there isn't one yet * Fork this
-repository * Create a branch to work on your changes * Push your local branch
-and submit a Pull Request
+repository * Create a branch to work on your changes * Run `pre-commit install`
+to install pre-commit hooks * Push your local branch and submit a Pull Request
```

### Comparing `itemloaders-1.0.6/itemloaders/__init__.py` & `itemloaders-1.1.0/itemloaders/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def unbound_method(method):
     """
     Allow to use single-argument functions as input or output processors
     (no need to define an unused first 'self' argument)
     """
     with suppress(AttributeError):
-        if '.' not in method.__qualname__:
+        if "." not in method.__qualname__:
             return method.__func__
     return method
 
 
 class ItemLoader:
     """
     Return a new Item Loader for populating the given item. If no item is
@@ -32,20 +32,20 @@
 
     When instantiated with a :param ``selector`` parameter the :class:`ItemLoader` class
     provides convenient mechanisms for extracting data from web pages
     using parsel_ selectors.
 
     :param item: The item instance to populate using subsequent calls to
         :meth:`~ItemLoader.add_xpath`, :meth:`~ItemLoader.add_css`,
-        or :meth:`~ItemLoader.add_value`.
+        :meth:`~ItemLoader.add_jmes` or :meth:`~ItemLoader.add_value`.
     :type item: :class:`dict` object
 
     :param selector: The selector to extract data from, when using the
-        :meth:`add_xpath` (resp. :meth:`add_css`) or :meth:`replace_xpath`
-        (resp. :meth:`replace_css`) method.
+        :meth:`add_xpath` (resp. :meth:`add_css`, :meth:`add_jmes`) or :meth:`replace_xpath`
+        (resp. :meth:`replace_css`, :meth:`replace_jmes`) method.
     :type selector: :class:`~parsel.selector.Selector` object
 
     The item, selector and the remaining keyword arguments are
     assigned to the Loader context (accessible through the :attr:`context` attribute).
 
     .. attribute:: item
 
@@ -101,15 +101,15 @@
 
     def __init__(self, item=None, selector=None, parent=None, **context):
         self.selector = selector
         context.update(selector=selector)
         if item is None:
             item = self.default_item_class()
         self._local_item = item
-        context['item'] = item
+        context["item"] = item
         self.context = context
         self.parent = parent
         self._local_values = {}
         # values from initial item
         for field_name, value in ItemAdapter(item).items():
             self._values.setdefault(field_name, [])
             self._values[field_name] += arg_to_iter(value)
@@ -134,32 +134,28 @@
         The supplied selector is applied relative to selector associated
         with this :class:`ItemLoader`. The nested loader shares the item
         with the parent :class:`ItemLoader` so calls to :meth:`add_xpath`,
         :meth:`add_value`, :meth:`replace_value`, etc. will behave as expected.
         """
         selector = self.selector.xpath(xpath)
         context.update(selector=selector)
-        subloader = self.__class__(
-            item=self.item, parent=self, **context
-        )
+        subloader = self.__class__(item=self.item, parent=self, **context)
         return subloader
 
     def nested_css(self, css, **context):
         """
         Create a nested loader with a css selector.
         The supplied selector is applied relative to selector associated
         with this :class:`ItemLoader`. The nested loader shares the item
         with the parent :class:`ItemLoader` so calls to :meth:`add_xpath`,
         :meth:`add_value`, :meth:`replace_value`, etc. will behave as expected.
         """
         selector = self.selector.css(css)
         context.update(selector=selector)
-        subloader = self.__class__(
-            item=self.item, parent=self, **context
-        )
+        subloader = self.__class__(item=self.item, parent=self, **context)
         return subloader
 
     def add_value(self, field_name, value, *processors, re=None, **kw):
         """
         Process and then add the given ``value`` for the given field.
 
         The value is first passed through :meth:`get_value` by giving the
@@ -242,17 +238,18 @@
             if value is None:
                 break
             _proc = proc
             proc = wrap_loader_context(proc, self.context)
             try:
                 value = proc(value)
             except Exception as e:
-                raise ValueError("Error with processor %s value=%r error='%s: %s'" %
-                                 (_proc.__class__.__name__, value,
-                                  type(e).__name__, str(e)))
+                raise ValueError(
+                    "Error with processor %s value=%r error='%s: %s'"
+                    % (_proc.__class__.__name__, value, type(e).__name__, str(e))
+                ) from e
         return value
 
     def load_item(self):
         """
         Populate the item with the data collected so far, and return it. The
         data collected is first passed through the :ref:`output processors
         <processors>` to get the final value to assign to each item field.
@@ -272,38 +269,36 @@
         """
         proc = self.get_output_processor(field_name)
         proc = wrap_loader_context(proc, self.context)
         value = self._values.get(field_name, [])
         try:
             return proc(value)
         except Exception as e:
-            raise ValueError("Error with output processor: field=%r value=%r error='%s: %s'" %
-                             (field_name, value, type(e).__name__, str(e)))
+            raise ValueError(
+                "Error with output processor: field=%r value=%r error='%s: %s'"
+                % (field_name, value, type(e).__name__, str(e))
+            ) from e
 
     def get_collected_values(self, field_name):
         """Return the collected values for the given field."""
         return self._values.get(field_name, [])
 
     def get_input_processor(self, field_name):
-        proc = getattr(self, '%s_in' % field_name, None)
+        proc = getattr(self, "%s_in" % field_name, None)
         if not proc:
             proc = self._get_item_field_attr(
-                field_name,
-                'input_processor',
-                self.default_input_processor
+                field_name, "input_processor", self.default_input_processor
             )
         return unbound_method(proc)
 
     def get_output_processor(self, field_name):
-        proc = getattr(self, '%s_out' % field_name, None)
+        proc = getattr(self, "%s_out" % field_name, None)
         if not proc:
             proc = self._get_item_field_attr(
-                field_name,
-                'output_processor',
-                self.default_output_processor
+                field_name, "output_processor", self.default_output_processor
             )
         return unbound_method(proc)
 
     def _get_item_field_attr(self, field_name, key, default=None):
         field_meta = ItemAdapter(self.item).get_field_meta(field_name)
         return field_meta.get(key, default)
 
@@ -312,16 +307,23 @@
         _proc = proc
         proc = wrap_loader_context(proc, self.context)
         try:
             return proc(value)
         except Exception as e:
             raise ValueError(
                 "Error with input processor %s: field=%r value=%r "
-                "error='%s: %s'" % (_proc.__class__.__name__, field_name,
-                                    value, type(e).__name__, str(e)))
+                "error='%s: %s'"
+                % (
+                    _proc.__class__.__name__,
+                    field_name,
+                    value,
+                    type(e).__name__,
+                    str(e),
+                )
+            ) from e
 
     def _check_selector_method(self):
         if self.selector is None:
             raise RuntimeError(
                 "To use XPath or CSS selectors, %s "
                 "must be instantiated with a selector" % self.__class__.__name__
             )
@@ -398,22 +400,22 @@
         Examples::
 
             # HTML snippet: <p class="product-name">Color TV</p>
             loader.add_css('name', 'p.product-name')
             # HTML snippet: <p id="price">the price is $1200</p>
             loader.add_css('price', 'p#price', re='the price is (.*)')
         """
-        values = self._get_cssvalues(css, **kw)
+        values = self._get_cssvalues(css)
         self.add_value(field_name, values, *processors, re=re, **kw)
 
     def replace_css(self, field_name, css, *processors, re=None, **kw):
         """
         Similar to :meth:`add_css` but replaces collected data instead of adding it.
         """
-        values = self._get_cssvalues(css, **kw)
+        values = self._get_cssvalues(css)
         self.replace_value(field_name, values, *processors, re=re, **kw)
 
     def get_css(self, css, *processors, re=None, **kw):
         """
         Similar to :meth:`ItemLoader.get_value` but receives a CSS selector
         instead of a value, which is used to extract a list of unicode strings
         from the selector associated with this :class:`ItemLoader`.
@@ -428,14 +430,74 @@
         Examples::
 
             # HTML snippet: <p class="product-name">Color TV</p>
             loader.get_css('p.product-name')
             # HTML snippet: <p id="price">the price is $1200</p>
             loader.get_css('p#price', TakeFirst(), re='the price is (.*)')
         """
-        values = self._get_cssvalues(css, **kw)
+        values = self._get_cssvalues(css)
         return self.get_value(values, *processors, re=re, **kw)
 
-    def _get_cssvalues(self, csss, **kw):
+    def _get_cssvalues(self, csss):
         self._check_selector_method()
         csss = arg_to_iter(csss)
         return flatten(self.selector.css(css).getall() for css in csss)
+
+    def add_jmes(self, field_name, jmes, *processors, re=None, **kw):
+        """
+        Similar to :meth:`ItemLoader.add_value` but receives a JMESPath selector
+        instead of a value, which is used to extract a list of unicode strings
+        from the selector associated with this :class:`ItemLoader`.
+
+        See :meth:`get_jmes` for ``kwargs``.
+
+        :param jmes: the JMESPath selector to extract data from
+        :type jmes: str
+
+        Examples::
+
+            # HTML snippet: {"name": "Color TV"}
+            loader.add_jmes('name')
+            # HTML snippet: {"price": the price is $1200"}
+            loader.add_jmes('price', TakeFirst(), re='the price is (.*)')
+        """
+        values = self._get_jmesvalues(jmes)
+        self.add_value(field_name, values, *processors, re=re, **kw)
+
+    def replace_jmes(self, field_name, jmes, *processors, re=None, **kw):
+        """
+        Similar to :meth:`add_jmes` but replaces collected data instead of adding it.
+        """
+        values = self._get_jmesvalues(jmes)
+        self.replace_value(field_name, values, *processors, re=re, **kw)
+
+    def get_jmes(self, jmes, *processors, re=None, **kw):
+        """
+        Similar to :meth:`ItemLoader.get_value` but receives a JMESPath selector
+        instead of a value, which is used to extract a list of unicode strings
+        from the selector associated with this :class:`ItemLoader`.
+
+        :param jmes: the JMESPath selector to extract data from
+        :type jmes: str
+
+        :param re: a regular expression to use for extracting data from the
+            selected JMESPath
+        :type re: str or typing.Pattern
+
+        Examples::
+
+            # HTML snippet: {"name": "Color TV"}
+            loader.get_jmes('name')
+            # HTML snippet: {"price": the price is $1200"}
+            loader.get_jmes('price', TakeFirst(), re='the price is (.*)')
+        """
+        values = self._get_jmesvalues(jmes)
+        return self.get_value(values, *processors, re=re, **kw)
+
+    def _get_jmesvalues(self, jmess):
+        self._check_selector_method()
+        jmess = arg_to_iter(jmess)
+        if not hasattr(self.selector, "jmespath"):
+            raise AttributeError(
+                "Please install parsel >= 1.8.1 to get jmespath support"
+            )
+        return flatten(self.selector.jmespath(jmes).getall() for jmes in jmess)
```

### Comparing `itemloaders-1.0.6/itemloaders/processors.py` & `itemloaders-1.1.0/itemloaders/processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 This module provides some commonly used processors for Item Loaders.
 
 See documentation in docs/topics/loaders.rst
 """
 from collections import ChainMap
 
-from itemloaders.utils import arg_to_iter
 from itemloaders.common import wrap_loader_context
+from itemloaders.utils import arg_to_iter
 
 
 class MapCompose:
     """
     A processor which is constructed from the composition of the given
     functions, similar to the :class:`Compose` processor. The difference with
     this processor is the way internal results are passed among functions,
@@ -47,15 +47,15 @@
     ['HELLO', 'THIS', 'IS', 'SOMETHING']
 
     As with the Compose processor, functions can receive Loader contexts, and
     ``__init__`` method keyword arguments are used as default context values.
     See :class:`Compose` processor for more info.
 
     .. _`parsel selectors`: https://parsel.readthedocs.io/en/latest/parsel.html#parsel.selector.Selector.extract
-    """
+    """  # noqa
 
     def __init__(self, *functions, **default_loader_context):
         self.functions = functions
         self.default_loader_context = default_loader_context
 
     def __call__(self, value, loader_context=None):
         values = arg_to_iter(value)
@@ -66,18 +66,19 @@
         wrapped_funcs = [wrap_loader_context(f, context) for f in self.functions]
         for func in wrapped_funcs:
             next_values = []
             for v in values:
                 try:
                     next_values += arg_to_iter(func(v))
                 except Exception as e:
-                    raise ValueError("Error in MapCompose with "
-                                     "%s value=%r error='%s: %s'" %
-                                     (str(func), value, type(e).__name__,
-                                      str(e)))
+                    raise ValueError(
+                        "Error in MapCompose with "
+                        "%s value=%r error='%s: %s'"
+                        % (str(func), value, type(e).__name__, str(e))
+                    ) from e
             values = next_values
         return values
 
 
 class Compose:
     """
     A processor which is constructed from the composition of the given
@@ -105,32 +106,34 @@
     Loader context values passed to functions are overridden with the currently
     active Loader context accessible through the :attr:`ItemLoader.context
     <itemloaders.ItemLoader.context>` attribute.
     """
 
     def __init__(self, *functions, **default_loader_context):
         self.functions = functions
-        self.stop_on_none = default_loader_context.get('stop_on_none', True)
+        self.stop_on_none = default_loader_context.get("stop_on_none", True)
         self.default_loader_context = default_loader_context
 
     def __call__(self, value, loader_context=None):
         if loader_context:
             context = ChainMap(loader_context, self.default_loader_context)
         else:
             context = self.default_loader_context
         wrapped_funcs = [wrap_loader_context(f, context) for f in self.functions]
         for func in wrapped_funcs:
             if value is None and self.stop_on_none:
                 break
             try:
                 value = func(value)
             except Exception as e:
-                raise ValueError("Error in Compose with "
-                                 "%s value=%r error='%s: %s'" %
-                                 (str(func), value, type(e).__name__, str(e)))
+                raise ValueError(
+                    "Error in Compose with "
+                    "%s value=%r error='%s: %s'"
+                    % (str(func), value, type(e).__name__, str(e))
+                ) from e
         return value
 
 
 class TakeFirst:
     """
     Returns the first non-null/non-empty value from the values received,
     so it's typically used as an output processor to single-valued fields.
@@ -142,15 +145,15 @@
     >>> proc = TakeFirst()
     >>> proc(['', 'one', 'two', 'three'])
     'one'
     """
 
     def __call__(self, values):
         for value in values:
-            if value is not None and value != '':
+            if value is not None and value != "":
                 return value
 
 
 class Identity:
     """
     The simplest processor, which doesn't do anything. It returns the original
     values unchanged. It doesn't receive any ``__init__`` method arguments, nor does it
@@ -193,14 +196,15 @@
     >>> proc_json_list('[{"foo":"bar"}, {"baz":"tar"}]')
     ['bar']
     """
 
     def __init__(self, json_path):
         self.json_path = json_path
         import jmespath
+
         self.compiled_path = jmespath.compile(self.json_path)
 
     def __call__(self, value):
         """Query value for the jmespath query and return answer
         :param value: a data structure (dict, list) to extract from
         :return: Element extracted according to jmespath query
         """
@@ -222,12 +226,12 @@
     >>> proc(['one', 'two', 'three'])
     'one two three'
     >>> proc = Join('<br>')
     >>> proc(['one', 'two', 'three'])
     'one<br>two<br>three'
     """
 
-    def __init__(self, separator=' '):
+    def __init__(self, separator=" "):
         self.separator = separator
 
     def __call__(self, values):
         return self.separator.join(values)
```

### Comparing `itemloaders-1.0.6/itemloaders.egg-info/PKG-INFO` & `itemloaders-1.1.0/itemloaders.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: itemloaders
-Version: 1.0.6
+Version: 1.1.0
 Summary: Base library for scrapy's ItemLoader
 Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte
 Author-email: opensource@zyte.com
 License: BSD
 Project-URL: Documentation, https://itemloaders.readthedocs.io/
 Project-URL: Source, https://github.com/scrapy/itemloaders
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===========
 itemloaders
 ===========
 
@@ -96,8 +96,9 @@
   `Pull Requests here <https://github.com/scrapy/itemloaders/pulls>`_
 
 * If you want to submit a code change
 
    * File an `issue here <https://github.com/scrapy/itemloaders/issues>`_, if there isn't one yet
    * Fork this repository
    * Create a branch to work on your changes
+   * Run `pre-commit install` to install pre-commit hooks
    * Push your local branch and submit a Pull Request
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: itemloaders Version: 1.0.6 Summary: Base library
+Metadata-Version: 2.1 Name: itemloaders Version: 1.1.0 Summary: Base library
 for scrapy's ItemLoader Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte Author-email: opensource@zyte.com License: BSD Project-URL:
 Documentation, https://itemloaders.readthedocs.io/ Project-URL: Source, https:/
 /github.com/scrapy/itemloaders Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Requires-Python: >=3.6
+Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/x-rst License-File: LICENSE ===========
 itemloaders =========== .. image:: https://img.shields.io/pypi/v/
 itemloaders.svg :target: https://pypi.python.org/pypi/itemloaders :alt: PyPI
 Version .. image:: https://img.shields.io/pypi/pyversions/itemloaders.svg :
 target: https://pypi.python.org/pypi/itemloaders :alt: Supported Python
 Versions .. image:: https://github.com/scrapy/itemloaders/workflows/CI/
 badge.svg?branch=master :target: https://github.com/scrapy/itemloaders/
@@ -42,9 +42,9 @@
 out the `documentation
 itemloaders.readthedocs.io/en/latest/>`_. Contributing ============ All
 contributions are welcome! * If you want to review some code, check open `Pull
 Requests here
 github.com/scrapy/itemloaders/pulls>`_ * If you want to submit a code change *
 File an `issue here
 github.com/scrapy/itemloaders/issues>`_, if there isn't one yet * Fork this
-repository * Create a branch to work on your changes * Push your local branch
-and submit a Pull Request
+repository * Create a branch to work on your changes * Run `pre-commit install`
+to install pre-commit hooks * Push your local branch and submit a Pull Request
```

### Comparing `itemloaders-1.0.6/setup.py` & `itemloaders-1.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
-with open('README.rst') as f:
+with open("README.rst") as f:
     long_description = f.read()
 
 setup(
-    name='itemloaders',
-    version='1.0.6',
-    url='https://github.com/scrapy/itemloaders',
+    name="itemloaders",
+    version="1.1.0",
+    url="https://github.com/scrapy/itemloaders",
     project_urls={
-        'Documentation': 'https://itemloaders.readthedocs.io/',
-        'Source': 'https://github.com/scrapy/itemloaders',
+        "Documentation": "https://itemloaders.readthedocs.io/",
+        "Source": "https://github.com/scrapy/itemloaders",
     },
     description="Base library for scrapy's ItemLoader",
     long_description=long_description,
     long_description_content_type="text/x-rst",
-    author='Zyte',
-    author_email='opensource@zyte.com',
-    license='BSD',
-    packages=find_packages(exclude=('tests', 'tests.*')),
+    author="Zyte",
+    author_email="opensource@zyte.com",
+    license="BSD",
+    packages=find_packages(exclude=("tests", "tests.*")),
     include_package_data=True,
     zip_safe=False,
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: BSD License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
     ],
-    python_requires='>=3.6',
+    python_requires=">=3.7",
     install_requires=[
         # before updating these versions, be sure they are not higher than
         # scrapy's requirements
-        'w3lib>=1.17.0',
-        'parsel>=1.5.0',
-        'jmespath>=0.9.5',
-        'itemadapter>=0.1.0',
+        "w3lib>=1.17.0",
+        "parsel>=1.5.0",
+        "jmespath>=0.9.5",
+        "itemadapter>=0.1.0",
     ],
     # extras_require=extras_require,
 )
```

