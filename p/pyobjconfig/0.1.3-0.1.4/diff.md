# Comparing `tmp/pyobjconfig-0.1.3.tar.gz` & `tmp/pyobjconfig-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjconfig-0.1.3.tar", last modified: Tue Apr 18 21:10:20 2023, max compression
+gzip compressed data, was "pyobjconfig-0.1.4.tar", last modified: Fri Apr 21 14:51:04 2023, max compression
```

## Comparing `pyobjconfig-0.1.3.tar` & `pyobjconfig-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 waltw     (1000) waltw     (1000)        0 2023-04-18 21:10:20.254562 pyobjconfig-0.1.3/
--rw-r--r--   0 waltw     (1000) waltw     (1000)     1067 2023-04-18 20:42:16.000000 pyobjconfig-0.1.3/LICENSE
--rw-r--r--   0 waltw     (1000) waltw     (1000)     3162 2023-04-18 21:10:20.254562 pyobjconfig-0.1.3/PKG-INFO
--rw-r--r--   0 waltw     (1000) waltw     (1000)     2871 2023-04-18 21:03:52.000000 pyobjconfig-0.1.3/README.md
-drwxr-xr-x   0 waltw     (1000) waltw     (1000)        0 2023-04-18 21:10:20.251229 pyobjconfig-0.1.3/pyobjconfig/
--rw-r--r--   0 waltw     (1000) waltw     (1000)      113 2023-04-18 20:42:16.000000 pyobjconfig-0.1.3/pyobjconfig/__init__.py
--rw-r--r--   0 waltw     (1000) waltw     (1000)    12438 2023-04-18 21:01:54.000000 pyobjconfig-0.1.3/pyobjconfig/common.py
--rw-r--r--   0 waltw     (1000) waltw     (1000)      844 2023-04-18 20:42:16.000000 pyobjconfig-0.1.3/pyobjconfig/torch.py
-drwxr-xr-x   0 waltw     (1000) waltw     (1000)        0 2023-04-18 21:10:20.254562 pyobjconfig-0.1.3/pyobjconfig.egg-info/
--rw-r--r--   0 waltw     (1000) waltw     (1000)     3162 2023-04-18 21:10:20.000000 pyobjconfig-0.1.3/pyobjconfig.egg-info/PKG-INFO
--rw-r--r--   0 waltw     (1000) waltw     (1000)      292 2023-04-18 21:10:20.000000 pyobjconfig-0.1.3/pyobjconfig.egg-info/SOURCES.txt
--rw-r--r--   0 waltw     (1000) waltw     (1000)        1 2023-04-18 21:10:20.000000 pyobjconfig-0.1.3/pyobjconfig.egg-info/dependency_links.txt
--rw-r--r--   0 waltw     (1000) waltw     (1000)        9 2023-04-18 21:10:20.000000 pyobjconfig-0.1.3/pyobjconfig.egg-info/requires.txt
--rw-r--r--   0 waltw     (1000) waltw     (1000)       12 2023-04-18 21:10:20.000000 pyobjconfig-0.1.3/pyobjconfig.egg-info/top_level.txt
--rw-r--r--   0 waltw     (1000) waltw     (1000)       38 2023-04-18 21:10:20.254562 pyobjconfig-0.1.3/setup.cfg
--rw-r--r--   0 waltw     (1000) waltw     (1000)      544 2023-04-18 21:03:57.000000 pyobjconfig-0.1.3/setup.py
-drwxr-xr-x   0 waltw     (1000) waltw     (1000)        0 2023-04-18 21:10:20.254562 pyobjconfig-0.1.3/test/
--rw-r--r--   0 waltw     (1000) waltw     (1000)     3418 2023-04-18 21:02:48.000000 pyobjconfig-0.1.3/test/test_pyobjconfig.py
+drwxr-xr-x   0 waltw     (1000) waltw     (1000)        0 2023-04-21 14:51:04.320670 pyobjconfig-0.1.4/
+-rw-r--r--   0 waltw     (1000) waltw     (1000)     1067 2023-04-18 20:42:16.000000 pyobjconfig-0.1.4/LICENSE
+-rw-r--r--   0 waltw     (1000) waltw     (1000)     3362 2023-04-21 14:51:04.320670 pyobjconfig-0.1.4/PKG-INFO
+-rw-r--r--   0 waltw     (1000) waltw     (1000)     3071 2023-04-21 14:50:29.000000 pyobjconfig-0.1.4/README.md
+drwxr-xr-x   0 waltw     (1000) waltw     (1000)        0 2023-04-21 14:51:04.320670 pyobjconfig-0.1.4/pyobjconfig/
+-rw-r--r--   0 waltw     (1000) waltw     (1000)      113 2023-04-18 20:42:16.000000 pyobjconfig-0.1.4/pyobjconfig/__init__.py
+-rw-r--r--   0 waltw     (1000) waltw     (1000)    13267 2023-04-21 14:48:25.000000 pyobjconfig-0.1.4/pyobjconfig/common.py
+-rw-r--r--   0 waltw     (1000) waltw     (1000)      844 2023-04-18 20:42:16.000000 pyobjconfig-0.1.4/pyobjconfig/torch.py
+drwxr-xr-x   0 waltw     (1000) waltw     (1000)        0 2023-04-21 14:51:04.320670 pyobjconfig-0.1.4/pyobjconfig.egg-info/
+-rw-r--r--   0 waltw     (1000) waltw     (1000)     3362 2023-04-21 14:51:04.000000 pyobjconfig-0.1.4/pyobjconfig.egg-info/PKG-INFO
+-rw-r--r--   0 waltw     (1000) waltw     (1000)      292 2023-04-21 14:51:04.000000 pyobjconfig-0.1.4/pyobjconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 waltw     (1000) waltw     (1000)        1 2023-04-21 14:51:04.000000 pyobjconfig-0.1.4/pyobjconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 waltw     (1000) waltw     (1000)        9 2023-04-21 14:51:04.000000 pyobjconfig-0.1.4/pyobjconfig.egg-info/requires.txt
+-rw-r--r--   0 waltw     (1000) waltw     (1000)       12 2023-04-21 14:51:04.000000 pyobjconfig-0.1.4/pyobjconfig.egg-info/top_level.txt
+-rw-r--r--   0 waltw     (1000) waltw     (1000)       38 2023-04-21 14:51:04.320670 pyobjconfig-0.1.4/setup.cfg
+-rw-r--r--   0 waltw     (1000) waltw     (1000)      544 2023-04-21 14:49:32.000000 pyobjconfig-0.1.4/setup.py
+drwxr-xr-x   0 waltw     (1000) waltw     (1000)        0 2023-04-21 14:51:04.320670 pyobjconfig-0.1.4/test/
+-rw-r--r--   0 waltw     (1000) waltw     (1000)     3988 2023-04-21 14:41:16.000000 pyobjconfig-0.1.4/test/test_pyobjconfig.py
```

### Comparing `pyobjconfig-0.1.3/LICENSE` & `pyobjconfig-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobjconfig-0.1.3/PKG-INFO` & `pyobjconfig-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjconfig
-Version: 0.1.3
+Version: 0.1.4
 Summary: An argparse+pydantic-based configuration system for Python.
 Home-page: https://github.com/wwoods/pyobjconfig
 Author: Walt Woods
 Author-email: woodswalben@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -83,9 +83,10 @@
 
 ## Usage with pytorch
 
 Pytorch overrides `__setattr__` in a way that is incompatible with the `ConfigurableObject` class provided by `pyobjconfig`. To work around this, use the `pyobjconfig.torch.ConfigurableModule` as a drop-in replacement for `torch.nn.Module`.
 
 
 # Changelog
+* 2023-04-21 - v0.1.4. `argparse.ArgumentParser` has `type` specified for each argument now, so local equality comparisons against previous `argparse_hparams()` before object instantiation will work.
 * 2023-04-18 - v0.1.3. Disallow `None` as parameter values because it serializes poorly, and disallow abbreviated parameter matches to avoid confusion.
 * 2021-01-14 - v0.1.2. Support lists on the command line.
```

### Comparing `pyobjconfig-0.1.3/README.md` & `pyobjconfig-0.1.4/pyobjconfig.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: pyobjconfig
+Version: 0.1.4
+Summary: An argparse+pydantic-based configuration system for Python.
+Home-page: https://github.com/wwoods/pyobjconfig
+Author: Walt Woods
+Author-email: woodswalben@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pyobjconfig
 
 `pyobjconfig` is a module suite designed with Machine Learning (ML) experiments in mind, but should work for a broad range of hierarchical configurations.
 
 ## Example usage
 
 Pyobjconfig supports configuring nested objects, such that each object has control over its own configuration:
@@ -73,9 +83,10 @@
 
 ## Usage with pytorch
 
 Pytorch overrides `__setattr__` in a way that is incompatible with the `ConfigurableObject` class provided by `pyobjconfig`. To work around this, use the `pyobjconfig.torch.ConfigurableModule` as a drop-in replacement for `torch.nn.Module`.
 
 
 # Changelog
+* 2023-04-21 - v0.1.4. `argparse.ArgumentParser` has `type` specified for each argument now, so local equality comparisons against previous `argparse_hparams()` before object instantiation will work.
 * 2023-04-18 - v0.1.3. Disallow `None` as parameter values because it serializes poorly, and disallow abbreviated parameter matches to avoid confusion.
 * 2021-01-14 - v0.1.2. Support lists on the command line.
```

### Comparing `pyobjconfig-0.1.3/pyobjconfig/common.py` & `pyobjconfig-0.1.4/pyobjconfig/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,16 +164,30 @@
             for k, v in cls.config.schema()['properties'].items():
                 if k.startswith('_'): continue
                 name = f'{prefix}{k}'
                 help = props.get(k) or ''
                 if 'default' in v:
                     help = help + f'  Default: {v["default"]}'
                 kw = {}
-                if v.get('type') == 'array':
+                if v.get('type') == 'array' and v.get('items', {}).get('type') == 'string':
+                    # To allow strings with a comma, do NOT use comma-separated
+                    # for this.
                     kw['action'] = 'append'
+                else:
+                    # Rely on pydantic type conversion
+                    v_field = cls.config.__fields__[k]
+                    def convert_str_to_type(arg, *, v=v, v_field=v_field):
+                        if v.get('type') == 'array':
+                            # Convert to comma-separated-list; 1-d only
+                            if arg.startswith('['):
+                                assert arg.endswith(']')
+                                arg = arg[1:-1]
+                            arg = arg.split(',')
+                        return pydantic.parse_obj_as(v_field.outer_type_, arg)
+                    kw['type'] = convert_str_to_type
                 parser.add_argument(f'--{name}', dest=name, help=help, **kw)
         for k in dir(cls):
             v = getattr(cls, k)
             if type(v) is type and issubclass(v, ConfigurableObject):
                 v._argparse_setup(prefix + k + '-', parser)
```

### Comparing `pyobjconfig-0.1.3/pyobjconfig/torch.py` & `pyobjconfig-0.1.4/pyobjconfig/torch.py`

 * *Files identical despite different names*

### Comparing `pyobjconfig-0.1.3/pyobjconfig.egg-info/PKG-INFO` & `pyobjconfig-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: pyobjconfig
-Version: 0.1.3
-Summary: An argparse+pydantic-based configuration system for Python.
-Home-page: https://github.com/wwoods/pyobjconfig
-Author: Walt Woods
-Author-email: woodswalben@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pyobjconfig
 
 `pyobjconfig` is a module suite designed with Machine Learning (ML) experiments in mind, but should work for a broad range of hierarchical configurations.
 
 ## Example usage
 
 Pyobjconfig supports configuring nested objects, such that each object has control over its own configuration:
@@ -83,9 +73,10 @@
 
 ## Usage with pytorch
 
 Pytorch overrides `__setattr__` in a way that is incompatible with the `ConfigurableObject` class provided by `pyobjconfig`. To work around this, use the `pyobjconfig.torch.ConfigurableModule` as a drop-in replacement for `torch.nn.Module`.
 
 
 # Changelog
+* 2023-04-21 - v0.1.4. `argparse.ArgumentParser` has `type` specified for each argument now, so local equality comparisons against previous `argparse_hparams()` before object instantiation will work.
 * 2023-04-18 - v0.1.3. Disallow `None` as parameter values because it serializes poorly, and disallow abbreviated parameter matches to avoid confusion.
 * 2021-01-14 - v0.1.2. Support lists on the command line.
```

### Comparing `pyobjconfig-0.1.3/setup.py` & `pyobjconfig-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md') as f:
     long_desc = f.read()
 
 setuptools.setup(
         name='pyobjconfig',
-        version='0.1.3',
+        version='0.1.4',
         author='Walt Woods',
         author_email='woodswalben@gmail.com',
         description="An argparse+pydantic-based configuration system for Python.",
         long_description=long_desc,
         long_description_content_type='text/markdown',
         url='https://github.com/wwoods/pyobjconfig',
         packages=setuptools.find_packages(),
```

### Comparing `pyobjconfig-0.1.3/test/test_pyobjconfig.py` & `pyobjconfig-0.1.4/test/test_pyobjconfig.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     obj = BaseObject.argparse_create(args)
     assert obj.config.a == 99
 
     args = ap.parse_args(['--b', 'yodel']).__dict__
     obj = BaseObject.argparse_create(args)
     assert obj.config.b == 'yodel'
 
-    with pytest.raises(TypeError) as exc:
+    with pytest.raises(SystemExit) as exc:
         args = ap.parse_args(['--a', 'yodel']).__dict__
         print(args)
         obj = BaseObject.argparse_create(args)
 
 
 def test_default_none():
     """Ensure that an object with a default value of None MUST be overridden.
@@ -92,26 +92,49 @@
         assert b.config.test == 'yay!'
         b = Base.argparse_create({}, env='BLEEP2')
         assert b.config.test == 'testing'
     finally:
         os.environ = old
 
 
-def test_list():
+def test_parse_types():
+    '''Ensure that types coming from argparse are correct, rather than relying
+    on pydantic.
+    '''
     class A(ConfigurableObject):
         class config(PydanticBaseModel):
-            thing: typing.List[int] = [1]
+            a: int
+            b: float
+            c: typing.List[int]
+            c2: typing.List[float]
+            c3: typing.List[str]
+            d: str
 
-    ap = argparse.ArgumentParser(description=__doc__)
+    ap = argparse.ArgumentParser()
     A.argparse_setup(ap)
+    args = ap.parse_args(['--a', '1', '--b', '2', '--c', '[1, 2, 3]',
+            '--c2', '1., 2.5, 3', '--c3', 'a,', '--c3', 'b', '--d', '4'])
+    assert args.a == 1
+    assert isinstance(args.a, int)
+
+    assert args.b == 2
+    assert isinstance(args.b, float)
+
+    assert args.c == [1, 2, 3]
+    assert isinstance(args.c, list)
+    assert isinstance(args.c[0], int)
+
+    assert args.c2 == [1., 2.5, 3.]
+    assert isinstance(args.c2, list)
+    assert isinstance(args.c2[0], float)
 
-    args = A.argparse_create(ap.parse_args([]).__dict__)
-    assert args.config.thing == [1]
-    args = A.argparse_create(ap.parse_args(['--thing', '2', '--thing', '3']).__dict__)
-    assert args.config.thing == [2, 3]
+    assert args.c3 == ['a,', 'b']
+
+    assert args.d == '4'
+    assert isinstance(args.d, str)
 
 
 def test_prefix():
     class A(ConfigurableObject):
         class B(ConfigurableObject):
             class config(PydanticBaseModel):
                 lr_value: float = 1
```

