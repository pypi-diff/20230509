# Comparing `tmp/cognite_power_ops-0.1.0.tar.gz` & `tmp/cognite_power_ops-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_power_ops-0.1.0.tar", max compression
+gzip compressed data, was "cognite_power_ops-0.2.0.tar", max compression
```

## Comparing `cognite_power_ops-0.1.0.tar` & `cognite_power_ops-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,36 @@
--rw-r--r--   0        0        0    10758 2023-05-03 06:52:34.424089 cognite_power_ops-0.1.0/LICENSE
--rw-r--r--   0        0        0       76 2023-05-03 06:52:34.424089 cognite_power_ops-0.1.0/cognite/powerops/__init__.py
--rw-r--r--   0        0        0       22 2023-05-03 06:52:34.424089 cognite_power_ops-0.1.0/cognite/powerops/version.py
--rw-r--r--   0        0        0      873 2023-05-03 06:52:34.428089 cognite_power_ops-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 cognite_power_ops-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-05-09 07:14:44.989373 cognite_power_ops-0.2.0/LICENSE
+-rw-r--r--   0        0        0       76 2023-05-09 07:14:44.989373 cognite_power_ops-0.2.0/cognite/powerops/__init__.py
+-rw-r--r--   0        0        0    10260 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/bootstrap.py
+-rw-r--r--   0        0        0    24685 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/config.py
+-rw-r--r--   0        0        0        0 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/__init__.py
+-rw-r--r--   0        0        0     2686 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/benchmarking_config.py
+-rw-r--r--   0        0        0     2984 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/bid_matrix_generator_config.py
+-rw-r--r--   0        0        0    13238 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/cdf_resource_collection.py
+-rw-r--r--   0        0        0     2513 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/common.py
+-rw-r--r--   0        0        0     1390 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/market_config.py
+-rw-r--r--   0        0        0    16603 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/plant.py
+-rw-r--r--   0        0        0     5114 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/reserve_scenario.py
+-rw-r--r--   0        0        0     1218 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/rkom_bid_combination_config.py
+-rw-r--r--   0        0        0      994 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/rkom_market_config.py
+-rw-r--r--   0        0        0     2113 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/shop_file_config.py
+-rw-r--r--   0        0        0     2815 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/shop_output_definition.py
+-rw-r--r--   0        0        0     9189 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/time_series_mapping.py
+-rw-r--r--   0        0        0     1144 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/transformation.py
+-rw-r--r--   0        0        0     1042 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/logger.py
+-rw-r--r--   0        0        0     2070 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/main.py
+-rw-r--r--   0        0        0        0 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/__init__.py
+-rw-r--r--   0        0        0     1936 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/asset_types.py
+-rw-r--r--   0        0        0     1424 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/cdf_auth.py
+-rw-r--r--   0        0        0     2724 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/cdf_utils.py
+-rw-r--r--   0        0        0      744 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/common.py
+-rw-r--r--   0        0        0      324 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/constants.py
+-rw-r--r--   0        0        0     3271 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/files.py
+-rw-r--r--   0        0        0     4979 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/labels.py
+-rw-r--r--   0        0        0     3165 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/powerops_asset_hierarchy.py
+-rw-r--r--   0        0        0      718 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/powerops_status_events.py
+-rw-r--r--   0        0        0     4495 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/relationship_types.py
+-rw-r--r--   0        0        0    11602 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/resource_generation.py
+-rw-r--r--   0        0        0     1495 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/serializer.py
+-rw-r--r--   0        0        0       22 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/version.py
+-rw-r--r--   0        0        0     1330 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 cognite_power_ops-0.2.0/PKG-INFO
```

### Comparing `cognite_power_ops-0.1.0/LICENSE` & `cognite_power_ops-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.1.0/pyproject.toml` & `cognite_power_ops-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-power-ops"
-version = "0.1.0"
+version = "0.2.0"
 description = "SDK for power markets operations on Cognite Data Fusion"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache 2.0"
 packages = [{include = "cognite", from = "."}]
 
 [tool.black]
 line-length = 120
@@ -19,17 +19,37 @@
 
 [tool.ruff]
 line-length = 120
 target-version = 'py39'
 
 [tool.poetry.dependencies]
 python = "^3.9"
+typer = "^0.9.0"
+PyYAML = "^6.0"
+arrow = "^1.2.2"
+cognite-sdk = {version = "^5.9.0", extras = ["pandas"]}
+msal = "^1.16.0"
+pydantic = "^1.9.0"
+numpy = "^1.23.2"
+strawberry-graphql = "^0.156.4"
+docopt = "^0.6.2"
+cachelib = "^0.10.2"
+retry = "^0.9.2"
+loguru = "^0.6.0"
+deepdiff = "^6.3.0"
+cognite-gql-pygen = "0.4.0"
+
+[tool.poetry.scripts]
+powerops = "cognite.powerops.main:main"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
+pytest-regressions = "^2.4.2"
 pre-commit = "^3.2.2"
 twine = "^4.0.2"
 pytest-cov = "^4.0.0"
+profilehooks = "^1.12.0"
+pytest-mock = "^3.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

