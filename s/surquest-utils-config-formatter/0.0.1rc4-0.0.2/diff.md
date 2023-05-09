# Comparing `tmp/surquest_utils_config_formatter-0.0.1rc4.tar.gz` & `tmp/surquest_utils_config_formatter-0.0.2.tar.gz`

## Comparing `surquest_utils_config_formatter-0.0.1rc4.tar` & `surquest_utils_config_formatter-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/package.base.dockerfile
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/.github/workflows/release.yml
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/.github/workflows/test.yml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/config/config.cloud.google.env.PROD.json
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/config/config.cloud.google.services.json
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/config/config.solution.json
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/config/naming.patterns.json
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/surquest/utils/config/__init__.py
--rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/surquest/utils/config/formatter.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/test/pytest.ini
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/test/formatter/test_formatter.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/LICENSE
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/README.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/pyproject.toml
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.1rc4/PKG-INFO
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/package.base.dockerfile
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/config/config.cloud.google.env.PROD.json
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/config/config.cloud.google.services.json
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/config/config.solution.json
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/config/naming.patterns.json
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/surquest/utils/config/__init__.py
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/surquest/utils/config/formatter.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/test/pytest.ini
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/test/formatter/test_formatter.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/README.md
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 surquest_utils_config_formatter-0.0.2/PKG-INFO
```

### Comparing `surquest_utils_config_formatter-0.0.1rc4/package.base.dockerfile` & `surquest_utils_config_formatter-0.0.2/package.base.dockerfile`

 * *Files identical despite different names*

### Comparing `surquest_utils_config_formatter-0.0.1rc4/.github/workflows/release.yml` & `surquest_utils_config_formatter-0.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `surquest_utils_config_formatter-0.0.1rc4/.github/workflows/test.yml` & `surquest_utils_config_formatter-0.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `surquest_utils_config_formatter-0.0.1rc4/config/config.cloud.google.services.json` & `surquest_utils_config_formatter-0.0.2/config/config.cloud.google.services.json`

 * *Files identical despite different names*

### Comparing `surquest_utils_config_formatter-0.0.1rc4/surquest/utils/config/formatter.py` & `surquest_utils_config_formatter-0.0.2/surquest/utils/config/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 The pyconfig module contains collection of
 objects (DotDict + Config) which helps you
 to access configurations in JSON files for
 Google Cloud Platform based projects.
 """
 
 import json
+import copy
 import re
 
 
 class DotDict(dict):
     """
     a dictionary that supports dot notation
     as well as dictionary access notation
@@ -126,24 +127,26 @@
         :return: formatted pattern
         :rtype: str
         """
 
         naming_pattern = self._get_config_item(name=pattern)
         naming_pattern = naming_pattern.replace("${", "{")
 
+        config = copy.copy(self.config)
+
         naming_pattern, config = self.change_letter_case(
             naming_pattern=naming_pattern,
-            config=self.config
+            config=config
         )
         naming_pattern, config = self.do_replace(
             naming_pattern=naming_pattern,
             config=config
         )
 
-        return naming_pattern.format(**self.config)
+        return naming_pattern.format(**config)
 
     def _get_config_item(self, name, source="naming_patterns"):
         """Method returns config item by dotted name or list.
 
         :param item: naming pattern name
         :type item: list|str
```

### Comparing `surquest_utils_config_formatter-0.0.1rc4/test/formatter/test_formatter.py` & `surquest_utils_config_formatter-0.0.2/test/formatter/test_formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,18 @@
                 }
             ),
             naming_patterns=Formatter.load_json(
                 path="../config/naming.patterns.json"
             )
         )
 
+        assert "ADM_FX_API_KEY_PROD" == formatter.get(
+            pattern="security.secrets.apiKey",
+        )
+
         assert "adm--exchange-rates--ingress--prod" == formatter.get(
             pattern="storage.buckets.ingress",
         )
 
         assert "adm_exchange_rates_raw" == formatter.get(
             pattern="bigquery.datasets.raw",
         )
```

### Comparing `surquest_utils_config_formatter-0.0.1rc4/.gitignore` & `surquest_utils_config_formatter-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `surquest_utils_config_formatter-0.0.1rc4/LICENSE` & `surquest_utils_config_formatter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `surquest_utils_config_formatter-0.0.1rc4/README.md` & `surquest_utils_config_formatter-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `surquest_utils_config_formatter-0.0.1rc4/pyproject.toml` & `surquest_utils_config_formatter-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "surquest-utils-config-formatter"
-version = "0.0.1rc4"
+version = "0.0.2"
 description = "ConfigFormatter helps you to follow the naming patterns of Google Cloud resources in your Python application."
 authors = [
     {name= "Michal Švarc", email= "michal.svarc@surquest.com"}
 ]
 readme = "README.md"
 dependencies = []
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License"
+]
 [project.optional-dependencies]
 test = [
     "pytest>=7.2.1",
     "pytest-cov>=4.0.0",
 ]
 
 [project.urls]
```

### Comparing `surquest_utils_config_formatter-0.0.1rc4/PKG-INFO` & `surquest_utils_config_formatter-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: surquest-utils-config-formatter
-Version: 0.0.1rc4
+Version: 0.0.2
 Summary: ConfigFormatter helps you to follow the naming patterns of Google Cloud resources in your Python application.
 Project-URL: Homepage, https://github.com/surquest/python-utils-loader
 Project-URL: Bug Tracker, https://github.com/surquest/python-utils-loader/issues
 Author-email: Michal Švarc <michal.svarc@surquest.com>
 License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Provides-Extra: test
 Requires-Dist: pytest-cov>=4.0.0; extra == 'test'
 Requires-Dist: pytest>=7.2.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 ![GitHub](https://img.shields.io/github/license/surquest/python-utils-config-formatter?style=flat-square)
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/surquest/python-utils-config-formatter/test.yml?branch=main&style=flat-square)
```

