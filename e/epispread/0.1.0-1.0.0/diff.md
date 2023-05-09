# Comparing `tmp/epispread-0.1.0.tar.gz` & `tmp/epispread-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epispread-0.1.0.tar", last modified: Mon Mar 27 05:07:47 2023, max compression
+gzip compressed data, was "epispread-1.0.0.tar", last modified: Tue May  9 15:59:16 2023, max compression
```

## Comparing `epispread-0.1.0.tar` & `epispread-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,51 @@
-drwxr-xr-x   0 siennabrent   (501) staff       (20)        0 2023-03-27 05:07:47.326236 epispread-0.1.0/
--rw-r--r--   0 siennabrent   (501) staff       (20)      408 2023-03-27 05:01:03.000000 epispread-0.1.0/.bumpversion.cfg
--rw-r--r--   0 siennabrent   (501) staff       (20)      523 2023-03-27 05:01:03.000000 epispread-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 siennabrent   (501) staff       (20)     1069 2023-02-19 22:31:32.000000 epispread-0.1.0/LICENSE
--rw-r--r--   0 siennabrent   (501) staff       (20)      413 2023-03-11 03:28:01.000000 epispread-0.1.0/MANIFEST.in
--rw-r--r--   0 siennabrent   (501) staff       (20)     2427 2023-03-11 04:17:32.000000 epispread-0.1.0/Makefile
--rw-r--r--   0 siennabrent   (501) staff       (20)     4058 2023-03-27 05:07:47.326085 epispread-0.1.0/PKG-INFO
--rw-r--r--   0 siennabrent   (501) staff       (20)     1993 2023-03-27 05:01:03.000000 epispread-0.1.0/README.md
-drwxr-xr-x   0 siennabrent   (501) staff       (20)        0 2023-03-27 05:07:47.317128 epispread-0.1.0/epispread/
--rw-r--r--   0 siennabrent   (501) staff       (20) 12326863 2023-03-03 02:58:24.000000 epispread-0.1.0/epispread/WHO-COVID-19-global-data.csv
--rw-r--r--   0 siennabrent   (501) staff       (20)       66 2023-03-03 21:28:29.000000 epispread-0.1.0/epispread/__init__.py
--rw-r--r--   0 siennabrent   (501) staff       (20)       85 2023-03-03 21:28:29.000000 epispread-0.1.0/epispread/__main__.py
--rw-r--r--   0 siennabrent   (501) staff       (20)       22 2023-03-03 04:35:25.000000 epispread-0.1.0/epispread/_version.py
--rw-r--r--   0 siennabrent   (501) staff       (20)    13809 2023-03-03 02:58:24.000000 epispread-0.1.0/epispread/poc_country.csv
--rw-r--r--   0 siennabrent   (501) staff       (20)     2501 2023-03-03 02:58:24.000000 epispread-0.1.0/epispread/resolve.csv
--rw-r--r--   0 siennabrent   (501) staff       (20)     2995 2023-03-27 05:01:03.000000 epispread-0.1.0/epispread/skeleton.py
-drwxr-xr-x   0 siennabrent   (501) staff       (20)        0 2023-03-27 05:07:47.325784 epispread-0.1.0/epispread/tests/
--rw-r--r--   0 siennabrent   (501) staff       (20)      319 2023-03-03 22:52:23.000000 epispread-0.1.0/epispread/tests/test-db.csv
--rw-r--r--   0 siennabrent   (501) staff       (20)     6033 2023-03-03 22:52:23.000000 epispread-0.1.0/epispread/tests/test-world.csv
--rw-r--r--   0 siennabrent   (501) staff       (20)     2381 2023-03-27 05:01:03.000000 epispread-0.1.0/epispread/tests/test_all.py
--rw-r--r--   0 siennabrent   (501) staff       (20)  1784274 2023-03-03 02:58:24.000000 epispread-0.1.0/epispread/time_series_covid19_confirmed_global.csv
--rw-r--r--   0 siennabrent   (501) staff       (20)   378115 2023-03-11 04:08:08.000000 epispread-0.1.0/epispread/world.csv
-drwxr-xr-x   0 siennabrent   (501) staff       (20)        0 2023-03-27 05:07:47.324916 epispread-0.1.0/epispread.egg-info/
--rw-r--r--   0 siennabrent   (501) staff       (20)     4058 2023-03-27 05:07:47.000000 epispread-0.1.0/epispread.egg-info/PKG-INFO
--rw-r--r--   0 siennabrent   (501) staff       (20)      592 2023-03-27 05:07:47.000000 epispread-0.1.0/epispread.egg-info/SOURCES.txt
--rw-r--r--   0 siennabrent   (501) staff       (20)        1 2023-03-27 05:07:47.000000 epispread-0.1.0/epispread.egg-info/dependency_links.txt
--rw-r--r--   0 siennabrent   (501) staff       (20)      156 2023-03-27 05:07:47.000000 epispread-0.1.0/epispread.egg-info/requires.txt
--rw-r--r--   0 siennabrent   (501) staff       (20)       10 2023-03-27 05:07:47.000000 epispread-0.1.0/epispread.egg-info/top_level.txt
--rw-r--r--   0 siennabrent   (501) staff       (20)     2171 2023-03-27 05:01:03.000000 epispread-0.1.0/pyproject.toml
--rw-r--r--   0 siennabrent   (501) staff       (20)       38 2023-03-27 05:07:47.326288 epispread-0.1.0/setup.cfg
--rw-r--r--   0 siennabrent   (501) staff       (20)       39 2023-03-03 04:35:25.000000 epispread-0.1.0/setup.py
+drwxr-xr-x   0 siennabrent   (501) staff       (20)        0 2023-05-09 15:59:16.478220 epispread-1.0.0/
+-rw-r--r--   0 siennabrent   (501) staff       (20)      408 2023-05-09 00:25:32.000000 epispread-1.0.0/.bumpversion.cfg
+-rw-r--r--   0 siennabrent   (501) staff       (20)        0 2023-04-06 04:02:02.000000 epispread-1.0.0/.nojekyll
+-rw-r--r--   0 siennabrent   (501) staff       (20)      709 2023-04-05 04:53:15.000000 epispread-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 siennabrent   (501) staff       (20)      523 2023-05-09 00:13:52.000000 epispread-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0 siennabrent   (501) staff       (20)     1069 2023-05-09 00:13:52.000000 epispread-1.0.0/LICENSE
+-rw-r--r--   0 siennabrent   (501) staff       (20)      810 2023-05-09 00:13:52.000000 epispread-1.0.0/MANIFEST.in
+-rw-r--r--   0 siennabrent   (501) staff       (20)     2746 2023-05-09 00:13:52.000000 epispread-1.0.0/Makefile
+-rw-r--r--   0 siennabrent   (501) staff       (20)     4474 2023-05-09 15:59:16.478066 epispread-1.0.0/PKG-INFO
+-rw-r--r--   0 siennabrent   (501) staff       (20)     2409 2023-05-09 00:13:52.000000 epispread-1.0.0/README.md
+drwxr-xr-x   0 siennabrent   (501) staff       (20)        0 2023-05-09 15:59:16.470871 epispread-1.0.0/docs/
+-rw-r--r--   0 siennabrent   (501) staff       (20)      634 2023-05-09 00:13:52.000000 epispread-1.0.0/docs/Makefile
+-rw-r--r--   0 siennabrent   (501) staff       (20)      462 2023-05-09 15:57:20.000000 epispread-1.0.0/docs/api.rst
+-rw-r--r--   0 siennabrent   (501) staff       (20)     1093 2023-05-09 15:57:20.000000 epispread-1.0.0/docs/conf.py
+drwxr-xr-x   0 siennabrent   (501) staff       (20)        0 2023-05-09 15:59:16.472651 epispread-1.0.0/docs/images/
+-rw-r--r--   0 siennabrent   (501) staff       (20)   146250 2023-05-09 00:13:52.000000 epispread-1.0.0/docs/images/mappic+180.jpg
+-rw-r--r--   0 siennabrent   (501) staff       (20)   130507 2023-05-09 00:13:52.000000 epispread-1.0.0/docs/images/mappic+280.jpg
+-rw-r--r--   0 siennabrent   (501) staff       (20)   138325 2023-05-09 00:13:52.000000 epispread-1.0.0/docs/images/mappic+80.jpg
+-rw-r--r--   0 siennabrent   (501) staff       (20)      900 2023-05-09 15:57:20.000000 epispread-1.0.0/docs/index.rst
+-rw-r--r--   0 siennabrent   (501) staff       (20)      765 2023-05-09 00:13:52.000000 epispread-1.0.0/docs/make.bat
+-rw-r--r--   0 siennabrent   (501) staff       (20)     1390 2023-05-09 00:13:52.000000 epispread-1.0.0/docs/requirements.txt
+drwxr-xr-x   0 siennabrent   (501) staff       (20)        0 2023-05-09 15:59:16.474058 epispread-1.0.0/epispread/
+-rw-r--r--   0 siennabrent   (501) staff       (20)      160 2023-05-09 00:13:52.000000 epispread-1.0.0/epispread/__init__.py
+-rw-r--r--   0 siennabrent   (501) staff       (20)        0 2023-05-09 00:13:52.000000 epispread-1.0.0/epispread/__main__.py
+-rw-r--r--   0 siennabrent   (501) staff       (20)       22 2023-05-09 00:25:32.000000 epispread-1.0.0/epispread/_version.py
+drwxr-xr-x   0 siennabrent   (501) staff       (20)        0 2023-05-09 15:59:16.475552 epispread-1.0.0/epispread/graph_classes/
+-rw-r--r--   0 siennabrent   (501) staff       (20)        0 2023-05-09 00:13:52.000000 epispread-1.0.0/epispread/graph_classes/__init__.py
+-rw-r--r--   0 siennabrent   (501) staff       (20)     4751 2023-05-09 00:13:52.000000 epispread-1.0.0/epispread/graph_classes/heat_map.py
+-rw-r--r--   0 siennabrent   (501) staff       (20)      734 2023-05-09 00:25:32.000000 epispread-1.0.0/epispread/graph_classes/time_series.py
+drwxr-xr-x   0 siennabrent   (501) staff       (20)        0 2023-05-09 15:59:16.476972 epispread-1.0.0/epispread/images/
+-rw-r--r--   0 siennabrent   (501) staff       (20)   146250 2023-05-09 00:13:52.000000 epispread-1.0.0/epispread/images/mappic+180.jpg
+-rw-r--r--   0 siennabrent   (501) staff       (20)   130507 2023-05-09 00:13:52.000000 epispread-1.0.0/epispread/images/mappic+280.jpg
+-rw-r--r--   0 siennabrent   (501) staff       (20)   138325 2023-05-09 00:13:52.000000 epispread-1.0.0/epispread/images/mappic+80.jpg
+-rw-r--r--   0 siennabrent   (501) staff       (20)     8670 2023-05-09 00:25:32.000000 epispread-1.0.0/epispread/skeleton.py
+drwxr-xr-x   0 siennabrent   (501) staff       (20)        0 2023-05-09 15:59:16.477632 epispread-1.0.0/epispread/tests/
+drwxr-xr-x   0 siennabrent   (501) staff       (20)        0 2023-05-09 15:59:16.477812 epispread-1.0.0/epispread/tests/data_files/
+-rw-r--r--   0 siennabrent   (501) staff       (20)       27 2023-05-09 00:13:52.000000 epispread-1.0.0/epispread/tests/data_files/file.csv
+-rw-r--r--   0 siennabrent   (501) staff       (20)      237 2023-05-09 00:13:52.000000 epispread-1.0.0/epispread/tests/test-db.csv
+-rw-r--r--   0 siennabrent   (501) staff       (20)     6033 2023-05-09 00:13:52.000000 epispread-1.0.0/epispread/tests/test-world.csv
+-rw-r--r--   0 siennabrent   (501) staff       (20)     6640 2023-05-09 00:13:52.000000 epispread-1.0.0/epispread/tests/test_all.py
+drwxr-xr-x   0 siennabrent   (501) staff       (20)        0 2023-05-09 15:59:16.475030 epispread-1.0.0/epispread.egg-info/
+-rw-r--r--   0 siennabrent   (501) staff       (20)     4474 2023-05-09 15:59:16.000000 epispread-1.0.0/epispread.egg-info/PKG-INFO
+-rw-r--r--   0 siennabrent   (501) staff       (20)      901 2023-05-09 15:59:16.000000 epispread-1.0.0/epispread.egg-info/SOURCES.txt
+-rw-r--r--   0 siennabrent   (501) staff       (20)        1 2023-05-09 15:59:16.000000 epispread-1.0.0/epispread.egg-info/dependency_links.txt
+-rw-r--r--   0 siennabrent   (501) staff       (20)      156 2023-05-09 15:59:16.000000 epispread-1.0.0/epispread.egg-info/requires.txt
+-rw-r--r--   0 siennabrent   (501) staff       (20)       10 2023-05-09 15:59:16.000000 epispread-1.0.0/epispread.egg-info/top_level.txt
+-rw-r--r--   0 siennabrent   (501) staff       (20)     2171 2023-05-09 00:25:32.000000 epispread-1.0.0/pyproject.toml
+-rw-r--r--   0 siennabrent   (501) staff       (20)     1390 2023-05-09 00:13:52.000000 epispread-1.0.0/requirements.txt
+-rw-r--r--   0 siennabrent   (501) staff       (20)       38 2023-05-09 15:59:16.478261 epispread-1.0.0/setup.cfg
+-rw-r--r--   0 siennabrent   (501) staff       (20)      104 2023-05-09 00:13:52.000000 epispread-1.0.0/setup.py
+-rw-r--r--   0 siennabrent   (501) staff       (20)       46 2023-05-08 18:58:15.000000 epispread-1.0.0/test.txt
```

### Comparing `epispread-0.1.0/CONTRIBUTING.md` & `epispread-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `epispread-0.1.0/LICENSE` & `epispread-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `epispread-0.1.0/Makefile` & `epispread-1.0.0/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 # BUILD #
 #########
 develop:  ## install dependencies and build library
 	python3 -m pip install -e .[develop]
 	python3 -m pip install pandas
 	python3 -m pip install geopandas
 	python3 -m pip install country-converter
+	python3 -m pip install requests-mock
 	python3 -m pip install matplotlib
 	python3 -m pip install datetime
 
 build:  ## build the python3 library
 	python3 setup.py build build_ext --inplace
 
 install:  ## install library
 	python3 -m pip install .
 
 #########
 # LINTS #
 #########
 lint:  ## run static analysis with flake8
 	python3 -m black --check epispread setup.py
-	python3 -m flake8 epispread setup.py
 
 # Alias
 lints: lint
 
 format:  ## run autoformatting with black
 	python3 -m black epispread/ setup.py
 
@@ -97,7 +97,22 @@
 help:
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
 print-%:
 	@echo '$*=$($*)'
 
 .PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help
+
+#########
+# PAGES #
+#########
+
+TMPREPO=/tmp/docs/epispread
+pages: 
+	rm -rf $(TMPREPO)
+	git clone -b gh-pages https://github.com/scb-school/epi-spread-visualizer.git $(TMPREPO)
+	rm -rf $(TMPREPO)/*
+	cp -r docs/_build/html/* $(TMPREPO)
+	cd $(TMPREPO);\
+	git add -A ;\
+	git commit -a -m 'auto-updating docs' ;\
+	git push
```

### Comparing `epispread-0.1.0/PKG-INFO` & `epispread-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epispread
-Version: 0.1.0
+Version: 1.0.0
 Summary: Tool for visualizing disease spread
 Author-email: Sienna <scb2197@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Sienna Brent
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,21 +39,25 @@
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # epi-spread-visualizer
 Tool to visualize disease spread based on input data.
 
-![](https://img.shields.io/github/license/scb-school/epi-spread-visualizer)
-![](https://img.shields.io/github/issues/scb-school/epi-spread-visualizer)
+![License](https://img.shields.io/github/license/scb-school/epi-spread-visualizer)
+![Issues](https://img.shields.io/github/issues/scb-school/epi-spread-visualizer)
+[![PyPI](https://img.shields.io/pypi/v/epispread)](https://pypi.org/project/epispread/0.1.0)
+
 # Overview
 With this library, I am creating a tool that will assist in visualizing the spread of a disease according to an inputted line listing of populations becoming sick over time, translating this data into a map that will change based on a slider simulating the passage of time. My library will use data visualization tools already in place, such as Plotly DASH, as well as some data-processing tools like Python Pandas, combining these two to make the final result.
 
 [![Build Status](https://github.com/scb-school/epi-spread-visualizer/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/scb-school/epi-spread-visualizer/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/scb-school/epi-spread-visualizer/branch/main/graph/badge.svg)](https://codecov.io/gh/scb-school/epi-spread-visualizer)
+[![Documentation Status](https://readthedocs.org/projects/epi-spread-visualizer/badge/?version=latest)](https://epi-spread-visualizer.readthedocs.io/en/latest/?badge=latest)
+![GitHub Pages](https://img.shields.io/website?label=GitHub%20Pages&url=https%3A%2F%2Fscb-school.github.io%2Fepi-spread-visualizer%2F)
 
 ## Details
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
```

### Comparing `epispread-0.1.0/README.md` & `epispread-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # epi-spread-visualizer
 Tool to visualize disease spread based on input data.
 
-![](https://img.shields.io/github/license/scb-school/epi-spread-visualizer)
-![](https://img.shields.io/github/issues/scb-school/epi-spread-visualizer)
+![License](https://img.shields.io/github/license/scb-school/epi-spread-visualizer)
+![Issues](https://img.shields.io/github/issues/scb-school/epi-spread-visualizer)
+[![PyPI](https://img.shields.io/pypi/v/epispread)](https://pypi.org/project/epispread/0.1.0)
+
 # Overview
 With this library, I am creating a tool that will assist in visualizing the spread of a disease according to an inputted line listing of populations becoming sick over time, translating this data into a map that will change based on a slider simulating the passage of time. My library will use data visualization tools already in place, such as Plotly DASH, as well as some data-processing tools like Python Pandas, combining these two to make the final result.
 
 [![Build Status](https://github.com/scb-school/epi-spread-visualizer/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/scb-school/epi-spread-visualizer/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/scb-school/epi-spread-visualizer/branch/main/graph/badge.svg)](https://codecov.io/gh/scb-school/epi-spread-visualizer)
+[![Documentation Status](https://readthedocs.org/projects/epi-spread-visualizer/badge/?version=latest)](https://epi-spread-visualizer.readthedocs.io/en/latest/?badge=latest)
+![GitHub Pages](https://img.shields.io/website?label=GitHub%20Pages&url=https%3A%2F%2Fscb-school.github.io%2Fepi-spread-visualizer%2F)
 
 ## Details
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
```

### Comparing `epispread-0.1.0/epispread/tests/test-world.csv` & `epispread-1.0.0/epispread/tests/test-world.csv`

 * *Files identical despite different names*

### Comparing `epispread-0.1.0/epispread.egg-info/PKG-INFO` & `epispread-1.0.0/epispread.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epispread
-Version: 0.1.0
+Version: 1.0.0
 Summary: Tool for visualizing disease spread
 Author-email: Sienna <scb2197@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Sienna Brent
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,21 +39,25 @@
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # epi-spread-visualizer
 Tool to visualize disease spread based on input data.
 
-![](https://img.shields.io/github/license/scb-school/epi-spread-visualizer)
-![](https://img.shields.io/github/issues/scb-school/epi-spread-visualizer)
+![License](https://img.shields.io/github/license/scb-school/epi-spread-visualizer)
+![Issues](https://img.shields.io/github/issues/scb-school/epi-spread-visualizer)
+[![PyPI](https://img.shields.io/pypi/v/epispread)](https://pypi.org/project/epispread/0.1.0)
+
 # Overview
 With this library, I am creating a tool that will assist in visualizing the spread of a disease according to an inputted line listing of populations becoming sick over time, translating this data into a map that will change based on a slider simulating the passage of time. My library will use data visualization tools already in place, such as Plotly DASH, as well as some data-processing tools like Python Pandas, combining these two to make the final result.
 
 [![Build Status](https://github.com/scb-school/epi-spread-visualizer/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/scb-school/epi-spread-visualizer/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/scb-school/epi-spread-visualizer/branch/main/graph/badge.svg)](https://codecov.io/gh/scb-school/epi-spread-visualizer)
+[![Documentation Status](https://readthedocs.org/projects/epi-spread-visualizer/badge/?version=latest)](https://epi-spread-visualizer.readthedocs.io/en/latest/?badge=latest)
+![GitHub Pages](https://img.shields.io/website?label=GitHub%20Pages&url=https%3A%2F%2Fscb-school.github.io%2Fepi-spread-visualizer%2F)
 
 ## Details
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
```

### Comparing `epispread-0.1.0/pyproject.toml` & `epispread-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "epispread"
 authors = [{name = "Sienna", email = "scb2197@columbia.edu"}]
 description="Tool for visualizing disease spread"
 readme = "README.md"
-version = "0.1.0"
+version = "1.0.0"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

