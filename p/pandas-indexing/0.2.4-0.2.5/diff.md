# Comparing `tmp/pandas-indexing-0.2.4.tar.gz` & `tmp/pandas-indexing-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-indexing-0.2.4.tar", last modified: Wed May  3 22:26:06 2023, max compression
+gzip compressed data, was "pandas-indexing-0.2.5.tar", last modified: Tue May  9 06:15:10 2023, max compression
```

## Comparing `pandas-indexing-0.2.4.tar` & `pandas-indexing-0.2.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:26:06.418072 pandas-indexing-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-03 22:26:06.418072 pandas-indexing-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:26:06.410071 pandas-indexing-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:26:06.410071 pandas-indexing-0.2.4/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   221702 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/notebooks/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 22:26:06.418072 pandas-indexing-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:26:06.402071 pandas-indexing-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:26:06.414072 pandas-indexing-0.2.4/src/pandas_indexing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:26:06.418072 pandas-indexing-0.2.4/src/pandas_indexing/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/datasets/remindhighre_power.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-03 22:25:44.000000 pandas-indexing-0.2.4/src/pandas_indexing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:26:06.418072 pandas-indexing-0.2.4/src/pandas_indexing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-03 22:26:06.000000 pandas-indexing-0.2.4/src/pandas_indexing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-03 22:26:06.000000 pandas-indexing-0.2.4/src/pandas_indexing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:26:06.000000 pandas-indexing-0.2.4/src/pandas_indexing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 22:26:06.000000 pandas-indexing-0.2.4/src/pandas_indexing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 22:26:06.000000 pandas-indexing-0.2.4/src/pandas_indexing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:15:10.876255 pandas-indexing-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-09 06:15:10.876255 pandas-indexing-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:15:10.868255 pandas-indexing-0.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:15:10.868255 pandas-indexing-0.2.5/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   362406 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/notebooks/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 06:15:10.876255 pandas-indexing-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:15:10.868255 pandas-indexing-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:15:10.872255 pandas-indexing-0.2.5/src/pandas_indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:15:10.876255 pandas-indexing-0.2.5/src/pandas_indexing/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/datasets/remindhighre_power.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-09 06:14:53.000000 pandas-indexing-0.2.5/src/pandas_indexing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:15:10.876255 pandas-indexing-0.2.5/src/pandas_indexing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-09 06:15:10.000000 pandas-indexing-0.2.5/src/pandas_indexing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-09 06:15:10.000000 pandas-indexing-0.2.5/src/pandas_indexing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:15:10.000000 pandas-indexing-0.2.5/src/pandas_indexing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-09 06:15:10.000000 pandas-indexing-0.2.5/src/pandas_indexing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 06:15:10.000000 pandas-indexing-0.2.5/src/pandas_indexing.egg-info/top_level.txt
```

### Comparing `pandas-indexing-0.2.4/CHANGELOG.rst` & `pandas-indexing-0.2.5/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 .. currentmodule:: pandas_indexing
 
 Changelog
 =========
 
+v0.2.5 (2023-05-04)
+------------------------------------------------------------
+* :func:`~core.formatlevel` and :func:`~core.extractlevel` (or their equivalents
+  :meth:`~accessors.DataFrameIdxAccessor.format` and
+  :meth:`~accessors.DataFrameIdxAccessor.extract`) make it easy to combine or split
+  index levels using format-string like templates; check examples in the guide
+  (:ref:`Selecting data`) :pull:`13`
+* :py:func:`~core.describelevel` superseeds the as-of-now deprecated
+  :py:func:`~core.summarylevel` :pull:`11`
+
 v0.2.4 (2023-05-03)
 ------------------------------------------------------------
 
 * Paper-bag release: Fix new accessors :py:func:`~accessors.IndexIdxAccessor.unique` and
   :py:func:`~accessors.IndexIdxAccessor.__repr__` and improve tests to catch trivial
   errors like these earlier :pull:`10`
```

### Comparing `pandas-indexing-0.2.4/CODE_OF_CONDUCT.md` & `pandas-indexing-0.2.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.4/CONTRIBUTING.rst` & `pandas-indexing-0.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.4/LICENSE` & `pandas-indexing-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.4/PKG-INFO` & `pandas-indexing-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.4
+Version: 0.2.5
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
```

### Comparing `pandas-indexing-0.2.4/README.rst` & `pandas-indexing-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.4/docs/api.rst` & `pandas-indexing-0.2.5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.4/docs/conf.py` & `pandas-indexing-0.2.5/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 # ones.
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.coverage",
     "sphinx.ext.doctest",
     "sphinx.ext.extlinks",
+    "sphinx.ext.autosectionlabel",
     # "sphinx.ext.ifconfig",
     "sphinx.ext.napoleon",
     "sphinx.ext.intersphinx",
     # "sphinx.ext.todo",
     # "sphinx.ext.viewcode",
     "nbsphinx",
 ]
```

### Comparing `pandas-indexing-0.2.4/docs/notebooks/introduction.ipynb` & `pandas-indexing-0.2.5/docs/notebooks/introduction.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9648662471064815%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, '# Test data set\\n')], delete: [0]}}, 5: {'outputs': "*

 * *            "{0: {'text': ['Index:\\n', ' * model    : REMIND-MAgPIE 2.1-4.3 (1)\\n', ' * scenario "*

 * *            ": DeepElec_SSP2_HighRE_Budg900 (1)\\n', ' * region   : World (1)\\n', ' * variable : "*

 * *            "Capacity|Electricity|Biomass, ... (20)\\n', ' * unit     : GW, GWh/yr (2)\\n', '\\n', "*

 * *            "'Columns:\\n', ' * <unnamed> : 2005, 2010, 2015, 2020, 2025, 2030, 2035, 2040, ... "*

 * *            "2 […]*

```diff
@@ -1,21 +1,12 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "8df2b6a3-ceed-40ca-9908-a92e55551a38",
-            "metadata": {},
-            "source": [
-                "# Introduction"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
             "id": "8096b98a",
             "metadata": {},
             "source": [
                 "Here we are giving a brief introduction in working with IAMC-styled data with pandas and pandas-indexing."
             ]
         },
         {
@@ -30,15 +21,15 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "814f4bb8-be13-47cd-9853-eb23f61a1da3",
             "metadata": {},
             "source": [
-                "## Test data set\n",
+                "# Test data set\n",
                 "\n",
                 "For experimenting and easy testing `pandas-indexing` brings along the power sector generation and capacity of the HighRE illustrative modelling pathway from the IPCC AR6 scenario database in IAMC format."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
@@ -358,34 +349,94 @@
                 "from pandas_indexing.datasets import remindhighre_power\n",
                 "\n",
                 "df = remindhighre_power()\n",
                 "df.head()"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "0d61c065",
+            "metadata": {},
+            "source": [
+                "# Usage styles\n",
+                "\n",
+                "`pandas-indexing` defines two different usage styles:\n",
+                "There are:\n",
+                "1. functions that can be imported from the toplevel module, like\n",
+                "   ```python\n",
+                "   from pandas_indexing import assignlevel\n",
+                "   assignlevel(df, unit=\"Mt CO2e/yr\")\n",
+                "   ```\n",
+                "2. convenience accessors that are hooking into pandas as extensions\n",
+                "   ```python\n",
+                "   import pandas_indexing.accessors\n",
+                "   df.idx.assign(unit=\"Mt CO2e/yr)\n",
+                "   ```\n",
+                "\n",
+                "Most of the functionality is available with both styles under slightly different names. I'll present the functional style here first (and add the alternative as comments)"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": 3,
             "id": "e7586672",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "model: REMIND-MAgPIE 2.1-4.3\n",
-                        "scenario: DeepElec_SSP2_HighRE_Budg900\n",
-                        "region: World\n",
-                        "variable: Capacity|Electricity|Biomass, Capacity|Electricity|Coal, Capacity|Electricity|Gas, Capacity|Electricity|Geothermal, Capacity|Electricity|Hydro, Capacity|Electricity|Nuclear, Capacity|Electricity|Oil, Capacity|Electricity|Other, Capacity|Electricity|Solar, Capacity|Electricity|Wind, Secondary Energy|Electricity|Biomass, Secondary Energy|Electricity|Coal, Secondary Energy|Electricity|Gas, Secondary Energy|Electricity|Geothermal, Secondary Energy|Electricity|Hydro, Secondary Energy|Electricity|Nuclear, Secondary Energy|Electricity|Oil, Secondary Energy|Electricity|Other, Secondary Energy|Electricity|Solar, Secondary Energy|Electricity|Wind\n",
-                        "unit: GW, GWh/yr\n"
+                        "Index:\n",
+                        " * model    : REMIND-MAgPIE 2.1-4.3 (1)\n",
+                        " * scenario : DeepElec_SSP2_HighRE_Budg900 (1)\n",
+                        " * region   : World (1)\n",
+                        " * variable : Capacity|Electricity|Biomass, ... (20)\n",
+                        " * unit     : GW, GWh/yr (2)\n",
+                        "\n",
+                        "Columns:\n",
+                        " * <unnamed> : 2005, 2010, 2015, 2020, 2025, 2030, 2035, 2040, ... 2100 (16)\n"
                     ]
                 }
             ],
             "source": [
-                "for name in df.index.names:\n",
-                "    print(f\"{name}: {', '.join(df.index.unique(name))}\")"
+                "from pandas_indexing.core import describelevel\n",
+                "\n",
+                "describelevel(df)  # or: df.idx"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "a4f23678",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "Index:\n",
+                            " * model    : REMIND-MAgPIE 2.1-4.3 (1)\n",
+                            " * scenario : DeepElec_SSP2_HighRE_Budg900 (1)\n",
+                            " * region   : World (1)\n",
+                            " * variable : Capacity|Electricity|Biomass, ... (20)\n",
+                            " * unit     : GW, GWh/yr (2)\n",
+                            "\n",
+                            "Columns:\n",
+                            " * <unnamed> : 2005, 2010, 2015, 2020, 2025, 2030, 2035, 2040, ... 2100 (16)"
+                        ]
+                    },
+                    "execution_count": 4,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "import pandas_indexing.accessors\n",
+                "\n",
+                "df.idx"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "5b948e75",
             "metadata": {},
@@ -397,34 +448,34 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "61d70ee2",
             "metadata": {},
             "source": [
-                "## Selecting data\n",
+                "# Selecting data\n",
                 "\n",
                 "For using pandas indexes effectively for computations, it makes sense to split the hierarchically variable index out into separate python variables: `generation` and `capacity`. The standard pandas tools for this job are `pd.DataFrame.loc` in conjunction with `pd.IndexSlice` or `pd.DataFrame.query`. \n",
                 "\n",
                 "`pandas_indexing` brings `ismatch` and `isin` to make this job as easy as possible."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 5,
             "id": "36d58553",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from pandas_indexing import ismatch, isin"
+                "from pandas_indexing import ismatch, isin  # no .idx equivalents"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "id": "982b9663",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "model                  scenario                      region  variable                         unit\n",
@@ -437,15 +488,15 @@
                             "                                                             Capacity|Electricity|Oil         GW         90.2329\n",
                             "                                                             Capacity|Electricity|Other       GW        469.5231\n",
                             "                                                             Capacity|Electricity|Solar       GW      11094.4847\n",
                             "                                                             Capacity|Electricity|Wind        GW       3522.8061\n",
                             "Name: 2030, dtype: float64"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.loc[ismatch(variable=\"Capacity|**\"), 2030]"
             ]
@@ -457,15 +508,15 @@
             "metadata": {},
             "source": [
                 "`ismatch` allows using a glob-like pattern to subset into one or multiple named levels, together with the standard `rename` method we can get cleaned up capacity and generation data easily:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 7,
             "id": "711f2683",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -945,15 +996,15 @@
                             "                                                          Nuclear    GW        0.0190  \n",
                             "                                                          Oil        GW        0.0126  \n",
                             "                                                          Other      GW     9334.4241  \n",
                             "                                                          Solar      GW    77430.1702  \n",
                             "                                                          Wind       GW    17368.8215  "
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "generation = df.loc[ismatch(variable=\"Secondary Energy|**\")].rename(\n",
                 "    index=lambda s: s.removeprefix(\"Secondary Energy|Electricity|\")\n",
@@ -963,23 +1014,1029 @@
                 ")\n",
                 "capacity"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
+            "id": "3087eb3c",
+            "metadata": {},
+            "source": [
+                "Since this extraction of data is relatively common, `extractlevel` simplifies this by matching against a format-like template string:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "16032dd2",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th>2005</th>\n",
+                            "      <th>2010</th>\n",
+                            "      <th>2015</th>\n",
+                            "      <th>2020</th>\n",
+                            "      <th>2025</th>\n",
+                            "      <th>2030</th>\n",
+                            "      <th>2035</th>\n",
+                            "      <th>2040</th>\n",
+                            "      <th>2045</th>\n",
+                            "      <th>2050</th>\n",
+                            "      <th>2055</th>\n",
+                            "      <th>2060</th>\n",
+                            "      <th>2070</th>\n",
+                            "      <th>2080</th>\n",
+                            "      <th>2090</th>\n",
+                            "      <th>2100</th>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>model</th>\n",
+                            "      <th>scenario</th>\n",
+                            "      <th>region</th>\n",
+                            "      <th>unit</th>\n",
+                            "      <th>carrier</th>\n",
+                            "      <th>fuel</th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th rowspan=\"10\" valign=\"top\">REMIND-MAgPIE 2.1-4.3</th>\n",
+                            "      <th rowspan=\"10\" valign=\"top\">DeepElec_SSP2_HighRE_Budg900</th>\n",
+                            "      <th rowspan=\"10\" valign=\"top\">World</th>\n",
+                            "      <th rowspan=\"10\" valign=\"top\">GWh/yr</th>\n",
+                            "      <th rowspan=\"10\" valign=\"top\">Electricity</th>\n",
+                            "      <th>Biomass</th>\n",
+                            "      <td>2.352778e+05</td>\n",
+                            "      <td>3.407222e+05</td>\n",
+                            "      <td>4.669444e+05</td>\n",
+                            "      <td>5.942778e+05</td>\n",
+                            "      <td>7.219167e+05</td>\n",
+                            "      <td>8.496389e+05</td>\n",
+                            "      <td>9.855833e+05</td>\n",
+                            "      <td>1.173833e+06</td>\n",
+                            "      <td>1.359639e+06</td>\n",
+                            "      <td>1.471139e+06</td>\n",
+                            "      <td>1.513056e+06</td>\n",
+                            "      <td>1.544750e+06</td>\n",
+                            "      <td>1.564583e+06</td>\n",
+                            "      <td>1.557556e+06</td>\n",
+                            "      <td>1.543056e+06</td>\n",
+                            "      <td>1.574306e+06</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Coal</th>\n",
+                            "      <td>7.419778e+06</td>\n",
+                            "      <td>8.252667e+06</td>\n",
+                            "      <td>9.246333e+06</td>\n",
+                            "      <td>1.075747e+07</td>\n",
+                            "      <td>6.045972e+06</td>\n",
+                            "      <td>8.733611e+05</td>\n",
+                            "      <td>6.444444e+03</td>\n",
+                            "      <td>5.027778e+03</td>\n",
+                            "      <td>3.694444e+03</td>\n",
+                            "      <td>2.416667e+03</td>\n",
+                            "      <td>1.555556e+03</td>\n",
+                            "      <td>9.444444e+02</td>\n",
+                            "      <td>4.444444e+02</td>\n",
+                            "      <td>5.277778e+02</td>\n",
+                            "      <td>5.555556e+02</td>\n",
+                            "      <td>5.000000e+02</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Gas</th>\n",
+                            "      <td>3.816028e+06</td>\n",
+                            "      <td>5.050500e+06</td>\n",
+                            "      <td>5.968778e+06</td>\n",
+                            "      <td>7.060083e+06</td>\n",
+                            "      <td>6.469250e+06</td>\n",
+                            "      <td>4.551528e+06</td>\n",
+                            "      <td>2.907250e+06</td>\n",
+                            "      <td>2.602278e+06</td>\n",
+                            "      <td>1.752056e+06</td>\n",
+                            "      <td>1.218361e+06</td>\n",
+                            "      <td>6.538889e+05</td>\n",
+                            "      <td>5.281944e+05</td>\n",
+                            "      <td>2.423333e+05</td>\n",
+                            "      <td>1.685833e+05</td>\n",
+                            "      <td>4.166667e+04</td>\n",
+                            "      <td>3.888889e+02</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Geothermal</th>\n",
+                            "      <td>6.041667e+04</td>\n",
+                            "      <td>9.677778e+04</td>\n",
+                            "      <td>1.799167e+05</td>\n",
+                            "      <td>3.474167e+05</td>\n",
+                            "      <td>5.260278e+05</td>\n",
+                            "      <td>6.213611e+05</td>\n",
+                            "      <td>6.291111e+05</td>\n",
+                            "      <td>6.177778e+05</td>\n",
+                            "      <td>5.893056e+05</td>\n",
+                            "      <td>5.187222e+05</td>\n",
+                            "      <td>4.333611e+05</td>\n",
+                            "      <td>3.603889e+05</td>\n",
+                            "      <td>2.924722e+05</td>\n",
+                            "      <td>2.492778e+05</td>\n",
+                            "      <td>2.059167e+05</td>\n",
+                            "      <td>1.937500e+05</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Hydro</th>\n",
+                            "      <td>2.976944e+06</td>\n",
+                            "      <td>3.557028e+06</td>\n",
+                            "      <td>4.386694e+06</td>\n",
+                            "      <td>5.302056e+06</td>\n",
+                            "      <td>5.813167e+06</td>\n",
+                            "      <td>6.173778e+06</td>\n",
+                            "      <td>6.423194e+06</td>\n",
+                            "      <td>6.604167e+06</td>\n",
+                            "      <td>6.717417e+06</td>\n",
+                            "      <td>6.770250e+06</td>\n",
+                            "      <td>6.782028e+06</td>\n",
+                            "      <td>6.775917e+06</td>\n",
+                            "      <td>6.722667e+06</td>\n",
+                            "      <td>6.655833e+06</td>\n",
+                            "      <td>6.631806e+06</td>\n",
+                            "      <td>6.533167e+06</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Nuclear</th>\n",
+                            "      <td>2.861861e+06</td>\n",
+                            "      <td>2.642750e+06</td>\n",
+                            "      <td>2.448556e+06</td>\n",
+                            "      <td>2.214167e+06</td>\n",
+                            "      <td>2.055667e+06</td>\n",
+                            "      <td>1.876222e+06</td>\n",
+                            "      <td>1.617278e+06</td>\n",
+                            "      <td>1.502778e+06</td>\n",
+                            "      <td>1.304083e+06</td>\n",
+                            "      <td>1.098694e+06</td>\n",
+                            "      <td>8.686111e+05</td>\n",
+                            "      <td>6.451944e+05</td>\n",
+                            "      <td>2.717500e+05</td>\n",
+                            "      <td>5.925000e+04</td>\n",
+                            "      <td>3.916667e+03</td>\n",
+                            "      <td>1.388889e+02</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Oil</th>\n",
+                            "      <td>1.088861e+06</td>\n",
+                            "      <td>1.016972e+06</td>\n",
+                            "      <td>8.353889e+05</td>\n",
+                            "      <td>6.174167e+05</td>\n",
+                            "      <td>4.317778e+05</td>\n",
+                            "      <td>1.960556e+05</td>\n",
+                            "      <td>6.919444e+04</td>\n",
+                            "      <td>4.797222e+04</td>\n",
+                            "      <td>3.175000e+04</td>\n",
+                            "      <td>1.169444e+04</td>\n",
+                            "      <td>6.722222e+03</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Other</th>\n",
+                            "      <td>0.000000e+00</td>\n",
+                            "      <td>0.000000e+00</td>\n",
+                            "      <td>4.444444e+02</td>\n",
+                            "      <td>2.166667e+03</td>\n",
+                            "      <td>8.913889e+04</td>\n",
+                            "      <td>4.938889e+05</td>\n",
+                            "      <td>1.204583e+06</td>\n",
+                            "      <td>1.985111e+06</td>\n",
+                            "      <td>2.790639e+06</td>\n",
+                            "      <td>3.488083e+06</td>\n",
+                            "      <td>4.020806e+06</td>\n",
+                            "      <td>4.434639e+06</td>\n",
+                            "      <td>5.261472e+06</td>\n",
+                            "      <td>6.099583e+06</td>\n",
+                            "      <td>6.740833e+06</td>\n",
+                            "      <td>7.547194e+06</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Solar</th>\n",
+                            "      <td>4.083333e+03</td>\n",
+                            "      <td>8.325000e+04</td>\n",
+                            "      <td>2.616111e+05</td>\n",
+                            "      <td>9.263611e+05</td>\n",
+                            "      <td>5.500722e+06</td>\n",
+                            "      <td>1.566242e+07</td>\n",
+                            "      <td>2.575731e+07</td>\n",
+                            "      <td>3.404253e+07</td>\n",
+                            "      <td>4.088394e+07</td>\n",
+                            "      <td>4.723214e+07</td>\n",
+                            "      <td>5.327061e+07</td>\n",
+                            "      <td>5.819236e+07</td>\n",
+                            "      <td>6.826367e+07</td>\n",
+                            "      <td>7.754106e+07</td>\n",
+                            "      <td>8.359456e+07</td>\n",
+                            "      <td>9.270394e+07</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Wind</th>\n",
+                            "      <td>1.091389e+05</td>\n",
+                            "      <td>5.946944e+05</td>\n",
+                            "      <td>8.323889e+05</td>\n",
+                            "      <td>1.482806e+06</td>\n",
+                            "      <td>3.695778e+06</td>\n",
+                            "      <td>8.141417e+06</td>\n",
+                            "      <td>1.318953e+07</td>\n",
+                            "      <td>1.727517e+07</td>\n",
+                            "      <td>2.112919e+07</td>\n",
+                            "      <td>2.367689e+07</td>\n",
+                            "      <td>2.569986e+07</td>\n",
+                            "      <td>2.771675e+07</td>\n",
+                            "      <td>3.280081e+07</td>\n",
+                            "      <td>3.570786e+07</td>\n",
+                            "      <td>3.840797e+07</td>\n",
+                            "      <td>4.123369e+07</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "                                                                                                 2005  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     2.352778e+05   \n",
+                            "                                                                             Coal        7.419778e+06   \n",
+                            "                                                                             Gas         3.816028e+06   \n",
+                            "                                                                             Geothermal  6.041667e+04   \n",
+                            "                                                                             Hydro       2.976944e+06   \n",
+                            "                                                                             Nuclear     2.861861e+06   \n",
+                            "                                                                             Oil         1.088861e+06   \n",
+                            "                                                                             Other       0.000000e+00   \n",
+                            "                                                                             Solar       4.083333e+03   \n",
+                            "                                                                             Wind        1.091389e+05   \n",
+                            "\n",
+                            "                                                                                                 2010  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     3.407222e+05   \n",
+                            "                                                                             Coal        8.252667e+06   \n",
+                            "                                                                             Gas         5.050500e+06   \n",
+                            "                                                                             Geothermal  9.677778e+04   \n",
+                            "                                                                             Hydro       3.557028e+06   \n",
+                            "                                                                             Nuclear     2.642750e+06   \n",
+                            "                                                                             Oil         1.016972e+06   \n",
+                            "                                                                             Other       0.000000e+00   \n",
+                            "                                                                             Solar       8.325000e+04   \n",
+                            "                                                                             Wind        5.946944e+05   \n",
+                            "\n",
+                            "                                                                                                 2015  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     4.669444e+05   \n",
+                            "                                                                             Coal        9.246333e+06   \n",
+                            "                                                                             Gas         5.968778e+06   \n",
+                            "                                                                             Geothermal  1.799167e+05   \n",
+                            "                                                                             Hydro       4.386694e+06   \n",
+                            "                                                                             Nuclear     2.448556e+06   \n",
+                            "                                                                             Oil         8.353889e+05   \n",
+                            "                                                                             Other       4.444444e+02   \n",
+                            "                                                                             Solar       2.616111e+05   \n",
+                            "                                                                             Wind        8.323889e+05   \n",
+                            "\n",
+                            "                                                                                                 2020  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     5.942778e+05   \n",
+                            "                                                                             Coal        1.075747e+07   \n",
+                            "                                                                             Gas         7.060083e+06   \n",
+                            "                                                                             Geothermal  3.474167e+05   \n",
+                            "                                                                             Hydro       5.302056e+06   \n",
+                            "                                                                             Nuclear     2.214167e+06   \n",
+                            "                                                                             Oil         6.174167e+05   \n",
+                            "                                                                             Other       2.166667e+03   \n",
+                            "                                                                             Solar       9.263611e+05   \n",
+                            "                                                                             Wind        1.482806e+06   \n",
+                            "\n",
+                            "                                                                                                 2025  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     7.219167e+05   \n",
+                            "                                                                             Coal        6.045972e+06   \n",
+                            "                                                                             Gas         6.469250e+06   \n",
+                            "                                                                             Geothermal  5.260278e+05   \n",
+                            "                                                                             Hydro       5.813167e+06   \n",
+                            "                                                                             Nuclear     2.055667e+06   \n",
+                            "                                                                             Oil         4.317778e+05   \n",
+                            "                                                                             Other       8.913889e+04   \n",
+                            "                                                                             Solar       5.500722e+06   \n",
+                            "                                                                             Wind        3.695778e+06   \n",
+                            "\n",
+                            "                                                                                                 2030  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     8.496389e+05   \n",
+                            "                                                                             Coal        8.733611e+05   \n",
+                            "                                                                             Gas         4.551528e+06   \n",
+                            "                                                                             Geothermal  6.213611e+05   \n",
+                            "                                                                             Hydro       6.173778e+06   \n",
+                            "                                                                             Nuclear     1.876222e+06   \n",
+                            "                                                                             Oil         1.960556e+05   \n",
+                            "                                                                             Other       4.938889e+05   \n",
+                            "                                                                             Solar       1.566242e+07   \n",
+                            "                                                                             Wind        8.141417e+06   \n",
+                            "\n",
+                            "                                                                                                 2035  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     9.855833e+05   \n",
+                            "                                                                             Coal        6.444444e+03   \n",
+                            "                                                                             Gas         2.907250e+06   \n",
+                            "                                                                             Geothermal  6.291111e+05   \n",
+                            "                                                                             Hydro       6.423194e+06   \n",
+                            "                                                                             Nuclear     1.617278e+06   \n",
+                            "                                                                             Oil         6.919444e+04   \n",
+                            "                                                                             Other       1.204583e+06   \n",
+                            "                                                                             Solar       2.575731e+07   \n",
+                            "                                                                             Wind        1.318953e+07   \n",
+                            "\n",
+                            "                                                                                                 2040  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     1.173833e+06   \n",
+                            "                                                                             Coal        5.027778e+03   \n",
+                            "                                                                             Gas         2.602278e+06   \n",
+                            "                                                                             Geothermal  6.177778e+05   \n",
+                            "                                                                             Hydro       6.604167e+06   \n",
+                            "                                                                             Nuclear     1.502778e+06   \n",
+                            "                                                                             Oil         4.797222e+04   \n",
+                            "                                                                             Other       1.985111e+06   \n",
+                            "                                                                             Solar       3.404253e+07   \n",
+                            "                                                                             Wind        1.727517e+07   \n",
+                            "\n",
+                            "                                                                                                 2045  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     1.359639e+06   \n",
+                            "                                                                             Coal        3.694444e+03   \n",
+                            "                                                                             Gas         1.752056e+06   \n",
+                            "                                                                             Geothermal  5.893056e+05   \n",
+                            "                                                                             Hydro       6.717417e+06   \n",
+                            "                                                                             Nuclear     1.304083e+06   \n",
+                            "                                                                             Oil         3.175000e+04   \n",
+                            "                                                                             Other       2.790639e+06   \n",
+                            "                                                                             Solar       4.088394e+07   \n",
+                            "                                                                             Wind        2.112919e+07   \n",
+                            "\n",
+                            "                                                                                                 2050  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     1.471139e+06   \n",
+                            "                                                                             Coal        2.416667e+03   \n",
+                            "                                                                             Gas         1.218361e+06   \n",
+                            "                                                                             Geothermal  5.187222e+05   \n",
+                            "                                                                             Hydro       6.770250e+06   \n",
+                            "                                                                             Nuclear     1.098694e+06   \n",
+                            "                                                                             Oil         1.169444e+04   \n",
+                            "                                                                             Other       3.488083e+06   \n",
+                            "                                                                             Solar       4.723214e+07   \n",
+                            "                                                                             Wind        2.367689e+07   \n",
+                            "\n",
+                            "                                                                                                 2055  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     1.513056e+06   \n",
+                            "                                                                             Coal        1.555556e+03   \n",
+                            "                                                                             Gas         6.538889e+05   \n",
+                            "                                                                             Geothermal  4.333611e+05   \n",
+                            "                                                                             Hydro       6.782028e+06   \n",
+                            "                                                                             Nuclear     8.686111e+05   \n",
+                            "                                                                             Oil         6.722222e+03   \n",
+                            "                                                                             Other       4.020806e+06   \n",
+                            "                                                                             Solar       5.327061e+07   \n",
+                            "                                                                             Wind        2.569986e+07   \n",
+                            "\n",
+                            "                                                                                                 2060  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     1.544750e+06   \n",
+                            "                                                                             Coal        9.444444e+02   \n",
+                            "                                                                             Gas         5.281944e+05   \n",
+                            "                                                                             Geothermal  3.603889e+05   \n",
+                            "                                                                             Hydro       6.775917e+06   \n",
+                            "                                                                             Nuclear     6.451944e+05   \n",
+                            "                                                                             Oil         2.777778e+01   \n",
+                            "                                                                             Other       4.434639e+06   \n",
+                            "                                                                             Solar       5.819236e+07   \n",
+                            "                                                                             Wind        2.771675e+07   \n",
+                            "\n",
+                            "                                                                                                 2070  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     1.564583e+06   \n",
+                            "                                                                             Coal        4.444444e+02   \n",
+                            "                                                                             Gas         2.423333e+05   \n",
+                            "                                                                             Geothermal  2.924722e+05   \n",
+                            "                                                                             Hydro       6.722667e+06   \n",
+                            "                                                                             Nuclear     2.717500e+05   \n",
+                            "                                                                             Oil         2.777778e+01   \n",
+                            "                                                                             Other       5.261472e+06   \n",
+                            "                                                                             Solar       6.826367e+07   \n",
+                            "                                                                             Wind        3.280081e+07   \n",
+                            "\n",
+                            "                                                                                                 2080  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     1.557556e+06   \n",
+                            "                                                                             Coal        5.277778e+02   \n",
+                            "                                                                             Gas         1.685833e+05   \n",
+                            "                                                                             Geothermal  2.492778e+05   \n",
+                            "                                                                             Hydro       6.655833e+06   \n",
+                            "                                                                             Nuclear     5.925000e+04   \n",
+                            "                                                                             Oil         2.777778e+01   \n",
+                            "                                                                             Other       6.099583e+06   \n",
+                            "                                                                             Solar       7.754106e+07   \n",
+                            "                                                                             Wind        3.570786e+07   \n",
+                            "\n",
+                            "                                                                                                 2090  \\\n",
+                            "model                 scenario                     region unit   carrier     fuel                       \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     1.543056e+06   \n",
+                            "                                                                             Coal        5.555556e+02   \n",
+                            "                                                                             Gas         4.166667e+04   \n",
+                            "                                                                             Geothermal  2.059167e+05   \n",
+                            "                                                                             Hydro       6.631806e+06   \n",
+                            "                                                                             Nuclear     3.916667e+03   \n",
+                            "                                                                             Oil         2.777778e+01   \n",
+                            "                                                                             Other       6.740833e+06   \n",
+                            "                                                                             Solar       8.359456e+07   \n",
+                            "                                                                             Wind        3.840797e+07   \n",
+                            "\n",
+                            "                                                                                                 2100  \n",
+                            "model                 scenario                     region unit   carrier     fuel                      \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Electricity Biomass     1.574306e+06  \n",
+                            "                                                                             Coal        5.000000e+02  \n",
+                            "                                                                             Gas         3.888889e+02  \n",
+                            "                                                                             Geothermal  1.937500e+05  \n",
+                            "                                                                             Hydro       6.533167e+06  \n",
+                            "                                                                             Nuclear     1.388889e+02  \n",
+                            "                                                                             Oil         2.777778e+01  \n",
+                            "                                                                             Other       7.547194e+06  \n",
+                            "                                                                             Solar       9.270394e+07  \n",
+                            "                                                                             Wind        4.123369e+07  "
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "from pandas_indexing import extractlevel, formatlevel\n",
+                "\n",
+                "splitdf = extractlevel(df, variable=\"Secondary Energy|{carrier}|{fuel}\", drop=True)\n",
+                "# or: df.idx.extract(variable=\"Secondary Energy|{carrier}|{fuel}\")\n",
+                "splitdf"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "405720c7",
+            "metadata": {},
+            "source": [
+                "The inverse operation is to combine strings back together with `formatlevel`:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "8e355684",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th>2005</th>\n",
+                            "      <th>2010</th>\n",
+                            "      <th>2015</th>\n",
+                            "      <th>2020</th>\n",
+                            "      <th>2025</th>\n",
+                            "      <th>2030</th>\n",
+                            "      <th>2035</th>\n",
+                            "      <th>2040</th>\n",
+                            "      <th>2045</th>\n",
+                            "      <th>2050</th>\n",
+                            "      <th>2055</th>\n",
+                            "      <th>2060</th>\n",
+                            "      <th>2070</th>\n",
+                            "      <th>2080</th>\n",
+                            "      <th>2090</th>\n",
+                            "      <th>2100</th>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>model</th>\n",
+                            "      <th>scenario</th>\n",
+                            "      <th>region</th>\n",
+                            "      <th>unit</th>\n",
+                            "      <th>variable</th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th rowspan=\"10\" valign=\"top\">REMIND-MAgPIE 2.1-4.3</th>\n",
+                            "      <th rowspan=\"10\" valign=\"top\">DeepElec_SSP2_HighRE_Budg900</th>\n",
+                            "      <th rowspan=\"10\" valign=\"top\">World</th>\n",
+                            "      <th rowspan=\"10\" valign=\"top\">GWh/yr</th>\n",
+                            "      <th>Secondary Energy|Electricity|Biomass</th>\n",
+                            "      <td>2.352778e+05</td>\n",
+                            "      <td>3.407222e+05</td>\n",
+                            "      <td>4.669444e+05</td>\n",
+                            "      <td>5.942778e+05</td>\n",
+                            "      <td>7.219167e+05</td>\n",
+                            "      <td>8.496389e+05</td>\n",
+                            "      <td>9.855833e+05</td>\n",
+                            "      <td>1.173833e+06</td>\n",
+                            "      <td>1.359639e+06</td>\n",
+                            "      <td>1.471139e+06</td>\n",
+                            "      <td>1.513056e+06</td>\n",
+                            "      <td>1.544750e+06</td>\n",
+                            "      <td>1.564583e+06</td>\n",
+                            "      <td>1.557556e+06</td>\n",
+                            "      <td>1.543056e+06</td>\n",
+                            "      <td>1.574306e+06</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Secondary Energy|Electricity|Coal</th>\n",
+                            "      <td>7.419778e+06</td>\n",
+                            "      <td>8.252667e+06</td>\n",
+                            "      <td>9.246333e+06</td>\n",
+                            "      <td>1.075747e+07</td>\n",
+                            "      <td>6.045972e+06</td>\n",
+                            "      <td>8.733611e+05</td>\n",
+                            "      <td>6.444444e+03</td>\n",
+                            "      <td>5.027778e+03</td>\n",
+                            "      <td>3.694444e+03</td>\n",
+                            "      <td>2.416667e+03</td>\n",
+                            "      <td>1.555556e+03</td>\n",
+                            "      <td>9.444444e+02</td>\n",
+                            "      <td>4.444444e+02</td>\n",
+                            "      <td>5.277778e+02</td>\n",
+                            "      <td>5.555556e+02</td>\n",
+                            "      <td>5.000000e+02</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Secondary Energy|Electricity|Gas</th>\n",
+                            "      <td>3.816028e+06</td>\n",
+                            "      <td>5.050500e+06</td>\n",
+                            "      <td>5.968778e+06</td>\n",
+                            "      <td>7.060083e+06</td>\n",
+                            "      <td>6.469250e+06</td>\n",
+                            "      <td>4.551528e+06</td>\n",
+                            "      <td>2.907250e+06</td>\n",
+                            "      <td>2.602278e+06</td>\n",
+                            "      <td>1.752056e+06</td>\n",
+                            "      <td>1.218361e+06</td>\n",
+                            "      <td>6.538889e+05</td>\n",
+                            "      <td>5.281944e+05</td>\n",
+                            "      <td>2.423333e+05</td>\n",
+                            "      <td>1.685833e+05</td>\n",
+                            "      <td>4.166667e+04</td>\n",
+                            "      <td>3.888889e+02</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Secondary Energy|Electricity|Geothermal</th>\n",
+                            "      <td>6.041667e+04</td>\n",
+                            "      <td>9.677778e+04</td>\n",
+                            "      <td>1.799167e+05</td>\n",
+                            "      <td>3.474167e+05</td>\n",
+                            "      <td>5.260278e+05</td>\n",
+                            "      <td>6.213611e+05</td>\n",
+                            "      <td>6.291111e+05</td>\n",
+                            "      <td>6.177778e+05</td>\n",
+                            "      <td>5.893056e+05</td>\n",
+                            "      <td>5.187222e+05</td>\n",
+                            "      <td>4.333611e+05</td>\n",
+                            "      <td>3.603889e+05</td>\n",
+                            "      <td>2.924722e+05</td>\n",
+                            "      <td>2.492778e+05</td>\n",
+                            "      <td>2.059167e+05</td>\n",
+                            "      <td>1.937500e+05</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Secondary Energy|Electricity|Hydro</th>\n",
+                            "      <td>2.976944e+06</td>\n",
+                            "      <td>3.557028e+06</td>\n",
+                            "      <td>4.386694e+06</td>\n",
+                            "      <td>5.302056e+06</td>\n",
+                            "      <td>5.813167e+06</td>\n",
+                            "      <td>6.173778e+06</td>\n",
+                            "      <td>6.423194e+06</td>\n",
+                            "      <td>6.604167e+06</td>\n",
+                            "      <td>6.717417e+06</td>\n",
+                            "      <td>6.770250e+06</td>\n",
+                            "      <td>6.782028e+06</td>\n",
+                            "      <td>6.775917e+06</td>\n",
+                            "      <td>6.722667e+06</td>\n",
+                            "      <td>6.655833e+06</td>\n",
+                            "      <td>6.631806e+06</td>\n",
+                            "      <td>6.533167e+06</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Secondary Energy|Electricity|Nuclear</th>\n",
+                            "      <td>2.861861e+06</td>\n",
+                            "      <td>2.642750e+06</td>\n",
+                            "      <td>2.448556e+06</td>\n",
+                            "      <td>2.214167e+06</td>\n",
+                            "      <td>2.055667e+06</td>\n",
+                            "      <td>1.876222e+06</td>\n",
+                            "      <td>1.617278e+06</td>\n",
+                            "      <td>1.502778e+06</td>\n",
+                            "      <td>1.304083e+06</td>\n",
+                            "      <td>1.098694e+06</td>\n",
+                            "      <td>8.686111e+05</td>\n",
+                            "      <td>6.451944e+05</td>\n",
+                            "      <td>2.717500e+05</td>\n",
+                            "      <td>5.925000e+04</td>\n",
+                            "      <td>3.916667e+03</td>\n",
+                            "      <td>1.388889e+02</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Secondary Energy|Electricity|Oil</th>\n",
+                            "      <td>1.088861e+06</td>\n",
+                            "      <td>1.016972e+06</td>\n",
+                            "      <td>8.353889e+05</td>\n",
+                            "      <td>6.174167e+05</td>\n",
+                            "      <td>4.317778e+05</td>\n",
+                            "      <td>1.960556e+05</td>\n",
+                            "      <td>6.919444e+04</td>\n",
+                            "      <td>4.797222e+04</td>\n",
+                            "      <td>3.175000e+04</td>\n",
+                            "      <td>1.169444e+04</td>\n",
+                            "      <td>6.722222e+03</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Secondary Energy|Electricity|Other</th>\n",
+                            "      <td>0.000000e+00</td>\n",
+                            "      <td>0.000000e+00</td>\n",
+                            "      <td>4.444444e+02</td>\n",
+                            "      <td>2.166667e+03</td>\n",
+                            "      <td>8.913889e+04</td>\n",
+                            "      <td>4.938889e+05</td>\n",
+                            "      <td>1.204583e+06</td>\n",
+                            "      <td>1.985111e+06</td>\n",
+                            "      <td>2.790639e+06</td>\n",
+                            "      <td>3.488083e+06</td>\n",
+                            "      <td>4.020806e+06</td>\n",
+                            "      <td>4.434639e+06</td>\n",
+                            "      <td>5.261472e+06</td>\n",
+                            "      <td>6.099583e+06</td>\n",
+                            "      <td>6.740833e+06</td>\n",
+                            "      <td>7.547194e+06</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Secondary Energy|Electricity|Solar</th>\n",
+                            "      <td>4.083333e+03</td>\n",
+                            "      <td>8.325000e+04</td>\n",
+                            "      <td>2.616111e+05</td>\n",
+                            "      <td>9.263611e+05</td>\n",
+                            "      <td>5.500722e+06</td>\n",
+                            "      <td>1.566242e+07</td>\n",
+                            "      <td>2.575731e+07</td>\n",
+                            "      <td>3.404253e+07</td>\n",
+                            "      <td>4.088394e+07</td>\n",
+                            "      <td>4.723214e+07</td>\n",
+                            "      <td>5.327061e+07</td>\n",
+                            "      <td>5.819236e+07</td>\n",
+                            "      <td>6.826367e+07</td>\n",
+                            "      <td>7.754106e+07</td>\n",
+                            "      <td>8.359456e+07</td>\n",
+                            "      <td>9.270394e+07</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Secondary Energy|Electricity|Wind</th>\n",
+                            "      <td>1.091389e+05</td>\n",
+                            "      <td>5.946944e+05</td>\n",
+                            "      <td>8.323889e+05</td>\n",
+                            "      <td>1.482806e+06</td>\n",
+                            "      <td>3.695778e+06</td>\n",
+                            "      <td>8.141417e+06</td>\n",
+                            "      <td>1.318953e+07</td>\n",
+                            "      <td>1.727517e+07</td>\n",
+                            "      <td>2.112919e+07</td>\n",
+                            "      <td>2.367689e+07</td>\n",
+                            "      <td>2.569986e+07</td>\n",
+                            "      <td>2.771675e+07</td>\n",
+                            "      <td>3.280081e+07</td>\n",
+                            "      <td>3.570786e+07</td>\n",
+                            "      <td>3.840797e+07</td>\n",
+                            "      <td>4.123369e+07</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "                                                                                                                  2005  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     2.352778e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        7.419778e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         3.816028e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  6.041667e+04   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       2.976944e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     2.861861e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         1.088861e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       0.000000e+00   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       4.083333e+03   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        1.091389e+05   \n",
+                            "\n",
+                            "                                                                                                                  2010  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     3.407222e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        8.252667e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         5.050500e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  9.677778e+04   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       3.557028e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     2.642750e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         1.016972e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       0.000000e+00   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       8.325000e+04   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        5.946944e+05   \n",
+                            "\n",
+                            "                                                                                                                  2015  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     4.669444e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        9.246333e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         5.968778e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  1.799167e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       4.386694e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     2.448556e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         8.353889e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       4.444444e+02   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       2.616111e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        8.323889e+05   \n",
+                            "\n",
+                            "                                                                                                                  2020  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     5.942778e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        1.075747e+07   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         7.060083e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  3.474167e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       5.302056e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     2.214167e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         6.174167e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       2.166667e+03   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       9.263611e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        1.482806e+06   \n",
+                            "\n",
+                            "                                                                                                                  2025  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     7.219167e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        6.045972e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         6.469250e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  5.260278e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       5.813167e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     2.055667e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         4.317778e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       8.913889e+04   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       5.500722e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        3.695778e+06   \n",
+                            "\n",
+                            "                                                                                                                  2030  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     8.496389e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        8.733611e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         4.551528e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  6.213611e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       6.173778e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     1.876222e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         1.960556e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       4.938889e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       1.566242e+07   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        8.141417e+06   \n",
+                            "\n",
+                            "                                                                                                                  2035  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     9.855833e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        6.444444e+03   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         2.907250e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  6.291111e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       6.423194e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     1.617278e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         6.919444e+04   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       1.204583e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       2.575731e+07   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        1.318953e+07   \n",
+                            "\n",
+                            "                                                                                                                  2040  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     1.173833e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        5.027778e+03   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         2.602278e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  6.177778e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       6.604167e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     1.502778e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         4.797222e+04   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       1.985111e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       3.404253e+07   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        1.727517e+07   \n",
+                            "\n",
+                            "                                                                                                                  2045  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     1.359639e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        3.694444e+03   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         1.752056e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  5.893056e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       6.717417e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     1.304083e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         3.175000e+04   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       2.790639e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       4.088394e+07   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        2.112919e+07   \n",
+                            "\n",
+                            "                                                                                                                  2050  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     1.471139e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        2.416667e+03   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         1.218361e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  5.187222e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       6.770250e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     1.098694e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         1.169444e+04   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       3.488083e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       4.723214e+07   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        2.367689e+07   \n",
+                            "\n",
+                            "                                                                                                                  2055  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     1.513056e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        1.555556e+03   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         6.538889e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  4.333611e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       6.782028e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     8.686111e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         6.722222e+03   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       4.020806e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       5.327061e+07   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        2.569986e+07   \n",
+                            "\n",
+                            "                                                                                                                  2060  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     1.544750e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        9.444444e+02   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         5.281944e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  3.603889e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       6.775917e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     6.451944e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         2.777778e+01   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       4.434639e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       5.819236e+07   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        2.771675e+07   \n",
+                            "\n",
+                            "                                                                                                                  2070  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     1.564583e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        4.444444e+02   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         2.423333e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  2.924722e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       6.722667e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     2.717500e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         2.777778e+01   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       5.261472e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       6.826367e+07   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        3.280081e+07   \n",
+                            "\n",
+                            "                                                                                                                  2080  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     1.557556e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        5.277778e+02   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         1.685833e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  2.492778e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       6.655833e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     5.925000e+04   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         2.777778e+01   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       6.099583e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       7.754106e+07   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        3.570786e+07   \n",
+                            "\n",
+                            "                                                                                                                  2090  \\\n",
+                            "model                 scenario                     region unit   variable                                                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     1.543056e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        5.555556e+02   \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         4.166667e+04   \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  2.059167e+05   \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       6.631806e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     3.916667e+03   \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         2.777778e+01   \n",
+                            "                                                                 Secondary Energy|Electricity|Other       6.740833e+06   \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       8.359456e+07   \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        3.840797e+07   \n",
+                            "\n",
+                            "                                                                                                                  2100  \n",
+                            "model                 scenario                     region unit   variable                                               \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  GWh/yr Secondary Energy|Electricity|Biomass     1.574306e+06  \n",
+                            "                                                                 Secondary Energy|Electricity|Coal        5.000000e+02  \n",
+                            "                                                                 Secondary Energy|Electricity|Gas         3.888889e+02  \n",
+                            "                                                                 Secondary Energy|Electricity|Geothermal  1.937500e+05  \n",
+                            "                                                                 Secondary Energy|Electricity|Hydro       6.533167e+06  \n",
+                            "                                                                 Secondary Energy|Electricity|Nuclear     1.388889e+02  \n",
+                            "                                                                 Secondary Energy|Electricity|Oil         2.777778e+01  \n",
+                            "                                                                 Secondary Energy|Electricity|Other       7.547194e+06  \n",
+                            "                                                                 Secondary Energy|Electricity|Solar       9.270394e+07  \n",
+                            "                                                                 Secondary Energy|Electricity|Wind        4.123369e+07  "
+                        ]
+                    },
+                    "execution_count": 9,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "formatlevel(splitdf, variable=\"Secondary Energy|{carrier}|{fuel}\", drop=True)\n",
+                "# or: df.idx.format(variable=\"Secondary Energy|{carrier}|{fuel}\")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
             "id": "e78ace7d",
             "metadata": {},
             "source": [
-                "So that we can easily calculate capacity factors (ratios of generation and capacity) directly, if we take care of removing the conflicting `unit` level. Similarly to `ismatch`, `isin` can be provided as an argument to `.loc[]` to select on named index levels with the difference that only exact matches are considered."
+                "With `generation` and `capacity` conveniently split into separate variables, we can calculate capacity factors (ratios of generation and capacity) directly, as long as we take care of removing the conflicting `unit` level. Similarly to `ismatch`, `isin` can be provided as an argument to `.loc[]` to select on named index levels with the difference that only exact matches are considered."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 10,
             "id": "9b4be2b0",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -1094,15 +2151,15 @@
                             "model                 scenario                     region variable              \n",
                             "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Geothermal  0.850021  \n",
                             "                                                          Hydro       0.399716  \n",
                             "                                                          Solar       0.149422  \n",
                             "                                                          Wind        0.298163  "
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "capacity_factor = generation.droplevel(\"unit\") / 8760 / capacity.droplevel(\"unit\")\n",
                 "capacity_factor.loc[isin(variable=[\"Solar\", \"Wind\", \"Hydro\", \"Geothermal\"]), 2030:2051]"
@@ -1110,30 +2167,30 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "b4d501a3",
             "metadata": {},
             "source": [
-                "Under the hood `isin` and `ismatch` generate `Selector` objects that can be called with data to generate boolean masks. They can be composed into complex queries intuitively, which are kept as a hierarchical structure of objects."
+                "Under the hood `isin` and `ismatch` generate `Selector` objects. They can be composed into complex queries intuitively, which are kept as a hierarchical structure of objects."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 11,
             "id": "4197be7d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "And(a=Isin(filters={'variable': ['Coal', 'Gas', 'Nuclear'], 'unit': 'GW'}), b=Not(a=Ismatch(filters={'variable': 'S*'}, regex=False)))"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "query = isin(variable=[\"Coal\", \"Gas\", \"Nuclear\"], unit=\"GW\") & ~ismatch(variable=\"S*\")\n",
                 "query"
@@ -1141,20 +2198,20 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "f137127f",
             "metadata": {},
             "source": [
-                "For evaluating the query one needs to pass in a data object to produce a boolean mask. Since pandas `.loc` indexer does exactly that, these queries work as expected.\n"
+                "For evaluating such a query one needs to pass in a data object to produce a boolean mask. Since pandas `.loc` indexer does exactly that, these queries work as expected.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 12,
             "id": "18401aa0",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "model                  scenario                      region  variable    unit\n",
@@ -1167,15 +2224,15 @@
                             "                                                             Oil         GW      False\n",
                             "                                                             Other       GW      False\n",
                             "                                                             Solar       GW      False\n",
                             "                                                             Wind        GW      False\n",
                             "dtype: bool"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "query(capacity)"
             ]
@@ -1201,15 +2258,15 @@
                 "```\n",
                 "\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 13,
             "id": "8b421dba",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -1329,15 +2386,15 @@
                             "\n",
                             "                                                                              2040  \n",
                             "model                 scenario                     region variable unit             \n",
                             "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Gas      GW    1289.4777  \n",
                             "                                                          Nuclear  GW     214.4376  "
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "high_capacity_fossil = capacity.loc[\n",
                 "    isin(variable=[\"Coal\", \"Gas\", \"Nuclear\"], unit=\"GW\") & (capacity[2030] > 250),\n",
@@ -1353,15 +2410,15 @@
             "metadata": {},
             "source": [
                 "The simple fact that this is an operation on `[]`, means that we can also use it to modify values in-place:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 14,
             "id": "71d7aa7d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -1481,15 +2538,15 @@
                             "\n",
                             "                                                                              2040  \n",
                             "model                 scenario                     region variable unit             \n",
                             "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Gas      GW    1000.0000  \n",
                             "                                                          Nuclear  GW     214.4376  "
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "high_capacity_fossil.loc[isin(variable=\"Gas\"), 2030:] = 1000.0\n",
                 "high_capacity_fossil"
@@ -1502,15 +2559,15 @@
             "metadata": {},
             "source": [
                 "Most methods in `pandas_indexing` do not care whether they are run on an index, a series or a dataframe, but will transiently take care of handing them down to the appropriate level:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 15,
             "id": "e0ff32d5",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "model                  scenario                      region  variable  unit  year\n",
@@ -1525,15 +2582,15 @@
                             "                                                             Nuclear   GW    2030     275.5920\n",
                             "                                                                             2040     214.4376\n",
                             "                                                                             2050     156.7766\n",
                             "                                                                             2060      92.0667\n",
                             "dtype: float64"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fossil_series = (\n",
                 "    capacity.loc[isin(variable=[\"Coal\", \"Gas\", \"Nuclear\"]), [2030, 2040, 2050, 2060]]\n",
@@ -1541,15 +2598,15 @@
                 "    .stack()\n",
                 ")\n",
                 "fossil_series"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 16,
             "id": "6d4686e6",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "model                  scenario                      region  variable  unit  year\n",
@@ -1558,161 +2615,163 @@
                             "                                                             Gas       GW    2030    1584.4033\n",
                             "                                                                             2050     562.8482\n",
                             "                                                             Nuclear   GW    2030     275.5920\n",
                             "                                                                             2050     156.7766\n",
                             "dtype: float64"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fossil_series.loc[isin(year=[2030, 2050])]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 17,
             "id": "8d4e91fb",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([False, False, False, False, False, False, False, False,  True,\n",
                             "        True,  True,  True])"
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "isin(fossil_series.index, variable=\"Nuclear\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "36c41351",
             "metadata": {},
             "source": [
-                "## Selecting based on a multi-index\n",
+                "# Selecting based on a multi-index\n",
                 "\n",
                 "If we need pairs of data like `Coal` in 2030 and `Gas` in 2040 and `Nuclear` in 2040 and 2050, based on a given multiindex, then this defines right-oriented `semijoin` like:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 18,
             "id": "cde4ff9f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "MultiIndex([(   'Coal', 2030),\n",
                             "            (    'Gas', 2035),\n",
                             "            ('Nuclear', 2040),\n",
                             "            ('Nuclear', 2050)],\n",
                             "           names=['variable', 'year'])"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "idx = pd.MultiIndex.from_tuples(\n",
                 "    [(\"Coal\", 2030), (\"Gas\", 2035), (\"Nuclear\", 2040), (\"Nuclear\", 2050)],\n",
                 "    names=[\"variable\", \"year\"],\n",
                 ")\n",
                 "idx"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 19,
             "id": "dc294f2f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "variable  year  model                  scenario                      region  unit\n",
                             "Coal      2030  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  World   GW      182.0149\n",
                             "Gas       2035  NaN                    NaN                           NaN     NaN          NaN\n",
                             "Nuclear   2040  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  World   GW      214.4376\n",
                             "          2050  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  World   GW      156.7766\n",
                             "dtype: float64"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from pandas_indexing import semijoin\n",
                 "\n",
-                "semijoin(fossil_series, idx, how=\"right\")"
+                "semijoin(\n",
+                "    fossil_series, idx, how=\"right\"\n",
+                ")  # or: fossil_series.idx.semijoin(idx, how=\"right\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "cbaa73b0",
             "metadata": {},
             "source": [
                 "Since the `(\"Gas\", 2035)` is not part of the original `fossil_series` it shows up as `NaN`s here, an inner join will skip it silently:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 20,
             "id": "f82d6bf4",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "variable  year  model                  scenario                      region  unit\n",
                             "Coal      2030  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  World   GW      182.0149\n",
                             "Nuclear   2040  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  World   GW      214.4376\n",
                             "          2050  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  World   GW      156.7766\n",
                             "dtype: float64"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "semijoin(fossil_series, idx, how=\"inner\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "f2e1e0e4",
             "metadata": {},
             "source": [
-                "## Projecting levels\n",
+                "# Projecting levels\n",
                 "\n",
                 "Often after selecting the right subsets, ie the interesting `model` or `scenario` it makes sense to consolidate the data to a given set of `levels`. That is what `projectlevel` is used for:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 21,
             "id": "6d0000aa",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "variable  year\n",
@@ -1727,38 +2786,39 @@
                             "Nuclear   2030     275.5920\n",
                             "          2040     214.4376\n",
                             "          2050     156.7766\n",
                             "          2060      92.0667\n",
                             "dtype: float64"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from pandas_indexing import projectlevel\n",
                 "\n",
                 "simple_fossil_series = projectlevel(fossil_series, [\"variable\", \"year\"])\n",
+                "# or: fossil_series.idx.project([\"variable\", \"year\"])\n",
                 "simple_fossil_series"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "715fe070",
             "metadata": {},
             "source": [
                 "`projectlevel` reduces the levels attached to a multiindex to the ones explicitly named. It is basically the complement to `droplevel` which removes the listed names"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 22,
             "id": "308fb920",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "model                  scenario                    \n",
@@ -1773,79 +2833,911 @@
                             "                       DeepElec_SSP2_HighRE_Budg900    True\n",
                             "                       DeepElec_SSP2_HighRE_Budg900    True\n",
                             "                       DeepElec_SSP2_HighRE_Budg900    True\n",
                             "                       DeepElec_SSP2_HighRE_Budg900    True\n",
                             "dtype: bool"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 22,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "projectlevel(fossil_series, [\"model\", \"scenario\"]) == fossil_series.droplevel(\n",
                 "    [\"variable\", \"unit\", \"region\", \"year\"]\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "6eb7b029",
             "metadata": {},
             "source": [
-                "## Assigning to levels\n",
+                "# Assigning to levels\n",
                 "\n",
-                "`assignlevel` allows to modify individual values with helpful keyword arguments:"
+                "`assignlevel` allows to modify individual values with helpful keyword arguments,"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
-            "id": "4f52e21a",
+            "execution_count": 23,
+            "id": "ca2a3c70",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th>2005</th>\n",
+                            "      <th>2010</th>\n",
+                            "      <th>2015</th>\n",
+                            "      <th>2020</th>\n",
+                            "      <th>2025</th>\n",
+                            "      <th>2030</th>\n",
+                            "      <th>2035</th>\n",
+                            "      <th>2040</th>\n",
+                            "      <th>2045</th>\n",
+                            "      <th>2050</th>\n",
+                            "      <th>2055</th>\n",
+                            "      <th>2060</th>\n",
+                            "      <th>2070</th>\n",
+                            "      <th>2080</th>\n",
+                            "      <th>2090</th>\n",
+                            "      <th>2100</th>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>model</th>\n",
+                            "      <th>scenario</th>\n",
+                            "      <th>region</th>\n",
+                            "      <th>variable</th>\n",
+                            "      <th>unit</th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th rowspan=\"20\" valign=\"top\">REMIND-MAgPIE 2.1-4.3</th>\n",
+                            "      <th rowspan=\"20\" valign=\"top\">DeepElec_SSP2_HighRE_Budg900</th>\n",
+                            "      <th rowspan=\"20\" valign=\"top\">World</th>\n",
+                            "      <th>Updated|Capacity|Electricity|Biomass</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>4.298430e+01</td>\n",
+                            "      <td>6.247170e+01</td>\n",
+                            "      <td>8.566980e+01</td>\n",
+                            "      <td>1.088834e+02</td>\n",
+                            "      <td>1.285653e+02</td>\n",
+                            "      <td>1.378452e+02</td>\n",
+                            "      <td>1.328316e+02</td>\n",
+                            "      <td>1.227382e+02</td>\n",
+                            "      <td>1.063772e+02</td>\n",
+                            "      <td>8.602650e+01</td>\n",
+                            "      <td>6.565480e+01</td>\n",
+                            "      <td>4.575910e+01</td>\n",
+                            "      <td>1.450470e+01</td>\n",
+                            "      <td>3.962800e+00</td>\n",
+                            "      <td>8.198000e-01</td>\n",
+                            "      <td>2.150000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Capacity|Electricity|Coal</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>1.238877e+03</td>\n",
+                            "      <td>1.525950e+03</td>\n",
+                            "      <td>1.876595e+03</td>\n",
+                            "      <td>2.075232e+03</td>\n",
+                            "      <td>1.225451e+03</td>\n",
+                            "      <td>1.820149e+02</td>\n",
+                            "      <td>1.353200e+00</td>\n",
+                            "      <td>1.072900e+00</td>\n",
+                            "      <td>7.763000e-01</td>\n",
+                            "      <td>5.029000e-01</td>\n",
+                            "      <td>3.111000e-01</td>\n",
+                            "      <td>1.836000e-01</td>\n",
+                            "      <td>7.830000e-02</td>\n",
+                            "      <td>9.180000e-02</td>\n",
+                            "      <td>9.650000e-02</td>\n",
+                            "      <td>8.660000e-02</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Capacity|Electricity|Gas</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>1.096674e+03</td>\n",
+                            "      <td>1.343108e+03</td>\n",
+                            "      <td>1.603169e+03</td>\n",
+                            "      <td>1.852649e+03</td>\n",
+                            "      <td>1.761806e+03</td>\n",
+                            "      <td>1.584403e+03</td>\n",
+                            "      <td>1.423539e+03</td>\n",
+                            "      <td>1.289478e+03</td>\n",
+                            "      <td>8.638716e+02</td>\n",
+                            "      <td>5.628482e+02</td>\n",
+                            "      <td>3.937209e+02</td>\n",
+                            "      <td>3.499091e+02</td>\n",
+                            "      <td>3.063883e+02</td>\n",
+                            "      <td>2.135970e+02</td>\n",
+                            "      <td>5.260450e+01</td>\n",
+                            "      <td>2.717000e-01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Capacity|Electricity|Geothermal</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>8.112900e+00</td>\n",
+                            "      <td>1.299850e+01</td>\n",
+                            "      <td>2.416120e+01</td>\n",
+                            "      <td>4.665730e+01</td>\n",
+                            "      <td>7.064690e+01</td>\n",
+                            "      <td>8.345060e+01</td>\n",
+                            "      <td>8.448930e+01</td>\n",
+                            "      <td>8.296880e+01</td>\n",
+                            "      <td>7.914520e+01</td>\n",
+                            "      <td>6.966280e+01</td>\n",
+                            "      <td>5.820210e+01</td>\n",
+                            "      <td>4.840070e+01</td>\n",
+                            "      <td>3.927950e+01</td>\n",
+                            "      <td>3.347930e+01</td>\n",
+                            "      <td>2.765300e+01</td>\n",
+                            "      <td>2.601980e+01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Capacity|Electricity|Hydro</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>8.065684e+02</td>\n",
+                            "      <td>9.633523e+02</td>\n",
+                            "      <td>1.239617e+03</td>\n",
+                            "      <td>1.500451e+03</td>\n",
+                            "      <td>1.669357e+03</td>\n",
+                            "      <td>1.786047e+03</td>\n",
+                            "      <td>1.858782e+03</td>\n",
+                            "      <td>1.902635e+03</td>\n",
+                            "      <td>1.925653e+03</td>\n",
+                            "      <td>1.933520e+03</td>\n",
+                            "      <td>1.931110e+03</td>\n",
+                            "      <td>1.922569e+03</td>\n",
+                            "      <td>1.893641e+03</td>\n",
+                            "      <td>1.860861e+03</td>\n",
+                            "      <td>1.846102e+03</td>\n",
+                            "      <td>1.805140e+03</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Capacity|Electricity|Nuclear</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>4.083700e+02</td>\n",
+                            "      <td>4.043094e+02</td>\n",
+                            "      <td>3.791375e+02</td>\n",
+                            "      <td>3.452239e+02</td>\n",
+                            "      <td>3.101729e+02</td>\n",
+                            "      <td>2.755920e+02</td>\n",
+                            "      <td>2.347028e+02</td>\n",
+                            "      <td>2.144376e+02</td>\n",
+                            "      <td>1.860849e+02</td>\n",
+                            "      <td>1.567766e+02</td>\n",
+                            "      <td>1.239472e+02</td>\n",
+                            "      <td>9.206670e+01</td>\n",
+                            "      <td>3.877600e+01</td>\n",
+                            "      <td>8.455000e+00</td>\n",
+                            "      <td>5.580000e-01</td>\n",
+                            "      <td>1.900000e-02</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Capacity|Electricity|Oil</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>5.112499e+02</td>\n",
+                            "      <td>4.630961e+02</td>\n",
+                            "      <td>3.709638e+02</td>\n",
+                            "      <td>2.817401e+02</td>\n",
+                            "      <td>1.932768e+02</td>\n",
+                            "      <td>9.023290e+01</td>\n",
+                            "      <td>3.159640e+01</td>\n",
+                            "      <td>2.190000e+01</td>\n",
+                            "      <td>1.450230e+01</td>\n",
+                            "      <td>5.341200e+00</td>\n",
+                            "      <td>3.064300e+00</td>\n",
+                            "      <td>1.200000e-02</td>\n",
+                            "      <td>1.200000e-02</td>\n",
+                            "      <td>1.200000e-02</td>\n",
+                            "      <td>1.210000e-02</td>\n",
+                            "      <td>1.260000e-02</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Capacity|Electricity|Other</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>0.000000e+00</td>\n",
+                            "      <td>0.000000e+00</td>\n",
+                            "      <td>3.396000e-01</td>\n",
+                            "      <td>1.656200e+00</td>\n",
+                            "      <td>8.110980e+01</td>\n",
+                            "      <td>4.695231e+02</td>\n",
+                            "      <td>1.253078e+03</td>\n",
+                            "      <td>2.254017e+03</td>\n",
+                            "      <td>3.341699e+03</td>\n",
+                            "      <td>4.267072e+03</td>\n",
+                            "      <td>4.925403e+03</td>\n",
+                            "      <td>5.433398e+03</td>\n",
+                            "      <td>6.432168e+03</td>\n",
+                            "      <td>7.478326e+03</td>\n",
+                            "      <td>8.321384e+03</td>\n",
+                            "      <td>9.334424e+03</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Capacity|Electricity|Solar</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>2.682400e+00</td>\n",
+                            "      <td>4.961380e+01</td>\n",
+                            "      <td>2.198533e+02</td>\n",
+                            "      <td>6.509654e+02</td>\n",
+                            "      <td>3.785689e+03</td>\n",
+                            "      <td>1.109448e+04</td>\n",
+                            "      <td>1.906378e+04</td>\n",
+                            "      <td>2.556775e+04</td>\n",
+                            "      <td>3.097003e+04</td>\n",
+                            "      <td>3.608447e+04</td>\n",
+                            "      <td>4.110399e+04</td>\n",
+                            "      <td>4.527457e+04</td>\n",
+                            "      <td>5.443399e+04</td>\n",
+                            "      <td>6.305545e+04</td>\n",
+                            "      <td>6.884808e+04</td>\n",
+                            "      <td>7.743017e+04</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Capacity|Electricity|Wind</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>3.226040e+01</td>\n",
+                            "      <td>1.811785e+02</td>\n",
+                            "      <td>4.124751e+02</td>\n",
+                            "      <td>6.682517e+02</td>\n",
+                            "      <td>1.616334e+03</td>\n",
+                            "      <td>3.522806e+03</td>\n",
+                            "      <td>5.459596e+03</td>\n",
+                            "      <td>6.821745e+03</td>\n",
+                            "      <td>7.986305e+03</td>\n",
+                            "      <td>9.064963e+03</td>\n",
+                            "      <td>9.934779e+03</td>\n",
+                            "      <td>1.082886e+04</td>\n",
+                            "      <td>1.320022e+04</td>\n",
+                            "      <td>1.459313e+04</td>\n",
+                            "      <td>1.601071e+04</td>\n",
+                            "      <td>1.736882e+04</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Secondary Energy|Electricity|Biomass</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>2.352778e+05</td>\n",
+                            "      <td>3.407222e+05</td>\n",
+                            "      <td>4.669444e+05</td>\n",
+                            "      <td>5.942778e+05</td>\n",
+                            "      <td>7.219167e+05</td>\n",
+                            "      <td>8.496389e+05</td>\n",
+                            "      <td>9.855833e+05</td>\n",
+                            "      <td>1.173833e+06</td>\n",
+                            "      <td>1.359639e+06</td>\n",
+                            "      <td>1.471139e+06</td>\n",
+                            "      <td>1.513056e+06</td>\n",
+                            "      <td>1.544750e+06</td>\n",
+                            "      <td>1.564583e+06</td>\n",
+                            "      <td>1.557556e+06</td>\n",
+                            "      <td>1.543056e+06</td>\n",
+                            "      <td>1.574306e+06</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Secondary Energy|Electricity|Coal</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>7.419778e+06</td>\n",
+                            "      <td>8.252667e+06</td>\n",
+                            "      <td>9.246333e+06</td>\n",
+                            "      <td>1.075747e+07</td>\n",
+                            "      <td>6.045972e+06</td>\n",
+                            "      <td>8.733611e+05</td>\n",
+                            "      <td>6.444444e+03</td>\n",
+                            "      <td>5.027778e+03</td>\n",
+                            "      <td>3.694444e+03</td>\n",
+                            "      <td>2.416667e+03</td>\n",
+                            "      <td>1.555556e+03</td>\n",
+                            "      <td>9.444444e+02</td>\n",
+                            "      <td>4.444444e+02</td>\n",
+                            "      <td>5.277778e+02</td>\n",
+                            "      <td>5.555556e+02</td>\n",
+                            "      <td>5.000000e+02</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Secondary Energy|Electricity|Gas</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>3.816028e+06</td>\n",
+                            "      <td>5.050500e+06</td>\n",
+                            "      <td>5.968778e+06</td>\n",
+                            "      <td>7.060083e+06</td>\n",
+                            "      <td>6.469250e+06</td>\n",
+                            "      <td>4.551528e+06</td>\n",
+                            "      <td>2.907250e+06</td>\n",
+                            "      <td>2.602278e+06</td>\n",
+                            "      <td>1.752056e+06</td>\n",
+                            "      <td>1.218361e+06</td>\n",
+                            "      <td>6.538889e+05</td>\n",
+                            "      <td>5.281944e+05</td>\n",
+                            "      <td>2.423333e+05</td>\n",
+                            "      <td>1.685833e+05</td>\n",
+                            "      <td>4.166667e+04</td>\n",
+                            "      <td>3.888889e+02</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Secondary Energy|Electricity|Geothermal</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>6.041667e+04</td>\n",
+                            "      <td>9.677778e+04</td>\n",
+                            "      <td>1.799167e+05</td>\n",
+                            "      <td>3.474167e+05</td>\n",
+                            "      <td>5.260278e+05</td>\n",
+                            "      <td>6.213611e+05</td>\n",
+                            "      <td>6.291111e+05</td>\n",
+                            "      <td>6.177778e+05</td>\n",
+                            "      <td>5.893056e+05</td>\n",
+                            "      <td>5.187222e+05</td>\n",
+                            "      <td>4.333611e+05</td>\n",
+                            "      <td>3.603889e+05</td>\n",
+                            "      <td>2.924722e+05</td>\n",
+                            "      <td>2.492778e+05</td>\n",
+                            "      <td>2.059167e+05</td>\n",
+                            "      <td>1.937500e+05</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Secondary Energy|Electricity|Hydro</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>2.976944e+06</td>\n",
+                            "      <td>3.557028e+06</td>\n",
+                            "      <td>4.386694e+06</td>\n",
+                            "      <td>5.302056e+06</td>\n",
+                            "      <td>5.813167e+06</td>\n",
+                            "      <td>6.173778e+06</td>\n",
+                            "      <td>6.423194e+06</td>\n",
+                            "      <td>6.604167e+06</td>\n",
+                            "      <td>6.717417e+06</td>\n",
+                            "      <td>6.770250e+06</td>\n",
+                            "      <td>6.782028e+06</td>\n",
+                            "      <td>6.775917e+06</td>\n",
+                            "      <td>6.722667e+06</td>\n",
+                            "      <td>6.655833e+06</td>\n",
+                            "      <td>6.631806e+06</td>\n",
+                            "      <td>6.533167e+06</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Secondary Energy|Electricity|Nuclear</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>2.861861e+06</td>\n",
+                            "      <td>2.642750e+06</td>\n",
+                            "      <td>2.448556e+06</td>\n",
+                            "      <td>2.214167e+06</td>\n",
+                            "      <td>2.055667e+06</td>\n",
+                            "      <td>1.876222e+06</td>\n",
+                            "      <td>1.617278e+06</td>\n",
+                            "      <td>1.502778e+06</td>\n",
+                            "      <td>1.304083e+06</td>\n",
+                            "      <td>1.098694e+06</td>\n",
+                            "      <td>8.686111e+05</td>\n",
+                            "      <td>6.451944e+05</td>\n",
+                            "      <td>2.717500e+05</td>\n",
+                            "      <td>5.925000e+04</td>\n",
+                            "      <td>3.916667e+03</td>\n",
+                            "      <td>1.388889e+02</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Secondary Energy|Electricity|Oil</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>1.088861e+06</td>\n",
+                            "      <td>1.016972e+06</td>\n",
+                            "      <td>8.353889e+05</td>\n",
+                            "      <td>6.174167e+05</td>\n",
+                            "      <td>4.317778e+05</td>\n",
+                            "      <td>1.960556e+05</td>\n",
+                            "      <td>6.919444e+04</td>\n",
+                            "      <td>4.797222e+04</td>\n",
+                            "      <td>3.175000e+04</td>\n",
+                            "      <td>1.169444e+04</td>\n",
+                            "      <td>6.722222e+03</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "      <td>2.777778e+01</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Secondary Energy|Electricity|Other</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>0.000000e+00</td>\n",
+                            "      <td>0.000000e+00</td>\n",
+                            "      <td>4.444444e+02</td>\n",
+                            "      <td>2.166667e+03</td>\n",
+                            "      <td>8.913889e+04</td>\n",
+                            "      <td>4.938889e+05</td>\n",
+                            "      <td>1.204583e+06</td>\n",
+                            "      <td>1.985111e+06</td>\n",
+                            "      <td>2.790639e+06</td>\n",
+                            "      <td>3.488083e+06</td>\n",
+                            "      <td>4.020806e+06</td>\n",
+                            "      <td>4.434639e+06</td>\n",
+                            "      <td>5.261472e+06</td>\n",
+                            "      <td>6.099583e+06</td>\n",
+                            "      <td>6.740833e+06</td>\n",
+                            "      <td>7.547194e+06</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Secondary Energy|Electricity|Solar</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>4.083333e+03</td>\n",
+                            "      <td>8.325000e+04</td>\n",
+                            "      <td>2.616111e+05</td>\n",
+                            "      <td>9.263611e+05</td>\n",
+                            "      <td>5.500722e+06</td>\n",
+                            "      <td>1.566242e+07</td>\n",
+                            "      <td>2.575731e+07</td>\n",
+                            "      <td>3.404253e+07</td>\n",
+                            "      <td>4.088394e+07</td>\n",
+                            "      <td>4.723214e+07</td>\n",
+                            "      <td>5.327061e+07</td>\n",
+                            "      <td>5.819236e+07</td>\n",
+                            "      <td>6.826367e+07</td>\n",
+                            "      <td>7.754106e+07</td>\n",
+                            "      <td>8.359456e+07</td>\n",
+                            "      <td>9.270394e+07</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>Updated|Secondary Energy|Electricity|Wind</th>\n",
+                            "      <th>bla</th>\n",
+                            "      <td>1.091389e+05</td>\n",
+                            "      <td>5.946944e+05</td>\n",
+                            "      <td>8.323889e+05</td>\n",
+                            "      <td>1.482806e+06</td>\n",
+                            "      <td>3.695778e+06</td>\n",
+                            "      <td>8.141417e+06</td>\n",
+                            "      <td>1.318953e+07</td>\n",
+                            "      <td>1.727517e+07</td>\n",
+                            "      <td>2.112919e+07</td>\n",
+                            "      <td>2.367689e+07</td>\n",
+                            "      <td>2.569986e+07</td>\n",
+                            "      <td>2.771675e+07</td>\n",
+                            "      <td>3.280081e+07</td>\n",
+                            "      <td>3.570786e+07</td>\n",
+                            "      <td>3.840797e+07</td>\n",
+                            "      <td>4.123369e+07</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
                         "text/plain": [
-                            "Index(['Updated|Capacity|Electricity|Biomass',\n",
-                            "       'Updated|Capacity|Electricity|Coal', 'Updated|Capacity|Electricity|Gas',\n",
-                            "       'Updated|Capacity|Electricity|Geothermal',\n",
-                            "       'Updated|Capacity|Electricity|Hydro',\n",
-                            "       'Updated|Capacity|Electricity|Nuclear',\n",
-                            "       'Updated|Capacity|Electricity|Oil',\n",
-                            "       'Updated|Capacity|Electricity|Other',\n",
-                            "       'Updated|Capacity|Electricity|Solar',\n",
-                            "       'Updated|Capacity|Electricity|Wind',\n",
-                            "       'Updated|Secondary Energy|Electricity|Biomass',\n",
-                            "       'Updated|Secondary Energy|Electricity|Coal',\n",
-                            "       'Updated|Secondary Energy|Electricity|Gas',\n",
-                            "       'Updated|Secondary Energy|Electricity|Geothermal',\n",
-                            "       'Updated|Secondary Energy|Electricity|Hydro',\n",
-                            "       'Updated|Secondary Energy|Electricity|Nuclear',\n",
-                            "       'Updated|Secondary Energy|Electricity|Oil',\n",
-                            "       'Updated|Secondary Energy|Electricity|Other',\n",
-                            "       'Updated|Secondary Energy|Electricity|Solar',\n",
-                            "       'Updated|Secondary Energy|Electricity|Wind'],\n",
-                            "      dtype='object', name='variable')"
+                            "                                                                                                                        2005  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   4.298430e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   1.238877e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   1.096674e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   8.112900e+00   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   8.065684e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   4.083700e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   5.112499e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   0.000000e+00   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   2.682400e+00   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   3.226040e+01   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   2.352778e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   7.419778e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   3.816028e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   6.041667e+04   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   2.976944e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   2.861861e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   1.088861e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   0.000000e+00   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   4.083333e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   1.091389e+05   \n",
+                            "\n",
+                            "                                                                                                                        2010  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   6.247170e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   1.525950e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   1.343108e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   1.299850e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   9.633523e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   4.043094e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   4.630961e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   0.000000e+00   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   4.961380e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   1.811785e+02   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   3.407222e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   8.252667e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   5.050500e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   9.677778e+04   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   3.557028e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   2.642750e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   1.016972e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   0.000000e+00   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   8.325000e+04   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   5.946944e+05   \n",
+                            "\n",
+                            "                                                                                                                        2015  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   8.566980e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   1.876595e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   1.603169e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   2.416120e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   1.239617e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   3.791375e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   3.709638e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   3.396000e-01   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   2.198533e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   4.124751e+02   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   4.669444e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   9.246333e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   5.968778e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   1.799167e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   4.386694e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   2.448556e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   8.353889e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   4.444444e+02   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   2.616111e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   8.323889e+05   \n",
+                            "\n",
+                            "                                                                                                                        2020  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   1.088834e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   2.075232e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   1.852649e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   4.665730e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   1.500451e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   3.452239e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   2.817401e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   1.656200e+00   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   6.509654e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   6.682517e+02   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   5.942778e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   1.075747e+07   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   7.060083e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   3.474167e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   5.302056e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   2.214167e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   6.174167e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   2.166667e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   9.263611e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   1.482806e+06   \n",
+                            "\n",
+                            "                                                                                                                        2025  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   1.285653e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   1.225451e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   1.761806e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   7.064690e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   1.669357e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   3.101729e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   1.932768e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   8.110980e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   3.785689e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   1.616334e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   7.219167e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   6.045972e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   6.469250e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   5.260278e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   5.813167e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   2.055667e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   4.317778e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   8.913889e+04   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   5.500722e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   3.695778e+06   \n",
+                            "\n",
+                            "                                                                                                                        2030  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   1.378452e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   1.820149e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   1.584403e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   8.345060e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   1.786047e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   2.755920e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   9.023290e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   4.695231e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   1.109448e+04   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   3.522806e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   8.496389e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   8.733611e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   4.551528e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   6.213611e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   6.173778e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   1.876222e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   1.960556e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   4.938889e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   1.566242e+07   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   8.141417e+06   \n",
+                            "\n",
+                            "                                                                                                                        2035  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   1.328316e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   1.353200e+00   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   1.423539e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   8.448930e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   1.858782e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   2.347028e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   3.159640e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   1.253078e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   1.906378e+04   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   5.459596e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   9.855833e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   6.444444e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   2.907250e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   6.291111e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   6.423194e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   1.617278e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   6.919444e+04   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   1.204583e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   2.575731e+07   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   1.318953e+07   \n",
+                            "\n",
+                            "                                                                                                                        2040  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   1.227382e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   1.072900e+00   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   1.289478e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   8.296880e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   1.902635e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   2.144376e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   2.190000e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   2.254017e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   2.556775e+04   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   6.821745e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   1.173833e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   5.027778e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   2.602278e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   6.177778e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   6.604167e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   1.502778e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   4.797222e+04   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   1.985111e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   3.404253e+07   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   1.727517e+07   \n",
+                            "\n",
+                            "                                                                                                                        2045  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   1.063772e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   7.763000e-01   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   8.638716e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   7.914520e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   1.925653e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   1.860849e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   1.450230e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   3.341699e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   3.097003e+04   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   7.986305e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   1.359639e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   3.694444e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   1.752056e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   5.893056e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   6.717417e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   1.304083e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   3.175000e+04   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   2.790639e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   4.088394e+07   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   2.112919e+07   \n",
+                            "\n",
+                            "                                                                                                                        2050  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   8.602650e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   5.029000e-01   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   5.628482e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   6.966280e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   1.933520e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   1.567766e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   5.341200e+00   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   4.267072e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   3.608447e+04   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   9.064963e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   1.471139e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   2.416667e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   1.218361e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   5.187222e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   6.770250e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   1.098694e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   1.169444e+04   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   3.488083e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   4.723214e+07   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   2.367689e+07   \n",
+                            "\n",
+                            "                                                                                                                        2055  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   6.565480e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   3.111000e-01   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   3.937209e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   5.820210e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   1.931110e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   1.239472e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   3.064300e+00   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   4.925403e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   4.110399e+04   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   9.934779e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   1.513056e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   1.555556e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   6.538889e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   4.333611e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   6.782028e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   8.686111e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   6.722222e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   4.020806e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   5.327061e+07   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   2.569986e+07   \n",
+                            "\n",
+                            "                                                                                                                        2060  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   4.575910e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   1.836000e-01   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   3.499091e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   4.840070e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   1.922569e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   9.206670e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   1.200000e-02   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   5.433398e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   4.527457e+04   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   1.082886e+04   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   1.544750e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   9.444444e+02   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   5.281944e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   3.603889e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   6.775917e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   6.451944e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   2.777778e+01   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   4.434639e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   5.819236e+07   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   2.771675e+07   \n",
+                            "\n",
+                            "                                                                                                                        2070  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   1.450470e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   7.830000e-02   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   3.063883e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   3.927950e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   1.893641e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   3.877600e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   1.200000e-02   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   6.432168e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   5.443399e+04   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   1.320022e+04   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   1.564583e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   4.444444e+02   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   2.423333e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   2.924722e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   6.722667e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   2.717500e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   2.777778e+01   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   5.261472e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   6.826367e+07   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   3.280081e+07   \n",
+                            "\n",
+                            "                                                                                                                        2080  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   3.962800e+00   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   9.180000e-02   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   2.135970e+02   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   3.347930e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   1.860861e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   8.455000e+00   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   1.200000e-02   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   7.478326e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   6.305545e+04   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   1.459313e+04   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   1.557556e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   5.277778e+02   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   1.685833e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   2.492778e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   6.655833e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   5.925000e+04   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   2.777778e+01   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   6.099583e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   7.754106e+07   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   3.570786e+07   \n",
+                            "\n",
+                            "                                                                                                                        2090  \\\n",
+                            "model                 scenario                     region variable                                        unit                 \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   8.198000e-01   \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   9.650000e-02   \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   5.260450e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   2.765300e+01   \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   1.846102e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   5.580000e-01   \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   1.210000e-02   \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   8.321384e+03   \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   6.884808e+04   \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   1.601071e+04   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   1.543056e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   5.555556e+02   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   4.166667e+04   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   2.059167e+05   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   6.631806e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   3.916667e+03   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   2.777778e+01   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   6.740833e+06   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   8.359456e+07   \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   3.840797e+07   \n",
+                            "\n",
+                            "                                                                                                                        2100  \n",
+                            "model                 scenario                     region variable                                        unit                \n",
+                            "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Updated|Capacity|Electricity|Biomass            bla   2.150000e-01  \n",
+                            "                                                          Updated|Capacity|Electricity|Coal               bla   8.660000e-02  \n",
+                            "                                                          Updated|Capacity|Electricity|Gas                bla   2.717000e-01  \n",
+                            "                                                          Updated|Capacity|Electricity|Geothermal         bla   2.601980e+01  \n",
+                            "                                                          Updated|Capacity|Electricity|Hydro              bla   1.805140e+03  \n",
+                            "                                                          Updated|Capacity|Electricity|Nuclear            bla   1.900000e-02  \n",
+                            "                                                          Updated|Capacity|Electricity|Oil                bla   1.260000e-02  \n",
+                            "                                                          Updated|Capacity|Electricity|Other              bla   9.334424e+03  \n",
+                            "                                                          Updated|Capacity|Electricity|Solar              bla   7.743017e+04  \n",
+                            "                                                          Updated|Capacity|Electricity|Wind               bla   1.736882e+04  \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Biomass    bla   1.574306e+06  \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Coal       bla   5.000000e+02  \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Gas        bla   3.888889e+02  \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Geothermal bla   1.937500e+05  \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Hydro      bla   6.533167e+06  \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   1.388889e+02  \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Oil        bla   2.777778e+01  \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Other      bla   7.547194e+06  \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Solar      bla   9.270394e+07  \n",
+                            "                                                          Updated|Secondary Energy|Electricity|Wind       bla   4.123369e+07  "
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "\"Updated|\" + projectlevel(df.index, \"variable\")"
+                "from pandas_indexing import assignlevel\n",
+                "\n",
+                "assignlevel(df, variable=\"Updated|\" + projectlevel(df.index, \"variable\"), unit=\"bla\")\n",
+                "# or: df.idx.assign(variable=df.index.idx.project(\"variable\"), unit=\"bla\")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "1349c89d",
+            "metadata": {},
+            "source": [
+                "This particular case is even more clearly handled with `formatlevel`:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
-            "id": "ca2a3c70",
+            "execution_count": 24,
+            "id": "f4cb55c2",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -2684,36 +4576,38 @@
                             "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   1.388889e+02  \n",
                             "                                                          Updated|Secondary Energy|Electricity|Oil        bla   2.777778e+01  \n",
                             "                                                          Updated|Secondary Energy|Electricity|Other      bla   7.547194e+06  \n",
                             "                                                          Updated|Secondary Energy|Electricity|Solar      bla   9.270394e+07  \n",
                             "                                                          Updated|Secondary Energy|Electricity|Wind       bla   4.123369e+07  "
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from pandas_indexing import assignlevel\n",
+                "from pandas_indexing import formatlevel\n",
                 "\n",
-                "assignlevel(df, variable=\"Updated|\" + projectlevel(df.index, \"variable\"), unit=\"bla\")"
+                "formatlevel(df, variable=\"Updated|{variable}\", unit=\"bla\")\n",
+                "# or: df.idx.format(variable=...)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "a8416465",
             "metadata": {},
             "source": [
-                "and as such avoids having to rely on `reset_index`, `set_index` pairs, which are painful for large data, since `set_index` is expensive!"
+                "Both functions avoid having to rely on `reset_index`, `set_index` pairs, which are painful for large data, since `set_index` is expensive!"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 25,
             "id": "72d60d5e",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -3534,42 +5428,170 @@
                             "                                                                   GWh/yr  1.388889e+02  \n",
                             "                                                                   GWh/yr  2.777778e+01  \n",
                             "                                                                   GWh/yr  7.547194e+06  \n",
                             "                                                                   GWh/yr  9.270394e+07  \n",
                             "                                                                   GWh/yr  4.123369e+07  "
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": 25,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.reset_index().assign(variable=\"Capacity\").set_index(df.index.names)"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "63103fb7",
+            "metadata": {},
+            "source": [
+                "# Examining level values and level combinations\n",
+                "\n",
+                "We already encountered the possibility to get an overview of the available levels and their values with describelevel:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 26,
+            "id": "029603e9",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Index:\n",
+                        " * model    : REMIND-MAgPIE 2.1-4.3 (1)\n",
+                        " * scenario : DeepElec_SSP2_HighRE_Budg900 (1)\n",
+                        " * region   : World (1)\n",
+                        " * variable : Capacity|Electricity|Biomass, ... (20)\n",
+                        " * unit     : GW, GWh/yr (2)\n",
+                        "\n",
+                        "Columns:\n",
+                        " * <unnamed> : 2005, 2010, 2015, 2020, 2025, 2030, 2035, 2040, ... 2100 (16)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "describelevel(df)  # or: df.idx"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "5938866f",
+            "metadata": {},
+            "source": [
+                "Often it is necessary to get programmatic access to the unique values of one or more levels:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 27,
+            "id": "f9fe7174",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "Index(['Capacity|Electricity|Biomass', 'Capacity|Electricity|Coal',\n",
+                            "       'Capacity|Electricity|Gas', 'Capacity|Electricity|Geothermal',\n",
+                            "       'Capacity|Electricity|Hydro', 'Capacity|Electricity|Nuclear',\n",
+                            "       'Capacity|Electricity|Oil', 'Capacity|Electricity|Other',\n",
+                            "       'Capacity|Electricity|Solar', 'Capacity|Electricity|Wind',\n",
+                            "       'Secondary Energy|Electricity|Biomass',\n",
+                            "       'Secondary Energy|Electricity|Coal', 'Secondary Energy|Electricity|Gas',\n",
+                            "       'Secondary Energy|Electricity|Geothermal',\n",
+                            "       'Secondary Energy|Electricity|Hydro',\n",
+                            "       'Secondary Energy|Electricity|Nuclear',\n",
+                            "       'Secondary Energy|Electricity|Oil',\n",
+                            "       'Secondary Energy|Electricity|Other',\n",
+                            "       'Secondary Energy|Electricity|Solar',\n",
+                            "       'Secondary Energy|Electricity|Wind'],\n",
+                            "      dtype='object', name='variable')"
+                        ]
+                    },
+                    "execution_count": 27,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "from pandas_indexing import uniquelevel\n",
+                "\n",
+                "uniquelevel(df, \"variable\")\n",
+                "# or: df.idx.unique(\"variable\")\n",
+                "# or in vanilla pandas: df.index.unique(\"variable\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 28,
+            "id": "23378320",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "MultiIndex([(           'Capacity|Electricity|Biomass',     'GW'),\n",
+                            "            (              'Capacity|Electricity|Coal',     'GW'),\n",
+                            "            (               'Capacity|Electricity|Gas',     'GW'),\n",
+                            "            (        'Capacity|Electricity|Geothermal',     'GW'),\n",
+                            "            (             'Capacity|Electricity|Hydro',     'GW'),\n",
+                            "            (           'Capacity|Electricity|Nuclear',     'GW'),\n",
+                            "            (               'Capacity|Electricity|Oil',     'GW'),\n",
+                            "            (             'Capacity|Electricity|Other',     'GW'),\n",
+                            "            (             'Capacity|Electricity|Solar',     'GW'),\n",
+                            "            (              'Capacity|Electricity|Wind',     'GW'),\n",
+                            "            (   'Secondary Energy|Electricity|Biomass', 'GWh/yr'),\n",
+                            "            (      'Secondary Energy|Electricity|Coal', 'GWh/yr'),\n",
+                            "            (       'Secondary Energy|Electricity|Gas', 'GWh/yr'),\n",
+                            "            ('Secondary Energy|Electricity|Geothermal', 'GWh/yr'),\n",
+                            "            (     'Secondary Energy|Electricity|Hydro', 'GWh/yr'),\n",
+                            "            (   'Secondary Energy|Electricity|Nuclear', 'GWh/yr'),\n",
+                            "            (       'Secondary Energy|Electricity|Oil', 'GWh/yr'),\n",
+                            "            (     'Secondary Energy|Electricity|Other', 'GWh/yr'),\n",
+                            "            (     'Secondary Energy|Electricity|Solar', 'GWh/yr'),\n",
+                            "            (      'Secondary Energy|Electricity|Wind', 'GWh/yr')],\n",
+                            "           names=['variable', 'unit'])"
+                        ]
+                    },
+                    "execution_count": 28,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "uniquelevel(df, [\"variable\", \"unit\"])"
+            ]
+        },
+        {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "c84e2a30-1880-4687-b450-6c5b4dac3c01",
             "metadata": {},
             "source": [
-                "## BEWARE: Pitfalls"
+                "# BEWARE: Pitfalls"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "ec137242",
             "metadata": {},
             "source": [
                 "`concat` ignores level order, so make sure to `reorder_levels` them"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 29,
             "id": "24d42af8-ffd3-4281-9d75-1449046fd6fd",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "variable  year   \n",
@@ -3596,26 +5618,26 @@
                             "2030      Nuclear     275.5920\n",
                             "2040      Nuclear     214.4376\n",
                             "2050      Nuclear     156.7766\n",
                             "2060      Nuclear      92.0667\n",
                             "dtype: float64"
                         ]
                     },
-                    "execution_count": 23,
+                    "execution_count": 29,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "pd.concat([simple_fossil_series, simple_fossil_series.swaplevel()])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 30,
             "id": "254197c5-8498-4c69-a30d-044e7edb7b53",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "variable  year\n",
@@ -3642,15 +5664,15 @@
                             "Nuclear   2030     275.5920\n",
                             "          2040     214.4376\n",
                             "          2050     156.7766\n",
                             "          2060      92.0667\n",
                             "dtype: float64"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 30,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "pd.concat(\n",
                 "    [\n",
@@ -3670,70 +5692,25 @@
             "source": [
                 "# Additional helpful multi-index helpers\n",
                 "\n",
                 "To know which labels exist in a given `level` the index's `unique` method is helpful:"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 25,
-            "id": "a8300699",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "MultiIndex([('REMIND-MAgPIE 2.1-4.3', 2030),\n",
-                            "            ('REMIND-MAgPIE 2.1-4.3', 2040),\n",
-                            "            ('REMIND-MAgPIE 2.1-4.3', 2050),\n",
-                            "            ('REMIND-MAgPIE 2.1-4.3', 2060)],\n",
-                            "           names=['model', 'year'])"
-                        ]
-                    },
-                    "execution_count": 25,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "projectlevel(fossil_series, [\"model\", \"year\"]).index.unique()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 26,
-            "id": "187e2a70",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "Int64Index([2030, 2040, 2050, 2060], dtype='int64', name='year')"
-                        ]
-                    },
-                    "execution_count": 26,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "fossil_series.index.unique(\"year\")"
-            ]
-        },
-        {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "46c57e84",
             "metadata": {},
             "source": [
                 "MultiIndex rendering is often annoying to read, since the important information might get abbreviated away, then converting it into a dataframe is helpful"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 31,
             "id": "5b7cb7db",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "MultiIndex([('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...),\n",
@@ -3747,26 +5724,26 @@
                             "            ('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...),\n",
                             "            ('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...),\n",
                             "            ('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...),\n",
                             "            ('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...)],\n",
                             "           names=['model', 'scenario', 'variable'])"
                         ]
                     },
-                    "execution_count": 27,
+                    "execution_count": 31,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "projectlevel(fossil_series.index, [\"model\", \"scenario\", \"variable\"])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 32,
             "id": "5b7cb7db",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -3881,15 +5858,15 @@
                             "7   REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900      Gas\n",
                             "8   REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  Nuclear\n",
                             "9   REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  Nuclear\n",
                             "10  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  Nuclear\n",
                             "11  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  Nuclear"
                         ]
                     },
-                    "execution_count": 28,
+                    "execution_count": 32,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "projectlevel(fossil_series.index, [\"model\", \"scenario\", \"variable\"]).to_frame(\n",
                 "    index=False\n",
```

### Comparing `pandas-indexing-0.2.4/pyproject.toml` & `pandas-indexing-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.4/src/pandas_indexing/__init__.py` & `pandas-indexing-0.2.5/src/pandas_indexing/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 
 from . import core, datasets
 from .arithmetics import add, divide, multiply, subtract
 from .core import (
     alignlevel,
     alignlevels,
     assignlevel,
+    describelevel,
     dropnalevel,
+    extractlevel,
+    formatlevel,
     index_names,
     projectlevel,
     semijoin,
     uniquelevel,
 )
 from .selectors import isin, ismatch
```

### Comparing `pandas-indexing-0.2.4/src/pandas_indexing/arithmetics.py` & `pandas-indexing-0.2.5/src/pandas_indexing/arithmetics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Provide aligned basic arithmetic ops.
+"""Provide aligned basic arithmetic ops.
 
 Simple arithmetic operations :py:func:`add`, :py:func:`divide`, :py:func:`multiply` and
 :py:func:`subtract` which allow setting the standard how="outer" alignment that pandas
 uses by default.
 
 In practice, this means if dataframes do not share the same axes one can choose to get
 the results for only the items index items existing in both indices (``how="inner"``) or
```

### Comparing `pandas-indexing-0.2.4/src/pandas_indexing/core.py` & `pandas-indexing-0.2.5/src/pandas_indexing/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Core module.
 """
+import re
 from functools import reduce
 from itertools import chain
 from operator import and_, or_
-from typing import Any, Literal, Optional, Sequence, TypeVar, Union
+from typing import Any, Literal, Optional, Sequence, Tuple, TypeVar, Union
 
 import numpy as np
+from deprecated import deprecated
 from pandas import DataFrame, Index, MultiIndex, Series
 from pandas.core.indexes.frozen import FrozenList
 
-from .utils import print_list
+from .utils import Axis, doc, get_axis, print_list
 
 
 Data = Union[Series, DataFrame]
 T = TypeVar("T", bound=Union[Index, DataFrame, Series])
 S = TypeVar("S", bound=Union[DataFrame, Series])
 
 
@@ -57,236 +59,275 @@
 
     if order:
         new_index = new_index.reorder_levels(order)
 
     return new_index
 
 
+@doc(
+    df="""
+    df : DataFrame, Series or Index
+        Index, Series or DataFrame of which to change index levels\
+    """
+)
 def assignlevel(
     df: T,
     frame: Optional[Data] = None,
     order: bool = False,
-    axis: int = 0,
+    axis: Axis = 0,
     **labels: Any,
 ) -> T:
-    """
-    Add or overwrite levels on a multiindex.
+    """Add or overwrite levels on a multiindex.
 
     Parameters
-    ----------
-    df : Series|DataFrame|MultiIndex
-        Series or DataFrame on which to change index or index to change
-    frame : Series|DataFrame, optional
+    ----------\
+    {df}
+    frame : Series or DataFrame, optional
         Additional labels
     order : list of str, optional
         Level names in desired order or False, by default False
-    axis : int, optional
-        Axis where to update multiindex, by default 0
+    axis : {{0, 1, "index", "columns"}}, default 0
+        Axis where to update multiindex
     **labels
         Labels for each new index level
 
     Returns
     -------
     df
         Series or DataFrame with changed index or new MultiIndex
     """
     if isinstance(df, Index):
         return _assignlevel(df, frame=frame, order=order, **labels)
 
-    if isinstance(df, Series):
-        index = df.index
-    elif isinstance(df, DataFrame):
-        index = df.index if axis == 0 else df.columns
-    else:
-        raise TypeError(
-            f"assignlevel expects an Index, Series or DataFrame ({type(df)=})"
-        )
-
+    index = get_axis(df, axis)
     new_index = _assignlevel(index, frame=frame, order=order, **labels)
-
     return df.set_axis(new_index, axis=axis)
 
 
 def _projectlevel(index: Index, levels: Sequence[str]) -> Index:
     levels = np.atleast_1d(levels)
     if len(levels) == 1:
         return index.get_level_values(levels[0])
 
     return index.droplevel(index.names.difference(levels)).reorder_levels(levels)
 
 
-def projectlevel(
-    index_or_series: T, levels: Sequence[str], axis: Union[int, str] = 0
-) -> T:
-    """
-    Project multiindex to given `levels`
+@doc(
+    index_or_data="""
+    index_or_data : DataFrame, Series or Index
+        Index, Series or DataFrame to project\
+    """
+)
+def projectlevel(index_or_data: T, levels: Sequence[str], axis: Axis = 0) -> T:
+    """Project multiindex to given ``levels``.
 
     Drops all levels except the ones explicitly mentioned from a given multiindex
     or an axis of a series or a dataframe.
 
     Parameters
-    ----------
-    index_or_series : MultiIndex|Series|DataFrame
-        MultiIndex, Series or DataFrame to project
-    levels : Sequence[str]
+    ----------\
+    {index_or_data}
+    levels : sequence of str
         Names of levels to project on (to keep)
-    axis : int, optional
-        Axis of DataFrame to project, by default 0
+    axis : {{0, 1, "index", "columns"}}, default 0
+        Axis of DataFrame to project
 
     Returns
     -------
-    index_or_series : Index|MultiIndex|Series|DataFrame
+    index_or_data : Index|MultiIndex|Series|DataFrame
 
     See also
     --------
     pandas.MultiIndex.droplevel
     pandas.Series.droplevel
     pandas.DataFrame.droplevel
     """
-    if isinstance(index_or_series, Index):
-        return _projectlevel(index_or_series, levels)
+    if isinstance(index_or_data, Index):
+        return _projectlevel(index_or_data, levels)
 
-    index = index_or_series.index if axis in (0, "index") else index_or_series.columns
-    return index_or_series.set_axis(_projectlevel(index, levels), axis=axis)
+    index = get_axis(index_or_data.index, axis)
+    return index_or_data.set_axis(_projectlevel(index, levels), axis=axis)
 
 
 def _notna(
     index: Index,
     subset: Optional[Sequence[str]] = None,
     how: Literal["any", "all"] = "any",
 ) -> np.ndarray:
-    index = ensure_multiindex(index)
+    if not isinstance(index, MultiIndex):
+        return index.notna()
 
     subset = index.names if subset is None else np.atleast_1d(subset)
     codes = [index.codes[index.names.index(n)] for n in subset]
     op = and_ if how == "any" else or_
     return reduce(op, [c != -1 for c in codes])
 
 
+def notna(
+    index_or_data: Union[Index, Series, DataFrame],
+    subset: Optional[Sequence[str]] = None,
+    how: Literal["any", "all"] = "any",
+    axis: Axis = 0,
+):
+    return _notna(get_axis(index_or_data, axis), subset, how)
+
+
+def isna(
+    index_or_data: Union[Index, Series, DataFrame],
+    subset: Optional[Sequence[str]] = None,
+    how: Literal["any", "all"] = "any",
+    axis: Axis = 0,
+):
+    return ~_notna(get_axis(index_or_data, axis), subset, how)
+
+
+@doc(
+    index_or_data="""
+    index_or_data : DataFrame, Series or Index
+        Index, Series or DataFrame of which to drop rows or columns\
+    """
+)
 def dropnalevel(
-    index_or_series: T,
+    index_or_data: T,
     subset: Optional[Sequence[str]] = None,
     how: Literal["any", "all"] = "any",
-    axis: Union[int, str] = 0,
+    axis: Axis = 0,
 ) -> T:
-    """
-    Remove missing index values.
+    """Remove missing index values.
 
-    Drops all index entries for which any or all (`how`) levels are
+    Drops all index entries for which any or all (``how``) levels are
     undefined.
 
     Parameters
-    ----------
-    index_or_series : MultiIndex|Series|DataFrame
-        MultiIndex, Series or DataFrame to project
+    ----------\
+    {index_or_data}
     subset : Sequence[str], optional
         Names of levels on which to check for NA values
-    how : "any" (default) or "all"
-        Whether to remove an entry if all levels are NA only a single one
-    axis : int, optional
-        Axis of DataFrame to check on, by default 0
+    how : {{"any", "all"}}
+        Whether to remove an entry if all levels are NA or only a single one
+    axis : {{0, 1, "index", "columns"}}, default 0
+        Axis of DataFrame to check on
 
     Returns
     -------
-    index_or_series : Index|MultiIndex|Series|DataFrame
+    index_or_data : Index|MultiIndex|Series|DataFrame
 
     See also
     --------
     pandas.DataFrame.dropna
     pandas.Series.dropna
     pandas.Index.dropna
     """
-    if isinstance(index_or_series, Index):
-        return index_or_series[_notna(index_or_series, subset, how)]
+    if isinstance(index_or_data, Index):
+        return index_or_data[_notna(index_or_data, subset, how)]
 
     if axis in (0, "index"):
-        return index_or_series.loc[_notna(index_or_series.index, subset, how)]
+        return index_or_data.loc[_notna(index_or_data.index, subset, how)]
 
-    return index_or_series.loc[:, _notna(index_or_series.columns, subset, how)]
+    return index_or_data.loc[:, _notna(index_or_data.columns, subset, how)]
 
 
+@doc(
+    index_or_data="""
+    index_or_data : DataFrame, Series or Index
+        Index, Series or DataFrame of which to describe index levels\
+    """
+)
 def uniquelevel(
     index_or_data: Union[DataFrame, Series, Index],
     levels: Union[str, Sequence[str], None],
-    axis: Union[int, Literal["index", "columns"]] = 0,
+    axis: Axis = 0,
 ) -> Index:
-    """
-    Return unique index levels.
+    """Return unique index levels.
 
     Parameters
-    ----------
-    index_or_data : Index|Series|DataFrame
-        Index, Series or DataFrame from which to get unique values
+    ----------\
+    {index_or_data}
     levels : str or Sequence[str], optional
         Names of levels to get unique values of
-    axis : int, optional
-        Axis of DataFrame to check on, by default 0
+    axis : {{0, 1, "index", "columns"}}, default 0
+        Axis of DataFrame to check on
 
     Returns
     -------
     unique_index : Index
 
     See also
     --------
     pandas.Index.unique
     """
-    if isinstance(index_or_data, (DataFrame, Series)):
-        index_or_data = (
-            index_or_data.index if axis in (0, "index") else index_or_data.columns
-        )
+    index = get_axis(index_or_data, axis)
 
     if levels is None or isinstance(levels, str):
-        return index_or_data.unique(level=levels)
+        return index.unique(level=levels)
 
     levels = list(levels)
     if len(levels) == 1:
-        return index_or_data.unique(level=levels[0])
+        return index.unique(level=levels[0])
 
-    return projectlevel(index_or_data, levels).unique()
+    return projectlevel(index, levels).unique()
 
 
-def _summarylevel(index: Index, n: int = 80) -> str:
+def _describelevel(index: Index, n: int = 80) -> str:
     def name(l):
         return "<unnamed>" if l is None else l
 
     c1 = max(len(name(l)) for l in index.names) + 1
     c2 = n - c1 - 5
     return "\n".join(
         f" * {name(l):{c1}}: {print_list(index.unique(l), c2)}" for l in index.names
     )
 
 
-def summarylevel(index_or_data: Union[DataFrame, Series, Index], n: int = 80):
-    """
-    Summarize index levels.
+@doc(
+    index_or_data="""
+    index_or_data : DataFrame, Series or Index
+        Index, Series or DataFrame of which to describe index levels\
+    """
+)
+def describelevel(
+    index_or_data: Union[DataFrame, Series, Index], n: int = 80, as_str: bool = False
+) -> Optional[str]:
+    """Describe index levels.
 
     Parameters
-    ----------
-    index_or_data : Index|Series|DataFrame
-        Index, Series or DataFrame of which to summarize index levels
+    ----------\
+    {index_or_data}
     n : int, default 80
         The maximum line length
+    as_str : bool, default False
+        Whether to return as string or print, instead
 
     Returns
     -------
-    summary : str
+    description : str, optional
+        if as_str is True
 
     See also
     --------
     pandas.DataFrame.describe
     """
     if isinstance(index_or_data, DataFrame):
-        index_desc = _summarylevel(index_or_data.index, n=n)
-        columns_desc = _summarylevel(index_or_data.columns, n=n)
-        return f"Index:\n{index_desc}\n\nColumns:\n{columns_desc}"
+        index_desc = _describelevel(index_or_data.index, n=n)
+        columns_desc = _describelevel(index_or_data.columns, n=n)
+        description = f"Index:\n{index_desc}\n\nColumns:\n{columns_desc}"
+    else:
+        if isinstance(index_or_data, Series):
+            index_or_data = index_or_data.index
+        description = f"Index:\n{_describelevel(index_or_data, n=n)}"
+
+    if as_str:
+        return description
+
+    print(description)
 
-    if isinstance(index_or_data, Series):
-        index_or_data = index_or_data.index
 
-    return f"Index:\n{_summarylevel(index_or_data, n=n)}"
+summarylevel = deprecated(
+    describelevel, reason="Use describelevel instead", version="v0.2.5"
+)
 
 
 def index_names(s, raise_on_index=False):
     if isinstance(s, (Series, DataFrame)):
         s = s.index
 
     if isinstance(s, MultiIndex):
@@ -343,80 +384,246 @@
 
     return (
         ensure_multiindex(l).reorder_levels(l_and_r.union(l_but_not_r)),
         ensure_multiindex(r).reorder_levels(l_and_r.union(r_but_not_l)),
     )
 
 
+@doc(
+    frame_or_series="""
+    frame_or_series : DataFrame or Series
+        Data to be filtered\
+    """
+)
 def semijoin(
-    df_or_series: S,
+    frame_or_series: S,
     other: Index,
     *,
     how: Literal["left", "right", "inner", "outer"] = "left",
     level: Union[str, int, None] = None,
     sort: bool = False,
-    axis: Literal[0, 1] = 0,
+    axis: Axis = 0,
 ) -> S:
-    """
-    Semijoin `df_or_series` by index `other`
+    """Semijoin ``data`` by index ``other``.
 
     Parameters
-    ----------
-    df_or_series : DataFrame or Series
-        data to be filtered
+    ----------\
+    {frame_or_series}
     other : Index
-        other index to join with
-    how : {'left', 'right', 'inner', 'outer'}
+        Other index to join with
+    how : {{'left', 'right', 'inner', 'outer'}}
         Join method to use
     level : None or str or int or
-        single level on which to join, if not given join on all
+        Single level on which to join, if not given join on all
     sort : bool, optional
-        whether to sort the index
-    axis : {0, 1}
+        Whether to sort the index
+    axis : {{0, 1, "index", "columns"}}
         Axis on which to join
 
     Returns
     -------
     DataFrame or Series
 
     Raises
     ------
     TypeError
         If axis is not 0 or 1, or
-        if df_or_series does not derive from DataFrame or Series
+        if frame_or_series does not derive from DataFrame or Series
 
     See also
     --------
     pandas.Index.join
     """
 
-    axes = df_or_series.axes
+    if isinstance(axis, str):
+        if axis == "index":
+            axis = 0
+        elif axis == "columns":
+            axis = 1
+        else:
+            raise ValueError(
+                f"axis can only be one of 0, 1, 'index' or 'columns', not: {axis}"
+            )
+
+    axes = frame_or_series.axes
     index = axes[axis]
     if level is None:
         index = ensure_multiindex(index)
         other = ensure_multiindex(other)
 
     new_index, left_idx, _ = index.join(
         other, how=how, level=level, return_indexers=True, sort=sort
     )
 
-    cls = df_or_series.__class__
+    cls = frame_or_series.__class__
     axes[axis] = new_index
 
     if left_idx is None:
-        return cls(df_or_series.values, *axes).__finalize__(df_or_series)
+        return cls(frame_or_series.values, *axes).__finalize__(frame_or_series)
 
-    if isinstance(df_or_series, DataFrame):
+    if isinstance(frame_or_series, DataFrame):
         if axis == 0:
             data = np.where(
-                left_idx[:, np.newaxis] != -1, df_or_series.values[left_idx, :], np.nan
+                left_idx[:, np.newaxis] != -1,
+                frame_or_series.values[left_idx, :],
+                np.nan,
             )
         elif axis == 1:
-            data = np.where(left_idx != -1, df_or_series.values[:, left_idx], np.nan)
-    elif isinstance(df_or_series, Series):
-        data = np.where(left_idx != -1, df_or_series.values[left_idx], np.nan)
+            data = np.where(left_idx != -1, frame_or_series.values[:, left_idx], np.nan)
+    elif isinstance(frame_or_series, Series):
+        data = np.where(left_idx != -1, frame_or_series.values[left_idx], np.nan)
     else:
         raise TypeError(
-            f"df_or_series must derive from DataFrame or Series, but is {type(df_or_series)}"
+            f"frame_or_series must derive from DataFrame or Series, but is {type(frame_or_series)}"
+        )
+
+    return cls(data, *axes).__finalize__(frame_or_series)
+
+
+def _extractlevel(
+    index: Index, drop: bool = False, **templates: str
+) -> Tuple[Index, list[str]]:
+    index = ensure_multiindex(index)
+    all_identifiers = set()
+
+    for dim, template in templates.items():
+        identifiers = re.findall(r"\{([a-zA-Z_]+)\}", template)
+        all_identifiers.update(identifiers)
+        if dim not in index.names:
+            raise ValueError(f"{dim} not a dimension of index: {index.names}")
+
+        levelnum = index.names.index(dim)
+        labels = index.levels[levelnum]
+        codes = index.codes[levelnum]
+
+        regex_pattern = reduce(
+            lambda s, ident: s.replace(rf"\{{{ident}\}}", rf"(?P<{ident}>.*?)"),
+            identifiers,
+            re.escape(template),
+        )
+        components = labels.str.extract(f"^{regex_pattern}$", expand=True)
+
+        index = assignlevel(
+            index, **{ident: components[ident].values[codes] for ident in identifiers}
         )
 
-    return cls(data, *axes).__finalize__(df_or_series)
+    if drop:
+        index = index.droplevel(list(set(templates) - all_identifiers))
+
+    return index, list(all_identifiers)
+
+
+@doc(
+    index_or_data="""
+    index_or_data : DataFrame, Series or Index
+        Data to modify\
+    """
+)
+def extractlevel(
+    index_or_data: T,
+    drop: bool = False,
+    dropna: bool = True,
+    axis: Axis = 0,
+    **templates: str,
+) -> T:
+    """Split an index ``dim`` ension into multiple ones based on a
+    ``template``.
+
+    Parameters
+    ----------\
+    {index_or_data}
+    drop : bool, default False
+        Whether to keep the split dimension
+    dropna : bool, default True
+        Whether to drop the non-matching levels
+    axis : {{0, 1, "index", "columns"}}, default 0
+        Axis of DataFrame to extract from
+    **templates : str
+        Templates for splitting one or multiple levels
+
+    Returns
+    -------
+    Index, Series or DataFrame
+
+    Raises
+    ------
+    ValueError
+        If ``dim`` is not a dimension of ``index_or_series``
+    """
+    if isinstance(index_or_data, Index):
+        index_or_data, identifiers = _extractlevel(index_or_data, drop, **templates)
+    else:
+        index, identifiers = _extractlevel(
+            get_axis(index_or_data, axis), drop, **templates
+        )
+        index_or_data = index_or_data.set_axis(index, axis=axis)
+
+    if dropna:
+        index_or_data = dropnalevel(index_or_data, subset=identifiers, axis=axis)
+
+    return index_or_data
+
+
+def _formatlevel(index: Index, drop: bool = False, **templates: str) -> Index:
+    levels = {}
+    used_levels = set()
+    for dim, template in templates.items():
+        # Build string
+        string = ""
+        prev_end = 0
+        for m in re.finditer(r"\{([a-zA-Z_]+)\}", template):
+            level = m.group(1)
+            start, end = m.span()
+            string += template[prev_end:start] + projectlevel(index, level).astype(str)
+            prev_end = end
+            used_levels.add(level)
+        string += template[prev_end:]
+
+        levels[dim] = string
+
+    if drop:
+        used_levels.difference_update(templates)
+        if used_levels:
+            index = index.droplevel(list(used_levels))
+
+    return assignlevel(index, **levels)
+
+
+@doc(
+    index_or_data="""
+    index_or_data : DataFrame, Series or Index
+        Data to modify\
+    """
+)
+def formatlevel(
+    index_or_data: T,
+    drop: bool = False,
+    axis: Axis = 0,
+    **templates: str,
+) -> T:
+    """Format index levels based on a ``template`` which can refer to other
+    levels.
+
+    Parameters
+    ----------\
+    {index_or_data}
+    drop : bool, default False
+        Whether to drop the used index levels
+    axis : {{0, 1, "index", "columns"}}, default 0
+        Axis of DataFrame to modify
+    **templates : str
+        Format templates for one or multiple levels
+
+    Returns
+    -------
+    Index, Series or DataFrame
+
+    Raises
+    ------
+    ValueError
+        If ``templates`` refer to non-existant levels
+    """
+    if isinstance(index_or_data, Index):
+        return _formatlevel(index_or_data, drop, **templates)
+
+    index = get_axis(index_or_data, axis)
+    return index_or_data.set_axis(_formatlevel(index, drop, **templates), axis=axis)
```

### Comparing `pandas-indexing-0.2.4/src/pandas_indexing/datasets/__init__.py` & `pandas-indexing-0.2.5/src/pandas_indexing/datasets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 from importlib.resources import open_text
 
 import pandas as pd
 
 
 def remindhighre_power():
-    """
-    Reads IAMC power sector data from REMIND's HighRE IMP scenario for AR6.
+    """Read IAMC power sector data from REMIND's HighRE IMP scenario for AR6.
 
     Returns
     -------
     pd.DataFrame
         Time-series like power sector data
 
     .. [1] Luderer, G., Madeddu, S., Merfort, L. et al. Impact of declining renewable
```

### Comparing `pandas-indexing-0.2.4/src/pandas_indexing/datasets/remindhighre_power.csv` & `pandas-indexing-0.2.5/src/pandas_indexing/datasets/remindhighre_power.csv`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.4/src/pandas_indexing/selectors.py` & `pandas-indexing-0.2.5/src/pandas_indexing/selectors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Selectors improve .loc[] indexing for multi-index pandas data.
+Selectors improve ``.loc[]`` indexing for multi-index pandas data.
 """
 
 from functools import reduce
 from operator import and_
 from typing import Any, Mapping, Optional, Union
 
 import numpy as np
@@ -87,32 +87,31 @@
         tests = (index.isin(np.atleast_1d(v), level=k) for k, v in filters.items())
         return reduce(and_, tests)
 
 
 def isin(
     df: Optional[Data] = None, ignore_missing_levels: bool = False, **filters: Any
 ) -> Union[Isin, Series]:
-    """
-    Constructs a MultiIndex selector.
+    """Constructs a MultiIndex selector.
 
     Arguments
     ---------
     df : Data, optional
-        Data on which to match, if missing an Isin object is returned
+        Data on which to match, if missing an ``Isin`` object is returned
     ignore_missing_levels : bool, default False
         If set, levels missing in data index will be ignored
     **filters
-        Filter to apply on given levels (lists are `or`ed, levels are `and`ed)
+        Filter to apply on given levels (lists are ``or`` ed, levels are ``and`` ed)
 
     Returns
     -------
     Isin or Series
 
-    Usage
-    -----
+    Example
+    -------
     >>> df.loc[isin(region="World", gas=["CO2", "N2O"])]
 
     or with explicit df to get a boolean mask
 
     >>> isin(df, region="World", gas=["CO2", "N2O"])
     """
 
@@ -172,38 +171,37 @@
 def ismatch(
     df: Union[None, Index, DataFrame, Series, str] = None,
     singlefilter: Optional[str] = None,
     regex: bool = False,
     ignore_missing_levels: bool = False,
     **filters,
 ) -> Union[Ismatch, Series]:
-    """
-    Constructs an Index or MultiIndex selector based on pattern matching.
+    """Constructs an Index or MultiIndex selector based on pattern matching.
 
     Arguments
     ---------
     df : Data, optional
-        Data on which to match, if missing an Isin object is returned.
+        Data on which to match, if missing an ``Isin`` object is returned.
     singlefilter : str, optional
-        Filter to apply on a non-multiindex index (can also be handed into the `df`
+        Filter to apply on a non-multiindex index (can also be handed into the ``df``
         argument)
     regex : bool, default False
         If set, filters are interpreted as plain regex strings, otherwise (by default) a
         glob-like syntax is used
     ignore_missing_levels : bool, default False
         If set, levels missing in data index will be ignored
     **filters
-        Filter to apply on given levels (lists are `or`ed, levels are `and`ed)
+        Filter to apply on given levels (lists are ``or`` ed, levels are ``and`` ed)
 
     Returns
     -------
     Isin or Series
 
-    Usage
-    -----
+    Example
+    -------
     for a multiindex:
 
     >>> df.loc[ismatch(variable="Emissions|*|Fossil Fuel and Industry")]
 
     for a single index:
 
     >>> df.loc[ismatch("*bla*")]
```

### Comparing `pandas-indexing-0.2.4/src/pandas_indexing.egg-info/PKG-INFO` & `pandas-indexing-0.2.5/src/pandas_indexing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.4
+Version: 0.2.5
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
```

### Comparing `pandas-indexing-0.2.4/src/pandas_indexing.egg-info/SOURCES.txt` & `pandas-indexing-0.2.5/src/pandas_indexing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

