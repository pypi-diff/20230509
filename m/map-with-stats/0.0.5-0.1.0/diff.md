# Comparing `tmp/map_with_stats-0.0.5.tar.gz` & `tmp/map_with_stats-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "map_with_stats-0.0.5.tar", last modified: Mon May  8 21:00:09 2023, max compression
+gzip compressed data, was "map_with_stats-0.1.0.tar", last modified: Tue May  9 12:34:21 2023, max compression
```

## Comparing `map_with_stats-0.0.5.tar` & `map_with_stats-0.1.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:09.075065 map_with_stats-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:09.063065 map_with_stats-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:09.067066 map_with_stats-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/.github/workflows/publish_prod.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/.github/workflows/publish_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/.github/workflows/publish_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:09.067066 map_with_stats-0.0.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-05-08 21:00:09.075065 map_with_stats-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:09.067066 map_with_stats-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/docs/faq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:09.067066 map_with_stats-0.0.5/docs/figs/
--rw-r--r--   0 runner    (1001) docker     (123)  5399925 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/docs/figs/map_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:09.071066 map_with_stats-0.0.5/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/environment/linux.env
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/environment/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/environment/requirements_lib.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/environment/windows.env
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 21:00:09.075065 map_with_stats-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:09.063065 map_with_stats-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:09.071066 map_with_stats-0.0.5/src/map_with_stats/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/src/map_with_stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 21:00:08.000000 map_with_stats-0.0.5/src/map_with_stats/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/src/map_with_stats/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/src/map_with_stats/map.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/src/map_with_stats/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/src/map_with_stats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:09.075065 map_with_stats-0.0.5/src/map_with_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-05-08 21:00:09.000000 map_with_stats-0.0.5/src/map_with_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-08 21:00:09.000000 map_with_stats-0.0.5/src/map_with_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:00:09.000000 map_with_stats-0.0.5/src/map_with_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-08 21:00:09.000000 map_with_stats-0.0.5/src/map_with_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 21:00:09.000000 map_with_stats-0.0.5/src/map_with_stats.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:09.075065 map_with_stats-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-08 20:59:59.000000 map_with_stats-0.0.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.896114 map_with_stats-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.892114 map_with_stats-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.892114 map_with_stats-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.github/workflows/publish_prod.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.github/workflows/publish_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.892114 map_with_stats-0.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-09 12:34:21.896114 map_with_stats-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.892114 map_with_stats-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/docs/faq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.892114 map_with_stats-0.1.0/docs/figs/
+-rw-r--r--   0 runner    (1001) docker     (123)  1021823 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/docs/figs/map_screenshot.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.896114 map_with_stats-0.1.0/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/environment/linux.env
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/environment/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/environment/requirements_lib.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/environment/windows.env
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 12:34:21.896114 map_with_stats-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.892114 map_with_stats-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.896114 map_with_stats-0.1.0/src/map_with_stats/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/src/map_with_stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 12:34:21.000000 map_with_stats-0.1.0/src/map_with_stats/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/src/map_with_stats/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/src/map_with_stats/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/src/map_with_stats/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/src/map_with_stats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.896114 map_with_stats-0.1.0/src/map_with_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-09 12:34:21.000000 map_with_stats-0.1.0/src/map_with_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-09 12:34:21.000000 map_with_stats-0.1.0/src/map_with_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 12:34:21.000000 map_with_stats-0.1.0/src/map_with_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 12:34:21.000000 map_with_stats-0.1.0/src/map_with_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 12:34:21.000000 map_with_stats-0.1.0/src/map_with_stats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.896114 map_with_stats-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/tests/test_utils.py
```

### Comparing `map_with_stats-0.0.5/.github/workflows/docs.yml` & `map_with_stats-0.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.0.5/.github/workflows/publish_template.yml` & `map_with_stats-0.1.0/.github/workflows/publish_template.yml`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     name: Upload release to PyPI
     runs-on: ubuntu-latest
     environment:
       name: ${{ inputs.environment-name }}
       url: ${{ inputs.environment-url }}
     steps:
       - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0 # Needs all tags to compute dynamic version
       - name: 🐍 Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.9"
       - name: 💻 Install dependencies
         run: pip install build
       - name: 🔨 Build distribution
```

### Comparing `map_with_stats-0.0.5/.github/workflows/test.yml` & `map_with_stats-0.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.0.5/.gitignore` & `map_with_stats-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.0.5/.pre-commit-config.yaml` & `map_with_stats-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.0.5/.vscode/settings.json` & `map_with_stats-0.1.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.0.5/LICENSE` & `map_with_stats-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.0.5/PKG-INFO` & `map_with_stats-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: map_with_stats
-Version: 0.0.5
+Version: 0.1.0
 Summary: Interactive map with a choropleth displaying some statistics as color per hectare
 Author: Mischa Lisovyi
 License: MIT License
         
         Copyright (c) 2023 Mischa Lisovyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,15 +60,15 @@
 
 The package allows to display an interactive map with a choropleth
 displaying some statistics as color per hectare (100x100 meter square).
 
 The package is created and tested to work for the **Switzerland coordinates**,
 however, one could try to use it for any other map with hectare statistics.
 
-![Example map](https://github.com/mlisovyi/map_with_stats/raw/main/docs/figs/map_screenshot.png)
+![Example map](https://github.com/mlisovyi/map_with_stats/raw/main/docs/figs/map_screenshot.jpeg)
 
 
 ## Installation
 
 ```bash
 pip install map_with_stats
 ```
```

### Comparing `map_with_stats-0.0.5/README.md` & `map_with_stats-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 The package allows to display an interactive map with a choropleth
 displaying some statistics as color per hectare (100x100 meter square).
 
 The package is created and tested to work for the **Switzerland coordinates**,
 however, one could try to use it for any other map with hectare statistics.
 
-![Example map](https://github.com/mlisovyi/map_with_stats/raw/main/docs/figs/map_screenshot.png)
+![Example map](https://github.com/mlisovyi/map_with_stats/raw/main/docs/figs/map_screenshot.jpeg)
 
 
 ## Installation
 
 ```bash
 pip install map_with_stats
 ```
```

### Comparing `map_with_stats-0.0.5/docs/index.md` & `map_with_stats-0.1.0/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 The package allows to display an interactive map with a choropleth
 displaying some statistics as color per hectare (100x100 meter square).
 
 The package is created and tested to work for the **Switzerland coordinates**,
 however, one could try to use it for any other map with hectare statistics.
 
-![Example map](https://github.com/mlisovyi/map_with_stats/raw/main/docs/figs/map_screenshot.png)
+![Example map](https://github.com/mlisovyi/map_with_stats/raw/main/docs/figs/map_screenshot.jpeg)
 
 
 ## Installation
 
 ```bash
 pip install map_with_stats
 ```
```

### Comparing `map_with_stats-0.0.5/mkdocs.yml` & `map_with_stats-0.1.0/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,17 @@
       permalink: true
 
   # Python Markdown Extensions
   - pymdownx.betterem:
       smart_enable: all
   - pymdownx.caret
   - pymdownx.details
+  - pymdownx.highlight
+  - pymdownx.inlinehilite
+  - pymdownx.superfences
   - pymdownx.tilde
 
 plugins:
   - search
   - mkdocstrings:
       handlers:
         python:
```

### Comparing `map_with_stats-0.0.5/pyproject.toml` & `map_with_stats-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 # the tool that generates a file with package version based on the latest tag
 # this file is **NOT** part of the git repository, as it changes with every commit
 [tool.setuptools_scm]
 write_to = "src/map_with_stats/_version.py"
 version_scheme = "post-release"
+local_scheme = "no-local-version"
 
 [project]
 name = "map_with_stats"
 dynamic = ["version"]
 authors = [{name="Mischa Lisovyi"}]
 description = "Interactive map with a choropleth displaying some statistics as color per hectare"
 readme = "README.md"
```

### Comparing `map_with_stats-0.0.5/src/map_with_stats/data.py` & `map_with_stats-0.1.0/src/map_with_stats/data.py`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.0.5/src/map_with_stats/map.py` & `map_with_stats-0.1.0/src/map_with_stats/map.py`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.0.5/src/map_with_stats/utils.py` & `map_with_stats-0.1.0/src/map_with_stats/utils.py`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.0.5/src/map_with_stats.egg-info/PKG-INFO` & `map_with_stats-0.1.0/src/map_with_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: map-with-stats
-Version: 0.0.5
+Version: 0.1.0
 Summary: Interactive map with a choropleth displaying some statistics as color per hectare
 Author: Mischa Lisovyi
 License: MIT License
         
         Copyright (c) 2023 Mischa Lisovyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,15 +60,15 @@
 
 The package allows to display an interactive map with a choropleth
 displaying some statistics as color per hectare (100x100 meter square).
 
 The package is created and tested to work for the **Switzerland coordinates**,
 however, one could try to use it for any other map with hectare statistics.
 
-![Example map](https://github.com/mlisovyi/map_with_stats/raw/main/docs/figs/map_screenshot.png)
+![Example map](https://github.com/mlisovyi/map_with_stats/raw/main/docs/figs/map_screenshot.jpeg)
 
 
 ## Installation
 
 ```bash
 pip install map_with_stats
 ```
```

### Comparing `map_with_stats-0.0.5/src/map_with_stats.egg-info/SOURCES.txt` & `map_with_stats-0.1.0/src/map_with_stats.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 .github/workflows/publish_template.yml
 .github/workflows/publish_test.yml
 .github/workflows/test.yml
 .vscode/settings.json
 docs/api.md
 docs/faq.md
 docs/index.md
-docs/figs/map_screenshot.png
+docs/figs/map_screenshot.jpeg
 environment/linux.env
 environment/requirements_dev.txt
 environment/requirements_lib.txt
 environment/windows.env
 src/map_with_stats/__init__.py
 src/map_with_stats/_version.py
 src/map_with_stats/data.py
```

### Comparing `map_with_stats-0.0.5/tests/test_data.py` & `map_with_stats-0.1.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.0.5/tests/test_utils.py` & `map_with_stats-0.1.0/tests/test_utils.py`

 * *Files identical despite different names*

