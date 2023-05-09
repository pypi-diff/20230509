# Comparing `tmp/pybrook-0.1.3.tar.gz` & `tmp/pybrook-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybrook-0.1.3.tar", max compression
+gzip compressed data, was "pybrook-0.1.4.tar", max compression
```

## Comparing `pybrook-0.1.3.tar` & `pybrook-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    34916 2023-05-09 13:38:36.699045 pybrook-0.1.3/LICENSE.md
--rw-r--r--   0        0        0     6563 2023-05-09 14:48:44.826974 pybrook-0.1.3/docs/index.md
--rw-r--r--   0        0        0      958 2023-05-09 13:38:36.706045 pybrook-0.1.3/pybrook/__init__.py
--rw-r--r--   0        0        0     6237 2023-05-09 13:38:36.706045 pybrook-0.1.3/pybrook/__main__.py
--rw-r--r--   0        0        0     1461 2023-05-09 13:38:36.706045 pybrook-0.1.3/pybrook/config.py
--rw-r--r--   0        0        0      701 2023-05-09 13:38:36.706045 pybrook-0.1.3/pybrook/consumers/__init__.py
--rw-r--r--   0        0        0    10592 2023-05-09 13:38:36.706045 pybrook-0.1.3/pybrook/consumers/base.py
--rw-r--r--   0        0        0     7310 2023-05-09 13:38:36.707045 pybrook-0.1.3/pybrook/consumers/dependency_resolver.py
--rw-r--r--   0        0        0     4541 2023-05-09 14:49:20.159821 pybrook-0.1.3/pybrook/consumers/field_generator.py
--rw-r--r--   0        0        0     5231 2023-05-09 13:38:36.707045 pybrook-0.1.3/pybrook/consumers/splitter.py
--rw-r--r--   0        0        0     6138 2023-05-09 13:38:36.707045 pybrook-0.1.3/pybrook/consumers/worker.py
--rw-r--r--   0        0        0     1720 2023-05-09 13:38:36.707045 pybrook-0.1.3/pybrook/encoding.py
--rw-r--r--   0        0        0      701 2023-05-09 13:38:36.707045 pybrook-0.1.3/pybrook/examples/__init__.py
--rw-r--r--   0        0        0     2571 2023-05-09 13:38:36.708045 pybrook-0.1.3/pybrook/examples/demo.py
--rw-r--r--   0        0        0     2469 2023-05-09 13:38:36.708045 pybrook-0.1.3/pybrook/examples/ztm.py
--rw-r--r--   0        0        0   697071 2023-05-09 13:38:36.712045 pybrook-0.1.3/pybrook/frontend/build/bundle.css
--rw-r--r--   0        0        0   263192 2023-05-09 13:38:36.715045 pybrook-0.1.3/pybrook/frontend/build/bundle.js
--rw-r--r--   0        0        0   875724 2023-05-09 13:38:36.724045 pybrook-0.1.3/pybrook/frontend/build/bundle.js.map
--rw-r--r--   0        0        0     3127 2023-05-09 13:38:36.724045 pybrook-0.1.3/pybrook/frontend/favicon.png
--rw-r--r--   0        0        0      890 2023-05-09 13:38:36.724045 pybrook-0.1.3/pybrook/frontend/global.css
--rw-r--r--   0        0        0      386 2023-05-09 13:38:36.724045 pybrook-0.1.3/pybrook/frontend/index.html
--rw-r--r--   0        0        0    32825 2023-05-09 13:38:36.724045 pybrook-0.1.3/pybrook/models.py
--rw-r--r--   0        0        0     2238 2023-05-09 13:38:36.725045 pybrook-0.1.3/pybrook/schemas.py
--rw-r--r--   0        0        0     1711 2023-05-09 14:30:42.261475 pybrook-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7950 1970-01-01 00:00:00.000000 pybrook-0.1.3/setup.py
--rw-r--r--   0        0        0     7754 1970-01-01 00:00:00.000000 pybrook-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-05-09 13:38:36.699045 pybrook-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0     6563 2023-05-09 14:48:44.826974 pybrook-0.1.4/docs/index.md
+-rw-r--r--   0        0        0      958 2023-05-09 13:38:36.706045 pybrook-0.1.4/pybrook/__init__.py
+-rw-r--r--   0        0        0     6237 2023-05-09 13:38:36.706045 pybrook-0.1.4/pybrook/__main__.py
+-rw-r--r--   0        0        0     1461 2023-05-09 13:38:36.706045 pybrook-0.1.4/pybrook/config.py
+-rw-r--r--   0        0        0      701 2023-05-09 13:38:36.706045 pybrook-0.1.4/pybrook/consumers/__init__.py
+-rw-r--r--   0        0        0    10592 2023-05-09 13:38:36.706045 pybrook-0.1.4/pybrook/consumers/base.py
+-rw-r--r--   0        0        0     7310 2023-05-09 13:38:36.707045 pybrook-0.1.4/pybrook/consumers/dependency_resolver.py
+-rw-r--r--   0        0        0     4541 2023-05-09 14:49:20.159821 pybrook-0.1.4/pybrook/consumers/field_generator.py
+-rw-r--r--   0        0        0     5231 2023-05-09 13:38:36.707045 pybrook-0.1.4/pybrook/consumers/splitter.py
+-rw-r--r--   0        0        0     6138 2023-05-09 13:38:36.707045 pybrook-0.1.4/pybrook/consumers/worker.py
+-rw-r--r--   0        0        0     1720 2023-05-09 13:38:36.707045 pybrook-0.1.4/pybrook/encoding.py
+-rw-r--r--   0        0        0      701 2023-05-09 13:38:36.707045 pybrook-0.1.4/pybrook/examples/__init__.py
+-rw-r--r--   0        0        0     2571 2023-05-09 13:38:36.708045 pybrook-0.1.4/pybrook/examples/demo.py
+-rw-r--r--   0        0        0     2469 2023-05-09 13:38:36.708045 pybrook-0.1.4/pybrook/examples/ztm.py
+-rw-r--r--   0        0        0   697071 2023-05-09 13:38:36.712045 pybrook-0.1.4/pybrook/frontend/build/bundle.css
+-rw-r--r--   0        0        0   263192 2023-05-09 13:38:36.715045 pybrook-0.1.4/pybrook/frontend/build/bundle.js
+-rw-r--r--   0        0        0   875724 2023-05-09 13:38:36.724045 pybrook-0.1.4/pybrook/frontend/build/bundle.js.map
+-rw-r--r--   0        0        0     3127 2023-05-09 13:38:36.724045 pybrook-0.1.4/pybrook/frontend/favicon.png
+-rw-r--r--   0        0        0      890 2023-05-09 13:38:36.724045 pybrook-0.1.4/pybrook/frontend/global.css
+-rw-r--r--   0        0        0      386 2023-05-09 13:38:36.724045 pybrook-0.1.4/pybrook/frontend/index.html
+-rw-r--r--   0        0        0    32825 2023-05-09 13:38:36.724045 pybrook-0.1.4/pybrook/models.py
+-rw-r--r--   0        0        0     2238 2023-05-09 13:38:36.725045 pybrook-0.1.4/pybrook/schemas.py
+-rw-r--r--   0        0        0     1836 2023-05-09 14:52:21.956032 pybrook-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     8055 1970-01-01 00:00:00.000000 pybrook-0.1.4/setup.py
+-rw-r--r--   0        0        0     7935 1970-01-01 00:00:00.000000 pybrook-0.1.4/PKG-INFO
```

### Comparing `pybrook-0.1.3/LICENSE.md` & `pybrook-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/docs/index.md` & `pybrook-0.1.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/__init__.py` & `pybrook-0.1.4/pybrook/__init__.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/__main__.py` & `pybrook-0.1.4/pybrook/__main__.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/config.py` & `pybrook-0.1.4/pybrook/config.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/consumers/__init__.py` & `pybrook-0.1.4/pybrook/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/consumers/base.py` & `pybrook-0.1.4/pybrook/consumers/base.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/consumers/dependency_resolver.py` & `pybrook-0.1.4/pybrook/consumers/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/consumers/field_generator.py` & `pybrook-0.1.4/pybrook/consumers/field_generator.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/consumers/splitter.py` & `pybrook-0.1.4/pybrook/consumers/splitter.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/consumers/worker.py` & `pybrook-0.1.4/pybrook/consumers/worker.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/encoding.py` & `pybrook-0.1.4/pybrook/encoding.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/examples/__init__.py` & `pybrook-0.1.4/pybrook/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/examples/demo.py` & `pybrook-0.1.4/pybrook/examples/demo.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/examples/ztm.py` & `pybrook-0.1.4/pybrook/examples/ztm.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/frontend/build/bundle.css` & `pybrook-0.1.4/pybrook/frontend/build/bundle.css`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/frontend/build/bundle.js` & `pybrook-0.1.4/pybrook/frontend/build/bundle.js`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/frontend/build/bundle.js.map` & `pybrook-0.1.4/pybrook/frontend/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/frontend/favicon.png` & `pybrook-0.1.4/pybrook/frontend/favicon.png`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/frontend/global.css` & `pybrook-0.1.4/pybrook/frontend/global.css`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/models.py` & `pybrook-0.1.4/pybrook/models.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pybrook/schemas.py` & `pybrook-0.1.4/pybrook/schemas.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.3/pyproject.toml` & `pybrook-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.poetry]
 name = "pybrook"
-version = "0.1.3"
-description = ""
+version = "0.1.4"
+description = "PyBrook - a real-time cloud computing framework for the Internet of Things."
+repository = "https://github.com/pybrook/pybrook"
 authors = ["Michał Rokita <mrokita@mrokita.pl>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [tool.poetry.scripts]
 pybrook = "pybrook.__main__:main"
```

### Comparing `pybrook-0.1.3/setup.py` & `pybrook-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,22 +24,22 @@
  'watchdog>=2.1.6,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['pybrook = pybrook.__main__:main']}
 
 setup_kwargs = {
     'name': 'pybrook',
-    'version': '0.1.3',
-    'description': '',
+    'version': '0.1.4',
+    'description': 'PyBrook - a real-time cloud computing framework for the Internet of Things.',
     'long_description': '# Introduction\n\nPyBrook - a real-time cloud computing framework for the Internet of Things.\nPyBrook enables users to define complex data processing models declaratively using the Python programming language.\nThe framework also provides a generic web interface that presents the collected data in real-time.\n\nPyBrook aims to make the development of real-time data processing services as easy as possible by utilising powerful \nmechanisms of the Python programming language and modern concepts like hot-reloading or deploying software in Linux Containers.\n\nA simple `docker-compose up` is enough to start playing with the framework.\n\n## Run demo with Docker\n\nIt is recommended to use `docker-compose` for learning (you can use the `docker-compose.yml` from the [project repository](https://github.com/pybrook/pybrook/blob/master/docker-compose.yml):\n\n```bash\ndocker-compose up\n```\n\nThis command will start all the services, including Redis with Redis Gears enabled.\n\nThe following services will be available:\n\n- OpenAPI docs (ReDoc): <http://localhost:8000/redoc> \n- OpenAPI docs (Swagger UI): <http://localhost:8000/docs> \n- PyBrook frontend: <http://localhost:8000/panel> \n- Locust panel for load testing: <http://localhost:8089>\n\nYou should probably visit the Locust panel first and start sending some reports.\n\n### Using your own model\n\nThe configured model is `pybrook.examples.demo`, but replacing it with your own is very easy.  \nFirst, you have to save your custom model somewhere. \nFor now, you can just copy the source of `pybrook.examples.demo` (attached below) and save it as `mymodel.py` in your working directory.\n\n??? example "Source of `pybrook.examples.demo`"\n\n    ```python linenums="1"\n    from datetime import datetime\n    from math import atan2, degrees\n    from typing import Optional, Sequence\n    \n    from pybrook.models import (\n        InReport,\n        OutReport,\n        PyBrook,\n        ReportField,\n        dependency,\n        historical_dependency,\n    )\n    \n    brook = PyBrook(\'redis://localhost\')\n    app = brook.app\n    \n    \n    @brook.input(\'ztm-report\', id_field=\'vehicle_number\')\n    class ZTMReport(InReport):\n        vehicle_number: int\n        time: datetime\n        lat: float\n        lon: float\n        brigade: str\n        line: str\n    \n    \n    @brook.output(\'location-report\')\n    class LocationReport(OutReport):\n        vehicle_number = ReportField(ZTMReport.vehicle_number)\n        lat = ReportField(ZTMReport.lat)\n        lon = ReportField(ZTMReport.lon)\n        line = ReportField(ZTMReport.line)\n        time = ReportField(ZTMReport.time)\n        brigade = ReportField(ZTMReport.brigade)\n    \n    \n    @brook.artificial_field()\n    def direction(lat_history: Sequence[float] = historical_dependency(\n        ZTMReport.lat, history_length=1),\n                        lon_history: Sequence[float] = historical_dependency(\n                            ZTMReport.lon, history_length=1),\n                        lat: float = dependency(ZTMReport.lat),\n                        lon: float = dependency(ZTMReport.lon)) -> Optional[float]:\n        prev_lat, = lat_history\n        prev_lon, = lon_history\n        if prev_lat and prev_lon:\n            return degrees(atan2(lon - prev_lon, lat - prev_lat))\n        else:\n            return None\n    \n    \n    @brook.output(\'direction-report\')\n    class DirectionReport(OutReport):\n        direction = ReportField(direction)\n    \n    \n    @brook.artificial_field()\n    async def counter(prev_values: Sequence[int] = historical_dependency(\n        \'counter\', history_length=1),\n                      time: datetime = dependency(ZTMReport.time)) -> int:\n        prev_value, = prev_values\n        if prev_value is None:\n            prev_value = -1\n        prev_value += 1\n        return prev_value\n    \n    \n    @brook.output(\'counter-report\')\n    class CounterReport(OutReport):\n        counter = ReportField(counter)\n    \n    \n    brook.set_meta(latitude_field=LocationReport.lat,\n                   longitude_field=LocationReport.lon,\n                   time_field=LocationReport.time,\n                   group_field=LocationReport.line,\n                   direction_field=DirectionReport.direction)\n    \n    if __name__ == \'__main__\':\n        brook.run()\n    ```\n\nAfter creating `mymodel.py`, you should add it to the `api` and `worker` containers, using a Docker volume.\nTo make PyBrook use `mymodel` instead of `pybrook.examples.demo`, you should also alter the arguments passed to `gunicorn` and `pybrook`. \nYou can simply add it to the default `docker-compose.yml`:\n\n```yaml hl_lines="20 21 10 11 12 13 14 24" linenums="1"\nservices:\n  api:\n    image: pybrook:latest\n    build:\n      context: .\n    environment:\n      REDIS_URL: redis://redis\n    ports:\n      - 8000:8000\n    volumes:\n      - ./mymodel.py:/src/mymodel.py\n    command: gunicorn mymodel:app \n          -w 4 -k uvicorn.workers.UvicornWorker \n          -b 0.0.0.0:8000\n  worker:\n    image: pybrook:latest\n    depends_on:\n      - api\n    environment:\n      REDIS_URL: redis://redis\n      DEFAULT_WORKERS: 8\n    volumes:\n      - ./mymodel.py:/src/mymodel.py\n    command: pybrook mymodel:brook\n  locust:\n    image: pybrook:latest\n    depends_on:\n      - api\n    ports:\n      - 8089:8089\n    command: locust -H http://api:8000\n  redis:\n    image: redislabs/redisgears:latest\n```\n\nThen run `docker-compose up --build` again, to start PyBrook - this time using your own model.\n\n## Setup & Development\n\nYou can install the PyBrook from PyPi using `pip`:\n\n```bash\npip install pybrook\n```\n\n## Running all services manually, without Docker\n\nTo run the `pybrook.examples.demo` model, you have to start all the required services manually:\n\n```bash\n# Redis + Redis Gears\ndocker run --net=host -d redislabs/redisgears\n# HTTP API based on pybrook.examples.demo - uvicorn\nuvicorn pybrook.examples.demo:app --reload  \n# PyBrook workers based on pybrook.examples.demo \npybrook pybrook.examples.demo:brook   \n# Locust - load testing\nlocust -H http://localhost:8000\n```\n\n## Contributing\n\nPyBrook uses [poetry](https://python-poetry.org) for dependency management.\nTo install all its development dependencies, simply run this command:\n\n```bash\npoetry install\n```\n\n### Tests\n\n```bash\nmake test\n```\n\n### Code quality\n\nThe source code of PyBrook is formatted using yapf and isort.  \nTo run them with the correct settings, use the following command:\n\n```bash\nmake format\n```\n\nPyBrook uses `mypy` for type checking and `flake8` for linting.\nUse the following command to run them with the appropriate settings:\n\n```bash\nmake lint\n```',
     'author': 'Michał Rokita',
     'author_email': 'mrokita@mrokita.pl',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/pybrook/pybrook',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `pybrook-0.1.3/PKG-INFO` & `pybrook-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pybrook
-Version: 0.1.3
-Summary: 
+Version: 0.1.4
+Summary: PyBrook - a real-time cloud computing framework for the Internet of Things.
+Home-page: https://github.com/pybrook/pybrook
 License: GPL-3.0-or-later
 Author: Michał Rokita
 Author-email: mrokita@mrokita.pl
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -23,14 +24,15 @@
 Requires-Dist: pandoc-crossref (>=0.1.1,<0.2.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: pytest (>=6.2.5,<7.0.0)
 Requires-Dist: redis[asyncio] (>=4.5.1,<5.0.0)
 Requires-Dist: uvicorn[standard] (>=0.20.0,<0.21.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Requires-Dist: watchdog (>=2.1.6,<3.0.0)
+Project-URL: Repository, https://github.com/pybrook/pybrook
 Description-Content-Type: text/markdown
 
 # Introduction
 
 PyBrook - a real-time cloud computing framework for the Internet of Things.
 PyBrook enables users to define complex data processing models declaratively using the Python programming language.
 The framework also provides a generic web interface that presents the collected data in real-time.
```

