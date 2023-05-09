# Comparing `tmp/llamatry-0.1.6.tar.gz` & `tmp/llamatry-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamatry-0.1.6.tar", max compression
+gzip compressed data, was "llamatry-0.1.7.tar", max compression
```

## Comparing `llamatry-0.1.6.tar` & `llamatry-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4503 2023-05-08 19:43:45.009742 llamatry-0.1.6/README.md
--rw-r--r--   0        0        0      148 2023-05-08 18:54:23.941377 llamatry-0.1.6/llamatry/__init__.py
--rw-r--r--   0        0        0     4624 2023-05-09 00:31:55.937375 llamatry-0.1.6/llamatry/completions.py
--rw-r--r--   0        0        0     2420 2023-05-08 19:28:40.685648 llamatry-0.1.6/llamatry/trace.py
--rw-r--r--   0        0        0      650 2023-05-09 00:32:27.442594 llamatry-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5343 1970-01-01 00:00:00.000000 llamatry-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     5687 2023-05-09 20:34:30.290019 llamatry-0.1.7/README.md
+-rw-r--r--   0        0        0      123 2023-05-09 20:28:16.877771 llamatry-0.1.7/llamatry/__init__.py
+-rw-r--r--   0        0        0     4899 2023-05-09 20:32:59.452233 llamatry-0.1.7/llamatry/openai.py
+-rw-r--r--   0        0        0     2420 2023-05-08 19:28:40.685648 llamatry-0.1.7/llamatry/trace.py
+-rw-r--r--   0        0        0      650 2023-05-09 20:35:41.677484 llamatry-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6527 1970-01-01 00:00:00.000000 llamatry-0.1.7/PKG-INFO
```

### Comparing `llamatry-0.1.6/README.md` & `llamatry-0.1.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 Import the necessary packages:
 
 ```python
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import ConsoleSpanExporter, SimpleSpanProcessor
 
-from llamatry import OpenAICompletionInstrumentor
+from llamatry import OpenAIInstrumentor
 
 import openai
 import os
 ```
 
 Set up open telemetry:
 
@@ -52,15 +52,15 @@
 ```python
 openai.api_key = os.environ["OPENAI_API_KEY"]
 ```
 
 Instrument the OpenAI API using Llamatry:
 
 ```python
-OpenAICompletionInstrumentor().instrument()
+OpenAIInstrumentor().instrument()
 ```
 
 Make API calls to the OpenAI API:
 
 ```python
 response = openai.ChatCompletion.create(
     messages=[
@@ -68,14 +68,56 @@
         {"role": "user", "content": "Who won the world series in 2020?"},
     ],
     max_tokens=50,
     temperature=0.5,
 )
 ```
 
+Console Export:
+
+```
+{
+    "name": "ChatCompletion.create",
+    "context": {
+        "trace_id": "0x6026b10ff364a1954df343ac2e292fd7",
+        "span_id": "0x3f04991076717d88",
+        "trace_state": "[]"
+    },
+    "kind": "SpanKind.INTERNAL",
+    "parent_id": "0x14abcdaf2d49f177",
+    "start_time": "2023-05-09T20:32:10.674716Z",
+    "end_time": "2023-05-09T20:32:11.827791Z",
+    "status": {
+        "status_code": "UNSET"
+    },
+    "attributes": {
+        "openai.create.model": "gpt-3.5-turbo",
+        "openai.create.max_tokens": 500,
+        "openai.create.temperature": 0.5,
+        "openai.response.id": "chatcmpl-7EOIE4fVofq83WPl1HFNkDI6yBPZ8",
+        "openai.response.created": 1683664330,
+        "openai.response.model": "gpt-3.5-turbo-0301",
+        "openai.usage.completion_tokens": 13,
+        "openai.usage.prompt_tokens": 30,
+        "openai.usage.total_tokens": 43
+    },
+    "events": [],
+    "links": [],
+    "resource": {
+        "attributes": {
+            "telemetry.sdk.language": "python",
+            "telemetry.sdk.name": "opentelemetry",
+            "telemetry.sdk.version": "1.17.0",
+            "service.name": "llamatry"
+        },
+        "schema_url": ""
+    }
+}
+```
+
 Traces and other information related to the OpenAI API calls will be output to the console. By using Llamatry, you can easily switch to other exporters supported by OpenTelemetry, such as Jaeger or Zipkin, to visualize and analyze the data in different ways.
 
 ## Decorator and Context Manager helpers
 
 Llamatry provides a convenient tracing utility with both decorator and context manager support. This allows you to trace your functions and code blocks easily using the provided Trace class.
 
 ### Using the Trace decorator
```

### Comparing `llamatry-0.1.6/llamatry/completions.py` & `llamatry-0.1.7/llamatry/openai.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,34 +2,43 @@
 from typing import Collection
 from opentelemetry import trace
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import SpanKind
 import openai
 
 
-class OpenAICompletionInstrumentor(BaseInstrumentor):
+class OpenAIInstrumentor(BaseInstrumentor):
     def _instrument(self, **kwargs):
         self._original_chatcompletion_create = openai.ChatCompletion.create
         self._original_chatcompletion_acreate = openai.ChatCompletion.acreate
         self._original_create = openai.Completion.create
         self._original_acreate = openai.Completion.acreate
+        self._original_embeddings_create = openai.Embedding.create
+        self._original_embeddings_acreate = openai.Embedding.acreate
+
         openai.ChatCompletion.create = self._trace_create(
             self._original_chatcompletion_create
         )
         openai.ChatCompletion.acreate = self._trace_acreate(
             self._original_chatcompletion_acreate
         )
         openai.Completion.create = self._trace_create(self._original_create)
         openai.Completion.acreate = self._trace_acreate(self._original_acreate)
+        openai.Embedding.create = self._trace_create(self._original_embeddings_create)
+        openai.Embedding.acreate = self._trace_acreate(
+            self._original_embeddings_acreate
+        )
 
     def _uninstrument(self, **kwargs):
         openai.ChatCompletion.create = self._original_chatcompletion_create
         openai.ChatCompletion.acreate = self._original_chatcompletion_acreate
         openai.Completion.create = self._original_completion_create
         openai.Completion.acreate = self._original_completion_acreate
+        openai.Embedding.create = self._original_embeddings_create
+        openai.Embedding.acreate = self._original_embeddings_acreate
 
     def instrumentation_dependencies(self) -> Collection[BaseInstrumentor]:
         return []
 
     @staticmethod
     def _set_span_attributes(span, kwargs, response):
         """
@@ -40,34 +49,32 @@
         :param kwargs: the kwargs passed to the create method
         :param response: the response from the create method
         """
         for key, value in kwargs.items():
             if isinstance(value, (str, bool, float, int)) and key != "prompt":
                 span.set_attribute(f"openai.create.{key}", value)
 
-        span.set_attribute("openai.id", response.get("id", ""))
-        span.set_attribute("openai.created", response.get("created", 0))
-        span.set_attribute("openai.model", response.get("model", None))
+        for key in ["id", "created", "model"]:
+            if key in response:
+                span.set_attribute(f"openai.response.{key}", response[key])
 
         usage = response.get("usage", None)
         if usage:
-            span.set_attribute("openai.usage.completion_tokens", usage.get("completion_tokens", 0))
-            span.set_attribute("openai.usage.prompt_tokens", usage.get("prompt_tokens", 0))
-            span.set_attribute("openai.usage.total_tokens", usage.get("total_tokens", 0))
-
-
+            for key in ["completion_tokens", "prompt_tokens", "total_tokens"]:
+                if key in usage:
+                    span.set_attribute(f"openai.usage.{key}", usage[key])
 
     def _trace_create(self, original_create):
         @functools.wraps(original_create)
         def wrapper(*args, **kwargs):
             stream = kwargs.get("stream", False)
             tracer = trace.get_tracer(__name__)
 
             with tracer.start_as_current_span(
-                "openai.ChatCompletion.create", kind=SpanKind.CLIENT
+                original_create.__qualname__,
             ) as span:
                 if stream:
 
                     def stream_wrapper():
                         first_chunk = True
                         for resp in original_create(*args, **kwargs):
                             if first_chunk:
@@ -85,15 +92,15 @@
 
     def _trace_acreate(self, original_acreate):
         @functools.wraps(original_acreate)
         async def wrapper(*args, **kwargs):
             stream = kwargs.get("stream", False)
             tracer = trace.get_tracer(__name__)
             with tracer.start_as_current_span(
-                "openai.ChatCompletion.acreate", kind=SpanKind.CLIENT
+                f"openai.{original_acreate.__qualname__}"
             ) as span:
                 response = await original_acreate(*args, **kwargs)
                 if stream:
 
                     async def stream_wrapper():
                         first_chunk = True
                         async for resp in response:
```

### Comparing `llamatry-0.1.6/llamatry/trace.py` & `llamatry-0.1.7/llamatry/trace.py`

 * *Files identical despite different names*

### Comparing `llamatry-0.1.6/pyproject.toml` & `llamatry-0.1.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llamatry"
-version = "0.1.6"
+version = "0.1.7"
 description = "opentelemetry instrumentation for openai's completions api"
 authors = ["Jason <jason@jxnl.co>"]
 readme = "README.md"
 repository = "https://github.com/jxnl/llamatry"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `llamatry-0.1.6/PKG-INFO` & `llamatry-0.1.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamatry
-Version: 0.1.6
+Version: 0.1.7
 Summary: opentelemetry instrumentation for openai's completions api
 Home-page: https://github.com/jxnl/llamatry
 Author: Jason
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -49,15 +49,15 @@
 Import the necessary packages:
 
 ```python
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import ConsoleSpanExporter, SimpleSpanProcessor
 
-from llamatry import OpenAICompletionInstrumentor
+from llamatry import OpenAIInstrumentor
 
 import openai
 import os
 ```
 
 Set up open telemetry:
 
@@ -73,15 +73,15 @@
 ```python
 openai.api_key = os.environ["OPENAI_API_KEY"]
 ```
 
 Instrument the OpenAI API using Llamatry:
 
 ```python
-OpenAICompletionInstrumentor().instrument()
+OpenAIInstrumentor().instrument()
 ```
 
 Make API calls to the OpenAI API:
 
 ```python
 response = openai.ChatCompletion.create(
     messages=[
@@ -89,14 +89,56 @@
         {"role": "user", "content": "Who won the world series in 2020?"},
     ],
     max_tokens=50,
     temperature=0.5,
 )
 ```
 
+Console Export:
+
+```
+{
+    "name": "ChatCompletion.create",
+    "context": {
+        "trace_id": "0x6026b10ff364a1954df343ac2e292fd7",
+        "span_id": "0x3f04991076717d88",
+        "trace_state": "[]"
+    },
+    "kind": "SpanKind.INTERNAL",
+    "parent_id": "0x14abcdaf2d49f177",
+    "start_time": "2023-05-09T20:32:10.674716Z",
+    "end_time": "2023-05-09T20:32:11.827791Z",
+    "status": {
+        "status_code": "UNSET"
+    },
+    "attributes": {
+        "openai.create.model": "gpt-3.5-turbo",
+        "openai.create.max_tokens": 500,
+        "openai.create.temperature": 0.5,
+        "openai.response.id": "chatcmpl-7EOIE4fVofq83WPl1HFNkDI6yBPZ8",
+        "openai.response.created": 1683664330,
+        "openai.response.model": "gpt-3.5-turbo-0301",
+        "openai.usage.completion_tokens": 13,
+        "openai.usage.prompt_tokens": 30,
+        "openai.usage.total_tokens": 43
+    },
+    "events": [],
+    "links": [],
+    "resource": {
+        "attributes": {
+            "telemetry.sdk.language": "python",
+            "telemetry.sdk.name": "opentelemetry",
+            "telemetry.sdk.version": "1.17.0",
+            "service.name": "llamatry"
+        },
+        "schema_url": ""
+    }
+}
+```
+
 Traces and other information related to the OpenAI API calls will be output to the console. By using Llamatry, you can easily switch to other exporters supported by OpenTelemetry, such as Jaeger or Zipkin, to visualize and analyze the data in different ways.
 
 ## Decorator and Context Manager helpers
 
 Llamatry provides a convenient tracing utility with both decorator and context manager support. This allows you to trace your functions and code blocks easily using the provided Trace class.
 
 ### Using the Trace decorator
```

