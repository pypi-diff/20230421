# Comparing `tmp/pyxxl-0.3.0a3.tar.gz` & `tmp/pyxxl-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxxl-0.3.0a3.tar", max compression
+gzip compressed data, was "pyxxl-0.3.1.tar", max compression
```

## Comparing `pyxxl-0.3.0a3.tar` & `pyxxl-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0    35149 2023-02-27 14:22:16.936166 pyxxl-0.3.0a3/LICENSE
--rw-r--r--   0        0        0     2701 2023-02-27 14:22:16.936166 pyxxl-0.3.0a3/README.md
--rw-r--r--   0        0        0     1960 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyproject.toml
--rw-r--r--   0        0        0      178 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/__init__.py
--rw-r--r--   0        0        0     1265 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/ctx.py
--rw-r--r--   0        0        0      259 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/enum.py
--rw-r--r--   0        0        0      981 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/error.py
--rw-r--r--   0        0        0    10272 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/executor.py
--rw-r--r--   0        0        0       82 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/logger/__init__.py
--rw-r--r--   0        0        0     1420 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/logger/common.py
--rw-r--r--   0        0        0     4043 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/logger/disk.py
--rw-r--r--   0        0        0     4215 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/logger/redis.py
--rw-r--r--   0        0        0     4612 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/main.py
--rw-r--r--   0        0        0      764 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/schema.py
--rw-r--r--   0        0        0     3649 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/server.py
--rw-r--r--   0        0        0     3945 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/setting.py
--rw-r--r--   0        0        0        0 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/tests/api/__init__.py
--rw-r--r--   0        0        0     2932 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/tests/api/test_server.py
--rw-r--r--   0        0        0     2131 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/tests/conftest.py
--rw-r--r--   0        0        0     1640 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/tests/test_client.py
--rw-r--r--   0        0        0      889 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/tests/test_context.py
--rw-r--r--   0        0        0     6368 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/tests/test_executor.py
--rw-r--r--   0        0        0     1646 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/tests/test_handler.py
--rw-r--r--   0        0        0     3697 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/tests/test_logger.py
--rw-r--r--   0        0        0      835 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/tests/test_register.py
--rw-r--r--   0        0        0     1616 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/tests/test_setting.py
--rw-r--r--   0        0        0      129 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/tests/test_utils.py
--rw-r--r--   0        0        0      872 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/tests/utils.py
--rw-r--r--   0        0        0      395 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/types.py
--rw-r--r--   0        0        0     1770 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/utils.py
--rw-r--r--   0        0        0     3920 2023-02-27 14:22:16.940166 pyxxl-0.3.0a3/pyxxl/xxl_client.py
--rw-r--r--   0        0        0     3688 1970-01-01 00:00:00.000000 pyxxl-0.3.0a3/setup.py
--rw-r--r--   0        0        0     3740 1970-01-01 00:00:00.000000 pyxxl-0.3.0a3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-21 09:30:19.865097 pyxxl-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3989 2023-04-21 09:30:19.865097 pyxxl-0.3.1/README.md
+-rw-r--r--   0        0        0     2083 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      178 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/__init__.py
+-rw-r--r--   0        0        0     1041 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/ctx.py
+-rw-r--r--   0        0        0      259 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/enum.py
+-rw-r--r--   0        0        0      981 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/error.py
+-rw-r--r--   0        0        0    12215 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/executor.py
+-rw-r--r--   0        0        0       82 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/logger/__init__.py
+-rw-r--r--   0        0        0     1420 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/logger/common.py
+-rw-r--r--   0        0        0     5026 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/logger/disk.py
+-rw-r--r--   0        0        0     4248 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/logger/redis.py
+-rw-r--r--   0        0        0     5064 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/main.py
+-rw-r--r--   0        0        0     2526 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/prometheus.py
+-rw-r--r--   0        0        0      764 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/schema.py
+-rw-r--r--   0        0        0     3835 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/server.py
+-rw-r--r--   0        0        0     4758 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/setting.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/tests/api/__init__.py
+-rw-r--r--   0        0        0      669 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/tests/api/test_metrics.py
+-rw-r--r--   0        0        0     2774 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/tests/api/test_server.py
+-rw-r--r--   0        0        0     2190 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/tests/conftest.py
+-rw-r--r--   0        0        0     1640 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_client.py
+-rw-r--r--   0        0        0      889 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_context.py
+-rw-r--r--   0        0        0     6572 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_executor.py
+-rw-r--r--   0        0        0     1391 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_handler.py
+-rw-r--r--   0        0        0     3697 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_logger.py
+-rw-r--r--   0        0        0      835 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_register.py
+-rw-r--r--   0        0        0     1804 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_setting.py
+-rw-r--r--   0        0        0      129 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_utils.py
+-rw-r--r--   0        0        0      872 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/utils.py
+-rw-r--r--   0        0        0      395 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/types.py
+-rw-r--r--   0        0        0     2016 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/utils.py
+-rw-r--r--   0        0        0     3923 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/xxl_client.py
+-rw-r--r--   0        0        0     5072 1970-01-01 00:00:00.000000 pyxxl-0.3.1/PKG-INFO
```

### Comparing `pyxxl-0.3.0a3/LICENSE` & `pyxxl-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.0a3/pyproject.toml` & `pyxxl-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,100 @@
 [tool.poetry]
-name = "pyxxl"
-version = "0.3.0a3"
-readme = "README.md"
-license = "GPL-3.0-only"
-description = "A Python executor for XXL-jobs"
 authors = ["fcfangcc <swjfc22@live.com>"]
-repository = "https://github.com/fcfangcc/pyxxl"
-keywords = ["XXL"]
 classifiers = [
-    "Topic :: Software Development :: Libraries :: Python Modules"
+  "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-
+description = "A Python executor for XXL-jobs"
+keywords = ["XXL"]
+license = "GPL-3.0-only"
+name = "pyxxl"
+readme = "README.md"
+repository = "https://github.com/fcfangcc/pyxxl"
+version = "0.3.1"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-aiohttp = "^3.8.1"
 aiofiles = "^22.1.0"
-redis = { version = "^4.4.0", optional = true }
-python-dotenv = { version = "*", optional = true }
+aiohttp = "^3.8.1"
+prometheus-client = {version = "*", optional = true}
+python = "^3.9"
+python-dotenv = {version = "*", optional = true}
+redis = {version = "^4.4.0", optional = true}
 
 [tool.poetry.extras]
-redis = ["redis"]
+all = ["redis", "python-dotenv", "prometheus-client"]
 dotenv = ["python-dotenv"]
-all = ["redis", "python-dotenv"]
+metrics = ["prometheus-client"]
+redis = ["redis"]
 
 [tool.poetry.group.doc.dependencies]
+mdx-include = "^1.4.2"
 mkdocs = "^1.4.2"
-mkdocstrings = { version = "^0.20.0", extras = ["python"] }
 mkdocs-material = "^9.0.9"
-mdx-include = "^1.4.2"
+mkdocstrings = {version = "^0.20.0", extras = ["python"]}
 
 [tool.poetry.group.dev.dependencies]
-pytest = "7.1.2"
-pytest-asyncio = "0.18.3"
-pre-commit = "2.19.0"
+black = "23.1.0"
 mypy = "0.942"
+pre-commit = "2.19.0"
+pytest = "7.1.2"
 pytest-aiohttp = "1.0.4"
+pytest-asyncio = "0.18.3"
 pytest-cov = "3.0.0"
 ruff = "^0.0.249"
-black = "23.1.0"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0"]
 
 # if your need
 # https://python-poetry.org/docs/repositories/#install-dependencies-from-a-private-repository
 [[tool.poetry.source]]
 name = "aliyun"
-url = "https://mirrors.aliyun.com/pypi/simple/"
 secondary = true
+url = "https://mirrors.aliyun.com/pypi/simple/"
 
 [tool.mypy]
-files = "pyxxl"
-ignore_missing_imports = true
 disallow_untyped_defs = true
 exclude = [
-    '^pyxxl/tests/test_.*\.py$',
-    '^pyxxl/tests/api/test_.*\.py$',
+  '^pyxxl/tests/test_.*\.py$',
+  '^pyxxl/tests/api/test_.*\.py$',
 ]
-
+files = "pyxxl"
+ignore_missing_imports = true
 
 [tool.coverage.run]
 concurrency = ["thread"]
 
 [tool.coverage.report]
 exclude_lines = [
-    "pragma: no cover",
-    "if __name__ == .__main__.",
-    "raise NotImplementedError",
-    "\\.\\.\\.",
-    "if TYPE_CHECKING",
+  "pragma: no cover",
+  "if __name__ == .__main__.",
+  "raise NotImplementedError",
+  "\\.\\.\\.",
+  "if TYPE_CHECKING",
 ]
 
 [tool.black]
 line-length = 119
-target-version = ['py38']
+target-version = ['py39']
 
 [tool.ruff]
+exclude = [
+  "__init__.py",
+]
 line-length = 119
 select = [
-    "E",
-    "W",
-    "F",
-    "I",
-    "C",
-    "B",
-    "PGH"
-]
-exclude = [
-    "__init__.py"
+  "E",
+  "W",
+  "F",
+  "I",
+  "C",
+  "B",
+  "PGH",
 ]
 
 ignore = [
-    "C408",  # Unnecessary `dict` call (rewrite as a literal)
+  "C408", # Unnecessary `dict` call (rewrite as a literal)
 ]
+
+[tool.pytest.ini_options]
+addopts = "--asyncio-mode auto"
```

### Comparing `pyxxl-0.3.0a3/pyxxl/ctx.py` & `pyxxl-0.3.1/pyxxl/ctx.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 import logging
 import threading
 from contextvars import ContextVar
 from typing import Any, Optional
 
 from pyxxl.schema import RunData
 
-_global_vars: ContextVar[dict] = ContextVar("pyxxl_vars", default={})
-
 
 class GlobalVars:
-    @staticmethod
-    def _set_var(name: str, obj: Any) -> None:
-        _global_vars.get()[name] = obj
-
-    @staticmethod
-    def _get_var(name: str) -> Any:
-        return _global_vars.get()[name]
-
-    @staticmethod
-    def try_get(name: str) -> Optional[Any]:
-        return _global_vars.get().get(name)
-
-    @staticmethod
-    def set_xxl_run_data(data: RunData) -> None:
-        GlobalVars._set_var("xxl_kwargs", data)
+    _DATA: ContextVar = ContextVar("_DATA")
+    _LOGGER: ContextVar = ContextVar("_LOGGER")
+    _EVENT: ContextVar = ContextVar("_EVENT")
+
+    @classmethod
+    def set_xxl_run_data(cls, data: RunData) -> None:
+        cls._DATA.set(data)
+
+    @classmethod
+    def try_get_data(cls) -> Optional[Any]:
+        return cls._DATA.get(None)
 
     @property
     def xxl_run_data(self) -> RunData:
-        return self._get_var("xxl_kwargs")
+        return self._DATA.get()
 
-    @staticmethod
-    def set_task_logger(logger: logging.Logger) -> None:
-        GlobalVars._set_var("task_logger", logger)
+    @classmethod
+    def set_task_logger(cls, logger: logging.Logger) -> None:
+        cls._LOGGER.set(logger)
 
     @property
     def logger(self) -> logging.Logger:  # pragma: no cover
-        return self._get_var("task_logger")
+        return self._LOGGER.get()
 
-    @staticmethod
-    def set_cancel_event(event: threading.Event) -> None:
-        GlobalVars._set_var("cancel_event", event)
+    @classmethod
+    def set_cancel_event(cls, event: threading.Event) -> None:
+        cls._EVENT.set(event)
 
     @property
     def cancel_event(self) -> threading.Event:  # pragma: no cover
-        return self._get_var("cancel_event")
+        return self._EVENT.get()
 
 
 g = GlobalVars()
```

### Comparing `pyxxl-0.3.0a3/pyxxl/error.py` & `pyxxl-0.3.1/pyxxl/error.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.0a3/pyxxl/executor.py` & `pyxxl-0.3.1/pyxxl/executor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,77 @@
+from __future__ import annotations
+
 import asyncio
 import logging
 import threading
 import time
 import warnings
 from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, Dict, List, MutableSet, Optional
 
 from pyxxl import error
 from pyxxl.ctx import g
 from pyxxl.enum import executorBlockStrategy
 from pyxxl.logger import DiskLog, LogBase
 from pyxxl.schema import RunData
 from pyxxl.setting import ExecutorConfig
 from pyxxl.types import DecoratedCallable
 from pyxxl.xxl_client import XXL
 
 logger = logging.getLogger(__name__)
+# https://docs.python.org/3.10/library/asyncio-task.html#asyncio.create_task
+_BACKGROUND_TASKS: MutableSet[asyncio.Task] = set()
+
+
+def spawn_task(task: asyncio.Task) -> None:
+    _BACKGROUND_TASKS.add(task)
+    task.add_done_callback(_BACKGROUND_TASKS.discard)
 
 
 @dataclass
 class HandlerInfo:
     handler: Callable
+    is_async: bool = False
 
     def __str__(self) -> str:
         return "<HandlerInfo {}>".format(self.handler.__name__)
 
-    @property
-    def is_async(self) -> bool:
-        return asyncio.iscoroutinefunction(self.handler)
+    def __post_init__(self) -> None:
+        self.is_async = asyncio.iscoroutinefunction(self.handler)
 
-    async def start_async(self, timeout: int) -> Any:
-        assert self.is_async
-        return await asyncio.wait_for(self.handler(), timeout=timeout)
-
-    async def start_sync(self, loop: asyncio.AbstractEventLoop, pool: ThreadPoolExecutor, timeout: int) -> Any:
-        assert not self.is_async
+    async def start(self, timeout: int) -> Any:
+        if self.is_async:
+            return await asyncio.wait_for(self.handler(), timeout=timeout)
+        # https://stackoverflow.com/questions/71416383/python-asyncio-cancelling-a-to-thread-task-wont-stop-the-thread
+        # 由于线程无法直接取消，这里发送一个event，供开发者自己接收信号来判断是否需要取消
         event = threading.Event()
         g.set_cancel_event(event)
         try:
-            return await asyncio.wait_for(loop.run_in_executor(pool, self.handler), timeout=timeout)
+            return await asyncio.wait_for(asyncio.to_thread(self.handler), timeout=timeout)
         except (asyncio.exceptions.TimeoutError, asyncio.CancelledError) as e:
             event.set()
             logger.debug("Get error for sync task {}".format(self))
             raise e
 
 
+class XXLTask:
+    def __init__(self, task: asyncio.Task, data: RunData):
+        self.task = task
+        self.data = data
+
+    def __str__(self) -> str:
+        return "<XXLTask task={} data={}>".format(self.task, self.data)
+
+    @property
+    def cancel(self) -> Any:
+        return self.task.cancel
+
+
 class JobHandler:
     def __init__(self) -> None:
         self._handlers: Dict[str, HandlerInfo] = {}
 
     def register(
         self, *args: Any, name: Optional[str] = None, replace: bool = False
     ) -> Callable[[DecoratedCallable], DecoratedCallable]:
@@ -89,14 +110,16 @@
         self,
         xxl_client: XXL,
         config: ExecutorConfig,
         *,
         handler: Optional[JobHandler] = None,
         loop: Optional[asyncio.AbstractEventLoop] = None,
         logger_factory: Optional[LogBase] = None,
+        successed_callback: Optional[Callable] = None,
+        failed_callback: Optional[Callable] = None,
     ) -> None:
         """执行器，真正的调度任务和策略都在这里
 
         Args:
             xxl_client (XXL): xxl客户端
             config (ExecutorConfig): 配置参数
             handler (Optional[JobHandler], optional): Defaults to None.
@@ -104,141 +127,165 @@
         """
 
         self.xxl_client = xxl_client
         self.config = config
 
         self.handler: JobHandler = handler or JobHandler()
         self.loop = loop or asyncio.get_event_loop()
-        self.tasks: Dict[int, asyncio.Task] = {}
-        self.queue: Dict[int, List[RunData]] = defaultdict(list)
+        self.tasks: Dict[int, XXLTask] = {}
+        self.queue: Dict[int, asyncio.Queue[RunData]] = defaultdict(
+            lambda: asyncio.Queue(maxsize=self.config.task_queue_length)
+        )
         self.lock = asyncio.Lock()
         self.thread_pool = ThreadPoolExecutor(
             max_workers=self.config.max_workers,
             thread_name_prefix="pyxxl_pool",
         )
         self.logger_factory = logger_factory or DiskLog(self.config.log_local_dir)
+        self.successed_callback = successed_callback or (lambda: 1)
+        self.failed_callback = failed_callback or (lambda x: 1)
+        self.loop.set_default_executor(self.thread_pool)
 
-    async def shutdown(self) -> None:
-        for _, task in self.tasks.items():
-            task.cancel()
-
-    async def run_job(self, run_data: RunData) -> None:
-        handler_obj = self.handler.get(run_data.executorHandler)
+    async def run_job(self, data: RunData) -> str:
+        handler_obj = self.handler.get(data.executorHandler)
         if not handler_obj:
-            logger.warning("handler %s not found." % run_data.executorHandler)
-            raise error.JobNotFoundError("handler %s not found." % run_data.executorHandler)
+            logger.warning("handler %s not found." % data.executorHandler)
+            raise error.JobNotFoundError("handler %s not found." % data.executorHandler)
 
         # 一个执行器同时只能执行一个jobId相同的任务
         async with self.lock:
-            current_task = self.tasks.get(run_data.jobId)
-            if current_task:
-                # 不用的阻塞策略
-                # pylint: disable=no-else-raise
-                if run_data.executorBlockStrategy == executorBlockStrategy.DISCARD_LATER.value:
-                    raise error.JobDuplicateError(
-                        "The same job [%s] is already executing and this has been discarded." % run_data.jobId
+            current_task = self.tasks.get(data.jobId)
+            if not current_task and self.get_queue(data.jobId).empty():
+                self.tasks[data.jobId] = XXLTask(self.loop.create_task(self._run(data)), data)
+                return "Running"
+
+            logger.warning("jobId {} is running. current_task={}".format(data.jobId, current_task))
+            # pylint: disable=no-else-raise
+            if data.executorBlockStrategy == executorBlockStrategy.DISCARD_LATER.value:
+                raise error.JobDuplicateError(
+                    "The same job [%s] is already executing and this has been discarded." % data
+                )
+            elif data.executorBlockStrategy == executorBlockStrategy.COVER_EARLY.value:
+                msg = "Job {} BlockStrategy is COVER_EARLY, logId {} replaced.".format(data.jobId, data.logId)
+                logger.warning(msg)
+                spawn_task(self.loop.create_task(self.cancel_job(data.jobId, include_queue=False)))
+                await self.get_queue(data.jobId).put(data)
+                return msg
+            elif data.executorBlockStrategy == executorBlockStrategy.SERIAL_EXECUTION.value:
+                queue = self.get_queue(data.jobId)
+                if queue.full():
+                    msg = "Job {job_id} is  SERIAL, queue length more than {maxsize}." "Job {job}  discard!".format(
+                        job_id=data.jobId, job=data, maxsize=queue.maxsize
                     )
-                elif run_data.executorBlockStrategy == executorBlockStrategy.COVER_EARLY.value:
-                    logger.warning("job %s is  COVER_EARLY, logId %s replaced." % (run_data.jobId, run_data.logId))
-                    await self._cancel(run_data.jobId)
-                elif run_data.executorBlockStrategy == executorBlockStrategy.SERIAL_EXECUTION.value:
-                    if len(self.queue[run_data.jobId]) >= self.config.task_queue_length:
-                        msg = (
-                            "job {job_id} is  SERIAL, queue length more than {max_length}."
-                            "logId {log_id}  discard!".format(
-                                job_id=run_data.jobId,
-                                log_id=run_data.logId,
-                                max_length=self.config.task_queue_length,
-                            )
-                        )
-                        logger.error(msg)
-                        raise error.JobDuplicateError(msg)
-                    else:
-                        queue = self.queue[run_data.jobId]
-                        logger.info(
-                            "job {job_id} is in queen, logId {log_id} ranked {ranked}th [max={max_length}]...".format(
-                                job_id=run_data.jobId,
-                                log_id=run_data.logId,
-                                ranked=len(queue) + 1,
-                                max_length=self.config.task_queue_length,
-                            )
-                        )
-                        queue.append(run_data)
-                        return
+                    logger.error(msg)
+                    raise error.JobDuplicateError(msg)
                 else:
-                    raise error.JobParamsError(
-                        "unknown executorBlockStrategy [%s]." % run_data.executorBlockStrategy,
-                        executorBlockStrategy=run_data.executorBlockStrategy,
+                    msg = "job {job_id} is in queen, logId {log_id} ranked {ranked}th [max={maxsize}]...".format(
+                        job_id=data.jobId, log_id=data.logId, ranked=queue.qsize() + 1, maxsize=queue.maxsize
                     )
+                    logger.info(msg)
+                    await queue.put(data)
+                    return msg
+            else:
+                raise error.JobParamsError(
+                    "unknown executorBlockStrategy [%s]." % data.executorBlockStrategy,
+                    executorBlockStrategy=data.executorBlockStrategy,
+                )
 
-            start_time = int(time.time() * 1000)
-            task = self.loop.create_task(self._run(handler_obj, start_time, run_data))
-            self.tasks[run_data.jobId] = task
+    async def cancel_job(self, job_id: int, include_queue: bool = True) -> None:
+        logger.warning("start kill job: job_id={}".format(job_id))
+        await asyncio.sleep(0.01)  # sleep for pytest
 
-    async def cancel_job(self, job_id: int) -> None:
         async with self.lock:
-            logger.warning("start kill job: job_id={}".format(job_id))
-            await self._cancel(job_id)
+            if include_queue:
+                queue = self.get_queue(job_id)
+                while not queue.empty():
+                    data = queue.get_nowait()
+                    logger.warning("Discard jobId {} from queue,data: {}".format(job_id, data))
+
+            task = self.tasks.get(job_id, None)
+            if task:
+                # https://docs.python.org/3/library/asyncio-task.html#asyncio.Task.cancel
+                task.cancel()
+                try:
+                    await task.task
+                except asyncio.CancelledError:
+                    logger.warning("Job %s cancelled." % job_id)
 
     async def is_running(self, job_id: int) -> bool:
         return job_id in self.tasks
 
-    async def _run(self, handler: HandlerInfo, start_time: int, data: RunData) -> None:
+    async def _run(self, data: RunData) -> None:
+        handler = self.handler.get(data.executorHandler)
+        assert handler
         g.set_xxl_run_data(data)
         g.set_task_logger(self.logger_factory.get_logger(data.logId))
+        start_time = int(time.time() * 1000)
         try:
             g.logger.info("Start job jobId=%s logId=%s [%s]" % (data.jobId, data.logId, data))
             timeout = data.executorTimeout or self.config.task_timeout
-            if handler.is_async:
-                result = await handler.start_async(timeout)
-            else:
-                result = await handler.start_sync(self.loop, self.thread_pool, timeout)
+            result = await handler.start(timeout)
             g.logger.info("Job finished jobId=%s logId=%s" % (data.jobId, data.logId))
             await self.xxl_client.callback(data.logId, start_time, code=200, msg=result)
+            self.successed_callback()
         except asyncio.CancelledError as e:
-            g.logger.warning(e, exc_info=True)
+            g.logger.info(e, exc_info=True)
             await self.xxl_client.callback(data.logId, start_time, code=500, msg="CancelledError")
+            self.failed_callback("cancelled")
         except asyncio.exceptions.TimeoutError as e:
             # 同步任务run_in_executor超时会抛出TimeoutError异常
-            # 但是注意线程里面的任务仍然在允许，可能会占满所有的线程池
-            # todo: 杀死线程
+            # !!! 但是注意线程里面的任务仍然在运行，可能会占满所有的线程池
             g.logger.warning(e, exc_info=True)
             await self.xxl_client.callback(data.logId, start_time, code=500, msg="TimeoutError")
+            self.failed_callback("timeout")
         except Exception as err:  # pylint: disable=broad-except
-            g.logger.exception(err)
+            g.logger.exception(err, exc_info=True)
             await self.xxl_client.callback(data.logId, start_time, code=500, msg=str(err))
+            self.failed_callback("exception")
         finally:
-            await self._finish(data.jobId)
+            if self.lock.locked():
+                await self._finish(data.jobId)
+            else:
+                async with self.lock:
+                    await self._finish(data.jobId)
 
     async def _finish(self, job_id: int) -> None:
-        self.tasks.pop(job_id, None)
-        # 如果有队列中的任务，开始执行队列中的任务
-        queue = self.queue[job_id]
-        if queue:
-            kwargs: RunData = queue.pop(0)
-            logger.info("JobId %s in queue[%s], start job with logId %s" % (kwargs.jobId, len(queue), kwargs.logId))
-            await self.run_job(kwargs)
-
-    async def _cancel(self, job_id: int) -> None:
-        task = self.tasks.pop(job_id, None)
-        if task:
-            task.cancel()
-            try:
-                await task
-            except asyncio.CancelledError:
-                logger.warning("Job %s cancelled." % job_id)
+        # 所有移除tasks的操作全部在这里执行
+        finish_task = self.tasks.pop(job_id, None)
+        logger.info("Finish task {}".format(finish_task))
+        queue = self.get_queue(job_id)
+        if not queue.empty():
+            data = queue.get_nowait()
+            logger.info(
+                "Get data from queue jobId={}, after queueSize={}, data={}".format(job_id, queue.qsize(), data)
+            )
+            self.tasks[job_id] = XXLTask(self.loop.create_task(self._run(data)), data)
+            queue.task_done()
+
+    async def shutdown(self) -> None:
+        await asyncio.sleep(0.01)  # sleep for pytest
+
+        async with self.lock:
+            self.queue.clear()
+            for _, task in self.tasks.items():
+                task.task.cancel()
 
     async def graceful_close(self, timeout: int = 60) -> None:
         """优雅关闭"""
+        await asyncio.sleep(0.01)  # sleep for pytest
 
         async def _graceful_close() -> None:
-            while len(self.tasks) > 0:
-                await asyncio.wait(self.tasks.values())
+            while len(self.tasks) > 0 or any(i.qsize() > 0 for i in self.queue.values()):
+                await asyncio.wait([i.task for i in self.tasks.values()])
+                await asyncio.sleep(0.05)
 
         await asyncio.wait_for(_graceful_close(), timeout=timeout)
 
     def reset_handler(self, handler: Optional[JobHandler] = None) -> None:
         self.handler = handler or JobHandler()
 
     @property
     def register(self) -> Any:
         return self.handler.register
+
+    def get_queue(self, job_id: int) -> asyncio.Queue[RunData]:
+        return self.queue[job_id]
```

### Comparing `pyxxl-0.3.0a3/pyxxl/logger/common.py` & `pyxxl-0.3.1/pyxxl/logger/common.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.0a3/pyxxl/logger/disk.py` & `pyxxl-0.3.1/pyxxl/logger/disk.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
 import time
+import weakref
 from contextlib import asynccontextmanager
 from logging import FileHandler
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, AsyncGenerator, List
 
 import aiofiles
 
@@ -19,36 +20,68 @@
 
 LOG_NAME_PREFIX = "pyxxl-{log_id}.log"
 LOG_NAME_REGEX = "pyxxl-*.log"
 MAX_LOG_TAIL_LINES = 1000
 logger = logging.getLogger(__name__)
 
 
+def _close_file_stream(_logger: logging.Logger) -> None:
+    # !!! StreamHandler remove会有问题，需要判断是否是FileHandler
+    for h in _logger.handlers:
+        if isinstance(h, logging.FileHandler):
+            logger.debug("close file log object: {}.".format(h))
+            h.close()
+            _logger.removeHandler(h)
+
+
+class XXLogger:
+    """为了可以关闭文件写入流"""
+
+    def __init__(self, logger: logging.Logger) -> None:
+        self._logger = logger
+
+        self._finalizer = weakref.finalize(self, _close_file_stream, self._logger)
+
+    def remove(self) -> None:
+        self._finalizer()
+
+    @property
+    def removed(self) -> bool:
+        return not self._finalizer.alive
+
+    def __getattr__(self, name: str) -> Any:
+        if name in ["info", "error", "warning", "debug", "exception", "handlers"]:
+            return getattr(self._logger, name)
+
+
 class DiskLog(LogBase):
     def __init__(self, log_path: str, log_tail_lines: int = 0, expired_days: int = 14) -> None:
         self.log_path = Path(log_path)
         if not self.log_path.exists():
             self.log_path.mkdir()  # pragma: no cover
             logger.info("create logdir %s" % self.log_path)  # pragma: no cover
         self.log_tail_lines = log_tail_lines or MAX_LOG_TAIL_LINES
         self.expired_days = expired_days
 
     def key(self, log_id: int) -> str:
         return self.log_path.joinpath(LOG_NAME_PREFIX.format(log_id=log_id)).absolute().as_posix()
 
-    def get_logger(self, log_id: int, *, stdout: bool = True, level: int = logging.INFO) -> logging.Logger:
+    def get_logger(  # type:ignore[override]
+        self, log_id: int, *, stdout: bool = True, level: int = logging.INFO
+    ) -> XXLogger:
         logger = logging.getLogger("pyxxl-task-{%s}" % log_id)
+        logger.propagate = False
         logger.setLevel(level)
         handlers: list[Handler] = [logging.StreamHandler()] if stdout else []
         handlers.append(FileHandler(self.key(log_id), delay=True))
         for h in handlers:
             h.setFormatter(STD_FORMATTER)
             h.setLevel(level)
             logger.addHandler(h)
-        return logger
+        return XXLogger(logger)
 
     async def get_logs(self, request: LogRequest, *, key: str = None) -> LogResponse:
         # todo: 优化获取中间行的逻辑，缓存之前每行日志的大小然后直接seek
         logs = ""
         to_line_num = request["fromLineNum"]  # start with 1
         is_end = False
         key = key or self.key(request["logId"])
```

### Comparing `pyxxl-0.3.0a3/pyxxl/logger/redis.py` & `pyxxl-0.3.1/pyxxl/logger/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
             raise TypeError(
                 "pool expect Union[str, redis.ConnectionPool], got %s." % type(redis_client)
             )  # pragma: no cover
         self.rclient = rclient
 
     def get_logger(self, log_id: int, *, stdout: bool = True, level: int = logging.INFO) -> logging.Logger:
         logger = logging.getLogger("pyxxl-task-{%s}" % log_id)
+        logger.propagate = False
         logger.setLevel(level)
         handlers: list[Handler] = [logging.StreamHandler()] if stdout else []
         handlers.append(RedisHandler(self.key(log_id), self.expired_days * 3600 * 24, self.rclient))
         for h in handlers:
             h.setFormatter(STD_FORMATTER)
             h.setLevel(level)
             logger.addHandler(h)
```

### Comparing `pyxxl-0.3.0a3/pyxxl/main.py` & `pyxxl-0.3.1/pyxxl/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 import asyncio
+import functools
 import logging
 from multiprocessing import Process
 from typing import AsyncGenerator, Optional
 
 from aiohttp import web
 
 from pyxxl.executor import Executor, JobHandler
 from pyxxl.logger import DiskLog, LogBase, RedisLog
 from pyxxl.server import create_app
 from pyxxl.setting import ExecutorConfig
-from pyxxl.utils import setup_logging
+from pyxxl.utils import setup_logging, try_import
 from pyxxl.xxl_client import XXL
 
 logger = logging.getLogger(__name__)
 
+if try_import("prometheus_client"):
+    from pyxxl import prometheus
+
+    Executor: Executor = functools.partial(  # type: ignore[no-redef]
+        Executor,
+        successed_callback=prometheus.success,
+        failed_callback=prometheus.failed,
+    )
+
 
 class PyxxlRunner:
     daemon: Optional[Process] = None
 
     def __init__(
         self,
         config: ExecutorConfig,
@@ -40,23 +50,26 @@
         Args:
             config (ExecutorConfig): 配置参数 [ExecutorConfig](/apis/config)
             handler (JobHandler, optional): 执行器支持的job,没有预先定义的job名称也会执行失败
         """
 
         self.handler = handler or JobHandler()
         self.config = config
-        if self.config.debug:
-            setup_logging(level=logging.DEBUG)
+        log_level = logging.DEBUG if self.config.debug else logging.INFO
+        setup_logging(self.config.executor_log_path, level=log_level)
 
     async def _register_task(self, xxl_client: XXL) -> None:
         # todo: 这是个调度器的bug，必须循环去注册，不然会显示为离线
         # https://github.com/xuxueli/xxl-job/issues/2090
-        while True:
-            await xxl_client.registry(self.config.executor_app_name, self.config.executor_baseurl)
-            await asyncio.sleep(10)
+        try:
+            while True:
+                await xxl_client.registry(self.config.executor_app_name, self.config.executor_baseurl)
+                await asyncio.sleep(10)
+        finally:
+            logger.warning("Register task is exit.")
 
     def _get_xxl_clint(self) -> XXL:
         """for moke"""
         return XXL(self.config.xxl_admin_baseurl, token=self.config.access_token)
 
     def _get_log(self) -> LogBase:
         if self.config.log_target == "disk":
@@ -106,15 +119,15 @@
         return app
 
     def run_executor(self, handle_signals: bool = True) -> None:
         """用aiohttp的web服务器启动执行器"""
         web.run_app(
             self.create_server_app(),
             port=self.config.executor_port,
-            host=self.config.executor_host,
+            host=self.config.executor_server_host,
             handle_signals=handle_signals,
         )
 
     def _runner(self) -> None:
         self.run_executor(handle_signals=True)
 
     def run_with_daemon(self) -> None:
```

### Comparing `pyxxl-0.3.0a3/pyxxl/schema.py` & `pyxxl-0.3.1/pyxxl/schema.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.0a3/pyxxl/server.py` & `pyxxl-0.3.1/pyxxl/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import TYPE_CHECKING
 
 from aiohttp import web
 
 from pyxxl import error
 from pyxxl.schema import RunData
+from pyxxl.utils import try_import
 
 if TYPE_CHECKING:
     from pyxxl.logger import LogBase
 
 logger = logging.getLogger(__name__)
 
 routes = web.RouteTableDef()
@@ -46,29 +47,30 @@
         "glueUpdatetime":1586629003727,             // GLUE脚本更新时间，用于判定脚本是否变更以及是否需要刷新
         "broadcastIndex":0,                         // 分片参数：当前分片
         "broadcastTotal":0                          // 分片参数：总分片
     }
     """
     data = await request.json()
     run_data = RunData(**data)
-    logger.debug("Get task request. jobId=%s logId=%s [%s]" % (run_data.jobId, run_data.logId, run_data))
+    logger.info("Get task request. jobId=%s logId=%s [%s]" % (run_data.jobId, run_data.logId, run_data))
+    msg = None
     try:
-        await request.app["executor"].run_job(run_data)
+        msg = await request.app["executor"].run_job(run_data)
     except error.JobDuplicateError as e:
         return web.json_response(dict(code=500, msg=e.message))
     except error.JobNotFoundError as e:
         return web.json_response(dict(code=500, msg=e.message))
 
-    return web.json_response(dict(code=200, msg=None))
+    return web.json_response(dict(code=200, msg=msg))
 
 
 @routes.post("/kill")
 async def kill(request: web.Request) -> web.Response:
     data = await request.json()
-    await request.app["executor"].cancel_job(data["jobId"])
+    await request.app["executor"].cancel_job(data["jobId"], include_queue=True)
     return web.json_response(dict(code=200, msg=None))
 
 
 @routes.post("/log")
 async def log(request: web.Request) -> web.Response:
     """
         {
@@ -92,8 +94,13 @@
     """
     xxl_admin_baseurl xxl调度中心的接口地址，如http://localhost:8080/xxl-job-admin/api/
     executor_names 执行器名称列表
     executor_baseurl 执行器http接口的地址 如http://172.17.0.1:9999
     """
     app = web.Application()
     app.add_routes(routes)
+    if try_import("prometheus_client"):
+        from pyxxl.prometheus import mount_app
+
+        mount_app(app)
+
     return app
```

### Comparing `pyxxl-0.3.0a3/pyxxl/setting.py` & `pyxxl-0.3.1/pyxxl/setting.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,14 +31,24 @@
     access_token: Optional[str] = None
     """调度器的token. Default: None"""
 
     executor_host: str = field(default_factory=get_network_ip)
     """执行器绑定的host,xxl-admin通过这个host来回调pyxxl执行器,如果不填会默认取第一个网卡的地址. Default: 获取到第一个网卡的ip地址"""
     executor_port: int = 9999
     """执行器绑定的http服务的端口,作用同host. Default: 9999"""
+    executor_log_path: str = "pyxxl.log"
+    """执行器日志输出的路径(注意路径必须存在). Default: pyxxl.log"""
+    executor_server_host: str = ""
+    """
+    执行器HTTP服务绑定的HOST,大部分情况下不需要设置. Default: executor_host
+
+    当执行器通过了端口转发暴露给admin的时候,需要把executor_host填写为直连admin的地址.
+    然后executor_server_host需要配置为0.0.0.0或者转发设备能访问的地址,不然会出现服务启动失败的情况
+
+    """
 
     max_workers: int = 30
     """执行器线程池（执行同步任务时使用）. Default: 30"""
     task_timeout: int = 60 * 10
     """任务的默认超时时间,如果调度器传了以参数executorTimeout为准. Default: 60 * 10"""
     task_queue_length: int = 30
     """任务的队列长度.单机串行的队列长度,当阻塞的任务大于此值时会抛弃. Default: 30"""
@@ -68,19 +78,25 @@
         except ImportError:  # pragma: no cover
             pass
 
         for param in inspect.signature(ExecutorConfig).parameters.values():
             env_val = os.getenv(param.name) or os.getenv(param.name.upper())
             if env_val is not None:
                 logger.debug("Get [%s] config from env: [%s]" % (param.name, env_val))
-                setattr(self, param.name, env_val)
+                if param.annotation is bool:
+                    real_value = env_val in ["true", "True"]
+                else:
+                    real_value = param.annotation(env_val)
+                setattr(self, param.name, real_value)
 
         self._valid_xxl_admin_baseurl()
         self._valid_executor_app_name()
         self._valid_logger_target()
+        if not self.executor_server_host:
+            self.executor_server_host = self.executor_host
 
     def _valid_xxl_admin_baseurl(self) -> None:
         _admin_url: URL = URL(self.xxl_admin_baseurl)
         if not (_admin_url.scheme.startswith("http") and _admin_url.path.endswith("/")):
             raise ValueError("admin_url must like http://localhost:8080/xxl-job-admin/api/")
 
     def _valid_executor_app_name(self) -> None:
```

### Comparing `pyxxl-0.3.0a3/pyxxl/tests/api/test_server.py` & `pyxxl-0.3.1/pyxxl/tests/api/test_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 import time
 
 import pytest
 from aiohttp.test_utils import TestClient
 
-# import logging
 
-# logger = logging.getLogger("pyxxl")
-# handler = logging.StreamHandler()
-# logger.addHandler(handler)
-# logger.setLevel(logging.DEBUG)
-
-
-async def _send_demoJobHandler(cli: TestClient, **kwargs):
+async def send_demoJobHandler(cli: TestClient, **kwargs):
     job_data = {
         "jobId": int(time.time() * 1000),
         "executorHandler": "demoJobHandler",
         "executorParams": "demoJobHandler",
         "executorBlockStrategy": "COVER_EARLY",
         "executorTimeout": 0,
         "logId": int(time.time() * 1000),
@@ -29,28 +22,28 @@
     job_data.update(kwargs)
     resp = await cli.post("/run", json=job_data)
     return resp, job_data["jobId"]
 
 
 @pytest.mark.asyncio
 async def test_run(cli: TestClient):
-    resp, _ = await _send_demoJobHandler(cli, executorBlockStrategy="DISCARD_LATER", jobId=100)
+    resp, _ = await send_demoJobHandler(cli, executorBlockStrategy="DISCARD_LATER", jobId=100)
     assert resp.status == 200
-    assert await resp.json() == {"code": 200, "msg": None}
+    assert await resp.json() == {"code": 200, "msg": "Running"}
     # error
-    resp, _ = await _send_demoJobHandler(cli, executorBlockStrategy="DISCARD_LATER", jobId=100)
+    resp, _ = await send_demoJobHandler(cli, executorBlockStrategy="DISCARD_LATER", jobId=100)
     assert resp.status == 200
     response_dict = await resp.json()
     assert response_dict["code"] == 500
     assert "already executing" in response_dict["msg"]
 
 
 @pytest.mark.asyncio
 async def test_run_not_found(cli: TestClient):
-    resp, _ = await _send_demoJobHandler(cli, executorHandler="test_run_not_found")
+    resp, _ = await send_demoJobHandler(cli, executorHandler="test_run_not_found")
     assert resp.status == 200
     response_dict = await resp.json()
     assert response_dict["code"] == 500
     assert "not found" in response_dict["msg"]
 
 
 @pytest.mark.asyncio
@@ -62,32 +55,32 @@
 
 @pytest.mark.asyncio
 async def test_idle_beat(cli: TestClient):
     resp = await cli.post("/idleBeat", json={"jobId": 1})
     assert resp.status == 200
     assert await resp.json() == {"code": 200, "msg": None}
 
-    resp, jobId = await _send_demoJobHandler(cli, jobId=300)
-    resp, jobId = await _send_demoJobHandler(cli, jobId=300)
+    resp, jobId = await send_demoJobHandler(cli, jobId=300)
+    resp, jobId = await send_demoJobHandler(cli, jobId=300)
     resp = await cli.post("/idleBeat", json={"jobId": jobId})
     response_data = await resp.json()
     assert response_data["code"] == 500
     assert response_data["msg"] == "job %s is running." % jobId
 
 
 @pytest.mark.asyncio
 async def test_kill(cli: TestClient):
-    resp, jobId = await _send_demoJobHandler(cli)
+    resp, jobId = await send_demoJobHandler(cli)
     resp = await cli.post("/kill", json={"jobId": jobId})
     assert await resp.json() == {"code": 200, "msg": None}
 
 
 @pytest.mark.asyncio
 async def test_log(cli: TestClient):
-    resp, jobId = await _send_demoJobHandler(cli)
+    resp, jobId = await send_demoJobHandler(cli)
     resp = await cli.post(
         "/log",
         json={
             "logId": jobId,
             "fromLineNum": 1,
         },
     )
```

### Comparing `pyxxl-0.3.0a3/pyxxl/tests/conftest.py` & `pyxxl-0.3.1/pyxxl/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import asyncio
-import logging
+import time
 from typing import Any, Generator
 
 import pytest
 import pytest_asyncio
 from aiohttp.web import Application
 from pytest_aiohttp.plugin import AiohttpClient, TestClient
 
 from pyxxl import ExecutorConfig
 from pyxxl.executor import Executor
 from pyxxl.tests.utils import INSTALL_REDIS, REDIS_TEST_URI, MokePyxxlRunner, MokeXXL
 from pyxxl.utils import setup_logging
 
-setup_logging(logging.INFO, custom_handlers=[logging.FileHandler("./testlogs.log")])
+setup_logging("./logs/pytest.log")
 
 GLOBAL_JOB_ID = 1
 GLOBAL_CONFIG: Any = dict(
     xxl_admin_baseurl="http://localhost:8080/xxl-job-admin/api/",
     executor_app_name="xxl-job-executor-sample",
     executor_host="127.0.0.1",
     graceful_close=False,
+    task_queue_length=5,
 )
 
 xxl_admin_baseurl = "http://localhost:8080/xxl-job-admin/api/"
 
 
 def _create_job_id() -> int:
     global GLOBAL_JOB_ID
@@ -47,26 +48,28 @@
             ExecutorConfig(**GLOBAL_CONFIG, log_target="redis", log_redis_uri=REDIS_TEST_URI),
             marks=pytest.mark.skipif(not INSTALL_REDIS, reason="no redis package."),
         ),
     ],
     ids=["disk", "redis"],
 )
 def executor(request: Any) -> Executor:
-    print(type(request))
     return Executor(MokeXXL("http://localhost:8080/xxl-job-admin/api/"), request.param, handler=None)
 
 
 @pytest.fixture(scope="session")
 def web_app(executor: Executor) -> Application:
-
     runner = MokePyxxlRunner(executor.config)
 
     @runner.handler.register(name="demoJobHandler")
     async def test_task() -> None:
-        await asyncio.sleep(60)
+        await asyncio.sleep(10)
+
+    @runner.handler.register(name="demoJobHandlerSync")
+    def test_task_sync() -> None:
+        time.sleep(5)
 
     return runner.create_server_app()
 
 
 @pytest_asyncio.fixture
 async def cli(aiohttp_client: AiohttpClient, web_app: Application) -> TestClient:
     return await aiohttp_client(web_app)
```

### Comparing `pyxxl-0.3.0a3/pyxxl/tests/test_client.py` & `pyxxl-0.3.1/pyxxl/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.0a3/pyxxl/tests/test_context.py` & `pyxxl-0.3.1/pyxxl/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.0a3/pyxxl/tests/test_executor.py` & `pyxxl-0.3.1/pyxxl/tests/test_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 from pyxxl.schema import RunData
 
 job_handler = JobHandler()
 
 
 @job_handler.register
 async def pytest_executor_async():
-    await asyncio.sleep(3)
+    await asyncio.sleep(2)
     return "成功30"
 
 
 @job_handler.register
 def pytest_executor_sync():
-    time.sleep(3)
+    time.sleep(2)
     return "成功30"
 
 
 @job_handler.register
 async def pytest_executor_error():
     assert 1 == 2
 
@@ -78,41 +78,39 @@
     assert executor.xxl_client.callback_result.get(1) == 200
     assert executor.xxl_client.callback_result.get(2) == 500
     assert executor.xxl_client.callback_result.get(3) is None
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("handler_name", HANDLER_NAMES)
-async def test_runner_cancel(executor: Executor, handler_name: str):
+async def test_runner_cancel(executor: Executor, handler_name: str, job_id: int):
     executor.reset_handler(job_handler)
     cancel_job_id, ok_job_id = 1100, 1200
-    await executor.run_job(
-        RunData(
-            **dict(
-                logId=cancel_job_id,
-                jobId=cancel_job_id,
-                executorHandler=handler_name,
-                executorBlockStrategy=executorBlockStrategy.SERIAL_EXECUTION.value,
-            )
-        )
-    )
-    await executor.run_job(
-        RunData(
-            **dict(
-                logId=ok_job_id,
-                jobId=ok_job_id,
-                executorHandler=handler_name,
-                executorBlockStrategy=executorBlockStrategy.SERIAL_EXECUTION.value,
-            )
-        )
+    base_data = dict(
+        executorHandler=handler_name,
+        executorBlockStrategy=executorBlockStrategy.SERIAL_EXECUTION.value,
     )
-    await executor.cancel_job(cancel_job_id)
+    await executor.run_job(RunData(logId=cancel_job_id, jobId=cancel_job_id, **base_data))
+    await executor.run_job(RunData(logId=ok_job_id, jobId=ok_job_id, **base_data))
+
+    await executor.cancel_job(cancel_job_id, include_queue=False)
     await executor.graceful_close()
-    assert executor.xxl_client.callback_result.get(cancel_job_id) is None
+    assert executor.xxl_client.callback_result.get(cancel_job_id) == 500
     assert executor.xxl_client.callback_result.get(ok_job_id) == 200
+    # include_queue =True
+    base_data.update({"jobId": job_id})
+    executor.xxl_client.clear_result()
+    cancel_log_id = job_id
+    queue_log_id = job_id + 1
+    await executor.run_job(RunData(logId=cancel_log_id, **base_data))
+    await executor.run_job(RunData(logId=queue_log_id, **base_data))
+    await executor.cancel_job(job_id, include_queue=True)
+    await executor.graceful_close()
+    assert executor.xxl_client.callback_result.get(cancel_log_id) == 500
+    assert executor.xxl_client.callback_result.get(queue_log_id) is None
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("handler_name", HANDLER_NAMES)
 async def test_runner_SERIAL_EXECUTION(executor: Executor, job_id: int, handler_name: str):
     executor.xxl_client.clear_result()
     executor.reset_handler(job_handler)
@@ -120,28 +118,27 @@
         jobId=job_id,
         executorHandler=handler_name,
         executorBlockStrategy=executorBlockStrategy.SERIAL_EXECUTION.value,
     )
     await executor.run_job(RunData(logId=11, **run_data))
     await executor.run_job(RunData(logId=12, **run_data))
     await executor.run_job(RunData(logId=13, **run_data))
-    assert len(executor.queue.get(job_id)) == 2
+    assert executor.queue.get(job_id).qsize() == 2
     await executor.graceful_close()
-    assert len(executor.queue.get(job_id)) == 0
+    assert executor.queue.get(job_id).qsize() == 0
     assert executor.xxl_client.callback_result.get(13) == 200
 
     # max_queue_length
-    executor.config.task_queue_length = 2
-    await executor.run_job(RunData(logId=11, **run_data))
-    await executor.run_job(RunData(logId=12, **run_data))
-    await executor.run_job(RunData(logId=13, **run_data))
+    for i in range(executor.config.task_queue_length + 1):
+        await executor.run_job(RunData(logId=100 + i, **run_data))
+
     with pytest.raises(JobDuplicateError, match="discard"):
-        await executor.run_job(RunData(logId=14, **run_data))
-    #
-    executor.config.task_queue_length = 30
+        await executor.run_job(RunData(logId=101 + i, **run_data))
+
+    await executor.shutdown()
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("handler_name", HANDLER_NAMES)
 async def test_runner_DISCARD_LATER(executor: Executor, job_id: int, handler_name: str):
     executor.reset_handler(job_handler)
     executor.xxl_client.clear_result()
@@ -168,15 +165,15 @@
         executorHandler=handler_name,
         executorBlockStrategy=executorBlockStrategy.COVER_EARLY.value,
     )
     await executor.run_job(RunData(logId=40, **run_data))
     await executor.run_job(RunData(logId=41, **run_data))
     await executor.graceful_close()
     assert executor.xxl_client.callback_result.get(41) == 200
-    assert executor.xxl_client.callback_result.get(40) is None
+    assert executor.xxl_client.callback_result.get(40) == 500
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("handler_name", HANDLER_NAMES)
 async def test_runner_OTHER(executor: Executor, job_id: int, handler_name: str):
     executor.reset_handler(job_handler)
     with pytest.raises(JobParamsError, match="unknown executorBlockStrategy"):
```

### Comparing `pyxxl-0.3.0a3/pyxxl/tests/test_handler.py` & `pyxxl-0.3.1/pyxxl/tests/test_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import asyncio
 import time
-from concurrent.futures import ThreadPoolExecutor
 
 import pytest
 
 from pyxxl.ctx import g
 from pyxxl.executor import HandlerInfo
 
 
@@ -15,55 +14,51 @@
     async def _handler():
         while True:
             await asyncio.sleep(0.5)
             r.append(1)
 
     handler = HandlerInfo(handler=_handler)
     with pytest.raises(asyncio.TimeoutError):
-        await handler.start_async(2)
+        await handler.start(2)
 
     await asyncio.sleep(1)
     now_r_num = len(r)
     await asyncio.sleep(2)
     assert len(r) == now_r_num
 
 
 @pytest.mark.asyncio
 async def test_sync_timeout_ok(event_loop):
-    thread_pool = ThreadPoolExecutor(max_workers=10)
     r = []
 
     def _handler():
         while len(r) < 10 and not g.cancel_event.is_set():
             time.sleep(0.5)
             r.append(1)
 
     handler = HandlerInfo(handler=_handler)
     with pytest.raises(asyncio.TimeoutError):
-        await handler.start_sync(event_loop, thread_pool, 2)
+        await handler.start(2)
 
     await asyncio.sleep(1)
     now_r_num = len(r)
     await asyncio.sleep(2)
     assert len(r) == now_r_num
 
 
 @pytest.mark.asyncio
 async def test_sync_timeout_error(event_loop):
-    thread_pool = ThreadPoolExecutor(max_workers=10)
-
     r = []
 
     def _handler():
         while len(r) < 10:  # 防止测试线程卡死
             time.sleep(0.5)
             r.append(1)
 
     handler = HandlerInfo(handler=_handler)
     with pytest.raises(asyncio.TimeoutError):
-        await handler.start_sync(event_loop, thread_pool, 2)
+        await handler.start(2)
 
     await asyncio.sleep(1)
     now_r_num = len(r)
     await asyncio.sleep(2)
     assert len(r) > now_r_num
-    thread_pool.shutdown(False)
```

### Comparing `pyxxl-0.3.0a3/pyxxl/tests/test_logger.py` & `pyxxl-0.3.1/pyxxl/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.0a3/pyxxl/tests/test_register.py` & `pyxxl-0.3.1/pyxxl/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.0a3/pyxxl/tests/test_setting.py` & `pyxxl-0.3.1/pyxxl/tests/test_setting.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,18 +15,22 @@
     )
     assert setting.executor_host == get_network_ip()
     assert setting.executor_app_name == "test"
 
     # from env
     os.environ["executor_app_name"] = "fromenv"
     os.environ["XXL_ADMIN_BASEURL"] = TEST_ADMIN_URL
+    os.environ["GRACEFUL_TIMEOUT"] = "500"
+    os.environ["GRACEFUL_CLOSE"] = "False"
 
     setting = ExecutorConfig(xxl_admin_baseurl="", executor_app_name="")
-    setting.executor_app_name = "fromenv"
-    setting.xxl_admin_baseurl = TEST_ADMIN_URL
+    assert setting.executor_app_name == "fromenv"
+    assert setting.xxl_admin_baseurl == TEST_ADMIN_URL
+    assert setting.graceful_timeout == 500
+    assert setting.graceful_close is False
     os.environ.clear()
 
 
 @pytest.mark.parametrize(
     "msg,error,kwargs",
     [
         ("admin_url", ValueError, dict(xxl_admin_baseurl="dddd", executor_app_name="test")),
```

### Comparing `pyxxl-0.3.0a3/pyxxl/tests/utils.py` & `pyxxl-0.3.1/pyxxl/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.0a3/pyxxl/utils.py` & `pyxxl-0.3.1/pyxxl/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,70 @@
 import importlib
 import logging
 import socket
+from logging.handlers import RotatingFileHandler
 from typing import Any, List, Optional
 
 from pyxxl.ctx import g
 
 DEFAULT_FORMAT = (
     "%(asctime)s.%(msecs)03d [%(threadName)s] [%(logId)s] "
     "%(levelname)s %(pathname)s(%(funcName)s:%(lineno)d) - %(message)s"
 )
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 STD_FORMATTER = logging.Formatter(DEFAULT_FORMAT, datefmt=DATE_FORMAT)
+DEFAULT_FILE_SIZE = 50 * 1024 * 1024
+DEFAULT_BACKUP_FILE_COUNT = 5
 
 
 def get_network_ip() -> str:
     """获取本机地址,会获取首个网络地址"""
     _, _, ipaddrlist = socket.gethostbyname_ex(socket.gethostname())
     return ipaddrlist[0]
 
 
 def _init_log_record_factory() -> None:
     old_factory = logging.getLogRecordFactory()
 
     def _record_factory(*args: Any, **kwargs: Any) -> logging.LogRecord:
         record: Any = old_factory(*args, **kwargs)
-        xxl_kwargs = g.try_get("xxl_kwargs")
+        xxl_kwargs = g.try_get_data()
         record.logId = xxl_kwargs.logId if xxl_kwargs else "NotInTask"
         return record
 
     logging.setLogRecordFactory(_record_factory)
 
 
 def setup_logging(
+    path: str,
     level: int = logging.INFO,
     custom_handlers: Optional[List[logging.Handler]] = None,
     std_formatter: Optional[logging.Formatter] = None,
 ) -> logging.Logger:
+    logger = logging.getLogger("pyxxl")
+    if logger.handlers:
+        return logger
+
     std_formatter = std_formatter or STD_FORMATTER
 
     _init_log_record_factory()
-    logger = logging.getLogger("pyxxl")
-    logger.setLevel(level)
 
-    handler = logging.StreamHandler()
-    handler.setFormatter(std_formatter)
-    handler.setLevel(level)
-    logger.addHandler(handler)
+    logger.setLevel(level)
 
+    handlers: List[logging.Handler] = [
+        logging.StreamHandler(),
+        RotatingFileHandler(path, maxBytes=DEFAULT_FILE_SIZE, backupCount=DEFAULT_BACKUP_FILE_COUNT, delay=True),
+    ]
     if custom_handlers:
-        for h in custom_handlers:
-            h.setFormatter(std_formatter)
-            h.setLevel(level)
-            logger.addHandler(h)
+        handlers.extend(custom_handlers)
+
+    for h in handlers:
+        h.setFormatter(std_formatter)
+        h.setLevel(level)
+        logger.addHandler(h)
     return logger
 
 
 def try_import(module: str) -> Optional[Any]:
     try:
         return importlib.import_module(module)
     except ImportError:
```

### Comparing `pyxxl-0.3.0a3/pyxxl/xxl_client.py` & `pyxxl-0.3.1/pyxxl/xxl_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 class XXL:
     def __init__(
         self,
         admin_url: str,
         token: Optional[str] = None,
         loop: Optional[asyncio.AbstractEventLoop] = None,
-        retry_times: int = 0,
+        retry_times: int = 1,
         retry_interval: int = 5,
         session: Optional[aiohttp.ClientSession] = None,
         **kwargs: Any,
     ) -> None:
         self.loop = loop or asyncio.get_event_loop()
         kwargs["loop"] = self.loop
 
@@ -54,24 +54,23 @@
         self.retry_times = retry_times
         self.retry_interval = retry_interval
         self.headers = {"XXL-JOB-ACCESS-TOKEN": token} if token else {}
 
     async def registry(self, key: str, value: str) -> bool:
         payload = dict(registryGroup="EXECUTOR", registryKey=key, registryValue=value)
         try:
-            await self._post("registry", payload, retry_times=1)
-            # logger.debug("Registry successful. %s" % payload)
+            await self._post("registry", payload, retry_times=5)
             return True
-        except XXLRegisterError as e:
+        except (XXLRegisterError, ClientError) as e:
             logger.error("Registry executor failed. %s", e.message)
         return False
 
     async def registryRemove(self, key: str, value: str) -> None:
         payload = dict(registryGroup="EXECUTOR", registryKey=key, registryValue=value)
-        await self._post("registryRemove", payload)
+        await self._post("registryRemove", payload, retry_times=3)
         logger.info("RegistryRemove successful. %s" % payload)
 
     async def callback(self, log_id: int, timestamp: int, code: int = 200, msg: str = None) -> None:
         payload = [
             {
                 "logId": log_id,
                 "logDateTim": timestamp,
@@ -79,27 +78,30 @@
                 "handleMsg": msg,
             }
         ]
         await self._post("callback", payload)
         logger.debug("Callback successful. %s" % payload)
 
     async def _post(self, path: str, payload: JsonType, retry_times: Optional[int] = None) -> Response:
-        times = 1
+        times = 0
         retry_times = retry_times or self.retry_times
-        while times <= retry_times or retry_times == 0:
+        while times < retry_times:
             try:
                 async with self.session.post(self.url_path + path, json=payload, headers=self.headers) as response:
                     if response.status == 200:
                         r = Response(**(await response.json()))
                         if not r.ok:
                             raise XXLRegisterError(r.msg or "")
                         return r
                     raise XXLRegisterError(await response.text())
             except aiohttp.ClientConnectionError as e:
-                logger.error(f"Connection error {times} times: {str(e)}, retry afert {self.retry_interval}")
-                await asyncio.sleep(self.retry_interval)
                 times += 1
-        raise ClientError("Connection error, retry times {}".format(times))
+                logger.warning(
+                    "Connection error {} times, retry after {}. {}".format(times, self.retry_interval, str(e))
+                )
+                await asyncio.sleep(self.retry_interval)
+
+        raise ClientError("Connection error after retry times {}".format(times))
 
     async def close(self) -> None:
         await self.session.close()
         logger.info("http session is closed.")
```

### Comparing `pyxxl-0.3.0a3/setup.py` & `pyxxl-0.3.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,231 +1,250 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 2770 7978 786c 272c 2027 7079   \.['pyxxl', 'py
-00000050: 7878 6c2e 6c6f 6767 6572 272c 2027 7079  xxl.logger', 'py
-00000060: 7878 6c2e 7465 7374 7327 2c20 2770 7978  xxl.tests', 'pyx
-00000070: 786c 2e74 6573 7473 2e61 7069 275d 0a0a  xl.tests.api']..
-00000080: 7061 636b 6167 655f 6461 7461 203d 205c  package_data = \
-00000090: 0a7b 2727 3a20 5b27 2a27 5d7d 0a0a 696e  .{'': ['*']}..in
-000000a0: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-000000b0: 205c 0a5b 2761 696f 6669 6c65 733e 3d32   \.['aiofiles>=2
-000000c0: 322e 312e 302c 3c32 332e 302e 3027 2c20  2.1.0,<23.0.0', 
-000000d0: 2761 696f 6874 7470 3e3d 332e 382e 312c  'aiohttp>=3.8.1,
-000000e0: 3c34 2e30 2e30 275d 0a0a 6578 7472 6173  <4.0.0']..extras
-000000f0: 5f72 6571 7569 7265 203d 205c 0a7b 2761  _require = \.{'a
-00000100: 6c6c 273a 205b 2772 6564 6973 3e3d 342e  ll': ['redis>=4.
-00000110: 342e 302c 3c35 2e30 2e30 272c 2027 7079  4.0,<5.0.0', 'py
-00000120: 7468 6f6e 2d64 6f74 656e 7627 5d2c 0a20  thon-dotenv'],. 
-00000130: 2764 6f74 656e 7627 3a20 5b27 7079 7468  'dotenv': ['pyth
-00000140: 6f6e 2d64 6f74 656e 7627 5d2c 0a20 2772  on-dotenv'],. 'r
-00000150: 6564 6973 273a 205b 2772 6564 6973 3e3d  edis': ['redis>=
-00000160: 342e 342e 302c 3c35 2e30 2e30 275d 7d0a  4.4.0,<5.0.0']}.
-00000170: 0a73 6574 7570 5f6b 7761 7267 7320 3d20  .setup_kwargs = 
-00000180: 7b0a 2020 2020 276e 616d 6527 3a20 2770  {.    'name': 'p
-00000190: 7978 786c 272c 0a20 2020 2027 7665 7273  yxxl',.    'vers
-000001a0: 696f 6e27 3a20 2730 2e33 2e30 6133 272c  ion': '0.3.0a3',
-000001b0: 0a20 2020 2027 6465 7363 7269 7074 696f  .    'descriptio
-000001c0: 6e27 3a20 2741 2050 7974 686f 6e20 6578  n': 'A Python ex
-000001d0: 6563 7574 6f72 2066 6f72 2058 584c 2d6a  ecutor for XXL-j
-000001e0: 6f62 7327 2c0a 2020 2020 276c 6f6e 675f  obs',.    'long_
-000001f0: 6465 7363 7269 7074 696f 6e27 3a20 2723  description': '#
-00000200: 2078 786c 2d6a 6f62 7320 e79a 8470 7974   xxl-jobs ...pyt
-00000210: 686f 6ee5 aea2 e688 b7e7 abaf e5ae 9ee7  hon.............
-00000220: 8eb0 5c6e 5c6e 3c70 2061 6c69 676e 3d22  ..\n\n<p align="
-00000230: 6365 6e74 6572 223e 5c6e 3c61 2068 7265  center">\n<a hre
-00000240: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
-00000250: 6f72 672f 7072 6f6a 6563 742f 7079 7878  org/project/pyxx
-00000260: 6c22 2074 6172 6765 743d 225f 626c 616e  l" target="_blan
-00000270: 6b22 3e5c 6e20 2020 203c 696d 6720 7372  k">\n    <img sr
-00000280: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000290: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-000002a0: 2f70 7978 786c 3f63 6f6c 6f72 3d25 3233  /pyxxl?color=%23
-000002b0: 3334 4430 3538 266c 6162 656c 3d70 7970  34D058&label=pyp
-000002c0: 6925 3230 7061 636b 6167 6522 2061 6c74  i%20package" alt
-000002d0: 3d22 5061 636b 6167 6520 7665 7273 696f  ="Package versio
-000002e0: 6e22 3e5c 6e3c 2f61 3e5c 6e3c 6120 6872  n">\n</a>\n<a hr
-000002f0: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
-00000300: 2e6f 7267 2f70 726f 6a65 6374 2f70 7978  .org/project/pyx
-00000310: 786c 2220 7461 7267 6574 3d22 5f62 6c61  xl" target="_bla
-00000320: 6e6b 223e 5c6e 2020 2020 3c69 6d67 2073  nk">\n    <img s
-00000330: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000340: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000350: 7079 7665 7273 696f 6e73 2f70 7978 786c  pyversions/pyxxl
-00000360: 2e73 7667 3f63 6f6c 6f72 3d25 3233 3334  .svg?color=%2334
-00000370: 4430 3538 2220 616c 743d 2253 7570 706f  D058" alt="Suppo
-00000380: 7274 6564 2050 7974 686f 6e20 7665 7273  rted Python vers
-00000390: 696f 6e73 223e 5c6e 3c2f 613e 5c6e 3c61  ions">\n</a>\n<a
-000003a0: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
-000003b0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-000003c0: 7079 7878 6c22 2074 6172 6765 743d 225f  pyxxl" target="_
-000003d0: 626c 616e 6b22 3e5c 6e20 2020 203c 696d  blank">\n    <im
-000003e0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-000003f0: 6d67 2e73 6869 656c 6473 2e69 6f2f 636f  mg.shields.io/co
-00000400: 6465 636f 762f 632f 6769 7468 7562 2f66  decov/c/github/f
-00000410: 6366 616e 6763 632f 7079 7878 6c3f 636f  cfangcc/pyxxl?co
-00000420: 6c6f 723d 2532 3333 3444 3035 3822 2061  lor=%2334D058" a
-00000430: 6c74 3d22 436f 7665 7261 6765 223e 5c6e  lt="Coverage">\n
-00000440: 3c2f 613e 5c6e 3c2f 703e 5c6e 5c6e e4bd  </a>\n</p>\n\n..
-00000450: bfe7 94a8 7079 7878 6ce5 8faf e4bb a5e6  ....pyxxl.......
-00000460: 96b9 e4be bfe7 9a84 e68a 8a50 7974 686f  ...........Pytho
-00000470: 6ee5 8699 e79a 84e6 96b9 e6b3 95e6 b3a8  n...............
-00000480: e586 8ce5 88b0 5b58 584c 2d4a 4f42 5d28  ......[XXL-JOB](
-00000490: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000004a0: 6f6d 2f78 7578 7565 6c69 2f78 786c 2d6a  om/xuxueli/xxl-j
-000004b0: 6f62 29e4 b8ad 2ce4 bdbf e794 a858 584c  ob)...,......XXL
-000004c0: 2d4a 4f42 2d41 444d 494e e7ae a1e7 9086  -JOB-ADMIN......
-000004d0: 5079 7468 6f6e e5ae 9ae6 97b6 e4bb bbe5  Python..........
-000004e0: 8aa1 e592 8ce5 91a8 e69c 9fe4 bbbb e58a  ................
-000004f0: a15c 6e5c 6ee5 ae9e e78e b0e5 8e9f e790  .\n\n...........
-00000500: 86ef bc9a e980 9ae8 bf87 5858 4c2d 4a4f  ..........XXL-JO
-00000510: 42e6 8f90 e4be 9be7 9a84 5245 5354 6675  B.........RESTfu
-00000520: 6c20 4150 49e6 8ea5 e58f a3e8 bf9b e8a1  l API...........
-00000530: 8ce5 afb9 e68e a55c 6e5c 6e3c 666f 6e74  .......\n\n<font
-00000540: 2063 6f6c 6f72 3d22 2364 6430 3030 3022   color="#dd0000"
-00000550: 3ee6 b3a8 e684 8fef bc81 efbc 81ef bc81  >...............
-00000560: e5a6 82e6 9e9c e794 a8e5 908c e6ad a5e7  ................
-00000570: 9a84 e696 b9e6 b395 efbc 8ce6 9e81 e7ab  ................
-00000580: afe6 8385 e586 b5e4 b88b e4bc 9ae5 8da1  ................
-00000590: e4bd 8fe4 b8bb e7ba bfe7 a88b e380 82e5  ................
-000005a0: a682 e69e 9ce6 97a0 e6b3 95e5 85a8 e5bc  ................
-000005b0: 82e6 ada5 e7bc 96e7 a88b e79a 84ef bc8c  ................
-000005c0: e8b0 a8e6 858e e4bd bfe7 94a8 e69c ace4  ................
-000005d0: bb93 e5ba 93e3 8082 3c2f 666f 6e74 3e5c  ........</font>\
-000005e0: 6e5c 6e23 2320 e5b7 b2e7 bb8f e694 afe6  n\n## ..........
-000005f0: 8c81 e79a 84e5 8a9f e883 bd5c 6e5c 6e2a  ...........\n\n*
-00000600: 20e6 89a7 e8a1 8ce5 99a8 e6b3 a8e5 868c   ...............
-00000610: e588 b06a 6f62 2d61 646d 696e 5c6e 2a20  ...job-admin\n* 
-00000620: 7461 736b e6b3 a8e5 868c efbc 8ce7 b1bb  task............
-00000630: e4bc bce4 ba8e 666c 6173 6be8 b7af e794  ......flask.....
-00000640: b1e8 a385 e9a5 b0e5 99a8 e79a 84e7 94a8  ................
-00000650: e6b3 955c 6e2a 20e4 bbbb e58a a1e7 9a84  ...\n* .........
-00000660: e7ae a1e7 9086 efbc 88e6 94af e68c 81e5  ................
-00000670: 9ca8 e795 8ce9 9da2 e4b8 8ae5 8f96 e6b6  ................
-00000680: 88ef bc8c e58f 91e8 b5b7 e7ad 89e6 938d  ................
-00000690: e4bd 9cef bc8c e4bb bbe5 8aa1 e5ae 8ce6  ................
-000006a0: 8890 e590 8ee4 bc9a e59b 9ee8 b083 6164  ..............ad
-000006b0: 6d69 6eef bc89 5c6e 2a20 e689 80e6 9c89  min...\n* ......
-000006c0: e998 bbe5 a19e e7ad 96e7 95a5 e79a 84e6  ................
-000006d0: 94af e68c 815c 6e2a 20e5 bc82 e6ad a5e6  .....\n* .......
-000006e0: 94af e68c 81ef bc88 e68e a8e8 8d90 efbc  ................
-000006f0: 895c 6e2a 206a 6f62 2d61 646d 696e e4b8  .\n* job-admin..
-00000700: 8ae6 9fa5 e79c 8be6 97a5 e5bf 975c 6e5c  .............\n\
-00000710: 6e23 2320 e980 82e9 858d e79a 8458 584c  n## .........XXL
-00000720: 2d4a 4f42 e789 88e6 9cac 5c6e 5c6e 2a20  -JOB......\n\n* 
-00000730: 5858 4c2d 4a4f 423a 322e 332e 305c 6e5c  XXL-JOB:2.3.0\n\
-00000740: 6ee5 a682 e981 87e5 88b0 e4b8 8de5 85bc  n...............
-00000750: e5ae b9e7 9a84 e683 85e5 86b5 e8af b769  ...............i
-00000760: 7373 7565 e591 8ae8 af89 e688 9158 584c  ssue.........XXL
-00000770: 2d4a 4f42 e789 88e6 9cac e688 91e4 bc9a  -JOB............
-00000780: e5b0 bde9 878f e980 82e9 858d 5c6e 5c6e  ............\n\n
-00000790: 2323 20e5 a682 e4bd 95e4 bdbf e794 a85c  ## ............\
-000007a0: 6e5c 6e60 6060 7368 656c 6c5c 6e70 6970  n\n```shell\npip
-000007b0: 2069 6e73 7461 6c6c 2070 7978 786c 5c6e   install pyxxl\n
-000007c0: 2320 e5a6 82e6 9e9c e697 a5e5 bf97 e99c  # ..............
-000007d0: 80e8 a681 e586 99e5 85a5 7265 6469 735c  ..........redis\
-000007e0: 6e70 6970 2069 6e73 7461 6c6c 2070 7978  npip install pyx
-000007f0: 786c 5b72 6564 6973 5d5c 6e23 20e5 a682  xl[redis]\n# ...
-00000800: e69e 9ce9 9c80 e8a6 81e4 bb8e 2e65 6e76  .............env
-00000810: e58a a0e8 bdbd e985 8de7 bdae 5c6e 7069  ............\npi
-00000820: 7020 696e 7374 616c 6c20 7079 7878 6c5b  p install pyxxl[
-00000830: 646f 7465 6e76 5d5c 6e23 20e5 ae89 e8a3  dotenv]\n# .....
-00000840: 85e6 8980 e69c 89e5 8a9f e883 bd5c 6e70  .............\np
-00000850: 6970 2069 6e73 7461 6c6c 2070 7978 786c  ip install pyxxl
-00000860: 5b61 6c6c 5d5c 6e60 6060 5c6e 5c6e 6060  [all]\n```\n\n``
-00000870: 6070 7974 686f 6e5c 6e69 6d70 6f72 7420  `python\nimport 
-00000880: 6173 796e 6369 6f5c 6e5c 6e66 726f 6d20  asyncio\n\nfrom 
-00000890: 7079 7878 6c20 696d 706f 7274 2045 7865  pyxxl import Exe
-000008a0: 6375 746f 7243 6f6e 6669 672c 2050 7978  cutorConfig, Pyx
-000008b0: 786c 5275 6e6e 6572 5c6e 5c6e 636f 6e66  xlRunner\n\nconf
-000008c0: 6967 203d 2045 7865 6375 746f 7243 6f6e  ig = ExecutorCon
-000008d0: 6669 6728 5c6e 2020 2020 7878 6c5f 6164  fig(\n    xxl_ad
-000008e0: 6d69 6e5f 6261 7365 7572 6c3d 2268 7474  min_baseurl="htt
-000008f0: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3830  p://localhost:80
-00000900: 3830 2f78 786c 2d6a 6f62 2d61 646d 696e  80/xxl-job-admin
-00000910: 2f61 7069 2f22 2c5c 6e20 2020 2065 7865  /api/",\n    exe
-00000920: 6375 746f 725f 6170 705f 6e61 6d65 3d22  cutor_app_name="
-00000930: 7878 6c2d 6a6f 622d 6578 6563 7574 6f72  xxl-job-executor
-00000940: 2d73 616d 706c 6522 2c5c 6e20 2020 2065  -sample",\n    e
-00000950: 7865 6375 746f 725f 686f 7374 3d22 3137  xecutor_host="17
-00000960: 322e 3137 2e30 2e31 222c 5c6e 295c 6e5c  2.17.0.1",\n)\n\
-00000970: 6e61 7070 203d 2050 7978 786c 5275 6e6e  napp = PyxxlRunn
-00000980: 6572 2863 6f6e 6669 6729 5c6e 5c6e 4061  er(config)\n\n@a
-00000990: 7070 2e68 616e 646c 6572 2e72 6567 6973  pp.handler.regis
-000009a0: 7465 7228 6e61 6d65 3d22 6465 6d6f 4a6f  ter(name="demoJo
-000009b0: 6248 616e 646c 6572 2229 5c6e 6173 796e  bHandler")\nasyn
-000009c0: 6320 6465 6620 7465 7374 5f74 6173 6b28  c def test_task(
-000009d0: 293a 5c6e 2020 2020 6177 6169 7420 6173  ):\n    await as
-000009e0: 796e 6369 6f2e 736c 6565 7028 3529 5c6e  yncio.sleep(5)\n
-000009f0: 2020 2020 7265 7475 726e 2022 e688 90e5      return "....
-00000a00: 8a9f 2e2e 2e22 5c6e 5c6e 2320 e5a6 82e6  ....."\n\n# ....
-00000a10: 9e9c e4bd a0e4 bba3 e7a0 81e9 878c e99d  ................
-00000a20: a2e6 b2a1 e69c 89e5 ae9e e78e b0e5 85a8  ................
-00000a30: e5bc 82e6 ada5 efbc 8ce8 afb7 e4bd bfe7  ................
-00000a40: 94a8 e590 8ce6 ada5 e587 bde6 95b0 efbc  ................
-00000a50: 8ce4 b88d e784 b6e4 bc9a e998 bbe5 a19e  ................
-00000a60: e585 b6e4 bb96 e4bb bbe5 8aa1 5c6e 4061  ............\n@a
-00000a70: 7070 2e68 616e 646c 6572 2e72 6567 6973  pp.handler.regis
-00000a80: 7465 7228 6e61 6d65 3d22 7878 7878 7822  ter(name="xxxxx"
-00000a90: 295c 6e64 6566 2074 6573 745f 7461 736b  )\ndef test_task
-00000aa0: 3328 293a 5c6e 2020 2020 7265 7475 726e  3():\n    return
-00000ab0: 2022 e688 90e5 8a9f 3322 5c6e 5c6e 5c6e   "......3"\n\n\n
-00000ac0: 6170 702e 7275 6e5f 6578 6563 7574 6f72  app.run_executor
-00000ad0: 2829 5c6e 6060 605c 6e5c 6e5c 6ee6 9bb4  ()\n```\n\n\n...
-00000ae0: e5a4 9ae7 a4ba e4be 8be5 928c e68e a5e5  ................
-00000af0: 8fa3 e696 87e6 a1a3 e8af b7e5 8f82 e880  ................
-00000b00: 8320 5b50 5958 584c e696 87e6 a1a3 5d28  . [PYXXL......](
-00000b10: 6874 7470 733a 2f2f 6663 6661 6e67 6363  https://fcfangcc
-00000b20: 2e67 6974 6875 622e 696f 2f70 7978 786c  .github.io/pyxxl
-00000b30: 2f65 7861 6d70 6c65 2f29 20ef bc8c e585  /example/) .....
-00000b40: b7e4 bd93 e4bb a3e7 a081 e59c a865 7861  .............exa
-00000b50: 6d70 6c65 e696 87e4 bbb6 e5a4 b9e4 b88b  mple............
-00000b60: e99d a25c 6e5c 6e5c 6e23 2320 e5bc 80e5  ...\n\n\n## ....
-00000b70: 8f91 e4ba bae5 9198 5c6e e4b8 8be9 9da2  ........\n......
-00000b80: e698 afe5 bc80 e58f 91e4 baba e591 98e5  ................
-00000b90: a682 e4bd 95e5 bfab e68d b7e7 9a84 e690  ................
-00000ba0: ade5 bbba e5bc 80e5 8f91 e8b0 83e8 af95  ................
-00000bb0: e78e afe5 a283 5c6e 5c6e 2323 2320 e590  ......\n\n### ..
-00000bc0: afe5 8aa8 7878 6ce7 9a84 e8b0 83e5 baa6  ....xxl.........
-00000bd0: e4b8 ade5 bf83 5c6e 5c6e 6060 6073 6865  ......\n\n```she
-00000be0: 6c6c 5c6e 2e2f 696e 6974 5f64 6576 5f65  ll\n./init_dev_e
-00000bf0: 6e76 2e73 685c 6e60 6060 5c6e 5c6e 5c6e  nv.sh\n```\n\n\n
-00000c00: 2323 2320 e590 afe5 8aa8 e689 a7e8 a18c  ### ............
-00000c10: e599 a85c 6e5c 6e5c 6e60 6060 7368 656c  ...\n\n\n```shel
-00000c20: 6c5c 6e23 2069 6620 796f 7520 6e65 6564  l\n# if you need
-00000c30: 2e20 7365 7420 7665 6e76 2069 6e20 7072  . set venv in pr
-00000c40: 6f6a 6563 742e 5c6e 2320 706f 6574 7279  oject.\n# poetry
-00000c50: 2063 6f6e 6669 6720 7669 7274 7561 6c65   config virtuale
-00000c60: 6e76 732e 696e 2d70 726f 6a65 6374 2074  nvs.in-project t
-00000c70: 7275 655c 6e70 6f65 7472 7920 696e 7374  rue\npoetry inst
-00000c80: 616c 6c20 2d2d 616c 6c2d 6578 7472 6173  all --all-extras
-00000c90: 5c6e 2320 e4bf aee6 94b9 6170 702e 7079  \n# ......app.py
-00000ca0: e4b8 ade7 9bb8 e585 b3e7 9a84 e985 8de7  ................
-00000cb0: bdae e4bf a1e6 81af 2ce7 84b6 e590 8ee5  ........,.......
-00000cc0: 90af e58a a85c 6e70 6f65 7472 7920 7275  .....\npoetry ru
-00000cd0: 6e20 7079 7468 6f6e 2065 7861 6d70 6c65  n python example
-00000ce0: 2f61 7070 2e70 795c 6e60 6060 5c6e 272c  /app.py\n```\n',
-00000cf0: 0a20 2020 2027 6175 7468 6f72 273a 2027  .    'author': '
-00000d00: 6663 6661 6e67 6363 272c 0a20 2020 2027  fcfangcc',.    '
-00000d10: 6175 7468 6f72 5f65 6d61 696c 273a 2027  author_email': '
-00000d20: 7377 6a66 6332 3240 6c69 7665 2e63 6f6d  swjfc22@live.com
-00000d30: 272c 0a20 2020 2027 6d61 696e 7461 696e  ',.    'maintain
-00000d40: 6572 273a 2027 4e6f 6e65 272c 0a20 2020  er': 'None',.   
-00000d50: 2027 6d61 696e 7461 696e 6572 5f65 6d61   'maintainer_ema
-00000d60: 696c 273a 2027 4e6f 6e65 272c 0a20 2020  il': 'None',.   
-00000d70: 2027 7572 6c27 3a20 2768 7474 7073 3a2f   'url': 'https:/
-00000d80: 2f67 6974 6875 622e 636f 6d2f 6663 6661  /github.com/fcfa
-00000d90: 6e67 6363 2f70 7978 786c 272c 0a20 2020  ngcc/pyxxl',.   
-00000da0: 2027 7061 636b 6167 6573 273a 2070 6163   'packages': pac
-00000db0: 6b61 6765 732c 0a20 2020 2027 7061 636b  kages,.    'pack
-00000dc0: 6167 655f 6461 7461 273a 2070 6163 6b61  age_data': packa
-00000dd0: 6765 5f64 6174 612c 0a20 2020 2027 696e  ge_data,.    'in
-00000de0: 7374 616c 6c5f 7265 7175 6972 6573 273a  stall_requires':
-00000df0: 2069 6e73 7461 6c6c 5f72 6571 7569 7265   install_require
-00000e00: 732c 0a20 2020 2027 6578 7472 6173 5f72  s,.    'extras_r
-00000e10: 6571 7569 7265 273a 2065 7874 7261 735f  equire': extras_
-00000e20: 7265 7175 6972 652c 0a20 2020 2027 7079  require,.    'py
-00000e30: 7468 6f6e 5f72 6571 7569 7265 7327 3a20  thon_requires': 
-00000e40: 273e 3d33 2e38 2c3c 342e 3027 2c0a 7d0a  '>=3.8,<4.0',.}.
-00000e50: 0a0a 7365 7475 7028 2a2a 7365 7475 705f  ..setup(**setup_
-00000e60: 6b77 6172 6773 290a                      kwargs).
+00000000: 2320 7878 6c2d 6a6f 6273 20e7 9a84 7079  # xxl-jobs ...py
+00000010: 7468 6f6e e5ae a2e6 88b7 e7ab afe5 ae9e  thon............
+00000020: e78e b00a 0a3c 7020 616c 6967 6e3d 2263  .....<p align="c
+00000030: 656e 7465 7222 3e0a 3c61 2068 7265 663d  enter">.<a href=
+00000040: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
+00000050: 672f 7072 6f6a 6563 742f 7079 7878 6c22  g/project/pyxxl"
+00000060: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000070: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+00000080: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000090: 6c64 732e 696f 2f70 7970 692f 762f 7079  lds.io/pypi/v/py
+000000a0: 7878 6c3f 636f 6c6f 723d 2532 3333 3444  xxl?color=%2334D
+000000b0: 3035 3826 6c61 6265 6c3d 7079 7069 2532  058&label=pypi%2
+000000c0: 3070 6163 6b61 6765 2220 616c 743d 2250  0package" alt="P
+000000d0: 6163 6b61 6765 2076 6572 7369 6f6e 223e  ackage version">
+000000e0: 0a3c 2f61 3e0a 3c61 2068 7265 663d 2268  .</a>.<a href="h
+000000f0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00000100: 7072 6f6a 6563 742f 7079 7878 6c22 2074  project/pyxxl" t
+00000110: 6172 6765 743d 225f 626c 616e 6b22 3e0a  arget="_blank">.
+00000120: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000130: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000140: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
+00000150: 696f 6e73 2f70 7978 786c 2e73 7667 3f63  ions/pyxxl.svg?c
+00000160: 6f6c 6f72 3d25 3233 3334 4430 3538 2220  olor=%2334D058" 
+00000170: 616c 743d 2253 7570 706f 7274 6564 2050  alt="Supported P
+00000180: 7974 686f 6e20 7665 7273 696f 6e73 223e  ython versions">
+00000190: 0a3c 2f61 3e0a 3c61 2068 7265 663d 2268  .</a>.<a href="h
+000001a0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+000001b0: 7072 6f6a 6563 742f 7079 7878 6c22 2074  project/pyxxl" t
+000001c0: 6172 6765 743d 225f 626c 616e 6b22 3e0a  arget="_blank">.
+000001d0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000001e0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000001f0: 732e 696f 2f63 6f64 6563 6f76 2f63 2f67  s.io/codecov/c/g
+00000200: 6974 6875 622f 6663 6661 6e67 6363 2f70  ithub/fcfangcc/p
+00000210: 7978 786c 3f63 6f6c 6f72 3d25 3233 3334  yxxl?color=%2334
+00000220: 4430 3538 2220 616c 743d 2243 6f76 6572  D058" alt="Cover
+00000230: 6167 6522 3e0a 3c2f 613e 0a3c 2f70 3e0a  age">.</a>.</p>.
+00000240: 0ae4 bdbf e794 a870 7978 786c e58f afe4  .......pyxxl....
+00000250: bba5 e696 b9e4 bebf e79a 84e6 8a8a 5079  ..............Py
+00000260: 7468 6f6e e586 99e7 9a84 e696 b9e6 b395  thon............
+00000270: e6b3 a8e5 868c e588 b05b 5858 4c2d 4a4f  .........[XXL-JO
+00000280: 425d 2868 7474 7073 3a2f 2f67 6974 6875  B](https://githu
+00000290: 622e 636f 6d2f 7875 7875 656c 692f 7878  b.com/xuxueli/xx
+000002a0: 6c2d 6a6f 6229 e4b8 ad2c e4bd bfe7 94a8  l-job)...,......
+000002b0: 5858 4c2d 4a4f 422d 4144 4d49 4ee7 aea1  XXL-JOB-ADMIN...
+000002c0: e790 8650 7974 686f 6ee5 ae9a e697 b6e4  ...Python.......
+000002d0: bbbb e58a a1e5 928c e591 a8e6 9c9f e4bb  ................
+000002e0: bbe5 8aa1 0a0a e5ae 9ee7 8eb0 e58e 9fe7  ................
+000002f0: 9086 efbc 9ae9 809a e8bf 8758 584c 2d4a  ...........XXL-J
+00000300: 4f42 e68f 90e4 be9b e79a 8452 4553 5466  OB.........RESTf
+00000310: 756c 2041 5049 e68e a5e5 8fa3 e8bf 9be8  ul API..........
+00000320: a18c e5af b9e6 8ea5 0a0a 3c66 6f6e 7420  ..........<font 
+00000330: 636f 6c6f 723d 2223 6464 3030 3030 223e  color="#dd0000">
+00000340: e6b3 a8e6 848f efbc 81ef bc81 efbc 81e5  ................
+00000350: a682 e69e 9ce7 94a8 e590 8ce6 ada5 e79a  ................
+00000360: 84e6 96b9 e6b3 95ef bc8c e8af b7e6 9fa5  ................
+00000370: e79c 8be4 b88b e99d a2e5 908c e6ad a5e4  ................
+00000380: bbbb e58a a1e6 b3a8 e684 8fe4 ba8b e9a1  ................
+00000390: b9e3 8082 3c2f 666f 6e74 3e0a 0a23 2320  ....</font>..## 
+000003a0: e5b7 b2e7 bb8f e694 afe6 8c81 e79a 84e5  ................
+000003b0: 8a9f e883 bd0a 0a2a 20e6 89a7 e8a1 8ce5  .......* .......
+000003c0: 99a8 e6b3 a8e5 868c e588 b06a 6f62 2d61  ...........job-a
+000003d0: 646d 696e 0a2a 2074 6173 6be6 b3a8 e586  dmin.* task.....
+000003e0: 8cef bc8c e7b1 bbe4 bcbc e4ba 8e66 6c61  .............fla
+000003f0: 736b e8b7 afe7 94b1 e8a3 85e9 a5b0 e599  sk..............
+00000400: a8e7 9a84 e794 a8e6 b395 0a2a 20e4 bbbb  ...........* ...
+00000410: e58a a1e7 9a84 e7ae a1e7 9086 efbc 88e6  ................
+00000420: 94af e68c 81e5 9ca8 e795 8ce9 9da2 e4b8  ................
+00000430: 8ae5 8f96 e6b6 88ef bc8c e58f 91e8 b5b7  ................
+00000440: e7ad 89e6 938d e4bd 9cef bc8c e4bb bbe5  ................
+00000450: 8aa1 e5ae 8ce6 8890 e590 8ee4 bc9a e59b  ................
+00000460: 9ee8 b083 6164 6d69 6eef bc89 0a2a 20e6  ....admin....* .
+00000470: 8980 e69c 89e9 98bb e5a1 9ee7 ad96 e795  ................
+00000480: a5e7 9a84 e694 afe6 8c81 0a2a 20e5 bc82  ...........* ...
+00000490: e6ad a5e6 94af e68c 81ef bc88 e68e a8e8  ................
+000004a0: 8d90 efbc 890a 2a20 6a6f 622d 6164 6d69  ......* job-admi
+000004b0: 6ee4 b88a e69f a5e7 9c8b e697 a5e5 bf97  n...............
+000004c0: 0a0a 2323 20e9 8082 e985 8de7 9a84 5858  ..## .........XX
+000004d0: 4c2d 4a4f 42e7 8988 e69c ac0a 0a2a 2058  L-JOB........* X
+000004e0: 584c 2d4a 4f42 3a32 2e33 2e30 0a0a e5a6  XL-JOB:2.3.0....
+000004f0: 82e9 8187 e588 b0e4 b88d e585 bce5 aeb9  ................
+00000500: e79a 84e6 8385 e586 b5e8 afb7 6973 7375  ............issu
+00000510: 65e5 918a e8af 89e6 8891 5858 4c2d 4a4f  e.........XXL-JO
+00000520: 42e7 8988 e69c ace6 8891 e4bc 9ae5 b0bd  B...............
+00000530: e987 8fe9 8082 e985 8d0a 0a23 2320 e5a6  ...........## ..
+00000540: 82e4 bd95 e4bd bfe7 94a8 0a0a 6060 6073  ............```s
+00000550: 6865 6c6c 0a70 6970 2069 6e73 7461 6c6c  hell.pip install
+00000560: 2070 7978 786c 0a23 20e5 a682 e69e 9ce6   pyxxl.# .......
+00000570: 97a5 e5bf 97e9 9c80 e8a6 81e5 8699 e585  ................
+00000580: a572 6564 6973 0a70 6970 2069 6e73 7461  .redis.pip insta
+00000590: 6c6c 2022 7079 7878 6c5b 7265 6469 735d  ll "pyxxl[redis]
+000005a0: 220a 2320 e5a6 82e6 9e9c e99c 80e8 a681  ".# ............
+000005b0: e4bb 8e2e 656e 76e5 8aa0 e8bd bde9 858d  ....env.........
+000005c0: e7bd ae0a 7069 7020 696e 7374 616c 6c20  ....pip install 
+000005d0: 2270 7978 786c 5b64 6f74 656e 765d 220a  "pyxxl[dotenv]".
+000005e0: 2320 e5ae 89e8 a385 e689 80e6 9c89 e58a  # ..............
+000005f0: 9fe8 83bd 0a70 6970 2069 6e73 7461 6c6c  .....pip install
+00000600: 2022 7079 7878 6c5b 616c 6c5d 220a 6060   "pyxxl[all]".``
+00000610: 600a 0a60 6060 7079 7468 6f6e 0a69 6d70  `..```python.imp
+00000620: 6f72 7420 6173 796e 6369 6f0a 0a66 726f  ort asyncio..fro
+00000630: 6d20 7079 7878 6c20 696d 706f 7274 2045  m pyxxl import E
+00000640: 7865 6375 746f 7243 6f6e 6669 672c 2050  xecutorConfig, P
+00000650: 7978 786c 5275 6e6e 6572 0a0a 636f 6e66  yxxlRunner..conf
+00000660: 6967 203d 2045 7865 6375 746f 7243 6f6e  ig = ExecutorCon
+00000670: 6669 6728 0a20 2020 2078 786c 5f61 646d  fig(.    xxl_adm
+00000680: 696e 5f62 6173 6575 726c 3d22 6874 7470  in_baseurl="http
+00000690: 3a2f 2f6c 6f63 616c 686f 7374 3a38 3038  ://localhost:808
+000006a0: 302f 7878 6c2d 6a6f 622d 6164 6d69 6e2f  0/xxl-job-admin/
+000006b0: 6170 692f 222c 0a20 2020 2065 7865 6375  api/",.    execu
+000006c0: 746f 725f 6170 705f 6e61 6d65 3d22 7878  tor_app_name="xx
+000006d0: 6c2d 6a6f 622d 6578 6563 7574 6f72 2d73  l-job-executor-s
+000006e0: 616d 706c 6522 2c0a 2020 2020 6578 6563  ample",.    exec
+000006f0: 7574 6f72 5f68 6f73 743d 2231 3732 2e31  utor_host="172.1
+00000700: 372e 302e 3122 2c0a 290a 0a61 7070 203d  7.0.1",.)..app =
+00000710: 2050 7978 786c 5275 6e6e 6572 2863 6f6e   PyxxlRunner(con
+00000720: 6669 6729 0a0a 4061 7070 2e68 616e 646c  fig)..@app.handl
+00000730: 6572 2e72 6567 6973 7465 7228 6e61 6d65  er.register(name
+00000740: 3d22 6465 6d6f 4a6f 6248 616e 646c 6572  ="demoJobHandler
+00000750: 2229 0a61 7379 6e63 2064 6566 2074 6573  ").async def tes
+00000760: 745f 7461 736b 2829 3a0a 2020 2020 6177  t_task():.    aw
+00000770: 6169 7420 6173 796e 6369 6f2e 736c 6565  ait asyncio.slee
+00000780: 7028 3529 0a20 2020 2072 6574 7572 6e20  p(5).    return 
+00000790: 22e6 8890 e58a 9f2e 2e2e 220a 0a23 20e5  "........."..# .
+000007a0: a682 e69e 9ce4 bda0 e4bb a3e7 a081 e987  ................
+000007b0: 8ce9 9da2 e6b2 a1e6 9c89 e5ae 9ee7 8eb0  ................
+000007c0: e585 a8e5 bc82 e6ad a5ef bc8c e8af b7e4  ................
+000007d0: bdbf e794 a8e5 908c e6ad a5e5 87bd e695  ................
+000007e0: b0ef bc8c e4b8 8de7 84b6 e4bc 9ae9 98bb  ................
+000007f0: e5a1 9ee5 85b6 e4bb 96e4 bbbb e58a a10a  ................
+00000800: 4061 7070 2e68 616e 646c 6572 2e72 6567  @app.handler.reg
+00000810: 6973 7465 7228 6e61 6d65 3d22 7878 7878  ister(name="xxxx
+00000820: 7822 290a 6465 6620 7465 7374 5f74 6173  x").def test_tas
+00000830: 6b33 2829 3a0a 2020 2020 7265 7475 726e  k3():.    return
+00000840: 2022 e688 90e5 8a9f 3322 0a0a 0a61 7070   "......3"...app
+00000850: 2e72 756e 5f65 7865 6375 746f 7228 290a  .run_executor().
+00000860: 6060 600a 0a0a e69b b4e5 a49a e7a4 bae4  ```.............
+00000870: be8b e592 8ce6 8ea5 e58f a3e6 9687 e6a1  ................
+00000880: a3e8 afb7 e58f 82e8 8083 205b 5059 5858  .......... [PYXX
+00000890: 4ce6 9687 e6a1 a35d 2868 7474 7073 3a2f  L......](https:/
+000008a0: 2f66 6366 616e 6763 632e 6769 7468 7562  /fcfangcc.github
+000008b0: 2e69 6f2f 7079 7878 6c2f 6578 616d 706c  .io/pyxxl/exampl
+000008c0: 652f 2920 efbc 8ce5 85b7 e4bd 93e4 bba3  e/) ............
+000008d0: e7a0 81e5 9ca8 6578 616d 706c 65e6 9687  ......example...
+000008e0: e4bb b6e5 a4b9 e4b8 8be9 9da2 0a0a 2323  ..............##
+000008f0: 20e7 9b91 e68e a7e6 8c87 e6a0 870a 0a60   ..............`
+00000900: 6060 7368 656c 6c0a 7069 7020 696e 7374  ``shell.pip inst
+00000910: 616c 6c20 2270 7978 786c 5b6d 6574 7269  all "pyxxl[metri
+00000920: 6373 5d22 0a60 6060 0a0a e5ae 89e8 a385  cs]".```........
+00000930: 6d65 7472 6963 73e6 89a9 e5b1 95e5 908e  metrics.........
+00000940: efbc 8ce6 89a7 e8a1 8ce5 99a8 e4bc 9ae8  ................
+00000950: 87aa e58a a8e5 8aa0 e8bd bd70 726f 6d65  ...........prome
+00000960: 7468 6575 73e7 9a84 e68c 87e6 a087 e79b  theus...........
+00000970: 91e6 8ea7 e58a 9fe8 83bd 0a0a e8ae bfe9  ................
+00000980: 97ae e59c b0e5 9d80 e4b8 ba3a 2068 7474  ...........: htt
+00000990: 703a 2f2f 6578 6563 7574 6f72 5f68 6f73  p://executor_hos
+000009a0: 743a 706f 7274 2f6d 6574 7269 6373 0a0a  t:port/metrics..
+000009b0: 2323 20e5 908c e6ad a5e4 bbbb e58a a1e6  ## .............
+000009c0: b3a8 e684 8fe4 ba8b e9a1 b90a e590 8ce6  ................
+000009d0: ada5 e4bb bbe5 8aa1 e4bc 9ae6 94be e588  ................
+000009e0: b0e7 babf e7a8 8be6 b1a0 e4b8 ade8 bf90  ................
+000009f0: e8a1 8cef bc8c e697 a0e6 b395 e6ad a3e7  ................
+00000a00: a1ae e68e a5e5 8f97 6361 6e63 656c e4bf  ........cancel..
+00000a10: a1e5 8fb7 e592 8c74 696d 656f 7574 e985  .......timeout..
+00000a20: 8de7 bdae 0a0a e5a6 82e6 9e9c e99c 80e8  ................
+00000a30: a681 e4bd bfe7 94a8 e590 8ce6 ada5 e4bb  ................
+00000a40: bbe5 8aa1 e5b9 b6e4 b894 e697 a0e6 b395  ................
+00000a50: e68e a7e5 88b6 efbc 88e9 a284 e696 99ef  ................
+00000a60: bc89 e987 8ce9 9da2 e689 a7e8 a18c e697  ................
+00000a70: b6e9 97b4 efbc 8ce5 8f88 e99c 80e8 a681  ................
+00000a80: e8bf 9be8 a18c e8b6 85e6 97b6 e592 8c63  ...............c
+00000a90: 616e 6365 6ce5 8a9f e883 bde7 9a84 efbc  ancel...........
+00000aa0: 8ce9 9c80 e8a6 81e6 8ea5 e58f 9770 7978  .............pyx
+00000ab0: 786c e58f 91e5 87ba e79a 8463 616e 6365  xl.........cance
+00000ac0: 6c5f 6576 656e 74ef bc8c e5bd 93e8 afa5  l_event.........
+00000ad0: 6361 6e63 656c 5f65 7665 6e74 e8a2 abe8  cancel_event....
+00000ae0: aebe e7bd aee6 97b6 e99c 80e8 a681 e4b8  ................
+00000af0: ade6 96ad e4bb bbe5 8aa1 efbc 8ce4 b88b  ................
+00000b00: e99d a2e6 98af e4b8 80e4 b8aa e6a1 88e4  ................
+00000b10: be8b 3a0a 0a60 6060 7079 7468 6f6e 0a2e  ..:..```python..
+00000b20: 2e2e 0a0a 4061 7070 2e68 616e 646c 6572  ....@app.handler
+00000b30: 2e72 6567 6973 7465 7228 6e61 6d65 3d22  .register(name="
+00000b40: 7379 6e63 5f66 756e 6322 290a 6465 6620  sync_func").def 
+00000b50: 7379 6e63 5f6c 6f6f 705f 6465 6d6f 2829  sync_loop_demo()
+00000b60: 3a0a 2020 2020 2320 e5a6 82e6 9e9c e590  :.    # ........
+00000b70: 8ce6 ada5 e4bb bbe5 8aa1 e987 8ce9 9da2  ................
+00000b80: e69c 89e5 beaa e78e afef bc8c e4b8 bae4  ................
+00000b90: ba86 e694 afe6 8c81 6361 6e63 656c e693  ........cancel..
+00000ba0: 8de4 bd9c efbc 8ce5 bf85 e9a1 bbe6 af8f  ................
+00000bb0: e6ac a1e9 83bd e588 a4e6 96ad 672e 6361  ............g.ca
+00000bc0: 6e63 656c 5f65 7665 6e74 2e0a 2020 2020  ncel_event..    
+00000bd0: 7461 736b 5f70 6172 616d 735f 6c69 7374  task_params_list
+00000be0: 203d 205b 5d0a 2020 2020 7768 696c 6520   = [].    while 
+00000bf0: 6e6f 7420 672e 6361 6e63 656c 5f65 7665  not g.cancel_eve
+00000c00: 6e74 2e69 735f 7365 7428 2920 616e 6420  nt.is_set() and 
+00000c10: 7461 736b 5f70 6172 6173 6d5f 6c69 7374  task_parasm_list
+00000c20: 3a0a 2020 2020 2020 2020 7061 7261 6d73  :.        params
+00000c30: 203d 2074 6173 6b5f 7061 7261 6d73 5f6c   = task_params_l
+00000c40: 6973 742e 706f 7028 290a 2020 2020 2020  ist.pop().      
+00000c50: 2020 7469 6d65 2e73 6c65 6570 2833 290a    time.sleep(3).
+00000c60: 2020 2020 7265 7475 726e 2022 6f6b 220a      return "ok".
+00000c70: 0a23 20e5 a682 e4b8 8be4 bba3 e7a0 81e4  .# .............
+00000c80: bc9a e980 a0e6 8890 e7ba bfe7 a88b e6b1  ................
+00000c90: a0e9 878c e79a 84e7 babf e7a8 8be8 a2ab  ................
+00000ca0: e6b0 b8e8 bf9c e58d a0e7 94a8 efbc 8c74  ...............t
+00000cb0: 696d 656f 7574 2063 616e 6365 6ce5 85a8  imeout cancel...
+00000cc0: e983 a8e4 b88d e794 9fe6 9588 0a40 6170  .............@ap
+00000cd0: 702e 6861 6e64 6c65 722e 7265 6769 7374  p.handler.regist
+00000ce0: 6572 286e 616d 653d 2273 796e 635f 6675  er(name="sync_fu
+00000cf0: 6e63 3222 290a 6465 6620 7379 6e63 5f6c  nc2").def sync_l
+00000d00: 6f6f 705f 6465 6d6f 3228 293a 0a20 2020  oop_demo2():.   
+00000d10: 2077 6869 6c65 2054 7275 653a 0a20 2020   while True:.   
+00000d20: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
+00000d30: 3329 2023 20e6 a8a1 e68b 9fe4 bda0 e8bf  3) # ...........
+00000d40: 90e8 a18c e79a 84e4 bbbb e58a a10a 2020  ..............  
+00000d50: 2020 7265 7475 726e 2022 6f6b 220a 0a60    return "ok"..`
+00000d60: 6060 0a0a 0a23 2320 e5bc 80e5 8f91 e4ba  ``...## ........
+00000d70: bae5 9198 0ae4 b88b e99d a2e6 98af e5bc  ................
+00000d80: 80e5 8f91 e4ba bae5 9198 e5a6 82e4 bd95  ................
+00000d90: e5bf abe6 8db7 e79a 84e6 90ad e5bb bae5  ................
+00000da0: bc80 e58f 91e8 b083 e8af 95e7 8eaf e5a2  ................
+00000db0: 830a 0a23 2323 20e5 90af e58a a878 786c  ...### ......xxl
+00000dc0: e79a 84e8 b083 e5ba a6e4 b8ad e5bf 830a  ................
+00000dd0: 0a60 6060 7368 656c 6c0a 2e2f 696e 6974  .```shell../init
+00000de0: 5f64 6576 5f65 6e76 2e73 680a 6060 600a  _dev_env.sh.```.
+00000df0: 0a0a 2323 2320 e590 afe5 8aa8 e689 a7e8  ..### ..........
+00000e00: a18c e599 a80a 0a0a 6060 6073 6865 6c6c  ........```shell
+00000e10: 0a23 2069 6620 796f 7520 6e65 6564 2e20  .# if you need. 
+00000e20: 7365 7420 7665 6e76 2069 6e20 7072 6f6a  set venv in proj
+00000e30: 6563 742e 0a23 2070 6f65 7472 7920 636f  ect..# poetry co
+00000e40: 6e66 6967 2076 6972 7475 616c 656e 7673  nfig virtualenvs
+00000e50: 2e69 6e2d 7072 6f6a 6563 7420 7472 7565  .in-project true
+00000e60: 0a70 6f65 7472 7920 696e 7374 616c 6c20  .poetry install 
+00000e70: 2d2d 616c 6c2d 6578 7472 6173 0a23 20e4  --all-extras.# .
+00000e80: bfae e694 b961 7070 2e70 79e4 b8ad e79b  .....app.py.....
+00000e90: b8e5 85b3 e79a 84e9 858d e7bd aee4 bfa1  ................
+00000ea0: e681 af2c e784 b6e5 908e e590 afe5 8aa8  ...,............
+00000eb0: 0a70 6f65 7472 7920 7275 6e20 7079 7468  .poetry run pyth
+00000ec0: 6f6e 2065 7861 6d70 6c65 2f61 7070 2e70  on example/app.p
+00000ed0: 790a 6060 600a 0a23 2320 e585 b6e4 bb96  y.```..## ......
+00000ee0: 0a0a 2a20 e794 b1e4 ba8e e7a7 8de7 a78d  ..* ............
+00000ef0: 332e 39e4 b98b e590 8ee6 898d e58a a0e5  3.9.............
+00000f00: 85a5 e79a 84e8 afad e6b3 95e4 b88e e789  ................
+00000f10: b9e6 80a7 efbc 8ce5 878f e5b0 91e5 bc80  ................
+00000f20: e58f 91e4 b88e e980 82e9 858d e688 90e6  ................
+00000f30: 9cac efbc 8ce8 aea1 e588 92e5 908e e7bb  ................
+00000f40: ade7 8988 e69c ace4 b88d e586 8de9 8082  ................
+00000f50: e985 8d50 7974 686f 6e33 2e39 e4bb a5e4  ...Python3.9....
+00000f60: b88b e789 88e6 9cac efbc 8c30 2e33 2e30  ...........0.3.0
+00000f70: e69c 80e5 908e e4b8 80e4 b8aa e694 afe6  ................
+00000f80: 8c81 5079 7468 6f6e 332e 38e7 9a84 e789  ..Python3.8.....
+00000f90: 88e6 9cac 0a                             .....
```

### Comparing `pyxxl-0.3.0a3/PKG-INFO` & `pyxxl-0.3.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: pyxxl
-Version: 0.3.0a3
+Version: 0.3.1
 Summary: A Python executor for XXL-jobs
 Home-page: https://github.com/fcfangcc/pyxxl
 License: GPL-3.0-only
 Keywords: XXL
 Author: fcfangcc
 Author-email: swjfc22@live.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Provides-Extra: dotenv
+Provides-Extra: metrics
 Provides-Extra: redis
 Requires-Dist: aiofiles (>=22.1.0,<23.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
-Requires-Dist: python-dotenv ; extra == "dotenv" or extra == "all"
-Requires-Dist: redis (>=4.4.0,<5.0.0) ; extra == "redis" or extra == "all"
+Requires-Dist: prometheus-client ; extra == "all" or extra == "metrics"
+Requires-Dist: python-dotenv ; extra == "all" or extra == "dotenv"
+Requires-Dist: redis (>=4.4.0,<5.0.0) ; extra == "all" or extra == "redis"
 Project-URL: Repository, https://github.com/fcfangcc/pyxxl
 Description-Content-Type: text/markdown
 
 # xxl-jobs 的python客户端实现
 
 <p align="center">
 <a href="https://pypi.org/project/pyxxl" target="_blank">
@@ -39,15 +40,15 @@
 </a>
 </p>
 
 使用pyxxl可以方便的把Python写的方法注册到[XXL-JOB](https://github.com/xuxueli/xxl-job)中,使用XXL-JOB-ADMIN管理Python定时任务和周期任务
 
 实现原理：通过XXL-JOB提供的RESTful API接口进行对接
 
-<font color="#dd0000">注意！！！如果用同步的方法，极端情况下会卡住主线程。如果无法全异步编程的，谨慎使用本仓库。</font>
+<font color="#dd0000">注意！！！如果用同步的方法，请查看下面同步任务注意事项。</font>
 
 ## 已经支持的功能
 
 * 执行器注册到job-admin
 * task注册，类似于flask路由装饰器的用法
 * 任务的管理（支持在界面上取消，发起等操作，任务完成后会回调admin）
 * 所有阻塞策略的支持
@@ -61,19 +62,19 @@
 如遇到不兼容的情况请issue告诉我XXL-JOB版本我会尽量适配
 
 ## 如何使用
 
 ```shell
 pip install pyxxl
 # 如果日志需要写入redis
-pip install pyxxl[redis]
+pip install "pyxxl[redis]"
 # 如果需要从.env加载配置
-pip install pyxxl[dotenv]
+pip install "pyxxl[dotenv]"
 # 安装所有功能
-pip install pyxxl[all]
+pip install "pyxxl[all]"
 ```
 
 ```python
 import asyncio
 
 from pyxxl import ExecutorConfig, PyxxlRunner
 
@@ -98,14 +99,50 @@
 
 app.run_executor()
 ```
 
 
 更多示例和接口文档请参考 [PYXXL文档](https://fcfangcc.github.io/pyxxl/example/) ，具体代码在example文件夹下面
 
+## 监控指标
+
+```shell
+pip install "pyxxl[metrics]"
+```
+
+安装metrics扩展后，执行器会自动加载prometheus的指标监控功能
+
+访问地址为: http://executor_host:port/metrics
+
+## 同步任务注意事项
+同步任务会放到线程池中运行，无法正确接受cancel信号和timeout配置
+
+如果需要使用同步任务并且无法控制（预料）里面执行时间，又需要进行超时和cancel功能的，需要接受pyxxl发出的cancel_event，当该cancel_event被设置时需要中断任务，下面是一个案例:
+
+```python
+...
+
+@app.handler.register(name="sync_func")
+def sync_loop_demo():
+    # 如果同步任务里面有循环，为了支持cancel操作，必须每次都判断g.cancel_event.
+    task_params_list = []
+    while not g.cancel_event.is_set() and task_parasm_list:
+        params = task_params_list.pop()
+        time.sleep(3)
+    return "ok"
+
+# 如下代码会造成线程池里的线程被永远占用，timeout cancel全部不生效
+@app.handler.register(name="sync_func2")
+def sync_loop_demo2():
+    while True:
+        time.sleep(3) # 模拟你运行的任务
+    return "ok"
+
+```
+
 
 ## 开发人员
 下面是开发人员如何快捷的搭建开发调试环境
 
 ### 启动xxl的调度中心
 
 ```shell
@@ -120,7 +157,11 @@
 # if you need. set venv in project.
 # poetry config virtualenvs.in-project true
 poetry install --all-extras
 # 修改app.py中相关的配置信息,然后启动
 poetry run python example/app.py
 ```
 
+## 其他
+
+* 由于种种3.9之后才加入的语法与特性，减少开发与适配成本，计划后续版本不再适配Python3.9以下版本，0.3.0最后一个支持Python3.8的版本
+
```

