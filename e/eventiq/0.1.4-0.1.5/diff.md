# Comparing `tmp/eventiq-0.1.4.tar.gz` & `tmp/eventiq-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventiq-0.1.4.tar", max compression
+gzip compressed data, was "eventiq-0.1.5.tar", max compression
```

## Comparing `eventiq-0.1.4.tar` & `eventiq-0.1.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0    11357 2023-05-02 19:28:01.090240 eventiq-0.1.4/LICENSE
--rw-r--r--   0        0        0     4666 2023-05-02 19:28:01.090240 eventiq-0.1.4/README.md
--rw-r--r--   0        0        0      704 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/__init__.py
--rw-r--r--   0        0        0       59 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/__main__.py
--rw-r--r--   0        0        0      407 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/_compat.py
--rw-r--r--   0        0        0       22 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/_version.py
--rw-r--r--   0        0        0      171 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/asyncapi/__init__.py
--rw-r--r--   0        0        0     2598 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/asyncapi/generator.py
--rw-r--r--   0        0        0     1579 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/asyncapi/models.py
--rw-r--r--   0        0        0      426 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/asyncapi/registry.py
--rw-r--r--   0        0        0        0 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/__init__.py
--rw-r--r--   0        0        0       59 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/kafka/__init__.py
--rw-r--r--   0        0        0     3673 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/kafka/broker.py
--rw-r--r--   0        0        0      482 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/kafka/settings.py
--rw-r--r--   0        0        0      181 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/nats/__init__.py
--rw-r--r--   0        0        0     5867 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/nats/broker.py
--rw-r--r--   0        0        0     2841 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/nats/middlewares.py
--rw-r--r--   0        0        0      617 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/nats/settings.py
--rw-r--r--   0        0        0       61 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/pubsub/__init__.py
--rw-r--r--   0        0        0     2359 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/pubsub/broker.py
--rw-r--r--   0        0        0      179 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/pubsub/settings.py
--rw-r--r--   0        0        0       65 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/rabbitmq/__init__.py
--rw-r--r--   0        0        0     5037 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/rabbitmq/broker.py
--rw-r--r--   0        0        0      816 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/rabbitmq/middlewares.py
--rw-r--r--   0        0        0      437 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/rabbitmq/settings.py
--rw-r--r--   0        0        0       59 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/redis/__init__.py
--rw-r--r--   0        0        0     1894 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/redis/broker.py
--rw-r--r--   0        0        0     1745 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/redis/middlewares.py
--rw-r--r--   0        0        0      305 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/redis/settings.py
--rw-r--r--   0        0        0     1978 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/backends/stub.py
--rw-r--r--   0        0        0     9233 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/broker.py
--rw-r--r--   0        0        0     2466 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/cli.py
--rw-r--r--   0        0        0        0 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/config/__init__.py
--rw-r--r--   0        0        0      995 2023-05-02 19:28:01.090240 eventiq-0.1.4/eventiq/config/factory.py
--rw-r--r--   0        0        0     1723 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/config/models.py
--rw-r--r--   0        0        0      226 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/config/settings.py
--rw-r--r--   0        0        0     4353 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/consumer.py
--rw-r--r--   0        0        0       92 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/defaults.py
--rw-r--r--   0        0        0      282 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/encoders/__init__.py
--rw-r--r--   0        0        0      670 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/encoders/json.py
--rw-r--r--   0        0        0      706 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/encoders/msgpack.py
--rw-r--r--   0        0        0      645 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/encoders/orjson.py
--rw-r--r--   0        0        0      494 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/encoders/pickle.py
--rw-r--r--   0        0        0      955 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/exceptions.py
--rw-r--r--   0        0        0     1584 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/http.py
--rw-r--r--   0        0        0     1014 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/logger.py
--rw-r--r--   0        0        0      784 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/message.py
--rw-r--r--   0        0        0     3333 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middleware.py
--rw-r--r--   0        0        0      354 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middlewares/__init__.py
--rw-r--r--   0        0        0      871 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middlewares/debug.py
--rw-r--r--   0        0        0      862 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middlewares/error.py
--rw-r--r--   0        0        0     1682 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middlewares/healthcheck.py
--rw-r--r--   0        0        0     4435 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middlewares/opentelemetry.py
--rw-r--r--   0        0        0     5115 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middlewares/prometheus.py
--rw-r--r--   0        0        0     3926 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/middlewares/retries.py
--rw-r--r--   0        0        0     2144 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/models.py
--rw-r--r--   0        0        0     1665 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/plugins.py
--rw-r--r--   0        0        0        0 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/py.typed
--rw-r--r--   0        0        0      740 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/runner.py
--rw-r--r--   0        0        0     3668 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/service.py
--rw-r--r--   0        0        0      643 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/settings.py
--rw-r--r--   0        0        0     1116 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/types.py
--rw-r--r--   0        0        0      216 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/utils/__init__.py
--rw-r--r--   0        0        0      192 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/utils/datetime.py
--rw-r--r--   0        0        0      390 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/utils/enum.py
--rw-r--r--   0        0        0      915 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/utils/functools.py
--rw-r--r--   0        0        0     1106 2023-05-02 19:28:01.094240 eventiq-0.1.4/eventiq/utils/imports.py
--rw-r--r--   0        0        0     4360 2023-05-02 19:28:01.094240 eventiq-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     7562 1970-01-01 00:00:00.000000 eventiq-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 21:04:19.342155 eventiq-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4649 2023-05-09 21:04:19.342155 eventiq-0.1.5/README.md
+-rw-r--r--   0        0        0      772 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/__main__.py
+-rw-r--r--   0        0        0       22 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/_version.py
+-rw-r--r--   0        0        0      171 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/asyncapi/__init__.py
+-rw-r--r--   0        0        0     2636 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/asyncapi/generator.py
+-rw-r--r--   0        0        0     1579 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/asyncapi/models.py
+-rw-r--r--   0        0        0      426 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/asyncapi/registry.py
+-rw-r--r--   0        0        0        0 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/kafka/__init__.py
+-rw-r--r--   0        0        0     3673 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/kafka/broker.py
+-rw-r--r--   0        0        0      482 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/kafka/settings.py
+-rw-r--r--   0        0        0      163 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/nats/__init__.py
+-rw-r--r--   0        0        0     5447 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/nats/broker.py
+-rw-r--r--   0        0        0     2809 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/nats/plugins.py
+-rw-r--r--   0        0        0      617 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/nats/settings.py
+-rw-r--r--   0        0        0       61 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/pubsub/__init__.py
+-rw-r--r--   0        0        0     2470 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/pubsub/broker.py
+-rw-r--r--   0        0        0      179 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/pubsub/settings.py
+-rw-r--r--   0        0        0       65 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     5044 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/rabbitmq/broker.py
+-rw-r--r--   0        0        0      816 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/rabbitmq/middlewares.py
+-rw-r--r--   0        0        0      437 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/rabbitmq/settings.py
+-rw-r--r--   0        0        0      121 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/redis/__init__.py
+-rw-r--r--   0        0        0     1894 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/redis/broker.py
+-rw-r--r--   0        0        0     1767 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/redis/plugins.py
+-rw-r--r--   0        0        0      305 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/redis/settings.py
+-rw-r--r--   0        0        0     2004 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/backends/stub.py
+-rw-r--r--   0        0        0     9560 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/broker.py
+-rw-r--r--   0        0        0     2466 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/cli.py
+-rw-r--r--   0        0        0        0 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/config/__init__.py
+-rw-r--r--   0        0        0     1220 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/config/factory.py
+-rw-r--r--   0        0        0     1824 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/config/models.py
+-rw-r--r--   0        0        0      226 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/config/settings.py
+-rw-r--r--   0        0        0     4206 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/consumer.py
+-rw-r--r--   0        0        0      558 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/context.py
+-rw-r--r--   0        0        0        0 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/contrib/__init__.py
+-rw-r--r--   0        0        0     1443 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/contrib/fastapi.py
+-rw-r--r--   0        0        0      282 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/encoders/__init__.py
+-rw-r--r--   0        0        0      670 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/encoders/json.py
+-rw-r--r--   0        0        0      706 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/encoders/msgpack.py
+-rw-r--r--   0        0        0      645 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/encoders/orjson.py
+-rw-r--r--   0        0        0      494 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/encoders/pickle.py
+-rw-r--r--   0        0        0      873 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/exceptions.py
+-rw-r--r--   0        0        0     1148 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/logger.py
+-rw-r--r--   0        0        0      784 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/message.py
+-rw-r--r--   0        0        0     3333 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middleware.py
+-rw-r--r--   0        0        0      354 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middlewares/__init__.py
+-rw-r--r--   0        0        0      871 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middlewares/debug.py
+-rw-r--r--   0        0        0      860 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middlewares/error.py
+-rw-r--r--   0        0        0     1729 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middlewares/healthcheck.py
+-rw-r--r--   0        0        0     4435 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middlewares/opentelemetry.py
+-rw-r--r--   0        0        0     5115 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middlewares/prometheus.py
+-rw-r--r--   0        0        0     3926 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/middlewares/retries.py
+-rw-r--r--   0        0        0     2352 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/models.py
+-rw-r--r--   0        0        0      585 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/plugins.py
+-rw-r--r--   0        0        0        0 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/py.typed
+-rw-r--r--   0        0        0      740 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/runner.py
+-rw-r--r--   0        0        0     3649 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/service.py
+-rw-r--r--   0        0        0      643 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/settings.py
+-rw-r--r--   0        0        0     1253 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/types.py
+-rw-r--r--   0        0        0      216 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/utils/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/utils/datetime.py
+-rw-r--r--   0        0        0      390 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/utils/enum.py
+-rw-r--r--   0        0        0     1862 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/utils/functools.py
+-rw-r--r--   0        0        0     1106 2023-05-09 21:04:19.346155 eventiq-0.1.5/eventiq/utils/imports.py
+-rw-r--r--   0        0        0     4258 2023-05-09 21:04:19.346155 eventiq-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     7448 1970-01-01 00:00:00.000000 eventiq-0.1.5/PKG-INFO
```

### Comparing `eventiq-0.1.4/LICENSE` & `eventiq-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/README.md` & `eventiq-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 *Note: This package is under active development and is not recommended for production use*
 
 ---
-Version: 0.1.4
+Version: 0.1.5
 
 Documentation: https://performancemedia.github.io/eventiq/
 
 Repository: https://github.com/performancemedia/eventiq
 
 ---
 ## About
 
-The package utilizes `pydantic`, `async_timeout` and `python-json-logger` as the only required dependencies.
+The package utilizes `pydantic` and `python-json-logger` as the only required dependencies.
 For messages [Cloud Events](https://cloudevents.io/) format is used.
 Service can be run as standalone processes, or included into starlette (e.g. FastAPI) applications.
 
 ## Installation
 
 ```shell
 pip install eventiq
```

### Comparing `eventiq-0.1.4/eventiq/__init__.py` & `eventiq-0.1.5/eventiq/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from ._version import __version__
 from .asyncapi import publishes
 from .broker import Broker
 from .consumer import Consumer, ConsumerGroup, ForwardResponse, GenericConsumer
+from .context import get_current_service
 from .message import Message
 from .middleware import Middleware
 from .models import CloudEvent
 from .plugins import BrokerPlugin, ServicePlugin
 from .runner import ServiceRunner
 from .service import Service
 from .types import RawMessage
@@ -22,8 +23,9 @@
     "Message",
     "Middleware",
     "RawMessage",
     "Service",
     "ServicePlugin",
     "ServiceRunner",
     "publishes",
+    "get_current_service",
 ]
```

### Comparing `eventiq-0.1.4/eventiq/asyncapi/generator.py` & `eventiq-0.1.5/eventiq/asyncapi/generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import functools
 import json
 from collections import defaultdict
 from itertools import chain
 from pathlib import Path
 
 from pydantic.schema import schema as all_schemas
 
@@ -58,14 +59,15 @@
                 description=consumer.description,
             )
         )
         channels[consumer.topic].subscribe = subscribe
     return channels
 
 
+@functools.lru_cache
 def get_async_api_spec(service: Service) -> AsyncAPI:
     channels = populate_channel_spec(service)
     definitions = get_all_models_schema(service)
     doc_model = AsyncAPI(
         info=Info(title=service.title, version=service.version),
         servers={},
         channels=channels,
```

### Comparing `eventiq-0.1.4/eventiq/asyncapi/models.py` & `eventiq-0.1.5/eventiq/asyncapi/models.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/backends/kafka/broker.py` & `eventiq-0.1.5/eventiq/backends/kafka/broker.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/backends/nats/broker.py` & `eventiq-0.1.5/eventiq/backends/nats/broker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING, Any
 
 import nats
+from nats.aio.client import Client
 from nats.aio.msg import Msg as NatsMsg
 from nats.js import JetStreamContext
 
 from eventiq.broker import Broker
-from eventiq.exceptions import BrokerError, PublishError
-from eventiq.utils.functools import retry_async
+from eventiq.exceptions import PublishError
+from eventiq.utils.functools import retry
 
 from ...message import Message
 from .settings import JetStreamSettings, NatsSettings
 
 if TYPE_CHECKING:
     from eventiq import CloudEvent, Consumer, Service
 
@@ -43,56 +44,50 @@
         **kwargs: Any,
     ) -> None:
 
         super().__init__(**kwargs)
         self.url = url
         self.connection_options = connection_options or {}
         self._auto_flush = auto_flush
-        self._nc = None
+        self.client = Client()
 
     @property
     def message_proxy_class(self) -> type[Message]:
         return NatsMessageProxy
 
-    @property
-    def nc(self) -> nats.NATS:
-        if self._nc is None:
-            raise BrokerError("Broker not connected. Call await broker.connect() first")
-        return self._nc
-
     def parse_incoming_message(self, message: NatsMsg) -> Any:
         return self.encoder.decode(message.data)
 
     async def _start_consumer(self, service: Service, consumer: Consumer) -> None:
-        await self.nc.subscribe(
+        await self.client.subscribe(
             subject=consumer.topic,
             queue=f"{service.name}:{consumer.name}",
             cb=self.get_handler(service, consumer),
         )
 
     async def _disconnect(self) -> None:
-        await self.nc.close()
+        await self.client.close()
 
     async def flush(self):
-        await self.nc.flush()
+        await self.client.flush()
 
-    @retry_async(max_retries=3)
+    @retry(max_retries=3)
     async def _connect(self) -> None:
-        self._nc = await nats.connect(self.url, **self.connection_options)
+        self._nc = await self.client.connect(self.url, **self.connection_options)
 
-    @retry_async(max_retries=3)
+    @retry(max_retries=3)
     async def _publish(self, message: CloudEvent, **kwargs) -> None:
         data = self.encoder.encode(message.dict())
-        await self.nc.publish(message.topic, data, **kwargs)
+        await self.client.publish(message.topic, data, **kwargs)
         if self._auto_flush:
-            await self.nc.flush()
+            await self.client.flush()
 
     @property
     def is_connected(self) -> bool:
-        return self.nc.is_connected
+        return self.client.is_connected
 
     Settings = NatsSettings
 
 
 class JetStreamBroker(NatsBroker):
     """
     NatsBroker with JetStream enabled
@@ -113,36 +108,26 @@
         **kwargs: Any,
     ) -> None:
 
         super().__init__(**kwargs)
         self.prefetch_count = prefetch_count
         self.fetch_timeout = fetch_timeout
         self.jetstream_options = jetstream_options or {}
-        self._js = None
-
-    @property
-    def js(self) -> JetStreamContext:
-        if not (self._nc and self._js):
-            raise BrokerError("Broker not connected")
-        return self._js
-
-    async def _connect(self) -> None:
-        await super()._connect()
-        self._js = self.nc.jetstream(**self.jetstream_options)
+        self.js = JetStreamContext(self.client, **self.jetstream_options)
 
-    @retry_async(max_retries=3)
+    @retry(max_retries=3)
     async def _publish(
         self,
         message: CloudEvent,
-        timeout: float | None = None,
-        stream: str | None = None,
-        headers: dict[str, str] | None = None,
+        **kwargs,
     ) -> None:
         data = self.encoder.encode(message)
-        headers = headers or {}
+        headers = kwargs.get("headers", {})
+        timeout = kwargs.get("timeout")
+        stream = kwargs.get("stream")
         headers.setdefault("Content-Type", self.encoder.CONTENT_TYPE)
         try:
             await self.js.publish(
                 subject=message.topic,
                 payload=data,
                 timeout=timeout,
                 stream=stream,
```

### Comparing `eventiq-0.1.4/eventiq/backends/nats/middlewares.py` & `eventiq-0.1.5/eventiq/backends/nats/plugins.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,86 +3,81 @@
 from typing import TYPE_CHECKING, Any
 
 from nats.js.errors import KeyNotFoundError
 from nats.js.kv import KeyValue
 
 from eventiq.backends.nats.broker import JetStreamBroker
 from eventiq.middleware import Middleware
-from eventiq.utils.functools import retry_async
+from eventiq.plugins import BrokerPlugin
+from eventiq.types import ID, ResultBackend
+from eventiq.utils.functools import retry
 
 if TYPE_CHECKING:
-    from eventiq.broker import Broker
-    from eventiq.consumer import Consumer
-    from eventiq.models import CloudEvent
-    from eventiq.types import Encoder
+    from eventiq import Broker, CloudEvent, Consumer, Service
 
 
-class NatsJetStreamResultMiddleware(Middleware):
-    def __init__(
-        self,
-        bucket: str,
-        encoder: Encoder | None = None,
-        store_exceptions: bool = False,
-        **kv_options: Any,
-    ):
-        self.bucket = bucket
-        self.store_exceptions = store_exceptions
-        if encoder is None:
-            from eventiq.encoders import get_default_encoder
+class _NatsJetStreamResultMiddleware(Middleware):
+    def __init__(self, result_backend: JetStreamResultBackend):
+        self.result_backend = result_backend
 
-            encoder = get_default_encoder()
-        self.encoder = encoder
-        self.options = kv_options
-        self._kv = None
-
-    @property
-    def kv(self) -> KeyValue:
-        if self._kv is None:
-            raise ValueError("Middleware not configured")
-        return self._kv
-
-    @retry_async(max_retries=3, backoff=5)
-    async def get(self, key: str) -> Any | None:
-        kv = await self.kv.get(key)
-        return self.encoder.decode(kv.value)
+    async def after_service_start(self, broker: Broker, service: Service):
+        self.result_backend.buckets[service.name] = await broker.js.create_key_value(  # type: ignore[attr-defined]
+            bucket=service.name, **self.result_backend.options
+        )
 
-    async def get_or_none(self, key: str):
-        try:
-            return await self.get(key)
-        except KeyNotFoundError:
-            self.logger.warning(f"Key {key} not found")
-            return None
-
-    async def get_message_result(
-        self, consumer_name: str, message_id: str
-    ) -> Any | None:
-        # TODO: timeout
-        return await self.get(f"{consumer_name}:{message_id}")
-
-    async def after_broker_connect(self, broker: Broker) -> None:
-        if isinstance(broker, JetStreamBroker):
-            self._kv = await broker.js.create_key_value(
-                bucket=self.bucket, **self.options
-            )
-        else:
-            self.logger.warning("Expected JetstreamBroker, got %s", type(broker))
-
-    @retry_async(max_retries=3, backoff=10)
+    @retry(max_retries=3, backoff=10)
     async def after_process_message(
         self,
-        broker: JetStreamBroker,
+        broker: Broker,
+        service: Service,
         consumer: Consumer,
         message: CloudEvent,
         result: Any | None = None,
         exc: Exception | None = None,
-    ):
+    ) -> None:
         """Store message result in JetStream K/V Store"""
-        if consumer.options.get("store_results"):
-            if exc is None:
+        if consumer.options.get("store_results", True) is False:
+            return
 
-                data = self.encoder.encode(result)
-                await self.kv.put(f"{consumer.name}:{message.id}", data)
-            elif exc and self.store_exceptions:
-                data = self.encoder.encode(
-                    {"type": type(exc).__name__, "detail": str(exc)}
-                )
-                await self.kv.put(f"{consumer.name}:{message.id}", data)
+        kv = self.result_backend.buckets.get(service.name)
+
+        if kv is None:
+            self.logger.warning(f"Bucket {service.name} not found")
+            return
+
+        if exc is None:
+            data = broker.encoder.encode(result)
+        elif exc and self.result_backend.store_exceptions:
+            data = broker.encoder.encode(
+                {"type": type(exc).__name__, "detail": str(exc)}
+            )
+        else:
+            return
+        await kv.put(str(message.id), data)
+
+
+class JetStreamResultBackend(BrokerPlugin[JetStreamBroker], ResultBackend):
+    def __init__(
+        self, broker: JetStreamBroker, store_exceptions: bool = False, **options: Any
+    ):
+        super().__init__(broker)
+        self.store_exceptions = store_exceptions
+        self.options = options
+        self.broker.add_middleware(_NatsJetStreamResultMiddleware(self))
+        self.buckets: dict[str, KeyValue] = {}
+
+    @retry(max_retries=3)
+    async def _get(self, kv: KeyValue, key: ID) -> Any:
+        return await kv.get(str(key))
+
+    async def get_result(self, service: str, message_id: ID) -> Any:
+        kv = self.buckets.get(service)
+        if kv is None:
+            self.logger.warning(f"Bucket {service} not found")
+            return
+
+        try:
+            data = await self._get(kv, message_id)
+            return self.broker.encoder.decode(data.value)
+        except KeyNotFoundError:
+            self.logger.warning(f"Key {message_id} not found")
+            return
```

### Comparing `eventiq-0.1.4/eventiq/backends/nats/settings.py` & `eventiq-0.1.5/eventiq/backends/nats/settings.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/backends/pubsub/broker.py` & `eventiq-0.1.5/eventiq/backends/pubsub/broker.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     SubscriberClient,
     SubscriberMessage,
     subscribe,
 )
 
 from eventiq.broker import Broker
 from eventiq.exceptions import BrokerError
-from eventiq.utils.functools import retry_async
+from eventiq.utils.functools import retry
 
 from .settings import PubSubSettings
 
 if TYPE_CHECKING:
     from eventiq import CloudEvent, Consumer, Service
 
 
@@ -58,25 +58,27 @@
 
     @property
     def client(self) -> PublisherClient:
         if self._client is None:
             raise BrokerError("Broker not connected")
         return self._client
 
-    @retry_async(max_retries=3)
+    @retry(max_retries=3)
     async def _publish(
         self,
         message: CloudEvent,
-        timeout: int = 10,
-        ordering_key: str | None = None,
-        **kwargs,
+        **kwargs: Any,
     ) -> None:
+        ordering_key = kwargs.get("ordering_key", str(message.id))
+        timeout = kwargs.get("timeout", 10)
         msg = PubsubMessage(
             data=self.encoder.encode(message.dict()),
-            ordering_key=ordering_key or message.id,
+            ordering_key=ordering_key,
+            content_type=self.encoder.CONTENT_TYPE,
+            **kwargs.get("headers"),
         )
         await self.client.publish(topic=message.topic, messages=[msg], timeout=timeout)
 
     async def _connect(self) -> None:
         self._client = PublisherClient(service_file=self.service_file)
 
     @property
```

### Comparing `eventiq-0.1.4/eventiq/backends/rabbitmq/broker.py` & `eventiq-0.1.5/eventiq/backends/rabbitmq/broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     Settings = RabbitMQSettings
 
     def __init__(
         self,
         *,
         url: str,
         default_prefetch_count: int = 10,
-        queue_options: dict[str, Any] = None,
+        queue_options: dict[str, Any] | None = None,
         exchange_name: str = "events",
         connection_options: dict[str, Any] | None = None,
         **kwargs: Any,
     ) -> None:
 
         super().__init__(**kwargs)
         self.url = url
```

### Comparing `eventiq-0.1.4/eventiq/backends/rabbitmq/middlewares.py` & `eventiq-0.1.5/eventiq/backends/rabbitmq/middlewares.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/backends/redis/broker.py` & `eventiq-0.1.5/eventiq/backends/redis/broker.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/backends/redis/middlewares.py` & `eventiq-0.1.5/eventiq/backends/redis/plugins.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
-from aioredis import Redis
+from eventiq import Middleware, Service
+from eventiq.plugins import BrokerPlugin
+from eventiq.types import ID, ResultBackend
+from eventiq.utils.functools import retry
 
-from eventiq import Middleware
-
-from ...utils.functools import retry_async
+from .broker import RedisBroker
 
 if TYPE_CHECKING:
-    from eventiq import Broker, CloudEvent, Consumer
-    from eventiq.types import Encoder
-
-    from .broker import RedisBroker
-
+    from eventiq import CloudEvent, Consumer
 
-class RedisResultMiddleware(Middleware):
-    def __init__(self, bucket: str, encoder: Encoder | None = None, ttl: int = 3600):
-        self.bucket = bucket
-        if encoder is None:
-            from eventiq.encoders import get_default_encoder
 
-            encoder = get_default_encoder()
-        self.encoder = encoder
+class _RedisResultMiddleware(Middleware):
+    def __init__(self, store_exceptions: bool, ttl: int):
+        self.store_exceptions = store_exceptions
         self.ttl = ttl
-        self._redis: Redis | None = None
 
-    @property
-    def redis(self) -> Redis:
-        assert self._redis
-        return self._redis
-
-    async def after_broker_connect(self, broker: RedisBroker) -> None:  # type: ignore[override]
-        assert isinstance(broker, RedisBroker)
-        self._redis = broker.redis
-
-    @retry_async(max_retries=3, backoff=10)
+    @retry(max_retries=3, backoff=10)
     async def after_process_message(
         self,
-        broker: Broker,
+        broker: RedisBroker,
+        service: Service,
         consumer: Consumer,
         message: CloudEvent,
         result: Any | None = None,
         exc: Exception | None = None,
     ) -> None:
-        if exc is None and consumer.options.get("store_results"):
-            data = self.encoder.encode(result)
-            ttl = consumer.options.get("result_ttl", self.ttl)
-            await self.redis.set(f"{consumer.name}:{message.id}", data, ex=ttl)
-
-    @retry_async(max_retries=3, backoff=5)
-    async def get_message_result(self, consumer_name: str, message_id: str):
-        value = await self.redis.get(f"{consumer_name}:{message_id}")
-        return self.encoder.decode(value)
+        if consumer.options.get("store_results", True) is False:
+            return
+
+        if exc is None:
+            data = broker.encoder.encode(result)
+
+        elif exc and self.store_exceptions:
+            data = broker.encoder.encode(
+                {"type": type(exc).__name__, "detail": str(exc)}
+            )
+        else:
+            return
+        await broker.redis.set(
+            f"{service.name}:{consumer.name}:{message.id}", data, ex=self.ttl
+        )
+
+
+class RedisResultBackend(BrokerPlugin[RedisBroker], ResultBackend):
+    def __init__(
+        self, broker: RedisBroker, store_exceptions: bool = False, ttl: int = 3600
+    ):
+        super().__init__(broker)
+        broker.add_middleware(_RedisResultMiddleware(store_exceptions, ttl))
+
+    async def get_result(self, service: str, message_id: ID):
+        res = await self.broker.redis.get(f"{service}:{message_id}")
+        if res:
+            return self.broker.encoder.decode(res)
```

### Comparing `eventiq-0.1.4/eventiq/backends/stub.py` & `eventiq-0.1.5/eventiq/backends/stub.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,9 +60,9 @@
 
     async def _ack(self, message: Message) -> None:
         message.queue.task_done()
 
     async def _nack(self, message: Message) -> None:
         await message.queue.put(message)
 
-    def is_connected(self) -> bool:
+    def is_connected(self) -> bool:  # type: ignore[override]
         return True
```

### Comparing `eventiq-0.1.4/eventiq/broker.py` & `eventiq-0.1.5/eventiq/broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,30 @@
 from __future__ import annotations
 
 import asyncio
 import functools
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Awaitable, Callable, Generic, Type, cast
 
-import async_timeout
 from pydantic import ValidationError
 
+from .context import _current_message, _current_service
 from .exceptions import DecodeError, Fail, Skip
 from .logger import LoggerMixin
 from .message import Message
 from .middleware import Middleware
 from .models import CloudEvent
 from .settings import BrokerSettings
 from .types import Encoder, RawMessage
 
 if TYPE_CHECKING:
     from eventiq import Consumer, Service
 
 
-class AbstractBroker(ABC, Generic[RawMessage]):
-    @abstractmethod
-    def parse_incoming_message(self, message: RawMessage) -> Any:
-        raise NotImplementedError
-
-    @property
-    @abstractmethod
-    def is_connected(self) -> bool:
-        """Return broker connection status"""
-        raise NotImplementedError
-
-    @abstractmethod
-    async def _publish(self, message: CloudEvent, **kwargs) -> None:
-        raise NotImplementedError
-
-    @abstractmethod
-    async def _connect(self) -> None:
-        raise NotImplementedError
-
-    @abstractmethod
-    async def _disconnect(self) -> None:
-        raise NotImplementedError
-
-    @abstractmethod
-    async def _start_consumer(self, service: Service, consumer: Consumer) -> None:
-        raise NotImplementedError
-
-    async def _ack(self, message: Message) -> None:
-        """Empty default implementation for backends that do not support explicit ack"""
-
-    async def _nack(self, message: Message) -> None:
-        """Same as for ._ack()"""
-
-
-class Broker(AbstractBroker[RawMessage], LoggerMixin, ABC):
+class Broker(Generic[RawMessage], LoggerMixin, ABC):
     """Base broker class
     :param description: Broker (Server) Description
     :param encoder: Encoder (Serializer) class
     :param middlewares: Optional list of middlewares
     """
 
     protocol: str
@@ -92,58 +58,65 @@
     def get_handler(
         self, service: Service, consumer: Consumer
     ) -> Callable[[RawMessage], Awaitable[Any | None]]:
         async def handler(raw_message: RawMessage) -> None:
             exc: Exception | None = None
             result: Any = None
             msg = self.message_proxy_class(raw_message)
+            s_token = _current_service.set(service)
             try:
                 parsed = self.parse_incoming_message(raw_message)
                 message = consumer.validate_message(parsed)
                 message.set_raw(msg)
             except (DecodeError, ValidationError) as e:
                 self.logger.exception("Message parsing error", exc_info=e)
                 msg.fail()
                 await self.ack(service, consumer, msg)
                 return
-
+            m_token = _current_message.set(message)
             try:
                 await self.dispatch_before(
                     "process_message", service, consumer, message
                 )
             except Skip:
                 self.logger.info(f"Skipped message {message.id}")
                 await self.dispatch_after("skip_message", service, consumer, message)
                 await self.ack(service, consumer, msg)
                 return
             try:
-                async with async_timeout.timeout(consumer.timeout):
-                    self.logger.info(f"Running consumer {consumer.name}")
-                    result = await consumer.process(message)
+                self.logger.info(
+                    f"Running consumer {consumer.name} with message {message.id}"
+                )
+                result = await asyncio.wait_for(
+                    consumer.process(message), timeout=consumer.timeout
+                )
                 if consumer.forward_response and result is not None:
                     await self.publish_event(
                         CloudEvent(
                             type=consumer.forward_response.as_type,
                             topic=consumer.forward_response.topic,
                             data=result,
                             source=service.name,
                         )
                     )
             # TODO: asyncio.CanceledError handling (?)
             except Exception as e:
                 self.logger.error(f"Exception in {consumer.name} {e}")
                 exc = e
             finally:
+                self.logger.info(f"Finished running consumer {consumer.name}")
                 await self.dispatch_after(
                     "process_message", service, consumer, message, result, exc
                 )
                 if exc is None or isinstance(exc, Fail) or msg.failed:
                     await self.ack(service, consumer, msg)
                 else:
                     await self.nack(service, consumer, msg)
+                _current_service.reset(s_token)
+                _current_message.reset(m_token)
 
         return handler
 
     async def ack(self, service: Service, consumer: Consumer, message: Message) -> None:
         await self.dispatch_before("ack", service, consumer, message)
         await self._ack(message)
         await self.dispatch_after("ack", service, consumer, message)
@@ -262,7 +235,39 @@
 
     @classmethod
     def from_env(
         cls,
         **kwargs,
     ) -> Broker:
         return cls.from_settings(BrokerSettings(), **kwargs)
+
+    @abstractmethod
+    def parse_incoming_message(self, message: RawMessage) -> Any:
+        raise NotImplementedError
+
+    @property
+    @abstractmethod
+    def is_connected(self) -> bool:
+        """Return broker connection status"""
+        raise NotImplementedError
+
+    @abstractmethod
+    async def _publish(self, message: CloudEvent, **kwargs) -> None:
+        raise NotImplementedError
+
+    @abstractmethod
+    async def _connect(self) -> None:
+        raise NotImplementedError
+
+    @abstractmethod
+    async def _disconnect(self) -> None:
+        raise NotImplementedError
+
+    @abstractmethod
+    async def _start_consumer(self, service: Service, consumer: Consumer) -> None:
+        raise NotImplementedError
+
+    async def _ack(self, message: Message) -> None:
+        """Empty default implementation for backends that do not support explicit ack"""
+
+    async def _nack(self, message: Message) -> None:
+        """Same as for ._ack()"""
```

### Comparing `eventiq-0.1.4/eventiq/cli.py` & `eventiq-0.1.5/eventiq/cli.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/config/models.py` & `eventiq-0.1.5/eventiq/config/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, Extra
 
 from eventiq.consumer import FnConsumer, GenericConsumer
 from eventiq.types import TagMeta
 from eventiq.utils.imports import ImportedType
 
@@ -33,37 +33,39 @@
     class Config:
         extra = Extra.allow
 
 
 class BrokerConfig(TypedModel):
     encoder: TypedModel
     middlewares: List[TypedModel]
+    context: dict[str, Union[TypedModel, Any]] = {}
 
 
 class ConsumerConfig(TypedModel):
     topic: str
     name: Optional[str]
-    timeout: Optional[int]
+    timeout: int = 120
     dynamic: bool = False
 
     def build(self):
         if callable(self.type) and not (
             isinstance(self.type, type) and issubclass(self.type, GenericConsumer)
         ):
             self.__dict__["fn"] = self.type
             self.type = FnConsumer
         return super().build()
 
 
 class ServiceConfig(BaseModel):
     name: str
+    broker: str = "default"
     title: Optional[str]
     version: str = "0.1.0"
     description: str = ""
     tags_metadata: List[TagMeta] = []
     instance_id_generator: Optional[ImportedType]
     consumers: List[ConsumerConfig]
 
 
 class AppConfig(BaseModel):
-    broker: BrokerConfig
+    brokers: Dict[str, BrokerConfig]
     services: List[ServiceConfig]
```

### Comparing `eventiq-0.1.4/eventiq/consumer.py` & `eventiq-0.1.5/eventiq/consumer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import asyncio
+import inspect
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Any, Generic, get_type_hints
+from typing import Any, Callable, Generic, get_type_hints
 
-from .defaults import DEFAULT_CONSUMER_TIME_LIMIT
 from .logger import get_logger
 from .types import FT, MessageHandlerT, T
-from .utils.functools import run_async
+from .utils.functools import to_async
 
 
 @dataclass(frozen=True)
 class ForwardResponse:
     topic: str
     as_type: str = "CloudEvent"
 
@@ -23,15 +23,15 @@
     event_type: T
 
     def __init__(
         self,
         *,
         topic: str,
         name: str,
-        timeout: int = DEFAULT_CONSUMER_TIME_LIMIT,
+        timeout: int = 120,
         dynamic: bool = False,
         forward_response: ForwardResponse | None = None,
         **options: Any,
     ):
         self._name = name
         self.topic = topic
         self.timeout = timeout
@@ -49,15 +49,15 @@
 
     @property
     @abstractmethod
     def description(self) -> str:
         raise NotImplementedError
 
     @abstractmethod
-    async def process(self, message: T):
+    async def process(self, message: T) -> Any | None:
         raise NotImplementedError
 
 
 class FnConsumer(Consumer[T]):
     def __init__(
         self,
         *,
@@ -67,15 +67,15 @@
         **options: Any,
     ) -> None:
         super().__init__(name=name or fn.__name__, topic=topic, **options)
         event_type = get_type_hints(fn).get("message")
         assert event_type, f"Unable to resolve type hint for 'message' in {fn.__name__}"
         self.event_type = event_type
         if not asyncio.iscoroutinefunction(fn):
-            fn = run_async(fn)
+            fn = to_async(fn)
         self.fn = fn
 
     async def process(self, message: T) -> Any | None:
         self.logger.info("Processing message <%s>", message.type)
         result = await self.fn(message)
         self.logger.info("Finished processing <%s>", message.type)
         return result
@@ -91,20 +91,16 @@
         super().__init__(
             name=name or str(getattr(type(self), "name", type(self).__name__)),
             topic=topic,
             **options,
         )
 
     def __init_subclass__(cls, **kwargs):
-        if "abstract" not in kwargs:
-            cls.event_type = cls.__orig_bases__[0].__args__[0]
-            if not hasattr(cls, "name"):
-                cls.name = cls.__name__
-            if not asyncio.iscoroutinefunction(cls.process):
-                cls.process = run_async(cls.process)
+        if not inspect.isabstract(cls) and not asyncio.iscoroutinefunction(cls.process):
+            cls.process = to_async(cls.process)
 
     @property
     def description(self) -> str:
         return self.__doc__ or ""
 
 
 class ConsumerGroup:
@@ -122,15 +118,15 @@
         topic: str,
         *,
         name: str | None = None,
         timeout: int = 120,
         dynamic: bool = False,
         forward_response: ForwardResponse | None = None,
         **options,
-    ):
+    ) -> Callable[[MessageHandlerT], MessageHandlerT]:
         def wrapper(func_or_cls: MessageHandlerT) -> MessageHandlerT:
             cls: type[Consumer] = FnConsumer
             if isinstance(func_or_cls, type) and issubclass(
                 func_or_cls, GenericConsumer
             ):
                 cls = func_or_cls
             elif callable(func_or_cls):
```

### Comparing `eventiq-0.1.4/eventiq/encoders/json.py` & `eventiq-0.1.5/eventiq/encoders/json.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/encoders/msgpack.py` & `eventiq-0.1.5/eventiq/encoders/msgpack.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/encoders/orjson.py` & `eventiq-0.1.5/eventiq/encoders/orjson.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/exceptions.py` & `eventiq-0.1.5/eventiq/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from __future__ import annotations
 
 
 class ConfigurationError(Exception):
     """Raised by framework when invalid configuration is supplied"""
 
 
-class PluginLoadError(ImportError):
-    """Raised when unable to load plugin"""
-
-
 class BrokerError(Exception):
     """Base Exception for broker related errors"""
 
 
 class PublishError(BrokerError):
     """Raised when publishing a message fails"""
```

### Comparing `eventiq-0.1.4/eventiq/logger.py` & `eventiq-0.1.5/eventiq/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import inspect
 import logging
 from typing import Type, Union
 
 from pythonjsonlogger import jsonlogger
 
-from eventiq.utils.datetime import utc_now
+from .context import get_current_message
+from .utils.datetime import utc_now
 
 
 class EventiqJsonFormatter(jsonlogger.JsonFormatter):
     def add_fields(self, log_record, record, message_dict):
         super().add_fields(log_record, record, message_dict)
         if "timestamp" not in log_record:
             log_record["timestamp"] = utc_now()
 
+        msg = get_current_message()
+        if msg:
+            log_record.update(msg.log_context)
+
         log_record["level"] = record.levelname.upper()
 
 
 def setup_logging(level, fmt: str = "%(name) %(level) %(message)") -> None:
     handler = logging.StreamHandler()
     handler.setFormatter(EventiqJsonFormatter(fmt))
     logging.basicConfig(handlers=[handler], level=level)
```

### Comparing `eventiq-0.1.4/eventiq/message.py` & `eventiq-0.1.5/eventiq/message.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/middleware.py` & `eventiq-0.1.5/eventiq/middleware.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/middlewares/debug.py` & `eventiq-0.1.5/eventiq/middlewares/debug.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/middlewares/error.py` & `eventiq-0.1.5/eventiq/middlewares/error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING, Any
 
 from eventiq.middleware import Middleware
-from eventiq.utils.functools import run_async
+from eventiq.utils.functools import to_async
 
 if TYPE_CHECKING:
     from eventiq import Broker, CloudEvent, Consumer, Service
 
 
 class ErrorHandlerMiddleware(Middleware):
     def __init__(self, errors: type[Exception] | tuple[type[Exception]], callback):
         if not asyncio.iscoroutinefunction(callback):
-            callback = run_async(callback)
+            callback = to_async(callback)
         self.cb = callback
         self.exc = errors
 
     async def after_process_message(
         self,
         broker: Broker,
         service: Service,
```

### Comparing `eventiq-0.1.4/eventiq/middlewares/healthcheck.py` & `eventiq-0.1.5/eventiq/middlewares/healthcheck.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 from __future__ import annotations
 
 import asyncio
 import os
 from pathlib import Path
-from typing import TYPE_CHECKING, Awaitable, Callable, Sequence
+from typing import TYPE_CHECKING
 
 from eventiq.middleware import Middleware
 
 if TYPE_CHECKING:
     from eventiq.broker import Broker
 
 
 class HealthCheckMiddleware(Middleware):
     """Middleware for performing basic health checks on broker"""
 
     BASE_DIR = os.getenv("HEALTHCHECK_DIR", "/tmp")  # nosec
 
-    def __init__(
-        self,
-        interval: int = 30,
-        file_mode: bool = False,
-        checkers: Sequence[Callable[..., Awaitable[bool]]] | None = None,
-    ):
+    def __init__(self, interval: int = 30, file_mode: bool = False):
         self.interval = interval
         self.file_mode = file_mode
-        self._checkers = checkers
         self._broker: Broker | None = None
         self._task: asyncio.Task | None = None
 
     async def after_broker_connect(self, broker: Broker):
         self._broker = broker
         if self.file_mode:
             self._task = asyncio.create_task(self._run_forever())
@@ -39,15 +33,21 @@
             await self._task
 
     async def _run_forever(self):
         p = Path(os.path.join(self.BASE_DIR, "healthy"))
         p.touch(exist_ok=True)
         try:
             while True:
-                if not self.get_health_status():
+                try:
+                    unhealthy = not self._broker.is_connected
+                except Exception as e:
+                    self.logger.exception("Healthcheck failed", exc_info=e)
+                    unhealthy = True
+
+                if unhealthy:
                     p.rename(os.path.join(self.BASE_DIR, "unhealthy"))
                     break
                 await asyncio.sleep(self.interval)
         except asyncio.CancelledError:
             pass
 
     def get_health_status(self) -> bool:
```

### Comparing `eventiq-0.1.4/eventiq/middlewares/opentelemetry.py` & `eventiq-0.1.5/eventiq/middlewares/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/middlewares/prometheus.py` & `eventiq-0.1.5/eventiq/middlewares/prometheus.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/middlewares/retries.py` & `eventiq-0.1.5/eventiq/middlewares/retries.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/models.py` & `eventiq-0.1.5/eventiq/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from datetime import datetime, timedelta
 from typing import Any, Dict, Generic, Optional
 
 from pydantic import Extra, Field, validator
 from pydantic.fields import PrivateAttr
 from pydantic.generics import GenericModel
 
+from .context import get_current_service
 from .message import Message
 from .types import ID, D
 from .utils import str_uuid
 from .utils.datetime import utc_now
 
 
 class CloudEvent(GenericModel, Generic[D]):
     specversion: Optional[str] = "1.0"
     content_type: str = Field("application/json", alias="datacontenttype")
     id: ID = Field(default_factory=str_uuid)
     time: datetime = Field(default_factory=utc_now)
     topic: str = Field(..., alias="subject")
     type: Optional[str] = None
     source: Optional[str] = None
-    data: Optional[D] = None
+    data: D
     trace_ctx: Dict[str, str] = {}
 
     _raw: Optional[Any] = PrivateAttr()
 
     def __eq__(self, other):
         if not isinstance(other, CloudEvent):
             return False
@@ -35,29 +36,37 @@
 
     @property
     def raw(self) -> Message:
         if self._raw is None:
             raise AttributeError("raw property accessible only for incoming messages")
         return self._raw
 
+    @property
+    def service(self):
+        return get_current_service()
+
+    @property
+    def log_context(self) -> Dict[str, Any]:
+        return {"message_id": str(self.id)}
+
     def _set(self, name: str, value: Any):
         object.__setattr__(self, name, value)
 
     def set_source(self, value: str) -> None:
         self._set("source", value)
 
     def set_raw(self, value: Message):
         self._set("_raw", value)
 
     def dict(self, **kwargs: Any) -> Dict[str, Any]:
         kwargs.setdefault("by_alias", True)
         return super().dict(**kwargs)
 
     @classmethod
-    def new(cls, obj: D, **kwargs):
+    def new(cls, obj: D, **kwargs: Any):
         return cls(data=obj, **kwargs)
 
     @property
     def age(self) -> timedelta:
         return utc_now() - self.time
 
     def fail(self):
```

### Comparing `eventiq-0.1.4/eventiq/runner.py` & `eventiq-0.1.5/eventiq/runner.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/service.py` & `eventiq-0.1.5/eventiq/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING, Any, Callable
 
 from .consumer import Consumer, ConsumerGroup, ForwardResponse
-from .defaults import DEFAULT_CONSUMER_TIME_LIMIT
 from .logger import LoggerMixin
 from .models import CloudEvent
 from .settings import ServiceSettings
 from .utils import generate_instance_id
 
 if TYPE_CHECKING:
     from .broker import Broker
@@ -23,32 +22,34 @@
         name: str,
         broker: Broker,
         title: str | None = None,
         version: str = "0.1.0",
         description: str = "",
         tags_metadata: list[TagMeta] | None = None,
         instance_id_generator: Callable[[], str] | None = None,
+        **context: Any,
     ):
         self.broker = broker
         self.name = name
         self.title = title or name.title()
         self.version = version
         self.description = description
         self.tags_metadata = tags_metadata or []
         self.id = (instance_id_generator or generate_instance_id)()
         self.consumer_group = ConsumerGroup()
+        self.context = context
         # TODO: task gathering?
         self._tasks: list[asyncio.Task] = []
 
     def subscribe(
         self,
         topic: str,
         *,
         name: str | None = None,
-        timeout: int = DEFAULT_CONSUMER_TIME_LIMIT,
+        timeout: int = 120,
         dynamic: bool = False,
         forward_response: ForwardResponse | None = None,
         **options,
     ):
         return self.consumer_group.subscribe(
             topic=topic,
             name=name,
@@ -80,16 +81,16 @@
 
     async def publish_event(self, message: CloudEvent, **kwargs):
         if not message.source:
             message.set_source(self.name)
         return await self.broker.publish_event(message, **kwargs)
 
     async def start(self):
-        await self.broker.dispatch_before("service_start", self)
         await self.broker.connect()
+        await self.broker.dispatch_before("service_start", self)
         for consumer in self.consumers.values():
             asyncio.create_task(self.broker.start_consumer(self, consumer))
         await self.broker.dispatch_after("service_start", self)
 
     async def stop(self, *args, **kwargs):
         await self.broker.dispatch_before("service_stop", self)
         await self.broker.disconnect()
```

### Comparing `eventiq-0.1.4/eventiq/settings.py` & `eventiq-0.1.5/eventiq/settings.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/eventiq/types.py` & `eventiq-0.1.5/eventiq/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     TypedDict,
     TypeVar,
     Union,
 )
 from uuid import UUID
 
 if TYPE_CHECKING:
-    from eventiq import CloudEvent, GenericConsumer
+    from . import CloudEvent, GenericConsumer
 
-ID = Union[str, int, UUID]
+ID = Union[UUID, int, str]
 
 
 RawMessage = TypeVar("RawMessage")
 
 T = TypeVar("T", bound="CloudEvent")
 D = TypeVar("D")
 
@@ -49,11 +49,16 @@
         """
         Deserialize bytes to python object
         :param data: input bytes
         :return: de-serialized object
         """
 
 
-FT = Callable[["CloudEvent"], Awaitable[Optional[Any]]]
+FT = Callable[["CloudEvent"], Union[Awaitable[Optional[Any]], Optional[Any]]]
 MessageHandlerT = Union[Type["GenericConsumer"], FT]
 
 ExcHandler = Callable[["CloudEvent", Exception], Awaitable]
+
+
+class ResultBackend(Protocol):
+    async def get_result(self, service: str, message_id: ID) -> Any | None:
+        ...
```

### Comparing `eventiq-0.1.4/eventiq/utils/functools.py` & `eventiq-0.1.5/eventiq/utils/functools.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,66 @@
 from __future__ import annotations
 
 import asyncio
 import functools
-from typing import Any, Awaitable, Callable
+import time
+from typing import Any, Awaitable, Callable, TypeVar
 
-CF = Callable[..., Awaitable[Any]]
+from typing_extensions import ParamSpec
 
+P = ParamSpec("P")
+R = TypeVar("R", bound=Any)
 
-def run_async(func: Callable[..., Any]) -> CF:
+
+def to_async(func: Callable[P, R]) -> Callable[P, Awaitable[R]]:
     @functools.wraps(func)
-    def wrapper(*args, **kwargs):
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> Awaitable[R]:
         loop = asyncio.get_running_loop()
         return loop.run_in_executor(None, functools.partial(func, *args, **kwargs))
 
     return wrapper
 
 
-def retry_async(max_retries: int = 5, backoff: int = 2):
-    def wrapper(func):
-        @functools.wraps(func)
-        async def wrapped(*args, **kwargs):
-            exc = None
-            for i in range(1, max_retries + 1):
-                try:
-                    return await func(*args, **kwargs)
-                except Exception as e:
-                    exc = e
-                    await asyncio.sleep(i**backoff)
-            else:
-                raise exc
+def _retry_async(
+    func: Callable[P, Awaitable[R]] | Callable[P, R], max_retries: int, backoff: int
+) -> Callable[P, R] | Callable[P, Awaitable[R]]:
+    @functools.wraps(func)
+    async def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
+        exc = None
+        for i in range(1, max_retries + 1):
+            try:
+                return await func(*args, **kwargs)
+            except Exception as e:
+                exc = e
+                await asyncio.sleep(backoff**i)
+        else:
+            raise exc  # type: ignore
 
-        return wrapped
+    return wrapper
+
+
+def _retry_sync(func: Callable[P, R], max_retries: int, backoff: int) -> Callable[P, R]:
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        exc = None
+        for i in range(1, max_retries + 1):
+            try:
+                return func(*args, **kwargs)
+            except Exception as e:
+                exc = e
+                time.sleep(i**backoff)
+        raise exc
 
     return wrapper
+
+
+def retry(max_retries: int = 5, backoff: int = 2):
+    def _wrapper(
+        func: Callable[P, R] | Callable[P, Awaitable[R]]
+    ) -> Callable[P, R] | Callable[P, Awaitable[R]]:
+
+        if asyncio.iscoroutinefunction(func):
+            return _retry_async(func, max_retries, backoff)
+
+        return _retry_sync(func, max_retries, backoff)
+
+    return _wrapper
```

### Comparing `eventiq-0.1.4/eventiq/utils/imports.py` & `eventiq-0.1.5/eventiq/utils/imports.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.4/pyproject.toml` & `eventiq-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventiq"
-version = "0.1.4"
+version = "0.1.5"
 description = "Cloud native framework for building event driven applications in Python."
 authors = ["Radzim Kowalow <radzim.kowalow@performance-media.pl>"]
 readme = "README.md"
 license = "Apache License 2.0"
 documentation = "https://performancemedia.github.io/eventiq/"
 repository = "https://github.com/performancemedia/eventiq"
 classifiers = [
@@ -30,43 +30,41 @@
 
 [tool.poetry.scripts]
 eventiq = "eventiq.cli:cli"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 pydantic = ">=1.0"
-async-timeout = ">=4.0"
 python-json-logger = ">=2.0"
 
 # cli
 aiorun = {version = "^2022.11.1", optional = true}
 typer = {version = ">=0.7.0", optional = true}
 
 # monitoring
 prometheus-client = {version = ">=0.16.0,<1.0", optional = true}
 opentelemetry-api = {version = "^1.17.0", optional = true}
 opentelemetry-sdk = {version = "^1.17.0", optional = true}
 opentelemetry-semantic-conventions = {version = "^0.38b0", optional = true}
 # encoders
-orjson = {version = ">=3.8.7,<4.0", optional = true}
+orjson = {version = ">=3.2.1,<=3.8.9", optional = true}
 ormsgpack = {version = ">=1.2.5,<2.0", optional = true}
 
 # brokers
 aio-pika = {version = ">=9.0.4", optional = true}
 nats-py = {version = ">=2.2,<3.0", optional = true}
 aiokafka = {version = ">=0.8,<1.0", optional = true}
 aioredis = {version = ">=2.0,<3.0", optional = true}
 gcloud-aio-pubsub = {version = ">=5.2.0,<6.0", optional = true}
 
 [tool.poetry.extras]
-all = ["aiorun", "typer", "prometheus-client", "orjson", "ormsgpack", "nats-py", "aioredis",
-    "aiokafka", "aio-pika", "gcloud-aio-pubsub",
-    "opentelemetry-api", "opentelemetry-sdk", "opentelemetry-semantic-conventions"
+all = ["aiorun", "typer", "prometheus-client", "orjson", "ormsgpack", "nats-py", "aioredis", "aiokafka", "aio-pika",
+    "gcloud-aio-pubsub", "opentelemetry-api", "opentelemetry-sdk", "opentelemetry-semantic-conventions"
 ]
-common = ["aiorun", "typer", "prometheus-client", "orjson", "opentelemetry-api", "opentelemetry-sdk", "opentelemetry-semantic-conventions"]
+common = ["aiorun", "typer", "prometheus-client", "orjson"]
 cli = ["aiorun", "typer"]
 
 # encoders
 orjson = ["orjson"]
 ormsgpack = ["ormsgpack"]
 # observability
 prometheus = ["prometheus-client"]
@@ -78,15 +76,15 @@
 redis = ["aioredis"]
 pubsub = ["gcloud-aio-pubsub"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.2"
 pytest-cov = "^4.0.0"
-mypy = "^0.961"
+mypy = "^1.2.0"
 black = "^22.3.0"
 isort = "^5.10.1"
 tox = "^3.25.0"
 bandit = "^1.7.4"
 fastapi = "^0.87.0"
 uvicorn = "^0.19.0"
 watchfiles = "^0.18.1"
@@ -112,15 +110,15 @@
 addopts = "--cov=./eventiq"
 testpaths = [
    "./tests"
 ]
 asyncio_mode = "auto"
 
 [tool.mypy]
-python_version = 3.9
+python_version = "3.11"
 namespace_packages = true
 ignore_missing_imports = true
 no_site_packages = true
 
 [tool.isort]
 profile = "black"
```

### Comparing `eventiq-0.1.4/PKG-INFO` & `eventiq-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventiq
-Version: 0.1.4
+Version: 0.1.5
 Summary: Cloud native framework for building event driven applications in Python.
 Home-page: https://github.com/performancemedia/eventiq
 License: Apache-2.0
 Keywords: framework,asyncio,microservice,event-driven
 Author: Radzim Kowalow
 Author-email: radzim.kowalow@performance-media.pl
 Requires-Python: >=3.8.1,<4.0
@@ -35,21 +35,20 @@
 Provides-Extra: pubsub
 Provides-Extra: rabbitmq
 Provides-Extra: redis
 Requires-Dist: aio-pika (>=9.0.4) ; extra == "all" or extra == "rabbitmq"
 Requires-Dist: aiokafka (>=0.8,<1.0) ; extra == "all" or extra == "kafka"
 Requires-Dist: aioredis (>=2.0,<3.0) ; extra == "all" or extra == "redis"
 Requires-Dist: aiorun (>=2022.11.1,<2023.0.0) ; extra == "all" or extra == "common" or extra == "cli"
-Requires-Dist: async-timeout (>=4.0)
 Requires-Dist: gcloud-aio-pubsub (>=5.2.0,<6.0) ; extra == "all" or extra == "pubsub"
 Requires-Dist: nats-py (>=2.2,<3.0) ; extra == "all" or extra == "nats"
-Requires-Dist: opentelemetry-api (>=1.17.0,<2.0.0) ; extra == "all" or extra == "common" or extra == "opentelemetry"
-Requires-Dist: opentelemetry-sdk (>=1.17.0,<2.0.0) ; extra == "all" or extra == "common" or extra == "opentelemetry"
-Requires-Dist: opentelemetry-semantic-conventions (>=0.38b0,<0.39) ; extra == "all" or extra == "common" or extra == "opentelemetry"
-Requires-Dist: orjson (>=3.8.7,<4.0) ; extra == "all" or extra == "common" or extra == "orjson"
+Requires-Dist: opentelemetry-api (>=1.17.0,<2.0.0) ; extra == "all" or extra == "opentelemetry"
+Requires-Dist: opentelemetry-sdk (>=1.17.0,<2.0.0) ; extra == "all" or extra == "opentelemetry"
+Requires-Dist: opentelemetry-semantic-conventions (>=0.38b0,<0.39) ; extra == "all" or extra == "opentelemetry"
+Requires-Dist: orjson (>=3.2.1,<=3.8.9) ; extra == "all" or extra == "common" or extra == "orjson"
 Requires-Dist: ormsgpack (>=1.2.5,<2.0) ; extra == "all" or extra == "ormsgpack"
 Requires-Dist: prometheus-client (>=0.16.0,<1.0) ; extra == "all" or extra == "common" or extra == "prometheus"
 Requires-Dist: pydantic (>=1.0)
 Requires-Dist: python-json-logger (>=2.0)
 Requires-Dist: typer (>=0.7.0) ; extra == "all" or extra == "common" or extra == "cli"
 Project-URL: Documentation, https://performancemedia.github.io/eventiq/
 Project-URL: Repository, https://github.com/performancemedia/eventiq
@@ -72,24 +71,24 @@
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 *Note: This package is under active development and is not recommended for production use*
 
 ---
-Version: 0.1.4
+Version: 0.1.5
 
 Documentation: https://performancemedia.github.io/eventiq/
 
 Repository: https://github.com/performancemedia/eventiq
 
 ---
 ## About
 
-The package utilizes `pydantic`, `async_timeout` and `python-json-logger` as the only required dependencies.
+The package utilizes `pydantic` and `python-json-logger` as the only required dependencies.
 For messages [Cloud Events](https://cloudevents.io/) format is used.
 Service can be run as standalone processes, or included into starlette (e.g. FastAPI) applications.
 
 ## Installation
 
 ```shell
 pip install eventiq
```

