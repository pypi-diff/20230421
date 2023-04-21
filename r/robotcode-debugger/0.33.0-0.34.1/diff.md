# Comparing `tmp/robotcode_debugger-0.33.0.tar.gz` & `tmp/robotcode_debugger-0.34.1.tar.gz`

## Comparing `robotcode_debugger-0.33.0.tar` & `robotcode_debugger-0.34.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/__version__.py
--rw-r--r--   0        0        0    14681 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/cli.py
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/client.py
--rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/dap_types.py
--rw-r--r--   0        0        0    49747 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/debugger.py
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/listeners.py
--rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/py.typed
--rw-r--r--   0        0        0    14877 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/launcher/__init__.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/launcher/__main__.py
--rw-r--r--   0        0        0     5430 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/launcher/cli.py
--rw-r--r--   0        0        0    12645 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/src/robotcode/debugger/launcher/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/LICENSE.txt
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/README.md
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/pyproject.toml
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 robotcode_debugger-0.33.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/__version__.py
+-rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/cli.py
+-rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/dap_types.py
+-rw-r--r--   0        0        0    49582 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/debugger.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/hooks.py
+-rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/listeners.py
+-rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/py.typed
+-rw-r--r--   0        0        0     7618 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/run.py
+-rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/launcher/__init__.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/launcher/cli.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/launcher/client.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/launcher/run.py
+-rw-r--r--   0        0        0    13643 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/src/robotcode/debugger/launcher/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/LICENSE.txt
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/README.md
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/pyproject.toml
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 robotcode_debugger-0.34.1/PKG-INFO
```

### Comparing `robotcode_debugger-0.33.0/src/robotcode/debugger/client.py` & `robotcode_debugger-0.34.1/src/robotcode/debugger/launcher/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,78 @@
 from __future__ import annotations
 
 import asyncio
 from typing import Any, Optional, Sequence
 
+from robotcode.core.event import event
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.jsonrpc2.server import TcpParams
+from robotcode.core.types import TcpParams
 
-from .dap_types import Event
-from .protocol import DebugAdapterProtocol
+from ..dap_types import Event
+from ..protocol import DebugAdapterProtocol
 
 
 class DAPClientProtocol(DebugAdapterProtocol):
     _logger = LoggingDescriptor()
 
-    def __init__(self, parent: DebugAdapterProtocol) -> None:
+    def __init__(self, parent: DebugAdapterProtocol, client: "DAPClient") -> None:
         super().__init__()
         self.parent = parent
+        self.client = client
         self.exited = False
         self.terminated = False
 
+    @_logger.call
     def handle_event(self, message: Event) -> None:
         if message.event == "exited":
             self.exited = True
+
         elif message.event == "terminated":
             self.terminated = True
+            if self.exited:
+                self.client.close()
+
         self.parent.send_event(Event(event=message.event, body=message.body))
 
 
 class DAPClientError(Exception):
     pass
 
 
 class DAPClient:
+    _logger = LoggingDescriptor()
+
     def __init__(self, parent: DebugAdapterProtocol, tcp_params: TcpParams = TcpParams(None, 0)) -> None:
         self.parent = parent
         self.tcp_params = tcp_params
         self._protocol: Optional[DAPClientProtocol] = None
         self._transport: Optional[asyncio.BaseTransport] = None
 
+    @event
+    def on_closed(sender) -> None:
+        ...
+
+    @_logger.call
     def close(self) -> None:
         if self._transport is not None:
             self._transport.close()
             self._transport = None
             self._protocol = None
 
+        self.on_closed(self)
+
     def __del__(self) -> None:
         self.close()
 
+    @_logger.call
     async def on_connection_lost(self, sender: Any, exc: Optional[BaseException]) -> None:
         if sender == self._protocol:
             self._protocol = None
 
+    @_logger.call
     async def connect(self, timeout: float = 5) -> DAPClientProtocol:
         async def wait() -> None:
             while self._protocol is None:
                 try:
                     if self.tcp_params.host is not None:
                         if isinstance(self.tcp_params.host, Sequence):
                             host = self.tcp_params.host[0]
@@ -79,20 +97,18 @@
             raise DAPClientError("Client already connected.")
 
         await asyncio.wait_for(wait(), timeout=timeout)
 
         return self.protocol
 
     def _create_protocol(self) -> DAPClientProtocol:
-        return DAPClientProtocol(self.parent)
+        return DAPClientProtocol(self.parent, self)
 
     @property
     def connected(self) -> bool:
         return self._protocol is not None
 
     @property
     def protocol(self) -> DAPClientProtocol:
-        import inspect
-
         if self._protocol is None:
-            raise DAPClientError(f"Client is not connected. {inspect.stack()[1][3]}")
+            raise DAPClientError("Client is not connected.")
         return self._protocol
```

### Comparing `robotcode_debugger-0.33.0/src/robotcode/debugger/dap_types.py` & `robotcode_debugger-0.34.1/src/robotcode/debugger/dap_types.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.33.0/src/robotcode/debugger/debugger.py` & `robotcode_debugger-0.34.1/src/robotcode/debugger/debugger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import itertools
 import os
 import pathlib
 import re
 import threading
+import traceback
 import weakref
 from collections import deque
 from enum import Enum
 from pathlib import Path, PurePath
 from typing import (
     Any,
     Callable,
@@ -21,14 +22,19 @@
     NamedTuple,
     Optional,
     Set,
     Tuple,
     Union,
 )
 
+from robot.errors import VariableError
+from robot.running import EXECUTION_CONTEXTS, Keyword
+from robot.running.userkeyword import UserKeywordHandler
+from robot.utils import NormalizedDict
+from robot.variables import evaluate_expression
 from robotcode.core.event import event
 from robotcode.core.logging import LoggingDescriptor
 
 from .dap_types import (
     Breakpoint,
     ContinuedEvent,
     ContinuedEventBody,
@@ -246,30 +252,34 @@
         self.output_messages: bool = False
         self.output_log: bool = False
         self.output_timestamps: bool = False
         self.group_output: bool = False
         self.hit_counts: Dict[HitCountEntry, int] = {}
         self.last_fail_message: Optional[str] = None
         self.stop_on_entry = False
-        self.no_debug = False
+        self._debug = True
         self.terminated = False
         self.terminated_requested = False
         self.attached = False
         self.path_mappings: List[PathMapping] = []
 
         self._keyword_to_evaluate: Optional[Callable[..., Any]] = None
         self._evaluated_keyword_result: Any = None
         self._evaluate_keyword_event = threading.Event()
         self._evaluate_keyword_event.set()
         self._after_evaluate_keyword_event = threading.Event()
         self._after_evaluate_keyword_event.set()
 
     @property
     def debug(self) -> bool:
-        return not self.no_debug
+        return self._debug
+
+    @debug.setter
+    def debug(self, value: bool) -> None:
+        self._debug = value
 
     @property
     def robot_report_file(self) -> Optional[str]:
         return self._robot_report_file
 
     @robot_report_file.setter
     def robot_report_file(self, value: Optional[str]) -> None:
@@ -442,17 +452,14 @@
             ]
 
         self._logger.error("not supported breakpoint")
 
         return []
 
     def process_start_state(self, source: str, line_no: int, type: str, status: str) -> None:
-        from robot.running.context import EXECUTION_CONTEXTS
-        from robot.variables.evaluation import evaluate_expression
-
         if self.state == State.Stopped:
             return
 
         if self.requested_state == RequestedState.Pause:
             self.state = State.Paused
             self.send_event(
                 self,
@@ -662,17 +669,14 @@
         column: Optional[int] = None,
         *,
         handler: Any = None,
         libname: Optional[str] = None,
         kwname: Optional[str] = None,
         longname: Optional[str] = None,
     ) -> StackFrameEntry:
-        from robot.running.context import EXECUTION_CONTEXTS
-        from robot.running.userkeyword import UserKeywordHandler
-
         path = pathlib.Path(source) if source is not None else None
         is_file = path is not None and path.is_file()
         if path is not None and not is_file and type in ["SETUP", "TEARDOWN"]:
             init_path = pathlib.Path(path, "__init__.robot")
             if init_path.exists() and init_path.is_file():
                 is_file = True
                 source = str(init_path)
@@ -716,16 +720,14 @@
         type: str,
         source: Optional[str],
         line: Optional[int],
         column: Optional[int] = None,
         *,
         handler: Any = None,
     ) -> None:
-        from robot.running.userkeyword import UserKeywordHandler
-
         self.full_stack_frames.popleft()
 
         if type in ["KEYWORD"] and source is None and line is None and column is None:
             return
 
         if type in ["SUITE", "TEST"]:
             self.stack_frames.popleft()
@@ -817,16 +819,14 @@
         line_no = attributes.get("lineno", 1)
         longname = attributes.get("longname", "")
         type = "TEST"
 
         self.remove_stackframe_entry(longname, type, source, line_no)
 
     def start_keyword(self, name: str, attributes: Dict[str, Any]) -> None:
-        from robot.running.context import EXECUTION_CONTEXTS
-
         status = attributes.get("status", "")
         source = attributes.get("source", None)
         line_no = attributes.get("lineno", None)
         type = attributes.get("type", "KEYWORD")
         libname = attributes.get("libname", None)
         kwname = attributes.get("kwname", None)
 
@@ -867,16 +867,14 @@
                 if v.type == "KEYWORD" and v.longname in self.CAUGHTED_KEYWORDS
             ),
             None,
         )
         return r is None
 
     def end_keyword(self, name: str, attributes: Dict[str, Any]) -> None:
-        from robot.running.context import EXECUTION_CONTEXTS
-
         type = attributes.get("type", None)
         if self.debug:
             status = attributes.get("status", "")
 
             if status == "FAIL" and type in ["KEYWORD", "SETUP", "TEARDOWN"]:
                 self.process_end_state(
                     status,
@@ -1004,23 +1002,31 @@
 
         if level == "FAIL":
             self.last_fail_message = msg
 
         if self.output_log:
             self._send_log_event(message["timestamp"], level, msg, OutputCategory.CONSOLE)
 
+    RE_FILE_LINE_MATCHER = re.compile(r".+\sin\sfile\s'(?P<file>.*)'\son\sline\s(?P<line>\d+):.*")
+
     def _send_log_event(self, timestamp: str, level: str, msg: str, category: Union[OutputCategory, str]) -> None:
         current_frame = self.full_stack_frames[0] if self.full_stack_frames else None
         source = (
             Source(path=str(self.map_path_to_client(current_frame.source)))
             if current_frame and current_frame.is_file and current_frame.source
             else None
         )
+
         line = current_frame.line if current_frame else None
 
+        match = self.RE_FILE_LINE_MATCHER.match(msg)
+        if match:
+            source = Source(path=str(self.map_path_to_client(match.group("file"))))
+            line = int(match.group("line"))
+
         self.send_event(
             self,
             OutputEvent(
                 body=OutputEventBody(
                     output=self._build_output(level, msg, timestamp),
                     category=category,
                     source=source,
@@ -1097,16 +1103,14 @@
         self,
         variables_reference: int,
         filter: Optional[Literal["indexed", "named"]] = None,
         start: Optional[int] = None,
         count: Optional[int] = None,
         format: Optional[ValueFormat] = None,
     ) -> List[Variable]:
-        from robot.utils.normalizing import NormalizedDict
-
         result = NormalizedDict(ignore="_")
 
         entry = next(
             (
                 v
                 for v in self.stack_frames
                 if variables_reference in [v.global_id(), v.suite_id(), v.test_id(), v.local_id()]
@@ -1186,20 +1190,14 @@
     def evaluate(
         self,
         expression: str,
         frame_id: Optional[int] = None,
         context: Union[EvaluateArgumentContext, str, None] = None,
         format: Optional[ValueFormat] = None,
     ) -> EvaluateResult:
-        from robot.errors import VariableError
-        from robot.running.context import EXECUTION_CONTEXTS
-        from robot.running.model import Keyword
-        from robot.variables.evaluation import evaluate_expression
-        from robot.variables.replacer import VariableReplacer
-
         if not expression:
             return EvaluateResult(result="")
 
         stack_frame = next((v for v in self.full_stack_frames if v.id == frame_id), None)
 
         evaluate_context = stack_frame.context() if stack_frame else None
 
@@ -1261,15 +1259,15 @@
                                 self.state = old_state
                                 self.condition.notify_all()
 
                                 self._after_evaluate_keyword_event.set()
 
             elif self.IS_VARIABLE_RE.match(expression.strip()):
                 try:
-                    result = VariableReplacer(vars.store).replace_scalar(expression)
+                    result = vars.replace_scalar(expression)
                 except VariableError:
                     if context is not None and (
                         isinstance(context, EvaluateArgumentContext)
                         and (
                             context
                             in [
                                 EvaluateArgumentContext.HOVER,
@@ -1287,23 +1285,23 @@
                         raise
             else:
                 result = evaluate_expression(vars.replace_string(expression), vars.store)
 
         except (SystemExit, KeyboardInterrupt):
             raise
         except BaseException as e:
-            result = e
+            self._logger.exception(e)
+            result = traceback.format_exc()
+            # result = e
 
         return EvaluateResult(repr(result), repr(type(result)))
 
     def set_variable(
         self, variables_reference: int, name: str, value: str, format: Optional[ValueFormat] = None
     ) -> SetVariableResult:
-        from robot.variables.evaluation import evaluate_expression
-
         entry = next(
             (
                 v
                 for v in self.full_stack_frames
                 if variables_reference in [v.global_id(), v.local_id(), v.suite_id(), v.test_id()]
             ),
             None,
```

### Comparing `robotcode_debugger-0.33.0/src/robotcode/debugger/listeners.py` & `robotcode_debugger-0.34.1/src/robotcode/debugger/listeners.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import re
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional, Union, cast
 
+from robot import result, running
+from robot.model import Message
+
 from .dap_types import Event, Model
 from .debugger import Debugger
 
 
 @dataclass
 class RobotExecutionEventBody(Model):
     type: str
@@ -13,17 +17,15 @@
     attributes: Optional[Dict[str, Any]] = None
     failed_keywords: Optional[List[Dict[str, Any]]] = None
 
 
 class ListenerV2:
     ROBOT_LISTENER_API_VERSION = "2"
 
-    def __init__(self, no_debug: bool = False) -> None:
-        self.no_debug = no_debug
-        self.debug = not no_debug
+    def __init__(self) -> None:
         self.failed_keywords: Optional[List[Dict[str, Any]]] = None
         self.last_fail_message: Optional[str] = None
 
     def start_suite(self, name: str, attributes: Dict[str, Any]) -> None:
         Debugger.instance().send_event(
             self,
             Event(
@@ -117,38 +119,112 @@
 
             if attributes["status"] == "FAIL" and attributes.get("source", None):
                 if self.failed_keywords is None:
                     self.failed_keywords = []
 
                 self.failed_keywords.insert(0, {"message": self.last_fail_message, **attributes})
 
-    def log_message(self, message: Dict[str, Any]) -> None:
-        current_frame = Debugger.instance().full_stack_frames[0] if Debugger.instance().full_stack_frames else None
-
-        if message["level"] == "FAIL":
-            self.last_fail_message = message["message"]
-            Debugger.instance().last_fail_message = self.last_fail_message
+    RE_FILE_LINE_MATCHER = re.compile(r".+\sin\sfile\s'(?P<file>.*)'\son\sline\s(?P<line>\d+):(?P<message>.*)")
 
-        source = current_frame.source if current_frame else None
-        line = current_frame.line if current_frame else None
-        column = current_frame.column if current_frame else None
+    def log_message(self, message: Dict[str, Any]) -> None:
+        if message["level"] in ["FAIL", "ERROR", "WARN"]:
+            current_frame = Debugger.instance().full_stack_frames[0] if Debugger.instance().full_stack_frames else None
 
-        name = next((e.name for e in Debugger.instance().full_stack_frames if e.type in ["SUITE", "TEST"]), None)
+            if message["level"] == "FAIL":
+                self.last_fail_message = message["message"]
+                Debugger.instance().last_fail_message = self.last_fail_message
+
+            source = current_frame.source if current_frame else None
+            line = current_frame.line if current_frame else None
+            column = current_frame.column if current_frame else None
+
+            item_id = next(
+                (
+                    (
+                        f"{Path(item.source).resolve() if item.source is not None else ''};{item.longname}"
+                        if item.type == "SUITE"
+                        else f"{Path(item.source).resolve() if item.source is not None else ''};"
+                        f"{item.longname};{item.line}"
+                    )
+                    for item in Debugger.instance().full_stack_frames
+                    if item.type in ["SUITE", "TEST"]
+                ),
+                None,
+            )
 
-        Debugger.instance().send_event(
-            self,
-            Event(
-                event="robotLog",
-                body={"itemId": name, "source": source, "lineno": line, "column": column, **dict(message)},
-            ),
-        )
+            msg = None
+            match = self.RE_FILE_LINE_MATCHER.match(message["message"])
+            if match:
+                source = match.group("file")
+                line = int(match.group("line"))
+                msg = match.group("message")
+                column = 0
+
+            Debugger.instance().send_event(
+                self,
+                Event(
+                    event="robotLog",
+                    body={
+                        "itemId": item_id,
+                        "source": source,
+                        "lineno": line,
+                        "column": column,
+                        **dict(message),
+                        **({"message": msg} if msg else {}),
+                    },
+                ),
+            )
 
         Debugger.instance().log_message(message)
 
     def message(self, message: Dict[str, Any]) -> None:
+        if message["level"] in ["FAIL", "ERROR", "WARN"]:
+            current_frame = Debugger.instance().full_stack_frames[0] if Debugger.instance().full_stack_frames else None
+
+            source = current_frame.source if current_frame else None
+            line = current_frame.line if current_frame else None
+            column = current_frame.column if current_frame else None
+
+            item_id = next(
+                (
+                    (
+                        f"{Path(item.source).resolve() if item.source is not None else ''};{item.longname}"
+                        if item.type == "SUITE"
+                        else f"{Path(item.source).resolve() if item.source is not None else ''};"
+                        f"{item.longname};{item.line}"
+                    )
+                    for item in Debugger.instance().full_stack_frames
+                    if item.type in ["SUITE", "TEST"]
+                ),
+                None,
+            )
+
+            msg = None
+            match = self.RE_FILE_LINE_MATCHER.match(message["message"])
+            if match:
+                source = match.group("file")
+                line = int(match.group("line"))
+                msg = match.group("message")
+                column = 0
+
+            Debugger.instance().send_event(
+                self,
+                Event(
+                    event="robotMessage",
+                    body={
+                        "itemId": item_id,
+                        "source": source,
+                        "lineno": line,
+                        "column": column,
+                        **dict(message),
+                        **({"message": msg} if msg else {}),
+                    },
+                ),
+            )
+
         Debugger.instance().message(message)
 
     def library_import(self, name: str, attributes: Dict[str, Any]) -> None:
         pass
 
     def resource_import(self, name: str, attributes: Dict[str, Any]) -> None:
         pass
@@ -177,45 +253,51 @@
 
 class ListenerV3:
     ROBOT_LISTENER_API_VERSION = "3"
 
     def __init__(self) -> None:
         self._event_sended = False
 
-    def start_suite(self, data: Any, result: Any) -> None:
-        from robot.running import TestCase, TestSuite
+    def start_suite(self, data: running.TestSuite, result: result.TestSuite) -> None:
+        """Called when a suite starts."""
+
+        def enqueue(item: Union[running.TestSuite, running.TestCase]) -> Iterator[str]:
+            if isinstance(item, running.TestSuite):
+                yield f"{Path(item.source).resolve() if item.source is not None else ''};{item.longname}"
 
-        def enqueue(item: Union[TestSuite, TestCase]) -> Iterator[str]:
-            if isinstance(item, TestSuite):
                 for s in item.suites:
                     yield from enqueue(s)
                 for s in item.tests:
                     yield from enqueue(s)
-
-                yield f"{Path(item.source).resolve() if item.source is not None else ''};{item.longname}"
                 return
 
             yield f"{Path(item.source).resolve() if item.source is not None else ''};{item.longname};{item.lineno}"
 
         if self._event_sended:
             return
 
-        items = list(reversed(list(enqueue(cast(TestSuite, data)))))
+        items = list(reversed(list(enqueue(cast(running.TestSuite, data)))))
 
         Debugger.instance().send_event(
             self,
             Event(
                 event="robotEnqueued",
                 body={"items": items},
             ),
         )
 
         self._event_sended = True
 
-    def end_suite(self, data: Any, result: Any) -> None:
+    def end_suite(self, data: running.TestSuite, result: result.TestSuite) -> None:
+        pass
+
+    def start_test(self, data: running.TestCase, result: result.TestCase) -> None:
+        pass
+
+    def end_test(self, data: running.TestCase, result: result.TestCase) -> None:
         pass
 
-    def start_test(self, data: Any, result: Any) -> None:
+    def log_message(self, message: Message) -> None:
         pass
 
-    def end_test(self, data: Any, result: Any) -> None:
+    def message(self, message: Message) -> None:
         pass
```

### Comparing `robotcode_debugger-0.33.0/src/robotcode/debugger/protocol.py` & `robotcode_debugger-0.34.1/src/robotcode/debugger/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.33.0/src/robotcode/debugger/server.py` & `robotcode_debugger-0.34.1/src/robotcode/debugger/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import asyncio
 import os
 from typing import Any, Callable, Dict, List, Literal, Optional, Union
 
 from robotcode.core import async_tools
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.core.types import ServerMode, TcpParams
 from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.jsonrpc2.server import JsonRPCServer, JsonRpcServerMode, TcpParams
+from robotcode.jsonrpc2.server import JsonRPCServer
 
 from .dap_types import (
     AttachRequestArguments,
     Capabilities,
     ConfigurationDoneArguments,
     ContinueArguments,
     ContinueResponseBody,
@@ -115,21 +116,21 @@
     @_logger.call
     async def wait_for_client(self, timeout: float = 5) -> bool:
         await asyncio.wait_for(self._connected_event.wait(), timeout)
 
         return self._connected
 
     @_logger.call
-    async def wait_for_initialized(self, timeout: float = 60) -> bool:
+    async def wait_for_initialized(self, timeout: float = 30) -> bool:
         await asyncio.wait_for(self._initialized_event.wait(), timeout)
 
         return self._initialized
 
     @_logger.call
-    async def wait_for_disconnected(self, timeout: float = 60) -> bool:
+    async def wait_for_disconnected(self, timeout: float = 30) -> bool:
         await asyncio.wait_for(self._disconnected_event.wait(), timeout)
 
         return self._connected
 
     @rpc_method(name="initialize", param_type=InitializeRequestArguments)
     async def _initialize(self, arguments: InitializeRequestArguments, *args: Any, **kwargs: Any) -> Capabilities:
         self._initialized = True
@@ -375,17 +376,20 @@
         )
         return SetExceptionBreakpointsResponseBody(breakpoints=result) if result else None
 
 
 class DebugAdapterServer(JsonRPCServer[DebugAdapterServerProtocol]):
     def __init__(
         self,
+        mode: ServerMode = ServerMode.TCP,
         tcp_params: TcpParams = TcpParams(None, TCP_DEFAULT_PORT),
+        pipe_name: Optional[str] = None,
     ):
         super().__init__(
-            mode=JsonRpcServerMode.TCP,
+            mode=mode,
             tcp_params=tcp_params,
+            pipe_name=pipe_name,
         )
         self.protocol = DebugAdapterServerProtocol()
 
     def create_protocol(self) -> DebugAdapterServerProtocol:
         return self.protocol
```

### Comparing `robotcode_debugger-0.33.0/src/robotcode/debugger/launcher/server.py` & `robotcode_debugger-0.34.1/src/robotcode/debugger/launcher/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from __future__ import annotations
 
 import asyncio
+import itertools
 import os
+import sys
 from pathlib import Path
 from typing import Any, Dict, List, Literal, Optional
 
 from robotcode.core.logging import LoggingDescriptor
-from robotcode.core.utils.version import Version, create_version_from_str
-from robotcode.debugger.client import DAPClient, DAPClientError
-from robotcode.debugger.dap_types import (
+from robotcode.core.types import ServerMode, TcpParams
+from robotcode.jsonrpc2.protocol import rpc_method
+from robotcode.jsonrpc2.server import JsonRPCServer
+from robotcode.robot.utils import get_robot_version
+
+from ..cli import DEBUGGER_DEFAULT_PORT, DEBUGPY_DEFAULT_PORT
+from ..dap_types import (
     AttachRequest,
     AttachRequestArguments,
     Capabilities,
     ConfigurationDoneArguments,
     ConfigurationDoneRequest,
     DisconnectArguments,
     DisconnectRequest,
@@ -29,28 +35,16 @@
     RunInTerminalRequest,
     RunInTerminalRequestArguments,
     RunInTerminalResponseBody,
     TerminateArguments,
     TerminatedEvent,
     TerminateRequest,
 )
-from robotcode.debugger.protocol import DebugAdapterProtocol
-from robotcode.jsonrpc2.protocol import rpc_method
-from robotcode.jsonrpc2.server import JsonRPCServer, JsonRpcServerMode, TcpParams
-
-_robot_version: Optional[Version] = None
-
-
-def get_robot_version() -> Version:
-    global _robot_version
-    if _robot_version is None:
-        import robot.version
-
-        _robot_version = create_version_from_str(robot.version.get_version())
-    return _robot_version
+from ..protocol import DebugAdapterProtocol
+from .client import DAPClient, DAPClientError
 
 
 class OutputProtocol(asyncio.SubprocessProtocol):
     def __init__(self, parent: LauncherDebugAdapterProtocol) -> None:
         super().__init__()
         self.parent = parent
 
@@ -141,83 +135,94 @@
 
     @rpc_method(name="launch", param_type=LaunchRequestArguments)
     async def _launch(
         self,
         request: str,
         python: str,
         cwd: str = ".",
+        profiles: Optional[List[str]] = None,
         target: Optional[str] = None,
         paths: Optional[List[str]] = None,
         args: Optional[List[str]] = None,
         env: Optional[Dict[str, Optional[Any]]] = None,
         console: Optional[Literal["internalConsole", "integratedTerminal", "externalTerminal"]] = "integratedTerminal",
         name: Optional[str] = None,
         no_debug: Optional[bool] = None,
         robotPythonPath: Optional[List[str]] = None,  # noqa: N803
         launcherArgs: Optional[List[str]] = None,  # noqa: N803
         launcherTimeout: Optional[int] = None,  # noqa: N803
         debuggerArgs: Optional[List[str]] = None,  # noqa: N803
         debuggerTimeout: Optional[int] = None,  # noqa: N803
         attachPython: Optional[bool] = False,  # noqa: N803
+        attachPythonPort: Optional[int] = None,  # noqa: N803
         variables: Optional[Dict[str, Any]] = None,
         outputDir: Optional[str] = None,  # noqa: N803
         outputMessages: Optional[bool] = False,  # noqa: N803
         outputLog: Optional[bool] = False,  # noqa: N803
         outputTimestamps: Optional[bool] = False,  # noqa: N803
         groupOutput: Optional[bool] = False,  # noqa: N803
         stopOnEntry: Optional[bool] = False,  # noqa: N803
         dryRun: Optional[bool] = None,  # noqa: N803
         mode: Optional[str] = None,
         variableFiles: Optional[List[str]] = None,  # noqa: N803
         languages: Optional[List[str]] = None,
         arguments: Optional[LaunchRequestArguments] = None,
         include: Optional[List[str]] = None,
         exclude: Optional[List[str]] = None,
+        robotCodeArgs: Optional[List[str]] = None,  # noqa: N803
         *_args: Any,
         **_kwargs: Any,
     ) -> None:
         from robotcode.core.utils.net import find_free_port
 
         connect_timeout = launcherTimeout or 10
 
-        port = find_free_port()
+        port = find_free_port(DEBUGGER_DEFAULT_PORT)
 
         debugger_script = (
             Path(Path(__file__).parent.parent) if self.debugger_script is None else Path(self.debugger_script)
         )
 
-        run_args = [python, "-u", str(debugger_script)]
+        run_args = [
+            python,
+            str(debugger_script),
+            *itertools.chain.from_iterable(["--profile", p] for p in profiles or []),
+            *(robotCodeArgs or []),
+            "debug",
+        ]
 
-        run_args += ["-p", str(port)]
+        if no_debug:
+            run_args += ["--no-debug"]
 
-        run_args += ["-w"]
+        if port != DEBUGGER_DEFAULT_PORT:
+            run_args += ["--tcp", str(port)]
 
         if debuggerTimeout is not None:
-            run_args += ["-t", str(debuggerTimeout)]
-
-        if no_debug:
-            run_args += ["-n"]
+            run_args += ["wait-for-client-timeout", str(debuggerTimeout)]
 
         if attachPython and not no_debug:
-            run_args += ["-d", "-dp", str(find_free_port()), "-dw"]
+            run_args += ["--debugpy"]
+
+            if attachPythonPort is not None and attachPythonPort != DEBUGPY_DEFAULT_PORT:
+                run_args += ["--debugpy-port", str(attachPythonPort or 0)]
 
         if outputMessages:
-            run_args += ["-om"]
+            run_args += ["--output-messages"]
 
-        if outputLog:
-            run_args += ["-ol"]
+        if not outputLog:
+            run_args += ["--no-output-log"]
 
         if outputTimestamps:
-            run_args += ["-ot"]
+            run_args += ["--output-timestamps"]
 
         if groupOutput:
-            run_args += ["-og"]
+            run_args += ["--group-output"]
 
         if stopOnEntry:
-            run_args += ["-soe"]
+            run_args += ["--stop-on-entry"]
 
         run_args += debuggerArgs or []
 
         run_args += ["--"]
 
         if get_robot_version() >= (6, 0) and languages:
             for lang in languages:
@@ -297,22 +302,35 @@
                 env=run_env,
             )
 
         else:
             raise ValueError(f'Unknown console type "{console}".')
 
         self.client = DAPClient(self, TcpParams(None, port))
+        self.client.on_closed.add(self._client_on_closed)
         try:
             await self.client.connect(connect_timeout)
-        except asyncio.TimeoutError:
-            raise asyncio.TimeoutError("Can't connect to debugger.")
+        except asyncio.TimeoutError as e:
+            self._logger.exception(e)
+
+            if self.loop is not None:
+                self.loop.call_later(0, sys.exit, 255)
+            else:
+                sys.exit(255)
+
+            raise asyncio.TimeoutError("Can't connect to debugger.") from e
 
         if self._initialize_arguments is not None:
             await self.client.protocol.send_request_async(InitializeRequest(arguments=self._initialize_arguments))
 
+    def _client_on_closed(self, sender: Any) -> None:
+        self._logger.info("Client closed.")
+        if self.loop is not None:
+            self.loop.call_later(1, self.loop.stop)
+
     @rpc_method(name="configurationDone", param_type=ConfigurationDoneArguments)
     async def _configuration_done(
         self,
         arguments: Optional[ConfigurationDoneArguments] = None,
         *args: Any,
         **kwargs: Any,
     ) -> None:
@@ -333,34 +351,37 @@
     async def _terminate(self, arguments: Optional[TerminateArguments] = None, *args: Any, **kwargs: Any) -> None:
         if self.client.connected:
             await self.client.protocol.send_request_async(TerminateRequest(arguments=arguments))
         else:
             self.send_event(Event("terminateRequested"))
             await self.send_event_async(TerminatedEvent())
 
+    @_logger.call
     async def handle_unknown_command(self, message: Request) -> Any:
         if self.connected:
-            self._logger.debug("Forward request to client...")
+            self._logger.debug(lambda: f"Unknown request, forward to client: {message}")
 
             return await self.client.protocol.send_request_async(message)
 
         return await super().handle_unknown_command(message)
 
 
-TCP_DEFAULT_PORT = 6611
-
-
 class LauncherServer(JsonRPCServer[LauncherDebugAdapterProtocol]):
     def __init__(
         self,
-        mode: JsonRpcServerMode = JsonRpcServerMode.STDIO,
-        tcp_params: TcpParams = TcpParams(None, TCP_DEFAULT_PORT),
+        mode: ServerMode = ServerMode.STDIO,
+        tcp_params: TcpParams = TcpParams(None, 0),
+        pipe_name: Optional[str] = None,
         debugger_script: Optional[str] = None,
     ):
         super().__init__(
             mode=mode,
             tcp_params=tcp_params,
+            pipe_name=pipe_name,
         )
         self.debugger_script = debugger_script
+        self.protocol: Optional[LauncherDebugAdapterProtocol] = None
 
     def create_protocol(self) -> LauncherDebugAdapterProtocol:
-        return LauncherDebugAdapterProtocol(debugger_script=self.debugger_script)
+        self.protocol = LauncherDebugAdapterProtocol(debugger_script=self.debugger_script)
+
+        return self.protocol
```

### Comparing `robotcode_debugger-0.33.0/.gitignore` & `robotcode_debugger-0.34.1/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.33.0/LICENSE.txt` & `robotcode_debugger-0.34.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.33.0/README.md` & `robotcode_debugger-0.34.1/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.33.0/pyproject.toml` & `robotcode_debugger-0.34.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -21,20 +21,27 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Operating System :: OS Independent",
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
-dependencies = ["robotcode-jsonrpc2", "robotframework>=4.1.0"]
 dynamic = ["version"]
+dependencies = [
+  "robotframework>=4.1.0",
+  "robotcode-jsonrpc2==0.34.1",
+  "robotcode-runner==0.34.1",
+]
 
 [project.optional-dependencies]
 debugpy = ["debugpy"]
 
+[project.entry-points.robotcode]
+debugger = "robotcode.debugger.hooks"
+
 [project.scripts]
 'robotcode.debugger' = 'robotcode.debugger.__main__:main'
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
```

### Comparing `robotcode_debugger-0.33.0/PKG-INFO` & `robotcode_debugger-0.34.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-debugger
-Version: 0.33.0
+Version: 0.34.1
 Summary: RobotCode Debugger for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2
+Requires-Dist: robotcode-jsonrpc2==0.34.1
+Requires-Dist: robotcode-runner==0.34.1
 Requires-Dist: robotframework>=4.1.0
 Provides-Extra: debugpy
 Requires-Dist: debugpy; extra == 'debugpy'
 Description-Content-Type: text/markdown
 
 # robotcode-debugger
```

