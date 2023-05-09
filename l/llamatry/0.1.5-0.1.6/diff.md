# Comparing `tmp/llamatry-0.1.5.tar.gz` & `tmp/llamatry-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamatry-0.1.5.tar", max compression
+gzip compressed data, was "llamatry-0.1.6.tar", max compression
```

## Comparing `llamatry-0.1.5.tar` & `llamatry-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4503 2023-05-08 19:43:45.009742 llamatry-0.1.5/README.md
--rw-r--r--   0        0        0      148 2023-05-08 18:54:23.941377 llamatry-0.1.5/llamatry/__init__.py
--rw-r--r--   0        0        0     4385 2023-05-09 00:25:55.348493 llamatry-0.1.5/llamatry/completions.py
--rw-r--r--   0        0        0     2420 2023-05-08 19:28:40.685648 llamatry-0.1.5/llamatry/trace.py
--rw-r--r--   0        0        0      650 2023-05-09 00:27:00.884449 llamatry-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5343 1970-01-01 00:00:00.000000 llamatry-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4503 2023-05-08 19:43:45.009742 llamatry-0.1.6/README.md
+-rw-r--r--   0        0        0      148 2023-05-08 18:54:23.941377 llamatry-0.1.6/llamatry/__init__.py
+-rw-r--r--   0        0        0     4624 2023-05-09 00:31:55.937375 llamatry-0.1.6/llamatry/completions.py
+-rw-r--r--   0        0        0     2420 2023-05-08 19:28:40.685648 llamatry-0.1.6/llamatry/trace.py
+-rw-r--r--   0        0        0      650 2023-05-09 00:32:27.442594 llamatry-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5343 1970-01-01 00:00:00.000000 llamatry-0.1.6/PKG-INFO
```

### Comparing `llamatry-0.1.5/README.md` & `llamatry-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `llamatry-0.1.5/llamatry/completions.py` & `llamatry-0.1.6/llamatry/completions.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,18 +40,25 @@
         :param kwargs: the kwargs passed to the create method
         :param response: the response from the create method
         """
         for key, value in kwargs.items():
             if isinstance(value, (str, bool, float, int)) and key != "prompt":
                 span.set_attribute(f"openai.create.{key}", value)
 
-        span.set_attribute("openai.response.id", response.get("id", ""))
-        span.set_attribute("openai.response.created", response.get("created", 0))
-        span.set_attribute("openai.response.usage", response.get("usage", None))
-        span.set_attribute("openai.response.model", response.get("model", None))
+        span.set_attribute("openai.id", response.get("id", ""))
+        span.set_attribute("openai.created", response.get("created", 0))
+        span.set_attribute("openai.model", response.get("model", None))
+
+        usage = response.get("usage", None)
+        if usage:
+            span.set_attribute("openai.usage.completion_tokens", usage.get("completion_tokens", 0))
+            span.set_attribute("openai.usage.prompt_tokens", usage.get("prompt_tokens", 0))
+            span.set_attribute("openai.usage.total_tokens", usage.get("total_tokens", 0))
+
+
 
     def _trace_create(self, original_create):
         @functools.wraps(original_create)
         def wrapper(*args, **kwargs):
             stream = kwargs.get("stream", False)
             tracer = trace.get_tracer(__name__)
```

### Comparing `llamatry-0.1.5/llamatry/trace.py` & `llamatry-0.1.6/llamatry/trace.py`

 * *Files identical despite different names*

### Comparing `llamatry-0.1.5/pyproject.toml` & `llamatry-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llamatry"
-version = "0.1.5"
+version = "0.1.6"
 description = "opentelemetry instrumentation for openai's completions api"
 authors = ["Jason <jason@jxnl.co>"]
 readme = "README.md"
 repository = "https://github.com/jxnl/llamatry"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `llamatry-0.1.5/PKG-INFO` & `llamatry-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamatry
-Version: 0.1.5
+Version: 0.1.6
 Summary: opentelemetry instrumentation for openai's completions api
 Home-page: https://github.com/jxnl/llamatry
 Author: Jason
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

