# Comparing `tmp/sat-utils-1.1.3.tar.gz` & `tmp/sat-utils-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sat-utils-1.1.3.tar", last modified: Tue May  9 13:35:18 2023, max compression
+gzip compressed data, was "sat-utils-1.1.4.tar", last modified: Tue May  9 13:40:33 2023, max compression
```

## Comparing `sat-utils-1.1.3.tar` & `sat-utils-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       36 2023-05-05 19:40:30.015119 sat-utils-1.1.3/.coveragerc
--rw-r--r--   0        0        0      220 2023-05-04 18:57:03.282604 sat-utils-1.1.3/.editorconfig
--rw-r--r--   0        0        0      522 2023-05-05 13:45:33.481647 sat-utils-1.1.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      799 2023-05-05 13:45:33.481647 sat-utils-1.1.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      507 2023-05-05 19:55:26.778801 sat-utils-1.1.3/.github/workflows/unit-test.yml
--rw-r--r--   0        0        0     3127 2023-05-05 13:59:16.248588 sat-utils-1.1.3/.gitignore
--rw-r--r--   0        0        0      875 2023-05-04 18:57:03.282604 sat-utils-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      452 2023-05-05 19:21:22.269195 sat-utils-1.1.3/Dockerfile
--rw-r--r--   0        0        0     1101 2023-05-05 13:45:33.481647 sat-utils-1.1.3/LICENSE
--rw-r--r--   0        0        0      562 2023-05-09 13:10:43.655515 sat-utils-1.1.3/Makefile
--rw-r--r--   0        0        0     2102 2023-05-05 18:52:51.002148 sat-utils-1.1.3/README.md
--rw-r--r--   0        0        0       24 2023-05-05 19:53:36.881860 sat-utils-1.1.3/bandit.yml
--rw-r--r--   0        0        0     2474 2023-05-05 15:13:27.197689 sat-utils-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      214 2023-05-05 19:48:39.279311 sat-utils-1.1.3/pytest.ini
--rw-r--r--   0        0        0    20604 2023-05-05 14:13:37.388157 sat-utils-1.1.3/requirements/base/base.txt
--rw-r--r--   0        0        0    63054 2023-05-05 14:13:40.956190 sat-utils-1.1.3/requirements/dev/dev.txt
--rw-r--r--   0        0        0       56 2023-05-05 19:40:01.490874 sat-utils-1.1.3/sat/__init__.py
--rw-r--r--   0        0        0     1328 2023-05-05 19:03:13.131659 sat-utils-1.1.3/sat/logs.py
--rw-r--r--   0        0        0     1171 2023-05-05 18:11:06.915108 sat-utils-1.1.3/sat/slack.py
--rw-r--r--   0        0        0        0 2023-05-05 13:45:33.481647 sat-utils-1.1.3/tests/__init__.py
--rw-r--r--   0        0        0      677 2023-05-05 19:50:19.888173 sat-utils-1.1.3/tests/test_logger.py
--rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 sat-utils-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0       36 2023-05-05 19:40:30.015119 sat-utils-1.1.4/.coveragerc
+-rw-r--r--   0        0        0      220 2023-05-04 18:57:03.282604 sat-utils-1.1.4/.editorconfig
+-rw-r--r--   0        0        0      522 2023-05-05 13:45:33.481647 sat-utils-1.1.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      799 2023-05-05 13:45:33.481647 sat-utils-1.1.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      507 2023-05-05 19:55:26.778801 sat-utils-1.1.4/.github/workflows/unit-test.yml
+-rw-r--r--   0        0        0     3127 2023-05-05 13:59:16.248588 sat-utils-1.1.4/.gitignore
+-rw-r--r--   0        0        0      875 2023-05-04 18:57:03.282604 sat-utils-1.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      452 2023-05-05 19:21:22.269195 sat-utils-1.1.4/Dockerfile
+-rw-r--r--   0        0        0     1101 2023-05-05 13:45:33.481647 sat-utils-1.1.4/LICENSE
+-rw-r--r--   0        0        0      562 2023-05-09 13:10:43.655515 sat-utils-1.1.4/Makefile
+-rw-r--r--   0        0        0     2102 2023-05-05 18:52:51.002148 sat-utils-1.1.4/README.md
+-rw-r--r--   0        0        0       24 2023-05-05 19:53:36.881860 sat-utils-1.1.4/bandit.yml
+-rw-r--r--   0        0        0     2317 2023-05-09 13:39:20.757802 sat-utils-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      214 2023-05-05 19:48:39.279311 sat-utils-1.1.4/pytest.ini
+-rw-r--r--   0        0        0    20604 2023-05-05 14:13:37.388157 sat-utils-1.1.4/requirements/base/base.txt
+-rw-r--r--   0        0        0    63054 2023-05-05 14:13:40.956190 sat-utils-1.1.4/requirements/dev/dev.txt
+-rw-r--r--   0        0        0       56 2023-05-05 19:40:01.490874 sat-utils-1.1.4/sat/__init__.py
+-rw-r--r--   0        0        0     1328 2023-05-05 19:03:13.131659 sat-utils-1.1.4/sat/logs.py
+-rw-r--r--   0        0        0     1171 2023-05-05 18:11:06.915108 sat-utils-1.1.4/sat/slack.py
+-rw-r--r--   0        0        0        0 2023-05-05 13:45:33.481647 sat-utils-1.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      677 2023-05-05 19:50:19.888173 sat-utils-1.1.4/tests/test_logger.py
+-rw-r--r--   0        0        0     3318 1970-01-01 00:00:00.000000 sat-utils-1.1.4/PKG-INFO
```

### Comparing `sat-utils-1.1.3/.github/PULL_REQUEST_TEMPLATE.md` & `sat-utils-1.1.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.3/.github/workflows/publish.yml` & `sat-utils-1.1.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.3/.gitignore` & `sat-utils-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.3/.pre-commit-config.yaml` & `sat-utils-1.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.3/LICENSE` & `sat-utils-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.3/Makefile` & `sat-utils-1.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.3/README.md` & `sat-utils-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.3/pyproject.toml` & `sat-utils-1.1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 [build-system]
 requires = ["flit_core>=3.2"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sat-utils"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Ryan Semmler", email="rsemmle@ncsu.edu" },
 ]
 description = "Contains a collection of shared utility functions"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
-  "fastapi>=0.95.1, <1.0.0",
-  "pyjwt>=2.6.0, <3.0.0",
   "slack-sdk>=3.21.0, <4.0.0",
-  "pyodbc>=4.0.39, <5.0.0",
-  "cx-Oracle>=8.3.0, <9.0.0",
-  "mysql-connector-python>=8.0.33, <9.0.0",
   "requests>=2.29.0, <3.0.0",
 ]
 
 [project.optional-dependencies]
 dev = [
   "pytest>=6.2.5, <7.0.0",
   "pytest-mock>=3.10.0, <4.0.0",
```

### Comparing `sat-utils-1.1.3/requirements/base/base.txt` & `sat-utils-1.1.4/requirements/base/base.txt`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.3/requirements/dev/dev.txt` & `sat-utils-1.1.4/requirements/dev/dev.txt`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.3/sat/logs.py` & `sat-utils-1.1.4/sat/logs.py`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.3/sat/slack.py` & `sat-utils-1.1.4/sat/slack.py`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.3/tests/test_logger.py` & `sat-utils-1.1.4/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `sat-utils-1.1.3/PKG-INFO` & `sat-utils-1.1.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
 Name: sat-utils
-Version: 1.1.3
+Version: 1.1.4
 Summary: Contains a collection of shared utility functions
 Author-email: Ryan Semmler <rsemmle@ncsu.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: fastapi>=0.95.1, <1.0.0
-Requires-Dist: pyjwt>=2.6.0, <3.0.0
 Requires-Dist: slack-sdk>=3.21.0, <4.0.0
-Requires-Dist: pyodbc>=4.0.39, <5.0.0
-Requires-Dist: cx-Oracle>=8.3.0, <9.0.0
-Requires-Dist: mysql-connector-python>=8.0.33, <9.0.0
 Requires-Dist: requests>=2.29.0, <3.0.0
 Requires-Dist: pytest>=6.2.5, <7.0.0 ; extra == "dev"
 Requires-Dist: pytest-mock>=3.10.0, <4.0.0 ; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0, <5.0.0 ; extra == "dev"
 Requires-Dist: coverage[toml]>=6.2 ; extra == "dev"
 Requires-Dist: black>=23.3.0, <24.0.0 ; extra == "dev"
 Requires-Dist: mypy>=1.2.0, <2.0.0 ; extra == "dev"
```

