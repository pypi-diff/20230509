# Comparing `tmp/llamatry-0.1.4.tar.gz` & `tmp/llamatry-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamatry-0.1.4.tar", max compression
+gzip compressed data, was "llamatry-0.1.5.tar", max compression
```

## Comparing `llamatry-0.1.4.tar` & `llamatry-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4401 2023-05-08 19:30:29.882868 llamatry-0.1.4/README.md
--rw-r--r--   0        0        0      148 2023-05-08 18:54:23.941377 llamatry-0.1.4/llamatry/__init__.py
--rw-r--r--   0        0        0     4817 2023-05-08 18:43:18.145718 llamatry-0.1.4/llamatry/completions.py
--rw-r--r--   0        0        0     2420 2023-05-08 19:28:40.685648 llamatry-0.1.4/llamatry/trace.py
--rw-r--r--   0        0        0      650 2023-05-08 19:11:11.079726 llamatry-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 llamatry-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4503 2023-05-08 19:43:45.009742 llamatry-0.1.5/README.md
+-rw-r--r--   0        0        0      148 2023-05-08 18:54:23.941377 llamatry-0.1.5/llamatry/__init__.py
+-rw-r--r--   0        0        0     4385 2023-05-09 00:25:55.348493 llamatry-0.1.5/llamatry/completions.py
+-rw-r--r--   0        0        0     2420 2023-05-08 19:28:40.685648 llamatry-0.1.5/llamatry/trace.py
+-rw-r--r--   0        0        0      650 2023-05-09 00:27:00.884449 llamatry-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5343 1970-01-01 00:00:00.000000 llamatry-0.1.5/PKG-INFO
```

### Comparing `llamatry-0.1.4/README.md` & `llamatry-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -82,24 +82,28 @@
 
 To use the `Trace` class as a decorator, you can decorate your function using `@Trace.trace`. The function's name will be used as the span name by default. If you want to set a custom span name, you can provide it as an argument: `@Trace.trace("custom_span_name")`. By default if you decorate a function all arguments that are `(str, int, float, bool)` will be set as attributes.
 
 ```python
 from llamatry import Trace
 
 @Trace.trace
-def your_function():
+def your_function(a, b):
     # Your function implementation
-    span = Trace.get_current_span()
-    span.set_attribute("foo", "bar")
+    # a, b and automatically set as span attributes
     pass
 
 @Trace.trace("custom_span_name")
 def another_function():
     # Your function implementation
     pass
+
+with Trace.span("custom_span_name") as span:
+    # Your code block here
+    span.set_attribute("foo", "bar")
+    pass
 ```
 
 ### Using the Trace context manager
 
 To use the Trace class as a context manager, use the `with` statement followed by `Trace.span("custom_span_name")`.
 
 ```python
```

### Comparing `llamatry-0.1.4/llamatry/completions.py` & `llamatry-0.1.5/llamatry/completions.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,30 +40,18 @@
         :param kwargs: the kwargs passed to the create method
         :param response: the response from the create method
         """
         for key, value in kwargs.items():
             if isinstance(value, (str, bool, float, int)) and key != "prompt":
                 span.set_attribute(f"openai.create.{key}", value)
 
-        usage = response.get("usage", {})
         span.set_attribute("openai.response.id", response.get("id", ""))
         span.set_attribute("openai.response.created", response.get("created", 0))
-
-        # only set these attributes if the response is a stream since the are
-        # not present in the non-streaming response
-        if kwargs.get("stream", False):
-            span.set_attribute(
-                "openai.usage.prompt_tokens", usage.get("prompt_tokens", None)
-            )
-            span.set_attribute(
-                "openai.usage.completion_tokens", usage.get("completion_tokens", None)
-            )
-            span.set_attribute(
-                "openai.usage.total_tokens", usage.get("total_tokens", None)
-            )
+        span.set_attribute("openai.response.usage", response.get("usage", None))
+        span.set_attribute("openai.response.model", response.get("model", None))
 
     def _trace_create(self, original_create):
         @functools.wraps(original_create)
         def wrapper(*args, **kwargs):
             stream = kwargs.get("stream", False)
             tracer = trace.get_tracer(__name__)
```

### Comparing `llamatry-0.1.4/llamatry/trace.py` & `llamatry-0.1.5/llamatry/trace.py`

 * *Files identical despite different names*

### Comparing `llamatry-0.1.4/pyproject.toml` & `llamatry-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llamatry"
-version = "0.1.4"
+version = "0.1.5"
 description = "opentelemetry instrumentation for openai's completions api"
 authors = ["Jason <jason@jxnl.co>"]
 readme = "README.md"
 repository = "https://github.com/jxnl/llamatry"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `llamatry-0.1.4/PKG-INFO` & `llamatry-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamatry
-Version: 0.1.4
+Version: 0.1.5
 Summary: opentelemetry instrumentation for openai's completions api
 Home-page: https://github.com/jxnl/llamatry
 Author: Jason
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -103,24 +103,28 @@
 
 To use the `Trace` class as a decorator, you can decorate your function using `@Trace.trace`. The function's name will be used as the span name by default. If you want to set a custom span name, you can provide it as an argument: `@Trace.trace("custom_span_name")`. By default if you decorate a function all arguments that are `(str, int, float, bool)` will be set as attributes.
 
 ```python
 from llamatry import Trace
 
 @Trace.trace
-def your_function():
+def your_function(a, b):
     # Your function implementation
-    span = Trace.get_current_span()
-    span.set_attribute("foo", "bar")
+    # a, b and automatically set as span attributes
     pass
 
 @Trace.trace("custom_span_name")
 def another_function():
     # Your function implementation
     pass
+
+with Trace.span("custom_span_name") as span:
+    # Your code block here
+    span.set_attribute("foo", "bar")
+    pass
 ```
 
 ### Using the Trace context manager
 
 To use the Trace class as a context manager, use the `with` statement followed by `Trace.span("custom_span_name")`.
 
 ```python
```

