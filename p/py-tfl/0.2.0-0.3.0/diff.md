# Comparing `tmp/py_tfl-0.2.0.tar.gz` & `tmp/py_tfl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_tfl-0.2.0.tar", max compression
+gzip compressed data, was "py_tfl-0.3.0.tar", max compression
```

## Comparing `py_tfl-0.2.0.tar` & `py_tfl-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1068 2023-05-07 20:36:18.972115 py_tfl-0.2.0/LICENSE
--rw-r--r--   0        0        0     4221 2023-05-07 20:36:18.972115 py_tfl-0.2.0/README.md
--rw-r--r--   0        0        0     2346 2023-05-07 20:36:18.976115 py_tfl-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      121 2023-05-07 20:36:18.976115 py_tfl-0.2.0/tfl/__init__.py
--rw-r--r--   0        0        0       68 2023-05-07 20:36:18.976115 py_tfl-0.2.0/tfl/cli/__init__.py
--rw-r--r--   0        0        0     1345 2023-05-07 20:36:18.976115 py_tfl-0.2.0/tfl/cli/_async_typer.py
--rw-r--r--   0        0        0     1656 2023-05-07 20:36:18.976115 py_tfl-0.2.0/tfl/cli/main.py
--rw-r--r--   0        0        0        0 2023-05-07 20:36:18.976115 py_tfl-0.2.0/tfl/cli/py.typed
--rw-r--r--   0        0        0      298 2023-05-07 20:36:18.976115 py_tfl-0.2.0/tfl/clients/__init__.py
--rw-r--r--   0        0        0     4650 2023-05-07 20:36:18.976115 py_tfl-0.2.0/tfl/clients/_accident_stats_client.py
--rw-r--r--   0        0        0     1696 2023-05-07 20:36:18.976115 py_tfl-0.2.0/tfl/clients/_auth.py
--rw-r--r--   0        0        0     5000 2023-05-07 20:36:18.976115 py_tfl-0.2.0/tfl/clients/_client.py
--rw-r--r--   0        0        0     4463 2023-05-07 20:36:18.976115 py_tfl-0.2.0/tfl/clients/_lift_disruptions_client.py
--rw-r--r--   0        0        0        0 2023-05-07 20:36:18.976115 py_tfl-0.2.0/tfl/clients/py.typed
--rw-r--r--   0        0        0        0 2023-05-07 20:36:18.976115 py_tfl-0.2.0/tfl/py.typed
--rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 py_tfl-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-09 18:55:40.123287 py_tfl-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4316 2023-05-09 18:55:40.123287 py_tfl-0.3.0/README.md
+-rw-r--r--   0        0        0     2346 2023-05-09 18:55:40.127288 py_tfl-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/cli/__init__.py
+-rw-r--r--   0        0        0     1345 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/cli/_async_typer.py
+-rw-r--r--   0        0        0     2056 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/cli/main.py
+-rw-r--r--   0        0        0        0 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/cli/py.typed
+-rw-r--r--   0        0        0      359 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/clients/__init__.py
+-rw-r--r--   0        0        0     4650 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/clients/_accident_stats_client.py
+-rw-r--r--   0        0        0     4484 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/clients/_air_quality_client.py
+-rw-r--r--   0        0        0     1696 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/clients/_auth.py
+-rw-r--r--   0        0        0     5000 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/clients/_client.py
+-rw-r--r--   0        0        0     4463 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/clients/_lift_disruptions_client.py
+-rw-r--r--   0        0        0        0 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/clients/py.typed
+-rw-r--r--   0        0        0        0 2023-05-09 18:55:40.127288 py_tfl-0.3.0/tfl/py.typed
+-rw-r--r--   0        0        0     5490 1970-01-01 00:00:00.000000 py_tfl-0.3.0/PKG-INFO
```

### Comparing `py_tfl-0.2.0/LICENSE` & `py_tfl-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_tfl-0.2.0/README.md` & `py_tfl-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,18 +14,21 @@
 A Python package for the [Transport for London (TFL) API](https://api-portal.tfl.gov.uk).
 
 The TFL API is a RESTful API that provides data related to all modes of transport in London, including cycle hire,
 buses, roads, and the underground. Anonymous access to the TFL API is limited to 50 requests a minute. If you want to
 call the API more than that, you'll need to subscribe to a "Product" which lets you bypass this limit with a
 subscription-key that you append to your requests.
 
-Currently, this package only supports the
-[Lift Disruptions API](https://api-portal.tfl.gov.uk/api-details#api=Disruptions-Lifts-v2&operation=get) and
-[Accident Stats API](https://api-portal.tfl.gov.uk/api-details#api=AccidentStats&operation=AccidentStats_Get). However,
-the plan is to add support for all the TFL APIs. Contributions are welcome!
+Currently, we support the following APIs:
+
+- [Accident Stats API](https://api-portal.tfl.gov.uk/api-details#api=AccidentStats&operation=AccidentStats_Get)
+- [Air Quality API](https://api-portal.tfl.gov.uk/api-details#api=AirQuality&operation=AirQuality_Get)
+- [Lift Disruptions API](https://api-portal.tfl.gov.uk/api-details#api=Disruptions-Lifts-v2&operation=get)
+
+The plan is to add support for all the TFL APIs. Contributions are welcome!
 
 ## Installation
 
 ```bash
 pip install py-tfl
 ```
```

### Comparing `py_tfl-0.2.0/pyproject.toml` & `py_tfl-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "py-tfl"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Python package for the Transport for London (TFL) API."
 authors = ["Cellan Hall <hallcellan@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "tfl"},
 ]
 homepage = "https://ce11an.github.io/tfl/"
```

### Comparing `py_tfl-0.2.0/tfl/cli/_async_typer.py` & `py_tfl-0.3.0/tfl/cli/_async_typer.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.2.0/tfl/cli/main.py` & `py_tfl-0.3.0/tfl/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,25 @@
     """Gets all accident details for accidents occurring in the specified year."""
     async with clients.AccidentStatsClient(auth=tfl.clients.Auth(key=key) if key else None) as client:
         response = await client.get_accident_stats(year=year)
     rich.print(response.json())
     raise typer.Exit()
 
 
+@app.async_command()
+async def air_quality(
+    key: Annotated[Optional[str], typer.Argument(envvar="TFL_API_KEY", help="TFL API key.")] = None,
+) -> None:
+    """Get air quality data feed."""
+    async with clients.AirQualityClient(auth=tfl.clients.Auth(key=key) if key else None) as client:
+        response = await client.get_air_quality()
+    rich.print(response.json())
+    raise typer.Exit()
+
+
 # noinspection PyUnusedLocal
 @app.callback()
 def main(
     version: Annotated[
         bool, typer.Option("--version", callback=version_callback, is_eager=True, help="Show the version and exit.")
     ] = False
 ) -> None:
```

### Comparing `py_tfl-0.2.0/tfl/clients/_accident_stats_client.py` & `py_tfl-0.3.0/tfl/clients/_accident_stats_client.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.2.0/tfl/clients/_auth.py` & `py_tfl-0.3.0/tfl/clients/_auth.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.2.0/tfl/clients/_client.py` & `py_tfl-0.3.0/tfl/clients/_client.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.2.0/tfl/clients/_lift_disruptions_client.py` & `py_tfl-0.3.0/tfl/clients/_lift_disruptions_client.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.2.0/PKG-INFO` & `py_tfl-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tfl
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python package for the Transport for London (TFL) API.
 Home-page: https://ce11an.github.io/tfl/
 Author: Cellan Hall
 Author-email: hallcellan@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -42,18 +42,21 @@
 A Python package for the [Transport for London (TFL) API](https://api-portal.tfl.gov.uk).
 
 The TFL API is a RESTful API that provides data related to all modes of transport in London, including cycle hire,
 buses, roads, and the underground. Anonymous access to the TFL API is limited to 50 requests a minute. If you want to
 call the API more than that, you'll need to subscribe to a "Product" which lets you bypass this limit with a
 subscription-key that you append to your requests.
 
-Currently, this package only supports the
-[Lift Disruptions API](https://api-portal.tfl.gov.uk/api-details#api=Disruptions-Lifts-v2&operation=get) and
-[Accident Stats API](https://api-portal.tfl.gov.uk/api-details#api=AccidentStats&operation=AccidentStats_Get). However,
-the plan is to add support for all the TFL APIs. Contributions are welcome!
+Currently, we support the following APIs:
+
+- [Accident Stats API](https://api-portal.tfl.gov.uk/api-details#api=AccidentStats&operation=AccidentStats_Get)
+- [Air Quality API](https://api-portal.tfl.gov.uk/api-details#api=AirQuality&operation=AirQuality_Get)
+- [Lift Disruptions API](https://api-portal.tfl.gov.uk/api-details#api=Disruptions-Lifts-v2&operation=get)
+
+The plan is to add support for all the TFL APIs. Contributions are welcome!
 
 ## Installation
 
 ```bash
 pip install py-tfl
 ```
```

