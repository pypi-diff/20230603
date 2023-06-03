# Comparing `tmp/continuedev-0.1.0.tar.gz` & `tmp/continuedev-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuedev-0.1.0.tar", max compression
+gzip compressed data, was "continuedev-0.1.1.tar", max compression
```

## Comparing `continuedev-0.1.0.tar` & `continuedev-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,55 @@
--rw-r--r--   0        0        0      470 2023-05-24 03:34:05.182637 continuedev-0.1.0/README.md
--rw-r--r--   0        0        0      518 2023-05-21 18:46:30.772882 continuedev-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-21 18:46:30.776856 continuedev-0.1.0/src/continuedev/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 18:46:30.776937 continuedev-0.1.0/src/continuedev/libs/__init__.py
--rw-r--r--   0        0        0        4 2023-05-21 18:46:30.777355 continuedev-0.1.0/src/continuedev/libs/chroma/.gitignore
--rw-r--r--   0        0        0     2108 2023-05-21 18:46:30.777730 continuedev-0.1.0/src/continuedev/libs/chroma/query.py
--rw-r--r--   0        0        0      565 2023-05-21 18:46:30.777844 continuedev-0.1.0/src/continuedev/libs/chroma/replace.py
--rw-r--r--   0        0        0     7251 2023-05-21 18:46:30.777961 continuedev-0.1.0/src/continuedev/libs/chroma/update.py
--rw-r--r--   0        0        0    13904 2023-05-24 03:19:13.559370 continuedev-0.1.0/src/continuedev/libs/core.py
--rw-r--r--   0        0        0      711 2023-05-21 18:46:30.778494 continuedev-0.1.0/src/continuedev/libs/llm/__init__.py
--rw-r--r--   0        0        0      691 2023-05-21 18:46:30.778901 continuedev-0.1.0/src/continuedev/libs/llm/hugging_face.py
--rw-r--r--   0        0        0     6199 2023-05-24 01:17:03.358032 continuedev-0.1.0/src/continuedev/libs/llm/openai.py
--rw-r--r--   0        0        0     2776 2023-05-24 01:19:23.891082 continuedev-0.1.0/src/continuedev/libs/llm/prompt_utils.py
--rw-r--r--   0        0        0     3801 2023-05-24 01:25:24.223397 continuedev-0.1.0/src/continuedev/libs/llm/prompters.py
--rw-r--r--   0        0        0      872 2023-05-21 18:46:30.780030 continuedev-0.1.0/src/continuedev/libs/llm/utils.py
--rw-r--r--   0        0        0      621 2023-05-24 03:09:24.428263 continuedev-0.1.0/src/continuedev/libs/observation.py
--rw-r--r--   0        0        0     4036 2023-05-24 03:35:08.502539 continuedev-0.1.0/src/continuedev/libs/policy.py
--rw-r--r--   0        0        0        1 2023-05-21 18:46:30.780867 continuedev-0.1.0/src/continuedev/libs/steps/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-24 03:27:50.967710 continuedev-0.1.0/src/continuedev/libs/steps/chroma.py
--rw-r--r--   0        0        0      574 2023-05-24 03:35:05.485249 continuedev-0.1.0/src/continuedev/libs/steps/draft/abstract_method.py
--rw-r--r--   0        0        0     2758 2023-05-24 03:35:03.211602 continuedev-0.1.0/src/continuedev/libs/steps/draft/dlt.py
--rw-r--r--   0        0        0     1547 2023-05-24 03:35:04.554871 continuedev-0.1.0/src/continuedev/libs/steps/draft/redux.py
--rw-r--r--   0        0        0     1415 2023-05-24 03:35:06.359141 continuedev-0.1.0/src/continuedev/libs/steps/draft/typeorm.py
--rw-r--r--   0        0        0    11702 2023-05-24 03:29:55.483511 continuedev-0.1.0/src/continuedev/libs/steps/main.py
--rw-r--r--   0        0        0     1414 2023-05-21 18:46:30.782197 continuedev-0.1.0/src/continuedev/libs/steps/migration.py
--rw-r--r--   0        0        0     6580 2023-05-24 03:27:25.433009 continuedev-0.1.0/src/continuedev/libs/steps/nate.py
--rw-r--r--   0        0        0     1076 2023-05-21 18:46:30.782538 continuedev-0.1.0/src/continuedev/libs/steps/pytest.py
--rw-r--r--   0        0        0     6974 2023-05-24 03:33:25.130638 continuedev-0.1.0/src/continuedev/libs/steps/ty.py
--rw-r--r--   0        0        0     5703 2023-05-24 01:27:12.974789 continuedev-0.1.0/src/continuedev/libs/util/copy_codebase.py
--rw-r--r--   0        0        0      433 2023-05-21 18:46:30.784135 continuedev-0.1.0/src/continuedev/libs/util/map_path.py
--rw-r--r--   0        0        0      597 2023-05-21 18:46:30.784870 continuedev-0.1.0/src/continuedev/libs/util/queue.py
--rw-r--r--   0        0        0      668 2023-05-24 03:06:34.065779 continuedev-0.1.0/src/continuedev/libs/util/traceback_parsers.py
--rw-r--r--   0        0        0        0 2023-05-21 18:46:30.785146 continuedev-0.1.0/src/continuedev/models/__init__.py
--rw-r--r--   0        0        0    11397 2023-05-24 03:13:55.083298 continuedev-0.1.0/src/continuedev/models/filesystem.py
--rw-r--r--   0        0        0     4525 2023-05-24 03:12:57.315687 continuedev-0.1.0/src/continuedev/models/filesystem_edit.py
--rw-r--r--   0        0        0      978 2023-05-21 19:13:50.102492 continuedev-0.1.0/src/continuedev/models/generate_json_schema.py
--rw-r--r--   0        0        0     3937 2023-05-21 18:46:30.786214 continuedev-0.1.0/src/continuedev/models/main.py
--rw-r--r--   0        0        0      741 2023-05-21 18:46:30.786759 continuedev-0.1.0/src/continuedev/plugins/__init__.py
--rw-r--r--   0        0        0      767 2023-05-21 18:46:30.787256 continuedev-0.1.0/src/continuedev/plugins/load.py
--rw-r--r--   0        0        0      144 2023-05-21 18:46:30.787592 continuedev-0.1.0/src/continuedev/plugins/policy/__init__.py
--rw-r--r--   0        0        0      247 2023-05-21 18:46:30.788064 continuedev-0.1.0/src/continuedev/plugins/policy/hookspecs.py
--rw-r--r--   0        0        0        0 2023-05-21 18:46:30.788123 continuedev-0.1.0/src/continuedev/plugins/policy/libs/__init__.py
--rw-r--r--   0        0        0      617 2023-05-21 18:46:30.788633 continuedev-0.1.0/src/continuedev/plugins/policy/libs/alternate.py
--rw-r--r--   0        0        0      142 2023-05-21 18:46:30.788805 continuedev-0.1.0/src/continuedev/plugins/step/__init__.py
--rw-r--r--   0        0        0      359 2023-05-24 03:15:15.526923 continuedev-0.1.0/src/continuedev/plugins/step/hookspecs.py
--rw-r--r--   0        0        0        0 2023-05-24 03:16:24.862810 continuedev-0.1.0/src/continuedev/plugins/step/libs/__init__.py
--rw-r--r--   0        0        0      217 2023-05-21 18:46:30.789469 continuedev-0.1.0/src/continuedev/plugins/step/libs/hello_world.py
--rw-r--r--   0        0        0    10804 2023-05-24 03:18:42.094014 continuedev-0.1.0/src/continuedev/server/ide.py
--rw-r--r--   0        0        0     2372 2023-05-24 03:17:19.924014 continuedev-0.1.0/src/continuedev/server/ide_protocol.py
--rw-r--r--   0        0        0      829 2023-05-21 18:46:30.791730 continuedev-0.1.0/src/continuedev/server/main.py
--rw-r--r--   0        0        0     6690 2023-05-24 03:34:58.288680 continuedev-0.1.0/src/continuedev/server/notebook.py
--rw-r--r--   0        0        0     1361 1970-01-01 00:00:00.000000 continuedev-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1019 2023-06-02 18:03:06.540784 continuedev-0.1.1/README.md
+-rw-r--r--   0        0        0      622 2023-06-03 00:20:33.127699 continuedev-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-21 18:46:30.776856 continuedev-0.1.1/src/continuedev/__init__.py
+-rw-r--r--   0        0        0     6856 2023-06-02 23:45:17.392715 continuedev-0.1.1/src/continuedev/core/agent.py
+-rw-r--r--   0        0        0     7161 2023-06-02 18:03:06.542074 continuedev-0.1.1/src/continuedev/core/autopilot.py
+-rw-r--r--   0        0        0      930 2023-06-02 18:03:06.542160 continuedev-0.1.1/src/continuedev/core/config.py
+-rw-r--r--   0        0        0      710 2023-06-02 18:03:06.542235 continuedev-0.1.1/src/continuedev/core/env.py
+-rw-r--r--   0        0        0     4867 2023-06-02 18:03:06.542338 continuedev-0.1.1/src/continuedev/core/main.py
+-rw-r--r--   0        0        0      621 2023-06-02 18:03:06.542524 continuedev-0.1.1/src/continuedev/core/observation.py
+-rw-r--r--   0        0        0     4456 2023-06-02 18:03:06.542622 continuedev-0.1.1/src/continuedev/core/policy.py
+-rw-r--r--   0        0        0     5337 2023-06-02 18:03:06.542723 continuedev-0.1.1/src/continuedev/core/sdk.py
+-rw-r--r--   0        0        0        0 2023-05-21 18:46:30.776937 continuedev-0.1.1/src/continuedev/libs/__init__.py
+-rw-r--r--   0        0        0        4 2023-05-21 18:46:30.777355 continuedev-0.1.1/src/continuedev/libs/chroma/.gitignore
+-rw-r--r--   0        0        0     2108 2023-05-21 18:46:30.777730 continuedev-0.1.1/src/continuedev/libs/chroma/query.py
+-rw-r--r--   0        0        0      565 2023-05-21 18:46:30.777844 continuedev-0.1.1/src/continuedev/libs/chroma/replace.py
+-rw-r--r--   0        0        0     7251 2023-05-21 18:46:30.777961 continuedev-0.1.1/src/continuedev/libs/chroma/update.py
+-rw-r--r--   0        0        0      711 2023-05-21 18:46:30.778494 continuedev-0.1.1/src/continuedev/libs/llm/__init__.py
+-rw-r--r--   0        0        0      791 2023-06-02 18:03:06.542816 continuedev-0.1.1/src/continuedev/libs/llm/hf_inference_api.py
+-rw-r--r--   0        0        0      691 2023-05-21 18:46:30.778901 continuedev-0.1.1/src/continuedev/libs/llm/hugging_face.py
+-rw-r--r--   0        0        0     6286 2023-06-02 18:03:06.543101 continuedev-0.1.1/src/continuedev/libs/llm/openai.py
+-rw-r--r--   0        0        0     2776 2023-05-24 01:19:23.891082 continuedev-0.1.1/src/continuedev/libs/llm/prompt_utils.py
+-rw-r--r--   0        0        0     3801 2023-05-24 01:25:24.223397 continuedev-0.1.1/src/continuedev/libs/llm/prompters.py
+-rw-r--r--   0        0        0      872 2023-05-21 18:46:30.780030 continuedev-0.1.1/src/continuedev/libs/llm/utils.py
+-rw-r--r--   0        0        0        1 2023-05-21 18:46:30.780867 continuedev-0.1.1/src/continuedev/libs/steps/__init__.py
+-rw-r--r--   0        0        0     2072 2023-06-02 18:03:06.543426 continuedev-0.1.1/src/continuedev/libs/steps/chroma.py
+-rw-r--r--   0        0        0     1205 2023-06-02 18:03:06.543542 continuedev-0.1.1/src/continuedev/libs/steps/continue_step.py
+-rw-r--r--   0        0        0     7071 2023-06-02 18:03:06.543663 continuedev-0.1.1/src/continuedev/libs/steps/core/core.py
+-rw-r--r--   0        0        0      604 2023-06-02 18:03:06.543937 continuedev-0.1.1/src/continuedev/libs/steps/draft/abstract_method.py
+-rw-r--r--   0        0        0     4403 2023-06-02 18:03:06.544229 continuedev-0.1.1/src/continuedev/libs/steps/draft/dlt.py
+-rw-r--r--   0        0        0     1485 2023-06-02 18:03:06.544492 continuedev-0.1.1/src/continuedev/libs/steps/draft/redux.py
+-rw-r--r--   0        0        0     1445 2023-06-02 18:03:06.544744 continuedev-0.1.1/src/continuedev/libs/steps/draft/typeorm.py
+-rw-r--r--   0        0        0    12613 2023-06-02 18:03:06.544990 continuedev-0.1.1/src/continuedev/libs/steps/main.py
+-rw-r--r--   0        0        0     1439 2023-06-02 18:03:06.545259 continuedev-0.1.1/src/continuedev/libs/steps/migration.py
+-rw-r--r--   0        0        0     6623 2023-06-02 18:03:06.545484 continuedev-0.1.1/src/continuedev/libs/steps/nate.py
+-rw-r--r--   0        0        0     1101 2023-06-02 18:03:06.545632 continuedev-0.1.1/src/continuedev/libs/steps/pytest.py
+-rw-r--r--   0        0        0        0 2023-06-02 18:03:06.545662 continuedev-0.1.1/src/continuedev/libs/steps/react_posthog.py
+-rw-r--r--   0        0        0      869 2023-06-02 18:03:06.545908 continuedev-0.1.1/src/continuedev/libs/steps/steps_on_startup.py
+-rw-r--r--   0        0        0     7057 2023-06-02 18:03:06.546095 continuedev-0.1.1/src/continuedev/libs/steps/ty.py
+-rw-r--r--   0        0        0     5747 2023-06-02 04:56:35.173706 continuedev-0.1.1/src/continuedev/libs/util/copy_codebase.py
+-rw-r--r--   0        0        0      433 2023-05-21 18:46:30.784135 continuedev-0.1.1/src/continuedev/libs/util/map_path.py
+-rw-r--r--   0        0        0      597 2023-05-21 18:46:30.784870 continuedev-0.1.1/src/continuedev/libs/util/queue.py
+-rw-r--r--   0        0        0      501 2023-06-02 18:03:06.546185 continuedev-0.1.1/src/continuedev/libs/util/telemetry.py
+-rw-r--r--   0        0        0      668 2023-05-24 03:06:34.065779 continuedev-0.1.1/src/continuedev/libs/util/traceback_parsers.py
+-rw-r--r--   0        0        0        0 2023-05-21 18:46:30.785146 continuedev-0.1.1/src/continuedev/models/__init__.py
+-rw-r--r--   0        0        0    11397 2023-05-24 03:13:55.083298 continuedev-0.1.1/src/continuedev/models/filesystem.py
+-rw-r--r--   0        0        0     4785 2023-06-02 18:03:06.546467 continuedev-0.1.1/src/continuedev/models/filesystem_edit.py
+-rw-r--r--   0        0        0     1082 2023-06-02 18:03:06.546744 continuedev-0.1.1/src/continuedev/models/generate_json_schema.py
+-rw-r--r--   0        0        0     5240 2023-06-02 18:03:06.547073 continuedev-0.1.1/src/continuedev/models/main.py
+-rw-r--r--   0        0        0     4268 2023-06-02 18:03:06.547175 continuedev-0.1.1/src/continuedev/server/gui.py
+-rw-r--r--   0        0        0      837 2023-06-02 18:03:06.547267 continuedev-0.1.1/src/continuedev/server/gui_protocol.py
+-rw-r--r--   0        0        0    11083 2023-06-02 20:58:40.940099 continuedev-0.1.1/src/continuedev/server/ide.py
+-rw-r--r--   0        0        0     2342 2023-06-02 18:03:06.547971 continuedev-0.1.1/src/continuedev/server/ide_protocol.py
+-rw-r--r--   0        0        0     1050 2023-06-02 23:42:31.427657 continuedev-0.1.1/src/continuedev/server/main.py
+-rw-r--r--   0        0        0     3100 2023-06-02 18:03:06.548263 continuedev-0.1.1/src/continuedev/server/session_manager.py
+-rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 continuedev-0.1.1/PKG-INFO
```

### Comparing `continuedev-0.1.0/pyproject.toml` & `continuedev-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "continuedev"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Nate Sesti <sestinj@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fastapi = "^0.95.1"
@@ -15,11 +15,15 @@
 uvicorn = "^0.21.1"
 python-dotenv = "^1.0.0"
 nest-asyncio = "^1.5.6"
 websockets = "^11.0.2"
 urllib3 = "1.26.15"
 gpt-index = "^0.6.8"
 setuptools = "^67.7.2"
+posthog = "^3.0.1"
+
+[tool.poetry.scripts]
+typegen = "src.continuedev.models.generate_json_schema:main" 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `continuedev-0.1.0/src/continuedev/libs/chroma/query.py` & `continuedev-0.1.1/src/continuedev/libs/chroma/query.py`

 * *Files identical despite different names*

### Comparing `continuedev-0.1.0/src/continuedev/libs/chroma/replace.py` & `continuedev-0.1.1/src/continuedev/libs/chroma/replace.py`

 * *Files identical despite different names*

### Comparing `continuedev-0.1.0/src/continuedev/libs/chroma/update.py` & `continuedev-0.1.1/src/continuedev/libs/chroma/update.py`

 * *Files identical despite different names*

### Comparing `continuedev-0.1.0/src/continuedev/libs/core.py` & `continuedev-0.1.1/src/continuedev/libs/steps/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,423 +1,358 @@
-import traceback
-import time
-from typing import Callable, Coroutine, Dict, Generator, List, Tuple, Union
-from ..models.filesystem_edit import EditDiff, FileEdit, FileEditWithFullContents, FileSystemEdit
-from ..models.filesystem import FileSystem
-from pydantic import BaseModel, parse_file_as, validator
-from .llm import LLM
-from .observation import Observation, UserInputObservation
-from ..server.ide_protocol import AbstractIdeProtocolServer
-from .util.queue import AsyncSubscriptionQueue
-
-
-class ContinueBaseModel(BaseModel):
-    class Config:
-        underscore_attrs_are_private = True
-
-
-class HistoryNode(ContinueBaseModel):
-    """A point in history, a list of which make up History"""
-    step: "Step"
-    observation: Union[Observation, None]
-    depth: int
-
-
-class History(ContinueBaseModel):
-    """A history of steps taken and their results"""
-    timeline: List[HistoryNode]
-    current_index: int
-
-    def add_node(self, node: HistoryNode):
-        self.timeline.insert(self.current_index + 1, node)
-        self.current_index += 1
+from typing import Coroutine, List, Union
 
-    def get_current(self) -> Union[HistoryNode, None]:
-        if self.current_index < 0:
-            return None
-        return self.timeline[self.current_index]
+from pydantic import BaseModel
 
-    def remove_current_and_substeps(self):
-        self.timeline.pop(self.current_index)
-        while self.get_current() is not None and self.get_current().depth > 0:
-            self.timeline.pop(self.current_index)
-
-    def take_next_step(self) -> Union["Step", None]:
-        if self.has_future():
-            self.current_index += 1
-            current_state = self.get_current()
-            if current_state is None:
-                return None
-            return current_state.step
-        return None
+from ..util.traceback_parsers import parse_python_traceback
+from ..llm import LLM
+from ...models.main import Traceback, Range
+from ...models.filesystem_edit import EditDiff, FileEdit
+from ...models.filesystem import RangeInFile, RangeInFileWithContents
+from ...core.observation import Observation, TextObservation, TracebackObservation
+from ..llm.prompt_utils import MarkdownStyleEncoderDecoder
+from textwrap import dedent
+from ...core.main import Step
+from ...core.sdk import ContinueSDK, Models
+from ...core.observation import Observation
+import subprocess
+from .core.core import EditCodeStep
 
-    def get_current_index(self) -> int:
-        return self.current_index
 
-    def has_future(self) -> bool:
-        return self.current_index < len(self.timeline) - 1
+class RunCodeStep(Step):
+    cmd: str
 
-    def step_back(self):
-        self.current_index -= 1
+    async def describe(self, models: Models) -> Coroutine[str, None, None]:
+        return f"Ran command: `{self.cmd}`"
 
-    def last_observation(self) -> Union[Observation, None]:
-        state = self.get_current()
-        if state is None:
+    async def run(self, sdk: ContinueSDK) -> Coroutine[Observation, None, None]:
+        result = subprocess.run(
+            self.cmd.split(), stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        stdout = result.stdout.decode("utf-8")
+        stderr = result.stderr.decode("utf-8")
+        print(stdout, stderr)
+
+        # If it fails, return the error
+        tb = parse_python_traceback(stdout) or parse_python_traceback(stderr)
+        if tb:
+            return TracebackObservation(traceback=tb)
+        else:
+            self.hide = True
             return None
-        return state.observation
 
-    @classmethod
-    def from_empty(cls):
-        return cls(timeline=[], current_index=-1)
 
+class Policy(BaseModel):
+    pass
 
-class FullState(ContinueBaseModel):
-    """A full state of the program, including the history"""
-    history: History
-    active: bool
-    user_input_queue: List[str]
 
+class RunPolicyUntilDoneStep(Step):
+    policy: "Policy"
 
-class Policy(ContinueBaseModel):
-    """A rule that determines which step to take next"""
+    async def run(self, sdk: ContinueSDK) -> Coroutine[Observation, None, None]:
+        next_step = self.policy.next(sdk.history)
+        while next_step is not None:
+            observation = await sdk.run_step(next_step)
+            next_step = self.policy.next(sdk.history)
+        return observation
 
-    # Note that history is mutable, kinda sus
-    def next(self, history: History = History.from_empty()) -> "Step":
-        raise NotImplementedError
 
+class RunCommandStep(Step):
+    cmd: str
+    name: str = "Run command"
+    _description: str = None
 
-class ContinueSDK:
-    """The SDK provided as parameters to a step"""
-    llm: LLM
-    ide: AbstractIdeProtocolServer
-    __agent: "Agent"
+    async def describe(self, models: Models) -> Coroutine[str, None, None]:
+        if self._description is not None:
+            return self._description
+        return self.cmd
 
-    def __init__(self, agent: "Agent", llm: Union[LLM, None] = None):
-        if llm is None:
-            self.llm = agent.llm
+    async def run(self, sdk: ContinueSDK) -> Coroutine[Observation, None, None]:
+        cwd = await sdk.ide.getWorkspaceDirectory()
+        result = subprocess.run(
+            self.cmd.split(), stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=cwd)
+        stdout = result.stdout.decode("utf-8")
+        stderr = result.stderr.decode("utf-8")
+        print(stdout, stderr)
+
+        # If it fails, return the error
+        if result.returncode != 0:
+            return TextObservation(text=stderr)
         else:
-            self.llm = llm
-        self.ide = agent.ide
-        self.__agent = agent
-
-    @property
-    def history(self) -> History:
-        return self.__agent.history
-
-    async def run_step(self, step: "Step") -> Coroutine[Observation, None, None]:
-        return await self.__agent._run_singular_step(step)
-
-    async def apply_filesystem_edit(self, edit: FileSystemEdit):
-        await self.run_step(FileSystemEditStep(edit=edit))
-
-    async def wait_for_user_input(self) -> str:
-        return await self.__agent.wait_for_user_input()
-
-
-class Agent(ContinueBaseModel):
-    llm: LLM
-    policy: Policy
-    ide: AbstractIdeProtocolServer
-    history: History = History.from_empty()
-    _on_update_callbacks: List[Callable[["FullState"], None]] = []
-
-    _active: bool = False
-    _should_halt: bool = False
-    _main_user_input_queue: List[str] = []
-
-    _user_input_queue = AsyncSubscriptionQueue()
-
-    class Config:
-        arbitrary_types_allowed = True
-
-    def get_full_state(self) -> FullState:
-        return FullState(history=self.history, active=self._active, user_input_queue=self._main_user_input_queue)
-
-    def on_update(self, callback: Callable[["FullState"], None]):
-        """Subscribe to changes to state"""
-        self._on_update_callbacks.append(callback)
-
-    def update_subscribers(self):
-        full_state = self.get_full_state()
-        for callback in self._on_update_callbacks:
-            callback(full_state)
-
-    def __get_step_params(self, step: "Step"):
-        return ContinueSDK(agent=self, llm=self.llm.with_system_message(step.system_message))
-
-    def give_user_input(self, input: str, index: int):
-        self._user_input_queue.post(index, input)
-
-    async def wait_for_user_input(self) -> str:
-        self._active = False
-        self.update_subscribers()
-        await self._user_input_queue.get(self.history.current_index)
-        self._active = True
-        self.update_subscribers()
-
-    _manual_edits_buffer: List[FileEditWithFullContents] = []
-
-    async def reverse_to_index(self, index: int):
-        try:
-            while self.history.get_current_index() >= index:
-                current_step = self.history.get_current().step
-                self.history.step_back()
-                if issubclass(current_step.__class__, ReversibleStep):
-                    await current_step.reverse(self.__get_step_params(current_step))
-
-                self.update_subscribers()
-        except Exception as e:
-            print(e)
-
-    def handle_manual_edits(self, edits: List[FileEditWithFullContents]):
-        for edit in edits:
-            self._manual_edits_buffer.append(edit)
-            # TODO: You're storing a lot of unecessary data here. Can compress into EditDiffs on the spot, and merge.
-            # self._manual_edits_buffer = merge_file_edit(self._manual_edits_buffer, edit)
-
-    def handle_traceback(self, traceback: str):
-        raise NotImplementedError
-
-    _step_depth: int = 0
-
-    async def _run_singular_step(self, step: "Step", is_future_step: bool = False) -> Coroutine[Observation, None, None]:
-        if not is_future_step:
-            # Check manual edits buffer, clear out if needed by creating a ManualEditStep
-            if len(self._manual_edits_buffer) > 0:
-                manualEditsStep = ManualEditStep.from_sequence(
-                    self._manual_edits_buffer)
-                self._manual_edits_buffer = []
-                await self._run_singular_step(manualEditsStep)
-
-        # Update history - do this first so we get top-first tree ordering
-        self.history.add_node(HistoryNode(
-            step=step, observation=None, depth=self._step_depth))
-
-        # Run step
-        self._step_depth += 1
-        observation = await step(self.__get_step_params(step))
-        self._step_depth -= 1
+            return TextObservation(text=stdout)
 
-        # Add observation to history
-        self.history.get_current().observation = observation
 
-        # Update its description
-        step._set_description(await step.describe(self.llm))
-
-        # Call all subscribed callbacks
-        self.update_subscribers()
+class FasterEditHighlightedCodeStep(Step):
+    user_input: str
+    hide = True
+    _completion: str = "Edit Code"
+    _edit_diffs: Union[List[EditDiff], None] = None
+    _prompt: str = dedent("""\
+        You will be given code to edit in order to perfectly satisfy the user request. All the changes you make must be described as replacements, which you should format in the following way:
+        FILEPATH
+        <FILE_TO_EDIT>
+        REPLACE_ME
+        <CODE_TO_REPLACE>
+        REPLACE_WITH
+        <CODE_TO_REPLACE_WITH>
+
+        where <CODE_TO_REPLACE> and <CODE_TO_REPLACE_WITH> can be multiple lines, but should be the mininum needed to make the edit. Be sure to maintain existing whitespace at the start of lines.
+
+        For example, if you want to replace the code `x = 1` with `x = 2` in main.py, you would write:
+        FILEPATH
+        main.py
+        REPLACE_ME
+        x = 1
+        REPLACE_WITH
+        x = 2
+        If you wanted to delete the code
+        ```
+        def sum(a, b):
+            return a + b
+        ```
+        in main.py, you would write:
+        FILEPATH
+        main.py
+        REPLACE_ME
+        def sum(a, b):
+            return a + b
+        REPLACE_WITH
+
+        You may need to make multiple edits; respond with exactly as many as needed.
+
+        Below is the code before changes:
+
+        {code}
+
+        This is the user request: "{user_input}"
+        Here is the description of changes to make:
+""")
 
-        return observation
+    async def describe(self, models: Models) -> Coroutine[str, None, None]:
+        return "Editing highlighted code"
 
-    async def run_from_step(self, step: "Step"):
-        # if self._active:
-        #     raise RuntimeError("Agent is already running")
-        self._active = True
-
-        next_step = step
-        is_future_step = False
-        while not (next_step is None or self._should_halt):
-            try:
-                if is_future_step:
-                    # If future step, then we are replaying and need to delete the step from history so it can be replaced
-                    self.history.remove_current_and_substeps()
-
-                observation = await self._run_singular_step(next_step, is_future_step)
-                if next_step := self.policy.next(self.history):
-                    is_future_step = False
-                elif next_step := self.history.take_next_step():
-                    is_future_step = True
+    async def run(self, sdk: ContinueSDK) -> Coroutine[Observation, None, None]:
+        range_in_files = await sdk.ide.getHighlightedCode()
+        if len(range_in_files) == 0:
+            # Get the full contents of all open files
+            files = await sdk.ide.getOpenFiles()
+            contents = {}
+            for file in files:
+                contents[file] = await sdk.ide.readFile(file)
+
+            range_in_files = [RangeInFile.from_entire_file(
+                filepath, content) for filepath, content in contents.items()]
+
+        rif_with_contents = []
+        for range_in_file in range_in_files:
+            file_contents = await sdk.ide.readRangeInFile(range_in_file)
+            rif_with_contents.append(
+                RangeInFileWithContents.from_range_in_file(range_in_file, file_contents))
+        enc_dec = MarkdownStyleEncoderDecoder(rif_with_contents)
+        code_string = enc_dec.encode()
+        prompt = self._prompt.format(
+            code=code_string, user_input=self.user_input)
+
+        rif_dict = {}
+        for rif in rif_with_contents:
+            rif_dict[rif.filepath] = rif.contents
+
+        completion = (await sdk.models.gpt35()).complete(prompt)
+
+        # Temporarily doing this to generate description.
+        self._prompt = prompt
+        self._completion = completion
+        print(completion)
+
+        # ALTERNATIVE DECODING STEP HERE
+        raw_file_edits = []
+        lines = completion.split("\n")
+        current_edit = {}
+        status = "FILEPATH"
+        for i in range(0, len(lines)):
+            line = lines[i]
+            if line == "FILEPATH":
+                if "FILEPATH" in current_edit:
+                    raw_file_edits.append(current_edit)
+                current_edit = {}
+                status = "FILEPATH"
+            elif line == "REPLACE_ME":
+                status = "REPLACE_ME"
+            elif line == "REPLACE_WITH":
+                status = "REPLACE_WITH"
+            elif status == "FILEPATH":
+                current_edit["filepath"] = line
+            elif status == "REPLACE_ME":
+                if "replace_me" in current_edit:
+                    current_edit["replace_me"] += "\n" + line
+                else:
+                    current_edit["replace_me"] = line
+            elif status == "REPLACE_WITH":
+                if "replace_with" in current_edit:
+                    current_edit["replace_with"] += "\n" + line
                 else:
-                    next_step = None
+                    current_edit["replace_with"] = line
+        if "filepath" in current_edit:
+            raw_file_edits.append(current_edit)
+
+        file_edits = []
+        for edit in raw_file_edits:
+            filepath = edit["filepath"]
+            replace_me = edit["replace_me"]
+            replace_with = edit["replace_with"]
+            file_edits.append(
+                FileEdit(filepath=filepath, range=Range.from_lines_snippet_in_file(content=rif_dict[filepath], snippet=replace_me), replacement=replace_with))
+        # ------------------------------
+
+        self._edit_diffs = []
+        for file_edit in file_edits:
+            diff = await sdk.apply_filesystem_edit(file_edit)
+            self._edit_diffs.append(diff)
+
+        for filepath in set([file_edit.filepath for file_edit in file_edits]):
+            await sdk.ide.saveFile(filepath)
+            await sdk.ide.setFileOpen(filepath)
 
-            except Exception as e:
-                print(
-                    f"Error while running step: \n{''.join(traceback.format_tb(e.__traceback__))}\n{e}")
-                next_step = None
-
-        self._active = False
-
-        # Doing this so active can make it to the frontend after steps are done. But want better state syncing tools
-        for callback in self._on_update_callbacks:
-            callback(None)
-
-    async def run_from_observation(self, observation: Observation):
-        next_step = self.policy.next(self.history)
-        await self.run_from_step(next_step)
-
-    async def run_policy(self):
-        first_step = self.policy.next(self.history)
-        await self.run_from_step(first_step)
-
-    async def _request_halt(self):
-        if self._active:
-            self._should_halt = True
-            while self._active:
-                time.sleep(0.1)
-        self._should_halt = False
         return None
 
-    async def accept_user_input(self, user_input: str):
-        self._main_user_input_queue.append(user_input)
-        self.update_subscribers()
 
-        if len(self._main_user_input_queue) > 1:
-            return
-
-        # await self._request_halt()
-        # Just run the step that takes user input, and
-        # then up to the policy to decide how to deal with it.
-        self._main_user_input_queue.pop(0)
-        self.update_subscribers()
-        await self.run_from_step(UserInputStep(user_input=user_input))
+class StarCoderEditHighlightedCodeStep(Step):
+    user_input: str
+    hide = False
+    _prompt: str = "<commit_before>{code}<commit_msg>{user_request}<commit_after>"
 
-        while len(self._main_user_input_queue) > 0:
-            await self.run_from_step(UserInputStep(
-                user_input=self._main_user_input_queue.pop(0)))
+    _prompt_and_completion: str = ""
 
-    async def accept_refinement_input(self, user_input: str, index: int):
-        await self._request_halt()
-        await self.reverse_to_index(index)
-        await self.run_from_step(UserInputStep(user_input=user_input))
+    async def describe(self, models: Models) -> Coroutine[str, None, None]:
+        return (await models.gpt35()).complete(f"{self._prompt_and_completion}\n\nPlease give brief a description of the changes made above using markdown bullet points:")
 
+    async def run(self, sdk: ContinueSDK) -> Coroutine[Observation, None, None]:
+        range_in_files = await sdk.ide.getHighlightedCode()
+        if len(range_in_files) == 0:
+            # Get the full contents of all open files
+            files = await sdk.ide.getOpenFiles()
+            contents = {}
+            for file in files:
+                contents[file] = await sdk.ide.readFile(file)
+
+            range_in_files = [RangeInFile.from_entire_file(
+                filepath, content) for filepath, content in contents.items()]
+
+        rif_with_contents = []
+        for range_in_file in range_in_files:
+            file_contents = await sdk.ide.readRangeInFile(range_in_file)
+            rif_with_contents.append(
+                RangeInFileWithContents.from_range_in_file(range_in_file, file_contents))
+
+        rif_dict = {}
+        for rif in rif_with_contents:
+            rif_dict[rif.filepath] = rif.contents
+
+        for rif in rif_with_contents:
+            prompt = self._prompt.format(
+                code=rif.contents, user_request=self.user_input)
+            completion = str((await sdk.models.starcoder()).complete(prompt))
+            eot_token = "<|endoftext|>"
+            if completion.endswith(eot_token):
+                completion = completion[:completion.rindex(eot_token)]
+
+            self._prompt_and_completion += prompt + completion
+
+            await sdk.ide.applyFileSystemEdit(
+                FileEdit(filepath=rif.filepath, range=rif.range, replacement=completion))
+            await sdk.ide.saveFile(rif.filepath)
+            await sdk.ide.setFileOpen(rif.filepath)
 
-class Step(ContinueBaseModel):
-    name: str = None
-    hide: bool = False
-    _description: Union[str, None] = None
 
-    system_message: Union[str, None] = None
+class EditHighlightedCodeStep(Step):
+    user_input: str
+    hide = True
+    _prompt: str = dedent("""Below is the code before changes:
 
-    class Config:
-        copy_on_model_validation = False
+{code}
 
-    async def describe(self, llm: LLM) -> Coroutine[str, None, None]:
-        if self._description is not None:
-            return self._description
-        return "Running step: " + self.name
+This is the user request:
 
-    def _set_description(self, description: str):
-        self._description = description
+{user_input}
 
-    def dict(self, *args, **kwargs):
-        d = super().dict(*args, **kwargs)
-        if self._description is not None:
-            d["description"] = self._description
-        else:
-            d["description"] = self.name
-        return d
+This is the code after being changed to perfectly satisfy the user request:
+    """)
 
-    @validator("name", pre=True, always=True)
-    def name_is_class_name(cls, name):
-        if name is None:
-            return cls.__name__
-        return name
+    async def describe(self, models: Models) -> Coroutine[str, None, None]:
+        return "Editing highlighted code"
 
     async def run(self, sdk: ContinueSDK) -> Coroutine[Observation, None, None]:
-        raise NotImplementedError
+        range_in_files = await sdk.ide.getHighlightedCode()
+        if len(range_in_files) == 0:
+            # Get the full contents of all open files
+            files = await sdk.ide.getOpenFiles()
+            contents = {}
+            for file in files:
+                contents[file] = await sdk.ide.readFile(file)
+
+            range_in_files = [RangeInFile.from_entire_file(
+                filepath, content) for filepath, content in contents.items()]
+
+        await sdk.run_step(EditCodeStep(
+            range_in_files=range_in_files, prompt=self._prompt.format(code="{code}", user_input=self.user_input)))
 
-    async def __call__(self, sdk: ContinueSDK) -> Coroutine[Observation, None, None]:
-        return await self.run(sdk)
-
-    def __rshift__(self, other: "Step"):
-        steps = []
-        if isinstance(self, SequentialStep):
-            steps = self.steps
-        else:
-            steps.append(self)
-        if isinstance(other, SequentialStep):
-            steps += other.steps
-        else:
-            steps.append(other)
-        return SequentialStep(steps=steps)
 
+class FindCodeStep(Step):
+    prompt: str
 
-class SequentialStep(Step):
-    steps: list[Step]
-    hide: bool = True
+    async def describe(self, models: Models) -> Coroutine[str, None, None]:
+        return "Finding code"
 
     async def run(self, sdk: ContinueSDK) -> Coroutine[Observation, None, None]:
-        for step in self.steps:
-            observation = await sdk.run_step(step)
-        return observation
+        return await sdk.ide.getOpenFiles()
 
 
-class ReversibleStep(Step):
-    async def reverse(self, sdk: ContinueSDK):
-        raise NotImplementedError
+class UserInputStep(Step):
+    user_input: str
 
 
-class FileSystemEditStep(ReversibleStep):
-    edit: FileSystemEdit
-    _diff: Union[EditDiff, None] = None
+class SolveTracebackStep(Step):
+    traceback: Traceback
 
-    hide: bool = True
+    async def describe(self, models: Models) -> Coroutine[str, None, None]:
+        return f"```\n{self.traceback.full_traceback}\n```"
 
-    async def run(self, sdk: "ContinueSDK") -> Coroutine[Observation, None, None]:
-        self._diff = await sdk.ide.applyFileSystemEdit(self.edit)
-        return None
+    async def run(self, sdk: ContinueSDK) -> Coroutine[Observation, None, None]:
+        prompt = dedent("""I ran into this problem with my Python code:
 
-    async def reverse(self, sdk: "ContinueSDK"):
-        await sdk.ide.applyFileSystemEdit(self._diff.backward)
-        # Where and when should file saves happen?
+                {traceback}
 
+                Below are the files that might need to be fixed:
 
-class ManualEditStep(ReversibleStep):
-    edit_diff: EditDiff
-    hide: bool = True
+                {code}
 
-    hide: bool = True
+                This is what the code should be in order to avoid the problem:
+            """).format(traceback=self.traceback.full_traceback, code="{code}")
 
-    async def describe(self, llm: LLM) -> Coroutine[str, None, None]:
-        return "Manual edit step"
-        # TODO - only handling FileEdit here, but need all other types of FileSystemEdits
-        # Also requires the merge_file_edit function
-        # return llm.complete(dedent(f"""This code was replaced:
-
-        #     {self.edit_diff.backward.replacement}
-
-        #     With this code:
-
-        #     {self.edit_diff.forward.replacement}
-
-        #     Maximally concise summary of changes in bullet points (can use markdown):
-        # """))
-
-    @classmethod
-    def from_sequence(cls, edits: List[FileEditWithFullContents]) -> "ManualEditStep":
-        diffs = []
-        for edit in edits:
-            _, diff = FileSystem.apply_edit_to_str(
-                edit.fileContents, edit.fileEdit)
-            diffs.append(diff)
-        return cls(edit_diff=EditDiff.from_sequence(diffs))
+        range_in_files = []
+        for frame in self.traceback.frames:
+            content = await sdk.ide.readFile(frame.filepath)
+            range_in_files.append(
+                RangeInFile.from_entire_file(frame.filepath, content))
 
-    async def run(self, sdk: ContinueSDK) -> Coroutine[Observation, None, None]:
+        await sdk.run_step(EditCodeStep(
+            range_in_files=range_in_files, prompt=prompt))
         return None
 
-    async def reverse(self, sdk: ContinueSDK):
-        await sdk.ide.applyFileSystemEdit(self.edit_diff.backward)
-
 
-class UserInputStep(Step):
-    user_input: str
-    name: str = "User Input"
-    hide: bool = True
+class MessageStep(Step):
+    name: str = "Message"
+    message: str
 
-    async def describe(self, llm: LLM) -> Coroutine[str, None, None]:
-        return self.user_input
+    async def describe(self, models: Models) -> Coroutine[str, None, None]:
+        return self.message
 
-    async def run(self, sdk: ContinueSDK) -> Coroutine[UserInputObservation, None, None]:
-        return UserInputObservation(user_input=self.user_input)
-
-
-class ValidatorObservation(Observation):
-    passed: bool
-    observation: Observation
+    async def run(self, sdk: ContinueSDK) -> Coroutine[Observation, None, None]:
+        return TextObservation(text=self.message)
 
 
-class Validator(Step):
-    def run(self, sdk: ContinueSDK) -> ValidatorObservation:
-        raise NotImplementedError
+class EmptyStep(Step):
+    hide: bool = True
 
+    async def describe(self, models: Models) -> Coroutine[str, None, None]:
+        return ""
 
-HistoryNode.update_forward_refs()
+    async def run(self, sdk: ContinueSDK) -> Coroutine[Observation, None, None]:
+        pass
```

### Comparing `continuedev-0.1.0/src/continuedev/libs/llm/__init__.py` & `continuedev-0.1.1/src/continuedev/libs/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `continuedev-0.1.0/src/continuedev/libs/llm/hugging_face.py` & `continuedev-0.1.1/src/continuedev/libs/llm/hugging_face.py`

 * *Files identical despite different names*

### Comparing `continuedev-0.1.0/src/continuedev/libs/llm/openai.py` & `continuedev-0.1.1/src/continuedev/libs/llm/openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import time
 from typing import Any, Dict, Generator, List, Union
 import openai
 import aiohttp
 from ..llm import LLM
 from pydantic import BaseModel, validator
 
+DEFAULT_MAX_TOKENS = 2048
+
 
 class OpenAI(LLM):
     api_key: str
     completion_count: int = 0
     default_model: str = "text-davinci-003"
 
     @validator("api_key", pre=True, always=True)
@@ -18,15 +20,15 @@
         return v
 
     def with_system_message(self, system_message: Union[str, None]):
         return OpenAI(api_key=self.api_key, system_message=system_message)
 
     def stream_chat(self, messages, **kwargs) -> Generator[Union[Any, List, Dict], None, None]:
         self.completion_count += 1
-        args = {"max_tokens": 512, "temperature": 0.5, "top_p": 1,
+        args = {"max_tokens": DEFAULT_MAX_TOKENS, "temperature": 0.5, "top_p": 1,
                 "frequency_penalty": 0, "presence_penalty": 0} | kwargs
         args["stream"] = True
         args["model"] = "gpt-3.5-turbo"
 
         for chunk in openai.ChatCompletion.create(
             messages=messages,
             **args,
@@ -34,15 +36,15 @@
             if "content" in chunk.choices[0].delta:
                 yield chunk.choices[0].delta.content
             else:
                 continue
 
     def stream_complete(self, prompt: str, **kwargs) -> Generator[Union[Any, List, Dict], None, None]:
         self.completion_count += 1
-        args = {"model": self.default_model, "max_tokens": 512, "temperature": 0.5,
+        args = {"model": self.default_model, "max_tokens": DEFAULT_MAX_TOKENS, "temperature": 0.5,
                 "top_p": 1, "frequency_penalty": 0, "presence_penalty": 0, "suffix": None} | kwargs
         args["stream"] = True
 
         if args["model"] == "gpt-3.5-turbo":
             generator = openai.ChatCompletion.create(
                 messages=[{
                     "role": "user",
@@ -60,15 +62,15 @@
             for chunk in generator:
                 yield chunk.choices[0].text
 
     def complete(self, prompt: str, **kwargs) -> str:
         t1 = time.time()
 
         self.completion_count += 1
-        args = {"model": self.default_model, "max_tokens": 512, "temperature": 0.5, "top_p": 1,
+        args = {"model": self.default_model, "max_tokens": DEFAULT_MAX_TOKENS, "temperature": 0.5, "top_p": 1,
                 "frequency_penalty": 0, "presence_penalty": 0, "stream": False} | kwargs
 
         if args["model"] == "gpt-3.5-turbo":
             messages = [{
                 "role": "user",
                 "content": prompt
             }]
@@ -128,15 +130,15 @@
 
                 return await asyncio.gather(*tasks)
 
         return asyncio.run(fn())
 
     def parallel_complete(self, prompts: list[str], suffixes: Union[list[str], None] = None, **kwargs) -> list[str]:
         self.completion_count += len(prompts)
-        args = {"model": self.default_model, "max_tokens": 512, "temperature": 0.5,
+        args = {"model": self.default_model, "max_tokens": DEFAULT_MAX_TOKENS, "temperature": 0.5,
                 "top_p": 1, "frequency_penalty": 0, "presence_penalty": 0} | kwargs
 
         async def fn():
             async with aiohttp.ClientSession() as session:
                 tasks = []
 
                 async def get(prompt, suffix):
```

### Comparing `continuedev-0.1.0/src/continuedev/libs/llm/prompt_utils.py` & `continuedev-0.1.1/src/continuedev/libs/llm/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `continuedev-0.1.0/src/continuedev/libs/llm/prompters.py` & `continuedev-0.1.1/src/continuedev/libs/llm/prompters.py`

 * *Files identical despite different names*

### Comparing `continuedev-0.1.0/src/continuedev/libs/llm/utils.py` & `continuedev-0.1.1/src/continuedev/libs/llm/utils.py`

 * *Files identical despite different names*

### Comparing `continuedev-0.1.0/src/continuedev/libs/observation.py` & `continuedev-0.1.1/src/continuedev/core/observation.py`

 * *Files identical despite different names*

### Comparing `continuedev-0.1.0/src/continuedev/libs/policy.py` & `continuedev-0.1.1/src/continuedev/core/policy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from typing import List, Tuple, Type
 
-from .steps.ty import CreatePipelineStep
-from .core import Step, Validator, Policy, History
+from ..libs.steps.steps_on_startup import StepsOnStartupStep
+from ..libs.steps.draft.dlt import CreatePipelineStep
+from .main import Step, Validator, History, Policy
 from .observation import Observation, TracebackObservation, UserInputObservation
-from .steps.main import EditCodeStep, EditHighlightedCodeStep, SolveTracebackStep, RunCodeStep, FasterEditHighlightedCodeStep
-from .steps.nate import WritePytestsStep, CreateTableStep
-from .steps.chroma import AnswerQuestionChroma, EditFileChroma
+from ..libs.steps.main import EditHighlightedCodeStep, SolveTracebackStep, RunCodeStep, FasterEditHighlightedCodeStep, StarCoderEditHighlightedCodeStep, MessageStep, EmptyStep
+from ..libs.steps.nate import WritePytestsStep, CreateTableStep
+# from ..libs.steps.chroma import AnswerQuestionChroma, EditFileChroma
+from ..libs.steps.continue_step import ContinueStepStep
 
 
 class DemoPolicy(Policy):
     ran_code_last: bool = False
-    cmd: str
 
     def next(self, history: History) -> Step:
-        observation = history.last_observation()
+        # At the very start, run initial Steps spcecified in the config
+        if history.get_current() is None:
+            return MessageStep(message="Welcome to Continue!") >> StepsOnStartupStep()
+
+        observation = history.get_current().observation
         if observation is not None and isinstance(observation, UserInputObservation):
             # This could be defined with ObservationTypePolicy. Ergonomics not right though.
             if " test" in observation.user_input.lower():
                 return WritePytestsStep(instructions=observation.user_input)
             elif "/dlt" in observation.user_input.lower() or " dlt" in observation.user_input.lower():
                 return CreatePipelineStep()
             elif "/table" in observation.user_input:
                 return CreateTableStep(sql_str=" ".join(observation.user_input.split(" ")[1:]))
-            elif "/ask" in observation.user_input:
-                return AnswerQuestionChroma(question=" ".join(observation.user_input.split(" ")[1:]))
-            elif "/edit" in observation.user_input:
-                return EditFileChroma(request=" ".join(observation.user_input.split(" ")[1:]))
-            return EditHighlightedCodeStep(user_input=observation.user_input)
+            # elif "/ask" in observation.user_input:
+            #     return AnswerQuestionChroma(question=" ".join(observation.user_input.split(" ")[1:]))
+            # elif "/edit" in observation.user_input:
+            #     return EditFileChroma(request=" ".join(observation.user_input.split(" ")[1:]))
+            elif "/step" in observation.user_input:
+                return ContinueStepStep(prompt=" ".join(observation.user_input.split(" ")[1:]))
+            return StarCoderEditHighlightedCodeStep(user_input=observation.user_input)
 
         state = history.get_current()
-        if state is None or not self.ran_code_last:
-            self.ran_code_last = True
-            return RunCodeStep(cmd=self.cmd)
 
         if observation is not None and isinstance(observation, TracebackObservation):
             self.ran_code_last = False
             return SolveTracebackStep(traceback=observation.traceback)
         else:
             return None
```

### Comparing `continuedev-0.1.0/src/continuedev/libs/steps/chroma.py` & `continuedev-0.1.1/src/continuedev/libs/steps/chroma.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from textwrap import dedent
 from typing import Coroutine, Union
-from ...models.filesystem_edit import AddDirectory, AddFile
-from ..observation import Observation, TextObservation
-from ..core import Step, ContinueSDK
-from .main import EditCodeStep, EditFileStep, RunCommandStep, WaitForUserConfirmationStep
+from ...core.observation import Observation, TextObservation
+from ...core.main import Step, ContinueSDK
+from .core.core import EditFileStep
 from ..chroma.query import query_codebase_index
-from .main import EditFileStep
+from .core.core import EditFileStep
 
 
 class AnswerQuestionChroma(Step):
     question: str
     _answer: Union[str, None] = None
     name: str = "Answer Question"
 
@@ -37,15 +36,15 @@
 
             Here is the question to answer:
 
             {self.question}
 
             Here is the answer:""")
 
-        answer = sdk.llm.complete(prompt)
+        answer = (await sdk.models.gpt35()).complete(prompt)
         print(answer)
         self._answer = answer
 
         await sdk.ide.setFileOpen(files[0])
 
 
 class EditFileChroma(Step):
```

### Comparing `continuedev-0.1.0/src/continuedev/libs/steps/draft/abstract_method.py` & `continuedev-0.1.1/src/continuedev/libs/steps/draft/abstract_method.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from ...core import ContinueSDK, Step
+from ....core.sdk import ContinueSDK
+from ....core.main import Step
 
 
 class ImplementAbstractMethodStep(Step):
     name: str = "Implement abstract method for all subclasses"
     method_name: str
     class_name: str
```

### Comparing `continuedev-0.1.0/src/continuedev/libs/steps/draft/redux.py` & `continuedev-0.1.1/src/continuedev/libs/steps/draft/redux.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from textwrap import dedent
-from ....models.filesystem_edit import AddFile
-from ...core import Step, ContinueSDK
-from ..main import WaitForUserInputStep, EditFileStep
+from ....core.main import Step
+from ....core.sdk import ContinueSDK
+from ..core.core import EditFileStep
 
 
 class EditReduxStateStep(Step):
 
     description: str  # e.g. "I want to load data from the weatherapi.com API"
 
     async def run(self, sdk: ContinueSDK):
```

### Comparing `continuedev-0.1.0/src/continuedev/libs/steps/draft/typeorm.py` & `continuedev-0.1.1/src/continuedev/libs/steps/draft/typeorm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from textwrap import dedent
-from ...core import Step, ContinueSDK
+from ....core.main import Step
+from ....core.sdk import ContinueSDK
 
 
 class CreateTableStep(Step):
     sql_str: str
     name: str = "Create a table in TypeORM"
 
     async def run(self, sdk: ContinueSDK):
```

### Comparing `continuedev-0.1.0/src/continuedev/libs/steps/migration.py` & `continuedev-0.1.1/src/continuedev/libs/steps/migration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # When an edit is made to an existing class or a new sqlalchemy class is created,
 # this should be kicked off.
 
 from ...models.filesystem import RangeInFile
 from .main import EditCodeStep, RunCommandStep
-from ..core import Step
+from ...core.main import Step
 
 
 class MigrationStep(Step):
     name: str = "Create and run an alembic migration."
 
     edited_file: str
 
     async def run(self, sdk):
         recent_edits = await sdk.ide.get_recent_edits(self.edited_file)
         recent_edits_string = "\n\n".join(
             map(lambda x: x.to_string(), recent_edits))
-        description = await sdk.llm.complete(f"{recent_edits_string}\n\nGenerate a short description of the migration made in the above changes:\n")
+        description = await (await sdk.models.gpt35()).complete(f"{recent_edits_string}\n\nGenerate a short description of the migration made in the above changes:\n")
         await sdk.run_step(RunCommandStep(cmd=f"cd libs && poetry run alembic revision --autogenerate -m {description}"))
         migration_file = f"libs/alembic/versions/{?}.py"
         contents = await sdk.ide.readFile(migration_file)
         await sdk.run_step(EditCodeStep(
             range_in_files=[RangeInFile.from_entire_file(migration_file, contents)],
             prompt=f"Here are the changes made to the sqlalchemy classes:\n\n{recent_edits_string}\n\nThis is the generated migration file:\n\n{{code}}\n\nReview the migration file to make sure it correctly reflects the changes made to the sqlalchemy classes.",
         ))
```

### Comparing `continuedev-0.1.0/src/continuedev/libs/steps/nate.py` & `continuedev-0.1.1/src/continuedev/libs/steps/nate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import asyncio
 from textwrap import dedent
 import time
 from typing import Coroutine, Union
 
-from ...models.main import Range
 from ...models.filesystem import RangeInFile
 from ...models.filesystem_edit import AddDirectory, AddFile
-from ..observation import Observation, TextObservation
-from ..core import Step, ContinueSDK
-from .main import EditCodeStep, EditFileStep, RunCommandStep, WaitForUserConfirmationStep
+from ...core.observation import Observation, TextObservation
+from ...core.main import Step, ContinueSDK
+from .main import RunCommandStep
+from .core.core import WaitForUserConfirmationStep, EditCodeStep, EditFileStep
 import os
 
 
 class WritePytestsStep(Step):
     for_filepath: Union[str, None] = None
     instructions: str = "Write unit tests for this file."
 
@@ -42,15 +41,15 @@
 Here are additional instructions:
 
 "{self.instructions}"
 
 Here is a complete set of pytest unit tests:
 
         """)
-        # tests = sdk.llm.complete(prompt)
+        # tests = (await sdk.models.gpt35()).complete(prompt)
         tests = '''
 import pytest
 
 from ..calculator import Calculator
 
 
 @pytest.fixture
@@ -166,17 +165,17 @@
   @Column()
   order_status: string;
 
   @Column()
   tracking_number: string;
 }'''
         time.sleep(2)
-        # orm_entity = sdk.llm.complete(
+        # orm_entity = (await sdk.models.gpt35()).complete(
         #     f"{self.sql_str}\n\nWrite a TypeORM entity called {entity_name} for this table, importing as necessary:")
-        # sdk.llm.complete("What is the name of the entity?")
+        # (await sdk.models.gpt35()).complete("What is the name of the entity?")
         await sdk.apply_filesystem_edit(AddFile(filepath=f"/Users/natesesti/Desktop/continue/extension/examples/python/MyProject/src/entity/{entity_name}.ts", content=orm_entity))
         await sdk.ide.setFileOpen(f"/Users/natesesti/Desktop/continue/extension/examples/python/MyProject/src/entity/{entity_name}.ts", True)
 
         # Add entity to data-source.ts
         await sdk.run_step(EditFileStep(
             filepath=f"/Users/natesesti/Desktop/continue/extension/examples/python/MyProject/src/data-source.ts",
             prompt=f"{{code}}\nAdd the {entity_name} entity:\n",
```

### Comparing `continuedev-0.1.0/src/continuedev/libs/steps/pytest.py` & `continuedev-0.1.1/src/continuedev/libs/steps/pytest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from textwrap import dedent
 from ...models.filesystem_edit import AddDirectory, AddFile
-from ..core import Step, ContinueSDK
+from ...core.main import Step, ContinueSDK
 import os
 
 
 class WritePytestsStep(Step):
     for_filepath: str
 
     async def run(self, sdk: ContinueSDK):
@@ -29,9 +29,9 @@
 
             Here are additional instructions:
 
             "{self.instructions}"
 
             Here is a complete set of pytest unit tests:
         """)
-        tests = sdk.llm.complete(prompt)
+        tests = (await sdk.models.gpt35()).complete(prompt)
         await sdk.apply_filesystem_edit(AddFile(filepath=path, content=tests))
```

### Comparing `continuedev-0.1.0/src/continuedev/libs/steps/ty.py` & `continuedev-0.1.1/src/continuedev/libs/steps/ty.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import subprocess
 from ...models.main import Position, Range
 from ...models.filesystem import RangeInFile
 from ...models.filesystem_edit import AddDirectory, AddFile, FileEdit
-from ..observation import DictObservation
-from ..core import History, Step, ContinueSDK, Policy
-from .main import EditCodeStep, RunCommandStep, WaitForUserInputStep, WaitForUserConfirmationStep
+from ...core.observation import DictObservation
+from ...core.main import History, Step, Policy
+from ...core.sdk import ContinueSDK
+from .main import RunCommandStep
+from ..steps.core.core import EditCodeStep, WaitForUserConfirmationStep, WaitForUserInputStep
 
 source_name = "weather_api"
 
 
 class SetupPipelineStep(Step):
 
     name = "Setup Pipeline"
 
     api_description: str  # e.g. "I want to load data from the weatherapi.com API"
 
     async def run(self, sdk: ContinueSDK):
-        # source_name = sdk.llm.complete(
+        # source_name = (await sdk.models.gpt35()).complete(
         #     f"Write a snake_case name for the data source described by {self.api_description}: ").strip()
         filename = f'/Users/natesesti/Desktop/continue/extension/examples/python/{source_name}.py'
 
         # running commands to get started when creating a new dlt pipeline
         process = subprocess.Popen(
             '/bin/bash', stdin=subprocess.PIPE, stdout=subprocess.PIPE)
         out, err = process.communicate(f'''
```

### Comparing `continuedev-0.1.0/src/continuedev/libs/util/copy_codebase.py` & `continuedev-0.1.1/src/continuedev/libs/util/copy_codebase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from pathlib import Path
 from typing import Iterable, List, Union
 from watchdog.observers import Observer
 from watchdog.events import PatternMatchingEventHandler
 from ..models.main import FileEdit, DeleteDirectory, DeleteFile, AddDirectory, AddFile, FileSystemEdit, Position, Range, RenameFile, RenameDirectory, SequentialFileSystemEdit
 from ..models.filesystem import FileSystem
-from ..libs.main import Agent
+from ..libs.main import Autopilot
 from ..libs.map_path import map_path
 from ..libs.steps.main import ManualEditAction
 import shutil
 import difflib
 
 
 def create_copy(orig_root: str, copy_root: str = None, ignore: Iterable[str] = []):
@@ -61,23 +61,23 @@
             raise Exception("Unexpected difflib.SequenceMatcher tag: " + tag)
 
     return edits
 
 
 # The whole usage of watchdog here should only be specific to RealFileSystem, you want to have a different "Observer" class for VirtualFileSystem, which would depend on being sent notifications
 class CopyCodebaseEventHandler(PatternMatchingEventHandler):
-    def __init__(self, ignore_directories: List[str], ignore_patterns: List[str], agent: Agent, orig_root: str, copy_root: str, filesystem: FileSystem):
+    def __init__(self, ignore_directories: List[str], ignore_patterns: List[str], autopilot: Autopilot, orig_root: str, copy_root: str, filesystem: FileSystem):
         super().__init__(ignore_directories=ignore_directories, ignore_patterns=ignore_patterns)
-        self.agent = agent
+        self.autopilot = autopilot
         self.orig_root = orig_root
         self.copy_root = copy_root
         self.filesystem = filesystem
 
-    # For now, we'll just make the update immediately, but eventually need to sync with agent.
-    # It should be the agent that makes the update right? It's just another action, everything comes from a single stream.
+    # For now, we'll just make the update immediately, but eventually need to sync with autopilot.
+    # It should be the autopilot that makes the update right? It's just another action, everything comes from a single stream.
 
     def _event_to_edit(self, event) -> Union[FileSystemEdit, None]:
         # NOTE: You'll need to map paths to create both an action within the copy filesystem (the one you take) and one in the original fileystem (the one you'll record and allow the user to accept). Basically just need a converter built in to the FileSystemEdit class
         src = event.src_path()
         if event.is_directory:
             if event.event_type == "moved":
                 return RenameDirectory(src, event.dest_path())
@@ -106,21 +106,21 @@
 
     def on_any_event(self, event):
         edit = self._event_to_edit(event)
         if edit is None:
             return
         edit = edit.with_mapped_paths(self.orig_root, self.copy_root)
         action = ManualEditAction(edit)
-        self.agent.act(action)
+        self.autopilot.act(action)
 
 
-def maintain_copy_workspace(agent: Agent, filesystem: FileSystem, orig_root: str, copy_root: str):
+def maintain_copy_workspace(autopilot: Autopilot, filesystem: FileSystem, orig_root: str, copy_root: str):
     observer = Observer()
     event_handler = CopyCodebaseEventHandler(
-        [".git"], [], agent, orig_root, copy_root, filesystem)
+        [".git"], [], autopilot, orig_root, copy_root, filesystem)
     observer.schedule(event_handler, orig_root, recursive=True)
     observer.start()
     try:
         while observer.isAlive():
             observer.join(1)
     finally:
         observer.stop()
```

### Comparing `continuedev-0.1.0/src/continuedev/libs/util/queue.py` & `continuedev-0.1.1/src/continuedev/libs/util/queue.py`

 * *Files identical despite different names*

### Comparing `continuedev-0.1.0/src/continuedev/libs/util/traceback_parsers.py` & `continuedev-0.1.1/src/continuedev/libs/util/traceback_parsers.py`

 * *Files identical despite different names*

### Comparing `continuedev-0.1.0/src/continuedev/models/filesystem.py` & `continuedev-0.1.1/src/continuedev/models/filesystem.py`

 * *Files identical despite different names*

### Comparing `continuedev-0.1.0/src/continuedev/models/filesystem_edit.py` & `continuedev-0.1.1/src/continuedev/models/filesystem_edit.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,18 @@
     def from_deletion(filepath: str, start: Position, end: Position) -> "FileEdit":
         return FileEdit(filepath, Range(start, end), "")
 
     @staticmethod
     def from_insertion(filepath: str, position: Position, content: str) -> "FileEdit":
         return FileEdit(filepath=filepath, range=Range.from_shorthand(position.line, position.character, position.line, position.character), replacement=content)
 
+    @staticmethod
+    def from_append(filepath: str, previous_content: str, appended_content: str) -> "FileEdit":
+        return FileEdit(filepath=filepath, range=Range.from_position(Position.from_end_of_file(previous_content)), replacement=appended_content)
+
 
 class FileEditWithFullContents(BaseModel):
     fileEdit: FileEdit
     fileContents: str
 
 
 class AddFile(AtomicFileSystemEdit):
```

### Comparing `continuedev-0.1.0/src/continuedev/models/generate_json_schema.py` & `continuedev-0.1.1/src/continuedev/models/generate_json_schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 from .main import *
 from .filesystem import RangeInFile, FileEdit
 from .filesystem_edit import FileEditWithFullContents
+from ..core.main import History, HistoryNode
 from pydantic import schema_json_of
 import os
 
 MODELS_TO_GENERATE = [
     Position, Range, Traceback, TracebackFrame
 ] + [
     RangeInFile, FileEdit
 ] + [
     FileEditWithFullContents
+] + [
+    History, HistoryNode
 ]
 
 RENAMES = {
     "ExampleClass": "RenamedName"
 }
 
-SCHEMA_DIR = "schema/json"
+SCHEMA_DIR = "../schema/json"
 
 
 def clear_schemas():
     for filename in os.listdir(SCHEMA_DIR):
         if filename.endswith(".json"):
             os.remove(os.path.join(SCHEMA_DIR, filename))
 
 
-if __name__ == "__main__":
+def main():
     clear_schemas()
     for model in MODELS_TO_GENERATE:
         title = RENAMES.get(model.__name__, model.__name__)
         try:
             json = schema_json_of(model, indent=2, title=title)
         except Exception as e:
             print(f"Failed to generate json schema for {title}: ", e)
             continue
 
         with open(f"{SCHEMA_DIR}/{title}.json", "w") as f:
             f.write(json)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `continuedev-0.1.0/src/continuedev/models/main.py` & `continuedev-0.1.1/src/continuedev/models/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from abc import ABC
 from typing import List, Union
 from pydantic import BaseModel, root_validator
 from functools import total_ordering
 
 
+class ContinueBaseModel(BaseModel):
+    class Config:
+        underscore_attrs_are_private = True
+
+
 @total_ordering
 class Position(BaseModel):
     line: int
     character: int
 
     def __hash__(self):
         return hash((self.line, self.character))
@@ -23,21 +28,25 @@
         else:
             return False
 
     @staticmethod
     def from_index(string: str, index: int) -> "Position":
         """Convert index in string to line and character"""
         line = string.count("\n", 0, index)
-        if line == 1:
+        if line == 0:
             character = index
         else:
             character = index - string.rindex("\n", 0, index) - 1
 
         return Position(line=line, character=character)
 
+    @staticmethod
+    def from_end_of_file(contents: str) -> "Position":
+        return Position.from_index(contents, len(contents))
+
 
 class Range(BaseModel):
     """A range in a file. 0-indexed."""
     start: Position
     end: Position
 
     def __hash__(self):
@@ -84,14 +93,42 @@
 
     @staticmethod
     def from_snippet_in_file(content: str, snippet: str) -> "Range":
         start_index = content.index(snippet)
         end_index = start_index + len(snippet)
         return Range.from_indices(content, start_index, end_index)
 
+    @staticmethod
+    def from_lines_snippet_in_file(content: str, snippet: str) -> "Range":
+        # lines is a substring of the content modulo whitespace on each line
+        content_lines = content.splitlines()
+        snippet_lines = snippet.splitlines()
+
+        start_line = -1
+        end_line = -1
+        looking_for_line = 0
+        for i in range(len(content_lines)):
+            if content_lines[i].strip() == snippet_lines[looking_for_line].strip():
+                if looking_for_line == len(snippet_lines) - 1:
+                    start_line = i - len(snippet_lines) + 1
+                    end_line = i
+                    break
+                looking_for_line += 1
+            else:
+                looking_for_line = 0
+
+        if start_line == -1 or end_line == -1:
+            raise ValueError("Snippet not found in content")
+
+        return Range.from_shorthand(start_line, 0, end_line, len(content_lines[end_line]) - 1)
+
+    @staticmethod
+    def from_position(position: Position) -> "Range":
+        return Range(start=position, end=position)
+
 
 class AbstractModel(ABC, BaseModel):
     @root_validator(pre=True)
     def check_is_subclass(cls, values):
         if not issubclass(cls, AbstractModel):
             raise TypeError(
                 "AbstractModel subclasses must be subclasses of AbstractModel")
```

### Comparing `continuedev-0.1.0/src/continuedev/server/ide.py` & `continuedev-0.1.1/src/continuedev/server/ide.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # This is a separate server from server/main.py
 import asyncio
+import json
 import os
 from typing import Any, Dict, List, Type, TypeVar, Union
 import uuid
 from fastapi import WebSocket, Body, APIRouter
 from uvicorn.main import Server
 
 from ..libs.util.queue import AsyncSubscriptionQueue
 from ..models.filesystem import FileSystem, RangeInFile, EditDiff, RealFileSystem
 from ..models.main import Traceback
 from ..models.filesystem_edit import AddDirectory, AddFile, DeleteDirectory, DeleteFile, FileSystemEdit, FileEdit, FileEditWithFullContents, RenameDirectory, RenameFile, SequentialFileSystemEdit
 from pydantic import BaseModel
-from .notebook import SessionManager, session_manager
+from .gui import SessionManager, session_manager
 from .ide_protocol import AbstractIdeProtocolServer
 
 
 router = APIRouter(prefix="/ide", tags=["ide"])
 
 
 # Graceful shutdown by closing websockets
@@ -86,104 +87,103 @@
     websocket: WebSocket
     session_manager: SessionManager
     sub_queue: AsyncSubscriptionQueue = AsyncSubscriptionQueue()
 
     def __init__(self, session_manager: SessionManager):
         self.session_manager = session_manager
 
-    async def _send_json(self, data: Any):
-        await self.websocket.send_json(data)
+    async def _send_json(self, message_type: str, data: Any):
+        await self.websocket.send_json({
+            "messageType": message_type,
+            "data": data
+        })
 
     async def _receive_json(self, message_type: str) -> Any:
         return await self.sub_queue.get(message_type)
 
     async def _send_and_receive_json(self, data: Any, resp_model: Type[T], message_type: str) -> T:
-        await self._send_json(data)
+        await self._send_json(message_type, data)
         resp = await self._receive_json(message_type)
         return resp_model.parse_obj(resp)
 
-    async def handle_json(self, data: Any):
-        t = data["messageType"]
-        if t == "openNotebook":
-            await self.openNotebook()
-        elif t == "setFileOpen":
+    async def handle_json(self, message_type: str, data: Any):
+        if message_type == "openGUI":
+            await self.openGUI()
+        elif message_type == "setFileOpen":
             await self.setFileOpen(data["filepath"], data["open"])
-        elif t == "fileEdits":
+        elif message_type == "fileEdits":
             fileEdits = list(
                 map(lambda d: FileEditWithFullContents.parse_obj(d), data["fileEdits"]))
             self.onFileEdits(fileEdits)
-        elif t in ["highlightedCode", "openFiles", "readFile", "editFile", "workspaceDirectory"]:
-            self.sub_queue.post(t, data)
+        elif message_type in ["highlightedCode", "openFiles", "readFile", "editFile", "workspaceDirectory"]:
+            self.sub_queue.post(message_type, data)
         else:
-            raise ValueError("Unknown message type", t)
+            raise ValueError("Unknown message type", message_type)
 
     # ------------------------------- #
     # Request actions in IDE, doesn't matter which Session
     def showSuggestion():
         pass
 
     async def setFileOpen(self, filepath: str, open: bool = True):
-        # Agent needs access to this.
-        await self.websocket.send_json({
-            "messageType": "setFileOpen",
+        # Autopilot needs access to this.
+        await self._send_json("setFileOpen", {
             "filepath": filepath,
             "open": open
         })
 
-    async def openNotebook(self):
+    async def openGUI(self):
         session_id = self.session_manager.new_session(self)
-        await self._send_json({
-            "messageType": "openNotebook",
+        await self._send_json("openGUI", {
             "sessionId": session_id
         })
 
     async def showSuggestionsAndWait(self, suggestions: List[FileEdit]) -> bool:
         ids = [str(uuid.uuid4()) for _ in suggestions]
         for i in range(len(suggestions)):
-            self._send_json({
-                "messageType": "showSuggestion",
+            self._send_json("showSuggestion", {
                 "suggestion": suggestions[i],
                 "suggestionId": ids[i]
             })
         responses = await asyncio.gather(*[
             self._receive_json(ShowSuggestionResponse)
             for i in range(len(suggestions))
-        ])  # WORKING ON THIS FLOW HERE. Fine now to just await for response, instead of doing something fancy with a "waiting" state on the agent.
-        # Just need connect the suggestionId to the IDE (and the notebook)
+        ])  # WORKING ON THIS FLOW HERE. Fine now to just await for response, instead of doing something fancy with a "waiting" state on the autopilot.
+        # Just need connect the suggestionId to the IDE (and the gui)
         return any([r.accepted for r in responses])
 
     # ------------------------------- #
-    # Here needs to pass message onto the Agent OR Agent just subscribes.
+    # Here needs to pass message onto the Autopilot OR Autopilot just subscribes.
     # This is where you might have triggers: plugins can subscribe to certian events
     # like file changes, tracebacks, etc...
 
     def onAcceptRejectSuggestion(self, suggestionId: str, accepted: bool):
         pass
 
     def onTraceback(self, traceback: Traceback):
-        # Same as below, maybe not every agent?
+        # Same as below, maybe not every autopilot?
         for _, session in self.session_manager.sessions.items():
-            session.agent.handle_traceback(traceback)
+            session.autopilot.handle_traceback(traceback)
 
     def onFileSystemUpdate(self, update: FileSystemEdit):
-        # Access to Agent (so SessionManager)
+        # Access to Autopilot (so SessionManager)
         pass
 
-    def onCloseNotebook(self, session_id: str):
+    def onCloseGUI(self, session_id: str):
         # Accesss to SessionManager
         pass
 
-    def onOpenNotebookRequest(self):
+    def onOpenGUIRequest(self):
         pass
 
     def onFileEdits(self, edits: List[FileEditWithFullContents]):
-        # Send the file edits to ALL agents.
+        # Send the file edits to ALL autopilots.
         # Maybe not ideal behavior
         for _, session in self.session_manager.sessions.items():
-            session.agent.handle_manual_edits(edits)
+            session.autopilot.handle_manual_edits(edits)
 
     # Request information. Session doesn't matter.
     async def getOpenFiles(self) -> List[str]:
         resp = await self._send_and_receive_json({
             "messageType": "openFiles"
         }, OpenFilesResponse, "openFiles")
         return resp.openFiles
@@ -206,16 +206,15 @@
             "messageType": "readFile",
             "filepath": filepath
         }, ReadFileResponse, "readFile")
         return resp.contents
 
     async def saveFile(self, filepath: str):
         """Save a file"""
-        await self._send_json({
-            "messageType": "saveFile",
+        await self._send_json("saveFile", {
             "filepath": filepath
         })
 
     async def readRangeInFile(self, range_in_file: RangeInFile) -> str:
         """Read a range in a file"""
         full_contents = await self.readFile(range_in_file.filepath)
         return FileSystem.read_range_in_str(full_contents, range_in_file.range)
@@ -289,14 +288,21 @@
 ideProtocolServer = IdeProtocolServer(session_manager)
 
 
 @router.websocket("/ws")
 async def websocket_endpoint(websocket: WebSocket):
     await websocket.accept()
     print("Accepted websocket connection from, ", websocket.client)
-    await websocket.send_json({"messageType": "connected"})
+    await websocket.send_json({"messageType": "connected", "data": {}})
     ideProtocolServer.websocket = websocket
     while True:
-        data = await websocket.receive_json()
-        await ideProtocolServer.handle_json(data)
+        message = await websocket.receive_text()
+        message = json.loads(message)
+
+        if "messageType" not in message or "data" not in message:
+            continue
+        message_type = message["messageType"]
+        data = message["data"]
+
+        await ideProtocolServer.handle_json(message_type, data)
 
     await websocket.close()
```

### Comparing `continuedev-0.1.0/src/continuedev/server/ide_protocol.py` & `continuedev-0.1.1/src/continuedev/server/ide_protocol.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         """Get the workspace directory"""
 
     @abstractmethod
     async def setFileOpen(self, filepath: str, open: bool = True):
         """Set whether a file is open"""
 
     @abstractmethod
-    async def openNotebook(self):
-        """Open a notebook"""
+    async def openGUI(self):
+        """Open a GUI"""
 
     @abstractmethod
     async def showSuggestionsAndWait(self, suggestions: List[FileEdit]) -> bool:
         """Show suggestions to the user and wait for a response"""
 
     @abstractmethod
     def onAcceptRejectSuggestion(self, suggestionId: str, accepted: bool):
@@ -40,20 +40,20 @@
         """Called when a traceback is received"""
 
     @abstractmethod
     def onFileSystemUpdate(self, update: FileSystemEdit):
         """Called when a file system update is received"""
 
     @abstractmethod
-    def onCloseNotebook(self, session_id: str):
-        """Called when a notebook is closed"""
+    def onCloseGUI(self, session_id: str):
+        """Called when a GUI is closed"""
 
     @abstractmethod
-    def onOpenNotebookRequest(self):
-        """Called when a notebook is requested to be opened"""
+    def onOpenGUIRequest(self):
+        """Called when a GUI is requested to be opened"""
 
     @abstractmethod
     async def getOpenFiles(self) -> List[str]:
         """Get a list of open files"""
 
     @abstractmethod
     async def getHighlightedCode(self) -> List[RangeInFile]:
```

### Comparing `continuedev-0.1.0/PKG-INFO` & `continuedev-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 Metadata-Version: 2.1
 Name: continuedev
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Nate Sesti
 Author-email: sestinj@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boltons (>=23.0.0,<24.0.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: gpt-index (>=0.6.8,<0.7.0)
 Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
+Requires-Dist: posthog (>=3.0.1,<4.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: setuptools (>=67.7.2,<68.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Requires-Dist: urllib3 (==1.26.15)
 Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
 Requires-Dist: websockets (>=11.0.2,<12.0.0)
 Description-Content-Type: text/markdown
 
-## Steps to start
+# Continue PyPI Package
 
-- `cd continue/continue`
+Continue is a Python library for automating repetitive sequences of software development tasks using language models. Using our VS Code extension, you can build, run, and refine these recipes as they natively interact with your codebase. Download on [our GitHub](https://github.com/continuedev/continue).
+
+## Continue Server
+
+The Continue server acts as a bridge between the Continue React app and your IDE, running your recipes and acting on the codebase. Start it by running the following commands:
+
+- `cd continuedev`
 - Make sure packages are installed with `poetry install`
 - `poetry shell`
 - `cd ..`
-- `python3 -m continuedev.src.continuedev`
-
-## Steps to generate JSON Schema
+- `python3 -m continuedev.src.continuedev.server.main`
 
-Same up until last step and then `python3 -m continuedev.src.scripts.gen_json_schema`.
+## Scripts
 
-## Start the server
+`poetry run typegen` to generate JSONSchema .json files from the Pydantic types defined in the `models` directory.
 
-Same steps, then `uvicorn continue.src.server.main:app --reload`.
+`poetry build` will output wheel and tarball files in `./dist`.
 
-## To build
+## Writing Steps
 
-Run `poetry build` and it will output wheel and tarball files in `./dist`.
+See the `src/continuedev/libs/steps` folder for examples of writing a Continue step. See our documentation for tutorials.
```

