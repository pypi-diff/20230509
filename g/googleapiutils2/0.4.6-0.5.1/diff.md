# Comparing `tmp/googleapiutils2-0.4.6.tar.gz` & `tmp/googleapiutils2-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.4.6.tar", max compression
+gzip compressed data, was "googleapiutils2-0.5.1.tar", max compression
```

## Comparing `googleapiutils2-0.4.6.tar` & `googleapiutils2-0.5.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1071 2022-12-30 01:32:12.340806 googleapiutils2-0.4.6/LICENSE
--rw-r--r--   0        0        0       96 2023-01-30 06:00:44.616601 googleapiutils2-0.4.6/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-01-15 05:10:18.196566 googleapiutils2-0.4.6/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    14624 2023-05-09 18:49:08.407236 googleapiutils2-0.4.6/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      297 2022-12-30 01:32:12.341593 googleapiutils2-0.4.6/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.4.6/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1049 2022-12-30 01:32:12.342019 googleapiutils2-0.4.6/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1178 2022-12-30 01:32:12.342148 googleapiutils2-0.4.6/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      118 2023-01-30 06:00:44.617619 googleapiutils2-0.4.6/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     6494 2023-05-09 18:46:09.012912 googleapiutils2-0.4.6/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    11511 2023-05-09 18:46:09.013129 googleapiutils2-0.4.6/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     4699 2023-05-09 18:46:09.013605 googleapiutils2-0.4.6/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     6822 2023-05-09 17:40:05.660193 googleapiutils2-0.4.6/googleapiutils2/utils.py
--rw-r--r--   0        0        0      685 2023-05-09 18:46:09.014272 googleapiutils2-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 googleapiutils2-0.4.6/setup.py
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 googleapiutils2-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-12-30 01:32:12.340806 googleapiutils2-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2215 2023-05-09 19:39:40.689070 googleapiutils2-0.5.1/README.md
+-rw-r--r--   0        0        0       96 2023-01-30 06:00:44.616601 googleapiutils2-0.5.1/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-01-15 05:10:18.196566 googleapiutils2-0.5.1/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    14624 2023-05-09 18:49:08.407236 googleapiutils2-0.5.1/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      297 2022-12-30 01:32:12.341593 googleapiutils2-0.5.1/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.5.1/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1049 2022-12-30 01:32:12.342019 googleapiutils2-0.5.1/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1178 2022-12-30 01:32:12.342148 googleapiutils2-0.5.1/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      118 2023-01-30 06:00:44.617619 googleapiutils2-0.5.1/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     6494 2023-05-09 18:46:09.012912 googleapiutils2-0.5.1/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    11511 2023-05-09 18:46:09.013129 googleapiutils2-0.5.1/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     4699 2023-05-09 18:46:09.013605 googleapiutils2-0.5.1/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     6822 2023-05-09 17:40:05.660193 googleapiutils2-0.5.1/googleapiutils2/utils.py
+-rw-r--r--   0        0        0      738 2023-05-09 19:57:52.205231 googleapiutils2-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3240 1970-01-01 00:00:00.000000 googleapiutils2-0.5.1/setup.py
+-rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 googleapiutils2-0.5.1/PKG-INFO
```

### Comparing `googleapiutils2-0.4.6/LICENSE` & `googleapiutils2-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.4.6/googleapiutils2/drive/drive.py` & `googleapiutils2-0.5.1/googleapiutils2/drive/drive.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.4.6/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.5.1/googleapiutils2/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.4.6/googleapiutils2/geocode/misc.py` & `googleapiutils2-0.5.1/googleapiutils2/geocode/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.4.6/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.5.1/googleapiutils2/sheets/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.4.6/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.5.1/googleapiutils2/sheets/sheets.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.4.6/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.5.1/googleapiutils2/sheets/sheets_value_range.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.4.6/googleapiutils2/utils.py` & `googleapiutils2-0.5.1/googleapiutils2/utils.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.4.6/pyproject.toml` & `googleapiutils2-0.5.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.4.6"
-description = "Simple and convenient wrapper for Google's Python API."
+version = "0.5.1"
+description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
+readme = "README.md"
+keywords = ["google", "googleapi", "googleapiutils2"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 google-auth-httplib2 = "^0.1.0"
 google-auth-oauthlib = "^0.5.1"
 google-api-python-client = "^2.47.0"
 requests = "^2.28.1"
```

