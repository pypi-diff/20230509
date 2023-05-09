# Comparing `tmp/granian-0.3.2.tar.gz` & `tmp/granian-0.4.0.tar.gz`

## Comparing `granian-0.3.2.tar` & `granian-0.4.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 granian-0.3.2/Cargo.toml
--rw-r--r--   0     1001      123     1486 2023-05-02 22:06:38.000000 granian-0.3.2/LICENSE
--rw-r--r--   0     1001      123     1846 2023-05-02 22:06:38.000000 granian-0.3.2/README.md
--rw-r--r--   0     1001      123       54 2023-05-02 22:06:38.000000 granian-0.3.2/build.rs
--rw-r--r--   0     1001      123       28 2023-05-02 22:06:38.000000 granian-0.3.2/granian/__init__.py
--rw-r--r--   0     1001      123       22 2023-05-02 22:06:38.000000 granian-0.3.2/granian/__version__.py
--rw-r--r--   0     1001      123      275 2023-05-02 22:06:38.000000 granian-0.3.2/granian/_futures.py
--rw-r--r--   0     1001      123     1868 2023-05-02 22:06:38.000000 granian-0.3.2/granian/_granian.pyi
--rw-r--r--   0     1001      123     1677 2023-05-02 22:06:38.000000 granian-0.3.2/granian/_internal.py
--rw-r--r--   0     1001      123     2862 2023-05-02 22:06:38.000000 granian-0.3.2/granian/_loops.py
--rw-r--r--   0     1001      123       93 2023-05-02 22:06:38.000000 granian-0.3.2/granian/_types.py
--rw-r--r--   0     1001      123     4909 2023-05-02 22:06:38.000000 granian-0.3.2/granian/asgi.py
--rw-r--r--   0     1001      123     3015 2023-05-02 22:06:38.000000 granian-0.3.2/granian/cli.py
--rw-r--r--   0     1001      123      357 2023-05-02 22:06:38.000000 granian-0.3.2/granian/constants.py
--rw-r--r--   0     1001      123     1328 2023-05-02 22:06:38.000000 granian-0.3.2/granian/log.py
--rw-r--r--   0     1001      123      153 2023-05-02 22:06:38.000000 granian-0.3.2/granian/net.py
--rw-r--r--   0     1001      123        0 2023-05-02 22:06:38.000000 granian-0.3.2/granian/py.typed
--rw-r--r--   0     1001      123      840 2023-05-02 22:06:38.000000 granian-0.3.2/granian/rsgi.py
--rw-r--r--   0     1001      123    10718 2023-05-02 22:06:38.000000 granian-0.3.2/granian/server.py
--rw-r--r--   0     1001      123     2068 2023-05-02 22:06:38.000000 granian-0.3.2/granian/wsgi.py
--rw-r--r--   0     1001      123     1633 2023-05-02 22:06:38.000000 granian-0.3.2/pyproject.toml
--rw-r--r--   0     1001      123     5747 2023-05-02 22:06:38.000000 granian-0.3.2/src/asgi/callbacks.rs
--rw-r--r--   0     1001      123     1611 2023-05-02 22:06:38.000000 granian-0.3.2/src/asgi/errors.rs
--rw-r--r--   0     1001      123     4605 2023-05-02 22:06:38.000000 granian-0.3.2/src/asgi/http.rs
--rw-r--r--   0     1001      123    15092 2023-05-02 22:06:38.000000 granian-0.3.2/src/asgi/io.rs
--rw-r--r--   0     1001      123      329 2023-05-02 22:06:38.000000 granian-0.3.2/src/asgi/mod.rs
--rw-r--r--   0     1001      123     2735 2023-05-02 22:06:38.000000 granian-0.3.2/src/asgi/serve.rs
--rw-r--r--   0     1001      123     2708 2023-05-02 22:06:38.000000 granian-0.3.2/src/asgi/types.rs
--rw-r--r--   0     1001      123     4835 2023-05-02 22:06:38.000000 granian-0.3.2/src/callbacks.rs
--rw-r--r--   0     1001      123      415 2023-05-02 22:06:38.000000 granian-0.3.2/src/http.rs
--rw-r--r--   0     1001      123      550 2023-05-02 22:06:38.000000 granian-0.3.2/src/lib.rs
--rw-r--r--   0     1001      123     4921 2023-05-02 22:06:38.000000 granian-0.3.2/src/rsgi/callbacks.rs
--rw-r--r--   0     1001      123      565 2023-05-02 22:06:38.000000 granian-0.3.2/src/rsgi/errors.rs
--rw-r--r--   0     1001      123     5026 2023-05-02 22:06:38.000000 granian-0.3.2/src/rsgi/http.rs
--rw-r--r--   0     1001      123    10269 2023-05-02 22:06:38.000000 granian-0.3.2/src/rsgi/io.rs
--rw-r--r--   0     1001      123      609 2023-05-02 22:06:38.000000 granian-0.3.2/src/rsgi/mod.rs
--rw-r--r--   0     1001      123     2735 2023-05-02 22:06:38.000000 granian-0.3.2/src/rsgi/serve.rs
--rw-r--r--   0     1001      123     5607 2023-05-02 22:06:38.000000 granian-0.3.2/src/rsgi/types.rs
--rw-r--r--   0     1001      123     8066 2023-05-02 22:06:38.000000 granian-0.3.2/src/runtime.rs
--rw-r--r--   0     1001      123     4301 2023-05-02 22:06:38.000000 granian-0.3.2/src/tcp.rs
--rw-r--r--   0     1001      123     2431 2023-05-02 22:06:38.000000 granian-0.3.2/src/tls.rs
--rw-r--r--   0     1001      123      837 2023-05-02 22:06:38.000000 granian-0.3.2/src/utils.rs
--rw-r--r--   0     1001      123    16359 2023-05-02 22:06:38.000000 granian-0.3.2/src/workers.rs
--rw-r--r--   0     1001      123     3435 2023-05-02 22:06:38.000000 granian-0.3.2/src/ws.rs
--rw-r--r--   0     1001      123     1027 2023-05-02 22:06:38.000000 granian-0.3.2/src/wsgi/callbacks.rs
--rw-r--r--   0     1001      123      308 2023-05-02 22:06:38.000000 granian-0.3.2/src/wsgi/errors.rs
--rw-r--r--   0     1001      123     1638 2023-05-02 22:06:38.000000 granian-0.3.2/src/wsgi/http.rs
--rw-r--r--   0     1001      123      312 2023-05-02 22:06:38.000000 granian-0.3.2/src/wsgi/mod.rs
--rw-r--r--   0     1001      123     1984 2023-05-02 22:06:38.000000 granian-0.3.2/src/wsgi/serve.rs
--rw-r--r--   0     1001      123     4127 2023-05-02 22:06:38.000000 granian-0.3.2/src/wsgi/types.rs
--rw-r--r--   0     1001      123     3078 2023-05-02 22:06:38.000000 granian-0.3.2/tests/apps/asgi.py
--rw-r--r--   0     1001      123     2490 2023-05-02 22:06:38.000000 granian-0.3.2/tests/apps/rsgi.py
--rw-r--r--   0     1001      123      861 2023-05-02 22:06:38.000000 granian-0.3.2/tests/apps/wsgi.py
--rw-r--r--   0     1001      123     1759 2023-05-02 22:06:38.000000 granian-0.3.2/tests/conftest.py
--rw-r--r--   0     1001      123     1139 2023-05-02 22:06:38.000000 granian-0.3.2/tests/fixtures/tls/cert.pem
--rw-r--r--   0     1001      123     1704 2023-05-02 22:06:38.000000 granian-0.3.2/tests/fixtures/tls/key.pem
--rw-r--r--   0     1001      123     1830 2023-05-02 22:06:38.000000 granian-0.3.2/tests/test_asgi.py
--rw-r--r--   0     1001      123     1851 2023-05-02 22:06:38.000000 granian-0.3.2/tests/test_https.py
--rw-r--r--   0     1001      123     1450 2023-05-02 22:06:38.000000 granian-0.3.2/tests/test_rsgi.py
--rw-r--r--   0     1001      123     2487 2023-05-02 22:06:38.000000 granian-0.3.2/tests/test_ws.py
--rw-r--r--   0     1001      123     1438 2023-05-02 22:06:38.000000 granian-0.3.2/tests/test_wsgi.py
--rw-r--r--   0     1001      123    30382 2023-05-02 22:06:38.000000 granian-0.3.2/Cargo.lock
--rw-r--r--   0        0        0     3673 1970-01-01 00:00:00.000000 granian-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 granian-0.4.0/Cargo.toml
+-rw-r--r--   0     1001      123     1486 2023-05-09 12:42:50.000000 granian-0.4.0/LICENSE
+-rw-r--r--   0     1001      123     4024 2023-05-09 12:42:50.000000 granian-0.4.0/README.md
+-rw-r--r--   0     1001      123       54 2023-05-09 12:42:50.000000 granian-0.4.0/build.rs
+-rw-r--r--   0     1001      123       28 2023-05-09 12:42:50.000000 granian-0.4.0/granian/__init__.py
+-rw-r--r--   0     1001      123       22 2023-05-09 12:42:50.000000 granian-0.4.0/granian/__version__.py
+-rw-r--r--   0     1001      123     1868 2023-05-09 12:42:50.000000 granian-0.4.0/granian/_granian.pyi
+-rw-r--r--   0     1001      123     1677 2023-05-09 12:42:50.000000 granian-0.4.0/granian/_internal.py
+-rw-r--r--   0     1001      123     2862 2023-05-09 12:42:50.000000 granian-0.4.0/granian/_loops.py
+-rw-r--r--   0     1001      123       93 2023-05-09 12:42:50.000000 granian-0.4.0/granian/_types.py
+-rw-r--r--   0     1001      123     4682 2023-05-09 12:42:50.000000 granian-0.4.0/granian/asgi.py
+-rw-r--r--   0     1001      123     3590 2023-05-09 12:42:50.000000 granian-0.4.0/granian/cli.py
+-rw-r--r--   0     1001      123      357 2023-05-09 12:42:50.000000 granian-0.4.0/granian/constants.py
+-rw-r--r--   0     1001      123     1328 2023-05-09 12:42:50.000000 granian-0.4.0/granian/log.py
+-rw-r--r--   0     1001      123      153 2023-05-09 12:42:50.000000 granian-0.4.0/granian/net.py
+-rw-r--r--   0     1001      123        0 2023-05-09 12:42:50.000000 granian-0.4.0/granian/py.typed
+-rw-r--r--   0     1001      123      462 2023-05-09 12:42:50.000000 granian-0.4.0/granian/rsgi.py
+-rw-r--r--   0     1001      123    10646 2023-05-09 12:42:50.000000 granian-0.4.0/granian/server.py
+-rw-r--r--   0     1001      123     2068 2023-05-09 12:42:50.000000 granian-0.4.0/granian/wsgi.py
+-rw-r--r--   0     1001      123     1624 2023-05-09 12:42:50.000000 granian-0.4.0/pyproject.toml
+-rw-r--r--   0     1001      123     5700 2023-05-09 12:42:50.000000 granian-0.4.0/src/asgi/callbacks.rs
+-rw-r--r--   0     1001      123     1611 2023-05-09 12:42:50.000000 granian-0.4.0/src/asgi/errors.rs
+-rw-r--r--   0     1001      123     4765 2023-05-09 12:42:50.000000 granian-0.4.0/src/asgi/http.rs
+-rw-r--r--   0     1001      123    15092 2023-05-09 12:42:50.000000 granian-0.4.0/src/asgi/io.rs
+-rw-r--r--   0     1001      123      329 2023-05-09 12:42:50.000000 granian-0.4.0/src/asgi/mod.rs
+-rw-r--r--   0     1001      123     2995 2023-05-09 12:42:50.000000 granian-0.4.0/src/asgi/serve.rs
+-rw-r--r--   0     1001      123     2708 2023-05-09 12:42:50.000000 granian-0.4.0/src/asgi/types.rs
+-rw-r--r--   0     1001      123     8605 2023-05-09 12:42:50.000000 granian-0.4.0/src/callbacks.rs
+-rw-r--r--   0     1001      123      415 2023-05-09 12:42:50.000000 granian-0.4.0/src/http.rs
+-rw-r--r--   0     1001      123      550 2023-05-09 12:42:50.000000 granian-0.4.0/src/lib.rs
+-rw-r--r--   0     1001      123     4934 2023-05-09 12:42:50.000000 granian-0.4.0/src/rsgi/callbacks.rs
+-rw-r--r--   0     1001      123      565 2023-05-09 12:42:50.000000 granian-0.4.0/src/rsgi/errors.rs
+-rw-r--r--   0     1001      123     5186 2023-05-09 12:42:50.000000 granian-0.4.0/src/rsgi/http.rs
+-rw-r--r--   0     1001      123    10350 2023-05-09 12:42:50.000000 granian-0.4.0/src/rsgi/io.rs
+-rw-r--r--   0     1001      123      609 2023-05-09 12:42:50.000000 granian-0.4.0/src/rsgi/mod.rs
+-rw-r--r--   0     1001      123     2995 2023-05-09 12:42:50.000000 granian-0.4.0/src/rsgi/serve.rs
+-rw-r--r--   0     1001      123     5619 2023-05-09 12:42:50.000000 granian-0.4.0/src/rsgi/types.rs
+-rw-r--r--   0     1001      123     8066 2023-05-09 12:42:50.000000 granian-0.4.0/src/runtime.rs
+-rw-r--r--   0     1001      123     4301 2023-05-09 12:42:50.000000 granian-0.4.0/src/tcp.rs
+-rw-r--r--   0     1001      123     2431 2023-05-09 12:42:50.000000 granian-0.4.0/src/tls.rs
+-rw-r--r--   0     1001      123      837 2023-05-09 12:42:50.000000 granian-0.4.0/src/utils.rs
+-rw-r--r--   0     1001      123    16456 2023-05-09 12:42:50.000000 granian-0.4.0/src/workers.rs
+-rw-r--r--   0     1001      123     3435 2023-05-09 12:42:50.000000 granian-0.4.0/src/ws.rs
+-rw-r--r--   0     1001      123     1027 2023-05-09 12:42:50.000000 granian-0.4.0/src/wsgi/callbacks.rs
+-rw-r--r--   0     1001      123      308 2023-05-09 12:42:50.000000 granian-0.4.0/src/wsgi/errors.rs
+-rw-r--r--   0     1001      123     1638 2023-05-09 12:42:50.000000 granian-0.4.0/src/wsgi/http.rs
+-rw-r--r--   0     1001      123      312 2023-05-09 12:42:50.000000 granian-0.4.0/src/wsgi/mod.rs
+-rw-r--r--   0     1001      123     2206 2023-05-09 12:42:50.000000 granian-0.4.0/src/wsgi/serve.rs
+-rw-r--r--   0     1001      123     4151 2023-05-09 12:42:50.000000 granian-0.4.0/src/wsgi/types.rs
+-rw-r--r--   0     1001      123     3078 2023-05-09 12:42:50.000000 granian-0.4.0/tests/apps/asgi.py
+-rw-r--r--   0     1001      123     2490 2023-05-09 12:42:50.000000 granian-0.4.0/tests/apps/rsgi.py
+-rw-r--r--   0     1001      123      861 2023-05-09 12:42:50.000000 granian-0.4.0/tests/apps/wsgi.py
+-rw-r--r--   0     1001      123     1759 2023-05-09 12:42:50.000000 granian-0.4.0/tests/conftest.py
+-rw-r--r--   0     1001      123     1139 2023-05-09 12:42:50.000000 granian-0.4.0/tests/fixtures/tls/cert.pem
+-rw-r--r--   0     1001      123     1704 2023-05-09 12:42:50.000000 granian-0.4.0/tests/fixtures/tls/key.pem
+-rw-r--r--   0     1001      123     1830 2023-05-09 12:42:50.000000 granian-0.4.0/tests/test_asgi.py
+-rw-r--r--   0     1001      123     1851 2023-05-09 12:42:50.000000 granian-0.4.0/tests/test_https.py
+-rw-r--r--   0     1001      123     1450 2023-05-09 12:42:50.000000 granian-0.4.0/tests/test_rsgi.py
+-rw-r--r--   0     1001      123     2487 2023-05-09 12:42:50.000000 granian-0.4.0/tests/test_ws.py
+-rw-r--r--   0     1001      123     1438 2023-05-09 12:42:50.000000 granian-0.4.0/tests/test_wsgi.py
+-rw-r--r--   0     1001      123    33385 2023-05-09 12:42:50.000000 granian-0.4.0/Cargo.lock
+-rw-r--r--   0        0        0     5801 1970-01-01 00:00:00.000000 granian-0.4.0/PKG-INFO
```

### Comparing `granian-0.3.2/Cargo.toml` & `granian-0.4.0/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "granian"
-version = "0.3.2"
+version = "0.4.0"
 description = "A Rust HTTP server for Python applications"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 edition = "2021"
 
 keywords = ["web", "asyncio"]
 
@@ -26,28 +26,25 @@
     "!*.so",
 ]
 
 [lib]
 name = "_granian"
 crate-type = ["cdylib"]
 
-[package.metadata.maturin]
-name = "granian._granian"
-
 [dependencies]
 bytes = "1"
 futures = "0.3"
 hyper = { version = "=0.14", features = ["http1", "http2", "server", "stream", "runtime", "tcp"] }
 log = "0.4"
 mimalloc = { version = "0.1.34", default-features = false, features = ["local_dynamic_tls"] }
 once_cell = "1.5"
 pin-project = "1.0"
-pyo3 = { version = "=0.17", features = ["extension-module"] }
-pyo3-asyncio = { version = "=0.17", features = ["tokio-runtime"] }
-pyo3-log = "=0.7"
+pyo3 = { version = "=0.18", features = ["extension-module"] }
+pyo3-asyncio = { version = "=0.18", features = ["tokio-runtime"] }
+pyo3-log = "=0.8"
 rustls-pemfile = "1.0"
 socket2 = { version = "0.4", features = ["all"] }
 tls-listener = { version = "0.5", features = ["rustls", "hyper-h1", "hyper-h2"] }
 tokio = { version = "1.24", features = ["full"] }
 tokio-rustls = "0.23"
 tokio-tungstenite = "0.17"
 tokio-util = { version = "0.7", features = ["codec"] }
```

### Comparing `granian-0.3.2/LICENSE` & `granian-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/granian/_granian.pyi` & `granian-0.4.0/granian/_granian.pyi`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/granian/_internal.py` & `granian-0.4.0/granian/_internal.py`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/granian/_loops.py` & `granian-0.4.0/granian/_loops.py`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/granian/asgi.py` & `granian-0.4.0/granian/asgi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import asyncio
 
 from functools import wraps
 
-from ._futures import future_with_watcher
 from ._granian import ASGIScope as Scope
 
 
 class LifespanProtocol:
     error_transition = 'Invalid lifespan state transition'
 
     def __init__(self, callable):
@@ -118,16 +117,16 @@
 }
 
 
 def _callback_wrapper(callback, scope_opts):
     root_url_path = scope_opts.get('url_path_prefix') or ''
 
     @wraps(callback)
-    def wrapper(watcher, scope: Scope):
-        coro = callback(
+    def wrapper(scope: Scope, proto):
+        return callback(
             {
                 "type": scope.proto,
                 "asgi": {
                     "version": "3.0",
                     "spec_version": "2.3"
                 },
                 "http_version": scope.http_version,
@@ -138,17 +137,11 @@
                 "root_path": root_url_path,
                 "path": scope.path,
                 "raw_path": scope.path.encode("ascii"),
                 "query_string": scope.query_string.encode('latin-1'),
                 "headers": scope.headers,
                 "extensions": {}
             },
-            watcher.proto.receive,
-            _send_wrappers[scope.proto](watcher.proto.send)
-        )
-        watcher.event_loop.call_soon_threadsafe(
-            future_with_watcher,
-            coro,
-            watcher,
-            context=watcher.context
+            proto.receive,
+            _send_wrappers[scope.proto](proto.send)
         )
     return wrapper
```

### Comparing `granian-0.3.2/granian/cli.py` & `granian-0.4.0/granian/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 from pathlib import Path
 from typing import Optional
 
 import typer
 
 from .__version__ import __version__
 from .constants import Interfaces, HTTPModes, Loops, ThreadModes
@@ -50,14 +52,22 @@
         help="Maximum number of connections to hold in backlog."
     ),
     log_level: LogLevels = typer.Option(
         LogLevels.info.value,
         help="Log level",
         case_sensitive=False
     ),
+    log_config: Optional[Path] = typer.Option(
+        None,
+        help="Logging configuration file (json)",
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True
+    ),
     ssl_keyfile: Optional[Path] = typer.Option(
         None,
         help="SSL key file",
         exists=True,
         file_okay=True,
         dir_okay=False,
         readable=True
@@ -83,26 +93,36 @@
         None,
         "--version",
         callback=version_callback,
         is_eager=True,
         help="Shows the version and exit."
     )
 ):
+    log_dictconfig = None
+    if log_config:
+        with log_config.open() as log_config_file:
+            try:
+                log_dictconfig = json.loads(log_config_file.read())
+            except Exception:
+                print("Unable to parse provided logging config.")
+                raise typer.Exit(1)
+
     Granian(
         app,
         address=host,
         port=port,
         interface=interface,
         workers=workers,
         threads=threads,
         pthreads=threads,
         threading_mode=threading_mode,
         loop=loop,
         http=http,
         websockets=websockets,
         backlog=backlog,
         log_level=log_level,
+        log_dictconfig=log_dictconfig,
         ssl_cert=ssl_certificate,
         ssl_key=ssl_keyfile,
         url_path_prefix=url_path_prefix,
         reload=reload
     ).serve()
```

### Comparing `granian-0.3.2/granian/log.py` & `granian-0.4.0/granian/log.py`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/granian/server.py` & `granian-0.4.0/granian/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 from ._granian import ASGIWorker, RSGIWorker, WSGIWorker
 from ._internal import load_target
 from .asgi import LifespanProtocol, _callback_wrapper as _asgi_call_wrap
 from .constants import Interfaces, HTTPModes, Loops, ThreadModes
 from .log import LogLevels, configure_logging, logger
 from .net import SocketHolder
-from .rsgi import _callback_wrapper as _rsgi_call_wrap
 from .wsgi import _callback_wrapper as _wsgi_call_wrap
 
 multiprocessing.allow_connection_pickling()
 
 
 class Granian:
     SIGNALS = {signal.SIGINT, signal.SIGTERM}
@@ -189,15 +188,15 @@
             *ssl_ctx
         )
         serve = getattr(worker, {
             ThreadModes.runtime: "serve_rth",
             ThreadModes.workers: "serve_wth"
         }[threading_mode])
         serve(
-            _rsgi_call_wrap(callback),
+            callback,
             loop,
             contextvars.copy_context(),
             shutdown_event.wait()
         )
 
     @staticmethod
     def _spawn_wsgi_worker(
```

### Comparing `granian-0.3.2/granian/wsgi.py` & `granian-0.4.0/granian/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/pyproject.toml` & `granian-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python",
@@ -27,15 +26,15 @@
     "description",
     "keywords",
     "license",
     "readme",
     "version"
 ]
 
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "watchfiles~=0.18",
     "typer~=0.4",
     "uvloop~=0.17.0; sys_platform != 'win32' and platform_python_implementation == 'CPython'"
 ]
 
 [project.optional-dependencies]
@@ -51,12 +50,13 @@
 Funding = "https://github.com/sponsors/gi0baro"
 Source = "https://github.com/emmett-framework/granian"
 
 [project.scripts]
 granian = "granian:cli.cli"
 
 [build-system]
-requires = ["maturin>=0.12,<0.13"]
+requires = ["maturin>=0.14.17,<0.15"]
 build-backend = "maturin"
 
 [tool.maturin]
+module-name = "granian._granian"
 bindings = "pyo3"
```

### Comparing `granian-0.3.2/src/asgi/callbacks.rs` & `granian-0.4.0/src/asgi/callbacks.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,132 @@
 use hyper::{Body, Request, Response};
 use pyo3::prelude::*;
 use tokio::sync::oneshot;
 
 use crate::{
-    callbacks::CallbackWrapper,
+    callbacks::{
+        CallbackWrapper,
+        callback_impl_run,
+        callback_impl_loop_step,
+        callback_impl_loop_wake,
+        callback_impl_loop_err
+    },
     runtime::RuntimeRef,
     ws::{HyperWebsocket, UpgradeData}
 };
 use super::{
-    errors::{ASGIFlowError, error_flow},
-    io::{ASGIHTTPProtocol, ASGIWebsocketProtocol},
+    io::{ASGIHTTPProtocol as HTTPProtocol, ASGIWebsocketProtocol as WebsocketProtocol},
     types::ASGIScope as Scope
 };
 
 
 #[pyclass]
-pub(crate) struct CallbackWatcherHTTP {
-    #[pyo3(get)]
-    proto: Py<ASGIHTTPProtocol>,
-    #[pyo3(get)]
+pub(crate) struct CallbackRunnerHTTP {
+    proto: Py<HTTPProtocol>,
     event_loop: PyObject,
-    #[pyo3(get)]
-    context: PyObject
+    context: PyObject,
+    cb: PyObject
 }
 
-impl CallbackWatcherHTTP {
+impl CallbackRunnerHTTP {
     pub fn new(
         py: Python,
         cb: CallbackWrapper,
-        proto: ASGIHTTPProtocol
+        proto: HTTPProtocol,
+        scope: Scope
     ) -> Self {
+        let pyproto = Py::new(py, proto).unwrap();
         Self {
-            proto: Py::new(py, proto).unwrap(),
+            proto: pyproto.clone(),
             event_loop: cb.context.event_loop(py).into(),
             context: cb.context.context(py).into(),
+            cb: cb.callback.call1(py, (scope, pyproto)).unwrap()
         }
     }
-}
 
-#[pymethods]
-impl CallbackWatcherHTTP {
-    fn done(&mut self, py: Python) {
+    fn done(&self, py: Python) {
         if let Ok(mut proto) = self.proto.as_ref(py).try_borrow_mut() {
             if let Some(tx) = proto.tx() {
                 let mut res = Response::new("Internal server error".into());
                 *res.status_mut() = hyper::StatusCode::INTERNAL_SERVER_ERROR;
                 let _ = tx.send(res);
             }
         }
     }
 
-    fn err(&mut self, py: Python) {
+    fn err(&self, py: Python) {
         log::warn!("Application callable raised an exception");
         self.done(py)
     }
+
+    callback_impl_run!();
+    callback_impl_loop_err!();
+}
+
+#[pymethods]
+impl CallbackRunnerHTTP {
+    fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<PyObject> {
+        callback_impl_loop_step!(pyself, py)
+    }
+
+    fn _loop_wake(pyself: PyRef<'_, Self>, py: Python, fut: PyObject) -> PyResult<PyObject> {
+        callback_impl_loop_wake!(pyself, py, fut)
+    }
 }
 
 #[pyclass]
-pub(crate) struct CallbackWatcherWebsocket {
-    #[pyo3(get)]
-    proto: Py<ASGIWebsocketProtocol>,
-    #[pyo3(get)]
+pub(crate) struct CallbackRunnerWebsocket {
+    proto: Py<WebsocketProtocol>,
     event_loop: PyObject,
-    #[pyo3(get)]
-    context: PyObject
+    context: PyObject,
+    cb: PyObject
 }
 
-impl CallbackWatcherWebsocket {
+impl CallbackRunnerWebsocket {
     pub fn new(
         py: Python,
         cb: CallbackWrapper,
-        proto: ASGIWebsocketProtocol
+        proto: WebsocketProtocol,
+        scope: Scope
     ) -> Self {
+        let pyproto = Py::new(py, proto).unwrap();
         Self {
-            proto: Py::new(py, proto).unwrap(),
+            proto: pyproto.clone(),
             event_loop: cb.context.event_loop(py).into(),
             context: cb.context.context(py).into(),
+            cb: cb.callback.call1(py, (scope, pyproto)).unwrap()
         }
     }
-}
 
-#[pymethods]
-impl CallbackWatcherWebsocket {
-    fn done(&mut self, py: Python) {
+    fn done(&self, py: Python) {
         if let Ok(mut proto) = self.proto.as_ref(py).try_borrow_mut() {
             if let (Some(tx), res) = proto.tx() {
                 let _ = tx.send(res);
             }
         }
     }
 
-    fn err(&mut self, py: Python) {
+    fn err(&self, py: Python) {
         log::warn!("Application callable raised an exception");
         self.done(py)
     }
+
+    callback_impl_run!();
+    callback_impl_loop_err!();
+}
+
+#[pymethods]
+impl CallbackRunnerWebsocket {
+    fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<PyObject> {
+        callback_impl_loop_step!(pyself, py)
+    }
+
+    fn _loop_wake(pyself: PyRef<'_, Self>, py: Python, fut: PyObject) -> PyResult<PyObject> {
+        callback_impl_loop_wake!(pyself, py, fut)
+    }
 }
 
 // NOTE: we cannot use single `impl` function as structs with pyclass won't handle
 //       dyn fields easily.
 // pub(crate) async fn call(
 //     cb: CallbackWrapper,
 //     protocol: impl ASGIProtocol + IntoPy<PyObject>,
@@ -115,116 +144,76 @@
 //             log::warn!("Application callable raised an exception");
 //             error_flow!()
 //         },
 //         _ => error_flow!()
 //     }
 // }
 
-pub(crate) async fn call_rtb_http(
+pub(crate) fn call_rtb_http(
     cb: CallbackWrapper,
     rt: RuntimeRef,
     req: Request<Body>,
     scope: Scope
-) -> Result<Response<Body>, ASGIFlowError> {
-    let callback = cb.callback.clone();
+) -> oneshot::Receiver<Response<Body>> {
     let (tx, rx) = oneshot::channel();
-    let protocol = ASGIHTTPProtocol::new(rt, req, tx);
+    let protocol = HTTPProtocol::new(rt, req, tx);
 
     Python::with_gil(|py| {
-        callback.call1(py, (CallbackWatcherHTTP::new(py, cb, protocol), scope))
-    })?;
+        let _ = CallbackRunnerHTTP::new(py, cb, protocol, scope).run(py);
+    });
 
-    match rx.await {
-        Ok(res) => {
-            Ok(res)
-        },
-        _ => {
-            log::error!("ASGI protocol failure");
-            error_flow!()
-        }
-    }
+    rx
 }
 
-pub(crate) async fn call_rtt_http(
+pub(crate) fn call_rtt_http(
     cb: CallbackWrapper,
     rt: RuntimeRef,
     req: Request<Body>,
     scope: Scope
-) -> Result<Response<Body>, ASGIFlowError> {
-    let callback = cb.callback.clone();
+) -> oneshot::Receiver<Response<Body>> {
     let (tx, rx) = oneshot::channel();
-    let protocol = ASGIHTTPProtocol::new(rt, req, tx);
+    let protocol = HTTPProtocol::new(rt, req, tx);
 
     tokio::task::spawn_blocking(move || {
         Python::with_gil(|py| {
-            let _ = callback.call1(
-                py, (CallbackWatcherHTTP::new(py, cb, protocol), scope)
-            );
+            let _ = CallbackRunnerHTTP::new(py, cb, protocol, scope).run(py);
         });
     });
 
-    match rx.await {
-        Ok(res) => {
-            Ok(res)
-        },
-        _ => {
-            log::error!("ASGI protocol failure");
-            error_flow!()
-        }
-    }
+    rx
 }
 
-pub(crate) async fn call_rtb_ws(
+pub(crate) fn call_rtb_ws(
     cb: CallbackWrapper,
     rt: RuntimeRef,
     ws: HyperWebsocket,
     upgrade: UpgradeData,
     scope: Scope
-) -> Result<bool, ASGIFlowError> {
-    let callback = cb.callback.clone();
+) -> oneshot::Receiver<bool> {
     let (tx, rx) = oneshot::channel();
-    let protocol = ASGIWebsocketProtocol::new(rt, tx, ws, upgrade);
+    let protocol = WebsocketProtocol::new(rt, tx, ws, upgrade);
 
     Python::with_gil(|py| {
-        callback.call1(py, (CallbackWatcherWebsocket::new(py, cb, protocol), scope))
-    })?;
+        let _ = CallbackRunnerWebsocket::new(py, cb, protocol, scope).run(py);
+    });
 
-    match rx.await {
-        Ok(res) => {
-            Ok(res)
-        },
-        _ => {
-            log::error!("ASGI protocol failure");
-            error_flow!()
-        }
-    }
+    rx
 }
 
-pub(crate) async fn call_rtt_ws(
+pub(crate) fn call_rtt_ws(
     cb: CallbackWrapper,
     rt: RuntimeRef,
     ws: HyperWebsocket,
     upgrade: UpgradeData,
     scope: Scope
-) -> Result<bool, ASGIFlowError> {
-    let callback = cb.callback.clone();
+) -> oneshot::Receiver<bool> {
     let (tx, rx) = oneshot::channel();
-    let protocol = ASGIWebsocketProtocol::new(rt, tx, ws, upgrade);
+    let protocol = WebsocketProtocol::new(rt, tx, ws, upgrade);
 
     tokio::task::spawn_blocking(move || {
         Python::with_gil(|py| {
-            let _ = callback.call1(
-                py, (CallbackWatcherWebsocket::new(py, cb, protocol), scope)
-            );
+            let _ = CallbackRunnerWebsocket::new(py, cb, protocol, scope).run(py);
         });
     });
 
-    match rx.await {
-        Ok(res) => {
-            Ok(res)
-        },
-        _ => {
-            log::error!("ASGI protocol failure");
-            error_flow!()
-        }
-    }
+    rx
 }
```

### Comparing `granian-0.3.2/src/asgi/errors.rs` & `granian-0.4.0/src/asgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/src/asgi/http.rs` & `granian-0.4.0/src/asgi/http.rs`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,18 @@
     };
 }
 
 macro_rules! handle_http_response {
     ($handler:expr, $rt:expr, $callback:expr, $req:expr, $scope:expr) => {
         match $handler($callback, $rt, $req, $scope).await {
             Ok(res) => res,
-            _ => response_500()
+            _ => {
+                log::error!("ASGI protocol failure");
+                response_500()
+            }
         }
     }
 }
 
 macro_rules! handle_request {
     ($func_name:ident, $handler:expr) => {
         pub(crate) async fn $func_name(
@@ -98,14 +101,15 @@
                                                 .header(HK_SERVER, HV_SERVER)
                                                 .body(Body::from(""))
                                                 .unwrap()
                                         ).await;
                                     };
                                 },
                                 _ => {
+                                    log::error!("ASGI protocol failure");
                                     let _ = tx_ref.send(response_500()).await;
                                 }
                             }
                         });
 
                         match resrx.recv().await {
                             Some(res) => {
```

### Comparing `granian-0.3.2/src/asgi/io.rs` & `granian-0.4.0/src/asgi/io.rs`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/src/asgi/serve.rs` & `granian-0.4.0/src/rsgi/serve.rs`

 * *Files 5% similar despite different names*

```diff
@@ -8,44 +8,57 @@
         serve_rth_ssl,
         serve_wth_ssl
     }
 };
 use super::http::{handle_rtb, handle_rtt, handle_rtb_ws, handle_rtt_ws};
 
 #[pyclass(module="granian._granian")]
-pub struct ASGIWorker {
+pub struct RSGIWorker {
     config: WorkerConfig
 }
 
-impl ASGIWorker {
+impl RSGIWorker {
     serve_rth!(_serve_rth, handle_rtb);
     serve_rth!(_serve_rth_ws, handle_rtb_ws);
     serve_wth!(_serve_wth, handle_rtt);
     serve_wth!(_serve_wth_ws, handle_rtt_ws);
     serve_rth_ssl!(_serve_rth_ssl, handle_rtb);
     serve_rth_ssl!(_serve_rth_ssl_ws, handle_rtb_ws);
     serve_wth_ssl!(_serve_wth_ssl, handle_rtt);
     serve_wth_ssl!(_serve_wth_ssl_ws, handle_rtt_ws);
 }
 
 #[pymethods]
-impl ASGIWorker {
+impl RSGIWorker {
     #[new]
-    #[args(socket_fd, threads="1", http1_buffer_max="65535")]
+    #[pyo3(
+        signature = (
+            worker_id,
+            socket_fd,
+            threads=1,
+            pthreads=1,
+            http_mode="1",
+            http1_buffer_max=65535,
+            websockets_enabled=false,
+            ssl_enabled=false,
+            ssl_cert=None,
+            ssl_key=None
+        )
+    )]
     fn new(
         worker_id: i32,
         socket_fd: i32,
         threads: usize,
         pthreads: usize,
-        http_mode: String,
+        http_mode: &str,
         http1_buffer_max: usize,
         websockets_enabled: bool,
         ssl_enabled: bool,
-        ssl_cert: Option<String>,
-        ssl_key: Option<String>
+        ssl_cert: Option<&str>,
+        ssl_key: Option<&str>
     ) -> PyResult<Self> {
         Ok(Self {
             config: WorkerConfig::new(
                 worker_id,
                 socket_fd,
                 threads,
                 pthreads,
```

### Comparing `granian-0.3.2/src/asgi/types.rs` & `granian-0.4.0/src/asgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/src/lib.rs` & `granian-0.4.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/src/rsgi/callbacks.rs` & `granian-0.4.0/src/rsgi/callbacks.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,206 +1,195 @@
 use pyo3::prelude::*;
 use tokio::sync::oneshot;
 
 use crate::{
-    callbacks::CallbackWrapper,
+    callbacks::{
+        CallbackWrapper,
+        callback_impl_run,
+        callback_impl_loop_step,
+        callback_impl_loop_wake,
+        callback_impl_loop_err
+    },
     runtime::RuntimeRef,
     ws::{HyperWebsocket, UpgradeData}
 };
 use super::{
-    errors::error_proto,
     io::{RSGIHTTPProtocol as HTTPProtocol, RSGIWebsocketProtocol as WebsocketProtocol},
     types::{RSGIScope as Scope, PyResponse, PyResponseBytes}
 };
 
 
 #[pyclass]
-pub(crate) struct CallbackWatcherHTTP {
-    #[pyo3(get)]
+pub(crate) struct CallbackRunnerHTTP {
     proto: Py<HTTPProtocol>,
-    #[pyo3(get)]
     event_loop: PyObject,
-    #[pyo3(get)]
-    context: PyObject
+    context: PyObject,
+    cb: PyObject
 }
 
-impl CallbackWatcherHTTP {
+impl CallbackRunnerHTTP {
     pub fn new(
         py: Python,
         cb: CallbackWrapper,
-        proto: HTTPProtocol
+        proto: HTTPProtocol,
+        scope: Scope
     ) -> Self {
+        let pyproto = Py::new(py, proto).unwrap();
         Self {
-            proto: Py::new(py, proto).unwrap(),
+            proto: pyproto.clone(),
             event_loop: cb.context.event_loop(py).into(),
-            context: cb.context.context(py).into()
+            context: cb.context.context(py).into(),
+            cb: cb.callback.call1(py, (scope, pyproto)).unwrap()
         }
     }
-}
 
-#[pymethods]
-impl CallbackWatcherHTTP {
-    fn done(&mut self, py: Python) {
+    fn done(&self, py: Python) {
         if let Ok(mut proto) = self.proto.as_ref(py).try_borrow_mut() {
             if let Some(tx) = proto.tx() {
                 let _ = tx.send(
                     PyResponse::Bytes(PyResponseBytes::empty(500, Vec::new()))
                 );
             }
         }
     }
 
-    fn err(&mut self, py: Python) {
+    fn err(&self, py: Python) {
         log::warn!("Application callable raised an exception");
         self.done(py)
     }
+
+    callback_impl_run!();
+    callback_impl_loop_err!();
+}
+
+#[pymethods]
+impl CallbackRunnerHTTP {
+    fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<PyObject> {
+        callback_impl_loop_step!(pyself, py)
+    }
+
+    fn _loop_wake(pyself: PyRef<'_, Self>, py: Python, fut: PyObject) -> PyResult<PyObject> {
+        callback_impl_loop_wake!(pyself, py, fut)
+    }
 }
 
 #[pyclass]
-pub(crate) struct CallbackWatcherWebsocket {
-    #[pyo3(get)]
+pub(crate) struct CallbackRunnerWebsocket {
     proto: Py<WebsocketProtocol>,
-    #[pyo3(get)]
     event_loop: PyObject,
-    #[pyo3(get)]
-    context: PyObject
+    context: PyObject,
+    cb: PyObject
 }
 
-impl CallbackWatcherWebsocket {
+impl CallbackRunnerWebsocket {
     pub fn new(
         py: Python,
         cb: CallbackWrapper,
-        proto: WebsocketProtocol
+        proto: WebsocketProtocol,
+        scope: Scope
     ) -> Self {
+        let pyproto = Py::new(py, proto).unwrap();
         Self {
-            proto: Py::new(py, proto).unwrap(),
+            proto: pyproto.clone(),
             event_loop: cb.context.event_loop(py).into(),
             context: cb.context.context(py).into(),
+            cb: cb.callback.call1(py, (scope, pyproto)).unwrap()
         }
     }
-}
 
-#[pymethods]
-impl CallbackWatcherWebsocket {
-    fn done(&mut self, py: Python) {
+    fn done(&self, py: Python) {
         if let Ok(mut proto) = self.proto.as_ref(py).try_borrow_mut() {
             if let (Some(tx), res) = proto.tx() {
                 let _ = tx.send(res);
             }
         }
     }
 
-    fn err(&mut self, py: Python) {
+    fn err(&self, py: Python) {
         log::warn!("Application callable raised an exception");
         self.done(py)
     }
+
+    callback_impl_run!();
+    callback_impl_loop_err!();
 }
 
-pub(crate) async fn call_rtb_http(
+#[pymethods]
+impl CallbackRunnerWebsocket {
+    fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<PyObject> {
+        callback_impl_loop_step!(pyself, py)
+    }
+
+    fn _loop_wake(pyself: PyRef<'_, Self>, py: Python, fut: PyObject) -> PyResult<PyObject> {
+        callback_impl_loop_wake!(pyself, py, fut)
+    }
+}
+
+pub(crate) fn call_rtb_http(
     cb: CallbackWrapper,
     rt: RuntimeRef,
     req: hyper::Request<hyper::Body>,
     scope: Scope
-) -> PyResult<PyResponse> {
-    let callback = cb.callback.clone();
+) -> oneshot::Receiver<PyResponse> {
     let (tx, rx) = oneshot::channel();
     let protocol = HTTPProtocol::new(rt, tx, req);
 
     Python::with_gil(|py| {
-        callback.call1(py, (CallbackWatcherHTTP::new(py, cb, protocol), scope))
-    })?;
+        let _ = CallbackRunnerHTTP::new(py, cb, protocol, scope).run(py);
+    });
 
-    match rx.await {
-        Ok(res) => {
-            Ok(res)
-        },
-        _ => {
-            log::error!("RSGI protocol failure");
-            error_proto!()
-        }
-    }
+    rx
 }
 
-pub(crate) async fn call_rtt_http(
+pub(crate) fn call_rtt_http(
     cb: CallbackWrapper,
     rt: RuntimeRef,
     req: hyper::Request<hyper::Body>,
     scope: Scope
-) -> PyResult<PyResponse> {
-    let callback = cb.callback.clone();
+) -> oneshot::Receiver<PyResponse> {
     let (tx, rx) = oneshot::channel();
     let protocol = HTTPProtocol::new(rt, tx, req);
 
     tokio::task::spawn_blocking(move || {
         Python::with_gil(|py| {
-            let _ = callback.call1(
-                py, (CallbackWatcherHTTP::new(py, cb, protocol), scope)
-            );
+            let _ = CallbackRunnerHTTP::new(py, cb, protocol, scope).run(py);
         });
     });
 
-    match rx.await {
-        Ok(res) => {
-            Ok(res)
-        },
-        _ => {
-            log::error!("RSGI protocol failure");
-            error_proto!()
-        }
-    }
+    rx
 }
 
-pub(crate) async fn call_rtb_ws(
+pub(crate) fn call_rtb_ws(
     cb: CallbackWrapper,
     rt: RuntimeRef,
     ws: HyperWebsocket,
     upgrade: UpgradeData,
     scope: Scope
-) -> PyResult<(i32, bool)> {
-    let callback = cb.callback.clone();
+) -> oneshot::Receiver<(i32, bool)> {
     let (tx, rx) = oneshot::channel();
     let protocol = WebsocketProtocol::new(rt, tx, ws, upgrade);
 
     Python::with_gil(|py| {
-        callback.call1(py, (CallbackWatcherWebsocket::new(py, cb, protocol), scope))
-    })?;
+        let _ = CallbackRunnerWebsocket::new(py, cb, protocol, scope).run(py);
+    });
 
-    match rx.await {
-        Ok(res) => {
-            Ok(res)
-        },
-        _ => {
-            log::error!("RSGI protocol failure");
-            error_proto!()
-        }
-    }
+    rx
 }
 
-pub(crate) async fn call_rtt_ws(
+pub(crate) fn call_rtt_ws(
     cb: CallbackWrapper,
     rt: RuntimeRef,
     ws: HyperWebsocket,
     upgrade: UpgradeData,
     scope: Scope
-) -> PyResult<(i32, bool)> {
-    let callback = cb.callback.clone();
+) -> oneshot::Receiver<(i32, bool)> {
     let (tx, rx) = oneshot::channel();
     let protocol = WebsocketProtocol::new(rt, tx, ws, upgrade);
 
     tokio::task::spawn_blocking(move || {
         Python::with_gil(|py| {
-            let _ = callback.call1(
-                py, (CallbackWatcherWebsocket::new(py, cb, protocol), scope)
-            );
+            let _ = CallbackRunnerWebsocket::new(py, cb, protocol, scope).run(py);
         });
     });
 
-    match rx.await {
-        Ok(res) => {
-            Ok(res)
-        },
-        _ => {
-            log::error!("RSGI protocol failure");
-            error_proto!()
-        }
-    }
+    rx
 }
```

### Comparing `granian-0.3.2/src/rsgi/errors.rs` & `granian-0.4.0/src/rsgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/src/rsgi/http.rs` & `granian-0.4.0/src/rsgi/http.rs`

 * *Files 11% similar despite different names*

```diff
@@ -41,15 +41,18 @@
         match $handler($callback, $rt, $req, $scope).await {
             Ok(PyResponse::Bytes(pyres)) => {
                 pyres.to_response()
             },
             Ok(PyResponse::File(pyres)) => {
                 pyres.to_response().await
             },
-            _ => response_500()
+            _ => {
+                log::error!("RSGI protocol failure");
+                response_500()
+            }
         }
     };
 }
 
 macro_rules! handle_request {
     ($func_name:ident, $handler:expr) => {
         pub(crate) async fn $func_name(
@@ -107,14 +110,15 @@
                                                 .header(HK_SERVER, HV_SERVER)
                                                 .body(Body::from(""))
                                                 .unwrap()
                                         ).await;
                                     }
                                 },
                                 _ => {
+                                    log::error!("RSGI protocol failure");
                                     let _ = tx_ref.send(response_500()).await;
                                 }
                             }
                         });
 
                         return match resrx.recv().await {
                             Some(res) => {
```

### Comparing `granian-0.3.2/src/rsgi/io.rs` & `granian-0.4.0/src/rsgi/io.rs`

 * *Files 6% similar despite different names*

```diff
@@ -51,42 +51,42 @@
             let body = hyper::body::to_bytes(&mut *req).await.unwrap();
             Ok(Python::with_gil(|py| {
                 PyBytes::new(py, &body[..]).as_ref().to_object(py)
             }))
         })
     }
 
-    #[args(status="200", headers="vec![]")]
+    #[pyo3(signature = (status=200, headers=vec![]))]
     fn response_empty(&mut self, status: u16, headers: Vec<(String, String)>) {
         if let Some(tx) = self.tx.take() {
             let _ = tx.send(
                 PyResponse::Bytes(PyResponseBytes::empty(status, headers))
             );
         }
     }
 
-    #[args(status="200", headers="vec![]")]
+    #[pyo3(signature = (status=200, headers=vec![], body=vec![]))]
     fn response_bytes(&mut self, status: u16, headers: Vec<(String, String)>, body: Vec<u8>) {
         if let Some(tx) = self.tx.take() {
             let _ = tx.send(
                 PyResponse::Bytes(PyResponseBytes::from_bytes(status, headers, body))
             );
         }
     }
 
-    #[args(status="200", headers="vec![]")]
+    #[pyo3(signature = (status=200, headers=vec![], body="".to_string()))]
     fn response_str(&mut self, status: u16, headers: Vec<(String, String)>, body: String) {
         if let Some(tx) = self.tx.take() {
             let _ = tx.send(
                 PyResponse::Bytes(PyResponseBytes::from_string(status, headers, body))
             );
         }
     }
 
-    #[args(status="200", headers="vec![]")]
+    #[pyo3(signature = (status, headers, file))]
     fn response_file(&mut self, status: u16, headers: Vec<(String, String)>, file: String) {
         if let Some(tx) = self.tx.take() {
             let _ = tx.send(
                 PyResponse::File(PyResponseFile::new(status, headers, file))
             );
         }
     }
@@ -260,15 +260,15 @@
     pub fn new(data: Py<PyString>) -> Self {
         Self { kind: WebsocketMessageType::Text as usize, data: data }
     }
 }
 
 #[pymethods]
 impl RSGIWebsocketProtocol {
-    #[args(status="None")]
+    #[pyo3(signature = (status=None))]
     fn close(&mut self, py: Python, status: Option<i32>) -> PyResult<()> {
         self.status = status.unwrap_or(0);
         if let Some(tx) = self.tx.take() {
             if let Ok(mut transport) = self.transport.try_lock() {
                 if let Some(transport) = transport.take() {
                     if let Ok(trx) = transport.try_borrow_mut(py) {
                         trx.close();
```

### Comparing `granian-0.3.2/src/rsgi/mod.rs` & `granian-0.4.0/src/rsgi/mod.rs`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/src/rsgi/serve.rs` & `granian-0.4.0/src/asgi/serve.rs`

 * *Files 14% similar despite different names*

```diff
@@ -8,44 +8,57 @@
         serve_rth_ssl,
         serve_wth_ssl
     }
 };
 use super::http::{handle_rtb, handle_rtt, handle_rtb_ws, handle_rtt_ws};
 
 #[pyclass(module="granian._granian")]
-pub struct RSGIWorker {
+pub struct ASGIWorker {
     config: WorkerConfig
 }
 
-impl RSGIWorker {
+impl ASGIWorker {
     serve_rth!(_serve_rth, handle_rtb);
     serve_rth!(_serve_rth_ws, handle_rtb_ws);
     serve_wth!(_serve_wth, handle_rtt);
     serve_wth!(_serve_wth_ws, handle_rtt_ws);
     serve_rth_ssl!(_serve_rth_ssl, handle_rtb);
     serve_rth_ssl!(_serve_rth_ssl_ws, handle_rtb_ws);
     serve_wth_ssl!(_serve_wth_ssl, handle_rtt);
     serve_wth_ssl!(_serve_wth_ssl_ws, handle_rtt_ws);
 }
 
 #[pymethods]
-impl RSGIWorker {
+impl ASGIWorker {
     #[new]
-    #[args(socket_fd, threads="1", http1_buffer_max="65535")]
+    #[pyo3(
+        signature = (
+            worker_id,
+            socket_fd,
+            threads=1,
+            pthreads=1,
+            http_mode="1",
+            http1_buffer_max=65535,
+            websockets_enabled=false,
+            ssl_enabled=false,
+            ssl_cert=None,
+            ssl_key=None
+        )
+    )]
     fn new(
         worker_id: i32,
         socket_fd: i32,
         threads: usize,
         pthreads: usize,
-        http_mode: String,
+        http_mode: &str,
         http1_buffer_max: usize,
         websockets_enabled: bool,
         ssl_enabled: bool,
-        ssl_cert: Option<String>,
-        ssl_key: Option<String>
+        ssl_cert: Option<&str>,
+        ssl_key: Option<&str>
     ) -> PyResult<Self> {
         Ok(Self {
             config: WorkerConfig::new(
                 worker_id,
                 socket_fd,
                 threads,
                 pthreads,
```

### Comparing `granian-0.3.2/src/rsgi/types.rs` & `granian-0.4.0/src/rsgi/types.rs`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         Ok(ret)
     }
 
     fn __contains__(&self, key: &str) -> bool {
         self.inner.contains_key(key)
     }
 
-    #[args(key, default="None")]
+    #[pyo3(signature = (key, default=None))]
     fn get(&self, py: Python, key: &str, default: Option<PyObject>) -> Option<PyObject> {
         match self.inner.get(key) {
             Some(val) => {
                 match val.to_str() {
                     Ok(string) => Some(PyString::new(py, string).into()),
                     _ => default
                 }
```

### Comparing `granian-0.3.2/src/runtime.rs` & `granian-0.4.0/src/runtime.rs`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/src/tcp.rs` & `granian-0.4.0/src/tcp.rs`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/src/tls.rs` & `granian-0.4.0/src/tls.rs`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/src/utils.rs` & `granian-0.4.0/src/utils.rs`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/src/workers.rs` & `granian-0.4.0/src/workers.rs`

 * *Files 2% similar despite different names*

```diff
@@ -26,32 +26,32 @@
 
 impl WorkerConfig {
     pub fn new(
         id: i32,
         socket_fd: i32,
         threads: usize,
         pthreads: usize,
-        http_mode: String,
+        http_mode: &str,
         http1_buffer_max: usize,
         websockets_enabled: bool,
         ssl_enabled: bool,
-        ssl_cert: Option<String>,
-        ssl_key: Option<String>
+        ssl_cert: Option<&str>,
+        ssl_key: Option<&str>
     ) -> Self {
         Self {
             id,
             socket_fd,
             threads,
             pthreads,
-            http_mode,
+            http_mode: http_mode.into(),
             http1_buffer_max,
             websockets_enabled,
             ssl_enabled,
-            ssl_cert,
-            ssl_key
+            ssl_cert: ssl_cert.map_or(None, |v| Some(v.into())),
+            ssl_key: ssl_key.map_or(None, |v| Some(v.into()))
         }
     }
 
     #[cfg(unix)]
     pub fn tcp_listener(&self) -> TcpListener {
         unsafe {
             TcpListener::from_raw_fd(self.socket_fd)
```

### Comparing `granian-0.3.2/src/ws.rs` & `granian-0.4.0/src/ws.rs`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/src/wsgi/callbacks.rs` & `granian-0.4.0/src/wsgi/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/src/wsgi/http.rs` & `granian-0.4.0/src/wsgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/src/wsgi/serve.rs` & `granian-0.4.0/src/wsgi/serve.rs`

 * *Files 12% similar despite different names*

```diff
@@ -22,25 +22,37 @@
     serve_rth_ssl!(_serve_rth_ssl, handle_rtb);
     serve_wth_ssl!(_serve_wth_ssl, handle_rtt);
 }
 
 #[pymethods]
 impl WSGIWorker {
     #[new]
-    #[args(socket_fd, threads="1", http1_buffer_max="65535")]
+    #[pyo3(
+        signature = (
+            worker_id,
+            socket_fd,
+            threads=1,
+            pthreads=1,
+            http_mode="1",
+            http1_buffer_max=65535,
+            ssl_enabled=false,
+            ssl_cert=None,
+            ssl_key=None
+        )
+    )]
     fn new(
         worker_id: i32,
         socket_fd: i32,
         threads: usize,
         pthreads: usize,
-        http_mode: String,
+        http_mode: &str,
         http1_buffer_max: usize,
         ssl_enabled: bool,
-        ssl_cert: Option<String>,
-        ssl_key: Option<String>
+        ssl_cert: Option<&str>,
+        ssl_key: Option<&str>
     ) -> PyResult<Self> {
         Ok(Self {
             config: WorkerConfig::new(
                 worker_id,
                 socket_fd,
                 threads,
                 pthreads,
```

### Comparing `granian-0.3.2/src/wsgi/types.rs` & `granian-0.4.0/src/wsgi/types.rs`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                 let bytes = self.inner.split_to(next_split);
                 Some(PyBytes::new(py, &bytes[..]))
             },
             _ => None
         }
     }
 
-    #[args(size="None")]
+    #[pyo3(signature = (size=None))]
     fn read<'p>(&mut self, py: Python<'p>, size: Option<usize>) -> &'p PyBytes {
         match size {
             None => {
                 let bytes = self.inner.split_to(self.inner.len());
                 PyBytes::new(py, &bytes[..])
             },
             Some(size) => {
@@ -61,15 +61,15 @@
                 self.inner = self.inner.slice(1..);
                 PyBytes::new(py, &bytes[..])
             },
             _ => PyBytes::new(py, b"")
         }
     }
 
-    #[args(_hint="None")]
+    #[pyo3(signature = (_hint=None))]
     fn readlines<'p>(&mut self, py: Python<'p>, _hint: Option<PyObject>) -> &'p PyList {
         let lines: Vec<&PyBytes> = self.inner
             .split(|&c| c == LINE_SPLIT)
             .map(|item| PyBytes::new(py, &item[..]))
             .collect();
         self.inner.clear();
         PyList::new(py, lines)
```

### Comparing `granian-0.3.2/tests/apps/asgi.py` & `granian-0.4.0/tests/apps/asgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/tests/apps/rsgi.py` & `granian-0.4.0/tests/apps/rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/tests/apps/wsgi.py` & `granian-0.4.0/tests/apps/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/tests/conftest.py` & `granian-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/tests/fixtures/tls/cert.pem` & `granian-0.4.0/tests/fixtures/tls/cert.pem`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/tests/fixtures/tls/key.pem` & `granian-0.4.0/tests/fixtures/tls/key.pem`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/tests/test_asgi.py` & `granian-0.4.0/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/tests/test_https.py` & `granian-0.4.0/tests/test_https.py`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/tests/test_rsgi.py` & `granian-0.4.0/tests/test_rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/tests/test_ws.py` & `granian-0.4.0/tests/test_ws.py`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/tests/test_wsgi.py` & `granian-0.4.0/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.3.2/Cargo.lock` & `granian-0.4.0/Cargo.lock`

 * *Files 12% similar despite different names*

```diff
@@ -30,56 +30,56 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "block-buffer"
-version = "0.10.3"
+version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69cce20737498f97b993470a6e536b8523f0af7892a4f928cceb1ac5e52ebe7e"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.11.1"
+version = "3.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "572f695136211188308f16ad2ca5c851a712c464060ae6974944458eb83880ba"
+checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
 [[package]]
 name = "bytes"
-version = "1.3.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfb24e866b15a1af2a1b663f10c6b6b8f397a84aadb828f12e5b289ec23a3a3c"
+checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
 name = "cc"
-version = "1.0.78"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a20104e2335ce8a659d6dd92a51a767a0c062599c73b343fd152cb401e828c3d"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
@@ -113,88 +113,88 @@
 checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "futures"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38390104763dc37a5145a53c29c63c1290b5d316d6086ec32c293f6736051bb0"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "52ba265a92256105f45b719605a571ffe2d1f0fea3807304b522c1d778f79eed"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04909a7a7e4633ae6c4a9ab280aeb86da1236243a77b694a49eacd659a4bd3ac"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7acc85df6714c176ab5edf386123fafe217be88c0840ec11f199441134a074e2"
+checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00f5fb52a06bdcadeb54e8d3671f8888a39697dcb0b81b23b55174030427f4eb"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdfb8ce053d86b91919aad980c220b1fb8401a9394410e1c289ed7e66b61835d"
+checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39c15cf1a4aa79df40f1bb462fb39676d0ad9e366c2a33b590d7c66f4f81fcf9"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
 
 [[package]]
 name = "futures-task"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ffb393ac5d9a6eaa9d3fdf37ae2776656b706e200c8e16b1bdb227f5198e6ea"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-util"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "197676987abd2f9cadff84926f410af1c183608d36641465df73ae8211dc65d6"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -202,63 +202,63 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "granian"
-version = "0.3.2"
+version = "0.4.0"
 dependencies = [
  "bytes",
  "futures",
  "hyper",
  "log",
  "mimalloc",
  "once_cell",
  "pin-project",
  "pyo3",
  "pyo3-asyncio",
- "pyo3-build-config",
+ "pyo3-build-config 0.17.3",
  "pyo3-log",
  "rustls-pemfile",
  "socket2",
  "tls-listener",
  "tokio",
  "tokio-rustls",
  "tokio-tungstenite",
  "tokio-util",
  "tungstenite",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.15"
+version = "0.3.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f9f29bc9dda355256b2916cf526ab02ce0aeaaaf2bad60d65ef3f12f11dd0f4"
+checksum = "17f8a914c2987b688368b5138aa05321db91f4090cf26118185672ad588bce21"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -282,17 +282,17 @@
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "http"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75f43d41e26995c17e71ee126451dd3941010b0514a81a9d11f3b341debc2399"
+checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
@@ -316,17 +316,17 @@
 name = "httpdate"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
 
 [[package]]
 name = "hyper"
-version = "0.14.23"
+version = "0.14.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "034711faac9d2166cb1baf1a2fb0b60b1f277f8492fd72176c17f3515e1abd3c"
+checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
@@ -350,54 +350,54 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da2d6f23ffea9d7e76c53eee25dfb67bcd8fde7f1198b0855350698c9f07c780"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itoa"
-version = "1.0.5"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.60"
+version = "0.3.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49409df3e3bf0856b916e2ceaca09ee28e6871cf7d9ce97a692cacfdb2a25a47"
+checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "libmimalloc-sys"
-version = "0.1.30"
+version = "0.1.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8c7cbf8b89019683667e347572e6d55a7df7ea36b0c4ce69961b0cde67b174"
+checksum = "f4ac0e912c8ef1b735e92369695618dc5b1819f5a7bf3f167301a3ba1cea515e"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "lock_api"
@@ -422,79 +422,79 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mimalloc"
-version = "0.1.34"
+version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9dcb174b18635f7561a0c6c9fc2ce57218ac7523cf72c50af80e2d79ab8f3ba1"
+checksum = "4e2894987a3459f3ffb755608bd82188f8ed00d0ae077f1edea29c068d639d98"
 dependencies = [
  "libmimalloc-sys",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.5"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5d732bc30207a6423068df043e3d02e0735b155ad7ce1a6f76fe2baa5b158de"
+checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
 dependencies = [
  "libc",
  "log",
  "wasi",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.6"
+version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba1ef8814b5c993410bb3adfad7a5ed269563e4a2f90c41f5d85be7fb47133bf"
+checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
@@ -512,15 +512,15 @@
 name = "pin-project-internal"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "069bdb1e05adc7a8990dce9cc75370895fbe4e3d58b9b73bf1aee56359344a55"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
@@ -535,43 +535,43 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.49"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57a8eca9f9c4ffde41714334dee777596264c7825420f521abc92b5b5deb63a5"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
- "pyo3-build-config",
+ "pyo3-build-config 0.18.3",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-asyncio"
-version = "0.17.0"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1febe3946b26194628f00526929ee6f8559f9e807f811257e94d4c456103be0e"
+checksum = "d3564762e37035cfc486228e10b0528460fa026d681b5763873c693aa0d5c260"
 dependencies = [
  "futures",
  "once_cell",
  "pin-project-lite",
  "pyo3",
  "tokio",
 ]
@@ -583,62 +583,72 @@
 checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
+name = "pyo3-build-config"
+version = "0.18.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+dependencies = [
+ "once_cell",
+ "target-lexicon",
+]
+
+[[package]]
 name = "pyo3-ffi"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
- "pyo3-build-config",
+ "pyo3-build-config 0.18.3",
 ]
 
 [[package]]
 name = "pyo3-log"
-version = "0.7.0"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5695ccff5060c13ca1751cf8c857a12da9b0bf0378cb071c5e0326f7c7e4c1b"
+checksum = "f9c8b57fe71fb5dcf38970ebedc2b1531cf1c14b1b9b4c560a182a57e115575c"
 dependencies = [
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -739,103 +749,114 @@
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51e73328dc4ac0c7ccbda3a494dfa03df1de2f46018127f60c693f2648455b0"
+checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "slab"
-version = "0.4.7"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4614a76b2a8be0058caa9dbbaf66d988527d86d003c11a94fbd335d7661edcef"
+checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "socket2"
-version = "0.4.7"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02e2d2db9033d13a1567121ddd7a095ee144db4e1ca1b1bda3419bc0da294ebd"
+checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
+name = "syn"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "thiserror"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fb327af4685e4d03fa8cbcf1716380da910eeb2bb8be417e7f9fd3fb164f36f"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
  "tinyvec_macros",
 ]
 
 [[package]]
 name = "tinyvec_macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cda74da7e1a664f795bb1f8a87ec406fb89a02522cf6e50620d016add6dbbf5c"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tls-listener"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c9d4ff21187d434ac7709bfc7441ca88f63681247e5ad99f0f08c8c91ddc103d"
 dependencies = [
@@ -845,41 +866,40 @@
  "thiserror",
  "tokio",
  "tokio-rustls",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.24.1"
+version = "1.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d9f76183f91ecfb55e1d7d5602bd1d979e38a3a522fe900241cf195624d67ae"
+checksum = "c3c786bf8134e5a3a166db9b29ab8f48134739014a3eca7bc6bfa95d673b136f"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
- "memchr",
  "mio",
  "num_cpus",
  "parking_lot",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "1.8.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d266c00fde287f55d3f1c3e96c500c362a2b8c695076ec180f27918820bc6df8"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.23.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c43ee83903113e03984cb9e5cebe6c04a5116269e900e3ddba8f068a62adda59"
@@ -899,17 +919,17 @@
  "log",
  "tokio",
  "tungstenite",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.4"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bb2e075f03b3d66d8d8785356224ba688d2906a371015e225beeb65ca92c740"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
@@ -970,23 +990,23 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.8"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "099b7128301d285f79ddd55b9a83d5e6b9e97c92e0ea0daebee7263e932de992"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -1042,71 +1062,71 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.83"
+version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eaf9f5aceeec8be17c128b2e93e031fb8a4d469bb9c4ae2d7dc1888b26887268"
+checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.83"
+version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8ffb332579b0557b52d268b91feab8df3615f265d5270fec2a8c95b17c1142"
+checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.83"
+version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "052be0f94026e6cbc75cdefc9bae13fd6052cdcaf532fa6c45e7ae33a1e6c810"
+checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.83"
+version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07bc0c051dc5f23e307b13285f9d75df86bfdf816c5721e573dec1f9b8aa193c"
+checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.83"
+version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c38c045535d93ec4f0b4defec448e4291638ee608530863b1e2ba115d4fff7f"
+checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
 
 [[package]]
 name = "web-sys"
-version = "0.3.60"
+version = "0.3.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcda906d8be16e728fd5adc5b729afad4e444e106ab28cd1c7256e54fa61510f"
+checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki"
@@ -1138,61 +1158,136 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
+version = "0.45.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+dependencies = [
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
+name = "windows-targets"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+dependencies = [
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
+]
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+
+[[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

