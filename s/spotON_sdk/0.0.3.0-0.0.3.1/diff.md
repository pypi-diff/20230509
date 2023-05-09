# Comparing `tmp/spotON_sdk-0.0.3.0.tar.gz` & `tmp/spotON_sdk-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.3.0.tar", last modified: Tue May  9 10:07:06 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.3.1.tar", last modified: Tue May  9 10:38:53 2023, max compression
```

## Comparing `spotON_sdk-0.0.3.0.tar` & `spotON_sdk-0.0.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.3.0/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.3.0/LICENSE
--rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.3.0/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-09 10:06:30.699812 spotON_sdk-0.0.3.0/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.3.0/spotON_sdk/constants/bidding_zones.py
--rw-r--r--   0        0        0     4567 2023-05-09 10:06:06.205353 spotON_sdk-0.0.3.0/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     2065 2023-05-08 20:49:26.007366 spotON_sdk-0.0.3.0/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.3.0/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0     3480 2023-05-09 10:03:04.606749 spotON_sdk-0.0.3.0/spotON_sdk/logic/Entsoe_query.py
--rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.3.0/spotON_sdk/logic/dataframe_modifier.py
--rw-r--r--   0        0        0      201 2023-05-08 20:50:42.181852 spotON_sdk-0.0.3.0/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.3.1/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.3.1/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-09 10:38:44.665543 spotON_sdk-0.0.3.1/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.3.1/spotON_sdk/constants/bidding_zones.py
+-rw-r--r--   0        0        0     4567 2023-05-09 10:06:06.205353 spotON_sdk-0.0.3.1/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     2065 2023-05-08 20:49:26.007366 spotON_sdk-0.0.3.1/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.3.1/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0     3480 2023-05-09 10:03:04.606749 spotON_sdk-0.0.3.1/spotON_sdk/logic/Entsoe_query.py
+-rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.3.1/spotON_sdk/logic/dataframe_modifier.py
+-rw-r--r--   0        0        0      201 2023-05-08 20:50:42.181852 spotON_sdk-0.0.3.1/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.3.1/PKG-INFO
```

### Comparing `spotON_sdk-0.0.3.0/.gitignore` & `spotON_sdk-0.0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.0/LICENSE` & `spotON_sdk-0.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.0/spotON_sdk/constants/bidding_zones.py` & `spotON_sdk-0.0.3.1/spotON_sdk/constants/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.0/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.3.1/spotON_sdk/constants/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.0/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.3.1/spotON_sdk/constants/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.0/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.3.1/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.0/spotON_sdk/logic/Entsoe_query.py` & `spotON_sdk-0.0.3.1/spotON_sdk/logic/Entsoe_query.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.0/spotON_sdk/logic/dataframe_modifier.py` & `spotON_sdk-0.0.3.1/spotON_sdk/logic/dataframe_modifier.py`

 * *Files identical despite different names*

