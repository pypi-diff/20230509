# Comparing `tmp/latch_o11y-0.1.1.tar.gz` & `tmp/latch_o11y-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_o11y-0.1.1.tar", max compression
+gzip compressed data, was "latch_o11y-0.1.3.tar", max compression
```

## Comparing `latch_o11y-0.1.1.tar` & `latch_o11y-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     7052 2023-04-27 17:53:53.729206 latch_o11y-0.1.1/LICENSE
--rw-r--r--   0        0        0       14 2023-04-27 17:54:11.934983 latch_o11y-0.1.1/README.md
--rw-r--r--   0        0        0     6840 2023-04-27 21:02:53.439523 latch_o11y-0.1.1/latch_o11y/o11y.py
--rw-r--r--   0        0        0      953 2023-04-27 21:19:48.977493 latch_o11y-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 latch_o11y-0.1.1/setup.py
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 latch_o11y-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 17:53:53.729206 latch_o11y-0.1.3/LICENSE
+-rw-r--r--   0        0        0       14 2023-04-27 17:54:11.934983 latch_o11y-0.1.3/README.md
+-rw-r--r--   0        0        0     7048 2023-05-09 21:34:27.276447 latch_o11y-0.1.3/latch_o11y/o11y.py
+-rw-r--r--   0        0        0        0 2023-05-09 17:04:17.188957 latch_o11y-0.1.3/latch_o11y/py.typed
+-rw-r--r--   0        0        0     1257 2023-05-09 21:34:50.312612 latch_o11y-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 latch_o11y-0.1.3/setup.py
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 latch_o11y-0.1.3/PKG-INFO
```

### Comparing `latch_o11y-0.1.1/LICENSE` & `latch_o11y-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_o11y-0.1.1/latch_o11y/o11y.py` & `latch_o11y-0.1.3/latch_o11y/o11y.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 import functools
 import inspect
+from dataclasses import dataclass
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Awaitable, Callable, Concatenate, ParamSpec, TypeAlias, TypeVar
 
 import orjson
 import structlog as slog
+from latch_config.config import DatadogConfig, LoggingMode, read_config
 from opentelemetry import trace
 from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.resources import Attributes, LabelValue, Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.trace import Tracer
 from opentelemetry.trace.span import INVALID_SPAN, INVALID_SPAN_CONTEXT, Span
 from structlog.types import EventDict, WrappedLogger
 
-from latch_config.config import LoggingMode, config
+
+@dataclass(frozen=True)
+class Config:
+    datadog: DatadogConfig
+    logging_mode: LoggingMode = LoggingMode.console_json
+
+
+config = read_config(Config)
 
 
 def add_timestamp(logger: WrappedLogger, name: str, x: EventDict) -> EventDict:
     # the default slog.processors.TimeStamper is not great with timezones
     utc = datetime.now(timezone.utc)
     x["timestamp"] = utc.astimezone().isoformat()
     return x
```

### Comparing `latch_o11y-0.1.1/setup.py` & `latch_o11y-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 packages = \
 ['latch_o11y']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['latch-config>=0.1.1,<0.2.0',
+['latch-config>=0.1.4,<0.2.0',
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-exporter-otlp-proto-grpc>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'orjson>=3.8.5,<4.0.0',
  'structlog>=22.3.0,<23.0.0']
 
 setup_kwargs = {
     'name': 'latch-o11y',
-    'version': '0.1.1',
+    'version': '0.1.3',
     'description': 'Observability for latch python backend services',
     'long_description': '# python-o11y\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `latch_o11y-0.1.1/PKG-INFO` & `latch_o11y-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: latch-o11y
-Version: 0.1.1
+Version: 0.1.3
 Summary: Observability for latch python backend services
 License: CC0 1.0
 Author: Max Smolin
 Author-email: max@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: latch-config (>=0.1.1,<0.2.0)
+Requires-Dist: latch-config (>=0.1.4,<0.2.0)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: orjson (>=3.8.5,<4.0.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
 Description-Content-Type: text/markdown
```

