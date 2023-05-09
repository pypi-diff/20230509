# Comparing `tmp/amplitude-data-wrapper-0.3.8.tar.gz` & `tmp/amplitude_data_wrapper-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amplitude-data-wrapper-0.3.8.tar", max compression
+gzip compressed data, was "amplitude_data_wrapper-0.3.9.tar", max compression
```

## Comparing `amplitude-data-wrapper-0.3.8.tar` & `amplitude_data_wrapper-0.3.9.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1062 2022-08-16 12:59:05.385355 amplitude-data-wrapper-0.3.8/LICENSE
--rw-r--r--   0        0        0     4322 2022-08-16 12:31:25.379733 amplitude-data-wrapper-0.3.8/README.md
--rw-r--r--   0        0        0      757 2022-08-16 18:31:12.887150 amplitude-data-wrapper-0.3.8/pyproject.toml
--rw-r--r--   0        0        0       51 2022-08-16 12:31:25.380519 amplitude-data-wrapper-0.3.8/src/amplitude_data_wrapper/__init__.py
--rw-r--r--   0        0        0    15281 2022-08-16 18:48:41.479058 amplitude-data-wrapper-0.3.8/src/amplitude_data_wrapper/analytics_api.py
--rw-r--r--   0        0        0     5301 2022-08-16 19:06:50.128277 amplitude-data-wrapper-0.3.8/setup.py
--rw-r--r--   0        0        0     5163 2022-08-16 19:06:50.128695 amplitude-data-wrapper-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-08-16 12:59:05.385355 amplitude_data_wrapper-0.3.9/LICENSE
+-rw-r--r--   0        0        0     4322 2022-08-16 12:31:25.379733 amplitude_data_wrapper-0.3.9/README.md
+-rw-r--r--   0        0        0       51 2022-08-16 12:31:25.380519 amplitude_data_wrapper-0.3.9/amplitude_data_wrapper/__init__.py
+-rw-r--r--   0        0        0    15281 2022-08-16 18:48:41.479058 amplitude_data_wrapper-0.3.9/amplitude_data_wrapper/analytics_api.py
+-rw-r--r--   0        0        0      842 2023-05-09 10:05:32.345651 amplitude_data_wrapper-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     5214 1970-01-01 00:00:00.000000 amplitude_data_wrapper-0.3.9/PKG-INFO
```

### Comparing `amplitude-data-wrapper-0.3.8/LICENSE` & `amplitude_data_wrapper-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.3.8/README.md` & `amplitude_data_wrapper-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.3.8/pyproject.toml` & `amplitude_data_wrapper-0.3.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amplitude-data-wrapper"
-version = "0.3.8"
+version = "0.3.9"
 description = "python wrapper for using the amplitude analytics and taxonomy APIs"
 authors = ["Tobias McVey <tobias.mcvey@nav.no>"]
 license = "MIT"
 readme="README.md"
 homepage = "https://github.com/navikt/amplitude-data-wrapper"
 repository = "https://github.com/navikt/amplitude-data-wrapper"
 documentation = "https://github.com/navikt/amplitude-data-wrapper"
@@ -19,10 +19,14 @@
 [tool.poetry.dev-dependencies]
 ipykernel = "^6.7.0"
 python-decouple = "^3.6"
 black = "^22.3.0"
 twine = "^4.0.1"
 keyring = "^23.6.0"
 
+[tool.poetry.group.dev.dependencies]
+ipykernel = "^6.21.1"
+python-dotenv = "^1.0.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `amplitude-data-wrapper-0.3.8/src/amplitude_data_wrapper/analytics_api.py` & `amplitude_data_wrapper-0.3.9/amplitude_data_wrapper/analytics_api.py`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.3.8/setup.py` & `amplitude_data_wrapper-0.3.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,191 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: amplitude-data-wrapper
+Version: 0.3.9
+Summary: python wrapper for using the amplitude analytics and taxonomy APIs
+Home-page: https://github.com/navikt/amplitude-data-wrapper
+License: MIT
+Keywords: amplitude
+Author: Tobias McVey
+Author-email: tobias.mcvey@nav.no
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: tqdm (>=4.62.3,<5.0.0)
+Project-URL: Documentation, https://github.com/navikt/amplitude-data-wrapper
+Project-URL: Repository, https://github.com/navikt/amplitude-data-wrapper
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Amplitude data wrapper
 
-packages = \
-['amplitude_data_wrapper']
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests>=2.27.1,<3.0.0', 'tqdm>=4.62.3,<5.0.0']
-
-setup_kwargs = {
-    'name': 'amplitude-data-wrapper',
-    'version': '0.3.8',
-    'description': 'python wrapper for using the amplitude analytics and taxonomy APIs',
-    'long_description': '# Amplitude data wrapper\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nThis is a wrapper for [Amplitude](https://amplitude.com/) APIs. You can use it to query and export data from your account and use the taxonomy API.\n\nBuilt with [requests](https://requests.readthedocs.io/en/latest/) and [tqdm](https://github.com/tqdm/tqdm)\n\n**Why use this package instead of other wrappers?**\n\nThis package supports regions and so you can use it with Amplitude accounts in the EU and USA.\n\nThis package also supports using a proxy so you can keep your project API keys and API secrets confidential.\n\n## Supported Amplitude APIs and docs\n\n- [Amplitude data wrapper](#amplitude-data-wrapper)\n  - [Supported Amplitude APIs and docs](#supported-amplitude-apis-and-docs)\n    - [Dashboard Rest API](#dashboard-rest-api)\n    - [Privacy API](#privacy-api)\n    - [Cohort API](#cohort-api)\n    - [Export API](#export-api)\n    - [Taxonomy API](#taxonomy-api)\n\nSee examples below and in [example.py](example.py)\n\nInstall with\n\n```\npip install amplitude-data-wrapper\n```\n\n### Dashboard Rest API\n\n[Results from an existing chart](https://developers.amplitude.com/docs/dashboard-rest-api#results-from-an-existing-chart)\n\nGet data from EU account by setting `region=1`.\n\n```python\nfrom amplitude_data_wrapper import get_chart\n\nr = get_chart(chart_id, api_key, api_secret, region=1)\nr.status_code  # 200\nr.text # print data\n```\n\nGet data from US account by setting `region=2`.\n\n```python\nfrom amplitude_data_wrapper import get_chart\n\nr = get_chart(chart_id, api_key, api_secret, region=2)\nr.status_code  # 200\nr.text # print data\n```\n\nGet data from EU account with a proxy by setting region and proxy using a dictionary.\n\n```python\nfrom amplitude_data_wrapper import get_chart\n\nproxies = {"http": "http://myproxy.domain.org/path"}\nr = get_chart(chart_id, api_key, api_secret, region=1, proxy=proxies)\nr.status_code  # 200\nr.text # print data\n```\n\n[Event segmentation](https://developers.amplitude.com/docs/dashboard-rest-api#event-segmentation) lets you export events with segments and filters.\n\n```python\nour_event_dict = {\n    "event_type": "pageview",\n    "group_by": [{"type": "event", "value": "app"}, {"type": "event", "value": "team"}],\n}\ndata = get_event_segmentation(\n    api_key=api_key,\n    secret=api_secret,\n    start="20220601",\n    end="20220602",\n    event=our_event_dict,\n    metrics="uniques",\n    interval=1,\n    limit=1000,\n)\n```\n\n[User search](https://developers.amplitude.com/docs/dashboard-rest-api#user-search) lets you search for a user with a specific Amplitude ID, Device ID, User ID, or User ID prefix.\n\n```python\nuser = find_user(\n    user=example_id_eu, \n    api_key=api_key, \n    secret=api_secret,\n    region=1)\n```\n\n### Privacy API\n\nDelete user data with a [deletion job](https://developers.amplitude.com/docs/user-deletion#deletion-job)\n\n```python\ndeleteme = delete_user_data(\n    user["matches"][0]["amplitude_id"],\n    email=email,\n    api_key=api_key,\n    secret=api_secret,\n    region=1,\n    ignore_invalid_id=True,\n    delete_from_org=False,\n)\n```\n\n[Get a list of deletion jobs](https://developers.amplitude.com/docs/user-deletion#get)\n\n```python\ntobe_deleted = get_deletion_jobs(\n    start="2022-06-01",\n    end="2022-07-01",\n    api_key=api_key,\n    secret=api_secret,\n    region=1,\n)\n```\n\n### Cohort API\n\n[Getting one cohort](https://developers.amplitude.com/docs/behavioral-cohorts-api#getting-one-cohort)\n\n```python\nproxies = {"http": "http://myproxy.domain.org/path"}\nfile_path = "path-to/cohortdata.csv"\nkull = get_cohort(\n    api_key,\n    api_secret,\n    cohort_id,\n    filename=file_path,\n    props=1,\n    region=1,\n    proxy=proxies,\n)\n```\n\n### Export API\n\n[Export API - Export your project\'s event data](https://developers.amplitude.com/docs/export-api#export-api---export-your-projects-event-data)\n\n```python\nstart = "20220601T00"\nend = "20220601T01"\ndata = export_project_data(\n    start=start,\n    end=end,\n    api_key=api_key,\n    secret=api_secret,\n    filename="path-to/projectdata_eu.zip",\n    region=1,\n)\n```\n\n### Taxonomy API\n\n[Get all event types](https://developers.amplitude.com/docs/taxonomy-api#get-all-event-types)\n\n```python\ntypes = get_all_event_types(\n    api_key=api_key, \n    secret=api_secret, \n    region=1)\n```',
-    'author': 'Tobias McVey',
-    'author_email': 'tobias.mcvey@nav.no',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/navikt/amplitude-data-wrapper',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+This is a wrapper for [Amplitude](https://amplitude.com/) APIs. You can use it to query and export data from your account and use the taxonomy API.
+
+Built with [requests](https://requests.readthedocs.io/en/latest/) and [tqdm](https://github.com/tqdm/tqdm)
+
+**Why use this package instead of other wrappers?**
+
+This package supports regions and so you can use it with Amplitude accounts in the EU and USA.
+
+This package also supports using a proxy so you can keep your project API keys and API secrets confidential.
+
+## Supported Amplitude APIs and docs
+
+- [Amplitude data wrapper](#amplitude-data-wrapper)
+  - [Supported Amplitude APIs and docs](#supported-amplitude-apis-and-docs)
+    - [Dashboard Rest API](#dashboard-rest-api)
+    - [Privacy API](#privacy-api)
+    - [Cohort API](#cohort-api)
+    - [Export API](#export-api)
+    - [Taxonomy API](#taxonomy-api)
+
+See examples below and in [example.py](example.py)
+
+Install with
+
+```
+pip install amplitude-data-wrapper
+```
+
+### Dashboard Rest API
 
+[Results from an existing chart](https://developers.amplitude.com/docs/dashboard-rest-api#results-from-an-existing-chart)
 
-setup(**setup_kwargs)
+Get data from EU account by setting `region=1`.
+
+```python
+from amplitude_data_wrapper import get_chart
+
+r = get_chart(chart_id, api_key, api_secret, region=1)
+r.status_code  # 200
+r.text # print data
+```
+
+Get data from US account by setting `region=2`.
+
+```python
+from amplitude_data_wrapper import get_chart
+
+r = get_chart(chart_id, api_key, api_secret, region=2)
+r.status_code  # 200
+r.text # print data
+```
+
+Get data from EU account with a proxy by setting region and proxy using a dictionary.
+
+```python
+from amplitude_data_wrapper import get_chart
+
+proxies = {"http": "http://myproxy.domain.org/path"}
+r = get_chart(chart_id, api_key, api_secret, region=1, proxy=proxies)
+r.status_code  # 200
+r.text # print data
+```
+
+[Event segmentation](https://developers.amplitude.com/docs/dashboard-rest-api#event-segmentation) lets you export events with segments and filters.
+
+```python
+our_event_dict = {
+    "event_type": "pageview",
+    "group_by": [{"type": "event", "value": "app"}, {"type": "event", "value": "team"}],
+}
+data = get_event_segmentation(
+    api_key=api_key,
+    secret=api_secret,
+    start="20220601",
+    end="20220602",
+    event=our_event_dict,
+    metrics="uniques",
+    interval=1,
+    limit=1000,
+)
+```
+
+[User search](https://developers.amplitude.com/docs/dashboard-rest-api#user-search) lets you search for a user with a specific Amplitude ID, Device ID, User ID, or User ID prefix.
+
+```python
+user = find_user(
+    user=example_id_eu, 
+    api_key=api_key, 
+    secret=api_secret,
+    region=1)
+```
+
+### Privacy API
+
+Delete user data with a [deletion job](https://developers.amplitude.com/docs/user-deletion#deletion-job)
+
+```python
+deleteme = delete_user_data(
+    user["matches"][0]["amplitude_id"],
+    email=email,
+    api_key=api_key,
+    secret=api_secret,
+    region=1,
+    ignore_invalid_id=True,
+    delete_from_org=False,
+)
+```
+
+[Get a list of deletion jobs](https://developers.amplitude.com/docs/user-deletion#get)
+
+```python
+tobe_deleted = get_deletion_jobs(
+    start="2022-06-01",
+    end="2022-07-01",
+    api_key=api_key,
+    secret=api_secret,
+    region=1,
+)
+```
+
+### Cohort API
+
+[Getting one cohort](https://developers.amplitude.com/docs/behavioral-cohorts-api#getting-one-cohort)
+
+```python
+proxies = {"http": "http://myproxy.domain.org/path"}
+file_path = "path-to/cohortdata.csv"
+kull = get_cohort(
+    api_key,
+    api_secret,
+    cohort_id,
+    filename=file_path,
+    props=1,
+    region=1,
+    proxy=proxies,
+)
+```
+
+### Export API
+
+[Export API - Export your project's event data](https://developers.amplitude.com/docs/export-api#export-api---export-your-projects-event-data)
+
+```python
+start = "20220601T00"
+end = "20220601T01"
+data = export_project_data(
+    start=start,
+    end=end,
+    api_key=api_key,
+    secret=api_secret,
+    filename="path-to/projectdata_eu.zip",
+    region=1,
+)
+```
+
+### Taxonomy API
+
+[Get all event types](https://developers.amplitude.com/docs/taxonomy-api#get-all-event-types)
+
+```python
+types = get_all_event_types(
+    api_key=api_key, 
+    secret=api_secret, 
+    region=1)
+```
```

