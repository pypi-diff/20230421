# Comparing `tmp/pystream-pipeline-0.1.2.tar.gz` & `tmp/pystream_pipeline-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystream-pipeline-0.1.2.tar", max compression
+gzip compressed data, was "pystream_pipeline-0.1.3.tar", max compression
```

## Comparing `pystream-pipeline-0.1.2.tar` & `pystream_pipeline-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,24 @@
--rw-r--r--   0        0        0     1090 2022-06-26 02:39:18.716178 pystream-pipeline-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     1222 2022-10-30 14:47:55.626384 pystream-pipeline-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      147 2022-10-30 14:48:00.613616 pystream-pipeline-0.1.2/pystream/__init__.py
--rw-r--r--   0        0        0        0 2022-06-22 14:34:03.315670 pystream-pipeline-0.1.2/pystream/data/__init__.py
--rw-r--r--   0        0        0      138 2022-06-22 14:34:03.315670 pystream-pipeline-0.1.2/pystream/data/pipeline_data.py
--rw-r--r--   0        0        0       45 2022-06-28 16:02:07.781479 pystream-pipeline-0.1.2/pystream/functional/__init__.py
--rw-r--r--   0        0        0     3975 2022-08-05 11:56:16.627737 pystream-pipeline-0.1.2/pystream/functional/functions.py
--rw-r--r--   0        0        0        0 2022-06-22 14:34:03.316670 pystream-pipeline-0.1.2/pystream/pipeline/__init__.py
--rw-r--r--   0        0        0     7821 2022-10-30 14:46:44.222860 pystream-pipeline-0.1.2/pystream/pipeline/parallel_pipeline.py
--rw-r--r--   0        0        0     6450 2022-10-30 14:46:44.223863 pystream-pipeline-0.1.2/pystream/pipeline/pipeline.py
--rw-r--r--   0        0        0     1128 2022-10-30 14:46:44.223863 pystream-pipeline-0.1.2/pystream/pipeline/pipeline_base.py
--rw-r--r--   0        0        0      844 2022-08-04 12:26:39.813041 pystream-pipeline-0.1.2/pystream/pipeline/serial_pipeline.py
--rw-r--r--   0        0        0        0 2022-06-22 14:34:03.320670 pystream-pipeline-0.1.2/pystream/stage/__init__.py
--rw-r--r--   0        0        0      762 2022-06-24 14:13:30.394189 pystream-pipeline-0.1.2/pystream/stage/stage.py
--rw-r--r--   0        0        0     2712 2022-06-29 12:15:58.800826 pystream-pipeline-0.1.2/README.md
--rw-r--r--   0        0        0     3451 2022-10-30 14:54:07.121128 pystream-pipeline-0.1.2/setup.py
--rw-r--r--   0        0        0     3768 2022-10-30 14:54:07.121128 pystream-pipeline-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2022-06-26 02:39:18.716178 pystream_pipeline-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     1335 2023-04-21 07:33:12.702888 pystream_pipeline-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      208 2023-04-21 07:33:12.704389 pystream_pipeline-0.1.3/pystream/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-22 14:34:03.315670 pystream_pipeline-0.1.3/pystream/data/__init__.py
+-rw-r--r--   0        0        0      633 2023-01-21 12:44:41.244926 pystream_pipeline-0.1.3/pystream/data/pipeline_data.py
+-rw-r--r--   0        0        0       77 2022-12-01 14:43:42.910747 pystream_pipeline-0.1.3/pystream/functional/__init__.py
+-rw-r--r--   0        0        0     3178 2022-12-01 14:43:42.911747 pystream_pipeline-0.1.3/pystream/functional/functions.py
+-rw-r--r--   0        0        0        0 2022-06-22 14:34:03.316670 pystream_pipeline-0.1.3/pystream/pipeline/__init__.py
+-rw-r--r--   0        0        0     1660 2023-03-30 13:45:11.925848 pystream_pipeline-0.1.3/pystream/pipeline/automation.py
+-rw-r--r--   0        0        0     8703 2023-03-31 08:29:09.234875 pystream_pipeline-0.1.3/pystream/pipeline/parallel_pipeline.py
+-rw-r--r--   0        0        0     7645 2023-04-21 07:26:53.809651 pystream_pipeline-0.1.3/pystream/pipeline/pipeline.py
+-rw-r--r--   0        0        0      753 2022-12-15 15:22:39.581811 pystream_pipeline-0.1.3/pystream/pipeline/pipeline_base.py
+-rw-r--r--   0        0        0     1771 2023-02-09 03:44:30.082271 pystream_pipeline-0.1.3/pystream/pipeline/serial_pipeline.py
+-rw-r--r--   0        0        0        0 2022-06-22 14:34:03.320670 pystream_pipeline-0.1.3/pystream/stage/__init__.py
+-rw-r--r--   0        0        0     1901 2023-03-31 08:39:51.605872 pystream_pipeline-0.1.3/pystream/stage/container.py
+-rw-r--r--   0        0        0      921 2023-02-08 09:22:39.151513 pystream_pipeline-0.1.3/pystream/stage/final_stage.py
+-rw-r--r--   0        0        0     1019 2023-03-30 08:08:48.513849 pystream_pipeline-0.1.3/pystream/stage/stage.py
+-rw-r--r--   0        0        0      150 2023-01-21 07:50:28.323633 pystream_pipeline-0.1.3/pystream/utils/errors.py
+-rw-r--r--   0        0        0      185 2023-02-10 02:02:52.625958 pystream_pipeline-0.1.3/pystream/utils/general.py
+-rw-r--r--   0        0        0      539 2023-03-30 13:46:48.402280 pystream_pipeline-0.1.3/pystream/utils/logger.py
+-rw-r--r--   0        0        0     5672 2023-01-21 07:50:28.323633 pystream_pipeline-0.1.3/pystream/utils/profiler.py
+-rw-r--r--   0        0        0     2968 2023-04-21 07:26:53.809651 pystream_pipeline-0.1.3/README.md
+-rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 pystream_pipeline-0.1.3/setup.py
+-rw-r--r--   0        0        0     4190 1970-01-01 00:00:00.000000 pystream_pipeline-0.1.3/PKG-INFO
```

### Comparing `pystream-pipeline-0.1.2/LICENSE.md` & `pystream_pipeline-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pystream-pipeline-0.1.2/pyproject.toml` & `pystream_pipeline-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pystream-pipeline"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python package to create and manage fast parallelized data processing pipeline for real-time application"
 authors = ["Mukhlas Adib <adib.rasyidy@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/MukhlasAdib/pystream-pipeline"
 repository = "https://github.com/MukhlasAdib/pystream-pipeline"
 documentation = "https://pystream-pipeline.readthedocs.io/"
@@ -21,20 +21,25 @@
 ]
 include = [
     "LICENSE.md",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
+pandas = "^1.5.2"
+loguru = "^0.6.0"
+tabulate = "^0.9.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.2.0"
 black = "^22.3.0"
 docutils = "^0.17.1"
 numpy = "^1.22.0"
 opencv-python = "^4.5.5"
 Sphinx = "^5.0.2"
 sphinx-rtd-theme = "^1.0.0"
+ipykernel = "^6.19.4"
+pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pystream-pipeline-0.1.2/pystream/functional/functions.py` & `pystream_pipeline-0.1.3/pystream/functional/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
+from concurrent.futures import ThreadPoolExecutor
 from typing import Any, Callable, List
 
 
 _default_executor = ThreadPoolExecutor(max_workers=10)
 
 
 def func_parallel_thread(
@@ -47,38 +47,14 @@
         res = executor.map(lambda func: func(x), funcs)
         [r for r in res]
         return x
 
     return wrapper
 
 
-def func_parallel_process(
-    funcs: List[Callable[[], Any]], max_workers: int = 5
-) -> Callable[[], Any]:
-    """CURRENTLY UNSTABLE.
-    Create a function made of functions that are executed in parallel
-    using ProcessPoolExecutor from concurrent module.
-
-    Args:
-        funcs (List[Callable[[], Any]]): the list of functions
-            to be executed. It is assumed that all of the arguments
-            and output variables are already contained in each function.
-
-    Returns:
-        Callable[[], Any]: The returned function to execute the serial
-        functions.
-    """
-
-    def wrapper():
-        with ProcessPoolExecutor(max_workers=max_workers) as executor:
-            executor.map(lambda func: func(), funcs)
-
-    return wrapper
-
-
 def func_serial(funcs: List[Callable[[Any], Any]]) -> Callable[[Any], Any]:
     """Create a function made of functions that are executed in serial
 
     Args:
         funcs (List[Callable[[Any], Any]]): the list of functions to be executed. It
             only takes one argument which supposed to be anything and returns the
             processing results. The output of function i will be used as the input
```

### Comparing `pystream-pipeline-0.1.2/pystream/pipeline/parallel_pipeline.py` & `pystream_pipeline-0.1.3/pystream/pipeline/parallel_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from dataclasses import dataclass
 from queue import Empty, Full, Queue
 from threading import Event, get_ident, Thread
 import time
-from typing import List
+from typing import List, Optional
 
 from pystream.data.pipeline_data import PipelineData
 from pystream.pipeline.pipeline_base import PipelineBase
+from pystream.stage.container import StageContainer
+from pystream.stage.final_stage import FinalStage
 from pystream.stage.stage import Stage, StageCallable
-
-
-class PipelineTerminated(Exception):
-    pass
+from pystream.utils.errors import PipelineTerminated
+from pystream.utils.logger import LOGGER
+from pystream.utils.profiler import ProfilerHandler
 
 
 def send_output(
     data: PipelineData,
     output_queue: Queue,
     block: bool = True,
     replace: bool = False,
@@ -89,14 +90,15 @@
         super().__init__(name=name, daemon=True)
         self.stage = stage
         self.links = links
         self.all_out = all_out
         self.output_enabled = True
         self.daemon = True
         self.replace_output = replace_output
+        self.send_output_timeout = 10
 
     def run(self) -> None:
         self.start_thread()
         self.run_loop()
 
     def start_thread(self):
         self.print_log("Thread started...")
@@ -105,85 +107,97 @@
 
     def run_loop(self):
         while not self.links.stopper.is_set():
             try:
                 data: PipelineData = self.links.input_queue.get(timeout=1)
             except Empty:
                 continue
-            data.data = self.stage(data.data)
+            data = self.stage(data)
             if self.output_enabled:
                 send_output(
                     data,
                     self.links.output_queue,
                     block=self.all_out,
                     replace=self.replace_output,
+                    timeout=self.send_output_timeout,
                 )
         self.process_cleanup()
 
     def process_cleanup(self):
         self.print_log(f"Terminating thread...")
         self.links.stopper.set()
         if isinstance(self.stage, Stage):
             self.stage.cleanup()
         while not self.links.input_queue.empty():
             self.links.input_queue.get()
         time.sleep(1)
         self.print_log(f"Thread terminated...")
 
     def print_log(self, msg: str) -> None:
-        print(f"FROM {self.name} ({get_ident()}): {msg}")
+        LOGGER.debug(f"({self.name} {get_ident()}) {msg}")
 
 
 class StagedThreadPipeline(PipelineBase):
     def __init__(
         self,
         stages: List[StageCallable],
+        names: List[Optional[str]],
         block_input: bool = True,
         input_timeout: float = 10,
+        profiler_handler: Optional[ProfilerHandler] = None,
     ) -> None:
         """The class that will handle the parallel pipeline
         based on multi-threading.
 
         Args:
             stages (List[StageCallable]): The stages to be run
                 in sequence.
+            names (List[Optional[str]]): Stage names. If the name is None,
+                default stage name will be given.
             block_input (bool, optional): Whether to set the forward method
                 into blocking mode with the specified timeout in input_timeout.
                 Defaults to True.
             input_timeout (float, optional): Blocking timeout for the forward
                 method in seconds. Defaults to 10.
+            profiler_handler (Optional[ProfilerHandler]): Handler for the profiler.
+                If None, no profiling attempt will be done.
         """
-        self.stages = stages
+        self.final_stage = FinalStage(profiler_handler)
+        self.stages: List[Stage] = [
+            StageContainer(stage, name) for stage, name in zip(stages, names)
+        ]
+        self.stages.append(self.final_stage)
         self.block_input = block_input
         self.input_timeout = input_timeout
 
         self.build_pipeline()
         self.run_pipeline()
         self.results = PipelineData()
 
     def build_pipeline(self):
         """Build the pipeline."""
         # Create the first link
         self.stopper = Event()
         self.starter = Event()
         # The first stage's input is the output
         # of the pipeline handler
-        self.main_output_queue = input_queue = Queue(maxsize=1)
+        input_queue = Queue(maxsize=1)
+        self.main_output_queue = input_queue
         self.stage_threads: List[StageThread] = []
         self.stage_links: List[StageLinks] = []
         # Create the stage threars one by one along with the links
         for _, stage in enumerate(self.stages):
             output_queue = Queue(maxsize=1)
             links = StageLinks(
                 input_queue=input_queue,
                 output_queue=output_queue,
                 stopper=self.stopper,
                 starter=self.starter,
             )
-            self.stage_threads.append(StageThread(stage, links, f"PyStream-Stage"))
+            self.stage_threads.append(StageThread(stage, links, stage.name))
             self.stage_links.append(links)
             input_queue = output_queue
         # Replace output of the last stage to avoid blocking
         self.stage_threads[-1].all_out = False
         self.stage_threads[-1].replace_output = True
         # The last stage's output is the input of the pipeline handler
         self.main_input_queue = input_queue
```

### Comparing `pystream-pipeline-0.1.2/pystream/pipeline/pipeline.py` & `pystream_pipeline-0.1.3/pystream/pipeline/pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,114 @@
 from __future__ import annotations
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
-from threading import Event, Thread
-import time
-from typing import Any, Callable, List, Optional
-
-from pystream.data.pipeline_data import PipelineData
+from pystream.data.pipeline_data import (
+    InputGeneratorRequest,
+    PipelineData,
+    _request_generator,
+)
+from pystream.pipeline.automation import PipelineAutomation
 from pystream.pipeline.pipeline_base import PipelineBase
 from pystream.stage.stage import StageCallable
-from .serial_pipeline import SerialPipeline
-from .parallel_pipeline import StagedThreadPipeline
-
-
-class PipelineUndefined(Exception):
-    pass
+from pystream.pipeline.serial_pipeline import SerialPipeline
+from pystream.pipeline.parallel_pipeline import StagedThreadPipeline
+from pystream.utils.errors import PipelineUndefined
+from pystream.utils.general import _PIPELINE_NAME_IN_PROFILE
+from pystream.utils.logger import LOGGER
+from pystream.utils.profiler import ProfilerHandler
 
 
 class Pipeline:
     """The pipeline constructor
 
     Args:
         input_generator (Optional[Callable[[], Any]], optional): Function that will be
             used to generate input data if you want the pipeline to run autonomously.
             If None, the input needs to be given by invoking "forward" method.
             Defaults to None.
+        use_profiler (bool, optional): Whether to implement profiler to the pipeline.
+            Defaults to False.
     """
 
-    def __init__(self, input_generator: Optional[Callable[[], Any]] = None) -> None:
+    def __init__(
+        self,
+        input_generator: Optional[Callable[[], Any]] = None,
+        use_profiler: bool = False,
+    ) -> None:
         self.stages_sequence: List[StageCallable] = []
+        self.stage_names: List[Optional[str]] = []
         self.pipeline: Optional[PipelineBase] = None
-        self.__input_generator: Callable[[], Any] = lambda: None
+
+        self._input_generator: Callable[[], Any] = lambda: None
         if input_generator is not None:
-            self.__input_generator = input_generator
+            self._input_generator = input_generator
 
-        self.__loop_period = 0.01
-        self.__loop_is_start = Event()
-        self.__loop_thread = Thread(
-            target=self.__loop_handler, name="PyStream-InputGen", daemon=True
-        )
+        self.profiler = ProfilerHandler() if use_profiler else None
+        self._automation = None
 
-    def add(self, stage: StageCallable) -> None:
+    def add(self, stage: StageCallable, name: Optional[str] = None) -> None:
         """Add a stage into the pipeline
 
         The stage is in type of StageCallable, which is Union[Callable[[T], T], Stage].
         Thus, a stage can be defined in two ways:
 
         (1) A stage can be a function that takes
         an input data (of any type)  and then returns an output data of the same type.
 
         (2) A stage can be a class that inherits from pystream.Stage class, which is an
         abstract class. Methods `__call__` and `cleanup` need to be defined there. Use this
         if the stage need a special cleanup procedure.
 
         Args:
             stage (StageCallable): the stage to be added
+            name (Optional[str]): the stage name. If None default stage name will be given,
+                i.e. Stage_i where i is the stage sequence number. Defaults to None.
         """
         self.stages_sequence.append(stage)
+        self.stage_names.append(name)
 
     def serialize(self) -> Pipeline:
         """Turn the pipeline into serial pipeline. All stages will
         be run in sequential and blocking mode.
 
         Returns:
             Pipeline: this pipeline itself
         """
-        self.pipeline = SerialPipeline(self.stages_sequence)
+        self.pipeline = SerialPipeline(
+            self.stages_sequence, self.stage_names, profiler_handler=self.profiler
+        )
         return self
 
     def parallelize(
         self, block_input: bool = True, input_timeout: float = 10
     ) -> Pipeline:
         """Turn the pipeline into independent stage pipeline. Each stage
         will live in different thread and work asynchronously. However,
         the data will be passed to the stages in the same order as defined
 
         Args:
             block_input (bool, optional): Whether to set the forward method
-                into blocking mode with the specified timeout in input_timeout.
-                Defaults to True.
+                into blocking mode if the first stage is busy with the specified
+                timeout in input_timeout. Defaults to True.
             input_timeout (float, optional): Blocking timeout for the forward
                 method in seconds. Defaults to 10.
 
         Returns:
             Pipeline: this pipeline itself
         """
         self.pipeline = StagedThreadPipeline(
-            self.stages_sequence, block_input=block_input, input_timeout=input_timeout
+            self.stages_sequence,
+            self.stage_names,
+            block_input=block_input,
+            input_timeout=input_timeout,
+            profiler_handler=self.profiler,
         )
         return self
 
-    def forward(self, data: Any) -> bool:
+    def forward(self, data: Any = _request_generator) -> bool:
         """Forward data into the pipeline
 
         Args:
             data (Any): the data. If data none, data generated
                 from the input generator will be pushed instead.
 
         Raises:
@@ -101,34 +117,34 @@
 
         Returns:
             bool: True if the data has been forwarded successfully,
             False otherwise.
         """
         if self.pipeline is None:
             raise PipelineUndefined("Pipeline has not been defined")
-        pipeline_data = self.__generate_pipeline_data(data)
-        return self.pipeline.forward(pipeline_data)
+        pipeline_data = self._generate_pipeline_data(data)
+        return self._push_pipeline_data(pipeline_data)
 
     def start_loop(self, period: float = 0.01) -> None:
         """Start the pipeline in autonomous mode. Data generated
         from input generator will be pushed into the pipeline at each
         defined period of time.
 
         Args:
             period (float, optional): Period to push the data.
                 Defaults to 0.01.
         """
-        self.__loop_period = period
-        self.__loop_is_start.set()
-        self.__loop_thread.start()
+        self._automation = PipelineAutomation(pipeline=self, period=period)
+        self._automation.start()
 
     def stop_loop(self) -> None:
         """Stop the autonomous operation of the pipeline"""
-        self.__loop_is_start.clear()
-        self.__loop_thread.join()
+        if self._automation is None:
+            return
+        self._automation.stop()
 
     def get_results(self) -> Any:
         """Get latest results from the pipeline
 
         Raises:
             PipelineUndefined: raised if method `serialize` and
                 `parallelize` has not been invoked.
@@ -141,31 +157,37 @@
         if self.pipeline is None:
             raise PipelineUndefined("Pipeline has not been defined")
         return self.pipeline.get_results().data
 
     def cleanup(self) -> None:
         """Stop and cleanup the pipeline. Do nothing if the pipeline has not
         been initialized"""
-        if self.pipeline is None:
-            return
-        self.pipeline.cleanup()
-        self.pipeline = None
+        if self.pipeline is not None:
+            self.pipeline.cleanup()
+            self.pipeline = None
+
+    def get_profiles(self) -> Tuple[Dict[str, float], Dict[str, float]]:
+        """Get profiles data
+
+        Returns:
+            Tuple[Dict[str, float], Dict[str, float]]: dictionary of the latency and
+            throughput data respectively. The data is a dict where the key is the
+            stage name
+        """
+        if self.profiler is None:
+            LOGGER.error("Cannot get profiles because profiler is not activated")
+            return {}, {}
+        return self.profiler.summarize()
 
-    def __generate_pipeline_data(self, data: Any) -> PipelineData:
+    def _generate_pipeline_data(self, data: Any = _request_generator) -> PipelineData:
         """Handle whether to use input generator or given user data"""
-        if data is None:
-            return PipelineData(data=self.__input_generator())
+        if isinstance(data, InputGeneratorRequest):
+            return PipelineData(data=self._input_generator())
         else:
             return PipelineData(data=data)
 
-    def __loop_handler(self) -> None:
-        """Function to be run by the input generator thread"""
+    def _push_pipeline_data(self, data: PipelineData) -> bool:
+        """Push the pipeline data into the pipeline"""
         if self.pipeline is None:
             raise PipelineUndefined("Pipeline has not been defined")
-        self.__loop_is_start.wait()
-        check_period = max(0.001, self.__loop_period / 10)
-        while self.__loop_is_start.is_set():
-            last_update = time.time()
-            data = self.__generate_pipeline_data(None)
-            self.pipeline.forward(data)
-            while time.time() - last_update < self.__loop_period:
-                time.sleep(check_period)
+        data.profile.tick_start(_PIPELINE_NAME_IN_PROFILE)
+        return self.pipeline.forward(data)
```

### Comparing `pystream-pipeline-0.1.2/pystream/pipeline/pipeline_base.py` & `pystream_pipeline-0.1.3/pystream/stage/stage.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 from abc import ABC, abstractmethod
-from typing import List
+from typing import Callable, TypeVar, Union
 
-from pystream.stage.stage import StageCallable
-from pystream.data.pipeline_data import PipelineData
 
+T = TypeVar("T")
 
-class PipelineBase(ABC):
-    @abstractmethod
-    def __init__(
-        self,
-        stages: List[StageCallable],
-    ) -> None:
-        """The class that will handle the pipeline.
 
-        Args:
-            stages (List[StageCallable]): The stages to be run
-                in sequence.
-        """
-        pass
+class Stage(ABC):
+    """Base class for the pipeline stage. As an example, stages that
+    have a cleanup routine should be defined as a subclass of this class.
 
-    @abstractmethod
-    def forward(self, data_input: PipelineData) -> bool:
-        """Send data to be processed by pipeline
-
-        Args:
-            data_input (PipelineData): the input data
+    Useful property:
+        name (str): the stage name, if not defined by the child instance,
+            the name will be assigned automatically after the pipeline
+            is constructed. Defaults to ""
+    """
 
-        Returns:
-            bool: True if the data is sent successfully, False otherwise
-        """
-        pass
+    name: str = ""
 
     @abstractmethod
-    def get_results(self) -> PipelineData:
-        """Get output from the last stage
+    def __call__(self, data: T) -> T:
+        """Main process of the stage.
+
+        Args:
+            data (T): Input data
 
         Returns:
-            PipelineData: the obtained data
+            T: output data, should be in the same type as input data
         """
         pass
 
     @abstractmethod
     def cleanup(self) -> None:
-        """Cleanup the pipeline."""
+        """Cleanup method for the stage. This method will be invoked
+        during pipeline cleanup step"""
         pass
+
+
+StageCallable = Union[Callable[[T], T], Stage]
```

### Comparing `pystream-pipeline-0.1.2/README.md` & `pystream_pipeline-0.1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 ## Concepts
 
 In general, PyStream is a package, fully implemented in python, that helps you manage a data pipeline and optimize its operation performance. The main feature of PyStream is that it can build your data pipeline in asynchronous and independent multi-threaded stages model, and hopefully multi-process model in the future.
 
 A PyStream **pipeline** is constructed by several **stages**, where each stage represents a single set of data processing operations that you define by your own. When the stages have been defined, the pipeline can be operated in two modes:
 
 - **Serial mode:** In this mode, each stage are executed in blocking fashion. The later stages will only be executed when the previous ones have been executed, and the next data can only be processed if the previous data have been processed by the final stage. There is only one data stream that can be processed at any time.
+
 - **Parallel mode:** In this mode, each stage live in a separate parallel thread. If a data has been finished being processed by a stage, the results will be send to the next stage. Since each stage runs in parallel, that stage can immediately take next data input if exist and process it immediately. This way, we can process multiple data at one time, thus increasing the throughput of your pipeline.
 
 Whatever the mode you choose, you only need to focus on implementation of your own data processing codes and pack them into several stages. PyStream will handle the pipeline executions including the threads and the linking of stages for you.
 
 ## Installation
 
 You can install this package using `pip`.
 
 ```bash
 pip install pystream-pipeline
 ```
 
-If you want to build this package from source or develop it, we recommend you to use Poetry. First install Poetry by following the instructions in its documentation site (you can google it). Then clone this repository and install all the dependencies. Poetry can help you do this and it will also setup a new virtual environment for you.
+If you want to build this package from source or develop it, we recommend you to use Poetry. First install Poetry by following the instructions in [its documentation site](https://python-poetry.org/docs/#installation). Then clone this repository and install all the dependencies. Poetry can help you do this and it will also setup a new virtual environment for you.
 
 ```bash
 poetry install
 ```
 
 To build the wheel file, you can run
 
@@ -36,8 +37,12 @@
 ```
 
 You can find the wheel file inside `dist` directory.
 
 ## Sample Usage
 
 API of PyStream can be found in this project [documentation](https://pystream-pipeline.readthedocs.io/).
-See `dummy_pipeline.py` to see how PyStream can be used to build a dummy pipeline.
+
+You can also access some examples:
+
+- See [`demo.ipynb`](demo.ipynb) to see how PyStream can be used to build a dummy pipeline.
+- See how PyStream is used to increase the throughput of a vehicle environment mapping system in [this repository](https://github.com/MukhlasAdib/KITTI_Mapping/tree/main/app).
```

### Comparing `pystream-pipeline-0.1.2/setup.py` & `pystream_pipeline-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,29 +2,34 @@
 from setuptools import setup
 
 packages = \
 ['pystream',
  'pystream.data',
  'pystream.functional',
  'pystream.pipeline',
- 'pystream.stage']
+ 'pystream.stage',
+ 'pystream.utils']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['loguru>=0.6.0,<0.7.0', 'pandas>=1.5.2,<2.0.0', 'tabulate>=0.9.0,<0.10.0']
+
 setup_kwargs = {
     'name': 'pystream-pipeline',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Python package to create and manage fast parallelized data processing pipeline for real-time application',
-    'long_description': '# PyStream - Real Time Python Pipeline Manager\n\nThis package provides tools to build and boost up a python data pipeline for real time processing. This package is managed using [Poetry](https://python-poetry.org/ ).\n\nFor more detailed guidelines, visit this project [documentation](https://pystream-pipeline.readthedocs.io/).\n\n## Concepts\n\nIn general, PyStream is a package, fully implemented in python, that helps you manage a data pipeline and optimize its operation performance. The main feature of PyStream is that it can build your data pipeline in asynchronous and independent multi-threaded stages model, and hopefully multi-process model in the future.\n\nA PyStream **pipeline** is constructed by several **stages**, where each stage represents a single set of data processing operations that you define by your own. When the stages have been defined, the pipeline can be operated in two modes:\n\n- **Serial mode:** In this mode, each stage are executed in blocking fashion. The later stages will only be executed when the previous ones have been executed, and the next data can only be processed if the previous data have been processed by the final stage. There is only one data stream that can be processed at any time.\n- **Parallel mode:** In this mode, each stage live in a separate parallel thread. If a data has been finished being processed by a stage, the results will be send to the next stage. Since each stage runs in parallel, that stage can immediately take next data input if exist and process it immediately. This way, we can process multiple data at one time, thus increasing the throughput of your pipeline.\n\nWhatever the mode you choose, you only need to focus on implementation of your own data processing codes and pack them into several stages. PyStream will handle the pipeline executions including the threads and the linking of stages for you.\n\n## Installation\n\nYou can install this package using `pip`.\n\n```bash\npip install pystream-pipeline\n```\n\nIf you want to build this package from source or develop it, we recommend you to use Poetry. First install Poetry by following the instructions in its documentation site (you can google it). Then clone this repository and install all the dependencies. Poetry can help you do this and it will also setup a new virtual environment for you.\n\n```bash\npoetry install\n```\n\nTo build the wheel file, you can run\n\n```bash\npoetry build\n```\n\nYou can find the wheel file inside `dist` directory.\n\n## Sample Usage\n\nAPI of PyStream can be found in this project [documentation](https://pystream-pipeline.readthedocs.io/).\nSee `dummy_pipeline.py` to see how PyStream can be used to build a dummy pipeline.\n',
+    'long_description': '# PyStream - Real Time Python Pipeline Manager\n\nThis package provides tools to build and boost up a python data pipeline for real time processing. This package is managed using [Poetry](https://python-poetry.org/ ).\n\nFor more detailed guidelines, visit this project [documentation](https://pystream-pipeline.readthedocs.io/).\n\n## Concepts\n\nIn general, PyStream is a package, fully implemented in python, that helps you manage a data pipeline and optimize its operation performance. The main feature of PyStream is that it can build your data pipeline in asynchronous and independent multi-threaded stages model, and hopefully multi-process model in the future.\n\nA PyStream **pipeline** is constructed by several **stages**, where each stage represents a single set of data processing operations that you define by your own. When the stages have been defined, the pipeline can be operated in two modes:\n\n- **Serial mode:** In this mode, each stage are executed in blocking fashion. The later stages will only be executed when the previous ones have been executed, and the next data can only be processed if the previous data have been processed by the final stage. There is only one data stream that can be processed at any time.\n\n- **Parallel mode:** In this mode, each stage live in a separate parallel thread. If a data has been finished being processed by a stage, the results will be send to the next stage. Since each stage runs in parallel, that stage can immediately take next data input if exist and process it immediately. This way, we can process multiple data at one time, thus increasing the throughput of your pipeline.\n\nWhatever the mode you choose, you only need to focus on implementation of your own data processing codes and pack them into several stages. PyStream will handle the pipeline executions including the threads and the linking of stages for you.\n\n## Installation\n\nYou can install this package using `pip`.\n\n```bash\npip install pystream-pipeline\n```\n\nIf you want to build this package from source or develop it, we recommend you to use Poetry. First install Poetry by following the instructions in [its documentation site](https://python-poetry.org/docs/#installation). Then clone this repository and install all the dependencies. Poetry can help you do this and it will also setup a new virtual environment for you.\n\n```bash\npoetry install\n```\n\nTo build the wheel file, you can run\n\n```bash\npoetry build\n```\n\nYou can find the wheel file inside `dist` directory.\n\n## Sample Usage\n\nAPI of PyStream can be found in this project [documentation](https://pystream-pipeline.readthedocs.io/).\n\nYou can also access some examples:\n\n- See [`demo.ipynb`](demo.ipynb) to see how PyStream can be used to build a dummy pipeline.\n- See how PyStream is used to increase the throughput of a vehicle environment mapping system in [this repository](https://github.com/MukhlasAdib/KITTI_Mapping/tree/main/app).\n',
     'author': 'Mukhlas Adib',
     'author_email': 'adib.rasyidy@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/MukhlasAdib/pystream-pipeline',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pystream-pipeline-0.1.2/PKG-INFO` & `pystream_pipeline-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: pystream-pipeline
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package to create and manage fast parallelized data processing pipeline for real-time application
 Home-page: https://github.com/MukhlasAdib/pystream-pipeline
 License: MIT
 Keywords: data-pipeline,parallelization,data-processing,performance,real-time
 Author: Mukhlas Adib
 Author-email: adib.rasyidy@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://pystream-pipeline.readthedocs.io/
 Project-URL: Repository, https://github.com/MukhlasAdib/pystream-pipeline
 Description-Content-Type: text/markdown
 
 # PyStream - Real Time Python Pipeline Manager
 
 This package provides tools to build and boost up a python data pipeline for real time processing. This package is managed using [Poetry](https://python-poetry.org/ ).
@@ -31,27 +35,28 @@
 ## Concepts
 
 In general, PyStream is a package, fully implemented in python, that helps you manage a data pipeline and optimize its operation performance. The main feature of PyStream is that it can build your data pipeline in asynchronous and independent multi-threaded stages model, and hopefully multi-process model in the future.
 
 A PyStream **pipeline** is constructed by several **stages**, where each stage represents a single set of data processing operations that you define by your own. When the stages have been defined, the pipeline can be operated in two modes:
 
 - **Serial mode:** In this mode, each stage are executed in blocking fashion. The later stages will only be executed when the previous ones have been executed, and the next data can only be processed if the previous data have been processed by the final stage. There is only one data stream that can be processed at any time.
+
 - **Parallel mode:** In this mode, each stage live in a separate parallel thread. If a data has been finished being processed by a stage, the results will be send to the next stage. Since each stage runs in parallel, that stage can immediately take next data input if exist and process it immediately. This way, we can process multiple data at one time, thus increasing the throughput of your pipeline.
 
 Whatever the mode you choose, you only need to focus on implementation of your own data processing codes and pack them into several stages. PyStream will handle the pipeline executions including the threads and the linking of stages for you.
 
 ## Installation
 
 You can install this package using `pip`.
 
 ```bash
 pip install pystream-pipeline
 ```
 
-If you want to build this package from source or develop it, we recommend you to use Poetry. First install Poetry by following the instructions in its documentation site (you can google it). Then clone this repository and install all the dependencies. Poetry can help you do this and it will also setup a new virtual environment for you.
+If you want to build this package from source or develop it, we recommend you to use Poetry. First install Poetry by following the instructions in [its documentation site](https://python-poetry.org/docs/#installation). Then clone this repository and install all the dependencies. Poetry can help you do this and it will also setup a new virtual environment for you.
 
 ```bash
 poetry install
 ```
 
 To build the wheel file, you can run
 
@@ -60,9 +65,13 @@
 ```
 
 You can find the wheel file inside `dist` directory.
 
 ## Sample Usage
 
 API of PyStream can be found in this project [documentation](https://pystream-pipeline.readthedocs.io/).
-See `dummy_pipeline.py` to see how PyStream can be used to build a dummy pipeline.
+
+You can also access some examples:
+
+- See [`demo.ipynb`](demo.ipynb) to see how PyStream can be used to build a dummy pipeline.
+- See how PyStream is used to increase the throughput of a vehicle environment mapping system in [this repository](https://github.com/MukhlasAdib/KITTI_Mapping/tree/main/app).
```

