# Comparing `tmp/lektor-responsive-image-0.1a1.tar.gz` & `tmp/lektor-responsive-image-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpr2mgjsg8/tmpxp6d7brs/lektor-responsive-image-0.1a1.tar", last modified: Sat Feb 13 23:55:38 2021, max compression
+gzip compressed data, was "lektor-responsive-image-1.0.0b1.tar", last modified: Fri Apr 21 02:07:46 2023, max compression
```

## Comparing `lektor-responsive-image-0.1a1.tar` & `lektor-responsive-image-1.0.0b1.tar`

### file list

```diff
@@ -1,44 +1,40 @@
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/.github/
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/.github/workflows/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      526 2021-02-13 23:46:38.000000 lektor-responsive-image-0.1a1/.github/workflows/tests.yml
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       53 2021-02-13 23:44:18.000000 lektor-responsive-image-0.1a1/.gitignore
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       89 2021-02-13 23:54:50.000000 lektor-responsive-image-0.1a1/CHANGES.md
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1062 2021-02-13 23:44:18.000000 lektor-responsive-image-0.1a1/LICENSE
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      165 2021-02-13 23:44:18.000000 lektor-responsive-image-0.1a1/MANIFEST.in
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     5181 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/PKG-INFO
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     3212 2021-02-13 23:52:56.000000 lektor-responsive-image-0.1a1/README.md
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/lektor_responsive_image.egg-info/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     5181 2021-02-13 23:55:38.000000 lektor-responsive-image-0.1a1/lektor_responsive_image.egg-info/PKG-INFO
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      850 2021-02-13 23:55:38.000000 lektor-responsive-image-0.1a1/lektor_responsive_image.egg-info/SOURCES.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)        1 2021-02-13 23:55:38.000000 lektor-responsive-image-0.1a1/lektor_responsive_image.egg-info/dependency_links.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       83 2021-02-13 23:55:38.000000 lektor-responsive-image-0.1a1/lektor_responsive_image.egg-info/entry_points.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       24 2021-02-13 23:55:38.000000 lektor-responsive-image-0.1a1/lektor_responsive_image.egg-info/top_level.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     5532 2021-02-13 23:04:19.000000 lektor-responsive-image-0.1a1/lektor_responsive_image.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      146 2021-02-13 23:44:18.000000 lektor-responsive-image-0.1a1/pyproject.toml
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1226 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/setup.cfg
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       57 2021-02-13 23:44:18.000000 lektor-responsive-image-0.1a1/setup.py
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/tests/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1011 2021-02-13 23:04:06.000000 lektor-responsive-image-0.1a1/tests/conftest.py
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/tests/test-site/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       27 2021-02-13 23:04:06.000000 lektor-responsive-image-0.1a1/tests/test-site/Test Site.lektorproject
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/tests/test-site/assets/
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/tests/test-site/assets/static/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      538 2021-02-13 23:04:06.000000 lektor-responsive-image-0.1a1/tests/test-site/assets/static/style.css
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/tests/test-site/content/
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/tests/test-site/content/about/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      144 2021-02-13 23:04:06.000000 lektor-responsive-image-0.1a1/tests/test-site/content/about/contents.lr
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      135 2021-02-13 23:04:06.000000 lektor-responsive-image-0.1a1/tests/test-site/content/contents.lr
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)    13264 2021-02-13 23:04:06.000000 lektor-responsive-image-0.1a1/tests/test-site/content/dummy.pdf
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/tests/test-site/content/projects/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       96 2021-02-13 23:04:06.000000 lektor-responsive-image-0.1a1/tests/test-site/content/projects/contents.lr
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)    69568 2021-02-13 23:04:06.000000 lektor-responsive-image-0.1a1/tests/test-site/content/test.jpg
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/tests/test-site/models/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      133 2021-02-13 23:04:06.000000 lektor-responsive-image-0.1a1/tests/test-site/models/page.ini
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/tests/test-site/templates/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      804 2021-02-13 23:04:06.000000 lektor-responsive-image-0.1a1/tests/test-site/templates/layout.html
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-13 23:55:38.106504 lektor-responsive-image-0.1a1/tests/test-site/templates/macros/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      475 2021-02-13 23:04:06.000000 lektor-responsive-image-0.1a1/tests/test-site/templates/macros/pagination.html
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      154 2021-02-13 23:04:06.000000 lektor-responsive-image-0.1a1/tests/test-site/templates/page.html
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     6530 2021-02-13 23:42:40.000000 lektor-responsive-image-0.1a1/tests/test_plugin.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      849 2021-02-13 23:47:13.000000 lektor-responsive-image-0.1a1/tox.ini
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:07:46.803563 lektor-responsive-image-1.0.0b1/
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       53 2021-02-13 23:44:18.000000 lektor-responsive-image-1.0.0b1/.gitignore
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      239 2023-04-21 02:04:20.000000 lektor-responsive-image-1.0.0b1/CHANGES.md
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1062 2021-02-13 23:44:18.000000 lektor-responsive-image-1.0.0b1/LICENSE
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       15 2023-04-20 22:56:57.000000 lektor-responsive-image-1.0.0b1/MANIFEST.in
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     5709 2023-04-21 02:07:46.803563 lektor-responsive-image-1.0.0b1/PKG-INFO
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     3216 2021-12-17 16:54:41.000000 lektor-responsive-image-1.0.0b1/README.md
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:07:46.799563 lektor-responsive-image-1.0.0b1/lektor_responsive_image.egg-info/
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     5709 2023-04-21 02:07:46.000000 lektor-responsive-image-1.0.0b1/lektor_responsive_image.egg-info/PKG-INFO
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      803 2023-04-21 02:07:46.000000 lektor-responsive-image-1.0.0b1/lektor_responsive_image.egg-info/SOURCES.txt
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)        1 2023-04-21 02:07:46.000000 lektor-responsive-image-1.0.0b1/lektor_responsive_image.egg-info/dependency_links.txt
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       82 2023-04-21 02:07:46.000000 lektor-responsive-image-1.0.0b1/lektor_responsive_image.egg-info/entry_points.txt
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       24 2023-04-21 02:07:46.000000 lektor-responsive-image-1.0.0b1/lektor_responsive_image.egg-info/top_level.txt
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     5791 2023-04-21 01:19:47.000000 lektor-responsive-image-1.0.0b1/lektor_responsive_image.py
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1692 2023-04-21 01:21:51.000000 lektor-responsive-image-1.0.0b1/pyproject.toml
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       38 2023-04-21 02:07:46.803563 lektor-responsive-image-1.0.0b1/setup.cfg
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:07:46.803563 lektor-responsive-image-1.0.0b1/tests/
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1164 2023-04-21 01:13:17.000000 lektor-responsive-image-1.0.0b1/tests/conftest.py
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:07:46.803563 lektor-responsive-image-1.0.0b1/tests/test-site/
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       27 2021-02-13 23:04:06.000000 lektor-responsive-image-1.0.0b1/tests/test-site/Test Site.lektorproject
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:07:46.799563 lektor-responsive-image-1.0.0b1/tests/test-site/assets/
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:07:46.803563 lektor-responsive-image-1.0.0b1/tests/test-site/assets/static/
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      538 2021-02-13 23:04:06.000000 lektor-responsive-image-1.0.0b1/tests/test-site/assets/static/style.css
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:07:46.803563 lektor-responsive-image-1.0.0b1/tests/test-site/content/
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:07:46.803563 lektor-responsive-image-1.0.0b1/tests/test-site/content/about/
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      144 2021-02-13 23:04:06.000000 lektor-responsive-image-1.0.0b1/tests/test-site/content/about/contents.lr
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      135 2021-02-13 23:04:06.000000 lektor-responsive-image-1.0.0b1/tests/test-site/content/contents.lr
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)    13264 2021-02-13 23:04:06.000000 lektor-responsive-image-1.0.0b1/tests/test-site/content/dummy.pdf
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:07:46.803563 lektor-responsive-image-1.0.0b1/tests/test-site/content/projects/
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       96 2021-02-13 23:04:06.000000 lektor-responsive-image-1.0.0b1/tests/test-site/content/projects/contents.lr
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)    69568 2021-02-13 23:04:06.000000 lektor-responsive-image-1.0.0b1/tests/test-site/content/test.jpg
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:07:46.803563 lektor-responsive-image-1.0.0b1/tests/test-site/models/
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      133 2021-02-13 23:04:06.000000 lektor-responsive-image-1.0.0b1/tests/test-site/models/page.ini
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:07:46.803563 lektor-responsive-image-1.0.0b1/tests/test-site/templates/
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      804 2021-02-13 23:04:06.000000 lektor-responsive-image-1.0.0b1/tests/test-site/templates/layout.html
+drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:07:46.803563 lektor-responsive-image-1.0.0b1/tests/test-site/templates/macros/
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      475 2021-02-13 23:04:06.000000 lektor-responsive-image-1.0.0b1/tests/test-site/templates/macros/pagination.html
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      154 2021-02-13 23:04:06.000000 lektor-responsive-image-1.0.0b1/tests/test-site/templates/page.html
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     7135 2023-04-21 01:19:47.000000 lektor-responsive-image-1.0.0b1/tests/test_plugin.py
+-rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1304 2023-04-21 01:19:47.000000 lektor-responsive-image-1.0.0b1/tox.ini
```

### Comparing `lektor-responsive-image-0.1a1/LICENSE` & `lektor-responsive-image-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `lektor-responsive-image-0.1a1/README.md` & `lektor-responsive-image-1.0.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 This plugin also registers a Jinja global function named `responsive_image`.
 It expects a single argument, which should be an `Image` instance.
 It returns an object which has an `.attr` attribute whose value is
 a dict of attribute which could be set on an `<img>` tag to generate
 markup for a multi-resolution image.  E.g.
 
-```jinja2
+```html+jinja
 {% set image = this.attachments.get('figure.png') %}
 {% set img_attrs = responsive_image(image).attrs %}
 <figure class="figure">
   <img class="figure-img" {{ img_attrs|xmlattr }}>
   <figcaption class="figure-caption text-center">
     {{- this.caption -}}
   </figcaption>
```

### Comparing `lektor-responsive-image-0.1a1/lektor_responsive_image.egg-info/SOURCES.txt` & `lektor-responsive-image-1.0.0b1/lektor_responsive_image.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 .gitignore
 CHANGES.md
 LICENSE
 MANIFEST.in
 README.md
 lektor_responsive_image.py
 pyproject.toml
-setup.cfg
-setup.py
 tox.ini
-.github/workflows/tests.yml
 lektor_responsive_image.egg-info/PKG-INFO
 lektor_responsive_image.egg-info/SOURCES.txt
 lektor_responsive_image.egg-info/dependency_links.txt
 lektor_responsive_image.egg-info/entry_points.txt
 lektor_responsive_image.egg-info/top_level.txt
 tests/conftest.py
 tests/test_plugin.py
```

### Comparing `lektor-responsive-image-0.1a1/lektor_responsive_image.py` & `lektor-responsive-image-1.0.0b1/lektor_responsive_image.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,44 @@
-# -*- coding: utf-8 -*-
-from functools import wraps
-import inspect
-try:
-    from urllib.parse import urlparse
-except ImportError:             # pragma: no cover
-    from urlparse import urlparse
+import sys
+from urllib.parse import urlparse
 
+import mistune
 from lektor.context import get_ctx
 from lektor.db import Image
-from lektor.pluginsystem import (
-    Plugin,
-    get_plugin,
-    )
+from lektor.pluginsystem import get_plugin
+from lektor.pluginsystem import Plugin
 from lektor.utils import join_path
 from markupsafe import escape
 from werkzeug.utils import cached_property
 
+HAVE_MISTUNE0 = mistune.__version__.startswith("0.")
 
-def ignore_unsupported_kwargs(f):
-    getargspec = inspect.getfullargspec if hasattr(inspect, 'getfullargspec') \
-                 else inspect.getargspec
-    supported_args = getargspec(f).args
-
-    @wraps(f)
-    def wrapped(*args, **kwargs):
-        supported_kwargs = set(supported_args[len(args):]).intersection(kwargs)
-        return f(*args, **{k: kwargs[k] for k in supported_kwargs})
-    return wrapped
+try:
+    from lektor.markdown import controller_class
+except ImportError:
+    # Lektor < 3.4
+    from lektor.markdown import ImprovedRenderer
+    from lektor.markdown import MarkdownConfig
+else:
+    # Lektor >= 3.4
+    _mistune_module = sys.modules[controller_class.__module__]
+    ImprovedRenderer = _mistune_module.ImprovedRenderer
+    MarkdownConfig = _mistune_module.MarkdownConfig
 
 
 def fmt_attrs(attrs):
-    return ' '.join('{}="{}"'.format(key, escape(val))
+    """Format a dict to markup suitable for use as HTML tag attributes."""
+    return ' '.join(f'{key}="{escape(val)}"'
                     for key, val in attrs.items()
                     if val is not None)
 
 
-class ResponsiveImage(object):
+class ResponsiveImage:
+    """Helper class to compute attributes for multi-resolution responsive images.
+    """
     DEFAULT_CONFIG = {
         'widths': [480, 800, 1200, 2400],
         'quality': 92,
         'default_width': 1200,
         'sizes': None,
         }
 
@@ -64,15 +63,15 @@
     @cached_property
     def srcset(self):
         url_to = self.ctx.url_to
         widths = list(self.iter_widths())
         if len(widths) > 1:
             def image_info(width):
                 image = self.resize_image(width)
-                return "{url} {width}w".format(url=url_to(image), width=width)
+                return f"{url_to(image)} {width}w"
             return ', '.join(map(image_info, self.iter_widths()))
 
     @property
     def sizes(self):
         return self.config.get('sizes')
 
     def iter_widths(self):
@@ -96,19 +95,19 @@
 
     def resize_image(self, width):
         image = self.image
         if width is None or width >= image.width:
             return image
         # We (should) never upscale.  Upscale=True is passed here
         # solely to avoid triggering a deprecation warning.
-        thumbnail = ignore_unsupported_kwargs(self.image.thumbnail)
-        return thumbnail(width, quality=self.config['quality'], upscale=True)
+        return self.image.thumbnail(width, quality=self.config['quality'], upscale=True)
 
 
 def resolve_image(record, src):
+    """Resolve local image URL to Lektor Image record."""
     if record is None:
         return None
     url = urlparse(src)
     if url.scheme or url.netloc:
         return None
 
     path = url.path
@@ -116,33 +115,38 @@
         assert record.path is not None   # FIXME: better error reporting?
         path = join_path(record.path, path)
     source = record.pad.get(path)
     if isinstance(source, Image):
         return source
 
 
-class ResponsiveImageMixin(object):
-    """Render markdown images at responsive resolutions (using srcset).
-
+class ResponsiveImageMixin:
+    """Markdown renderer mixin to render local images at multiple resolutions.
     """
 
-    def image(self, src, title, text):
-        image = resolve_image(self.record, src)
+    def image(self, src, *args):
+        # Under Lektor >= 3.4, the record is available at self.lektor.record.
+        # Prior to that, it's at self.record.
+        renderer_helper = getattr(self, "lektor", self)
+        record = renderer_helper.record
+
+        image = resolve_image(record, src)
         if image is not None and image.format in ('png', 'gif', 'jpeg'):
-            plugin = get_plugin('responsive-image', env=self.record.pad.env)
-            attrs = {'alt': text, 'title': title or None}
+            alt, title = reversed(args) if HAVE_MISTUNE0 else args
+            attrs = {'alt': alt, 'title': title or None}
+            plugin = get_plugin('responsive-image', env=record.pad.env)
             attrs.update(plugin.responsive_image(image).attrs)
-            return "<img {}>".format(fmt_attrs(attrs))
+            return f"<img {fmt_attrs(attrs)}>"
         else:
-            return super(ResponsiveImageMixin, self).image(src, title, text)
+            return super().image(src, *args)
 
 
 class ResponsiveImagePlugin(Plugin):
     name = 'Responsive Image'
-    description = u'Support for responsive-resolutioned images.'
+    description = 'Support for multi-resolution responsive images.'
 
     def on_setup_env(self, **extra):
         self.env.jinja_env.globals['responsive_image'] = self.responsive_image
 
     def on_markdown_config(self, config, **extra):
         config.renderer_mixins.append(ResponsiveImageMixin)
```

### Comparing `lektor-responsive-image-0.1a1/tests/conftest.py` & `lektor-responsive-image-1.0.0b1/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# -*- coding: utf-8 -*-
 import os
+from contextlib import ExitStack
 
 import pytest
-
 from lektor.builder import Builder
 from lektor.context import Context
 from lektor.project import Project
 
 
 @pytest.fixture
 def lektor_env():
@@ -22,15 +21,18 @@
 @pytest.fixture
 def lektor_builder(lektor_pad, tmp_path):
     return Builder(lektor_pad, str(tmp_path))
 
 
 @pytest.fixture
 def lektor_build_state(lektor_builder):
-    with lektor_builder.new_build_state() as build_state:
+    build_state = lektor_builder.new_build_state()
+    with ExitStack() as stack:
+        if hasattr(build_state, "__enter__"):
+            build_state = stack.enter_context(build_state)  # lektor < 3.4
         yield build_state
 
 
 @pytest.fixture
 def lektor_source(lektor_pad):
     return lektor_pad.root
```

### Comparing `lektor-responsive-image-0.1a1/tests/test-site/assets/static/style.css` & `lektor-responsive-image-1.0.0b1/tests/test-site/assets/static/style.css`

 * *Files identical despite different names*

### Comparing `lektor-responsive-image-0.1a1/tests/test-site/content/dummy.pdf` & `lektor-responsive-image-1.0.0b1/tests/test-site/content/dummy.pdf`

 * *Files identical despite different names*

### Comparing `lektor-responsive-image-0.1a1/tests/test-site/content/test.jpg` & `lektor-responsive-image-1.0.0b1/tests/test-site/content/test.jpg`

 * *Files identical despite different names*

### Comparing `lektor-responsive-image-0.1a1/tests/test-site/templates/layout.html` & `lektor-responsive-image-1.0.0b1/tests/test-site/templates/layout.html`

 * *Files identical despite different names*

### Comparing `lektor-responsive-image-0.1a1/tests/test_plugin.py` & `lektor-responsive-image-1.0.0b1/tests/test_plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-# -*- coding: utf-8 -*-
 import re
+from contextlib import ExitStack
 
 import pytest
-
 from inifile import IniFile
-from lektor.markdown import (
-    ImprovedRenderer,
-    MarkdownConfig,
-    )
-
-from lektor_responsive_image import (
-    ResponsiveImage,
-    resolve_image,
-    ResponsiveImageMixin,
-    ResponsiveImagePlugin,
-    )
+
+from lektor_responsive_image import HAVE_MISTUNE0
+from lektor_responsive_image import ImprovedRenderer
+from lektor_responsive_image import MarkdownConfig
+from lektor_responsive_image import resolve_image
+from lektor_responsive_image import ResponsiveImage
+from lektor_responsive_image import ResponsiveImageMixin
+from lektor_responsive_image import ResponsiveImagePlugin
+
+try:
+    from lektor.markdown.controller import RendererContext
+except ModuleNotFoundError:
+    RendererContext = None
 
 
-class DummyImage(object):
+class DummyImage:
     def __init__(self, width, height, format='jpeg', quality=None):
         self.width = width
         self.height = height
         self.format = format
         self.quality = quality
 
     def thumbnail(self, width, quality=None, upscale=None):
         height = int(self.height * width / self.width + 0.5)
         return DummyImage(width, height, format=self.format, quality=quality)
 
 
-class DummyContext(object):
+class DummyContext:
     def url_to(self, image):
-        return 'img-{}.jpg'.format(image.width)
+        return f'img-{image.width}.jpg'
 
 
-class TestResponsiveImage(object):
+class TestResponsiveImage:
     @pytest.fixture
     def width(self):
         return 2400
 
     @pytest.fixture
     def image(self, width):
         height = int(3 * width / 4)
@@ -100,15 +101,15 @@
         assert resp_image.resize_image(image.width) is image
         assert resp_image.resize_image(image.width + 1) is image
         resized = resp_image.resize_image(image.width - 1)
         assert resized.width == image.width - 1
         assert resized.quality == 92
 
 
-class Test_resolve_image(object):
+class Test_resolve_image:
     def test_no_record(self):
         assert resolve_image(None, 'test.jpg') is None
 
     def test_external_url(self, lektor_pad):
         assert resolve_image(lektor_pad.root,
                              'http://example.com/test.jpg') is None
 
@@ -133,42 +134,53 @@
 
 @pytest.fixture
 def load_plugin(lektor_env):
     lektor_env.plugin_controller.instanciate_plugin(
         'responsive-image', ResponsiveImagePlugin)
 
 
-class TestResponsiveImageMixin(object):
+class RendererWithMixin(ResponsiveImageMixin, ImprovedRenderer):
+    pass
+
+
+class TestResponsiveImageMixin:
     @pytest.fixture
     def record(self, lektor_pad):
         return lektor_pad.root
 
     @pytest.fixture
     def mixin(self, record):
-        class Renderer(ResponsiveImageMixin, ImprovedRenderer):
-            def __init__(self, record):
-                self.record = record
-        return Renderer(record)
+        with ExitStack() as stack:
+            renderer = RendererWithMixin()
+            if RendererContext is not None:
+                stack.enter_context(
+                    RendererContext(record, meta={}, field_options={})
+                )
+            else:  # lektor < 3.4
+                renderer.record = record
+            yield renderer
 
     @pytest.mark.usefixtures('load_plugin', 'lektor_context')
     def test(self, mixin):
-        img = mixin.image('test.jpg', 'TITLE', 'ALT')
+        args = ("TITLE", "ALT") if HAVE_MISTUNE0 else ("ALT", "TITLE")
+        img = mixin.image('test.jpg', *args)
         assert re.match(r'<img.*>', img)
         assert 'alt="ALT"' in img
         assert 'srcset=' in img
 
     @pytest.mark.usefixtures('load_plugin', 'lektor_context')
     def test_not_resolvable(self, mixin):
-        img = mixin.image('foo.jpg', 'TITLE', 'ALT')
+        args = ("TITLE", "ALT") if HAVE_MISTUNE0 else ("ALT", "TITLE")
+        img = mixin.image('foo.jpg', *args)
         assert re.match(r'<img.*>', img)
         assert 'alt="ALT"' in img
         assert 'srcset=' not in img
 
 
-class TestResponsiveImagePlugin(object):
+class TestResponsiveImagePlugin:
     @pytest.fixture
     def plugin(self, lektor_env):
         return ResponsiveImagePlugin(lektor_env, 'responsive-image')
 
     def test_on_setup_env(self, plugin, lektor_env):
         plugin.on_setup_env()
         jinja_globals = lektor_env.jinja_env.globals
```

