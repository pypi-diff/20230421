# Comparing `tmp/taskiq_dependencies-1.1.2.tar.gz` & `tmp/taskiq_dependencies-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_dependencies-1.1.2.tar", max compression
+gzip compressed data, was "taskiq_dependencies-1.2.0.tar", max compression
```

## Comparing `taskiq_dependencies-1.1.2.tar` & `taskiq_dependencies-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2841 2023-03-26 14:51:57.103051 taskiq_dependencies-1.1.2/README.md
--rw-r--r--   0        0        0     1621 2023-03-26 14:51:57.103051 taskiq_dependencies-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      325 2023-03-26 14:51:57.103051 taskiq_dependencies-1.1.2/taskiq_dependencies/__init__.py
--rw-r--r--   0        0        0     9106 2023-03-26 14:51:57.103051 taskiq_dependencies-1.1.2/taskiq_dependencies/ctx.py
--rw-r--r--   0        0        0     3084 2023-03-26 14:51:57.103051 taskiq_dependencies-1.1.2/taskiq_dependencies/dependency.py
--rw-r--r--   0        0        0     6966 2023-03-26 14:51:57.103051 taskiq_dependencies-1.1.2/taskiq_dependencies/graph.py
--rw-r--r--   0        0        0        0 2023-03-26 14:51:57.103051 taskiq_dependencies-1.1.2/taskiq_dependencies/py.typed
--rw-r--r--   0        0        0     3973 1970-01-01 00:00:00.000000 taskiq_dependencies-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3539 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/README.md
+-rw-r--r--   0        0        0     1621 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      386 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/taskiq_dependencies/__init__.py
+-rw-r--r--   0        0        0     9648 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/taskiq_dependencies/ctx.py
+-rw-r--r--   0        0        0     3189 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/taskiq_dependencies/dependency.py
+-rw-r--r--   0        0        0     7257 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/taskiq_dependencies/graph.py
+-rw-r--r--   0        0        0        0 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/taskiq_dependencies/py.typed
+-rw-r--r--   0        0        0      573 2023-04-20 22:54:44.095250 taskiq_dependencies-1.2.0/taskiq_dependencies/utils.py
+-rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 taskiq_dependencies-1.2.0/PKG-INFO
```

### Comparing `taskiq_dependencies-1.1.2/README.md` & `taskiq_dependencies-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -93,7 +93,35 @@
 
 with graph.sync_ctx({DefaultDep: DefaultDep()}) as ctx:
     print(ctx.resolve_kwargs())
 
 ```
 
 You can run this code. It will resolve dd dependency into a `DefaultDep` variable you provide.
+
+
+## Getting parameters information
+
+If you want to get the information about how this dependency was specified,
+you can use special class `ParamInfo` for that.
+
+```python
+from taskiq_dependencies import Depends, DependencyGraph, ParamInfo
+
+
+def dependency(info: ParamInfo = Depends()) -> str:
+    assert info.name == "dd"
+    return info.name
+
+def target_func(dd: str = Depends(dependency)):
+    print(dd)
+    return 1
+
+
+graph = DependencyGraph(target_func)
+
+with graph.sync_ctx() as ctx:
+    print(ctx.resolve_kwargs())
+
+```
+
+The ParamInfo has the information about name and parameters signature. It's useful if you want to create a dependency that changes based on parameter name, or signature.
```

### Comparing `taskiq_dependencies-1.1.2/pyproject.toml` & `taskiq_dependencies-1.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq-dependencies"
-version = "1.1.2"
+version = "1.2.0"
 description = "FastAPI like dependency injection implementation"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 packages = [{include = "taskiq_dependencies"}]
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
```

### Comparing `taskiq_dependencies-1.1.2/taskiq_dependencies/ctx.py` & `taskiq_dependencies-1.2.0/taskiq_dependencies/ctx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import asyncio
 import inspect
 from copy import copy
 from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional
 
+from taskiq_dependencies.utils import ParamInfo
+
 if TYPE_CHECKING:
     from taskiq_dependencies.graph import DependencyGraph  # pragma: no cover
 
 
 class BaseResolveContext:
     """Base resolver context."""
 
@@ -58,14 +60,19 @@
             # Now we get list of dependencies for current top-level dependency
             # and iterate over it.
             for subdep in self.graph.dependencies[dep]:
                 # If we don't have known dependency function,
                 # we skip it.
                 if subdep.dependency is None:
                     continue
+                # If the user want to get ParamInfo,
+                # we get declaration of the current dependency.
+                if subdep.dependency == ParamInfo:
+                    kwargs[subdep.param_name] = ParamInfo(dep.param_name, dep.signature)
+                    continue
                 if subdep.use_cache:
                     # If this dependency can be calculated, using cache,
                     # we try to get it from cache.
                     kwargs[subdep.param_name] = cache[subdep.dependency]
                 else:
                     # If this dependency doesn't use cache,
                     # we resolve it's dependencies and
@@ -78,15 +85,20 @@
                         resolved_kwargs.update(subdep.kwargs)
                     kwargs[subdep.param_name] = yield subdep.dependency(
                         **resolved_kwargs,
                     )
 
             # We don't want to calculate least function,
             # Because it's a target function.
-            if index < len(self.graph.ordered_deps) - 1:
+            if (  # noqa: WPS337
+                index < len(self.graph.ordered_deps) - 1
+                # We skip all ParamInfo dependencies,
+                # because we calculate them when needed.
+                and dep.dependency != ParamInfo
+            ):
                 user_kwargs = dep.kwargs
                 user_kwargs.update(kwargs)
                 cache[dep.dependency] = yield dep.dependency(**user_kwargs)
         return kwargs
 
 
 class SyncResolveContext(BaseResolveContext):
```

### Comparing `taskiq_dependencies-1.1.2/taskiq_dependencies/dependency.py` & `taskiq_dependencies-1.2.0/taskiq_dependencies/dependency.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import uuid
 from typing import (  # noqa: WPS235
     Any,
     AsyncGenerator,
     Callable,
     Coroutine,
     Dict,
@@ -103,20 +104,22 @@
 
     def __init__(  # noqa: WPS234
         self,
         dependency: Optional[Union[Type[Any], Callable[..., Any]]] = None,
         *,
         use_cache: bool = True,
         kwargs: Optional[Dict[str, Any]] = None,
+        signature: Optional[inspect.Parameter] = None,
     ) -> None:
         self._id = uuid.uuid4()
         self.dependency = dependency
         self.use_cache = use_cache
         self.param_name = ""
         self.kwargs = kwargs or {}
+        self.signature = signature
 
     def __hash__(self) -> int:
         return hash(self._id)
 
     def __eq__(self, rhs: object) -> bool:
         """
         Overriden eq operation.
```

### Comparing `taskiq_dependencies-1.1.2/taskiq_dependencies/graph.py` & `taskiq_dependencies-1.2.0/taskiq_dependencies/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,17 +96,21 @@
                 continue
             # Get signature and type hints.
             sign = inspect.signature(dep.dependency)
             if inspect.isclass(dep.dependency):
                 # If this is a class, we need to get signature of
                 # an __init__ method.
                 hints = get_type_hints(dep.dependency.__init__)  # noqa: WPS609
-            else:
-                # If this is function, we get it's type hints.
+            elif inspect.isfunction(dep.dependency):
+                # If this is function or an instance of a class, we get it's type hints.
                 hints = get_type_hints(dep.dependency)
+            else:
+                hints = get_type_hints(
+                    dep.dependency.__call__,  # type: ignore # noqa: WPS609
+                )
 
             # Now we need to iterate over parameters, to
             # find all parameters, that have TaskiqDepends as it's
             # default vaule.
             for param_name, param in sign.parameters.items():
                 default_value = param.default
 
@@ -115,14 +119,15 @@
                 if FastapiDepends is not None and isinstance(  # noqa: WPS337
                     default_value,
                     FastapiDepends,
                 ):
                     default_value = Dependency(
                         dependency=default_value.dependency,
                         use_cache=default_value.use_cache,
+                        signature=param,
                     )
 
                 # We check, that default value is an instance of
                 # TaskiqDepends.
                 if not isinstance(default_value, Dependency):
                     continue
 
@@ -154,14 +159,15 @@
 
                 # Now we construct new TaskiqDepends instance
                 # with correct dependency function and cache.
                 dep_obj = Dependency(
                     dependency_func,
                     use_cache=default_value.use_cache,
                     kwargs=default_value.kwargs,
+                    signature=param,
                 )
                 # Also we set the parameter name,
                 # it will help us in future when
                 # we're going to resolve all dependencies.
                 dep_obj.param_name = param_name
 
                 # We append current dependency
```

### Comparing `taskiq_dependencies-1.1.2/PKG-INFO` & `taskiq_dependencies-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-dependencies
-Version: 1.1.2
+Version: 1.2.0
 Summary: FastAPI like dependency injection implementation
 Keywords: taskiq,dependencies,injection,async,DI
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -121,7 +121,35 @@
 with graph.sync_ctx({DefaultDep: DefaultDep()}) as ctx:
     print(ctx.resolve_kwargs())
 
 ```
 
 You can run this code. It will resolve dd dependency into a `DefaultDep` variable you provide.
 
+
+## Getting parameters information
+
+If you want to get the information about how this dependency was specified,
+you can use special class `ParamInfo` for that.
+
+```python
+from taskiq_dependencies import Depends, DependencyGraph, ParamInfo
+
+
+def dependency(info: ParamInfo = Depends()) -> str:
+    assert info.name == "dd"
+    return info.name
+
+def target_func(dd: str = Depends(dependency)):
+    print(dd)
+    return 1
+
+
+graph = DependencyGraph(target_func)
+
+with graph.sync_ctx() as ctx:
+    print(ctx.resolve_kwargs())
+
+```
+
+The ParamInfo has the information about name and parameters signature. It's useful if you want to create a dependency that changes based on parameter name, or signature.
+
```

