# Comparing `tmp/highlight_io-0.4.9.tar.gz` & `tmp/highlight_io-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highlight_io-0.4.9.tar", max compression
+gzip compressed data, was "highlight_io-0.5.0.tar", max compression
```

## Comparing `highlight_io-0.4.9.tar` & `highlight_io-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0      350 2023-03-06 07:22:47.581214 highlight_io-0.4.9/README.md
--rw-r--r--   0        0        0       64 2023-03-06 07:22:47.585934 highlight_io-0.4.9/highlight_io/__init__.py
--rw-r--r--   0        0        0      155 2023-03-06 07:22:47.586006 highlight_io-0.4.9/highlight_io/integrations/__init__.py
--rw-r--r--   0        0        0      717 2023-04-11 23:45:03.063104 highlight_io-0.4.9/highlight_io/integrations/aws.py
--rw-r--r--   0        0        0      740 2023-04-11 23:45:03.063208 highlight_io-0.4.9/highlight_io/integrations/azure.py
--rw-r--r--   0        0        0     1631 2023-03-06 07:22:47.586615 highlight_io-0.4.9/highlight_io/integrations/django.py
--rw-r--r--   0        0        0      722 2023-03-06 07:22:47.586847 highlight_io-0.4.9/highlight_io/integrations/fastapi.py
--rw-r--r--   0        0        0     1519 2023-03-06 07:22:47.586917 highlight_io-0.4.9/highlight_io/integrations/flask.py
--rw-r--r--   0        0        0      747 2023-04-11 23:45:03.063318 highlight_io-0.4.9/highlight_io/integrations/gcp.py
--rw-r--r--   0        0        0     1072 2023-04-11 23:45:03.063459 highlight_io-0.4.9/highlight_io/integrations/serverless.py
--rw-r--r--   0        0        0     6801 2023-04-19 17:13:56.388150 highlight_io-0.4.9/highlight_io/sdk.py
--rw-r--r--   0        0        0     1698 2023-05-23 20:14:18.490479 highlight_io-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 highlight_io-0.4.9/setup.py
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 highlight_io-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0      350 2023-06-03 00:42:53.945658 highlight_io-0.5.0/README.md
+-rw-r--r--   0        0        0       64 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/__init__.py
+-rw-r--r--   0        0        0      155 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/__init__.py
+-rw-r--r--   0        0        0      717 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/aws.py
+-rw-r--r--   0        0        0      740 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/azure.py
+-rw-r--r--   0        0        0     1631 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/django.py
+-rw-r--r--   0        0        0      722 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/fastapi.py
+-rw-r--r--   0        0        0     1519 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/flask.py
+-rw-r--r--   0        0        0      747 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/gcp.py
+-rw-r--r--   0        0        0     1072 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/serverless.py
+-rw-r--r--   0        0        0     7937 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/sdk.py
+-rw-r--r--   0        0        0     1716 2023-06-03 00:42:53.945658 highlight_io-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 highlight_io-0.5.0/PKG-INFO
```

### Comparing `highlight_io-0.4.9/highlight_io/integrations/aws.py` & `highlight_io-0.5.0/highlight_io/integrations/aws.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.9/highlight_io/integrations/azure.py` & `highlight_io-0.5.0/highlight_io/integrations/azure.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.9/highlight_io/integrations/django.py` & `highlight_io-0.5.0/highlight_io/integrations/django.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.9/highlight_io/integrations/fastapi.py` & `highlight_io-0.5.0/highlight_io/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.9/highlight_io/integrations/flask.py` & `highlight_io-0.5.0/highlight_io/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.9/highlight_io/integrations/gcp.py` & `highlight_io-0.5.0/highlight_io/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.9/highlight_io/integrations/serverless.py` & `highlight_io-0.5.0/highlight_io/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.9/highlight_io/sdk.py` & `highlight_io-0.5.0/highlight_io/sdk.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,35 @@
 from opentelemetry._logs.severity import std_to_otel
 from opentelemetry.exporter.otlp.proto.http import Compression
 from opentelemetry.exporter.otlp.proto.http._log_exporter import OTLPLogExporter
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
 from opentelemetry.instrumentation.logging import LoggingInstrumentor
 from opentelemetry.sdk._logs import LoggerProvider, LogRecord
 from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
-from opentelemetry.sdk.trace import TracerProvider, _Span
+from opentelemetry.sdk.trace import TracerProvider, Span
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 
 from highlight_io.integrations import Integration
 
 
+class LogHandler(logging.Handler):
+    def __init__(self, highlight: "H", level=logging.NOTSET):
+        self.highlight = highlight
+        super(LogHandler, self).__init__(level=level)
+
+    def emit(self, record: logging.LogRecord):
+        ctx = contextlib.nullcontext
+        span = trace.get_current_span()
+        if span is None or not span.is_recording():
+            ctx = self.highlight.trace
+
+        with ctx():
+            self.highlight.log_hook(trace.get_current_span(), record)
+
+
 class H(object):
     REQUEST_HEADER = "X-Highlight-Request"
     OTLP_HTTP = "https://otel.highlight.io:4318"
     _instance: "H" = None
 
     @classmethod
     def get_instance(cls) -> "H":
@@ -29,38 +44,39 @@
             )
         return cls._instance
 
     def __init__(
         self,
         project_id: str,
         integrations: typing.List[Integration] = None,
-        record_logs: bool = True,
         otlp_endpoint: str = "",
+        instrument_logging: bool = True,
+        log_level=logging.DEBUG,
     ):
         """
         Setup Highlight backend instrumentation.
 
         Example:
             import highlight_io
             H = highlight_io.H('project_id', ...)
 
 
         :param project_id: a string that corresponds to the verbose id of your project from app.highlight.io/setup
         :param integrations: a list of Integrations that allow connecting with your framework, like Flask or Django.
-        :param record_logs: defaults to True. set False if you want to disable python logging recording.
+        :param instrument_logging: defaults to True. set False to disable auto-instrumentation of python `logging` methods.
         :param otlp_endpoint: set to a custom otlp destination
         :return: a configured H instance
         """
         H._instance = self
         self._project_id = project_id
         self._integrations = integrations or []
-        self._record_logs = record_logs
         self._otlp_endpoint = otlp_endpoint or H.OTLP_HTTP
-        if self._record_logs:
-            self._instrument_logs()
+        self._log_handler = LogHandler(self, level=log_level)
+        if instrument_logging:
+            self._instrument_logging()
 
         self._trace_provider = TracerProvider()
         self._trace_provider.add_span_processor(
             BatchSpanProcessor(
                 OTLPSpanExporter(
                     f"{self._otlp_endpoint}/v1/traces", compression=Compression.Gzip
                 ),
@@ -150,15 +166,35 @@
         """
         span = trace.get_current_span()
         if not span:
             raise RuntimeError("H.record_exception called without a span context")
         span.record_exception(e)
         logging.exception("Highlight caught an error", exc_info=e)
 
-    def _log_hook(self, span: _Span, record: logging.LogRecord):
+    @property
+    def logging_handler(self) -> logging.Handler:
+        """A logging handler implementing `logging.Handler` that allows plugging highlight_io
+        into your existing logging setup.
+
+        Example:
+            import highlight_io
+            from loguru import logger
+
+            H = highlight_io.H('project_id', ...)
+
+            logger.add(
+                H.logging_handler,
+                format="{message}",
+                level="INFO",
+                backtrace=True,
+            )
+        """
+        return self._log_handler
+
+    def log_hook(self, span: Span, record: logging.LogRecord):
         if span and span.is_recording():
             ctx = span.get_span_context()
             # record.created is sec but timestamp should be ns
             ts = int(record.created * 1000.0 * 1000.0 * 1000.0)
             attributes = span.attributes.copy()
             attributes["code.function"] = record.funcName
             attributes["code.namespace"] = record.module
@@ -174,11 +210,11 @@
                 severity_number=std_to_otel(record.levelno),
                 body=record.getMessage(),
                 resource=span.resource,
                 attributes=attributes,
             )
             self.log.emit(r)
 
-    def _instrument_logs(self):
+    def _instrument_logging(self):
         LoggingInstrumentor().instrument(
-            set_logging_format=True, log_hook=self._log_hook
+            set_logging_format=True, log_hook=self.log_hook
         )
```

### Comparing `highlight_io-0.4.9/pyproject.toml` & `highlight_io-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highlight-io"
-version = "0.4.9"
+version = "0.5.0"
 description = "Session replay and error monitoring: stop guessing why bugs happen!"
 license = "Apache-2.0"
 authors = [
     "Vadim Korolik <vadim@highlight.io>",
     "Jay Khatri <jay@highlight.io>",
 ]
 readme = "README.md"
@@ -43,14 +43,15 @@
 azure-functions = "^1.13.2"
 black = "^23"
 functions-framework = "^3.3.0"
 pytest = "^7.2.1"
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.20.3"
+loguru = "^0.7.0"
 
 [tool.poetry.extras]
 Django = ["django"]
 FastAPI = ["fastapi", "uvicorn"]
 Flask = ["blinker", "flask"]
 
 [build-system]
```

### Comparing `highlight_io-0.4.9/PKG-INFO` & `highlight_io-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highlight-io
-Version: 0.4.9
+Version: 0.5.0
 Summary: Session replay and error monitoring: stop guessing why bugs happen!
 Home-page: https://www.highlight.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Vadim Korolik
 Author-email: vadim@highlight.io
 Requires-Python: >=3.8,<4.0
```

