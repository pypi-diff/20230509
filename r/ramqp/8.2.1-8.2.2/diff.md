# Comparing `tmp/ramqp-8.2.1.tar.gz` & `tmp/ramqp-8.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramqp-8.2.1.tar", max compression
+gzip compressed data, was "ramqp-8.2.2.tar", max compression
```

## Comparing `ramqp-8.2.1.tar` & `ramqp-8.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0        0        0        0 2023-04-18 15:38:13.433533 ramqp-8.2.1/LICENSES/
--rw-r--r--   0        0        0    15177 2023-04-18 15:38:13.433533 ramqp-8.2.1/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     7466 2023-04-18 15:38:13.434533 ramqp-8.2.1/README.md
--rw-r--r--   0        0        0     1460 2023-04-18 15:38:27.666185 ramqp-8.2.1/pyproject.toml
--rw-r--r--   0        0        0      321 2023-04-18 15:38:13.437533 ramqp-8.2.1/ramqp/__init__.py
--rw-r--r--   0        0        0    13047 2023-04-18 15:38:13.437533 ramqp-8.2.1/ramqp/abstract.py
--rw-r--r--   0        0        0      668 2023-04-18 15:38:13.438534 ramqp-8.2.1/ramqp/amqp.py
--rw-r--r--   0        0        0     2729 2023-04-18 15:38:13.438534 ramqp-8.2.1/ramqp/config.py
--rw-r--r--   0        0        0     8841 2023-04-18 15:38:13.439534 ramqp-8.2.1/ramqp/depends.py
--rw-r--r--   0        0        0     7010 2023-04-18 15:38:13.439534 ramqp-8.2.1/ramqp/metrics.py
--rw-r--r--   0        0        0     8537 2023-04-18 15:38:13.440534 ramqp-8.2.1/ramqp/mo.py
--rw-r--r--   0        0        0        0 2023-04-18 15:38:13.491540 ramqp-8.2.1/ramqp/py.typed
--rw-r--r--   0        0        0     1367 2023-04-18 15:38:13.440534 ramqp-8.2.1/ramqp/utils.py
--rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 ramqp-8.2.1/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-05-09 10:47:02.065215 ramqp-8.2.2/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-05-09 10:47:02.065215 ramqp-8.2.2/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     7466 2023-05-09 10:47:02.066215 ramqp-8.2.2/README.md
+-rw-r--r--   0        0        0     1460 2023-05-09 10:47:23.495078 ramqp-8.2.2/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-05-09 10:47:02.068215 ramqp-8.2.2/ramqp/__init__.py
+-rw-r--r--   0        0        0    13047 2023-05-09 10:47:02.068215 ramqp-8.2.2/ramqp/abstract.py
+-rw-r--r--   0        0        0      668 2023-05-09 10:47:02.068215 ramqp-8.2.2/ramqp/amqp.py
+-rw-r--r--   0        0        0     2729 2023-05-09 10:47:02.068215 ramqp-8.2.2/ramqp/config.py
+-rw-r--r--   0        0        0     8841 2023-05-09 10:47:02.069216 ramqp-8.2.2/ramqp/depends.py
+-rw-r--r--   0        0        0     7010 2023-05-09 10:47:02.069216 ramqp-8.2.2/ramqp/metrics.py
+-rw-r--r--   0        0        0     8537 2023-05-09 10:47:02.069216 ramqp-8.2.2/ramqp/mo.py
+-rw-r--r--   0        0        0        0 2023-05-09 10:47:02.241230 ramqp-8.2.2/ramqp/py.typed
+-rw-r--r--   0        0        0     1367 2023-05-09 10:47:02.070216 ramqp-8.2.2/ramqp/utils.py
+-rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 ramqp-8.2.2/PKG-INFO
```

### Comparing `ramqp-8.2.1/LICENSES/MPL-2.0.txt` & `ramqp-8.2.2/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.1/README.md` & `ramqp-8.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.1/pyproject.toml` & `ramqp-8.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ramqp"
-version = "8.2.1"
+version = "8.2.2"
 description = "Rammearkitektur AMQP library (aio_pika wrapper)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ramqp"
 keywords = ["os2mo", "amqp"]
 packages = [ { include = "ramqp" } ]
 include = ["ramqp/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aio-pika = ">=8.3,<10.0"
-structlog = "^22.3.0"
+structlog = "^23.1.0"
 prometheus-client = "^0.16.0"
 pydantic = "^1.10.5"
 more-itertools = "^9.1.0"
 fastapi = ">=0.95.0,<1.0"
 anyio = "^3.6.2"
 ra-utils = "^1.12.4"
```

### Comparing `ramqp-8.2.1/ramqp/abstract.py` & `ramqp-8.2.2/ramqp/abstract.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.1/ramqp/amqp.py` & `ramqp-8.2.2/ramqp/amqp.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.1/ramqp/config.py` & `ramqp-8.2.2/ramqp/config.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.1/ramqp/depends.py` & `ramqp-8.2.2/ramqp/depends.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.1/ramqp/metrics.py` & `ramqp-8.2.2/ramqp/metrics.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.1/ramqp/mo.py` & `ramqp-8.2.2/ramqp/mo.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.1/ramqp/utils.py` & `ramqp-8.2.2/ramqp/utils.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.2.1/PKG-INFO` & `ramqp-8.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramqp
-Version: 8.2.1
+Version: 8.2.2
 Summary: Rammearkitektur AMQP library (aio_pika wrapper)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
@@ -15,15 +15,15 @@
 Requires-Dist: aio-pika (>=8.3,<10.0)
 Requires-Dist: anyio (>=3.6.2,<4.0.0)
 Requires-Dist: fastapi (>=0.95.0,<1.0)
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: ra-utils (>=1.12.4,<2.0.0)
-Requires-Dist: structlog (>=22.3.0,<23.0.0)
+Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Project-URL: Repository, https://git.magenta.dk/rammearkitektur/ramqp
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: 2021 Magenta ApS <https://magenta.dk>
 SPDX-License-Identifier: MPL-2.0
 -->
```

