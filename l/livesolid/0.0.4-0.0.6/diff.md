# Comparing `tmp/livesolid-0.0.4.tar.gz` & `tmp/livesolid-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livesolid-0.0.4.tar", last modified: Mon May  1 05:18:48 2023, max compression
+gzip compressed data, was "livesolid-0.0.6.tar", last modified: Mon May  8 22:05:28 2023, max compression
```

## Comparing `livesolid-0.0.4.tar` & `livesolid-0.0.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-01 05:18:48.629975 livesolid-0.0.4/
--rw-r--r--   0 mtm        (501) staff       (20)      592 2023-04-28 13:28:55.000000 livesolid-0.0.4/.coveragerc
--rw-r--r--   0 mtm        (501) staff       (20)      566 2023-04-28 13:28:55.000000 livesolid-0.0.4/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       57 2023-04-28 13:28:55.000000 livesolid-0.0.4/.isort.cfg
--rw-r--r--   0 mtm        (501) staff       (20)     1670 2023-04-28 14:23:15.000000 livesolid-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 mtm        (501) staff       (20)      530 2023-04-28 13:28:55.000000 livesolid-0.0.4/.readthedocs.yml
--rw-r--r--   0 mtm        (501) staff       (20)       87 2023-04-28 13:28:55.000000 livesolid-0.0.4/AUTHORS.rst
--rw-r--r--   0 mtm        (501) staff       (20)      128 2023-04-28 13:28:55.000000 livesolid-0.0.4/CHANGELOG.rst
--rw-r--r--   0 mtm        (501) staff       (20)    13840 2023-04-28 13:28:55.000000 livesolid-0.0.4/CONTRIBUTING.rst
--rw-r--r--   0 mtm        (501) staff       (20)     1083 2023-04-28 13:28:55.000000 livesolid-0.0.4/LICENSE.txt
--rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-05-01 05:18:48.630146 livesolid-0.0.4/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)     2084 2023-04-28 13:28:55.000000 livesolid-0.0.4/README.rst
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-01 05:18:48.621644 livesolid-0.0.4/docs/
--rw-r--r--   0 mtm        (501) staff       (20)     1154 2023-04-28 13:28:55.000000 livesolid-0.0.4/docs/Makefile
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-01 05:18:48.622227 livesolid-0.0.4/docs/_static/
--rw-r--r--   0 mtm        (501) staff       (20)       18 2023-04-28 13:28:55.000000 livesolid-0.0.4/docs/_static/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       41 2023-04-28 13:28:55.000000 livesolid-0.0.4/docs/authors.rst
--rw-r--r--   0 mtm        (501) staff       (20)       43 2023-04-28 13:28:55.000000 livesolid-0.0.4/docs/changelog.rst
--rw-r--r--   0 mtm        (501) staff       (20)     9742 2023-04-28 13:36:58.000000 livesolid-0.0.4/docs/conf.py
--rw-r--r--   0 mtm        (501) staff       (20)       33 2023-04-28 13:28:55.000000 livesolid-0.0.4/docs/contributing.rst
--rw-r--r--   0 mtm        (501) staff       (20)     2321 2023-04-28 13:28:55.000000 livesolid-0.0.4/docs/index.rst
--rw-r--r--   0 mtm        (501) staff       (20)       67 2023-04-28 13:28:55.000000 livesolid-0.0.4/docs/license.rst
--rw-r--r--   0 mtm        (501) staff       (20)       39 2023-04-28 13:28:55.000000 livesolid-0.0.4/docs/readme.rst
--rw-r--r--   0 mtm        (501) staff       (20)      233 2023-04-28 13:28:55.000000 livesolid-0.0.4/docs/requirements.txt
--rw-r--r--   0 mtm        (501) staff       (20)      346 2023-04-28 13:28:55.000000 livesolid-0.0.4/pyproject.toml
--rw-r--r--   0 mtm        (501) staff       (20)     1253 2023-05-01 05:18:48.631064 livesolid-0.0.4/setup.cfg
--rw-r--r--   0 mtm        (501) staff       (20)      704 2023-04-28 13:28:55.000000 livesolid-0.0.4/setup.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-01 05:18:48.608466 livesolid-0.0.4/src/
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-01 05:18:48.623953 livesolid-0.0.4/src/livesolid/
--rw-r--r--   0 mtm        (501) staff       (20)      577 2023-04-28 13:28:55.000000 livesolid-0.0.4/src/livesolid/__init__.py
--rw-r--r--   0 mtm        (501) staff       (20)      779 2023-04-28 14:23:22.000000 livesolid-0.0.4/src/livesolid/lib.py
--rw-r--r--   0 mtm        (501) staff       (20)     2881 2023-04-28 14:28:31.000000 livesolid-0.0.4/src/livesolid/main.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-01 05:18:48.628296 livesolid-0.0.4/src/livesolid/templates/
--rw-r--r--   0 mtm        (501) staff       (20)      398 2023-05-01 05:17:18.000000 livesolid-0.0.4/src/livesolid/templates/Makefile.j2
--rw-r--r--   0 mtm        (501) staff       (20)     1184 2023-04-28 14:17:25.000000 livesolid-0.0.4/src/livesolid/templates/goreleaser.yaml.j2
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-01 05:18:48.627526 livesolid-0.0.4/src/livesolid.egg-info/
--rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-05-01 05:18:48.000000 livesolid-0.0.4/src/livesolid.egg-info/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)      810 2023-05-01 05:18:48.000000 livesolid-0.0.4/src/livesolid.egg-info/SOURCES.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-01 05:18:48.000000 livesolid-0.0.4/src/livesolid.egg-info/dependency_links.txt
--rw-r--r--   0 mtm        (501) staff       (20)       49 2023-05-01 05:18:48.000000 livesolid-0.0.4/src/livesolid.egg-info/entry_points.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-01 05:18:48.000000 livesolid-0.0.4/src/livesolid.egg-info/not-zip-safe
--rw-r--r--   0 mtm        (501) staff       (20)       93 2023-05-01 05:18:48.000000 livesolid-0.0.4/src/livesolid.egg-info/requires.txt
--rw-r--r--   0 mtm        (501) staff       (20)       10 2023-05-01 05:18:48.000000 livesolid-0.0.4/src/livesolid.egg-info/top_level.txt
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-01 05:18:48.629572 livesolid-0.0.4/tests/
--rw-r--r--   0 mtm        (501) staff       (20)      277 2023-04-28 13:28:55.000000 livesolid-0.0.4/tests/conftest.py
--rw-r--r--   0 mtm        (501) staff       (20)      594 2023-04-28 13:28:55.000000 livesolid-0.0.4/tests/test_skeleton.py
--rw-r--r--   0 mtm        (501) staff       (20)     2851 2023-04-28 13:28:55.000000 livesolid-0.0.4/tox.ini
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-08 22:05:28.418765 livesolid-0.0.6/
+-rw-r--r--   0 mtm        (501) staff       (20)      592 2023-04-28 13:28:55.000000 livesolid-0.0.6/.coveragerc
+-rw-r--r--   0 mtm        (501) staff       (20)      566 2023-04-28 13:28:55.000000 livesolid-0.0.6/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       57 2023-04-28 13:28:55.000000 livesolid-0.0.6/.isort.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)     1670 2023-04-28 14:23:15.000000 livesolid-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 mtm        (501) staff       (20)      530 2023-04-28 13:28:55.000000 livesolid-0.0.6/.readthedocs.yml
+-rw-r--r--   0 mtm        (501) staff       (20)       87 2023-04-28 13:28:55.000000 livesolid-0.0.6/AUTHORS.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      128 2023-04-28 13:28:55.000000 livesolid-0.0.6/CHANGELOG.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    13840 2023-04-28 13:28:55.000000 livesolid-0.0.6/CONTRIBUTING.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     1083 2023-04-28 13:28:55.000000 livesolid-0.0.6/LICENSE.txt
+-rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-05-08 22:05:28.418930 livesolid-0.0.6/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)     2084 2023-04-28 13:28:55.000000 livesolid-0.0.6/README.rst
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-08 22:05:28.410995 livesolid-0.0.6/docs/
+-rw-r--r--   0 mtm        (501) staff       (20)     1154 2023-04-28 13:28:55.000000 livesolid-0.0.6/docs/Makefile
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-08 22:05:28.411571 livesolid-0.0.6/docs/_static/
+-rw-r--r--   0 mtm        (501) staff       (20)       18 2023-04-28 13:28:55.000000 livesolid-0.0.6/docs/_static/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       41 2023-04-28 13:28:55.000000 livesolid-0.0.6/docs/authors.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       43 2023-04-28 13:28:55.000000 livesolid-0.0.6/docs/changelog.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     9742 2023-04-28 13:36:58.000000 livesolid-0.0.6/docs/conf.py
+-rw-r--r--   0 mtm        (501) staff       (20)       33 2023-04-28 13:28:55.000000 livesolid-0.0.6/docs/contributing.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     2321 2023-04-28 13:28:55.000000 livesolid-0.0.6/docs/index.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       67 2023-04-28 13:28:55.000000 livesolid-0.0.6/docs/license.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       39 2023-04-28 13:28:55.000000 livesolid-0.0.6/docs/readme.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      233 2023-04-28 13:28:55.000000 livesolid-0.0.6/docs/requirements.txt
+-rw-r--r--   0 mtm        (501) staff       (20)      346 2023-04-28 13:28:55.000000 livesolid-0.0.6/pyproject.toml
+-rw-r--r--   0 mtm        (501) staff       (20)     1253 2023-05-08 22:05:28.419804 livesolid-0.0.6/setup.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)      704 2023-04-28 13:28:55.000000 livesolid-0.0.6/setup.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-08 22:05:28.397179 livesolid-0.0.6/src/
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-08 22:05:28.413446 livesolid-0.0.6/src/livesolid/
+-rw-r--r--   0 mtm        (501) staff       (20)      577 2023-04-28 13:28:55.000000 livesolid-0.0.6/src/livesolid/__init__.py
+-rw-r--r--   0 mtm        (501) staff       (20)      779 2023-04-28 14:23:22.000000 livesolid-0.0.6/src/livesolid/lib.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2881 2023-04-28 14:28:31.000000 livesolid-0.0.6/src/livesolid/main.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-08 22:05:28.417359 livesolid-0.0.6/src/livesolid/templates/
+-rw-r--r--   0 mtm        (501) staff       (20)      420 2023-05-08 19:14:32.000000 livesolid-0.0.6/src/livesolid/templates/Makefile.j2
+-rw-r--r--   0 mtm        (501) staff       (20)     1184 2023-04-28 14:17:25.000000 livesolid-0.0.6/src/livesolid/templates/goreleaser.yaml.j2
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-08 22:05:28.416438 livesolid-0.0.6/src/livesolid.egg-info/
+-rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-05-08 22:05:28.000000 livesolid-0.0.6/src/livesolid.egg-info/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)      810 2023-05-08 22:05:28.000000 livesolid-0.0.6/src/livesolid.egg-info/SOURCES.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-08 22:05:28.000000 livesolid-0.0.6/src/livesolid.egg-info/dependency_links.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       49 2023-05-08 22:05:28.000000 livesolid-0.0.6/src/livesolid.egg-info/entry_points.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-08 22:05:27.000000 livesolid-0.0.6/src/livesolid.egg-info/not-zip-safe
+-rw-r--r--   0 mtm        (501) staff       (20)       93 2023-05-08 22:05:28.000000 livesolid-0.0.6/src/livesolid.egg-info/requires.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       10 2023-05-08 22:05:28.000000 livesolid-0.0.6/src/livesolid.egg-info/top_level.txt
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-08 22:05:28.418353 livesolid-0.0.6/tests/
+-rw-r--r--   0 mtm        (501) staff       (20)      277 2023-04-28 13:28:55.000000 livesolid-0.0.6/tests/conftest.py
+-rw-r--r--   0 mtm        (501) staff       (20)      594 2023-04-28 13:28:55.000000 livesolid-0.0.6/tests/test_skeleton.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2851 2023-04-28 13:28:55.000000 livesolid-0.0.6/tox.ini
```

### Comparing `livesolid-0.0.4/.coveragerc` & `livesolid-0.0.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/.gitignore` & `livesolid-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/.pre-commit-config.yaml` & `livesolid-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/.readthedocs.yml` & `livesolid-0.0.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/CONTRIBUTING.rst` & `livesolid-0.0.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/LICENSE.txt` & `livesolid-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/PKG-INFO` & `livesolid-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livesolid
-Version: 0.0.4
+Version: 0.0.6
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `livesolid-0.0.4/README.rst` & `livesolid-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/docs/Makefile` & `livesolid-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/docs/conf.py` & `livesolid-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/docs/index.rst` & `livesolid-0.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/setup.cfg` & `livesolid-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/setup.py` & `livesolid-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/src/livesolid/__init__.py` & `livesolid-0.0.6/src/livesolid/__init__.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/src/livesolid/lib.py` & `livesolid-0.0.6/src/livesolid/lib.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/src/livesolid/main.py` & `livesolid-0.0.6/src/livesolid/main.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/src/livesolid/templates/goreleaser.yaml.j2` & `livesolid-0.0.6/src/livesolid/templates/goreleaser.yaml.j2`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/src/livesolid.egg-info/PKG-INFO` & `livesolid-0.0.6/src/livesolid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livesolid
-Version: 0.0.4
+Version: 0.0.6
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `livesolid-0.0.4/src/livesolid.egg-info/SOURCES.txt` & `livesolid-0.0.6/src/livesolid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/tests/test_skeleton.py` & `livesolid-0.0.6/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.4/tox.ini` & `livesolid-0.0.6/tox.ini`

 * *Files identical despite different names*

