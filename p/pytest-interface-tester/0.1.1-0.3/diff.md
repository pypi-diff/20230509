# Comparing `tmp/pytest-interface-tester-0.1.1.tar.gz` & `tmp/pytest-interface-tester-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-interface-tester-0.1.1.tar", last modified: Mon May  1 15:01:12 2023, max compression
+gzip compressed data, was "pytest-interface-tester-0.3.tar", last modified: Tue May  9 13:54:53 2023, max compression
```

## Comparing `pytest-interface-tester-0.1.1.tar` & `pytest-interface-tester-0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.498055 pytest-interface-tester-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.494055 pytest-interface-tester-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.494055 pytest-interface-tester-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/.github/workflows/build_wheels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/.github/workflows/quality_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-01 15:01:12.498055 pytest-interface-tester-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.498055 pytest-interface-tester-0.1.1/interface_tester/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.498055 pytest-interface-tester-0.1.1/interface_tester/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/cli/discover.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/interface_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/interface_tester/schema_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.498055 pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-01 15:01:12.000000 pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-01 15:01:12.000000 pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:01:12.000000 pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-01 15:01:12.000000 pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-01 15:01:12.000000 pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 15:01:12.000000 pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:01:12.498055 pytest-interface-tester-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.494055 pytest-interface-tester-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:01:12.498055 pytest-interface-tester-0.1.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/tests/unit/test_collect_interface_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/tests/unit/test_collect_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-01 15:00:57.000000 pytest-interface-tester-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:54:53.955825 pytest-interface-tester-0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:54:53.951825 pytest-interface-tester-0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:54:53.951825 pytest-interface-tester-0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/.github/workflows/build_wheels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/.github/workflows/quality_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-09 13:54:53.951825 pytest-interface-tester-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:54:53.951825 pytest-interface-tester-0.3/interface_tester/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/interface_tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:54:53.951825 pytest-interface-tester-0.3/interface_tester/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/interface_tester/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/interface_tester/cli/discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/interface_tester/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/interface_tester/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/interface_tester/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/interface_tester/interface_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/interface_tester/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/interface_tester/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/interface_tester/schema_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:54:53.951825 pytest-interface-tester-0.3/pytest_interface_tester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-09 13:54:53.000000 pytest-interface-tester-0.3/pytest_interface_tester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-09 13:54:53.000000 pytest-interface-tester-0.3/pytest_interface_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:54:53.000000 pytest-interface-tester-0.3/pytest_interface_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-09 13:54:53.000000 pytest-interface-tester-0.3/pytest_interface_tester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 13:54:53.000000 pytest-interface-tester-0.3/pytest_interface_tester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-09 13:54:53.000000 pytest-interface-tester-0.3/pytest_interface_tester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:54:53.955825 pytest-interface-tester-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:54:53.951825 pytest-interface-tester-0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:54:53.951825 pytest-interface-tester-0.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/tests/unit/test_collect_interface_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/tests/unit/test_collect_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-09 13:54:44.000000 pytest-interface-tester-0.3/tox.ini
```

### Comparing `pytest-interface-tester-0.1.1/.github/workflows/build_wheels.yaml` & `pytest-interface-tester-0.3/.github/workflows/build_wheels.yaml`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1.1/.github/workflows/quality_checks.yaml` & `pytest-interface-tester-0.3/.github/workflows/quality_checks.yaml`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1.1/PKG-INFO` & `pytest-interface-tester-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-interface-tester
-Version: 0.1.1
+Version: 0.3
 Summary: Pytest plugin for checking charm relation interface protocol compliance.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/canonical/interface-tester-pytest
 Keywords: juju,relation interfaces
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
@@ -32,15 +32,15 @@
 - The maintainers of the spec repo want to be able to automatically verify if all the registered charms that claim to implement a relation interface do in fact comply with its specification.
 - The maintainers of the charm repo want to be able to automatically verify that their implementation of the standardized relation interfaces are in fact compliant.
 
 The interface tester package facilitates both these verification flows.
 
 # How to use the interface_tester in the spec repo
 
-Follow the instructions [here](https://github.com/canonical/charm-relation-interfaces/README_INTERFACE_TESTS.md).
+Follow the instructions [here](https://github.com/canonical/charm-relation-interfaces/blob/main/README_INTERFACE_TESTS.md).
 
 # How to use the interface_tester in the charm repo
 
 1) Ensure that [charm-relation-interfaces](https://github.com/canonical/charm-relation-interfaces) has one or more interface tests and a schema for the interface you want to test. If that is not the case, ask the maintainers of the interface (or its 'official' implementation) to add some.
 2) Install this package.
 3) Add a `...charm-root/tests/interface_tests/conftest.py` file containing at least:
    ```python
```

### Comparing `pytest-interface-tester-0.1.1/README.md` & `pytest-interface-tester-0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - The maintainers of the spec repo want to be able to automatically verify if all the registered charms that claim to implement a relation interface do in fact comply with its specification.
 - The maintainers of the charm repo want to be able to automatically verify that their implementation of the standardized relation interfaces are in fact compliant.
 
 The interface tester package facilitates both these verification flows.
 
 # How to use the interface_tester in the spec repo
 
-Follow the instructions [here](https://github.com/canonical/charm-relation-interfaces/README_INTERFACE_TESTS.md).
+Follow the instructions [here](https://github.com/canonical/charm-relation-interfaces/blob/main/README_INTERFACE_TESTS.md).
 
 # How to use the interface_tester in the charm repo
 
 1) Ensure that [charm-relation-interfaces](https://github.com/canonical/charm-relation-interfaces) has one or more interface tests and a schema for the interface you want to test. If that is not the case, ask the maintainers of the interface (or its 'official' implementation) to add some.
 2) Install this package.
 3) Add a `...charm-root/tests/interface_tests/conftest.py` file containing at least:
    ```python
```

### Comparing `pytest-interface-tester-0.1.1/interface_tester/cli/discover.py` & `pytest-interface-tester-0.3/interface_tester/cli/discover.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1.1/interface_tester/collector.py` & `pytest-interface-tester-0.3/interface_tester/collector.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1.1/interface_tester/errors.py` & `pytest-interface-tester-0.3/interface_tester/errors.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1.1/interface_tester/interface_test.py` & `pytest-interface-tester-0.3/interface_tester/interface_test.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1.1/interface_tester/plugin.py` & `pytest-interface-tester-0.3/interface_tester/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1.1/interface_tester/runner.py` & `pytest-interface-tester-0.3/interface_tester/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import typing
 from typing import Dict, List, Optional, Type
 
 from ops.charm import CharmBase
-from scenario import Event, Relation, State
+from scenario import Event, Relation, State, trigger
 
 from .errors import InvalidTestCaseError
 from .interface_test import SchemaConfig, logger
 from .schema_base import DataBagSchema
 
 if typing.TYPE_CHECKING:
     from .interface_test import _InterfaceTestCase
 
 
 def _assert_case_plays(
     event: Event, state: State, charm_type: Type["CharmBase"], meta, actions, config
 ) -> State:
     try:
-        state_out = state.trigger(
+        state_out = trigger(
+            state,
             event,
             charm_type=charm_type,
             meta=meta,
             actions=actions,
             config=config,
         )
     except Exception as e:
```

### Comparing `pytest-interface-tester-0.1.1/interface_tester/schema_base.py` & `pytest-interface-tester-0.3/interface_tester/schema_base.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1.1/pyproject.toml` & `pytest-interface-tester-0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pytest-interface-tester"
 
-version = "0.1.1"
+version = "0.3"
 authors = [
     { name = "Pietro Pasotti", email = "pietro.pasotti@canonical.com" },
 ]
 description = "Pytest plugin for checking charm relation interface protocol compliance."
 license.text = "Apache-2.0"
 keywords = ["juju", "relation interfaces"]
 
 dependencies = [
-    "pydantic",
-    "typer",
-    "ops-scenario",
+    "pydantic==1.10.7",
+    "typer==0.7.0",
+    "ops-scenario==3.0.1",
     "pytest"
 ]
 
 readme = "README.md"
 requires-python = ">=3.8"
 
 classifiers = [
```

### Comparing `pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/PKG-INFO` & `pytest-interface-tester-0.3/pytest_interface_tester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-interface-tester
-Version: 0.1.1
+Version: 0.3
 Summary: Pytest plugin for checking charm relation interface protocol compliance.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/canonical/interface-tester-pytest
 Keywords: juju,relation interfaces
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
@@ -32,15 +32,15 @@
 - The maintainers of the spec repo want to be able to automatically verify if all the registered charms that claim to implement a relation interface do in fact comply with its specification.
 - The maintainers of the charm repo want to be able to automatically verify that their implementation of the standardized relation interfaces are in fact compliant.
 
 The interface tester package facilitates both these verification flows.
 
 # How to use the interface_tester in the spec repo
 
-Follow the instructions [here](https://github.com/canonical/charm-relation-interfaces/README_INTERFACE_TESTS.md).
+Follow the instructions [here](https://github.com/canonical/charm-relation-interfaces/blob/main/README_INTERFACE_TESTS.md).
 
 # How to use the interface_tester in the charm repo
 
 1) Ensure that [charm-relation-interfaces](https://github.com/canonical/charm-relation-interfaces) has one or more interface tests and a schema for the interface you want to test. If that is not the case, ask the maintainers of the interface (or its 'official' implementation) to add some.
 2) Install this package.
 3) Add a `...charm-root/tests/interface_tests/conftest.py` file containing at least:
    ```python
```

### Comparing `pytest-interface-tester-0.1.1/pytest_interface_tester.egg-info/SOURCES.txt` & `pytest-interface-tester-0.3/pytest_interface_tester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1.1/tests/unit/test_collect_interface_tests.py` & `pytest-interface-tester-0.3/tests/unit/test_collect_interface_tests.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1.1/tests/unit/test_collect_schemas.py` & `pytest-interface-tester-0.3/tests/unit/test_collect_schemas.py`

 * *Files identical despite different names*

### Comparing `pytest-interface-tester-0.1.1/tox.ini` & `pytest-interface-tester-0.3/tox.ini`

 * *Files identical despite different names*

